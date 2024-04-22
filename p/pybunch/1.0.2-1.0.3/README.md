# Comparing `tmp/pybunch-1.0.2.tar.gz` & `tmp/pybunch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.2.tar", last modified: Mon Apr 22 16:04:35 2024, max compression
+gzip compressed data, was "pybunch-1.0.3.tar", last modified: Mon Apr 22 22:19:46 2024, max compression
```

## Comparing `pybunch-1.0.2.tar` & `pybunch-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-22 16:04:29.000000 pybunch-1.0.2/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 16:04:29.000000 pybunch-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 16:04:29.000000 pybunch-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 16:04:35.131050 pybunch-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 16:04:29.000000 pybunch-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.127050 pybunch-1.0.2/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:29.000000 pybunch-1.0.2/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 16:04:29.000000 pybunch-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:04:35.131050 pybunch-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-22 16:04:29.000000 pybunch-1.0.2/src/pybunch/packed_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:04:35.131050 pybunch-1.0.2/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 16:04:35.000000 pybunch-1.0.2/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-22 22:19:42.000000 pybunch-1.0.3/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 22:19:42.000000 pybunch-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 22:19:42.000000 pybunch-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 22:19:46.500621 pybunch-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 22:19:42.000000 pybunch-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:42.000000 pybunch-1.0.3/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-22 22:19:42.000000 pybunch-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:19:46.500621 pybunch-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.496621 pybunch-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-22 22:19:42.000000 pybunch-1.0.3/src/pybunch/packed_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:46.500621 pybunch-1.0.3/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 22:19:46.000000 pybunch-1.0.3/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.2/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.3/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.2/LICENSE` & `pybunch-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.2/PKG-INFO` & `pybunch-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.2/pyproject.toml` & `pybunch-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.2/src/pybunch/__main__.py` & `pybunch-1.0.3/src/pybunch/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 import importlib.resources
 import argparse
 from functools import cached_property
 from pathlib import Path
-from dataclasses import dataclass
 from typing import Dict
 
 from . import packed_base
-from .packed_base import DynamicLocalImporter
+from .packed_base import DynamicLocalImporter, ModulePath, ModuleDescription
 
 
 module = str
 
 
-@dataclass(frozen=True)
 class Project:
-    package_mapping: Dict[Path, Path]
-    sources_package: str = None
+    def __init__(self, package_mapping: Dict[ModulePath, Path], package: str):
+        if package is not None:
+            package_mapping = {ModulePath(package) / relative_path: absolute_path
+                               for relative_path, absolute_path in package_mapping.items()}
+        self._package_mapping = package_mapping
+        self._package = package
 
     @property
     def dynamic_local_importer(self):
-        return DynamicLocalImporter(
-            {'.'.join(relative_path.parts): absolute_path.read_text()
-             for relative_path, absolute_path in self.package_mapping.items()},
-            sources_package=self.sources_package
-        )
+        module_descriptions = {}
+        for relative_path, absolute_path in self._package_mapping.items():
+            name = '.'.join(relative_path.parts)
+            module_descriptions[name] = ModuleDescription(name, code=absolute_path.read_text())
+
+        return DynamicLocalImporter(module_descriptions)
 
     @cached_property
     def packed_code_base(self):
         packed_base_file = importlib.resources.files(packed_base) / 'packed_base.py'
         with packed_base_file.open("rt") as f:
             return f.read()
 
     def pack(self, entrypoint: str, statically_optimize: bool = False) -> str:
-        entrypoint_path = Path(*entrypoint.split('.'))
-        if entrypoint_path not in self.package_mapping:
+        entrypoint_path = ModulePath.from_name(entrypoint)
+        if self._package is not None and entrypoint_path.parts[0] != self._package:
+            entrypoint_path = ModulePath(self._package) / entrypoint_path
+        if entrypoint_path not in self._package_mapping:
             raise ValueError("Nonexistent entrypoint")
+        entrypoint = str(entrypoint_path)
 
-        included_packages = set(self.package_mapping.keys())
+        included_packages = set(self._package_mapping.keys())
         if statically_optimize:
             dli = self.dynamic_local_importer
             dli.import_module(entrypoint)
 
-            loaded_modules = dli.modules
-            included_packages = {relative_path for relative_path in self.package_mapping
+            loaded_modules = {ModulePath.from_name(name) for name in dli.loaded_modules}
+            included_packages = {relative_path for relative_path in self._package_mapping
                                  if (relative_path in loaded_modules) or
                                  (relative_path.name == '__init__' and relative_path.parent in loaded_modules)}
 
-        code_mapping = ',\n'.join(f'''\t'{'.'.join(pth.parts)}': """
-{self.package_mapping[pth].read_text()}
-"""''' for pth in included_packages)
+        package_entries = []
+        for pth in included_packages:
+            name = '.'.join(pth.parts)
+            code = f'''\t'{name}': ModuleDescription('{name}', code="""
+{self._package_mapping[pth].read_text()}
+""")'''
+            package_entries.append(code)
 
         packed_code = self.packed_code_base + f"""\n
 dli = DynamicLocalImporter({{
-{code_mapping}
-}}, sources_package={repr(sources_package)})
+{',\n'.join(package_entries)}
+}})
 dli.execute_module('{entrypoint}')
 """
 
         return packed_code
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog='pybunch',
                                      description='Pack a python project into a single executable file')
     parser.add_argument('-r', '--root', type=Path, required=True, help='Project root')
     parser.add_argument('-e', '--entrypoint', required=True, type=module,
                         help='Entry point of python project, relative to the project root')
-    parser.add_argument('-sp', '--sources-package', required=False, default=None, type=module,
+    parser.add_argument('-p', '--package', required=False, default=None, type=module,
                         help='Package for bundled sources, allowing to import them with absolute imports'
                              ' to that package')
     parser.add_argument('-so', '--statically-optimize', action='store_true',
                         help='Include only files that are statically imported from the entrypoint'
                              ' (executes code to determine)')
     parser.add_argument('-o', '--output', required=True, type=Path,
                         help='Output path for packed file')
 
     args = parser.parse_args()
     root = args.root
     entrypoint = args.entrypoint
-    sources_package = args.sources_package
+    package = args.package
     statically_optimize = args.statically_optimize
     out_file = args.output
 
-    project = Project({pth.relative_to(root).with_suffix(''): pth for pth in root.glob('**/*.py')},
-                      sources_package=sources_package)
+    project = Project({ModulePath(*pth.relative_to(root).with_suffix('').parts): pth for pth in root.glob('**/*.py')},
+                      package)
     out_file.write_text(project.pack(entrypoint, statically_optimize=statically_optimize))
```

### Comparing `pybunch-1.0.2/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.3/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

