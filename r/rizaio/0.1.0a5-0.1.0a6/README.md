# Comparing `tmp/rizaio-0.1.0a5.tar.gz` & `tmp/rizaio-0.1.0a6.tar.gz`

## Comparing `rizaio-0.1.0a5.tar` & `rizaio-0.1.0a6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_base_client.py
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_files.py
--rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_typing.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/lib/.keep
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/resources/__init__.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/resources/v1.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/types/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/types/v1_execute_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/riza/types/v1_execute_response.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_base_client.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_resource.py
--rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/lib/.keep
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/resources/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/resources/sandbox.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/types/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/types/sandbox_execute_params.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/src/rizaio/types/sandbox_execute_response.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 rizaio-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_base_client.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_files.py
+-rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_typing.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/lib/.keep
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/resources/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/resources/v1.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/v1_execute_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/v1_execute_response.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_base_client.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_resource.py
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/lib/.keep
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/resources/__init__.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/resources/command.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/__init__.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/command_exec_params.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/command_exec_response.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/PKG-INFO
```

### Comparing `rizaio-0.1.0a5/src/riza/__init__.py` & `rizaio-0.1.0a6/src/riza/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_base_client.py` & `rizaio-0.1.0a6/src/riza/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_client.py` & `rizaio-0.1.0a6/src/riza/_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_compat.py` & `rizaio-0.1.0a6/src/riza/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_exceptions.py` & `rizaio-0.1.0a6/src/riza/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_files.py` & `rizaio-0.1.0a6/src/riza/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_models.py` & `rizaio-0.1.0a6/src/riza/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_qs.py` & `rizaio-0.1.0a6/src/riza/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_resource.py` & `rizaio-0.1.0a6/src/riza/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_response.py` & `rizaio-0.1.0a6/src/riza/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_streaming.py` & `rizaio-0.1.0a6/src/riza/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_types.py` & `rizaio-0.1.0a6/src/riza/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/__init__.py` & `rizaio-0.1.0a6/src/riza/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_logs.py` & `rizaio-0.1.0a6/src/riza/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_proxy.py` & `rizaio-0.1.0a6/src/riza/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_sync.py` & `rizaio-0.1.0a6/src/riza/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_transform.py` & `rizaio-0.1.0a6/src/riza/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_typing.py` & `rizaio-0.1.0a6/src/riza/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/_utils/_utils.py` & `rizaio-0.1.0a6/src/riza/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/riza/resources/v1.py` & `rizaio-0.1.0a6/src/riza/resources/v1.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/__init__.py` & `rizaio-0.1.0a6/src/rizaio/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_base_client.py` & `rizaio-0.1.0a6/src/rizaio/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_client.py` & `rizaio-0.1.0a6/src/rizaio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "AsyncRiza",
     "Client",
     "AsyncClient",
 ]
 
 
 class Riza(SyncAPIClient):
-    sandbox: resources.Sandbox
+    command: resources.Command
     with_raw_response: RizaWithRawResponse
     with_streaming_response: RizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -100,15 +100,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.sandbox = resources.Sandbox(self)
+        self.command = resources.Command(self)
         self.with_raw_response = RizaWithRawResponse(self)
         self.with_streaming_response = RizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -210,15 +210,15 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncRiza(AsyncAPIClient):
-    sandbox: resources.AsyncSandbox
+    command: resources.AsyncCommand
     with_raw_response: AsyncRizaWithRawResponse
     with_streaming_response: AsyncRizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -268,15 +268,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.sandbox = resources.AsyncSandbox(self)
+        self.command = resources.AsyncCommand(self)
         self.with_raw_response = AsyncRizaWithRawResponse(self)
         self.with_streaming_response = AsyncRizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -379,28 +379,28 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class RizaWithRawResponse:
     def __init__(self, client: Riza) -> None:
-        self.sandbox = resources.SandboxWithRawResponse(client.sandbox)
+        self.command = resources.CommandWithRawResponse(client.command)
 
 
 class AsyncRizaWithRawResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.sandbox = resources.AsyncSandboxWithRawResponse(client.sandbox)
+        self.command = resources.AsyncCommandWithRawResponse(client.command)
 
 
 class RizaWithStreamedResponse:
     def __init__(self, client: Riza) -> None:
-        self.sandbox = resources.SandboxWithStreamingResponse(client.sandbox)
+        self.command = resources.CommandWithStreamingResponse(client.command)
 
 
 class AsyncRizaWithStreamedResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.sandbox = resources.AsyncSandboxWithStreamingResponse(client.sandbox)
+        self.command = resources.AsyncCommandWithStreamingResponse(client.command)
 
 
 Client = Riza
 
 AsyncClient = AsyncRiza
