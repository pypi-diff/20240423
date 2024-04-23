# Comparing `tmp/bxsolana_trader-2.0.1.tar.gz` & `tmp/bxsolana-trader-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana_trader-2.0.1.tar", last modified: Tue Apr 23 20:05:04 2024, max compression
+gzip compressed data, was "bxsolana-trader-2.1.0.tar", last modified: Mon Mar 18 18:52:17 2024, max compression
```

## Comparing `bxsolana_trader-2.0.1.tar` & `bxsolana-trader-2.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.360295 bxsolana_trader-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-04-23 20:05:04.360295 bxsolana_trader-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.344296 bxsolana_trader-2.0.1/bxsolana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.348296 bxsolana_trader-2.0.1/bxsolana/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      670 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      718 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/order_lifecycle.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9198 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/order_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14230 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/request_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5286 2024-04-23 19:32:57.000000 bxsolana_trader-2.0.1/bxsolana/examples/stream_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5194 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/examples/transaction_request_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.352295 bxsolana_trader-2.0.1/bxsolana/provider/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-04-23 19:58:33.000000 bxsolana_trader-2.0.1/bxsolana/provider/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1290 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2809 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/grpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32770 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/http_error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/jsonrpc_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/package_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4955 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/provider/ws.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.352295 bxsolana_trader-2.0.1/bxsolana/transaction/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/transaction/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/transaction/memo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/transaction/private_txs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2402 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/bxsolana/transaction/signing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.360295 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-04-23 20:05:04.000000 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2024-04-23 20:05:04.000000 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-23 20:05:04.000000 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2024-04-23 20:05:04.000000 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-23 20:05:04.000000 bxsolana_trader-2.0.1/bxsolana_trader.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      677 2024-04-23 20:05:04.360295 bxsolana_trader-2.0.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.356295 bxsolana_trader-2.0.1/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.356295 bxsolana_trader-2.0.1/test/integration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/private.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/public.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      852 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/test_grpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/test_http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      664 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/integration/test_ws.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.356295 bxsolana_trader-2.0.1/test/unit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/unit/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 20:05:04.360295 bxsolana_trader-2.0.1/test/unit/transaction/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/unit/transaction/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      834 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/unit/transaction/test_memo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4629 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.1/test/unit/transaction/test_signing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/examples/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      670 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      718 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/order_lifecycle.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9198 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/order_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14230 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/request_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4603 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/stream_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5194 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/transaction_request_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/provider/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1290 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2809 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/grpc.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32775 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/http.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/http_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/jsonrpc_patch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/package_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4955 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/ws.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/transaction/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      535 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/memo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/private_txs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2402 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/signing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      145 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      677 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/integration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/private.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/public.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      852 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/stream.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      701 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_grpc.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_http.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      664 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_ws.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/unit/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/unit/transaction/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      834 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/test_memo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4629 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/test_signing.py
```

### Comparing `bxsolana_trader-2.0.1/LICENSE` & `bxsolana-trader-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/PKG-INFO` & `bxsolana-trader-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: aiohttp==3.8.1
 Requires-Dist: grpclib==0.4.3
 Requires-Dist: aiounittest==1.4.1
 Requires-Dist: base58==2.1.1
 Requires-Dist: solana==0.31.0
 Requires-Dist: solders==0.19.0
 Requires-Dist: bx-jsonrpc-py==0.2.0
-Requires-Dist: bxsolana-trader-proto==0.0.65
+Requires-Dist: bxsolana-trader-proto==0.0.63
 
 # Solana Trader Python Client
 
 Provides a Python SDK for bloXroute's Solana Trader API.
 
 ## Installation
```

### Comparing `bxsolana_trader-2.0.1/README.md` & `bxsolana-trader-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/constants.py` & `bxsolana-trader-2.1.0/bxsolana/examples/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/order_lifecycle.py` & `bxsolana-trader-2.1.0/bxsolana/examples/order_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/order_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/order_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/request_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/request_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/stream_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/stream_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 from bxsolana_trader_proto import api as proto
 from .. import provider
 
 
 async def do_stream(api: provider.Provider, run_slow: bool = False):
     item_count = 0
