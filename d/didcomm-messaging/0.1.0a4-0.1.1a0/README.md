# Comparing `tmp/didcomm_messaging-0.1.0a4.tar.gz` & `tmp/didcomm_messaging-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didcomm_messaging-0.1.0a4.tar", last modified: Wed Jan 24 19:48:03 2024, max compression
+gzip compressed data, was "didcomm_messaging-0.1.1a0.tar", last modified: Tue Apr 23 18:55:15 2024, max compression
```

## Comparing `didcomm_messaging-0.1.0a4.tar` & `didcomm_messaging-0.1.1a0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0    11357 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     3592 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/README.md
--rw-r--r--   0        0        0     3329 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/__init__.py
--rw-r--r--   0        0        0      221 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/__init__.py
--rw-r--r--   0        0        0       52 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/__init__.py
--rw-r--r--   0        0        0    14000 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/askar.py
--rw-r--r--   0        0        0     7510 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/authlib.py
--rw-r--r--   0        0        0      646 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/basic.py
--rw-r--r--   0        0        0     4085 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/base.py
--rw-r--r--   0        0        0    15151 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/jwe.py
--rw-r--r--   0        0        0       42 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/__init__.py
--rw-r--r--   0        0        0     3880 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multibase.py
--rw-r--r--   0        0        0     2264 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multicodec.py
--rw-r--r--   0        0        0     6753 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/packaging.py
--rw-r--r--   0        0        0     2487 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/__init__.py
--rw-r--r--   0        0        0     1227 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/peer.py
--rw-r--r--   0        0        0     5339 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/routing.py
--rw-r--r--   0        0        0     1589 2024-01-24 19:48:03.577793 didcomm_messaging-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/__init__.py
--rw-r--r--   0        0        0     6607 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_askar.py
--rw-r--r--   0        0        0     3154 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_askar_x_authlib.py
--rw-r--r--   0        0        0     2124 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_authlib.py
--rw-r--r--   0        0        0      740 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_didresolver.py
--rw-r--r--   0        0        0     2020 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_packaging.py
--rw-r--r--   0        0        0      771 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_secrets.py
--rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0     3592 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/README.md
+-rw-r--r--   0        0        0     4855 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/__init__.py
+-rw-r--r--   0        0        0    13927 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/askar.py
+-rw-r--r--   0        0        0     7510 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/authlib.py
+-rw-r--r--   0        0        0      646 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/basic.py
+-rw-r--r--   0        0        0     4084 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/base.py
+-rw-r--r--   0        0        0    15121 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/jwe.py
+-rw-r--r--   0        0        0       42 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/__init__.py
+-rw-r--r--   0        0        0     3880 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multibase.py
+-rw-r--r--   0        0        0     2264 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multicodec.py
+-rw-r--r--   0        0        0     6742 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/packaging.py
+-rw-r--r--   0        0        0    12388 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/quickstart.py
+-rw-r--r--   0        0        0     2487 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/__init__.py
+-rw-r--r--   0        0        0     1227 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/peer.py
+-rw-r--r--   0        0        0     3811 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/web.py
+-rw-r--r--   0        0        0     5947 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/didcomm_messaging/routing.py
+-rw-r--r--   0        0        0     1590 2024-04-23 18:55:15.950390 didcomm_messaging-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/__init__.py
+-rw-r--r--   0        0        0     6607 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_askar.py
+-rw-r--r--   0        0        0     3166 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_askar_x_authlib.py
+-rw-r--r--   0        0        0     2124 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_authlib.py
+-rw-r--r--   0        0        0      740 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_didresolver.py
+-rw-r--r--   0        0        0     2787 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_didweb.py
+-rw-r--r--   0        0        0     2197 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_packaging.py
+-rw-r--r--   0        0        0      771 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_secrets.py
+-rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.1a0/PKG-INFO
```

### Comparing `didcomm_messaging-0.1.0a4/LICENSE` & `didcomm_messaging-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/README.md` & `didcomm_messaging-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/askar.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/askar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Askar backend for DIDComm Messaging."""
+
 from collections import OrderedDict
 import hashlib
 import json
 from typing import Optional, Sequence, Union
 
 from pydid import VerificationMethod
 
@@ -129,17 +130,15 @@
         """Get the key ID."""
         return self._kid
 
 
 class AskarCryptoService(CryptoService[AskarKey, AskarSecretKey]):
     """CryptoService backend implemented using Askar."""
 
-    async def ecdh_es_encrypt(
-        self, to_keys: Sequence[AskarKey], message: bytes
-    ) -> bytes:
+    async def ecdh_es_encrypt(self, to_keys: Sequence[AskarKey], message: bytes) -> bytes:
         """Encode a message into DIDComm v2 anonymous encryption."""
         builder = JweBuilder(with_flatten_recipients=False)
 
         alg_id = "ECDH-ES+A256KW"
         enc_id = "XC20P"
         enc_alg = KeyAlg.XC20P
         wrap_alg = KeyAlg.A256KW
@@ -221,31 +220,27 @@
         if not enc_alg or enc_alg not in (
             "A128GCM",
             "A256GCM",
             "A128CBC-HS256",
             "A256CBC-HS512",
             "XC20P",
         ):
-            raise CryptoServiceError(
-                f"Unsupported ECDH-ES content encryption: {enc_alg}"
-            )
+            raise CryptoServiceError(f"Unsupported ECDH-ES content encryption: {enc_alg}")
 
         epk_header = recip.header.get("epk")
         if not epk_header:
             raise CryptoServiceError("Missing ephemeral key")
 
         try:
             epk = Key.from_jwk(epk_header)
         except AskarError:
             raise CryptoServiceError("Error loading ephemeral key")
 
         try:
-            cek = ecdh.EcdhEs(
-                alg_id, None, wrapper.apv_bytes
-            ).receiver_unwrap_key(  # type: ignore
+            cek = ecdh.EcdhEs(alg_id, None, wrapper.apv_bytes).receiver_unwrap_key(  # type: ignore
                 wrap_alg,
                 enc_alg,
                 epk,
                 recip_key.key,
                 recip.encrypted_key,
             )
         except AskarError:
```

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/authlib.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/basic.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/basic.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/base.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """CryptoService and SecretsManager interfaces for DIDComm Messaging."""
 
-
 from abc import ABC, abstractmethod
 from typing import Generic, Mapping, Optional, Sequence, TypeVar, Union
 
 from pydid import VerificationMethod
 
 from didcomm_messaging.multiformats import multibase, multicodec
```

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/jwe.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/jwe.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,17 +252,15 @@
 
     @classmethod
     def _deserialize(cls, parsed: Mapping[str, Any]) -> "JweEnvelope":  # noqa: C901
         protected_b64 = parsed[IDENT_PROTECTED]
         try:
             protected: dict = json.loads(from_b64url(protected_b64))
         except json.JSONDecodeError:
-            raise ValueError(
-                "Invalid JWE: invalid JSON for protected headers"
-            ) from None
+            raise ValueError("Invalid JWE: invalid JSON for protected headers") from None
         unprotected = parsed.get("unprotected") or {}
         if protected.keys() & unprotected.keys():
             raise ValueError("Invalid JWE: duplicate header")
 
         encrypted_key = protected.get(IDENT_ENC_KEY) or parsed.get(IDENT_ENC_KEY)
         recipients = None
         protected_recipients = False
```

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multibase.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multibase.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multicodec.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multicodec.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/packaging.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/packaging.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """PackagingService interface."""
 
-
 from dataclasses import dataclass
 import hashlib
 from typing import Generic, Literal, Optional, Sequence, Tuple, Union
 
 from pydid import DIDUrl, VerificationMethod
 from didcomm_messaging.crypto import P, S, CryptoService, SecretsManager
 from didcomm_messaging.crypto.jwe import JweEnvelope, b64url, from_b64url
@@ -24,27 +23,16 @@
 class PackagingServiceError(Exception):
     """Represents an error from the DIDComm Messaging interface."""
 
 
 class PackagingService(Generic[P, S]):
     """DIDComm Messaging interface."""
 
-    def __init__(
-        self,
-        resolver: DIDResolver,
-        crypto: CryptoService[P, S],
-        secrets: SecretsManager[S],
-    ):
-        """Initialize the KMS."""
-        self.resolver = resolver
-        self.crypto = crypto
-        self.secrets = secrets
-
     async def extract_packed_message_metadata(  # noqa: C901
-        self, enc_message: Union[str, bytes]
+        self, enc_message: Union[str, bytes], secrets: SecretsManager[S]
     ) -> PackedMessageMetadata:
         """Extract metadata from a packed DIDComm message."""
         try:
             wrapper = JweEnvelope.from_json(enc_message)
         except ValueError:
             raise PackagingServiceError("Invalid packed message")
 
@@ -57,15 +45,15 @@
             raise PackagingServiceError(
                 f"Unsupported DIDComm encryption algorithm: {alg}"
             )
 
         sender_kid = None
         recip_key = None
         for kid in wrapper.recipient_key_ids:
-            recip_key = await self.secrets.get_secret_by_kid(kid)
+            recip_key = await secrets.get_secret_by_kid(kid)
             if recip_key:
                 break
 
         if not recip_key:
             raise PackagingServiceError("No recognized recipient key")
 
         expected_apv = b64url(
@@ -93,48 +81,50 @@
                 raise PackagingServiceError("Mismatch between skid and apu")
             if not sender_kid:
                 raise PackagingServiceError("Sender key ID not provided")
 
         return PackedMessageMetadata(wrapper, method, recip_key, sender_kid)
 
     async def unpack(
-        self, enc_message: Union[str, bytes]
+        self,
+        crypto: CryptoService[P, S],
+        resolver: DIDResolver,
+        secrets: SecretsManager[S],
+        enc_message: Union[str, bytes],
     ) -> Tuple[bytes, PackedMessageMetadata]:
         """Unpack a DIDComm message."""
-        metadata = await self.extract_packed_message_metadata(enc_message)
+        metadata = await self.extract_packed_message_metadata(enc_message, secrets)
 
         if metadata.method == "ECDH-ES":
             return (
-                await self.crypto.ecdh_es_decrypt(enc_message, metadata.recip_key),
+                await crypto.ecdh_es_decrypt(enc_message, metadata.recip_key),
                 metadata,
             )
 
         if not metadata.sender_kid:
             raise PackagingServiceError("Missing sender key ID")
 
-        sender_vm = await self.resolver.resolve_and_dereference_verification_method(
+        sender_vm = await resolver.resolve_and_dereference_verification_method(
             metadata.sender_kid
         )
-        sender_key = self.crypto.verification_method_to_public_key(sender_vm)
+        sender_key = crypto.verification_method_to_public_key(sender_vm)
 
         return (
-            await self.crypto.ecdh_1pu_decrypt(
-                enc_message, metadata.recip_key, sender_key
-            ),
+            await crypto.ecdh_1pu_decrypt(enc_message, metadata.recip_key, sender_key),
             metadata,
         )
 
-    async def recip_for_kid_or_default_for_did(self, kid_or_did: str) -> P:
+    async def recip_for_kid_or_default_for_did(
+        self, crypto: CryptoService[P, S], resolver: DIDResolver, kid_or_did: str
+    ) -> P:
         """Resolve a verification method for a kid or return default recip."""
         if "#" in kid_or_did:
-            vm = await self.resolver.resolve_and_dereference_verification_method(
-                kid_or_did
-            )
+            vm = await resolver.resolve_and_dereference_verification_method(kid_or_did)
         else:
-            doc = await self.resolver.resolve_and_parse(kid_or_did)
+            doc = await resolver.resolve_and_parse(kid_or_did)
             if not doc.key_agreement:
                 raise PackagingServiceError(
                     "No key agreement methods found; cannot determine recipient"
                 )
 
             default = doc.key_agreement[0]
             if isinstance(default, DIDUrl):
@@ -142,22 +132,22 @@
                 if not isinstance(vm, VerificationMethod):
                     raise PackagingServiceError(
                         f"Expected verification method, found: {type(vm)}"
                     )
             else:
                 vm = default
 
-        return self.crypto.verification_method_to_public_key(vm)
+        return crypto.verification_method_to_public_key(vm)
 
-    async def default_sender_kid_for_did(self, did: str) -> str:
+    async def default_sender_kid_for_did(self, resolver: DIDResolver, did: str) -> str:
         """Determine the kid of the default sender key for a DID."""
         if "#" in did:
             return did
 
-        doc = await self.resolver.resolve_and_parse(did)
+        doc = await resolver.resolve_and_parse(did)
         if not doc.key_agreement:
             raise PackagingServiceError(
                 "No key agreement methods found; cannot determine recipient"
             )
 
         default = doc.key_agreement[0]
         if isinstance(default, DIDUrl):
@@ -171,25 +161,29 @@
 
         if not vm.id.did:
             return vm.id.as_absolute(vm.controller)
         return vm.id
 
     async def pack(
         self,
+        crypto: CryptoService[P, S],
+        resolver: DIDResolver,
+        secrets: SecretsManager[S],
         message: bytes,
         to: Sequence[str],
         frm: Optional[str] = None,
         **options,
     ):
         """Pack a DIDComm message."""
-        recip_keys = [await self.recip_for_kid_or_default_for_did(kid) for kid in to]
-        sender_kid = await self.default_sender_kid_for_did(frm) if frm else None
-        sender_key = (
-            await self.secrets.get_secret_by_kid(sender_kid) if sender_kid else None
-        )
+        recip_keys = [
+            await self.recip_for_kid_or_default_for_did(crypto, resolver, kid)
+            for kid in to
+        ]
+        sender_kid = await self.default_sender_kid_for_did(resolver, frm) if frm else None
+        sender_key = await secrets.get_secret_by_kid(sender_kid) if sender_kid else None
         if frm and not sender_key:
             raise PackagingServiceError("No sender key found")
 
         if sender_key:
-            return await self.crypto.ecdh_1pu_encrypt(recip_keys, sender_key, message)
+            return await crypto.ecdh_1pu_encrypt(recip_keys, sender_key, message)
         else:
-            return await self.crypto.ecdh_es_encrypt(recip_keys, message)
+            return await crypto.ecdh_es_encrypt(recip_keys, message)
```

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/__init__.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/peer.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/peer.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/didcomm_messaging/routing.py` & `didcomm_messaging-0.1.1a0/didcomm_messaging/routing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """RoutingService interface."""
 
 import json
 import uuid
 
 from typing import Tuple, List, Dict, Any
 from pydid.service import DIDCommV2Service
+from didcomm_messaging.crypto.base import P, S, CryptoService, SecretsManager
 from didcomm_messaging.packaging import PackagingService
 from didcomm_messaging.resolver import DIDResolver
 
 
 class RoutingServiceError(Exception):
     """Raised when an error occurs in the RoutingService."""
 
 
 class RoutingService:
     """RoutingService."""
 
-    def __init__(self, packaging: PackagingService, resolver: DIDResolver):
-        """Initialize the RoutingService."""
-        self.packaging = packaging
-        self.resolver = resolver
-
-    async def _resolve_services(self, to: str) -> List[DIDCommV2Service]:
-        if not await self.resolver.is_resolvable(to):
+    async def _resolve_services(
+        self, resolver: DIDResolver, to: str
+    ) -> List[DIDCommV2Service]:
+        if not await resolver.is_resolvable(to):
             return []
-        did_doc = await self.resolver.resolve_and_parse(to)
+        did_doc = await resolver.resolve_and_parse(to)
         services = []
         if did_doc.service:  # service is not guaranteed to exist
             for did_service in did_doc.service:
+                if did_service.type != "DIDCommMessaging":
+                    continue
                 if "didcomm/v2" in did_service.service_endpoint.accept:
                     services.append(did_service)
         if not services:
             return []
         return services
 
-    async def is_forwardable_service(self, service: DIDCommV2Service) -> bool:
+    async def is_forwardable_service(
+        self, resolver: DIDResolver, service: DIDCommV2Service
+    ) -> bool:
         """Determine if the uri of a service is a service we should forward to."""
         endpoint = service.service_endpoint.uri
-        found_forwardable_service = await self.resolver.is_resolvable(endpoint)
+        found_forwardable_service = await resolver.is_resolvable(endpoint)
         return found_forwardable_service
 
     def _create_forward_message(
-        self, to: str, next_target: str, message: str
+        self, to: str, next_target: str, message: bytes
     ) -> Dict[Any, Any]:
         return {
             "typ": "application/didcomm-plain+json",
             "type": "https://didcomm.org/routing/2.0/forward",
             "id": str(uuid.uuid4()),
             "to": [to],
             # "expires_time": 123456, #  time to expire the forward message, in epoch time
@@ -58,50 +60,64 @@
                         "json": json.loads(message),
                     },
                 },
             ],
         }
 
     async def prepare_forward(
-        self, to: str, encoded_message: bytes
+        self,
+        crypto: CryptoService[P, S],
+        packaging: PackagingService,
+        resolver: DIDResolver,
+        secrets: SecretsManager[S],
+        to: str,
+        encoded_message: bytes,
     ) -> Tuple[bytes, DIDCommV2Service]:
         """Prepare a forward message, if necessary.
 
         Args:
