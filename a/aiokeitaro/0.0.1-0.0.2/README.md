# Comparing `tmp/aiokeitaro-0.0.1.tar.gz` & `tmp/aiokeitaro-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokeitaro-0.0.1.tar", last modified: Tue Apr 23 10:07:23 2024, max compression
+gzip compressed data, was "aiokeitaro-0.0.2.tar", last modified: Tue Apr 23 10:35:28 2024, max compression
```

## Comparing `aiokeitaro-0.0.1.tar` & `aiokeitaro-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:07:23.195196 aiokeitaro-0.0.1/
--rw-rw-rw-   0        0        0     1068 2024-04-23 09:54:45.000000 aiokeitaro-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4081 2024-04-23 10:07:23.194191 aiokeitaro-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2024-04-23 10:06:35.000000 aiokeitaro-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 10:07:23.070864 aiokeitaro-0.0.1/aiokeitaro/
--rw-rw-rw-   0        0        0       74 2021-07-29 12:14:22.000000 aiokeitaro-0.0.1/aiokeitaro/__init__.py
--rw-rw-rw-   0        0        0     1774 2024-04-23 09:27:06.000000 aiokeitaro-0.0.1/aiokeitaro/api.py
--rw-rw-rw-   0        0        0     1315 2024-04-23 09:26:00.000000 aiokeitaro-0.0.1/aiokeitaro/keitaro.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:07:23.190167 aiokeitaro-0.0.1/aiokeitaro/resources/
--rw-rw-rw-   0        0        0      420 2021-07-29 12:14:22.000000 aiokeitaro-0.0.1/aiokeitaro/resources/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-04-23 09:56:37.000000 aiokeitaro-0.0.1/aiokeitaro/resources/affiliate_networks.py
--rw-rw-rw-   0        0        0      900 2024-04-23 09:56:38.000000 aiokeitaro-0.0.1/aiokeitaro/resources/botlist.py
--rw-rw-rw-   0        0        0     3278 2024-04-23 09:56:38.000000 aiokeitaro-0.0.1/aiokeitaro/resources/campaigns.py
--rw-rw-rw-   0        0        0      511 2024-04-23 09:56:39.000000 aiokeitaro-0.0.1/aiokeitaro/resources/clicks.py
--rw-rw-rw-   0        0        0     1517 2024-04-23 09:56:40.000000 aiokeitaro-0.0.1/aiokeitaro/resources/domains.py
--rw-rw-rw-   0        0        0      821 2024-04-23 09:56:41.000000 aiokeitaro-0.0.1/aiokeitaro/resources/groups.py
--rw-rw-rw-   0        0        0     2183 2024-04-23 09:56:41.000000 aiokeitaro-0.0.1/aiokeitaro/resources/integrations.py
--rw-rw-rw-   0        0        0     1635 2024-04-23 09:56:43.000000 aiokeitaro-0.0.1/aiokeitaro/resources/landing_pages.py
--rw-rw-rw-   0        0        0      491 2024-04-23 09:56:44.000000 aiokeitaro-0.0.1/aiokeitaro/resources/logs.py
--rw-rw-rw-   0        0        0     1745 2024-04-23 09:56:45.000000 aiokeitaro-0.0.1/aiokeitaro/resources/offers.py
--rw-rw-rw-   0        0        0     1155 2024-04-23 09:56:45.000000 aiokeitaro-0.0.1/aiokeitaro/resources/reports.py
--rw-rw-rw-   0        0        0     3056 2024-04-23 09:56:46.000000 aiokeitaro-0.0.1/aiokeitaro/resources/streams.py
--rw-rw-rw-   0        0        0      943 2024-04-23 09:56:47.000000 aiokeitaro-0.0.1/aiokeitaro/resources/traffic_sources.py
--rw-rw-rw-   0        0        0      636 2024-04-23 09:56:49.000000 aiokeitaro-0.0.1/aiokeitaro/resources/users.py
--rw-rw-rw-   0        0        0     1876 2024-04-23 09:25:56.000000 aiokeitaro-0.0.1/aiokeitaro/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:07:23.192179 aiokeitaro-0.0.1/aiokeitaro.egg-info/
--rw-rw-rw-   0        0        0     4081 2024-04-23 10:07:22.000000 aiokeitaro-0.0.1/aiokeitaro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2024-04-23 10:07:22.000000 aiokeitaro-0.0.1/aiokeitaro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:07:22.000000 aiokeitaro-0.0.1/aiokeitaro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 10:07:22.000000 aiokeitaro-0.0.1/aiokeitaro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 10:07:22.000000 aiokeitaro-0.0.1/aiokeitaro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2024-04-23 09:54:30.000000 aiokeitaro-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 10:07:23.196188 aiokeitaro-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1168 2024-04-23 09:51:31.000000 aiokeitaro-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:35:28.571517 aiokeitaro-0.0.2/
+-rw-rw-rw-   0        0        0     1068 2024-04-23 09:54:45.000000 aiokeitaro-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4322 2024-04-23 10:35:28.569943 aiokeitaro-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3508 2024-04-23 10:32:12.000000 aiokeitaro-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 10:35:28.508746 aiokeitaro-0.0.2/aiokeitaro/
+-rw-rw-rw-   0        0        0       74 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-23 10:28:21.000000 aiokeitaro-0.0.2/aiokeitaro/api.py
+-rw-rw-rw-   0        0        0     1417 2024-04-23 10:29:31.000000 aiokeitaro-0.0.2/aiokeitaro/keitaro.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:35:28.566382 aiokeitaro-0.0.2/aiokeitaro/resources/
+-rw-rw-rw-   0        0        0      420 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/affiliate_networks.py
+-rw-rw-rw-   0        0        0      900 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/botlist.py
+-rw-rw-rw-   0        0        0     3278 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/campaigns.py
+-rw-rw-rw-   0        0        0      511 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/clicks.py
+-rw-rw-rw-   0        0        0     1517 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/domains.py
+-rw-rw-rw-   0        0        0      821 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/groups.py
+-rw-rw-rw-   0        0        0     2183 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/integrations.py
+-rw-rw-rw-   0        0        0     1635 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/landing_pages.py
+-rw-rw-rw-   0        0        0      491 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/logs.py
+-rw-rw-rw-   0        0        0     1745 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/offers.py
+-rw-rw-rw-   0        0        0     1155 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/reports.py
+-rw-rw-rw-   0        0        0     3056 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/streams.py
+-rw-rw-rw-   0        0        0      943 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/traffic_sources.py
+-rw-rw-rw-   0        0        0      636 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/resources/users.py
+-rw-rw-rw-   0        0        0     1876 2024-04-23 10:11:25.000000 aiokeitaro-0.0.2/aiokeitaro/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:35:28.568378 aiokeitaro-0.0.2/aiokeitaro.egg-info/
+-rw-rw-rw-   0        0        0     4322 2024-04-23 10:35:28.000000 aiokeitaro-0.0.2/aiokeitaro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2024-04-23 10:35:28.000000 aiokeitaro-0.0.2/aiokeitaro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:35:28.000000 aiokeitaro-0.0.2/aiokeitaro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 10:35:28.000000 aiokeitaro-0.0.2/aiokeitaro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 10:35:28.000000 aiokeitaro-0.0.2/aiokeitaro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2024-04-23 10:32:29.000000 aiokeitaro-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:35:28.572052 aiokeitaro-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2024-04-23 10:32:21.000000 aiokeitaro-0.0.2/setup.py
```

### Comparing `aiokeitaro-0.0.1/LICENSE` & `aiokeitaro-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/PKG-INFO` & `aiokeitaro-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: aiokeitaro
-Version: 0.0.1
-Summary: Unofficial Asynchronous Keitaro Admin API client
-Home-page: https://github.com/developerreva/aiokeitaro
-Author: Developereva
-Author-email: developereva@protonmail.com
-Project-URL: Source Code, https://github.com/developerreva/aiokeitaro
-Project-URL: Documentation, https://github.com/ysomad/keitaro#-getting-started
-Project-URL: Keitaro Admin API Documentation, https://admin-api.docs.keitaro.io/
-Keywords: python python3 api-client aiohttp api-wrapper keitaro keitaro-tracker
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-
 # keitaro
 
 keitaro is a simple and easy to use API wrapper library for [Keitaro](https://keitaro.io/) Admin API written in Python3 and [aiohttp](https://pypi.org/project/aiohttp/)
 
 ## 📄 Official Keitaro resources
 
 -   [Keitaro Website](https://keitaro.io/)
@@ -36,31 +17,42 @@
 ### Keitaro tracker initialization
 
 Begin by importing Keitaro class from aiokeitaro module and passing Admin API key and URL of Keitaro tracker to it
 
 ```python
 from aiokeitaro import Keitaro
 
-api = Keitaro('API key', 'URL')
+api = Keitaro('API KEY', 'URL with http or https (if is domain)')
 ```
 
 ## ⚙ What can it do
 
 All aiokeitaro functionality is presented in [Google Sheet](https://docs.google.com/spreadsheets/d/1XqRT8XuUG3XfI8GnJMfEKezJmI_3_MllDNermPeUCqA/edit#gid=0)
 
 ## 📚 Examples
 
 If API request was successful, status code 200 will be received and a response in the json format.
 
 ```python
-from aiokeitaro import Keitaro
+import asyncio
+from aiokeitaro import Keitaro, Offer
+
+async def main():
+    api = Keitaro('API KEY', 'URL with http or https (if is domain)')
+    
+    # Create an instance of the Offer class
+    offer = Offer(api)
+    
+    # Call the get method on the instance
+    ss = await offer.get()
+    print(ss)
+
+# run main.py
+asyncio.run(main())
 
-api = Keitaro('API key', 'URL')
-affnetwork = await api.affnetworks.delete(14)
-print(affnetwork)
 ```
 
 <details>
   <summary>
     <i>Click to see a response sample</i>
     <a href="https://admin-api.docs.keitaro.io/#tag/Affiliate-Networks/paths/~1affiliate_networks~1{id}/delete">
     Admin API reference</a>
@@ -83,21 +75,21 @@
 </details>
 
 ### Get all offers or specific one
 
 To get all offers call get() method without any arguments
 
 ```python
-all_offers = await api.offers.get()
+all_offers = await offer.get()
 ```
 
 Let's try to get a specific offer by its id
 
 ```python
-dummy_offer = await api.offers.get(21)
+dummy_offer = await offer.get(21)
 ```
 
 As a result you'll get a response in JSON format
 
 <details>
   <summary>
     <i>Click to see a response sample</i>
@@ -141,11 +133,11 @@
   'state': 'disabled',
   'cost_type': 'CPC',
   'cost_value': '5',
   'cost_currency': 'USD',
   'cost_auto': True
 }
 
-campaign = await api.campaigns.create(payload)
+campaign = await campaigns.create(payload)
 ```
 
 The non-asynchronous module is located here: https://github.com/ysomad/keitaro
```

#### html2text {}

```diff
@@ -1,49 +1,40 @@
-Metadata-Version: 2.1 Name: aiokeitaro Version: 0.0.1 Summary: Unofficial
-Asynchronous Keitaro Admin API client Home-page: https://github.com/
-developerreva/aiokeitaro Author: Developereva Author-email:
-developereva@protonmail.com Project-URL: Source Code, https://github.com/
-developerreva/aiokeitaro Project-URL: Documentation, https://github.com/ysomad/
-keitaro#-getting-started Project-URL: Keitaro Admin API Documentation, https://
-admin-api.docs.keitaro.io/ Keywords: python python3 api-client aiohttp api-
-wrapper keitaro keitaro-tracker Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: aiohttp # keitaro keitaro is a
-simple and easy to use API wrapper library for [Keitaro](https://keitaro.io/
-) Admin API written in Python3 and [aiohttp](https://pypi.org/project/aiohttp/
-) ## ð Official Keitaro resources - [Keitaro Website](https://keitaro.io/) -
-[Admin API documentation](https://admin-api.docs.keitaro.io/) - [Technical
-Support](https://t.me/keitarobot) ## ð Getting Started ### Installation Pypi
-package is not updated, you can build it using setup.py ### Keitaro tracker
-initialization Begin by importing Keitaro class from aiokeitaro module and
-passing Admin API key and URL of Keitaro tracker to it ```python from
-aiokeitaro import Keitaro api = Keitaro('API key', 'URL') ``` ## â What can
-it do All aiokeitaro functionality is presented in [Google Sheet](https://
+# keitaro keitaro is a simple and easy to use API wrapper library for [Keitaro]
+(https://keitaro.io/) Admin API written in Python3 and [aiohttp](https://
+pypi.org/project/aiohttp/) ## ð Official Keitaro resources - [Keitaro
+Website](https://keitaro.io/) - [Admin API documentation](https://admin-
+api.docs.keitaro.io/) - [Technical Support](https://t.me/keitarobot) ## ð
+Getting Started ### Installation Pypi package is not updated, you can build it
+using setup.py ### Keitaro tracker initialization Begin by importing Keitaro
+class from aiokeitaro module and passing Admin API key and URL of Keitaro
+tracker to it ```python from aiokeitaro import Keitaro api = Keitaro('API KEY',
+'URL with http or https (if is domain)') ``` ## â What can it do All
+aiokeitaro functionality is presented in [Google Sheet](https://
 docs.google.com/spreadsheets/d/1XqRT8XuUG3XfI8GnJMfEKezJmI_3_MllDNermPeUCqA/
 edit#gid=0) ## ð Examples If API request was successful, status code 200
-will be received and a response in the json format. ```python from aiokeitaro
-import Keitaro api = Keitaro('API key', 'URL') affnetwork = await
-api.affnetworks.delete(14) print(affnetwork) ``` Click to see a response sample
-_A_d_m_i_n_ _A_P_I_ _r_e_f_e_r_e_n_c_e
+will be received and a response in the json format. ```python import asyncio
+from aiokeitaro import Keitaro, Offer async def main(): api = Keitaro('API
+KEY', 'URL with http or https (if is domain)') # Create an instance of the
+Offer class offer = Offer(api) # Call the get method on the instance ss = await
+offer.get() print(ss) # run main.py asyncio.run(main()) ``` Click to see a
+response sample _A_d_m_i_n_ _A_P_I_ _r_e_f_e_r_e_n_c_e
 { "id": 14, "name": "string", "postback_url": "string", "offer_param":
 "string", "state": "string", "template_name": "string", "notes": "string",
 "pull_api_options": "string", "created_at": "string", "updated_at": "string",
 "offers": "string" }
 ### Get all offers or specific one To get all offers call get() method without
-any arguments ```python all_offers = await api.offers.get() ``` Let's try to
-get a specific offer by its id ```python dummy_offer = await api.offers.get(21)
-``` As a result you'll get a response in JSON format Click to see a response
-sample
+any arguments ```python all_offers = await offer.get() ``` Let's try to get a
+specific offer by its id ```python dummy_offer = await offer.get(21) ``` As a
+result you'll get a response in JSON format Click to see a response sample
 [ { "id": 21, "name": "string", "group_id": 0, "action_type": "string",
 "action_payload": "string", "action_options": [], "affiliate_network_id": 0,
 "payout_value": 0, "payout_currency": "string", "payout_type": "string",
 "state": "string", "created_at": {}, "updated_at": {}, "payout_auto": true,
 "payout_upsell": true, "country": [], "notes": "string", "affiliate_network":
 "string", "archive": "string", "local_path": "string", "preview_path": "string"
 } ]
 ### Campaign creation To create an advertising campaign, you can simply call
 create() method of the campaigns resource ```python payload = { 'name': 'Dummy
 campaign', 'state': 'disabled', 'cost_type': 'CPC', 'cost_value': '5',
-'cost_currency': 'USD', 'cost_auto': True } campaign = await
-api.campaigns.create(payload) ``` The non-asynchronous module is located here:
-https://github.com/ysomad/keitaro
+'cost_currency': 'USD', 'cost_auto': True } campaign = await campaigns.create
+(payload) ``` The non-asynchronous module is located here: https://github.com/
+ysomad/keitaro
```

### Comparing `aiokeitaro-0.0.1/aiokeitaro/api.py` & `aiokeitaro-0.0.2/aiokeitaro/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
         Preparing http request for api call: building endpoint and payload
         """
         endpoint = API.build_url(self.resource_path, *path_params)
         payload = self._build_payload(query_params)
         
         response = await self.client.send_request(
-            method, endpoint, data=json.dumps(payload))
+            method, endpoint)
         
         return response
 
     async def get(self, *path_params, **query_params):
         return await self.prepare_request('GET', *path_params, **query_params)
 
     async def post(self, *path_params, **query_params):
```

### Comparing `aiokeitaro-0.0.1/aiokeitaro/keitaro.py` & `aiokeitaro-0.0.2/aiokeitaro/keitaro.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import aiohttp
 
 from .utils import build_host_url
 from .api import API
+from .resources import Affiliate, Campaign
 
 class Keitaro:
     api_endpoint = 'admin_api/v1/'
 
     def __init__(self, api_key: str, host: str, from_env: bool = False) -> None:
         if from_env:
             self.api_key = os.environ[api_key]
@@ -32,16 +33,18 @@
         self._host = build_host_url(host)
 
     async def send_request(self, method: str, endpoint: str, *kwargs):
         """
         Sends HTTP request to Keitaro Admin API
         """
         print(f'{method} {endpoint}')
-        print(f'payload: {kwargs.get("data")}')
+        kwargs_dict = dict(kwargs)
+        print(f'payload: {kwargs_dict.get("data")}')
         url = API.build_url(self.host, Keitaro.api_endpoint, endpoint)
+        print(url)
 
         async with aiohttp.ClientSession() as session:
             async with session.request(
                 method, url, headers={'Api-Key': self.api_key}, *kwargs
             ) as response:
                 data = await response.json()
                 print(f'response: {data}')
```

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/affiliate_networks.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/affiliate_networks.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/botlist.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/botlist.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/campaigns.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/campaigns.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/domains.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/domains.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/groups.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/groups.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/integrations.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/integrations.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/landing_pages.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/landing_pages.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/offers.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/offers.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/reports.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/reports.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/streams.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/streams.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/traffic_sources.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/traffic_sources.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/resources/users.py` & `aiokeitaro-0.0.2/aiokeitaro/resources/users.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro/utils.py` & `aiokeitaro-0.0.2/aiokeitaro/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/aiokeitaro.egg-info/PKG-INFO` & `aiokeitaro-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokeitaro
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial Asynchronous Keitaro Admin API client
 Home-page: https://github.com/developerreva/aiokeitaro
 Author: Developereva
 Author-email: developereva@protonmail.com
 Project-URL: Source Code, https://github.com/developerreva/aiokeitaro
 Project-URL: Documentation, https://github.com/ysomad/keitaro#-getting-started
 Project-URL: Keitaro Admin API Documentation, https://admin-api.docs.keitaro.io/
@@ -36,31 +36,42 @@
 ### Keitaro tracker initialization
 
 Begin by importing Keitaro class from aiokeitaro module and passing Admin API key and URL of Keitaro tracker to it
 
 ```python
 from aiokeitaro import Keitaro
 
-api = Keitaro('API key', 'URL')
+api = Keitaro('API KEY', 'URL with http or https (if is domain)')
 ```
 
 ## ⚙ What can it do
 
 All aiokeitaro functionality is presented in [Google Sheet](https://docs.google.com/spreadsheets/d/1XqRT8XuUG3XfI8GnJMfEKezJmI_3_MllDNermPeUCqA/edit#gid=0)
 
 ## 📚 Examples
 
 If API request was successful, status code 200 will be received and a response in the json format.
 
 ```python
-from aiokeitaro import Keitaro
+import asyncio
+from aiokeitaro import Keitaro, Offer
+
+async def main():
+    api = Keitaro('API KEY', 'URL with http or https (if is domain)')
+    
+    # Create an instance of the Offer class
+    offer = Offer(api)
+    
+    # Call the get method on the instance
+    ss = await offer.get()
+    print(ss)
+
+# run main.py
+asyncio.run(main())
 
-api = Keitaro('API key', 'URL')
-affnetwork = await api.affnetworks.delete(14)
-print(affnetwork)
 ```
 
 <details>
   <summary>
     <i>Click to see a response sample</i>
     <a href="https://admin-api.docs.keitaro.io/#tag/Affiliate-Networks/paths/~1affiliate_networks~1{id}/delete">
     Admin API reference</a>
@@ -83,21 +94,21 @@
 </details>
 
 ### Get all offers or specific one
 
 To get all offers call get() method without any arguments
 
 ```python
-all_offers = await api.offers.get()
+all_offers = await offer.get()
 ```
 
 Let's try to get a specific offer by its id
 
 ```python
-dummy_offer = await api.offers.get(21)
+dummy_offer = await offer.get(21)
 ```
 
 As a result you'll get a response in JSON format
 
 <details>
   <summary>
     <i>Click to see a response sample</i>
@@ -141,11 +152,11 @@
   'state': 'disabled',
   'cost_type': 'CPC',
   'cost_value': '5',
   'cost_currency': 'USD',
   'cost_auto': True
 }
 
-campaign = await api.campaigns.create(payload)
+campaign = await campaigns.create(payload)
 ```
 
 The non-asynchronous module is located here: https://github.com/ysomad/keitaro
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiokeitaro Version: 0.0.1 Summary: Unofficial
+Metadata-Version: 2.1 Name: aiokeitaro Version: 0.0.2 Summary: Unofficial
 Asynchronous Keitaro Admin API client Home-page: https://github.com/
 developerreva/aiokeitaro Author: Developereva Author-email:
 developereva@protonmail.com Project-URL: Source Code, https://github.com/
 developerreva/aiokeitaro Project-URL: Documentation, https://github.com/ysomad/
 keitaro#-getting-started Project-URL: Keitaro Admin API Documentation, https://
 admin-api.docs.keitaro.io/ Keywords: python python3 api-client aiohttp api-
 wrapper keitaro keitaro-tracker Classifier: Programming Language :: Python :: 3
@@ -13,37 +13,38 @@
 ) Admin API written in Python3 and [aiohttp](https://pypi.org/project/aiohttp/
 ) ## ð Official Keitaro resources - [Keitaro Website](https://keitaro.io/) -
 [Admin API documentation](https://admin-api.docs.keitaro.io/) - [Technical
 Support](https://t.me/keitarobot) ## ð Getting Started ### Installation Pypi
 package is not updated, you can build it using setup.py ### Keitaro tracker
 initialization Begin by importing Keitaro class from aiokeitaro module and
 passing Admin API key and URL of Keitaro tracker to it ```python from
-aiokeitaro import Keitaro api = Keitaro('API key', 'URL') ``` ## â What can
-it do All aiokeitaro functionality is presented in [Google Sheet](https://
-docs.google.com/spreadsheets/d/1XqRT8XuUG3XfI8GnJMfEKezJmI_3_MllDNermPeUCqA/
-edit#gid=0) ## ð Examples If API request was successful, status code 200
-will be received and a response in the json format. ```python from aiokeitaro
-import Keitaro api = Keitaro('API key', 'URL') affnetwork = await
-api.affnetworks.delete(14) print(affnetwork) ``` Click to see a response sample
-_A_d_m_i_n_ _A_P_I_ _r_e_f_e_r_e_n_c_e
+aiokeitaro import Keitaro api = Keitaro('API KEY', 'URL with http or https (if
+is domain)') ``` ## â What can it do All aiokeitaro functionality is
+presented in [Google Sheet](https://docs.google.com/spreadsheets/d/
+1XqRT8XuUG3XfI8GnJMfEKezJmI_3_MllDNermPeUCqA/edit#gid=0) ## ð Examples If
+API request was successful, status code 200 will be received and a response in
+the json format. ```python import asyncio from aiokeitaro import Keitaro, Offer
+async def main(): api = Keitaro('API KEY', 'URL with http or https (if is
+domain)') # Create an instance of the Offer class offer = Offer(api) # Call the
+get method on the instance ss = await offer.get() print(ss) # run main.py
+asyncio.run(main()) ``` Click to see a response sample _A_d_m_i_n_ _A_P_I_ _r_e_f_e_r_e_n_c_e
 { "id": 14, "name": "string", "postback_url": "string", "offer_param":
 "string", "state": "string", "template_name": "string", "notes": "string",
 "pull_api_options": "string", "created_at": "string", "updated_at": "string",
 "offers": "string" }
 ### Get all offers or specific one To get all offers call get() method without
-any arguments ```python all_offers = await api.offers.get() ``` Let's try to
-get a specific offer by its id ```python dummy_offer = await api.offers.get(21)
-``` As a result you'll get a response in JSON format Click to see a response
-sample
+any arguments ```python all_offers = await offer.get() ``` Let's try to get a
+specific offer by its id ```python dummy_offer = await offer.get(21) ``` As a
+result you'll get a response in JSON format Click to see a response sample
 [ { "id": 21, "name": "string", "group_id": 0, "action_type": "string",
 "action_payload": "string", "action_options": [], "affiliate_network_id": 0,
 "payout_value": 0, "payout_currency": "string", "payout_type": "string",
 "state": "string", "created_at": {}, "updated_at": {}, "payout_auto": true,
 "payout_upsell": true, "country": [], "notes": "string", "affiliate_network":
 "string", "archive": "string", "local_path": "string", "preview_path": "string"
 } ]
 ### Campaign creation To create an advertising campaign, you can simply call
 create() method of the campaigns resource ```python payload = { 'name': 'Dummy
 campaign', 'state': 'disabled', 'cost_type': 'CPC', 'cost_value': '5',
-'cost_currency': 'USD', 'cost_auto': True } campaign = await
-api.campaigns.create(payload) ``` The non-asynchronous module is located here:
-https://github.com/ysomad/keitaro
+'cost_currency': 'USD', 'cost_auto': True } campaign = await campaigns.create
+(payload) ``` The non-asynchronous module is located here: https://github.com/
+ysomad/keitaro
```

### Comparing `aiokeitaro-0.0.1/aiokeitaro.egg-info/SOURCES.txt` & `aiokeitaro-0.0.2/aiokeitaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiokeitaro-0.0.1/setup.py` & `aiokeitaro-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name='aiokeitaro',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(exclude=['tests']),
     install_requires=['aiohttp'],
     package_data={
         '': ['*.py']
     },
     author='Developereva',
     author_email='developereva@protonmail.com',
```

