# Comparing `tmp/bookcache-0.0.1.tar.gz` & `tmp/bookcache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookcache-0.0.1.tar", max compression
+gzip compressed data, was "bookcache-0.0.2.tar", max compression
```

## Comparing `bookcache-0.0.1.tar` & `bookcache-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-22 22:15:00.120000 bookcache-0.0.1/bookcache/__init__.py
--rw-r--r--   0        0        0      673 2024-04-22 22:26:38.000000 bookcache-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 22:15:00.130000 bookcache-0.0.1/README.md
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 bookcache-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-04-23 18:05:34.000000 bookcache-0.0.2/bookcache/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-23 19:33:18.000000 bookcache-0.0.2/bookcache/cache.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:35:34.000000 bookcache-0.0.2/bookcache/py.typed
+-rw-r--r--   0        0        0      692 2024-04-23 05:28:08.000000 bookcache-0.0.2/bookcache/types/CachedItem.py
+-rw-r--r--   0        0        0      193 2024-04-23 01:38:46.000000 bookcache-0.0.2/bookcache/utils/runner.py
+-rw-r--r--   0        0        0     1093 2024-04-22 23:04:48.000000 bookcache-0.0.2/LICENCE
+-rw-r--r--   0        0        0      799 2024-04-23 20:31:22.000000 bookcache-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-22 22:34:26.000000 bookcache-0.0.2/README.md
+-rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 bookcache-0.0.2/PKG-INFO
```

### Comparing `bookcache-0.0.1/pyproject.toml` & `bookcache-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "bookcache"
-version = "0.0.1"
+version = "0.0.2"
 description = "An in-memory keystore caching system."
 authors = ["NotAussie <NotAussie@duck.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["caching", "cache", "keystore"]
+repository = "https://github.com/NotAussie/bookcache"
+homepage = "https://pypi.org/project/bookcache/"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Framework :: AsyncIO",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Topic :: Database",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+pydantic = "^2.7.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

