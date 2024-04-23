# Comparing `tmp/python-cryptapi-1.0.4.tar.gz` & `tmp/python-cryptapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cryptapi-1.0.4.tar", last modified: Mon Dec  4 21:44:17 2023, max compression
+gzip compressed data, was "python-cryptapi-1.0.5.tar", last modified: Tue Apr 23 13:08:24 2024, max compression
```

## Comparing `python-cryptapi-1.0.4.tar` & `python-cryptapi-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-12-04 21:44:17.636930 python-cryptapi-1.0.4/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     5211 2023-12-04 21:44:17.636573 python-cryptapi-1.0.4/PKG-INFO
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     4557 2023-12-04 21:37:01.000000 python-cryptapi-1.0.4/README.md
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-12-04 21:44:17.635170 python-cryptapi-1.0.4/cryptapi/
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     4084 2023-12-04 21:33:16.000000 python-cryptapi-1.0.4/cryptapi/CryptAPI.py
--rw-rw-r--   0 arianoangelo   (501) staff       (20)       37 2023-03-09 13:07:40.000000 python-cryptapi-1.0.4/cryptapi/__init__.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-12-04 21:44:17.636190 python-cryptapi-1.0.4/python_cryptapi.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     5211 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)      292 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-12-04 21:44:17.000000 python-cryptapi-1.0.4/python_cryptapi.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-12-04 21:44:17.637042 python-cryptapi-1.0.4/setup.cfg
--rw-rw-r--   0 arianoangelo   (501) staff       (20)     1023 2023-12-04 21:35:18.000000 python-cryptapi-1.0.4/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 13:08:24.525665 python-cryptapi-1.0.5/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     5263 2024-04-23 13:08:24.525455 python-cryptapi-1.0.5/PKG-INFO
+-rw-rw-r--   0 arianoangelo   (501) staff       (20)     4609 2024-04-23 13:01:52.000000 python-cryptapi-1.0.5/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 13:08:24.523968 python-cryptapi-1.0.5/cryptapi/
+-rw-rw-r--   0 arianoangelo   (501) staff       (20)     3973 2024-04-23 13:01:31.000000 python-cryptapi-1.0.5/cryptapi/CryptAPI.py
+-rw-rw-r--   0 arianoangelo   (501) staff       (20)       37 2023-03-09 13:07:40.000000 python-cryptapi-1.0.5/cryptapi/__init__.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 13:08:24.525178 python-cryptapi-1.0.5/python_cryptapi.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     5263 2024-04-23 13:08:24.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      292 2024-04-23 13:08:24.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2024-04-23 13:08:24.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-12-04 21:44:17.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-23 13:08:24.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-23 13:08:24.000000 python-cryptapi-1.0.5/python_cryptapi.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2024-04-23 13:08:24.525716 python-cryptapi-1.0.5/setup.cfg
+-rw-rw-r--   0 arianoangelo   (501) staff       (20)     1023 2024-04-23 12:53:59.000000 python-cryptapi-1.0.5/setup.py
```

### Comparing `python-cryptapi-1.0.4/PKG-INFO` & `python-cryptapi-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cryptapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Library for CryptAPI payment gateway
 Home-page: https://github.com/cryptapi/python-cryptapi
 Author: CryptAPI
 Author-email: info@cryptapi.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 ### Generating a new Address
 
 ```python
 from cryptapi import CryptAPIHelper
 
 ca = CryptAPIHelper(coin, myAddress, callbackUrl, params, cryptapiParams)
 
-address = ca.getAddress()['address_in']
+address = ca.get_address()['address_in']
 ```
 
 Where:
 
 * `coin` is the coin you wish to use, from CryptAPI's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...).
 * `myAddress` is your own crypto address, where your funds will be sent to.
 * `callbackUrl` is the URL that will be called upon payment.
@@ -161,7 +161,11 @@
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 
 #### 1.0.4
 * Minor fixes
+
+#### 1.0.5
+* Minor fixes
+* Improve error handling
```

### Comparing `python-cryptapi-1.0.4/README.md` & `python-cryptapi-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ### Generating a new Address
 
 ```python
 from cryptapi import CryptAPIHelper
 
 ca = CryptAPIHelper(coin, myAddress, callbackUrl, params, cryptapiParams)
 
-address = ca.getAddress()['address_in']
+address = ca.get_address()['address_in']
 ```
 
 Where:
 
 * `coin` is the coin you wish to use, from CryptAPI's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...).
 * `myAddress` is your own crypto address, where your funds will be sent to.
 * `callbackUrl` is the URL that will be called upon payment.
@@ -142,7 +142,11 @@
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 
 #### 1.0.4
 * Minor fixes
+
+#### 1.0.5
+* Minor fixes
+* Improve error handling
```

### Comparing `python-cryptapi-1.0.4/cryptapi/CryptAPI.py` & `python-cryptapi-1.0.5/cryptapi/CryptAPI.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 """
 CryptAPI's Python Helper
 """
 
 import requests
 from requests.models import PreparedRequest
 
+
+class CryptAPIException(Exception):
+    pass
+
+
 class CryptAPIHelper:
     CRYPTAPI_URL = 'https://api.cryptapi.io/'
     CRYPTAPI_HOST = 'api.cryptapi.io'
 
     def __init__(self, coin, own_address, callback_url, parameters=None, ca_params=None):
