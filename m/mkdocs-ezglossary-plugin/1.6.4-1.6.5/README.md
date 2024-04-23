# Comparing `tmp/mkdocs_ezglossary_plugin-1.6.4.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.4.tar", last modified: Tue Apr 23 11:06:07 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.5.tar", last modified: Tue Apr 23 13:10:24 2024, max compression
```

## Comparing `mkdocs_ezglossary_plugin-1.6.4.tar` & `mkdocs_ezglossary_plugin-1.6.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.759533 mkdocs_ezglossary_plugin-1.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.759533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.489910 mkdocs_ezglossary_plugin-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 13:10:24.489910 mkdocs_ezglossary_plugin-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 13:10:24.489910 mkdocs_ezglossary_plugin-1.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.481911 mkdocs_ezglossary_plugin-1.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.485911 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.485911 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.489910 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 13:10:24.000000 mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:10:24.485911 mkdocs_ezglossary_plugin-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-23 13:09:56.000000 mkdocs_ezglossary_plugin-1.6.5/tests/test_summary.py
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/LICENSE` & `mkdocs_ezglossary_plugin-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.4
+Version: 1.6.5
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,14 +18,16 @@
 This plugin adds glossary support for mkdocs. It supports
 
 -   Defining multiple glossaries
 -   Linking to glossary entries in text
 -   Printing a summary of your glossary with definitions and
     references anywhere in your documentation.
 -   Customizable output
