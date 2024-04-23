# Comparing `tmp/bedrock_bot-1.0.5.tar.gz` & `tmp/bedrock_bot-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.5.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.6.tar", max compression
```

## Comparing `bedrock_bot-1.0.5.tar` & `bedrock_bot-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/README.md
--rw-r--r--   0        0        0       91 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2453 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3173 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-22 05:48:16.124873 bedrock_bot-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/README.md
+-rw-r--r--   0        0        0       91 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2675 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3173 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/model.py
+-rw-r--r--   0        0        0      152 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-22 06:10:22.112108 bedrock_bot-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.6/PKG-INFO
```

### Comparing `bedrock_bot-1.0.5/LICENSE` & `bedrock_bot-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.5/README.md` & `bedrock_bot-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.5/bedrock_bot/cli.py` & `bedrock_bot-1.0.6/bedrock_bot/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+import boto3
 import click
 from botocore.config import Config
 
 from . import model_list
 from .util import formatted_print
 
 
@@ -18,29 +19,35 @@
         raise click.BadParameter(
             f"Invalid value: {value}. Allowed values are: {available_models}"
         )
 
 
 @click.command()
 @click.argument("args", nargs=-1)
-@click.option("-r", "--region", help="The AWS region to use for requests")
+@click.option(
+    "-r",
+    "--region",
+    help="The AWS region to use for requests. If no default region is specified, defaults to us-east-1",
+)
 @click.option("--raw-output", help="Don't interpret markdown in the AI response")
 @click.option(
     "-m",
     "--model",
     type=click.Choice(available_models(), case_sensitive=False),
     default="Claude-3-Haiku",
     help="The model to use for requests",
 )
 def main(model, region, raw_output, args):
     model = model_class_from_input(model)
 
     boto_config = Config()
     if region:
         boto_config = Config(region_name=region)
+    elif boto3.setup_default_session() and not boto3.DEFAULT_SESSION.region_name:
+        boto_config = Config(region_name="us-east-1")
 
     instance = model(boto_config=boto_config)
 
     print(
         f"Hello! I am an AI assistant powered by Amazon Bedrock and using the model {instance.name}. Enter 'quit' or"
         + " 'exit' at any time to exit. How may I help you today?"
     )
```

### Comparing `bedrock_bot-1.0.5/bedrock_bot/model.py` & `bedrock_bot-1.0.6/bedrock_bot/model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.5/PKG-INFO` & `bedrock_bot-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

