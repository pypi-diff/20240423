# Comparing `tmp/pybunch-1.0.3.tar.gz` & `tmp/pybunch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.3.tar", last modified: Mon Apr 22 22:19:46 2024, max compression
+gzip compressed data, was "pybunch-1.0.4.tar", last modified: Mon Apr 22 23:21:47 2024, max compression
```

## Comparing `pybunch-1.0.3.tar` & `pybunch-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-22 22:19:42.000000 pybunch-1.0.3/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 22:19:42.000000 pybunch-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 22:19:42.000000 pybunch-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 22:19:46.500621 pybunch-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 22:19:42.000000 pybunch-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 22:19:42.000000 pybunch-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:19:46.500621 pybunch-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/packed_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.654644 pybunch-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-22 23:21:43.000000 pybunch-1.0.4/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 23:21:43.000000 pybunch-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 23:21:43.000000 pybunch-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 23:21:47.658644 pybunch-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 23:21:43.000000 pybunch-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:43.000000 pybunch-1.0.4/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 23:21:43.000000 pybunch-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:21:47.658644 pybunch-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.654644 pybunch-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-22 23:21:43.000000 pybunch-1.0.4/src/pybunch/packed_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:21:47.658644 pybunch-1.0.4/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 23:21:47.000000 pybunch-1.0.4/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.3/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.4/.github/workflows/publish-to-pypi.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
 
-on: [push, workflow_dispatch]
+on:
+  push:
+    tags:
+      - '**'
+  workflow_dispatch:
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
@@ -25,15 +29,14 @@
       uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: Publish Python 🐍 distribution 📦 to PyPI
-    if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: pypi
       url: https://pypi.org/p/pybunch  # Replace <project-name> with your PyPI project name
```

### Comparing `pybunch-1.0.3/LICENSE` & `pybunch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.3/PKG-INFO` & `pybunch-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.3/pyproject.toml` & `pybunch-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.3/src/pybunch/__main__.py` & `pybunch-1.0.4/src/pybunch/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,36 +4,33 @@
 from pathlib import Path
 from typing import Dict
 
 from . import packed_base
 from .packed_base import DynamicLocalImporter, ModulePath, ModuleDescription
 
 
-module = str
-
-
 class Project:
     def __init__(self, package_mapping: Dict[ModulePath, Path], package: str):
         if package is not None:
             package_mapping = {ModulePath(package) / relative_path: absolute_path
                                for relative_path, absolute_path in package_mapping.items()}
         self._package_mapping = package_mapping
         self._package = package
 
     @property
-    def dynamic_local_importer(self):
+    def dynamic_local_importer(self) -> DynamicLocalImporter:
         module_descriptions = {}
         for relative_path, absolute_path in self._package_mapping.items():
             name = '.'.join(relative_path.parts)
             module_descriptions[name] = ModuleDescription(name, code=absolute_path.read_text())
 
         return DynamicLocalImporter(module_descriptions)
 
     @cached_property
-    def packed_code_base(self):
+    def packed_code_base(self) -> str:
         packed_base_file = importlib.resources.files(packed_base) / 'packed_base.py'
         with packed_base_file.open("rt") as f:
             return f.read()
 
     def pack(self, entrypoint: str, statically_optimize: bool = False) -> str:
         entrypoint_path = ModulePath.from_name(entrypoint)
         if self._package is not None and entrypoint_path.parts[0] != self._package:
@@ -70,17 +67,17 @@
         return packed_code
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog='pybunch',
                                      description='Pack a python project into a single executable file')
     parser.add_argument('-r', '--root', type=Path, required=True, help='Project root')
