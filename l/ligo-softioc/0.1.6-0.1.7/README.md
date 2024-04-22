# Comparing `tmp/ligo_softioc-0.1.6.tar.gz` & `tmp/ligo_softioc-0.1.7.tar.gz`

## Comparing `ligo_softioc-0.1.6.tar` & `ligo_softioc-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/setup.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/examples/active.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/examples/alarm.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/examples/passive.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/examples/rename.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/print_ini
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/alarm.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/alarm_family.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/load_ioc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/py.typed
--rw-r--r--   0        0        0    23195 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/soft_ioc.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/sorted_dict.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/src/ligo_softioc/util.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/tests/alarm.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/tests/rename.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/tests/test_load_ioc.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/.gitignore
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/COPYING
--rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/LICENSE
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 ligo_softioc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/setup.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/examples/active.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/examples/alarm.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/examples/passive.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/examples/rename.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/print_ini
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/alarm.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/alarm_family.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/load_ioc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/py.typed
+-rw-r--r--   0        0        0    23195 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/soft_ioc.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/sorted_dict.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/src/ligo_softioc/util.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/tests/alarm.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/tests/rename.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/tests/test_load_ioc.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/COPYING
+-rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/LICENSE
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 ligo_softioc-0.1.7/PKG-INFO
```

### Comparing `ligo_softioc-0.1.6/examples/active.py` & `ligo_softioc-0.1.7/examples/active.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/examples/alarm.py` & `ligo_softioc-0.1.7/examples/alarm.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/examples/passive.py` & `ligo_softioc-0.1.7/examples/passive.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/examples/rename.py` & `ligo_softioc-0.1.7/examples/rename.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/alarm.py` & `ligo_softioc-0.1.7/src/ligo_softioc/alarm.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/alarm_family.py` & `ligo_softioc-0.1.7/src/ligo_softioc/alarm_family.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/load_ioc.py` & `ligo_softioc-0.1.7/src/ligo_softioc/load_ioc.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from importlib.util import spec_from_file_location, module_from_spec
 import os.path as path
 from inspect import signature
 
 if TYPE_CHECKING:
     from .soft_ioc import SoftIOC
 
+
 def load_ioc_commandline(parser: Optional[ArgumentParser]=None,
                          commandline_args: Optional[List[str]]=None) -> "SoftIOC":
     """
     :param parser: if None, create new parser
     :param commandline_args: if None, use sys.argv.  A zeroeth value is added automatically when not None.
     :return:
     """
@@ -50,14 +51,20 @@
 
     return load_ioc(args.ioc_path, args.build_function, right)
 
 
 def load_ioc(mod_fname: str, func_name: str, args: List[str]) -> "SoftIOC":
     if not path.exists(mod_fname):
         raise ModuleNotFoundError(f"{mod_fname} doesn't exist")
+    try:
+        abs_path = path.abspath(mod_fname)
+        script_dir = path.dirname(abs_path)
+        sys.path.append(script_dir)
+    except Exception:
+        pass
     ioc_spec = spec_from_file_location("ioc", mod_fname)
     if ioc_spec is None:
         raise ModuleNotFoundError(f"Couldn't load a module from {mod_fname}.")
     ioc_mod = module_from_spec(ioc_spec)
     if ioc_mod.__loader__ is not None:
         ioc_mod.__loader__.exec_module(ioc_mod)
     else:
```

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/soft_ioc.py` & `ligo_softioc-0.1.7/src/ligo_softioc/soft_ioc.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/sorted_dict.py` & `ligo_softioc-0.1.7/src/ligo_softioc/sorted_dict.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/src/ligo_softioc/util.py` & `ligo_softioc-0.1.7/src/ligo_softioc/util.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/tests/alarm.py` & `ligo_softioc-0.1.7/tests/rename.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 X1:IOC-HOSTNAME
 X1:IOC-PROCESS
 X1:IOC-ERROR_MESSAGE
 X1:IOC-ERROR_GPS
 X1:IOC-ERROR_TIMESTAMP
 """
 
-from ligo_softioc import SoftIOC, Alarm
+from ligo_softioc import SoftIOC
 import sys
 
 process_count = 0
 
 def process(ioc: SoftIOC, gps_time_sec: int) -> None:
     """
     Update the custom channels.
@@ -60,42 +60,42 @@
     :return:
     """
 
     # setup the ioc with a channel prefix.
     # the ioc will by default run process() about 10 times per second
     ioc = SoftIOC(
         prefix="X1:IOC-",
-        process_func=process)
+        process_func=process,
+        ioc_chan_prefix="FOO_",
+        custom_channel_names={
+            "START_GPS": "START_TIME_X",
+            "UPTIME_SEC": "UPTIME_Y",
+            "NOT_A_CHANNEL": "SHOULD_NEVER_APPEAR",  # generates a warning because not used.
+            # "FOO_UPTIME_Y": "UPTIME_Z",  # should throw value error exception
+        }
+    )
 
     # add in some channels
 
     channels = {
         "INPUT": {'prec': 3},
         "SQUARED_OUTPUT": {'prec': 3},
     }
 
     ioc.add_channels(channels)
 
     ioc.add_channel("PROCESS_COUNT", {'type': 'int'})
 
-    alarm = Alarm("test_alarm", "Test alarm triggered", lambda: ioc.getParam("SQUARED_OUTPUT") >= 100,
-                  pv="SQUARED_OUTPUT"
-                  )
-
-    ioc.add(alarm)
-
     # call this when all channels are added.
     # and before you try to set the value of any channel
     ioc.finalize_channels()
 
     # setup the input varible so we know how it'll start
     ioc.setParam("INPUT", 0)
 
-
-
     return ioc
 
 
 if __name__ == "__main__":
 
     ioc = build_ioc()
```

