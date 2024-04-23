# Comparing `tmp/mkdocs_ezglossary_plugin-1.6.3.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.3.tar", last modified: Mon Apr 22 14:00:31 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.4.tar", last modified: Tue Apr 23 11:06:07 2024, max compression
```

## Comparing `mkdocs_ezglossary_plugin-1.6.3.tar` & `mkdocs_ezglossary_plugin-1.6.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.329543 mkdocs_ezglossary_plugin-1.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 14:00:31.000000 mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:00:31.333543 mkdocs_ezglossary_plugin-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-22 14:00:07.000000 mkdocs_ezglossary_plugin-1.6.3/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.759533 mkdocs_ezglossary_plugin-1.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.759533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 11:06:07.000000 mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:06:07.763533 mkdocs_ezglossary_plugin-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-23 11:05:41.000000 mkdocs_ezglossary_plugin-1.6.4/tests/test_summary.py
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/LICENSE` & `mkdocs_ezglossary_plugin-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.3
+Version: 1.6.4
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/README.md` & `mkdocs_ezglossary_plugin-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/setup.cfg` & `mkdocs_ezglossary_plugin-1.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.6.3
+version = 1.6.4
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import hashlib
 import logging
 
 log = logging.getLogger(__name__)
 
 
+def get_id(section: str, term: str, linktype: str, n: str):
+    return str(hashlib.md5(f"{section}_{term}_{linktype}_{n}".encode()).hexdigest())
+
+
 class Entry:
     """ An entry in the glossary. """
 
     def __init__(self, target, page, definition):
         self.target = target
         """ The anchor to directly point to this specific link. """
 
@@ -26,15 +31,15 @@
     def __init__(self):
         self.clear()
 
     def add(self, section, term, linktype, page, definition=None, anchor=None):
         term = term.strip()
         log.debug(f"glossary.add({section}, {term}, {linktype}, '{definition}', {anchor})")
         links = self._links(section, term, linktype)
