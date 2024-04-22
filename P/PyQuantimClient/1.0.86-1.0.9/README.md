# Comparing `tmp/pyquantimclient-1.0.86.tar.gz` & `tmp/PyQuantimClient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquantimclient-1.0.86.tar", last modified: Mon Apr 22 22:14:22 2024, max compression
+gzip compressed data, was "PyQuantimClient-1.0.9.tar", last modified: Mon Dec 19 20:05:36 2022, max compression
```

## Comparing `pyquantimclient-1.0.86.tar` & `PyQuantimClient-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:22.574053 pyquantimclient-1.0.86/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 22:14:22.574053 pyquantimclient-1.0.86/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:22.574053 pyquantimclient-1.0.86/PyQuantimClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 22:14:22.000000 pyquantimclient-1.0.86/PyQuantimClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 22:14:22.000000 pyquantimclient-1.0.86/PyQuantimClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:14:22.000000 pyquantimclient-1.0.86/PyQuantimClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 22:14:22.000000 pyquantimclient-1.0.86/PyQuantimClient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:14:22.574053 pyquantimclient-1.0.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:22.574053 pyquantimclient-1.0.86/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/bi.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (127)    19944 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/preprocess_co.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/risk.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 22:14:13.000000 pyquantimclient-1.0.86/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/preprocess_co.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/risk.py
```

### Comparing `pyquantimclient-1.0.86/src/api.py` & `PyQuantimClient-1.0.9/src/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,52 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import requests, json
 
 class quantim:
-    def __init__(self, username, password, secretpool, env="pdn", api_url=None):
+    def __init__(self, username, password, secretpool, env="qa"):
         self.username = username
         self.password = password
         self.secretpool = secretpool
         self.env = env
 
-        if api_url is None:
-            self.api_url = "https://api-quantimqa.sura-im.com/" if env=="qa" else "https://api-quantim.sura-im.com/"
-        else:
-            self.api_url = api_url
-
-    def get_token(self):
+    def get_header(self):
         if self.secretpool=='ALM':
-            token_url = f"{self.api_url}token"
+            token_url = "https://api-quantimqa.sura-im.com/oauthback/token" if self.env=="qa" else "https://api-quantim.sura-im.com/oauthback/token"
             data = {"username":self.username, "password":self.password}
         else:
-            token_url = f"{self.api_url}tokendynamicpool"
+            token_url = "https://api-quantimqa.sura-im.com/tokendynamicpool" if self.env=="qa" else "https://api-quantim.sura-im.com/tokendynamicpool"
             data = {"username":self.username, "password":self.password, "secretpool":self.secretpool}
 
         headers = {"Accept": "*/*",'Content-Type': 'application/json', 'Access-Control-Allow-Origin': '*'}
         access_token_response = requests.post(token_url, data=json.dumps(data), headers=headers, verify=False, allow_redirects=False)
         tokens = json.loads(access_token_response.text)
         access_token = tokens['id_token']
-
-        return access_token
-
-    def get_header(self):
-        '''
-        Build request header
-        '''
-        access_token = self.get_token()
         api_call_headers = {"Accept": "*/*", 'Authorization': 'Bearer ' + access_token, 'Content-Type': 'application/json', 'Access-Control-Allow-Origin': '*'}
 
         return api_call_headers
 
     def api_call(self, endpoint, method="post", data=None, verify=False):
         '''
         data: when method get, data is an array of key values.
         '''
         api_call_headers = self.get_header()
-        api_url = f"{self.api_url}{endpoint}"
         if method.lower()=='post':
+            api_url = f"{'https://api-quantimqa.sura-im.com/' if self.env=='qa' else 'https://api-quantim.sura-im.com/'}{endpoint}"
             api_call_response = requests.post(api_url, headers=api_call_headers, data=json.dumps(data), verify=verify)
         elif method.lower()=='get':
