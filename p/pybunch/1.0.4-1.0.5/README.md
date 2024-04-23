# Comparing `tmp/pybunch-1.0.4.tar.gz` & `tmp/pybunch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.4.tar", last modified: Mon Apr 22 23:21:47 2024, max compression
+gzip compressed data, was "pybunch-1.0.5.tar", last modified: Tue Apr 23 08:21:26 2024, max compression
```

## Comparing `pybunch-1.0.4.tar` & `pybunch-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.654644 pybunch-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-22 23:21:43.000000 pybunch-1.0.4/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 23:21:43.000000 pybunch-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 23:21:43.000000 pybunch-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 23:21:47.658644 pybunch-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 23:21:43.000000 pybunch-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 23:21:43.000000 pybunch-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:21:47.658644 pybunch-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.654644 pybunch-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/packed_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:21:22.000000 pybunch-1.0.5/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:21:22.000000 pybunch-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:21:22.000000 pybunch-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:21:26.556660 pybunch-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:21:22.000000 pybunch-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:21:22.000000 pybunch-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:21:26.556660 pybunch-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/packed_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.4/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.5/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.4/LICENSE` & `pybunch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.4/PKG-INFO` & `pybunch-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.4/pyproject.toml` & `pybunch-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.4/src/pybunch/__main__.py` & `pybunch-1.0.5/src/pybunch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                                  (relative_path.name == '__init__' and relative_path.parent in loaded_modules)}
 
         package_entries = []
         for pth in included_packages:
             name = '.'.join(pth.parts)
             code = f'''\t'{name}': ModuleDescription('{name}', code="""
 {self._package_mapping[pth].read_text()}
-""")'''
+"""[1:])'''
             package_entries.append(code)
 
         packed_code = self.packed_code_base + f"""\n
 dli = DynamicLocalImporter({{
 {',\n'.join(package_entries)}
 }})
 dli.execute_module('{entrypoint}')
```

### Comparing `pybunch-1.0.4/src/pybunch/packed_base.py` & `pybunch-1.0.5/src/pybunch/packed_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import division
 
 import importlib
 import itertools
 import runpy
 import sys
 import os
+import traceback
 from contextlib import contextmanager
 
 _module_type = type(os)
 
 
 class ModulePath(object):
     def __init__(self, *parts):
@@ -71,16 +72,18 @@
         return 'ModulePath%s' % repr(self.parts)
 
 
 class ModuleDescription(object):
     def __init__(self, name, code):
         # type: (str, str) -> None
         self.name = name
+        self.file_name = 'pybunch <%s>' % name
         self.path = ModulePath(*name.split('.'))
-        self.code = code
+        self.source_code = code
+        self.compiled = compile(code, self.file_name, 'exec')
         self._module = None  # type: _module_type | None
 
     def is_package(self, name):
         # type: (str) -> bool
         return self.path.parts[-1] == '__init__'
 
     def load_module(self, name):
@@ -90,24 +93,26 @@
             if self.is_package(None):
                 module = _module_type(parent)
                 module.__path__ = []
             else:
                 module = _module_type(self.name)
 
             module.__package__ = parent
-            module.__file__ = "pybunch <%s>" % self.name
-            module.__loader__ = self
-            exec(self.code, module.__dict__)
+            module.__file__ = self.file_name
+            exec(self.compiled, module.__dict__)
             self._module = module
 
         return sys.modules.setdefault(name, self._module)
 
     def get_code(self, name):
-        # type: (str) -> str
-        return self.code
+        # type: (str) -> 'code'
+        return self.compiled
+
+    def get_source(self, *args, **kwargs):
+        return self.source_code
 
 
 RESOLVED_IMPORT_EXTERNAL = 'External'
 RESOLVED_IMPORT_MISSING_LOCAL = 'Missing Local'
 RESOLVED_IMPORT_LEAF_MODULE = 'Leaf Module'
 RESOLVED_IMPORT_INTERMEDIATE_MODULE = 'Intermediate Module'
 
@@ -160,22 +165,35 @@
     def add_to_meta_path(self):
         # type: () -> 'Generator[None, None, None]'
         old_meta_path = sys.meta_path
         sys.meta_path = [self] + sys.meta_path
         yield
         sys.meta_path = old_meta_path
 
+    @property
+    @contextmanager
+    def with_custom_stacktrace(self):
+        old_except_hook = sys.excepthook
+        print_exception = traceback.print_exception
+
+        def except_hook(ex_type, ex, tb):
+            print_exception(ex_type, ex, tb)
+
+        sys.excepthook = except_hook
+        yield
+        sys.excepthook = old_except_hook
+
     def import_module(self, module):
         # type: (str) -> _module_type
-        with self.add_to_meta_path:
+        with self.add_to_meta_path, self.with_custom_stacktrace:
             importlib.import_module(module)
 
     def execute_module(self, module):
         # type: (str) -> _module_type
-        with self.add_to_meta_path:
+        with self.add_to_meta_path, self.with_custom_stacktrace:
             new_globals = runpy.run_module(module, run_name='__main__')
 
         current_globals = globals()
         keys_to_delete = set(current_globals.keys()).difference(new_globals)
         current_globals.update(new_globals)
         for key in keys_to_delete:
             del current_globals[key]
```

### Comparing `pybunch-1.0.4/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.5/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

