# Comparing `tmp/mlx_vlm-0.0.1.tar.gz` & `tmp/mlx_vlm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.1.tar", last modified: Tue Apr 23 00:27:19 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.2.tar", last modified: Tue Apr 23 00:48:08 2024, max compression
```

## Comparing `mlx_vlm-0.0.1.tar` & `mlx_vlm-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/sample_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24904 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-23 00:27:19.000000 mlx_vlm-0.0.1/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 00:27:19.000000 mlx_vlm-0.0.1/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:27:19.000000 mlx_vlm-0.0.1/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:27:19.000000 mlx_vlm-0.0.1/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 00:27:19.000000 mlx_vlm-0.0.1/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:27:19.883928 mlx_vlm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 00:27:14.000000 mlx_vlm-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/sample_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24904 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/setup.py
```

### Comparing `mlx_vlm-0.0.1/LICENSE` & `mlx_vlm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/convert.py` & `mlx_vlm-0.0.2/mlx_vlm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/generate.py` & `mlx_vlm-0.0.2/mlx_vlm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/base.py` & `mlx_vlm-0.0.2/mlx_vlm/models/base.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.2/mlx_vlm/models/llava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.2/mlx_vlm/models/llava/llava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.2/mlx_vlm/models/llava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.2/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.2/mlx_vlm/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm/utils.py` & `mlx_vlm-0.0.2/mlx_vlm/utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/mlx_vlm.egg-info/SOURCES.txt` & `mlx_vlm-0.0.2/mlx_vlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.1/setup.py` & `mlx_vlm-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 setup(
     name="mlx-vlm",
     version=__version__,
     description="Vision LLMs on Apple silicon with MLX and the Hugging Face Hub",
     long_description=open(root_dir / "README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author_email="prince.gdt@gmail.com",
-    author="MLX Contributors",
+    author="Prince Canuma",
     url="https://github.com/Blaizzy/mlx-vlm",
     license="MIT",
     install_requires=requirements,
     packages=find_packages(where=root_dir),
     python_requires=">=3.8",
 )
```

