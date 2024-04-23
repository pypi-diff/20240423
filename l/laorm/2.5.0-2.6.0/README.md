# Comparing `tmp/laorm-2.5.0.tar.gz` & `tmp/laorm-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laorm-2.5.0.tar", max compression
+gzip compressed data, was "laorm-2.6.0.tar", max compression
```

## Comparing `laorm-2.5.0.tar` & `laorm-2.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      208 2024-04-22 15:38:09.993985 laorm-2.5.0/laorm/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-12 16:47:47.467701 laorm-2.5.0/laorm/PPA.py
--rw-r--r--   0        0        0    15585 2024-04-22 15:37:38.334525 laorm-2.5.0/laorm/stream.py
--rw-r--r--   0        0        0    11558 2024-01-12 14:31:32.745557 laorm-2.5.0/LICENSE
--rw-r--r--   0        0        0     1362 2024-04-22 15:38:09.789642 laorm-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 laorm-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      208 2024-04-22 15:52:43.277851 laorm-2.6.0/laorm/__init__.py
+-rw-r--r--   0        0        0     1505 2024-04-12 16:47:47.467701 laorm-2.6.0/laorm/PPA.py
+-rw-r--r--   0        0        0    15602 2024-04-22 15:52:17.706716 laorm-2.6.0/laorm/stream.py
+-rw-r--r--   0        0        0    11558 2024-01-12 14:31:32.745557 laorm-2.6.0/LICENSE
+-rw-r--r--   0        0        0     1362 2024-04-22 15:52:43.115003 laorm-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 laorm-2.6.0/PKG-INFO
```

### Comparing `laorm-2.5.0/laorm/PPA.py` & `laorm-2.6.0/laorm/PPA.py`

 * *Files identical despite different names*

### Comparing `laorm-2.5.0/laorm/stream.py` & `laorm-2.6.0/laorm/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         """
         primaryId参数是对主键进行限制
         """
         cls.state_machine.mode = "delete"
 
         if isinstance(primaryId, list) and primaryId != []:
             cls.state_machine.process_keyword(
-                "where", f"{cls.primaryKey} in ({', '.join(map(str, primaryId))})"
+                "where", f"{cls.primaryKey} in ({", ".join(map(lambda id: f"'{id}'", primaryId))})"
             )
         else:
             cls.state_machine.process_keyword("where", f"{cls.primaryKey}={primaryId}")
         await cls.exec(True)
         return cls
 
     @classmethod
```

### Comparing `laorm-2.5.0/LICENSE` & `laorm-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laorm-2.5.0/pyproject.toml` & `laorm-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laorm"
-version = "2.5.0"
+version = "2.6.0"
 description = "A python async orm tool"
 authors = ["larry <176286171@qq.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/mryzhou/laorm"
 
 repository = "https://github.com/mryzhou/laorm.git"  # 可选，指定项目仓库地址
```

### Comparing `laorm-2.5.0/PKG-INFO` & `laorm-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laorm
-Version: 2.5.0
+Version: 2.6.0
 Summary: A python async orm tool
 Home-page: https://github.com/mryzhou/laorm
 License: Apache-2.0
 Author: larry
 Author-email: 176286171@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

