# Comparing `tmp/aws_textract_pipeline-0.2.1.tar.gz` & `tmp/aws_textract_pipeline-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_textract_pipeline-0.2.1.tar", last modified: Sun Apr 21 20:55:09 2024, max compression
+gzip compressed data, was "aws_textract_pipeline-0.3.1.tar", last modified: Tue Apr 23 15:19:48 2024, max compression
```

## Comparing `aws_textract_pipeline-0.2.1.tar` & `aws_textract_pipeline-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.669847 aws_textract_pipeline-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      368 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5962 2024-04-21 20:55:09.669608 aws_textract_pipeline-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3728 2024-04-21 20:51:13.000000 aws_textract_pipeline-0.2.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.665689 aws_textract_pipeline-0.2.1/aws_textract_pipeline/
--rw-r--r--   0 sanhehu    (501) staff       (20)      331 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2024-04-21 20:53:35.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      766 2024-04-21 20:04:18.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4328 2024-04-21 14:35:20.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/doc_type.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.666570 aws_textract_pipeline-0.2.1/aws_textract_pipeline/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4545 2024-04-21 20:14:36.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/landing.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-04-20 15:07:38.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2555 2024-04-21 14:45:56.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/segment.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    33401 2024-04-21 20:27:24.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/tracker.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.667511 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7191 2024-04-17 20:40:30.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/better_dataclasses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5196 2024-04-17 20:40:50.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7575 2024-04-17 20:39:26.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2556 2024-04-18 13:51:22.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    21876 2024-04-20 15:07:08.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/nested_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3040 2024-04-19 20:32:58.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline/workspace.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.668463 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5962 2024-04-21 20:55:09.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1254 2024-04-21 20:55:09.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-04-21 20:55:09.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      485 2024-04-21 20:55:09.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2024-04-21 20:55:09.000000 aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1496 2024-04-21 20:54:46.000000 aws_textract_pipeline-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.2.1/requirements-furo-sphinx-search.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      203 2024-04-18 13:52:29.000000 aws_textract_pipeline-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      285 2024-04-21 20:33:57.000000 aws_textract_pipeline-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-04-21 20:55:09.669904 aws_textract_pipeline-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7655 2024-04-17 19:46:14.000000 aws_textract_pipeline-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-21 20:55:09.668274 aws_textract_pipeline-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      502 2024-04-19 17:03:57.000000 aws_textract_pipeline-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      705 2024-04-17 20:57:49.000000 aws_textract_pipeline-0.2.1/tests/test_doc_type.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1504 2024-04-21 20:14:26.000000 aws_textract_pipeline-0.2.1/tests/test_landing.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      418 2024-04-20 02:39:27.000000 aws_textract_pipeline-0.2.1/tests/test_segment.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3449 2024-04-21 20:22:15.000000 aws_textract_pipeline-0.2.1/tests/test_tracker.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1247 2024-04-19 16:43:15.000000 aws_textract_pipeline-0.2.1/tests/test_workspace.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.468687 aws_textract_pipeline-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      368 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5962 2024-04-23 15:19:48.468477 aws_textract_pipeline-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3728 2024-04-21 20:51:13.000000 aws_textract_pipeline-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.463154 aws_textract_pipeline-0.3.1/aws_textract_pipeline/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      331 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2024-04-23 15:18:38.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      893 2024-04-22 17:16:06.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4328 2024-04-21 14:35:20.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/doc_type.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.463864 aws_textract_pipeline-0.3.1/aws_textract_pipeline/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4545 2024-04-21 20:14:36.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/landing.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-04-20 15:07:38.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2555 2024-04-21 14:45:56.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/segment.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    40312 2024-04-23 15:19:29.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/tracker.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.465748 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7191 2024-04-17 20:40:30.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/better_dataclasses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5196 2024-04-17 20:40:50.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7575 2024-04-17 20:39:26.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2556 2024-04-18 13:51:22.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    21876 2024-04-20 15:07:08.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3040 2024-04-19 20:32:58.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline/workspace.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.467397 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5962 2024-04-23 15:19:48.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1254 2024-04-23 15:19:48.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-04-23 15:19:48.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      485 2024-04-23 15:19:48.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2024-04-23 15:19:48.000000 aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1966 2024-04-23 15:19:03.000000 aws_textract_pipeline-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-04-17 19:38:23.000000 aws_textract_pipeline-0.3.1/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      203 2024-04-18 13:52:29.000000 aws_textract_pipeline-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      285 2024-04-21 20:33:57.000000 aws_textract_pipeline-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-04-23 15:19:48.468735 aws_textract_pipeline-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7655 2024-04-17 19:46:14.000000 aws_textract_pipeline-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-04-23 15:19:48.467080 aws_textract_pipeline-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      502 2024-04-19 17:03:57.000000 aws_textract_pipeline-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      705 2024-04-17 20:57:49.000000 aws_textract_pipeline-0.3.1/tests/test_doc_type.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1504 2024-04-21 20:14:26.000000 aws_textract_pipeline-0.3.1/tests/test_landing.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      418 2024-04-20 02:39:27.000000 aws_textract_pipeline-0.3.1/tests/test_segment.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3449 2024-04-21 20:22:15.000000 aws_textract_pipeline-0.3.1/tests/test_tracker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1247 2024-04-19 16:43:15.000000 aws_textract_pipeline-0.3.1/tests/test_workspace.py
```

### Comparing `aws_textract_pipeline-0.2.1/AUTHORS.rst` & `aws_textract_pipeline-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/LICENSE.txt` & `aws_textract_pipeline-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/PKG-INFO` & `aws_textract_pipeline-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_textract_pipeline
-Version: 0.2.1
+Version: 0.3.1
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_textract_pipeline-project
-Download-URL: https://pypi.python.org/pypi/aws_textract_pipeline/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_textract_pipeline/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_textract_pipeline-0.2.1/README.rst` & `aws_textract_pipeline-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/api.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,11 +15,14 @@
 from .landing import LandingDocument
 from .landing import get_md5_of_bytes
 from .landing import get_tar_file_md5
 from .landing import get_doc_md5
 from .segment import SegmentPdfResult
 from .segment import segment_pdf
 from .tracker import ComponentToTextractOutputResult
