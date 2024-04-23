# Comparing `tmp/tipo-kgen-0.0.7.tar.gz` & `tmp/tipo-kgen-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipo-kgen-0.0.7.tar", last modified: Fri Apr 19 07:28:57 2024, max compression
+gzip compressed data, was "tipo-kgen-0.0.8.tar", last modified: Tue Apr 23 07:28:21 2024, max compression
```

## Comparing `tipo-kgen-0.0.7.tar` & `tipo-kgen-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:57.063987 tipo-kgen-0.0.7/
--rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      409 2024-04-19 07:28:57.062986 tipo-kgen-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:57.026945 tipo-kgen-0.0.7/kgen/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.7/kgen/__init__.py
--rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.7/kgen/formatter.py
--rw-rw-rw-   0        0        0     4254 2024-04-19 03:08:22.000000 tipo-kgen-0.0.7/kgen/generate.py
--rw-rw-rw-   0        0        0     1145 2024-04-19 07:28:22.000000 tipo-kgen-0.0.7/kgen/logging.py
--rw-rw-rw-   0        0        0     1072 2024-04-19 06:48:03.000000 tipo-kgen-0.0.7/kgen/metainfo.py
--rw-rw-rw-   0        0        0     2937 2024-04-19 03:14:34.000000 tipo-kgen-0.0.7/kgen/models.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:57.051473 tipo-kgen-0.0.7/kgen/tag-list/
--rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.7/kgen/tag-list/__init__.py
--rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.7/kgen/tag-list/artist.txt
--rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.7/kgen/tag-list/characters.txt
--rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.7/kgen/tag-list/copyrights.txt
--rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.7/kgen/tag-list/meta.txt
--rw-rw-rw-   0        0        0      204 2024-04-19 03:04:45.000000 tipo-kgen-0.0.7/kgen/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:28:57.063987 tipo-kgen-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-19 07:28:31.000000 tipo-kgen-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:57.062986 tipo-kgen-0.0.7/tipo_kgen.egg-info/
--rw-rw-rw-   0        0        0      409 2024-04-19 07:28:56.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-19 07:28:56.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:28:56.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-19 07:28:56.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-19 07:28:56.000000 tipo-kgen-0.0.7/tipo_kgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.737453 tipo-kgen-0.0.8/
+-rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      409 2024-04-23 07:28:21.736448 tipo-kgen-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.708150 tipo-kgen-0.0.8/kgen/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.8/kgen/__init__.py
+-rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.8/kgen/formatter.py
+-rw-rw-rw-   0        0        0     4254 2024-04-19 03:08:22.000000 tipo-kgen-0.0.8/kgen/generate.py
+-rw-rw-rw-   0        0        0     1145 2024-04-19 07:28:22.000000 tipo-kgen-0.0.8/kgen/logging.py
+-rw-rw-rw-   0        0        0     1072 2024-04-19 06:48:03.000000 tipo-kgen-0.0.8/kgen/metainfo.py
+-rw-rw-rw-   0        0        0     2971 2024-04-23 07:27:15.000000 tipo-kgen-0.0.8/kgen/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.718666 tipo-kgen-0.0.8/kgen/tag-list/
+-rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.8/kgen/tag-list/__init__.py
+-rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/artist.txt
+-rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/characters.txt
+-rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/copyrights.txt
+-rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/meta.txt
+-rw-rw-rw-   0        0        0      204 2024-04-19 03:04:45.000000 tipo-kgen-0.0.8/kgen/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:28:21.738452 tipo-kgen-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-23 07:28:17.000000 tipo-kgen-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.736448 tipo-kgen-0.0.8/tipo_kgen.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/top_level.txt
```

### Comparing `tipo-kgen-0.0.7/LICENSE` & `tipo-kgen-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/README.md` & `tipo-kgen-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/formatter.py` & `tipo-kgen-0.0.8/kgen/formatter.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/generate.py` & `tipo-kgen-0.0.8/kgen/generate.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/logging.py` & `tipo-kgen-0.0.8/kgen/logging.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/metainfo.py` & `tipo-kgen-0.0.8/kgen/metainfo.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/models.py` & `tipo-kgen-0.0.8/kgen/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from transformers import LlamaForCausalLM, LlamaTokenizer
 
 from .logging import logger
 
 
 model_dir = pathlib.Path(__file__).parent / "models"
 model_list = [
+    "KBlueLeaf/DanTagGen-delta",
     "KBlueLeaf/DanTagGen-beta",
     "KBlueLeaf/DanTagGen-alpha",
     "KBlueLeaf/DanTagGen-gamma",
 ]
 gguf_name = [
     "ggml-model-Q6_K.gguf",
     "ggml-model-Q8_0.gguf",
```

### Comparing `tipo-kgen-0.0.7/kgen/tag-list/artist.txt` & `tipo-kgen-0.0.8/kgen/tag-list/artist.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/tag-list/characters.txt` & `tipo-kgen-0.0.8/kgen/tag-list/characters.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/tag-list/copyrights.txt` & `tipo-kgen-0.0.8/kgen/tag-list/copyrights.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/kgen/tag-list/meta.txt` & `tipo-kgen-0.0.8/kgen/tag-list/meta.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.7/setup.py` & `tipo-kgen-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tipo-kgen",
     packages=find_packages(),
-    version="0.0.7",
+    version="0.0.8",
     license="Apache 2.0",
     url="https://github.com/KohakuBlueleaf/KGen",
     description=(
         "TIPO: Text to Image genration through "
         "text Presampling with LLMs for Optimal prompting"
     ),
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
```