-    print("streaming market depth updates...")
-    async for response in api.get_market_depths_stream(
-        get_market_depths_request=proto.GetMarketDepthsRequest(
-            markets=["SOLUSDC"], limit=10, project=proto.Project.P_OPENBOOK
-        )
-    ):
-        print(response.to_json())
-        item_count += 1
-        if item_count == 1:
-            item_count = 0
-            break
-
-    print("streaming orderbook updates...")
-    async for response in api.get_orderbooks_stream(
-        get_orderbooks_request=proto.GetOrderbooksRequest(
-            markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
-        )
-    ):
-        print(response.to_json())
-        item_count += 1
-        if item_count == 1:
-            item_count = 0
-            break
+
+    if run_slow:
+        print("streaming orderbook updates...")
+        async for response in api.get_orderbooks_stream(
+            get_orderbooks_request=proto.GetOrderbooksRequest(
+                markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
+            )
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 1:
+                item_count = 0
+                break
 
     if run_slow:
         print("streaming ticker updates...")
         async for response in api.get_tickers_stream(
             get_tickers_stream_request=proto.GetTickersStreamRequest(
                 markets=[
                     "BONK/SOL",
@@ -138,19 +128,7 @@
             get_priority_fee_request=proto.GetPriorityFeeRequest()
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
-
-    if run_slow:
-        print("streaming bundle tip updates...")
-        async for response in api.get_bundle_tip_stream(
-            get_bundle_tip_request=proto.GetBundleResultRequest()
-        ):
-            print(response.to_json())
-            item_count += 1
-            if item_count == 1:
-                item_count = 0
-                break
-
```

### Comparing `bxsolana_trader-2.0.1/bxsolana/examples/transaction_request_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/transaction_request_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/base.py` & `bxsolana-trader-2.1.0/bxsolana/provider/base.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/constants.py` & `bxsolana-trader-2.1.0/bxsolana/provider/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/grpc.py` & `bxsolana-trader-2.1.0/bxsolana/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/http.py` & `bxsolana-trader-2.1.0/bxsolana/provider/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
         get_account_balance_request: proto.GetAccountBalanceRequest,
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> proto.GetAccountBalanceResponse:
         async with self._session.get(
-            f"{self._endpoint_v2}/balance?ownerAddress={get_account_balance_request.owner_address}"
+            f"{self._endpoint}/account/balance?ownerAddress={get_account_balance_request.owner_address}"
         ) as res:
             return await map_response(res, proto.GetAccountBalanceResponse())
 
     async def get_token_accounts(
         self,
         get_token_accounts_request: proto.GetTokenAccountsRequest,
         *,
```

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/http_error.py` & `bxsolana-trader-2.1.0/bxsolana/provider/http_error.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/jsonrpc_patch.py` & `bxsolana-trader-2.1.0/bxsolana/provider/jsonrpc_patch.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/provider/ws.py` & `bxsolana-trader-2.1.0/bxsolana/provider/ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/transaction/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/transaction/memo.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/transaction/private_txs.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/private_txs.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana/transaction/signing.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/signing.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/bxsolana_trader.egg-info/PKG-INFO` & `bxsolana-trader-2.1.0/bxsolana_trader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: aiohttp==3.8.1
 Requires-Dist: grpclib==0.4.3
 Requires-Dist: aiounittest==1.4.1
 Requires-Dist: base58==2.1.1
 Requires-Dist: solana==0.31.0
 Requires-Dist: solders==0.19.0
 Requires-Dist: bx-jsonrpc-py==0.2.0
-Requires-Dist: bxsolana-trader-proto==0.0.65
+Requires-Dist: bxsolana-trader-proto==0.0.63
 
 # Solana Trader Python Client
 
 Provides a Python SDK for bloXroute's Solana Trader API.
 
 ## Installation
```

### Comparing `bxsolana_trader-2.0.1/bxsolana_trader.egg-info/SOURCES.txt` & `bxsolana-trader-2.1.0/bxsolana_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/setup.cfg` & `bxsolana-trader-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bxsolana-trader
-version = 2.0.1
+version = 2.1.0
 description = Python SDK for bloXroute's Solana Trader API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = bloXroute Labs
 author_email = support@bloxroute.com
 url = https://github.com/bloXroute-Labs/solana-trader-client-python
 keywords = serum, solana, blockchain, trader, grpc, stream
@@ -16,13 +16,13 @@
 	aiohttp==3.8.1
 	grpclib==0.4.3
 	aiounittest==1.4.1
 	base58==2.1.1
 	solana==0.31.0
 	solders==0.19.0
 	bx-jsonrpc-py==0.2.0
-	bxsolana-trader-proto==0.0.65
+	bxsolana-trader-proto==0.0.63
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bxsolana_trader-2.0.1/test/integration/private.py` & `bxsolana-trader-2.1.0/test/integration/private.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/integration/public.py` & `bxsolana-trader-2.1.0/test/integration/public.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/integration/stream.py` & `bxsolana-trader-2.1.0/test/integration/stream.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/integration/test_grpc.py` & `bxsolana-trader-2.1.0/test/integration/test_grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/integration/test_http.py` & `bxsolana-trader-2.1.0/test/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/integration/test_ws.py` & `bxsolana-trader-2.1.0/test/integration/test_ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/unit/transaction/test_memo.py` & `bxsolana-trader-2.1.0/test/unit/transaction/test_memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.1/test/unit/transaction/test_signing.py` & `bxsolana-trader-2.1.0/test/unit/transaction/test_signing.py`

 * *Files identical despite different names*