+from .tracker import TextractOutputToTextAndJsonResult
 from .tracker import Component
 from .tracker import Data
+from .tracker import StepEnum
+from .tracker import MoveToNextStepResult
 from .tracker import BaseStatusAndUpdateTimeIndex
 from .tracker import BaseTracker
```

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/doc_type.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/doc_type.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/landing.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/landing.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/paths.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/paths.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/segment.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/segment.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/tracker.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/tracker.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from pathlib_mate import Path, T_PATH_ARG
 import pynamodb_mate as pm
 from s3pathlib import S3Path
 from boto_session_manager import BotoSesManager
 
 import aws_textract.api as aws_textract
+from .vendor.better_enum import BetterStrEnum
 from .vendor.better_dataclasses import DataClass
 
 from .logger import logger
 from .doc_type import DocTypeEnum, S3ContentTypeEnum
 from .landing import MetadataKeyEnum, LandingDocument, get_doc_md5
 from .segment import segment_pdf
 from .workspace import Workspace
@@ -38,14 +39,23 @@
 import json
 
 
 # ------------------------------------------------------------------------------
 # DynamoDB ORM Model
 # ------------------------------------------------------------------------------
 @dataclasses.dataclass
+class Component(DataClass):
+    """
+    Metadata for each component.
+    """
+
+    id: str = dataclasses.field()
+
+
+@dataclasses.dataclass
 class ComponentToTextractOutputResult(DataClass):
     """
     The returned object for creating textract output for all components of a
     document. This information will be used to parse the textract output data
     later.
 
     :param is_single_textract_api_call: it is more efficient to use single
@@ -89,20 +99,17 @@
                     verbose=verbose,
                 )
                 if verbose:
                     print("")
 
 
 @dataclasses.dataclass
-class Component(DataClass):
-    """
-    Metadata for each component.
-    """
-
-    id: str = dataclasses.field()
+class TextractOutputToTextAndJsonResult(DataClass):
+    text_list: T.List[str] = dataclasses.field(default_factory=list)
+    json_list: T.List[dict] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
 class Data(DataClass):
     """
     Additional data about this document.
 
@@ -194,14 +201,32 @@
     s09000_hil_output_to_hil_post_process_pending = 9000
     s09020_hil_output_to_hil_post_process_in_progress = 9020
     s09040_hil_output_to_hil_post_process_failed = 9040
     s09060_hil_output_to_hil_post_process_succeeded = 9060
     s09080_hil_output_to_hil_post_process_ignored = 9080
 
 
+class StepEnum(BetterStrEnum):
+    do_nothing = "do_nothing"
+    landing_to_raw = "landing_to_raw"
+    raw_to_component = "raw_to_component"
+    component_to_textract_output = "component_to_textract_output"
+    textract_output_to_text_and_json = "textract_output_to_text_and_json"
+
+
+@dataclasses.dataclass
+class MoveToNextStepResult(DataClass):
+    # fmt: off
+    step: str = dataclasses.field()
+    components: T.List[Component] = dataclasses.field(default_factory=list)
+    component_to_textract_output_result: T.Optional[ComponentToTextractOutputResult] = dataclasses.field(default=None)
+    textract_output_to_text_and_json_result: T.Optional[TextractOutputToTextAndJsonResult] = dataclasses.field(default=None)
+    # fmt: on
+
+
 class BaseStatusAndUpdateTimeIndex(
     pm.patterns.status_tracker.StatusAndUpdateTimeIndex,
 ):
     """
     Status Tracker GSI index, to allow lookup by status.
     """
 
@@ -451,16 +476,16 @@
         debug: bool = False,
     ):
         """
         Copy document from landing to raw.
         """
         self.check_status_range(
             valid_status=[
-                StatusEnum.s01000_landing_to_raw_pending.value,
-                StatusEnum.s01040_landing_to_raw_failed.value,
+                self.STATUS_ENUM.s01000_landing_to_raw_pending.value,
+                self.STATUS_ENUM.s01040_landing_to_raw_failed.value,
             ]
         )
         with self.start_landing_to_raw(debug=debug):
             s3path_landing = S3Path(self.data_obj.landing_uri)
             s3path_raw = workspace.get_raw_s3path(doc_id=self.doc_id)
             metadata = s3path_landing.metadata.copy()
             metadata[MetadataKeyEnum.doc_id.value] = self.doc_id
@@ -502,17 +527,17 @@
             the intermediate files
         :param clear_tmp_dir: whether to clear the temporary directory after the
             operation.
         :param debug:
         """
         self.check_status_range(
             valid_status=[
-                StatusEnum.s01060_landing_to_raw_succeeded.value,
-                StatusEnum.s02000_raw_to_component_pending.value,
-                StatusEnum.s02040_raw_to_component_failed.value,
+                self.STATUS_ENUM.s01060_landing_to_raw_succeeded.value,
+                self.STATUS_ENUM.s02000_raw_to_component_pending.value,
+                self.STATUS_ENUM.s02040_raw_to_component_failed.value,
             ]
         )
 
         tmp_dir = Path(tmp_dir)
         dir_root = tmp_dir / self.doc_id
         dir_root.mkdir(parents=True, exist_ok=True)
         s3path_raw = workspace.get_raw_s3path(doc_id=self.doc_id)
@@ -570,15 +595,15 @@
                 raise NotImplementedError
 
     def raw_to_component(
         self,
         bsm: "BotoSesManager",
         workspace: "Workspace",
         tmp_dir: T_PATH_ARG = dir_tmp,
-        clear_tmp_dir: bool = False,
+        clear_tmp_dir: bool = True,
         debug: bool = False,
     ) -> T.List[Component]:
         """
         Wrapper of the :meth:`BaseTracker._raw_to_component` method.
         """
         with logger.disabled(disable=not debug):
             return self._raw_to_component(
@@ -648,17 +673,17 @@
         debug: bool = False,
     ) -> ComponentToTextractOutputResult:  # pragma: no cover
         """
         See the :meth:`BaseTracker.component_to_textract_output` method for more details.
         """
         self.check_status_range(
             valid_status=[
-                StatusEnum.s02060_raw_to_component_succeeded.value,
-                StatusEnum.s03000_component_to_textract_output_pending.value,
-                StatusEnum.s03040_component_to_textract_output_failed.value,
+                self.STATUS_ENUM.s02060_raw_to_component_succeeded.value,
+                self.STATUS_ENUM.s03000_component_to_textract_output_pending.value,
+                self.STATUS_ENUM.s03040_component_to_textract_output_failed.value,
             ]
         )
 
         # prepare textract API arguments
         feature_types = list()
         for flag, feature in [
             (use_table_feature, "TABLES"),
@@ -781,15 +806,15 @@
     def _textract_output_to_text_and_json_helper(
         self,
         bsm: "BotoSesManager",
         workspace: "Workspace",
         job_id: str,
         comp_id: str,
         base_metadata: dict,
-    ):  # pragma: no cover
+    ) -> T.Tuple[str, dict]:  # pragma: no cover
         """
         This is a utility function to simplify the code.
         """
         base_metadata[MetadataKeyEnum.component_id.value] = comp_id
 
         # Get merged data
         res = aws_textract.better_boto.get_document_analysis(
@@ -826,70 +851,77 @@
         )
         s3path_json.write_text(
             json.dumps(res),
             bsm=bsm,
             metadata=base_metadata,
             content_type=S3ContentTypeEnum.json.value,
         )
+        return text, res
 
     @logger.start_and_end(msg="Textract Output to Text and Json")
     def _textract_output_to_text_and_json(
         self,
         bsm: "BotoSesManager",
         workspace: "Workspace",
         debug: bool = False,
-    ):  # pragma: no cover
+    ) -> TextractOutputToTextAndJsonResult:  # pragma: no cover
         """
         See :meth:`BaseTracker.textract_output_to_text_and_json` for details.
         """
         self.check_status_range(
             valid_status=[
-                StatusEnum.s03060_component_to_textract_output_succeeded.value,
-                StatusEnum.s05000_textract_output_to_text_and_json_pending.value,
-                StatusEnum.s05040_textract_output_to_text_and_json_failed.value,
+                self.STATUS_ENUM.s03060_component_to_textract_output_succeeded.value,
+                self.STATUS_ENUM.s05000_textract_output_to_text_and_json_pending.value,
+                self.STATUS_ENUM.s05040_textract_output_to_text_and_json_failed.value,
             ]
         )
 
         data_obj = self.data_obj
         component_to_textract_output_result = (
             data_obj.component_to_textract_output_result
         )
         s3path_raw = workspace.get_raw_s3path(doc_id=self.doc_id)
         metadata = s3path_raw.metadata.copy()
+        textract_output_to_text_and_json_result = TextractOutputToTextAndJsonResult()
         with self.start_textract_output_to_text_and_json(debug=debug):
             if component_to_textract_output_result.is_single_textract_api_call:
                 comp_id = _root_
                 job_id = component_to_textract_output_result.job_id
-                self._textract_output_to_text_and_json_helper(
+                text, res = self._textract_output_to_text_and_json_helper(
                     bsm=bsm,
                     workspace=workspace,
                     job_id=job_id,
                     comp_id=comp_id,
                     base_metadata=metadata,
                 )
+                textract_output_to_text_and_json_result.text_list.append(text)
+                textract_output_to_text_and_json_result.json_list.append(res)
             else:
                 for comp, job_id in zip(
                     data_obj.components,
                     component_to_textract_output_result.job_id_list,
                 ):
                     comp_id = comp.id
-                    self._textract_output_to_text_and_json_helper(
+                    text, res = self._textract_output_to_text_and_json_helper(
                         bsm=bsm,
                         workspace=workspace,
                         job_id=job_id,
                         comp_id=comp_id,
                         base_metadata=metadata,
                     )
+                    textract_output_to_text_and_json_result.text_list.append(text)
+                    textract_output_to_text_and_json_result.json_list.append(res)
+        return textract_output_to_text_and_json_result
 
     def textract_output_to_text_and_json(
         self,
         bsm: "BotoSesManager",
         workspace: "Workspace",
         debug: bool = False,
-    ):  # pragma: no cover
+    ) -> TextractOutputToTextAndJsonResult:  # pragma: no cover
         """
         Parse textract output data, and convert them into text and json view.
 
         Wrapper of the :meth:`BaseTracker._textract_output_to_text_and_json` method.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param workspace: :class:`aws_textract_pipeline.workspace.Workspace` object.
@@ -897,7 +929,130 @@
         """
         with logger.disabled(disable=not debug):
             return self._textract_output_to_text_and_json(
                 bsm=bsm,
                 workspace=workspace,
                 debug=debug,
             )
+
+    def get_next_step(self) -> StepEnum:  # pragma: no cover
+        """
+        Identify the next step of the pipeline based on the current status.
+        """
+        if self.status in [
+            self.STATUS_ENUM.s01000_landing_to_raw_pending.value,
+            self.STATUS_ENUM.s01020_landing_to_raw_in_progress.value,
+        ]:
+            return StepEnum.landing_to_raw
+        elif self.status == self.STATUS_ENUM.s01020_landing_to_raw_in_progress.value:
+            if self.is_locked() is False:
+                return StepEnum.landing_to_raw
+        elif self.status in [
+            self.STATUS_ENUM.s01060_landing_to_raw_succeeded.value,
+            self.STATUS_ENUM.s02000_raw_to_component_pending.value,
+            self.STATUS_ENUM.s02040_raw_to_component_failed.value,
+        ]:
+            return StepEnum.raw_to_component
+        elif self.status == self.STATUS_ENUM.s02020_raw_to_component_in_progress.value:
+            if self.is_locked() is False:
+                return StepEnum.raw_to_component
+        elif self.status in [
+            self.STATUS_ENUM.s02060_raw_to_component_succeeded.value,
+            self.STATUS_ENUM.s03000_component_to_textract_output_pending.value,
+            self.STATUS_ENUM.s03040_component_to_textract_output_failed.value,
+        ]:
+            return StepEnum.component_to_textract_output
+        elif (
+            self.status
+            == self.STATUS_ENUM.s03020_component_to_textract_output_in_progress.value
+        ):
+            if self.is_locked() is False:
+                return StepEnum.component_to_textract_output
+        elif self.status in [
+            self.STATUS_ENUM.s03060_component_to_textract_output_succeeded.value,
+            self.STATUS_ENUM.s05000_textract_output_to_text_and_json_pending.value,
+            self.STATUS_ENUM.s05040_textract_output_to_text_and_json_failed.value,
+        ]:
+            return StepEnum.textract_output_to_text_and_json
+        elif (
+            self.status
+            == self.STATUS_ENUM.s05020_textract_output_to_text_and_json_in_progress.value
+        ):
+            if self.is_locked() is False:
+                return StepEnum.textract_output_to_text_and_json
+        else:  # ignored status
+            pass
+
+    def move_to_next_stage(
+        self,
+        bsm: "BotoSesManager",
+        workspace: "Workspace",
+        tmp_dir: T_PATH_ARG = dir_tmp,
+        clear_tmp_dir: bool = True,
+        use_table_feature: bool = False,
+        use_form_feature: bool = False,
+        use_query_feature: bool = False,
+        use_signature_feature: bool = False,
+        use_layout_feature: bool = False,
+        sns_topic_arn: T.Optional[str] = None,
+        role_arn: T.Optional[str] = None,
+        debug: bool = False,
+    ):  # pragma: no cover
+        """
+        Move the document to the next step of the pipeline. Smartly execute
+        one of the following step:
+
+        - :meth:`landing_to_raw`
+        - :meth:`raw_to_component`
+        - :meth:`component_to_textract_output`
+        - :meth:`textract_output_to_text_and_json`
+        """
+        next_step = self.get_next_step()
+        if next_step is StepEnum.landing_to_raw:
+            self.landing_to_raw(bsm=bsm, workspace=workspace, debug=debug)
+            return MoveToNextStepResult(
+                step=StepEnum.landing_to_raw.value,
+            )
+        elif next_step is StepEnum.raw_to_component:
+            components = self.raw_to_component(
+                bsm=bsm,
+                workspace=workspace,
+                tmp_dir=tmp_dir,
+                clear_tmp_dir=clear_tmp_dir,
+                debug=debug,
+            )
+            return MoveToNextStepResult(
+                step=StepEnum.raw_to_component.value,
+                components=components,
+            )
+        elif next_step is StepEnum.component_to_textract_output:
+            component_to_textract_output_result = self.component_to_textract_output(
+                bsm=bsm,
+                workspace=workspace,
+                use_table_feature=use_table_feature,
+                use_form_feature=use_form_feature,
+                use_query_feature=use_query_feature,
+                use_signature_feature=use_signature_feature,
+                use_layout_feature=use_layout_feature,
+                sns_topic_arn=sns_topic_arn,
+                role_arn=role_arn,
+                debug=debug,
+            )
+            return MoveToNextStepResult(
+                step=StepEnum.component_to_textract_output.value,
+                component_to_textract_output_result=component_to_textract_output_result,
+            )
+        elif next_step is StepEnum.textract_output_to_text_and_json:
+            textract_output_to_text_and_json_result = (
+                self.textract_output_to_text_and_json(
+                    bsm=bsm, workspace=workspace, debug=debug
+                )
+            )
+            return MoveToNextStepResult(
+                step=StepEnum.textract_output_to_text_and_json.value,
+                textract_output_to_text_and_json_result=textract_output_to_text_and_json_result,
+            )
+        else:  # ignored status
+            return MoveToNextStepResult(
+                step=StepEnum.do_nothing.value,
+            )
+        # fmt: on
```

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/better_dataclasses.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/better_dataclasses.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/better_enum.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/better_enum.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/hashes.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/mock_aws.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/mock_aws.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/nested_logger.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/nested_logger.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/vendor/pytest_cov_helper.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline/workspace.py` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline/workspace.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/PKG-INFO` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_textract_pipeline
-Version: 0.2.1
+Version: 0.3.1
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_textract_pipeline-project
-Download-URL: https://pypi.python.org/pypi/aws_textract_pipeline/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_textract_pipeline/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_textract_pipeline-0.2.1/aws_textract_pipeline.egg-info/SOURCES.txt` & `aws_textract_pipeline-0.3.1/aws_textract_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/release-history.rst` & `aws_textract_pipeline-0.3.1/release-history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2024-04-23)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Add the following public API:
+    - ``aws_textract_pipeline.api.TextractOutputToTextAndJsonResult``
+    - ``aws_textract_pipeline.api.StepEnum``
+    - ``aws_textract_pipeline.api.MoveToNextStepResult``
+    - ``aws_textract_pipeline.api.BaseTracker.get_next_step``
+    - ``aws_textract_pipeline.api.BaseTracker.move_to_next_step_result``
+
+
 0.2.1 (2024-04-21)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 - Add the following public API:
     - ``aws_textract_pipeline.api.ext_to_doc_type_mapper``
     - ``aws_textract_pipeline.api.doc_type_to_content_type_mapper``
     - ``aws_textract_pipeline.api.get_doc_md5``
     - ``aws_textract_pipeline.api.SegmentPdfResult``
```

### Comparing `aws_textract_pipeline-0.2.1/requirements-doc.txt` & `aws_textract_pipeline-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/setup.py` & `aws_textract_pipeline-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/tests/test_doc_type.py` & `aws_textract_pipeline-0.3.1/tests/test_doc_type.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/tests/test_landing.py` & `aws_textract_pipeline-0.3.1/tests/test_landing.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/tests/test_tracker.py` & `aws_textract_pipeline-0.3.1/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `aws_textract_pipeline-0.2.1/tests/test_workspace.py` & `aws_textract_pipeline-0.3.1/tests/test_workspace.py`

 * *Files identical despite different names*

