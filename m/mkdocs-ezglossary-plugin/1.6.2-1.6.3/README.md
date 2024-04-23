# Comparing `tmp/mkdocs_ezglossary_plugin-1.6.2.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.2.tar", last modified: Mon Apr 22 10:06:43 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.3.tar", last modified: Mon Apr 22 14:00:31 2024, max compression
```

## Comparing `mkdocs_ezglossary_plugin-1.6.2.tar` & `mkdocs_ezglossary_plugin-1.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.132145 mkdocs_ezglossary_plugin-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.132145 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 10:06:43.000000 mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:06:43.136144 mkdocs_ezglossary_plugin-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-22 10:06:17.000000 mkdocs_ezglossary_plugin-1.6.2/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.329543 mkdocs_ezglossary_plugin-1.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_summary.py
```

### Comparing `mkdocs_ezglossary_plugin-1.6.2/LICENSE` & `mkdocs_ezglossary_plugin-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.2
+Version: 1.6.3
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.2/README.md` & `mkdocs_ezglossary_plugin-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/setup.cfg` & `mkdocs_ezglossary_plugin-1.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.6.2
+version = 1.6.3
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self):
         self.clear()
 
     def add(self, section, term, linktype, page, definition=None, anchor=None):
         term = term.strip()
         log.debug(f"glossary.add({section}, {term}, {linktype}, '{definition}', {anchor})")
         links = self._links(section, term, linktype)
-        _id = f"{section}_{term}_{linktype}_{len(links)}".replace(" ", "_")
+        _id = f"{section}_{term}_{linktype}_{len(links)}".replace(" ", "_").replace("-", "_")
         anchor = _id if anchor is None else anchor
         links[_id] = Entry(anchor, page, definition)
         return _id
 
     def has(self, section: str) -> bool:
         """ Check if the glossary has a section named **section**.
```

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.2
+Version: 1.6.3
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.2/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.6.3/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/tests/test_link.py` & `mkdocs_ezglossary_plugin-1.6.3/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.6.3/tests/test_page_ref.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.2/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.6.3/tests/test_summary.py`

 * *Files identical despite different names*

