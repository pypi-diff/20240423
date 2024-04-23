# Comparing `tmp/qase-python-commons-2.0.9.tar.gz` & `tmp/qase_python_commons-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-python-commons-2.0.9.tar", last modified: Mon Mar 11 14:10:20 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.0.tar", last modified: Tue Apr 23 20:00:34 2024, max compression
```

## Comparing `qase-python-commons-2.0.9.tar` & `qase_python_commons-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.021024 qase-python-commons-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.021024 qase-python-commons-2.0.9/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qaseio/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qaseio/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase-python-commons-2.0.9/pyproject.toml` & `qase_python_commons-3.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 [build-system]
-requires = ["setuptools>=69", "wheel"]
+requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "2.0.9"
+version = "3.0.0"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: Apache Software License',
+    'Topic :: Software Development :: Quality Assurance',
+    'Topic :: Software Development :: Testing',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-python-commons"}
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 dependencies = [
     "certifi>=2024.2.2",
-    "qaseio>=4.0.0,<5.0.0",
     "attrs>=23.2.0",
+    "qaseio",
     "more_itertools"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
@@ -31,16 +43,16 @@
     "requests",
     "urllib3",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-minversion = 3.8
-envlist = py{38,39,310,311}
+minversion = 3.7
+envlist = py{37,38,39,310,311}
 
 [testenv]
 deps =
     pytest
     pytest-cov
 passenv =
     HOME
@@ -62,15 +74,15 @@
 [tool.flake8]
 exclude = [".tox", "build", "dist", ".eggs", "docs/conf.py"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
-source = ["src/qaseio/commons"]
+source = ["src/qase/commons"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
     # Don't complain about missing debug-only code:
     "def __repr__",
     "if self\\.debug",
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/config.py` & `qase_python_commons-3.0.0/src/qase/commons/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 import os
 import json
+from .logger import Logger
+
 
 class ConfigManager:
 
-    def __init__(self, config_file = './qase.config.json', env_vars_prefix = 'QASE_'):
-        self.config_file = config_file
-        self.env_vars_prefix = env_vars_prefix
+    def __init__(self, config_file='./qase.config.json', env_vars_prefix='QASE_'):
+        self.logger = Logger()
         self.config = {}
+        self.parseBool = lambda d: d in ("y", "yes", "true", "1", 1, True)
 
-    def load_config(self):
-        # Load from file
         try:
-            if os.path.exists(self.config_file):
-                with open(self.config_file, "r") as file:
+            if os.path.exists(config_file):
+                with open(config_file, "r") as file:
                     self.config = json.load(file)
         except Exception as e:
-            print(f"⚠️  Failed to load config from file {self.config_file}: {e}")
+            self.logger.log("Failed to load config from file", "error")
 
         # Load from env vars
         try:
             for key, value in os.environ.items():
-                if key.startswith(self.env_vars_prefix):
-                    self._set_config(key[len(self.env_vars_prefix):].lower(), value)
+                if key.startswith(env_vars_prefix):
+                    self._set_config(key[len(env_vars_prefix):].lower().replace('_', '.'), value)
         except Exception as e:
-            print(f"⚠️  Failed to load config from env vars: {e}")
+            self.logger.log("Failed to load config from env vars {e}", "error")
+
+    def get(self, key, default=None, value_type=None):
+        # Use _get_config method to get the value. If None, return default.
+        value = self._get_config(key)
+        if value_type and value_type == bool:
+            return self.parseBool(value or default)
+        return value or default
+
+    def validate_config(self):
+        if self.validator:
+            self.validator.validate(self.config)
 
-    def get(self, key):
-        return self._get_config(key)
+    def set(self, key, value):
+        self._set_config(key, value)
 
     def _get_keys(self, config, prefix=""):
         for key, value in config.items():
             if isinstance(value, dict):
-                yield from self._get_keys(value, f"{prefix}{key}_")
+                yield from self._get_keys(value, f"{prefix}{key}.")
             else:
                 yield f"{prefix}{key}"
 
-    def _set_config(self, key, value):
-        keys = key.split("_")
+    def _set_config(self, key, value, delimiter="."):
+        keys = key.split(delimiter)
         config = self.config
         for key in keys[:-1]:
             config = config.setdefault(key, {})
         config[keys[-1]] = value
 
     def _get_config(self, key):
-        keys = key.split("_")
+        keys = key.split(".")
         config = self.config
         for key in keys[:-1]:
             config = config.get(key, {})
-        return config.get(keys[-1], None)
+        return config.get(keys[-1], None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/interceptor.py` & `qase_python_commons-3.0.0/src/qase/commons/profilers/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,111 @@
 import sys
 import uuid
 from functools import wraps
-from qaseio.commons.models.runtime import Runtime
-from qaseio.commons.models.step import Step, StepRequestData
+from ..models.runtime import Runtime
+from ..models.step import Step, StepRequestData, StepType
 
-class Interceptor:
+
+class NetworkProfiler:
     _instance = None
 
     def __init__(self, runtime: Runtime, track_on_fail: bool = True):
         self._original_functions = {}
         self.runtime = runtime
         self.track_on_fail = track_on_fail
         self.step = None
 
     def enable(self):
-        self._apply_wrappers()
-
-    def disable(self):
-        self._remove_wrappers()
-
-    def _apply_wrappers(self):
         if 'requests' in sys.modules:
             import requests
             self._original_functions['requests'] = requests.Session.send
             requests.Session.send = self._requests_send_wrapper(requests.Session.send)
 
         if 'urllib3' in sys.modules:
             import urllib3
             self._original_functions['urllib3'] = urllib3.PoolManager.request
             urllib3.PoolManager.request = self._urllib3_request_wrapper(urllib3.PoolManager.request)
 
-    def _remove_wrappers(self):
+    def disable(self):
         if 'requests' in self._original_functions:
             import requests
             requests.Session.send = self._original_functions['requests']
 
         if 'urllib3' in self._original_functions:
             import urllib3
             urllib3.PoolManager.request = self._original_functions['urllib3']
 
     def _requests_send_wrapper(self, func):
         @wraps(func)
         def wrapper(self, request, *args, **kwargs):
-            InterceptorSingleton.get_instance()._log_pre_request(request)
+            NetworkProfilerSingleton.get_instance()._log_pre_request(request)
             response = func(self, request, *args, **kwargs)
-            InterceptorSingleton.get_instance()._log_post_response(response)
+            NetworkProfilerSingleton.get_instance()._log_post_response(response)
             return response
+
         return wrapper
 
     def _urllib3_request_wrapper(self, func):
         @wraps(func)
         def wrapper(self, method, url, *args, **kwargs):
-            interceptor = InterceptorSingleton.get_instance()
+            interceptor = NetworkProfilerSingleton.get_instance()
             request = lambda: None
             request.method = method
             request.url = url
 
             interceptor._log_pre_request(request)
             response = func(self, method, url, *args, **kwargs)
             if response is not None and interceptor.track_on_fail and response.status >= 400:
                 interceptor._log_post_response(response, url=url)
             return response
+
         return wrapper
 
     @staticmethod
     def _log_pre_request(request):
-        InterceptorSingleton.get_instance().step = Step(
-            id = str(uuid.uuid4()),
-            step_type = 'request',
-            data = StepRequestData(
-                request_method = request.method,
-                request_url = request.url,
-                request_body = getattr(request, "body", ""),
-                request_headers = getattr(request, "headers", {}),
+        NetworkProfilerSingleton.get_instance().step = Step(
+            id=str(uuid.uuid4()),
+            step_type=StepType.REQUEST,
+            data=StepRequestData(
+                request_method=request.method,
+                request_url=request.url,
+                request_body=request.body,
+                request_headers=request.headers,
             ),
         )
 
     @staticmethod
     def _log_post_response(response, url=None, *args, **kwargs):
         status = response.status if hasattr(response, 'status') else response.status_code
-        interceptor = InterceptorSingleton.get_instance()
-        if interceptor.step is None:
-            return
-        interceptor.step.data.add_response(
-            status_code = status,
-            response_body = str(response.data if hasattr(response, 'data') else response.content) if interceptor.track_on_fail and status >= 400 else None,
-            response_headers = response.headers if interceptor.track_on_fail and status >= 400 else None,
+        profiler = NetworkProfilerSingleton.get_instance()
+        profiler.step.data.add_response(
+            status_code=status,
+            response_body=str(response.data if hasattr(response,
+                                                       'data') else response.content) if profiler.track_on_fail and status >= 400 else None,
+            response_headers=response.headers if profiler.track_on_fail and status >= 400 else None,
         )
-        interceptor.runtime.add_step(interceptor.step)
-        interceptor.runtime.finish_step(
-            id = interceptor.step.id,
-            status = 'passed' if status < 400 else 'failed',
+        profiler.runtime.add_step(profiler.step)
+        profiler.runtime.finish_step(
+            id=profiler.step.id,
+            status='passed' if status < 400 else 'failed',
         )
-        interceptor.step = None
-    
-class InterceptorSingleton:
+        profiler.step = None
+
+
+class NetworkProfilerSingleton:
     _instance = None
 
     @staticmethod
     def init(**kwargs):
-        if InterceptorSingleton._instance is None:
-            InterceptorSingleton._instance = Interceptor(**kwargs)
+        if NetworkProfilerSingleton._instance is None:
+            NetworkProfilerSingleton._instance = NetworkProfiler(**kwargs)
 
     @staticmethod
-    def get_instance() -> Interceptor:
+    def get_instance() -> NetworkProfiler:
         """ Static access method"""
-        if InterceptorSingleton._instance is None:
+        if NetworkProfilerSingleton._instance is None:
             raise Exception("Init plugin first")
-        return InterceptorSingleton._instance
+        return NetworkProfilerSingleton._instance
 
     def __init__(self):
         """ Virtually private constructor"""
         raise Exception("Use get_instance()")
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/loader.py` & `qase_python_commons-3.0.0/src/qase/commons/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from qaseio.api_client import ApiClient
 from qaseio.configuration import Configuration
 from qaseio.api.plans_api import PlansApi
 from qaseio.rest import ApiException
+
 import certifi
 
+
 class TestOpsPlanLoader:
-    def __init__(self, api_token, host = 'qase.io'):
+    def __init__(self, api_token, host='qase.io'):
         configuration = Configuration()
         configuration.api_key['TokenAuth'] = api_token
         configuration.host = f'https://api.{host}/v1'
 
         self.client = ApiClient(configuration)
         self.case_list = []
 
         configuration.ssl_ca_cert = certifi.where()
 
     def load(self, code: str, plan_id: int) -> list:
-        api_instance = PlansApi(self.client)
         try:
-            response = api_instance.get_plan(code=code, id=plan_id)
+            response = PlansApi(self.client).get_plan(code=code, id=plan_id)
             if hasattr(response, 'result'):
                 self.case_list = [c.case_id for c in response.result.cases]
                 return self.case_list
             raise ValueError("Unable to find given plan")
         except ApiException as e:
             print("Unable to load test plan data: %s\n" % e)
-        return []
+        return []
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/models/attachment.py` & `qase_python_commons-3.0.0/src/qase/commons/models/attachment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import os
 import uuid
-from typing import Optional
+from typing import Optional, Union
 from io import BytesIO, StringIO
 import json
+import pathlib
+
 
 class Attachment:
-    def __init__(self, 
+    def __init__(self,
                  file_name: str,
                  mime_type: str,
                  content: Optional[str] = None,
-                 file_path: Optional[str] = None):
+                 file_path: Optional[str] = None,
+                 temporary: bool = False):
         self.file_name = file_name
         self.mime_type = mime_type
         if (not content) and (not file_path):
             raise ValueError('Either content or file_path must be provided.')
         self.file_path = file_path
         self.content = content
+        self.temporary = temporary
 
         if (not isinstance(content, str)) and (not isinstance(content, bytes)):
             self.content = json.dumps(self.content, default=lambda o: o.__dict__, sort_keys=False, indent=4)
 
         self.size = self._get_size(content)
         self.id = str(uuid.uuid4())
-        
+
     def _get_size(self, content):
         if self.file_path:
             return os.path.getsize(self.file_path)
         elif content:
             return len(content)
         else:
             return 0
-        
-    def get_id(self):
+
+    def get_id(self) -> str:
         return self.id
-    
+
     def get_for_upload(self) -> BytesIO:
         if self.file_path:
-            with open(self.file_path, "rb") as fc:
-                content = BytesIO(fc.read())
+            return pathlib.Path(os.path.abspath(self.file_path))
         else:
             if isinstance(self.content, str):
-                content = BytesIO(bytes(self.content, 'utf-8'))
+                content = BytesIO(self.content.encode('utf-8'))
             elif isinstance(self.content, bytes):
                 content = BytesIO(self.content)
         content.name = self.file_name
         content.mime = self.mime_type
         return content
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/models/result.py` & `qase_python_commons-3.0.0/src/qase/commons/models/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 from typing import Type, Optional, Union, Dict, List
 from pathlib import PosixPath
 import time
 import uuid
 import json
-from qaseio.commons.models.step import Step
-from qaseio.commons.models.suite import Suite
-from qaseio.commons.models.relation import Relation
-from qaseio.commons.models.attachment import Attachment
-from qaseio.commons.utils import QaseUtils
+from .step import Step
+from .suite import Suite
+from .attachment import Attachment
+from .relation import Relation
+from .. import QaseUtils
+
 
 class Field:
-    def __init__(self, 
+    def __init__(self,
                  name: str,
                  value: Union[str, list]):
         self.name = name
         self.value = value
 
+
 class Execution(object):
-    def __init__(self, 
-                    status: Optional[str] = None,
-                    end_time: int = 0, 
-                    duration: int = 0, 
-                    stacktrace: Optional[str] = None, 
-                    thread: Optional[str] = QaseUtils.get_thread_name()
-                    ):
+    def __init__(self,
+                 status: Optional[str] = None,
+                 end_time: int = 0,
+                 duration: int = 0,
+                 stacktrace: Optional[str] = None,
+                 thread: Optional[str] = QaseUtils.get_thread_name()
+                 ):
         self.start_time = time.time()
         self.status = status
         self.end_time = end_time
         self.duration = duration
         self.stacktrace = stacktrace
         self.thread = thread
 
     def set_status(self, status: Optional[str]):
-        if (status in ['passed', 'failed', 'skipped', 'untested']):
+        if status in ['passed', 'failed', 'skipped', 'untested']:
             self.status = status
         else:
             raise ValueError('Step status must be one of: passed, failed, skipped, untested')
-        
+
     def get_status(self):
         return self.status
 
     def complete(self):
         self.end_time = time.time()
         self.duration = (int)((self.end_time - self.start_time) * 1000)
 
+
 class Request(object):
     def __init__(self,
-            method: str,
-            url: str,
-            status: int,
-            request_headers: Dict[str, str],
-            request_body: str,
-            response_headers: Dict[str, str],
-            response_body: str):
+                 method: str,
+                 url: str,
+                 status: int,
+                 request_headers: Dict[str, str],
+                 request_body: str,
+                 response_headers: Dict[str, str],
+                 response_body: str):
         self.method = method
         self.url = url
         self.status = status
         self.request_headers = request_headers
         self.request_body = request_body
         self.response_headers = response_headers
         self.response_body = response_body
 
+
 class Result(object):
     def __init__(self, title: str, signature: str) -> None:
         self.id: str = str(uuid.uuid4())
         self.title: str = title
         self.signature: str = signature
         self.run_id: Optional[str] = None
         self.testops_id: Optional[int] = None
@@ -78,15 +82,15 @@
         self.muted: bool = False
         self.message: Optional[str] = None
         self.suite: Optional[Type[Suite]] = None
         QaseUtils.get_host_data()
 
     def add_message(self, message: str) -> None:
         self.message = message
-    
+
     def add_field(self, field: Type[Field]) -> None:
         self.fields[field.name] = field.value
 
     def add_steps(self, steps: List[Type[Step]]) -> None:
         self.steps = QaseUtils().build_tree(steps)
 
     def add_attachment(self, attachment: Attachment) -> None:
@@ -102,37 +106,38 @@
         self.relations.append(relation)
 
     def add_suite(self, suite: Type[Suite]) -> None:
         self.suite = suite
 
     def get_status(self) -> Optional[str]:
         return self.execution.status
-    
+
     def get_id(self) -> str:
         return self.id
-    
+
     def get_title(self) -> str:
         return self.title
-    
+
     def get_field(self, name: str) -> Optional[Type[Field]]:
         if name in self.fields:
             return self.fields[name]
         return None
-    
+
     def get_testops_id(self) -> Optional[int]:
         if self.testops_id is None:
             # Hack for old API
             return 0
         return self.testops_id
-    
+
     def get_duration(self) -> int:
         return self.execution.duration
 
     def get_suite_title(self) -> Optional[str]:
         if self.suite:
             return self.suite.title
 
     def set_run_id(self, run_id: str) -> None:
         self.run_id = run_id
 
     def to_json(self) -> str:
-        return json.dumps(self, default=lambda o: o.__str__() if isinstance(o, PosixPath) else o.__dict__, sort_keys=False, indent=4)
+        return json.dumps(self, default=lambda o: o.__str__() if isinstance(o, PosixPath) else o.__dict__,
+                          sort_keys=False, indent=4)
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/models/run.py` & `qase_python_commons-3.0.0/src/qase/commons/models/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 import json
 from typing import Optional, List
 
+
 class RunExecution(object):
     def __init__(self,
                  start_time: float,
                  end_time: float,
                  cumulative_duration: int = 0,
                  ) -> None:
         self.start_time = start_time
         self.end_time = end_time
-        self.duration = int((end_time - start_time)*1000)
+        self.duration = int((end_time - start_time) * 1000)
         self.cumulative_duration = cumulative_duration
 
     def track(self, result: dict):
         self.cumulative_duration += result["execution"]["duration"]
 
+
 class RunStats(object):
     def __init__(self) -> None:
         self.passed = 0
         self.failed = 0
         self.skipped = 0
         self.broken = 0
         self.muted = 0
         self.total = 0
-        
+
     def track(self, result: dict):
         status = result["execution"]["status"]
         if status == "passed":
             self.passed += 1
         elif status == "failed":
             self.failed += 1
         elif status == "skipped":
             self.skipped += 1
         elif status == "broken":
             self.broken += 1
         self.total += 1
         if result.get('muted', False):
             self.muted += 1
-            
+
 
 class Run(object):
-    def __init__(self, 
+    def __init__(self,
                  title: str,
                  start_time: float,
                  end_time: float,
                  results: List[str] = [],
                  threads: List[str] = [],
                  suites: List[str] = [],
                  environment: Optional[str] = None
                  ):
+        self.host_data = None
         self.title = title
         self.execution = RunExecution(start_time=start_time, end_time=end_time)
         self.stats = RunStats()
         self.results = results
         self.threads = threads
         self.suites = suites
         self.environment = environment
-    
+
     def to_json(self) -> str:
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=False, indent=4)
-    
+
     def add_result(self, result: dict):
         compact_result = {
             "id": result["id"],
             "title": result["title"],
             "status": result["execution"]["status"],
             "duration": result["execution"]["duration"],
             "thread": result["execution"]["thread"]
         }
         self.results.append(compact_result)
         self.execution.track(result)
         self.stats.track(result)
-        if (result["execution"]["thread"] not in self.threads):
+        if result["execution"]["thread"] not in self.threads:
             self.threads.append(result["execution"]["thread"])
 
     def add_host_data(self, host_data: dict):
-        self.host_data = host_data
+        self.host_data = host_data
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/models/step.py` & `qase_python_commons-3.0.0/src/qase/commons/models/step.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,114 +1,133 @@
+from enum import Enum
 from typing import Optional, Union, Dict, List, Type
 import time
 import uuid
-from qaseio.commons.models.attachment import Attachment
+from .attachment import Attachment
+
+
+class StepType(Enum):
+    TEXT = 'text'
+    ASSERT = 'assert'
+    GHERKIN = 'gherkin'
+    REQUEST = 'request'
+    DB_QUERY = 'db_query'
+    SLEEP = 'sleep'
+
 
 class StepTextData(object):
     def __init__(self, action: str, expected_result: Optional[str] = None):
         self.action = action
         self.expected_result = expected_result
 
+
 class StepAssertData(object):
     def __init__(self, expected: str, actual: str, message: str):
         self.expected = expected
         self.actual = actual
         self.message = message
 
+
 class StepGherkinData(object):
     def __init__(self, keyword: str, name: str, line: int):
         self.keyword = keyword
         self.name = name
         self.line = line
 
+
 class StepRequestData(object):
     def __init__(self, request_body: str, request_headers: Dict[str, str], request_method: str, request_url: str):
-        if (isinstance(request_body, bytes)):
+        self.response_headers = None
+        self.response_body = None
+        self.status_code = None
+        if isinstance(request_body, bytes):
             request_body = request_body.decode('utf-8')
         self.request_body = request_body
-        if (isinstance(request_headers, bytes)):
+        if isinstance(request_headers, bytes):
             request_headers = request_headers.decode('utf-8')
         self.request_headers = request_headers
         self.request_method = request_method
         self.request_url = request_url
 
-    def add_response(self, status_code: int, response_body: Optional[str] = None, response_headers: Optional[Dict[str, str]] = None):
+    def add_response(self, status_code: int, response_body: Optional[str] = None,
+                     response_headers: Optional[Dict[str, str]] = None):
         self.status_code = status_code
 
-        if (isinstance(response_body, bytes)):
+        if isinstance(response_body, bytes):
             response_body = response_body.decode('utf-8')
         self.response_body = response_body
-        if (isinstance(response_headers, bytes)):
+        if isinstance(response_headers, bytes):
             response_headers = response_headers.decode('utf-8')
         self.response_headers = response_headers
 
+
 class StepDbQueryData(object):
     def __init__(self, query: str, expected_result: str):
         self.query = query
 
+
 class StepSleepData(object):
     def __init__(self, duration: int):
         self.duration = duration
 
+
 class StepExecution(object):
     def __init__(self, status: Optional[str] = 'untested', end_time: int = 0, duration: int = 0):
         self.start_time = time.time()
         self.status = status
         self.end_time = end_time
         self.duration = duration
 
     def set_status(self, status: Optional[str]):
-        if (status in ['passed', 'failed', 'skipped', 'untested']):
+        if status in ['passed', 'failed', 'skipped', 'untested']:
             self.status = status
         else:
             raise ValueError('Step status must be one of: passed, failed, skipped, untested')
-        
+
     def complete(self):
         self.end_time = time.time()
         self.duration = int((self.end_time - self.start_time) * 1000)
 
+
 class Step(object):
-    def __init__(self, 
-        step_type: str, 
-        id: Optional[str], 
-        data: Optional[Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData]] = None, 
-        parent_id: Optional[str] = None
-    ):
-        if (id):
+    def __init__(self,
+                 step_type: StepType,
+                 id: Optional[str],
+                 data: Optional[
+                     Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData, StepSleepData]] = None,
+                 parent_id: Optional[str] = None
+                 ):
+        if id:
             self.id = id
         else:
             self.id = str(uuid.uuid4())
 
-        if (step_type in ['text', 'assert', 'gherkin', 'request']):
-            self.step_type = step_type
-        else:
-            raise ValueError('Step type must be one of: text, assert, gherkin, request')
-        
+        self.step_type = step_type
         self.data = data
         self.parent_id = parent_id
         self.execution = StepExecution()
         self.attachments = []
         self.steps = []
 
     def set_parent_id(self, parent_id: Optional[str]):
         self.parent_id = parent_id
 
     def get_parent_id(self) -> Optional[str]:
         return self.parent_id
 
     def get_steps(self, as_dict: bool = False):
-        if (as_dict):
+        if as_dict:
             return {step.id: step for step in self.steps}
         else:
             return self.steps
 
-    def set_data(self, data: Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData]):
+    def set_data(self, data: Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData, StepSleepData]):
         self.data = data
 
     def add_step(self, step: Type['Step']):
         self.steps.append(step)
 
     def set_steps(self, steps: List[Type['Step']]):
         self.steps = steps
 
     def add_attachment(self, attachment: Attachment):
-        self.attachments.append(attachment)
+        self.attachments.append(attachment)
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/report.py` & `qase_python_commons-3.0.0/src/qase/commons/reporters/report.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,138 @@
 import time
 import os
 import shutil
 import json
 import re
-from qaseio.commons.models.result import Result
-from qaseio.commons.models.run import Run
-from qaseio.commons.models.attachment import Attachment
-from qaseio.commons.utils import QaseUtils
-from typing import Optional
+from ..models import Result, Run, Attachment
+from .. import QaseUtils, ConfigManager, Logger
+
 
 class QaseReport:
     def __init__(
-        self, 
-        report_path: Optional[str] = "build/qase-report",
-        format: Optional[str] = "json",
-        environment: Optional[str] = None
+            self,
+            config: ConfigManager,
+            logger: Logger
     ):
-        self.report_path = report_path
-        if not format:
-            self.format = "json"
-        else:
-            self.format = format
-        
+        self.duration = 0
+        self.results = []
+        self.attachments = []
+        self.config = config
+        self.logger = logger
+
+        self.report_path = self.config.get("report.path", "./build/qase-report")
+        self.format = self.config.get("report.format", "json")
+
         self.start_time = None
         self.end_time = None
         self.run_id = None
-        self.environment = environment
-
-        pass
+        self.environment = self.config.get("environment", None)
 
     def start_run(self):
         self._check_report_path()
         self.start_time = str(time.time())
-        pass
 
-    def complete_run(self, is_main: bool=True, exit_code = None):
-        if (is_main):
-            self.end_time = str(time.time())
-            self._compile_report()
-        else:
-            pass
+    def complete_run(self, exit_code=None):
+        self.end_time = str(time.time())
+        self._compile_report()
+
+    def complete_worker(self):
+        pass
 
     def add_result(self, result: Result):
         result.set_run_id(self.run_id)
         for attachment in result.attachments:
             self._persist_attachment(attachment)
 
         if result.steps:
             self._persist_attachments_in_steps(result.steps)
 
         self._store_result(result)
 
+    def set_run_id(self, run_id):
+        self.run_id = run_id
+
+    def add_attachment(self, attachment: Attachment) -> None:
+        self.attachments.append(attachment)
+
+    def get_results(self):
+        return self.results
+
+    def set_results(self, results):
+        self.results = results
+
     def _persist_attachment(self, attachment: Attachment):
         if attachment.content:
             if isinstance(attachment.content, str):
                 mode = "w"
             if isinstance(attachment.content, bytes):
                 mode = "wb"
             with open(f"{self.report_path}/attachments/{attachment.id}-{attachment.file_name}", mode) as f:
                 f.write(attachment.content)
             # Clear content to save memory and avoid double writing
             attachment.content = None
         elif attachment.file_path:
-            shutil.copy2(os.path.abspath(attachment.file_path), f"{self.report_path}/attachments/{attachment.id}-{attachment.file_name}")
+            shutil.copy2(os.path.abspath(attachment.file_path),
+                         f"{self.report_path}/attachments/{attachment.id}-{attachment.file_name}")
 
     def _persist_attachments_in_steps(self, steps: list):
         for step in steps:
             if step.attachments:
                 for attachment in step.attachments:
                     self._persist_attachment(attachment)
                 if step.steps:
                     self._persist_attachments_in_steps(step.steps)
 
-    def add_attachment(self, attachment: Attachment) -> None:
-        self.attachments.append(attachment)
-
     # Method saves result to a file
     def _store_result(self, result: Result):
-        self._store_object(result, self.report_path+"/results/", result.id)
+        self._store_object(result, self.report_path + "/results/", result.id)
 
     def _check_report_path(self):
-        for path in [self.report_path, self.report_path+"/results/", self.report_path+"/attachments/"]:
+        for path in [self.report_path, self.report_path + "/results/", self.report_path + "/attachments/"]:
             self._recreate_dir(path)
 
-    def _recreate_dir(self, path):
+    @staticmethod
+    def _recreate_dir(path):
         if os.path.exists(path):
             shutil.rmtree(path)
         os.makedirs(path)
 
     def _update_run_duration(self, time):
         self.duration += time
-        
+
     # Method builds final report
     def _compile_report(self):
         run = Run(
-            title = "Test run",
+            title="Test run",
             start_time=float(self.start_time),
             end_time=float(self.end_time),
             environment=self.environment
         )
-        for file in os.listdir(self.report_path+"/results"):
-            with open(self.report_path+"/results/"+file, 'r') as source:
+        for file in os.listdir(self.report_path + "/results"):
+            with open(self.report_path + "/results/" + file, 'r') as source:
                 result = self._read_object(source)
                 run.add_result(result)
 
         run.add_host_data(QaseUtils.get_host_data())
-        
+
         self._store_object(run, self.report_path, "report")
 
     # Saves a model to a file
     def _store_object(self, object, path, filename):
         data = object.to_json()
-        if (self.format == 'jsonp'):
+        if self.format == 'jsonp':
             data = f"qaseJsonp({data});"
         with open(f"{path}/{filename}.{self.format}", 'w', encoding='utf-8') as f:
             f.write(data)
 
     def _read_object(self, source):
         data = source.read()
-        if (self.format == 'json'):
+        if self.format == 'json':
             return json.loads(data)
-        elif (self.format == 'jsonp'):
+        elif self.format == 'jsonp':
             jsonp_pattern = r'\w+\(\s*({[\s\S]*})\s*\);'
             match = re.search(jsonp_pattern, data)
             if match:
                 data = match.group(1)
                 return json.loads(data)
             else:
                 raise ValueError('Invalid JSONP format')
```

### Comparing `qase-python-commons-2.0.9/src/qaseio/commons/testops.py` & `qase_python_commons-3.0.0/src/qase/commons/reporters/testops.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,372 +1,369 @@
-from qaseio.api_client import ApiClient
-from qaseio.configuration import Configuration
+import threading
+import certifi
+
 from qaseio.api.attachments_api import AttachmentsApi
 from qaseio.api.environments_api import EnvironmentsApi
 from qaseio.api.projects_api import ProjectsApi
 from qaseio.api.results_api import ResultsApi
 from qaseio.api.runs_api import RunsApi
-from qaseio.models import RunCreate, ResultcreateBulk, ResultCreate, ResultCreateCase
-from qaseio.rest import ApiException
-from qaseio.commons.models.attachment import Attachment
-from qaseio.commons.models.step import Step
-
-from qaseio.commons.models.result import Result
-
+from qaseio.api_client import ApiClient
+from qaseio.configuration import Configuration
+from qaseio.models import RunCreate, ResultcreateBulk
 from datetime import datetime
-import more_itertools
-import certifi
+from typing import List, Dict, Union
+from .. import ConfigManager, Logger, ReporterException
+from ..models import Attachment, Step, Result
+from ..models.step import StepType
+
+DEFAULT_BATCH_SIZE = 200
 
-class TestOpsRunNotFoundException(Exception):
-    pass
 
 class QaseTestOps:
 
-    def __init__(self,
-            api_token,
-            project_code,
-            run_id=None,
-            plan_id=None,
-            bulk=True,
-            run_title=None,
-            environment=None,
-            host="qase.io",
-            complete_run=False,
-            defect=False,
-            chunk_size=200) -> None:
-
-        configuration = Configuration()
-        configuration.api_key['TokenAuth'] = api_token
-        configuration.host = f'https://api.{host}/v1'
-        configuration.ssl_ca_cert = certifi.where()
+    def __init__(self, config: ConfigManager, logger: Logger) -> None:
+        self.config = config
+        self.logger = logger
 
-        self.client = ApiClient(configuration)
+        self._prepare_client()
 
-        parseBool = lambda d : d in ("y", "yes", "true", "1", 1, True)
+        run_id = self.config.get('testops.run.id')
+        plan_id = self.config.get('testops.plan.id')
 
-        self.project_code = project_code
+        self.project_code = self.config.get('testops.project')
         self.run_id = int(run_id) if run_id else run_id
         self.plan_id = int(plan_id) if plan_id else plan_id
-        self.bulk = parseBool(bulk)
-        self.defect = parseBool(defect)
-        self.complete_after_run = parseBool(complete_run)
+        self.defect = self.config.get('testops_defect', False, bool)
+        self.complete_after_run = self.config.get('testops.run.complete', False, bool)
         self.environment = None
-        self.host = host
-        self.enabled = True
-        self.chunk_size = min(2000, max(10, int(chunk_size)))
+
+        self.batch_size = min(2000, max(1, int(self.config.get('testops.batch.size', DEFAULT_BATCH_SIZE))))
+        self.send_semaphore = threading.Semaphore(
+            self.config.get('testops.batch.threads', 4))  # Semaphore to limit concurrent sends
+        self.lock = threading.Lock()
+
+        environment = self.config.get('environment', None)
         if environment:
             if isinstance(environment, int) or (isinstance(environment, str) and environment.isnumeric()):
                 self.environment = environment
             elif isinstance(environment, str):
                 self.environment = self._get_environment(environment, self.project_code)
 
+        run_title = self.config.get('testops.run.title', None)
         if run_title and run_title != '':
             self.run_title = run_title
         else:
             self.run_title = "Automated Run {}".format(str(datetime.now()))
 
         self.run = None
 
+        # Container for test results
         self.results = []
+
+        # Container for processed results
+        self.processed = []
         self.attachments = {}
 
         """Verify that project exists in TestOps"""
         self._get_project(self.project_code)
 
-    def _get_project(self, project):
-        if self.enabled:
-            api_instance = ProjectsApi(self.client)
-            try:
-                response = api_instance.get_project(code=project)
-                if hasattr(response, 'result'):
-                    return response.result
-                raise ValueError("Unable to find given project code")
-            except ApiException as e:
-                self.enabled = False
-                print("[Qase] ⚠️  Disabling Qase TestOps reporter. Exception when calling ProjectApi->get_project: %s\n" % e)
+    def _prepare_client(self) -> None:
+        try:
+            configuration = Configuration()
+            configuration.api_key['TokenAuth'] = self.config.get('testops.api.token')
+            configuration.ssl_ca_cert = certifi.where()
+            host = self.config.get('testops.api.host', 'qase.io')
+            if self.config.get('testops.api.enterprise', False, bool):
+                configuration.host = f'https://api-{host}/v1'
+                self.web = f'https://{host}'
+            else:
+                configuration.host = f'https://api.{host}/v1'
+                self.web = f'https://app.{host}'
+
+            self.client = ApiClient(configuration)
+        except Exception as e:
+            self.logger.log(f"Error at preparing API client: {e}", "error")
+            raise ReporterException(e)
+
+    # Method loads project from Qase TestOps by code and returns project data
+    def _get_project(self, code: str) -> Dict:
+        try:
+            response = ProjectsApi(self.client).get_project(code=code)
+            if hasattr(response, 'result'):
+                return response.result
+            raise ReporterException("Unable to find given project code")
+        except Exception as e:
+            self.logger.log("Exception when calling ProjectApi->get_project: %s\n" % e, "error")
+            raise ReporterException("Exception when calling ProjectApi")
 
     # Method loads environment by name and returns environment id
-    def _get_environment(self, environment: str, project: str):
-        if self.enabled:
+    # If environment not found or exception raised, returns None
+    def _get_environment(self, environment: str, code: str) -> Union[str, None]:
+        try:
             api_instance = EnvironmentsApi(self.client)
-            response = api_instance.get_environments(code=project)
-            if hasattr(response, 'result'):
+            response = api_instance.get_environments(code=code)
+            if hasattr(response, 'result') and hasattr(response.result, 'entities'):
                 for env in response.result.entities:
                     if env.slug == environment:
                         return env.id
-        return None
+            return None
+        except Exception as e:
+            self.logger.log("Exception when calling EnvironmentsApi->get_environments: %s\n" % e, "error")
+            raise ReporterException(e)
+
+    def _send_results_threaded(self, results):
+        try:
+            api_results = ResultsApi(self.client)
+            results_to_send = [self._prepare_result(result) for result in results]
+            api_results.create_result_bulk(
+                code=self.project_code,
+                id=self.run_id,
+                resultcreate_bulk=ResultcreateBulk(
+                    results=results_to_send
+                )
+            )
+            with self.lock:
+                self.processed.extend(results)
+        except Exception as e:
+            with self.lock:
+                self.logger.log(f"Error at sending results for run {self.run_id}: {e}", "error")
+            raise  # Re-raise the exception to be caught by the thread handler
+        finally:
+            self.send_semaphore.release()  # Release semaphore whether success or exception
+
+    def _send_results(self) -> None:
+        if self.results:
+            # Acquire semaphore before starting the send operation
+            self.send_semaphore.acquire()
+            results_to_send = self.results.copy()
+            self.results = []
+
+            # Start a new thread for sending results
+            send_thread = threading.Thread(target=self._send_results_threaded, args=(results_to_send,))
+            send_thread.start()
+        else:
+            self.logger.log("No results to send", "info")
 
-    def _send_bulk_results(self):
-        if self.enabled and self.results:
-            print()
-            print(f"[Qase] Uploading attachments for Run ID: {self.run_id}...")
+    def _old_send_results(self) -> None:
+        if self.results and len(self.results) > 0:
             results = []
             for result in self.results:
-                attached = []
-                if result.attachments:
-                    for attachment in result.attachments:
-                        attached.extend(self._upload(attachment))
-
-                steps = []
-                for step in result.steps:
-                    prepared = self._prepare_step(step)
-                    steps.append(prepared)
-
-                case_data = {
-                    "title": result.get_title(),
-                    "description": result.get_field('description'),
-                    "precondtions": result.get_field('precondtions'),
-                    "postconditions": result.get_field('postconditions'),
-                }
-
-                for key, param in result.params.items():
-                    # Hack to match old TestOps API
-                    if param == "": result.params[key] = "empty"
-
-                if (result.get_field('severity')):
-                    case_data["severity"] = result.get_field('severity')
-
-                if (result.get_field('priority')):
-                    case_data["priority"] = result.get_field('priority')
-
-                if (result.get_field('layer')):
-                    case_data["layer"] = result.get_field('layer')
-
-                if result.get_suite_title():
-                    case_data["suite_title"] = "\t".join(result.get_suite_title().split("."))
-
-                results.append({
-                    "case_id": result.get_testops_id(),
-                    "status": result.execution.status,
-                    "stacktrace": result.execution.stacktrace,
-                    "time_ms": result.execution.duration,
-                    "comment": result.message,
-                    "attachments": [attach.hash for attach in attached],
-                    "case": case_data,
-                    "steps": steps,
-                    "param": result.params,
-                    "defect": self.defect
-                })
+                results.append(self._prepare_result(result))
 
             api_results = ResultsApi(self.client)
-            print(f"[Qase] Sending results to test run {self.run_id}. Total results: {len(results)}. Results in a chunk: {self.chunk_size}.")
-
-            i = 1
-
-            for chunk in more_itertools.chunked(results, self.chunk_size):
-                try:
-                    print(f"[Qase] Sending chunk #{i}. Chunk size: {len(chunk)}... ")
-                    api_results.create_result_bulk(
-                        code=self.project_code,
-                        id=self.run_id,
-                        resultcreate_bulk=ResultcreateBulk(
-                            results=chunk
-                        )
-                    )
-                    print(f"[Qase] Chunk #{i} was sent successfully.")
-                    i = i+1
-                except Exception as e:
-                    print(f"[Qase] ⚠️  Error at sending results for run {self.run_id} (Chunk #{i}): {e}")
-                    raise e
-
-    def _complete_run(self):
-        if self.enabled:
-            api_runs = RunsApi(self.client)
-            print(f"[Qase] Completing run {self.run_id}")
-            res = api_runs.get_run(self.project_code, self.run_id).result
-            if res.status == 1:
-                print(f"[Qase] Run ID:{self.run_id} already finished")
-                return
             try:
-                api_runs.complete_run(self.project_code, self.run_id)
-                print(f"[Qase] Run ID:{self.run_id} was completed successfully")
+                api_results.create_result_bulk(
+                    code=self.project_code,
+                    id=self.run_id,
+                    resultcreate_bulk=ResultcreateBulk(
+                        results=results
+                    )
+                )
             except Exception as e:
-                print(f"[Qase] ⚠️  Run ID:{self.run_id} was completed with error: {e}")
+                self.logger.log(f"Error at sending results for run {self.run_id}: {e}", "error")
+                raise ReporterException(e)
 
-    def _check_run(self):
-        if self.enabled:
-            if self.plan_id and not self.run_id:
-                self._create_run(plan_id=self.plan_id, environment_id=self.environment)
-            if not self.run_id and not self.plan_id:
-                self._create_run(environment_id=self.environment)
-                pass
-            if not self.run and not self._load_run:
-                raise TestOpsRunNotFoundException(
-                    "Unable to find given test run."
-                )
+            # Moving processed results to another list, so we can use them later for fallback.
+            self.processed += self.results
+            self.results = []
+        else:
+            self.logger.log("No results to send", "info")
+
+    def _prepare_result(self, result: Result) -> Dict:
+        attached = []
+        if result.attachments:
+            for attachment in result.attachments:
+                attached.extend(self._upload(attachment))
+
+        steps = []
+        for step in result.steps:
+            prepared = self._prepare_step(step)
+            steps.append(prepared)
+
+        case_data = {
+            "title": result.get_title(),
+            "description": result.get_field('description'),
+            "preconditions": result.get_field('preconditions'),
+            "postconditions": result.get_field('postconditions'),
+        }
+
+        for key, param in result.params.items():
+            # Hack to match old TestOps API
+            if param == "": result.params[key] = "empty"
+
+        if result.get_field('severity'):
+            case_data["severity"] = result.get_field('severity')
+
+        if result.get_field('priority'):
+            case_data["priority"] = result.get_field('priority')
+
+        if result.get_field('layer'):
+            case_data["layer"] = result.get_field('layer')
+
+        if result.get_suite_title():
+            case_data["suite_title"] = "\t".join(result.get_suite_title().split("."))
+
+        result_model = {
+            "status": result.execution.status,
+            "stacktrace": result.execution.stacktrace,
+            "time_ms": result.execution.duration,
+            "comment": result.message,
+            "attachments": [attach.hash for attach in attached],
+            "steps": steps,
+            "param": result.params,
+            "defect": self.defect
+        }
+
+        test_ops_id = result.get_testops_id()
 
-    def set_run_id(self, run_id):
+        if test_ops_id:
+            result_model["case_id"] = test_ops_id
+            result_model["case"] = None
+            return result_model
+
+        result_model["case_id"] = None
+        result_model["case"] = case_data
+        return result_model
+
+    def _complete_run(self) -> None:
+        api_runs = RunsApi(self.client)
+        self.logger.log(f"Completing run {self.run_id}", "info")
+        res = api_runs.get_run(self.project_code, self.run_id).result
+        if res.status == 1:
+            self.logger.log(f"Run {self.run_id} already completed", "info")
+            return
+        try:
+            api_runs.complete_run(self.project_code, self.run_id)
+            self.logger.log(f"Run {self.run_id} was completed successfully", "info")
+        except Exception as e:
+            self.logger.log(f"Error at completing run {self.run_id}: {e}", "error")
+            raise ReporterException(e)
+
+    def set_run_id(self, run_id) -> None:
         self.run_id = int(run_id)
 
-    def _load_run(self):
-        if self.enabled:
-            api_runs = RunsApi(self.client)
-            if self.run_id:
-                run = api_runs.get_run(
-                    code=self.project_code,
-                    id=self.run_id,
-                ).result
-                if run.id:
-                    return True
-                return False
-
-    def _create_run(self, plan_id=None, environment_id=None, cases=[]):
-        if self.enabled:
-            api_runs = RunsApi(self.client)
-            kwargs = dict(
-                    title=self.run_title,
-                    cases=cases,
-                    environment_id=(int(environment_id) if environment_id else None),
-                    plan_id=(int(plan_id) if plan_id else plan_id),
-                    is_autotest=True
+    def _load_run(self) -> bool:
+        api_runs = RunsApi(self.client)
+        if self.run_id and isinstance(self.run_id, int):
+            run = api_runs.get_run(
+                code=self.project_code,
+                id=self.run_id,
+            ).result
+            if run.id:
+                return True
+        return False
+
+    def _create_run(self, plan_id=None, environment_id=None, cases: List = []) -> None:
+        kwargs = dict(
+            title=self.run_title,
+            cases=cases,
+            environment_id=(int(environment_id) if environment_id else None),
+            plan_id=(int(plan_id) if plan_id else plan_id),
+            is_autotest=True
+        )
+        try:
+            result = RunsApi(self.client).create_run(
+                code=self.project_code,
+                run_create=RunCreate(**{k: v for k, v in kwargs.items() if v is not None})
             )
-            try:
-                result = api_runs.create_run(
-                    code=self.project_code,
-                    run_create=RunCreate(**{k: v for k, v in kwargs.items() if v is not None})
-                )
-                self.run_id = result.result.id
-                self.run = result.result
+            self.run_id = result.result.id
+            self.run = result.result
 
-                print()
-                print(
-                    "[Qase] TestOps: created test run "
-                    "https://app.{}/run/{}/dashboard/{}".format(
-                        self.host, self.project_code, self.run_id
-                    )
-                )
-            except Exception as e:
-                self.enabled = False
-                print()
-                print(f"[Qase] ⚠️  Disabling Qase TestOps reporter. Unable to create test run: {e}")
+            self.logger.log(f"Test run was created: {self.web}/run/{self.project_code}/dashboard/{self.run_id}", "info")
 
-    def _upload(self, attachment: Attachment):
-        api_attachments = AttachmentsApi(self.client)
-
-        return api_attachments.upload_attachment(
+        except Exception as e:
+            self.logger.log(f"Error at creating test run: {e}", "error")
+            raise ReporterException(e)
+
+    def _upload(self, attachment: Attachment) -> Dict:
+        try:
+            return AttachmentsApi(self.client).upload_attachment(
                 self.project_code, file=[attachment.get_for_upload()],
             ).result
-    
+        except Exception as e:
+            self.logger.log(f"Error at uploading attachment: {e}", "error")
+            raise ReporterException(e)
+
     # This method contains a lot of hacks to match old TestOps API.
-    def _prepare_step(self, step: Step):
+    def _prepare_step(self, step: Step) -> Dict:
         prepared_children = []
 
-        prepared_step = {
-            "time": step.execution.duration,
-        }
-        
-        prepared_step["status"] = step.execution.status
-        if step.execution.status == 'untested':
-            prepared_step["status"] = 'passed'
-        
-        if step.step_type == "text":
-            prepared_step['action'] = step.data.action
-            if step.data.expected_result:
-                prepared_step['expected_result'] = step.data.expected_result
-        
-        if step.step_type == "request":
-            prepared_step['action'] = step.data.request_method + " " + step.data.request_url
-            if (step.data.request_body):
-                step.attachments.append(Attachment(file_name='request_body.txt', content=step.data.request_body, mime_type='text/plain'))
-            if (step.data.request_headers):
-                step.attachments.append(Attachment(file_name='request_headers.txt', content=step.data.request_headers, mime_type='text/plain'))
-            if (step.data.response_body):
-                step.attachments.append(Attachment(file_name='response_body.txt', content=step.data.response_body, mime_type='text/plain'))
-            if (step.data.response_headers):
-                step.attachments.append(Attachment(file_name='response_headers.txt', content=step.data.response_headers, mime_type='text/plain'))
-
-        if step.attachments:
-            uploaded_attachments = []
-            for file in step.attachments:
-                uploaded_attachments.extend(self._upload(file))
-            prepared_step['attachments'] = [attach.hash for attach in uploaded_attachments]
-
-        if step.steps:
-            for substep in step.steps:
-                prepared_children.append(self._prepare_step(substep))
-            prepared_step["steps"] = prepared_children
-        return prepared_step
-
-    def _send_result(self, result: Result):
-        if self.enabled:
-            api_results = ResultsApi(self.client)
-            print()
-            print(f"[Qase] Sending a result to test run {self.run_id}...")
+        try:
+            prepared_step = {"time": step.execution.duration, "status": step.execution.status}
 
-            attached = []
-            if result.attachments:
-                for attachment in result.attachments:
-                    attached.extend(self._upload(attachment))
-
-            steps = []
-            for step in result.steps:
-                prepared = self._prepare_step(step)
-                steps.append(prepared)
-
-            case_data = {
-                "title": result.get_title(),
-                "description": result.get_field('description'),
-                "precondtions": result.get_field('precondtions'),
-                "postconditions": result.get_field('postconditions'),
-            }
-
-            for key, param in result.params.items():
-                # Hack to match old TestOps API
-                if param == "":
-                    result.params[key] = "empty"
-
-            if (result.get_field('severity')):
-                case_data["severity"] = result.get_field('severity')
+            if step.execution.status == 'untested':
+                prepared_step["status"] = 'passed'
 
-            if (result.get_field('priority')):
-                case_data["priority"] = result.get_field('priority')
+            if step.step_type == StepType.TEXT:
+                prepared_step['action'] = step.data.action
+                if step.data.expected_result:
+                    prepared_step['expected_result'] = step.data.expected_result
+
+            if step.step_type == StepType.REQUEST:
+                prepared_step['action'] = step.data.request_method + " " + step.data.request_url
+                if step.data.request_body:
+                    step.attachments.append(
+                        Attachment(file_name='request_body.txt', content=step.data.request_body, mime_type='text/plain',
+                                   temporary=True))
+                if step.data.request_headers:
+                    step.attachments.append(
+                        Attachment(file_name='request_headers.txt', content=step.data.request_headers,
+                                   mime_type='text/plain', temporary=True))
+                if step.data.response_body:
+                    step.attachments.append(Attachment(file_name='response_body.txt', content=step.data.response_body,
+                                                       mime_type='text/plain', temporary=True))
+                if step.data.response_headers:
+                    step.attachments.append(
+                        Attachment(file_name='response_headers.txt', content=step.data.response_headers,
+                                   mime_type='text/plain', temporary=True))
+
+            if step.step_type == StepType.GHERKIN:
+                prepared_step['action'] = step.data.keyword
+
+            if step.step_type == StepType.SLEEP:
+                prepared_step['action'] = f"Sleep for {step.data.duration} seconds"
+
+            if step.attachments:
+                uploaded_attachments = []
+                for file in step.attachments:
+                    uploaded_attachments.extend(self._upload(file))
+                prepared_step['attachments'] = [attach.hash for attach in uploaded_attachments]
+
+            if step.steps:
+                for substep in step.steps:
+                    prepared_children.append(self._prepare_step(substep))
+                prepared_step["steps"] = prepared_children
+            return prepared_step
+        except Exception as e:
+            self.logger.log(f"Error at preparing step: {e}", "error")
+            raise ReporterException(e)
 
-            if (result.get_field('layer')):
-                case_data["layer"] = result.get_field('layer')
+    # Lifecycle methods
+    def start_run(self) -> str:
+        if self.plan_id and not self.run_id:
+            self._create_run(plan_id=self.plan_id, environment_id=self.environment)
+        if not self.run_id and not self.plan_id:
+            self._create_run(environment_id=self.environment)
+        if not self.run and not self._load_run:
+            raise ReporterException("Unable to find given test run.")
+        return self.run_id
+
+    def complete_run(self, exit_code=None) -> None:
+        if len(self.results) > 0:
+            self._send_results()
+        if self.complete_after_run:
+            self._complete_run()
+
+    def complete_worker(self) -> None:
+        if len(self.results) > 0:
+            self._send_results()
+
+    def add_result(self, result: Result) -> None:
+        self.results.append(result)
+        if len(self.results) >= self.batch_size:
+            self._send_results()
 
-            if result.get_suite_title():
-                case_data["suite_title"] = "\t".join(result.get_suite_title().split("."))
+    def get_results(self) -> List:
+        return self.results + self.processed
 
-            try:
-                api_results.create_result(
-                    code=self.project_code,
-                    id=self.run_id,
-                    result_create=ResultCreate(
-                        case_id=result.get_testops_id(),
-                        status=result.execution.status,
-                        stacktrace=result.execution.stacktrace,
-                        time_ms=result.execution.duration,
-                        comment=result.message,
-                        attachments = [attach.hash for attach in attached],
-                        defect=self.defect,
-                        case=ResultCreateCase(
-                            **{k: v for k, v in case_data.items() if v is not None}
-                        ),
-                        steps=steps,
-                        param=result.params
-                    )
-                )
-                print(f"[Qase] Results of run {self.run_id} was sent")
-            except Exception as e:
-                print(f"[Qase] ⚠️  Error at sending results for run {self.run_id}: {e}")
-                raise e
-
-    # Lifecycle methods
-    def start_run(self):
-        if self.enabled:
-            """Verify test run"""
-            self._check_run()
-            return self.run_id
-
-    def complete_run(self, is_main=True, exit_code=None):
-        if self.enabled:
-            if self.bulk:
-                self._send_bulk_results()
-            if self.complete_after_run and is_main:
-                self._complete_run()
-
-    def add_result(self, result: Result):
-        if self.enabled:
-            if self.bulk:
-                self.results.append(result)
-            else:
-                self._send_result(result)
+    def set_results(self, results) -> None:
+        self.results = results
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

