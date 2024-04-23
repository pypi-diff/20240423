# Comparing `tmp/rickled-1.1.1.tar.gz` & `tmp/rickled-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rickled-1.1.1.tar", last modified: Tue Mar 19 23:32:36 2024, max compression
+gzip compressed data, was "dist\rickled-1.1.2.tar", last modified: Tue Apr 23 21:30:35 2024, max compression
```

## Comparing `rickled-1.1.1.tar` & `rickled-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/
--rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4790 2024-03-19 23:32:36.000000 rickled-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4955 2024-03-19 23:27:49.000000 rickled-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled/
--rw-rw-rw-   0        0        0    56302 2024-03-19 21:48:46.000000 rickled-1.1.1/rickled/__init__.py
--rw-rw-rw-   0        0        0       48 2024-03-19 23:32:35.000000 rickled-1.1.1/rickled/__version__.py
--rw-rw-rw-   0        0        0    22915 2024-03-19 23:24:58.000000 rickled-1.1.1/rickled/cli.py
--rw-rw-rw-   0        0        0     2470 2024-03-19 23:24:58.000000 rickled-1.1.1/rickled/net.py
--rw-rw-rw-   0        0        0    14955 2024-03-19 21:48:46.000000 rickled-1.1.1/rickled/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/
--rw-rw-rw-   0        0        0     4790 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-19 23:32:36.000000 rickled-1.1.1/rickled.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-03-19 23:32:36.000000 rickled-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2195 2024-03-19 23:25:24.000000 rickled-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/tests/integration/
--rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-1.1.1/tests/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 23:32:36.000000 rickled-1.1.1/tests/unittest/
--rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-1.1.1/tests/unittest/__init__.py
--rw-rw-rw-   0        0        0     9029 2024-03-19 23:24:58.000000 rickled-1.1.1/tests/unittest/test_advanced.py
--rw-rw-rw-   0        0        0        0 2023-09-14 16:37:08.000000 rickled-1.1.1/tests/unittest/test_cli.py
--rw-rw-rw-   0        0        0        0 2023-07-21 00:44:56.000000 rickled-1.1.1/tests/unittest/test_net.py
--rw-rw-rw-   0        0        0     1717 2024-03-19 23:24:58.000000 rickled-1.1.1/tests/unittest/test_object_rickler.py
--rw-rw-rw-   0        0        0    12493 2024-03-19 23:24:58.000000 rickled-1.1.1/tests/unittest/test_rickle.py
--rw-rw-rw-   0        0        0     6174 2024-03-19 23:24:58.000000 rickled-1.1.1/tests/unittest/test_schema_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/
+-rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4790 2024-04-23 21:30:35.000000 rickled-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5086 2024-04-23 21:25:49.000000 rickled-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled/
+-rw-rw-rw-   0        0        0    56442 2024-04-20 17:00:51.000000 rickled-1.1.2/rickled/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-04-23 21:30:34.000000 rickled-1.1.2/rickled/__version__.py
+-rw-rw-rw-   0        0        0    27437 2024-04-20 16:50:34.000000 rickled-1.1.2/rickled/cli.py
+-rw-rw-rw-   0        0        0     3906 2024-04-20 13:17:12.000000 rickled-1.1.2/rickled/net.py
+-rw-rw-rw-   0        0        0    15674 2024-04-18 21:18:48.000000 rickled-1.1.2/rickled/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/
+-rw-rw-rw-   0        0        0     4790 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-04-23 21:30:35.000000 rickled-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2195 2024-04-09 19:28:11.000000 rickled-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/integration/
+-rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-1.1.2/tests/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/unittest/
+-rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-1.1.2/tests/unittest/__init__.py
+-rw-rw-rw-   0        0        0     9041 2024-04-20 16:57:44.000000 rickled-1.1.2/tests/unittest/test_advanced.py
+-rw-rw-rw-   0        0        0        0 2023-09-14 16:37:08.000000 rickled-1.1.2/tests/unittest/test_cli.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 00:44:56.000000 rickled-1.1.2/tests/unittest/test_net.py
+-rw-rw-rw-   0        0        0     1717 2024-04-09 19:28:11.000000 rickled-1.1.2/tests/unittest/test_object_rickler.py
+-rw-rw-rw-   0        0        0    12510 2024-04-20 16:59:01.000000 rickled-1.1.2/tests/unittest/test_rickle.py
+-rw-rw-rw-   0        0        0     6174 2024-04-09 19:28:11.000000 rickled-1.1.2/tests/unittest/test_schema_tool.py
```

### Comparing `rickled-1.1.1/LICENSE` & `rickled-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rickled-1.1.1/PKG-INFO` & `rickled-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickle
 Download-URL: https://github.com/Zipfian-Science/rickle/archive/v_01.tar.gz
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Keywords: Pickle,Python,YAML,JSON
@@ -124,10 +124,10 @@
 'hell world!'
 ```
 
 ## Release
 
 See the version history in [changelog](https://zipfian.science/docs/rickle/changelog.html).
 
-- Date: 2024-03-20
-- Version: 1.1.1
+- Date: 2024-04-23
+- Version: 1.1.2
```

