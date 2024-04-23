# Comparing `tmp/kodexa_cli-7.0.8649253175.tar.gz` & `tmp/kodexa_cli-7.0.8800850149.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-7.0.8649253175.tar", max compression
+gzip compressed data, was "kodexa_cli-7.0.8800850149.tar", max compression
```

## Comparing `kodexa_cli-7.0.8649253175.tar` & `kodexa_cli-7.0.8800850149.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0    11357 2024-04-11 15:25:00.726642 kodexa_cli-7.0.8649253175/LICENSE
--rw-r--r--   0        0        0     2157 2024-04-11 15:25:00.726642 kodexa_cli-7.0.8649253175/README.md
--rw-r--r--   0        0        0       64 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      402 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/Dockerfile
--rw-r--r--   0        0        0      174 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/health-check.conf
--rw-r--r--   0        0        0        0 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/index.html
--rw-r--r--   0        0        0      349 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/.helmignore
--rw-r--r--   0        0        0      140 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/Chart.yaml
--rw-r--r--   0        0        0     1528 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0     1791 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/deployment.yaml
--rw-r--r--   0        0        0      410 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/service.yaml
--rw-r--r--   0        0        0      330 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/values.yaml
--rw-r--r--   0        0        0    48988 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      722 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      808 2024-04-11 15:25:12.006599 kodexa_cli-7.0.8649253175/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8649253175/setup.py
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8649253175/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 13:00:08.562095 kodexa_cli-7.0.8800850149/LICENSE
+-rw-r--r--   0        0        0     2101 2024-04-23 13:00:08.562095 kodexa_cli-7.0.8800850149/README.md
+-rw-r--r--   0        0        0       64 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      402 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      174 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0        0 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-container/index.html
+-rw-r--r--   0        0        0      349 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1528 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1791 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      410 2024-04-23 13:00:08.570095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/templates/service.yaml
+-rw-r--r--   0        0        0      330 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    49226 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      722 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2024-04-23 13:00:08.574095 kodexa_cli-7.0.8800850149/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      808 2024-04-23 13:00:26.638075 kodexa_cli-7.0.8800850149/pyproject.toml
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8800850149/PKG-INFO
```

### Comparing `kodexa_cli-7.0.8649253175/LICENSE` & `kodexa_cli-7.0.8800850149/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/README.md` & `kodexa_cli-7.0.8800850149/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,15 @@
   and then use that content to drive the processing of the document.
 
 # Command Line Tools
 
 This repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It
 allows you to configure components and manage aspects of your Kodexa Platform installation.
 
-## Documentation & Examples
-
-Documentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)
+You can learn about about Kodexa at https://support.kodexa.ai
 
 ## Set-up
 
 We use poetry to manage our dependencies, so you can install them with:
 
     poetry install
```

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8800850149/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/deployment.yaml` & `kodexa_cli-7.0.8800850149/kodexa_cli/charts/resource-pack/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/cli.py` & `kodexa_cli-7.0.8800850149/kodexa_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 def get_current_kodexa_url():
     try:
         return KodexaPlatform.get_url()
     except:
         return ""
 
- 
+
 def get_current_access_token():
     try:
         return KodexaPlatform.get_access_token()
     except:
         return ""
 
 
@@ -1089,20 +1089,26 @@
 
         if kodexa_url == "":
             print("Using default as https://platform.kodexa.ai")
             kodexa_url = "https://platform.kodexa.ai"
         token = input("Enter your token: ")
         profile_name = input("Enter your profile name (default): ")
     except Exception as error:
-        print("ERROR", error)
+        import better_exceptions
+        import sys
+        print("\n".join(
+            better_exceptions.format_exception(*sys.exc_info())))
     else:
         try:
             KodexaPlatform.login(kodexa_url, token, profile_name)
         except Exception as error:
-            print("ERROR", error)
+            import better_exceptions
+            import sys
+            print("\n".join(
+                better_exceptions.format_exception(*sys.exc_info())))
 
 
 @cli.command()
 @click.argument("files", nargs=-1)
 @pass_info
 def mkdocs(_: Info, files: list[str]):
     """
@@ -1419,7 +1425,8 @@
                 os.path.join(output, "health-check.conf"),
             )
             print(
                 "\nIn order to make the resource pack available you will need to run the following commands:\n"
             )
             print(f"docker build -t {repository}/{package_name}-container:{version} .")
             print(f"docker push {repository}/{package_name}-container:{version}")
+
```

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/documentation.py` & `kodexa_cli-7.0.8800850149/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/header.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/model.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/options.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-7.0.8800850149/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8649253175/pyproject.toml` & `kodexa_cli-7.0.8800850149/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "7.0.08649253175"
+version = "7.0.08800850149"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli.cli:safe_entry_point'
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 kodexa = "^7.0.0"
 click = "^8.1.7"
 PyYAML = "^6.0"
 rich = "^13.7.0"
 wrapt = "^1.15.0"
 jinja2 = "^3.1.2"
```

### Comparing `kodexa_cli-7.0.8649253175/PKG-INFO` & `kodexa_cli-7.0.8800850149/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 7.0.8649253175
+Version: 7.0.8800850149
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: kodexa (>=7.0.0,<8.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Description-Content-Type: text/markdown
@@ -43,17 +43,15 @@
   and then use that content to drive the processing of the document.
 
 # Command Line Tools
 
 This repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It
 allows you to configure components and manage aspects of your Kodexa Platform installation.
 
-## Documentation & Examples
-
-Documentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)
+You can learn about about Kodexa at https://support.kodexa.ai
 
 ## Set-up
 
 We use poetry to manage our dependencies, so you can install them with:
 
     poetry install
```

