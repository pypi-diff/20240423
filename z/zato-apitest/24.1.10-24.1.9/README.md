# Comparing `tmp/zato_apitest-24.1.10.tar.gz` & `tmp/zato-apitest-24.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.10.tar", last modified: Tue Apr 23 13:28:48 2024, max compression
+gzip compressed data, was "zato-apitest-24.1.9.tar", last modified: Tue Mar 12 11:43:29 2024, max compression
```

## Comparing `zato_apitest-24.1.10.tar` & `zato-apitest-24.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    42880 2019-06-24 21:01:23.000000 zato_apitest-24.1.10/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.10/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.10/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.10/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2635 2024-04-23 13:28:22.000000 zato_apitest-24.1.10/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.719539 zato_apitest-24.1.10/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.719539 zato_apitest-24.1.10/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      227 2024-03-10 13:49:27.000000 zato_apitest-24.1.10/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1816 2024-03-10 14:48:12.000000 zato_apitest-24.1.10/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4343 2024-03-11 14:35:09.000000 zato_apitest-24.1.10/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      226 2024-03-11 14:35:24.000000 zato_apitest-24.1.10/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4721 2024-03-11 14:47:07.000000 zato_apitest-24.1.10/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1882 2024-03-11 14:38:08.000000 zato_apitest-24.1.10/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      172 2024-03-11 12:18:58.000000 zato_apitest-24.1.10/src/zato/apitest/steps/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29967 2024-04-23 13:22:38.000000 zato_apitest-24.1.10/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22095 2024-03-12 11:34:29.000000 zato_apitest-24.1.10/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7341 2024-03-11 14:38:39.000000 zato_apitest-24.1.10/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13748 2024-03-11 14:38:52.000000 zato_apitest-24.1.10/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-23 13:28:48.723539 zato_apitest-24.1.10/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-23 13:28:46.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-23 13:28:48.000000 zato_apitest-24.1.10/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    42880 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato-apitest-24.1.9/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato-apitest-24.1.9/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2634 2024-03-12 11:43:11.000000 zato-apitest-24.1.9/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      227 2024-03-10 13:49:27.000000 zato-apitest-24.1.9/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1816 2024-03-10 14:48:12.000000 zato-apitest-24.1.9/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4343 2024-03-11 14:35:09.000000 zato-apitest-24.1.9/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      226 2024-03-11 14:35:24.000000 zato-apitest-24.1.9/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4721 2024-03-11 14:47:07.000000 zato-apitest-24.1.9/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1882 2024-03-11 14:38:08.000000 zato-apitest-24.1.9/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      172 2024-03-11 12:18:58.000000 zato-apitest-24.1.9/src/zato/apitest/steps/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29777 2024-03-12 11:41:01.000000 zato-apitest-24.1.9/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22095 2024-03-12 11:34:29.000000 zato-apitest-24.1.9/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7341 2024-03-11 14:38:39.000000 zato-apitest-24.1.9/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13748 2024-03-11 14:38:52.000000 zato-apitest-24.1.9/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:27.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.10/LICENSE.txt` & `zato-apitest-24.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/PKG-INFO` & `zato-apitest-24.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.10
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.10 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.10/setup.py` & `zato-apitest-24.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.10'
+version = '24.1.9'
 
 LONG_DESCRIPTION = """
 
 Write API tests for your [API integrations](https://zato.io) in plain English, with no programming needed.
 
 Here is how it looks:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- """ Copyright (C) 2024, Zato Source s.r.o. https://
 zato.io Proprietary product. This is not open source software, reproduction is
 prohibited. """ # stdlib import os from setuptools import setup, find_packages
-version = '24.1.10' LONG_DESCRIPTION = """ Write API tests for your [API
+version = '24.1.9' LONG_DESCRIPTION = """ Write API tests for your [API
 integrations](https://zato.io) in plain English, with no programming needed.
 Here is how it looks: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/
 _r_o_o_t_/_s_t_a_t_i_c_/_i_m_g_/_a_p_i_t_e_s_t_/_a_p_i_t_e_s_t_._j_p_g_) More information about API testing at
 https://zato.io. """ def parse_requirements(requirements): # type: ignore
 ignored = ['#', 'setuptools', '-e'] with open(requirements) as f: return [line
 for line in f if line.strip() and not any(line.startswith(prefix) for prefix in
 ignored)] setup( name = 'zato-apitest', version = version, scripts = ['src/
```

### Comparing `zato_apitest-24.1.10/src/zato/apitest/__init__.py` & `zato-apitest-24.1.9/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/cli.py` & `zato-apitest-24.1.9/src/zato/apitest/cli.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/init.py` & `zato-apitest-24.1.9/src/zato/apitest/init.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/run.py` & `zato-apitest-24.1.9/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/steps/common.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,33 +97,28 @@
     address = ctx.zato.request.get('address')
     url_path = ctx.zato.request.get('url_path', '/')
     qs = ctx.zato.request.get('query_string', '')
     files = None
     data = ''
 
     if 'data_impl' in ctx.zato.request:
-        if ctx.zato.request.get('is_xml'):
+        if ctx.zato.request.is_xml:
             data = etree.tostring(ctx.zato.request.data_impl)
-        elif ctx.zato.request.get('is_json'):
+        elif ctx.zato.request.is_json:
             data = json.dumps(ctx.zato.request.data_impl, indent=2)
             ctx.zato.request.headers['Content-Type'] = 'application/json'
-        elif ctx.zato.request.get('is_raw'):
+        elif ctx.zato.request.is_raw:
             data = ctx.zato.request.data_impl
-        elif ctx.zato.request.get('is_form'):
+        elif ctx.zato.request.is_form:
             data = ctx.zato.request.get('form', '')
             files = ctx.zato.request.get('files', None)
             ctx.zato.request.headers['Content-Type'] = 'application/x-www-form-urlencoded'
-
             if files is not None:
                 # multipart/formdata should let requests set the content-type header
                 del ctx.zato.request.headers['Content-Type']
-        else:
-            # Default to JSON
-            data = json.dumps(ctx.zato.request.data_impl, indent=2)
-            ctx.zato.request.headers['Content-Type'] = 'application/json'
 
     ctx.zato.request.method = method
     ctx.zato.request.data = data
     ctx.zato.full_address = '{}{}{}'.format(address, url_path, qs)
 
     auth = None
 
@@ -232,15 +227,16 @@
     ctx.zato.request.data = data
 
     if ctx.zato.request.get('is_json'):
         ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
     elif ctx.zato.request.get('is_raw'):
         ctx.zato.request.data_impl = ctx.zato.request.data
     else:
-        ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
+        if not ctx.zato.request.format:
+            raise ValueError('Format not set, cannot proceed')
 
 # ################################################################################################################################
 
 @given('request "{request_path}"')
 @util.obtain_values
 def given_request(ctx:'Context', request_path:'str') -> 'None':
     return given_request_impl(ctx, util.get_data(ctx, 'request', request_path))
@@ -496,15 +492,15 @@
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 @then('I store "{path}" from response under "{name}", default "{default}"')
 @util.obtain_values
 def then_store_path_under_name_with_default(ctx:'Context', path:'str', name:'str', default:'str') -> 'None':
-    if ctx.zato.request.get('is_xml'):
+    if ctx.zato.request.is_xml:
         value = ctx.zato.response.data_impl.xpath(path)
         if value:
             if len(value) == 1:
                 value = value[0].text
             else:
                 value = [elem.text for elem in value]
         else:
```

### Comparing `zato_apitest-24.1.10/src/zato/apitest/steps/json.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/json.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/typing_.py` & `zato-apitest-24.1.9/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato/apitest/util.py` & `zato-apitest-24.1.9/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.10/src/zato_apitest.egg-info/PKG-INFO` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.10
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.10 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.10/src/zato_apitest.egg-info/SOURCES.txt` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

