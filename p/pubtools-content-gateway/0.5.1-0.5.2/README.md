# Comparing `tmp/pubtools-content-gateway-0.5.1.tar.gz` & `tmp/pubtools_content_gateway-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubtools-content-gateway-0.5.1.tar", last modified: Mon Jul 10 07:29:36 2023, max compression
+gzip compressed data, was "pubtools_content_gateway-0.5.2.tar", last modified: Tue Apr 23 12:26:37 2024, max compression
```

## Comparing `pubtools-content-gateway-0.5.1.tar` & `pubtools_content_gateway-0.5.2.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/_content_gateway.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/entrypoints_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_cgw.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_staged_cgw.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    29726 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_cgw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_staged_cgw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.855295 pubtools_content_gateway-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-23 12:26:37.855295 pubtools_content_gateway-0.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.851295 pubtools_content_gateway-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/_content_gateway.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/entrypoints_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/push_base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/push_cgw.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/docs/push_staged_cgw.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.851295 pubtools_content_gateway-0.5.2/pubtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.851295 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29726 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_staged_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/pubtools/_content_gateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.851295 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 12:26:37.000000 pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 12:26:37.855295 pubtools_content_gateway-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:26:37.851295 pubtools_content_gateway-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_cgw_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20700 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_cgw_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_cgw_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_push_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_push_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_push_staged_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-23 12:26:30.000000 pubtools_content_gateway-0.5.2/tests/test_utils.py
```

### Comparing `pubtools-content-gateway-0.5.1/LICENSE` & `pubtools_content_gateway-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/CHANGELOG.rst` & `pubtools_content_gateway-0.5.2/docs/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ChangeLog
 =========
 
+0.5.2 (2024-04-23)
+------------------
+* adjust schema for Pub pushes without pushItemPath
+
 0.5.1 (2023-07-10)
 ------------------
 * Fix release workflow
 
 0.5.0 (2023-07-10)
 ------------------
 * Support RAW content push
```

### Comparing `pubtools-content-gateway-0.5.1/docs/Makefile` & `pubtools_content_gateway-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/README.rst` & `pubtools_content_gateway-0.5.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/_content_gateway.rst` & `pubtools_content_gateway-0.5.2/docs/_content_gateway.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/conf.py` & `pubtools_content_gateway-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/entrypoints_reference.rst` & `pubtools_content_gateway-0.5.2/docs/entrypoints_reference.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/index.rst` & `pubtools_content_gateway-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/push_cgw.rst` & `pubtools_content_gateway-0.5.2/docs/push_cgw.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/docs/push_staged_cgw.rst` & `pubtools_content_gateway-0.5.2/docs/push_staged_cgw.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_authentication.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_authentication.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_client.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_client.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_session.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/cgw_session.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_base.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_base.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_cgw.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_cgw.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_staged_cgw.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/push_staged_cgw.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,57 +92,64 @@
 
         for item in self.push_items:
             if isinstance(item, CGWPushItem):
                 parsed_items = yaml_parser(os.path.join(item.origin, item.src))
                 parsed_items = format_cgw_items(parsed_items)
 
                 for pitem in parsed_items:
-                    validate_data(pitem, staged=True)
+                    validate_data(pitem)
 
                 parsed_items = sort_items(parsed_items)
                 try:
                     for pitem in parsed_items:
                         if pitem["type"] == "product":
                             self.process_product(pitem)
                         if pitem.get("type") == "product_version":
                             self.process_version(pitem)
                         if pitem["type"] == "file":
