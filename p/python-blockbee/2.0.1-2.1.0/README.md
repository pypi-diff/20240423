# Comparing `tmp/python-blockbee-2.0.1.tar.gz` & `tmp/python-blockbee-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-blockbee-2.0.1.tar", last modified: Fri Apr 19 08:40:49 2024, max compression
+gzip compressed data, was "python-blockbee-2.1.0.tar", last modified: Tue Apr 23 11:49:10 2024, max compression
```

## Comparing `python-blockbee-2.0.1.tar` & `python-blockbee-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.082203 python-blockbee-2.0.1/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-13 17:33:47.000000 python-blockbee-2.0.1/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)    25166 2024-04-19 08:40:49.082034 python-blockbee-2.0.1/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)    24510 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/README.md
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.080728 python-blockbee-2.0.1/blockbee/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     8787 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/blockbee/BlockBee.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3244 2024-03-18 10:36:06.000000 python-blockbee-2.0.1/blockbee/BlockBeeCheckout.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       89 2024-03-14 16:00:34.000000 python-blockbee-2.0.1/blockbee/__init__.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.081806 python-blockbee-2.0.1/python_blockbee.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)    25166 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)      329 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-13 17:38:51.000000 python-blockbee-2.0.1/python_blockbee.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2024-04-19 08:40:49.082254 python-blockbee-2.0.1/setup.cfg
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1026 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 11:49:10.113911 python-blockbee-2.1.0/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-13 17:33:47.000000 python-blockbee-2.1.0/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    25495 2024-04-23 11:49:10.113761 python-blockbee-2.1.0/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    24839 2024-04-23 11:47:37.000000 python-blockbee-2.1.0/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 11:49:10.112538 python-blockbee-2.1.0/blockbee/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     5377 2024-04-23 11:47:37.000000 python-blockbee-2.1.0/blockbee/BlockBee.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1873 2024-04-23 11:45:26.000000 python-blockbee-2.1.0/blockbee/BlockBeeCheckout.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1883 2024-04-23 10:56:26.000000 python-blockbee-2.1.0/blockbee/BlockBeeRequests.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      136 2024-04-23 08:46:47.000000 python-blockbee-2.1.0/blockbee/__init__.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-23 11:49:10.113409 python-blockbee-2.1.0/python_blockbee.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    25495 2024-04-23 11:49:10.000000 python-blockbee-2.1.0/python_blockbee.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      358 2024-04-23 11:49:10.000000 python-blockbee-2.1.0/python_blockbee.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2024-04-23 11:49:10.000000 python-blockbee-2.1.0/python_blockbee.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-13 17:38:51.000000 python-blockbee-2.1.0/python_blockbee.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-23 11:49:10.000000 python-blockbee-2.1.0/python_blockbee.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-23 11:49:10.000000 python-blockbee-2.1.0/python_blockbee.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2024-04-23 11:49:10.113969 python-blockbee-2.1.0/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1026 2024-04-23 08:46:47.000000 python-blockbee-2.1.0/setup.py
```

### Comparing `python-blockbee-2.0.1/LICENSE` & `python-blockbee-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-blockbee-2.0.1/PKG-INFO` & `python-blockbee-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python Library for BlockBee payment gateway
 Home-page: https://github.com/blockbee-io/python-blockbee
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -124,15 +124,14 @@
 ```
 For object creation, same parameters as before. You must first call ``getAddress` as this method requires the payment address to have been created.
 
 #### Where:
 
 * ``value`` is the value requested to the user in the coin to which the request was done. **Optional**, can be empty if you don't wish to add the value to the QR Code.
 * ``size`` Size of the QR Code image in pixels. Optional, leave empty to use the default size of 512.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with `qr_code` (base64 encoded image data) and `payment_uri` (the value encoded in the QR), see https://docs.blockbee.io/#operation/qrcode for more information.
 
 #### Response sample:
 ```json
 {
   "status": "success",
@@ -147,22 +146,21 @@
 ```
 
 ### Estimating transaction fees
 
 ```python
 from blockbee import BlockBeeHelper
 
-fees = BlockBeeHelper.get_estimate(coin, addresses, priority, api_key)
+fees = BlockBeeHelper.get_estimate(coin, addresses, priority)
 ```
 
 #### Where: 
 * ``coin`` is the coin you wish to check, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``addresses`` The number of addresses to forward the funds to. Optional, defaults to 1.
 * ``priority`` Confirmation priority, (check [this](https://support.blockbee.io/article/how-the-priority-parameter-works) article to learn more about it). Optional, defaults to ``default``.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``estimated_cost`` and ``estimated_cost_usd``, see https://docs.blockbee.io/#operation/estimate for more information.
 
 #### Response sample:
 
 ```json
 {
@@ -180,23 +178,22 @@
 ### Converting between coins and fiat
 
 ```python
 from blockbee import BlockBeeHelper
 
 bb = BlockBeeHelper(coin, own_address, callback_url, params, bb_params, api_key)
 
-conversion = bb.get_conversion(value, from_coin, api_key)
+conversion = bb.get_conversion(value, from_coin)
 ```
 
 #### Where:
 
 * ``coin`` the target currency to convert to, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``value`` value to convert in `from`.
 * ``from_coin`` currency to convert from, FIAT or crypto.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``value_coin`` and ``exchange_rate``, see https://docs.blockbee.io/#operation/convert for more information.
 
 #### Response sample:
 
 ```json
 { 
@@ -207,20 +204,17 @@
 ```
 
 ### Getting supported coins
 
 ```python
 from blockbee import BlockBeeHelper
 
-supportedCoins = BlockBeeHelper.get_supported_coins(api_key)
+supportedCoins = BlockBeeHelper.get_supported_coins()
 ```
 
-### Where: 
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
-
 > Response is an array with all supported coins.
 
 #### Response sample:
 
 ```json
 {
   "btc": {
@@ -397,24 +391,41 @@
 #### Response sample:
 
 If `process` is `false`.
 ```json
 {
   "status": "success",
   "request_ids": [
-    103227,
-    103228
+    "42d5245e-0a29-402a-9a7e-355e38f1d81d",
+    "080a546e-4045-4c73-870c-4d9ec08c9cab"
   ]
 }
 ```
 
 If `process` is `true`.
 ```json
 {
   "status": "success",
+  "payout_info": {
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
+    "status": "Pending Payment",
+    "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
+    "requests": {
+      "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.5",
+      "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.1"
+    },
+    "total_requested": "0.6",
+    "total_with_fee": "0.603",
+    "error": "None",
+    "blockchain_fee": 0,
+    "fee": "0.003",
+    "coin": "bep20_usdt",
+    "txid": "",
+    "timestamp": "23/04/2024 11:13:49"
+  },
   "queued": true
 }
 ```
 
 ### List Payouts / Payout Requests
 
 List all Payouts or Payout Requests in your account.
@@ -439,15 +450,15 @@
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payouts": [
     {
-      "id": 2460,
+      "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
       "status": "Done",
       "total_requested": "0.6",
       "total_with_fee": "0.606",
       "total_fiat": "",
       "fee": "0.006",
       "coin": "polygon_matic",
       "timestamp": "13/03/2024 17:48:39"
@@ -497,15 +508,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2461,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Created",
     "from": "",
     "requests": {
       "0xA8EbeD50f2e05fB4a25b2DdCdc651A7CA769B5CF": "0.300000000000000000",
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.200000000000000000"
     },
     "total_requested": "0.5",
@@ -560,15 +571,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2463,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Done",
     "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
     "requests": {
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.500000000000000000",
       "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.100000000000000000"
     },
     "total_requested": "0.6",
@@ -614,11 +625,15 @@
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
 #### 2.0.1
 * Minor bugfixes
 
+#### 2.1.0
+* Minor bugfixes
+* Improve error handling
+
 ### Breaking Changes
 
 #### 2.0.0
 * `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.1/README.md` & `python-blockbee-2.1.0/python_blockbee.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: python-blockbee
+Version: 2.1.0
+Summary: Python Library for BlockBee payment gateway
+Home-page: https://github.com/blockbee-io/python-blockbee
+Author: BlockBee
+Author-email: info@blockbee.io
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [<img src="https://blockbee.io/static/assets/images/blockbee_logo_nospaces.png" width="300"/>](image.png)
 
 # BlockBee's Python Library
 Python implementation of BlockBee's payment gateway
 
 ## Table of Contents
 1. [Requirements](#requirements)
@@ -105,15 +124,14 @@
 ```
 For object creation, same parameters as before. You must first call ``getAddress` as this method requires the payment address to have been created.
 
 #### Where:
 
 * ``value`` is the value requested to the user in the coin to which the request was done. **Optional**, can be empty if you don't wish to add the value to the QR Code.
 * ``size`` Size of the QR Code image in pixels. Optional, leave empty to use the default size of 512.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with `qr_code` (base64 encoded image data) and `payment_uri` (the value encoded in the QR), see https://docs.blockbee.io/#operation/qrcode for more information.
 
 #### Response sample:
 ```json
 {
   "status": "success",
@@ -128,22 +146,21 @@
 ```
 
 ### Estimating transaction fees
 
 ```python
 from blockbee import BlockBeeHelper
 
-fees = BlockBeeHelper.get_estimate(coin, addresses, priority, api_key)
+fees = BlockBeeHelper.get_estimate(coin, addresses, priority)
 ```
 
 #### Where: 
 * ``coin`` is the coin you wish to check, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``addresses`` The number of addresses to forward the funds to. Optional, defaults to 1.
 * ``priority`` Confirmation priority, (check [this](https://support.blockbee.io/article/how-the-priority-parameter-works) article to learn more about it). Optional, defaults to ``default``.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``estimated_cost`` and ``estimated_cost_usd``, see https://docs.blockbee.io/#operation/estimate for more information.
 
 #### Response sample:
 
 ```json
 {
@@ -161,23 +178,22 @@
 ### Converting between coins and fiat
 
 ```python
 from blockbee import BlockBeeHelper
 
 bb = BlockBeeHelper(coin, own_address, callback_url, params, bb_params, api_key)
 
-conversion = bb.get_conversion(value, from_coin, api_key)
+conversion = bb.get_conversion(value, from_coin)
 ```
 
 #### Where:
 
 * ``coin`` the target currency to convert to, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``value`` value to convert in `from`.
 * ``from_coin`` currency to convert from, FIAT or crypto.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``value_coin`` and ``exchange_rate``, see https://docs.blockbee.io/#operation/convert for more information.
 
 #### Response sample:
 
 ```json
 { 
@@ -188,20 +204,17 @@
 ```
 
 ### Getting supported coins
 
 ```python
 from blockbee import BlockBeeHelper
 
-supportedCoins = BlockBeeHelper.get_supported_coins(api_key)
+supportedCoins = BlockBeeHelper.get_supported_coins()
 ```
 
-### Where: 
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
-
 > Response is an array with all supported coins.
 
 #### Response sample:
 
 ```json
 {
   "btc": {
@@ -378,24 +391,41 @@
 #### Response sample:
 
 If `process` is `false`.
 ```json
 {
   "status": "success",
   "request_ids": [
-    103227,
-    103228
+    "42d5245e-0a29-402a-9a7e-355e38f1d81d",
+    "080a546e-4045-4c73-870c-4d9ec08c9cab"
   ]
 }
 ```
 
 If `process` is `true`.
 ```json
 {
   "status": "success",
+  "payout_info": {
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
+    "status": "Pending Payment",
+    "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
+    "requests": {
+      "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.5",
+      "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.1"
+    },
+    "total_requested": "0.6",
+    "total_with_fee": "0.603",
+    "error": "None",
+    "blockchain_fee": 0,
+    "fee": "0.003",
+    "coin": "bep20_usdt",
+    "txid": "",
+    "timestamp": "23/04/2024 11:13:49"
+  },
   "queued": true
 }
 ```
 
 ### List Payouts / Payout Requests
 
 List all Payouts or Payout Requests in your account.
@@ -420,15 +450,15 @@
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payouts": [
     {
-      "id": 2460,
+      "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
       "status": "Done",
       "total_requested": "0.6",
       "total_with_fee": "0.606",
       "total_fiat": "",
       "fee": "0.006",
       "coin": "polygon_matic",
       "timestamp": "13/03/2024 17:48:39"
@@ -478,15 +508,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2461,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Created",
     "from": "",
     "requests": {
       "0xA8EbeD50f2e05fB4a25b2DdCdc651A7CA769B5CF": "0.300000000000000000",
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.200000000000000000"
     },
     "total_requested": "0.5",
@@ -541,15 +571,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2463,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Done",
     "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
     "requests": {
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.500000000000000000",
       "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.100000000000000000"
     },
     "total_requested": "0.6",
@@ -595,11 +625,15 @@
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
 #### 2.0.1
 * Minor bugfixes
 
+#### 2.1.0
+* Minor bugfixes
+* Improve error handling
+
 ### Breaking Changes
 
 #### 2.0.0
-* `create_payout` parameters were changed and will require you to update your code.
+* `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.1/python_blockbee.egg-info/PKG-INFO` & `python-blockbee-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: python-blockbee
-Version: 2.0.1
-Summary: Python Library for BlockBee payment gateway
-Home-page: https://github.com/blockbee-io/python-blockbee
-Author: BlockBee
-Author-email: info@blockbee.io
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [<img src="https://blockbee.io/static/assets/images/blockbee_logo_nospaces.png" width="300"/>](image.png)
 
 # BlockBee's Python Library
 Python implementation of BlockBee's payment gateway
 
 ## Table of Contents
 1. [Requirements](#requirements)
@@ -124,15 +105,14 @@
 ```
 For object creation, same parameters as before. You must first call ``getAddress` as this method requires the payment address to have been created.
 
 #### Where:
 
 * ``value`` is the value requested to the user in the coin to which the request was done. **Optional**, can be empty if you don't wish to add the value to the QR Code.
 * ``size`` Size of the QR Code image in pixels. Optional, leave empty to use the default size of 512.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with `qr_code` (base64 encoded image data) and `payment_uri` (the value encoded in the QR), see https://docs.blockbee.io/#operation/qrcode for more information.
 
 #### Response sample:
 ```json
 {
   "status": "success",
@@ -147,22 +127,21 @@
 ```
 
 ### Estimating transaction fees
 
 ```python
 from blockbee import BlockBeeHelper
 
-fees = BlockBeeHelper.get_estimate(coin, addresses, priority, api_key)
+fees = BlockBeeHelper.get_estimate(coin, addresses, priority)
 ```
 
 #### Where: 
 * ``coin`` is the coin you wish to check, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``addresses`` The number of addresses to forward the funds to. Optional, defaults to 1.
 * ``priority`` Confirmation priority, (check [this](https://support.blockbee.io/article/how-the-priority-parameter-works) article to learn more about it). Optional, defaults to ``default``.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``estimated_cost`` and ``estimated_cost_usd``, see https://docs.blockbee.io/#operation/estimate for more information.
 
 #### Response sample:
 
 ```json
 {
@@ -180,23 +159,22 @@
 ### Converting between coins and fiat
 
 ```python
 from blockbee import BlockBeeHelper
 
 bb = BlockBeeHelper(coin, own_address, callback_url, params, bb_params, api_key)
 
-conversion = bb.get_conversion(value, from_coin, api_key)
+conversion = bb.get_conversion(value, from_coin)
 ```
 
 #### Where:
 
 * ``coin`` the target currency to convert to, from BlockBee's supported currencies (e.g 'btc', 'eth', 'erc20_usdt', ...)
 * ``value`` value to convert in `from`.
 * ``from_coin`` currency to convert from, FIAT or crypto.
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
 
 > Response is an object with ``value_coin`` and ``exchange_rate``, see https://docs.blockbee.io/#operation/convert for more information.
 
 #### Response sample:
 
 ```json
 { 
@@ -207,20 +185,17 @@
 ```
 
 ### Getting supported coins
 
 ```python
 from blockbee import BlockBeeHelper
 
-supportedCoins = BlockBeeHelper.get_supported_coins(api_key)
+supportedCoins = BlockBeeHelper.get_supported_coins()
 ```
 
-### Where: 
-* ``api_key`` is the API Key provided by BlockBee's [dashboard](https://dash.blockbee.io/).
-
 > Response is an array with all supported coins.
 
 #### Response sample:
 
 ```json
 {
   "btc": {
@@ -397,24 +372,41 @@
 #### Response sample:
 
 If `process` is `false`.
 ```json
 {
   "status": "success",
   "request_ids": [
-    103227,
-    103228
+    "42d5245e-0a29-402a-9a7e-355e38f1d81d",
+    "080a546e-4045-4c73-870c-4d9ec08c9cab"
   ]
 }
 ```
 
 If `process` is `true`.
 ```json
 {
   "status": "success",
+  "payout_info": {
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
+    "status": "Pending Payment",
+    "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
+    "requests": {
+      "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.5",
+      "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.1"
+    },
+    "total_requested": "0.6",
+    "total_with_fee": "0.603",
+    "error": "None",
+    "blockchain_fee": 0,
+    "fee": "0.003",
+    "coin": "bep20_usdt",
+    "txid": "",
+    "timestamp": "23/04/2024 11:13:49"
+  },
   "queued": true
 }
 ```
 
 ### List Payouts / Payout Requests
 
 List all Payouts or Payout Requests in your account.
@@ -439,15 +431,15 @@
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payouts": [
     {
-      "id": 2460,
+      "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
       "status": "Done",
       "total_requested": "0.6",
       "total_with_fee": "0.606",
       "total_fiat": "",
       "fee": "0.006",
       "coin": "polygon_matic",
       "timestamp": "13/03/2024 17:48:39"
@@ -497,15 +489,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2461,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Created",
     "from": "",
     "requests": {
       "0xA8EbeD50f2e05fB4a25b2DdCdc651A7CA769B5CF": "0.300000000000000000",
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.200000000000000000"
     },
     "total_requested": "0.5",
@@ -560,15 +552,15 @@
 
 #### Response sample:
 
 ```json
 {
   "status": "success",
   "payout_info": {
-    "id": 2463,
+    "id": "88e5eacc-d5a5-4b8a-8133-e23136151b7c",
     "status": "Done",
     "from": "0x18B211A1Ba5880C7d62C250B6441C2400d588589",
     "requests": {
       "0xA6B78B56ee062185E405a1DDDD18cE8fcBC4395d": "0.500000000000000000",
       "0x18B211A1Ba5880C7d62C250B6441C2400d588589": "0.100000000000000000"
     },
     "total_requested": "0.6",
@@ -614,11 +606,15 @@
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
 #### 2.0.1
 * Minor bugfixes
 
+#### 2.1.0
+* Minor bugfixes
+* Improve error handling
+
 ### Breaking Changes
 
 #### 2.0.0
-* `create_payout` parameters were changed and will require you to update your code.
+* `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.1/setup.py` & `python-blockbee-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 
     name='python-blockbee',
 
-    version='2.0.1',
+    version='2.1.0',
 
     packages=find_packages(),
 
     author="BlockBee",
 
     author_email="info@blockbee.io",
     install_requires=[
```

