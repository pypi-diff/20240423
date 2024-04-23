# Comparing `tmp/linker_atom-0.0.35.tar.gz` & `tmp/linker_atom-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linker_atom-0.0.35.tar", max compression
+gzip compressed data, was "linker_atom-0.0.36.tar", max compression
```

## Comparing `linker_atom-0.0.35.tar` & `linker_atom-0.0.36.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-11-06 06:28:38.000000 linker_atom-0.0.35/LICENSE
--rw-r--r--   0        0        0     6720 2023-11-29 08:34:50.000000 linker_atom-0.0.35/README.md
--rw-r--r--   0        0        0       23 2024-02-06 02:37:19.000000 linker_atom-0.0.35/linker_atom/__init__.py
--rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/__init__.py
--rw-r--r--   0        0        0     1010 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/app.py
--rw-r--r--   0        0        0     2640 2024-02-05 09:56:12.000000 linker_atom-0.0.35/linker_atom/api/base.py
--rw-r--r--   0        0        0      228 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/dependencies.py
--rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/interface/__init__.py
--rw-r--r--   0        0        0      357 2023-11-09 02:57:06.000000 linker_atom-0.0.35/linker_atom/api/interface/healthcheck.py
--rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/middleware/__init__.py
--rw-r--r--   0        0        0     7386 2024-02-05 09:56:12.000000 linker_atom-0.0.35/linker_atom/api/middleware/event.py
--rw-r--r--   0        0        0      829 2024-01-23 09:22:34.000000 linker_atom-0.0.35/linker_atom/api/middleware/http.py
--rw-r--r--   0        0        0      228 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/route.py
--rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/schema/__init__.py
--rw-r--r--   0        0        0      175 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/api/schema/payload.py
--rw-r--r--   0        0        0     1462 2024-01-23 09:22:34.000000 linker_atom-0.0.35/linker_atom/api/schema/response.py
--rw-r--r--   0        0        0     1553 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/compile_run.py
--rw-r--r--   0        0        0     1523 2023-12-07 06:34:17.000000 linker_atom-0.0.35/linker_atom/config/__init__.py
--rw-r--r--   0        0        0      284 2023-11-22 06:34:38.000000 linker_atom-0.0.35/linker_atom/config/logger.py
--rw-r--r--   0        0        0     1321 2023-11-14 02:13:51.000000 linker_atom-0.0.35/linker_atom/config/serving.py
--rw-r--r--   0        0        0      591 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/config/skywalking.py
--rwxr-xr-x   0        0        0   200904 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/dependency/model_protector.so
--rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/lib/__init__.py
--rw-r--r--   0        0        0     3579 2024-01-30 09:37:40.000000 linker_atom-0.0.35/linker_atom/lib/common.py
--rw-r--r--   0        0        0     2199 2024-01-22 08:40:32.000000 linker_atom-0.0.35/linker_atom/lib/exception.py
--rw-r--r--   0        0        0     7105 2023-12-13 09:50:01.000000 linker_atom-0.0.35/linker_atom/lib/load_image.py
--rw-r--r--   0        0        0     9118 2024-02-06 02:37:19.000000 linker_atom-0.0.35/linker_atom/lib/log.py
--rw-r--r--   0        0        0      949 2024-02-05 09:56:12.000000 linker_atom-0.0.35/linker_atom/lib/requests.py
--rw-r--r--   0        0        0     1747 2023-11-06 06:28:38.000000 linker_atom-0.0.35/linker_atom/lib/share_memory.py
--rw-r--r--   0        0        0      727 2024-02-06 02:37:19.000000 linker_atom-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 linker_atom-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-11-06 06:28:38.000000 linker_atom-0.0.36/LICENSE
+-rw-r--r--   0        0        0     6720 2023-11-29 08:34:50.000000 linker_atom-0.0.36/README.md
+-rw-r--r--   0        0        0       23 2024-02-06 02:37:19.000000 linker_atom-0.0.36/linker_atom/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/__init__.py
+-rw-r--r--   0        0        0     1010 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/app.py
+-rw-r--r--   0        0        0     2640 2024-02-05 09:56:12.000000 linker_atom-0.0.36/linker_atom/api/base.py
+-rw-r--r--   0        0        0      228 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/dependencies.py
+-rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/interface/__init__.py
+-rw-r--r--   0        0        0      357 2023-11-09 02:57:06.000000 linker_atom-0.0.36/linker_atom/api/interface/healthcheck.py
+-rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/middleware/__init__.py
+-rw-r--r--   0        0        0     7386 2024-02-05 09:56:12.000000 linker_atom-0.0.36/linker_atom/api/middleware/event.py
+-rw-r--r--   0        0        0      829 2024-01-23 09:22:34.000000 linker_atom-0.0.36/linker_atom/api/middleware/http.py
+-rw-r--r--   0        0        0      228 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/route.py
+-rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/schema/__init__.py
+-rw-r--r--   0        0        0      175 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/api/schema/payload.py
+-rw-r--r--   0        0        0     1462 2024-01-23 09:22:34.000000 linker_atom-0.0.36/linker_atom/api/schema/response.py
+-rw-r--r--   0        0        0     1553 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/compile_run.py
+-rw-r--r--   0        0        0     1640 2024-04-23 02:19:24.000000 linker_atom-0.0.36/linker_atom/config/__init__.py
+-rw-r--r--   0        0        0      284 2023-11-22 06:34:38.000000 linker_atom-0.0.36/linker_atom/config/logger.py
+-rw-r--r--   0        0        0     1321 2023-11-14 02:13:51.000000 linker_atom-0.0.36/linker_atom/config/serving.py
+-rw-r--r--   0        0        0      591 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/config/skywalking.py
+-rwxr-xr-x   0        0        0   200904 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/dependency/model_protector.so
+-rw-r--r--   0        0        0        0 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/lib/__init__.py
+-rw-r--r--   0        0        0     3579 2024-01-30 09:37:40.000000 linker_atom-0.0.36/linker_atom/lib/common.py
+-rw-r--r--   0        0        0     2199 2024-01-22 08:40:32.000000 linker_atom-0.0.36/linker_atom/lib/exception.py
+-rw-r--r--   0        0        0     7105 2023-12-13 09:50:01.000000 linker_atom-0.0.36/linker_atom/lib/load_image.py
+-rw-r--r--   0        0        0     9118 2024-02-06 02:37:19.000000 linker_atom-0.0.36/linker_atom/lib/log.py
+-rw-r--r--   0        0        0      949 2024-02-05 09:56:12.000000 linker_atom-0.0.36/linker_atom/lib/requests.py
+-rw-r--r--   0        0        0     1747 2023-11-06 06:28:38.000000 linker_atom-0.0.36/linker_atom/lib/share_memory.py
+-rw-r--r--   0        0        0      727 2024-04-23 02:20:59.000000 linker_atom-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 linker_atom-0.0.36/PKG-INFO
```

### Comparing `linker_atom-0.0.35/LICENSE` & `linker_atom-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/README.md` & `linker_atom-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/api/app.py` & `linker_atom-0.0.36/linker_atom/api/app.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/api/base.py` & `linker_atom-0.0.36/linker_atom/api/base.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/api/middleware/event.py` & `linker_atom-0.0.36/linker_atom/api/middleware/event.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/api/middleware/http.py` & `linker_atom-0.0.36/linker_atom/api/middleware/http.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/api/schema/response.py` & `linker_atom-0.0.36/linker_atom/api/schema/response.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/compile_run.py` & `linker_atom-0.0.36/linker_atom/compile_run.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/config/__init__.py` & `linker_atom-0.0.36/linker_atom/config/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             return ServingConfig.parse_raw(self.serving_meta_raw)
         return ServingConfig()
     
     @property
     def healthcheck_url(self) -> str:
         if not self.serving_meta_raw:
             return self.atom_api_prefix + self.serving_config.atom_healthcheck_url