+            api_url = f"{'https://api-quantimqa.sura-im.com/' if self.env=='qa' else 'https://api-quantim.sura-im.com/'}{endpoint}"
             if data is not None:
                 api_url = api_url + '?'+'&'.join([f"{x['key']}={x['value']}" for x in data])
             api_call_response = requests.get(api_url, headers=api_call_headers, data=None, verify=verify)
         else:
             print("Method not supported!")
             return None
-        
-        try:
-            resp = json.loads(api_call_response.text)
-        except:
-            resp = api_call_response.text
-        return resp
+        return json.loads(api_call_response.text)
 
     def retrieve_s3_df(self, bucket, key, sep=','):
         '''
         Get series
         '''
         data = {'bucket':bucket, 'key':key, 'sep':sep}
         resp = self.api_call('retrieve_data_s3', method="post", data=data, verify=False)
@@ -77,31 +60,7 @@
         payload = df.to_dict(orient='records')
         data = {'bucket':bucket, 'file_name':key, 'payload':payload, 'sep':sep, 'overwrite':overwrite}
         try:
             resp = self.api_call('load_data_s3', method="post", data=data, verify=False)
         except:
             resp = {'success':False, 'message':'Check permissions!'}
         return resp
-
-    def upload_with_presigned_url(self, local_file_path, bucket, key):
-        """
-        Upload a local file to S3 using a presigned URL.
-        """
-        data = {'bucket':bucket, 'key':key}
-        try:
-            presigned_url = self.api_call('link_data_s3', method="post", data=data, verify=False)
-        except Exception as e:
-            print(f"Error with presigned url: {e}")
-            return False
-
-        with open(local_file_path, 'rb') as file:
-            try:
-                response = requests.put(presigned_url, data=file, verify=False)
-                if response.status_code == 200:
-                    print("File uploaded successfully")
-                    return True
-                else:
-                    print(f"Error uploading file. Status code: {response.status_code}")
-                    return False
-            except Exception as e:
-                print(f"Error uploading file: {e}")
-                return False
```

### Comparing `pyquantimclient-1.0.86/src/benchmarks.py` & `PyQuantimClient-1.0.9/src/benchmarks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import datetime as dt
 from .api import quantim
 
 class benchmarks(quantim):
-    def __init__(self, username, password, secretpool, env="pdn", api_url=None):
-        super().__init__(username, password, secretpool, env, api_url)
+    def __init__(self, username, password, secretpool, env="qa"):
+        super().__init__(username, password, secretpool, env)
 
     def load_constraints(self, file_name, sep=',', country='CO'):
         '''
         Load portfolio file to s3.
         '''
         if ~np.all(np.in1d(country, ['CO', 'CL', 'PE', 'MX', 'UY'])):
             raise ValueError('Country not supported.')
```

### Comparing `pyquantimclient-1.0.86/src/data.py` & `PyQuantimClient-1.0.9/src/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import datetime as dt
 from .api import quantim
 
 class time_series(quantim):
-    def __init__(self, username, password, secretpool, env="pdn", api_url=None):
-        super().__init__(username, password, secretpool, env, api_url)
+    def __init__(self, username, password, secretpool, env="qa"):
+        super().__init__(username, password, secretpool, env)
 
-    def get_series(self, tks, ref_curr='Origen', join='outer', verify=False):
+    def get_series(self, tks, ref_curr='Origen', join='outer'):
         '''
         Get series
         '''
         data = {'tks':list(tks), 'ref_curr':ref_curr, 'join':join}
-        resp = self.api_call('get_series', method="post", data=data, verify=verify)
-        ts, summ, tks_invalid = pd.DataFrame(resp['ts']).set_index("Date"), pd.DataFrame(resp['summ']), resp['tks_invalid']
-        return ts, summ, tks_invalid
+        resp = self.api_call('get_series', method="post", data=data, verify=False)
+        ref_curr, ts, summ = resp['ref_curr'], pd.DataFrame(resp['ts']).set_index("Date"), pd.DataFrame(resp['summ'])
+        return ref_curr, ts, summ
```

### Comparing `pyquantimclient-1.0.86/src/energy.py` & `PyQuantimClient-1.0.9/src/energy.py`

 * *Files identical despite different names*

