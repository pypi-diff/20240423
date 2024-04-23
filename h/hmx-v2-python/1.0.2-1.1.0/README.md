# Comparing `tmp/hmx-v2-python-1.0.2.tar.gz` & `tmp/hmx-v2-python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx-v2-python-1.0.2.tar", last modified: Sun Apr 14 03:17:59 2024, max compression
+gzip compressed data, was "hmx-v2-python-1.1.0.tar", last modified: Tue Apr 23 11:48:28 2024, max compression
```

## Comparing `hmx-v2-python-1.0.2.tar` & `hmx-v2-python-1.1.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.507400 hmx-v2-python-1.0.2/
--rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/LICENSE
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-14 03:17:59.507530 hmx-v2-python-1.0.2/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/README.md
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.497088 hmx-v2-python-1.0.2/hmx2/
--rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.501105 hmx-v2-python-1.0.2/hmx2/abis/
--rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/abis/Calculator.json
--rw-r--r--   0 adirut     (501) staff       (20)    79531 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/ERC20.json
--rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/GlpManager.json
--rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.2/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 adirut     (501) staff       (20)    26127 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/PerpStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/abis/TradeHelper.json
--rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.502179 hmx-v2-python-1.0.2/hmx2/constants/
--rw-r--r--   0 adirut     (501) staff       (20)       97 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.2/hmx2/constants/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1953 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/constants/assets.py
--rw-r--r--   0 adirut     (501) staff       (20)      294 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/common.py
--rw-r--r--   0 adirut     (501) staff       (20)     1700 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/contracts.py
--rw-r--r--   0 adirut     (501) staff       (20)     7052 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/markets.py
--rw-r--r--   0 adirut     (501) staff       (20)    10357 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/pricefeed.py
--rw-r--r--   0 adirut     (501) staff       (20)     5414 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/constants/tokens.py
--rw-r--r--   0 adirut     (501) staff       (20)      118 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/enum.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.502660 hmx-v2-python-1.0.2/hmx2/helpers/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/helpers/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/helpers/contract_loader.py
--rw-r--r--   0 adirut     (501) staff       (20)      519 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/helpers/mapper.py
--rw-r--r--   0 adirut     (501) staff       (20)      636 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/helpers/util.py
--rw-r--r--   0 adirut     (501) staff       (20)     2771 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/hmx_client.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503198 hmx-v2-python-1.0.2/hmx2/modules/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503466 hmx-v2-python-1.0.2/hmx2/modules/calculator/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     6048 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503785 hmx-v2-python-1.0.2/hmx2/modules/oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504031 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504294 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1003 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504515 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.505109 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)     3321 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.505457 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)    14072 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/private.py
--rw-r--r--   0 adirut     (501) staff       (20)    29226 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/public.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.506411 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     1752 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/SOURCES.txt
--rw-r--r--   0 adirut     (501) staff       (20)        1 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/dependency_links.txt
--rw-r--r--   0 adirut     (501) staff       (20)      154 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/requires.txt
--rw-r--r--   0 adirut     (501) staff       (20)       11 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/top_level.txt
--rw-r--r--   0 adirut     (501) staff       (20)       79 2024-04-14 03:17:59.507758 hmx-v2-python-1.0.2/setup.cfg
--rw-r--r--   0 adirut     (501) staff       (20)     1456 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/setup.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.507294 hmx-v2-python-1.0.2/tests/
--rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/tests/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/tests/constants.py
--rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.2/tests/test_create_market_order.py
--rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/tests/test_deposit_collateral.py
--rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/tests/test_get_adaptive_fee.py
--rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/tests/test_init.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.150835 hmx-v2-python-1.1.0/
+-rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/LICENSE
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-23 11:48:28.151065 hmx-v2-python-1.1.0/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/README.md
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.139582 hmx-v2-python-1.1.0/hmx2/
+-rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.143667 hmx-v2-python-1.1.0/hmx2/abis/
+-rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/abis/Calculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)    79531 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/ERC20.json
+-rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/GlpManager.json
+-rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.1.0/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)    26127 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.144902 hmx-v2-python-1.1.0/hmx2/constants/
+-rw-r--r--   0 adirut     (501) staff       (20)      107 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     2053 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/assets.py
+-rw-r--r--   0 adirut     (501) staff       (20)      330 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/common.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1769 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/contracts.py
+-rw-r--r--   0 adirut     (501) staff       (20)       52 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/intent.py
+-rw-r--r--   0 adirut     (501) staff       (20)     7448 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/markets.py
+-rw-r--r--   0 adirut     (501) staff       (20)    10909 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/pricefeed.py
+-rw-r--r--   0 adirut     (501) staff       (20)    10061 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/tokens.py
+-rw-r--r--   0 adirut     (501) staff       (20)      237 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/enum.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.145640 hmx-v2-python-1.1.0/hmx2/helpers/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/helpers/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 adirut     (501) staff       (20)      519 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/helpers/mapper.py
+-rw-r--r--   0 adirut     (501) staff       (20)      741 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/helpers/util.py
+-rw-r--r--   0 adirut     (501) staff       (20)     2771 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/hmx_client.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.145943 hmx-v2-python-1.1.0/hmx2/modules/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.146163 hmx-v2-python-1.1.0/hmx2/modules/calculator/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     6048 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.146789 hmx-v2-python-1.1.0/hmx2/modules/oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147137 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147500 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1003 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147853 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.148523 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3321 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.148781 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)    19733 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/modules/private.py
+-rw-r--r--   0 adirut     (501) staff       (20)    29817 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/modules/public.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.149469 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     1777 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/SOURCES.txt
+-rw-r--r--   0 adirut     (501) staff       (20)        1 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/dependency_links.txt
+-rw-r--r--   0 adirut     (501) staff       (20)      172 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/requires.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       11 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/top_level.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       79 2024-04-23 11:48:28.151303 hmx-v2-python-1.1.0/setup.cfg
+-rw-r--r--   0 adirut     (501) staff       (20)     1481 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/setup.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.150726 hmx-v2-python-1.1.0/tests/
+-rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/tests/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/tests/constants.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.1.0/tests/test_create_market_order.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/tests/test_deposit_collateral.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/tests/test_init.py
```

### Comparing `hmx-v2-python-1.0.2/LICENSE` & `hmx-v2-python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/PKG-INFO` & `hmx-v2-python-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.0.2
+Version: 1.1.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.0.2/README.md` & `hmx-v2-python-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/CIXPriceAdapter.json` & `hmx-v2-python-1.1.0/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/Calculator.json` & `hmx-v2-python-1.1.0/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/ConfigStorage.json` & `hmx-v2-python-1.1.0/hmx2/abis/ConfigStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/CrossMarginHandler.json` & `hmx-v2-python-1.1.0/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/ERC20.json` & `hmx-v2-python-1.1.0/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/GlpManager.json` & `hmx-v2-python-1.1.0/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/GmPriceAdapter.json` & `hmx-v2-python-1.1.0/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/LimitTradeHandler.json` & `hmx-v2-python-1.1.0/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/OnchainPricelens.json` & `hmx-v2-python-1.1.0/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/PerpStorage.json` & `hmx-v2-python-1.1.0/hmx2/abis/PerpStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/TradeHelper.json` & `hmx-v2-python-1.1.0/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/abis/VaultStorage.json` & `hmx-v2-python-1.1.0/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/constants/assets.py` & `hmx-v2-python-1.1.0/hmx2/constants/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,18 +54,22 @@
 ASSET_ATOM = "ATOM"
 ASSET_1000SHIB = "1000SHIB"
 ASSET_1000PEPE = "1000PEPE"
 ASSET_ICP = "ICP"
 ASSET_MANTA = "MANTA"
 ASSET_STRK = "STRK"
 ASSET_PYTH = "PYTH"
