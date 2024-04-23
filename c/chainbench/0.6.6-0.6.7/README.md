# Comparing `tmp/chainbench-0.6.6.tar.gz` & `tmp/chainbench-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.6.6.tar", max compression
+gzip compressed data, was "chainbench-0.6.7.tar", max compression
```

## Comparing `chainbench-0.6.6.tar` & `chainbench-0.6.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2024-04-09 05:42:16.689645 chainbench-0.6.6/LICENSE
--rw-r--r--   0        0        0    12165 2024-04-09 05:42:16.689645 chainbench-0.6.6/README.md
--rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/__main__.py
--rw-r--r--   0        0        0    15103 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3732 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2760 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1158 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0     2776 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      344 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0     1272 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      427 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4252 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1655 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1931 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2897 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0     3514 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2223 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6482 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5934 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    12501 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     5443 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      416 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/__init__.py
--rw-r--r--   0        0        0     2895 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/ethereum.py
--rw-r--r--   0        0        0     4622 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/evm.py
--rw-r--r--   0        0        0     4672 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/http.py
--rw-r--r--   0        0        0      799 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/__init__.py
--rw-r--r--   0        0        0      516 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/common.py
--rw-r--r--   0        0        0     9082 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/ethereum.py
--rw-r--r--   0        0        0    10003 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/evm.py
--rw-r--r--   0        0        0     2885 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/solana.py
--rw-r--r--   0        0        0     3680 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/starknet.py
--rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6218 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/util/cli.py
--rw-r--r--   0        0        0    12953 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/event.py
--rw-r--r--   0        0        0     5766 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/rng.py
--rw-r--r--   0        0        0      337 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/rpc.py
--rw-r--r--   0        0        0      455 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/timer.py
--rw-r--r--   0        0        0      953 2024-04-09 05:42:16.693645 chainbench-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    12756 1970-01-01 00:00:00.000000 chainbench-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 09:37:04.066810 chainbench-0.6.7/LICENSE
+-rw-r--r--   0        0        0    12165 2024-04-23 09:37:04.066810 chainbench-0.6.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/__main__.py
+-rw-r--r--   0        0        0    15103 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2760 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1158 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0     2776 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      344 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0     1272 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      427 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4252 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1655 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1931 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2897 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0     3514 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6482 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    18785 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     5443 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      416 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     2895 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/ethereum.py
+-rw-r--r--   0        0        0     4622 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/evm.py
+-rw-r--r--   0        0        0     4672 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/http.py
+-rw-r--r--   0        0        0      799 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/common.py
+-rw-r--r--   0        0        0     9082 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/ethereum.py
+-rw-r--r--   0        0        0    10003 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/evm.py
+-rw-r--r--   0        0        0     2885 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/solana.py
+-rw-r--r--   0        0        0     3680 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/starknet.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6218 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/cli.py
+-rw-r--r--   0        0        0    12953 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/event.py
+-rw-r--r--   0        0        0     5766 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/rng.py
+-rw-r--r--   0        0        0      337 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      455 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/timer.py
+-rw-r--r--   0        0        0      953 2024-04-23 09:37:04.070809 chainbench-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0    12756 1970-01-01 00:00:00.000000 chainbench-0.6.7/PKG-INFO
```

### Comparing `chainbench-0.6.6/LICENSE` & `chainbench-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/README.md` & `chainbench-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/main.py` & `chainbench-0.6.7/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/avalanche/general.py` & `chainbench-0.6.7/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/bsc/general.py` & `chainbench-0.6.7/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/ethereum/consensus.py` & `chainbench-0.6.7/chainbench/profile/ethereum/consensus.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/ethereum/general.py` & `chainbench-0.6.7/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/evm/debug_trace.py` & `chainbench-0.6.7/chainbench/profile/evm/debug_trace.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/evm/heavy.py` & `chainbench-0.6.7/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/evm/light.py` & `chainbench-0.6.7/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/oasis/general.py` & `chainbench-0.6.7/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/polygon/general.py` & `chainbench-0.6.7/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/solana/general.py` & `chainbench-0.6.7/chainbench/profile/solana/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/profile/starknet/wallet.py` & `chainbench-0.6.7/chainbench/profile/starknet/wallet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/test_data/__init__.py` & `chainbench-0.6.7/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/test_data/blockchain.py` & `chainbench-0.6.7/chainbench/test_data/blockchain.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/test_data/ethereum.py` & `chainbench-0.6.7/chainbench/test_data/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/test_data/evm.py` & `chainbench-0.6.7/chainbench/test_data/evm.py`

 * *Files 26% similar despite different names*

```diff
@@ -120,14 +120,25 @@
                 "0x3EE2200Efb3400fAbB9AacF31297cBdD1d435D47",
                 "0x1CE0c2827e2eF14D5C4f29a091d735A204794041",
                 "0xbA2aE424d960c26247Dd6c32edC70B295c744C43",
                 "0x7083609fCE4d1d8Dc0C979AAb8c869Ea2C873402",
                 "0xF8A0BF9cF54Bb92F17374d9e9A321E6a111a51bD",
             ],
         },
