# Comparing `tmp/lazy_mongo_log-0.1.3.tar.gz` & `tmp/lazy_mongo_log-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo_log-0.1.3.tar", max compression
+gzip compressed data, was "lazy_mongo_log-0.1.5.tar", max compression
```

## Comparing `lazy_mongo_log-0.1.3.tar` & `lazy_mongo_log-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3109 2024-04-16 01:31:03.429959 lazy_mongo_log-0.1.3/README.md
--rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.3/lazy_mongo_log/__init__.py
--rw-r--r--   0        0        0     4455 2024-04-05 05:22:01.113043 lazy_mongo_log-0.1.3/lazy_mongo_log/lazy_mongo_log.py
--rw-r--r--   0        0        0      203 2024-04-16 07:06:33.271199 lazy_mongo_log-0.1.3/lazy_mongo_log/schemas.py
--rw-r--r--   0        0        0      323 2024-04-16 07:08:43.370358 lazy_mongo_log-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3109 2024-04-16 01:31:03.429959 lazy_mongo_log-0.1.5/README.md
+-rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.5/lazy_mongo_log/__init__.py
+-rw-r--r--   0        0        0     4526 2024-04-17 07:10:52.946569 lazy_mongo_log-0.1.5/lazy_mongo_log/lazy_mongo_log.py
+-rw-r--r--   0        0        0      199 2024-04-23 01:18:37.121916 lazy_mongo_log-0.1.5/lazy_mongo_log/schemas.py
+-rw-r--r--   0        0        0      323 2024-04-23 01:17:00.583251 lazy_mongo_log-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.5/PKG-INFO
```

### Comparing `lazy_mongo_log-0.1.3/README.md` & `lazy_mongo_log-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lazy_mongo_log-0.1.3/lazy_mongo_log/lazy_mongo_log.py` & `lazy_mongo_log-0.1.5/lazy_mongo_log/lazy_mongo_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
                     type=type,
                     keyword=keyword,
                 )
 
                 if log_selector != None:
                     document = log_selector(document, **kwargs)
 
+                if document == None:
+                    return False
+
                 result = self.collection.insert_one(document)
 
                 return result.acknowledged
             except:
                 return False
 
         return True
```

### Comparing `lazy_mongo_log-0.1.3/PKG-INFO` & `lazy_mongo_log-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lazy-mongo-log
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: lazy-schema (>=0.2.1,<0.3.0)
+Requires-Dist: lazy-schema (>=0.2.6,<0.3.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Lazy Mongo Log
 Write to MongoDB as you print!
 
 # Installation
```

