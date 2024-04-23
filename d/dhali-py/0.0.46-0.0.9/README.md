# Comparing `tmp/dhali_py-0.0.46.tar.gz` & `tmp/dhali-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhali_py-0.0.46.tar", last modified: Tue Apr 23 19:03:28 2024, max compression
+gzip compressed data, was "dhali-py-0.0.9.tar", last modified: Thu May 11 19:21:46 2023, max compression
```

## Comparing `dhali_py-0.0.46.tar` & `dhali-py-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.378624 dhali_py-0.0.46/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.374624 dhali_py-0.0.46/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 19:03:19.000000 dhali_py-0.0.46/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.374624 dhali_py-0.0.46/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-23 19:03:19.000000 dhali_py-0.0.46/.github/workflows/package_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 19:03:19.000000 dhali_py-0.0.46/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 19:03:19.000000 dhali_py-0.0.46/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 19:03:19.000000 dhali_py-0.0.46/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-04-23 19:03:19.000000 dhali_py-0.0.46/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 19:03:19.000000 dhali_py-0.0.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 19:03:28.378624 dhali_py-0.0.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 19:03:19.000000 dhali_py-0.0.46/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.374624 dhali_py-0.0.46/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.374624 dhali_py-0.0.46/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 19:03:19.000000 dhali_py-0.0.46/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-23 19:03:19.000000 dhali_py-0.0.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-23 19:03:28.378624 dhali_py-0.0.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 19:03:19.000000 dhali_py-0.0.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.370624 dhali_py-0.0.46/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.374624 dhali_py-0.0.46/src/dhali/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 19:03:19.000000 dhali_py-0.0.46/src/dhali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-23 19:03:19.000000 dhali_py-0.0.46/src/dhali/payment_claim_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.378624 dhali_py-0.0.46/src/dhali_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 19:03:28.000000 dhali_py-0.0.46/src/dhali_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:03:28.378624 dhali_py-0.0.46/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 19:03:19.000000 dhali_py-0.0.46/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:03:19.000000 dhali_py-0.0.46/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/workflows/package_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 19:21:37.000000 dhali-py-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 19:21:37.000000 dhali-py-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-11 19:21:37.000000 dhali-py-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 19:21:37.000000 dhali-py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-11 19:21:46.856405 dhali-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 19:21:37.000000 dhali-py-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 19:21:37.000000 dhali-py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-11 19:21:46.856405 dhali-py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 19:21:37.000000 dhali-py-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/src/dhali/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/payment_claim_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/src/dhali_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tests/test_transaction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tox.ini
```

### Comparing `dhali_py-0.0.46/.github/workflows/package_test.yaml` & `dhali-py-0.0.9/.github/workflows/package_test.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -22,7 +22,10 @@
           pip install flake8 pytest .[testing]
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+      - name: Test with pytest
+        run: |
+          pytest
```

### Comparing `dhali_py-0.0.46/.github/workflows/release.yaml` & `dhali-py-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/CONTRIBUTING.rst` & `dhali-py-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/LICENSE` & `dhali-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/README.rst` & `dhali-py-0.0.9/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 
 ========
 Dhali-py
 ========
 
 
 This python package is intended to support interfacing with Dhali.
-It offers a cli tools for creating payment claims used to access Dhali::
+It is used by Dhali to support payment-claim transaction validation on the Dhali backend microservices.
 
-        $ dhali create-xrpl-payment-claim -h
-        usage: dhali create-xrpl-payment-claim [-h] [-s SOURCE_SECRET] [-a AUTH_CLAIM_AMOUNT] [-t TOTAL_AMOUNT_CONTAINED_IN_CHANNEL]
-
-        options:
-        -h, --help            show this help message and exit
-        -s SOURCE_SECRET, --source_secret SOURCE_SECRET
-        -a AUTH_CLAIM_AMOUNT, --auth_claim_amount AUTH_CLAIM_AMOUNT
-                                Amount (in drops) that claim authorises to be extracted from the channel (must be less than --total_amount_contained_in_channel)
-        -t TOTAL_AMOUNT_CONTAINED_IN_CHANNEL, --total_amount_contained_in_channel TOTAL_AMOUNT_CONTAINED_IN_CHANNEL
-                                Total drops to escrow in the channel (must be less than total amount of XRP in wallet)
+It also offers two cli tools for creating payment claim objects used to access Dhali.
 
 Install and run
 ===============
 
 1. `pip install .`
-2. To generate a test XRPL wallet or determine you wallet's seed::
+2. To generate a test XRPL wallet::
 
         dhali create-xrpl-wallet
 
 3. To generate a Dhali payment claim::
 
-        dhali create-xrpl-payment-claim -s <secret from 2.> -a 500000 -t 1000000
+        dhali create-xrpl-payment-claim -s <secret from 2.> -d rstbSTpPcyxMsiXwkBxS9tFTrg2JsDNxWk -a 10000000 -i <sequence number from 2.> -t 100000000
 
 
 .. _pyscaffold-notes:
+
+Note
+====
+
+This project has been set up using PyScaffold 4.3.1. For details and usage
+information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `dhali_py-0.0.46/docs/Makefile` & `dhali-py-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/docs/conf.py` & `dhali-py-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/docs/index.rst` & `dhali-py-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/setup.cfg` & `dhali-py-0.0.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,23 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	xrpl-py==2.5.0
+	xrpl-py==1.7.0
+	fastapi==0.81.0
+	google==3.0.0
+	google-api-core==2.11.0
+	google-auth==2.16.2
+	google-cloud==0.34.0
+	google-cloud-vision==3.4.0
+	googleapis-common-protos==1.58.0
+	google-cloud-firestore==2.10.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `dhali_py-0.0.46/setup.py` & `dhali-py-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/src/dhali/__init__.py` & `dhali-py-0.0.9/src/dhali/__init__.py`

 * *Files identical despite different names*

### Comparing `dhali_py-0.0.46/tox.ini` & `dhali-py-0.0.9/tox.ini`

 * *Files identical despite different names*