-    parser.add_argument('-e', '--entrypoint', required=True, type=module,
+    parser.add_argument('-e', '--entrypoint', required=True, type=str,
                         help='Entry point of python project, relative to the project root')
-    parser.add_argument('-p', '--package', required=False, default=None, type=module,
+    parser.add_argument('-p', '--package', required=False, default=None, type=str,
                         help='Package for bundled sources, allowing to import them with absolute imports'
                              ' to that package')
     parser.add_argument('-so', '--statically-optimize', action='store_true',
                         help='Include only files that are statically imported from the entrypoint'
                              ' (executes code to determine)')
     parser.add_argument('-o', '--output', required=True, type=Path,
                         help='Output path for packed file')
```

### Comparing `pybunch-1.0.3/src/pybunch/packed_base.py` & `pybunch-1.0.4/src/pybunch/packed_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,19 @@
         # type: (str, str) -> None
         self.name = name
         self.path = ModulePath(*name.split('.'))
         self.code = code
         self._module = None  # type: _module_type | None
 
     def is_package(self, name):
+        # type: (str) -> bool
         return self.path.parts[-1] == '__init__'
 
     def load_module(self, name):
+        # type: (str) -> _module_type
         if self._module is None:
             parent = '.'.join(self.path.parts[:-1])
             if self.is_package(None):
                 module = _module_type(parent)
                 module.__path__ = []
             else:
                 module = _module_type(self.name)
@@ -96,33 +98,35 @@
             module.__loader__ = self
             exec(self.code, module.__dict__)
             self._module = module
 
         return sys.modules.setdefault(name, self._module)
 
     def get_code(self, name):
+        # type: (str) -> str
         return self.code
 
 
 RESOLVED_IMPORT_EXTERNAL = 'External'
 RESOLVED_IMPORT_MISSING_LOCAL = 'Missing Local'
 RESOLVED_IMPORT_LEAF_MODULE = 'Leaf Module'
 RESOLVED_IMPORT_INTERMEDIATE_MODULE = 'Intermediate Module'
 
 
-class DynamicLocalImporter:
+class DynamicLocalImporter(object):
     def __init__(self, module_descriptions):
-        # type: (dict[str, ModuleDescription], _module_type) -> None
+        # type: (dict[str, ModuleDescription]) -> None
         self._module_descriptions = {ModulePath.from_name(name): description
                                      for name, description in module_descriptions.items()}
 
-        self._module_specs = {}  # dict[ModulePath, _module_type]
+        self._module_specs = {}  # dict[str, _module_type]
 
     @property
     def loaded_modules(self):
+        # type: () -> set[str]
         return set(self._module_specs.keys())
 
     @staticmethod
     def attempt_resolve_local_import(name, local_modules, module_aliases=None):
         # type: (str, list[ModulePath], dict[ModulePath, ModulePath]) -> tuple[str, ModulePath | None]
         local_modules = set(local_modules)
         if module_aliases is None:
@@ -150,28 +154,35 @@
             return RESOLVED_IMPORT_MISSING_LOCAL, None
         else:
             return RESOLVED_IMPORT_EXTERNAL, None
 
     @property
     @contextmanager
     def add_to_meta_path(self):
+        # type: () -> 'Generator[None, None, None]'
         old_meta_path = sys.meta_path
         sys.meta_path = [self] + sys.meta_path
         yield
         sys.meta_path = old_meta_path
 
     def import_module(self, module):
         # type: (str) -> _module_type
         with self.add_to_meta_path:
             importlib.import_module(module)
 
     def execute_module(self, module):
         # type: (str) -> _module_type
         with self.add_to_meta_path:
-            runpy.run_module(module, run_name='__main__')
+            new_globals = runpy.run_module(module, run_name='__main__')
+
+        current_globals = globals()
+        keys_to_delete = set(current_globals.keys()).difference(new_globals)
+        current_globals.update(new_globals)
+        for key in keys_to_delete:
+            del current_globals[key]
 
     def find_spec(self, name, path, target=None):
         # type: (str, str, object) -> 'ModuleSpec'
         from importlib.util import spec_from_loader
 
         if name not in self._module_specs:
             module_aliases = {}
@@ -186,14 +197,15 @@
                                                             is_package=True)
 
         module_spec = self._module_specs.get(name, None)
         if module_spec is not None:
             return module_spec
 
     def find_module(self, name, path=None):
+        # type: (str, str) -> ModuleDescription
         module_aliases = {}
         resolution_type, module_path = self.attempt_resolve_local_import(name, self._module_descriptions.keys(),
                                                                          module_aliases)
 
         if resolution_type == RESOLVED_IMPORT_LEAF_MODULE:
             return self._module_descriptions[module_path]
         elif resolution_type == RESOLVED_IMPORT_INTERMEDIATE_MODULE:
```

### Comparing `pybunch-1.0.3/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.4/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