+-   Unicode support
+-   PDF support
 
 ## Documentation
 
 -   Read the [full documentation](https://realtimeprojects.github.io/mkdocs-ezglossary)
 
 ## Prerequisites
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/README.md` & `mkdocs_ezglossary_plugin-1.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 This plugin adds glossary support for mkdocs. It supports
 
 -   Defining multiple glossaries
 -   Linking to glossary entries in text
 -   Printing a summary of your glossary with definitions and
     references anywhere in your documentation.
 -   Customizable output
+-   Unicode support
+-   PDF support
 
 ## Documentation
 
 -   Read the [full documentation](https://realtimeprojects.github.io/mkdocs-ezglossary)
 
 ## Prerequisites
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/setup.cfg` & `mkdocs_ezglossary_plugin-1.6.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.6.4
+version = 1.6.5
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import hashlib
 import logging
+import html
 
 log = logging.getLogger(__name__)
 
 
 def get_id(section: str, term: str, linktype: str, n: str):
     return str(hashlib.md5(f"{section}_{term}_{linktype}_{n}".encode()).hexdigest())
 
@@ -28,15 +29,15 @@
 class Glossary:
     """ The complete glossary for all sections """
 
     def __init__(self):
         self.clear()
 
     def add(self, section, term, linktype, page, definition=None, anchor=None):
-        term = term.strip()
+        term = html.unescape(term.strip())
         log.debug(f"glossary.add({section}, {term}, {linktype}, '{definition}', {anchor})")
         links = self._links(section, term, linktype)
         _id = get_id(section, term, linktype, len(links))
         anchor = _id if anchor is None else anchor
         links[_id] = Entry(anchor, page, definition)
         return _id
 
@@ -69,30 +70,30 @@
 
                     `defs`
                     : returns all definitions for the term
 
             Returns:
                 A list of either `definitions` or `references` for the given term.
         """
-        links = self._links(section, term, linktype).values()
+        links = self._links(section, html.unescape(term), linktype).values()
         return list(links)
 
     def definition(self, section: str, term: str) -> str:
         """ Get the definition for a term.
 
             Args:
                 section:
                     The name of the section
                 term:
                     The term to get the definition for
 
             Returns:
                 The definition of the term
         """
-        defs = self.get(section, term, 'defs')
+        defs = self.get(section, html.unescape(term), 'defs')
         if not defs:
             return ""
         return defs[0].definition
 
     def terms(self, section: str) -> list[str]:
         """ Return a list of entries for a specific section.
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 import os
-from html import parser
+from html import parser, unescape
 
 from mkdocs.plugins import BasePlugin, event_priority
 from mkdocs import config
 from mkdocs.config import config_options as co
 
 from .glossary import Glossary
 
@@ -13,16 +13,16 @@
 
 log = logging.getLogger("mkdocs.plugins.ezglossary")
 
 
 class __re:
     def __init__(self):
         self.ws = r"[\n ]*"
-        self.section = r"([^:<>\"\|]+)"
-        self.term = r"([^:<>\"\|]+)"
+        self.section = r"([^:<>\"\|/#][^:<>\"\|/]*)"
+        self.term = self.section
         self.text = r"([^>]+)"
         self.dt = rf"<dt>(<.*>)?{self.section}:{self.term}(<.*>)?<\/dt>"
         self.dt_default = rf"<dt>(<.*>)?{self.term}(<.*>)?<\/dt>"
         self.dd = r"<dd>\n?((.|\n)+?)<\/dd>"
         self.options = r"([\\\|\=\w\+]+)"
 
 
@@ -208,15 +208,15 @@
 
         regex = fr"{self._reflink}:{_re.section}:{_re.term}"
         return re.sub(regex, _replace, output)
 
     def _replace_glossary_links(self, output, page, root):
         def _replace(mo):
             section = mo.group(1)
-            term = mo.group(2)
+            term = unescape(mo.group(2))
             text = mo.group(3)
             _id = mo.group(4)
             defs = self._glossary.get(section, term, 'defs')
 
             if len(defs) == 0:
                 log.warning(f"page '{page.url}' refers to undefined glossary entry {section}:{term}")
                 term = "" if term == "__None__" else term
@@ -242,14 +242,15 @@
         regex = fr"{self._uuid}:{_re.section}:{_re.term}:<{_re.text}>:(\w+)"
         return re.sub(regex, _replace, output)
 
     def _find_definitions(self, content, page):
         log.debug(f"_find_definitions({page})")
 
         def _add_entry(section, term, definition, fmt_pre, fmt_post):
+            term = unescape(term)
             log.debug(f"glossary: found definition: {section}:{term}:{definition} {fmt_pre}:{fmt_post}")
 
             if self.config.tooltip == "none":
                 _tooltip = ""
             if self.config.tooltip == "short":
                 _tooltip = definition.split("\n")[0]
             if self.config.tooltip == "full":
@@ -262,15 +263,15 @@
             _id = self._glossary.add(section, term, 'defs', page, _tooltip)
 
             inline_refs = self._get_config(section, 'inline_refs')
             reflink = f"\n{self._reflink}:{section}:{term}" if inline_refs != "none" else ""
             return template.render("definition.html",
                                    self.config,
                                    target=_id,
-                                   term=term,
+                                   term=unescape(term),
                                    definition=definition,
                                    reflink=reflink,
                                    fmt_pre=fmt_pre if fmt_pre else "",
                                    fmt_post=fmt_post if fmt_post else "")
 
         def _replace(mo):
             fmt_pre = mo.group(1)
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.4
+Version: 1.6.5
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,14 +18,16 @@
 This plugin adds glossary support for mkdocs. It supports
 
 -   Defining multiple glossaries
 -   Linking to glossary entries in text
 -   Printing a summary of your glossary with definitions and
     references anywhere in your documentation.
 -   Customizable output
+-   Unicode support
+-   PDF support
 
 ## Documentation
 
 -   Read the [full documentation](https://realtimeprojects.github.io/mkdocs-ezglossary)
 
 ## Prerequisites
```

### Comparing `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.6.5/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.6.5/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/tests/test_link.py` & `mkdocs_ezglossary_plugin-1.6.5/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.6.5/tests/test_page_ref.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.4/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.6.5/tests/test_summary.py`

 * *Files identical despite different names*

