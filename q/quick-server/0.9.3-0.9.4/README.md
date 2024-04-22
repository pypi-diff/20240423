# Comparing `tmp/quick_server-0.9.3.tar.gz` & `tmp/quick_server-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_server-0.9.3.tar", last modified: Mon Apr 22 01:55:30 2024, max compression
+gzip compressed data, was "quick_server-0.9.4.tar", last modified: Mon Apr 22 19:09:26 2024, max compression
```

## Comparing `quick_server-0.9.3.tar` & `quick_server-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.759650 quick_server-0.9.3/
--rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.3/LICENSE
--rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.3/MANIFEST.in
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 01:55:30.759421 quick_server-0.9.3/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.3/README.rst
--rw-r--r--   0 krause     (501) staff       (20)     3878 2024-04-22 01:53:35.000000 quick_server-0.9.3/pyproject.toml
--rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 01:55:30.759687 quick_server-0.9.3/setup.cfg
--rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.3/setup.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.755005 quick_server-0.9.3/src/
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.758430 quick_server-0.9.3/src/quick_server/
--rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/__main__.py
--rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.3/src/quick_server/favicon.ico
--rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.3/src/quick_server/py.typed
--rw-r--r--   0 krause     (501) staff       (20)   149248 2024-04-22 01:53:35.000000 quick_server-0.9.3/src/quick_server/quick_server.py
--rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker.js
--rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker.legacy.js
--rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker_request.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.759175 quick_server-0.9.3/src/quick_server.egg-info/
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)      456 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/SOURCES.txt
--rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/dependency_links.txt
--rw-r--r--   0 krause     (501) staff       (20)       13 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/top_level.txt
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.254434 quick_server-0.9.4/
+-rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.4/LICENSE
+-rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.4/MANIFEST.in
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 19:09:26.254238 quick_server-0.9.4/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.4/README.rst
+-rw-r--r--   0 krause     (501) staff       (20)     3878 2024-04-22 19:01:33.000000 quick_server-0.9.4/pyproject.toml
+-rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 19:09:26.254472 quick_server-0.9.4/setup.cfg
+-rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.4/setup.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.250941 quick_server-0.9.4/src/
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.253382 quick_server-0.9.4/src/quick_server/
+-rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/__main__.py
+-rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.4/src/quick_server/favicon.ico
+-rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.4/src/quick_server/py.typed
+-rw-r--r--   0 krause     (501) staff       (20)   149916 2024-04-22 19:08:48.000000 quick_server-0.9.4/src/quick_server/quick_server.py
+-rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker.js
+-rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker.legacy.js
+-rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker_request.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.254028 quick_server-0.9.4/src/quick_server.egg-info/
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)      456 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/SOURCES.txt
+-rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/dependency_links.txt
+-rw-r--r--   0 krause     (501) staff       (20)       13 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/top_level.txt
```

### Comparing `quick_server-0.9.3/LICENSE` & `quick_server-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/PKG-INFO` & `quick_server-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.3
+Version: 0.9.4
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `quick_server-0.9.3/README.rst` & `quick_server-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/pyproject.toml` & `quick_server-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
     name = "quick_server"
     description = "QuickServer is a quick to use and easy to set up server implementation."
     readme = "README.rst"
-    version = "0.9.3"
+    version = "0.9.4"
     authors = [
         {name = "Josua Krause", email = "josua.krause@gmail.com"},
     ]
     keywords = [
         "server",
         "REST",
         "file",
```

### Comparing `quick_server-0.9.3/setup.py` & `quick_server-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server/__init__.py` & `quick_server-0.9.4/src/quick_server/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server/__main__.py` & `quick_server-0.9.4/src/quick_server/__main__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server/quick_server.py` & `quick_server-0.9.4/src/quick_server/quick_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,14 +713,16 @@
 
     server_version: str = f"QuickServer/{__version__}"
 
     protocol_version: str = "HTTP/1.1"
 
     common_invalid_paths: set[str] = set()
 
+    debug_proxy: bool = False
+
     def __str__(self) -> str:
         return f"{self.__class__.__name__}[{self.command} {self.path}]"
 
     def convert_argmap(
             self,
             query: str | bytes,
             ) -> dict[str, str | bool | int | float]:
@@ -1299,34 +1301,41 @@
     def send_to_proxy(self, proxy_url: str) -> None:
         """
         Forward the request to the given proxy.
 
         Args:
             proxy_url (str): The proxy URL.
         """
+        is_debug = self.debug_proxy
         clen = _GETHEADER(self.headers, "content-length")
         clen = int(clen) if clen is not None else 0
         if clen > 0:
             payload: bytes | None = self.rfile.read(clen)
         else:
             payload = None
 
         method = thread_local.method
         headers_in = dict(self.headers.items())
+        if is_debug:
+            msg(f"proxy to {method} {proxy_url}: {headers_in=} {payload=}")
         req = Request(
             proxy_url,
             data=payload,
             headers=headers_in,
             method=method)
 
         def process(response: Any) -> None:
             bio = BytesIO()
             shutil.copyfileobj(response, bio)
             outlen = bio.tell()
             thread_local.size = outlen
+            if is_debug:
+                msg(
+                    f"response {response.code} {dict(response.headers)=} "
+                    f"{outlen=}")
             self.send_response(response.code)
             has_content_length = False
             is_chunked = False
             for (hkey, hval) in response.headers.items():
                 lower_key = f"{hkey}".lower()
                 lower_val = f"{hval}".strip().lower()
                 if lower_key == "content-length":
@@ -2630,14 +2639,24 @@
         start with '/'.
 
         Args:
             invalid_paths (Iterable[str]): The new set of paths.
         """
         QuickServerRequestHandler.common_invalid_paths = set(invalid_paths)
 
+    def set_debug_proxy(self, is_debug_proxy: bool) -> None:
+        """
+        Sets whether to provide information about proxied requests.
+
+        Args:
+            is_debug_proxy (bool): If True, additional information is printed
+                on each proxy request.
+        """
+        QuickServerRequestHandler.debug_proxy = is_debug_proxy
+
     # request processing #
 
     def _process_request(
             self,
             request: bytes,
             client_address: tuple[str, int]) -> None:
         """Actually processes the request."""
```

### Comparing `quick_server-0.9.3/src/quick_server/worker.js` & `quick_server-0.9.4/src/quick_server/worker.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server/worker.legacy.js` & `quick_server-0.9.4/src/quick_server/worker.legacy.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server/worker_request.py` & `quick_server-0.9.4/src/quick_server/worker_request.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.3/src/quick_server.egg-info/PKG-INFO` & `quick_server-0.9.4/src/quick_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.3
+Version: 0.9.4
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

