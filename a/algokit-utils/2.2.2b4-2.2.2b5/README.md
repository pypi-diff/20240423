# Comparing `tmp/algokit_utils-2.2.2b4-py3-none-any.whl.zip` & `tmp/algokit_utils-2.2.2b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 46585 bytes, number of entries: 20
+Zip file size: 46801 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     4963 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx    10732 b- defN 80-Jan-01 00:00 algokit_utils/_debugging.py
 -rw-r--r--  2.0 unx     6786 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     5947 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    58661 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    59092 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx     7216 b- defN 80-Jan-01 00:00 algokit_utils/asset.py
 -rw-r--r--  2.0 unx      812 b- defN 80-Jan-01 00:00 algokit_utils/common.py
 -rw-r--r--  2.0 unx     4279 b- defN 80-Jan-01 00:00 algokit_utils/config.py
--rw-r--r--  2.0 unx    34668 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    35110 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     5584 b- defN 80-Jan-01 00:00 algokit_utils/dispenser_api.py
 -rw-r--r--  2.0 unx     2617 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     8238 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx    12803 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     5313 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1673 b- defN 16-Jan-01 00:00 algokit_utils-2.2.2b4.dist-info/RECORD
-20 files, 175690 bytes uncompressed, 43863 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1674 b- defN 16-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/RECORD
+20 files, 181129 bytes uncompressed, 44079 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-2.2.2b4.dist-info/LICENSE
+Filename: algokit_utils-2.2.2b5.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-2.2.2b4.dist-info/METADATA
+Filename: algokit_utils-2.2.2b5.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-2.2.2b4.dist-info/WHEEL
+Filename: algokit_utils-2.2.2b5.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-2.2.2b4.dist-info/RECORD
+Filename: algokit_utils-2.2.2b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -1,9 +1,10 @@
 import base64
 import copy
+import dataclasses
 import json
 import logging
 import re
 import typing
 from math import ceil
 from pathlib import Path
 from typing import Any, Literal, cast, overload
@@ -54,15 +55,14 @@
     TransactionResponse,
 )
 
 if typing.TYPE_CHECKING:
     from algosdk.v2client.algod import AlgodClient
     from algosdk.v2client.indexer import IndexerClient
 
-
 logger = logging.getLogger(__name__)
 
 
 """A dictionary `dict[str, Any]` representing ABI argument names and values"""
 
 __all__ = [
     "ApplicationClient",
@@ -371,28 +371,28 @@
         /,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: CreateCallParameters | CreateCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with application id == 0 and the schema and source of client's app_spec to atc"""
         approval_program, clear_program = self._check_is_compiled()
-        transaction_parameters = _convert_transaction_parameters(transaction_parameters)
+        transaction_parameters = _convert_transaction_parameters(CreateCallParameters, transaction_parameters)
 
         extra_pages = transaction_parameters.extra_pages or num_extra_program_pages(
             approval_program.raw_binary, clear_program.raw_binary
         )
 
         self.add_method_call(
             atc,
             app_id=0,
             abi_method=call_abi_method,
             abi_args=abi_kwargs,
             on_complete=transaction_parameters.on_complete or transaction.OnComplete.NoOpOC,
             call_config=au_spec.CallConfig.CREATE,
-            parameters=transaction_parameters,
+            parameters=_convert_transaction_parameters(TransactionParameters, transaction_parameters),
             approval_program=approval_program.raw_binary,
             clear_program=clear_program.raw_binary,
             global_schema=self.app_spec.global_state_schema,
             local_schema=self.app_spec.local_state_schema,
             extra_pages=extra_pages,
         )
 
@@ -563,20 +563,20 @@
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: OnCompleteCallParameters | OnCompleteCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with specified parameters to atc"""
-        _parameters = _convert_transaction_parameters(transaction_parameters)
+        _parameters = _convert_transaction_parameters(OnCompleteCallParameters, transaction_parameters)
         self.add_method_call(
             atc,
             abi_method=call_abi_method,
             abi_args=abi_kwargs,
-            parameters=_parameters,
+            parameters=_convert_transaction_parameters(TransactionParameters, transaction_parameters),
             on_complete=_parameters.on_complete or transaction.OnComplete.NoOpOC,
         )
 
     @overload
     def call(
         self,
         call_abi_method: ABIMethod | Literal[True],
@@ -603,15 +603,15 @@
         self,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: OnCompleteCallParameters | OnCompleteCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with specified parameters"""
         atc = AtomicTransactionComposer()
-        _parameters = _convert_transaction_parameters(transaction_parameters)
+        _parameters = _convert_transaction_parameters(OnCompleteCallParameters, transaction_parameters)
         self.compose_call(
             atc,
             call_abi_method=call_abi_method,
             transaction_parameters=_parameters,
             **abi_kwargs,
         )
 
@@ -999,15 +999,15 @@
         app_args: list[bytes] | None = None,
         call_config: au_spec.CallConfig = au_spec.CallConfig.CALL,
     ) -> None:
         """Adds a transaction to the AtomicTransactionComposer passed"""
         if app_id is None:
             self._load_reference_and_check_app_id()
             app_id = self.app_id
