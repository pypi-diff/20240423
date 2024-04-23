# Comparing `tmp/sphinxawesome_theme-5.1.3.tar.gz` & `tmp/sphinxawesome_theme-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.1.3.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.1.4.tar", max compression
```

## Comparing `sphinxawesome_theme-5.1.3.tar` & `sphinxawesome_theme-5.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2024-04-18 12:40:01.359816 sphinxawesome_theme-5.1.3/LICENSE
--rw-r--r--   0        0        0     2294 2024-04-18 12:40:01.359816 sphinxawesome_theme-5.1.3/README.md
--rw-r--r--   0        0        0     2682 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/pyproject.toml
--rw-r--r--   0        0        0     7311 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     4166 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     1394 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2841 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/genindex.html
--rw-r--r--   0        0        0     7675 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12751 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1013 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1192 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5135 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3242 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7816 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      932 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1226 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    30104 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff
--rw-r--r--   0        0        0    21956 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
--rw-r--r--   0        0        0    21088 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
--rw-r--r--   0        0        0    28620 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
--rw-r--r--   0        0        0    23072 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
--rw-r--r--   0        0        0    23148 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
--rw-r--r--   0        0        0    30232 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
--rw-r--r--   0        0        0    29416 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
--rw-r--r--   0        0        0    28636 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
--rw-r--r--   0        0        0    22188 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
--rw-r--r--   0        0        0    21820 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
--rw-r--r--   0        0        0     4495 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.css
--rw-r--r--   0        0        0        0 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.js
--rw-r--r--   0        0        0     1338 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.css
--rw-r--r--   0        0        0        0 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.js
--rw-r--r--   0        0        0    27896 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
--rw-r--r--   0        0        0    49649 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.css
--rw-r--r--   0        0        0    55861 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js
--rw-r--r--   0        0        0       93 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      358 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2369 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-23 15:22:40.387702 sphinxawesome_theme-5.1.4/LICENSE
+-rw-r--r--   0        0        0     2294 2024-04-23 15:22:40.387702 sphinxawesome_theme-5.1.4/README.md
+-rw-r--r--   0        0        0     2682 2024-04-23 15:22:40.391702 sphinxawesome_theme-5.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7311 2024-04-23 15:22:40.391702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     4166 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     1394 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2841 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/genindex.html
+-rw-r--r--   0        0        0     7675 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12751 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1013 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1192 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5135 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3242 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7816 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      932 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1226 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    21956 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
+-rw-r--r--   0        0        0    30184 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
+-rw-r--r--   0        0        0    21088 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
+-rw-r--r--   0        0        0    28620 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
+-rw-r--r--   0        0        0    23072 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
+-rw-r--r--   0        0        0    23148 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
+-rw-r--r--   0        0        0    30232 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
+-rw-r--r--   0        0        0    29416 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
+-rw-r--r--   0        0        0    28636 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
+-rw-r--r--   0        0        0    22188 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
+-rw-r--r--   0        0        0    21820 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
+-rw-r--r--   0        0        0     4495 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.css
+-rw-r--r--   0        0        0        0 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.js
+-rw-r--r--   0        0        0     1338 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.css
+-rw-r--r--   0        0        0        0 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.js
+-rw-r--r--   0        0        0    27896 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
+-rw-r--r--   0        0        0    49637 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.css
+-rw-r--r--   0        0        0    56143 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js
+-rw-r--r--   0        0        0       93 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      353 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2369 2024-04-23 15:22:40.395702 sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.4/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.1.3/LICENSE` & `sphinxawesome_theme-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/README.md` & `sphinxawesome_theme-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/pyproject.toml` & `sphinxawesome_theme-5.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.1.3"
+version = "5.1.4"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -46,15 +46,15 @@
 mypy = "^1.0"
 
 [tool.poetry.group.lint.dependencies]
 pre-commit = [
   { version = "^3.5", python = ">=3.8,<3.9"},
   { version = "^3.6", python = ">=3.9,<=3.12"},
 ]
-ruff = ">=0.0.269,<0.3.8"
+ruff = ">=0.0.269,<0.4.2"
 
 [tool.poetry.group.netlify.dependencies]
 nox = {version = ">=2023.4.22,<2025.0.0", python = "3.8"}
 poetry = {version = "^1.4.2", python = "3.8"}
 pipx = {version = "^1.2.0", python = "3.8"}
 pip = {version = ">=23.1.2,<25.0.0", python = "3.8"}
