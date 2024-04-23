# Comparing `tmp/testit_adapter_pytest-3.0.2.tar.gz` & `tmp/testit_adapter_pytest-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_adapter_pytest-3.0.2.tar", last modified: Mon Apr 22 12:43:21 2024, max compression
+gzip compressed data, was "testit_adapter_pytest-3.1.0.tar", last modified: Tue Apr 23 15:10:25 2024, max compression
```

## Comparing `testit_adapter_pytest-3.0.2.tar` & `testit_adapter_pytest-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/executable_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-22 12:43:15.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:21.505155 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 12:43:21.000000 testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:25.956847 testit_adapter_pytest-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-04-23 15:10:25.956847 testit_adapter_pytest-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:10:25.956847 testit_adapter_pytest-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:25.952847 testit_adapter_pytest-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:25.952847 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:25.956847 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/executable_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-23 15:10:21.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:25.956847 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 15:10:25.000000 testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit_adapter_pytest-3.0.2/PKG-INFO` & `testit_adapter_pytest-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 3.0.2
+Version: 3.1.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==3.0.2
+Requires-Dist: testit-python-commons==3.1.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit_adapter_pytest-3.0.2/README.md` & `testit_adapter_pytest-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/setup.py` & `testit_adapter_pytest-3.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='3.0.2',
+    version='3.1.0',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
     classifiers=[
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==3.0.2'],
+    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==3.1.0'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_context.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_context.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_manager.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_manager.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/fixture_storage.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/fixture_storage.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/listener.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pickle
+from importlib.metadata import metadata
 from uuid import uuid4
 
 from packaging import version
 
 import pytest
 
 import testit_python_commons.services as adapter
@@ -57,26 +58,29 @@
 
     def get_deselected_items(self) -> list:
         return self._deselected_items
 
 
 class TmsListener(object):
     __executable_test = None
+    __pytest_info = None
     __pytest_check_info = None
     __failures = None
 
     def __init__(self, adapter_manager: AdapterManager, step_manager: StepManager):
         self.__adapter_manager = adapter_manager
         self.__step_manager = step_manager
         self.fixture_manager = FixtureManager()
         self._cache = ItemCache()
         self.__test_result_ids = {}
 
     @pytest.hookimpl
     def pytest_configure(self, config):
+        self.__pytest_info = metadata("pytest")
+
         if not hasattr(config, "workerinput") and not hasattr(self, "test_run_id"):
             config.test_run_id = self.__adapter_manager.get_test_run_id()
         else:
             config.test_run_id = pickle.loads(config.workerinput["test_run_id"])
 
         self.__adapter_manager.set_test_run_id(config.test_run_id)
 
@@ -299,30 +303,33 @@
         self.fixture_manager.stop_after_fixture(uuid,
                                                 outcome=utils.get_status(exc_val),
                                                 steps=results_steps_data,
                                                 message=utils.get_message(exc_type, exc_val),
                                                 stacktrace=utils.get_traceback(exc_tb))
 
     def _update_fixtures_external_ids(self, item):
-        for fixturedef in _test_fixtures(item):
+        for fixturedef in self._test_fixtures(item):
             group_uuid = self._cache.get(fixturedef)
             if group_uuid:
                 group = self.fixture_manager.get_item(group_uuid)
             else:
                 group_uuid = self._cache.push(fixturedef)
                 group = FixturesContainer(uuid=group_uuid)
                 self.fixture_manager.start_group(group_uuid, group)
             if item.nodeid not in group.node_ids:
                 self.fixture_manager.update_group(group_uuid, node_ids=item.nodeid)
 
+    def _test_fixtures(self, item):
+        fixturemanager = item.session._fixturemanager
+        fixturedefs = []
+
+        if hasattr(item, "_request") and hasattr(item._request, "fixturenames"):
+            for name in item._request.fixturenames:
+                if self.__pytest_info and version.parse(self.__pytest_info["version"]) >= version.parse("8.1.0"):
+                    fixturedefs_pytest = fixturemanager.getfixturedefs(name, item)
+                else:
+                    fixturedefs_pytest = fixturemanager.getfixturedefs(name, item.nodeid)
 
-def _test_fixtures(item):
-    fixturemanager = item.session._fixturemanager
-    fixturedefs = []
-
-    if hasattr(item, "_request") and hasattr(item._request, "fixturenames"):
-        for name in item._request.fixturenames:
-            fixturedefs_pytest = fixturemanager.getfixturedefs(name, item.nodeid)
-            if fixturedefs_pytest:
-                fixturedefs.extend(fixturedefs_pytest)
+                if fixturedefs_pytest:
+                    fixturedefs.extend(fixturedefs_pytest)
 
-    return fixturedefs
+        return fixturedefs
```

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/executable_test.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/executable_test.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/models/fixture.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/models/fixture.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/plugin.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest/utils.py` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest/utils.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 3.0.2
+Version: 3.1.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==3.0.2
+Requires-Dist: testit-python-commons==3.1.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit_adapter_pytest-3.0.2/src/testit_adapter_pytest.egg-info/SOURCES.txt` & `testit_adapter_pytest-3.1.0/src/testit_adapter_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