### Comparing `rickled-1.1.1/README.md` & `rickled-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # rickle - Smart Python tools for working with YAML
 
 ![PyPI - Version](https://img.shields.io/pypi/v/rickled)
 [![Downloads](https://static.pepy.tech/badge/rickled)](https://pepy.tech/project/rickled)
 [![Downloads](https://static.pepy.tech/badge/rickled/month)](https://pepy.tech/project/rickled)
+[![General badge](https://img.shields.io/badge/Coverage-75+-<COLOR>.svg)](https://zipfian.science/docs/rickle/coverage/index.html)
 
 ```
 ██████╗ ██╗ ██████╗██╗  ██╗██╗     ███████╗
 ██╔══██╗██║██╔════╝██║ ██╔╝██║     ██╔════╝
 ██████╔╝██║██║     █████╔╝ ██║     █████╗  
 ██╔══██╗██║██║     ██╔═██╗ ██║     ██╔══╝  
 ██║  ██║██║╚██████╗██║  ██╗███████╗███████╗
```

### Comparing `rickled-1.1.1/rickled/__init__.py` & `rickled-1.1.2/rickled/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             object: Initiliased `cls`.
         """
         if len(args) > 0:
             obj = cls(**args)
         else:
             obj = cls()
 
-        for name, value in rickle.dict().items():
+        for name, value in rickle.dict(True).items():
             if isinstance(value, dict) and 'type' in value.keys():
                 if value['type'] == 'function':
                     _name = value.get('name', name)
                     _load = value['load']
                     _args = value.get('args', None)
                     _import = value.get('import', None)
                     f = rickle.add_function(name=_name, load=_load, args=_args, imports=_import,
@@ -689,66 +689,66 @@
             try:
                 self._recursive_search(self.dict(), key)
                 return True
             except StopIteration:
                 return False
         return False
 
-    def to_yaml_file(self, file_path : str, serialised : bool = True):
+    def to_yaml_file(self, file_path : str, serialised : bool = False):
         """
         Does a self dump to a YAML file.
 
         Args:
             file_path (str): File path.
-            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = True).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
         """
         self_as_dict = self.dict(serialised=serialised)
         with open(file_path, 'w', encoding='utf-8') as fs:
             yaml.safe_dump(self_as_dict, fs)
 
-    def to_yaml_string(self, serialised : bool = True):
+    def to_yaml_string(self, serialised : bool = False):
         """
         Dumps self to YAML string.
 
         Args:
-            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = True).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
 
         Returns:
             str: YAML representation.
         """
         self_as_dict = self.dict(serialised=serialised)
         return yaml.safe_dump(self_as_dict, None)
 
-    def to_json_file(self, file_path: str, serialised : bool = True):
+    def to_json_file(self, file_path: str, serialised : bool = False):
         """
         Does a self dump to a JSON file.
 
         Args:
             file_path (str): File path.
-            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = True).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
         """
         self_as_dict = self.dict(serialised=serialised)
         with open(file_path, 'w', encoding='utf-8') as fs:
             json.dump(self_as_dict, fs)
 
-    def to_json_string(self, serialised : bool = True):
+    def to_json_string(self, serialised : bool = False):
         """
         Dumps self to YAML string.
 
         Args:
-            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = True).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
 
         Returns:
             str: JSON representation.
         """
@@ -950,21 +950,24 @@
         """
         d = dict()
         for key, value in self.__dict__.items():
             if self.__eval_name(key):
                 continue
             if serialised and key in self.__meta_info.keys():
                 d[key] = self.__meta_info[key]
+            # Revisit this at some later point
             elif key in self.__meta_info.keys() and \
-                    self.__meta_info[key]['type'] in ['function', 'lambda', 'class_definition']:
-                d[key] = self.__meta_info[key]
+                    self.__meta_info[key]['type'] in ['function', 'lambda', 'class_definition', 'module_import', 'base64']:
+                # d[key] = self.__meta_info[key]
+                continue
             elif key in self.__meta_info.keys() and \
                     self.__meta_info[key]['type'] in ['from_file', 'html_page', 'api_json'] and \
                     self.__meta_info[key]['hot_load']:
-                d[key] = self.__meta_info[key]
+                # d[key] = self.__meta_info[key]
+                continue
             elif isinstance(value, BaseRickle):
                 d[key] = value.dict(serialised=serialised)
             elif isinstance(value, list):
                 new_list = list()
                 for element in value:
                     if isinstance(element, BaseRickle):
                         new_list.append(element.dict(serialised=serialised))
```

### Comparing `rickled-1.1.1/rickled/net.py` & `rickled-1.1.2/rickled/net.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sys
 import traceback
 import warnings
 import json
 
+import yaml
+
 from rickled import Rickle
 
 try:
     from twisted.web import server, resource
     from twisted.internet import reactor, endpoints, ssl
     from twisted.python import log
 except ModuleNotFoundError as exc:
@@ -22,56 +24,79 @@
     warnings.warn('Required Python package "pyopenssl" not found.', ImportWarning)
 
 
 class HttpResource(resource.Resource):
     isLeaf = True
     numberRequests = 0
 
-    def __init__(self, rickle):
+    def __init__(self, rickle, serialised: bool = False, output_type: str = 'json'):
         self.rickle = rickle
+        self.serialised = serialised
+        self.output_type = output_type.strip().lower()
         super().__init__()
 
     def render_GET(self, request):
 
         uri = request.uri.decode("utf-8")
 
-        content = self.rickle(uri)
+        try:
+            content = self.rickle(uri)
+        except NameError as exc:
+            request.setResponseCode(404)
+            request.setHeader(b"content-type", b"text/html")
+            response = f"<html><h1>Not Found</h1> {str(exc)}</html>"
+            return response.encode("utf-8")
 
+        request.setResponseCode(200)
         try:
             if isinstance(content, Rickle):
-                request.setHeader(b"content-type", b"application/json")
-                response = content.dict(True)
-                response = json.dumps(response)
+                response = content.dict(self.serialised)
+                if self.output_type == 'json':
+                    request.setHeader(b"content-type", b"application/json")
+                    response = json.dumps(response)
+                else:
+                    request.setHeader(b"content-type", b"application/yaml")
+                    response = yaml.safe_dump(response)
             elif isinstance(content, dict) or isinstance(content, list):
-                request.setHeader(b"content-type", b"application/json")
-                response = json.dumps(content)
+                if self.output_type == 'json':
+                    request.setHeader(b"content-type", b"application/json")
+                    response = json.dumps(content)
+                else:
+                    request.setHeader(b"content-type", b"application/yaml")
+                    response = yaml.safe_dump(content)
+            elif isinstance(content, bytes):
+                request.setHeader(b"content-type", b"application/x-binary")
+                return content
             elif isinstance(content, str):
                 request.setHeader(b"content-type", b"text/html")
                 response = content
+            elif isinstance(content, int) or isinstance(content, float) or isinstance(content, bool):
+                request.setHeader(b"content-type", b"text/html")
+                response = str(content)
             else:
                 response = content
         except:
-            status_code = 500
-            request.setResponseCode(status_code)
+            request.setResponseCode(500)
             request.setHeader(b"content-type", b"text/html")
             response = traceback.format_exc()
 
 
         return response.encode("utf-8")
 
-def serve_rickle_http(rickle, port: int = 8080, interface: str = ''):
+def serve_rickle_http(rickle, port: int = 8080, interface: str = '', serialised : bool = False, output_type: str = 'json'):
     log.startLogging(sys.stdout)
-    site = server.Site(HttpResource(rickle))
+    site = server.Site(HttpResource(rickle, serialised=serialised, output_type=output_type))
     reactor.listenTCP(port, site, interface=interface)
     reactor.run()
 
-def serve_rickle_https(rickle, path_to_private_key: str, path_to_certificate: str, port: int = 8080, interface: str = ''):
+def serve_rickle_https(rickle, path_to_private_key: str, path_to_certificate: str, port: int = 8080,
+                       interface: str = '', serialised : bool = False, output_type: str = 'json'):
     log.startLogging(sys.stdout)
     ssl_context = ssl.DefaultOpenSSLContextFactory(
         path_to_private_key,
         path_to_certificate,
     )
 
-    site = server.Site(HttpResource(rickle))
+    site = server.Site(HttpResource(rickle, serialised=serialised, output_type=output_type))
 
     reactor.listenSSL(port, site, ssl_context, interface=interface)
     reactor.run()
```

### Comparing `rickled-1.1.1/rickled/tools.py` & `rickled-1.1.2/rickled/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,60 +27,74 @@
         silent (bool): Suppress verbose output (default = None).
     """
 
     def __init__(self,
                  input_files: List[str] = None,
                  input_directories: List[str] = None,
                  schema: Union[str, dict] = None,
+                 output_files: List[str] = None,
                  output_dir: str = None,
                  silent: bool = False,
+                 default_output_type: str = 'yaml'
                  ):
         self.input_files = input_files
         self.input_directories = input_directories
 
         if isinstance(schema, str):
             self.schema = Converter.infer_read_file_type(schema)
         else:
             self.schema = schema
 
+        self.output_files = output_files
+
         self.output_dir = output_dir
 
         self.silent = silent
 
+        self.default_output_type = default_output_type
+
     def do_generation(self):
         """
         Generates schema files for the given input files.
         """
         if self.input_files is None and self.input_directories is None:
             raise ValueError("Either input_files or input_directories must be defined!")
 
         if self.input_files is None and not self.input_directories is None:
             self.input_files = list()
             for d in self.input_directories:
                 dir_path = Path(d)
                 self.input_files.extend(list(dir_path.glob("*.yaml")))
                 self.input_files.extend(list(dir_path.glob("*.json")))
 
-
-        self.output_files = list()
-        for input_file in self.input_files:
-            self.output_files.append(f"{os.path.splitext(input_file)[0]}.schema.yaml")
+        if self.output_files is None:
+            self.output_files = list()
+            out_dir = f"{self.output_dir}/" if self.output_dir else './'
+            for input_file in self.input_files:
+                self.output_files.append(f"{out_dir}{os.path.splitext(input_file)[0]}.schema.{self.default_output_type.lower()}")
 
 
         zipped = zip(self.input_files, self.output_files)
 
         for pair in zipped:
             try:
                 input_data = Converter.infer_read_file_type(pair[0])
                 output_file = Path(pair[1])
 
+                suffix = output_file.suffix.lower() if output_file.suffix else f".{self.default_output_type}"
+
                 schema = Schema.generate_schema_from_obj(input_data)
 
-                with output_file.open("w") as fout:
-                    yaml.safe_dump(schema, fout)
+                if suffix == '.yaml':
+                    with output_file.open("w") as fout:
+                        yaml.safe_dump(schema, fout)
+
+                if suffix == '.json':
+                    with output_file.open("w") as fout:
+                        json.dump(schema, fout)
 
                 if not self.silent:
                     print(f"{cli_bcolors.OKBLUE}{pair[0]}{cli_bcolors.ENDC} -> {cli_bcolors.OKBLUE}{pair[1]}{cli_bcolors.ENDC}")
                 continue
             except Exception as exc:
                 if not self.silent:
                     print(f"{cli_bcolors.FAIL}{str(exc)}{cli_bcolors.ENDC}")
@@ -154,22 +168,22 @@
             return float
         if isinstance(value, bool):
             return bool
 
     @staticmethod
     def _data_types_to_schema(value: Union[list, dict, str, int, float, bool, None]):
 
+        if value == bool:
+            return {'type': 'bool'}
         if value == str:
             return {'type': 'str'}
         if value == int:
             return {'type': 'int'}
         if value == float:
             return {'type': 'float'}
-        if value == bool:
-            return {'type': 'bool'}
         if value is None:
             return {'type': 'any'}
 
         if isinstance(value, dict):
             named_schema = {'type': 'dict', 'schema': dict()}
             for k, v in value.items():
                 named_schema['schema'][k] = Schema._data_types_to_schema(v)
@@ -197,15 +211,15 @@
             dict: Schema detected from obj.
 
         """
         rep = Schema._extract_data_types(obj)
         return Schema._data_types_to_schema(rep)
 
     @staticmethod
-    def schema_validation(obj, schema: dict, path: str = 'root', no_print: bool = False) -> bool:
+    def schema_validation(obj, schema: dict, path: str = '', no_print: bool = False) -> bool:
         """
         Validates if obj conforms to schema.
 
         Args:
             obj: The object to check.
             schema (dict): The schema in dict form.
             path (str): The current path of the object tree (default = 'root').
@@ -213,15 +227,15 @@
 
         Returns:
             bool: True if the object conforms.
         """
         new_path = path
         if schema['type'] == 'dict':
             for k, v in schema['schema'].items():
-                new_path = f"{new_path}->{k}"
+                new_path = f"{new_path}/{k}"
                 req = v.get('required', False)
                 nullable = v.get('nullable', False)
                 present = k in obj.keys()
                 if not present:
                     if req:
                         if not no_print:
                             print(f"Required {cli_bcolors.FAIL}'{k}'{cli_bcolors.ENDC} (per schema {v}),\n In {obj},\n Path {cli_bcolors.WARNING}{new_path}{cli_bcolors.ENDC}")
@@ -262,15 +276,15 @@
                     f"Length '{obj}' == {cli_bcolors.FAIL}{obj_length}{cli_bcolors.ENDC},\n Required length {cli_bcolors.OKBLUE}{length}{cli_bcolors.ENDC} (per schema {schema['schema']}),\n In {obj},\n Path {cli_bcolors.WARNING}{new_path}{cli_bcolors.ENDC}")
                 return False
 
             if schema_len > 0:
                 single_type = schema['schema'][0]
 
                 for i in range(obj_length):
-                    new_path = f"{new_path}->[{i}]"
+                    new_path = f"{new_path}/[{i}]"
                     o = obj[i]
                     if single_type['type'] != 'any' and type(o).__name__ != single_type['type']:
                         if not no_print:
                             print(
                             f"Type '{o}' == {cli_bcolors.FAIL}'{type(o).__name__}'{cli_bcolors.ENDC},\n Required type {cli_bcolors.OKBLUE}'{single_type['type']}'{cli_bcolors.ENDC} (per schema {single_type}),\n In {o},\n Path {cli_bcolors.WARNING}{new_path}{cli_bcolors.ENDC}")
                         return False
                     if single_type['type'] in ['dict', 'list']:
@@ -353,22 +367,23 @@
 
         if self.input_files is None and not self.input_directories is None:
             # set output to none as it should not be defined in this scenario
             self.output_files = None
             self.input_files = list()
             for d in self.input_directories:
                 dir_path = Path(d)
+                # TODO extend glo range here if expanding
                 self.input_files.extend(list(dir_path.glob("*.yaml")))
                 self.input_files.extend(list(dir_path.glob("*.json")))
 
 
         if self.output_files is None:
             self.output_files = list()
             for input_file in self.input_files:
-                self.output_files.append(f"{os.path.splitext(input_file)[0]}.{self.default_output_type}")
+                self.output_files.append(f"{os.path.splitext(input_file)[0]}.{self.default_output_type.lower()}")
 
 
         zipped = zip(self.input_files, self.output_files)
 
         for pair in zipped:
             try:
                 input_data = Converter.infer_read_file_type(pair[0])
```

### Comparing `rickled-1.1.1/rickled.egg-info/PKG-INFO` & `rickled-1.1.2/rickled.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickle
 Download-URL: https://github.com/Zipfian-Science/rickle/archive/v_01.tar.gz
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Keywords: Pickle,Python,YAML,JSON
@@ -124,10 +124,10 @@
 'hell world!'
 ```
 
 ## Release
 
 See the version history in [changelog](https://zipfian.science/docs/rickle/changelog.html).
 
-- Date: 2024-03-20
-- Version: 1.1.1
+- Date: 2024-04-23
+- Version: 1.1.2
```

### Comparing `rickled-1.1.1/rickled.egg-info/SOURCES.txt` & `rickled-1.1.2/rickled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rickled-1.1.1/setup.py` & `rickled-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `rickled-1.1.1/tests/unittest/test_advanced.py` & `rickled-1.1.2/tests/unittest/test_advanced.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         r = Rickle(s)
 
         observed = r.random_joke()
 
         self.assertTrue(isinstance(observed, Rickle))
 
-        d = r.dict()
+        d = r.dict(True)
 
         self.assertTrue(isinstance(d['random_joke'], dict))
 
         s = """
 random_joke:
   type: api_json
   url: https://official-joke-api.appspot.com/random_joke
@@ -243,15 +243,15 @@
 
         r = Rickle(s)
 
         observed = r.page()
 
         self.assertTrue(isinstance(observed, str))
 
-        d = r.dict()
+        d = r.dict(True)
 
         self.assertTrue(isinstance(d['page'], dict))
 
         s = """
 page:
     type: html_page
     url: https://zipfian.science
@@ -288,15 +288,15 @@
 
         r = Rickle(s)
 
         observed = r.another_rick()
 
         self.assertTrue(isinstance(observed, str))
 
-        d = r.dict()
+        d = r.dict(True)
 
         self.assertTrue(isinstance(d['another_rick'], dict))
 
         s = """
 another_rick:
    type: from_file
    file_path: './tests/placebos/test_config.json'
```

### Comparing `rickled-1.1.1/tests/unittest/test_object_rickler.py` & `rickled-1.1.2/tests/unittest/test_object_rickler.py`

 * *Files identical despite different names*

### Comparing `rickled-1.1.1/tests/unittest/test_rickle.py` & `rickled-1.1.2/tests/unittest/test_rickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
         self.assertTrue(True)
 
     def test_load_dump_load(self):
         files = ['./tests/placebos/test_config.yaml', './tests/placebos/test_second.yaml']
         test_conf_yaml = Rickle(files, deep=True, load_lambda=True)
 
-        test_conf_yaml.to_yaml_file('./test_out.yaml')
+        test_conf_yaml.to_yaml_file('./test_out.yaml', serialised=True)
 
         test_conf_yaml_reload = Rickle('./test_out.yaml', deep=True, load_lambda=True)
 
         test_conf_yaml_reload.BASICS.outer_math_e()
 
         obj = test_conf_yaml_reload.TesterClass()
         obj.datenow()
```

### Comparing `rickled-1.1.1/tests/unittest/test_schema_tool.py` & `rickled-1.1.2/tests/unittest/test_schema_tool.py`

 * *Files identical despite different names*

