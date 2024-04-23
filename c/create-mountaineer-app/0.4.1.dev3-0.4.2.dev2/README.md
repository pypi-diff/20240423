# Comparing `tmp/create_mountaineer_app-0.4.1.dev3.tar.gz` & `tmp/create_mountaineer_app-0.4.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_mountaineer_app-0.4.1.dev3.tar", max compression
+gzip compressed data, was "create_mountaineer_app-0.4.2.dev2.tar", max compression
```

## Comparing `create_mountaineer_app-0.4.1.dev3.tar` & `create_mountaineer_app-0.4.2.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1593 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/README.md
--rw-r--r--   0        0        0        1 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0        0        0     7904 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0        0        0      292 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0        0        0      816 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0        0        0     4277 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/builder.py
--rw-r--r--   0        0        0     4656 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/cli.py
--rw-r--r--   0        0        0        0 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0        0        0     1383 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/base.py
--rw-r--r--   0        0        0     4591 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0        0        0     1832 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/venv.py
--rw-r--r--   0        0        0     1336 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/external.py
--rw-r--r--   0        0        0     1925 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/generation.py
--rw-r--r--   0        0        0      327 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/io.py
--rw-r--r--   0        0        0       30 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0        0        0      212 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0        0        0      190 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0        0        0      137 2024-04-16 23:40:49.769380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0        0        0      109 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0        0        0      170 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/.env
--rw-r--r--   0        0        0     3373 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0        0        0      645 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0        0        0       17 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0        0        0      767 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0        0        0      947 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0        0        0      282 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0        0        0      227 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0        0        0     1124 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0        0        0       84 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0        0        0      157 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0        0        0      208 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0        0        0        0 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0        0        0     1219 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0        0        0      995 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0        0        0       95 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0        0        0      524 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0        0        0      117 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0        0        0      195 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0        0        0      332 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0        0        0     1493 2024-04-16 23:40:49.773380 create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0        0        0     1219 2024-04-16 23:41:01.013374 create_mountaineer_app-0.4.1.dev3/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 create_mountaineer_app-0.4.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1593 2024-04-23 16:37:34.961180 create_mountaineer_app-0.4.2.dev2/README.md
+-rw-r--r--   0        0        0        1 2024-04-23 16:37:34.961349 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:37:34.961421 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-23 16:37:34.961485 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0        0        0     7904 2024-04-23 16:37:34.961563 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0        0        0      292 2024-04-23 16:37:34.961626 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0        0        0      816 2024-04-23 16:37:34.961687 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0        0        0     4277 2024-04-23 16:37:34.961752 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/builder.py
+-rw-r--r--   0        0        0     4656 2024-04-23 16:37:34.961830 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:37:34.961894 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0        0        0     1383 2024-04-23 16:37:34.961953 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/base.py
+-rw-r--r--   0        0        0     4591 2024-04-23 16:37:34.962017 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0        0        0     1832 2024-04-23 16:37:34.962075 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0        0        0     1336 2024-04-23 16:37:34.962134 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/external.py
+-rw-r--r--   0        0        0     1925 2024-04-23 16:37:34.962195 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/generation.py
+-rw-r--r--   0        0        0      327 2024-04-23 16:37:34.962253 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/io.py
+-rw-r--r--   0        0        0       30 2024-04-23 16:37:34.962371 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0        0        0      212 2024-04-23 16:37:34.962427 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-23 16:37:34.962745 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0        0        0      137 2024-04-23 16:37:34.962916 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0        0        0      109 2024-04-23 16:37:34.963020 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0        0        0      170 2024-04-23 16:37:34.963231 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0        0        0     3373 2024-04-23 16:37:34.963305 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0        0        0      645 2024-04-23 16:37:34.963380 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0        0        0       17 2024-04-23 16:37:34.963648 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0        0        0      767 2024-04-23 16:37:34.963743 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0        0        0      947 2024-04-23 16:37:34.963812 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0        0        0      282 2024-04-23 16:37:34.963887 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0        0        0      227 2024-04-23 16:37:34.964074 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-23 16:37:34.964251 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0        0        0     1124 2024-04-23 16:37:34.964339 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0        0        0       84 2024-04-23 16:37:34.964394 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0        0        0      157 2024-04-23 16:37:34.964555 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-23 16:37:34.964629 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:37:34.964705 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-23 16:37:34.964833 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0        0        0      995 2024-04-23 16:37:34.965030 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0        0        0       95 2024-04-23 16:37:34.965093 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0        0        0      524 2024-04-23 16:37:34.965153 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0        0        0      117 2024-04-23 16:37:34.965219 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0        0        0      195 2024-04-23 16:37:34.965284 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0        0        0      332 2024-04-23 16:37:34.965348 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0        0        0     1493 2024-04-23 16:37:34.965569 create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0        0        0     1219 2024-04-23 16:37:59.365704 create_mountaineer_app-0.4.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 create_mountaineer_app-0.4.2.dev2/PKG-INFO
```

### Comparing `create_mountaineer_app-0.4.1.dev3/README.md` & `create_mountaineer_app-0.4.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/common.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/test_builder.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/__tests__/test_generation.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/builder.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/cli.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/base.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/poetry.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/environments/venv.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/external.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/generation.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/.gitignore` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/README.md` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/app.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/cli.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/create_mountaineer_app/templates/project/pyproject.toml` & `create_mountaineer_app-0.4.2.dev2/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.4.1.dev3/pyproject.toml` & `create_mountaineer_app-0.4.2.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "create-mountaineer-app"
-version = "0.4.1.dev3"
+version = "0.4.2.dev2"
 description = ""
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 questionary = "^2.0.1"
```

### Comparing `create_mountaineer_app-0.4.1.dev3/PKG-INFO` & `create_mountaineer_app-0.4.2.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-mountaineer-app
-Version: 0.4.1.dev3
+Version: 0.4.2.dev2
 Summary: 
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

