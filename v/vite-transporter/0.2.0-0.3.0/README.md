# Comparing `tmp/vite_transporter-0.2.0.tar.gz` & `tmp/vite_transporter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.2.0.tar` & `vite_transporter-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.2.0/LICENSE
--rw-r--r--   0        0        0     3718 2024-04-21 15:35:16.830834 vite_transporter-0.2.0/README.md
--rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.2.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.2.0/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 20:38:37.815908 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 20:38:37.816282 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 20:38:37.816137 vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.2.0/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.2.0/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.2.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.2.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.2.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.2.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.2.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-17 18:51:11.871806 vite_transporter-0.2.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.2.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.2.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.2.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.2.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.2.0/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.2.0/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.2.0/requirements/main.txt
--rw-r--r--   0        0        0     2185 2024-04-21 15:41:46.643269 vite_transporter-0.2.0/vite_transporter/__init__.py
--rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.2.0/vite_transporter/_headers.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.2.0/vite_transporter/_html_tags.py
--rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.2.0/vite_transporter/helpers.py
--rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.2.0/vite_transporter/parser.py
--rw-r--r--   0        0        0        0 2024-04-17 15:35:45.579326 vite_transporter-0.2.0/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4555 2024-04-21 15:40:31.645154 vite_transporter-0.2.0/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4629 2024-04-21 15:43:46.126181 vite_transporter-0.2.0/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 vite_transporter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3718 2024-04-21 15:35:16.830834 vite_transporter-0.3.0/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.3.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.3.0/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 20:38:37.815908 vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 20:38:37.816282 vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 20:38:37.816137 vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.3.0/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.3.0/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.3.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.3.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.3.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.3.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.3.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-17 18:51:11.871806 vite_transporter-0.3.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.3.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.3.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.3.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.3.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.3.0/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.3.0/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.3.0/requirements/main.txt
+-rw-r--r--   0        0        0     2185 2024-04-22 20:02:54.680872 vite_transporter-0.3.0/vite_transporter/__init__.py
+-rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.3.0/vite_transporter/_headers.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.3.0/vite_transporter/_html_tags.py
+-rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.3.0/vite_transporter/helpers.py
+-rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.3.0/vite_transporter/parser.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:35:45.579326 vite_transporter-0.3.0/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4555 2024-04-22 20:02:38.939765 vite_transporter-0.3.0/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4629 2024-04-22 20:02:47.164430 vite_transporter-0.3.0/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 vite_transporter-0.3.0/PKG-INFO
```

### Comparing `vite_transporter-0.2.0/.gitignore` & `vite_transporter-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/LICENSE` & `vite_transporter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/README.md` & `vite_transporter-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_flask_demo/__init__.py` & `vite_transporter-0.3.0/app_flask_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.3.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_quart_demo/__init__.py` & `vite_transporter-0.3.0/app_quart_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.3.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/Index.jsx` & `vite_transporter-0.3.0/app_vite_demo/Index.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/__router__.jsx` & `vite_transporter-0.3.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/assets/ili.gif` & `vite_transporter-0.3.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/index.css` & `vite_transporter-0.3.0/app_vite_demo/index.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/package-lock.json` & `vite_transporter-0.3.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/app_vite_demo/package.json` & `vite_transporter-0.3.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/pyproject.toml` & `vite_transporter-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/vite_transporter/__init__.py` & `vite_transporter-0.3.0/vite_transporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from .helpers import Colr as _Colr
 from .helpers import PyProjectConfig as _PyProjectConfig
 from .helpers import _compile
 from .parser import ArgumentParser as _ArgumentParser
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 def _cli():
     pars = _ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
```

### Comparing `vite_transporter-0.2.0/vite_transporter/_headers.py` & `vite_transporter-0.3.0/vite_transporter/_headers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/vite_transporter/_html_tags.py` & `vite_transporter-0.3.0/vite_transporter/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/vite_transporter/helpers.py` & `vite_transporter-0.3.0/vite_transporter/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/vite_transporter/parser.py` & `vite_transporter-0.3.0/vite_transporter/parser.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.2.0/vite_transporter/platform/flask.py` & `vite_transporter-0.3.0/vite_transporter/platform/flask.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     @staticmethod
     def _load_cors_headers(app: Flask, cors_allowed_hosts: t.Optional[list] = None) -> None:
         if cors_allowed_hosts:
             print(
                 f"\n\r{Colr.WARNING}{Colr.BOLD}vite-transporter is disabling CORS restrictions for:"
                 f"{Colr.END}{Colr.END}\n\r"
-                f"{Colr.OKCYAN}{", ".join(cors_allowed_hosts)}{Colr.END}\n\r"
+                f"{Colr.OKCYAN}{', '.join(cors_allowed_hosts)}{Colr.END}\n\r"
             )
 
             @app.after_request
             def after_request(response):
                 response.headers["Access-Control-Allow-Origin"] = ", ".join(cors_allowed_hosts)
                 response.headers["Access-Control-Allow-Headers"] = ", ".join(
                     http_headers
```

### Comparing `vite_transporter-0.2.0/vite_transporter/platform/quart.py` & `vite_transporter-0.3.0/vite_transporter/platform/quart.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     @staticmethod
     def _load_cors_headers(app: Quart, cors_allowed_hosts: t.Optional[list] = None) -> None:
         if cors_allowed_hosts:
             print(
                 f"\n\r{Colr.WARNING}{Colr.BOLD}vite-transporter is disabling CORS restrictions for:"
                 f"{Colr.END}{Colr.END}\n\r"
-                f"{Colr.OKCYAN}{", ".join(cors_allowed_hosts)}{Colr.END}\n\r"
+                f"{Colr.OKCYAN}{', '.join(cors_allowed_hosts)}{Colr.END}\n\r"
             )
 
             @app.after_request
             async def after_request(response):
                 response.headers["Access-Control-Allow-Origin"] = ", ".join(cors_allowed_hosts)
                 response.headers["Access-Control-Allow-Headers"] = ", ".join(
                     http_headers
```

### Comparing `vite_transporter-0.2.0/PKG-INFO` & `vite_transporter-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

