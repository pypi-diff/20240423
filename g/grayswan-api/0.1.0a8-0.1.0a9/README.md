# Comparing `tmp/grayswan_api-0.1.0a8.tar.gz` & `tmp/grayswan_api-0.1.0a9.tar.gz`

## Comparing `grayswan_api-0.1.0a8.tar` & `grayswan_api-0.1.0a9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/__init__.py
--rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_base_client.py
--rw-r--r--   0        0        0    15272 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_compat.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_constants.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_files.py
--rw-r--r--   0        0        0    26100 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_qs.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_resource.py
--rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_response.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_streaming.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_types.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/resources/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/chat.py
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/completion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/types/__init__.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/completion_create_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/src/grayswan/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/__init__.py
+-rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_base_client.py
+-rw-r--r--   0        0        0    15272 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_compat.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_constants.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_files.py
+-rw-r--r--   0        0        0    26100 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_qs.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_resource.py
+-rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_response.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_streaming.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_types.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/resources/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/chat.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/completion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/types/__init__.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/completion_create_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/src/grayswan/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a9/PKG-INFO
```

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/__init__.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_base_client.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_base_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_client.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_compat.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_compat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_exceptions.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_exceptions.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_files.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_files.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_models.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_models.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_qs.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_qs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_resource.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_resource.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_response.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_streaming.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_streaming.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_types.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_types.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/__init__.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_logs.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_proxy.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_sync.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_transform.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_typing.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/_utils/_utils.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/__init__.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/chat.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/resources/chat/completion.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/resources/chat/completion.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/__init__.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/completion_create_params.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/src/gray_swan_security/types/chat/completion_create_response.py` & `grayswan_api-0.1.0a9/src/gray_swan_security/types/chat/completion_create_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/LICENSE` & `grayswan_api-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a8/pyproject.toml` & `grayswan_api-0.1.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grayswan-api"
-version = "0.1.0-alpha.8"
+version = "0.1.0-alpha.9"
 description = "The official Python library for the Gray Swan Security API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Gray Swan Security", email = "dev-feedback@grayswan.ai" },
 ]
 dependencies = [
```

### Comparing `grayswan_api-0.1.0a8/PKG-INFO` & `grayswan_api-0.1.0a9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grayswan-api
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: The official Python library for the Gray Swan Security API
 Project-URL: Homepage, https://github.com/grayswansecurity/grayswan-python
 Project-URL: Repository, https://github.com/grayswansecurity/grayswan-python
 Author-email: Gray Swan Security <dev-feedback@grayswan.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -63,15 +63,15 @@
 
 client = GraySwanSecurity(
     # This is the default and can be omitted
     api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
 )
 
 completion_create_response = client.chat.completion.create(
-    messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+    messages=[{"role": "system"}, {"role": "user"}],
     model="cygnet-v0.2",
 )
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `GRAYSWAN_BEARER_TOKEN="My API Key"` to your `.env` file
@@ -90,15 +90,15 @@
     # This is the default and can be omitted
     api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
 )
 
 
 async def main() -> None:
     completion_create_response = await client.chat.completion.create(
-        messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+        messages=[{"role": "system"}, {"role": "user"}],
         model="cygnet-v0.2",
     )
 
 
 asyncio.run(main())
 ```
 
@@ -126,15 +126,15 @@
 import gray_swan_security
 from gray_swan_security import GraySwanSecurity
 
 client = GraySwanSecurity()
 
 try:
     client.chat.completion.create(
-        messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+        messages=[{"role": "system"}, {"role": "user"}],
         model="cygnet-v0.2",
     )
 except gray_swan_security.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except gray_swan_security.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
@@ -172,15 +172,15 @@
 client = GraySwanSecurity(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).chat.completion.create(
-    messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+    messages=[{"role": "system"}, {"role": "user"}],
     model="cygnet-v0.2",
 )
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
@@ -198,15 +198,15 @@
 # More granular control:
 client = GraySwanSecurity(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 client.with_options(timeout=5 * 1000).chat.completion.create(
-    messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+    messages=[{"role": "system"}, {"role": "user"}],
     model="cygnet-v0.2",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/grayswansecurity/grayswan-python/tree/main/#retries).
@@ -243,17 +243,15 @@
 from gray_swan_security import GraySwanSecurity
 
 client = GraySwanSecurity()
 response = client.chat.completion.with_raw_response.create(
     messages=[{
         "role": "system"
     }, {
-        "role": "system"
-    }, {
-        "role": "system"
+        "role": "user"
     }],
     model="cygnet-v0.2",
 )
 print(response.headers.get('X-My-Header'))
 
 completion = response.parse()  # get the object that `chat.completion.create()` would have returned
 print(completion)
@@ -267,15 +265,15 @@
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
 with client.chat.completion.with_streaming_response.create(
-    messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
+    messages=[{"role": "system"}, {"role": "user"}],
     model="cygnet-v0.2",
 ) as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
```

