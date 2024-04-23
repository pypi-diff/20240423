# Comparing `tmp/pybunch-1.0.5.tar.gz` & `tmp/pybunch-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.5.tar", last modified: Tue Apr 23 08:21:26 2024, max compression
+gzip compressed data, was "pybunch-1.0.6.tar", last modified: Tue Apr 23 08:42:41 2024, max compression
```

## Comparing `pybunch-1.0.5.tar` & `pybunch-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:21:22.000000 pybunch-1.0.5/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:21:22.000000 pybunch-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:21:22.000000 pybunch-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:21:26.556660 pybunch-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:21:22.000000 pybunch-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:22.000000 pybunch-1.0.5/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:21:22.000000 pybunch-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:21:26.556660 pybunch-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.552660 pybunch-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:21:22.000000 pybunch-1.0.5/src/pybunch/packed_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:21:26.556660 pybunch-1.0.5/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:21:26.000000 pybunch-1.0.5/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.052087 pybunch-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:42:36.000000 pybunch-1.0.6/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:42:36.000000 pybunch-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:42:36.000000 pybunch-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:42:41.056087 pybunch-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:42:36.000000 pybunch-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:42:36.000000 pybunch-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:42:41.056087 pybunch-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.052087 pybunch-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/packed_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.5/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.6/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.5/LICENSE` & `pybunch-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.5/PKG-INFO` & `pybunch-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.5/pyproject.toml` & `pybunch-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.5/src/pybunch/__main__.py` & `pybunch-1.0.6/src/pybunch/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib.resources
-import argparse
 from functools import cached_property
 from pathlib import Path
 from typing import Dict
 
 from . import packed_base
 from .packed_base import DynamicLocalImporter, ModulePath, ModuleDescription
 
@@ -45,50 +44,33 @@
             dli.import_module(entrypoint)
 
             loaded_modules = {ModulePath.from_name(name) for name in dli.loaded_modules}
             included_packages = {relative_path for relative_path in self._package_mapping
                                  if (relative_path in loaded_modules) or
                                  (relative_path.name == '__init__' and relative_path.parent in loaded_modules)}
 
+        code_entries = []
         package_entries = []
         for pth in included_packages:
             name = '.'.join(pth.parts)
-            code = f'''\t'{name}': ModuleDescription('{name}', code="""
-{self._package_mapping[pth].read_text()}
-"""[1:])'''
-            package_entries.append(code)
+            escaped_name = 'PYBUNCH_%s' % '_'.join(pth.parts).upper()
+            code = self._package_mapping[pth].read_text()
 
-        packed_code = self.packed_code_base + f"""\n
+            code_entries.append(f'# Code for module <{name}>\n{escaped_name} = """\\n{code}\\n"""[1:]')
+            package_entries.append(f"'{name}': ModuleDescription('{name}', code={escaped_name})")
+
+        header = ''.join(entry + "\n\n\n" for entry in code_entries)
+        footer = f"""\n\n
 dli = DynamicLocalImporter({{
-{',\n'.join(package_entries)}
+{',\n'.join("    %s" % entry for entry in package_entries)}
 }})
 dli.execute_module('{entrypoint}')
 """
 
-        return packed_code
-
+        packed_code_base_lines = self.packed_code_base.splitlines()
+        last_import_line = max(lineno for lineno, line in enumerate(packed_code_base_lines)
+                               if line.startswith("import ") or line.startswith("from "))
+        future_code = '\n'.join(packed_code_base_lines[:last_import_line + 1])
+        packed_code_base = '\n'.join(packed_code_base_lines[last_import_line + 2:])
+        packed_code = future_code + "\n\n\n" + header + packed_code_base + footer
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(prog='pybunch',
-                                     description='Pack a python project into a single executable file')
-    parser.add_argument('-r', '--root', type=Path, required=True, help='Project root')
-    parser.add_argument('-e', '--entrypoint', required=True, type=str,
-                        help='Entry point of python project, relative to the project root')
-    parser.add_argument('-p', '--package', required=False, default=None, type=str,
-                        help='Package for bundled sources, allowing to import them with absolute imports'
-                             ' to that package')
-    parser.add_argument('-so', '--statically-optimize', action='store_true',
-                        help='Include only files that are statically imported from the entrypoint'
-                             ' (executes code to determine)')
-    parser.add_argument('-o', '--output', required=True, type=Path,
-                        help='Output path for packed file')
-
-    args = parser.parse_args()
-    root = args.root
-    entrypoint = args.entrypoint
-    package = args.package
-    statically_optimize = args.statically_optimize
-    out_file = args.output
-
-    project = Project({ModulePath(*pth.relative_to(root).with_suffix('').parts): pth for pth in root.glob('**/*.py')},
-                      package)
-    out_file.write_text(project.pack(entrypoint, statically_optimize=statically_optimize))
+        return packed_code
```

### Comparing `pybunch-1.0.5/src/pybunch/packed_base.py` & `pybunch-1.0.6/src/pybunch/packed_base.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.5/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.6/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