+        97: {
+            "name": "bsc-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0xbDa40aCd71540DE69e3D85f88f9fd0E97f575A7F",
+                "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd",
+                "0xae13d989daC2f0dEbFf460aC112a837C89BAa7cd",
+                "0x1efde6C6346EEdD82576903F65c7eC4141C54FFf",
+                "0x0000000000000000000000000000000000002005",
+            ],
+        },
         137: {
             "name": "polygon-mainnet",
             "start_block": 35000000,
             "contract_addresses": [
                 "0x7ceB23fD6bC0adD59E62ac25578270cFf1b9f619",
                 "0xc2132D05D31c914a87C6611C10748AEb04B58e8F",
                 "0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174",
@@ -136,14 +147,25 @@
                 "0x0000000000000000000000000000000000001010",
                 "0x1BFD67037B42Cf73acF2047067bd4F2C47D9BfD6",
                 "0x6f8a06447Ff6FcF75d803135a7de15CE88C1d4ec",
                 "0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063",
                 "0xb33EaAd8d922B1083446DC23f610c2567fB5180f",
             ],
         },
+        80002: {
+            "name": "polygon-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x41E94Eb019C0762f9Bfcf9Fb1E58725BfB0e7582",
+                "0xF9bAfe82B6B65091580E403BC0B6F8d15b59FaF6",
+                "0xC4Af1A414d115882CE5E270C2a42888AeF5d75D5",
+                "0x13F793FAadA9b42BeFEF18048658813CF6FE790F",
+                "0x48bD4aD223b2d454c045aBF22CDa1b716B64d380",
+            ],
+        },
         23294: {
             "name": "oasis-sapphire-mainnet",
             "start_block": 0,
             "contract_addresses": [
                 "0x39d22B78A7651A76Ffbde2aaAB5FD92666Aca520",
                 "0x8Bc2B030b299964eEfb5e1e0b36991352E56D2D3",
                 "0x6b59C68405B0216C2C8ba1EC1f8DCcBd47892c58",
@@ -164,14 +186,25 @@
                 "0xFE6B19286885a4F7F55AdAD09C3Cd1f906D2478F",
                 "0x2147EFFF675e4A4eE1C2f918d181cDBd7a8E208f",
                 "0x39cf1BD5f15fb22eC3D9Ff86b0727aFc203427cc",
                 "0x19860CCB0A68fd4213aB9D8266F7bBf05A8dDe98",
                 "0x8a0cAc13c7da965a312f08ea4229c37869e85cB9",
             ],
         },
+        43113: {
+            "name": "avalanche-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x5425890298aed601595a70AB815c96711a31Bc65",
+                "0xA089a21902914C3f3325dBE2334E9B466071E5f1",
+                "0xd00B9BBC6EDC3953Ec502d73E7FA7C59f628d947",
+                "0x45ea5d57BA80B5e3b0Ed502e9a08d568c96278F9",
+                "0xEdDEB2ff49830f3aa30Fee2F7FaBC5136845304a",
+            ],
+        },
         8453: {
             "name": "base-mainnet",
             "start_block": 1,
             "contract_addresses": [
                 "0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913",
                 "0x50c5725949A6F0c72E6C4a641F24049A917DB0Cb",
                 "0x2Ae3F1Ec7F1F5012CFEab0185bfc7aa3cf0DEc22",
@@ -180,23 +213,131 @@
                 "0x09188484e1Ab980DAeF53a9755241D759C5B7d60",
                 "0xd9aAEc86B65D86f6A7B5B1b0c42FFA531710b6CA",
                 "0x4200000000000000000000000000000000000006",
                 "0xE3B53AF74a4BF62Ae5511055290838050bf764Df",
                 "0x78a087d713Be963Bf307b18F2Ff8122EF9A63ae9",
             ],
         },
