# Comparing `tmp/inni-0.2.1.tar.gz` & `tmp/inni-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inni-0.2.1.tar", max compression
+gzip compressed data, was "inni-0.3.0.tar", max compression
```

## Comparing `inni-0.2.1.tar` & `inni-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.2.1/LICENSE
--rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.2.1/inni/__init__.py
--rw-r--r--   0        0        0     3079 2024-04-10 09:44:17.476489 inni-0.2.1/inni/cli.py
--rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.2.1/inni/config.py
--rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.2.1/inni/loader.py
--rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.2.1/inni/modules/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.2.1/inni/modules/base.py
--rw-r--r--   0        0        0     3298 2024-04-18 17:13:22.390200 inni-0.2.1/inni/modules/bitrix.py
--rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.2.1/inni/modules/dummy.py
--rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.2.1/inni/modules/email.py
--rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.2.1/inni/modules/jira.py
--rw-r--r--   0        0        0      495 2024-04-17 20:23:23.861455 inni-0.2.1/inni/modules/runner.py
--rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.2.1/inni/modules/skype.py
--rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.2.1/inni/template.py
--rw-r--r--   0        0        0      724 2024-04-18 17:14:47.943649 inni-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 inni-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34580 2024-03-31 18:16:37.639008 inni-0.3.0/LICENSE
+-rw-r--r--   0        0        0       72 2024-03-31 18:16:37.639008 inni-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 18:16:37.639008 inni-0.3.0/inni/__init__.py
+-rw-r--r--   0        0        0     4130 2024-04-23 08:27:43.914857 inni-0.3.0/inni/cli.py
+-rw-r--r--   0        0        0      846 2024-04-09 15:08:28.211108 inni-0.3.0/inni/config.py
+-rw-r--r--   0        0        0      302 2024-04-09 15:08:28.211108 inni-0.3.0/inni/loader.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:08:28.211108 inni-0.3.0/inni/modules/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-09 15:08:28.211108 inni-0.3.0/inni/modules/base.py
+-rw-r--r--   0        0        0     3298 2024-04-23 08:27:43.914857 inni-0.3.0/inni/modules/bitrix.py
+-rw-r--r--   0        0        0      495 2024-04-09 15:08:28.211108 inni-0.3.0/inni/modules/dummy.py
+-rw-r--r--   0        0        0     1558 2024-04-09 15:08:28.211108 inni-0.3.0/inni/modules/email.py
+-rw-r--r--   0        0        0     3631 2024-04-23 08:27:43.914857 inni-0.3.0/inni/modules/jira.py
+-rw-r--r--   0        0        0     1027 2024-04-09 15:08:28.211108 inni-0.3.0/inni/modules/skype.py
+-rw-r--r--   0        0        0      407 2024-04-09 15:08:28.211108 inni-0.3.0/inni/template.py
+-rw-r--r--   0        0        0      724 2024-04-23 08:29:37.477543 inni-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 inni-0.3.0/PKG-INFO
```

### Comparing `inni-0.2.1/LICENSE` & `inni-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/config.py` & `inni-0.3.0/inni/config.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/modules/base.py` & `inni-0.3.0/inni/modules/base.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/modules/bitrix.py` & `inni-0.3.0/inni/modules/bitrix.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/modules/email.py` & `inni-0.3.0/inni/modules/email.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/modules/jira.py` & `inni-0.3.0/inni/modules/jira.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/inni/modules/skype.py` & `inni-0.3.0/inni/modules/skype.py`

 * *Files identical despite different names*

### Comparing `inni-0.2.1/pyproject.toml` & `inni-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inni"
-version = "0.2.1"
+version = "0.3.0"
 description = "Modular system to perform tasks surrounding log-in and log-out."
 authors = ["Ceda EI <ceda_ei@webionite.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://gitlab.com/ceda_ei/inni"
 repository = "https://gitlab.com/ceda_ei/inni"
```

### Comparing `inni-0.2.1/PKG-INFO` & `inni-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inni
-Version: 0.2.1
+Version: 0.3.0
 Summary: Modular system to perform tasks surrounding log-in and log-out.
 Home-page: https://gitlab.com/ceda_ei/inni
 License: GPL-3.0
 Author: Ceda EI
 Author-email: ceda_ei@webionite.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