```

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/deprecated.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/genindex.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/logos.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.css` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.css` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/awesome-sphinx-design.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.css` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(a1e4997bd1fb9d7822e1.woff2) format("woff2"),url(70e1dc5f5622381d6e9e.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(2fe080a3bf49bdc12fcb.woff2) format("woff2"),url(c226d7283d0d52c2d32c.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:500;src:url(4f183a25813446a47ad9.woff2) format("woff2"),url(63a0f5d460fb58135365.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(a61d04152f1635036f0d.woff2) format("woff2"),url(39bd78ffb50669d6855a.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(5f68b8c26e28d783a591.woff2) format("woff2"),url(06b2bbbc4b7413514f6a.woff) format("woff")}
+@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(5f68b8c26e28d783a591.woff2) format("woff2"),url(1d5fc702ab9000c3247a.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:700;src:url(0fecf1cc5677455886b4.woff2) format("woff2"),url(84504970850f0632d9c3.woff) format("woff")}
-/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-tap-highlight-color:transparent}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-feature-settings:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;letter-spacing:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e1e7ef;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p:first-child{margin-top:0}#content section>p.lead{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a.viewcode-back{color:#65758b!important;color:hsl(var(--muted-foreground))!important;position:absolute;right:0}#content a:not(.toc-backref){color:#0f1729;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#65758b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}table th:is(.dark *){font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f1729;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;border-color:#0284c7;border-color:rgba(2,132,199,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0f9ff;background-color:rgba(240,249,255,var(--tw-bg-opacity));--tw-text-opacity:1;color:#0c4a6e;color:rgba(12,74,110,var(--tw-text-opacity))}.dark .note{background-color:rgba(96,165,250,.15);--tw-text-opacity:1;color:#e0f2fe;color:rgba(224,242,254,var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0fdf4;background-color:rgba(240,253,244,var(--tw-bg-opacity));--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark .hint,.dark .tip{background-color:rgba(74,222,128,.15);--tw-text-opacity:1;color:#dcfce7;color:rgba(220,252,231,var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fef2f2;background-color:rgba(254,242,242,var(--tw-bg-opacity));--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark .danger,.dark .error{background-color:hsla(0,91%,71%,.15);--tw-text-opacity:1;color:#fee2e2;color:rgba(254,226,226,var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fefce8;background-color:rgba(254,252,232,var(--tw-bg-opacity));--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{background-color:rgba(250,204,21,.15);--tw-text-opacity:1;color:#fef9c3;color:rgba(254,249,195,var(--tw-text-opacity))}div.versionadded{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{font-weight:500;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}div.versionadded .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#22c55e;color:rgba(34,197,94,var(--tw-text-opacity))}div.versionchanged{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{font-weight:500;--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}div.versionchanged .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#eab308;color:rgba(234,179,8,var(--tw-text-opacity))}div.deprecated{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{font-weight:500;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}div.deprecated .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#f87171;color:rgba(248,113,113,var(--tw-text-opacity))}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.highlight .gp,.highlight-pycon .go,.highlight-python .go{-webkit-user-select:none;-moz-user-select:none;user-select:none}.literal-block-wrapper{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2em .3em;position:relative;white-space:nowrap}code .ge,code em{color:#0f1729;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}:where(h1,h2,h3,h4,h5,h6) code{font-size:inherit}pre{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgba(255,255,255,var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{background-color:#f1f5f9;background-color:hsl(var(--muted));color:inherit;--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] mark:is(.dark *){--tw-bg-opacity:1;background-color:#334155;background-color:rgba(51,65,85,var(--tw-bg-opacity));--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] ins{background-color:rgba(34,197,94,.3);--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{left:2px;position:absolute;--tw-content:"\002b";content:"\002b";content:var(--tw-content)}pre code [id^=line-] ins:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}pre code [id^=line-] del{background-color:rgba(239,68,68,.3);--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{left:2px;position:absolute;--tw-content:"\2212";content:"\2212";content:var(--tw-content)}pre code [id^=line-] del:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgba(254,202,202,var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{background-color:rgba(34,197,94,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.highlight-diff .gi:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.highlight-diff .gd{background-color:rgba(239,68,68,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.highlight-diff .gd:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{border-color:#e1e7ef;border-color:hsl(var(--border));border-top-width:1px;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;padding-top:1.5rem;scroll-margin:5rem}.sig-name{color:#0f1729;color:hsl(var(--accent-foreground))}em.property{color:#65758b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#65758b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{visibility:hidden;fill:currentColor;color:#65758b;color:hsl(var(--muted-foreground))}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{bottom:.25rem;left:0;position:absolute;top:.25rem;width:1px;--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgba(229,231,235,var(--tw-bg-opacity));--tw-content:"";content:"";content:var(--tw-content)}#left-sidebar ul ul:is(.dark *):before{content:var(--tw-content);--tw-bg-opacity:1;background-color:#262626;background-color:rgba(38,38,38,var(--tw-bg-opacity))}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#65758b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,41,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e1e7ef;border-color:hsl(var(--border));border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#65758b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f1729;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f1729;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#65758b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f1729;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px;clip:rect(0,0,0,0);border-width:0;white-space:nowrap}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.max-h-\[calc\(var\(100vh\)-5rem\)\]{max-height:calc(var(100vh) - 5rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e1e7ef;border-color:hsl(var(--border))}.border-input{border-color:#e1e7ef;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgba(55,65,81,var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-2{padding-top:.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f1729;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,41,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#65758b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgba(185,28,28,var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgba(255,255,255,var(--tw-text-opacity))}.underline{text-decoration-line:underline}.no-underline{text-decoration-line:none}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f1729;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,41,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f1729;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:outline-offset-\[-1px\]:focus-visible{outline-offset:-1px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f1729;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
+/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-tap-highlight-color:transparent}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-feature-settings:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;letter-spacing:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e1e7ef;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p:first-child{margin-top:0}#content section>p.lead{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a.viewcode-back{color:#65758b!important;color:hsl(var(--muted-foreground))!important;position:absolute;right:0}#content a:not(.toc-backref){color:#0f1729;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#65758b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}table th:is(.dark *){font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f1729;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;border-color:#0284c7;border-color:rgba(2,132,199,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0f9ff;background-color:rgba(240,249,255,var(--tw-bg-opacity));--tw-text-opacity:1;color:#0c4a6e;color:rgba(12,74,110,var(--tw-text-opacity))}.dark .note{background-color:rgba(96,165,250,.15);--tw-text-opacity:1;color:#e0f2fe;color:rgba(224,242,254,var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0fdf4;background-color:rgba(240,253,244,var(--tw-bg-opacity));--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark .hint,.dark .tip{background-color:rgba(74,222,128,.15);--tw-text-opacity:1;color:#dcfce7;color:rgba(220,252,231,var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fef2f2;background-color:rgba(254,242,242,var(--tw-bg-opacity));--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark .danger,.dark .error{background-color:hsla(0,91%,71%,.15);--tw-text-opacity:1;color:#fee2e2;color:rgba(254,226,226,var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fefce8;background-color:rgba(254,252,232,var(--tw-bg-opacity));--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{background-color:rgba(250,204,21,.15);--tw-text-opacity:1;color:#fef9c3;color:rgba(254,249,195,var(--tw-text-opacity))}div.versionadded{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{font-weight:500;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}div.versionadded .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#22c55e;color:rgba(34,197,94,var(--tw-text-opacity))}div.versionchanged{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{font-weight:500;--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}div.versionchanged .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#eab308;color:rgba(234,179,8,var(--tw-text-opacity))}div.deprecated{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{font-weight:500;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}div.deprecated .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#f87171;color:rgba(248,113,113,var(--tw-text-opacity))}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.highlight .gp,.highlight-pycon .go,.highlight-python .go{-webkit-user-select:none;-moz-user-select:none;user-select:none}.literal-block-wrapper{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2em .3em;position:relative;white-space:nowrap}code .ge,code em{color:#0f1729;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}:where(h1,h2,h3,h4,h5,h6) code{font-size:inherit}pre{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgba(255,255,255,var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{background-color:#f1f5f9;background-color:hsl(var(--muted));color:inherit;--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] mark:is(.dark *){--tw-bg-opacity:1;background-color:#334155;background-color:rgba(51,65,85,var(--tw-bg-opacity));--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] ins{background-color:rgba(34,197,94,.3);--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{left:2px;position:absolute;--tw-content:"\002b";content:"\002b";content:var(--tw-content)}pre code [id^=line-] ins:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}pre code [id^=line-] del{background-color:rgba(239,68,68,.3);--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{left:2px;position:absolute;--tw-content:"\2212";content:"\2212";content:var(--tw-content)}pre code [id^=line-] del:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgba(254,202,202,var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{background-color:rgba(34,197,94,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.highlight-diff .gi:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.highlight-diff .gd{background-color:rgba(239,68,68,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.highlight-diff .gd:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{border-color:#e1e7ef;border-color:hsl(var(--border));border-top-width:1px;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;padding-top:1.5rem;scroll-margin:5rem}.sig-name{color:#0f1729;color:hsl(var(--accent-foreground))}em.property{color:#65758b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#65758b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{visibility:hidden;fill:currentColor;color:#65758b;color:hsl(var(--muted-foreground))}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{bottom:.25rem;left:0;position:absolute;top:.25rem;width:1px;--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgba(229,231,235,var(--tw-bg-opacity));--tw-content:"";content:"";content:var(--tw-content)}#left-sidebar ul ul:is(.dark *):before{content:var(--tw-content);--tw-bg-opacity:1;background-color:#262626;background-color:rgba(38,38,38,var(--tw-bg-opacity))}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#65758b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,41,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e1e7ef;border-color:hsl(var(--border));border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#65758b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f1729;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f1729;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#65758b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f1729;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px;clip:rect(0,0,0,0);border-width:0;white-space:nowrap}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(100vh-5rem\)\]{max-height:calc(100vh - 5rem)}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e1e7ef;border-color:hsl(var(--border))}.border-input{border-color:#e1e7ef;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgba(55,65,81,var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-2{padding-top:.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f1729;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,41,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#65758b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgba(185,28,28,var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgba(255,255,255,var(--tw-text-opacity))}.underline{text-decoration-line:underline}.no-underline{text-decoration-line:none}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f1729;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,41,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f1729;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:outline-offset-\[-1px\]:focus-visible{outline-offset:-1px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f1729;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
```

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/static/theme.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -461,150 +461,71 @@
                         let i = e();
                         JSON.stringify(i), r ? n = i : queueMicrotask((() => {
                             t(i, n), n = i
                         })), r = !1
                     }));
                 return () => a(i)
             }
+            var v = [],
+                m = [],
+                g = [];
 
-            function v(e, t, n = {}) {
-                e.dispatchEvent(new CustomEvent(t, {
-                    detail: n,
-                    bubbles: !0,
-                    composed: !0,
-                    cancelable: !0
-                }))
-            }
-
-            function m(e, t) {
-                if ("function" == typeof ShadowRoot && e instanceof ShadowRoot) return void Array.from(e.children).forEach((e => m(e, t)));
-                let n = !1;
-                if (t(e, (() => n = !0)), n) return;
-                let r = e.firstElementChild;
-                for (; r;) m(r, t), r = r.nextElementSibling
-            }
-
-            function g(e, ...t) {
-                console.warn(`Alpine Warning: ${e}`, ...t)
-            }
-            var x = !1,
-                b = [],
-                w = [];
-
-            function E() {
-                return b.map((e => e()))
-            }
-
-            function S() {
-                return b.concat(w).map((e => e()))
-            }
-
-            function A(e) {
-                b.push(e)
-            }
-
-            function O(e) {
-                w.push(e)
-            }
-
-            function k(e, t = !1) {
-                return j(e, (e => {
-                    if ((t ? S() : E()).some((t => e.matches(t)))) return !0
-                }))
-            }
-
-            function j(e, t) {
-                if (e) {
-                    if (t(e)) return e;
-                    if (e._x_teleportBack && (e = e._x_teleportBack), e.parentElement) return j(e.parentElement, t)
-                }
-            }
-            var C = [];
-
-            function T(e, t = m, n = (() => {})) {
-                ! function(r) {
-                    we = !0;
-                    let i = Symbol();
-                    Se = i, Ee.set(i, []);
-                    let o = () => {
-                        for (; Ee.get(i).length;) Ee.get(i).shift()();
-                        Ee.delete(i)
-                    };
-                    t(e, ((e, t) => {
-                        n(e, t), C.forEach((n => n(e, t))), xe(e, e.attributes).forEach((e => e())), e._x_ignore && t()
-                    })), we = !1, o()
-                }()
-            }
-
-            function L(e, t = m) {
-                t(e, (e => {
-                    I(e),
-                        function(e) {
-                            if (e._x_cleanups)
-                                for (; e._x_cleanups.length;) e._x_cleanups.pop()()
-                        }(e)
-                }))
+            function x(e, t) {
+                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, m.push(t))
             }
-            var $ = [],
-                M = [],
-                N = [];
 
-            function P(e, t) {
-                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, M.push(t))
+            function b(e) {
+                v.push(e)
             }
 
-            function R(e) {
-                $.push(e)
-            }
-
-            function q(e, t, n) {
+            function w(e, t, n) {
                 e._x_attributeCleanups || (e._x_attributeCleanups = {}), e._x_attributeCleanups[t] || (e._x_attributeCleanups[t] = []), e._x_attributeCleanups[t].push(n)
             }
 
-            function I(e, t) {
+            function E(e, t) {
                 e._x_attributeCleanups && Object.entries(e._x_attributeCleanups).forEach((([n, r]) => {
                     (void 0 === t || t.includes(n)) && (r.forEach((e => e())), delete e._x_attributeCleanups[n])
                 }))
             }
-            var D = new MutationObserver(K),
-                z = !1;
+            var S = new MutationObserver(L),
+                A = !1;
 
-            function B() {
-                D.observe(document, {
+            function O() {
+                S.observe(document, {
                     subtree: !0,
                     childList: !0,
                     attributes: !0,
                     attributeOldValue: !0
-                }), z = !0
+                }), A = !0
             }
 
-            function F() {
+            function k() {
                 ! function() {
-                    let e = D.takeRecords();
-                    H.push((() => e.length > 0 && K(e)));
-                    let t = H.length;
+                    let e = S.takeRecords();
+                    j.push((() => e.length > 0 && L(e)));
+                    let t = j.length;
                     queueMicrotask((() => {
-                        if (H.length === t)
-                            for (; H.length > 0;) H.shift()()
+                        if (j.length === t)
+                            for (; j.length > 0;) j.shift()()
                     }))
-                }(), D.disconnect(), z = !1
+                }(), S.disconnect(), A = !1
             }
-            var H = [];
+            var j = [];
 
-            function W(e) {
-                if (!z) return e();
-                F();
+            function C(e) {
+                if (!A) return e();
+                k();
                 let t = e();
-                return B(), t
+                return O(), t
             }
-            var V = !1,
-                U = [];
+            var T = !1,
+                $ = [];
 
-            function K(e) {
-                if (V) return void(U = U.concat(e));
+            function L(e) {
+                if (T) return void($ = $.concat(e));
                 let t = new Set,
                     n = new Set,
                     r = new Map,
                     i = new Map;
                 for (let o = 0; o < e.length; o++)
                     if (!e[o].target._x_ignoreMutationObserver && ("childList" === e[o].type && (e[o].addedNodes.forEach((e => 1 === e.nodeType && t.add(e))), e[o].removedNodes.forEach((e => 1 === e.nodeType && n.add(e)))), "attributes" === e[o].type)) {
                         let t = e[o].target,
@@ -617,77 +538,77 @@
                                 })
                             },
                             l = () => {
                                 i.has(t) || i.set(t, []), i.get(t).push(n)
                             };
                         t.hasAttribute(n) && null === a ? s() : t.hasAttribute(n) ? (l(), s()) : l()
                     } i.forEach(((e, t) => {
-                    I(t, e)
+                    E(t, e)
                 })), r.forEach(((e, t) => {
-                    $.forEach((n => n(t, e)))
+                    v.forEach((n => n(t, e)))
                 }));
-                for (let e of n) t.has(e) || (M.forEach((t => t(e))), L(e));
+                for (let e of n) t.has(e) || m.forEach((t => t(e)));
                 t.forEach((e => {
                     e._x_ignoreSelf = !0, e._x_ignore = !0
                 }));
-                for (let e of t) n.has(e) || e.isConnected && (delete e._x_ignoreSelf, delete e._x_ignore, N.forEach((t => t(e))), e._x_ignore = !0, e._x_ignoreSelf = !0);
+                for (let e of t) n.has(e) || e.isConnected && (delete e._x_ignoreSelf, delete e._x_ignore, g.forEach((t => t(e))), e._x_ignore = !0, e._x_ignoreSelf = !0);
                 t.forEach((e => {
                     delete e._x_ignoreSelf, delete e._x_ignore
                 })), t = null, n = null, r = null, i = null
             }
 
-            function Z(e) {
-                return Y(X(e))
+            function M(e) {
+                return R(P(e))
             }
 
-            function J(e, t, n) {
-                return e._x_dataStack = [t, ...X(n || e)], () => {
+            function N(e, t, n) {
+                return e._x_dataStack = [t, ...P(n || e)], () => {
                     e._x_dataStack = e._x_dataStack.filter((e => e !== t))
                 }
             }
 
-            function X(e) {
-                return e._x_dataStack ? e._x_dataStack : "function" == typeof ShadowRoot && e instanceof ShadowRoot ? X(e.host) : e.parentNode ? X(e.parentNode) : []
+            function P(e) {
+                return e._x_dataStack ? e._x_dataStack : "function" == typeof ShadowRoot && e instanceof ShadowRoot ? P(e.host) : e.parentNode ? P(e.parentNode) : []
             }
 
-            function Y(e) {
+            function R(e) {
                 return new Proxy({
                     objects: e
-                }, G)
+                }, q)
             }
-            var G = {
+            var q = {
                 ownKeys({
                     objects: e
                 }) {
                     return Array.from(new Set(e.flatMap((e => Object.keys(e)))))
                 },
                 has({
                     objects: e
                 }, t) {
                     return t != Symbol.unscopables && e.some((e => Object.prototype.hasOwnProperty.call(e, t) || Reflect.has(e, t)))
                 },
                 get({
                     objects: e
                 }, t, n) {
-                    return "toJSON" == t ? Q : Reflect.get(e.find((e => Reflect.has(e, t))) || {}, t, n)
+                    return "toJSON" == t ? I : Reflect.get(e.find((e => Reflect.has(e, t))) || {}, t, n)
                 },
                 set({
                     objects: e
                 }, t, n, r) {
                     const i = e.find((e => Object.prototype.hasOwnProperty.call(e, t))) || e[e.length - 1],
                         o = Object.getOwnPropertyDescriptor(i, t);
                     return o?.set && o?.get ? Reflect.set(i, t, n, r) : Reflect.set(i, t, n)
                 }
             };
 
-            function Q() {
+            function I() {
                 return Reflect.ownKeys(this).reduce(((e, t) => (e[t] = Reflect.get(this, t), e)), {})
             }
 
-            function ee(e) {
+            function D(e) {
                 let t = (n, r = "") => {
                     Object.entries(Object.getOwnPropertyDescriptors(n)).forEach((([i, {
                         value: o,
                         enumerable: a
                     }]) => {
                         if (!1 === a || void 0 === o) return;
                         if ("object" == typeof o && null !== o && o.__v_skip) return;
@@ -695,226 +616,226 @@
                         var l;
                         "object" == typeof o && null !== o && o._x_interceptor ? n[i] = o.initialize(e, s, i) : "object" != typeof(l = o) || Array.isArray(l) || null === l || o === n || o instanceof Element || t(o, s)
                     }))
                 };
                 return t(e)
             }
 
-            function te(e, t = (() => {})) {
+            function z(e, t = (() => {})) {
                 let n = {
                     initialValue: void 0,
                     _x_interceptor: !0,
                     initialize(t, n, r) {
                         return e(this.initialValue, (() => function(e, t) {
                             return t.split(".").reduce(((e, t) => e[t]), e)
-                        }(t, n)), (e => ne(t, n, e)), n, r)
+                        }(t, n)), (e => B(t, n, e)), n, r)
                     }
                 };
                 return t(n), e => {
                     if ("object" == typeof e && null !== e && e._x_interceptor) {
                         let t = n.initialize.bind(n);
                         n.initialize = (r, i, o) => {
                             let a = e.initialize(r, i, o);
                             return n.initialValue = a, t(r, i, o)
                         }
                     } else n.initialValue = e;
                     return n
                 }
             }
 
-            function ne(e, t, n) {
+            function B(e, t, n) {
                 if ("string" == typeof t && (t = t.split(".")), 1 !== t.length) {
                     if (0 === t.length) throw error;
-                    return e[t[0]] || (e[t[0]] = {}), ne(e[t[0]], t.slice(1), n)
+                    return e[t[0]] || (e[t[0]] = {}), B(e[t[0]], t.slice(1), n)
                 }
                 e[t[0]] = n
             }
-            var re = {};
+            var F = {};
 
-            function ie(e, t) {
-                re[e] = t
+            function H(e, t) {
+                F[e] = t
             }
 
-            function oe(e, t) {
-                return Object.entries(re).forEach((([n, r]) => {
+            function W(e, t) {
+                return Object.entries(F).forEach((([n, r]) => {
                     let i = null;
                     Object.defineProperty(e, `$${n}`, {
                         get() {
                             return r(t, function() {
                                 if (i) return i;
                                 {
-                                    let [e, n] = Ae(t);
+                                    let [e, n] = ue(t);
                                     return i = {
-                                        interceptor: te,
+                                        interceptor: z,
                                         ...e
-                                    }, P(t, n), i
+                                    }, x(t, n), i
                                 }
                             }())
                         },
                         enumerable: !1
                     })
                 })), e
             }
 
-            function ae(e, t, n, ...r) {
+            function V(e, t, n, ...r) {
                 try {
                     return n(...r)
                 } catch (n) {
-                    se(n, e, t)
+                    U(n, e, t)
                 }
             }
 
-            function se(e, t, n = void 0) {
+            function U(e, t, n = void 0) {
                 e = Object.assign(e ?? {
                     message: "No error message given."
                 }, {
                     el: t,
                     expression: n
                 }), console.warn(`Alpine Expression Error: ${e.message}\n\n${n?'Expression: "'+n+'"\n\n':""}`, t), setTimeout((() => {
                     throw e
                 }), 0)
             }
-            var le = !0;
+            var K = !0;
 
-            function ce(e) {
-                let t = le;
-                le = !1;
+            function Z(e) {
+                let t = K;
+                K = !1;
                 let n = e();
-                return le = t, n
+                return K = t, n
             }
 
-            function ue(e, t, n = {}) {
+            function J(e, t, n = {}) {
                 let r;
-                return fe(e, t)((e => r = e), n), r
+                return X(e, t)((e => r = e), n), r
             }
 
-            function fe(...e) {
-                return de(...e)
+            function X(...e) {
+                return Y(...e)
             }
-            var de = pe;
+            var Y = G;
 
-            function pe(e, t) {
+            function G(e, t) {
                 let n = {};
-                oe(n, e);
-                let r = [n, ...X(e)],
+                W(n, e);
+                let r = [n, ...P(e)],
                     i = "function" == typeof t ? function(e, t) {
                         return (n = (() => {}), {
                             scope: r = {},
                             params: i = []
                         } = {}) => {
-                            he(n, t.apply(Y([r, ...e]), i))
+                            ee(n, t.apply(R([r, ...e]), i))
                         }
                     }(r, t) : function(e, t, n) {
                         let r = function(e, t) {
-                            if (_e[e]) return _e[e];
+                            if (Q[e]) return Q[e];
                             let n = Object.getPrototypeOf((async function() {})).constructor,
                                 r = /^[\n\s]*if.*\(.*\)/.test(e.trim()) || /^(let|const)\s/.test(e.trim()) ? `(async()=>{ ${e} })()` : e;
                             let i = (() => {
                                 try {
                                     let t = new n(["__self", "scope"], `with (scope) { __self.result = ${r} }; __self.finished = true; return __self.result;`);
                                     return Object.defineProperty(t, "name", {
                                         value: `[Alpine] ${e}`
                                     }), t
                                 } catch (n) {
-                                    return se(n, t, e), Promise.resolve()
+                                    return U(n, t, e), Promise.resolve()
                                 }
                             })();
-                            return _e[e] = i, i
+                            return Q[e] = i, i
                         }(t, n);
                         return (i = (() => {}), {
                             scope: o = {},
                             params: a = []
                         } = {}) => {
                             r.result = void 0, r.finished = !1;
-                            let s = Y([o, ...e]);
+                            let s = R([o, ...e]);
                             if ("function" == typeof r) {
-                                let e = r(r, s).catch((e => se(e, n, t)));
-                                r.finished ? (he(i, r.result, s, a, n), r.result = void 0) : e.then((e => {
-                                    he(i, e, s, a, n)
-                                })).catch((e => se(e, n, t))).finally((() => r.result = void 0))
+                                let e = r(r, s).catch((e => U(e, n, t)));
+                                r.finished ? (ee(i, r.result, s, a, n), r.result = void 0) : e.then((e => {
+                                    ee(i, e, s, a, n)
+                                })).catch((e => U(e, n, t))).finally((() => r.result = void 0))
                             }
                         }
                     }(r, t, e);
-                return ae.bind(null, e, t, i)
+                return V.bind(null, e, t, i)
             }
-            var _e = {};
+            var Q = {};
 
-            function he(e, t, n, r, i) {
-                if (le && "function" == typeof t) {
+            function ee(e, t, n, r, i) {
+                if (K && "function" == typeof t) {
                     let o = t.apply(n, r);
-                    o instanceof Promise ? o.then((t => he(e, t, n, r))).catch((e => se(e, i, t))) : e(o)
+                    o instanceof Promise ? o.then((t => ee(e, t, n, r))).catch((e => U(e, i, t))) : e(o)
                 } else "object" == typeof t && t instanceof Promise ? t.then((t => e(t))) : e(t)
             }
-            var ye = "x-";
+            var te = "x-";
 
-            function ve(e = "") {
-                return ye + e
+            function ne(e = "") {
+                return te + e
             }
-            var me = {};
+            var re = {};
 
-            function ge(e, t) {
-                return me[e] = t, {
+            function ie(e, t) {
+                return re[e] = t, {
                     before(t) {
-                        if (!me[t]) return void console.warn(String.raw`Cannot find directive \`${t}\`. \`${e}\` will use the default order of execution`);
-                        const n = Me.indexOf(t);
-                        Me.splice(n >= 0 ? n : Me.indexOf("DEFAULT"), 0, e)
+                        if (!re[t]) return void console.warn(String.raw`Cannot find directive \`${t}\`. \`${e}\` will use the default order of execution`);
+                        const n = me.indexOf(t);
+                        me.splice(n >= 0 ? n : me.indexOf("DEFAULT"), 0, e)
                     }
                 }
             }
 
