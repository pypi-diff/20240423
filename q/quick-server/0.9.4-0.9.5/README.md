# Comparing `tmp/quick_server-0.9.4.tar.gz` & `tmp/quick_server-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_server-0.9.4.tar", last modified: Mon Apr 22 19:09:26 2024, max compression
+gzip compressed data, was "quick_server-0.9.5.tar", last modified: Mon Apr 22 23:37:02 2024, max compression
```

## Comparing `quick_server-0.9.4.tar` & `quick_server-0.9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.254434 quick_server-0.9.4/
--rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.4/LICENSE
--rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.4/MANIFEST.in
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 19:09:26.254238 quick_server-0.9.4/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.4/README.rst
--rw-r--r--   0 krause     (501) staff       (20)     3878 2024-04-22 19:01:33.000000 quick_server-0.9.4/pyproject.toml
--rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 19:09:26.254472 quick_server-0.9.4/setup.cfg
--rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.4/setup.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.250941 quick_server-0.9.4/src/
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.253382 quick_server-0.9.4/src/quick_server/
--rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/__main__.py
--rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.4/src/quick_server/favicon.ico
--rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.4/src/quick_server/py.typed
--rw-r--r--   0 krause     (501) staff       (20)   149916 2024-04-22 19:08:48.000000 quick_server-0.9.4/src/quick_server/quick_server.py
--rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker.js
--rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker.legacy.js
--rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.4/src/quick_server/worker_request.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 19:09:26.254028 quick_server-0.9.4/src/quick_server.egg-info/
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)      456 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/SOURCES.txt
--rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/dependency_links.txt
--rw-r--r--   0 krause     (501) staff       (20)       13 2024-04-22 19:09:26.000000 quick_server-0.9.4/src/quick_server.egg-info/top_level.txt
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 23:37:02.107987 quick_server-0.9.5/
+-rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.5/LICENSE
+-rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.5/MANIFEST.in
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 23:37:02.107796 quick_server-0.9.5/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.5/README.rst
+-rw-r--r--   0 krause     (501) staff       (20)     3878 2024-04-22 23:36:43.000000 quick_server-0.9.5/pyproject.toml
+-rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 23:37:02.108026 quick_server-0.9.5/setup.cfg
+-rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.5/setup.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 23:37:02.103249 quick_server-0.9.5/src/
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 23:37:02.106316 quick_server-0.9.5/src/quick_server/
+-rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.5/src/quick_server/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.5/src/quick_server/__main__.py
+-rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.5/src/quick_server/favicon.ico
+-rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.5/src/quick_server/py.typed
+-rw-r--r--   0 krause     (501) staff       (20)   150749 2024-04-22 23:36:43.000000 quick_server-0.9.5/src/quick_server/quick_server.py
+-rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.5/src/quick_server/worker.js
+-rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.5/src/quick_server/worker.legacy.js
+-rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.5/src/quick_server/worker_request.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 23:37:02.107574 quick_server-0.9.5/src/quick_server.egg-info/
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 23:37:02.000000 quick_server-0.9.5/src/quick_server.egg-info/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)      456 2024-04-22 23:37:02.000000 quick_server-0.9.5/src/quick_server.egg-info/SOURCES.txt
+-rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 23:37:02.000000 quick_server-0.9.5/src/quick_server.egg-info/dependency_links.txt
+-rw-r--r--   0 krause     (501) staff       (20)       13 2024-04-22 23:37:02.000000 quick_server-0.9.5/src/quick_server.egg-info/top_level.txt
```

### Comparing `quick_server-0.9.4/LICENSE` & `quick_server-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/PKG-INFO` & `quick_server-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.4
+Version: 0.9.5
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `quick_server-0.9.4/README.rst` & `quick_server-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/pyproject.toml` & `quick_server-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
     name = "quick_server"
     description = "QuickServer is a quick to use and easy to set up server implementation."
     readme = "README.rst"
-    version = "0.9.4"
+    version = "0.9.5"
     authors = [
         {name = "Josua Krause", email = "josua.krause@gmail.com"},
     ]
     keywords = [
         "server",
         "REST",
         "file",
```

### Comparing `quick_server-0.9.4/setup.py` & `quick_server-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server/__init__.py` & `quick_server-0.9.5/src/quick_server/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server/__main__.py` & `quick_server-0.9.5/src/quick_server/__main__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server/quick_server.py` & `quick_server-0.9.5/src/quick_server/quick_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,32 @@
             res = obj
         return res
 
     return json.dumps(
         do_map(json_obj), indent=2, sort_keys=True, allow_nan=False)
 
 
+def json_compact(obj: Any) -> str:
+    """
+    Creates a compact JSON from the given object. This function does not
+    correct for ECMAscript consumers.
+
+    Args:
+        obj (Any): The object.
+
+    Returns:
+        str: A JSON without any spaces or new lines.
+    """
+    return json.dumps(
+        obj,
+        sort_keys=True,
+        indent=None,
+        separators=(",", ":"))
+
+
 LOG_FILE: TextIO | None = None
 
 
 def set_log_file(fname: TextIO) -> None:
     """Sets the log file. Defaults to STD_ERR."""
     global LOG_FILE
 
@@ -981,14 +999,16 @@
                 alarm.cancel()
             ongoing = False
 
     def _handle_special(self, send_body: bool, method_str: str) -> bool:
         # pylint: disable=protected-access
 
         path = self.path
