# Comparing `tmp/sema4ai_actions-0.3.0.tar.gz` & `tmp/sema4ai_actions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.3.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.3.1.tar", max compression
```

## Comparing `sema4ai_actions-0.3.0.tar` & `sema4ai_actions-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2958 2024-04-22 19:53:41.822063 sema4ai_actions-0.3.0/README.md
--rw-r--r--   0        0        0      971 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4975 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    11619 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7519 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11151 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8376 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    31250 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2141 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      252 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    11986 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     4355 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     4478 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/_secret.py
--rw-r--r--   0        0        0     2277 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-04-22 19:53:41.826063 sema4ai_actions-0.3.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 sema4ai_actions-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-04-23 11:43:04.195086 sema4ai_actions-0.3.1/README.md
+-rw-r--r--   0        0        0      971 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4975 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    11619 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11151 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8376 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    31250 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      336 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2141 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      252 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    11986 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     4355 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     4478 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/_secret.py
+-rw-r--r--   0        0        0     2277 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:43:04.199086 sema4ai_actions-0.3.1/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.3.1/PKG-INFO
```

### Comparing `sema4ai_actions-0.3.0/README.md` & `sema4ai_actions-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# ⚡️ robocorp-actions
+# ⚡️ sema4ai-actions
 
-A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Robocorp Action Server](../action_server/).
+A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Sema4.ai Action Server](https://github.com/sema4ai/actions#readme).
 
 ## Getting started
 
-If you have not setup Action Server already, see the [🏃‍♂️ Quickstart](https://github.com/robocorp/robocorp#quickstart) on how to do that.
+If you have not setup Action Server already, see the [🏃‍♂️ Quickstart](https://github.com/sema4ai/actions#quickstart) on how to do that.
 
 Decorate your Python function with the `@action` decorator:
 
 ```py
-from robocorp.actions import action
+from sema4ai.actions import action
 
 @action
 def sum_numbers(a: float, b: float) -> float:
     ...
 ```
 
 **And your function is now an ⚡️Action!**
@@ -59,21 +59,21 @@
 ```
 
 ### Execution
 
 To get the full benefits of your actions, the suggested way to run them is using Action Server. But it's also possible to do that directly in command line by passing the named arguments:
 
 ```sh
-python -m robocorp.actions run -- --city=Helsinki --days=3
+python -m sema4ai.actions run -- --city=Helsinki --days=3
 ```
 
 ## Guides
 
-- [Request headers](https://github.com/robocorp/robocorp/blob/master/actions/docs/guides/00-request.md)
+- [Request headers](https://github.com/sema4ai/actions/blob/master/actions/docs/guides/00-request.md)
 
 ## API Reference
 
-Explore our [API](https://github.com/robocorp/robocorp/blob/master/actions/docs/api/README.md) for extensive documentation.
+Explore our [API](https://github.com/sema4ai/actions/blob/master/actions/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
-A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/actions/docs/CHANGELOG.md).
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/sema4ai/actions/blob/master/actions/docs/CHANGELOG.md).
```

### Comparing `sema4ai_actions-0.3.0/pyproject.toml` & `sema4ai_actions-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.3.0"
+version = "0.3.1"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._secret import Secret
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_action_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,25 @@
                 f"Error: the {env_name} is expected to be a json list containing "
                 f"only strings. Found: {lst_info_to_decrypt}."
             )
 
     return lst_info_to_decrypt
 
 
+def _decrypt(key: bytes, iv: bytes, ciphertext: bytes, tag: bytes) -> bytes:
+    from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+
+    decryptor = Cipher(
+        algorithms.AES(key),
+        modes.GCM(iv, tag),
+    ).decryptor()
+
+    return decryptor.update(ciphertext) + decryptor.finalize()
+
+
 class ActionContext:
     """
     This is data received as input which may or may not be encrypted.
 
     When a user requests the actual value, it'll be decrypted if that's the case.
     """
 
@@ -108,82 +119,77 @@
 
         if not self._encrypted:
             raise RuntimeError("Expected data to be encrypted if it reached here!")
 
         from robocorp import log
 
         with log.suppress():
-            from cryptography.hazmat.primitives.ciphers.aead import AESGCM
-
             keys = _get_str_list_from_env(
                 "ACTION_SERVER_DECRYPT_KEYS", env=self._env or os.environ
             )
 
             if not keys:
                 raise RuntimeError(
                     "The information in the X-Action-Server seems to be encrypted, but decryption keys are not available in ACTION_SERVER_DECRYPT_KEYS."
                 )
 
             cipher = self._encrypted_data["cipher"]
             algorithm = self._encrypted_data["algorithm"]
             iv = self._encrypted_data["iv"]
-            auth_tag = self._encrypted_data.get("auth-tag")
+            auth_tag = self._encrypted_data["auth-tag"]
 
             if not isinstance(cipher, str):
                 raise RuntimeError(
                     f"Expected the cipher to be a str. Found: {cipher!r}"
                 )
 
             if not isinstance(algorithm, str):
                 raise RuntimeError(
                     f"Expected the algorithm to be a str. Found: {algorithm!r}"
                 )
 
             if not isinstance(iv, str):
                 raise RuntimeError(f"Expected the iv to be a str. Found: {iv!r}")
 
+            if not isinstance(auth_tag, str):
+                raise RuntimeError(
+                    f"Expected the auth-tag to be a str. Found: {auth_tag!r}"
+                )
+
             try:
                 cipher_decoded_base_64: bytes = base64.b64decode(cipher)
             except Exception:
                 raise RuntimeError(
                     "Unable to decode the 'cipher' field passed to X-Action-Context as base64."
                 )
 
             try:
                 iv_decoded_base_64: bytes = base64.b64decode(iv)
             except Exception:
                 raise RuntimeError(
                     "Unable to decode the 'iv' field passed to X-Action-Context as base64."
                 )
 
-            if not auth_tag:
-                auth_tag_decoded_base_64: bytes = b""
-            else:
-                if isinstance(auth_tag, str):
-                    try:
-                        auth_tag_decoded_base_64 = base64.b64decode(auth_tag)
-                    except Exception:
-                        raise RuntimeError(
-                            "Unable to decode the 'auth-tag' field passed to X-Action-Context as base64."
-                        )
-                else:
-                    raise RuntimeError(
-                        f"Expected the auth-tag to be a str. Found: {auth_tag!r}"
-                    )
+            try:
+                auth_tag_decoded_base_64 = base64.b64decode(auth_tag)
+            except Exception:
+                raise RuntimeError(
+                    "Unable to decode the 'auth-tag' field passed to X-Action-Context as base64."
+                )
 
             if algorithm != "aes256-gcm":
                 raise RuntimeError(
                     f"Unable to recognize X-Action-Context encryption algorithm: {algorithm}"
                 )
 
             for key in keys:
                 k: bytes = base64.b64decode(key.encode("ascii"))
-                aesgcm = AESGCM(k)
                 try:
-                    raw_data = aesgcm.decrypt(
+                    raw_data = _decrypt(
+                        k,
                         iv_decoded_base_64,
                         cipher_decoded_base_64,
                         auth_tag_decoded_base_64,
                     )
                     break
                 except Exception:
                     continue
```

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_commands.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/_secret.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.3.1/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.3.0/PKG-INFO` & `sema4ai_actions-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,26 +16,26 @@
 Requires-Dist: docstring_parser_fork (>=0.0.5,<0.0.6)
 Requires-Dist: psutil (>=5.0,<6.0)
 Requires-Dist: robocorp-log (>=2.4,<3)
 Requires-Dist: robocorp-truststore (>=0.8.0)
 Project-URL: Repository, https://github.com/Sema4AI/actions/
 Description-Content-Type: text/markdown
 
-# ⚡️ robocorp-actions
+# ⚡️ sema4ai-actions
 
-A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Robocorp Action Server](../action_server/).
+A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Sema4.ai Action Server](https://github.com/sema4ai/actions#readme).
 
 ## Getting started
 
-If you have not setup Action Server already, see the [🏃‍♂️ Quickstart](https://github.com/robocorp/robocorp#quickstart) on how to do that.
+If you have not setup Action Server already, see the [🏃‍♂️ Quickstart](https://github.com/sema4ai/actions#quickstart) on how to do that.
 
 Decorate your Python function with the `@action` decorator:
 
 ```py
-from robocorp.actions import action
+from sema4ai.actions import action
 
 @action
 def sum_numbers(a: float, b: float) -> float:
     ...
 ```
 
 **And your function is now an ⚡️Action!**
@@ -81,22 +81,22 @@
 ```
 
 ### Execution
 
 To get the full benefits of your actions, the suggested way to run them is using Action Server. But it's also possible to do that directly in command line by passing the named arguments:
 
 ```sh
-python -m robocorp.actions run -- --city=Helsinki --days=3
+python -m sema4ai.actions run -- --city=Helsinki --days=3
 ```
 
 ## Guides
 
-- [Request headers](https://github.com/robocorp/robocorp/blob/master/actions/docs/guides/00-request.md)
+- [Request headers](https://github.com/sema4ai/actions/blob/master/actions/docs/guides/00-request.md)
 
 ## API Reference
 
-Explore our [API](https://github.com/robocorp/robocorp/blob/master/actions/docs/api/README.md) for extensive documentation.
+Explore our [API](https://github.com/sema4ai/actions/blob/master/actions/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
-A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/actions/docs/CHANGELOG.md).
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/sema4ai/actions/blob/master/actions/docs/CHANGELOG.md).
```