-            function xe(e, t, n) {
+            function oe(e, t, n) {
                 if (t = Array.from(t), e._x_virtualDirectives) {
                     let n = Object.entries(e._x_virtualDirectives).map((([e, t]) => ({
                             name: e,
                             value: t
                         }))),
-                        r = be(n);
+                        r = ae(n);
                     n = n.map((e => r.find((t => t.name === e.name)) ? {
                         name: `x-bind:${e.name}`,
                         value: `"${e.value}"`
                     } : e)), t = t.concat(n)
                 }
                 let r = {},
-                    i = t.map(ke(((e, t) => r[e] = t))).filter(Te).map(function(e, t) {
+                    i = t.map(de(((e, t) => r[e] = t))).filter(he).map(function(e, t) {
                         return ({
                             name: n,
                             value: r
                         }) => {
-                            let i = n.match(Le()),
+                            let i = n.match(ye()),
                                 o = n.match(/:([a-zA-Z0-9\-_:]+)/),
                                 a = n.match(/\.[^.\]]+(?=[^\]]*$)/g) || [],
                                 s = t || e[n] || n;
                             return {
                                 type: i ? i[1] : null,
                                 value: o ? o[1] : null,
                                 modifiers: a.map((e => e.replace(".", ""))),
                                 expression: r,
                                 original: s
                             }
                         }
-                    }(r, n)).sort(Ne);
+                    }(r, n)).sort(ge);
                 return i.map((t => function(e, t) {
-                    let n = me[t.type] || (() => {}),
-                        [r, i] = Ae(e);
-                    q(e, t.original, i);
+                    let n = re[t.type] || (() => {}),
+                        [r, i] = ue(e);
+                    w(e, t.original, i);
                     let o = () => {
-                        e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, r), n = n.bind(n, e, t, r), we ? Ee.get(Se).push(n) : n())
+                        e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, r), n = n.bind(n, e, t, r), se ? le.get(ce).push(n) : n())
                     };
                     return o.runCleanups = i, o
                 }(e, t)))
             }
 
