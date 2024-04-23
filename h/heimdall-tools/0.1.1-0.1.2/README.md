# Comparing `tmp/heimdall_tools-0.1.1.tar.gz` & `tmp/heimdall_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdall_tools-0.1.1.tar", last modified: Sun Apr 21 16:47:51 2024, max compression
+gzip compressed data, was "heimdall_tools-0.1.2.tar", last modified: Tue Apr 23 07:53:45 2024, max compression
```

## Comparing `heimdall_tools-0.1.1.tar` & `heimdall_tools-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1143 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/PKG-INFO
--rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      556 2024-04-21 16:39:40.000000 heimdall_tools-0.1.1/README.md
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.700622 heimdall_tools-0.1.1/heimdall_tools/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.1.1/heimdall_tools/__init__.py
--rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)     2483 2024-04-21 15:43:23.000000 heimdall_tools-0.1.1/heimdall_tools/mysql_client.py
--rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-08 11:55:43.000000 heimdall_tools-0.1.1/heimdall_tools/sns.py
--rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1208 2024-04-11 13:49:12.000000 heimdall_tools-0.1.1/heimdall_tools/sqs.py
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.720373 heimdall_tools-0.1.1/heimdall_tools.egg-info/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1143 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/PKG-INFO
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      309 2024-04-21 16:47:50.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       29 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/requires.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/top_level.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/setup.cfg
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      861 2024-04-21 16:47:33.000000 heimdall_tools-0.1.1/setup.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.421256 heimdall_tools-0.1.2/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1177 2024-04-23 07:53:45.417749 heimdall_tools-0.1.2/PKG-INFO
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      576 2024-04-23 07:53:00.000000 heimdall_tools-0.1.2/README.md
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.409654 heimdall_tools-0.1.2/heimdall_tools/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.1.2/heimdall_tools/__init__.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)     2458 2024-04-23 07:52:00.000000 heimdall_tools-0.1.2/heimdall_tools/mysql_client.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-08 11:55:43.000000 heimdall_tools-0.1.2/heimdall_tools/sns.py
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1208 2024-04-11 13:49:12.000000 heimdall_tools-0.1.2/heimdall_tools/sqs.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.417749 heimdall_tools-0.1.2/heimdall_tools.egg-info/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1177 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      309 2024-04-23 07:53:45.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       29 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/requires.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/top_level.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-04-23 07:53:45.421256 heimdall_tools-0.1.2/setup.cfg
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      861 2024-04-23 07:53:35.000000 heimdall_tools-0.1.2/setup.py
```

### Comparing `heimdall_tools-0.1.1/PKG-INFO` & `heimdall_tools-0.1.2/heimdall_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
-Name: heimdall_tools
-Version: 0.1.1
+Name: heimdall-tools
+Version: 0.1.2
 Summary: Custom package including all modules required for my application
 Home-page: https://github.com/your_username/your_package
 Author: Robin Thomas
 Author-email: robin@clockhash.com
 License: MIT
-Description: #Heimdall Tools
+Description: # Heimdall Tools
         
         This is a custom package created to use different modules in a single place.
         The wrapper methods are designed in a way to produce the best results to the application.
         This helps in code reusability and to improve the performance of application
         
-        #Create or modify package
+        # Create or modify package
+        
         i. Add the new module in heimdall_tools folder
         ii. Modify setup.py 
             ..* add dependices
         iii. Create the update package file
         python setup.py sdist 
         iv. Upload to pypi using twine
         twine upload dist/*
         
-        #how to install package
-        pip install heimdall_tools
+        #  how to install package
+        
+        pip install [--upgrade] heimdall_tools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `heimdall_tools-0.1.1/README.md` & `heimdall_tools-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-#Heimdall Tools
+# Heimdall Tools
 
 This is a custom package created to use different modules in a single place.
 The wrapper methods are designed in a way to produce the best results to the application.
 This helps in code reusability and to improve the performance of application
 
-#Create or modify package
+# Create or modify package
+
 i. Add the new module in heimdall_tools folder
 ii. Modify setup.py 
     ..* add dependices
 iii. Create the update package file
 python setup.py sdist 
 iv. Upload to pypi using twine
 twine upload dist/*
 
-#how to install package
-pip install heimdall_tools
+#  how to install package
+
+pip install [--upgrade] heimdall_tools
```

### Comparing `heimdall_tools-0.1.1/heimdall_tools/mysql_client.py` & `heimdall_tools-0.1.2/heimdall_tools/mysql_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     username: String
     password: String
     host: String
     database_name: String
     raise_on_warnings: Bool
 """""
 class MYSQL_DB_CLIENT:
-    def __init__(self, username, password, hostname, database_name, raise_on_warnings) -> None:
+    def __init__(self, username, password, hostname, database_name, raise_on_warnings = True) -> None:
         self.username = username
         self.password =password
         self.hostname = hostname
         self.database_name = database_name
         self.raise_on_warnings = raise_on_warnings
         self.cursor = None 
 
@@ -54,14 +54,12 @@
         AND floors.floor_position = %s
         AND sensor_type.type_id = %s
         AND sensors.sensor_name = %s
         """
         # Execute the query
         self.cursor.execute(query, (customer_name, site_name, building_name, floor_position, type_id, sensor_name))
         result = self.cursor.fetchone()
-        sensor_id = -1
         if result:
             print(f"MYSQL LOGS: Result --> {result}")
-            sensor_id = result['sensor_id']
+            #sensor_id = result['sensor_id']
         
-        return sensor_id
-    
+        return result
```

### Comparing `heimdall_tools-0.1.1/heimdall_tools/sns.py` & `heimdall_tools-0.1.2/heimdall_tools/sns.py`

 * *Files identical despite different names*

### Comparing `heimdall_tools-0.1.1/heimdall_tools/sqs.py` & `heimdall_tools-0.1.2/heimdall_tools/sqs.py`

 * *Files identical despite different names*

### Comparing `heimdall_tools-0.1.1/heimdall_tools.egg-info/PKG-INFO` & `heimdall_tools-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
-Name: heimdall-tools
-Version: 0.1.1
+Name: heimdall_tools
+Version: 0.1.2
 Summary: Custom package including all modules required for my application
 Home-page: https://github.com/your_username/your_package
 Author: Robin Thomas
 Author-email: robin@clockhash.com
 License: MIT
-Description: #Heimdall Tools
+Description: # Heimdall Tools
         
         This is a custom package created to use different modules in a single place.
         The wrapper methods are designed in a way to produce the best results to the application.
         This helps in code reusability and to improve the performance of application
         
-        #Create or modify package
+        # Create or modify package
+        
         i. Add the new module in heimdall_tools folder
         ii. Modify setup.py 
             ..* add dependices
         iii. Create the update package file
         python setup.py sdist 
         iv. Upload to pypi using twine
         twine upload dist/*
         
-        #how to install package
-        pip install heimdall_tools
+        #  how to install package
+        
+        pip install [--upgrade] heimdall_tools
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `heimdall_tools-0.1.1/setup.py` & `heimdall_tools-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 packs= find_packages()
 print(packs)
 
 setup(
     name='heimdall_tools',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     #packages=['heimdall_tools'],
     install_requires=[
         'boto3',
         'mysql-connector-python',
         # Add any other dependencies here
     ],
```