```

### Comparing `rizaio-0.1.0a5/src/rizaio/_compat.py` & `rizaio-0.1.0a6/src/rizaio/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_exceptions.py` & `rizaio-0.1.0a6/src/rizaio/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_files.py` & `rizaio-0.1.0a6/src/rizaio/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_models.py` & `rizaio-0.1.0a6/src/rizaio/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_qs.py` & `rizaio-0.1.0a6/src/rizaio/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_resource.py` & `rizaio-0.1.0a6/src/rizaio/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_response.py` & `rizaio-0.1.0a6/src/rizaio/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_streaming.py` & `rizaio-0.1.0a6/src/rizaio/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_types.py` & `rizaio-0.1.0a6/src/rizaio/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/__init__.py` & `rizaio-0.1.0a6/src/rizaio/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_logs.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_proxy.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_sync.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_transform.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_typing.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/_utils/_utils.py` & `rizaio-0.1.0a6/src/rizaio/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/src/rizaio/resources/sandbox.py` & `rizaio-0.1.0a6/src/rizaio/resources/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Dict, List
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import SandboxExecuteResponse, sandbox_execute_params
+from ..types import CommandExecResponse, command_exec_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -21,41 +21,41 @@
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
 
-__all__ = ["Sandbox", "AsyncSandbox"]
+__all__ = ["Command", "AsyncCommand"]
 
 
-class Sandbox(SyncAPIResource):
+class Command(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> SandboxWithRawResponse:
-        return SandboxWithRawResponse(self)
+    def with_raw_response(self) -> CommandWithRawResponse:
+        return CommandWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> SandboxWithStreamingResponse:
-        return SandboxWithStreamingResponse(self)
+    def with_streaming_response(self) -> CommandWithStreamingResponse:
+        return CommandWithStreamingResponse(self)
 
-    def execute(
+    def exec(
         self,
         *,
         code: str,
         language: Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"],
         args: List[str] | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SandboxExecuteResponse:
+    ) -> CommandExecResponse:
         """Run a script in a secure, isolated sandbox.
 
         Scripts can read from stdin and
         write to stdout or stderr. They can access environment variables and command
         line arguments.
 
         Args:
@@ -83,47 +83,47 @@
                 {
                     "code": code,
                     "language": language,
                     "args": args,
                     "env": env,
                     "stdin": stdin,
                 },
-                sandbox_execute_params.SandboxExecuteParams,
+                command_exec_params.CommandExecParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=SandboxExecuteResponse,
+            cast_to=CommandExecResponse,
         )
 
 
-class AsyncSandbox(AsyncAPIResource):
+class AsyncCommand(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncSandboxWithRawResponse:
-        return AsyncSandboxWithRawResponse(self)
+    def with_raw_response(self) -> AsyncCommandWithRawResponse:
+        return AsyncCommandWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncSandboxWithStreamingResponse:
-        return AsyncSandboxWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncCommandWithStreamingResponse:
+        return AsyncCommandWithStreamingResponse(self)
 
-    async def execute(
+    async def exec(
         self,
         *,
         code: str,
         language: Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"],
         args: List[str] | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SandboxExecuteResponse:
+    ) -> CommandExecResponse:
         """Run a script in a secure, isolated sandbox.
 
         Scripts can read from stdin and
         write to stdout or stderr. They can access environment variables and command
         line arguments.
 
         Args:
@@ -151,50 +151,50 @@
                 {
                     "code": code,
                     "language": language,
                     "args": args,
                     "env": env,
                     "stdin": stdin,
                 },
-                sandbox_execute_params.SandboxExecuteParams,
+                command_exec_params.CommandExecParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=SandboxExecuteResponse,
+            cast_to=CommandExecResponse,
         )
 
 
-class SandboxWithRawResponse:
-    def __init__(self, sandbox: Sandbox) -> None:
-        self._sandbox = sandbox
+class CommandWithRawResponse:
+    def __init__(self, command: Command) -> None:
+        self._command = command
 
-        self.execute = to_raw_response_wrapper(
-            sandbox.execute,
+        self.exec = to_raw_response_wrapper(
+            command.exec,
         )
 
 
-class AsyncSandboxWithRawResponse:
-    def __init__(self, sandbox: AsyncSandbox) -> None:
-        self._sandbox = sandbox
+class AsyncCommandWithRawResponse:
+    def __init__(self, command: AsyncCommand) -> None:
+        self._command = command
 
-        self.execute = async_to_raw_response_wrapper(
-            sandbox.execute,
+        self.exec = async_to_raw_response_wrapper(
+            command.exec,
         )
 
 
-class SandboxWithStreamingResponse:
-    def __init__(self, sandbox: Sandbox) -> None:
-        self._sandbox = sandbox
+class CommandWithStreamingResponse:
+    def __init__(self, command: Command) -> None:
+        self._command = command
 
-        self.execute = to_streamed_response_wrapper(
-            sandbox.execute,
+        self.exec = to_streamed_response_wrapper(
+            command.exec,
         )
 
 
-class AsyncSandboxWithStreamingResponse:
-    def __init__(self, sandbox: AsyncSandbox) -> None:
-        self._sandbox = sandbox
+class AsyncCommandWithStreamingResponse:
+    def __init__(self, command: AsyncCommand) -> None:
+        self._command = command
 
-        self.execute = async_to_streamed_response_wrapper(
-            sandbox.execute,
+        self.exec = async_to_streamed_response_wrapper(
+            command.exec,
         )
```

### Comparing `rizaio-0.1.0a5/src/rizaio/types/sandbox_execute_params.py` & `rizaio-0.1.0a6/src/rizaio/types/command_exec_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Dict, List
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["SandboxExecuteParams"]
+__all__ = ["CommandExecParams"]
 
 
-class SandboxExecuteParams(TypedDict, total=False):
+class CommandExecParams(TypedDict, total=False):
     code: Required[str]
     """The code to execute in the sandbox."""
 
     language: Required[Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"]]
     """The interpreter to use when executing code."""
 
     args: List[str]
```

### Comparing `rizaio-0.1.0a5/src/rizaio/types/sandbox_execute_response.py` & `rizaio-0.1.0a6/src/rizaio/types/command_exec_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Optional
 
 from .._models import BaseModel
 
-__all__ = ["SandboxExecuteResponse"]
+__all__ = ["CommandExecResponse"]
 
 
-class SandboxExecuteResponse(BaseModel):
+class CommandExecResponse(BaseModel):
     exit_code: Optional[int] = None
     """The exit code returned by the script.
 
     Will be `0` on success and non-zero on failure.
     """
 
     stderr: Optional[str] = None
```

### Comparing `rizaio-0.1.0a5/LICENSE` & `rizaio-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a5/pyproject.toml` & `rizaio-0.1.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rizaio"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "The official Python library for the riza API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Riza", email = "hello@riza.io" },
 ]
 dependencies = [
```

### Comparing `rizaio-0.1.0a5/PKG-INFO` & `rizaio-0.1.0a6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rizaio
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: The official Python library for the riza API
 Project-URL: Homepage, https://github.com/riza-io/riza-api-python
 Project-URL: Repository, https://github.com/riza-io/riza-api-python
 Author-email: Riza <hello@riza.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -62,19 +62,19 @@
 from rizaio import Riza
 
 client = Riza(
     # This is the default and can be omitted
     api_key=os.environ.get("RIZA_API_KEY"),
 )
 
-sandbox_execute_response = client.sandbox.execute(
+command_exec_response = client.command.exec(
     code='print("Hello world!")',
     language="PYTHON",
 )
-print(sandbox_execute_response.exit_code)
+print(command_exec_response.exit_code)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `RIZA_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
@@ -90,19 +90,19 @@
 client = AsyncRiza(
     # This is the default and can be omitted
     api_key=os.environ.get("RIZA_API_KEY"),
 )
 
 
 async def main() -> None:
-    sandbox_execute_response = await client.sandbox.execute(
+    command_exec_response = await client.command.exec(
         code='print("Hello world!")',
         language="PYTHON",
     )
-    print(sandbox_execute_response.exit_code)
+    print(command_exec_response.exit_code)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -127,15 +127,15 @@
 ```python
 import rizaio
 from rizaio import Riza
 
 client = Riza()
 
 try:
-    client.sandbox.execute(
+    client.command.exec(
         code='print("Hello world!")',
         language="PYTHON",
     )
 except rizaio.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except rizaio.RateLimitError as e:
@@ -173,15 +173,15 @@
 # Configure the default for all requests:
 client = Riza(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).sandbox.execute(
+client.with_options(max_retries=5).command.exec(
     code='print("Hello world!")',
     language="PYTHON",
 )
 ```
 
 ### Timeouts
 
@@ -199,15 +199,15 @@
 
 # More granular control:
 client = Riza(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).sandbox.execute(
+client.with_options(timeout=5 * 1000).command.exec(
     code='print("Hello world!")',
     language="PYTHON",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
@@ -241,36 +241,36 @@
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from rizaio import Riza
 
 client = Riza()
-response = client.sandbox.with_raw_response.execute(
+response = client.command.with_raw_response.exec(
     code="print(\"Hello world!\")",
     language="PYTHON",
 )
 print(response.headers.get('X-My-Header'))
 
-sandbox = response.parse()  # get the object that `sandbox.execute()` would have returned
-print(sandbox.exit_code)
+command = response.parse()  # get the object that `command.exec()` would have returned
+print(command.exit_code)
 ```
 
 These methods return an [`APIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.sandbox.with_streaming_response.execute(
+with client.command.with_streaming_response.exec(
     code='print("Hello world!")',
     language="PYTHON",
 ) as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
```