-        _id = f"{section}_{term}_{linktype}_{len(links)}".replace(" ", "_").replace("-", "_")
+        _id = get_id(section, term, linktype, len(links))
         anchor = _id if anchor is None else anchor
         links[_id] = Entry(anchor, page, definition)
         return _id
 
     def has(self, section: str) -> bool:
         """ Check if the glossary has a section named **section**.
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 log = logging.getLogger("mkdocs.plugins.ezglossary")
 
 
 class __re:
     def __init__(self):
         self.ws = r"[\n ]*"
-        self.section = r"(\w+)"
-        self.term = r"([\w -]+)"
+        self.section = r"([^:<>\"\|]+)"
+        self.term = r"([^:<>\"\|]+)"
         self.text = r"([^>]+)"
         self.dt = rf"<dt>(<.*>)?{self.section}:{self.term}(<.*>)?<\/dt>"
         self.dt_default = rf"<dt>(<.*>)?{self.term}(<.*>)?<\/dt>"
         self.dd = r"<dd>\n?((.|\n)+?)<\/dd>"
         self.options = r"([\\\|\=\w\+]+)"
 
 
@@ -42,15 +42,15 @@
     templates = config.config_options.Type(str, default="")
 
 
 class GlossaryPlugin(BasePlugin[GlossaryConfig]):
     def __init__(self):
         self._glossary = Glossary()
         self._uuid = "6251a85a-47d0-11ee-be56-0242ac120002"
-        self._reflink = "6251a85a-47d0-11ee-be56-0242ac120002"
+        self._reflink = "886d7696-137e-4a59-a39d-6f7d311d5bd1"
 
     def on_pre_build(self, config, **kwargs):
         if self.config.strict and "_" not in self.config.sections:
             self.config.sections.append("_")
         if self.config.strict and len(self.config.sections) == 0:
             log.error("ezglossary: no sections defined, but 'strict' is true, plugin disabled")
         self._glossary.clear()
@@ -164,15 +164,15 @@
 
     def _register_glossary_links(self, output, page):
 
         def _add_link(section, term, text):
             section = "_" if (section == "default" or section is None) else section
             term = term if term else "__None__"
             text = text if text else "__None__"
-            log.debug(f"glossary: found {section}/{term}/{text}")
+            log.debug(f"glossary: found link: {section}/{term}/{text}")
             _id = self._glossary.add(section, term, 'refs', page)
             return f"{self._uuid}:{section}:{term}:<{text}>:{_id}"
 
         def _replace(mo):
             return _add_link(mo.group(1), mo.group(2), mo.group(4))
 
         def _replace_default(mo):
@@ -192,14 +192,15 @@
 
         return output
 
     def _replace_inline_refs(self, output, page, root):
         def _replace(mo):
             section = mo.group(1)
             term = mo.group(2)
+            log.debug(f"inline_refs: looking up: '{section}/{term}'")
 
             mode = self._get_config(section, 'inline_refs')
 
             entries = self._glossary.get(section, term, 'refs')
             return template.render(f"refs-{mode}.html",
                                    self.config,
                                    entries=entries,
@@ -241,15 +242,15 @@
         regex = fr"{self._uuid}:{_re.section}:{_re.term}:<{_re.text}>:(\w+)"
         return re.sub(regex, _replace, output)
 
     def _find_definitions(self, content, page):
         log.debug(f"_find_definitions({page})")
 
         def _add_entry(section, term, definition, fmt_pre, fmt_post):
-            log.debug(f"found entry: {section}:{term}:{definition} {fmt_pre}:{fmt_post}")
+            log.debug(f"glossary: found definition: {section}:{term}:{definition} {fmt_pre}:{fmt_post}")
 
             if self.config.tooltip == "none":
                 _tooltip = ""
             if self.config.tooltip == "short":
                 _tooltip = definition.split("\n")[0]
             if self.config.tooltip == "full":
                 _tooltip = definition
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.3
+Version: 1.6.4
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.6.4/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.3/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.6.4/tests/test_definitions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 import logging
 import mock
 
 from yaxp import xpath
 
+from mkdocs_ezglossary_plugin.glossary import get_id
+
 
 log = logging.getLogger(__name__)
 
 
 def test_default_config(simple, config):
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(id="test_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("test", "first", "defs", 0), text="first")))
     dl = dl.has(xpath.dd(text="first term"))
-    dl = dl.has(xpath.dt.has(xpath.a(id="test_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("test", "second", "defs", 0), text="second")))
     dl = dl.has(xpath.dd(text="*second term"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(id="demo_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("demo", "first", "defs", 0), text="first")))
     dl = dl.has(xpath.dd(text="demo 1"))
-    dl = dl.has(xpath.dt.has(xpath.a(id="demo_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("demo", "second", "defs", 0), text="second")))
     dl = dl.has(xpath.dd(text="demo 2"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
     dl = dl.has(xpath.dd(text="*demo 2").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
 
 def test_inline_refs(simple, config):
     config['inline_refs'] = "short"
     html = mock.render_single(simple, config)
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(id="test_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("test", "first", "defs", 0), text="first")))
     dl = dl.has(xpath.dd(text="*first term").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
     dl = xpath.dl()
-    dl = dl.has(xpath.dt.has(xpath.a(id="test_third_defs_0", text="third")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("test", "third", "defs", 0), text="third")))
     dl = dl.has(xpath.dd(text="*third term").has(xpath.a(title="Hello",
-                                                         href="../simple.md#test_third_refs_0",
+                                                         href="../simple.md#" + get_id("test", "third", "refs", 0),
                                                          text="*[1]")))
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_default_section(simple, config):
     config['use_default'] = True
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(id="__default_defs_0", text="default")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("_", "default", "defs", 0), text="default")))
     dl = dl.has(xpath.dd(text="default term"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(id="demo_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("demo", "first", "defs", 0), text="first")))
     dl = dl.has(xpath.dd(text="demo 1"))
-    dl = dl.has(xpath.dt.has(xpath.a(id="demo_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id=get_id("demo", "second", "defs", 0), text="second")))
     dl = dl.has(xpath.dd(text="demo 2"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
     dl = dl.has(xpath.dd(text="*demo 2").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
 
 def test_formatted_dt(simple, config):
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.bold.em.code.has(xpath.a(id="demo_formatted_defs_0", text="formatted")))
+    dl = dl.has(xpath.dt.bold.em.code.has(xpath.a(id=get_id("demo", "formatted", "defs", 0), text="formatted")))
     dl = dl.has(xpath.dd(text="formatted dd"))
     assert len(html.xpath(str(dl)))
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.6.4/tests/test_page_ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import mock
 
 import yaml
 from yaxp import xpath as xp
 
+from mkdocs_ezglossary_plugin.glossary import get_id
+
 mycommand = mock.Page(
     title="My Command",
     file="mycommand.md",
     ctype="markdown",
     content="""
 # Help page
 
@@ -59,15 +61,15 @@
     pages = mock.render([mycommand, commands], config)
 
     dl = xp.dl(_class="#mkdocs-ezglossary-summary", _id="page")
     dl = dl.has(xp.dt.a(href="../mycommand.md#",
                         text="help1"))
     assert len(pages['commands.md'].xpath(str(dl))) == 1
 
-    dd = xp.dd.ul.li.a(href="../commands.md#cmd_help2_refs_0",
+    dd = xp.dd.ul.li.a(href="../commands.md#" + get_id("cmd", "help2", "refs", 0),
                        text="Commands")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="cmd")
     dl = dl.has(dd)
     dl = dl.has(xp.dt.a(text="help2"))
     assert len(pages['commands.md'].xpath(str(dl))) == 1
 
 
@@ -127,12 +129,12 @@
     assert len(pages['commands.md'].xpath(str(dl))) == 1
 
 
 def test_page_ref_link(config):
     pages = mock.render([mycommand, commands], config)
 
     dl = xp.body.p.a(_class="mkdocs-ezglossary-link",
-                     id="cmd_help2_refs_0",
+                     id=get_id("cmd", "help2", "refs", 0),
                      title="page subtitle",
                      href="../mycommand.md#",
                      text="help2")
     assert len(pages['commands.md'].xpath(str(dl))) == 1