+ASSET_PENDLE = "PENDLE"
+ASSET_W = "W"
+ASSET_ENA = "ENA"
 
 ASSETS = [ASSET_ETH, ASSET_BTC, ASSET_AAPL, ASSET_JPY, ASSET_XAU, ASSET_AMZN,
           ASSET_MSFT, ASSET_TSLA, ASSET_EUR, ASSET_XAG, ASSET_AUD, ASSET_GBP,
           ASSET_ADA, ASSET_MATIC, ASSET_SUI, ASSET_ARB, ASSET_OP, ASSET_LTC,
           ASSET_COIN, ASSET_GOOG, ASSET_BNB, ASSET_SOL, ASSET_QQQ, ASSET_XRP,
           ASSET_USDC, ASSET_USDT, ASSET_DAI, ASSET_GLP, ASSET_NVDA, ASSET_LINK,
           ASSET_CHF, ASSET_DOGE, ASSET_CAD, ASSET_SGD, ASSET_CNH, ASSET_wstETH,
           ASSET_HKD, ASSET_BCH, ASSET_MEME, ASSET_gmBTC, ASSET_gmETH, ASSET_SEK,
           ASSET_DIX, ASSET_JTO, ASSET_STX, ASSET_ORDI, ASSET_TIA, ASSET_AVAX,
           ASSET_INJ, ASSET_DOT, ASSET_SEI, ASSET_ATOM, ASSET_1000SHIB, ASSET_1000PEPE,
-          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH, ASSET_USDCe]
+          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH, ASSET_USDCe, ASSET_PENDLE,
+          ASSET_W, ASSET_ENA]
```

### Comparing `hmx-v2-python-1.0.2/hmx2/constants/contracts.py` & `hmx-v2-python-1.1.0/hmx2/constants/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     "VAULT_STORAGE_ADDRESS": "0x56CC5A9c0788e674f17F7555dC8D3e2F1C0313C0",
     "DIX_PRICE_ADAPTER_ADDRESS": "0x222918d230c5A29F334fFb3020aD57b8CeBD1B82",
     "GM_BTC_PRICE_ADAPTER_ADDRESS": "0x85680bba8a94c9be1DDd7Be802885DFCe95F8164",
     "GM_ETH_PRICE_ADAPTER_ADDRESS": "0x700083c72eBc86CbFc865830F5706a2DbC392f26",
     "TRADE_HELPER_ADDRESS": "0x963Cbe4cFcDC58795869be74b80A328b022DE00C",
     "ONCHAIN_PRICELENS_ADDRESS": "0x7D8eAa8dF02526c711F4ff1f97F6c5324212DBBa",
     "CALCULATOR_ADDRESS": "0x0FdE910552977041Dc8c7ef652b5a07B40B9e006",
