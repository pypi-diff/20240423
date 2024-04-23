# Comparing `tmp/pingen2sdk-0.2.0.tar.gz` & `tmp/pingen2sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingen2sdk-0.2.0.tar", last modified: Fri Apr 19 10:20:31 2024, max compression
+gzip compressed data, was "pingen2sdk-0.3.1.tar", last modified: Tue Apr 23 08:12:50 2024, max compression
```

## Comparing `pingen2sdk-0.2.0.tar` & `pingen2sdk-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.794072 pingen2sdk-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-19 10:20:31.794072 pingen2sdk-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.786071 pingen2sdk-0.2.0/pingen2sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.790072 pingen2sdk-0.2.0/pingen2sdk/api_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/batch_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/letter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/letters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/organisations.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/api_resources/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pingen2sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.794072 pingen2sdk-0.2.0/pingen2sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-19 10:20:31.000000 pingen2sdk-0.2.0/pingen2sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 10:20:31.000000 pingen2sdk-0.2.0/pingen2sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:20:31.000000 pingen2sdk-0.2.0/pingen2sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 10:20:31.000000 pingen2sdk-0.2.0/pingen2sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 10:20:31.000000 pingen2sdk-0.2.0/pingen2sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:20:31.794072 pingen2sdk-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.790072 pingen2sdk-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:31.790072 pingen2sdk-0.2.0/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_batch_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_letter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_letters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_organisations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_user_accociations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/api_resources/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 10:20:26.000000 pingen2sdk-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.091928 pingen2sdk-0.3.1/pingen2sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/pingen2sdk/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/batch_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/letter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/letters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/organisations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/api_resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pingen2sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/pingen2sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 08:12:50.000000 pingen2sdk-0.3.1/pingen2sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:50.095928 pingen2sdk-0.3.1/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_batch_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_letter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_letters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_organisations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_user_accociations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/api_resources/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-23 08:12:44.000000 pingen2sdk-0.3.1/tox.ini
```

### Comparing `pingen2sdk-0.2.0/LICENSE` & `pingen2sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/PKG-INFO` & `pingen2sdk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingen2sdk
-Version: 0.2.0
+Version: 0.3.1
 Summary: Official Python Pingen SDK for API V2
 Author-email: Pingen GmbH <info@pingen.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pingencom/pingen2-sdk-python
 Project-URL: Bug Tracker, https://github.com/pingencom/pingen2-sdk-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pingen2sdk-0.2.0/README.md` & `pingen2sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/__init__.py` & `pingen2sdk-0.3.1/pingen2sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api.py` & `pingen2sdk-0.3.1/pingen2sdk/api.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/__init__.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/batch_events.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/batch_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/batches.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/batches.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/file_upload.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/file_upload.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/letter_events.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/letter_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/letters.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/letters.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/organisations.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/organisations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/user_associations.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/user_associations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/api_resources/users.py` & `pingen2sdk-0.3.1/pingen2sdk/api_resources/users.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/error.py` & `pingen2sdk-0.3.1/pingen2sdk/error.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/oauth.py` & `pingen2sdk-0.3.1/pingen2sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk/response.py` & `pingen2sdk-0.3.1/pingen2sdk/response.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pingen2sdk.egg-info/PKG-INFO` & `pingen2sdk-0.3.1/pingen2sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingen2sdk
-Version: 0.2.0
+Version: 0.3.1
 Summary: Official Python Pingen SDK for API V2
 Author-email: Pingen GmbH <info@pingen.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pingencom/pingen2-sdk-python
 Project-URL: Bug Tracker, https://github.com/pingencom/pingen2-sdk-python/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pingen2sdk-0.2.0/pingen2sdk.egg-info/SOURCES.txt` & `pingen2sdk-0.3.1/pingen2sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/pyproject.toml` & `pingen2sdk-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pingen2sdk"
-version = "0.2.0"
+version = "0.3.1"
 authors = [
   { name="Pingen GmbH", email="info@pingen.com" },
 ]
 description = "Official Python Pingen SDK for API V2"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -26,8 +26,8 @@
    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = { text = "BSD-3-Clause" }
 dependencies = ['requests>=2.31.0','typing-extensions','response']
 
 [project.urls]
 "Homepage" = "https://github.com/pingencom/pingen2-sdk-python"
-"Bug Tracker" = "https://github.com/pingencom/pingen2-sdk-python/issues"
+"Bug Tracker" = "https://github.com/pingencom/pingen2-sdk-python/issues"
```

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_batch_events.py` & `pingen2sdk-0.3.1/tests/api_resources/test_batch_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_batches.py` & `pingen2sdk-0.3.1/tests/api_resources/test_batches.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_file_upload.py` & `pingen2sdk-0.3.1/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_letter_events.py` & `pingen2sdk-0.3.1/tests/api_resources/test_letter_events.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_letters.py` & `pingen2sdk-0.3.1/tests/api_resources/test_letters.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,20 +316,17 @@
             },
             json=self._get_expected_payload("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx111"),
             status=201,
         )
 
         response = letters.upload_and_create_letter(
             "tests/api_resources/files/lorem.pdf",
+            "lorem.pdf",
             "left",
-            True,
-            "fast",
-            "simplex",
-            "color",
-            "ACME GmbH | Strasse 3 | 8000 Zürich",
+            False,
         )
 
         assert response.data["data"]["id"] == "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxx111"
         assert response.status_code == 201
         assert response.headers == {
             "Content-Type": "application/vnd.api+json",
             "X-Request-Id": "requestx-xxxx-xxxx-xxxx-xxxxxxxxxxx3",
```

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_organisations.py` & `pingen2sdk-0.3.1/tests/api_resources/test_organisations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_user_accociations.py` & `pingen2sdk-0.3.1/tests/api_resources/test_user_accociations.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/api_resources/test_users.py` & `pingen2sdk-0.3.1/tests/api_resources/test_users.py`

 * *Files identical despite different names*

### Comparing `pingen2sdk-0.2.0/tests/test_oauth.py` & `pingen2sdk-0.3.1/tests/test_oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
             )
 
     def test_authorize_url(self):
         url = pingen2sdk.OAuth.authorize_url(
             scope="letter",
             state="RANDOMGENERATEDSTRING",
             client_id="testClientId",
+            response_type="code"
         )
 
         result = requests.utils.urlparse(url)
         query = result.query
         params = dict(x.split("=") for x in query.split("&"))
 
         assert result.scheme == "https"
```

### Comparing `pingen2sdk-0.2.0/tox.ini` & `pingen2sdk-0.3.1/tox.ini`

 * *Files identical despite different names*

