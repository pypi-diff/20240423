# Comparing `tmp/onchainpay_sdk-0.0.1.tar.gz` & `tmp/onchainpay_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onchainpay_sdk-0.0.1.tar", last modified: Mon Apr 22 16:08:41 2024, max compression
+gzip compressed data, was "onchainpay_sdk-0.0.2.tar", last modified: Tue Apr 23 17:11:01 2024, max compression
```

## Comparing `onchainpay_sdk-0.0.1.tar` & `onchainpay_sdk-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.024607 onchainpay_sdk-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/address_book/
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/address_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/advanced_account/
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/advanced_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/auto_swaps/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/auto_swaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/basic_actions/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/basic_actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/blockchain_addresses/
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/blockchain_addresses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_swaps/
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_swaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/invoices/
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/kyt/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/kyt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orders/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.028607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orphan_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orphan_transactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/partners_api/
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/partners_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/personal_addresses/
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/personal_addresses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/recurring_payments/
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/recurring_payments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/webhooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/withdraws/
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/withdraws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/requester.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 16:08:36.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:08:41.032607 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-22 16:08:41.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-22 16:08:41.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:08:41.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 16:08:41.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 16:08:41.000000 onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.049219 onchainpay_sdk-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/address_book/
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/address_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/advanced_account/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/advanced_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/auto_swaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/auto_swaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/basic_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/basic_actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.053218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/blockchain_addresses/
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/blockchain_addresses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_swaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_swaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/invoices/
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/kyt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/kyt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orders/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orphan_transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orphan_transactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/partners_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/partners_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/personal_addresses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/personal_addresses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/recurring_payments/
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/recurring_payments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/withdraws/
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/withdraws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 17:10:46.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:11:01.057218 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 17:11:01.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 17:11:01.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:11:01.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 17:11:01.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 17:11:01.000000 onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/top_level.txt
```

### Comparing `onchainpay_sdk-0.0.1/LICENSE` & `onchainpay_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onchainpay_sdk-0.0.1/PKG-INFO` & `onchainpay_sdk-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onchainpay_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for onchainpay.io API
 Home-page: https://github.com/onchainpay/onchainpay_sdk
 Author: onchainpay.io Team
 Author-email: hello@onchainpay.io
 Project-URL: Bug Tracker, https://github.com/onchainpay/onchainpay_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `onchainpay_sdk-0.0.1/setup.cfg` & `onchainpay_sdk-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = onchainpay_sdk
-version = 0.0.1
+version = 0.0.2
 author = onchainpay.io Team
 author_email = hello@onchainpay.io
 description = SDK for onchainpay.io API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/onchainpay/onchainpay_sdk
 project_urls =
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,41 +30,72 @@
         self._orphan_transactions = None
         self._address_book = None
         self._webhooks = None
 
         self._public_key = public_key
         self._private_key = private_key
 
+        self._partners_api_public_key = None
+        self._partners_api_private_key = None
+
+        self._advancedBalanceId = None
+
+        self._set_advanced_balance_id()
+
     def request(
             self,
             method: str,
             base_url: str,
             path: str,
+            api_type: str = "public",
             payload: dict = None,
     ):
         if payload and not isinstance(payload, dict):
             raise ValueError("Payload must be a dictionary")
 
+        public_key = self._public_key
+        private_key = self._private_key
+
+        if api_type == "partners":
+            public_key = self._partners_api_public_key
+            private_key = self._partners_api_private_key
+
         method = method.lower()
         url = f"{base_url}{path}"
-        api = APIRequestor(self._public_key, self._private_key, url, payload)
+        api = APIRequestor(public_key, private_key, url, payload)
 
         if method == "post":
             response = api.post()
         else:
-            raise InternalSDKError("Internal SDK error. Method not allowed")
+            raise InternalSDKError("Method not allowed")
 
         if isinstance(response, dict):
             return response
 
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return response.text
 
+    def init_partners_api(self, public_key: str, private_key: str):
+        if not public_key:
+            raise AuthenticationError("Public key is required to initialize partners api")
+        if not private_key:
+            raise AuthenticationError("Private key is required to initialize partners api")
+
+        self._partners_api_public_key = public_key
+        self._partners_api_private_key = private_key
+
+    def _set_advanced_balance_id(self):
+        response = self.advanced_account.get_advanced_balances()
+        if response.get("success") is True:
+            self._advancedBalanceId = response.get("response")[0].get("advancedBalanceId")
+        else:
+            raise InternalSDKError("Unable to get advanced balance id")
+
     @property
     def advanced_account(self):
         if self._advanced_account is None:
             from onchainpay_sdk.domains.advanced_account import AdvancedAccount
             self._advanced_account = AdvancedAccount(self, self._base_url)
 
         return self._advanced_account
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/address_book/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/address_book/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,57 +43,57 @@
             path="/address-book/add",
             payload=payload
         )
 
     """
     Deleting an address from the address book
 
-    :param required str address_id: The ID of the address in the system
+    :param required str addressId: The ID of the address in the system
     :return: dict
-    :raise ValueError: if address_id is not provided
+    :raise ValueError: if addressId is not provided
 
     :example:
     >>> sdk.address_book.delete_address("cd3867c2-2d55-4bfa-be7e-b2964ccedcc4")
     """
 
-    def delete_address(self, address_id: str):
-        check_required_field(address_id, "address_id")
+    def delete_address(self, addressId: str):
+        check_required_field(addressId, "addressId")
 
         payload = {
-            "addressId": address_id
+            "addressId": addressId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/address-book/remove",
             payload=payload
         )
 
     """
     Updating information at
 
-    :param required str address_id: The ID of the address in the system
+    :param required str addressId: The ID of the address in the system
     :param required str alias: Address name
     :param str comment: Comment on the address
     :return: dict
-    :raise ValueError: if address_id is not provided
+    :raise ValueError: if addressId is not provided
 
     :example:
     >>> sdk.address_book.update_address(
             "cd3867c2-2d55-4bfa-be7e-b2964ccedcc4",
             "Alias #2",
         )
     """
 
