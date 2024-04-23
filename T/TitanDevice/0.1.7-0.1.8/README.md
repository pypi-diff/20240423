# Comparing `tmp/TitanDevice-0.1.7.tar.gz` & `tmp/TitanDevice-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.7.tar", last modified: Tue Apr 23 10:13:28 2024, max compression
+gzip compressed data, was "TitanDevice-0.1.8.tar", last modified: Tue Apr 23 10:20:27 2024, max compression
```

## Comparing `TitanDevice-0.1.7.tar` & `TitanDevice-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.7/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.610948 TitanDevice-0.1.7/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:13:25.000000 TitanDevice-0.1.7/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      704 2024-04-23 10:13:25.000000 TitanDevice-0.1.7/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.7/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1783 2024-04-23 09:32:44.000000 TitanDevice-0.1.7/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      217 2024-04-23 09:14:41.000000 TitanDevice-0.1.7/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:20:27.054749 TitanDevice-0.1.8/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:20:27.054749 TitanDevice-0.1.8/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.8/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:20:27.054749 TitanDevice-0.1.8/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:20:27.000000 TitanDevice-0.1.8/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:20:27.000000 TitanDevice-0.1.8/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:20:27.000000 TitanDevice-0.1.8/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:20:27.000000 TitanDevice-0.1.8/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:20:27.000000 TitanDevice-0.1.8/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:20:27.054749 TitanDevice-0.1.8/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:20:25.000000 TitanDevice-0.1.8/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:20:27.054749 TitanDevice-0.1.8/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      704 2024-04-23 10:13:25.000000 TitanDevice-0.1.8/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.8/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1909 2024-04-23 10:20:25.000000 TitanDevice-0.1.8/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      224 2024-04-23 10:20:25.000000 TitanDevice-0.1.8/titan/_device_models.py
```

### Comparing `TitanDevice-0.1.7/PKG-INFO` & `TitanDevice-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.7/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.1.8/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.7/setup.py` & `TitanDevice-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.7",
+    version="0.1.8",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.1.7/titan/__init__.py` & `TitanDevice-0.1.8/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.1.7/titan/_device_manager.py` & `TitanDevice-0.1.8/titan/_device_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,13 +40,17 @@
             )
         return self._frida_info
 
     def __is_frida_running(self) -> bool:
         return self._device.shell("pgrep frida-server").strip() != ""
 
     def __is_frida_installed(self) -> bool:
-        return self._device.shell("su -c ls /data/local/tmp/frida-server").strip() != ""
+        return 'No such file or directory' not in self._device.shell(
+            "su -c ls /data/local/tmp/frida-server"
+        ).strip()
 
-    def __get_frida_version(self) -> str:
+    def __get_frida_version(self) -> str | None:
+        if not self.__is_frida_installed():
+            return None
         return self._device.shell(
             "su -c /data/local/tmp/frida-server --version"
         ).strip()
```

