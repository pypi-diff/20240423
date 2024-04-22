# Comparing `tmp/pyunfoldedcircleremote-0.7.0.tar.gz` & `tmp/pyunfoldedcircleremote-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunfoldedcircleremote-0.7.0.tar", max compression
+gzip compressed data, was "pyunfoldedcircleremote-0.7.1.tar", max compression
```

## Comparing `pyunfoldedcircleremote-0.7.0.tar` & `pyunfoldedcircleremote-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.7.0/LICENSE
--rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.7.0/README.md
--rw-r--r--   0        0        0      604 2024-04-21 20:44:46.839229 pyunfoldedcircleremote-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/__init__.py
--rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/const.py
--rw-r--r--   0        0        0    66094 2024-04-21 21:46:23.254016 pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/remote.py
--rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/remote_websocket.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.7.1/LICENSE
+-rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.7.1/README.md
+-rw-r--r--   0        0        0      604 2024-04-22 22:12:00.976251 pyunfoldedcircleremote-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/__init__.py
+-rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/const.py
+-rw-r--r--   0        0        0    66147 2024-04-22 22:12:06.194670 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote.py
+-rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote_websocket.py
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.7.1/PKG-INFO
```

### Comparing `pyunfoldedcircleremote-0.7.0/LICENSE` & `pyunfoldedcircleremote-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.0/pyproject.toml` & `pyunfoldedcircleremote-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUnfoldedCircleRemote"
-version = "0.7.0"
+version = "0.7.1"
 description = "A python library to interact with the Unfolded Circle Remote"
 authors = ["Jack Powell <jackjpowell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jackjpowell/py-unfolded-circle"
 packages = [{include = "pyUnfoldedCircleRemote", from = "src"}]
```

### Comparing `pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/const.py` & `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/const.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/remote.py` & `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1065,14 +1065,15 @@
                         # The offset as a percent to adjust step percentage by
                         percentage_offset = offset / 100
                     match update_state:
                         case "START":
                             self._update_percent = 0
                         case "RUN":
                             current_step = progress.get("current_step")
+                            self._update_percent = 0
                         case "PROGRESS":
                             step_offset = offset * (current_step - 1)
                             self._update_percent = (
                                 percentage_offset * progress.get("current_percent")
                             ) + step_offset
                         case "SUCCESS":
                             self._update_percent = 100
```

### Comparing `pyunfoldedcircleremote-0.7.0/src/pyUnfoldedCircleRemote/remote_websocket.py` & `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote_websocket.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.0/PKG-INFO` & `pyunfoldedcircleremote-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUnfoldedCircleRemote
-Version: 0.7.0
+Version: 0.7.1
 Summary: A python library to interact with the Unfolded Circle Remote
 Home-page: https://github.com/jackjpowell/py-unfolded-circle
 License: MIT
 Author: Jack Powell
 Author-email: jackjpowell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

