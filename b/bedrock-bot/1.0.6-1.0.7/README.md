# Comparing `tmp/bedrock_bot-1.0.6.tar.gz` & `tmp/bedrock_bot-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.6.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.7.tar", max compression
```

## Comparing `bedrock_bot-1.0.6.tar` & `bedrock_bot-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/README.md
--rw-r--r--   0        0        0       91 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2675 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3173 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/README.md
+-rw-r--r--   0        0        0       91 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3173 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/model.py
+-rw-r--r--   0        0        0      175 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.7/PKG-INFO
```

### Comparing `bedrock_bot-1.0.6/LICENSE` & `bedrock_bot-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.6/README.md` & `bedrock_bot-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.6/bedrock_bot/cli.py` & `bedrock_bot-1.0.7/bedrock_bot/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,39 @@
         return [x for x in model_list if x.name.lower() == value.lower()][0]
     except IndexError:
         raise click.BadParameter(
             f"Invalid value: {value}. Allowed values are: {available_models}"
         )
 
 
+def generate_boto_config(region):
+    boto_config = Config()
+    if region:
+        boto_config = Config(region_name=region)
+    elif boto3.setup_default_session() and not boto3.DEFAULT_SESSION.region_name:
+        boto_config = Config(region_name="us-east-1")
+    return boto_config
+
+
+def get_user_input(instance, args):
+    if instance.messages == [] and not sys.stdin.isatty():
+        user_input = sys.stdin.read()
+        print(f"> {user_input}")
+    elif instance.messages == [] and args:
+        user_input = " ".join(args)
+        print(f"> {user_input}")
+    elif not sys.stdin.isatty():
+        print(
+            "Note that you can only do one-shot requests when providing input via stdin"
+        )
+        exit()
+    else:
+        user_input = input("> ")
+
+
 @click.command()
 @click.argument("args", nargs=-1)
 @click.option(
     "-r",
     "--region",
     help="The AWS region to use for requests. If no default region is specified, defaults to us-east-1",
 )
@@ -34,46 +59,28 @@
     "--model",
     type=click.Choice(available_models(), case_sensitive=False),
     default="Claude-3-Haiku",
     help="The model to use for requests",
 )
 def main(model, region, raw_output, args):
     model = model_class_from_input(model)
-
-    boto_config = Config()
-    if region:
-        boto_config = Config(region_name=region)
-    elif boto3.setup_default_session() and not boto3.DEFAULT_SESSION.region_name:
-        boto_config = Config(region_name="us-east-1")
-
+    boto_config = generate_boto_config(region)
     instance = model(boto_config=boto_config)
 
     print(
         f"Hello! I am an AI assistant powered by Amazon Bedrock and using the model {instance.name}. Enter 'quit' or"
         + " 'exit' at any time to exit. How may I help you today?"
     )
     print(
         "(You can clear existing context by starting a query with 'new>' or 'reset>')"
     )
 
     while True:
         print()
-        if instance.messages == [] and not sys.stdin.isatty():
-            user_input = sys.stdin.read()
-            print(f"> {user_input}")
-        elif instance.messages == [] and args:
-            user_input = " ".join(args)
-            print(f"> {user_input}")
-        elif not sys.stdin.isatty():
-            print(
-                "Note that you can only do one-shot requests when providing input via stdin"
-            )
-            exit()
-        else:
-            user_input = input("> ")
+        user_input = get_user_input(instance, args)
 
         if not user_input:
             continue
         if user_input.lower() == "quit" or user_input.lower() == "exit":
             print("\nGoodbye!")
             sys.exit()
         if user_input.lower().startswith("new>") or user_input.lower().startswith(
```

### Comparing `bedrock_bot-1.0.6/bedrock_bot/model.py` & `bedrock_bot-1.0.7/bedrock_bot/model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.6/PKG-INFO` & `bedrock_bot-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.88,<2.0.0)
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: rich (>=13.0.0,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Bedrock Bot
 
 This project is a basic CLI-based chat bot that uses Bedrock to resolve questions. It can take input from stdin, CLI arguments or interactively when no parameters have been passed.
 
 ## Installation
```

