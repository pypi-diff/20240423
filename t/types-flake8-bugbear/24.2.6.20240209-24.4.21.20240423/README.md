# Comparing `tmp/types-flake8-bugbear-24.2.6.20240209.tar.gz` & `tmp/types-flake8-bugbear-24.4.21.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-bugbear-24.2.6.20240209.tar", last modified: Fri Feb  9 02:12:29 2024, max compression
+gzip compressed data, was "types-flake8-bugbear-24.4.21.20240423.tar", last modified: Tue Apr 23 02:19:16 2024, max compression
```

## Comparing `types-flake8-bugbear-24.2.6.20240209.tar` & `types-flake8-bugbear-24.4.21.20240423.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:12:29.638361 types-flake8-bugbear-24.2.6.20240209/
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-09 02:12:29.638361 types-flake8-bugbear-24.2.6.20240209/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:12:29.638361 types-flake8-bugbear-24.2.6.20240209/bugbear-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/bugbear-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/bugbear-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/bugbear-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 02:12:29.638361 types-flake8-bugbear-24.2.6.20240209/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-09 02:12:26.000000 types-flake8-bugbear-24.2.6.20240209/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:12:29.638361 types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-09 02:12:29.000000 types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-09 02:12:29.000000 types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 02:12:29.000000 types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-09 02:12:29.000000 types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:16.308453 types-flake8-bugbear-24.4.21.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 02:19:16.308453 types-flake8-bugbear-24.4.21.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:16.308453 types-flake8-bugbear-24.4.21.20240423/bugbear-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/bugbear-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/bugbear-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/bugbear-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:16.308453 types-flake8-bugbear-24.4.21.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-23 02:19:15.000000 types-flake8-bugbear-24.4.21.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:16.308453 types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 02:19:16.000000 types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 02:19:16.000000 types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:16.000000 types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 02:19:16.000000 types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/top_level.txt
```

### Comparing `types-flake8-bugbear-24.2.6.20240209/CHANGELOG.md` & `types-flake8-bugbear-24.4.21.20240423/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+## 24.4.21.20240423 (2024-04-23)
+
+[stubsabot] Bump flake8-bugbear to 24.4.21 (#11806)
+
+Release: https://pypi.org/pypi/flake8-bugbear/24.4.21
+Homepage: https://github.com/PyCQA/flake8-bugbear
+Repository: https://github.com/PyCQA/flake8-bugbear
+Typeshed stubs: https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear
+Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
+Diff: https://github.com/PyCQA/flake8-bugbear/compare/24.2.6...24.4.21
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `bugbear.py`.
+ - Total lines of Python code added: 192.
+ - Total lines of Python code deleted: 88.
+
 ## 24.2.6.20240209 (2024-02-09)
 
 [stubsabot] Bump flake8-bugbear to 24.2.6 (#11379)
 
 ## 24.1.17.20240201 (2024-02-01)
 
 [stubsabot] Bump flake8-bugbear to 24.1.17 (#11278)
```

### Comparing `types-flake8-bugbear-24.2.6.20240209/PKG-INFO` & `types-flake8-bugbear-24.4.21.20240423/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 24.2.6.20240209
+Version: 24.4.21.20240423
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`.
 
 This version of `types-flake8-bugbear` aims to provide accurate annotations
-for `flake8-bugbear==24.2.6`.
+for `flake8-bugbear==24.4.21`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4eeb0e62bbf5d0e302043a10c2e14caafd40378d` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-flake8-bugbear-24.2.6.20240209/bugbear-stubs/__init__.pyi` & `types-flake8-bugbear-24.4.21.20240423/bugbear-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-bugbear-24.2.6.20240209/setup.py` & `types-flake8-bugbear-24.4.21.20240423/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`.
 
 This version of `types-flake8-bugbear` aims to provide accurate annotations
-for `flake8-bugbear==24.2.6`.
+for `flake8-bugbear==24.4.21`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4eeb0e62bbf5d0e302043a10c2e14caafd40378d` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="24.2.6.20240209",
+      version="24.4.21.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md",
```

### Comparing `types-flake8-bugbear-24.2.6.20240209/types_flake8_bugbear.egg-info/PKG-INFO` & `types-flake8-bugbear-24.4.21.20240423/types_flake8_bugbear.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 24.2.6.20240209
+Version: 24.4.21.20240423
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`.
 
 This version of `types-flake8-bugbear` aims to provide accurate annotations
-for `flake8-bugbear==24.2.6`.
+for `flake8-bugbear==24.4.21`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4eeb0e62bbf5d0e302043a10c2e14caafd40378d` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

