# Comparing `tmp/strledger-0.5.1.tar.gz` & `tmp/strledger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strledger-0.5.1.tar", max compression
+gzip compressed data, was "strledger-0.6.0.tar", max compression
```

## Comparing `strledger-0.5.1.tar` & `strledger-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-11-28 02:22:56.502545 strledger-0.5.1/LICENSE
--rw-r--r--   0        0        0     1056 2023-11-28 02:22:56.502720 strledger-0.5.1/README.md
--rw-r--r--   0        0        0     1388 2023-11-28 02:27:18.648027 strledger-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-11-28 02:22:56.505393 strledger-0.5.1/strledger/__init__.py
--rw-r--r--   0        0        0     7517 2023-11-28 02:22:56.505638 strledger-0.5.1/strledger/cli.py
--rw-r--r--   0        0        0     5918 2023-11-28 02:22:56.505861 strledger-0.5.1/strledger/core.py
--rw-r--r--   0        0        0        0 2023-11-28 02:22:56.505903 strledger-0.5.1/strledger/py.typed
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 strledger-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-23 09:34:52.502306 strledger-0.6.0/README.md
+-rw-r--r--   0        0        0     1365 2024-04-23 09:46:49.514314 strledger-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-23 09:34:52.505392 strledger-0.6.0/strledger/__init__.py
+-rw-r--r--   0        0        0     9195 2024-04-23 09:34:52.505783 strledger-0.6.0/strledger/cli.py
+-rw-r--r--   0        0        0     7066 2024-04-23 09:34:52.505980 strledger-0.6.0/strledger/core.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.6.0/strledger/py.typed
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 strledger-0.6.0/PKG-INFO
```

### Comparing `strledger-0.5.1/LICENSE` & `strledger-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strledger-0.5.1/README.md` & `strledger-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 
 ## Cli Usage
 ```text
 Usage: strledger [OPTIONS] COMMAND [ARGS]...
 
   Stellar Ledger commands.
 
-  This project is built on the basis of ledgerctl, you can check ledgerctl for more features.
+  This project is built on the basis of ledgerctl, you can check ledgerctl for
+  more features.
 
 Options:
   -v, --verbose  Display exchanged APDU.
   --help         Show this message and exit.
 
 Commands:
-  app-info     Get Stellar app info.
-  get-address  Get Stellar public address.
-  sign-tx      Sign a base64-encoded transaction envelope.
-  version      Get strledger version info.
+  app-info      Get Stellar app info.
+  get-address   Get Stellar public address.
+  sign-auth     Sign a base64-encoded soroban authorization...
+  sign-tx       Sign a base64-encoded transaction envelope.
+  sign-tx-hash  Sign a hex encoded transaction hash.
+  version       Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
 from strledger import get_default_client
```

