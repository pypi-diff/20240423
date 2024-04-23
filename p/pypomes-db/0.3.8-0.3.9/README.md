# Comparing `tmp/pypomes_db-0.3.8.tar.gz` & `tmp/pypomes_db-0.3.9.tar.gz`

## Comparing `pypomes_db-0.3.8.tar` & `pypomes_db-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    10939 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/PKG-INFO
```

### Comparing `pypomes_db-0.3.8/src/pypomes_db/__init__.py` & `pypomes_db-0.3.9/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.8/src/pypomes_db/db_common.py` & `pypomes_db-0.3.9/src/pypomes_db/db_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
 DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER")
 DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
 DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
 DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
 
 
-def _assert_query_quota(errors: list[str], query: str, where_vals: tuple,
-                        count: int, require_min: int, require_max: int) -> bool:
+def _assert_query_quota(errors: list[str],
+                        query: str,
+                        where_vals: tuple,
+                        count: int,
+                        require_min: int,
+                        require_max: int) -> bool:
 
     # initialize the return variable
     result: bool = True
 
     # has an exact number of tuples been defined but not returned ?
     if isinstance(require_min, int) and isinstance(require_max, int) and \
             require_min == require_max and require_min != count:
@@ -44,15 +48,16 @@
 
     :param exception: the exception raised
     :return: the formatted error message
     """
     return f"Error accessing '{DB_NAME}' at '{DB_HOST}': {str_sanitize(f'{exception}')}"
 
 
-def _db_build_query_msg(query_stmt: str, bind_vals: tuple) -> str:
+def _db_build_query_msg(query_stmt: str,
+                        bind_vals: tuple) -> str:
     """
     Format and return the message indicative of an empty search.
 
     :param query_stmt: the query command
     :param bind_vals: values associated with the query command
     :return: message indicative of empty search
     """
@@ -65,16 +70,19 @@
             else:
                 sval: str = str(val)
             result = result.replace("?", sval, 1)
 
     return result
 
 
-def _db_log(errors: list[str], err_msg: str, logger: Logger,
-            query_stmt: str, bind_vals: tuple = None) -> None:
+def _db_log(errors: list[str],
+            err_msg: str,
+            logger: Logger,
+            query_stmt: str,
+            bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
 
     :param errors: incidental errors
     :param err_msg: the error message
     :param logger: the logger object
     :param query_stmt: the query statement
```

### Comparing `pypomes_db-0.3.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.3.9/src/pypomes_db/db_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         from . import oracle_pomes
     case "postgres":
         from . import postgres_pomes
     case "sqlserver":
         from . import sqlserver_pomes
 
 
-def db_connect(errors: list[str] | None, logger: Logger = None) -> Any:
+def db_connect(errors: list[str] | None,
+               logger: Logger = None) -> Any:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -26,16 +27,19 @@
             result = postgres_pomes.db_connect(errors, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_connect(errors, logger)
 
     return result
 
 
-def db_exists(errors: list[str], table: str,
-              where_attrs: list[str], where_vals: tuple, logger: Logger = None) -> bool:
+def db_exists(errors: list[str],
+              table: str,
+              where_attrs: list[str],
+              where_vals: tuple,
+              logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
     For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
 
     :param errors: incidental error messages
@@ -55,16 +59,19 @@
                                require_nonempty=False,
                                logger=logger)
     result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
-def db_select_one(errors: list[str] | None, sel_stmt: str, where_vals: tuple,
-                  require_nonempty: bool = False, logger: Logger = None) -> tuple:
+def db_select_one(errors: list[str] | None,
+                  sel_stmt: str,
+                  where_vals: tuple,
+                  require_nonempty: bool = False,
+                  logger: Logger = None) -> tuple:
     """
     Search the database and return the first tuple that satisfies the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
 
@@ -82,16 +89,20 @@
                                        require_min=require_min,
                                        require_max=1,
                                        logger=logger)
 
     return reply[0] if reply else None
 
 
-def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
-                  require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
+def db_select_all(errors: list[str] | None,
+                  sel_stmt: str,
+                  where_vals: tuple = None,
+                  require_min: int = None,
+                  require_max: int = None,
+                  logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -112,16 +123,18 @@
             result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max,  logger)
         case "sqlserver":
             result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max, logger)
 
     return result
 
 
