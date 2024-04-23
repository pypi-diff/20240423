# Comparing `tmp/socassess-0.2.1.tar.gz` & `tmp/socassess-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socassess-0.2.1.tar", max compression
+gzip compressed data, was "socassess-0.2.2.tar", max compression
```

## Comparing `socassess-0.2.1.tar` & `socassess-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2024-04-09 20:18:26.510048 socassess-0.2.1/LICENSE
--rw-r--r--   0        0        0     7455 2024-04-09 20:18:26.510208 socassess-0.2.1/README.md
--rw-r--r--   0        0        0     1177 2024-04-09 20:18:41.660696 socassess-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-09 20:18:26.515285 socassess-0.2.1/src/socassess/__init__.py
--rw-r--r--   0        0        0      114 2024-04-09 20:18:26.515414 socassess-0.2.1/src/socassess/ai/__init__.py
--rw-r--r--   0        0        0     1419 2024-04-09 20:18:26.515495 socassess-0.2.1/src/socassess/ai/ai.py
--rw-r--r--   0        0        0     1142 2024-04-09 20:18:26.515570 socassess-0.2.1/src/socassess/ai/config.py
--rw-r--r--   0        0        0      592 2024-04-09 20:18:26.515658 socassess-0.2.1/src/socassess/config.py
--rw-r--r--   0        0        0     3666 2024-04-09 20:18:26.515744 socassess-0.2.1/src/socassess/console.py
--rw-r--r--   0        0        0     5423 2024-04-09 20:18:26.515860 socassess-0.2.1/src/socassess/create.py
--rw-r--r--   0        0        0     1653 2024-04-09 20:18:26.515939 socassess-0.2.1/src/socassess/display.py
--rw-r--r--   0        0        0      123 2024-04-09 20:18:26.516042 socassess-0.2.1/src/socassess/email/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-09 20:18:26.516120 socassess-0.2.1/src/socassess/email/config.py
--rw-r--r--   0        0        0     2012 2024-04-09 20:18:26.516204 socassess-0.2.1/src/socassess/email/email.py
--rw-r--r--   0        0        0     1252 2024-04-09 20:18:26.516283 socassess-0.2.1/src/socassess/email/expert.py
--rw-r--r--   0        0        0      110 2024-04-09 20:18:26.516362 socassess-0.2.1/src/socassess/exception.py
--rw-r--r--   0        0        0     7104 2024-04-09 20:18:26.516497 socassess-0.2.1/src/socassess/feedback.py
--rw-r--r--   0        0        0     1710 2024-04-09 20:18:26.516580 socassess-0.2.1/src/socassess/feedback_helper.py
--rw-r--r--   0        0        0      372 2024-04-09 20:18:26.516656 socassess-0.2.1/src/socassess/level.py
--rw-r--r--   0        0        0     2319 2024-04-09 20:18:26.516731 socassess-0.2.1/src/socassess/parse_args.py
--rw-r--r--   0        0        0     2090 2024-04-09 20:18:26.516818 socassess-0.2.1/src/socassess/socassess.template.toml
--rw-r--r--   0        0        0      142 2024-04-09 20:18:26.516895 socassess-0.2.1/src/socassess/userargs.py
--rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 socassess-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-23 00:15:22.768323 socassess-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7455 2024-04-23 00:15:22.768323 socassess-0.2.2/README.md
+-rw-r--r--   0        0        0     1177 2024-04-23 00:15:22.776322 socassess-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/ai/__init__.py
+-rw-r--r--   0        0        0     1419 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/ai/ai.py
+-rw-r--r--   0        0        0     1142 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/ai/config.py
+-rw-r--r--   0        0        0      592 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/config.py
+-rw-r--r--   0        0        0     3666 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/console.py
+-rw-r--r--   0        0        0     5423 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/create.py
+-rw-r--r--   0        0        0     1653 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/display.py
+-rw-r--r--   0        0        0      123 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/email/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/email/config.py
+-rw-r--r--   0        0        0     2012 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/email/email.py
+-rw-r--r--   0        0        0     1252 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/email/expert.py
+-rw-r--r--   0        0        0      110 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/exception.py
+-rw-r--r--   0        0        0     7109 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/feedback.py
+-rw-r--r--   0        0        0     1710 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/feedback_helper.py
+-rw-r--r--   0        0        0      372 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/level.py
+-rw-r--r--   0        0        0     2319 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/parse_args.py
+-rw-r--r--   0        0        0     2090 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/socassess.template.toml
+-rw-r--r--   0        0        0      142 2024-04-23 00:15:22.776322 socassess-0.2.2/src/socassess/userargs.py
+-rw-r--r--   0        0        0     8663 1970-01-01 00:00:00.000000 socassess-0.2.2/PKG-INFO
```

### Comparing `socassess-0.2.1/LICENSE` & `socassess-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/README.md` & `socassess-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/pyproject.toml` & `socassess-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "socassess"
-version = "0.2.1"
+version = "0.2.2"
 description = "make test-based assessment's feedback easy to setup"
 authors = ["Huanyi Chen <huanyi.chen@uwaterloo.ca>"]
 readme = "README.md"
 homepage = "https://github.com/h365chen/socassess"
 repository = "https://github.com/h365chen/socassess"
 keywords = ["automated", "feedback", "education"]
 classifiers = [
```

### Comparing `socassess-0.2.1/src/socassess/ai/ai.py` & `socassess-0.2.2/src/socassess/ai/ai.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/ai/config.py` & `socassess-0.2.2/src/socassess/ai/config.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/config.py` & `socassess-0.2.2/src/socassess/config.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/console.py` & `socassess-0.2.2/src/socassess/console.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/create.py` & `socassess-0.2.2/src/socassess/create.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/display.py` & `socassess-0.2.2/src/socassess/display.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/email/config.py` & `socassess-0.2.2/src/socassess/email/config.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/email/email.py` & `socassess-0.2.2/src/socassess/email/email.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/email/expert.py` & `socassess-0.2.2/src/socassess/email/expert.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/feedback.py` & `socassess-0.2.2/src/socassess/feedback.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,23 +130,23 @@
     # step1: handle non regex matches
     if cur_set.issubset(frozenset(outcomes)):
         return True
 
     # step2: handle regex matches
     for cs in cur_set:
         matched = False
-        m = re.match('(.*?)\[\*\]::(passed|failed)', cs, flags=re.I)
+        m = re.match('(.*?)\\[\\*\\]::(passed|failed)', cs, flags=re.I)
         # only regex patterns can be left after step1; otherwise, it means
         # there is no match
         if m is None:
             return False
         pattern = m.group(1)  # prefix pattern
         ot = m.group(2)  # "passed" or "failed"
         for t in outcomes:
-            m = re.match(f'{pattern}\[.*\]::(passed|failed)', t, flags=re.I)
+            m = re.match(f'{pattern}\\[.*\\]::(passed|failed)', t, flags=re.I)
             # mismatching "passed" or "failed"
             if m is not None:
                 matched = True
                 if m.group(1) != ot:
                     return False
         if not matched:
             return False
```

### Comparing `socassess-0.2.1/src/socassess/feedback_helper.py` & `socassess-0.2.2/src/socassess/feedback_helper.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/parse_args.py` & `socassess-0.2.2/src/socassess/parse_args.py`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/src/socassess/socassess.template.toml` & `socassess-0.2.2/src/socassess/socassess.template.toml`

 * *Files identical despite different names*

### Comparing `socassess-0.2.1/PKG-INFO` & `socassess-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: socassess
-Version: 0.2.1
+Version: 0.2.2
 Summary: make test-based assessment's feedback easy to setup
 Home-page: https://github.com/h365chen/socassess
 Keywords: automated,feedback,education
 Author: Huanyi Chen
 Author-email: huanyi.chen@uwaterloo.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: pytest (>=7.4.1,<8.0.0)
```

