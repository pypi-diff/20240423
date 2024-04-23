# Comparing `tmp/pytest_embedded_serial-1.8.3.tar.gz` & `tmp/pytest_embedded_serial-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_serial-1.8.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_serial-1.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_serial-1.8.3.tar` & `pytest_embedded_serial-1.8.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/LICENSE
--rw-r--r--   0        0        0      195 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/README.md
--rw-r--r--   0        0        0     3293 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/pyproject.toml
--rw-r--r--   0        0        0      176 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/pytest_embedded_serial/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/pytest_embedded_serial/dut.py
--rw-r--r--   0        0        0     6184 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/pytest_embedded_serial/serial.py
--rw-r--r--   0        0        0     1653 2024-04-09 09:44:39.840723 pytest_embedded_serial-1.8.3/tests/test_serial.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/LICENSE
+-rw-r--r--   0        0        0      195 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/README.md
+-rw-r--r--   0        0        0     3293 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0      176 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/pytest_embedded_serial/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/pytest_embedded_serial/dut.py
+-rw-r--r--   0        0        0     6184 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/pytest_embedded_serial/serial.py
+-rw-r--r--   0        0        0     1653 2024-04-23 07:21:22.781428 pytest_embedded_serial-1.8.4/tests/test_serial.py
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.8.4/PKG-INFO
```

### Comparing `pytest_embedded_serial-1.8.3/LICENSE` & `pytest_embedded_serial-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.3/pyproject.toml` & `pytest_embedded_serial-1.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.3",
+    "pytest-embedded~=1.8.4",
     "pyserial~=3.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
```

### Comparing `pytest_embedded_serial-1.8.3/pytest_embedded_serial/dut.py` & `pytest_embedded_serial-1.8.4/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.3/pytest_embedded_serial/serial.py` & `pytest_embedded_serial-1.8.4/pytest_embedded_serial/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.3/tests/test_serial.py` & `pytest_embedded_serial-1.8.4/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.3/PKG-INFO` & `pytest_embedded_serial-1.8.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-serial
-Version: 1.8.3
+Version: 1.8.4
 Summary: Make pytest-embedded plugin work with Serial.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.3
+Requires-Dist: pytest-embedded~=1.8.4
 Requires-Dist: pyserial~=3.0
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-serial
```
