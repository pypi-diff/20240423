# Comparing `tmp/able_recipe_test-1.0.14.10.tar.gz` & `tmp/able_recipe_test-1.0.14.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "able_recipe_test-1.0.14.10.tar", last modified: Tue Apr 23 12:16:02 2024, max compression
+gzip compressed data, was "able_recipe_test-1.0.14.11.tar", last modified: Tue Apr 23 12:29:38 2024, max compression
```

## Comparing `able_recipe_test-1.0.14.10.tar` & `able_recipe_test-1.0.14.11.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2570 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/CHANGELOG.rst
--rw-r--r--   0 b3b       (1000) b3b       (1000)     1071 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/LICENSE
--rw-r--r--   0 b3b       (1000) b3b       (1000)       90 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/MANIFEST.in
--rw-r--r--   0 b3b       (1000) b3b       (1000)     3179 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/PKG-INFO
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2425 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/README.rst
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/able/
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2457 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/__init__.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     5612 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/adapter.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)    10840 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/advertising.py
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/able/android/
--rw-r--r--   0 b3b       (1000) b3b       (1000)        0 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/android/__init__.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     3407 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/android/dispatcher.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     6651 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/android/jni.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)    11866 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/dispatcher.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     7843 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/filters.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2024 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/permissions.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2217 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/queue.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)      690 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/scan_settings.py
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.670057 able_recipe_test-1.0.14.10/able/src/
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.670057 able_recipe_test-1.0.14.10/able/src/org/
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/able/src/org/able/
--rw-r--r--   0 b3b       (1000) b3b       (1000)    12850 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/src/org/able/BLE.java
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2834 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/src/org/able/BLEAdvertiser.java
--rw-r--r--   0 b3b       (1000) b3b       (1000)     1254 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/src/org/able/PythonBluetooth.java
--rw-r--r--   0 b3b       (1000) b3b       (1000)      671 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/src/org/able/PythonBluetoothAdvertiser.java
--rw-r--r--   0 b3b       (1000) b3b       (1000)     2277 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/structures.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)      946 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.10/able/utils.py
--rw-r--r--   0 b3b       (1000) b3b       (1000)       26 2024-04-23 12:12:46.000000 able_recipe_test-1.0.14.10/able/version.py
-drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/
--rw-r--r--   0 b3b       (1000) b3b       (1000)     3179 2024-04-23 12:16:02.000000 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/PKG-INFO
--rw-rw-r--   0 b3b       (1000) b3b       (1000)      679 2024-04-23 12:16:02.000000 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/SOURCES.txt
--rw-rw-r--   0 b3b       (1000) b3b       (1000)        1 2024-04-23 12:16:02.000000 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/dependency_links.txt
--rw-rw-r--   0 b3b       (1000) b3b       (1000)        1 2024-04-23 12:15:51.000000 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/not-zip-safe
--rw-rw-r--   0 b3b       (1000) b3b       (1000)        5 2024-04-23 12:16:02.000000 able_recipe_test-1.0.14.10/able_recipe_test.egg-info/top_level.txt
--rw-r--r--   0 b3b       (1000) b3b       (1000)       38 2024-04-23 12:16:02.674057 able_recipe_test-1.0.14.10/setup.cfg
--rw-r--r--   0 b3b       (1000) b3b       (1000)     4731 2024-04-23 12:15:47.000000 able_recipe_test-1.0.14.10/setup.py
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2570 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/CHANGELOG.rst
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     1071 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/LICENSE
+-rw-r--r--   0 b3b       (1000) b3b       (1000)       90 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/MANIFEST.in
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     3179 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/PKG-INFO
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2425 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/README.rst
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.180520 able_recipe_test-1.0.14.11/able/
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2457 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/__init__.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     5612 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/adapter.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)    10840 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/advertising.py
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/able/android/
+-rw-r--r--   0 b3b       (1000) b3b       (1000)        0 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/android/__init__.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     3407 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/android/dispatcher.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     6651 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/android/jni.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)    11866 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/dispatcher.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     7843 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/filters.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2024 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/permissions.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2217 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/queue.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)      690 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/scan_settings.py
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.180520 able_recipe_test-1.0.14.11/able/src/
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.180520 able_recipe_test-1.0.14.11/able/src/org/
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/able/src/org/able/
+-rw-r--r--   0 b3b       (1000) b3b       (1000)    12850 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/src/org/able/BLE.java
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2834 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/src/org/able/BLEAdvertiser.java
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     1254 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/src/org/able/PythonBluetooth.java
+-rw-r--r--   0 b3b       (1000) b3b       (1000)      671 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/src/org/able/PythonBluetoothAdvertiser.java
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     2277 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/structures.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)      946 2023-07-23 20:48:49.000000 able_recipe_test-1.0.14.11/able/utils.py
+-rw-r--r--   0 b3b       (1000) b3b       (1000)       26 2024-04-23 12:29:30.000000 able_recipe_test-1.0.14.11/able/version.py
+drwxrwxr-x   0 b3b       (1000) b3b       (1000)        0 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     3179 2024-04-23 12:29:38.000000 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/PKG-INFO
+-rw-rw-r--   0 b3b       (1000) b3b       (1000)      679 2024-04-23 12:29:38.000000 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 b3b       (1000) b3b       (1000)        1 2024-04-23 12:29:38.000000 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 b3b       (1000) b3b       (1000)        1 2024-04-23 12:15:51.000000 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/not-zip-safe
+-rw-rw-r--   0 b3b       (1000) b3b       (1000)        5 2024-04-23 12:29:38.000000 able_recipe_test-1.0.14.11/able_recipe_test.egg-info/top_level.txt
+-rw-r--r--   0 b3b       (1000) b3b       (1000)       38 2024-04-23 12:29:38.184521 able_recipe_test-1.0.14.11/setup.cfg
+-rw-r--r--   0 b3b       (1000) b3b       (1000)     4731 2024-04-23 12:29:07.000000 able_recipe_test-1.0.14.11/setup.py
```

### Comparing `able_recipe_test-1.0.14.10/CHANGELOG.rst` & `able_recipe_test-1.0.14.11/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/LICENSE` & `able_recipe_test-1.0.14.11/LICENSE`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/PKG-INFO` & `able_recipe_test-1.0.14.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: able_recipe_test
-Version: 1.0.14.10
+Version: 1.0.14.11
 Summary: Bluetooth Low Energy for Android
 Home-page: https://github.com/b3b/able
 Author: b3b
 Author-email: ash.b3b@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/b3b/able/blob/master/CHANGELOG.rst
 Keywords: android ble bluetooth kivy
```

