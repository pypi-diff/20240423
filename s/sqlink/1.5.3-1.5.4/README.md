# Comparing `tmp/sqlink-1.5.3.tar.gz` & `tmp/sqlink-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlink-1.5.3.tar", last modified: Wed Apr  3 01:20:37 2024, max compression
+gzip compressed data, was "sqlink-1.5.4.tar", last modified: Tue Apr 23 08:40:31 2024, max compression
```

## Comparing `sqlink-1.5.3.tar` & `sqlink-1.5.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.819467 sqlink-1.5.3/
--rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1044 2024-04-03 01:20:37.819467 sqlink-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 01:20:37.819467 sqlink-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      642 2024-04-03 01:16:11.000000 sqlink-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.776151 sqlink-1.5.3/sqlink/
--rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.3/sqlink/__init__.py
--rw-rw-rw-   0        0        0    23642 2024-04-03 01:04:37.000000 sqlink-1.5.3/sqlink/dao.py
--rw-rw-rw-   0        0        0     4738 2024-03-18 10:38:12.000000 sqlink-1.5.3/sqlink/database.py
--rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.3/sqlink/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.803838 sqlink-1.5.3/sqlink.egg-info/
--rw-rw-rw-   0        0        0     1044 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.819467 sqlink-1.5.3/test/
--rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_basic_dao.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_comment.py
--rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_create_table.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_database.py
--rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_entity.py
--rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.3/test/test_entity_check_ignore_type.py
--rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_entity_parse.py
--rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_env.py
--rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_execte_sql_with_daofunc.py
--rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_execute_sql_without_dao_func.py
--rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_fetch_one.py
--rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_fetch_type.py
--rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_foreign_key.py
--rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_handle_bool.py
--rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_ignore.py
--rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_insert_conflict.py
--rw-rw-rw-   0        0        0      526 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_main.py
--rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_select_one_field.py
--rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_table_substitute.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.740952 sqlink-1.5.4/
+-rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1044 2024-04-23 08:40:31.739966 sqlink-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:40:31.740952 sqlink-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      642 2024-04-23 08:39:49.000000 sqlink-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.700437 sqlink-1.5.4/sqlink/
+-rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.4/sqlink/__init__.py
+-rw-rw-rw-   0        0        0    24034 2024-04-23 08:34:25.000000 sqlink-1.5.4/sqlink/dao.py
+-rw-rw-rw-   0        0        0     4738 2024-03-18 10:38:12.000000 sqlink-1.5.4/sqlink/database.py
+-rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.4/sqlink/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.716451 sqlink-1.5.4/sqlink.egg-info/
+-rw-rw-rw-   0        0        0     1044 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.738961 sqlink-1.5.4/test/
+-rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_basic_dao.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_comment.py
+-rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_create_table.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_database.py
+-rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_entity.py
+-rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.4/test/test_entity_check_ignore_type.py
+-rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_entity_parse.py
+-rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_env.py
+-rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_execte_sql_with_daofunc.py
+-rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_execute_sql_without_dao_func.py
+-rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_fetch_one.py
+-rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_fetch_type.py
+-rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_foreign_key.py
+-rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_handle_bool.py
+-rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_ignore.py
+-rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_insert_conflict.py
+-rw-rw-rw-   0        0        0      526 2024-04-23 08:39:29.000000 sqlink-1.5.4/test/test_main.py
+-rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_select_one_field.py
+-rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_table_substitute.py
```

### Comparing `sqlink-1.5.3/LICENSE.txt` & `sqlink-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/PKG-INFO` & `sqlink-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.3
+Version: 1.5.4
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: Nanhai
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.3/README.md` & `sqlink-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/setup.py` & `sqlink-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_pypi.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlink",
-    version="1.5.3",
+    version="1.5.4",
     author="Nanhai",
     author_email="nanhai@163.com",
     description="a efficient and concise sql framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/sqlink",
     packages=['sqlink'],
```

### Comparing `sqlink-1.5.3/sqlink/dao.py` & `sqlink-1.5.4/sqlink/dao.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 import copy
-from collections import namedtuple
+from collections import namedtuple, OrderedDict
 from dataclasses import make_dataclass, dataclass
 
 from sqlink.entity import _parse_constraints, is_entity, FOREIGN_KEY_PLACEHOLDER, \
     CONSTRAINT_TYPE_IGNORE, CONSTRAINT_TYPE_AUTO_PRIMARY_KEY, CONSTRAINT_TYPE_FOREIGN_KEY, \
     CONSTRAINT_TYPE_DATATYPE, CONSTRAINT_TYPE_COMMENT
 
 # ====================================================================================================================
 # 模块常量
 TABLE_SUBSTITUTE = '__'  # 约定的表名代替符，内部可自动替换为与Dao绑定的Entity的类名。
 FETCH_FLAG = ('limit 1', 'limit 1;')
 _DATACLASS = 'dataclass'
 _RECORD = 'Record'
