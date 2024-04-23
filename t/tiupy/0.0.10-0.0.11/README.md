# Comparing `tmp/tiupy-0.0.10.tar.gz` & `tmp/tiupy-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiupy-0.0.10.tar", last modified: Mon Oct  9 19:58:16 2023, max compression
+gzip compressed data, was "tiupy-0.0.11.tar", last modified: Tue Apr 23 16:47:02 2024, max compression
```

## Comparing `tiupy-0.0.10.tar` & `tiupy-0.0.11.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-10-09 19:58:16.807072 tiupy-0.0.10/
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-10-09 19:42:01.000000 tiupy-0.0.10/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     3763 2023-10-09 19:58:16.807072 tiupy-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3232 2023-10-09 19:52:31.000000 tiupy-0.0.10/README.md
--rw-------   0 runner    (1000) runner    (1000)      544 2023-09-20 21:38:16.000000 tiupy-0.0.10/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-10-09 19:58:16.807072 tiupy-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      844 2023-10-09 19:57:17.000000 tiupy-0.0.10/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-10-09 19:58:16.803072 tiupy-0.0.10/tiupy/
--rw-------   0 runner    (1000) runner    (1000)       20 2023-10-09 19:40:15.000000 tiupy-0.0.10/tiupy/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2262 2023-10-09 19:40:15.000000 tiupy-0.0.10/tiupy/tiu.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-10-09 19:58:16.807072 tiupy-0.0.10/tiupy/utils/
--rw-------   0 runner    (1000) runner    (1000)       46 2023-10-09 19:40:15.000000 tiupy-0.0.10/tiupy/utils/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      648 2023-10-09 19:40:15.000000 tiupy-0.0.10/tiupy/utils/headers.py
--rw-------   0 runner    (1000) runner    (1000)     2795 2023-10-09 19:40:15.000000 tiupy-0.0.10/tiupy/utils/objects.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-10-09 19:58:16.807072 tiupy-0.0.10/tiupy.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3763 2023-10-09 19:58:16.000000 tiupy-0.0.10/tiupy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-10-09 19:58:16.000000 tiupy-0.0.10/tiupy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-10-09 19:58:16.000000 tiupy-0.0.10/tiupy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2023-10-09 19:58:16.000000 tiupy-0.0.10/tiupy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-23 16:47:02.004342 tiupy-0.0.11/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2024-04-23 16:43:42.000000 tiupy-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     3739 2024-04-23 16:47:02.000342 tiupy-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3208 2024-04-23 16:43:42.000000 tiupy-0.0.11/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-23 16:47:02.004342 tiupy-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      844 2024-04-23 16:43:42.000000 tiupy-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-23 16:47:01.928334 tiupy-0.0.11/tiupy/
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-23 16:43:42.000000 tiupy-0.0.11/tiupy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2015 2024-04-23 16:43:42.000000 tiupy-0.0.11/tiupy/tiu.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-23 16:47:01.996341 tiupy-0.0.11/tiupy/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-23 16:43:42.000000 tiupy-0.0.11/tiupy/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-23 16:43:42.000000 tiupy-0.0.11/tiupy/utils/headers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2795 2024-04-23 16:43:42.000000 tiupy-0.0.11/tiupy/utils/objects.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-23 16:47:01.996341 tiupy-0.0.11/tiupy.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3739 2024-04-23 16:47:01.000000 tiupy-0.0.11/tiupy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      243 2024-04-23 16:47:01.000000 tiupy-0.0.11/tiupy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-23 16:47:01.000000 tiupy-0.0.11/tiupy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-23 16:47:01.000000 tiupy-0.0.11/tiupy.egg-info/top_level.txt
```

### Comparing `tiupy-0.0.10/LICENSE` & `tiupy-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `tiupy-0.0.10/PKG-INFO` & `tiupy-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiupy
-Version: 0.0.10
+Version: 0.0.11
 Summary: A web scraper for TIU student system
 Home-page: https://github.com/heromr/tiupy
 Author: HeroMR
 License: MIT
 Keywords: tiu uni,tishk university,tiu scraper,tiu API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,30 +63,30 @@
   <p>
     The Tiu module provides the following methods for interaction:
   </p>
 
   <h3 style="color: #0d47a1;" align="center">`login(username: str, password: str)`</h3>
   <p>Login to the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.login(username='your_username', password='your_password')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.login(username='your_username', password='your_password')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`sid_login(SID: str)`</h3>
   <p>Login using a session ID (SID).</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.sid_login(SID='your_session_id')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.sid_login(SID='your_session_id')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`logout()`</h3>
   <p>Log out from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.logout()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.logout()</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`get_courses_data()`</h3>
   <p>Fetch course data from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = await tiu.get_courses_data()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = tiu.get_courses_data()</code></pre>
 </div>
 
 <div align="center">
   <h2>License</h2>
 
   <p>
     This module is open-source and available under the MIT License. See the <a href="https://github.com/heromr/tiupy/blob/main/LICENSE">LICENSE</a> file for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiupy Version: 0.0.10 Summary: A web scraper for
+Metadata-Version: 2.1 Name: tiupy Version: 0.0.11 Summary: A web scraper for
 TIU student system Home-page: https://github.com/heromr/tiupy Author: HeroMR
 License: MIT Keywords: tiu uni,tishk university,tiu scraper,tiu API Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
                               ************ ttiiuuppyy ************
@@ -25,20 +25,20 @@
 tiu = Tiu()
 You can customize the initialization by providing optional parameters like
 proxies and request timeout.
                               ********** MMeetthhooddss **********
 The Tiu module provides the following methods for interaction:
                 ******** ``llooggiinn((uusseerrnnaammee:: ssttrr,, ppaasssswwoorrdd:: ssttrr))`` ********
 Login to the TIU website.
-await tiu.login(username='your_username', password='your_password')
+tiu.login(username='your_username', password='your_password')
                         ******** ``ssiidd__llooggiinn((SSIIDD:: ssttrr))`` ********
 Login using a session ID (SID).
-await tiu.sid_login(SID='your_session_id')
+tiu.sid_login(SID='your_session_id')
                              ******** ``llooggoouutt(())`` ********
 Log out from the TIU website.
-await tiu.logout()
+tiu.logout()
                         ******** ``ggeett__ccoouurrsseess__ddaattaa(())`` ********
 Fetch course data from the TIU website.
-courses_data = await tiu.get_courses_data()
+courses_data = tiu.get_courses_data()
                               ********** LLiicceennssee **********
 This module is open-source and available under the MIT License. See the _L_I_C_E_N_S_E
                             file for more details.
```