-  }
+    "INTENT_ADDRESS": "0xA5b749203967e3ddF48006a7d7C258E59Ac07A96",
+  },
 }
 
 # ------ ABI Path ------
 ERC20_ABI_PATH = "abis/ERC20.json"
 CROSS_MARGIN_HANDLER_ABI_PATH = "abis/CrossMarginHandler.json"
 LIMIT_TRADE_HANDLER_ABI_PATH = "abis/LimitTradeHandler.json"
 VAULT_STORAGE_ABI_PATH = "abis/VaultStorage.json"
```

### Comparing `hmx-v2-python-1.0.2/hmx2/constants/markets.py` & `hmx-v2-python-1.1.0/hmx2/constants/markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
   ASSET_ATOM,
   ASSET_1000PEPE,
   ASSET_1000SHIB,
   ASSET_SEK,
   ASSET_ICP,
   ASSET_MANTA,
   ASSET_STRK,
-  ASSET_PYTH
+  ASSET_PYTH,
+  ASSET_PENDLE,
+  ASSET_W,
+  ASSET_ENA,
 )
 
 
 # ------ Market ------
 MARKET_ETH_USD = 0
 MARKET_BTC_USD = 1
 MARKET_AAPL_USD = 2
@@ -101,14 +104,17 @@
 MARKET_1000PEPE_USD = 44
 MARKET_1000SHIB_USD = 45
 MARKET_USD_SEK = 46
 MARKET_ICP_USD = 47
 MARKET_MANTA_USD = 48
 MARKET_STRK_USD = 49
 MARKET_PYTH_USD = 50