-def db_insert(errors: list[str] | None, insert_stmt: str,
-              insert_vals: tuple, logger: Logger = None) -> int:
+def db_insert(errors: list[str] | None,
+              insert_stmt: str,
+              insert_vals: tuple,
+              logger: Logger = None) -> int:
     """
     Insert a tuple, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param logger: optional logger
@@ -135,16 +148,19 @@
             result = postgres_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
-def db_update(errors: list[str] | None, update_stmt: str,
-              update_vals: tuple, where_vals: tuple, logger: Logger = None) -> int:
+def db_update(errors: list[str] | None,
+              update_stmt: str,
+              update_vals: tuple,
+              where_vals: tuple,
+              logger: Logger = None) -> int:
     """
     Update one or more tuples in the database, as defined by the command *update_stmt*.
 
     The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
 
     :param errors: incidental error messages
@@ -163,16 +179,18 @@
             result = postgres_pomes.db_modify(errors, update_stmt, values, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_modify(errors, update_stmt, values, logger)
 
     return result
 
 
-def db_delete(errors: list[str] | None, delete_stmt: str,
-              where_vals: tuple, logger: Logger = None) -> int:
+def db_delete(errors: list[str] | None,
+              delete_stmt: str,
+              where_vals: tuple,
+              logger: Logger = None) -> int:
     """
     Delete one or more tuples in the database, as defined by the *delete_stmt* command.
 
     The values for selecting the tuples to be deleted are in *where_vals*.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
@@ -188,16 +206,18 @@
             result = postgres_pomes.db_modify(errors, delete_stmt, where_vals, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_modify(errors, delete_stmt, where_vals, logger)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
-                   insert_vals: list[tuple], logger: Logger = None) -> int:
+def db_bulk_insert(errors: list[str] | None,
+                   insert_stmt: str,
+                   insert_vals: list[tuple],
+                   logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
@@ -209,16 +229,18 @@
             result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
-def db_call_function(errors: list[str] | None, func_name: str,
-                     func_vals: tuple, logger: Logger = None) -> list[tuple]:
+def db_call_function(errors: list[str] | None,
+                     func_name: str,
+                     func_vals: tuple,
+                     logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param logger: optional logger
@@ -232,16 +254,18 @@
             result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
 
     return result
 
 
-def db_call_procedure(errors: list[str] | None, proc_name: str,
-                      proc_vals: tuple, logger: Logger = None) -> list[tuple]:
+def db_call_procedure(errors: list[str] | None,
+                      proc_name: str,
+                      proc_vals: tuple,
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param logger: optional logger
```

### Comparing `pypomes_db-0.3.8/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.3.9/src/pypomes_db/oracle_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from oracledb import Connection, connect
 
 from .db_common import (
     DB_NAME, DB_HOST, DB_PORT, DB_PWD, DB_USER,
     _assert_query_quota, _db_log, _db_except_msg
 )
 
-# TODO: db_bulk_insert, db_exec_stored_procedure
+# TODO: db_bulk_insert, db_call_function, db_call_procedure
 
 
 def db_connect(errors: list[str], logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
@@ -34,16 +34,20 @@
 
     # log the results
     _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
-                  require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
+def db_select_all(errors: list[str] | None,
+                  sel_stmt: str,
+                  where_vals: tuple = None,
+                  require_min: int = None,
+                  require_max: int = None,
+                  logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -92,16 +96,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, sel_stmt, where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
-                   insert_vals: list[tuple], logger: Logger = None) -> int:
+def db_bulk_insert(errors: list[str] | None,
+                   insert_stmt: str,
+                   insert_vals: list[tuple],
+                   logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
@@ -136,16 +142,18 @@
     # log the results
     _db_log(errors, err_msg, logger, insert_stmt, insert_vals[0])
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def db_call_function(errors: list[str] | None, func_name: str,
-                     func_vals: tuple, logger: Logger = None) -> list[tuple]:
+def db_call_function(errors: list[str] | None,
+                     func_name: str,
+                     func_vals: tuple,
+                     logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param logger: optional logger
@@ -178,16 +186,18 @@
     # log the results
     _db_log(errors, err_msg, logger, func_name, func_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def db_call_procedure(errors: list[str] | None, proc_name: str,
-                      proc_vals: tuple, logger: Logger = None) -> list[tuple]:
+def db_call_procedure(errors: list[str] | None,
+                      proc_name: str,
+                      proc_vals: tuple,
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param logger: optional logger
@@ -220,15 +230,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, proc_name, proc_vals)
 
     return result
 
 
-def db_modify(errors: list[str] | None, modify_stmt: str, bind_vals: tuple | list[tuple], logger: Logger) -> int:
+def db_modify(errors: list[str] | None,
+              modify_stmt: str,
+              bind_vals: tuple | list[tuple],
+              logger: Logger) -> int:
     """
     Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
 
     The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
```

### Comparing `pypomes_db-0.3.8/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.3.9/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from .db_common import (
     DB_NAME, DB_HOST, DB_PORT, DB_PWD, DB_USER,
     _assert_query_quota, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str] | None, logger: Logger = None) -> connection:
