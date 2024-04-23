# Comparing `tmp/mkdocs_ezglossary_plugin-1.6.6.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.6.tar", last modified: Tue Apr 23 15:17:28 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.7.tar", last modified: Tue Apr 23 16:09:44 2024, max compression
```

## Comparing `mkdocs_ezglossary_plugin-1.6.6.tar` & `mkdocs_ezglossary_plugin-1.6.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.757438 mkdocs_ezglossary_plugin-1.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.757438 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 15:17:28.000000 mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:17:28.761438 mkdocs_ezglossary_plugin-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-23 15:17:04.000000 mkdocs_ezglossary_plugin-1.6.6/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.641578 mkdocs_ezglossary_plugin-1.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.641578 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 16:09:44.000000 mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:09:44.645578 mkdocs_ezglossary_plugin-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-23 16:09:20.000000 mkdocs_ezglossary_plugin-1.6.7/tests/test_summary.py
```

### Comparing `mkdocs_ezglossary_plugin-1.6.6/LICENSE` & `mkdocs_ezglossary_plugin-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.6
+Version: 1.6.7
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.6/README.md` & `mkdocs_ezglossary_plugin-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/setup.cfg` & `mkdocs_ezglossary_plugin-1.6.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.6.6
+version = 1.6.7
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 log = logging.getLogger("mkdocs.plugins.ezglossary")
 
 
 class __re:
     def __init__(self):
         self.ws = r"[\n ]*"
-        self.section = r"([^:<>\"\|/\@#][^:<>\"\|/\@]*)"
+        self.section = r"([^:<>\"\|/\@&#][^:<>\"\|/\@]*)"
         self.term = self.section
         self.text = r"([^>]+)"
         self.dt = rf"<dt>(<.*>)?{self.section}:{self.term}(<.*>)?<\/dt>"
         self.dt_default = rf"<dt>(<.*>)?{self.term}(<.*>)?<\/dt>"
         self.dd = r"<dd>\n?((.|\n)+?)<\/dd>"
         self.options = r"([\\\|\=\w\+]+)"
```

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.6
+Version: 1.6.7
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.6/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.6.7/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.6.7/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/tests/test_link.py` & `mkdocs_ezglossary_plugin-1.6.7/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.6.7/tests/test_page_ref.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.6/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.6.7/tests/test_summary.py`

 * *Files identical despite different names*

