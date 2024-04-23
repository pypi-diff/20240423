# Comparing `tmp/mkdocs_drawio_exporter-0.9.0.tar.gz` & `tmp/mkdocs_drawio_exporter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_drawio_exporter-0.9.0.tar", max compression
+gzip compressed data, was "mkdocs_drawio_exporter-0.9.1.tar", max compression
```

## Comparing `mkdocs_drawio_exporter-0.9.0.tar` & `mkdocs_drawio_exporter-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2022-05-28 16:23:43.820835 mkdocs_drawio_exporter-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     5162 2024-04-20 13:34:58.570127 mkdocs_drawio_exporter-0.9.0/README.md
--rw-r--r--   0        0        0       86 2024-04-03 12:37:18.104252 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/__init__.py
--rw-r--r--   0        0        0    13942 2024-04-20 13:34:58.570948 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/exporter.py
--rw-r--r--   0        0        0     3422 2024-04-20 13:16:29.256842 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/plugin.py
--rw-r--r--   0        0        0       36 2024-04-03 12:37:18.105168 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/tests/__init__.py
--rw-r--r--   0        0        0    12808 2024-04-20 13:16:29.257645 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/tests/exporter.py
--rw-r--r--   0        0        0     1916 2024-04-20 13:34:58.571241 mkdocs_drawio_exporter-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6924 1970-01-01 00:00:00.000000 mkdocs_drawio_exporter-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-03-07 22:31:08.152197 mkdocs_drawio_exporter-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     5162 2024-04-23 20:18:55.177247 mkdocs_drawio_exporter-0.9.1/README.md
+-rw-r--r--   0        0        0       86 2024-04-23 21:11:53.417999 mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/__init__.py
+-rw-r--r--   0        0        0    14022 2024-04-23 21:35:34.821663 mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/exporter.py
+-rw-r--r--   0        0        0     3422 2024-04-23 21:35:34.821958 mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/plugin.py
+-rw-r--r--   0        0        0       36 2024-03-08 00:35:25.135717 mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/tests/__init__.py
+-rw-r--r--   0        0        0    12808 2024-04-23 20:18:55.179247 mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/tests/exporter.py
+-rw-r--r--   0        0        0     1916 2024-04-23 21:35:16.369769 mkdocs_drawio_exporter-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6924 1970-01-01 00:00:00.000000 mkdocs_drawio_exporter-0.9.1/PKG-INFO
```

### Comparing `mkdocs_drawio_exporter-0.9.0/LICENSE.md` & `mkdocs_drawio_exporter-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio_exporter-0.9.0/README.md` & `mkdocs_drawio_exporter-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/exporter.py` & `mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# FIXME: drop once we upgrade to Python 3.9
+from __future__ import annotations
+
 import fnmatch
 import hashlib
 import os.path
 import re
 import shutil
 import subprocess
 import sys
@@ -264,15 +267,15 @@
                 filename = match.group(2)
                 page_index = 0
 
             if fnmatch.fnmatch(filename, config["sources"]):
                 source = Source(filename, page_index)
                 source.resolve_rel_path(page_dest_path)
                 content_sources.append(source)
-                img_src = f"{filename}-{page_index}.{config["format"]}"
+                img_src = f"{filename}-{page_index}.{config['format']}"
 
                 # Cache the file on-demand and read file content only if we
                 # need to inline the file's content.
                 content = None
                 if "{content}" in config["embed_format"]:
                     img_path = self.make_cache_filename(
                             source.source_rel, page_index, config['cache_dir'])
```

### Comparing `mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/plugin.py` & `mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
                     self.exporter.drawio_executable_paths(sys.platform))
             self.exporter.validate_config(self.config)
         except ConfigurationError as e:
             raise mkdocs.exceptions.ConfigurationError(str(e))
 
         os.makedirs(self.config['cache_dir'], exist_ok=True)
 
-        log.debug(f'Using Draw.io executable "{self.config['drawio_executable']}", '
-                f'arguments {self.config['drawio_args']} and '
-                f'cache directory "{self.config['cache_dir']}"')
+        log.debug(f'Using Draw.io executable "{self.config["drawio_executable"]}", '
+                f'arguments {self.config["drawio_args"]} and '
+                f'cache directory "{self.config["cache_dir"]}"')
 
     def on_post_page(self, output_content, page, **kwargs):
         output_content, content_sources = self.exporter.rewrite_image_embeds(
                 page.file.dest_path, output_content, self.config)
 
         self.sources += content_sources
 
@@ -69,15 +69,15 @@
 
     def on_post_build(self, config):
         sources = set(self.sources)
         log.debug(f'Found {len(sources)} unique sources in {len(self.sources)} total embeds')
         self.sources = []
 
         for source in sources:
-            dest_rel_path = f'{source.source_rel}-{source.page_index}.{self.config['format']}'
+            dest_rel_path = f'{source.source_rel}-{source.page_index}.{self.config["format"]}'
             abs_src_path = os.path.join(config['docs_dir'], source.source_rel)
             abs_dest_path = os.path.join(config['site_dir'], dest_rel_path)
             cache_filename, exit_status = self.exporter.ensure_file_cached(
                     abs_src_path, source.source_rel, source.page_index,
                     self.config)
 
             if exit_status not in (None, 0):
```

### Comparing `mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/tests/exporter.py` & `mkdocs_drawio_exporter-0.9.1/mkdocs_drawio_exporter/tests/exporter.py`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio_exporter-0.9.0/pyproject.toml` & `mkdocs_drawio_exporter-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-drawio-exporter"
-version = "0.9.0"
+version = "0.9.1"
 description = "Exports your Draw.io diagrams at build time for easier embedding into your documentation"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Luke Carrier <luke@carrier.family>",
 ]
 classifiers = [
```

### Comparing `mkdocs_drawio_exporter-0.9.0/PKG-INFO` & `mkdocs_drawio_exporter-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-drawio-exporter
-Version: 0.9.0
+Version: 0.9.1
 Summary: Exports your Draw.io diagrams at build time for easier embedding into your documentation
 License: MIT
 Author: Luke Carrier
 Author-email: luke@carrier.family
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