-                            found = None
-                            for push_item in self.push_items:
-                                if isinstance(push_item, DirectoryPushItem):
-                                    found = "directory_item"
-                                elif (
-                                    push_item.src.replace(push_item.origin, "").lstrip("/")
-                                    == pitem["metadata"]["pushItemPath"]
-                                ):
-                                    found = "file_item"
-                                if found:
-                                    break
-                            else:
-                                raise ValueError(
-                                    "Unable to find push item with path:%s" % pitem["metadata"]["pushItemPath"]
-                                )
-                            if found == "file_item":
-                                pulp_push_unit = self.pulp_push_units[self.push_item_str(push_item)]
-                                pulp_push_item = self.processed_push_items[self.push_item_str(push_item)]
-                                pitem["metadata"]["downloadURL"] = pulp_push_unit.cdn_path
-                                pitem["metadata"]["md5"] = pulp_push_item.md5sum
-                                pitem["metadata"]["sha256"] = pulp_push_unit.sha256sum
-                                pitem["metadata"]["size"] = os.stat(push_item.src).st_size
-                            else:
-                                filename = pitem["metadata"]["pushItemPath"].split("/")[-1]
-                                file_path = os.path.join(push_item.src, filename)
-                                with open(file_path, "rb") as f:
-                                    bytes = f.read()
-                                    pitem["metadata"]["md5"] = hashlib.md5(bytes).hexdigest()
-                                    pitem["metadata"]["sha256"] = hashlib.sha256(bytes).hexdigest()
-                                pitem["metadata"]["size"] = os.path.getsize(file_path)
-                                pitem["metadata"]["downloadURL"] = "/content/origin/files/sha256/{0}/{1}/{2}".format(
-                                    pitem["metadata"]["sha256"][:2], pitem["metadata"]["sha256"], filename
-                                )
+                            if "pushItemPath" in pitem["metadata"]:
+                                # push to CDN and set required pitem attributes for CGW entry
+                                found = None
+                                for push_item in self.push_items:
+                                    if isinstance(push_item, DirectoryPushItem):
+                                        found = "directory_item"
+                                    elif (
+                                        push_item.src.replace(push_item.origin, "").lstrip("/")
+                                        == pitem["metadata"]["pushItemPath"]
+                                    ):
+                                        found = "file_item"
+                                    if found:
+                                        break
+                                else:
+                                    raise ValueError(
+                                        "Unable to find push item with path:%s" % pitem["metadata"]["pushItemPath"]
+                                    )
+                                if found == "file_item":
+                                    pulp_push_unit = self.pulp_push_units[self.push_item_str(push_item)]
+                                    pulp_push_item = self.processed_push_items[self.push_item_str(push_item)]
+                                    pitem["metadata"]["downloadURL"] = pulp_push_unit.cdn_path
+                                    pitem["metadata"]["md5"] = pulp_push_item.md5sum
+                                    pitem["metadata"]["sha256"] = pulp_push_unit.sha256sum
+                                    pitem["metadata"]["size"] = os.stat(push_item.src).st_size
+                                else:
+                                    filename = pitem["metadata"]["pushItemPath"].split("/")[-1]
+                                    file_path = os.path.join(push_item.src, filename)
+                                    with open(file_path, "rb") as f:
+                                        bytes = f.read()
+                                        pitem["metadata"]["md5"] = hashlib.md5(bytes).hexdigest()
+                                        pitem["metadata"]["sha256"] = hashlib.sha256(bytes).hexdigest()
+                                    pitem["metadata"]["size"] = os.path.getsize(file_path)
+                                    pitem["metadata"]["downloadURL"] = (
+                                        "/content/origin/files/sha256/{0}/{1}/{2}".format(
+                                            pitem["metadata"]["sha256"][:2],
+                                            pitem["metadata"]["sha256"],
+                                            filename,
+                                        )
+                                    )
+                            # carry out CGW operations
                             self.process_file(pitem)
 
                     self.make_visible()
                     LOG.info("\n All CGW operations are successfully completed...!")
                 except Exception as error:
                     LOG.exception("Exception occurred during the CGW operation %s" % error)
                     LOG.info("Rolling back the partial operation")
```

### Comparing `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/utils.py` & `pubtools_content_gateway-0.5.2/pubtools/_content_gateway/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,113 +43,110 @@
                 "ga": {"type": "boolean"},
                 "termsAndConditions": {"type": "string"},
                 "trackingDisabled": {"type": "boolean"},
                 "hidden": {"type": "boolean"},
                 "invisible": {"type": "boolean"},
                 "releaseDate": {"type": "string"},
             },