+MARKET_PENDLE_USD = 51
+MARKET_W_USD = 52
+MARKET_ENA_USD = 53
 
 
 DELISTED_MARKET = [
     MARKET_AAPL_USD,
     MARKET_AMZN_USD,
     MARKET_MSFT_USD,
     MARKET_TSLA_USD,
@@ -371,8 +377,23 @@
     "display_decimal": 3,
   },
   MARKET_PYTH_USD: {
     "name": "PYTHUSD",
     "asset": ASSET_PYTH,
     "display_decimal": 4,
   },
+  MARKET_PENDLE_USD: {
+    "name": "PENDLEUSD",
+    "asset": ASSET_PENDLE,
+    "display_decimal": 4,
+  },
+  MARKET_W_USD: {
+    "name": "WUSD",
+    "asset": ASSET_W,
+    "display_decimal": 3,
+  },
+  MARKET_ENA_USD: {
+    "name": "ENAUSD",
+    "asset": ASSET_ENA,
+    "display_decimal": 3,
+  },
 }
```

### Comparing `hmx-v2-python-1.0.2/hmx2/constants/pricefeed.py` & `hmx-v2-python-1.1.0/hmx2/constants/pricefeed.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,17 @@
   ASSET_1000PEPE,
   ASSET_ICP,
   ASSET_SEK,
   ASSET_MANTA,
   ASSET_STRK,
   ASSET_PYTH,
   ASSET_wstETH,
+  ASSET_W,
+  ASSET_PENDLE,
+  ASSET_ENA,
 )
 DEFAULT_PYTH_PRICE_SERVICE_URL = "https://hermes.pyth.network"
 
 
 GET_LATEST_PRICE_FEEDS_ENDPOINT = "api/latest_price_feeds"
 
 PRICE_FEED_IDS = {
@@ -116,14 +119,17 @@
     ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
     ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
     ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
     ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
     ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
     ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
     ASSET_wstETH: "0x6df640f3b8963d8f8358f791f352b8364513f6ab1cca5ed3f1f7b5448980e784",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
   },
   421614: {
     ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
     ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
     ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
     ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
     ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
@@ -172,9 +178,12 @@
     ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
     ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
     ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
     ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
     ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
     ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
     ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
   }
 }
```

### Comparing `hmx-v2-python-1.0.2/hmx2/helpers/mapper.py` & `hmx-v2-python-1.1.0/hmx2/helpers/mapper.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/helpers/util.py` & `hmx-v2-python-1.1.0/hmx2/helpers/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import math
 from web3 import Web3
 
 
 # Convert asset_name to hex (0x77~)
 def convert_asset_to_byte32(asset_name):
   return Web3.to_hex(text=asset_name).ljust(66, '0')
 
@@ -20,7 +21,11 @@
   check_sub_account_id_param(sub_account_id)
   return Web3.to_checksum_address(hex(int(account, 16) ^ sub_account_id))
 
 
 def check_sub_account_id_param(sub_account_id: int):
   if sub_account_id not in range(0, 256):
     raise Exception("Invalid sub account id")
+
+
+def from_number_to_e30(n: float | int) -> int:
+  return math.floor(n * 10 ** 8) * 10 ** 22
```

### Comparing `hmx-v2-python-1.0.2/hmx2/hmx_client.py` & `hmx-v2-python-1.1.0/hmx2/hmx_client.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/calculator/calculator.py` & `hmx-v2-python-1.1.0/hmx2/modules/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/oracle_middleware.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/oracle_middleware.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/private.py` & `hmx-v2-python-1.1.0/hmx2/modules/private.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from eth_abi.packed import encode_packed
 from web3 import Web3, Account
 from web3.middleware.signing import construct_sign_and_send_raw_middleware
 from web3.logs import DISCARD
 from time import sleep
 from hmx2.constants.contracts import (
   CROSS_MARGIN_HANDLER_ABI_PATH,
   LIMIT_TRADE_HANDLER_ABI_PATH,
@@ -12,28 +13,45 @@
   CALCULATOR_ABI_PATH
 )
 from hmx2.constants.common import (
   ADDRESS_ZERO,
   MAX_UINT,
   EXECUTION_FEE,
   BPS,
+  MAX_UINT54,
+  MINUTES
 )
