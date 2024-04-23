# Comparing `tmp/appmesh-0.8.6-py3-none-any.whl.zip` & `tmp/appmesh-0.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15674 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 04:36 appmesh/__init__.py
--rw-r--r--  2.0 unx    57114 b- defN 24-Apr-22 04:36 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/RECORD
-6 files, 68466 bytes uncompressed, 14852 bytes compressed:  78.3%
+Zip file size: 15970 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 11:32 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58527 b- defN 24-Apr-22 11:32 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-Apr-22 11:32 appmesh-0.8.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 11:32 appmesh-0.8.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-22 11:32 appmesh-0.8.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-22 11:32 appmesh-0.8.7.dist-info/RECORD
+6 files, 69879 bytes uncompressed, 15148 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.8.6.dist-info/METADATA
+Filename: appmesh-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.8.6.dist-info/WHEEL
+Filename: appmesh-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.8.6.dist-info/top_level.txt
+Filename: appmesh-0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.8.6.dist-info/RECORD
+Filename: appmesh-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -335,21 +335,37 @@
         self.jwt_token = None
         resp = self._request_http(
             AppMeshClient.Method.POST,
             path="/appmesh/login",
             header={
                 "Username": base64.b64encode(user_name.encode()),
                 "Password": base64.b64encode(user_pwd.encode()),
-                "Totp": base64.b64encode(totp_key.encode()),
                 "Expire-Seconds": self._parse_duration(timeout_seconds),
             },
         )
         if resp.status_code == HTTPStatus.OK:
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
+        elif resp.status_code == HTTPStatus.UNAUTHORIZED and "totp_challenge" in resp.json():
+            challenge = resp.json()["totp_challenge"]
+            resp = self._request_http(
+                AppMeshClient.Method.POST,
+                path="/appmesh/totp/validate",
+                header={
+                    "Username": base64.b64encode(user_name.encode()),
+                    "Totp-Challenge": base64.b64encode(challenge.encode()),
+                    "Totp": base64.b64encode(totp_key.encode()),
+                    "Expire-Seconds": self._parse_duration(timeout_seconds),
+                },
+            )
+            if resp.status_code == HTTPStatus.OK:
+                if "Access-Token" in resp.json():
+                    self.jwt_token = resp.json()["Access-Token"]
+            else:
+                print(resp.text)
         else:
             print(resp.text)
             # resp.raise_for_status()
         return self.jwt_token
 
     def logoff(self) -> bool:
         """Logoff current session from server
@@ -442,25 +458,44 @@
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/totp/setup",
             header={"Totp": base64.b64encode(totp_key.encode())},
         )
         return resp.status_code == HTTPStatus.OK
 
-    def totp_disable(self) -> bool:
+    def totp_validate(self, totp_key: str) -> bool:
+        """Validate TOTP key
+
+        Args:
+            totp_key (str): TOTP key
+
+        Returns:
+            bool: success or failure.
+        """
+        resp = self._request_http(
+            method=AppMeshClient.Method.POST,
+            path=f"/appmesh/totp/validate",
+            header={"Totp": base64.b64encode(totp_key.encode())},
+        )
+        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
+
+    def totp_disable(self, user="self") -> bool:
         """Disable 2FA for current user
 
+        Args:
+            user (str, optional): user name for disable TOTP.
+
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
-            path=f"/appmesh/totp/disable",
+            path=f"/appmesh/totp/{user}/disable",
         )
-        return resp.status_code == HTTPStatus.OK
+        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
 
     @staticmethod
     def _parse_totp_uri(totp_uri: str) -> dict:
         """Extract TOTP parameters
 
         Args:
             totp_uri (str): TOTP uri
```

## Comparing `appmesh-0.8.6.dist-info/METADATA` & `appmesh-0.8.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.8.6
+Version: 0.8.7
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.8.6 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.8.7 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