### Comparing `ligo_softioc-0.1.6/tests/rename.py` & `ligo_softioc-0.1.7/tests/alarm.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,82 +19,85 @@
 X1:IOC-HOSTNAME
 X1:IOC-PROCESS
 X1:IOC-ERROR_MESSAGE
 X1:IOC-ERROR_GPS
 X1:IOC-ERROR_TIMESTAMP
 """
 
-from ligo_softioc import SoftIOC
+from ligo_softioc import SoftIOC, Alarm
 import sys
 
 process_count = 0
 
+current_input = 0
+
 def process(ioc: SoftIOC, gps_time_sec: int) -> None:
     """
     Update the custom channels.
 
     Auto-generated channels are auto-updated.
     :param ioc:
     :param gps_time_sec:
     :return:
     """
-    global process_count
+    global process_count, current_input
     process_count += 1
 
     # Read the input - change this value with caput
     in_val = ioc.getParam("INPUT")
 
     # square INPUT and write it to SQUARED_OUTPUT
-    ioc.setParam("SQUARED_OUTPUT", in_val ** 2)
+    if in_val != current_input:
+        current_input = in_val
+        ioc.setParam("SQUARED_OUTPUT", in_val ** 2)
 
     # set to how many times process() has run
     ioc.setParam("PROCESS_COUNT", process_count)
 
 
 def build_ioc() -> SoftIOC:
     """
     Build a new SoftIOC that's completely ready to run
 
     Separate the ioc build from 'if __name__ == "__main__"'
     so that halper scripts can load the IOC and create the object
     to interrogate it.
     :return:
     """
+    global current_input
 
     # setup the ioc with a channel prefix.
     # the ioc will by default run process() about 10 times per second
     ioc = SoftIOC(
         prefix="X1:IOC-",
-        process_func=process,
-        ioc_chan_prefix="FOO_",
-        custom_channel_names={
-            "START_GPS": "START_TIME_X",
-            "UPTIME_SEC": "UPTIME_Y",
-            "NOT_A_CHANNEL": "SHOULD_NEVER_APPEAR",  # generates a warning because not used.
-            # "FOO_UPTIME_Y": "UPTIME_Z",  # should throw value error exception
-        }
-    )
+        process_func=process)
 
     # add in some channels
 
     channels = {
         "INPUT": {'prec': 3},
         "SQUARED_OUTPUT": {'prec': 3},
     }
 
     ioc.add_channels(channels)
 
     ioc.add_channel("PROCESS_COUNT", {'type': 'int'})
 
+    alarm = Alarm("test_alarm", "Test alarm triggered", lambda: ioc.getParam("SQUARED_OUTPUT") >= 100,
+                  pv="SQUARED_OUTPUT"
+                  )
+
+    ioc.add(alarm)
+
     # call this when all channels are added.
     # and before you try to set the value of any channel
     ioc.finalize_channels()
 
     # setup the input varible so we know how it'll start
-    ioc.setParam("INPUT", 0)
+    ioc.setParam("INPUT", current_input)
 
     return ioc
 
 
 if __name__ == "__main__":
 
     ioc = build_ioc()
```

### Comparing `ligo_softioc-0.1.6/tests/test_load_ioc.py` & `ligo_softioc-0.1.7/tests/test_load_ioc.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/COPYING` & `ligo_softioc-0.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/LICENSE` & `ligo_softioc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/README.md` & `ligo_softioc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/pyproject.toml` & `ligo_softioc-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.6/PKG-INFO` & `ligo_softioc-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ligo-softioc
-Version: 0.1.6
+Version: 0.1.7
 Summary: Support library for writing EPICS SoftIOCs in Python.
 Project-URL: Homepage, https://git.ligo.org/cds/admin/softioc
 Project-URL: Issues, https://git.ligo.org/cds/admin/softioc/-/issues
 Author-email: Erik von Reis <evonreis@caltech.edu>
 License-File: COPYING
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