-from hmx2.enum import Cmd
+from hmx2.constants.intent import (
+  INTENT_TRADE_API,
+)
+from hmx2.constants.markets import MARKET_PROFILE
+from hmx2.enum import (
+  Action,
+  Cmd,
+)
+from eth_account import Account
+from secp256k1 import PrivateKey
+
+from eth_account.messages import encode_typed_data
+from time import time
 from hmx2.helpers.contract_loader import load_contract
 from simple_multicall_v6 import Multicall
 from hmx2.helpers.mapper import (
   get_contract_address,
   get_token_profile,
   get_collateral_address_asset_map,
   get_collateral_address_list
 )
-from hmx2.helpers.util import check_sub_account_id_param
+from hmx2.helpers.util import check_sub_account_id_param, from_number_to_e30
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from eth_abi.abi import encode
 import decimal
+import math
+import requests as r
+import json
 
 decimal.getcontext().prec = 15
 decimal.getcontext().rounding = "ROUND_HALF_DOWN"
 
 
 class Private(object):
 
@@ -153,15 +171,15 @@
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
       self.token_profile['WETH']['address'],
       amount_wei,
       True
     ).transact({"from": self.eth_signer.address, "value": amount_wei})
 
-  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent=False):
     '''
     Post a market order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -175,14 +193,22 @@
 
     :param reduce_only: required
     :type reduce_only: bool
 
     :param tp_token
     :type tp_token: str in list COLLATERALS address
     '''
+    if intent:
+      while True:
+        try:
+          return self.__create_intent_trade_order(sub_account_id, market_index, buy, size, reduce_only, tp_token)
+        except Exception as e:
+          # print(e)
+          sleep(0.5)
+
     check_sub_account_id_param(sub_account_id)
 
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": 0,
@@ -202,15 +228,15 @@
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
     args["order"] = events[0]["args"]
     return args
 
-  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent: bool = False):
     '''
     Post a trigger order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -230,14 +256,23 @@
 
     :param reduce_only: required
     :type reduce_only: bool
 
     :param tp_token
     :type tp_token: str in list COLLATERALS address
     '''
