# Comparing `tmp/paketoi-0.1.0.tar.gz` & `tmp/paketoi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paketoi-0.1.0.tar", max compression
+gzip compressed data, was "paketoi-0.1.1.tar", max compression
```

## Comparing `paketoi-0.1.0.tar` & `paketoi-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1059 2024-04-21 06:03:01.535292 paketoi-0.1.0/LICENSE
--rw-r--r--   0        0        0     1715 2024-04-21 06:27:57.772955 paketoi-0.1.0/README.md
--rw-r--r--   0        0        0     4366 2024-04-21 06:17:04.502194 paketoi-0.1.0/paketoi/__init__.py
--rw-r--r--   0        0        0       60 2024-04-21 06:02:45.460205 paketoi-0.1.0/paketoi/__main__.py
--rw-r--r--   0        0        0    11667 2024-04-21 06:04:15.682571 paketoi-0.1.0/paketoi/resources/cp-python3.10-arm64.json
--rw-r--r--   0        0        0    23773 2024-04-21 06:04:15.682856 paketoi-0.1.0/paketoi/resources/cp-python3.10-x86_64.json
--rw-r--r--   0        0        0    12651 2024-04-21 06:04:15.683108 paketoi-0.1.0/paketoi/resources/cp-python3.11-arm64.json
--rw-r--r--   0        0        0    25833 2024-04-21 06:04:15.683401 paketoi-0.1.0/paketoi/resources/cp-python3.11-x86_64.json
--rw-r--r--   0        0        0    22341 2024-04-21 06:04:15.683899 paketoi-0.1.0/paketoi/resources/cp-python3.12-arm64.json
--rw-r--r--   0        0        0    36383 2024-04-21 06:04:15.684253 paketoi-0.1.0/paketoi/resources/cp-python3.12-x86_64.json
--rw-r--r--   0        0        0     9679 2024-04-21 06:04:15.684526 paketoi-0.1.0/paketoi/resources/cp-python3.8-arm64.json
--rw-r--r--   0        0        0    19619 2024-04-21 06:04:15.685245 paketoi-0.1.0/paketoi/resources/cp-python3.8-x86_64.json
--rw-r--r--   0        0        0    10640 2024-04-21 06:04:15.685476 paketoi-0.1.0/paketoi/resources/cp-python3.9-arm64.json
--rw-r--r--   0        0        0    21628 2024-04-21 06:04:15.685725 paketoi-0.1.0/paketoi/resources/cp-python3.9-x86_64.json
--rw-r--r--   0        0        0      788 2024-04-21 06:37:29.041952 paketoi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 paketoi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-21 06:03:01.535292 paketoi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3812 2024-04-22 16:20:40.853194 paketoi-0.1.1/README.md
+-rw-r--r--   0        0        0     4366 2024-04-21 06:17:04.502194 paketoi-0.1.1/paketoi/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-21 06:02:45.460205 paketoi-0.1.1/paketoi/__main__.py
+-rw-r--r--   0        0        0    11667 2024-04-21 06:04:15.682571 paketoi-0.1.1/paketoi/resources/cp-python3.10-arm64.json
+-rw-r--r--   0        0        0    23773 2024-04-21 06:04:15.682856 paketoi-0.1.1/paketoi/resources/cp-python3.10-x86_64.json
+-rw-r--r--   0        0        0    12651 2024-04-21 06:04:15.683108 paketoi-0.1.1/paketoi/resources/cp-python3.11-arm64.json
+-rw-r--r--   0        0        0    25833 2024-04-21 06:04:15.683401 paketoi-0.1.1/paketoi/resources/cp-python3.11-x86_64.json
+-rw-r--r--   0        0        0    22341 2024-04-21 06:04:15.683899 paketoi-0.1.1/paketoi/resources/cp-python3.12-arm64.json
+-rw-r--r--   0        0        0    36383 2024-04-21 06:04:15.684253 paketoi-0.1.1/paketoi/resources/cp-python3.12-x86_64.json
+-rw-r--r--   0        0        0     9679 2024-04-21 06:04:15.684526 paketoi-0.1.1/paketoi/resources/cp-python3.8-arm64.json
+-rw-r--r--   0        0        0    19619 2024-04-21 06:04:15.685245 paketoi-0.1.1/paketoi/resources/cp-python3.8-x86_64.json
+-rw-r--r--   0        0        0    10640 2024-04-21 06:04:15.685476 paketoi-0.1.1/paketoi/resources/cp-python3.9-arm64.json
+-rw-r--r--   0        0        0    21628 2024-04-21 06:04:15.685725 paketoi-0.1.1/paketoi/resources/cp-python3.9-x86_64.json
+-rw-r--r--   0        0        0      904 2024-04-23 04:15:32.303088 paketoi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 paketoi-0.1.1/PKG-INFO
```

### Comparing `paketoi-0.1.0/LICENSE` & `paketoi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/__init__.py` & `paketoi-0.1.1/paketoi/__init__.py`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.10-arm64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.10-arm64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.10-x86_64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.10-x86_64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.11-arm64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.11-arm64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.11-x86_64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.11-x86_64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.12-arm64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.12-arm64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.12-x86_64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.12-x86_64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.8-arm64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.8-arm64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.8-x86_64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.8-x86_64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.9-arm64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.9-arm64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/paketoi/resources/cp-python3.9-x86_64.json` & `paketoi-0.1.1/paketoi/resources/cp-python3.9-x86_64.json`

 * *Files identical despite different names*

### Comparing `paketoi-0.1.0/pyproject.toml` & `paketoi-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "paketoi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Build AWS Lambda deployment packages (zip files) for Python projects"
 authors = ["Miikka Koskinen <miikka.koskinen@iki.fi>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+license = "MIT"
+homepage = "https://codeberg.org/miikka/paketoi"
+repository = "https://codeberg.org/miikka/paketoi"
 
 [tool.poetry.scripts]
 paketoi = "paketoi:build"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pex = "^2.2.2"
```

