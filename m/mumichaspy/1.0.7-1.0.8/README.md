# Comparing `tmp/mumichaspy-1.0.7.tar.gz` & `tmp/mumichaspy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mumichaspy-1.0.7.tar", last modified: Thu Mar 14 23:55:45 2024, max compression
+gzip compressed data, was "mumichaspy-1.0.8.tar", last modified: Tue Apr 23 08:45:55 2024, max compression
```

## Comparing `mumichaspy-1.0.7.tar` & `mumichaspy-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.238870 mumichaspy-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-14 23:55:45.238870 mumichaspy-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 23:55:45.238870 mumichaspy-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.230870 mumichaspy-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.230870 mumichaspy-1.0.7/src/mumichaspy/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.234870 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.234870 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/crud.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-14 23:55:33.000000 mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/testing_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:55:45.234870 mumichaspy-1.0.7/src/mumichaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-14 23:55:45.000000 mumichaspy-1.0.7/src/mumichaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-14 23:55:45.000000 mumichaspy-1.0.7/src/mumichaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 23:55:45.000000 mumichaspy-1.0.7/src/mumichaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-14 23:55:45.000000 mumichaspy-1.0.7/src/mumichaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-14 23:55:45.000000 mumichaspy-1.0.7/src/mumichaspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.337202 mumichaspy-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 08:45:55.333202 mumichaspy-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:45:55.337202 mumichaspy-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.329202 mumichaspy-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.333202 mumichaspy-1.0.8/src/mumichaspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.333202 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.333202 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-23 08:45:40.000000 mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/testing_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:45:55.333202 mumichaspy-1.0.8/src/mumichaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 08:45:55.000000 mumichaspy-1.0.8/src/mumichaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-23 08:45:55.000000 mumichaspy-1.0.8/src/mumichaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:45:55.000000 mumichaspy-1.0.8/src/mumichaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 08:45:55.000000 mumichaspy-1.0.8/src/mumichaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 08:45:55.000000 mumichaspy-1.0.8/src/mumichaspy.egg-info/top_level.txt
```

### Comparing `mumichaspy-1.0.7/LICENSE` & `mumichaspy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/PKG-INFO` & `mumichaspy-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumichaspy
-Version: 1.0.7
+Version: 1.0.8
 Summary: An implementation of Microservice Chassis pattern in Python
 Author-email: Alain PEREZ RIAÑO <aperez@mondragon.edu>
 Project-URL: Homepage, https://github.com/mu-sse/mumichaspy
 Project-URL: Issues, https://github.com/mu-sse/mumichaspy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mumichaspy-1.0.7/README.md` & `mumichaspy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/pyproject.toml` & `mumichaspy-1.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "mumichaspy/_version.py"
 
 [project]
 name = "mumichaspy"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
     { name="Alain PEREZ RIAÑO", email="aperez@mondragon.edu" },
 ]
 description = "An implementation of Microservice Chassis pattern in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/config.py` & `mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/config.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/mocks.py` & `mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/mocks.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/time.py` & `mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/time.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy/fastapi_jwt_chassis/validation.py` & `mumichaspy-1.0.8/src/mumichaspy/fastapi_jwt_chassis/validation.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/crud.py` & `mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/crud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,116 @@
 # -*- coding: utf-8 -*-
 """CRUD helpers for SQLAlchemy."""
 
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.future import select
+from sqlalchemy.sql.selectable import Select
+from sqlalchemy.orm import DeclarativeMeta
+from typing import Type, Dict, Any, Optional
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 # Generic CRUD functions ##########################################################################
 # READ
 async def get_list(
-    db: AsyncSession, model, offset: int = None, limit: int = None, order_by: str = None
+    db: AsyncSession,
+    model: Type[DeclarativeMeta],
+    offset: Optional[int] = None,
+    limit: Optional[int] = None,
+    order_by: Optional[str] = None,
+    filters: Optional[Dict[str, Any]] = None,
 ):
     """Retrieve a list of elements from database"""
     stmt = select(model)