-        parameters = _convert_transaction_parameters(parameters)
+        parameters = _convert_transaction_parameters(TransactionParameters, parameters)
         method = self._resolve_method(abi_method, abi_args, on_complete, call_config)
         sp = parameters.suggested_params or self.suggested_params or self.algod_client.suggested_params()
         signer, sender = self.resolve_signer_sender(parameters.signer, parameters.sender)
         if parameters.boxes is not None:
             # TODO: algosdk actually does this, but it's type hints say otherwise...
             encoded_boxes = [(id_, algosdk.encoding.encode_as_bytes(name)) for id_, name in parameters.boxes]
         else:
@@ -1313,19 +1313,26 @@
                     "failure-message": failure_message,
                     "exec-trace": exec_trace,
                 }
             )
     return traces
 
 
+_TParams = typing.TypeVar("_TParams", TransactionParameters, OnCompleteCallParameters, CreateCallParameters)
+
+
 def _convert_transaction_parameters(
-    args: TransactionParameters | TransactionParametersDict | None,
-) -> CreateCallParameters:
-    _args = args.__dict__ if isinstance(args, TransactionParameters) else (args or {})
-    return CreateCallParameters(**_args)
+    cls: type[_TParams],
+    args: object | None,
+) -> _TParams:
+    if args is None:
+        return cls()
+    args_dict = args.__dict__ if not isinstance(args, dict) else (args or {})
+    _args = {f.name: args_dict[f.name] for f in dataclasses.fields(cls) if f.name in args_dict}
+    return cls(**_args)
 
 
 def get_sender_from_signer(signer: TransactionSigner | None) -> str | None:
     """Returns the associated address of a signer, return None if no address found"""
 
     if isinstance(signer, AccountTransactionSigner):
         sender = address_from_private_key(signer.private_key)  # type: ignore[no-untyped-call]
```

## algokit_utils/deploy.py

```diff
@@ -19,14 +19,15 @@
     OnCompleteActionName,
 )
 from algokit_utils.models import (
     ABIArgsDict,
     ABIMethod,
     Account,
     CreateCallParameters,
+    TransactionParameters,
     TransactionResponse,
 )
 
 if TYPE_CHECKING:
     from algosdk.v2client.algod import AlgodClient
     from algosdk.v2client.indexer import IndexerClient
 
@@ -720,15 +721,15 @@
                     "Cannot determine if App is updatable and on_update=UpdateApp, will attempt to update app"
                 )
             return self._update_app()
 
     def _create_app(self) -> DeployResponse:
         assert self.app_client.existing_deployments
 
