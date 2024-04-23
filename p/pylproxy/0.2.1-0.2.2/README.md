# Comparing `tmp/pylproxy-0.2.1.tar.gz` & `tmp/pylproxy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylproxy-0.2.1.tar", max compression
+gzip compressed data, was "pylproxy-0.2.2.tar", max compression
```

## Comparing `pylproxy-0.2.1.tar` & `pylproxy-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     8323 2024-04-22 20:21:43.665587 pylproxy-0.2.1/pylproxy/__init__.py
--rw-r--r--   0        0        0     1691 2024-04-22 14:27:26.958429 pylproxy-0.2.1/pylproxy/api.py
--rw-r--r--   0        0        0      474 2024-04-18 21:36:12.950393 pylproxy-0.2.1/pylproxy/nginx/docker-compose.yml
--rw-r--r--   0        0        0       58 2024-04-17 20:45:18.481433 pylproxy-0.2.1/pylproxy/nginx/Dockerfile
--rw-r--r--   0        0        0     1040 2024-04-18 21:20:30.239239 pylproxy-0.2.1/pylproxy/nginx/nginx.conf
--rw-r--r--   0        0        0      114 2024-04-18 21:16:19.640178 pylproxy-0.2.1/pylproxy/nginx/node_env.env
--rw-r--r--   0        0        0      892 2024-03-06 22:09:31.206070 pylproxy-0.2.1/pylproxy/nginx/yagna/Dockerfile
--rw-r--r--   0        0        0      704 2024-04-22 14:40:42.682454 pylproxy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 13:30:06.690327 pylproxy-0.2.1/README.md
--rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 pylproxy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8370 2024-04-22 20:39:29.397790 pylproxy-0.2.2/pylproxy/__init__.py
+-rw-r--r--   0        0        0     1691 2024-04-22 14:27:26.958429 pylproxy-0.2.2/pylproxy/api.py
+-rw-r--r--   0        0        0      474 2024-04-18 21:36:12.950393 pylproxy-0.2.2/pylproxy/nginx/docker-compose.yml
+-rw-r--r--   0        0        0       58 2024-04-17 20:45:18.481433 pylproxy-0.2.2/pylproxy/nginx/Dockerfile
+-rw-r--r--   0        0        0     1040 2024-04-18 21:20:30.239239 pylproxy-0.2.2/pylproxy/nginx/nginx.conf
+-rw-r--r--   0        0        0      114 2024-04-18 21:16:19.640178 pylproxy-0.2.2/pylproxy/nginx/node_env.env
+-rw-r--r--   0        0        0      892 2024-03-06 22:09:31.206070 pylproxy-0.2.2/pylproxy/nginx/yagna/Dockerfile
+-rw-r--r--   0        0        0      704 2024-04-22 20:43:03.936919 pylproxy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:06.690327 pylproxy-0.2.2/README.md
+-rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 pylproxy-0.2.2/PKG-INFO
```

### Comparing `pylproxy-0.2.1/pylproxy/__init__.py` & `pylproxy-0.2.2/pylproxy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,15 @@
                     )
                     await response.prepare(request)
                     response_body = b""
                     async for line in resp.content:
                         response_body += line
                         await response.write(line)
 
+                    await response.write_eof()
                     self._logger.info(
                         f"Request from {extra_headers[CALLER_HEADER]} "
                         f"for {server_addr}:{server_port}{request.raw_path} "
                         f"routed to {extra_headers[CALLEE_HEADER]} at {host}:{port}"
                     )
                     if self._callback_response:
                         callback_response_obj: ResponseCallbackObj = {
```

### Comparing `pylproxy-0.2.1/pylproxy/api.py` & `pylproxy-0.2.2/pylproxy/api.py`

 * *Files identical despite different names*

### Comparing `pylproxy-0.2.1/pylproxy/nginx/nginx.conf` & `pylproxy-0.2.2/pylproxy/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `pylproxy-0.2.1/pylproxy/nginx/yagna/Dockerfile` & `pylproxy-0.2.2/pylproxy/nginx/yagna/Dockerfile`

 * *Files identical despite different names*

### Comparing `pylproxy-0.2.1/pyproject.toml` & `pylproxy-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylproxy"
-version = "0.2.1"
+version = "0.2.2"
 description = "Proxy for use in Goth instead of mitmproxy"
 authors = ["scx1332 <sieciech.czajka@golem.network>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.9"
 python = "^3.10"
```