-            "required": ["productName", "productCode", "versionName", "termsAndConditions"],
-        },
-    },
-    "required": ["type", "action", "metadata"],
-}
-
-FILE_SCHEMA = {
-    "type": "object",
-    "properties": {
-        "type": {"type": "string"},
-        "action": {"type": "string", "enum": ["create", "update", "delete"]},
-        "metadata": {
-            "type": "object",
-            "properties": {
-                "productName": {"type": "string"},
-                "productCode": {"type": ["string", "null"]},
-                "productVersionName": {"type": ["string", "number", "null"]},
-                "description": {"type": ["string", "null"]},
-                "label": {"type": ["string", "null"]},
-                "order": {"type": "integer"},
-                "hidden": {"type": "boolean"},
-                "invisible": {"type": "boolean"},
-                "type": {"type": "string"},
-                "differentProductThankYouPage": {"type": ["number", "null"]},
-                "downloadURL": {"type": "string"},
-                "shortURL": {"type": "string"},
-                "size": {"type": ["number", "null"]},
-                "md5": {"type": ["string", "number", "null"]},
-            },
             "required": [
                 "productName",
                 "productCode",
-                "productVersionName",
-                "downloadURL",
+                "versionName",
+                "termsAndConditions",
             ],
         },
     },
     "required": ["type", "action", "metadata"],
 }
 