-            function be(e) {
-                return Array.from(e).map(ke()).filter((e => !Te(e)))
+            function ae(e) {
+                return Array.from(e).map(de()).filter((e => !he(e)))
             }
-            var we = !1,
-                Ee = new Map,
-                Se = Symbol();
+            var se = !1,
+                le = new Map,
+                ce = Symbol();
 
-            function Ae(e) {
+            function ue(e) {
                 let t = [],
                     [n, r] = function(e) {
                         let t = () => {};
                         return [n => {
                             let r = o(n);
                             return e._x_effects || (e._x_effects = new Set, e._x_runEffects = () => {
                                 e._x_effects.forEach((e => e()))
@@ -925,63 +846,142 @@
                             t()
                         }]
                     }(e);
                 return t.push(r), [{
                     Alpine: _t,
                     effect: n,
                     cleanup: e => t.push(e),
-                    evaluateLater: fe.bind(fe, e),
-                    evaluate: ue.bind(ue, e)
+                    evaluateLater: X.bind(X, e),
+                    evaluate: J.bind(J, e)
                 }, () => t.forEach((e => e()))]
             }
-            var Oe = (e, t) => ({
+            var fe = (e, t) => ({
                 name: n,
                 value: r
             }) => (n.startsWith(e) && (n = n.replace(e, t)), {
                 name: n,
                 value: r
             });
 
-            function ke(e = (() => {})) {
+            function de(e = (() => {})) {
                 return ({
                     name: t,
                     value: n
                 }) => {
                     let {
                         name: r,
                         value: i
-                    } = je.reduce(((e, t) => t(e)), {
+                    } = pe.reduce(((e, t) => t(e)), {
                         name: t,
                         value: n
                     });
                     return r !== t && e(r, t), {
                         name: r,
                         value: i
                     }
                 }
             }
-            var je = [];
+            var pe = [];
 
-            function Ce(e) {
-                je.push(e)
+            function _e(e) {
+                pe.push(e)
             }
 
-            function Te({
+            function he({
                 name: e
             }) {
-                return Le().test(e)
+                return ye().test(e)
+            }
+            var ye = () => new RegExp(`^${te}([^:^.]+)\\b`),
+                ve = "DEFAULT",
+                me = ["ignore", "ref", "data", "id", "anchor", "bind", "init", "for", "model", "modelable", "transition", "show", "if", ve, "teleport"];
+
+            function ge(e, t) {
+                let n = -1 === me.indexOf(e.type) ? ve : e.type,
+                    r = -1 === me.indexOf(t.type) ? ve : t.type;
+                return me.indexOf(n) - me.indexOf(r)
+            }
+
+            function xe(e, t, n = {}) {
+                e.dispatchEvent(new CustomEvent(t, {
+                    detail: n,
+                    bubbles: !0,
+                    composed: !0,
+                    cancelable: !0
+                }))
+            }
+
+            function be(e, t) {
+                if ("function" == typeof ShadowRoot && e instanceof ShadowRoot) return void Array.from(e.children).forEach((e => be(e, t)));
+                let n = !1;
+                if (t(e, (() => n = !0)), n) return;
+                let r = e.firstElementChild;
+                for (; r;) be(r, t), r = r.nextElementSibling
+            }
+
+            function we(e, ...t) {
+                console.warn(`Alpine Warning: ${e}`, ...t)
+            }
+            var Ee = !1,
+                Se = [],
+                Ae = [];
+
+            function Oe() {
+                return Se.map((e => e()))
+            }
+
+            function ke() {
+                return Se.concat(Ae).map((e => e()))
+            }
+
+            function je(e) {
+                Se.push(e)
+            }
+
+            function Ce(e) {
+                Ae.push(e)
+            }
+
+            function Te(e, t = !1) {
+                return $e(e, (e => {
+                    if ((t ? ke() : Oe()).some((t => e.matches(t)))) return !0
+                }))
+            }
+
+            function $e(e, t) {
+                if (e) {
+                    if (t(e)) return e;
+                    if (e._x_teleportBack && (e = e._x_teleportBack), e.parentElement) return $e(e.parentElement, t)
+                }
+            }
+            var Le = [];
+
+            function Me(e, t = be, n = (() => {})) {
+                ! function(r) {
+                    se = !0;
+                    let i = Symbol();
+                    ce = i, le.set(i, []);
+                    let o = () => {
+                        for (; le.get(i).length;) le.get(i).shift()();
+                        le.delete(i)
+                    };
+                    t(e, ((e, t) => {
+                        n(e, t), Le.forEach((n => n(e, t))), oe(e, e.attributes).forEach((e => e())), e._x_ignore && t()
+                    })), se = !1, o()
+                }()
             }
-            var Le = () => new RegExp(`^${ye}([^:^.]+)\\b`),
-                $e = "DEFAULT",
-                Me = ["ignore", "ref", "data", "id", "anchor", "bind", "init", "for", "model", "modelable", "transition", "show", "if", $e, "teleport"];
-
-            function Ne(e, t) {
-                let n = -1 === Me.indexOf(e.type) ? $e : e.type,
-                    r = -1 === Me.indexOf(t.type) ? $e : t.type;
-                return Me.indexOf(n) - Me.indexOf(r)
+
+            function Ne(e, t = be) {
+                t(e, (e => {
+                    E(e),
+                        function(e) {
+                            if (e._x_cleanups)
+                                for (; e._x_cleanups.length;) e._x_cleanups.pop()()
+                        }(e)
+                }))
             }
             var Pe = [],
                 Re = !1;
 
             function qe(e = (() => {})) {
                 return queueMicrotask((() => {
                     Re || setTimeout((() => {
@@ -1086,38 +1086,38 @@
                 start: r,
                 end: i
             } = {}, o = (() => {}), a = (() => {})) {
                 if (e._x_transitioning && e._x_transitioning.cancel(), 0 === Object.keys(n).length && 0 === Object.keys(r).length && 0 === Object.keys(i).length) return o(), void a();
                 let s, l, c;
                 ! function(e, t) {
                     let n, r, i, o = Fe((() => {
-                        W((() => {
+                        C((() => {
                             n = !0, r || t.before(), i || (t.end(), Ie()), t.after(), e.isConnected && t.cleanup(), delete e._x_transitioning
                         }))
                     }));
                     e._x_transitioning = {
                         beforeCancels: [],
                         beforeCancel(e) {
                             this.beforeCancels.push(e)
                         },
                         cancel: Fe((function() {
                             for (; this.beforeCancels.length;) this.beforeCancels.shift()();
                             o()
                         })),
                         finish: o
-                    }, W((() => {
+                    }, C((() => {
                         t.start(), t.during()
                     })), Re = !0, requestAnimationFrame((() => {
                         if (n) return;
                         let o = 1e3 * Number(getComputedStyle(e).transitionDuration.replace(/,.*/, "").replace("s", "")),
                             a = 1e3 * Number(getComputedStyle(e).transitionDelay.replace(/,.*/, "").replace("s", ""));
-                        0 === o && (o = 1e3 * Number(getComputedStyle(e).animationDuration.replace("s", ""))), W((() => {
+                        0 === o && (o = 1e3 * Number(getComputedStyle(e).animationDuration.replace("s", ""))), C((() => {
                             t.before()
                         })), r = !0, requestAnimationFrame((() => {
-                            n || (W((() => {
+                            n || (C((() => {
                                 t.end()
                             })), Ie(), setTimeout(e._x_transitioning.finish, o + a), i = !0)
                         }))
                     }))
                 }(e, {
                     start() {
                         s = t(e, r)
@@ -1143,15 +1143,15 @@
                 if ("scale" === t && isNaN(r)) return n;
                 if ("duration" === t || "delay" === t) {
                     let e = r.match(/([0-9]+)ms/);
                     if (e) return e[1]
                 }
                 return "origin" === t && ["top", "right", "left", "center", "bottom"].includes(e[e.indexOf(t) + 2]) ? [r, e[e.indexOf(t) + 2]].join(" ") : r
             }
-            ge("transition", ((e, {
+            ie("transition", ((e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 evaluate: i
             }) => {
                 "function" == typeof r && (r = i(r)), !1 !== r && (r && "boolean" != typeof r ? function(e, t, n) {
@@ -1376,19 +1376,19 @@
             function dt(e, t, n) {
                 let r = [];
                 for (; r.length;) r.pop()();
                 let i = Object.entries(t).map((([e, t]) => ({
                         name: e,
                         value: t
                     }))),
-                    o = be(i);
+                    o = ae(i);
                 return i = i.map((e => o.find((t => t.name === e.name)) ? {
                     name: `x-bind:${e.name}`,
                     value: `"${e.value}"`
-                } : e)), xe(e, i, n).map((e => {
+                } : e)), oe(e, i, n).map((e => {
                     r.push(e.runCleanups), e()
                 })), () => {
                     for (; r.length;) r.pop()()
                 }
             }
             var pt = {},
                 _t = {
@@ -1400,128 +1400,139 @@
                     },
                     get effect() {
                         return o
                     },
                     get raw() {
                         return s
                     },
-                    version: "3.13.8",
+                    version: "3.13.9",
                     flushAndStopDeferringMutations: function() {
-                        V = !1, K(U), U = []
+                        T = !1, L($), $ = []
                     },
-                    dontAutoEvaluateFunctions: ce,
+                    dontAutoEvaluateFunctions: Z,
                     disableEffectScheduling: function(e) {
                         _ = !1, e(), _ = !0
                     },
-                    startObservingMutations: B,
-                    stopObservingMutations: F,
+                    startObservingMutations: O,
+                    stopObservingMutations: k,
                     setReactivityEngine: function(e) {
                         i = e.reactive, a = e.release, o = t => e.effect(t, {
                             scheduler: e => {
                                 _ ? function(e) {
                                     var t;
                                     t = e, u.includes(t) || u.push(t), c || l || (l = !0, queueMicrotask(p))
                                 }(e) : e()
                             }
                         }), s = e.raw
                     },
-                    onAttributeRemoved: q,
-                    onAttributesAdded: R,
-                    closestDataStack: X,
+                    onAttributeRemoved: w,
+                    onAttributesAdded: b,
+                    closestDataStack: P,
                     skipDuringClone: Ze,
                     onlyDuringClone: function(e) {
                         return (...t) => Ke && e(...t)
                     },
-                    addRootSelector: A,
-                    addInitSelector: O,
+                    addRootSelector: je,
+                    addInitSelector: Ce,
                     interceptClone: Xe,
-                    addScopeToNode: J,
+                    addScopeToNode: N,
                     deferMutations: function() {
-                        V = !0
+                        T = !0
                     },
-                    mapAttributes: Ce,
-                    evaluateLater: fe,
+                    mapAttributes: _e,
+                    evaluateLater: X,
                     interceptInit: function(e) {
-                        C.push(e)
+                        Le.push(e)
                     },
                     setEvaluator: function(e) {
-                        de = e
+                        Y = e
                     },
-                    mergeProxies: Y,
+                    mergeProxies: R,
                     extractProp: function(e, t, n, r = !0) {
                         if (e._x_bindings && void 0 !== e._x_bindings[t]) return e._x_bindings[t];
                         if (e._x_inlineBindings && void 0 !== e._x_inlineBindings[t]) {
                             let n = e._x_inlineBindings[t];
-                            return n.extract = r, ce((() => ue(e, n.expression)))
+                            return n.extract = r, Z((() => J(e, n.expression)))
                         }
                         return it(e, t, n)
                     },
-                    findClosest: j,
-                    onElRemoved: P,
-                    closestRoot: k,
-                    destroyTree: L,
-                    interceptor: te,
+                    findClosest: $e,
+                    onElRemoved: x,
+                    closestRoot: Te,
+                    destroyTree: Ne,
+                    interceptor: z,
                     transition: Ve,
                     setStyles: Be,
-                    mutateDom: W,
-                    directive: ge,
+                    mutateDom: C,
+                    directive: ie,
                     entangle: st,
                     throttle: at,
                     debounce: ot,
-                    evaluate: ue,
-                    initTree: T,
+                    evaluate: J,
+                    initTree: Me,
                     nextTick: qe,
-                    prefixed: ve,
+                    prefixed: ne,
                     prefix: function(e) {
-                        ye = e
+                        te = e
                     },
                     plugin: function(e) {
                         (Array.isArray(e) ? e : [e]).forEach((e => e(_t)))
                     },
-                    magic: ie,
+                    magic: H,
                     store: function(e, t) {
                         if (ut || (ct = i(ct), ut = !0), void 0 === t) return ct[e];
-                        ct[e] = t, "object" == typeof t && null !== t && t.hasOwnProperty("init") && "function" == typeof t.init && ct[e].init(), ee(ct[e])
+                        ct[e] = t, "object" == typeof t && null !== t && t.hasOwnProperty("init") && "function" == typeof t.init && ct[e].init(), D(ct[e])
                     },
                     start: function() {
                         var e;
-                        x && g("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), x = !0, document.body || g("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), v(document, "alpine:init"), v(document, "alpine:initializing"), B(), e = e => T(e, m), N.push(e), P((e => L(e))), R(((e, t) => {
-                            xe(e, t).forEach((e => e()))
-                        })), Array.from(document.querySelectorAll(S().join(","))).filter((e => !k(e.parentElement, !0))).forEach((e => {
-                            T(e)
-                        })), v(document, "alpine:initialized")
+                        Ee && we("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), Ee = !0, document.body || we("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), xe(document, "alpine:init"), xe(document, "alpine:initializing"), O(), e = e => Me(e, be), g.push(e), x((e => Ne(e))), b(((e, t) => {
+                            oe(e, t).forEach((e => e()))
+                        })), Array.from(document.querySelectorAll(ke().join(","))).filter((e => !Te(e.parentElement, !0))).forEach((e => {
+                            Me(e)
+                        })), xe(document, "alpine:initialized"), setTimeout((() => {
+                            [
+                                ["ui", "dialog", ["[x-dialog], [x-popover]"]],
+                                ["anchor", "anchor", ["[x-anchor]"]],
+                                ["sort", "sort", ["[x-sort]"]]
+                            ].forEach((([e, t, n]) => {
+                                var r;
+                                r = t, Object.keys(re).includes(r) || n.some((t => {
+                                    if (document.querySelector(t)) return we(`found "${t}", but missing ${e} plugin`), !0
+                                }))
+                            }))
+                        }))
                     },
                     clone: function(e, t) {
                         t._x_dataStack || (t._x_dataStack = e._x_dataStack), Ke = !0, Ye = !0, Ge((() => {
                             ! function(e) {
                                 let t = !1;
-                                T(e, ((e, n) => {
-                                    m(e, ((e, r) => {
+                                Me(e, ((e, n) => {
+                                    be(e, ((e, r) => {
                                         if (t && function(e) {
-                                                return E().some((t => e.matches(t)))
+                                                return Oe().some((t => e.matches(t)))
                                             }(e)) return r();
                                         t = !0, n(e, r)
                                     }))
                                 }))
                             }(t)
                         })), Ke = !1, Ye = !1
                     },
                     cloneNode: function(e, t) {
                         Je.forEach((n => n(e, t))), Ke = !0, Ge((() => {
-                            T(t, ((e, t) => {
+                            Me(t, ((e, t) => {
                                 t(e, (() => {}))
                             }))
                         })), Ke = !1
                     },
                     bound: function(e, t, n) {
                         return e._x_bindings && void 0 !== e._x_bindings[t] ? e._x_bindings[t] : it(e, t, n)
                     },
-                    $data: Z,
+                    $data: M,
                     watch: y,
-                    walk: m,
+                    walk: be,
                     data: function(e, t) {
                         pt[e] = t
                     },
                     bind: function(e, t) {
                         let n = "function" != typeof t ? () => t : t;
                         return e instanceof Element ? dt(e, n()) : (ft[e] = n, () => {})
                     }
@@ -1546,16 +1557,16 @@
                 kt = e => "string" == typeof e && "NaN" !== e && "-" !== e[0] && "" + parseInt(e, 10) === e,
                 jt = e => {
                     const t = Object.create(null);
                     return n => t[n] || (t[n] = e(n))
                 },
                 Ct = /-(\w)/g,
                 Tt = (jt((e => e.replace(Ct, ((e, t) => t ? t.toUpperCase() : "")))), /\B([A-Z])/g),
-                Lt = (jt((e => e.replace(Tt, "-$1").toLowerCase())), jt((e => e.charAt(0).toUpperCase() + e.slice(1)))),
-                $t = (jt((e => e ? `on${Lt(e)}` : "")), (e, t) => e !== t && (e == e || t == t)),
+                $t = (jt((e => e.replace(Tt, "-$1").toLowerCase())), jt((e => e.charAt(0).toUpperCase() + e.slice(1)))),
+                Lt = (jt((e => e ? `on${$t(e)}` : "")), (e, t) => e !== t && (e == e || t == t)),
                 Mt = new WeakMap,
                 Nt = [],
                 Pt = Symbol("iterate"),
                 Rt = Symbol("Map key iterate"),
                 qt = 0;
 
             function It(e) {
@@ -1629,47 +1640,47 @@
                 Kt = Xt(!0),
                 Zt = Jt();
 
             function Jt() {
                 const e = {};
                 return ["includes", "indexOf", "lastIndexOf"].forEach((t => {
                     e[t] = function(...e) {
-                        const n = Ln(this);
+                        const n = $n(this);
                         for (let e = 0, t = this.length; e < t; e++) Ft(n, "get", e + "");
                         const r = n[t](...e);
-                        return -1 === r || !1 === r ? n[t](...e.map(Ln)) : r
+                        return -1 === r || !1 === r ? n[t](...e.map($n)) : r
                     }
                 })), ["push", "pop", "shift", "unshift", "splice"].forEach((t => {
                     e[t] = function(...e) {
                         zt.push(Dt), Dt = !1;
-                        const n = Ln(this)[t].apply(this, e);
+                        const n = $n(this)[t].apply(this, e);
                         return Bt(), n
                     }
                 })), e
             }
 
             function Xt(e = !1, t = !1) {
                 return function(n, r, i) {
                     if ("__v_isReactive" === r) return !e;
                     if ("__v_isReadonly" === r) return e;
                     if ("__v_raw" === r && i === (e ? t ? kn : On : t ? An : Sn).get(n)) return n;
                     const o = xt(n);
                     if (!e && o && gt(Zt, r)) return Reflect.get(Zt, r, i);
                     const a = Reflect.get(n, r, i);
-                    return (wt(r) ? Vt.has(r) : Wt(r)) ? a : (e || Ft(n, "get", r), t ? a : $n(a) ? o && kt(r) ? a : a.value : Et(a) ? e ? Cn(a) : jn(a) : a)
+                    return (wt(r) ? Vt.has(r) : Wt(r)) ? a : (e || Ft(n, "get", r), t ? a : Ln(a) ? o && kt(r) ? a : a.value : Et(a) ? e ? Cn(a) : jn(a) : a)
                 }
             }
 
             function Yt(e = !1) {
                 return function(t, n, r, i) {
                     let o = t[n];
-                    if (!e && (r = Ln(r), o = Ln(o), !xt(t) && $n(o) && !$n(r))) return o.value = r, !0;
+                    if (!e && (r = $n(r), o = $n(o), !xt(t) && Ln(o) && !Ln(r))) return o.value = r, !0;
                     const a = xt(t) && kt(n) ? Number(n) < t.length : gt(t, n),
                         s = Reflect.set(t, n, r, i);
-                    return t === Ln(i) && (a ? $t(r, o) && Ht(t, "set", n, r, o) : Ht(t, "add", n, r)), s
+                    return t === $n(i) && (a ? Lt(r, o) && Ht(t, "set", n, r, o) : Ht(t, "add", n, r)), s
                 }
             }
             var Gt = {
                     get: Ut,
                     set: Yt(),
                     deleteProperty: function(e, t) {
                         const n = gt(e, t),
@@ -1696,88 +1707,88 @@
                 },
                 en = e => Et(e) ? jn(e) : e,
                 tn = e => Et(e) ? Cn(e) : e,
                 nn = e => e,
                 rn = e => Reflect.getPrototypeOf(e);
 
             function on(e, t, n = !1, r = !1) {
-                const i = Ln(e = e.__v_raw),
-                    o = Ln(t);
+                const i = $n(e = e.__v_raw),
+                    o = $n(t);
                 t !== o && !n && Ft(i, "get", t), !n && Ft(i, "get", o);
                 const {
                     has: a
                 } = rn(i), s = r ? nn : n ? tn : en;
                 return a.call(i, t) ? s(e.get(t)) : a.call(i, o) ? s(e.get(o)) : void(e !== i && e.get(t))
             }
 
             function an(e, t = !1) {
                 const n = this.__v_raw,
-                    r = Ln(n),
-                    i = Ln(e);
+                    r = $n(n),
+                    i = $n(e);
                 return e !== i && !t && Ft(r, "has", e), !t && Ft(r, "has", i), e === i ? n.has(e) : n.has(e) || n.has(i)
             }
 
             function sn(e, t = !1) {
-                return e = e.__v_raw, !t && Ft(Ln(e), "iterate", Pt), Reflect.get(e, "size", e)
+                return e = e.__v_raw, !t && Ft($n(e), "iterate", Pt), Reflect.get(e, "size", e)
             }
 
             function ln(e) {
-                e = Ln(e);
-                const t = Ln(this);
+                e = $n(e);
+                const t = $n(this);
                 return rn(t).has.call(t, e) || (t.add(e), Ht(t, "add", e, e)), this
             }
 
             function cn(e, t) {
-                t = Ln(t);
-                const n = Ln(this),
+                t = $n(t);
+                const n = $n(this),
                     {
                         has: r,
                         get: i
                     } = rn(n);
                 let o = r.call(n, e);
-                o ? En(n, r, e) : (e = Ln(e), o = r.call(n, e));
+                o ? En(n, r, e) : (e = $n(e), o = r.call(n, e));
                 const a = i.call(n, e);
-                return n.set(e, t), o ? $t(t, a) && Ht(n, "set", e, t, a) : Ht(n, "add", e, t), this
+                return n.set(e, t), o ? Lt(t, a) && Ht(n, "set", e, t, a) : Ht(n, "add", e, t), this
             }
 
             function un(e) {
-                const t = Ln(this),
+                const t = $n(this),
                     {
                         has: n,
                         get: r
                     } = rn(t);
                 let i = n.call(t, e);
-                i ? En(t, n, e) : (e = Ln(e), i = n.call(t, e));
+                i ? En(t, n, e) : (e = $n(e), i = n.call(t, e));
                 const o = r ? r.call(t, e) : void 0,
                     a = t.delete(e);
                 return i && Ht(t, "delete", e, void 0, o), a
             }
 
             function fn() {
-                const e = Ln(this),
+                const e = $n(this),
                     t = 0 !== e.size,
                     n = bt(e) ? new Map(e) : new Set(e),
                     r = e.clear();
                 return t && Ht(e, "clear", void 0, void 0, n), r
             }
 
             function dn(e, t) {
                 return function(n, r) {
                     const i = this,
                         o = i.__v_raw,
-                        a = Ln(o),
+                        a = $n(o),
                         s = t ? nn : e ? tn : en;
                     return !e && Ft(a, "iterate", Pt), o.forEach(((e, t) => n.call(r, s(e), s(t), i)))
                 }
             }
 
             function pn(e, t, n) {
                 return function(...r) {
                     const i = this.__v_raw,
-                        o = Ln(i),
+                        o = $n(i),
                         a = bt(o),
                         s = "entries" === e || e === Symbol.iterator && a,
                         l = "keys" === e && a,
                         c = i[e](...r),
                         u = n ? nn : t ? tn : en;
                     return !t && Ft(o, "iterate", l ? Rt : Pt), {
                         next() {
@@ -1800,15 +1811,15 @@
                 }
             }
 
             function _n(e) {
                 return function(...t) {
                     {
                         const n = t[0] ? `on key "${t[0]}" ` : "";
-                        console.warn(`${Lt(e)} operation ${n}failed: target is readonly.`, Ln(this))
+                        console.warn(`${$t(e)} operation ${n}failed: target is readonly.`, $n(this))
                     }
                     return "delete" !== e && this
                 }
             }
 
             function hn() {
                 const e = {
@@ -1885,15 +1896,15 @@
                     get: xn(!1, !1)
                 },
                 wn = {
                     get: xn(!0, !1)
                 };
 
             function En(e, t, n) {
-                const r = Ln(n);
+                const r = $n(n);
                 if (r !== n && t.call(e, r)) {
                     const t = Ot(e);
                     console.warn(`Reactive ${t} contains both the raw and reactive versions of the same object${"Map"===t?" as keys":""}, which can lead to inconsistencies. Avoid differentiating between the raw and reactive versions of an object and only use the reactive version if possible.`)
                 }
             }
             var Sn = new WeakMap,
                 An = new WeakMap,
@@ -1929,67 +1940,67 @@
                 }(Ot(s));
                 var s;
                 if (0 === a) return e;
                 const l = new Proxy(e, 2 === a ? r : n);
                 return i.set(e, l), l
             }
 
-            function Ln(e) {
-                return e && Ln(e.__v_raw) || e
+            function $n(e) {
+                return e && $n(e.__v_raw) || e
             }
 
-            function $n(e) {
+            function Ln(e) {
                 return Boolean(e && !0 === e.__v_isRef)
             }
-            ie("nextTick", (() => qe)), ie("dispatch", (e => v.bind(v, e))), ie("watch", ((e, {
+            H("nextTick", (() => qe)), H("dispatch", (e => xe.bind(xe, e))), H("watch", ((e, {
                 evaluateLater: t,
                 cleanup: n
             }) => (e, r) => {
                 let i = t(e),
                     o = y((() => {
                         let e;
                         return i((t => e = t)), e
                     }), r);
                 n(o)
-            })), ie("store", (function() {
+            })), H("store", (function() {
                 return ct
-            })), ie("data", (e => Z(e))), ie("root", (e => k(e))), ie("refs", (e => (e._x_refs_proxy || (e._x_refs_proxy = Y(function(e) {
+            })), H("data", (e => M(e))), H("root", (e => Te(e))), H("refs", (e => (e._x_refs_proxy || (e._x_refs_proxy = R(function(e) {
                 let t = [];
-                return j(e, (e => {
+                return $e(e, (e => {
                     e._x_refs && t.push(e._x_refs)
                 })), t
             }(e))), e._x_refs_proxy)));
             var Mn = {};
 
             function Nn(e) {
                 return Mn[e] || (Mn[e] = 0), ++Mn[e]
             }
 
             function Pn(e, t, n) {
-                ie(t, (r => g(`You can't use [$${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
+                H(t, (r => we(`You can't use [$${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
             }
-            ie("id", ((e, {
+            H("id", ((e, {
                 cleanup: t
             }) => (n, r = null) => function(e, t, n, r) {
                 if (e._x_id || (e._x_id = {}), e._x_id[t]) return e._x_id[t];
                 let i = r();
                 return e._x_id[t] = i, n((() => {
                     delete e._x_id[t]
                 })), i
             }(e, `${n}${r?`-${r}`:""}`, t, (() => {
                 let t = function(e, t) {
-                        return j(e, (e => {
+                        return $e(e, (e => {
                             if (e._x_ids && e._x_ids[t]) return !0
                         }))
                     }(e, n),
                     i = t ? t._x_ids[n] : Nn(n);
                 return r ? `${n}-${i}-${r}` : `${n}-${i}`
             })))), Xe(((e, t) => {
                 e._x_id && (t._x_id = e._x_id)
-            })), ie("el", (e => e)), Pn("Focus", "focus", "focus"), Pn("Persist", "persist", "persist"), ge("modelable", ((e, {
+            })), H("el", (e => e)), Pn("Focus", "focus", "focus"), Pn("Persist", "persist", "persist"), ie("modelable", ((e, {
                 expression: t
             }, {
                 effect: n,
                 evaluateLater: r,
                 cleanup: i
             }) => {
                 let o = r(t),
@@ -2022,45 +2033,45 @@
                             },
                             set(e) {
                                 l(e)
                             }
                         });
                     i(r)
                 }))
-            })), ge("teleport", ((e, {
+            })), ie("teleport", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 cleanup: r
             }) => {
-                "template" !== e.tagName.toLowerCase() && g("x-teleport can only be used on a <template> tag", e);
+                "template" !== e.tagName.toLowerCase() && we("x-teleport can only be used on a <template> tag", e);
                 let i = qn(n),
                     o = e.content.cloneNode(!0).firstElementChild;
                 e._x_teleport = o, o._x_teleportBack = e, e.setAttribute("data-teleport-template", !0), o.setAttribute("data-teleport-target", !0), e._x_forwardEvents && e._x_forwardEvents.forEach((t => {
                     o.addEventListener(t, (t => {
                         t.stopPropagation(), e.dispatchEvent(new t.constructor(t.type, t))
                     }))
-                })), J(o, {}, e);
+                })), N(o, {}, e);
                 let a = (e, t, n) => {
                     n.includes("prepend") ? t.parentNode.insertBefore(e, t) : n.includes("append") ? t.parentNode.insertBefore(e, t.nextSibling) : t.appendChild(e)
                 };
-                W((() => {
-                    a(o, i, t), T(o), o._x_ignore = !0
+                C((() => {
+                    a(o, i, t), Me(o), o._x_ignore = !0
                 })), e._x_teleportPutBack = () => {
                     let r = qn(n);
-                    W((() => {
+                    C((() => {
                         a(e._x_teleport, r, t)
                     }))
                 }, r((() => o.remove()))
             }));
             var Rn = document.createElement("div");
 
             function qn(e) {
                 let t = Ze((() => document.querySelector(e)), (() => Rn))();
-                return t || g(`Cannot find x-teleport element for selector: "${e}"`), t
+                return t || we(`Cannot find x-teleport element for selector: "${e}"`), t
             }
             var In = () => {};
 
             function Dn(e, t, n, r) {
                 let i = e,
                     o = e => r(e),
                     a = {},
@@ -2075,20 +2086,20 @@
                         t = zn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
                     o = at(o, t)
                 }
                 return n.includes("prevent") && (o = s(o, ((e, t) => {
                     t.preventDefault(), e(t)
                 }))), n.includes("stop") && (o = s(o, ((e, t) => {
                     t.stopPropagation(), e(t)
-                }))), n.includes("self") && (o = s(o, ((t, n) => {
-                    n.target === e && t(n)
-                }))), (n.includes("away") || n.includes("outside")) && (i = document, o = s(o, ((t, n) => {
-                    e.contains(n.target) || !1 !== n.target.isConnected && (e.offsetWidth < 1 && e.offsetHeight < 1 || !1 !== e._x_isShown && t(n))
                 }))), n.includes("once") && (o = s(o, ((e, n) => {
                     e(n), i.removeEventListener(t, o, a)
+                }))), (n.includes("away") || n.includes("outside")) && (i = document, o = s(o, ((t, n) => {
+                    e.contains(n.target) || !1 !== n.target.isConnected && (e.offsetWidth < 1 && e.offsetHeight < 1 || !1 !== e._x_isShown && t(n))
+                }))), n.includes("self") && (o = s(o, ((t, n) => {
+                    n.target === e && t(n)
                 }))), o = s(o, ((e, r) => {
                     (function(e) {
                         return ["keydown", "keyup"].includes(e)
                     })(t) && function(e, t) {
                         let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture"].includes(e)));
                         if (n.includes("debounce")) {
                             let e = n.indexOf("debounce");
@@ -2134,15 +2145,15 @@
                 };
                 return n[e] = e, Object.keys(n).map((t => {
                     if (n[t] === e) return t
                 })).filter((e => e))
             }
 
             function Fn(e, t, n, r) {
-                return W((() => {
+                return C((() => {
                     if (n instanceof CustomEvent && void 0 !== n.detail) return null !== n.detail && void 0 !== n.detail ? n.detail : n.target.value;
                     if ("checkbox" === e.type) {
                         if (Array.isArray(r)) {
                             let e = null;
                             return e = t.includes("number") ? Hn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : n.target.value, n.target.checked ? r.concat([e]) : r.filter((t => !(t == e)))
                         }
                         return n.target.checked
@@ -2168,44 +2179,44 @@
                 modifiers: t
             }, {
                 cleanup: n
             }) => {
                 t.includes("self") ? e._x_ignoreSelf = !0 : e._x_ignore = !0, n((() => {
                     t.includes("self") ? delete e._x_ignoreSelf : delete e._x_ignore
                 }))
-            }, ge("ignore", In), ge("effect", Ze(((e, {
+            }, ie("ignore", In), ie("effect", Ze(((e, {
                 expression: t
             }, {
                 effect: n
             }) => {
-                n(fe(e, t))
-            }))), ge("model", ((e, {
+                n(X(e, t))
+            }))), ie("model", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 effect: r,
                 cleanup: i
             }) => {
                 let o = e;
                 t.includes("parent") && (o = e.parentNode);
-                let a, s = fe(o, n);
-                a = "string" == typeof n ? fe(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? fe(o, `${n()} = __placeholder`) : () => {};
+                let a, s = X(o, n);
+                a = "string" == typeof n ? X(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? X(o, `${n()} = __placeholder`) : () => {};
                 let l = () => {
                         let e;
                         return s((t => e = t)), Wn(e) ? e.get() : e
                     },
                     c = e => {
                         let t;
                         s((e => t = e)), Wn(t) ? t.set(e) : a((() => {}), {
                             scope: {
                                 __placeholder: e
                             }
                         })
                     };
-                "string" == typeof n && "radio" === e.type && W((() => {
+                "string" == typeof n && "radio" === e.type && C((() => {
                     e.hasAttribute("name") || e.setAttribute("name", n)
                 }));
                 var u = "select" === e.tagName.toLowerCase() || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
                 let f = Ke ? () => {} : Dn(e, u, t, (n => {
                     c(Fn(e, t, n, l()))
                 }));
                 if (t.includes("fill") && ([void 0, null, ""].includes(l()) || "checkbox" === e.type && Array.isArray(l())) && c(Fn(e, t, {
@@ -2220,52 +2231,52 @@
                     get() {
                         return l()
                     },
                     set(e) {
                         c(e)
                     }
                 }, e._x_forceModelUpdate = t => {
-                    void 0 === t && "string" == typeof n && n.match(/\./) && (t = ""), window.fromModel = !0, W((() => Qe(e, "value", t))), delete window.fromModel
+                    void 0 === t && "string" == typeof n && n.match(/\./) && (t = ""), window.fromModel = !0, C((() => Qe(e, "value", t))), delete window.fromModel
                 }, r((() => {
                     let n = l();
                     t.includes("unintrusive") && document.activeElement.isSameNode(e) || e._x_forceModelUpdate(n)
                 }))
-            })), ge("cloak", (e => queueMicrotask((() => W((() => e.removeAttribute(ve("cloak")))))))), O((() => `[${ve("init")}]`)), ge("init", Ze(((e, {
+            })), ie("cloak", (e => queueMicrotask((() => C((() => e.removeAttribute(ne("cloak")))))))), Ce((() => `[${ne("init")}]`)), ie("init", Ze(((e, {
                 expression: t
             }, {
                 evaluate: n
-            }) => "string" == typeof t ? !!t.trim() && n(t, {}, !1) : n(t, {}, !1)))), ge("text", ((e, {
+            }) => "string" == typeof t ? !!t.trim() && n(t, {}, !1) : n(t, {}, !1)))), ie("text", ((e, {
                 expression: t
             }, {
                 effect: n,
                 evaluateLater: r
             }) => {
                 let i = r(t);
                 n((() => {
                     i((t => {
-                        W((() => {
+                        C((() => {
                             e.textContent = t
                         }))
                     }))
                 }))
-            })), ge("html", ((e, {
+            })), ie("html", ((e, {
                 expression: t
             }, {
                 effect: n,
                 evaluateLater: r
             }) => {
                 let i = r(t);
                 n((() => {
                     i((t => {
-                        W((() => {
-                            e.innerHTML = t, e._x_ignoreSelf = !0, T(e), delete e._x_ignoreSelf
+                        C((() => {
+                            e.innerHTML = t, e._x_ignoreSelf = !0, Me(e), delete e._x_ignoreSelf
                         }))
                     }))
                 }))
-            })), Ce(Oe(":", ve("bind:")));
+            })), _e(fe(":", ne("bind:")));
             var Vn = (e, {
                 value: t,
                 modifiers: n,
                 expression: r,
                 original: i
             }, {
                 effect: o,
@@ -2275,28 +2286,28 @@
                     let t = {};
                     return s = t, Object.entries(ft).forEach((([e, t]) => {
                         Object.defineProperty(s, e, {
                             get() {
                                 return (...e) => t(...e)
                             }
                         })
-                    })), void fe(e, r)((t => {
+                    })), void X(e, r)((t => {
                         dt(e, t, i)
                     }), {
                         scope: t
                     })
                 }
                 var s;
                 if ("key" === t) return function(e, t) {
                     e._x_keyExpression = t
                 }(e, r);
                 if (e._x_inlineBindings && e._x_inlineBindings[t] && e._x_inlineBindings[t].extract) return;
-                let l = fe(e, r);
+                let l = X(e, r);
                 o((() => l((i => {
-                    void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), W((() => Qe(e, t, i, n)))
+                    void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), C((() => Qe(e, t, i, n)))
                 })))), a((() => {
                     e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedStyles && e._x_undoAddedStyles()
                 }))
             };
 
             function Un(e, t, n, r) {
                 let i = {};
@@ -2306,71 +2317,71 @@
                     i[e] = t[e]
                 })) : i[e.item] = t, e.index && (i[e.index] = n), e.collection && (i[e.collection] = r), i
             }
 
             function Kn() {}
 
             function Zn(e, t, n) {
-                ge(t, (r => g(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
+                ie(t, (r => we(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
             }
             Vn.inline = (e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }) => {
                 t && (e._x_inlineBindings || (e._x_inlineBindings = {}), e._x_inlineBindings[t] = {
                     expression: r,
                     extract: !1
                 })
-            }, ge("bind", Vn), A((() => `[${ve("data")}]`)), ge("data", ((e, {
+            }, ie("bind", Vn), je((() => `[${ne("data")}]`)), ie("data", ((e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
                 if (function(e) {
                         return !!Ke && (!!Ye || e.hasAttribute("data-has-alpine-state"))
                     }(e)) return;
                 t = "" === t ? "{}" : t;
                 let r = {};
-                oe(r, e);
+                W(r, e);
                 let o = {};
                 var a, s;
                 a = o, s = r, Object.entries(pt).forEach((([e, t]) => {
                     Object.defineProperty(a, e, {
                         get() {
                             return (...e) => t.bind(s)(...e)
                         },
                         enumerable: !1
                     })
                 }));
-                let l = ue(e, t, {
+                let l = J(e, t, {
                     scope: o
                 });
-                void 0 !== l && !0 !== l || (l = {}), oe(l, e);
+                void 0 !== l && !0 !== l || (l = {}), W(l, e);
                 let c = i(l);
-                ee(c);
-                let u = J(e, c);
-                c.init && ue(e, c.init), n((() => {
-                    c.destroy && ue(e, c.destroy), u()
+                D(c);
+                let u = N(e, c);
+                c.init && J(e, c.init), n((() => {
+                    c.destroy && J(e, c.destroy), u()
                 }))
             })), Xe(((e, t) => {
                 e._x_dataStack && (t._x_dataStack = e._x_dataStack, t.setAttribute("data-has-alpine-state", !0))
-            })), ge("show", ((e, {
+            })), ie("show", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 effect: r
             }) => {
-                let i = fe(e, n);
+                let i = X(e, n);
                 e._x_doHide || (e._x_doHide = () => {
-                    W((() => {
+                    C((() => {
                         e.style.setProperty("display", "none", t.includes("important") ? "important" : void 0)
                     }))
                 }), e._x_doShow || (e._x_doShow = () => {
-                    W((() => {
+                    C((() => {
                         1 === e.style.length && "none" === e.style.display ? e.removeAttribute("style") : e.style.removeProperty("display")
                     }))
                 });
                 let o, a = () => {
                         e._x_doHide(), e._x_isShown = !1
                     },
                     s = () => {
@@ -2380,15 +2391,15 @@
                     c = Fe((e => e ? s() : a()), (t => {
                         "function" == typeof e._x_toggleAndCascadeWithTransitions ? e._x_toggleAndCascadeWithTransitions(e, t, s, a) : t ? l() : a()
                     })),
                     u = !0;
                 r((() => i((e => {
                     (u || e !== o) && (t.includes("immediate") && (e ? l() : a()), c(e), o = e, u = !1)
                 }))))
-            })), ge("for", ((e, {
+            })), ie("for", ((e, {
                 expression: t
             }, {
                 effect: n,
                 cleanup: r
             }) => {
                 let o = function(e) {
                         let t = /,([^,\}\]]*)(?:,([^,\}\]]*))?$/,
@@ -2396,40 +2407,40 @@
                         if (!n) return;
                         let r = {};
                         r.items = n[2].trim();
                         let i = n[1].replace(/^\s*\(|\)\s*$/g, "").trim(),
                             o = i.match(t);
                         return o ? (r.item = i.replace(t, "").trim(), r.index = o[1].trim(), o[2] && (r.collection = o[2].trim())) : r.item = i, r
                     }(t),
-                    a = fe(e, o.items),
-                    s = fe(e, e._x_keyExpression || "index");
+                    a = X(e, o.items),
+                    s = X(e, e._x_keyExpression || "index");
                 e._x_prevKeys = [], e._x_lookup = {}, n((() => function(e, t, n, r) {
                     let o = e;
                     n((n => {
                         var a;
                         a = n, !Array.isArray(a) && !isNaN(a) && n >= 0 && (n = Array.from(Array(n).keys(), (e => e + 1))), void 0 === n && (n = []);
                         let s = e._x_lookup,
                             l = e._x_prevKeys,
                             c = [],
                             u = [];
                         if ("object" != typeof(f = n) || Array.isArray(f))
                             for (let i = 0; i < n.length; i++) {
                                 let o = Un(t, n[i], i, n);
                                 r((t => {
-                                    u.includes(t) && g("Duplicate key on x-for", e), u.push(t)
+                                    u.includes(t) && we("Duplicate key on x-for", e), u.push(t)
                                 }), {
                                     scope: {
                                         index: i,
                                         ...o
                                     }
                                 }), c.push(o)
                             } else n = Object.entries(n).map((([i, o]) => {
                                 let a = Un(t, o, i, n);
                                 r((t => {
-                                    u.includes(t) && g("Duplicate key on x-for", e), u.push(t)
+                                    u.includes(t) && we("Duplicate key on x-for", e), u.push(t)
                                 }), {
                                     scope: {
                                         index: i,
                                         ...a
                                     }
                                 }), c.push(a)
                             }));
@@ -2456,96 +2467,96 @@
                         }
                         for (let e = 0; e < h.length; e++) {
                             let t = h[e];
                             s[t]._x_effects && s[t]._x_effects.forEach(d), s[t].remove(), s[t] = null, delete s[t]
                         }
                         for (let e = 0; e < _.length; e++) {
                             let [t, n] = _[e], r = s[t], i = s[n], a = document.createElement("div");
-                            W((() => {
-                                i || g('x-for ":key" is undefined or invalid', o, n, s), i.after(a), r.after(i), i._x_currentIfEl && i.after(i._x_currentIfEl), a.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), a.remove()
+                            C((() => {
+                                i || we('x-for ":key" is undefined or invalid', o, n, s), i.after(a), r.after(i), i._x_currentIfEl && i.after(i._x_currentIfEl), a.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), a.remove()
                             })), i._x_refreshXForScope(c[u.indexOf(n)])
                         }
                         for (let e = 0; e < p.length; e++) {
                             let [t, n] = p[e], r = "template" === t ? o : s[t];
                             r._x_currentIfEl && (r = r._x_currentIfEl);
                             let a = c[n],
                                 l = u[n],
                                 f = document.importNode(o.content, !0).firstElementChild,
                                 d = i(a);
-                            J(f, d, o), f._x_refreshXForScope = e => {
+                            N(f, d, o), f._x_refreshXForScope = e => {
                                 Object.entries(e).forEach((([e, t]) => {
                                     d[e] = t
                                 }))
-                            }, W((() => {
-                                r.after(f), Ze((() => T(f)))()
-                            })), "object" == typeof l && g("x-for key cannot be an object, it must be a string or an integer", o), s[l] = f
+                            }, C((() => {
+                                r.after(f), Ze((() => Me(f)))()
+                            })), "object" == typeof l && we("x-for key cannot be an object, it must be a string or an integer", o), s[l] = f
                         }
                         for (let e = 0; e < y.length; e++) s[y[e]]._x_refreshXForScope(c[u.indexOf(y[e])]);
                         o._x_prevKeys = u
                     }))
                 }(e, o, a, s))), r((() => {
                     Object.values(e._x_lookup).forEach((e => e.remove())), delete e._x_prevKeys, delete e._x_lookup
                 }))
             })), Kn.inline = (e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
-                let r = k(e);
+                let r = Te(e);
                 r._x_refs || (r._x_refs = {}), r._x_refs[t] = e, n((() => delete r._x_refs[t]))
-            }, ge("ref", Kn), ge("if", ((e, {
+            }, ie("ref", Kn), ie("if", ((e, {
                 expression: t
             }, {
                 effect: n,
                 cleanup: r
             }) => {
-                "template" !== e.tagName.toLowerCase() && g("x-if can only be used on a <template> tag", e);
-                let i = fe(e, t);
+                "template" !== e.tagName.toLowerCase() && we("x-if can only be used on a <template> tag", e);
+                let i = X(e, t);
                 n((() => i((t => {
                     t ? (() => {
                         if (e._x_currentIfEl) return e._x_currentIfEl;
                         let t = e.content.cloneNode(!0).firstElementChild;
-                        J(t, {}, e), W((() => {
-                            e.after(t), Ze((() => T(t)))()
+                        N(t, {}, e), C((() => {
+                            e.after(t), Ze((() => Me(t)))()
                         })), e._x_currentIfEl = t, e._x_undoIf = () => {
-                            m(t, (e => {
+                            be(t, (e => {
                                 e._x_effects && e._x_effects.forEach(d)
                             })), t.remove(), delete e._x_currentIfEl
                         }
                     })() : e._x_undoIf && (e._x_undoIf(), delete e._x_undoIf)
                 })))), r((() => e._x_undoIf && e._x_undoIf()))
-            })), ge("id", ((e, {
+            })), ie("id", ((e, {
                 expression: t
             }, {
                 evaluate: n
             }) => {
                 n(t).forEach((t => function(e, t) {
                     e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = Nn(t))
                 }(e, t)))
             })), Xe(((e, t) => {
                 e._x_ids && (t._x_ids = e._x_ids)
-            })), Ce(Oe("@", ve("on:"))), ge("on", Ze(((e, {
+            })), _e(fe("@", ne("on:"))), ie("on", Ze(((e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 cleanup: i
             }) => {
-                let o = r ? fe(e, r) : () => {};
+                let o = r ? X(e, r) : () => {};
                 "template" === e.tagName.toLowerCase() && (e._x_forwardEvents || (e._x_forwardEvents = []), e._x_forwardEvents.includes(t) || e._x_forwardEvents.push(t));
                 let a = Dn(e, t, n, (e => {
                     o((() => {}), {
                         scope: {
                             $event: e
                         },
                         params: [e]
                     })
                 }));
                 i((() => a()))
-            }))), Zn("Collapse", "collapse", "collapse"), Zn("Intersect", "intersect", "intersect"), Zn("Focus", "trap", "focus"), Zn("Mask", "mask", "mask"), _t.setEvaluator(pe), _t.setReactivityEngine({
+            }))), Zn("Collapse", "collapse", "collapse"), Zn("Intersect", "intersect", "intersect"), Zn("Focus", "trap", "focus"), Zn("Mask", "mask", "mask"), _t.setEvaluator(G), _t.setReactivityEngine({
                 reactive: jn,
                 effect: function(e, t = vt) {
                     (function(e) {
                         return e && !0 === e._isEffect
                     })(e) && (e = e.raw);
                     const n = function(e, t) {
                         const n = function() {
@@ -2562,15 +2573,15 @@
                         return n.id = qt++, n.allowRecurse = !!t.allowRecurse, n._isEffect = !0, n.active = !0, n.raw = e, n.deps = [], n.options = t, n
                     }(e, t);
                     return t.lazy || n(), n
                 },
                 release: function(e) {
                     e.active && (It(e), e.options.onStop && e.options.onStop(), e.active = !1)
                 },
-                raw: Ln
+                raw: $n
             });
             var Jn = _t,
                 Xn = n(122),
                 Yn = n.n(Xn);
 
             function Gn(e, t) {
                 e.classList.remove("scale-100"), t.classList.add("scale-100"), e.classList.add("scale-0"), t.classList.remove("scale-0")
```

### Comparing `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.1.4/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.3/PKG-INFO` & `sphinxawesome_theme-5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.1.3
+Version: 5.1.4
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.3 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.4 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