-        84531: {
-            "name": "base-goerli-testnet",
+        84532: {
+            "name": "base-sepolia-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x87C51CD469A0E1E2aF0e0e597fD88D9Ae4BaA967",
+                "0xBF916435e1E3548525F4e3Fe851c5aB0Da3F8Bf1",
+                "0x036CbD53842c5426634e7929541eC2318f3dCF7e",
+                "0xf960d27DC82e5a587441CCbFa8B0Ba7E0f8740B3",
+                "0x3a673d6896Ee19dd3d7930563792848B1BEd84dF",
+            ],
+        },
+        42161: {
+            "name": "arbitrum-mainnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0xFd086bC7CD5C481DCC9C85ebE478A1C0b69FCbb9",
+                "0xFF970A61A04b1cA14834A43f5dE4533eBDDB5CC8",
+                "0xaf88d065e77c8cC2239327C5EDb3A432268e5831",
+                "0x2f2a2543B76A4166549F7aaB2e75Bef0aefC5B0f",
+                "0xf97f4df75117a78c1A5a0DBb814Af92458539FB4",
+                "0xFa7F8980b0f1E64A2062791cc3b0871572f1F7f0",
+                "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1",
+                "0x912CE59144191C1204E64559FE8253a0e49E6548",
+                "0x25d887Ce7a35172C62FeBFD67a1856F20FaEbB00",
+                "0x9623063377AD1B27544C965cCd7342f7EA7e88C7",
+            ],
+        },
+        421614: {
+            "name": "arbitrum-sepolia-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x9aA40Cc99973d8407a2AE7B2237d26E615EcaFd2",
+                "0x3E27fAe625f25291bFda517f74bf41DC40721dA2",
+                "0x980B62Da83eFf3D4576C647993b0c1D7faf17c73",
+                "0xDbc8c016287437ce2cF69fF64c245A4D74599A40",
+                "0xb1D4538B4571d411F07960EF2838Ce337FE1E80E",
+            ],
+        },
+        10: {
+            "name": "optimism-mainnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58",
+                "0x0b2C639c533813f4Aa9D7837CAf62653d097Ff85",
+                "0x7F5c764cBc14f9669B88837ca1490cCa17c31607",
+                "0x68f180fcCe6836688e9084f035309E29Bf0A2095",
+                "0x350a791Bfc2C21F9Ed5d10980Dad2e2638ffa7f6",
+                "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1",
+                "0x4200000000000000000000000000000000000042",
+                "0xFdb794692724153d1488CcdBE0C56c252596735F",
+                "0xdC6fF44d5d932Cbd77B52E5612Ba0529DC6226F1",
+                "0x99C59ACeBFEF3BBFB7129DC90D1a11DB0E91187f",
+            ],
+        },
+        11155420: {
+            "name": "optimism-sepolia-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x5fd84259d66Cd46123540766Be93DFE6D43130D7",
+                "0xb210fba65DC617bE30eB6B0b99B3CDd5556EF82e",
+                "0x298b4c4F9bE251c100724a3bEAe234BD1652CBcE",
+                "0xE4aB69C077896252FAFBD49EFD26B5D171A32410",
+                "0x0c21E17F8F9131260FA264dD56C8395F7B692149",
+            ],
+        },
+        250: {
+            "name": "fantom-mainnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0xBE41772587872A92184873d55B09C6bB6F59f895",
+                "0x04068DA6C83AFCFA0e13ba15A6696662335D5B75",
+                "0x82f0B8B456c1A451378467398982d4834b6829c1",
+                "0x21be370D5312f44cB42ce377BC9b8a0cEF1A4C83",
+                "0x2F6F07CDcf3588944Bf4C42aC74ff24bF56e7590",
+                "0x841FAD6EAe12c286d1Fd18d1d525DFfA75C7EFFE",
+                "0x8D11eC38a3EB5E956B052f67Da8Bdc9bef8Abf3E",
+                "0x5Cc61A78F164885776AA610fb0FE1257df78E59B",
+                "0x049d68029688eAbF473097a2fC38ef61633A3C7A",
+                "0x6c021Ae822BEa943b2E66552bDe1D2696a53fbB7",
+            ],
+        },
+        4002: {
+            "name": "fantom-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0xeccCAf43A81AADf68962346c62F07f8e9bfDa3AA",
+                "0xf1277d1Ed8AD466beddF92ef448A132661956621",
+                "0x75Cc4fDf1ee3E781C1A3Ee9151D5c6Ce34Cf5C61",
+                "0xEAe1274dBdD006b5eA3197729BF5f11B8fbb427E",
+                "0x5538e600dc919f72858dd4D4F5E4327ec6f2af60",
+            ],
+        },
+        2020: {
+            "name": "ronin-mainnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0xa8754b9fa15fc18bb59458815510e40a12cd2014",
+                "0xc99a6a985ed2cac1ef41640596c5a5f9f4e19ef5",
+                "0x97a9107c1793bc407d6f527b77e7fff4d812bece",
+                "0xc39a2430b0b6f1edad1681672b47c857c1be0998",
+                "0xe514d9deb7966c8be0ca922de8a064264ea6bcd4",
+                "0x0b7007c13325c48911f73a2dad5fa5dcbf808adc",
+                "0x7eae20d11ef8c779433eb24503def900b9d28ad7",
+                "0x1b918543b518e34902e1e8dd76052bee43c762ff",
+                "0x306a28279d04a47468ed83d55088d0dcd1369294",
+                "0x2ecb08f87f075b5769fe543d0e52e40140575ea7",
+            ],
+        },
+        2021: {
+            "name": "ronin-testnet",
             "start_block": 1,
             "contract_addresses": [
-                "0x231401dC8b53338d78c08f83CC4EBc74148196d0",
-                "0xF175520C52418dfE19C8098071a252da48Cd1C19",
-                "0x4B2d9827F7Ee26e8e1732b4614A35fBEa1f06D7A",
-                "0x41927EfAd7C649DB0605E53d7D409AEb2F499608",
-                "0xf0efcf5b2e7E8580d7D7aac0c11f5066541585D0",
+                "0x3c4e17b9056272ce1b49f6900d8cfd6171a1869d",
+                "0x29c6f8349a028e1bdfc68bfa08bdee7bc5d47e16",
+                "0xa959726154953bae111746e265e6d754f48570e6",
+                "0x04ef1d4f687bb20eedcf05c7f710c078ba39f328",
+                "0x067fbff8990c58ab90bae3c97241c5d736053f77",
             ],
         },
         # TODO: Move StarkNet out of EVMNetwork
         23448594291968334: {
             "name": "starknet-mainnet",
             "start_block": 100000,
             "contract_addresses": [],
```

### Comparing `chainbench-0.6.6/chainbench/test_data/solana.py` & `chainbench-0.6.7/chainbench/test_data/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/test_data/starknet.py` & `chainbench-0.6.7/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/tools/discovery/clients.json` & `chainbench-0.6.7/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/tools/discovery/methods.json` & `chainbench-0.6.7/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/tools/discovery/rpc.py` & `chainbench-0.6.7/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/ethereum.py` & `chainbench-0.6.7/chainbench/user/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/evm.py` & `chainbench-0.6.7/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/http.py` & `chainbench-0.6.7/chainbench/user/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/methods/__init__.py` & `chainbench-0.6.7/chainbench/user/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/methods/common.py` & `chainbench-0.6.7/chainbench/user/methods/common.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/methods/ethereum.py` & `chainbench-0.6.7/chainbench/user/methods/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/methods/evm.py` & `chainbench-0.6.7/chainbench/user/methods/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/solana.py` & `chainbench-0.6.7/chainbench/user/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/user/starknet.py` & `chainbench-0.6.7/chainbench/user/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/cli.py` & `chainbench-0.6.7/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/event.py` & `chainbench-0.6.7/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/http.py` & `chainbench-0.6.7/chainbench/util/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/monitor.py` & `chainbench-0.6.7/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/notify.py` & `chainbench-0.6.7/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/chainbench/util/rng.py` & `chainbench-0.6.7/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.6/pyproject.toml` & `chainbench-0.6.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
```

### Comparing `chainbench-0.6.6/PKG-INFO` & `chainbench-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.6.6
+Version: 0.6.7
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

