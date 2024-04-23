# Comparing `tmp/plone.app.contentmenu-3.0.3.tar.gz` & `tmp/plone_app_contentmenu-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentmenu-3.0.3.tar", last modified: Thu Sep 14 12:47:12 2023, max compression
+gzip compressed data, was "plone_app_contentmenu-3.0.4.tar", last modified: Tue Apr 23 15:40:58 2024, max compression
```

## Comparing `plone.app.contentmenu-3.0.3.tar` & `plone_app_contentmenu-3.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.828319 plone.app.contentmenu-3.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      540 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      663 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1739 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)    13776 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18569 2023-09-14 12:47:12.828001 plone.app.contentmenu-3.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3834 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.820874 plone.app.contentmenu-3.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.821216 plone.app.contentmenu-3.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.824073 plone.app.contentmenu-3.0.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.826875 plone.app.contentmenu-3.0.3/plone/app/contentmenu/
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4139 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5580 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/contentmenu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      947 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/displayviewsmenu.py
--rw-r--r--   0 maurits    (501) staff       (20)     3846 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    38360 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/menu.py
--rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.827490 plone.app.contentmenu-3.0.3/plone/app/contentmenu/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    35089 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/tests/test_menu.py
--rw-r--r--   0 maurits    (501) staff       (20)     1130 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone/app/contentmenu/view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-09-14 12:47:12.823723 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18569 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3856 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-09-14 12:47:12.828398 plone.app.contentmenu-3.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1780 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     3926 2023-09-14 12:47:12.000000 plone.app.contentmenu-3.0.3/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.012099 plone_app_contentmenu-3.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)     1365 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      538 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     2023 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)    13968 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    19136 2024-04-23 15:40:58.011370 plone_app_contentmenu-3.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3834 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.004085 plone_app_contentmenu-3.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.004377 plone_app_contentmenu-3.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.006932 plone_app_contentmenu-3.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.009659 plone_app_contentmenu-3.0.4/plone/app/contentmenu/
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4139 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5612 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/contentmenu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      947 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/displayviewsmenu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3846 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    38360 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1299 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.010158 plone_app_contentmenu-3.0.4/plone/app/contentmenu/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35089 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/tests/test_menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1130 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone/app/contentmenu/view.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:40:58.010691 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    19136 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4283 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-23 15:40:58.012180 plone_app_contentmenu-3.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1736 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5065 2024-04-23 15:40:57.000000 plone_app_contentmenu-3.0.4/tox.ini
```

### Comparing `plone.app.contentmenu-3.0.3/.editorconfig` & `plone_app_contentmenu-3.0.4/.editorconfig`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 #
 # EditorConfig Configuration file, for more details see:
 # http://EditorConfig.org
 # EditorConfig is a convention description, that could be interpreted
 # by multiple editors to enforce common coding conventions for specific
 # file types
@@ -25,21 +25,22 @@
 # Max Line Length - a hard line wrap, should be disabled
 max_line_length = off
 
 [*.{py,cfg,ini}]
 # 4 space indentation
 indent_size = 4
 
-[*.{yml,zpt,pt,dtml,zcml}]
+[*.{yml,zpt,pt,dtml,zcml,html,xml}]
 # 2 space indentation
 indent_size = 2
 
-[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss,html}]  # Frontend development
+[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss}]  # Frontend development
 # 2 space indentation
 indent_size = 2
+max_line_length = 80
 
 [{Makefile,.gitmodules}]
 # Tab indentation (no size specified, but view as 4 spaces)
 indent_style = tab
 indent_size = unset
 tab_width = unset
```

### Comparing `plone.app.contentmenu-3.0.3/.flake8` & `plone_app_contentmenu-3.0.4/.flake8`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 [flake8]
 doctests = 1
 ignore =
     # black takes care of line length
     E501,
     # black takes care of where to break lines
```

### Comparing `plone.app.contentmenu-3.0.3/.gitignore` & `plone_app_contentmenu-3.0.4/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 # python related
 *.egg-info
 *.pyc
 *.pyo
 
+# translation related
+*.mo
+
 # tools related
 build/
 .coverage
+.*project
 coverage.xml
 dist/
 docs/_build
 __pycache__/
 .tox
 .vscode/
 node_modules/
@@ -27,14 +31,15 @@
 include/
 lib/
 lib64
 .mr.developer.cfg
 parts/
 pyvenv.cfg
 var/
