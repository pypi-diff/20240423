# Comparing `tmp/testsolar-testtool-sdk-py2-0.1.6.tar.gz` & `tmp/testsolar-testtool-sdk-py2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.6.tar", last modified: Thu Apr 18 11:39:34 2024, max compression
+gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.7.tar", last modified: Tue Apr 23 07:00:08 2024, max compression
```

## Comparing `testsolar-testtool-sdk-py2-0.1.6.tar` & `testsolar-testtool-sdk-py2-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/setup.py
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/
--rw-r--r--   0 root         (0) root         (0)     2327 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/reporter.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/pipe_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/decoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/tests/
--rw-r--r--   0 root         (0) root         (0)      493 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/tests/test_param.py
--rw-r--r--   0 root         (0) root         (0)      219 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/tests/test_decoder.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5965 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/tests/test_report.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-18 11:39:27.000000 testsolar-testtool-sdk-py2-0.1.6/tests/test_testresult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      714 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-18 11:39:34.000000 testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/
+-rw-r--r--   0 root         (0) root         (0)     2327 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/reporter.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/pipe_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/decoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/tests/
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_param.py
+-rw-r--r--   0 root         (0) root         (0)      219 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_decoder.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-04-23 07:00:02.000000 testsolar-testtool-sdk-py2-0.1.7/tests/test_testresult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      714 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 07:00:08.000000 testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/requires.txt
```

### Comparing `testsolar-testtool-sdk-py2-0.1.6/setup.py` & `testsolar-testtool-sdk-py2-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(req_file, 'r') as f:
         install_requires = [str(req) for req in parse_requirements(f)]
         return install_requires
 
 
 setup(
     name='testsolar-testtool-sdk-py2',
-    version='0.1.6',
+    version='0.1.7',
     author='asiazhang',
     author_email='asiazhang2002@gmail.com',
     description='Python2 SDK for TestSolar testtool',
     url='https://github.com/OpenTestSolar/testtool-sdk-python-py2',
     packages=find_packages(),
     python_requires='>=2.7, <3',
     classifiers=[
```

### Comparing `testsolar-testtool-sdk-py2-0.1.6/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/encoder.py` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/encoder.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/testresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         self.Url = url
         self.AttachmentType = attachment_type
 
 
 class TestCaseLog:
     __test__ = False
 
-    def __init__(self, time, level, content, assert_error, runtime_error, attachments):
-        # type: (datetime, LogLevel, str, Optional[TestCaseAssertError], Optional[TestCaseRuntimeError], List[Attachment]) -> None
+    def __init__(self, time, level, content, assert_error=None, runtime_error=None, attachments=None):
+        # type: (datetime, LogLevel, str, Optional[TestCaseAssertError], Optional[TestCaseRuntimeError], Optional[List[Attachment]]) -> None
         self.Time = time
         self.Level = level
         self.Content = content
         self.AssertError = assert_error
         self.RuntimeError = runtime_error
         self.Attachments = attachments
 
@@ -88,16 +88,16 @@
         self.EndTime = end_time
         self.Logs = logs
 
 
 class TestResult:
     __test__ = False
 
-    def __init__(self, test, start_time, result_type, message, end_time, steps):
-        # type: (TestCase, datetime, ResultType, str, Optional[datetime], List[TestCaseStep]) -> None
+    def __init__(self, test, start_time, result_type, message, end_time=None, steps=None):
+        # type: (TestCase, datetime, ResultType, str, Optional[datetime], Optional[List[TestCaseStep]]) -> None
         self.Test = test
         self.StartTime = start_time
         self.ResultType = result_type
         self.Message = message
         self.EndTime = end_time
         self.Steps = steps
```

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk/model/param.py` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk/model/param.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/tests/test_report.py` & `testsolar-testtool-sdk-py2-0.1.7/tests/test_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from testsolar_testtool_sdk.reporter import Reporter, convert_to_json
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 def get_random_unicode(length):
-    # type: (int) -> unicode
+    # type: (int) -> str
     return "文件不存在:파일 つかりません"
 
 
 def generate_demo_load_result():
     # type: () -> LoadResult
     r = LoadResult([], [])  # type: LoadResult
```

### Comparing `testsolar-testtool-sdk-py2-0.1.6/tests/test_testresult.py` & `testsolar-testtool-sdk-py2-0.1.7/tests/test_testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.6/testsolar_testtool_sdk_py2.egg-info/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.7/testsolar_testtool_sdk_py2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