### Comparing `able_recipe_test-1.0.14.10/README.rst` & `able_recipe_test-1.0.14.11/README.rst`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/__init__.py` & `able_recipe_test-1.0.14.11/able/__init__.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/adapter.py` & `able_recipe_test-1.0.14.11/able/adapter.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/advertising.py` & `able_recipe_test-1.0.14.11/able/advertising.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/android/dispatcher.py` & `able_recipe_test-1.0.14.11/able/android/dispatcher.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/android/jni.py` & `able_recipe_test-1.0.14.11/able/android/jni.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/dispatcher.py` & `able_recipe_test-1.0.14.11/able/dispatcher.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/filters.py` & `able_recipe_test-1.0.14.11/able/filters.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/permissions.py` & `able_recipe_test-1.0.14.11/able/permissions.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/queue.py` & `able_recipe_test-1.0.14.11/able/queue.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/scan_settings.py` & `able_recipe_test-1.0.14.11/able/scan_settings.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/src/org/able/BLE.java` & `able_recipe_test-1.0.14.11/able/src/org/able/BLE.java`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/src/org/able/BLEAdvertiser.java` & `able_recipe_test-1.0.14.11/able/src/org/able/BLEAdvertiser.java`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/src/org/able/PythonBluetooth.java` & `able_recipe_test-1.0.14.11/able/src/org/able/PythonBluetooth.java`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/src/org/able/PythonBluetoothAdvertiser.java` & `able_recipe_test-1.0.14.11/able/src/org/able/PythonBluetoothAdvertiser.java`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/structures.py` & `able_recipe_test-1.0.14.11/able/structures.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able/utils.py` & `able_recipe_test-1.0.14.11/able/utils.py`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/able_recipe_test.egg-info/PKG-INFO` & `able_recipe_test-1.0.14.11/able_recipe_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: able_recipe_test
-Version: 1.0.14.10
+Version: 1.0.14.11
 Summary: Bluetooth Low Energy for Android
 Home-page: https://github.com/b3b/able
 Author: b3b
 Author-email: ash.b3b@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/b3b/able/blob/master/CHANGELOG.rst
 Keywords: android ble bluetooth kivy
```

### Comparing `able_recipe_test-1.0.14.10/able_recipe_test.egg-info/SOURCES.txt` & `able_recipe_test-1.0.14.11/able_recipe_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `able_recipe_test-1.0.14.10/setup.py` & `able_recipe_test-1.0.14.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         "Programming Language :: Python :: 3.9",
     ],
     keywords="android ble bluetooth kivy",
     license="MIT",
     zip_safe=False,
     cmdclass={
         "install": InstallRecipe,
-        "bdist_wheel": build_sdist,
+        "bdist_wheel": bdist_wheel,
     },
     distclass=BinaryDistribution,
     # cmdclass={"bdist_wheel": bdist_wheel},
     # options={"bdist_wheel": {"universal": True}},
     # ext_modules=[Extension(name="able.force.rebuild", sources=[])],
     # options={"bdist_wheel": {"plat_name": "nowheel"}},
 )
```