+            crypto (CryptoService[P, S]): Crypto service
+            packaging (PackagingService): Packaging service
+            resolver (DIDResolver): Resolver instance
+            secrets (SecretsManager[S]): Secrets manager
             to (str): The recipient of the message. This will be a DID.
             encoded_message (bytes): The encoded message.
 
         Returns:
             The encoded message, and the services to forward to.
         """
 
         # Get the initial service
-        services = await self._resolve_services(to)
+        services = await self._resolve_services(resolver, to)
         chain = [
             {
                 "did": to,
                 "service": services,
             }
         ]
 
         # Loop through service DIDs until we run out of DIDs to forward to
         to_did = services[0].service_endpoint.uri
-        found_forwardable_service = await self.is_forwardable_service(services[0])
+        found_forwardable_service = await self.is_forwardable_service(
+            resolver, services[0]
+        )
         while found_forwardable_service:
-            services = await self._resolve_services(to_did)
+            services = await self._resolve_services(resolver, to_did)
             if services:
                 chain.append(
                     {
                         "did": to_did,
                         "service": services,
                     }
                 )
                 to_did = services[0].service_endpoint.uri
             found_forwardable_service = (
-                await self.is_forwardable_service(services[0]) if services else False
+                await self.is_forwardable_service(resolver, services[0])
+                if services
+                else False
             )
 
         if not chain[-1]["service"]:
             raise RoutingServiceError(f"No DIDCommV2 service endpoint found for {to}")
 
         # If we didn't find any services to forward to, just bail
         if len(chain) == 1:
@@ -121,18 +137,21 @@
             # the list, then wrapping message following routing key order
             routing_keys = service["service"][0].service_endpoint.routing_keys
             routing_keys.insert(0, service["did"])  # prepend did
 
             # Pack for each key
             while routing_keys:
                 key = routing_keys.pop()  # pop from end of list (reverse order)
-                packed_message = await self.packaging.pack(
+                packed_message = await packaging.pack(
+                    crypto,
+                    resolver,
+                    secrets,
                     json.dumps(
                         self._create_forward_message(key, next_target, packed_message)
-                    ),
+                    ).encode(),
                     [key],
                 )
                 next_target = key
 
         # Return the forward-packed message as well as the last service in the
         # chain, which is the destination of the top-level forward message.
         service = final_destination["service"]
```

### Comparing `didcomm_messaging-0.1.0a4/pyproject.toml` & `didcomm_messaging-0.1.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "didcomm-messaging"
-version = "0.1.0a4"
+version = "0.1.1a0"
 description = "DIDComm Messaging implemented with swappable backends."
 authors = [
     { name = "Daniel Bluhm", email = "dbluhm@pm.me" },
     { name = "Colton Wolkins", email = "colton@indicio.tech" },
     { name = "Micah Peltier", email = "micah@indicio.tech" },
 ]
 dependencies = [
@@ -32,18 +32,34 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest>=7.4.3",
+    "pytest-ruff>=0.1.1",
+    "pre-commit>=3.5.0",
+    "ruff>=0.4.1",
+    "pytest-asyncio>=0.21.1",
+    "pytest-cov>=4.1.0",
+]
+
 [tool.pytest.ini_options]
 addopts = "--doctest-glob README.md --ruff --cov didcomm_messaging"
 
 [tool.ruff]
+line-length = 90
+extend-exclude = [
+    "example*.py",
+]
+
+[tool.ruff.lint]
 select = [
     "E",
     "F",
     "C",
     "D",
     "TID",
 ]
@@ -58,37 +74,22 @@
     "D406",
     "D407",
     "D408",
     "D409",
     "D413",
     "D202",
 ]
-line-length = 90
-extend-exclude = [
-    "example*.py",
-]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/{tests}/*" = [
     "F841",
     "D",
     "E501",
 ]
 
-[tool.pdm.dev-dependencies]
-dev = [
-    "pytest>=7.4.3",
-    "pytest-ruff>=0.1.1",
-    "pre-commit>=3.5.0",
-    "black>=23.10.1",
-    "ruff>=0.1.3",
-    "pytest-asyncio>=0.21.1",
-    "pytest-cov>=4.1.0",
-]
-
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract",
 ]
 precision = 2
 show_missing = true
```

### Comparing `didcomm_messaging-0.1.0a4/tests/crypto/test_askar.py` & `didcomm_messaging-0.1.1a0/tests/crypto/test_askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/tests/crypto/test_askar_x_authlib.py` & `didcomm_messaging-0.1.1a0/tests/crypto/test_askar_x_authlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test compabibility between Askar and Authlib."""
+
 import json
 from aries_askar import Key, KeyAlg
 from authlib.jose import OKPKey
 import pytest
 
 from didcomm_messaging.crypto.backend.askar import (
     AskarCryptoService,
@@ -38,16 +39,17 @@
 @pytest.fixture
 def bob_authlib_key(bob_askar_key: Key):
     yield OKPKey.import_key(json.loads(bob_askar_key.get_jwk_secret()))
 
 
 @pytest.fixture
 def alice(alice_askar_key: Key, alice_authlib_key: OKPKey):
-    yield AskarSecretKey(alice_askar_key, ALICE_KID), AuthlibKey(
-        alice_authlib_key, ALICE_KID
+    yield (
+        AskarSecretKey(alice_askar_key, ALICE_KID),
+        AuthlibKey(alice_authlib_key, ALICE_KID),
     )
 
 
 @pytest.fixture
 def bob(bob_askar_key: Key, bob_authlib_key: OKPKey):
     yield AuthlibSecretKey(bob_authlib_key, BOB_KID), AskarKey(bob_askar_key, BOB_KID)
```

### Comparing `didcomm_messaging-0.1.0a4/tests/crypto/test_authlib.py` & `didcomm_messaging-0.1.1a0/tests/crypto/test_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/tests/test_didresolver.py` & `didcomm_messaging-0.1.1a0/tests/test_didresolver.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/tests/test_packaging.py` & `didcomm_messaging-0.1.1a0/tests/test_packaging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Test PackagingService."""
+
 import pytest
 
 from aries_askar import Key, KeyAlg
 from didcomm_messaging.crypto.backend.askar import AskarCryptoService, AskarSecretKey
 from didcomm_messaging.crypto.backend.basic import InMemorySecretsManager
+from didcomm_messaging.crypto.base import CryptoService
 from didcomm_messaging.packaging import PackagingService
 from didcomm_messaging.multiformats import multibase
 from didcomm_messaging.multiformats import multicodec
 from didcomm_messaging.resolver.peer import Peer2, Peer4
-from didcomm_messaging.resolver import PrefixResolver
+from didcomm_messaging.resolver import DIDResolver, PrefixResolver
 from did_peer_2 import KeySpec, generate
 
 
 @pytest.fixture
 def secrets():
     """Fixture for secrets."""
     yield InMemorySecretsManager()
@@ -21,25 +23,30 @@
 @pytest.fixture
 def crypto():
     """Fixture for crypto."""
     yield AskarCryptoService()
 
 
 @pytest.fixture
-def packaging(secrets, crypto):
+def resolver():
+    yield PrefixResolver({"did:peer:2": Peer2(), "did:peer:4": Peer4()})
+
+
+@pytest.fixture
+def packaging():
     """Fixture for packaging."""
-    yield PackagingService(
-        PrefixResolver({"did:peer:2": Peer2(), "did:peer:4": Peer4()}), crypto, secrets
-    )
+    yield PackagingService()
 
 
 # TODO More thorough tests
 @pytest.mark.asyncio
 async def test_packer_basic(
+    crypto: CryptoService,
     secrets: InMemorySecretsManager,
+    resolver: DIDResolver,
     packaging: PackagingService,
 ):
     """Test basic packaging.
 
     This is a happy path test.
     """
     verkey = Key.generate(KeyAlg.ED25519)
@@ -59,10 +66,10 @@
             ),
         ],
         [],
     )
     await secrets.add_secret(AskarSecretKey(verkey, f"{did}#key-1"))
     await secrets.add_secret(AskarSecretKey(xkey, f"{did}#key-2"))
     message = b"hello world"
-    packed = await packaging.pack(message, [did], did)
-    unpacked, meta = await packaging.unpack(packed)
+    packed = await packaging.pack(crypto, resolver, secrets, message, [did], did)
+    unpacked, meta = await packaging.unpack(crypto, resolver, secrets, packed)
     assert unpacked == message
```

### Comparing `didcomm_messaging-0.1.0a4/tests/test_secrets.py` & `didcomm_messaging-0.1.1a0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a4/PKG-INFO` & `didcomm_messaging-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: didcomm-messaging
-Version: 0.1.0a4
+Version: 0.1.1a0
 Summary: DIDComm Messaging implemented with swappable backends.
 Author-Email: Daniel Bluhm <dbluhm@pm.me>, Colton Wolkins <colton@indicio.tech>, Micah Peltier <micah@indicio.tech>
 License: Apache-2.0
 Requires-Python: >=3.9
 Requires-Dist: base58>=2.1.1
 Requires-Dist: pydid>=0.4.2
 Requires-Dist: aries-askar>=0.2.9; extra == "askar"
 Requires-Dist: did-peer-2>=0.1.2; extra == "did-peer"
 Requires-Dist: did-peer-4>=0.1.2; extra == "did-peer"
 Requires-Dist: authlib>=1.2.1; extra == "authlib"
 Requires-Dist: pycryptodomex>=3.19.0; extra == "authlib"
 Provides-Extra: askar
-Provides-Extra: did_peer
+Provides-Extra: did-peer
 Provides-Extra: authlib
 Description-Content-Type: text/markdown
 
 # didcomm-messaging-python
 
 This is a minimal but flexible implementation of [DIDComm Messaging](https://identity.foundation/didcomm-messaging/spec/v2.1/). To learn more about DIDComm Messaging, check out the spec or visit [didcomm.org](https://didcomm.org) to learn about DIDComm Messaging protocols defined by the community.
```