+local.cfg
 
 # mxdev
 /instance/
 /.make-sentinels/
 /*-mxdev.txt
 /reports/
 /sources/
```

### Comparing `plone.app.contentmenu-3.0.3/CHANGES.rst` & `plone_app_contentmenu-3.0.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.4 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Check if "dropdown" is needed for menu items.
+  [szakitibi] (#61)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.0.3 (2023-09-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix "Add item to default page" modal form. [sverbois] (#54)
```

### Comparing `plone.app.contentmenu-3.0.3/PKG-INFO` & `plone_app_contentmenu-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentmenu
-Version: 3.0.3
+Version: 3.0.4
 Summary: Plone's content menu implementation
 Home-page: https://pypi.org/project/plone.app.contentmenu
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone contentmenu menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,26 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: setuptools
+Requires-Dist: plone.base
+Requires-Dist: plone.locking
+Requires-Dist: plone.memoize
+Requires-Dist: plone.app.content>=2.0
+Requires-Dist: plone.protect>=3.0.0
+Requires-Dist: plone.portlets
+Requires-Dist: plone.registry
+Requires-Dist: Zope
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.contenttypes[test]; extra == "test"
 
 Introduction
 ============
 
 plone.app.contentmenu contains the logic that powers Plone's content menu which is part of the toolbar.
 
 It provides the menus items (and its submenues) for
@@ -152,14 +163,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.4 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Check if "dropdown" is needed for menu items.
+  [szakitibi] (#61)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.0.3 (2023-09-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix "Add item to default page" modal form. [sverbois] (#54)
```

### Comparing `plone.app.contentmenu-3.0.3/README.rst` & `plone_app_contentmenu-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/docs/LICENSE.GPL` & `plone_app_contentmenu-3.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/docs/LICENSE.txt` & `plone_app_contentmenu-3.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/configure.zcml` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/contentmenu.pt` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/contentmenu.pt`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
           id="${menuItem/extra/id}"
       >
 
         <a class="${python:'nav-link dropdown-toggle' if submenu else 'nav-link'}"
            aria-expanded="${python:'false' if submenu else ''}"
            href="#"
            data-bs-offset="0,0"
-           data-bs-toggle="dropdown"
+           data-bs-toggle="${python: 'dropdown' if submenu else ''}"
            tal:define="
              state_class menuItem/extra/class | nothing;
              state_class python:'label-%s' % state_class if state_class else '';
            "
            tal:attributes="
              href python:menuItem['action'] or 'javascript:void(0)';
              style python:'cursor: default;; pointer-events: none' if not menuItem['action'] else None;
```

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/displayviewsmenu.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/displayviewsmenu.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/interfaces.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/menu.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/testing.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/tests/test_menu.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone/app/contentmenu/view.py` & `plone_app_contentmenu-3.0.4/plone/app/contentmenu/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/PKG-INFO` & `plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentmenu
-Version: 3.0.3
+Version: 3.0.4
 Summary: Plone's content menu implementation
 Home-page: https://pypi.org/project/plone.app.contentmenu
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone contentmenu menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,26 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: setuptools
+Requires-Dist: plone.base
+Requires-Dist: plone.locking
+Requires-Dist: plone.memoize
+Requires-Dist: plone.app.content>=2.0
+Requires-Dist: plone.protect>=3.0.0
+Requires-Dist: plone.portlets
+Requires-Dist: plone.registry
+Requires-Dist: Zope
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.contenttypes[test]; extra == "test"
 
 Introduction
 ============
 
 plone.app.contentmenu contains the logic that powers Plone's content menu which is part of the toolbar.
 
 It provides the menus items (and its submenues) for
@@ -152,14 +163,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.4 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Check if "dropdown" is needed for menu items.
+  [szakitibi] (#61)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.0.3 (2023-09-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix "Add item to default page" modal form. [sverbois] (#54)
```

### Comparing `plone.app.contentmenu-3.0.3/plone.app.contentmenu.egg-info/SOURCES.txt` & `plone_app_contentmenu-3.0.4/plone.app.contentmenu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentmenu-3.0.3/pyproject.toml` & `plone_app_contentmenu-3.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
+[build-system]
+requires = ["setuptools>=68.2"]
+
 [tool.towncrier]
 directory = "news/"
 filename = "CHANGES.rst"
 title_format = "{version} ({project_date})"
 underlines = ["-", ""]
 
 [[tool.towncrier.type]]
@@ -33,20 +36,44 @@
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "tests"
 name = "Tests"
 showcontent = true
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  towncrier_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.isort]
 profile = "plone"
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  isort_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.black]
 target-version = ["py38"]
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  black_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.codespell]
 ignore-words-list = "discreet,"
 skip = "*.po,"
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  codespell_ignores = "foo,bar"
@@ -98,15 +125,14 @@
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
-#  """
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
     ".meta.toml",
     ".pre-commit-config.yaml",
```

### Comparing `plone.app.contentmenu-3.0.3/setup.py` & `plone_app_contentmenu-3.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.3"
+version = "3.0.4"
 long_description = open("README.rst").read() + "\n"
 long_description += open("CHANGES.rst").read()
 
 setup(
     name="plone.app.contentmenu",
     version=version,
     description="Plone's content menu implementation",
@@ -47,11 +47,10 @@
         "plone.base",
         "plone.locking",
         "plone.memoize",
         "plone.app.content >= 2.0",
         "plone.protect >= 3.0.0",
         "plone.portlets",
         "plone.registry",
-        "zope.browsermenu",
-        "zope.contentprovider",
+        "Zope",
     ],
 )
```

### Comparing `plone.app.contentmenu-3.0.3/tox.ini` & `plone_app_contentmenu-3.0.4/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 [tox]
 # We need 4.4.0 for constrain_package_deps.
 min_version = 4.4.0
 envlist =
     lint
     test
@@ -28,14 +28,29 @@
     false
 # Make sure typos like `tox -e formaat` are caught instead of silently doing nothing.
 # See https://github.com/tox-dev/tox/issues/2858.
 commands =
     echo "Unrecognized environment name {envname}"
     false
 
+##
+# Add extra configuration options in .meta.toml:
+#  [tox]
+#  testenv_options = """
+#  basepython = /usr/bin/python3.8
+#  """
+##
+
+[testenv:init]
+description = Prepare environment
+skip_install = true
+commands =
+    echo "Initial setup complete"
+
+
 [testenv:format]
 description = automatically reformat code
 skip_install = true
 deps =
     pre-commit
 commands =
     pre-commit run -a pyupgrade
@@ -52,17 +67,17 @@
     pre-commit run -a
 
 [testenv:dependencies]
 description = check if the package defines all its dependencies
 skip_install = true
 deps =
     build
-    z3c.dependencychecker==2.11
+    z3c.dependencychecker==2.14.3
 commands =
-    python -m build --sdist --no-isolation
+    python -m build --sdist
     dependencychecker
 
 [testenv:dependencies-graph]
 description = generate a graph out of the dependencies of the package
 skip_install = false
 allowlist_externals =
     sh
@@ -73,18 +88,41 @@
     sh -c 'pipdeptree --exclude setuptools,wheel,pipdeptree,zope.interface,zope.component --graph-output svg > dependencies.svg'
 
 [testenv:test]
 description = run the distribution tests
 use_develop = true
 skip_install = false
 constrain_package_deps = true
-set_env = ROBOT_BROWSER=headlesschrome
+set_env =
+    ROBOT_BROWSER=headlesschrome
+
+##
+# Specify extra test environment variables in .meta.toml:
+#  [tox]
+#  test_environment_variables = """
+#      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
+#  """
+#
+# Set constrain_package_deps .meta.toml:
+#  [tox]
+#  constrain_package_deps = "false"
+##
 deps =
     zope.testrunner
     -c https://dist.plone.org/release/6.0-dev/constraints.txt
+    
+##
+# Specify additional deps in .meta.toml:
+#  [tox]
+#  test_deps_additional = "-esources/plonegovbr.portal_base[test]"
+#
+# Specify a custom constraints file in .meta.toml:
+#  [tox]
+#  constraints_file = "https://my-server.com/constraints.txt"
+##
 commands =
     zope-testrunner --all --test-path={toxinidir} -s plone.app.contentmenu {posargs}
 extras =
     test
 
 ##
 # Add extra configuration options in .meta.toml:
@@ -96,61 +134,83 @@
 ##
 
 [testenv:coverage]
 description = get a test coverage report
 use_develop = true
 skip_install = false
 constrain_package_deps = true
-set_env = ROBOT_BROWSER=headlesschrome
+set_env =
+    ROBOT_BROWSER=headlesschrome
+
+##
+# Specify extra test environment variables in .meta.toml:
+#  [tox]
+#  test_environment_variables = """
+#      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
+#  """
+##
 deps =
     coverage
     zope.testrunner
     -c https://dist.plone.org/release/6.0-dev/constraints.txt
+    
 commands =
     coverage run --branch --source plone.app.contentmenu {envbindir}/zope-testrunner --quiet --all --test-path={toxinidir} -s plone.app.contentmenu {posargs}
     coverage report -m --format markdown
+    coverage xml
 extras =
     test
 
 
 [testenv:release-check]
 description = ensure that the distribution is ready to release
 skip_install = true
 deps =
     twine
     build
     towncrier
     -c https://dist.plone.org/release/6.0-dev/constraints.txt
+    
 commands =
     # fake version to not have to install the package
     # we build the change log as news entries might break
     # the README that is displayed on PyPI
     towncrier build --version=100.0.0 --yes
-    python -m build --sdist --no-isolation
+    python -m build --sdist
     twine check dist/*
 
 [testenv:circular]
 description = ensure there are no cyclic dependencies
 use_develop = true
 skip_install = false
+set_env =
+
+##
+# Specify extra test environment variables in .meta.toml:
+#  [tox]
+#  test_environment_variables = """
+#      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
+#  """
+##
 allowlist_externals =
     sh
 deps =
     pipdeptree
     pipforester
     -c https://dist.plone.org/release/6.0-dev/constraints.txt
+    
 commands =
     # Generate the full dependency tree
     sh -c 'pipdeptree -j > forest.json'
     # Generate a DOT graph with the circular dependencies, if any
     pipforester -i forest.json -o forest.dot --cycles
     # Report if there are any circular dependencies, i.e. error if there are any
     pipforester -i forest.json --check-cycles -o /dev/null
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [tox]
 #  extra_lines = """
-#      my_other_environment
+#  _your own configuration lines_
 #  """
 ##
```