### Comparing `tiupy-0.0.10/README.md` & `tiupy-0.0.11/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,30 +47,30 @@
   <p>
     The Tiu module provides the following methods for interaction:
   </p>
 
   <h3 style="color: #0d47a1;" align="center">`login(username: str, password: str)`</h3>
   <p>Login to the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.login(username='your_username', password='your_password')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.login(username='your_username', password='your_password')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`sid_login(SID: str)`</h3>
   <p>Login using a session ID (SID).</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.sid_login(SID='your_session_id')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.sid_login(SID='your_session_id')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`logout()`</h3>
   <p>Log out from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.logout()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.logout()</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`get_courses_data()`</h3>
   <p>Fetch course data from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = await tiu.get_courses_data()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = tiu.get_courses_data()</code></pre>
 </div>
 
 <div align="center">
   <h2>License</h2>
 
   <p>
     This module is open-source and available under the MIT License. See the <a href="https://github.com/heromr/tiupy/blob/main/LICENSE">LICENSE</a> file for more details.
```

#### html2text {}

```diff
@@ -18,20 +18,20 @@
 tiu = Tiu()
 You can customize the initialization by providing optional parameters like
 proxies and request timeout.
                               ********** MMeetthhooddss **********
 The Tiu module provides the following methods for interaction:
                 ******** ``llooggiinn((uusseerrnnaammee:: ssttrr,, ppaasssswwoorrdd:: ssttrr))`` ********
 Login to the TIU website.
