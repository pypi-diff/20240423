# Comparing `tmp/wagtail_tabbed_structblock-0.0.1.tar.gz` & `tmp/wagtail_tabbed_structblock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_tabbed_structblock-0.0.1.tar", max compression
+gzip compressed data, was "wagtail_tabbed_structblock-0.0.3.tar", max compression
```

## Comparing `wagtail_tabbed_structblock-0.0.1.tar` & `wagtail_tabbed_structblock-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0        0 2024-04-23 18:04:33.500137 wagtail_tabbed_structblock-0.0.1/README.md
--rw-r--r--   0        0        0      346 2024-04-23 18:08:41.599871 wagtail_tabbed_structblock-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 18:02:39.561604 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/README.md
--rw-r--r--   0        0        0        0 2024-04-23 17:44:19.860863 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/__init__.py
--rw-r--r--   0        0        0      167 2024-04-23 17:48:07.039507 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/apps.py
--rw-r--r--   0        0        0     1099 2024-04-23 17:53:37.806194 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/blocks.py
--rw-r--r--   0        0        0        0 2024-04-23 17:44:19.862839 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/migrations/__init__.py
--rw-r--r--   0        0        0    48673 2024-04-23 18:02:59.482390 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/poetry.lock
--rw-r--r--   0        0        0      436 2024-04-23 18:03:01.848431 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/pyproject.toml
--rw-r--r--   0        0        0      377 2024-04-23 18:00:45.553282 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/setup.py
--rw-r--r--   0        0        0      722 2024-04-23 17:46:28.930942 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
--rw-r--r--   0        0        0     1554 2024-04-23 17:46:28.931320 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
--rw-r--r--   0        0        0     1507 2024-04-04 20:27:49.738349 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
--rw-r--r--   0        0        0       60 2024-04-23 17:44:19.862666 wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/tests.py
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.1/setup.py
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/README.md
+-rw-r--r--   0        0        0      346 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/apps.py
+-rw-r--r--   0        0        0     1099 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/blocks.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/migrations/__init__.py
+-rw-r--r--   0        0        0    48673 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/poetry.lock
+-rw-r--r--   0        0        0      436 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/pyproject.toml
+-rw-r--r--   0        0        0      377 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/setup.py
+-rw-r--r--   0        0        0      722 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
+-rw-r--r--   0        0        0     1554 2024-04-23 19:50:44.188122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
+-rw-r--r--   0        0        0     1507 2024-04-23 19:50:44.192122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
+-rw-r--r--   0        0        0       60 2024-04-23 19:50:44.192122 wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/tests.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.3/PKG-INFO
```

### Comparing `wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/blocks.py` & `wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/poetry.lock` & `wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/poetry.lock`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css` & `wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js` & `wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.1/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html` & `wagtail_tabbed_structblock-0.0.3/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html`

 * *Files identical despite different names*

