# Comparing `tmp/md2weasypdf-0.0.4.tar.gz` & `tmp/md2weasypdf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.4.tar", last modified: Mon Apr 22 06:03:29 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.5.tar", last modified: Tue Apr 23 06:20:04 2024, max compression
```

## Comparing `md2weasypdf-0.0.4.tar` & `md2weasypdf-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/toa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 06:03:29.000000 md2weasypdf-0.0.4/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 06:03:29.453976 md2weasypdf-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 06:03:25.000000 md2weasypdf-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/setup.py
```

### Comparing `md2weasypdf-0.0.4/LICENSE` & `md2weasypdf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/PKG-INFO` & `md2weasypdf-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.4/README.md` & `md2weasypdf-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/__main__.py` & `md2weasypdf-0.0.5/md2weasypdf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.5/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/extensions/footnotes.py` & `md2weasypdf-0.0.5/md2weasypdf/extensions/footnotes.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.5/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/extensions/toa.py` & `md2weasypdf-0.0.5/md2weasypdf/extensions/toa.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.5/md2weasypdf/extensions/toc.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/md2weasypdf/printer.py` & `md2weasypdf-0.0.5/md2weasypdf/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         self._load_template.cache_clear()
         articles: List[Article] = []
         if self.input.is_dir():
             for article_path in sorted(iglob(os.path.join(self.input, "**/*.md"), recursive=True)):
                 if os.path.basename(article_path).startswith("_"):
                     continue
 
-                if self.filename_filter and not re.search(self.filename_filter, article_path):
+                if self.filename_filter and not re.search(self.filename_filter, Path(article_path).relative_to(self.input).as_posix()):
                     continue
 
                 articles.append(self._load_article(article_path))
 
         else:
             articles.append(self._load_article(self.input))
```

### Comparing `md2weasypdf-0.0.4/md2weasypdf.egg-info/PKG-INFO` & `md2weasypdf-0.0.5/md2weasypdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.4/md2weasypdf.egg-info/SOURCES.txt` & `md2weasypdf-0.0.5/md2weasypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.4/setup.cfg` & `md2weasypdf-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.4
+version = 0.0.5
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```