+        if not self.serving_config.atom_healthcheck_url:
+            return self.atom_api_prefix + '/v1/health/ping'
         return self.serving_config.atom_healthcheck_url
     
     class Config:
         env_file = "../env"
         env_file_encoding = "utf-8"
         env_prefix = "ATOM_"
         case_sensitive = True
```

### Comparing `linker_atom-0.0.35/linker_atom/config/serving.py` & `linker_atom-0.0.36/linker_atom/config/serving.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/config/skywalking.py` & `linker_atom-0.0.36/linker_atom/config/skywalking.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/dependency/model_protector.so` & `linker_atom-0.0.36/linker_atom/dependency/model_protector.so`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/common.py` & `linker_atom-0.0.36/linker_atom/lib/common.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/exception.py` & `linker_atom-0.0.36/linker_atom/lib/exception.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/load_image.py` & `linker_atom-0.0.36/linker_atom/lib/load_image.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/log.py` & `linker_atom-0.0.36/linker_atom/lib/log.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/requests.py` & `linker_atom-0.0.36/linker_atom/lib/requests.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/linker_atom/lib/share_memory.py` & `linker_atom-0.0.36/linker_atom/lib/share_memory.py`

 * *Files identical despite different names*

### Comparing `linker_atom-0.0.35/pyproject.toml` & `linker_atom-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linker-atom"
-version = "0.0.35"
+version = "0.0.36"
 description = "linker fastapi atom"
 authors = ["hanyu <han_yu@hzlh.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://git.linker.cc/research/common/linker_atom"
 classifiers = [
     'Operating System :: OS Independent',
```

### Comparing `linker_atom-0.0.35/PKG-INFO` & `linker_atom-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linker-atom
-Version: 0.0.35
+Version: 0.0.36
 Summary: linker fastapi atom
 Home-page: https://git.linker.cc/research/common/linker_atom
 License: MIT
 Author: hanyu
 Author-email: han_yu@hzlh.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

