# Comparing `tmp/pytonapi-0.2.4b2.tar.gz` & `tmp/pytonapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.2.4b2.tar", last modified: Sun Apr 21 20:36:05 2024, max compression
+gzip compressed data, was "pytonapi-0.2.5.tar", last modified: Tue Apr 23 00:03:01 2024, max compression
```

## Comparing `pytonapi-0.2.4b2.tar` & `pytonapi-0.2.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.392751 pytonapi-0.2.4b2/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5379 2024-04-21 20:36:05.392751 pytonapi-0.2.4b2/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.376751 pytonapi-0.2.4b2/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.376751 pytonapi-0.2.4b2/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9500 2024-04-21 20:29:39.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.380751 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2618 2024-04-20 20:10:31.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2349 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/websocket.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2174 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.388751 pytonapi-0.2.4b2/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/_address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/_balance.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.4b2/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.388751 pytonapi-0.2.4b2/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.4b2/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.392751 pytonapi-0.2.4b2/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4324 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2313 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.4b2/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-21 20:36:05.376751 pytonapi-0.2.4b2/pytonapi.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5379 2024-04-21 20:36:05.000000 pytonapi-0.2.4b2/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     2165 2024-04-21 20:36:05.000000 pytonapi-0.2.4b2/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-21 20:36:05.000000 pytonapi-0.2.4b2/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-21 20:36:05.000000 pytonapi-0.2.4b2/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-21 20:36:05.000000 pytonapi-0.2.4b2/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-21 20:36:05.392751 pytonapi-0.2.4b2/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      972 2024-04-21 20:35:03.000000 pytonapi-0.2.4b2/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.965819 pytonapi-0.2.5/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.5/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-23 00:03:01.965819 pytonapi-0.2.5/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.5/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.957818 pytonapi-0.2.5/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.957818 pytonapi-0.2.5/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9657 2024-04-22 23:59:07.000000 pytonapi-0.2.5/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.957818 pytonapi-0.2.5/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3760 2024-04-22 23:46:18.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2349 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/async_tonapi/methods/websocket.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-22 23:25:05.000000 pytonapi-0.2.5/pytonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.961818 pytonapi-0.2.5/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/_address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/_balance.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.5/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.961818 pytonapi-0.2.5/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.5/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.965819 pytonapi-0.2.5/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4324 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2313 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.5/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 00:03:01.957818 pytonapi-0.2.5/pytonapi.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-23 00:03:01.000000 pytonapi-0.2.5/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2165 2024-04-23 00:03:01.000000 pytonapi-0.2.5/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-23 00:03:01.000000 pytonapi-0.2.5/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-23 00:03:01.000000 pytonapi-0.2.5/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-23 00:03:01.000000 pytonapi-0.2.5/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-23 00:03:01.965819 pytonapi-0.2.5/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      970 2024-04-23 00:01:42.000000 pytonapi-0.2.5/setup.py
```

### Comparing `pytonapi-0.2.4b2/LICENSE` & `pytonapi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/PKG-INFO` & `pytonapi-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.4b2
+Version: 0.2.5
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.4b2/README.md` & `pytonapi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/client.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from pytonapi.exceptions import (
     TONAPIBadRequestError,
     TONAPIError,
     TONAPIInternalServerError,
     TONAPINotFoundError,
     TONAPIUnauthorizedError,
     TONAPITooManyRequestsError,
-    TONAPINotImplementedError
+    TONAPINotImplementedError,
+    TONAPISSEError,
 )
 
 
 class AsyncTonapiClient:
     """
     Asynchronous TON API Client.
     """
@@ -64,14 +65,16 @@
             data = await response.aread()
             try:
                 content = json.loads(data.decode())
             except json.JSONDecodeError:
                 content = data.decode()
         except httpx.ResponseNotRead:
             content = {"error": response.text}
+        except httpx.ReadError as read_error:
+            content = {"error": f"Read error occurred: {read_error}"}
         except Exception as e:
             raise TONAPIError(f"Failed to read response content: {e}")
 
         return content
 
     async def __process_response(self, response: httpx.Response) -> Dict[str, Any]:
         """
@@ -114,27 +117,29 @@
         timeout = httpx.Timeout(timeout=self.timeout)
         data = {"headers": self.headers, "params": params, "timeout": timeout}
 
         async with httpx.AsyncClient() as client:
             try:
                 async with client.stream("GET", url=url, **data) as response:
                     response: httpx.Response
-                    if response.status_code != 200:
-                        await self.__process_response(response)
+                    response.raise_for_status()
+
                     async for line in response.aiter_lines():
                         try:
                             key, value = line.split(": ", 1)
                         except ValueError:
                             continue
                         if value == "heartbeat":
                             continue
                         if key == "data":
                             yield value
             except httpx.LocalProtocolError:
                 raise TONAPIUnauthorizedError
+            except httpx.HTTPStatusError as e:
+                raise TONAPISSEError(e)
 
     async def _subscribe_websocket(
             self,
             method: str,
             params: Any,
     ) -> AsyncGenerator[Dict[str, Any], None]:
         """