+
+    if intent:
+      while True:
+        try:
+          return self.__create_intent_trigger_order(sub_account_id, market_index, buy, size, trigger_price, trigger_above_threshold, reduce_only, tp_token)
+        except Exception as e:
+          # print(e)
+          sleep(0.5)
+
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": Web3.to_wei(trigger_price, "tether"),
       "acceptable_price": Web3.to_wei(
         self.__add_slippage(
@@ -258,15 +293,15 @@
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
     args["order"] = events[0]["args"]
     return args
 
-  def update_trigger_order(self, sub_account_id: int, order_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+  def update_trigger_order(self, sub_account_id: int, order_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent: bool = False):
     '''
     Update a trigger order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param order_index: required
@@ -409,12 +444,123 @@
     )
 
   def __parse_log(self, tx, topic):
     receipt = self.eth_provider.eth.get_transaction_receipt(tx)
     return self.limit_trade_handler_instance.events[topic](
       ).process_receipt(receipt, DISCARD)
 
+  def __create_intent_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+    created_timestamp = math.floor(time())
+    expired_timestamp = created_timestamp + 240 * MINUTES
+
+    acceptable_price = self.__add_slippage(
+      trigger_price) if buy else self.__sub_slippage(trigger_price)
+    acceptable_price = from_number_to_e30(acceptable_price)
+
+    trigger_price = from_number_to_e30(trigger_price)
+
+    # trunc to e8
+    size = from_number_to_e30(size)
+
+    json_body = json_body = self.__encode_and_build_trade_order(
+      market_index, size, buy, trigger_price, acceptable_price, trigger_above_threshold, reduce_only, tp_token, created_timestamp, expired_timestamp, sub_account_id)
+
+    return self.__upsert_intent_trade_orders_api(json_body)
+
+  def __create_intent_trade_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO):
+    created_timestamp = math.floor(time())
+    expired_timestamp = created_timestamp + 240 * MINUTES
+
+    acceptable_price = MAX_UINT54 if buy else 0
+    trigger_price = 0
+
+    # trunc to e8
+    size = from_number_to_e30(size)
+
+    json_body = self.__encode_and_build_trade_order(
+      market_index, size, buy, trigger_price, acceptable_price, True, reduce_only, tp_token, created_timestamp, expired_timestamp, sub_account_id)
+
+    return self.__upsert_intent_trade_orders_api(json_body)
+
+  def __upsert_intent_trade_orders_api(self, req):
+    return r.post(f'{INTENT_TRADE_API}/v1/intent-handler/orders.upsert', headers={'Content-Type': 'application/json'}, data=req)
+
+  def __encode_and_build_trade_order(self, market_index: int, size: int, buy: bool, trigger_price: int, acceptable_price: int, trigger_above_threshold: bool, reduce_only: bool, tp_token: str, created_timestamp: int, expired_timestamp: int, sub_account_id: int):
+    full_message = {
+      "domain": {
+        "name": "IntentHander",
+        "version": "1.0.0",
+        "chainId": self.chain_id,
+        "verifyingContract": get_contract_address(self.chain_id)['INTENT_ADDRESS']
+      },
+      "types": {
+        "TradeOrder": [
+          {"name": "marketIndex", "type": "uint256"},
+          {"name": "sizeDelta", "type": "int256"},
+          {"name": "triggerPrice", "type": "uint256"},
+          {"name": "acceptablePrice", "type": "uint256"},
+          {"name": "triggerAboveThreshold", "type": "bool"},
+          {"name": "reduceOnly", "type": "bool"},
+          {"name": "tpToken", "type": "address"},
+          {"name": "createdTimestamp", "type": "uint256"},
+          {"name": "expiryTimestamp", "type": "uint256"},
+          {"name": "account", "type": "address"},
+          {"name": "subAccountId", "type": "uint8"}
+        ]
+      },
+      "primaryType": "TradeOrder",
+      "message": {
+        "marketIndex": market_index,
+        "sizeDelta": str(size if buy else size * -1),
+        "triggerPrice": str(trigger_price),
+        "acceptablePrice": str(acceptable_price),
+        "triggerAboveThreshold": trigger_above_threshold,
+        "reduceOnly": reduce_only,
+        "tpToken": tp_token,
+        "createdTimestamp": created_timestamp,
+        "expiryTimestamp": expired_timestamp,
+        "account": self.eth_signer.address,
+        "subAccountId": sub_account_id
+      }
+    }
+
+    encoded_data = encode_typed_data(full_message=full_message)
+
+    sign_data = Account.sign_message(encoded_data, self.eth_signer.key)
+
+    signature = encode_packed(['bytes32', 'bytes32', 'uint8'], [
+        bytes.fromhex(hex(sign_data.r)[2:]), bytes.fromhex(hex(sign_data.s)[2:]), sign_data.v])
+
+    private_key = PrivateKey(
+      bytes(bytearray.fromhex(self.eth_signer.key.hex()[2:])))
+    pubkey_ser = private_key.pubkey.serialize(compressed=False).hex()
+
+    req_body = {
+      "chainId": self.chain_id,
+      "intentTradeOrders": [
+        {
+          "marketIndex": market_index,
+          "sizeDeltaE30": str(size if buy else size * -1),
+          "triggerPriceE30": str(trigger_price),
+          "acceptablePriceE30": str(acceptable_price),
+          "triggerAboveThreshold": trigger_above_threshold,
+          "reduceOnly": reduce_only,
+          "tpToken": tp_token,
+          "createdTimestamp": created_timestamp,
+          "expiryTimestamp": expired_timestamp,
+          "account": self.eth_signer.address,
+          "subAccountId": sub_account_id,
+          "signature": "0x" + signature.hex(),
+          "digest": sign_data.messageHash.hex(),
+          "publicKey": "0x" + pubkey_ser,
+        }
+      ]
+    }
+    json_body = json.dumps(req_body)
+
+    return json_body
+
   def get_public_address(self):
     '''
     Get the public address of the signer.
     '''
     return self.eth_signer.address
```

### Comparing `hmx-v2-python-1.0.2/hmx2/modules/public.py` & `hmx-v2-python-1.1.0/hmx2/modules/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,40 @@
 from hmx2.constants.contracts import (
   VAULT_STORAGE_ABI_PATH,
   PERP_STORAGE_ABI_PATH,
   CONFIG_STORAGE_ABI_PATH,
   TRADE_HELPER_ABI_PATH,
   CALCULATOR_ABI_PATH
 )
+from hmx2.constants.intent import INTENT_TRADE_API
 from hmx2.constants.markets import (
     MARKET_PROFILE,
     DELISTED_MARKET
 )
 from hmx2.constants.common import (
   BYTE_ZERO,
   HOURS,
   DAYS,
   YEARS
 )
+from hmx2.enum import IntentOrderStatus
 from hmx2.helpers.contract_loader import load_contract
 from hmx2.helpers.mapper import (
   get_collateral_address_asset_map,
   get_collateral_address_list,
   get_contract_address,
   get_token_profile,
 )
 from hmx2.helpers.util import get_sub_account
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from hmx2.modules.calculator.calculator import Calculator
 from simple_multicall_v6 import Multicall
 from eth_abi.abi import decode
 from typing import List
+import requests as r
 
 
 class Public(object):
   def __init__(self, chain_id: int, eth_provider: Web3, oracle_middleware: OracleMiddleware):
     self.chain_id = chain_id
     self.eth_provider = eth_provider
     self.oracle_middleware = oracle_middleware
@@ -813,7 +816,17 @@
           results[1][index].hex(), 16) / 10 ** token_profile[collateral]["decimals"]
       ret[token_profile[collateral]["symbol"]] = {
         'amount': amount,
         'value_usd': amount * collateral_price_dict[token_profile[collateral]["asset"]]
       }
 
     return ret
+
+  def get_active_intent_orders(self, address: str, sub_account_id: int):
+    return self.__get_intent_trade_orders_api(address, sub_account_id)
+
+  def __get_intent_trade_orders_api(self, address: str, sub_account_id: int):
+    params = {
+      "chainId": self.chain_id,
+      "status": IntentOrderStatus.Pending,
+    }
+    return r.get(f'{INTENT_TRADE_API}/v1/intent-handler/{address}/{sub_account_id}/trade-orders', headers={'Content-Type': 'application/json'}, params=params)
```

### Comparing `hmx-v2-python-1.0.2/hmx_v2_python.egg-info/PKG-INFO` & `hmx-v2-python-1.1.0/hmx_v2_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.0.2
+Version: 1.1.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.0.2/hmx_v2_python.egg-info/SOURCES.txt` & `hmx-v2-python-1.1.0/hmx_v2_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 hmx2/abis/PerpStorage.json
 hmx2/abis/TradeHelper.json
 hmx2/abis/VaultStorage.json
 hmx2/constants/__init__.py
 hmx2/constants/assets.py
 hmx2/constants/common.py
 hmx2/constants/contracts.py
+hmx2/constants/intent.py
 hmx2/constants/markets.py
 hmx2/constants/pricefeed.py
 hmx2/constants/tokens.py
 hmx2/helpers/__init__.py
 hmx2/helpers/contract_loader.py
 hmx2/helpers/mapper.py
 hmx2/helpers/util.py
```

### Comparing `hmx-v2-python-1.0.2/setup.py` & `hmx-v2-python-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     'eth_keys',
     'eth-account==0.10.0',
     'eth-abi>=4.0.0,<5.0.0',
     'uniswap-universal-router-decoder',
     'web3>=6.0.0,<7.0.0',
     'simple-multicall-v6',
     'responses',
-    'python-dotenv>=1.0.0'
+    'python-dotenv>=1.0.0',
+    'secp256k1==0.14.0'
 ]
 
 setup(
     name='hmx-v2-python',
-    version='1.0.2',
+    version='1.1.0',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx-v2-python-1.0.2/tests/constants.py` & `hmx-v2-python-1.1.0/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/tests/test_create_market_order.py` & `hmx-v2-python-1.1.0/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/tests/test_deposit_collateral.py` & `hmx-v2-python-1.1.0/tests/test_deposit_collateral.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/tests/test_get_adaptive_fee.py` & `hmx-v2-python-1.1.0/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.2/tests/test_init.py` & `hmx-v2-python-1.1.0/tests/test_init.py`

 * *Files identical despite different names*