-FILE_STAGED_SCHEMA = {
+FILE_SCHEMA = {
     "type": "object",
     "properties": {
         "type": {"type": "string"},
         "action": {"type": "string", "enum": ["create", "update", "delete"]},
         "metadata": {
-            "type": "object",
-            "properties": {
-                "productName": {"type": "string"},
-                "productCode": {"type": ["string", "null"]},
-                "productVersionName": {"type": ["string", "number", "null"]},
-                "description": {"type": ["string", "null"]},
-                "label": {"type": ["string", "null"]},
-                "order": {"type": "integer"},
-                "hidden": {"type": "boolean"},
-                "invisible": {"type": "boolean"},
-                "type": {"type": "string"},
-                "differentProductThankYouPage": {"type": ["number", "null"]},
-                "shortURL": {"type": "string"},
-                "pushItemPath": {"type": "string"},
-            },
-            "required": [
-                "productName",
-                "productCode",
-                "productVersionName",
-                "pushItemPath",
-            ],
+            "oneOf": [
+                {
+                    "type": "object",
+                    "properties": {
+                        "productName": {"type": "string"},
+                        "productCode": {"type": ["string", "null"]},
+                        "productVersionName": {"type": ["string", "number", "null"]},
+                        "description": {"type": ["string", "null"]},
+                        "label": {"type": ["string", "null"]},
+                        "order": {"type": "integer"},
+                        "hidden": {"type": "boolean"},
+                        "invisible": {"type": "boolean"},
+                        "type": {"type": "string"},
+                        "differentProductThankYouPage": {"type": ["number", "null"]},
+                        "shortURL": {"type": "string"},
+                        "pushItemPath": {"type": "string"},
+                    },
+                    "required": [
+                        "productName",
+                        "productCode",
+                        "productVersionName",
+                        "pushItemPath",
+                    ],
+                },
+                {
+                    "type": "object",
+                    "properties": {
+                        "productName": {"type": "string"},
+                        "productCode": {"type": ["string", "null"]},
+                        "productVersionName": {"type": ["string", "number", "null"]},
+                        "description": {"type": ["string", "null"]},
+                        "label": {"type": ["string", "null"]},
+                        "order": {"type": "integer"},
+                        "hidden": {"type": "boolean"},
+                        "invisible": {"type": "boolean"},
+                        "type": {"type": "string"},
+                        "differentProductThankYouPage": {"type": ["number", "null"]},
+                        "downloadURL": {"type": "string"},
+                        "shortURL": {"type": "string"},
+                        "size": {"type": ["number", "null"]},
+                        "md5": {"type": ["string", "number", "null"]},
+                    },
+                    "required": [
+                        "productName",
+                        "productCode",
+                        "productVersionName",
+                        "downloadURL",
+                    ],
+                },
+            ]
         },
     },
     "required": ["type", "action", "metadata"],
 }
 
 
-def validate_data(json_data, staged=False):
+def validate_data(json_data):
     """
     Validate that json_data contains all the necessary data
     with defined with json schemas
 
     Args:
         json_data (dict)
             JSON dictionary with content gateway data
-        staged (bool)
-            optional. Indicates if resulting json_data needs to
-            validate against FILE_STAGED_SCHEMA
 
     Raises:
         ValidationError
             The json_data type doesn't match with schema
     Returns:
         True: if validation succeed
     """
 
     item_type = json_data.get("type")
     if item_type == "product":
         validate(instance=json_data, schema=PRODUCT_SCHEMA)
     elif item_type == "product_version":
         validate(instance=json_data, schema=VERSION_SCHEMA)
     elif item_type == "file":
-        validate(instance=json_data, schema=FILE_STAGED_SCHEMA if staged else FILE_SCHEMA)
+        validate(instance=json_data, schema=FILE_SCHEMA)
     LOG.info("Data validation successful for %s: %s" % (item_type, json_data.get("metadata").get("productCode")))
     return True
 
 
 def yaml_parser(file_path):
     """
     Parse the yaml data into json data
@@ -200,25 +197,45 @@
     file_delete = []
     version_delete = []
     product_delete = []
     sorted_items = []
 
     for data in items:
         if data["type"] == "product":
-            product_create_update.append(data) if data["action"] in ["create", "update"] else product_delete.append(
-                data
+            (
+                product_create_update.append(data)
+                if data["action"]
+                in [
+                    "create",
+                    "update",
+                ]
+                else product_delete.append(data)
             )
 
         if data["type"] == "product_version":
-            version_create_update.append(data) if data["action"] in ["create", "update"] else version_delete.append(
-                data
+            (
+                version_create_update.append(data)
+                if data["action"]
+                in [
+                    "create",
+                    "update",
+                ]
+                else version_delete.append(data)
             )
 
         if data["type"] == "file":
-            file_create_update.append(data) if data["action"] in ["create", "update"] else file_delete.append(data)
+            (
+                file_create_update.append(data)
+                if data["action"]
+                in [
+                    "create",
+                    "update",
+                ]
+                else file_delete.append(data)
+            )
 
     sorted_items.extend(product_create_update)
     sorted_items.extend(version_create_update)
     sorted_items.extend(file_create_update)
     sorted_items.extend(file_delete)
     sorted_items.extend(version_delete)
     sorted_items.extend(product_delete)
```

### Comparing `pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/SOURCES.txt` & `pubtools_content_gateway-0.5.2/pubtools_content_gateway.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,8 +23,15 @@
 pubtools/_content_gateway/push_staged_cgw.py
 pubtools/_content_gateway/utils.py
 pubtools_content_gateway.egg-info/PKG-INFO
 pubtools_content_gateway.egg-info/SOURCES.txt
 pubtools_content_gateway.egg-info/dependency_links.txt
 pubtools_content_gateway.egg-info/entry_points.txt
 pubtools_content_gateway.egg-info/requires.txt
-pubtools_content_gateway.egg-info/top_level.txt
+pubtools_content_gateway.egg-info/top_level.txt
+tests/test_cgw_authentication.py
+tests/test_cgw_client.py
+tests/test_cgw_session.py
+tests/test_push_base.py
+tests/test_push_cgw.py
+tests/test_push_staged_cgw.py
+tests/test_utils.py
```

### Comparing `pubtools-content-gateway-0.5.1/setup.py` & `pubtools_content_gateway-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 setup(
     name="pubtools-content-gateway",
-    version="0.5.1",
+    version="0.5.2",
     description=get_description(),
     long_description_content_type="text/markdown",
     author="Javed Alam",
     author_email="jalam@redhat.com",
     url="https://github.com/release-engineering/pubtools-content-gateway",
     classifiers=classifiers,
     packages=find_packages(exclude=["tests"]),
```

