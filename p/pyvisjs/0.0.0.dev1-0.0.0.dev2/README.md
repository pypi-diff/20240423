# Comparing `tmp/pyvisjs-0.0.0.dev1.tar.gz` & `tmp/pyvisjs-0.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev1.tar", last modified: Mon Apr 22 18:17:39 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev2.tar", last modified: Tue Apr 23 07:03:06 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev1.tar` & `pyvisjs-0.0.0.dev2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.870387 pyvisjs-0.0.0.dev1/
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3385 2024-04-22 18:17:39.870387 pyvisjs-0.0.0.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1455 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.866387 pyvisjs-0.0.0.dev1/examples/
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.867387 pyvisjs-0.0.0.dev1/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.868387 pyvisjs-0.0.0.dev1/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.869387 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3385 2024-04-22 18:17:39.000000 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-22 18:17:39.000000 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 18:17:39.000000 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-22 18:17:39.000000 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 18:17:39.000000 pyvisjs-0.0.0.dev1/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 18:17:39.870387 pyvisjs-0.0.0.dev1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 18:17:39.869387 pyvisjs-0.0.0.dev1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-22 18:17:22.000000 pyvisjs-0.0.0.dev1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.011534 pyvisjs-0.0.0.dev2/
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3385 2024-04-23 07:03:06.010533 pyvisjs-0.0.0.dev2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/example.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.006533 pyvisjs-0.0.0.dev2/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.007534 pyvisjs-0.0.0.dev2/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.009534 pyvisjs-0.0.0.dev2/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.010533 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3385 2024-04-23 07:03:05.000000 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-04-23 07:03:05.000000 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:03:05.000000 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-23 07:03:05.000000 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 07:03:05.000000 pyvisjs-0.0.0.dev2/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:03:06.011534 pyvisjs-0.0.0.dev2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:03:06.009534 pyvisjs-0.0.0.dev2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-23 07:02:47.000000 pyvisjs-0.0.0.dev2/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev1/.gitignore` & `pyvisjs-0.0.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/CONTRIBUTING.md` & `pyvisjs-0.0.0.dev2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/LICENSE` & `pyvisjs-0.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/PKG-INFO` & `pyvisjs-0.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev1
+Version: 0.0.0.dev2
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev1/README.md` & `pyvisjs-0.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/examples/main.py` & `pyvisjs-0.0.0.dev2/examples/main.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/folder_structure.txt` & `pyvisjs-0.0.0.dev2/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/pyproject.toml` & `pyvisjs-0.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/pyvisjs/templates/basic.html` & `pyvisjs-0.0.0.dev2/pyvisjs/templates/basic.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev2/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev1/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev2/pyvisjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev1
+Version: 0.0.0.dev2
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev1/tests/test_network.py` & `pyvisjs-0.0.0.dev2/tests/test_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     n = Network("Network1")
     
     # assert
     assert n.name == "Network1"
     assert n.width == DEFAULT_WIDTH
     assert n.height == DEFAULT_HEIGHT
     assert n.env is not None
-    assert n.data == {}
+    assert n.data == {"nodes": [], "edges": []}
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_render_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
```

### Comparing `pyvisjs-0.0.0.dev1/tests/test_utils.py` & `pyvisjs-0.0.0.dev2/tests/test_utils.py`

 * *Files identical despite different names*