-    def update_address(self, address_id: str, alias: str = None, comment: str = None):
-        check_required_field(address_id, "address_id")
+    def update_address(self, addressId: str, alias: str = None, comment: str = None):
+        check_required_field(addressId, "addressId")
 
         payload = {
-            "addressId": address_id,
+            "addressId": addressId,
             "alias": alias,
             "comment": comment
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
@@ -109,15 +109,15 @@
     :param list networks: List of networks to search for addresses in
     :return: dict
     
     :example:
     >>> sdk.address_book.get_addresses()
     """
 
-    def get_addresses(self, limit: int = 10, page: int = None, networks: list = None):
+    def get_addresses(self, page: int = None, limit: int = 10, networks: list = None):
         payload = {
             "page": page,
             "limit": limit,
             "networks": networks
         }
 
         return self.sdk.request(
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/advanced_account/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/advanced_account/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from onchainpay_sdk import Client
-from onchainpay_sdk.resources.utils import check_required_field
 
 
 class AdvancedAccount:
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
@@ -20,53 +19,49 @@
         return self.sdk.request(
             "post", self.base_url, path="/advanced-balances"
         )
 
     """
     Get info about advanced balance by its id
 
-    :param required str balance_id: Advance balance identifier
     :return: dict
-    :raise ValueError: if balance_id is not provided
 
     :example:
-    >>> sdk.advanced_account.get_advanced_address_by_id("ba5716df-58c4-48f8-9401-68f6069fb4ff")
+    >>> sdk.advanced_account.get_advanced_balance()
     """
 
-    def get_advanced_address_by_id(self, balance_id: str):
-        check_required_field(balance_id, "balance_id")
-
-        payload = {"advancedBalanceId": balance_id}
+    def get_advanced_balance(self):
+        payload = {"advancedBalanceId": self.sdk._advancedBalanceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/advanced-balances", payload=payload
         )
 
     """
     Get payment address for advanced balance
 
-    :param required str balance_id: Advance balance identifier
     :param str currency: The coin in which you want to replenish the advance balance
     :param str network: The network of the coin in which you want to top up the advance balance
     :return: dict
-    :raise ValueError: if balance_id, network or currency is not provided
+    :raise ValueError: if network or currency is not provided
 
     :example:
     >>> sdk.advanced_account.get_payment_address(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff", 
             "ethereum", 
             "USDT"
         )
     """
 
-    def get_payment_address(self, balance_id: str, currency: str = None, network: str = None):
-        check_required_field(balance_id, "balance_id")
-
+    def get_payment_address(
+            self,
+            currency: str = None,
+            network: str = None
+    ):
         payload = {
-            "advancedBalanceId": balance_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
             "currency": currency,
             "network": network
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/auto_swaps/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/auto_swaps/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     Amount limits apply to creation:
         - the amount must be more than $30 in equivalent
         - the amount must be twice the commission of the network of the final coin/network
     
     :param required str address: The address to receive
     :param required str currency: The coin you want to receive
     :param required str network: The network where you want to receive coins
-    :param str amount_from: Outgoing amount
-    :param str amount_to: The final amount
-    :param bool fee_in_amount: To include the network commission in the amount to swap, 
+    :param str amountFrom: Outgoing amount
+    :param str amountTo: The final amount
+    :param bool feeInAmount: To include the network commission in the amount to swap, 
                                when specifying this parameter, the amountTo will be equal to the 
                                amount that the address will receive
     :param str webhook_url: URL for sending a status change notification
     :return: dict
     :raise ValueError: If address, currency, or network is not provided
     
     :example:
@@ -35,59 +35,59 @@
     """
 
     def create_swap(
             self,
             address: str,
             currency: str,
             network: str,
-            amount_from: str = None,
-            amount_to: str = None,
-            fee_in_amount: bool = None,
-            webhook_url: str = None,
+            amountFrom: str = None,
+            amountTo: str = None,
+            feeInAmount: bool = None,
+            webhookUrl: str = None,
     ):
         check_required_field(address, "address")
         check_required_field(currency, "currency")
         check_required_field(network, "network")
 
-        if amount_from is None and amount_to is None:
-            raise ValueError("amount_from or amount_to is required")
+        if amountFrom is None and amountTo is None:
+            raise ValueError("amountFrom or amountTo is required")
 
         payload = {
             "address": address,
             "currency": currency,
             "network": network,
-            "amountFrom": amount_from,
-            "amountTo": amount_to,
-            "feeInAmount": fee_in_amount,
-            "webhookUrl": webhook_url
+            "amountFrom": amountFrom,
+            "amountTo": amountTo,
+            "feeInAmount": feeInAmount,
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/auto-swaps/create",
             payload=payload
         )
 
     """
     Getting auto-swap data by its ID
     
-    :param required str swap_id: Auto-swap ID
+    :param required str id: Auto-swap ID
     :return: dict
-    :raise ValueError: If swap_id is not provided
+    :raise ValueError: If id is not provided
     
     :example:
     >>> sdk.auto_swaps.get_swap_by_id("18f36b77-bb02-4517-a548-d3989917e784")
     """
 
-    def get_swap_by_id(self, swap_id: str):
-        check_required_field(swap_id, "swap_id")
+    def get_swap_by_id(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": swap_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/auto-swaps/get", payload=payload
         )
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/basic_actions/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/basic_actions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     :return: dict
     :raise ValueError: if from_currency or to_currency is not provided
     
     :example:
     >>> sdk.basic_actions.get_current_price("BTC", "USDT")
     """
 
-    def get_currency_price(self, from_currency: str, to_currency: str):
-        check_required_field(from_currency, "from_currency")
-        check_required_field(to_currency, "to_currency")
+    def get_currency_price(self, fromCurrency: str, toCurrency: str):
+        check_required_field(fromCurrency, "fromCurrency")
+        check_required_field(toCurrency, "toCurrency")
 
         payload = {
-            "from": from_currency,
-            "to": to_currency
+            "from": fromCurrency,
+            "to": toCurrency
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/price-rate",
             payload=payload
@@ -71,27 +71,27 @@
     The method allows you to find an operation in the system by the address 
     of the transaction in the blockchain
 
     The response will indicate the type of operation, the direction of the transaction, 
     the address that was used for the operation and the body of the operation in the record 
     from the type
     
-    :param required str tx_hash: Transaction hash
+    :param required str tx: Transaction hash
     :return: dict
-    :raise ValueError: if tx_hash is not provided
+    :raise ValueError: if tx is not provided
     
     :example:
     >>> sdk.basic_actions.get_operation_by_tx_hash("0x788529118F2A28C60b9de2Ba0353f5EE4293e044")
     """
 
-    def get_operation_by_tx_hash(self, tx_hash: str):
-        check_required_field(tx_hash, "tx_hash")
+    def get_operation_by_tx_hash(self, tx: str):
+        check_required_field(tx, "tx")
 
         payload = {
-            "tx": tx_hash
+            "tx": tx
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/operation-by-tx-hash",
             payload=payload
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/blockchain_addresses/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/blockchain_addresses/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,70 +6,70 @@
         self.sdk = sdk
         self.base_url = base_url
 
     """
     The method allows you to find an address belonging to an organization by its ID, 
     regardless of its type
     
-    :param required str address_id: ID of the address in the system
+    :param required str id: ID of the address in the system
     :return: dict
-    :raise ValueError: If address_id is not provided
+    :raise ValueError: If id is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.find_by_id("d56bcbe4-586f-4980-b6ca-6e9f557750e8")
+    >>> sdk.blockchain_addresses.get_address_by_id("d56bcbe4-586f-4980-b6ca-6e9f557750e8")
     """
 
-    def get_address_by_id(self, address_id: str):
-        if not address_id:
-            raise ValueError("address ID is required")
+    def get_address_by_id(self, id: str):
+        if not id:
+            raise ValueError("id is required")
 
-        payload = {"id": address_id}
+        payload = {"id": id}
 
         return self.sdk.request(
             "post", self.base_url, path="/addresses/find-by-id", payload=payload
         )
 
     """
     To add a tracking address, you must specify the address itself and the URL for sending 
     notifications about transactions. The address will be monitored on all available networks.
     
     :param required str address: Address in the blockchain
-    :param required str webhook_url: URL for notifications when a transaction arrives
+    :param required str webhookUrl: URL for notifications when a transaction arrives
     :return: dict
-    :raise ValueError: If address or webhook_url is not provided
+    :raise ValueError: If address or webhookUrl is not provided
     
     :example:
     >>> sdk.blockchain_addresses.add_tracking_address(
             "0x788529118F2A28C60b9de2Ba0353f5EE4293e044", 
             "https://merchant.domain/webhooks/transaction"
         )
     """
 
-    def add_transaction_tracking(self, address: str, webhook_url: str):
+    def add_transaction_tracking(self, address: str, webhookUrl: str):
         if not address:
             raise ValueError("address is required")
-        if not webhook_url:
-            raise ValueError("webhook_url is required")
+        if not webhookUrl:
+            raise ValueError("webhookUrl is required")
 
-        payload = {"address": address, "webhookUrl": webhook_url}
+        payload = {"address": address, "webhookUrl": webhookUrl}
 
         return self.sdk.request(
             "post", self.base_url, path="/track-addresses/add-address", payload=payload
         )
 
     """
     The method allows you to find addresses belonging to an organization at an address 
     in the blockchain, regardless of the type and network
     
     :param required str address: Address in the blockchain
     :return: dict
     :raise ValueError: If address is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.search_by_address("0x788529118F2A28C60b9de2Ba0353f5EE4293e044")
+    >>> sdk.blockchain_addresses.get_address_by_address("0x788529118F2A28C60b9de2Ba0353f5EE4293e044")
     """
 
     def get_address_by_address(self, address: str):
         if not address:
             raise ValueError("address is required")
 
         payload = {"address": address}
@@ -78,199 +78,176 @@
             "post", self.base_url, path="/addresses/find-by-address", payload=payload
         )
 
     """
     The method allows you to set the meta-data for the address. 
     The field type is free, you can set any value
     
-    :param required str address_id: ID of the address in the system
+    :param required str id: ID of the address in the system
     :param any meta: Metadata to be set
     :return: dict
     :raise ValueError: If address_id is not provided
     
     :example:
     >>> sdk.blockchain_addresses.set_meta("d56bcbe4-586f-4980-b6ca-6e9f557750e8", {"key": "value"})
     """
 
-    def set_meta(self, address_id: str, meta: any = None):
-        if not address_id:
-            raise ValueError("address_id is required")
+    def set_meta(self, id: str, meta: any = None):
+        if not id:
+            raise ValueError("id is required")
 
-        payload = {"id": address_id, "meta": meta}
+        payload = {"id": id, "meta": meta}
 
         return self.sdk.request(
             "post", self.base_url, path="/addresses/set-meta", payload=payload
         )
 
     """
     The method allows you to get a list of transactions at the address.
     
-    :param required str address_id: Address ID
-    :param str tx_type: Transaction type (deposit, withdrawal)
+    :param required str id: Address ID
+    :param str type: Transaction type (deposit, withdrawal)
     :param list status: Array of statuses of a transaction (processed, error, rejected, pending)
     :param int limit: Maximum number of transactions to return 
                       (no less than 100 and no more than 1000, by default 100)
     :param int offset: Number of transactions to skip
     :return: dict
     :raise ValueError: If address_id is not provided
     
     :example:
     >>> sdk.blockchain_addresses.get_transactions("8e2d5033-139f-46d4-b769-4a2d2cee37c4")
     """
 
     def get_transactions(
             self,
-            address_id: str,
-            tx_type: str = None,
+            id: str,
+            type: str = None,
             status: list = None,
             limit: int = None,
             offset: int = None
     ):
 
-        if not address_id:
+        if not id:
             raise ValueError("address_id is required")
 
         payload = {
-            "id": address_id,
-            "type": tx_type,
+            "id": id,
+            "type": type,
             "status": status,
             "limit": limit,
             "offset": offset
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/addresses/transactions", payload=payload
         )
 
     """
     The method allows you to get PayIn address data (address, balance, identifier, etc.)
     
-    :param required str balance_id: Advance balance identifier
     :return: dict
-    :raise ValueError: If balance_id is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.get_payin_addresses("ba5716df-58c4-48f8-9401-68f6069fb4ff")
+    >>> sdk.blockchain_addresses.get_payin_addresses()
     """
 
-    def get_payin_addresses(self, balance_id: str):
-        if not balance_id:
-            raise ValueError("balance_id is required")
-
-        payload = {"advancedBalanceId": balance_id}
+    def get_payin_addresses(self):
+        payload = {"advancedBalanceId": self.sdk._advancedBalanceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/account-addresses", payload=payload
         )
 
     """
     Get business addresses for your advanced balance
     
-    :param required str balance_id: Advance balance identifier
     :return: dict
-    :raise ValueError: If balance_id is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.get_business_addresses("ba5716df-58c4-48f8-9401-68f6069fb4ff")
+    >>> sdk.blockchain_addresses.get_business_addresses()
     """
 
-    def get_business_addresses(self, balance_id: str):
-        if not balance_id:
-            raise ValueError("balance_id is required")
-
-        payload = {"advancedBalanceId": balance_id}
+    def get_business_addresses(self):
+        payload = {"advancedBalanceId": self.sdk._advancedBalanceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/business-addresses", payload=payload
         )
 
     """
     Get recurrent addresses for your advanced balance
     
-    :param required str balance_id: Advance balance identifier
     :return: dict
-    :raise ValueError: If balance_id is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.get_recurrent_addresses("ba5716df-58c4-48f8-9401-68f6069fb4ff")
+    >>> sdk.blockchain_addresses.get_recurrent_addresses()
     """
 
-    def get_recurrent_addresses(self, balance_id: str):
-        if not balance_id:
-            raise ValueError("balance_id is required")
-
-        payload = {"advancedBalanceId": balance_id}
+    def get_recurrent_addresses(self):
+        payload = {"advancedBalanceId": self.sdk._advancedBalanceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/recurrent-addresses", payload=payload
         )
 
     """
     The method allows you to get balances for this account.
     
     :param required str balance_id: Advance balance identifier
     :return: dict
     :raise ValueError: If balance_id is not provided
     
     :example:
-    >>> sdk.blockchain_addresses.get_payout_balances("ba5716df-58c4-48f8-9401-68f6069fb4ff")
+    >>> sdk.blockchain_addresses.get_payout_balances()
     """
 
-    def get_payout_addresses(self, balance_id: str):
-        if not balance_id:
-            raise ValueError("balance_id is required")
-
-        payload = {"advancedBalanceId": balance_id}
+    def get_payout_addresses(self):
+        payload = {"advancedBalanceId": self.sdk._advancedBalanceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/payout-balances", payload=payload
         )
 
     """
     The method allows you to create a new business address.
     
-    :param required str balance_id: Advance balance identifier
     :param required str currency: Coin ticker
     :param required str network: Network name
     :param required str alias: Address alias
     :param required str comment: Comment to the address
     :return: dict
-    :raise ValueError: If balance_id, currency, network, alias or comment is not provided
+    :raise ValueError: If currency, network, alias or comment is not provided
     
     :example:
     >>> sdk.blockchain_addresses.create_business_address(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
             "USDT",
             "ethereum",
             "My address alias",
             "My some address comment"
         )
     """
 
     def create_business_address(
             self,
-            balance_id: str,
             currency: str,
             network: str,
             alias: str,
             comment: str
     ):
-        if not balance_id:
-            raise ValueError("balance_id is required")
         if not currency:
             raise ValueError("currency is required")
         if not network:
             raise ValueError("network is required")
         if not alias:
             raise ValueError("alias is required")
         if not comment:
             raise ValueError("comment is required")
 
         payload = {
-            "advancedBalanceId": balance_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
             "currency": currency,
             "network": network,
             "alias": alias,
             "comment": comment
         }
 
         return self.sdk.request(
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_bridge/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_swaps/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,163 @@
 from onchainpay_sdk import Client
 from onchainpay_sdk.resources.utils import check_required_field
 
 
-class CrosschainBridge:
+class CrosschainSwaps:
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
-    The method allows you to get a commission token for cross-chain transfer
+    The method allows you to get a commission token for cross-chain exchange
     
-    :param required str balance_id: Identifier of the advance balance that will act as 
-                                    the payer of commissions
-    :param required str currency: The coin you want to exchange
-    :param required str network_from: Outgoing network
-    :param required str network_to: Network where you want to receive coins
-    :param required str amount: Amount to transfer
+    :param required str currencyFrom: Outgoing coin
+    :param required str currencyTo: Expected coin
+    :param required str networkFrom: Outgoing network
+    :param required str networkTo: Expected Network
+    :param str amountFrom: Exchange amount
+    :param str amountTo: Expected amount
     :return: dict
-    :raise ValueError: If balance_id, currency, network_from, network_to or amount 
-                           is not provided
+    :raise ValueError: If currencyFrom, currencyTo, networkFrom, networkTo 
+                           or either amountFrom or amountTo is not provided
     
     :example:
-    >>> sdk.crosschain_bridge.get_commission_token(
-            "d56bcbe4-586f-4980-b6ca-6e9f557750e8",
+    >>> sdk.crosschain_swaps.get_commission_token(
+            "USDT",
             "USDT",
             "ethereum",
             "tron",
             "100"
         )
     """
 
     def get_commission_token(
             self,
-            balance_id: str,
-            currency: str,
-            network_from: str,
-            network_to: str,
-            amount: str
+            currencyFrom: str,
+            currencyTo: str,
+            networkFrom: str,
+            networkTo: str,
+            amountFrom: str = None,
+            amountTo: str = None
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(currency, "currency")
-        check_required_field(network_from, "network_from")
-        check_required_field(network_to, "network_to")
-        check_required_field(amount, "amount")
+        check_required_field(currencyFrom, "currencyFrom")
+        check_required_field(currencyTo, "currencyTo")
+        check_required_field(networkFrom, "networkFrom")
+        check_required_field(networkTo, "networkTo")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "currency": currency,
-            "networkFrom": network_from,
-            "networkTo": network_to,
-            "amount": amount
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "currencyFrom": currencyFrom,
+            "currencyTo": currencyTo,
+            "networkFrom": networkFrom,
+            "networkTo": networkTo,
         }
 
+        if amountFrom:
+            payload["amountFrom"] = amountFrom
+        elif amountTo:
+            payload["amountTo"] = amountTo
+        else:
+            raise ValueError("You must provide either amountFrom or amountTo")
+
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/bridge/fee-token",
+            path="/swaps/fee-token",
             payload=payload
         )
 
     """
-    The method allows you to get limits for the amount of blockchain transfer
+    The method allows you to get limits for the amount of blockchain exchange
     
     :return: dict
     
     :example:
-    >>> sdk.crosschain_bridge.get_limits()
+    >>> sdk.crosschain_swaps.get_limits()
     """
 
     def get_limits(self):
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/bridge/limit"
+            path="/swaps/limit"
         )
 
     """
-    The method allows you to get information on a previously created cross-chain transfer
+    The method allows you to get information on a previously created cross-chain exchange
     
-    :param required str transfer_id: Cross-chain transfer ID
+    :param required str id: Swap ID
     :return: dict
-    :raise ValueError: If transfer_id is not provided
+    :raise ValueError: If id is not provided
     
     :example:
-    >>> sdk.crosschain_bridge.get_transfer_by_id("37ca03bc-e0f3-41d8-9ba3-fc214128fe08")
+    >>> sdk.crosschain_swaps.get_transfer_by_id("de2b4697-c758-4759-aa87-218a486589c7")
     """
 
-    def get_transfer_by_id(self, transfer_id: str):
-        check_required_field(transfer_id, "transfer_id")
+    def get_swap_by_id(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": transfer_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/bridge/get", payload=payload
+            path="/swaps/get", payload=payload
         )
 
     """
-    The method allows you to create a cross-chain transfer. 
-    Cross-chain transfer allows you to transfer your assets from one network to another
+    The method allows you to create a cross-chain exchange. 
+    Cross-chain exchange allows you to exchange one asset for another
     
-    :param required str balance_id: Identifier of the advance balance specified when creating 
-                                    the commission token 
-    :param required str address_from_id: Identifier of the outgoing address in the system, 
-                                         in the specified coin and network when creating 
-                                         the commission token. The specified amount will be 
-                                         debited from this address
-    :param required str address_to_id: Identifier of the destination address in the system 
-                                       where the coins should be delivered
-    :param required str fee_token: Commission token
-    :param str client_id: Unique transaction identifier in the merchant system, 
-                          to prevent duplication of creation
-    :param str webhook_url: URL address for operation status notification
+    :param required str addressFromId: Identifier of the outgoing address from which the specified
+                                         amount will be debited
+    :param required str addressToId: Identifier of the destination address where the coins will be
+                                       credited after the swap
+    :param required str feeToken: Commission token
+    :param str clientId: Unique exchange identifier in the merchant system 
+                          (to prevent duplicate requests)
+    :param str webhookUrl: URL address for operation status notification
     :return: dict
-    :raise ValueError: If balance_id, address_from_id, address_to_id or fee_token 
-                           is not provided
+    :raise ValueError: If addressFromId, addressToId or feeToken is not provided
     
     :example:
-    >>> sdk.crosschain_bridge.create_transfer(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
+    >>> sdk.crosschain_swaps.create_transfer(
             "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
             "0841afb1-f5a6-40c5-a2ff-881783c6e343",
             "U2FsdGVkX1/aencnde88lDxK7r/ySMC1dmw80rLIXoQ0kk/l5EG48/G8Ms8CuY6fYyxPVNw38lBCAWt/mTaQ
             he2pKhC01Vxk/PcuwApgjZUy1d7E3nEggxJVwBCmhvx0yCxGzrBEFhs41LIdJjaif0uMYWrDyEeaC0vyjVp1BPX
             k5rBjgJiIJveEfWgN0EItxRCjPl6A0TpC9KS2B0xCu0MP+eZ+Ve/8HC6KCS1SzHU=",
         )
     """
 
-    def create_transfer(
+    def create_swap(
             self,
-            balance_id: str,
-            address_from_id: str,
-            address_to_id: str,
-            fee_token: str,
-            client_id: str = None,
-            webhook_url: str = None
+            addressFromId: str,
+            addressToId: str,
+            feeToken: str,
+            clientId: str = None,
+            webhookUrl: str = None
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(address_from_id, "address_from_id")
-        check_required_field(address_to_id, "address_to_id")
-        check_required_field(fee_token, "fee_token")
+        check_required_field(addressFromId, "addressFromId")
+        check_required_field(addressToId, "addressToId")
+        check_required_field(feeToken, "feeToken")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "addressFromId": address_from_id,
-            "addressToId": address_to_id,
-            "feeToken": fee_token,
-            "clientId": client_id,
-            "webhookUrl": webhook_url
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "addressFromId": addressFromId,
+            "addressToId": addressToId,
+            "feeToken": feeToken,
+            "clientId": clientId,
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/bridge/create",
+            path="/swaps/create",
             payload=payload
         )
 
     def __repr__(self):
-        return "<onchainpay_sdk.CrosschainBridge>"
+        return "<onchainpay_sdk.CrosschainSwaps>"
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/crosschain_swaps/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/crosschain_bridge/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,166 +1,154 @@
 from onchainpay_sdk import Client
 from onchainpay_sdk.resources.utils import check_required_field
 
 
-class CrosschainSwaps:
+class CrosschainBridge:
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
-    The method allows you to get a commission token for cross-chain exchange
+    The method allows you to get a commission token for cross-chain transfer
     
-    :param required str balance_id: Advance balance identifier
-    :param required str currency_from: Outgoing coin
-    :param required str currency_to: Expected coin
-    :param required str network_from: Outgoing network
-    :param required str network_to: Expected Network
-    :param required str amount: Exchange amount
+    :param required str currency: The coin you want to exchange
+    :param required str networkFrom: Outgoing network
+    :param required str networkTo: Network where you want to receive coins
+    :param required str amount: Amount to transfer
     :return: dict
-    :raise ValueError: If balance_id, currency_from, currency_to, network_from, network_to 
-                           or amount is not provided
+    :raise ValueError: If currency, networkFrom, networkTo or amount 
+                           is not provided
     
     :example:
-    >>> sdk.crosschain_swaps.get_commission_token(
-            "d56bcbe4-586f-4980-b6ca-6e9f557750e8",
-            "USDT",
+    >>> sdk.crosschain_bridge.get_commission_token(
             "USDT",
             "ethereum",
             "tron",
             "100"
         )
     """
 
     def get_commission_token(
             self,
-            balance_id: str,
-            currency_from: str,
-            currency_to: str,
-            network_from: str,
-            network_to: str,
+            currency: str,
+            networkFrom: str,
+            networkTo: str,
             amount: str
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(currency_from, "currency_from")
-        check_required_field(currency_to, "currency_to")
-        check_required_field(network_from, "network_from")
-        check_required_field(network_to, "network_to")
+        check_required_field(currency, "currency")
+        check_required_field(networkFrom, "networkFrom")
+        check_required_field(networkTo, "networkTo")
         check_required_field(amount, "amount")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "currencyFrom": currency_from,
-            "currencyTo": currency_to,
-            "networkFrom": network_from,
-            "networkTo": network_to,
-            "amountFrom": amount
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "currency": currency,
+            "networkFrom": networkFrom,
+            "networkTo": networkTo,
+            "amount": amount
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/swaps/fee-token",
+            path="/bridge/fee-token",
             payload=payload
         )
 
     """
-    The method allows you to get limits for the amount of blockchain exchange
+    The method allows you to get limits for the amount of blockchain transfer
     
     :return: dict
     
     :example:
-    >>> sdk.crosschain_swaps.get_limits()
+    >>> sdk.crosschain_bridge.get_limits()
     """
 
     def get_limits(self):
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/swaps/limit"
+            path="/bridge/limit"
         )
 
     """
-    The method allows you to get information on a previously created cross-chain exchange
+    The method allows you to get information on a previously created cross-chain transfer
     
-    :param required str swap_id: Swap ID
+    :param required str id: Cross-chain transfer ID
     :return: dict
-    :raise ValueError: If swap_id is not provided
+    :raise ValueError: If id is not provided
     
     :example:
-    >>> sdk.crosschain_swaps.get_transfer_by_id("de2b4697-c758-4759-aa87-218a486589c7")
+    >>> sdk.crosschain_bridge.get_transfer_by_id("37ca03bc-e0f3-41d8-9ba3-fc214128fe08")
     """
 
-    def get_swap_by_id(self, swap_id: str):
-        check_required_field(swap_id, "swap_id")
+    def get_transfer_by_id(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": swap_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/swaps/get", payload=payload
+            path="/bridge/get", payload=payload
         )
 
     """
-    The method allows you to create a cross-chain exchange. 
-    Cross-chain exchange allows you to exchange one asset for another
+    The method allows you to create a cross-chain transfer. 
+    Cross-chain transfer allows you to transfer your assets from one network to another
     
-    :param required str balance_id: Identifier of the advance balance specified when creating 
-                                    the commission token 
-    :param required str address_from_id: Identifier of the outgoing address from which the specified
-                                         amount will be debited
-    :param required str address_to_id: Identifier of the destination address where the coins will be
-                                       credited after the swap
-    :param required str fee_token: Commission token
-    :param str client_id: Unique exchange identifier in the merchant system 
-                          (to prevent duplicate requests)
-    :param str webhook_url: URL address for operation status notification
+
+    :param required str addressFromId: Identifier of the outgoing address in the system, 
+                                         in the specified coin and network when creating 
+                                         the commission token. The specified amount will be 
+                                         debited from this address
+    :param required str addressToId: Identifier of the destination address in the system 
+                                       where the coins should be delivered
+    :param required str feeToken: Commission token
+    :param str clientId: Unique transaction identifier in the merchant system, 
+                          to prevent duplication of creation
+    :param str webhookUrl: URL address for operation status notification
     :return: dict
-    :raise ValueError: If balance_id, address_from_id, address_to_id or fee_token 
+    :raise ValueError: If balance_id, addressFromId, addressToId or feeToken 
                            is not provided
     
     :example:
-    >>> sdk.crosschain_swaps.create_transfer(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
-            "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
+    >>> sdk.crosschain_bridge.create_transfer(
             "0841afb1-f5a6-40c5-a2ff-881783c6e343",
             "U2FsdGVkX1/aencnde88lDxK7r/ySMC1dmw80rLIXoQ0kk/l5EG48/G8Ms8CuY6fYyxPVNw38lBCAWt/mTaQ
             he2pKhC01Vxk/PcuwApgjZUy1d7E3nEggxJVwBCmhvx0yCxGzrBEFhs41LIdJjaif0uMYWrDyEeaC0vyjVp1BPX
             k5rBjgJiIJveEfWgN0EItxRCjPl6A0TpC9KS2B0xCu0MP+eZ+Ve/8HC6KCS1SzHU=",
         )
     """
 
-    def create_swap(
+    def create_transfer(
             self,
-            balance_id: str,
-            address_from_id: str,
-            address_to_id: str,
-            fee_token: str,
-            client_id: str = None,
-            webhook_url: str = None
+            addressFromId: str,
+            addressToId: str,
+            feeToken: str,
+            clientId: str = None,
+            webhookUrl: str = None
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(address_from_id, "address_from_id")
-        check_required_field(address_to_id, "address_to_id")
-        check_required_field(fee_token, "fee_token")
+        check_required_field(addressFromId, "addressFromId")
+        check_required_field(addressToId, "addressToId")
+        check_required_field(feeToken, "feeToken")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "addressFromId": address_from_id,
-            "addressToId": address_to_id,
-            "feeToken": fee_token,
-            "clientId": client_id,
-            "webhookUrl": webhook_url
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "addressFromId": addressFromId,
+            "addressToId": addressToId,
+            "feeToken": feeToken,
+            "clientId": clientId,
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/swaps/create",
+            path="/bridge/create",
             payload=payload
         )
 
     def __repr__(self):
-        return "<onchainpay_sdk.CrosschainSwaps>"
+        return "<onchainpay_sdk.CrosschainBridge>"
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/invoices/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/invoices/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,113 +10,109 @@
     """
     The method allows you to create an invoices for payment without a strict indication 
     of the coin and network, you can specify a payment of 30 USD and a list of 
     coins/networks available for payment, the user himself will choose what is 
     more convenient for him to pay. 
     The amount will be automatically converted to the selected coin for payment
     
-    :param required str balance_id: Identifier of the advance balance for writing off commissions
     :param required str currency: Coins for payment. You can specify any available coin, 
                                   including fiat. On the invoices page, the amount in the specified 
                                   coin will be recalculated to the coins available for payment
     :param required str amount: Amount payable in the specified coin. On the invoices page, 
                                 the amount will be recalculated at the rate of coins 
                                 available for payment
     :param required str lifetime: Invoice lifetime in minutes
     :param list currencies: List of coins and networks available for payment, if you specify an 
                             empty array, all coins/networks available in the system will be selected
-    :param str external_id: A unique identifier in the merchant's system to prevent 
+    :param str externalId: A unique identifier in the merchant's system to prevent 
                             duplication of invoices
-    :param str order_id: Order ID in the merchant system
+    :param str order: Order ID in the merchant system
     :param str description: Order Description
-    :param bool include_fee: The flag allows you to include the commission of the blockchain 
+    :param bool includeFee: The flag allows you to include the commission of the blockchain 
                              network selected for payment in the amount payable. It will be useful 
                              to lay down your costs for the withdrawal of coins after payment.
-    :param list additional_fees: Array with the tariff names, which allows you to include commission 
+    :param list additionalFees: Array with the tariff names, which allows you to include commission 
                                  in final amount for the specified tariffs
-    :param str insurance_percent: Allows you to add the specified percentage to the payment amount
-    :param str slippage_percent: When opening the invoices page, the user can spend so much time on 
+    :param str insurancePercent: Allows you to add the specified percentage to the payment amount
+    :param str slippagePercent: When opening the invoices page, the user can spend so much time on 
                                  it that the exchange rate changes. If after the transition to 
                                  payment the amount changes more than the specified percentage, 
                                  then the amount payable will be recalculated at the current rate
-    :param str webhook_url: URL for notifications when the status of an invoices or amount 
+    :param str webhookURL: URL for notifications when the status of an invoices or amount 
                             received changes
-    :param str return_url: URL to specify as "Return to Store" on the checkout page
+    :param str returnURL: URL to specify as "Return to Store" on the checkout page
     :return: dict
-    :raise ValueError: If balance_id, currency, amount, or lifetime is not provided
+    :raise ValueError: If currency, amount, or lifetime is not provided
     
     :example:
     >>> sdk.invoices.create_invoice(
-            "cfda2034-0944-41c6-98e4-9146e8107dbc",
             "USD",
             "100",
             5,
         )
     """
 
     def create_invoice(
             self,
-            balance_id: str,
             currency: str,
             amount: str,
             lifetime: str,
             currencies: list = None,
-            external_id: str = None,
-            order_id: str = None,
+            externalId: str = None,
+            order: str = None,
             description: str = None,
-            webhook_url: str = None,
-            include_fee: bool = False,
-            additional_fees: list = None,
-            insurance_percent: str = None,
-            slippage_percent: str = None,
-            return_url: str = None,
+            webhookURL: str = None,
+            includeFee: bool = False,
+            additionalFees: list = None,
+            insurancePercent: str = None,
+            slippagePercent: str = None,
+            returnURL: str = None,
     ):
-        check_required_field(balance_id, "balance_id")
         check_required_field(currency, "currency")
         check_required_field(amount, "amount")
         check_required_field(lifetime, "lifetime")
 
         currencies = currencies or []
 
         payload = {
-            "advancedBalanceId": balance_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
             "currency": currency,
             "amount": amount,
             "lifetime": lifetime,
             "currencies": currencies,
-            "externalId": external_id,
-            "order": order_id,
+            "externalId": externalId,
+            "order": order,
             "description": description,
-            "webhookURL": webhook_url,
-            "returnURL": return_url,
-            "includeFee": include_fee,
-            "additionalFees": additional_fees,
-            "insurancePercent": insurance_percent,
-            "slippagePercent": slippage_percent,
+            "webhookURL": webhookURL,
+            "returnURL": returnURL,
+            "includeFee": includeFee,
+            "additionalFees": additionalFees,
+            "insurancePercent": insurancePercent,
+            "slippagePercent": slippagePercent,
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/make-invoice", payload=payload
         )
 
     """
     The method allows you to get information about the invoice
     
-    :param required str invoice_id: Invoice ID
+    :param required str invoiceId: Invoice ID
     :return: dict
-    :raise ValueError: If invoice_id is not provided
+    :raise ValueError: If invoiceId is not provided
     
     :example:
     >>> sdk.invoices.get_invoice_by_id("9f3318d2-66e6-4035-9841-055a83da8974")
     """
 
-    def get_invoice_by_id(self, invoice_id: str):
-        check_required_field(invoice_id, "invoice_id")
+    def get_invoice_by_id(self, invoiceId: str):
+        check_required_field(invoiceId, "invoiceId")
 
-        payload = {"invoiceId": invoice_id}
+        payload = {"invoiceId": invoiceId}
 
         return self.sdk.request(
             "post", self.base_url, path="/get-invoice", payload=payload
         )
 
     """
     The method allows you to get a list of invoices
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/kyt/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/kyt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,52 +6,51 @@
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
     The method allows you to check the risks of a completed transaction.
     
-    :param required str transaction_hash: Transaction hash
+    :param required str tx: Transaction hash
     :param required str currency: Currency
     :param required str network: Network
     :param required str output_address: Output address
     :param required str direction: Direction
     :return: dict
-    :raise ValueError: if transaction_hash, currency, network, output_address or direction 
-                       is not provided
+    :raise ValueError: if tx, currency, network, outputAddress or direction is not provided
     
     :example:
     >>> sdk.kyt.check_transaction_risk(
             "0x00E2453...",
             "USDT",
             "ethereum",
             "0x023434a...",
             "sent"
         )
     """
 
     def check_transaction_risk(
             self,
-            transaction_hash: str,
+            tx: str,
             currency: str,
             network: str,
-            output_address: str,
+            outputAddress: str,
             direction: str
     ):
-        check_required_field(transaction_hash, "transaction_hash")
+        check_required_field(tx, "tx")
         check_required_field(currency, "currency")
         check_required_field(network, "network")
-        check_required_field(output_address, "output_address")
+        check_required_field(outputAddress, "outputAddress")
         check_required_field(direction, "direction")
 
         payload = {
-            "tx": transaction_hash,
+            "tx": tx,
             "currency": currency,
             "network": network,
-            "outputAddress": output_address,
+            "outputAddress": outputAddress,
             "direction": direction
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/kyt/check-transfer",
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orders/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orders/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,97 +6,92 @@
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
     Create an order for payment
     
-    :param required str balance_id: Identifier of the advance balance for writing off commissions
     :param required str currency: Ticker of the coins in which the payment will be made
     :param required str network: The network of the coin in which the payment will be made
     :param required str amount: Payment amount
-    :param required str order_id: Order ID in the merchant system
+    :param required str order: Order ID in the merchant system
     :param required int lifetime: Order lifetime in seconds, available values from 1800 (30 minutes) 
                                   to 43200 (12 hours)
-    :param str error_url: URL to send webhook on error or order expiration
-    :param str success_url: URL to send webhook on successful payment
-    :param str return_url: URL to be placed on the payment page as "Return to Store" links
+    :param str errorWebhook: URL to send webhook on error or order expiration
+    :param str successWebhook: URL to send webhook on successful payment
+    :param str returnUrl: URL to be placed on the payment page as "Return to Store" links
     :param str description: Order description
-    :param bool check_risks: Whether to check incoming transactions for this order
+    :param bool checkRisks: Whether to check incoming transactions for this order
     :return: dict
-    :raise ValueError: If balance_id, currency, network, amount, order_id, or lifetime 
-                            is not provided
+    :raise ValueError: If balance_id, currency, network, amount, order, or lifetime is not provided
     
     :example:
     >>> sdk.orders.create_order(
-            "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
             "USDT",
             "ethereum",
             "0.0001",
             "order-1234",
             3600,
         )
     """
 
     def create_order(
             self,
-            balance_id: str,
             currency: str,
             network: str,
             amount: str,
-            order_id: str,
+            order: str,
             lifetime: int,
-            error_url: str = None,
-            success_url: str = None,
-            return_url: str = None,
+            errorWebhook: str = None,
+            successWebhook: str = None,
+            returnUrl: str = None,
             description: str = None,
-            check_risks: bool = False
+            checkRisks: bool = False
     ):
-        check_required_field("balance_id", balance_id)
         check_required_field("currency", currency)
         check_required_field("network", network)
         check_required_field("amount", amount)
-        check_required_field("order_id", order_id)
+        check_required_field("order", order)
         check_required_field("lifetime", lifetime)
 
         payload = {
-            "advancedBalanceId": balance_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
             "currency": currency,
             "network": network,
             "amount": amount,
-            "order": order_id,
+            "order": order,
             "lifetime": lifetime,
-            "errorWebhook": error_url,
-            "successWebhook": success_url,
-            "returnUrl": return_url,
+            "errorWebhook": errorWebhook,
+            "successWebhook": successWebhook,
+            "returnUrl": returnUrl,
             "description": description,
-            "checkRisks": check_risks
+            "checkRisks": checkRisks
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/make-order", payload=payload
         )
 
     """
     The method allows you to get information on a previously created order 
     by its identifier in the system
     
-    :param required str order_id: Order ID in the system
+    :param required str orderId: Order ID in the system
     :return: dict
-    :raise ValueError: If order_id is not provided
+    :raise ValueError: If orderId is not provided
     
     :example:
     >>> sdk.orders.get_order_by_id("8e2d5033-139f-46d4-b769-4a2d2cee37c4")
     """
 
-    def get_order_by_id(self, order_id: str):
-        check_required_field("order_id", order_id)
+    def get_order_by_id(self, orderId: str):
+        check_required_field("orderId", orderId)
 
         payload = {
-            "orderId": order_id
+            "orderId": orderId
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/order", payload=payload
         )
 
     """
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/orphan_transactions/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/orphan_transactions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,41 +6,41 @@
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
     Getting information about an orphan transaction by its ID
 
-    :param required str transaction_id: Transaction ID in the system
+    :param required str id: Transaction ID in the system
     :return: dict
-    :raise ValueError: if transaction_id is not provided
+    :raise ValueError: if id is not provided
 
     :example:
     >>> sdk.orphan_transactions.get_transaction_by_id("5cbf7135-d75a-4360-a9c4-8de7bf516baa")
     """
 
-    def get_transaction_by_id(self, transaction_id: str):
-        check_required_field(transaction_id, "transaction_id")
+    def get_transaction_by_id(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": transaction_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/orphan-deposits/get-deposit",
             payload=payload
         )
 
     """
     Getting a list of orphan transactions with the ability to filter by certain criteria
 
-    :param str transaction_id: Transaction ID in the system
-    :param str order_id: The ID of the order to which the address was linked at the time of 
+    :param str id: Transaction ID in the system
+    :param str orderId: The ID of the order to which the address was linked at the time of 
                          the transaction discovery
     :param str stage: The current stage of the transaction.
     :param str status: Status of the current stage of the transaction
     :param int limit: Number of transactions to return
     :param int offset: Offset for pagination
     :return: dict
 
@@ -48,24 +48,24 @@
     >>> sdk.orphan_transactions.get_transactions(
             5cbf7135-d75a-4360-a9c4-8de7bf516baa"
         )
     """
 
     def get_transactions(
             self,
-            transaction_id: str = None,
-            order_id: str = None,
+            id: str = None,
+            orderId: str = None,
             stage: str = None,
             status: str = None,
             limit: int = 10,
             offset: int = 0
     ):
         payload = {
-            "id": transaction_id,
-            "orderId": order_id,
+            "id": id,
+            "orderId": orderId,
             "status": status,
             "stage": stage,
             "limit": limit,
             "offset": offset
         }
 
         return self.sdk.request(
@@ -74,27 +74,27 @@
             path="/orphan-deposits/get-deposits",
             payload=payload
         )
 
     """
     Receiving a commission token to withdraw an orphan transaction
     
-    :param required str transaction_id: Transaction ID in the system
+    :param required str id: Transaction ID in the system
     :return: dict
-    :raise ValueError: if transaction_id is not provided
+    :raise ValueError: if id is not provided
     
     :example:
     >>> sdk.orphan_transactions.get_commission_token("5cbf7135-d75a-4360-a9c4-8de7bf516baa")
     """
 
-    def get_commission_token(self, transaction_id: str):
-        check_required_field(transaction_id, "transaction_id")
+    def get_commission_token(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": transaction_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/orphan-deposits/withdrawal-token",
             payload=payload
@@ -102,15 +102,15 @@
 
     """
     Receiving a commission token to withdraw an orphan transaction
     
     :param required str token: Withdrawal Token
     :param required str address: Output address
     :param str comment: Comment on the conclusion
-    :param str webhook_url: URL for sending a webhook about the withdrawal
+    :param str webhookUrl: URL for sending a webhook about the withdrawal
     :return: dict
     :raise ValueError: if token or address is not provided
     
     :example:
     >>> sdk.orphan_transactions.get_withdrawal(
             "5cbf7135-d75a-4360-a9c4-8de7bf516baa",
             "0x5cbf7135d75a4360a9c48de7bf516baa"
@@ -118,24 +118,24 @@
     """
 
     def get_withdrawal(
             self,
             token: str,
             address: str,
             comment: str = None,
-            webhook_url: str = None
+            webhookUrl: str = None
     ):
         check_required_field(token, "token")
         check_required_field(address, "address")
 
         payload = {
             "token": token,
             "address": address,
             "comment": comment,
-            "webhookUrl": webhook_url
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/orphan-deposits/withdrawal",
             payload=payload
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/partners_api/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/partners_api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,40 +25,42 @@
             "email": email
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/create-user",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get the user
     
-    :param required str user_id: User ID
+    :param required str id: User ID
     :return: dict
-    :raise ValueError: if user_id is not provided
+    :raise ValueError: if id is not provided
     
     :example:
     >>> sdk.partners_api.get_user("8efa4a83-86c9-4eb9-899a-27ce1079a2f8")
     """
 
-    def get_user_by_id(self, user_id: str):
-        check_required_field(user_id, "user_id")
+    def get_user_by_id(self, id: str):
+        check_required_field(id, "id")
 
         payload = {
-            "id": user_id
+            "id": id
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-user",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get all users
     
     :param int limit: Number of elements per page
     :param int offset: Number of items to skip
@@ -74,146 +76,148 @@
             "offset": offset
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-users",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to create an organization for the user
     
-    :param required str user_id: User ID
+    :param required str userId: User ID
     :return: dict
-    :raise ValueError: if user_id is not provided
+    :raise ValueError: if userId is not provided
     
     :example:
     >>> sdk.partners_api.create_organization("8efa4a83-86c9-4eb9-899a-27ce1079a2f8")
     """
 
-    def create_organization(self, user_id: str, name: str):
-        check_required_field(user_id, "user_id")
+    def create_organization(self, userId: str, name: str):
+        check_required_field(userId, "userId")
 
         payload = {
-            "userId": user_id,
+            "userId": userId,
             "name": name
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/create-user-organization",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get a list of organizations
     
-    :param required str user_id: User ID
+    :param required str userId: User ID
     :param int limit: Number of elements per page
     :param int offset: Number of items to skip
     :return: dict
-    :raise ValueError: if user_id is not provided
+    :raise ValueError: if userId is not provided
     
     :example:
     >>> sdk.partners_api.get_organizations("8efa4a83-86c9-4eb9-899a-27ce1079a2f8")
     """
 
-    def get_organizations(self, user_id: str, limit: int = 10, offset: int = 0):
-        check_required_field(user_id, "user_id")
+    def get_organizations(self, userId: str, limit: int = 10, offset: int = 0):
+        check_required_field(userId, "userId")
 
         payload = {
-            "userId": user_id,
+            "userId": userId,
             "limit": limit,
             "offset": offset
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-user-organizations",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get user's advanced balances
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :return: dict
-    :raise ValueError: if user_id is not provided
+    :raise ValueError: if userId is not provided
     
     :example:
     >>> sdk.partners_api.get_user_advanced_balance(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8",
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33"
         )
     """
 
-    def get_user_advanced_balance(self, user_id: str, organization_id: str):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
+    def get_user_advanced_balance(self, userId: str, organizationId: str):
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
+            "userId": userId,
+            "organizationId": organizationId,
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-organization-advanced-balance",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to top up the user's advance balance
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :param required str balance_id: ID of the advance balance
     :param required str amount: The amount for which the balance is replenished
     :return: dict
-    :raise ValueError: if user_id, organization_id, balance_id, amount are not provided
+    :raise ValueError: if userId, organizationId, balance_id, amount are not provided
     
     :example:
     >>> sdk.partners_api.replenish_user_balance(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8", 
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33", 
-            "a9053678-a307-4b05-9ba6-c045dea445f2", 
             "100"
         )
     """
 
     def replenish_user_balance(
             self,
-            user_id: str,
-            organization_id: str,
-            balance_id: str,
+            userId: str,
+            organizationId: str,
             amount: str
     ):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
-        check_required_field(balance_id, "balance_id")
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
         check_required_field(amount, "amount")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
-            "advancedBalanceId": balance_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "userId": userId,
+            "organizationId": organizationId,
             "amount": amount
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/top-up-advanced-balance",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get all the general rates on the service. 
     If an individual tariff is not specified for the user, then the general tariff for all users 
     is applied when the commission is deducted
     
@@ -223,213 +227,219 @@
     >>> sdk.partners_api.get_general_tariffs()
     """
 
     def get_general_tariffs(self):
         return self.sdk.request(
             "post",
             self.base_url,
-            path="/get-default-tariffs"
+            path="/get-default-tariffs",
+            api_type="partners"
         )
 
     """
     The method allows you to create or update an individual tariff.
 
     If a tariff already exists for this userId and action, then the rest of the specified d
     ata will overwrite this tariff
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :param required str action: Target action on the tariff
     :param required str amount: The commission percentage of the transaction amount (for example, 
                                 0.01 means a commission of 1% of the transaction amount)
-    :param required str tariff_type: Type of fare amount
+    :param required str type: Type of fare amount
     :param str comment: Tariff Comment
-    :param str min_amount: Minimum commission for debiting (for example, when performing an 
+    :param str minAmount: Minimum commission for debiting (for example, when performing an 
                            operation, 1% of the transaction amount will be debited, but not less 
                            than MinAmount)
-    :param str max_amount: The maximum commission for debiting (for example, when performing an 
+    :param str maxAmount: The maximum commission for debiting (for example, when performing an 
                            operation, 1% of the transaction amount will be debited, but no more 
                            than MaxAmount)
     :return: dict
-    :raise ValueError: if user_id, action, amount, tariff_type are not provided
+    :raise ValueError: if userId, action, amount, type are not provided
     
     :example:
     >>> sdk.partners_api.create_or_update_user_tariffs(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8", 
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33", 
             "INTERNAL_TRANSFER", 
             "100",
             "PERCENT"
         )
     """
 
     def create_or_update_organization_tariff(
             self,
-            user_id: str,
-            organization_id: str,
+            userId: str,
+            organizationId: str,
             action: str,
             amount: str,
-            tariff_type: str,
+            type: str,
             comment: str = None,
-            min_amount: str = None,
-            max_amount: str = None
+            minAmount: str = None,
+            maxAmount: str = None
     ):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
         check_required_field(action, "action")
         check_required_field(amount, "amount")
-        check_required_field(tariff_type, "tariff_type")
+        check_required_field(type, "type")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
+            "userId": userId,
+            "organizationId": organizationId,
             "action": action,
             "amount": amount,
-            "type": tariff_type,
+            "type": type,
             "comment": comment,
-            "minAmount": min_amount,
-            "maxAmount": max_amount
+            "minAmount": minAmount,
+            "maxAmount": maxAmount
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/set-organization-tariff",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get all individual tariffs. If an individual tariff is specified 
     for the user, the commission for the specified operation will be charged according to the 
     individual tariff
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :return: dict
-    :raise ValueError: if user_id, organization_id are not provided
+    :raise ValueError: if userId, organizationId are not provided
     
     :example:
     >>> sdk.partners_api.get_organization_tariffs(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8", 
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33"
         )
     """
 
-    def get_organization_tariffs(self, user_id: str, organization_id: str):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
+    def get_organization_tariffs(self, userId: str, organizationId: str):
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id
+            "userId": userId,
+            "organizationId": organizationId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-organization-tariffs",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to create an API key for the user
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :param required str alias: API key name
     :return: dict
-    :raise ValueError: if user_id, organization_id, alias are not provided
+    :raise ValueError: if userId, organizationId, alias are not provided
     
     :example:
     >>> sdk.partners_api.create_api_key(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8", 
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33", 
             "Integration key"
         )
     """
 
-    def create_api_key(self, user_id: str, organization_id: str, alias: str):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
+    def create_api_key(self, userId: str, organizationId: str, alias: str):
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
         check_required_field(alias, "alias")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
+            "userId": userId,
+            "organizationId": organizationId,
             "alias": alias
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/create-api-keys",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to get user's API keys
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
     :param int limit: Number of elements per page
     :param int offset: Number of items to skip
     :return: dict
-    :raise ValueError: if user_id is not provided
+    :raise ValueError: if userId is not provided
     
     :example:
     >>> sdk.partners_api.get_api_keys("8efa4a83-86c9-4eb9-899a-27ce1079a2f8")
     """
 
-    def get_api_keys(self, user_id: str, organization_id: str, limit: int = 10, offset: int = 0):
-        check_required_field(user_id, "user_id")
+    def get_api_keys(self, userId: str, organizationId: str, limit: int = 10, offset: int = 0):
+        check_required_field(userId, "userId")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
+            "userId": userId,
+            "organizationId": organizationId,
             "limit": limit,
             "offset": offset
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/get-api-keys",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     """
     The method allows you to delete the user's API key
     
-    :param required str user_id: User ID
-    :param required str organization_id: Organization ID
-    :param required str api_key_id: API key ID
+    :param required str userId: User ID
+    :param required str organizationId: Organization ID
+    :param required str keyId: API key ID
     :return: dict
-    :raise ValueError: if user_id, organization_id, api_key_id are not provided
+    :raise ValueError: if userId, organizationId, keyId are not provided
     
     :example:
     >>> sdk.partners_api.delete_api_key(
             "8efa4a83-86c9-4eb9-899a-27ce1079a2f8", 
             "e3b5315a-1de9-4b12-9c76-fb79fe4edf33", 
             "a9053678-a307-4b05-9ba6-c045dea445f2"
         )
     """
 
-    def delete_api_key(self, user_id: str, organization_id: str, api_key_id: str):
-        check_required_field(user_id, "user_id")
-        check_required_field(organization_id, "organization_id")
-        check_required_field(api_key_id, "api_key_id")
+    def delete_api_key(self, userId: str, organizationId: str, keyId: str):
+        check_required_field(userId, "userId")
+        check_required_field(organizationId, "organizationId")
+        check_required_field(keyId, "keyId")
 
         payload = {
-            "userId": user_id,
-            "organizationId": organization_id,
-            "keyId": api_key_id,
+            "userId": userId,
+            "organizationId": organizationId,
+            "keyId": keyId,
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/delete-api-keys",
-            payload=payload
+            payload=payload,
+            api_type="partners"
         )
 
     def __repr__(self):
         return "<onchainpay_sdk.PartnersApi>"
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/personal_addresses/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/personal_addresses/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,56 +9,56 @@
 
     """
     This method provides functionality of:
         - creating user
         - updating data of a previously created user when specifying the same clientId. 
           The sent parameter values overwrite the previous data.
         
-    :param required str client_id: User ID in the merchant system
-    :param str client_email: User email
-    :param str client_name: User name
-    :param str deposit_webhook_url: URL for notifications of new deposits
-    :param bool create_addresses: Create all addresses for the user
-    :param bool group_by_blockchain: Group addresses by blockchain networks 
+    :param required str clientId: User ID in the merchant system
+    :param str clientEmail: User email
+    :param str clientName: User name
+    :param str depositWebhookUrl: URL for notifications of new deposits
+    :param bool createAddresses: Create all addresses for the user
+    :param bool groupByBlockchain: Group addresses by blockchain networks 
                                     (for example, 1 address for bsc, fantom, ethereum networks). 
                                     This parameter has an effect only when createAddresses: true
-    :param bool check_risks: Check risks for every incoming transaction to the user's 
+    :param bool checkRisks: Check risks for every incoming transaction to the user's 
                              personal addresses. Information about risks will be sent in the webhook 
                              to the specified depositWebhookUrl in the risks field
     :return: dict
-    :raise ValueError: If client_id is not provided
+    :raise ValueError: If clientId is not provided
     
     :example:
     >>> sdk.personal_addresses.create_or_update_user(
             "id123",
-            client_email="user@mail.com",
-            client_name="User Name",
+            "user@mail.com",
+            "User Name",
         )
     """
 
     def create_or_update_user(
             self,
-            client_id: str,
-            client_email: str = None,
-            client_name: str = None,
-            deposit_webhook_url: str = None,
-            create_addresses: bool = None,
-            group_by_blockchain: bool = None,
-            check_risks: bool = False,
+            clientId: str,
+            clientEmail: str = None,
+            clientName: str = None,
+            depositWebhookUrl: str = None,
+            createAddresses: bool = None,
+            groupByBlockchain: bool = None,
+            checkRisks: bool = False,
     ):
-        check_required_field(client_id, "client_id")
+        check_required_field(clientId, "clientId")
 
         payload = {
-            "clientId": client_id,
-            "clientEmail": client_email,
-            "clientName": client_name,
-            "depositWebhookUrl": deposit_webhook_url,
-            "createAddresses": create_addresses,
-            "groupByBlockchain": group_by_blockchain,
-            "checkRisks": check_risks,
+            "clientId": clientId,
+            "clientEmail": clientEmail,
+            "clientName": clientName,
+            "depositWebhookUrl": depositWebhookUrl,
+            "createAddresses": createAddresses,
+            "groupByBlockchain": groupByBlockchain,
+            "checkRisks": checkRisks,
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/personal-addresses/create-user", payload=payload
         )
 
     """
@@ -69,46 +69,46 @@
         - Generate a new address for the user in the specified coin and network, when specifying 
           the parameter renewAddress. The new address will have isActive: true, previously
           generated addresses with the same coin and network will have isActive: false
     
     Note: At any time, a user can have only one active address in particular coin and network. 
     Deposits and withdrawals work at all addresses, regardless of the parameter isActive
 
-    :param required str user_id: User ID
+    :param required str id: User ID
     :param required str currency: Address coin
     :param required str network: Address network
-    :param bool renew_address: If set to true a new address will be issued to the user, 
+    :param bool renewAddress: If set to true a new address will be issued to the user, 
                                the old one will become inactive
     :return: dict
-    :raise ValueError: If user_id, currency, or network is not provided
+    :raise ValueError: If id, currency, or network is not provided
     
     :example:
     >>> sdk.personal_addresses.get_user_address(
             "463fa3c3-bc26-451a-9eb9-5cb0d7d7c5aa",
             "USDT",
             "ethereum",
         )
     """
 
     def get_user_address(
             self,
-            user_id: str,
+            id: str,
             currency: str,
             network: str,
-            renew_address: bool = False
+            renewAddress: bool = False
     ):
-        check_required_field(user_id, "user_id")
+        check_required_field(id, "id")
         check_required_field(currency, "currency")
         check_required_field(network, "network")
 
         payload = {
-            "id": user_id,
+            "id": id,
             "currency": currency,
             "network": network,
-            "renewAddress": renew_address
+            "renewAddress": renewAddress
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/personal-addresses/get-user-address", payload=payload
         )
 
     """
@@ -117,67 +117,67 @@
     addresses with isActive: true. Thus, if necessary, you can generate a new address for 
     a user in a certain coin and network, then all previous addresses in this coin and 
     network will have the parameter isActive: false (read more in the previous method 
     "Get/Renew personal address")
     
     :param int limit: Limit (for pagination)
     :param int offset: Offset (for pagination)
-    :param str user_id: Filter by User ID
-    :param bool is_active: Filter by parameter 'isActive'
+    :param str id: Filter by User ID
+    :param bool isActive: Filter by parameter 'isActive'
     :param list currency: Filter by currencies
     :param list network: Filter by networks
     :param dict balance: Filter by balance
     :return: dict
     
     :example:
     >>> sdk.personal_addresses.get_addresses(limit=10, offset=0)
     """
 
     def get_user_addresses(
             self,
-            user_id: str = None,
+            id: str = None,
             currency: list = None,
             network: list = None,
-            is_active: bool = None,
+            isActive: bool = None,
             balance: dict = None,
             limit: int = 10,
             offset: int = 0,
     ):
         payload = {
+            "id": id,
             "limit": limit,
             "offset": offset,
-            "id": user_id,
-            "isActive": is_active,
+            "isActive": isActive,
             "currency": currency,
             "network": network,
             "balance": balance
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/personal-addresses/get-user-addresses", payload=payload
         )
 
     """
     The method allows you to get user data by his id or clientId
     
-    :param str user_id: User ID in the system. Required, if 'clientId' was not provided
-    :param str client_id: User ID in the merchant system. Required, if 'id' was not provided
+    :param str id: User ID in the system. Required, if 'clientId' was not provided
+    :param str clientId: User ID in the merchant system. Required, if 'id' was not provided
     :return: dict
     
     :example:
     >>> sdk.personal_addresses.get_user("463fa3c3-bc26-451a-9eb9-5cb0d7d7c5aa")
     """
 
-    def get_user(self, user_id: str = None, client_id: str = None):
-        if not user_id and not client_id:
-            raise ValueError("user_id or client_id is required")
+    def get_user(self, id: str = None, clientId: str = None):
+        if not id and not clientId:
+            raise ValueError("id or clientId is required")
 
         payload = {
-            "id": user_id,
-            "clientId": client_id
+            "id": id,
+            "clientId": clientId
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/personal-addresses/get-user", payload=payload
         )
 
     def __repr__(self):
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/recurring_payments/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/recurring_payments/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,170 +8,170 @@
         self.sdk = sdk
 
     """
     The method creates a temporary link to connect the user. The user must follow the link and 
     give permission to spend coins from his address. After that, you will receive a webhook with 
     the status and payment link ID
     
-    :param required str merchant_id: Merchant ID in the system
-    :param required str client_id: Client ID in the merchant system
-    :param required str client_email: Client's mail in the merchant's system
-    :param str client_name: Client name in the merchant system
-    :param str return_url: URL to be used as "Return to Store" link
-    :param str webhook_url: URL to notify about connecting or denying a client's connection request
+    :param required str merchantId: Merchant ID in the system
+    :param required str clientId: Client ID in the merchant system
+    :param required str clientEmail: Client's mail in the merchant's system
+    :param str clientName: Client name in the merchant system
+    :param str returnUrl: URL to be used as "Return to Store" link
+    :param str webhookUrl: URL to notify about connecting or denying a client's connection request
     :return: dict
-    :raise ValueError: if merchant_id, client_id or client_email is not provided    
+    :raise ValueError: if merchantId, clientId or clientEmail is not provided    
     
     :example:
     >>> sdk.recurring_payments.create_payment_link(
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a", 
             "id1234", 
             "maiL@example.com",
         )
     """
 
     def create_payment_link(
             self,
-            merchant_id: str,
-            client_id: str,
-            client_email: str,
-            client_name: str = None,
-            return_url: str = None,
-            webhook_url: str = None,
+            merchantId: str,
+            clientId: str,
+            clientEmail: str,
+            clientName: str = None,
+            returnUrl: str = None,
+            webhookUrl: str = None,
     ):
-        check_required_field(merchant_id, "merchant_id")
-        check_required_field(client_id, "client_id")
-        check_required_field(client_email, "client_email")
+        check_required_field(merchantId, "merchantId")
+        check_required_field(clientId, "clientId")
+        check_required_field(clientEmail, "clientEmail")
 
         payload = {
-            "merchantId": merchant_id,
-            "clientId": client_id,
-            "clientEmail": client_email,
-            "clientName": client_name,
-            "returnUrl": return_url,
-            "webhookUrl": webhook_url
+            "merchantId": merchantId,
+            "clientId": clientId,
+            "clientEmail": clientEmail,
+            "clientName": clientName,
+            "returnUrl": returnUrl,
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/create-subscriber-billing-link",
             payload=payload
         )
 
     """
     The method allows you to get payment link data
     
-    :param required str payment_link_id: ID of the payment link in the system
-    :param required str merchant_id: Merchant ID in the system
+    :param required str id: ID of the payment link in the system
+    :param required str merchantId: Merchant ID in the system
     :return: dict
-    :raise ValueError: if payment_link_id or merchant_id is not provided
+    :raise ValueError: if id or merchantId is not provided
     
     :example:
     >>> sdk.recurring_payments.get_payment_link(
         "d56bcbe4-586f-4980-b6ca-6e9f557750e8", 
         "672c1e2d-354f-49a1-8a5b-75af87e92f0a"
     )
     """
 
-    def get_payment_link(self, payment_link_id: str, merchant_id: str):
-        check_required_field(payment_link_id, "payment_link_id")
-        check_required_field(merchant_id, "merchant_id")
+    def get_payment_link(self, id: str, merchantId: str):
+        check_required_field(id, "id")
+        check_required_field(merchantId, "merchantId")
 
         payload = {
-            "id": payment_link_id,
-            "merchantId": merchant_id
+            "id": id,
+            "merchantId": merchantId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/get-billing-link",
             payload=payload
         )
 
     """
     The method allows you to get a list of payment links for a specific user
     
-    :param required str merchant_id: Merchant ID in the system
-    :param str client_id: Client ID in the merchant system
-    :param str client_email: Client's mail in the merchant's system
+    :param required str merchantId: Merchant ID in the system
+    :param str clientId: Client ID in the merchant system
+    :param str clientEmail: Client's mail in the merchant's system
     :return: dict
-    :raise ValueError: if merchant_id is not provided
+    :raise ValueError: if merchantId is not provided
     
     :example:
     >>> sdk.recurring_payments.get_payment_links("672c1e2d-354f-49a1-8a5b-75af87e92f0a")
     """
 
-    def get_payment_links(self, merchant_id: str, client_id: str = None, client_email: str = None):
-        check_required_field(merchant_id, "merchant_id")
+    def get_payment_links(self, merchantId: str, clientId: str = None, clientEmail: str = None):
+        check_required_field(merchantId, "merchantId")
 
         payload = {
-            "merchantId": merchant_id,
-            "clientId": client_id,
-            "clientEmail": client_email
+            "merchantId": merchantId,
+            "clientId": clientId,
+            "clientEmail": clientEmail
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/get-billing-links-by-subscriber",
             payload=payload
         )
 
     """
     The method allows you to disable the payment link. You will no longer be able to connect 
     subscriptions and make payments using this payment link
     
-    :param required str payment_link_id: ID of the payment link in the system
-    :param required str merchant_id: Merchant ID in the system
+    :param required str id: ID of the payment link in the system
+    :param required str merchantId: Merchant ID in the system
     :return: dict
-    :raise ValueError: if payment_link_id or merchant_id is not provided
+    :raise ValueError: if id or merchantId is not provided
     
     :example:
     >>> sdk.recurring_payments.disable_payment_link(
             "d56bcbe4-586f-4980-b6ca-6e9f557750e8", 
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a"
         )
     """
 
-    def disable_payment_link(self, payment_link_id: str, merchant_id: str):
-        check_required_field(payment_link_id, "payment_link_id")
-        check_required_field(merchant_id, "merchant_id")
+    def disable_payment_link(self, id: str, merchantId: str):
+        check_required_field(id, "id")
+        check_required_field(merchantId, "merchantId")
 
         payload = {
-            "id": payment_link_id,
-            "merchantId": merchant_id
+            "id": id,
+            "merchantId": merchantId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/disable-subscriber-billing-link",
             payload=payload
         )
 
     """
     The method allows you to connect a subscription
     
-    :param required str merchant_id: Merchant ID in the system
-    :param required str billing_link_id: Payment link identifier 
+    :param required str merchantId: Merchant ID in the system
+    :param required str billingLinkId: Payment link identifier 
                                          (coins will be debited from the linked address)
     :param required str title: Subscription name
-    :param required int spend_interval: Write-off period in minutes. For convenience, 
+    :param required int spendInterval: Write-off period in minutes. For convenience, 
                                         you can specify: -1 - daily write-off; 
                                         -2 - weekly write-off; -3 - monthly write-off;
     :param required str currency: Payment currency. You can specify a fiat currency or any other, 
                                   the amount will be automatically converted to the currency of 
                                   the payment link
     :param required str amount: Payment amount in the specified currency
     :param str description: Subscription description
-    :param str webhook_url: Subscription charge notification URL
+    :param str webhookUrl: Subscription charge notification URL
     :return: dict
-    :raise ValueError: if merchant_id, billing_link_id, title, spend_interval, currency or amount 
+    :raise ValueError: if merchantId, billingLinkId, title, spendInterval, currency or amount 
                        is not provided
     
     :example:
     >>> sdk.recurring_payments.create_subscription(
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a", 
             "2bfbdf44-fb5b-4e75-9962-f28c0594e483", 
             "Premium", 
@@ -179,146 +179,146 @@
             "USD", 
             "100"
         )
     """
 
     def create_subscription(
             self,
-            merchant_id: str,
-            billing_link_id: str,
+            merchantId: str,
+            billingLinkId: str,
             title: str,
-            spend_interval: int,
+            spendInterval: int,
             currency: str,
             amount: str,
             description: str = None,
-            webhook_url: str = None,
+            webhookUrl: str = None,
     ):
-        check_required_field(merchant_id, "merchant_id")
-        check_required_field(billing_link_id, "billing_link_id")
+        check_required_field(merchantId, "merchantId")
+        check_required_field(billingLinkId, "billingLinkId")
         check_required_field(title, "title")
-        check_required_field(spend_interval, "spend_interval")
+        check_required_field(spendInterval, "spendInterval")
         check_required_field(currency, "currency")
         check_required_field(amount, "amount")
 
         payload = {
-            "merchantId": merchant_id,
-            "billingLinkId": billing_link_id,
+            "merchantId": merchantId,
+            "billingLinkId": billingLinkId,
             "title": title,
-            "spendInterval": spend_interval,
+            "spendInterval": spendInterval,
             "currency": currency,
             "amount": amount,
             "description": description,
-            "webhookUrl": webhook_url
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/create-subscription",
             payload=payload
         )
 
     """
     The method allows you to get information about the subscription
     
-    :param required str subscription_id: Subscription ID in the system
-    :param required str merchant_id: Merchant ID in the system
+    :param required str id: Subscription ID in the system
+    :param required str merchantId: Merchant ID in the system
     :return: dict
-    :raise ValueError: if subscription_id or merchant_id is not provided
+    :raise ValueError: if id or merchantId is not provided
     
     :example:
     >>> sdk.recurring_payments.get_subscription(
             "be1179ff-586f-4980-b6ca-7e11a93bb99f", 
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a"
         )
     """
 
-    def get_subscription(self, subscription_id: str, merchant_id: str):
-        check_required_field(subscription_id, "subscription_id")
-        check_required_field(merchant_id, "merchant_id")
+    def get_subscription(self, id: str, merchantId: str):
+        check_required_field(id, "id")
+        check_required_field(merchantId, "merchantId")
 
         payload = {
-            "id": subscription_id,
-            "merchantId": merchant_id
+            "id": id,
+            "merchantId": merchantId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/get-subscription",
             payload=payload
         )
 
     """
     The method allows you to disable a previously connected subscription
     
-    :param required str subscription_id: Subscription ID in the system
-    :param required str merchant_id: Merchant ID in the system
+    :param required str id: Subscription ID in the system
+    :param required str merchantId: Merchant ID in the system
     :return: dict
-    :raise ValueError: if subscription_id or merchant_id is not provided
+    :raise ValueError: if id or merchantId is not provided
     
     :example:
     >>> sdk.recurring_payments.cancel_subscription(
             "be1179ff-586f-4980-b6ca-7e11a93bb99f", 
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a"
         )
     """
 
-    def cancel_subscription(self, subscription_id: str, merchant_id: str):
-        check_required_field(subscription_id, "subscription_id")
-        check_required_field(merchant_id, "merchant_id")
+    def cancel_subscription(self, id: str, merchantId: str):
+        check_required_field(id, "id")
+        check_required_field(merchantId, "merchantId")
 
         payload = {
-            "id": subscription_id,
-            "merchantId": merchant_id
+            "id": id,
+            "merchantId": merchantId
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/cancel-subscription",
             payload=payload
         )
 
     """
     The method allows you to create a payment with an arbitrary amount in the coin in which 
     the address was connected
     
-    :param required str merchant_id: Merchant ID in the system
-    :param required str billing_link_id: Payment link identifier 
+    :param required str merchantId: Merchant ID in the system
+    :param required str billingLinkId: Payment link identifier 
                                          (coins will be debited from the linked address)
     :param required str amount: Payment amount
-    :param str webhook_url: Payment notification URL
+    :param str webhookUrl: Payment notification URL
     :return: dict
-    :raise ValueError: if merchant_id, billing_link_id or amount is not provided
+    :raise ValueError: if merchantId, billingLinkId or amount is not provided
     
     :example:
     >>> sdk.recurring_payments.create_payment(
             "672c1e2d-354f-49a1-8a5b-75af87e92f0a", 
             "2bfbdf44-fb5b-4e75-9962-f28c0594e483", 
             "100"
         )
     """
 
     def create_payment(
             self,
-            merchant_id: str,
-            billing_link_id: str,
+            merchantId: str,
+            billingLinkId: str,
             amount: str,
-            webhook_url: str = None
+            webhookUrl: str = None
     ):
-        check_required_field(merchant_id, "merchant_id")
-        check_required_field(billing_link_id, "billing_link_id")
+        check_required_field(merchantId, "merchantId")
+        check_required_field(billingLinkId, "billingLinkId")
         check_required_field(amount, "amount")
 
         payload = {
-            "merchantId": merchant_id,
-            "billingLinkId": billing_link_id,
+            "merchantId": merchantId,
+            "billingLinkId": billingLinkId,
             "amount": amount,
-            "webhookUrl": webhook_url
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post",
             self.base_url,
             path="/recurrents/make-payment",
             payload=payload
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/domains/withdraws/__init__.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/domains/withdraws/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,176 +6,163 @@
     def __init__(self, sdk: Client, base_url):
         self.base_url = base_url
         self.sdk = sdk
 
     """
     The method allows you to get data on the commission that will be debited during the withdrawal
     
-    :param required str balance_id: Identifier of the advance balance from which the commission 
-                                    will be paid
-    :param required str address_id: Identifier of the address from which you want to withdraw
+    :param required str addressId: Identifier of the address from which you want to withdraw
     :param required str amount: Amount you want to withdraw
     :param bool native: Deduct the gas fee (network fee) from the native balance of the address 
                         (available for payment addresses, PAY_OUT type)
     :return: dict
-    :raise ValueError: If balance_id, address_id, or amount is not provided
+    :raise ValueError: If addressId, or amount is not provided
     
     :example:
-    >>> sdk.withdraws.get_commission(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
+    >>> sdk.withdraws.get_commission_token(
             "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
             "2"
         )
     """
 
     def get_commission_token(
             self,
-            balance_id: str,
-            address_id: str,
+            addressId: str,
             amount: str,
             native: bool = None
-            ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(address_id, "address_id")
+    ):
+        check_required_field(addressId, "addressId")
         check_required_field(amount, "amount")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "addressId": address_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "addressId": addressId,
             "amount": amount,
             "native": native,
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/withdrawal-fee-token", payload=payload
         )
 
     """
     The method allows you to create a request to withdraw coins from an address
     
-    :param required str balance_id: Identifier of the advance balance for writing off commissions
-    :param required str address_id: Identifier of the address from which the coins 
+    :param required str addressId: Identifier of the address from which the coins 
                                     should be withdrawn
     :param required str address: Address for sending coins
     :param required str amount: Withdrawal amount
-    :param required str fee_token: Fee token that was not created when requesting /request-fee
+    :param required str feeToken: Fee token that was not created when requesting /request-fee
     :param str tag: Tag (memo) address (relevant for networks that support the tag, such as Ripple)
     :return: dict
-    :raise ValueError: If balance_id, address_id, address, amount, or fee_token is not provided
+    :raise ValueError: If addressId, address, amount, or feeToken is not provided
     
     :example:
     >>> sdk.withdraws.create_withdrawal(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
             "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
             "0x5b8b7b4b4a2f6c8a6e0b2f2f8e5b2b1c5c6b1c5b",
             "2",
             "0x00000005707Bf50EfA35a2db020eDe9Ac0780b9f"
         )
     """
 
     def create_withdrawal(
             self,
-            balance_id: str,
-            address_id: str,
+            addressId: str,
             address: str,
             amount: str,
-            fee_token: str,
+            feeToken: str,
             tag: str = None
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(address_id, "address_id")
+        check_required_field(addressId, "addressId")
         check_required_field(address, "address")
         check_required_field(amount, "amount")
-        check_required_field(fee_token, "fee_token")
+        check_required_field(feeToken, "feeToken")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "addressId": address_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "addressId": addressId,
             "address": address,
             "amount": amount,
-            "feeToken": fee_token,
+            "feeToken": feeToken,
             "tag": tag
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/make-withdrawal", payload=payload
         )
 
     """
     The method allows you to create a request to withdraw coins from an address and get the 
     execution result to the specified URL
 
-    :param required str balance_id: Identifier of the advance balance for writing off commissions
-    :param required str address_id: Identifier of the address from which the coins 
+    :param required str addressId: Identifier of the address from which the coins 
                                     should be withdrawn
     :param required str address: Address for sending coins
     :param required str amount: Withdrawal amount
-    :param required str fee_token: Fee token that was not created when requesting /request-fee
+    :param required str feeToken: Fee token that was not created when requesting /request-fee
     :param str tag: Tag (memo) address (relevant for networks that support the tag, such as Ripple)
     :return: dict
-    :raise ValueError: If balance_id, address_id, address, amount, or fee_token is not provided
+    :raise ValueError: If addressId, address, amount, or feeToken is not provided
 
     :example:
     >>> sdk.withdraws.create_withdrawal(
-            "ba5716df-58c4-48f8-9401-68f6069fb4ff",
             "8e2d5033-139f-46d4-b769-4a2d2cee37c4",
             "0x5b8b7b4b4a2f6c8a6e0b2f2f8e5b2b1c5c6b1c5b",
             "2",
             "0x00000005707Bf50EfA35a2db020eDe9Ac0780b9f",
             "no-tag",
             "https://webhook.site/4e5e1d6b-4c6b-4c6b-4c6b-4c6b4c6b4c6b"
         )
     """
 
     def create_async_withdrawal(
             self,
-            balance_id: str,
-            address_id: str,
+            addressId: str,
             address: str,
             amount: str,
-            fee_token: str,
+            feeToken: str,
             tag: str = None,
-            webhook_url: str = None
+            webhookUrl: str = None
     ):
-        check_required_field(balance_id, "balance_id")
-        check_required_field(address_id, "address_id")
+        check_required_field(addressId, "addressId")
         check_required_field(address, "address")
         check_required_field(amount, "amount")
-        check_required_field(fee_token, "fee_token")
+        check_required_field(feeToken, "feeToken")
 
         payload = {
-            "advancedBalanceId": balance_id,
-            "addressId": address_id,
+            "advancedBalanceId": self.sdk._advancedBalanceId,
+            "addressId": addressId,
             "address": address,
             "amount": amount,
-            "feeToken": fee_token,
+            "feeToken": feeToken,
             "tag": tag,
-            "webhookUrl": webhook_url
+            "webhookUrl": webhookUrl
         }
 
         return self.sdk.request(
             "post", self.base_url, path="/make-withdrawal-async", payload=payload
         )
 
     """
     The method allows you to get information about the output
     
-    :param str withdrawal_id: Withdrawal ID in the system
+    :param str withdrawalId: Withdrawal ID in the system
     :return: dict
-    :raise ValueError: If withdrawal_id is not provided
+    :raise ValueError: If withdrawalId is not provided
     
     :example:
     >>> sdk.withdraws.get_withdrawal_by_id("bd6631c2-7f8f-4509-ba4c-418b899465be")
     """
 
-    def get_withdrawal_by_id(self, withdrawal_id: str):
-        check_required_field(withdrawal_id, "withdrawal_id")
+    def get_withdrawal_by_id(self, withdrawalId: str):
+        check_required_field(withdrawalId, "withdrawalId")
 
         payload = {
-            "withdrawalId": withdrawal_id
+            "withdrawalId": withdrawalId
         }
 
         return self.sdk.request(
             "get", self.base_url, path="/get-withdrawal", payload=payload
         )
 
     def __repr__(self):
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/requester.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/requester.py`

 * *Files identical despite different names*

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk/resources/utils.py` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk/resources/utils.py`

 * *Files identical despite different names*

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/PKG-INFO` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onchainpay_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for onchainpay.io API
 Home-page: https://github.com/onchainpay/onchainpay_sdk
 Author: onchainpay.io Team
 Author-email: hello@onchainpay.io
 Project-URL: Bug Tracker, https://github.com/onchainpay/onchainpay_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `onchainpay_sdk-0.0.1/src/onchainpay_sdk.egg-info/SOURCES.txt` & `onchainpay_sdk-0.0.2/src/onchainpay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

