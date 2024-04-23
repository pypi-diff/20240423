# Comparing `tmp/eth-keys-0.5.0.tar.gz` & `tmp/eth_keys-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-keys-0.5.0.tar", last modified: Wed Jan 10 21:00:00 2024, max compression
+gzip compressed data, was "eth_keys-0.5.1.tar", last modified: Tue Apr 23 19:50:36 2024, max compression
```

## Comparing `eth-keys-0.5.0.tar` & `eth_keys-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.216775 eth-keys-0.5.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-01-10 20:45:10.000000 eth-keys-0.5.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-01-10 20:45:10.000000 eth-keys-0.5.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)    13536 2024-01-10 21:00:00.216775 eth-keys-0.5.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11521 2024-01-10 20:45:10.000000 eth-keys-0.5.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/eth_keys/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      159 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/__init__.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/eth_keys/backends/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      872 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1069 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/base.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3867 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/coincurve.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/eth_keys/backends/native/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       44 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/native/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4706 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/native/ecdsa.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2459 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/native/jacobian.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1964 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/backends/native/main.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      584 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/constants.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12458 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/datatypes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      229 2023-12-20 22:22:14.000000 eth-keys-0.5.0/eth_keys/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4274 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/main.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-20 22:22:14.000000 eth-keys-0.5.0/eth_keys/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/eth_keys/tools/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-20 22:22:14.000000 eth-keys-0.5.0/eth_keys/tools/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      871 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/tools/factories.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/eth_keys/utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-20 22:22:14.000000 eth-keys-0.5.0/eth_keys/utils/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      149 2023-12-20 22:22:14.000000 eth-keys-0.5.0/eth_keys/utils/address.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3490 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/utils/der.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1504 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/utils/module_loading.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      477 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/utils/numeric.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       70 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/utils/padding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2772 2024-01-10 20:45:10.000000 eth-keys-0.5.0/eth_keys/validation.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.216775 eth-keys-0.5.0/eth_keys.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)    13536 2024-01-10 21:00:00.000000 eth-keys-0.5.0/eth_keys.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1213 2024-01-10 21:00:00.000000 eth-keys-0.5.0/eth_keys.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-01-10 21:00:00.000000 eth-keys-0.5.0/eth_keys.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-20 22:27:47.000000 eth-keys-0.5.0/eth_keys.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      426 2024-01-10 21:00:00.000000 eth-keys-0.5.0/eth_keys.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        9 2024-01-10 21:00:00.000000 eth-keys-0.5.0/eth_keys.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3407 2024-01-10 20:52:49.000000 eth-keys-0.5.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-01-10 21:00:00.216775 eth-keys-0.5.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2063 2024-01-10 20:59:47.000000 eth-keys-0.5.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.212775 eth-keys-0.5.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.216775 eth-keys-0.5.0/tests/backends/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4155 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/backends/conftest.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      435 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/backends/strategies.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4820 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/backends/test_backends.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5565 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/backends/test_native_backend_against_coincurve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      635 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/conftest.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-10 21:00:00.216775 eth-keys-0.5.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      364 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_factories.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       53 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_import.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5806 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_key_and_signature_datastructures.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2251 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_key_api_proxy_methods.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      629 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_keyapi_backend_formats.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2340 2024-01-10 20:45:10.000000 eth-keys-0.5.0/tests/core/test_utils_der.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-04-15 20:01:55.000000 eth_keys-0.5.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-04-15 20:01:55.000000 eth_keys-0.5.1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)    13581 2024-04-23 19:50:36.644828 eth_keys-0.5.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11521 2024-04-15 20:01:55.000000 eth_keys-0.5.1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.640828 eth_keys-0.5.1/eth_keys/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      159 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.640828 eth_keys-0.5.1/eth_keys/backends/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      872 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1069 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/base.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3867 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/coincurve.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.640828 eth_keys-0.5.1/eth_keys/backends/native/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       44 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/native/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4706 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/native/ecdsa.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2459 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/native/jacobian.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1964 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/backends/native/main.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      584 2024-04-15 20:31:04.000000 eth_keys-0.5.1/eth_keys/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12458 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/datatypes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      229 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4274 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/main.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.640828 eth_keys-0.5.1/eth_keys/tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/tools/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      871 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/tools/factories.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/eth_keys/utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      149 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/utils/address.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3490 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/utils/der.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1504 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/utils/module_loading.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      499 2024-04-23 15:56:24.000000 eth_keys-0.5.1/eth_keys/utils/numeric.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       70 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/utils/padding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2772 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/eth_keys.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)    13581 2024-04-23 19:50:36.000000 eth_keys-0.5.1/eth_keys.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1225 2024-04-23 19:50:36.000000 eth_keys-0.5.1/eth_keys.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-23 19:50:36.000000 eth_keys-0.5.1/eth_keys.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-15 20:01:55.000000 eth_keys-0.5.1/eth_keys.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      420 2024-04-23 19:50:36.000000 eth_keys-0.5.1/eth_keys.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        9 2024-04-23 19:50:36.000000 eth_keys-0.5.1/eth_keys.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3441 2024-04-23 15:56:24.000000 eth_keys-0.5.1/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-23 19:50:36.644828 eth_keys-0.5.1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2110 2024-04-23 19:50:28.000000 eth_keys-0.5.1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/tests/backends/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4156 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/backends/conftest.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      439 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/backends/strategies.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4820 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/backends/test_backends.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5566 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/backends/test_native_backend_against_coincurve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      635 2024-04-15 20:01:55.000000 eth_keys-0.5.1/tests/conftest.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 19:50:36.644828 eth_keys-0.5.1/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      364 2024-04-15 20:01:55.000000 eth_keys-0.5.1/tests/core/test_factories.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      101 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/core/test_import_and_version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5807 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/core/test_key_and_signature_datastructures.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2252 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/core/test_key_api_proxy_methods.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      629 2024-04-15 20:01:55.000000 eth_keys-0.5.1/tests/core/test_keyapi_backend_formats.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2341 2024-04-23 15:56:24.000000 eth_keys-0.5.1/tests/core/test_utils_der.py
```

### Comparing `eth-keys-0.5.0/LICENSE` & `eth_keys-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/PKG-INFO` & `eth_keys-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-keys
-Version: 0.5.0
+Version: 0.5.1
 Summary: eth-keys: Common API for Ethereum key operations
 Home-page: https://github.com/ethereum/eth-keys
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Requires-Dist: eth-typing>=3
 Provides-Extra: coincurve
 Requires-Dist: coincurve>=12.0.0; extra == "coincurve"
