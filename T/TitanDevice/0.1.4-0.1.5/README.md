# Comparing `tmp/TitanDevice-0.1.4.tar.gz` & `tmp/TitanDevice-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.4.tar", last modified: Tue Apr 23 09:02:34 2024, max compression
+gzip compressed data, was "TitanDevice-0.1.5.tar", last modified: Tue Apr 23 09:46:29 2024, max compression
```

## Comparing `TitanDevice-0.1.4.tar` & `TitanDevice-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:02:34.309606 TitanDevice-0.1.4/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:02:34.305606 TitanDevice-0.1.4/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.4/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:02:34.305606 TitanDevice-0.1.4/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:02:34.000000 TitanDevice-0.1.4/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      315 2024-04-23 09:02:34.000000 TitanDevice-0.1.4/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 09:02:34.000000 TitanDevice-0.1.4/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 09:02:34.000000 TitanDevice-0.1.4/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 09:02:34.000000 TitanDevice-0.1.4/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 09:02:34.309606 TitanDevice-0.1.4/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 09:02:32.000000 TitanDevice-0.1.4/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:02:34.305606 TitanDevice-0.1.4/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      915 2024-04-23 08:15:59.000000 TitanDevice-0.1.4/tests/test__device_manager.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:02:34.305606 TitanDevice-0.1.4/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      118 2024-04-23 08:20:14.000000 TitanDevice-0.1.4/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.4/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1065 2024-04-23 09:02:32.000000 TitanDevice-0.1.4/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      127 2024-04-23 08:57:14.000000 TitanDevice-0.1.4/titan/device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:46:29.786480 TitanDevice-0.1.5/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:46:29.786480 TitanDevice-0.1.5/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.5/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:46:29.786480 TitanDevice-0.1.5/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:46:29.000000 TitanDevice-0.1.5/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 09:46:29.000000 TitanDevice-0.1.5/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 09:46:29.000000 TitanDevice-0.1.5/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 09:46:29.000000 TitanDevice-0.1.5/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 09:46:29.000000 TitanDevice-0.1.5/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 09:46:29.786480 TitanDevice-0.1.5/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 09:35:09.000000 TitanDevice-0.1.5/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:46:29.786480 TitanDevice-0.1.5/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      977 2024-04-23 09:46:26.000000 TitanDevice-0.1.5/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.5/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1783 2024-04-23 09:32:44.000000 TitanDevice-0.1.5/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      217 2024-04-23 09:14:41.000000 TitanDevice-0.1.5/titan/_device_models.py
```

### Comparing `TitanDevice-0.1.4/PKG-INFO` & `TitanDevice-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.4/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.1.5/TitanDevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.4/setup.py` & `TitanDevice-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.4",
+    version="0.1.5",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.1.4/titan/_device_manager.py` & `TitanDevice-0.1.5/titan/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from adbutils import adb
+from typing import overload
 
-from titan._device_exception import DeviceNoFoundException
-from titan.device_models import DeviceInfo
+from titan._device_manager import _DeviceManager
+from titan._device_models import DeviceInfo, FridaInfo
 
+device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
-class _DeviceManager(object):
-    _device: adb.device
-    _device_info: DeviceInfo = None
-
-    def __init__(self, device_serial: str):
-        if device_serial not in [device.serial for device in adb.device_list()]:
-            raise DeviceNoFoundException(device_serial)
-        self._device = adb.device(device_serial)
-
-    def get_info(self) -> DeviceInfo:
-        if self._device_info is None:
-            self._device_info = DeviceInfo(
-                serial=self._device.serial,
-                product=self._device.prop.name,
-                model=self._device.prop.model,
-                device=self._device.prop.device
-            )
-        return self._device_info
-
-    @staticmethod
-    def get_all_devices():
-        device_manager_list = [
-            _DeviceManager(device.serial)
-            for device in adb.device_list()
-        ]
-        return [device_manager.get_info() for device_manager in device_manager_list]
+
+def get_all_devices() -> list[DeviceInfo]:
+    return [device.get_info() for device in device_manager_list]
+
+
+@overload
+def get_frida_info(device_serial: str) -> FridaInfo:
+    return next(
+        filter(
+            lambda device: device.get_info().serial == device_serial,
+            device_manager_list
+        )
+    ).get_frida_info()
+
+
+@overload
+def get_frida_info(device_manager: _DeviceManager) -> FridaInfo:
+    return device_manager.get_frida_info()
+
+
+def get_frida_info(device: [str | _DeviceManager]) -> FridaInfo:
+    if isinstance(device, str):
+        return get_frida_info(device)
+    elif isinstance(device, _DeviceManager):
+        return get_frida_info(device)
+    else:
+        raise TypeError(f"Unsupported type: {type(device)}")
```