```

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/__init__.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/emulate.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/events.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/inscriptions.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/jettons.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/liteserver.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/rates.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/sse.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/sse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 import json
-from typing import List, Callable, Any, Awaitable, Tuple
+from typing import List, Callable, Any, Tuple
 
-from pytonapi.async_tonapi.client import AsyncTonapiClient
 from pytonapi.schema.events import TransactionEventData, TraceEventData, MempoolEventData
+from pytonapi.tonapi import TonapiClient
 
 
-class SSEMethod(AsyncTonapiClient):
+class SSEMethod(TonapiClient):
 
-    async def subscribe_to_transactions(
+    def subscribe_to_transactions(
             self,
             accounts: List[str],
-            handler: Callable[[TransactionEventData, ...], Awaitable[Any]],
+            handler: Callable[[TransactionEventData, ...], Any],
             args: Tuple[Any, ...] = (),
-    ) -> Any:
+    ) -> None:
         """
         Subscribes to transactions SSE events for the specified accounts.
 
         :param handler: A callable function to handle the SSEEvent
         :param accounts: A list of account addresses to subscribe to
         :param args: Additional arguments to pass to the handler
         """
         method = "v2/sse/accounts/transactions"
         params = {'accounts': accounts}
-        async for data in self._subscribe(method=method, params=params):
+        for data in self._subscribe(method=method, params=params):
             event = TransactionEventData(**json.loads(data))
-            result = await handler(event, *args)
-            if result is not None:
-                return result
+            handler(event, *args)
 
-    async def subscribe_to_traces(
+    def subscribe_to_traces(
             self,
             accounts: List[str],
-            handler: Callable[[TraceEventData, ...], Awaitable[Any]],
+            handler: Callable[[TraceEventData, ...], Any],
             args: Tuple[Any, ...] = (),
-    ) -> Any:
+    ) -> None:
         """
         Subscribes to traces SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
+
+        Returns:
+            None
         """
         method = "v2/sse/accounts/traces"
         params = {'accounts': accounts}
-        async for data in self._subscribe(method=method, params=params):
+        for data in self._subscribe(method=method, params=params):
             event = TraceEventData(**json.loads(data))
-            result = await handler(event, *args)
-            if result is not None:
-                return result
+            handler(event, *args)
 
-    async def subscribe_to_mempool(
+    def subscribe_to_mempool(
             self,
             accounts: List[str],
-            handler: Callable[[MempoolEventData, ...], Awaitable[Any]],
+            handler: Callable[[MempoolEventData, ...], Any],
             args: Tuple[Any, ...] = (),
-    ) -> Any:
+    ) -> None:
         """
         Subscribes to mempool SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
         """
         method = "v2/sse/mempool"
         params = {'accounts': accounts}
-        async for data in self._subscribe(method=method, params=params):
+        for data in self._subscribe(method=method, params=params):
             event = MempoolEventData(**json.loads(data))
-            result = await handler(event, *args)
-            if result is not None:
-                return result
+            handler(event, *args)
```

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/staking.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/tonconnect.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/wallet.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/async_tonapi/methods/websocket.py` & `pytonapi-0.2.5/pytonapi/async_tonapi/methods/websocket.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/exceptions.py` & `pytonapi-0.2.5/pytonapi/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,19 @@
             raise TONAPISSELimitReachedError(text)
         super().__init__(
             "API key is missing or invalid. "
             "You can get an access token here https://tonconsole.com/"
         )
 
 
-class TONAPISSELimitReachedError(TONAPIClientError):
+class TONAPISSEError(TONAPIServerError):
+    """Raised when the server encounters an error (HTTP 4xx)."""
+
+
+class TONAPISSELimitReachedError(TONAPISSEError):
     """Raises when the limit of streaming connections is reached (HTTP 401)."""
 
 
 class TONAPINotFoundError(TONAPIClientError):
     """Raised when the requested resource is not found (HTTP 404)."""
```

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/__init__.py` & `pytonapi-0.2.5/pytonapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/_address.py` & `pytonapi-0.2.5/pytonapi/schema/_address.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/_balance.py` & `pytonapi-0.2.5/pytonapi/schema/_balance.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/accounts.py` & `pytonapi-0.2.5/pytonapi/schema/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/blockchain.py` & `pytonapi-0.2.5/pytonapi/schema/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/dns.py` & `pytonapi-0.2.5/pytonapi/schema/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/events.py` & `pytonapi-0.2.5/pytonapi/schema/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/jettons.py` & `pytonapi-0.2.5/pytonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/liteserver.py` & `pytonapi-0.2.5/pytonapi/schema/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/nft.py` & `pytonapi-0.2.5/pytonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/staking.py` & `pytonapi-0.2.5/pytonapi/schema/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/schema/traces.py` & `pytonapi-0.2.5/pytonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/__init__.py` & `pytonapi-0.2.5/pytonapi/tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/client.py` & `pytonapi-0.2.5/pytonapi/tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/__init__.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/emulate.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/events.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/inscriptions.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/jettons.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/liteserver.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/rates.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/staking.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/tonconnect.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/tonapi/methods/wallet.py` & `pytonapi-0.2.5/pytonapi/tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi/utils.py` & `pytonapi-0.2.5/pytonapi/utils.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.2.5/pytonapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.4b2
+Version: 0.2.5
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.4b2/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.2.5/pytonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.4b2/setup.py` & `pytonapi-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.2.4b2",
+    version="0.2.5",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tonkeeper/pytonapi/",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
     install_requires=[
```