-        method, abi_args, parameters = _convert_deploy_args(
+        method, abi_args, parameters = _convert_create_deploy_args(
             self.create_args, self.new_app_metadata, self.signer, self.sender
         )
         create_response = self.app_client.create(
             method,
             parameters,
             **abi_args,
         )
@@ -747,15 +748,15 @@
 
         logger.info(
             f"Replacing {self.existing_app_metadata_or_reference.name} "
             f"({self.existing_app_metadata_or_reference.version}) with "
             f"{self.new_app_metadata.name} ({self.new_app_metadata.version}) in {self.creator} account."
         )
         atc = AtomicTransactionComposer()
-        create_method, create_abi_args, create_parameters = _convert_deploy_args(
+        create_method, create_abi_args, create_parameters = _convert_create_deploy_args(
             self.create_args, self.new_app_metadata, self.signer, self.sender
         )
         self.app_client.compose_create(
             atc,
             create_method,
             create_parameters,
             **create_abi_args,
@@ -846,34 +847,47 @@
 
 
 def _convert_deploy_args(
     _args: DeployCallArgs | DeployCallArgsDict | None,
     note: AppDeployMetaData,
     signer: TransactionSigner | None,
     sender: str | None,
-) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
+) -> tuple[ABIMethod | bool | None, ABIArgsDict, TransactionParameters]:
     args = _args.__dict__ if isinstance(_args, DeployCallArgs) else (_args or {})
 
-    # return most derived type, unused parameters are ignored
-    parameters = CreateCallParameters(
+    parameters = TransactionParameters(
         note=note.encode(),
         signer=signer,
         sender=sender,
         suggested_params=args.get("suggested_params"),
         lease=args.get("lease"),
         accounts=args.get("accounts"),
         foreign_assets=args.get("foreign_assets"),
         foreign_apps=args.get("foreign_apps"),
         boxes=args.get("boxes"),
         rekey_to=args.get("rekey_to"),
+    )
+
+    return args.get("method"), args.get("args") or {}, parameters
+
+
+def _convert_create_deploy_args(
+    _args: DeployCallArgs | DeployCallArgsDict | None,
+    note: AppDeployMetaData,
+    signer: TransactionSigner | None,
+    sender: str | None,
+) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
+    method, args, parameters = _convert_deploy_args(_args, note, signer, sender)
+    create_parameters = CreateCallParameters(
+        **parameters.__dict__,
         extra_pages=args.get("extra_pages"),
         on_complete=args.get("on_complete"),
     )
 
-    return args.get("method"), args.get("args") or {}, parameters
+    return method, args, create_parameters
 
 
 def get_app_id_from_tx_id(algod_client: "AlgodClient", tx_id: str) -> int:
     """Finds the app_id for provided transaction id"""
     result = algod_client.pending_transaction_info(tx_id)
     assert isinstance(result, dict)
     app_id = result["application-index"]
```

## algokit_utils/models.py

```diff
@@ -151,33 +151,94 @@
     """List of foreign assets (by asset id) to include in transaction"""
     rekey_to: str | None = None
     """Address to rekey to"""
 
 
 # CreateTransactionParameters is used by algokit-client-generator clients
 @dataclasses.dataclass(kw_only=True)
-class CreateTransactionParameters(TransactionParameters):
+class CreateTransactionParameters:
     """Additional parameters that can be included in a transaction when calling a create method"""
 
+    signer: TransactionSigner | None = None
+    """Signer to use when signing this transaction"""
+    sender: str | None = None
+    """Sender of this transaction"""
+    suggested_params: transaction.SuggestedParams | None = None
+    """SuggestedParams to use for this transaction"""
+    note: bytes | str | None = None
+    """Note for this transaction"""
+    lease: bytes | str | None = None
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
+    accounts: list[str] | None = None
+    """Accounts to include in transaction"""
+    foreign_apps: list[int] | None = None
+    """List of foreign apps (by app id) to include in transaction"""
+    foreign_assets: list[int] | None = None
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str | None = None
+    """Address to rekey to"""
     extra_pages: int | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
-class OnCompleteCallParameters(TransactionParameters):
+class OnCompleteCallParameters:
     """Additional parameters that can be included in a transaction when using the
     ApplicationClient.call/compose_call methods"""
 
+    signer: TransactionSigner | None = None
+    """Signer to use when signing this transaction"""
+    sender: str | None = None
+    """Sender of this transaction"""
+    suggested_params: transaction.SuggestedParams | None = None
+    """SuggestedParams to use for this transaction"""
+    note: bytes | str | None = None
+    """Note for this transaction"""
+    lease: bytes | str | None = None
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
+    accounts: list[str] | None = None
+    """Accounts to include in transaction"""
+    foreign_apps: list[int] | None = None
+    """List of foreign apps (by app id) to include in transaction"""
+    foreign_assets: list[int] | None = None
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str | None = None
+    """Address to rekey to"""
     on_complete: transaction.OnComplete | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
-class CreateCallParameters(OnCompleteCallParameters):
+class CreateCallParameters:
     """Additional parameters that can be included in a transaction when using the
     ApplicationClient.create/compose_create methods"""
 
+    signer: TransactionSigner | None = None
+    """Signer to use when signing this transaction"""
+    sender: str | None = None
+    """Sender of this transaction"""
+    suggested_params: transaction.SuggestedParams | None = None
+    """SuggestedParams to use for this transaction"""
+    note: bytes | str | None = None
+    """Note for this transaction"""
+    lease: bytes | str | None = None
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
+    accounts: list[str] | None = None
+    """Accounts to include in transaction"""
+    foreign_apps: list[int] | None = None
+    """List of foreign apps (by app id) to include in transaction"""
+    foreign_assets: list[int] | None = None
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str | None = None
+    """Address to rekey to"""
+    on_complete: transaction.OnComplete | None = None
     extra_pages: int | None = None
 
 
 class TransactionParametersDict(TypedDict, total=False):
     """Additional parameters that can be included in a transaction"""
 
     signer: TransactionSigner
@@ -198,25 +259,66 @@
     """List of foreign apps (by app id) to include in transaction"""
     foreign_assets: list[int]
     """List of foreign assets (by asset id) to include in transaction"""
     rekey_to: str
     """Address to rekey to"""
 
 
-class OnCompleteCallParametersDict(TypedDict, TransactionParametersDict, total=False):
+class OnCompleteCallParametersDict(TypedDict, total=False):
     """Additional parameters that can be included in a transaction when using the
     ApplicationClient.call/compose_call methods"""
 
+    signer: TransactionSigner
+    """Signer to use when signing this transaction"""
+    sender: str
+    """Sender of this transaction"""
+    suggested_params: transaction.SuggestedParams
+    """SuggestedParams to use for this transaction"""
+    note: bytes | str
+    """Note for this transaction"""
+    lease: bytes | str
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
+    accounts: list[str]
+    """Accounts to include in transaction"""
+    foreign_apps: list[int]
+    """List of foreign apps (by app id) to include in transaction"""
+    foreign_assets: list[int]
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str
+    """Address to rekey to"""
     on_complete: transaction.OnComplete
 
 
-class CreateCallParametersDict(TypedDict, OnCompleteCallParametersDict, total=False):
+class CreateCallParametersDict(TypedDict, total=False):
     """Additional parameters that can be included in a transaction when using the
     ApplicationClient.create/compose_create methods"""
 
+    signer: TransactionSigner
+    """Signer to use when signing this transaction"""
+    sender: str
+    """Sender of this transaction"""
+    suggested_params: transaction.SuggestedParams
+    """SuggestedParams to use for this transaction"""
+    note: bytes | str
+    """Note for this transaction"""
+    lease: bytes | str
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
+    accounts: list[str]
+    """Accounts to include in transaction"""
+    foreign_apps: list[int]
+    """List of foreign apps (by app id) to include in transaction"""
+    foreign_assets: list[int]
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str
+    """Address to rekey to"""
+    on_complete: transaction.OnComplete
     extra_pages: int
 
 
 # Pre 1.3.1 backwards compatibility
 @deprecated(reason="Use TransactionParameters instead", version="1.3.1")
 class RawTransactionParameters(TransactionParameters):
     """Deprecated, use TransactionParameters instead"""
```

## Comparing `algokit_utils-2.2.2b4.dist-info/LICENSE` & `algokit_utils-2.2.2b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-2.2.2b4.dist-info/METADATA` & `algokit_utils-2.2.2b5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 2.2.2b4
+Version: 2.2.2b5
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-2.2.2b4.dist-info/RECORD` & `algokit_utils-2.2.2b5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 algokit_utils/__init__.py,sha256=yeufbE_5wjRILZs_10UD5B3_sjdwAfPXskdFKskzXhg,4963
 algokit_utils/_debugging.py,sha256=4UC5NZGqxF32y742TUB34rX9kWaObXCCPOs-lbkQjGQ,10732
 algokit_utils/_ensure_funded.py,sha256=ZdEdUB43QGIQrg7cSSgNrDmWaLSUhli9x9I6juwKfgo,6786
 algokit_utils/_transfer.py,sha256=CyXGOR_Zy-2crQhk-78uUbB8Sj_ZeTzxPwOAHU7wwno,5947
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=xOZJ8i3y8wDJL0Uvaw1o-UmJKvSmbv8ib5RwGl4ar0w,58661
+algokit_utils/application_client.py,sha256=qylA2aI4Ecs532bIs6fyc6FgLnWey9PBzZBZW_jnYtk,59092
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/asset.py,sha256=jsc7T1dH9HZA3Yve2gRLObwUlK6xLDoQz0NxLLnqaGs,7216
 algokit_utils/common.py,sha256=K6-3_9dv2clDn0WMYb8AWE_N46kWWIXglZIPfHIowDs,812
 algokit_utils/config.py,sha256=oY3o1kPzVPRiQH--f4HzrMMNPojT078CSudqS9WQaEc,4279
-algokit_utils/deploy.py,sha256=ydE3QSq1lRkjXQC9zdFclywx8q1UgV9l-l3Mx-shbHg,34668
+algokit_utils/deploy.py,sha256=BxIFPtZd1lO8o_JmQQDIKk0O93E_bE-ZzglEWXwbefw,35110
 algokit_utils/dispenser_api.py,sha256=BpwEhKDig6qz54wbO-htG8hmLxFIrvdzXpESUb7Y1zw,5584
 algokit_utils/logic_error.py,sha256=YeE70qHZ6WBeoKCXqnto3uBg8R4ODXiNZkLmfEmASQo,2617
-algokit_utils/models.py,sha256=GWpZQ2bTGfkldM12VZntGlVJTFBTtWf5SM7ZYXC_LHE,8238
+algokit_utils/models.py,sha256=iJUiV6eLq5N_FKki4X5ll5rYQslU_wSPiSTtl61Z1CI,12803
 algokit_utils/network_clients.py,sha256=sj5y_g5uclddWCEyUCptA-KjWuAtLV06hZH4QIGM1yE,5313
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-2.2.2b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-2.2.2b4.dist-info/METADATA,sha256=ljuQvwihRxkVXBUYrOfYDY7t3IKXOQBOlYK-DWS_3ko,2207
-algokit_utils-2.2.2b4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-algokit_utils-2.2.2b4.dist-info/RECORD,,
+algokit_utils-2.2.2b5.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-2.2.2b5.dist-info/METADATA,sha256=8mkuN9VkBEa_Z2oH1GmzccM-SH63NFZmlBsXxc5CHQ4,2207
+algokit_utils-2.2.2b5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+algokit_utils-2.2.2b5.dist-info/RECORD,,
```