+        self.maybe_proxy_request(path)  # raises PDR on success
+
         # interpreting the URL masks to find which method to call
         method: ReqF[BytesIO | None] | None = None
         method_mask = None
         rem_path = ""
         segments: dict[str, str] = {}
 
         def is_match(
@@ -1169,39 +1189,14 @@
                     mpath = os.path.join(mpath, word)
                 # make path absolute and check if it exists
                 mpath = os.path.abspath(mpath)
                 if os.path.exists(mpath):
                     break
             # if pass is still None here the file cannot be found
             if mpath is None:
-
-                def forward(url_path: str, *, remove_last: bool) -> None:
-                    for (name, pxy) in self.server._folder_proxys:
-                        if not url_path.startswith(name):
-                            continue
-                        start_adj = 0 if remove_last else 1
-                        remain = url_path[len(name) - start_adj:]
-                        proxy = urlparse.urlparse(pxy)
-                        reala = urlparse.urlparse(init_path)
-                        pxya = urlparse.urlunparse((
-                            proxy[0],  # scheme
-                            proxy[1],  # netloc
-                            f"{proxy[2]}{remain}",  # path
-                            reala[3],  # params
-                            reala[4],  # query
-                            reala[5],  # fragment
-                        ))
-                        self.send_to_proxy(pxya)
-
-                # try proxies
-                # raises PreventDefaultResponse if successful
-                forward(orig_path, remove_last=False)
-                if len(orig_path) and orig_path[-1] != "/":
-                    forward(f"{orig_path}/", remove_last=True)
-
                 # out of luck
                 if orig_path not in self.common_invalid_paths:
                     msg(f"no matching folder alias: {orig_path}")
                 raise PreventDefaultResponse(404, "File not found")
             path: str = mpath
             if os.path.isdir(path):
                 if not is_folder:
@@ -1294,48 +1289,87 @@
         self.send_header(
             "Cache-Control",
             f"max-age={self.server.max_age}")
         self.end_headers()
         thread_local.size = 0
         return True
 
-    def send_to_proxy(self, proxy_url: str) -> None:
+    def maybe_proxy_request(self, orig_path: str) -> None:
+        """
+        Check if the given path needs to be proxied. If it is the case the
+        request is proxied and a `PreventDefaultResponse` exception is raised.
+
+        Args:
+            orig_path (str): The path.
+        """
+        # pylint: disable=protected-access
+
+        folder_proxys = self.server._folder_proxys
+
+        def forward(url_path: str, *, remove_last: bool) -> None:
+            for (name, pxy) in folder_proxys:
+                if not url_path.startswith(name):
+                    continue
+                start_adj = 0 if remove_last else 1
+                remain = url_path[len(name) - start_adj:]
+                proxy = urlparse.urlparse(pxy)
+                reala = urlparse.urlparse(orig_path)
+                pxya = urlparse.urlunparse((
+                    proxy[0],  # scheme
+                    proxy[1],  # netloc
+                    f"{proxy[2]}{remain}",  # path
+                    reala[3],  # params
+                    reala[4],  # query
+                    reala[5],  # fragment
+                ))
+                self.send_to_proxy(pxya, orig_path)
+
+        # try proxies
+        # raises PreventDefaultResponse if successful
+        forward(orig_path, remove_last=False)
+        if len(orig_path) and orig_path[-1] != "/":
+            forward(f"{orig_path}/", remove_last=True)
+
+    def send_to_proxy(self, proxy_url: str, orig_path: str) -> None:
         """
         Forward the request to the given proxy.
 
         Args:
             proxy_url (str): The proxy URL.
+            orig_path (str): The original URL path.
         """
         is_debug = self.debug_proxy
         clen = _GETHEADER(self.headers, "content-length")
         clen = int(clen) if clen is not None else 0
         if clen > 0:
             payload: bytes | None = self.rfile.read(clen)
         else:
             payload = None
 
         method = thread_local.method
         headers_in = dict(self.headers.items())
         if is_debug:
-            msg(f"proxy to {method} {proxy_url}: {headers_in=} {payload=}")
+            msg(
+                f"proxy {orig_path} to {method} {proxy_url}: "
+                f"headers={json_compact(headers_in)} {payload=}")
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
             if is_debug:
                 msg(
-                    f"response {response.code} {dict(response.headers)=} "
-                    f"{outlen=}")
+                    f"response {response.code} for {orig_path} {outlen=} "
+                    f"headers={json_compact(dict(response.headers))}")
             self.send_response(response.code)
             has_content_length = False
             is_chunked = False
             for (hkey, hval) in response.headers.items():
                 lower_key = f"{hkey}".lower()
                 lower_val = f"{hval}".strip().lower()
                 if lower_key == "content-length":
```

### Comparing `quick_server-0.9.4/src/quick_server/worker.js` & `quick_server-0.9.5/src/quick_server/worker.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server/worker.legacy.js` & `quick_server-0.9.5/src/quick_server/worker.legacy.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server/worker_request.py` & `quick_server-0.9.5/src/quick_server/worker_request.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.4/src/quick_server.egg-info/PKG-INFO` & `quick_server-0.9.5/src/quick_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.4
+Version: 0.9.5
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