### Comparing `strledger-0.5.1/pyproject.toml` & `strledger-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strledger"
-version = "0.5.1"
+version = "0.6.0"
 description = "Sign Stellar Transaction with Ledger on the command line."
 authors = ["overcat <4catcode@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/overcat/strledger"
 repository = "https://github.com/overcat/strledger"
 documentation = "https://github.com/overcat/strledger"
@@ -19,25 +19,25 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Typing :: Typed"
+    "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/overcat/strledger/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-click = "^8.0.1"
-stellar-sdk = { version = ">=8,<10", allow-prereleases = true}
-ledgerwallet = "^0.1.3"
+click = "^8.1.7"
+stellar-sdk = { version = ">=9,<10" }
+ledgerwallet = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-strledger = "strledger.cli:cli"
+strledger = "strledger.cli:cli"
```

### Comparing `strledger-0.5.1/strledger/cli.py` & `strledger-0.6.0/strledger/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 from stellar_sdk import (
     Network,
     parse_transaction_envelope_from_xdr,
     Server,
     TransactionEnvelope,
     FeeBumpTransactionEnvelope,
 )
+from stellar_sdk.xdr import HashIDPreimage
 from stellar_sdk.exceptions import BaseRequestError
 from stellar_sdk import __version__ as stellar_sdk_version
 from strledger import __issue__
 from strledger import __version__ as strledger_version
 from strledger.core import (
     SW,
     StrLedger,
     DEFAULT_KEYPAIR_INDEX,
     get_default_client,
     DeviceNotFoundException,
 )
+from stellar_sdk.utils import sha256
 
 _DEFAULT_HORIZON_SERVER_URL = "https://horizon.stellar.org"
 
 
 def echo_normal(message: str) -> None:
     click.echo(message)
 
@@ -235,14 +237,64 @@
             echo_error("The request to confirm the address was denied.")
             sys.exit(1)
         else:
             raise e
     echo_success(keypair.public_key)
 
 
+@cli.command(name="sign-auth")
+@click.option(
+    "-i",
+    "--keypair-index",
+    type=int,
+    required=False,
+    help="Keypair Index.",
+    default=DEFAULT_KEYPAIR_INDEX,
+    show_default=True,
+)
+@click.argument("soroban_authorization")
+@click.pass_obj
+def sign_soroban_authorization(
+    get_client: Callable[[], StrLedger],
+    keypair_index: int,
+    soroban_authorization: str,
+):
+    """Sign a base64-encoded soroban authorization (HashIDPreimage)."""
+    client = get_client()
+    try:
+        auth = HashIDPreimage.from_xdr(soroban_authorization)
+    except Exception:
+        echo_error(
+            "Failed to parse XDR.\n"
+            "Make sure to pass a valid base64-encoded soroban authorization."
+        )
+        sys.exit(1)
+
+    echo_normal(f"HashIDPreimage Hash: {sha256(auth.to_xdr_bytes()).hex()}")
+    echo_normal("Please confirm this transaction on Ledger.")
+
+    signature = None
+    try:
+        signature = client.sign_soroban_authorization(auth, keypair_index=keypair_index)
+        echo_success("Signed successfully.")
+        echo_success("Base64-encoded signature:")
+        echo_success(base64.b64encode(signature).decode())
+    except CommException as e:
+        if e.sw == SW.DENY:
+            echo_error("The request to sign the soroban auth was denied.")
+        elif e.sw == SW.UNKNOWN_ENVELOPE_TYPE:
+            echo_error(
+                "The transaction contains unsupported transaction envelope type."
+            )
+        else:
+            echo_error(f"Unknown exception, you can the problem here: {__issue__}")
+            raise
+        sys.exit(1)
+
+
 @cli.command(name="version")
 def version() -> None:
     """Get strledger version info."""
     echo_success(f"StrLedger Version: {strledger_version}")
     echo_success(f"Ledger Wallet Version: {ledger_wallet_version}")
     echo_success(f"Stellar SDK Version: {stellar_sdk_version}")
```

### Comparing `strledger-0.5.1/strledger/core.py` & `strledger-0.6.0/strledger/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ledgerwallet.transport import enumerate_devices
 from stellar_sdk import (
     Keypair,
     TransactionEnvelope,
     DecoratedSignature,
     FeeBumpTransactionEnvelope,
 )
+from stellar_sdk.xdr import HashIDPreimage, EnvelopeType
 
 __all__ = [
     "get_default_client",
     "DeviceNotFoundException",
     "DEFAULT_KEYPAIR_INDEX",
     "Ins",
     "P1",
@@ -28,14 +29,15 @@
 
 
 class Ins(IntEnum):
     GET_PK = 0x02
     SIGN_TX = 0x04
     GET_CONF = 0x06
     SIGN_TX_HASH = 0x08
+    SIGN_SOROBAN_AUTHORIZATION = 0x0A
 
 
 class P1(IntEnum):
     NONE = 0x00
     FIRST_APDU = 0x00
     MORE_APDU = 0x80
 
@@ -150,15 +152,15 @@
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> None:
         sign_data = transaction_envelope.signature_base()
         keypair = self.get_keypair(keypair_index=keypair_index)
 
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + sign_data
-        signature = self._send_payload(payload)
+        signature = self._send_payload(Ins.SIGN_TX, payload)
         assert isinstance(signature, bytes)
         decorated_signature = DecoratedSignature(keypair.signature_hint(), signature)
         transaction_envelope.signatures.append(decorated_signature)
 
     def sign_transaction_hash(
         self,
         transaction_hash: Union[str, bytes],
@@ -170,15 +172,38 @@
         payload = path + transaction_hash
 
         data = self.client.apdu_exchange(
             ins=Ins.SIGN_TX_HASH, data=payload, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
         )
         return data
 
-    def _send_payload(self, payload) -> Optional[Union[int, str]]:
+    def sign_soroban_authorization(
+        self,
+        soroban_authorization: Union[str, bytes, HashIDPreimage],
+        keypair_index: int = DEFAULT_KEYPAIR_INDEX,
+    ) -> bytes:
+        if isinstance(soroban_authorization, str):
+            soroban_authorization = HashIDPreimage.from_xdr(soroban_authorization)
+        if isinstance(soroban_authorization, bytes):
+            soroban_authorization = HashIDPreimage.from_xdr_bytes(soroban_authorization)
+
+        if (
+            soroban_authorization.type
+            != EnvelopeType.ENVELOPE_TYPE_SOROBAN_AUTHORIZATION
+        ):
+            raise ValueError(
+                f"Invalid type, expected {EnvelopeType.ENVELOPE_TYPE_SOROBAN_AUTHORIZATION}, but got {soroban_authorization.type}"
+            )
+        path = Bip32Path.build(f"44'/148'/{keypair_index}'")
+        payload = path + soroban_authorization.to_xdr_bytes()
+        signature = self._send_payload(Ins.SIGN_SOROBAN_AUTHORIZATION, payload)
+        assert isinstance(signature, bytes)
+        return signature
+
+    def _send_payload(self, ins: Ins, payload) -> Optional[Union[int, bytes]]:
         chunk_size = 255
         first = True
         while payload:
             if first:
                 p1 = P1.FIRST_APDU
                 first = False
             else:
@@ -186,11 +211,11 @@
 
             size = min(len(payload), chunk_size)
             if size != len(payload):
                 p2 = P2.MORE_APDU
             else:
                 p2 = P2.LAST_APDU
 
-            resp = self.client.apdu_exchange(Ins.SIGN_TX, payload[:size], p1, p2)
+            resp = self.client.apdu_exchange(ins, payload[:size], p1, p2)
             if resp:
                 return resp
             payload = payload[size:]
```

### Comparing `strledger-0.5.1/PKG-INFO` & `strledger-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strledger
-Version: 0.5.1
+Version: 0.6.0
 Summary: Sign Stellar Transaction with Ledger on the command line.
 Home-page: https://github.com/overcat/strledger
 License: MIT
 Keywords: stellar,ledger
 Author: overcat
 Author-email: 4catcode@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Typing :: Typed
-Requires-Dist: click (>=8.0.1,<9.0.0)
-Requires-Dist: ledgerwallet (>=0.1.3,<0.2.0)
-Requires-Dist: stellar-sdk (>=8,<10)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: ledgerwallet (>=0.4.0,<0.5.0)
+Requires-Dist: stellar-sdk (>=9,<10)
 Project-URL: Bug Tracker, https://github.com/overcat/strledger/issues
 Project-URL: Documentation, https://github.com/overcat/strledger
 Project-URL: Repository, https://github.com/overcat/strledger
 Description-Content-Type: text/markdown
 
 # strledger - Sign Stellar Transaction with Ledger on the command line.
 
@@ -42,25 +42,28 @@
 
 ## Cli Usage
 ```text
 Usage: strledger [OPTIONS] COMMAND [ARGS]...
 
   Stellar Ledger commands.
 
-  This project is built on the basis of ledgerctl, you can check ledgerctl for more features.
+  This project is built on the basis of ledgerctl, you can check ledgerctl for
+  more features.
 
 Options:
   -v, --verbose  Display exchanged APDU.
   --help         Show this message and exit.
 
 Commands:
-  app-info     Get Stellar app info.
-  get-address  Get Stellar public address.
-  sign-tx      Sign a base64-encoded transaction envelope.
-  version      Get strledger version info.
+  app-info      Get Stellar app info.
+  get-address   Get Stellar public address.
+  sign-auth     Sign a base64-encoded soroban authorization...
+  sign-tx       Sign a base64-encoded transaction envelope.
+  sign-tx-hash  Sign a hex encoded transaction hash.
+  version       Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
 from strledger import get_default_client
```