```

### Comparing `mkdocs_ezglossary_plugin-1.6.3/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.6.4/tests/test_summary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,119 @@
 import logging
 
 from yaxp import xpath as xp
 
+from mkdocs_ezglossary_plugin.glossary import get_id
+
 import mock
 
 log = logging.getLogger(__name__)
 
 
 def test_summary(simple, summary, config):
     config['inline_refs'] = "short"
     pages = mock.render([simple, summary], config)
     summary = pages["summary.md"]
     log.debug(summary)
 
     # first in test glossary
-    a = xp.a(href="../simple.md#test_first_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("test", "first", "defs", 0),
              text="first")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="test")
     dl = dl.has(xp.dt.has(a))
     assert len(summary.xpath(str(dl))) == 1
 
-    l1 = xp.a(href="../simple.md#test_first_refs_0")
+    l1 = xp.a(href="../simple.md#" + get_id("test", "first", "refs", 0))
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="test")
     dl = dl.has(xp.dl.has(a))
     assert len(summary.xpath(str(dl))) == 0
 
-    a = xp.a(href="../simple.md#test_third_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("test", "third", "defs", 0),
              text="third")
     dd = xp.dd
-    l1 = xp.ul.li.a(href="../simple.md#test_third_refs_0",
+    l1 = xp.ul.li.a(href="../simple.md#" + get_id("test", "third", "refs", 0),
                     text="Hello")
-    l2 = xp.ul.li.a(href="../summary.md#test_third_refs_1",
+    l2 = xp.ul.li.a(href="../summary.md#" + get_id("test", "third", "refs", 1),
                     text="Summary")
     dd = dd.has(l1)
     dd = dd.has(l2)
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="test")
     dl = dl.has(xp.dt.has(a))
     dl = dl.has(dd)
     assert len(summary.xpath(str(dl))) == 1
 
-    a = xp.a(href="../simple.md#demo_first_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("demo", "first", "defs", 0),
              text="first")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="demo")
     dl = dl.has(xp.dt.has(a))
     assert len(summary.xpath(str(dl))) == 1
 
-    a = xp.a(href="../simple.md#demo_third_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("demo", "third", "defs", 0),
              text="third")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="demo")
     dl = dl.has(xp.dt.has(a))
     assert len(summary.xpath(str(dl))) == 1
 
-    a = xp.a(href="../simple.md#demo_third_refs_0",
+    a = xp.a(href="../simple.md#" + get_id("demo", "third", "refs", 0),
              text="third")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="demo")
     dl = dl.has(xp.dd.has(a))
     assert len(summary.xpath(str(dl))) == 0
 
 
 def test_summary_noref(simple, summary, config):
     config['list_references'] = False
     pages = mock.render([simple, summary], config)
     summary = pages["summary.md"]
 
-    a = xp.a(href="../simple.md#test_first_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("test", "first", "defs", 0),
              text="first")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="test")
     dl = dl.has(xp.dt.has(a))
     assert len(summary.xpath(str(dl))) == 1
 
-    a = xp.a(href="../simple.md#test_third_refs_0",
+    a = xp.a(href="../simple.md#" + get_id("test", "third", "refs", 0),
              text="Hello")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="test")
     dl = dl.has(xp.dt(text="third"))
     dl = dl.has(xp.dd.has(a))
     assert len(summary.xpath(str(dl))) == 0
 
 
 def test_custom_summary(simple, summary, config):
     config['templates'] = "tests/custom"
     pages = mock.render([simple, summary], config)
     summary = pages["summary.md"]
 
-    dd = xp.dd.ul.li.a(href="../simple.md#test_third_refs_0",
+    dd = xp.dd.ul.li.a(href="../simple.md#" + get_id("test", "third", "refs", 0),
                        text="Hello")
     dl = xp.dl(_class="custom-summary", _id="test")
     dl = dl.has(xp.dt(text="third"))
     dl = dl.has(dd)
     assert len(summary.xpath(str(dl))) == 1
 
 
 def test_default_summary(simple, summary, config):
     config['use_default'] = True
     pages = mock.render([simple, summary], config)
     summary = pages["summary.md"]
     log.debug(summary)
 
-    a = xp.a(href="../simple.md#__default_defs_0",
+    a = xp.a(href="../simple.md#" + get_id("_", "default", "defs", 0),
              text="default")
     dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="_")
     dl = dl.has(xp.dt.has(a))
     assert len(summary.xpath(str(dl))) == 1
 
+    a = xp.a(href="../simple.md#" + get_id("_", "🚧🚧", "defs", 0),
+             text="🚧🚧")
+    dl = xp.dl(_class="mkdocs-ezglossary-summary", _id="_")
+    dl = dl.has(xp.dt.has(a))
+    assert len(summary.xpath(str(dl))) == 1
+
 
 def test_summary_table(simple, tablesummary, config):
     pages = mock.render([simple, tablesummary], config)
     summary = pages["tablesummary.md"]
     log.debug(summary)
 
     table = xp.div(_class="#mkdocs-ezglossary-summary").table(_id="demo")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