-        if parameters is None:
+        if not parameters:
             parameters = {}
 
-        if ca_params is None:
+        if not ca_params:
             ca_params = {}
 
+        if not callback_url:
+            raise Exception("Callback URL is Missing")
+
+        if not coin:
+            raise Exception('Coin is Missing')
+
+        if not own_address:
+            raise Exception('Address is Missing')
+
         self.coin = coin
         self.own_address = own_address
         self.callback_url = callback_url
         self.parameters = parameters
         self.ca_params = ca_params
         self.payment_Address = ''
 
     def get_address(self):
-        if self.coin is None or self.own_address is None:
-            return None
-
         coin = self.coin
 
         if self.parameters:
             req = PreparedRequest()
             req.prepare_url(self.callback_url, self.parameters)
             self.callback_url = req.url
 
@@ -46,73 +57,47 @@
 
         return None
 
     def get_logs(self):
         coin = self.coin
         callback_url = self.callback_url
 
-        if coin is None or callback_url is None:
-            return None
-
         if self.parameters:
             req = PreparedRequest()
             req.prepare_url(self.callback_url, self.parameters)
             self.callback_url = req.url
 
         params = {
             'callback': callback_url
         }
 
-        _logs = CryptAPIHelper.process_request(coin, endpoint='logs', params=params)
-
-        if _logs:
-            return _logs
-
-        return None
+        return CryptAPIHelper.process_request(coin, endpoint='logs', params=params)
 
     def get_qrcode(self, value='', size=300):
-        if self.coin is None:
-            return None
-
         params = {
             'address': self.payment_Address,
             'size': size
         }
 
         if value:
             params['value'] = value
 
-        _qrcode = CryptAPIHelper.process_request(self.coin, endpoint='qrcode', params=params)
-
-        if _qrcode:
-            return _qrcode
-
-        return None
+        return CryptAPIHelper.process_request(self.coin, endpoint='qrcode', params=params)
 
     def get_conversion(self, from_coin, value):
         params = {
             'from': from_coin,
             'value': value
         }
 
-        _value = CryptAPIHelper.process_request(self.coin, endpoint='convert', params=params)
-
-        if _value:
-            return _value
-
-        return None
+        return CryptAPIHelper.process_request(self.coin, endpoint='convert', params=params)
 
     @staticmethod
     def get_info(coin=''):
-        _info = CryptAPIHelper.process_request(coin, endpoint='info')
-
-        if _info:
-            return _info
-
-        return None
+        return CryptAPIHelper.process_request(coin, endpoint='info')
 
     @staticmethod
     def get_supported_coins():
         _info = CryptAPIHelper.get_info('')
 
         _info.pop('fee_tiers', None)
 
@@ -131,30 +116,32 @@
     @staticmethod
     def get_estimate(coin, addresses=1, priority='default'):
         params = {
             'addresses': addresses,
             'priority': priority
         }
 
-        _estimate = CryptAPIHelper.process_request(coin, endpoint='estimate', params=params)
-
-        if _estimate:
-            return _estimate
-
-        return None
+        return CryptAPIHelper.process_request(coin, endpoint='estimate', params=params)
 
     @staticmethod
-    def process_request(coin='', endpoint='', params=None):
-        if coin != '':
+    def process_request(coin=None, endpoint='', params=None):
+        if coin:
             coin += '/'
+        else:
+            coin = ''
 
         response = requests.get(
             url="{base_url}{coin}{endpoint}/".format(
                 base_url=CryptAPIHelper.CRYPTAPI_URL,
                 coin=coin.replace('_', '/'),
                 endpoint=endpoint,
             ),
             params=params,
             headers={'Host': CryptAPIHelper.CRYPTAPI_HOST},
         )
 
-        return response.json()
+        response_obj = response.json()
+
+        if response_obj.get('status') == 'error':
+            raise CryptAPIException(response_obj['error'])
+
+        return response_obj
```

### Comparing `python-cryptapi-1.0.4/python_cryptapi.egg-info/PKG-INFO` & `python-cryptapi-1.0.5/python_cryptapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cryptapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Library for CryptAPI payment gateway
 Home-page: https://github.com/cryptapi/python-cryptapi
 Author: CryptAPI
 Author-email: info@cryptapi.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 ### Generating a new Address
 
 ```python
 from cryptapi import CryptAPIHelper
 
 ca = CryptAPIHelper(coin, myAddress, callbackUrl, params, cryptapiParams)
 
-address = ca.getAddress()['address_in']
+address = ca.get_address()['address_in']
 ```
 
 Where:
 
 * `coin` is the coin you wish to use, from CryptAPI's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...).
 * `myAddress` is your own crypto address, where your funds will be sent to.
 * `callbackUrl` is the URL that will be called upon payment.
@@ -161,7 +161,11 @@
 * Minor fixes
 
 #### 1.0.3
 * Minor fixes
 
 #### 1.0.4
 * Minor fixes
+
+#### 1.0.5
+* Minor fixes
+* Improve error handling
```

### Comparing `python-cryptapi-1.0.4/setup.py` & `python-cryptapi-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 
     name='python-cryptapi',
 
-    version='1.0.4',
+    version='1.0.5',
 
     packages=find_packages(),
 
     author="CryptAPI",
 
     author_email="info@cryptapi.io",
     install_requires=[
```