-_ENABLED_BASIC_TYPES = (int, str, float, bytes, bool)
 PLACEHOLDER_DEFAULT = "?"
 PLACEHOLDER_SQLITE = "?"
 PLACEHOLDER_MYSQL = "%s"
 DB_TYPE_SQLITE = "sqlite"
 DB_TYPE_MYSQL = "mysql"
 PRIMARY_KEY_AUTO_FLAG_SQLITE = "AUTOINCREMENT"
 PRIMARY_KEY_AUTO_FLAG_MYSQL = "AUTO_INCREMENT"
@@ -526,14 +525,22 @@
     fields = [column[0] for column in cursor.description]
     Record = make_dataclass(_RECORD, fields)  # noqa
     if is_list:
         return [Record(*row) for row in result]
     return Record(*result)
 
 
+def __return_ordered_dict(cursor, result, is_list=True):
+    """返回查询结果为顺序字典"""
+    fields = [column[0] for column in cursor.description]
+    if is_list:
+        return [OrderedDict(zip(fields, item)) for item in result]
+    return OrderedDict(zip(fields, result))
+
+
 def __return_dict(cursor, result, is_list=True):
     """返回查询结果为字典"""
     fields = [column[0] for column in cursor.description]
     if is_list:
         return [dict(zip(fields, item)) for item in result]
     return dict(zip(fields, result))
 
@@ -585,22 +592,25 @@
     # 不做转换
     if not result or _fetch_type == tuple:
         return result
 
     elif is_entity(_fetch_type):
         return __return_entity(entity=_fetch_type, cursor=cursor, result=result, is_list=is_list)
 
-    elif _fetch_type in _ENABLED_BASIC_TYPES:
+    elif _fetch_type in (int, str, float, bytes, bool):
         return __return_one_field(result=result, fetch_type=_fetch_type, is_list=is_list)
 
     elif _fetch_type == _DATACLASS:
         return __return_dataclass(cursor=cursor, result=result, is_list=is_list)
 
     elif _fetch_type == dict:
         return __return_dict(cursor=cursor, result=result, is_list=is_list)
 
+    elif _fetch_type == "ordered_dict":
+        return __return_ordered_dict(cursor=cursor, result=result, is_list=is_list)
+
     elif _fetch_type == namedtuple:
         return __return_namedtuple(cursor=cursor, result=result, is_list=is_list)
 
     else:
         raise TypeError(
             f"Dao的查询结果格式设置错误，应该属于: 'tuple' 'dict' 'dataclass' 'entity'，但得到的是: {_fetch_type}")
```

### Comparing `sqlink-1.5.3/sqlink/database.py` & `sqlink-1.5.4/sqlink/database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/sqlink/entity.py` & `sqlink-1.5.4/sqlink/entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/sqlink.egg-info/PKG-INFO` & `sqlink-1.5.4/sqlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.3
+Version: 1.5.4
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: Nanhai
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.3/sqlink.egg-info/SOURCES.txt` & `sqlink-1.5.4/sqlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_basic_dao.py` & `sqlink-1.5.4/test/test_basic_dao.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_comment.py` & `sqlink-1.5.4/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_create_table.py` & `sqlink-1.5.4/test/test_create_table.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_database.py` & `sqlink-1.5.4/test/test_database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_entity.py` & `sqlink-1.5.4/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_entity_check_ignore_type.py` & `sqlink-1.5.4/test/test_entity_check_ignore_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_entity_parse.py` & `sqlink-1.5.4/test/test_entity_parse.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_env.py` & `sqlink-1.5.4/test/test_env.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_execte_sql_with_daofunc.py` & `sqlink-1.5.4/test/test_execte_sql_with_daofunc.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_execute_sql_without_dao_func.py` & `sqlink-1.5.4/test/test_execute_sql_without_dao_func.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_fetch_one.py` & `sqlink-1.5.4/test/test_fetch_one.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_fetch_type.py` & `sqlink-1.5.4/test/test_fetch_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_foreign_key.py` & `sqlink-1.5.4/test/test_foreign_key.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_handle_bool.py` & `sqlink-1.5.4/test/test_handle_bool.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_ignore.py` & `sqlink-1.5.4/test/test_ignore.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_insert_conflict.py` & `sqlink-1.5.4/test/test_insert_conflict.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_main.py` & `sqlink-1.5.4/test/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_select_one_field.py` & `sqlink-1.5.4/test/test_select_one_field.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.3/test/test_table_substitute.py` & `sqlink-1.5.4/test/test_table_substitute.py`

 * *Files identical despite different names*

