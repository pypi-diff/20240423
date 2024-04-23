# Comparing `tmp/pybunch-1.0.7.tar.gz` & `tmp/pybunch-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.7.tar", last modified: Tue Apr 23 08:47:32 2024, max compression
+gzip compressed data, was "pybunch-1.0.8.tar", last modified: Tue Apr 23 10:14:37 2024, max compression
```

## Comparing `pybunch-1.0.7.tar` & `pybunch-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:47:27.000000 pybunch-1.0.7/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:47:27.000000 pybunch-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:47:27.000000 pybunch-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:47:32.004324 pybunch-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:47:27.000000 pybunch-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:47:27.000000 pybunch-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:47:32.004324 pybunch-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/packed_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.743774 pybunch-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 10:14:33.000000 pybunch-1.0.8/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 10:14:33.000000 pybunch-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 10:14:33.000000 pybunch-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 10:14:37.747774 pybunch-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 10:14:33.000000 pybunch-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 10:14:33.000000 pybunch-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:14:37.747774 pybunch-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/packed_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.7/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.8/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.7/LICENSE` & `pybunch-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.7/PKG-INFO` & `pybunch-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.7/pyproject.toml` & `pybunch-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.7/src/pybunch/__main__.py` & `pybunch-1.0.8/src/pybunch/__main__.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.7/src/pybunch/packed_base.py` & `pybunch-1.0.8/src/pybunch/packed_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,24 @@
 class ModuleDescription(object):
     def __init__(self, name, code):
         # type: (str, str) -> None
         self.name = name
         self.file_name = 'pybunch <%s>' % name
         self.path = ModulePath(*name.split('.'))
         self.source_code = code
-        self.compiled = compile(code, self.file_name, 'exec')
+        self._compiled = None  # type: 'code'
         self._module = None  # type: _module_type | None
 
+
+    @property
+    def compiled(self):
+        if self._compiled is None:
+            self._compiled = compile(self.source_code, self.file_name, 'exec')
+        return self._compiled
+
     def is_package(self, name):
         # type: (str) -> bool
         return self.path.parts[-1] == '__init__'
 
     def load_module(self, name):
         # type: (str) -> _module_type
         if self._module is None:
```

### Comparing `pybunch-1.0.7/src/pybunch/project.py` & `pybunch-1.0.8/src/pybunch/project.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.7/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.8/src/pybunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

