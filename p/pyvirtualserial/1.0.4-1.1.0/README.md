# Comparing `tmp/pyvirtualserial-1.0.4.tar.gz` & `tmp/pyvirtualserial-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvirtualserial-1.0.4.tar", last modified: Wed Apr 10 18:07:12 2024, max compression
+gzip compressed data, was "pyvirtualserial-1.1.0.tar", last modified: Tue Apr 23 16:28:20 2024, max compression
```

## Comparing `pyvirtualserial-1.0.4.tar` & `pyvirtualserial-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.817884 pyvirtualserial-1.0.4/
--rw-rw-rw-   0        0        0      626 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.coveragerc
--rw-rw-rw-   0        0        0      620 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.gitignore
--rw-rw-rw-   0        0        0      557 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.readthedocs.yml
--rw-rw-rw-   0        0        0       85 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0       82 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14271 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1102 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3182 2024-04-10 18:07:12.817884 pyvirtualserial-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.804741 pyvirtualserial-1.0.4/docs/
--rw-rw-rw-   0        0        0     1183 2024-03-10 01:05:44.000000 pyvirtualserial-1.0.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.804741 pyvirtualserial-1.0.4/docs/_static/
--rw-rw-rw-   0        0        0       19 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/changelog.rst
--rw-rw-rw-   0        0        0    10136 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/contributing.rst
--rw-rw-rw-   0        0        0     1473 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/index.rst
--rw-rw-rw-   0        0        0       74 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/license.rst
--rw-rw-rw-   0        0        0       41 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/readme.rst
--rw-rw-rw-   0        0        0      509 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/requirements.txt
--rw-rw-rw-   0        0        0      355 2024-03-10 02:33:30.000000 pyvirtualserial-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       57 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/requirements.in
--rw-rw-rw-   0        0        0      411 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0     1381 2024-04-10 18:07:12.818884 pyvirtualserial-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-03-10 02:33:35.000000 pyvirtualserial-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.781946 pyvirtualserial-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.805742 pyvirtualserial-1.0.4/src/pyvirtualserial/
--rw-rw-rw-   0        0        0      851 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.814829 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/
--rw-rw-rw-   0        0        0     3137 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/linux_virtual_serial.py
--rw-rw-rw-   0        0        0     4096 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/window_virtual_serial.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.815828 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/
--rw-rw-rw-   0        0        0     1489 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/com0com.py
--rw-rw-rw-   0        0        0      480 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/context_managers.py
--rw-rw-rw-   0        0        0     1759 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/virtual_serial.py
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.816885 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/
--rw-rw-rw-   0        0        0     3182 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      887 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.815828 pyvirtualserial-1.0.4/tests/
--rw-rw-rw-   0        0        0       86 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/tests/conftest.py
--rw-rw-rw-   0        0        0     2944 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:20.005868 pyvirtualserial-1.1.0/
+-rw-rw-rw-   0        0        0      626 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/.coveragerc
+-rw-rw-rw-   0        0        0      620 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0      557 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0       85 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0       82 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14271 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1102 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3182 2024-04-23 16:28:20.005868 pyvirtualserial-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:19.989210 pyvirtualserial-1.1.0/docs/
+-rw-rw-rw-   0        0        0     1183 2024-03-10 01:05:44.000000 pyvirtualserial-1.1.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:19.989210 pyvirtualserial-1.1.0/docs/_static/
+-rw-rw-rw-   0        0        0       19 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0       43 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10136 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1473 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/license.rst
+-rw-rw-rw-   0        0        0       41 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/docs/readme.rst
+-rw-rw-rw-   0        0        0      509 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/docs/requirements.txt
+-rw-rw-rw-   0        0        0      355 2024-03-10 02:33:30.000000 pyvirtualserial-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/requirements.in
+-rw-rw-rw-   0        0        0      411 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0     1381 2024-04-23 16:28:20.007867 pyvirtualserial-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-03-10 02:33:35.000000 pyvirtualserial-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:19.965334 pyvirtualserial-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:19.991364 pyvirtualserial-1.1.0/src/pyvirtualserial/
+-rw-rw-rw-   0        0        0      851 2024-04-10 18:03:25.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:20.002868 pyvirtualserial-1.1.0/src/pyvirtualserial/bases/
+-rw-rw-rw-   0        0        0     3196 2024-04-23 16:27:27.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/bases/linux_virtual_serial.py
+-rw-rw-rw-   0        0        0     4096 2024-04-10 18:03:25.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/bases/window_virtual_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:20.003868 pyvirtualserial-1.1.0/src/pyvirtualserial/utils/
+-rw-rw-rw-   0        0        0     1489 2024-04-10 18:03:25.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/utils/com0com.py
+-rw-rw-rw-   0        0        0      480 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/utils/context_managers.py
+-rw-rw-rw-   0        0        0     1759 2024-04-10 18:03:25.000000 pyvirtualserial-1.1.0/src/pyvirtualserial/virtual_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:20.004867 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/
+-rw-rw-rw-   0        0        0     3182 2024-04-23 16:28:19.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-04-23 16:28:19.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:28:19.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 18:07:12.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2024-04-23 16:28:19.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 16:28:19.000000 pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 16:28:20.003868 pyvirtualserial-1.1.0/tests/
+-rw-rw-rw-   0        0        0       86 2024-03-10 02:25:56.000000 pyvirtualserial-1.1.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     2944 2024-02-29 19:28:26.000000 pyvirtualserial-1.1.0/tox.ini
```

### Comparing `pyvirtualserial-1.0.4/.coveragerc` & `pyvirtualserial-1.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/.gitignore` & `pyvirtualserial-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/.readthedocs.yml` & `pyvirtualserial-1.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/CONTRIBUTING.rst` & `pyvirtualserial-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/LICENSE.txt` & `pyvirtualserial-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/PKG-INFO` & `pyvirtualserial-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvirtualserial
-Version: 1.0.4
+Version: 1.1.0
 Summary: Library to create virtual serial ports on Windows and Linux.
 Home-page: https://github.com/byrondelgithub/PyVirtualSerial
 Author: byrondelgithub
 Author-email: rhurtado5c@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/byrondelgithub/PyVirtualSerial