-await tiu.login(username='your_username', password='your_password')
+tiu.login(username='your_username', password='your_password')
                         ******** ``ssiidd__llooggiinn((SSIIDD:: ssttrr))`` ********
 Login using a session ID (SID).
-await tiu.sid_login(SID='your_session_id')
+tiu.sid_login(SID='your_session_id')
                              ******** ``llooggoouutt(())`` ********
 Log out from the TIU website.
-await tiu.logout()
+tiu.logout()
                         ******** ``ggeett__ccoouurrsseess__ddaattaa(())`` ********
 Fetch course data from the TIU website.
-courses_data = await tiu.get_courses_data()
+courses_data = tiu.get_courses_data()
                               ********** LLiicceennssee **********
 This module is open-source and available under the MIT License. See the _L_I_C_E_N_S_E
                             file for more details.
```

### Comparing `tiupy-0.0.10/setup.py` & `tiupy-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
   long_description = f.read()
 
-VERSION = "0.0.10"
+VERSION = "0.0.11"
 DESCRIPTION = "A web scraper for TIU student system"
 
 setup(
     name="tiupy",
     version=VERSION,
     description=DESCRIPTION,
     author="HeroMR",
```

### Comparing `tiupy-0.0.10/tiupy/tiu.py` & `tiupy-0.0.11/tiupy/tiu.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,53 @@
-from httpx import AsyncClient
+from httpx import Client
 from typing import Optional, Any, Dict
 from .utils import headers, objects
 
 
 class Tiu:
     def __init__(self, proxies: Optional[dict] = None, request_timeout: Optional[int] = 60):
         self.base_url = "https://my.tiu.edu.iq"
         self.proxies = proxies
 
         self.sid = None
         self.request_timeout = request_timeout
         self.profile = objects.UserProfile(None)
 
-    async def __aenter__(self):
-        self.client = AsyncClient(proxies=self.proxies, timeout=self.request_timeout)
-        return self
-
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.client.aclose()
-    
-    async def make_request(self, method: str, endpoint: str, data: Optional[Dict[str, Any]] = None, params: Optional[Dict[str, Any]] = None):
+    def make_request(self, method: str, endpoint: str, data: Optional[Dict[str, Any]] = None, params: Optional[Dict[str, Any]] = None):
         url = self.base_url + endpoint
-        response = await self.client.request(method, url, headers=headers.Headers().headers, data=data, params=params)
-        response.raise_for_status()
-        return response
+        with Client(proxies=self.proxies, timeout=self.request_timeout) as client:
+            response = client.request(method, url, headers=headers.Headers().headers, data=data, params=params)
+            response.raise_for_status()
+            return response
     
-    async def _get_profile_info(self):
-        response = await self.make_request("GET", endpoint="/pages/home.php")
+    def _get_profile_info(self):
+        response = self.make_request("GET", endpoint="/pages/home.php")
         return response.text
     
-    async def login(self, username: str, password: str):
+    def login(self, username: str, password: str):
         data = {
             'username': username,
             'password': password,
-            'login.x': '0',  #Need to change?
-            'login.y': '0'   #Need to change?
+            'login.x': '0',  # Need to change?
+            'login.y': '0'   # Need to change?
         }
 
-        response = await self.make_request("POST", endpoint="/", data=data)
+        response = self.make_request("POST", endpoint="/", data=data)
 
         self.sid = response.cookies.get("PHPSESSID")
         headers.sid = self.sid
-        self.profile = objects.UserProfile(await self._get_profile_info())
+        self.profile = objects.UserProfile(self._get_profile_info())
         return response.status_code
     
-    async def sid_login(self, SID: str):
+    def sid_login(self, SID: str):
         self.sid = SID
         headers.sid = self.sid
-        self.profile = objects.UserProfile(await self._get_profile_info())
+        self.profile = objects.UserProfile(self._get_profile_info())
         return
     
-    async def logout(self):
-        response = await self.make_request("GET", endpoint="/pages/p999.php/")
+    def logout(self):
+        response = self.make_request("GET", endpoint="/pages/p999.php/")
         return response.status_code
     
-    async def get_courses_data(self):
-        response = await self.make_request("GET", endpoint="/pages/p103.php")
+    def get_courses_data(self):
+        response = self.make_request("GET", endpoint="/pages/p103.php")
         return objects.CourseData(response.text)
-
-
```

### Comparing `tiupy-0.0.10/tiupy/utils/headers.py` & `tiupy-0.0.11/tiupy/utils/headers.py`

 * *Files identical despite different names*

### Comparing `tiupy-0.0.10/tiupy/utils/objects.py` & `tiupy-0.0.11/tiupy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `tiupy-0.0.10/tiupy.egg-info/PKG-INFO` & `tiupy-0.0.11/tiupy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiupy
-Version: 0.0.10
+Version: 0.0.11
 Summary: A web scraper for TIU student system
 Home-page: https://github.com/heromr/tiupy
 Author: HeroMR
 License: MIT
 Keywords: tiu uni,tishk university,tiu scraper,tiu API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,30 +63,30 @@
   <p>
     The Tiu module provides the following methods for interaction:
   </p>
 
   <h3 style="color: #0d47a1;" align="center">`login(username: str, password: str)`</h3>
   <p>Login to the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.login(username='your_username', password='your_password')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.login(username='your_username', password='your_password')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`sid_login(SID: str)`</h3>
   <p>Login using a session ID (SID).</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.sid_login(SID='your_session_id')</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.sid_login(SID='your_session_id')</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`logout()`</h3>
   <p>Log out from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">await tiu.logout()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">tiu.logout()</code></pre>
 
   <h3 style="color: #0d47a1;" align="center">`get_courses_data()`</h3>
   <p>Fetch course data from the TIU website.</p>
 
-  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = await tiu.get_courses_data()</code></pre>
+  <pre style="background-color: #f5f5f5; padding: 10px;"><code style="color: #f44336;">courses_data = tiu.get_courses_data()</code></pre>
 </div>
 
 <div align="center">
   <h2>License</h2>
 
   <p>
     This module is open-source and available under the MIT License. See the <a href="https://github.com/heromr/tiupy/blob/main/LICENSE">LICENSE</a> file for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiupy Version: 0.0.10 Summary: A web scraper for
+Metadata-Version: 2.1 Name: tiupy Version: 0.0.11 Summary: A web scraper for
 TIU student system Home-page: https://github.com/heromr/tiupy Author: HeroMR
 License: MIT Keywords: tiu uni,tishk university,tiu scraper,tiu API Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
                               ************ ttiiuuppyy ************
@@ -25,20 +25,20 @@
 tiu = Tiu()
 You can customize the initialization by providing optional parameters like
 proxies and request timeout.
                               ********** MMeetthhooddss **********
 The Tiu module provides the following methods for interaction:
                 ******** ``llooggiinn((uusseerrnnaammee:: ssttrr,, ppaasssswwoorrdd:: ssttrr))`` ********
 Login to the TIU website.
-await tiu.login(username='your_username', password='your_password')
+tiu.login(username='your_username', password='your_password')
                         ******** ``ssiidd__llooggiinn((SSIIDD:: ssttrr))`` ********
 Login using a session ID (SID).
-await tiu.sid_login(SID='your_session_id')
+tiu.sid_login(SID='your_session_id')
                              ******** ``llooggoouutt(())`` ********
 Log out from the TIU website.
-await tiu.logout()
+tiu.logout()
                         ******** ``ggeett__ccoouurrsseess__ddaattaa(())`` ********
 Fetch course data from the TIU website.
-courses_data = await tiu.get_courses_data()
+courses_data = tiu.get_courses_data()
                               ********** LLiicceennssee **********
 This module is open-source and available under the MIT License. See the _L_I_C_E_N_S_E
                             file for more details.
```