+def db_connect(errors: list[str] | None,
+               logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -34,16 +35,20 @@
 
     # log the results
     _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None, sel_stmt: str, where_vals: tuple,
-                  require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
+def db_select_all(errors: list[str] | None,
+                  sel_stmt: str,
+                  where_vals: tuple = None,
+                  require_min: int = None,
+                  require_max: int = None,
+                  logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -91,16 +96,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, sel_stmt, where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
-                   insert_vals: list[tuple], logger: Logger = None) -> int:
+def db_bulk_insert(errors: list[str] | None,
+                   insert_stmt: str,
+                   insert_vals: list[tuple],
+                   logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The 'VALUES' clause in *insert_stmt' must be simply 'VALUES %s'.
     Note that, after the execution of 'execute_values', the 'cursor.rowcount' property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
@@ -137,16 +144,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, insert_stmt)
 
     return result
 
 
-def db_call_procedure(errors: list[str] | None, proc_name: str,
-                      proc_vals: tuple, logger: Logger = None) -> list[tuple]:
+def db_call_procedure(errors: list[str] | None,
+                      proc_name: str,
+                      proc_vals: tuple,
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
     :param logger: optional logger
@@ -183,15 +192,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, proc_stmt, proc_vals)
 
     return result
 
 
-def db_modify(errors: list[str] | None, modify_stmt: str, bind_vals: tuple | list[tuple], logger: Logger) -> int:
+def db_modify(errors: list[str] | None,
+              modify_stmt: str,
+              bind_vals: tuple | list[tuple],
+              logger: Logger) -> int:
     """
     Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
 
     The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
```

### Comparing `pypomes_db-0.3.8/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.3.9/src/pypomes_db/sqlserver_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 __db_driver: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
 __CONNECTION_KWARGS: Final[str] = (
     f"DRIVER={{{__db_driver}}};SERVER={DB_HOST},{DB_PORT};"
     f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
 )
 
 
-def db_connect(errors: list[str] | None, logger: Logger = None) -> Connection:
+def db_connect(errors: list[str] | None,
+               logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -35,16 +36,20 @@
 
     # log the results
     _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
-                  require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
+def db_select_all(errors: list[str] | None,
+                  sel_stmt: str,
+                  where_vals: tuple = None,
+                  require_min: int = None,
+                  require_max: int = None,
+                  logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -88,16 +93,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, sel_stmt, where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
-                   insert_vals: list[tuple], logger: Logger = None) -> int:
+def db_bulk_insert(errors: list[str] | None,
+                   insert_stmt: str,
+                   insert_vals: list[tuple],
+                   logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
@@ -128,16 +135,20 @@
 
     # log the results
     _db_log(errors, err_msg, logger, insert_stmt, insert_vals[0])
 
     return result
 
 
-def db_call_procedure(errors: list[str] | None, proc_name: str, proc_vals: tuple,
-                      require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
+def db_call_procedure(errors: list[str] | None,
+                      proc_name: str,
+                      proc_vals: tuple,
+                      require_min: int = None,
+                      require_max: int = None,
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param require_min: optionally defines the minimum number of tuples to be returned
@@ -178,15 +189,18 @@
 
     # log the results
     _db_log(errors, err_msg, logger, proc_stmt, proc_vals)
 
     return result
 
 
-def db_modify(errors: list[str] | None, modify_stmt: str, bind_vals: tuple | list[tuple], logger: Logger) -> int:
+def db_modify(errors: list[str] | None,
+              modify_stmt: str,
+              bind_vals: tuple | list[tuple],
+              logger: Logger) -> int:
     """
     Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
 
     The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
```

### Comparing `pypomes_db-0.3.8/LICENSE` & `pypomes_db-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.8/pyproject.toml` & `pypomes_db-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
 #   "oracledb>=2.1.1",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=0.7.3",
+    "pypomes_core>=0.8.7",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.3.8/PKG-INFO` & `pypomes_db-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.3.8
+Version: 0.3.9
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.7.3
+Requires-Dist: pypomes-core>=0.8.7
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