-    stmt = add_options_to_statement(stmt, offset, limit, order_by, model)
+    stmt = add_options_to_statement(stmt, offset, limit, order_by, model, filters)
     return await get_list_statement_result(db, stmt)
 
 
-async def get_element_by_id(db: AsyncSession, model, element_id):
+async def get_element_by_id(
+    db: AsyncSession, model: Type[DeclarativeMeta], element_id: Any
+):
     """Retrieve any DB element by id."""
     return await db.get(model, element_id)
 
 
-async def get_list_statement_result(db: AsyncSession, stmt):
+async def get_list_statement_result(db: AsyncSession, stmt: Select):
     """Execute given statement and return list of items."""
     result = await db.execute(stmt)
     item_list = result.unique().scalars().all()
     return item_list
 
 
-async def get_first_statement_result(db: AsyncSession, stmt):
+async def get_first_statement_result(db: AsyncSession, stmt: Select):
     """Execute given statement and return the first item."""
     result = await db.execute(stmt)
     item = result.scalar()
     return item
 
 
 # DELETE
-async def delete_element_by_id(db: AsyncSession, model, element_id):
+async def delete_element_by_id(
+    db: AsyncSession, model: Type[DeclarativeMeta], element_id: Any
+):
     """Delete any DB element by id."""
     element = await get_element_by_id(db, model, element_id)
     if element is not None:
         await db.delete(element)
         await db.commit()
     return element
 
 
 # CREATE
-async def create_element(db: AsyncSession, db_element):
+async def create_element(db: AsyncSession, db_element: Type[DeclarativeMeta]):
     """Insert a element in the database."""
 
     try:
         db.add(db_element)
         await db.commit()
         await db.refresh(db_element)
     except Exception as exc:
         logger.error(exc)
         await db.rollback()
         db_element = None
     return db_element
 
 
 # Optional parameters #############################################################################
-def set_order_by_to_statement(stmt, model, order_by):
+def set_order_by_to_statement(
+    stmt: Select, model: Type[DeclarativeMeta], order_by: Optional[str]
+):
     """Adds order by to given statement if needed."""
     if order_by is not None:
         if order_by.startswith("-"):
             stmt = stmt.order_by(getattr(model, order_by[1:]).desc())
         else:
             stmt = stmt.order_by(getattr(model, order_by))
     return stmt
 
 
-def add_options_to_statement(stmt, offset, limit, order_by, model):
+def add_options_to_statement(
+    stmt: Select, offset: int, limit: int, order_by: str, model, filters: dict
+) -> Select:
     """Adds options to given statement if needed: offset, limit, order_by."""
     stmt = set_order_by_to_statement(stmt, model, order_by)
     if offset is not None:
         stmt = stmt.offset(offset)
     if limit is not None:
         stmt = stmt.limit(limit)
+    if filters is not None:
+        stmt = set_filters_to_statement(stmt, model, filters)
+    return stmt
+
+
+def set_filters_to_statement(stmt: Select, model, filters: dict) -> Select:
+    """Adds filters to given statement if needed."""
+    if filters is None:
+        return stmt
+
+    for column, value in filters.items():
+        if hasattr(model, column):
+            stmt = stmt.filter(getattr(model, column) == value)
+        else:
+            logger.warning(f"Column {column} not found in model {model.__name__}")
     return stmt
```

### Comparing `mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/database.py` & `mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/database.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy/sqlalchemy_chassis/testing_helpers.py` & `mumichaspy-1.0.8/src/mumichaspy/sqlalchemy_chassis/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `mumichaspy-1.0.7/src/mumichaspy.egg-info/PKG-INFO` & `mumichaspy-1.0.8/src/mumichaspy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumichaspy
-Version: 1.0.7
+Version: 1.0.8
 Summary: An implementation of Microservice Chassis pattern in Python
 Author-email: Alain PEREZ RIAÑO <aperez@mondragon.edu>
 Project-URL: Homepage, https://github.com/mu-sse/mumichaspy
 Project-URL: Issues, https://github.com/mu-sse/mumichaspy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mumichaspy-1.0.7/src/mumichaspy.egg-info/SOURCES.txt` & `mumichaspy-1.0.8/src/mumichaspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