```

### Comparing `pyvirtualserial-1.0.4/README.rst` & `pyvirtualserial-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/docs/Makefile` & `pyvirtualserial-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/docs/conf.py` & `pyvirtualserial-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/docs/index.rst` & `pyvirtualserial-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/setup.cfg` & `pyvirtualserial-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/setup.py` & `pyvirtualserial-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial/__init__.py` & `pyvirtualserial-1.1.0/src/pyvirtualserial/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial/bases/linux_virtual_serial.py` & `pyvirtualserial-1.1.0/src/pyvirtualserial/bases/linux_virtual_serial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 File with the base of a Virtual Serial for Linux that uses pty and tty
 
 References:
     - https://docs.python.org/es/3/library/tty.html
     - https://docs.python.org/es/3.10/library/pty.html
 """
+
 import os
 import time
 from select import select
 
 if os.name == "posix":
     import os, pty, tty, termios
 from loguru import logger
@@ -23,15 +24,15 @@
     Base class for Virtual Serials in linux that uses the tool pty to create a
     master file and slave serial.
 
     The master file is used to communicate with the user, anything sent to the master
     will be also sent to the slave and viceversa.
     """
 
-    def __init__(self, timeout = 5, *args, **kwargs) -> None:
+    def __init__(self, timeout=5, *args, **kwargs) -> None:
         """
         Linux virtual serials dont need baudrate, ports or timeout.
         To access the slave port name please use the function :func:`get_slave_name`
         """
         self._timeout: int = timeout
         self._master: int = None
         self._slave: int = None
@@ -56,29 +57,31 @@
                 break
         logger.debug(f"Reading {b}")
         return b
 
     def read_until(self, expected) -> bytes:
         b = b""
         s_time = time.time()
-        while b[-len(expected):] != expected and time.time() - s_time < self._timeout:
+        while b[-len(expected) :] != expected:
+            if self._timeout is not None and time.time() - s_time >= self._timeout:
+                break
             b += self.read(1)
         logger.debug(f"Reading {b}")
         return b
-    
+
     def readline(self) -> bytes:
         line = self.read_until(b"\n")
         logger.debug(f"Reading line {line}")
         return line
 
     def readlines(self) -> list[bytes]:
         lines = self._reader.readlines()
         logger.debug(f"Reading lines {lines}")
         return lines
-    
+
     def read_all(self) -> bytes:
         response = b""
         rlist, _, _ = select([self._reader], [], [], 0)
         if rlist:
             response = self._reader.read1()
         logger.debug(f"Reading all {response}")
         return response
@@ -91,11 +94,11 @@
             str: Name of the slave serial port
         """
         return os.ttyname(self._slave)
 
     @property
     def timeout(self) -> int:
         return self._timeout
-    
+
     @timeout.setter
-    def timeout(self, timeout:int) -> None:
-        self._timeout = timeout
+    def timeout(self, timeout: int) -> None:
+        self._timeout = timeout
```

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial/bases/window_virtual_serial.py` & `pyvirtualserial-1.1.0/src/pyvirtualserial/bases/window_virtual_serial.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial/utils/com0com.py` & `pyvirtualserial-1.1.0/src/pyvirtualserial/utils/com0com.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial/virtual_serial.py` & `pyvirtualserial-1.1.0/src/pyvirtualserial/virtual_serial.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/PKG-INFO` & `pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvirtualserial
-Version: 1.0.4
+Version: 1.1.0
 Summary: Library to create virtual serial ports on Windows and Linux.
 Home-page: https://github.com/byrondelgithub/PyVirtualSerial
 Author: byrondelgithub
 Author-email: rhurtado5c@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/byrondelgithub/PyVirtualSerial
```

### Comparing `pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/SOURCES.txt` & `pyvirtualserial-1.1.0/src/pyvirtualserial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.4/tox.ini` & `pyvirtualserial-1.1.0/tox.ini`

 * *Files identical despite different names*

