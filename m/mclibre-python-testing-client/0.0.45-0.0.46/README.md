# Comparing `tmp/mclibre_python_testing_client-0.0.45.tar.gz` & `tmp/mclibre_python_testing_client-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mclibre_python_testing_client-0.0.45.tar", last modified: Mon Apr 22 15:33:22 2024, max compression
+gzip compressed data, was "mclibre_python_testing_client-0.0.46.tar", last modified: Tue Apr 23 16:40:05 2024, max compression
```

## Comparing `mclibre_python_testing_client-0.0.45.tar` & `mclibre_python_testing_client-0.0.46.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:22.403658 mclibre_python_testing_client-0.0.45/
--rw-rw-rw-   0        0        0    35184 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.45/LICENSE
--rw-rw-rw-   0        0        0      847 2024-04-22 15:33:22.402658 mclibre_python_testing_client-0.0.45/PKG-INFO
--rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.45/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:22.374531 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client/
--rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client/__init__.py
--rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client/__main__.py
--rw-rw-rw-   0        0        0    17315 2024-04-22 15:30:16.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client/mptc.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:22.400656 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/
--rw-rw-rw-   0        0        0      847 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-22 15:33:22.000000 mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 15:33:22.403658 mclibre_python_testing_client-0.0.45/setup.cfg
--rw-rw-rw-   0        0        0     1074 2024-04-22 15:30:44.000000 mclibre_python_testing_client-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.351105 mclibre_python_testing_client-0.0.46/
+-rw-rw-rw-   0        0        0    35184 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/LICENSE
+-rw-rw-rw-   0        0        0      847 2024-04-23 16:40:05.350105 mclibre_python_testing_client-0.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.46/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.321099 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/__init__.py
+-rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/__main__.py
+-rw-rw-rw-   0        0        0    18397 2024-04-23 16:26:37.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/mptc.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.349104 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 16:40:05.351105 mclibre_python_testing_client-0.0.46/setup.cfg
+-rw-rw-rw-   0        0        0     1074 2024-04-23 09:29:27.000000 mclibre_python_testing_client-0.0.46/setup.py
```

### Comparing `mclibre_python_testing_client-0.0.45/LICENSE` & `mclibre_python_testing_client-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `mclibre_python_testing_client-0.0.45/PKG-INFO` & `mclibre_python_testing_client-0.0.46/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mclibre_python_testing_client
-Version: 0.0.45
+Version: 0.0.46
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mclibre_python_testing_client-0.0.45/mclibre_python_testing_client/mptc.py` & `mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/mptc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import json
 import os
 import random
 import subprocess
 import sys
+
 import colorama
 
 # pytest is a required module
 try:
     exec("import pytest")
 except:
     print("[ERROR] Módulo no instalado: PyTest")
@@ -96,15 +97,15 @@
                 if len(args[0]) == 0:
                     string += ""
                 else:
                     string += str(args[0][0])
                     for j in range(1, len(args[0])):
                         string += " " + str(args[0][j])
                 partial_output = ""
-                if string[-2:] == ": " or string[-2:] == "? :" or string[-2:] == "= ":
+                if string[-2:] == ": " or string[-2:] == "? " or string[-2:] == "= ":
                     output.append(string)
                 else:
                     output.append(string.rstrip())
 
         program.input = mock_input
 
         program.print = lambda *args, **kwargs: generate_output(args, kwargs)
@@ -149,15 +150,41 @@
             json.dump(output, file, ensure_ascii=False)
 
         assert output == values["output"]
 """
         )
 
 
+def check_latest_version():
+    response = requests.get("https://pypi.org/pypi/mclibre-python-testing-client/json")
+    latest_version = response.json()["info"]["version"]
+    if sys.version_info >= (3, 8):
+        from importlib import metadata
+    else:
+        import importlib_metadata as metadata
+    actual_version = metadata.version("mclibre_python_testing_client")
+    if latest_version != actual_version:
+        print(
+            f"{colorama.Fore.YELLOW}[AVISO] Está utilizando la versión {actual_version} de MPTC.{colorama.Style.RESET_ALL}"
+        )
+        print(
+            f"{colorama.Fore.YELLOW}        Actualice a la versión {latest_version} con el comando:{colorama.Style.RESET_ALL}"
+        )
+        print(
+            f"{colorama.Fore.WHITE}        pip install --upgrade mclibre-python-testing-client{colorama.Style.RESET_ALL}"
+        )
+        print(
+            f"{colorama.Fore.YELLOW}        Pulse la tecla [Intro] o [Return] para continuar.{colorama.Style.RESET_ALL}"
+        )
+        input()
+
+
 def main():
+    check_latest_version()
+
     EXECUTION_ERROR = "Execution error"
     SYNTAX_ERROR = "Syntax error"
 
     parser = argparse.ArgumentParser(
         description="Herramienta de prueba para los ejercicios de programación del curso de Python de mclibre.org, disponible en https://www.mclibre.org/consultar/python/"
     )
 
@@ -423,19 +450,19 @@
                         for j in range(
                             min(len(i[0]["output"]), len(i[1])),
                             max(len(i[0]["output"]), len(i[1])),
                         ):
                             if 0 <= j < len(i[0]["output"]):
                                 print(f'  Resultado esperado: "{i[0]["output"][j]}"')
                             else:
-                                print(f"  No se esperaba ningún resultado.")
+                                print("  No se esperaba ningún resultado.")
                             if 0 <= j < len(i[1]):
                                 print(f'  Resultado obtenido: "{i[1][j]}"')
                             else:
-                                print(f"  No se obtuvo ningún resultado.")
+                                print("  No se obtuvo ningún resultado.")
                             print()
                 if len(errorReport) > 1:
                     print(
                         f"{colorama.Fore.RED}{len(errorReport)} tests han fallado. Por favor, corrija el programa y pruebe de nuevo.{colorama.Style.RESET_ALL}"
                     )
                 else:
                     print(
```

### Comparing `mclibre_python_testing_client-0.0.45/mclibre_python_testing_client.egg-info/PKG-INFO` & `mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mclibre_python_testing_client
-Version: 0.0.45
+Version: 0.0.46
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mclibre_python_testing_client-0.0.45/setup.py` & `mclibre_python_testing_client-0.0.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mclibre_python_testing_client",
-    version="0.0.45",
+    version="0.0.46",
     author="Bartolome Sintes",
     author_email="bartolome.sintes@gmail.com",
     description="Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BartolomeSintes/mclibre-python-testing/",
     # packages=setuptools.find_packages(),
```