@@ -33,24 +34,24 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: asn1tools>=0.146.2; extra == "dev"
 Requires-Dist: factory-boy>=3.0.1; extra == "dev"
 Requires-Dist: pyasn1>=0.4.5; extra == "dev"
-Requires-Dist: hypothesis<6,>=5.10.3; extra == "dev"
+Requires-Dist: hypothesis>=5.10.3; extra == "dev"
 Requires-Dist: eth-hash[pysha3]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: asn1tools>=0.146.2; extra == "test"
 Requires-Dist: factory-boy>=3.0.1; extra == "test"
 Requires-Dist: pyasn1>=0.4.5; extra == "test"
-Requires-Dist: hypothesis<6,>=5.10.3; extra == "test"
+Requires-Dist: hypothesis>=5.10.3; extra == "test"
 Requires-Dist: eth-hash[pysha3]; extra == "test"
 
 # eth-keys
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/eth-keys.svg?style=shield)](https://circleci.com/gh/ethereum/eth-keys)
 [![PyPI version](https://badge.fury.io/py/eth-keys.svg)](https://badge.fury.io/py/eth-keys)
```

### Comparing `eth-keys-0.5.0/README.md` & `eth_keys-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/__init__.py` & `eth_keys-0.5.1/eth_keys/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/base.py` & `eth_keys-0.5.1/eth_keys/backends/base.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/coincurve.py` & `eth_keys-0.5.1/eth_keys/backends/coincurve.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/native/ecdsa.py` & `eth_keys-0.5.1/eth_keys/backends/native/ecdsa.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/native/jacobian.py` & `eth_keys-0.5.1/eth_keys/backends/native/jacobian.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/backends/native/main.py` & `eth_keys-0.5.1/eth_keys/backends/native/main.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/constants.py` & `eth_keys-0.5.1/eth_keys/constants.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/datatypes.py` & `eth_keys-0.5.1/eth_keys/datatypes.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/main.py` & `eth_keys-0.5.1/eth_keys/main.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/tools/factories.py` & `eth_keys-0.5.1/eth_keys/tools/factories.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/utils/der.py` & `eth_keys-0.5.1/eth_keys/utils/der.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/utils/module_loading.py` & `eth_keys-0.5.1/eth_keys/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys/validation.py` & `eth_keys-0.5.1/eth_keys/validation.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/eth_keys.egg-info/PKG-INFO` & `eth_keys-0.5.1/eth_keys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-keys
-Version: 0.5.0
+Version: 0.5.1
 Summary: eth-keys: Common API for Ethereum key operations
 Home-page: https://github.com/ethereum/eth-keys
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-utils>=2
 Requires-Dist: eth-typing>=3
 Provides-Extra: coincurve
 Requires-Dist: coincurve>=12.0.0; extra == "coincurve"
@@ -33,24 +34,24 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: asn1tools>=0.146.2; extra == "dev"
 Requires-Dist: factory-boy>=3.0.1; extra == "dev"
 Requires-Dist: pyasn1>=0.4.5; extra == "dev"
-Requires-Dist: hypothesis<6,>=5.10.3; extra == "dev"
+Requires-Dist: hypothesis>=5.10.3; extra == "dev"
 Requires-Dist: eth-hash[pysha3]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: asn1tools>=0.146.2; extra == "test"
 Requires-Dist: factory-boy>=3.0.1; extra == "test"
 Requires-Dist: pyasn1>=0.4.5; extra == "test"
-Requires-Dist: hypothesis<6,>=5.10.3; extra == "test"
+Requires-Dist: hypothesis>=5.10.3; extra == "test"
 Requires-Dist: eth-hash[pysha3]; extra == "test"
 
 # eth-keys
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/eth-keys.svg?style=shield)](https://circleci.com/gh/ethereum/eth-keys)
 [![PyPI version](https://badge.fury.io/py/eth-keys.svg)](https://badge.fury.io/py/eth-keys)
```

### Comparing `eth-keys-0.5.0/eth_keys.egg-info/SOURCES.txt` & `eth_keys-0.5.1/eth_keys.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 eth_keys/utils/padding.py
 tests/conftest.py
 tests/backends/conftest.py
 tests/backends/strategies.py
 tests/backends/test_backends.py
 tests/backends/test_native_backend_against_coincurve.py
 tests/core/test_factories.py
-tests/core/test_import.py
+tests/core/test_import_and_version.py
 tests/core/test_key_and_signature_datastructures.py
 tests/core/test_key_api_proxy_methods.py
 tests/core/test_keyapi_backend_formats.py
 tests/core/test_utils_der.py
```

### Comparing `eth-keys-0.5.0/pyproject.toml` & `eth_keys-0.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.autoflake]
-remove_all_unused_imports = true
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
 combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
 force_sort_within_sections = true
-known_third_party = "hypothesis,pytest"
+honor_noqa = true
 known_first_party = "eth_keys"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
 check_untyped_defs = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = true
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = false
-disallow_subclassing_any = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
-strict_optional = false
 strict_equality = true
+strict_optional = false
 warn_redundant_casts = true
 warn_return_any = false
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.pydocstyle]
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = true
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/eth-keys/blob/main/newsfragments/README.md for instructions
-package = "eth_keys"
-filename = "CHANGELOG.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "eth-keys v{version} ({project_date})"
+filename = "CHANGELOG.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-keys/issues/{issue}>`__"
+package = "eth_keys"
+title_format = "eth-keys v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `eth-keys-0.5.0/setup.py` & `eth_keys-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "towncrier>=21,<22",
     ],
     "test": [
         "pytest>=7.0.0",
         "asn1tools>=0.146.2",
         "factory-boy>=3.0.1",
         "pyasn1>=0.4.5",
-        "hypothesis>=5.10.3,<6",
+        "hypothesis>=5.10.3",
         "eth-hash[pysha3]",
     ],
 }
 
 extras_require["dev"] = (
     extras_require["coincurve"]
     + extras_require["dev"]
@@ -41,15 +41,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-keys",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="0.5.0",
+    version="0.5.1",
     description="""eth-keys: Common API for Ethereum key operations""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-keys",
     include_package_data=True,
@@ -71,9 +71,10 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `eth-keys-0.5.0/tests/backends/conftest.py` & `eth_keys-0.5.1/tests/backends/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from eth_utils import (
     decode_hex,
     keccak,
 )
-import pytest
 
 MSG = b"message"
 MSGHASH = keccak(MSG)
 
 
 # This is a sample of signatures generated with a known-good implementation of the ECDSA
 # algorithm, which we use to test our ECC backends. If necessary, it can be generated
```

### Comparing `eth-keys-0.5.0/tests/backends/test_backends.py` & `eth_keys-0.5.1/tests/backends/test_backends.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
+import pytest
 
 from eth_utils import (
     keccak,
 )
 from hypothesis import (
     given,
 )
-import pytest
 from strategies import (
     message_hash_st,
     private_key_st,
 )
 
 from eth_keys import (
     KeyAPI,
```

### Comparing `eth-keys-0.5.0/tests/backends/test_native_backend_against_coincurve.py` & `eth_keys-0.5.1/tests/backends/test_native_backend_against_coincurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import pytest
+
 from eth_utils import (
     keccak,
 )
 from hypothesis import (
     given,
     settings,
     strategies as st,
 )
-import pytest
 from strategies import (
     message_hash_st,
     private_key_st,
     signature_st,
 )
 
 from eth_keys import (
```

### Comparing `eth-keys-0.5.0/tests/conftest.py` & `eth_keys-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/tests/core/test_key_and_signature_datastructures.py` & `eth_keys-0.5.1/tests/core/test_key_and_signature_datastructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import pytest
+
 from eth_utils import (
     ValidationError,
     decode_hex,
     encode_hex,
     is_canonical_address,
     is_checksum_address,
     is_normalized_address,
     is_same_address,
     keccak,
 )
-import pytest
 
 from eth_keys import (
     KeyAPI,
 )
 from eth_keys.backends import (
     NativeECCBackend,
 )
```

### Comparing `eth-keys-0.5.0/tests/core/test_key_api_proxy_methods.py` & `eth_keys-0.5.1/tests/core/test_key_api_proxy_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from eth_utils import (
     ValidationError,
     keccak,
 )
-import pytest
 
 from eth_keys import (
     KeyAPI,
 )
 from eth_keys.backends import (
     NativeECCBackend,
 )
```

### Comparing `eth-keys-0.5.0/tests/core/test_keyapi_backend_formats.py` & `eth_keys-0.5.1/tests/core/test_keyapi_backend_formats.py`

 * *Files identical despite different names*

### Comparing `eth-keys-0.5.0/tests/core/test_utils_der.py` & `eth_keys-0.5.1/tests/core/test_utils_der.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 import asn1tools
 from hypothesis import (
     example,
     given,
     settings,
     strategies as st,
 )
@@ -9,15 +11,14 @@
     decoder as pyasn1_decoder,
     encoder as pyasn1_encoder,
 )
 from pyasn1.type import (
     namedtype,
     univ,
 )
-import pytest
 
 from eth_keys.utils.der import (
     two_int_sequence_decoder,
     two_int_sequence_encoder,
 )
 
 ASN1_ECDSA_SPEC_STRING = """\
```

