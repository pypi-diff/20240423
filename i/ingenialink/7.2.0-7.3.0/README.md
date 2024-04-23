# Comparing `tmp/ingenialink-7.2.0.tar.gz` & `tmp/ingenialink-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingenialink-7.2.0.tar", last modified: Tue Mar 12 17:01:21 2024, max compression
+gzip compressed data, was "ingenialink-7.3.0.tar", last modified: Tue Apr 23 09:31:12 2024, max compression
```

## Comparing `ingenialink-7.2.0.tar` & `ingenialink-7.3.0.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.915103 ingenialink-7.2.0/
--rw-rw-rw-   0        0        0    17630 2024-03-12 17:00:07.000000 ingenialink-7.2.0/LICENSE.md
--rw-rw-rw-   0        0        0       35 2024-03-12 17:00:07.000000 ingenialink-7.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2586 2024-03-12 17:01:21.915103 ingenialink-7.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2024-03-12 17:00:07.000000 ingenialink-7.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.852614 ingenialink-7.2.0/ingenialink/
--rw-rw-rw-   0        0        0     1410 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.868236 ingenialink-7.2.0/ingenialink/bin/
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.868236 ingenialink-7.2.0/ingenialink/bin/FoE/
--rw-rw-rw-   0        0        0       23 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/bin/FoE/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.868236 ingenialink-7.2.0/ingenialink/bin/FoE/win_64x/
--rwxrwxrwx   0        0        0    44032 2024-03-12 16:59:25.000000 ingenialink-7.2.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/bin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.868236 ingenialink-7.2.0/ingenialink/canopen/
--rw-rw-rw-   0        0        0       90 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/canopen/__init__.py
--rw-rw-rw-   0        0        0     2080 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/canopen/dictionary.py
--rw-rw-rw-   0        0        0    38262 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/canopen/network.py
--rw-rw-rw-   0        0        0     2587 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/canopen/register.py
--rw-rw-rw-   0        0        0     5550 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/canopen/servo.py
--rw-rw-rw-   0        0        0     1008 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/constants.py
--rw-rw-rw-   0        0        0    14937 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/dictionary.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.868236 ingenialink-7.2.0/ingenialink/enums/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/enums/__init__.py
--rw-rw-rw-   0        0        0     1207 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/enums/register.py
--rw-rw-rw-   0        0        0     2892 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/enums/servo.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.883834 ingenialink-7.2.0/ingenialink/eoe/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/eoe/__init__.py
--rw-rw-rw-   0        0        0    13559 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/eoe/network.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.883834 ingenialink-7.2.0/ingenialink/ethercat/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethercat/__init__.py
--rw-rw-rw-   0        0        0     2720 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethercat/dictionary.py
--rw-rw-rw-   0        0        0    17220 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethercat/network.py
--rw-rw-rw-   0        0        0      114 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethercat/register.py
--rw-rw-rw-   0        0        0    11758 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethercat/servo.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.883834 ingenialink-7.2.0/ingenialink/ethernet/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethernet/__init__.py
--rw-rw-rw-   0        0        0     2481 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethernet/dictionary.py
--rw-rw-rw-   0        0        0    11825 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethernet/network.py
--rw-rw-rw-   0        0        0     2535 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethernet/register.py
--rw-rw-rw-   0        0        0     6266 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/ethernet/servo.py
--rw-rw-rw-   0        0        0     3572 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/exceptions.py
--rw-rw-rw-   0        0        0     2412 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/network.py
--rw-rw-rw-   0        0        0    17736 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/pdo.py
--rw-rw-rw-   0        0        0     8024 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/poller.py
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/py.typed
--rw-rw-rw-   0        0        0     7931 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/register.py
--rw-rw-rw-   0        0        0    45657 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/servo.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.899494 ingenialink-7.2.0/ingenialink/utils/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/__init__.py
--rw-rw-rw-   0        0        0     8356 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/_utils.py
--rw-rw-rw-   0        0        0     4486 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/constants.py
--rw-rw-rw-   0        0        0      684 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/errors.py
--rw-rw-rw-   0        0        0     7327 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/mcb.py
--rw-rw-rw-   0        0        0     4337 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/utils/udp.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.899494 ingenialink-7.2.0/ingenialink/virtual/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/virtual/__init__.py
--rw-rw-rw-   0        0        0     2844 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/virtual/dictionary.py
--rw-rw-rw-   0        0        0     2094 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/virtual/network.py
--rw-rw-rw-   0        0        0      338 2024-03-12 17:00:07.000000 ingenialink-7.2.0/ingenialink/virtual/servo.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.915103 ingenialink-7.2.0/ingenialink.egg-info/
--rw-rw-rw-   0        0        0     2586 2024-03-12 17:01:21.000000 ingenialink-7.2.0/ingenialink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1780 2024-03-12 17:01:21.000000 ingenialink-7.2.0/ingenialink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 17:01:21.000000 ingenialink-7.2.0/ingenialink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2024-03-12 17:01:21.000000 ingenialink-7.2.0/ingenialink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-03-12 17:01:21.000000 ingenialink-7.2.0/ingenialink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2024-03-12 17:00:07.000000 ingenialink-7.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 17:01:21.915103 ingenialink-7.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1775 2024-03-12 17:00:07.000000 ingenialink-7.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.899494 ingenialink-7.2.0/tests/
--rw-rw-rw-   0        0        0     2314 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_dictionary.py
--rw-rw-rw-   0        0        0     3157 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_mcb.py
--rw-rw-rw-   0        0        0     5358 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_register.py
--rw-rw-rw-   0        0        0    16975 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_servo.py
--rw-rw-rw-   0        0        0      914 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_utils.py
--rw-rw-rw-   0        0        0     7966 2024-03-12 17:00:07.000000 ingenialink-7.2.0/tests/test_virtual_drive.py
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.915103 ingenialink-7.2.0/virtual_drive/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/virtual_drive/__init__.py
--rw-rw-rw-   0        0        0    67232 2024-03-12 17:00:07.000000 ingenialink-7.2.0/virtual_drive/core.py
--rw-rw-rw-   0        0        0        0 2024-03-12 17:00:07.000000 ingenialink-7.2.0/virtual_drive/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-12 17:01:21.915103 ingenialink-7.2.0/virtual_drive/resources/
--rw-rw-rw-   0        0        0    29066 2024-03-12 17:00:07.000000 ingenialink-7.2.0/virtual_drive/resources/virtual_drive.xcf
--rw-rw-rw-   0        0        0   267654 2024-03-12 17:00:07.000000 ingenialink-7.2.0/virtual_drive/resources/virtual_drive.xdf
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/
+-rw-rw-rw-   0        0        0    17630 2024-04-23 09:30:10.000000 ingenialink-7.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0       35 2024-04-23 09:30:10.000000 ingenialink-7.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2586 2024-04-23 09:31:12.681591 ingenialink-7.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2024-04-23 09:30:10.000000 ingenialink-7.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/
+-rw-rw-rw-   0        0        0     1414 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/
+-rw-rw-rw-   0        0        0       23 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/bin/FoE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/linux/
+-rw-rw-rw-   0        0        0   148512 2024-04-23 09:24:47.000000 ingenialink-7.3.0/ingenialink/bin/FoE/linux/FoEUpdateFirmware
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/
+-rwxrwxrwx   0        0        0    44032 2024-04-23 09:24:47.000000 ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/bin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.634695 ingenialink-7.3.0/ingenialink/canopen/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/__init__.py
+-rw-rw-rw-   0        0        0     2779 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/dictionary.py
+-rw-rw-rw-   0        0        0    38811 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/network.py
+-rw-rw-rw-   0        0        0     2875 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/register.py
+-rw-rw-rw-   0        0        0     5239 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/canopen/servo.py
+-rw-rw-rw-   0        0        0      974 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/constants.py
+-rw-rw-rw-   0        0        0    41826 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/dictionary.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/__init__.py
+-rw-rw-rw-   0        0        0     1389 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/register.py
+-rw-rw-rw-   0        0        0     2892 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/enums/servo.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/eoe/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/eoe/__init__.py
+-rw-rw-rw-   0        0        0    13578 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/eoe/network.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/ethercat/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/__init__.py
+-rw-rw-rw-   0        0        0     6532 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/dictionary.py
+-rw-rw-rw-   0        0        0    19540 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/network.py
+-rw-rw-rw-   0        0        0      249 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/register.py
+-rw-rw-rw-   0        0        0     9439 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethercat/servo.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.650321 ingenialink-7.3.0/ingenialink/ethernet/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/__init__.py
+-rw-rw-rw-   0        0        0     2724 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/dictionary.py
+-rw-rw-rw-   0        0        0    11937 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/network.py
+-rw-rw-rw-   0        0        0     2823 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/register.py
+-rw-rw-rw-   0        0        0     6068 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/ethernet/servo.py
+-rw-rw-rw-   0        0        0     3725 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/exceptions.py
+-rw-rw-rw-   0        0        0     2412 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/network.py
+-rw-rw-rw-   0        0        0    21882 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/pdo.py
+-rw-rw-rw-   0        0        0     8024 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/poller.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/py.typed
+-rw-rw-rw-   0        0        0     8649 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/register.py
+-rw-rw-rw-   0        0        0    50678 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/servo.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.665944 ingenialink-7.3.0/ingenialink/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/__init__.py
+-rw-rw-rw-   0        0        0     9012 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/_utils.py
+-rw-rw-rw-   0        0        0     4486 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/constants.py
+-rw-rw-rw-   0        0        0      684 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/errors.py
+-rw-rw-rw-   0        0        0     7327 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/mcb.py
+-rw-rw-rw-   0        0        0     4337 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/utils/udp.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.665944 ingenialink-7.3.0/ingenialink/virtual/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/__init__.py
+-rw-rw-rw-   0        0        0     3224 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/dictionary.py
+-rw-rw-rw-   0        0        0     2094 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/network.py
+-rw-rw-rw-   0        0        0      315 2024-04-23 09:30:10.000000 ingenialink-7.3.0/ingenialink/virtual/servo.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/ingenialink.egg-info/
+-rw-rw-rw-   0        0        0     2586 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1824 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-23 09:31:12.000000 ingenialink-7.3.0/ingenialink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2024-04-23 09:30:10.000000 ingenialink-7.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 09:31:12.681591 ingenialink-7.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1775 2024-04-23 09:30:10.000000 ingenialink-7.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/tests/
+-rw-rw-rw-   0        0        0     7579 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_dictionary.py
+-rw-rw-rw-   0        0        0     3157 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_mcb.py
+-rw-rw-rw-   0        0        0     7922 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_register.py
+-rw-rw-rw-   0        0        0    16973 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_servo.py
+-rw-rw-rw-   0        0        0      914 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0     7966 2024-04-23 09:30:10.000000 ingenialink-7.3.0/tests/test_virtual_drive.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/virtual_drive/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/__init__.py
+-rw-rw-rw-   0        0        0    68129 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/core.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-23 09:31:12.681591 ingenialink-7.3.0/virtual_drive/resources/
+-rw-rw-rw-   0        0        0    29066 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xcf
+-rw-rw-rw-   0        0        0   267648 2024-04-23 09:30:10.000000 ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xdf
```

### Comparing `ingenialink-7.2.0/LICENSE.md` & `ingenialink-7.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/PKG-INFO` & `ingenialink-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.2.0
+Version: 7.3.0
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.2.0
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.0
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ingenialink-7.2.0/README.rst` & `ingenialink-7.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/__init__.py` & `ingenialink-7.3.0/ingenialink/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .ethernet.servo import EthernetServo
 
 from .ethercat.network import EthercatNetwork
 
 from .canopen.servo import CanopenServo
 from .canopen.network import CanopenNetwork, CAN_DEVICE, CAN_DEVICE, CAN_BAUDRATE
 from .canopen.register import CanopenRegister
-from .canopen.dictionary import CanopenDictionary
+from .canopen.dictionary import CanopenDictionaryV2
 
 from ingenialink.enums.register import REG_DTYPE, REG_ACCESS, REG_PHY
 
 from ingenialink.poller import Poller
 
 __all__ = [
     "EEPROM_FILE_FORMAT",
@@ -47,11 +47,11 @@
     "EthernetNetwork",
     "CanopenNetwork",
     "CAN_DEVICE",
     "CAN_BAUDRATE",
     "CanopenServo",
     "CanopenRegister",
     "Poller",
-    "CanopenDictionary",
+    "CanopenDictionaryV2",
 ]
 
-__version__ = "7.2.0"
+__version__ = "7.3.0"
```

### Comparing `ingenialink-7.2.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe` & `ingenialink-7.3.0/ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140007550
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri Mar 31 07:32:05 2023
+Time/Date		Fri Apr 19 13:01:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000007200
 SizeOfInitializedData	0000000000823200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000007550
@@ -1369,15 +1369,15 @@
 	reloc   14 offset   d0 [c0d0] DIR64
 	reloc   15 offset    0 [c000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x14000a118
 
 Type                Size     Rva      Offset
   2        CodeView 00000089 0000a318 00008918
-(format RSDS signature d8286b9f6a7b4c0c9e231d9a3c21dd7a age 1 pdb C:\jenkins1\workspace\_Ingenia_-_ingecatgateway_master\build\FoEUpdateFirmware\x64\Release\FoEUpdateFirmware.pdb)
+(format RSDS signature 3049f1c4dd394c759bcb59182ff1ffa9 age 1 pdb C:\jenkinsA\workspace\n_-_Ingenia_-_eoe_gateway_master\build\FoEUpdateFirmware\x64\Release\FoEUpdateFirmware.pdb)
  12         Feature 00000014 0000a3a4 000089a4
  13         CoffGrp 00000284 0000a3b8 000089b8
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -9626,46 +9626,47 @@
    14000a108:	and    %dh,0x63(%rax)
    14000a10b:	(bad)
    14000a10c:	jo     0x14000a118
    14000a10e:	add    %al,(%rax)
    14000a110:	add    %al,(%rax)
    14000a112:	add    %al,(%rax)
    14000a114:	addb   $0x0,0x41(%rsi,%rbp,1)
-   14000a11c:	jne    0x14000a0aa
-   14000a11e:	es add %al,%fs:(%rax)
+   14000a11c:	cmp    %ch,0x22(%rbx)
+   14000a11f:	data16 add %al,(%rax)
    14000a122:	add    %al,(%rax)
    14000a124:	add    (%rax),%al
    14000a126:	add    %al,(%rax)
    14000a128:	mov    %eax,(%rax)
    14000a12a:	add    %al,(%rax)
    14000a12c:	sbb    %ah,-0x76e80000(%rbx)
    14000a132:	add    %al,(%rax)
    14000a134:	add    %al,(%rax)
    14000a136:	add    %al,(%rax)
-   14000a138:	jne    0x14000a0c6
-   14000a13a:	es add %al,%fs:(%rax)
+   14000a138:	cmp    %ch,0x22(%rbx)
+   14000a13b:	data16 add %al,(%rax)
    14000a13e:	add    %al,(%rax)
    14000a140:	or     $0x0,%al
    14000a142:	add    %al,(%rax)
    14000a144:	adc    $0x0,%al
    14000a146:	add    %al,(%rax)
    14000a148:	movsb  %ds:(%rsi),%es:(%rdi)
    14000a149:	movabs %eax,0x89a40000
    14000a152:	add    %al,(%rax)
-   14000a154:	jne    0x14000a0e2
-   14000a156:	es add %al,%fs:(%rax)
+   14000a154:	cmp    %ch,0x22(%rbx)
+   14000a157:	data16 add %al,(%rax)
    14000a15a:	add    %al,(%rax)
    14000a15c:	or     $0x84000000,%eax
    14000a161:	add    (%rax),%al
    14000a163:	add    %bh,-0x47ffff5d(%rax)
    14000a169:	mov    %eax,(%rax)
    14000a16b:	add    %al,(%rax)
    14000a16d:	add    %al,(%rax)
-   14000a16f:	add    %dh,-0x74(%rbp)
-   14000a172:	es add %al,%fs:(%rax)
+   14000a16f:	add    %bh,(%rax)
+   14000a171:	imul   $0x66,(%rdx),%esp
+   14000a174:	add    %al,(%rax)
    14000a176:	add    %al,(%rax)
    14000a178:	(bad)
 	...
    14000a18d:	add    %al,(%rax)
    14000a18f:	add    %bh,(%rax)
    14000a191:	add    %eax,(%rax)
 	...
@@ -9706,37 +9707,39 @@
    14000a302:	add    %al,(%rax)
    14000a304:	add    %al,0x8000(%rax)
 	...
    14000a316:	add    %al,(%rax)
    14000a318:	push   %rdx
    14000a319:	push   %rbx
    14000a31a:	rex.R push %rbx
-   14000a31c:	lahf
-   14000a31d:	imul   $0xffffffd8,(%rax),%ebp
-   14000a320:	jnp    0x14000a38c
-   14000a322:	or     $0x4c,%al
-   14000a324:	sahf
-   14000a325:	and    -0x22dec366(%rip),%ebx        # 0x11d21dfc5
-   14000a32b:	jp     0x14000a32e
-   14000a32d:	add    %al,(%rax)
-   14000a32f:	add    %al,0x3a(%rbx)
-   14000a332:	pop    %rsp
-   14000a333:	push   $0x65
+   14000a31c:	(bad)
+   14000a31d:	int1
+   14000a31e:	rex.WB xor %dil,(%r9)
+   14000a321:	fnsave 0x4c(%rbp)
+   14000a324:	fwait
+   14000a325:	lret
+   14000a326:	pop    %rcx
+   14000a327:	sbb    %ch,(%rdi)
+   14000a329:	int1
+   14000a32a:	ljmp   *0x1(%rcx)
+   14000a330:	cmp    0x65(%r10,%r13,2),%bl
    14000a335:	outsb  %ds:(%rsi),(%dx)
    14000a336:	imul   $0x73,0x6e(%rcx),%ebp
-   14000a33a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   14000a33a:	pop    %r12
+   14000a33c:	ja     0x14000a3ad
    14000a33e:	jb     0x14000a3ab
    14000a340:	jae    0x14000a3b2
    14000a342:	(bad)
    14000a343:	movsxd 0x5c(%rbp),%esp
-   14000a346:	pop    %rdi
-   14000a347:	rex.WB outsb %ds:(%rsi),(%dx)
-   14000a349:	outsb  %gs:(%esi),(%dx)
-   14000a34c:	imul   $0x6e695f2d,0x5f(%rcx),%esp
-   14000a353:	movsxd %gs:0x74(%ecx),%esp
+   14000a346:	outsb  %ds:(%rsi),(%dx)
+   14000a347:	pop    %rdi
+   14000a348:	sub    $0x676e495f,%eax
+   14000a34d:	outsb  %gs:(%rsi),(%dx)
+   14000a34f:	imul   $0x6f655f2d,0x5f(%rcx),%esp
+   14000a356:	gs pop %rdi
    14000a358:	addr32 (bad)
    14000a35a:	je     0x14000a3c1
    14000a35c:	ja     0x14000a3bf
    14000a35e:	jns    0x14000a3bf
    14000a360:	insl   (%dx),%es:(%rdi)
    14000a361:	(bad)
    14000a362:	jae    0x14000a3d8
```

### Comparing `ingenialink-7.2.0/ingenialink/canopen/dictionary.py` & `ingenialink-7.3.0/ingenialink/canopen/dictionary.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,49 @@
-from typing import Optional
+from typing import Optional, List
 
-from ingenialink.dictionary import Dictionary
-from ingenialink.canopen.register import CanopenRegister
+from ingenialink.dictionary import DictionaryV2, Interface
+from ingenialink.canopen.register import CanopenRegister, REG_DTYPE, REG_ACCESS, RegCyclicType
 
 import ingenialogger
 import xml.etree.ElementTree as ET
 
 logger = ingenialogger.get_logger(__name__)
 
 
-class CanopenDictionary(Dictionary):
+class CanopenDictionaryV2(DictionaryV2):
     """Contains all registers and information of a CANopen dictionary.
 
     Args:
         dictionary_path: Path to the Ingenia dictionary.
 
     """
 
-    def __init__(self, dictionary_path: str) -> None:
-        super().__init__(dictionary_path)
+    MONITORING_DISTURBANCE_REGISTERS: List[CanopenRegister] = [
+        CanopenRegister(
+            identifier="MONITORING_DATA",
+            idx=0x58B2,
+            subidx=0x00,
+            cyclic=RegCyclicType.CONFIG,
+            dtype=REG_DTYPE.BYTE_ARRAY_512,
+            access=REG_ACCESS.RO,
+            subnode=0,
+        ),
+        CanopenRegister(
+            identifier="DISTURBANCE_DATA",
+            idx=0x58B4,
+            subidx=0x00,
+            cyclic=RegCyclicType.CONFIG,
+            dtype=REG_DTYPE.BYTE_ARRAY_512,
+            access=REG_ACCESS.WO,
+            subnode=0,
+        ),
+    ]
+
+    def __init__(self, dictionary_path: str):
+        super().__init__(dictionary_path, Interface.CAN)
 
     def _read_xdf_register(self, register: ET.Element) -> Optional[CanopenRegister]:
         current_read_register = super()._read_xdf_register(register)
         if current_read_register is None:
             return None
         try:
             aux_var = int(register.attrib["address"], 16)
```

### Comparing `ingenialink-7.2.0/ingenialink/canopen/network.py` & `ingenialink-7.3.0/ingenialink/canopen/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 import contextlib
 import os
+import platform
 import re
 import tempfile
 from collections import OrderedDict, defaultdict
 from enum import Enum
 from threading import Thread
 from time import sleep
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import canopen
 import ingenialogger
 from can import CanError
-from can.interfaces.ixxat.exceptions import VCIError
-from canopen import Network as NetworkLib
+
 
 from ingenialink.canopen.register import CanopenRegister
 from ingenialink.canopen.servo import (
     CANOPEN_SDO_RESPONSE_TIMEOUT,
     REG_ACCESS,
     REG_DTYPE,
     CanopenServo,
 )
+from ingenialink.enums.register import RegCyclicType
 from ingenialink.exceptions import ILError, ILFirmwareLoadError, ILObjectNotExist
 from ingenialink.network import NET_DEV_EVT, NET_PROT, NET_STATE, Network, SlaveInfo
-from ingenialink.utils._utils import convert_bytes_to_dtype
+from ingenialink.utils._utils import convert_bytes_to_dtype, DisableLogger
 from ingenialink.utils.mcb import MCB
 
+if platform.system() == "Windows":
+    with DisableLogger():
+        from can.interfaces.ixxat.exceptions import VCIError
+else:
+    VCIError = None
+from canopen import Network as NetworkLib
+
 logger = ingenialogger.get_logger(__name__)
 
 PROG_STAT_1 = CanopenRegister(
     idx=0x1F51,
     subidx=0x01,
-    cyclic="CONFIG",
+    cyclic=RegCyclicType.CONFIG,
     dtype=REG_DTYPE.U8,
     access=REG_ACCESS.RW,
     identifier="CIA302_BL_PROGRAM_CONTROL_1",
     subnode=0,
 )
 PROG_DL_1 = CanopenRegister(
     idx=0x1F50,
     subidx=0x01,
-    cyclic="CONFIG",
-    dtype=REG_DTYPE.DOMAIN,
+    cyclic=RegCyclicType.CONFIG,
+    dtype=REG_DTYPE.BYTE_ARRAY_512,
     access=REG_ACCESS.RW,
     identifier="CIA302_BL_PROGRAM_DATA",
     subnode=0,
 )
 FORCE_BOOT = CanopenRegister(
     idx=0x5EDE,
     subidx=0x00,
-    cyclic="CONFIG",
+    cyclic=RegCyclicType.CONFIG,
     dtype=REG_DTYPE.U32,
     access=REG_ACCESS.WO,
     identifier="DRV_BOOT_COCO_FORCE",
     subnode=0,
 )
 
 CIA301_DRV_ID_DEVICE_TYPE = CanopenRegister(
     idx=0x1000,
     subidx=0x00,
-    cyclic="CONFIG",
+    cyclic=RegCyclicType.CONFIG,
     dtype=REG_DTYPE.U32,
     access=REG_ACCESS.RO,
     identifier="",
     subnode=0,
 )
 
 CANOPEN_BOTT_NODE_GUARDING_PERIOD = 5
@@ -80,24 +88,26 @@
 APPLICATION_LOADED_STATE = 402
 
 CAN_CHANNELS: Dict[str, Union[Tuple[int, int], Tuple[str, str]]] = {
     "kvaser": (0, 1),
     "pcan": ("PCAN_USBBUS1", "PCAN_USBBUS2"),
     "ixxat": (0, 1),
     "virtual": (0, 1),
+    "socketcan": ("can0", "can1"),
 }
 
 
 class CAN_DEVICE(Enum):
     """CAN Device."""
 
     KVASER = "kvaser"
     PCAN = "pcan"
     IXXAT = "ixxat"
     VIRTUAL = "virtual"
+    SOCKETCAN = "socketcan"
 
 
 class CAN_BAUDRATE(Enum):
     """Baudrates."""
 
     Baudrate_1M = 1000000
     """1 Mbit/s"""
@@ -600,14 +610,19 @@
         """
         logger.debug(f"Waiting for register {register} to return <{expected_value}>")
         num_tries = 0
         value = None
         while num_tries < POLLING_MAX_TRIES:
             with contextlib.suppress(ILError):
                 value = servo.read(register, subnode=subnode)
+            if isinstance(value, bytes):
+                raise ValueError(
+                    f"Error reading register {register.identifier}. Expected data type"
+                    f" {register.dtype}, got bytes."
+                )
             if value == expected_value:
                 logger.debug(f"Success. Read value {value}. Num tries {num_tries}")
                 return True
             num_tries += 1
             logger.debug(f"Trying again {num_tries}. value {value}.")
             sleep(1)
         return False
```

### Comparing `ingenialink-7.2.0/ingenialink/canopen/register.py` & `ingenialink-7.3.0/ingenialink/canopen/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from ingenialink.enums.register import REG_ACCESS, REG_ADDRESS_TYPE, REG_DTYPE, REG_PHY
+from ingenialink.enums.register import (
+    REG_ACCESS,
+    REG_ADDRESS_TYPE,
+    REG_DTYPE,
+    REG_PHY,
+    RegCyclicType,
+)
 from ingenialink.register import Register
 
 
 class CanopenRegister(Register):
     """CANopen Register.
 
     Args:
@@ -21,14 +27,16 @@
         reg_range: Range (min, max).
         labels: Register labels.
         enums: Enumeration registers.
         cat_id: Category ID.
         scat_id: Sub-category ID.
         internal_use: Internal use.
         address_type: Address Type.
+        description: Register description.
+        default: Register default value.
 
     Raises:
         TypeError: If any of the parameters has invalid type.
         ILValueError: If the register is invalid.
         ILAccessError: Register with wrong access type.
 
     """
@@ -37,27 +45,29 @@
         self,
         idx: int,
         subidx: int,
         dtype: REG_DTYPE,
         access: REG_ACCESS,
         identifier: Optional[str] = None,
         units: Optional[str] = None,
-        cyclic: str = "CONFIG",
+        cyclic: RegCyclicType = RegCyclicType.CONFIG,
         phy: REG_PHY = REG_PHY.NONE,
         subnode: int = 1,
         storage: Any = None,
         reg_range: Union[
             Tuple[None, None], Tuple[int, int], Tuple[float, float], Tuple[str, str]
         ] = (None, None),
         labels: Optional[Dict[str, str]] = None,
         enums: Optional[Dict[str, int]] = None,
         cat_id: Optional[str] = None,
         scat_id: Optional[str] = None,
         internal_use: int = 0,
         address_type: Optional[REG_ADDRESS_TYPE] = None,
+        description: Optional[str] = None,
+        default: Optional[bytes] = None,
     ):
         super().__init__(
             dtype,
             access,
             identifier,
             units,
             cyclic,
@@ -67,14 +77,16 @@
             reg_range,
             labels,
             enums,
             cat_id,
             scat_id,
             internal_use,
             address_type,
+            description,
+            default,
         )
 
         self.__idx = idx
         self.__subidx = subidx
 
     @property
     def idx(self) -> int:
```

### Comparing `ingenialink-7.2.0/ingenialink/canopen/servo.py` & `ingenialink-7.3.0/ingenialink/ethernet/servo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,166 @@
-from typing import Any, Callable, Optional, Union
+import ipaddress
+import socket
+from typing import Optional
+
+from ingenialink.dictionary import Interface
+from ingenialink.exceptions import ILError, ILTimeoutError, ILIOError, ILWrongRegisterError
+from ingenialink.constants import PASSWORD_STORE_RESTORE_TCP_IP
+from ingenialink.ethernet.register import EthernetRegister
+from ingenialink.constants import MCB_CMD_READ, MCB_CMD_WRITE, ETH_MAX_WRITE_SIZE, ETH_BUF_SIZE
+from ingenialink.enums.register import REG_DTYPE, REG_ACCESS
+from ingenialink.servo import Servo
+from ingenialink.utils.mcb import MCB
+from ingenialink.utils._utils import convert_ip_to_int
 
-import canopen
-import ingenialogger
-from canopen.emcy import EmcyConsumer
+from ingenialink.ethernet.dictionary import EthernetDictionaryV2
 
-from ingenialink.canopen.dictionary import CanopenDictionary
-from ingenialink.canopen.register import CanopenRegister
-from ingenialink.constants import CAN_MAX_WRITE_SIZE
-from ingenialink.enums.register import REG_ACCESS, REG_DTYPE
-from ingenialink.exceptions import ILIOError
-from ingenialink.register import Register
-from ingenialink.servo import Servo
+import ingenialogger
 
 logger = ingenialogger.get_logger(__name__)
 
-CANOPEN_SDO_RESPONSE_TIMEOUT = 0.3
 
-
-class CanopenServo(Servo):
-    """CANopen Servo instance.
+class EthernetServo(Servo):
+    """Servo object for all the Ethernet slave functionalities.
 
     Args:
-        target: Node ID to be connected.
-        node: Remote Node of the drive.
+        socket: Socket.
         dictionary_path: Path to the dictionary.
         servo_status_listener: Toggle the listener of the servo for
             its status, errors, faults, etc.
+        is_eoe: True if communication is EoE. ``False`` by default.
 
     """
 
-    DICTIONARY_CLASS = CanopenDictionary
-    MAX_WRITE_SIZE = CAN_MAX_WRITE_SIZE
+    MAX_WRITE_SIZE = ETH_MAX_WRITE_SIZE
+
+    COMMS_ETH_IP = "COMMS_ETH_IP"
+    COMMS_ETH_NET_MASK = "COMMS_ETH_NET_MASK"
+    COMMS_ETH_NET_GATEWAY = "COMMS_ETH_GW"
 
-    STATUS_WORD_REGISTERS = "CIA402_DRV_STATE_STATUS"
-    RESTORE_COCO_ALL = "CIA301_COMMS_RESTORE_ALL"
-    STORE_COCO_ALL = "CIA301_COMMS_STORE_ALL"
-    MONITORING_DATA = CanopenRegister(
-        idx=0x58B2,
-        subidx=0x00,
-        cyclic="CONFIG",
-        dtype=REG_DTYPE.U16,
-        access=REG_ACCESS.RO,
-        subnode=0,
-    )
-    DIST_DATA = CanopenRegister(
-        idx=0x58B4,
-        subidx=0x00,
-        cyclic="CONFIG",
-        dtype=REG_DTYPE.U16,
-        access=REG_ACCESS.RW,
-        subnode=0,
-    )
+    interface = Interface.ETH
 
     def __init__(
         self,
-        target: int,
-        node: canopen.RemoteNode,
+        socket: socket.socket,
         dictionary_path: str,
         servo_status_listener: bool = False,
+        is_eoe: bool = False,
     ) -> None:
-        self.__node = node
-        self.__emcy_consumer = EmcyConsumer()
-        super(CanopenServo, self).__init__(target, dictionary_path, servo_status_listener)
-
-    def read(self, reg: Union[str, Register], subnode: int = 1) -> Union[int, float, str]:
-        value = super().read(reg, subnode=subnode)
-        if isinstance(value, str):
-            value = value.replace("\x00", "")
-        return value
-
-    def store_parameters(self, subnode: Optional[int] = None, sdo_timeout: int = 3) -> None:
-        """Store all the current parameters of the target subnode.
+        if is_eoe:
+            self.interface = Interface.EoE
+        self.socket = socket
+        self.ip_address, self.port = self.socket.getpeername()
+        super(EthernetServo, self).__init__(self.ip_address, dictionary_path, servo_status_listener)
+
+    def store_tcp_ip_parameters(self) -> None:
+        """Stores the TCP/IP values. Affects IP address,
+        subnet mask and gateway"""
+        self.write(reg=self.STORE_COCO_ALL, data=PASSWORD_STORE_RESTORE_TCP_IP, subnode=0)
+        logger.info("Store TCP/IP successfully done.")
+
+    def restore_tcp_ip_parameters(self) -> None:
+        """Restores the TCP/IP values back to default. Affects
+        IP address, subnet mask and gateway"""
+        self.write(reg=self.RESTORE_COCO_ALL, data=PASSWORD_STORE_RESTORE_TCP_IP, subnode=0)
+        logger.info("Restore TCP/IP successfully done.")
+
+    def change_tcp_ip_parameters(self, ip_address: str, subnet_mask: str, gateway: str) -> None:
+        """Stores the TCP/IP values. Affects IP address,
+        network mask and gateway
+
+        .. note::
+            The drive needs a power cycle after this
+            in order for the changes to be properly applied.
 
         Args:
-            subnode: Subnode of the axis. `None` by default which stores all the parameters.
-            sdo_timeout: Timeout value for each SDO response.
+            ip_address: IP Address to be changed.
+            subnet_mask: Subnet mask to be changed.
+            gateway: Gateway to be changed.
 
         Raises:
-            ILError: Invalid subnode.
-            ILObjectNotExist: Failed to write to the registers.
+            ValueError: If the drive or gateway IP is not a
+                valid IP address.
+            ValueError: If the drive IP and gateway IP are not
+                on the same network.
+            NetmaskValueError: If the subnet_mask is not a valid
+                netmask.
 
         """
-        self._change_sdo_timeout(sdo_timeout)
-        super().store_parameters(subnode)
-        self._change_sdo_timeout(CANOPEN_SDO_RESPONSE_TIMEOUT)
+        drive_ip = ipaddress.ip_address(ip_address)
+        gateway_ip = ipaddress.ip_address(gateway)
+        net = ipaddress.IPv4Network(f"{drive_ip}/{subnet_mask}", strict=False)
+
+        if gateway_ip not in net:
+            raise ValueError(
+                f"Drive IP {ip_address} and Gateway IP {gateway} are not on the same network."
+            )
+
+        int_ip_address = convert_ip_to_int(ip_address)
+        int_subnet_mask = convert_ip_to_int(subnet_mask)
+        int_gateway = convert_ip_to_int(gateway)
+
+        self.write(self.COMMS_ETH_IP, int_ip_address, subnode=0)
+        self.write(self.COMMS_ETH_NET_MASK, int_subnet_mask, subnode=0)
+        self.write(self.COMMS_ETH_NET_GATEWAY, int_gateway, subnode=0)
 
-    def _write_raw(self, reg: CanopenRegister, data: bytes) -> None:  # type: ignore [override]
         try:
-            self._lock.acquire()
-            self.__node.sdo.download(reg.idx, reg.subidx, data)
-        except Exception as e:
-            logger.error("Failed writing %s. Exception: %s", str(reg.identifier), e)
-            error_raised = f"Error writing {reg.identifier}"
-            raise ILIOError(error_raised) from e
-        finally:
-            self._lock.release()
-
-    def _read_raw(self, reg: CanopenRegister) -> bytes:  # type: ignore [override]
-        try:
-            self._lock.acquire()
-            value = self.__node.sdo.upload(reg.idx, reg.subidx)
-        except Exception as e:
-            logger.error("Failed reading %s. Exception: %s", str(reg.identifier), e)
-            error_raised = f"Error reading {reg.identifier}"
-            raise ILIOError(error_raised)
-        finally:
-            self._lock.release()
-        if not isinstance(value, bytes):
-            return bytes()
-        return value
-
-    def emcy_subscribe(self, cb: Callable[..., Any]) -> int:
-        """Subscribe to emergency messages.
+            self.store_tcp_ip_parameters()
+        except ILError:
+            self.store_parameters()
+
+    def _write_raw(self, reg: EthernetRegister, data: bytes) -> None:  # type: ignore [override]
+        self._send_mcb_frame(MCB_CMD_WRITE, reg.address, reg.subnode, data)
+
+    def _read_raw(self, reg: EthernetRegister) -> bytes:  # type: ignore [override]
+        return self._send_mcb_frame(MCB_CMD_READ, reg.address, reg.subnode)
+
+    def _send_mcb_frame(
+        self, cmd: int, reg: int, subnode: int, data: Optional[bytes] = None
+    ) -> bytes:
+        """Send an MCB frame to the drive.
 
         Args:
-            cb: Callback
+            cmd: Read/write command.
+            reg: Register address to be read/written.
+            subnode: Target axis of the drive.
+            data: Data to be written to the register.
 
         Returns:
-            Assigned slot.
-
+            The response frame.
         """
-        self.__emcy_consumer.add_callback(cb)
-
-        return len(self.__emcy_consumer.callbacks) - 1
+        frame = MCB.build_mcb_frame(cmd, subnode, reg, data)
+        self._lock.acquire()
+        try:
+            try:
+                self.socket.sendall(frame)
+            except socket.error as e:
+                raise ILIOError("Error sending data.") from e
+            try:
+                return self.__receive_mcb_frame(reg)
+            except ILWrongRegisterError as e:
+                logger.error(e)
+                return self.__receive_mcb_frame(reg)
+        finally:
+            self._lock.release()
 
-    def emcy_unsubscribe(self, slot: int) -> None:
-        """Unsubscribe from emergency messages.
+    def __receive_mcb_frame(self, reg: int) -> bytes:
+        """Receive frame from socket and return MCB data
 
         Args:
-            slot: Assigned slot when subscribed.
+            reg: expected address
 
-        """
-        del self.__emcy_consumer.callbacks[slot]
-
-    def _change_sdo_timeout(self, value: float) -> None:
-        """Changes the SDO timeout of the node."""
-        self.__node.sdo.RESPONSE_TIMEOUT = value
-
-    @staticmethod
-    def _monitoring_disturbance_map_can_address(address: int, subnode: int) -> int:
-        """Map CAN register address to IPB register address."""
-        return address - (0x2000 + (0x800 * (subnode - 1)))
-
-    def _monitoring_disturbance_data_to_map_register(
-        self, subnode: int, address: int, dtype: int, size: int
-    ) -> int:
-        """Arrange necessary data to map a monitoring/disturbance register.
+        Returns:
+            MCB message data in bytes
 
-        Args:
-            subnode: Subnode to be targeted.
-            address: Register address to map.
-            dtype: Register data type.
-            size: Size of data in bytes.
+        Raises:
+            ILTimeoutError: socket timeout
+            ILIOError: socket error
 
         """
-        ipb_address = self._monitoring_disturbance_map_can_address(address, subnode)
-        return super()._monitoring_disturbance_data_to_map_register(
-            subnode, ipb_address, dtype, size
-        )
-
-    @property
-    def node(self) -> canopen.RemoteNode:
-        """Remote node of the servo."""
-        return self.__node
+        try:
+            response = self.socket.recv(ETH_BUF_SIZE)
+        except socket.timeout as e:
+            raise ILTimeoutError("Timeout while receiving data.") from e
+        except socket.error as e:
+            raise ILIOError("Error receiving data.") from e
+        return MCB.read_mcb_data(reg, response)
```

### Comparing `ingenialink-7.2.0/ingenialink/constants.py` & `ingenialink-7.3.0/ingenialink/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ingenialink.register import REG_DTYPE
 
 
 DIST_FRAME_SIZE_BYTES = 128
 DIST_FRAME_SIZE = 512
-SINGLE_AXIS_MINIMUM_SUBNODES = 2
 
 DEFAULT_MESSAGE_RETRIES = 7
 DEFAULT_MESSAGE_TIMEOUT = 200
 
 DEFAULT_ETH_CONNECTION_TIMEOUT = 1
 DEFAULT_PDS_TIMEOUT = 1000
```

### Comparing `ingenialink-7.2.0/ingenialink/enums/register.py` & `ingenialink-7.3.0/ingenialink/enums/register.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     """Unsigned 64-bit integer."""
     S64 = 7
     """Signed 64-bit integer."""
     FLOAT = 8
     """Float."""
     STR = 10
     """String."""
-    DOMAIN = 15
-    """Domain."""
+    BYTE_ARRAY_512 = 15
+    """Buffer with size of 512 bytes."""
     BOOL = 99
     """Boolean."""
 
 
 class REG_ACCESS(Enum):
     """Access Type."""
 
@@ -64,7 +64,16 @@
     """Address Type."""
 
     NVM = 0
     NVM_NONE = 1
     NVM_CFG = 2
     NVM_LOCK = 3
     NVM_HW = 4
+
+
+class RegCyclicType(Enum):
+    """Cyclic Type."""
+
+    RX = "CYCLIC_RX"
+    TX = "CYCLIC_TX"
+    TXRX = "CYCLIC_TXRX"
+    CONFIG = "CONFIG"
```

### Comparing `ingenialink-7.2.0/ingenialink/enums/servo.py` & `ingenialink-7.3.0/ingenialink/enums/servo.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/eoe/network.py` & `ingenialink-7.3.0/ingenialink/eoe/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         return super().connect_to_slave(
             ip_address,
             dictionary,
             port,
             connection_timeout,
             servo_status_listener,
             net_status_listener,
+            True,
         )
 
     def __wait_eoe_starts(self) -> None:
         """Wait until the EoE service starts the EoE or the timeout was reached"""
         status = self._get_status_eoe_service()
         time_start = time.time()
         while not status & self.STATUS_EOE_BIT and self.WAIT_EOE_TIMEOUT > time.time() - time_start:
```

### Comparing `ingenialink-7.2.0/ingenialink/ethercat/dictionary.py` & `ingenialink-7.3.0/ingenialink/virtual/dictionary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,70 @@
-from typing import Optional
 import xml.etree.ElementTree as ET
+from typing import Optional
 
 import ingenialogger
 
-from ingenialink.dictionary import Dictionary
-from ingenialink.ethercat.register import EthercatRegister
-from ingenialink.constants import (
-    CANOPEN_ADDRESS_OFFSET,
-    CANOPEN_SUBNODE_0_ADDRESS_OFFSET,
-    MAP_ADDRESS_OFFSET,
-)
+from ingenialink.ethernet.dictionary import EthernetDictionaryV2
+from ingenialink.ethernet.register import EthernetRegister
 
 logger = ingenialogger.get_logger(__name__)
 
 
-class EthercatDictionary(Dictionary):
-    """Contains all registers and information of a EtherCAT dictionary.
+class VirtualDictionary(EthernetDictionaryV2):
+    """Contains all registers and information of a dictionary compatible with the virtual drive.
+
+    It adapts a canopen dictionary to work in the ethernet communication used for the virtual drive.
 
     Args:
         dictionary_path: Path to the Ingenia dictionary.
 
     """
 
-    def __init__(self, dictionary_path: str) -> None:
-        super().__init__(dictionary_path)
-
-    @staticmethod
-    def __get_cia_offset(subnode: int) -> int:
-        """Get the CiA offset for the register based on the subnode.
+    def _transform_canopen_index_to_mcb_address(self, index: int, subnode: int) -> int:
+        """CANopen index is an uint16 but MCB address only has 12 bits, so,
+        some index makes overflow in MCB frame.
 
         Args:
-            subnode: register subnode.
+            index: CANopen index
+            subnode: register subnode
 
-        Returs:
-            The CiA offset for the register.
+        Returns:
+            MCB address
 
         """
-        return (
-            CANOPEN_SUBNODE_0_ADDRESS_OFFSET
-            if subnode == 0
-            else CANOPEN_ADDRESS_OFFSET + MAP_ADDRESS_OFFSET * (subnode - 1)
-        )
+        return index - (0x2000 + (0x800 * (subnode - 1)))
 
-    def _read_xdf_register(self, register: ET.Element) -> Optional[EthercatRegister]:
+    def _read_xdf_register(self, register: ET.Element) -> Optional[EthernetRegister]:
         current_read_register = super()._read_xdf_register(register)
+
         if current_read_register is None:
             return None
+
+        if self.dict_interface == "CAN" and (
+            register.attrib["cat_id"] == "CIA402" or register.attrib["id"].startswith("CIA402_")
+        ):
+            return None
+
+        if current_read_register.identifier in ["MON_DATA_VALUE", "DIST_DATA_VALUE"]:
+            return None
+
         try:
-            idx = int(register.attrib["address"], 16) + self.__get_cia_offset(
-                current_read_register.subnode
-            )
-            subidx = 0x00
+            if self.dict_interface == "CAN":
+                reg_address = int(register.attrib["address"][:6], 16)
+                if current_read_register.subnode > 0:
+                    reg_address = self._transform_canopen_index_to_mcb_address(
+                        reg_address, current_read_register.subnode
+                    )
+                else:
+                    reg_address -= 0x5800
+            else:
+                reg_address = int(register.attrib["address"], 16)
 
-            ethercat_register = EthercatRegister(
-                idx,
-                subidx,
+            ethernet_register = EthernetRegister(
+                reg_address,
                 current_read_register.dtype,
                 current_read_register.access,
                 identifier=current_read_register.identifier,
                 units=current_read_register.units,
                 cyclic=current_read_register.cyclic,
                 phy=current_read_register.phy,
                 subnode=current_read_register.subnode,
@@ -68,14 +74,14 @@
                 enums=current_read_register.enums,
                 cat_id=current_read_register.cat_id,
                 scat_id=current_read_register.scat_id,
                 internal_use=current_read_register.internal_use,
                 address_type=current_read_register.address_type,
             )
 
-            return ethercat_register
+            return ethernet_register
 
         except KeyError as ke:
             logger.error(
                 f"Register with ID {current_read_register.identifier} has not attribute {ke}"
             )
             return None
```

### Comparing `ingenialink-7.2.0/ingenialink/ethercat/network.py` & `ingenialink-7.3.0/ingenialink/ethercat/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import os
 import platform
 import subprocess
 import sys
 import time
 from collections import OrderedDict, defaultdict
+from enum import Enum
 from threading import Thread
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import ingenialogger
 
 try:
     import pysoem
@@ -17,20 +18,30 @@
     pysoem_import_error = ex
 
 if TYPE_CHECKING:
     from pysoem import CdefSlave
 
 from ingenialink import bin as bin_module
 from ingenialink.ethercat.servo import EthercatServo
-from ingenialink.exceptions import ILError, ILFirmwareLoadError, ILStateError, ILTimeoutError
+from ingenialink.exceptions import ILError, ILFirmwareLoadError, ILStateError, ILWrongWorkingCount
 from ingenialink.network import NET_DEV_EVT, NET_PROT, NET_STATE, Network, SlaveInfo
 
 logger = ingenialogger.get_logger(__name__)
 
 
+class SlaveState(Enum):
+    INIT_STATE = 1
+    NONE_STATE = 0
+    OP_STATE = 8
+    PREOP_STATE = 2
+    SAFEOP_STATE = 4
+    STATE_ERROR = 16
+    SAFEOP_ERROR_STATE = SAFEOP_STATE + STATE_ERROR
+
+
 class NetStatusListener(Thread):
     """Network status listener thread to check if the drive is alive.
 
     Args:
         network: Network instance of the EtherCAT communication.
 
     """
@@ -70,15 +81,18 @@
         overlapping_io_map: Map PDOs to overlapping IO map.
 
     Raises:
         ImportError: WinPcap is not installed
 
     """
 
-    FOE_APPLICATION = {"win32": {"64bit": "FoE/win_64x/FoEUpdateFirmware.exe"}}
+    FOE_APPLICATION = {
+        "win32": {"64bit": "FoE/win_64x/FoEUpdateFirmware.exe"},
+        "linux": {"64bit": "FoE/linux/FoEUpdateFirmware"},
+    }
     FOE_ERRORS = {
         1: "Can’t read the input file.",
         2: "ECAT slave can’t reach the BOOT mode.",
         3: "No ECAT slave detected",
         4: "Can’t initialize the network adapter",
         5: "Drive can't init. Ensure the FW file is right",
     }
@@ -195,16 +209,18 @@
             raise ILError(f"Slave {slave_id} was not found.")
         slave = self._ecat_master.slaves[slave_id - 1]
         servo = EthercatServo(
             slave, slave_id, dictionary, self._connection_timeout, servo_status_listener
         )
         if not self._change_nodes_state(servo, pysoem.PREOP_STATE):
             raise ILStateError("Slave can not reach PreOp state")
+        servo.reset_pdo_mapping()
         self.servos.append(servo)
         self._set_servo_state(slave_id, NET_STATE.CONNECTED)
+        self.subscribe_to_status(slave_id, self._recover_from_power_cycle)
         if net_status_listener:
             self.start_status_listener()
         return servo
 
     def disconnect_from_slave(self, servo: EthercatServo) -> None:  # type: ignore [override]
         """Disconnects the slave from the network.
 
@@ -218,16 +234,27 @@
         self.servos.remove(servo)
         if not self.servos:
             self.stop_status_listener()
             self._ecat_master.close()
             self.__is_master_running = False
             self.__last_init_nodes = []
 
+    def config_pdo_maps(self) -> None:
+        """Configure the PDO maps.
+
+        It maps the PDO maps of each slave and sets its state to SafeOP.
+
+        """
+        if self._overlapping_io_map:
+            self._ecat_master.config_overlap_map()
+        else:
+            self._ecat_master.config_map()
+
     def start_pdos(self, timeout: float = 1.0) -> None:
-        """Configure the PDOs and set slave state to OP for all slaves with mapped PDOs
+        """Set all slaves with mapped PDOs to Operational State.
 
         Args:
             timeout: timeout in seconds to reach Op state, 1.0 seconds by default.
 
         Raises:
             ILStateError: If slaves can not reach SafeOp or Op state
 
@@ -240,18 +267,15 @@
             for servo in op_servo_list:
                 for rpdo_map in servo._rpdo_maps:
                     rpdo_map.get_item_bytes()
         except ILError as e:
             raise ILError(
                 "The RPDO values should be set before starting the PDO exchange process."
             ) from e
-        if self._overlapping_io_map:
-            self._ecat_master.config_overlap_map()
-        else:
-            self._ecat_master.config_map()
+        self.config_pdo_maps()
         self._ecat_master.state = pysoem.SAFEOP_STATE
         if not self._change_nodes_state(op_servo_list, pysoem.SAFEOP_STATE):
             raise ILStateError("Drives can not reach SafeOp state")
         self._change_nodes_state(op_servo_list, pysoem.OP_STATE)
         init_time = time.time()
         while not self._check_node_state(op_servo_list, pysoem.OP_STATE):
             self.send_receive_processdata()
@@ -262,38 +286,50 @@
         """For all slaves in OP or SafeOp state, set state to PreOp"""
         self._ecat_master.read_state()
         op_servo_list = [
             servo
             for servo in self.servos
             if servo.slave.state in [pysoem.OP_STATE, pysoem.SAFEOP_STATE]
         ]
-        if not self._change_nodes_state(op_servo_list, pysoem.PREOP_STATE):
-            logger.warning("Drive can not reach PreOp state")
+        if not self._change_nodes_state(op_servo_list, pysoem.INIT_STATE):
+            logger.warning("Not all drives could reach the Init state")
+        self.__init_nodes()
 
     def send_receive_processdata(self, timeout: float = ECAT_PROCESSDATA_TIMEOUT_S) -> None:
         """Send and receive PDOs
 
         Args:
             timeout: receive processdata timeout in seconds, 0.1 seconds by default.
 
         Raises:
-            ILError: If processdata working count is wrong
+            ILWrongWorkingCount: If processdata working count is wrong
 
         """
         for servo in self.servos:
             servo.process_pdo_inputs()
         if self._overlapping_io_map:
             self._ecat_master.send_overlap_processdata()
         else:
             self._ecat_master.send_processdata()
         processdata_wkc = self._ecat_master.receive_processdata(timeout=int(timeout * 1_000_000))
         if processdata_wkc != self._ecat_master.expected_wkc:
-            raise ILError(
+            self._ecat_master.read_state()
+            servos_state_msg = ""
+            for servo in self.servos:
+                servos_state_msg += (
+                    f"Slave {servo.slave_id}: state {SlaveState(servo.slave.state).name}"
+                )
+                if servo.slave.al_status != 0:
+                    al_status = pysoem.al_status_code_to_string(servo.slave.al_status)
+                    servos_state_msg += f", AL status {al_status}."
+                else:
+                    servos_state_msg += ". "
+            raise ILWrongWorkingCount(
                 f"Processdata working count is wrong, expected: {self._ecat_master.expected_wkc},"
-                f" real: {processdata_wkc}"
+                f" real: {processdata_wkc}. {servos_state_msg}"
             )
         for servo in self.servos:
             servo.generate_pdo_outputs()
 
     def _change_nodes_state(
         self, nodes: Union["EthercatServo", List["EthercatServo"]], target_state: int
     ) -> bool:
@@ -329,15 +365,15 @@
 
         return all(
             target_state == drive.slave.state_check(target_state, self.ECAT_STATE_CHANGE_TIMEOUT_NS)
             for drive in node_list
         )
 
     def subscribe_to_status(  # type: ignore [override]
-        self, slave_id: int, callback: Callable[[str, NET_DEV_EVT], None]
+        self, slave_id: int, callback: Callable[[NET_DEV_EVT], None]
     ) -> None:
         """Subscribe to network state changes.
 
         Args:
             slave_id: Slave ID of the drive to subscribe.
             callback: Callback function.
 
@@ -399,17 +435,27 @@
         if app_path is None:
             raise NotImplementedError(
                 "Load FW by ECAT is not implemented for this OS and architecture:"
                 f" {sys_name} {arch}"
             )
         exec_path = os.path.join(os.path.dirname(inspect.getfile(bin_module)), app_path)
         logger.debug(f"Call FoE application for {sys_name}-{arch}")
+        if sys_name == "linux":
+            try:
+                subprocess.run(
+                    f"chmod 777 {exec_path}",
+                    check=True,
+                    shell=True,
+                    encoding="utf-8",
+                )
+            except subprocess.CalledProcessError as e:
+                raise ILFirmwareLoadError("Could not change the FoE binary permissions.") from e
         try:
             subprocess.run(
-                [exec_path, self.interface_name, f"{slave_id}", fw_file],
+                f"{exec_path} {self.interface_name} {slave_id} {fw_file}",
                 check=True,
                 shell=True,
                 encoding="utf-8",
             )
         except subprocess.CalledProcessError as e:
             foe_return_error = self.FOE_ERRORS.get(e.returncode, self.UNKNOWN_FOE_ERROR)
             raise ILFirmwareLoadError(
@@ -433,7 +479,25 @@
     def _set_servo_state(self, slave_id: int, state: NET_STATE) -> None:
         self.__servos_state[slave_id] = state
 
     def _notify_status(self, slave_id: int, status: NET_DEV_EVT) -> None:
         """Notify subscribers of a network state change."""
         for callback in self.__observers_net_state[slave_id]:
             callback(status)
+
+    def _recover_from_power_cycle(self, status: NET_DEV_EVT) -> None:
+        """Transition the slaves to Pre-Op state after a power cycle.
+
+        Args:
+            status: The network status.
+
+        Raises:
+            ILStateError: If not all slaves reach PreOp state.
+
+        """
+        self._ecat_master.read_state()
+        if status == NET_DEV_EVT.ADDED and self._ecat_master.state == pysoem.INIT_STATE:
+            self.__init_nodes()
+            if not self._check_node_state(self.servos, pysoem.PREOP_STATE):
+                raise ILStateError(
+                    "The communication cannot be recovered. Not all slaves reached PreOp state"
+                )
```

### Comparing `ingenialink-7.2.0/ingenialink/ethercat/servo.py` & `ingenialink-7.3.0/ingenialink/ethercat/servo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import time
 from enum import Enum
-from typing import TYPE_CHECKING, List, Optional, Dict
+from typing import TYPE_CHECKING, List, Optional, Dict, Any
 
 import ingenialogger
 
 try:
     import pysoem
 except ImportError as ex:
     pysoem = None
     pysoem_import_error = ex
 
 if TYPE_CHECKING:
     from pysoem import CdefSlave
 
 from ingenialink.constants import CAN_MAX_WRITE_SIZE, CANOPEN_ADDRESS_OFFSET, MAP_ADDRESS_OFFSET
-from ingenialink.ethercat.dictionary import EthercatDictionary
 from ingenialink.ethercat.register import EthercatRegister
 from ingenialink.exceptions import ILIOError, ILTimeoutError, ILError
 from ingenialink.pdo import PDOServo, RPDOMap, TPDOMap
 from ingenialink.register import REG_ACCESS, REG_DTYPE
+from ingenialink.dictionary import Interface
 
 logger = ingenialogger.get_logger(__name__)
 
 
 class SDO_OPERATION_MSG(Enum):
     """Message for exceptions depending on the operation type."""
 
@@ -42,122 +42,25 @@
             its status, errors, faults, etc.
 
     Raises:
         ImportError: WinPcap is not installed
 
     """
 
-    DICTIONARY_CLASS = EthercatDictionary
     MAX_WRITE_SIZE = CAN_MAX_WRITE_SIZE
+    MONITORING_DATA_BUFFER_SIZE = 1024
 
     NO_RESPONSE_WORKING_COUNTER = 0
     TIMEOUT_WORKING_COUNTER = -5
     NOFRAME_WORKING_COUNTER = -1
 
-    MONITORING_DATA = EthercatRegister(
-        identifier="MONITORING_DATA",
-        units="",
-        subnode=0,
-        idx=0x58B2,
-        subidx=0x01,
-        cyclic="CONFIG",
-        dtype=REG_DTYPE.U16,
-        access=REG_ACCESS.RO,
-    )
-    DIST_DATA = EthercatRegister(
-        identifier="DISTURBANCE_DATA",
-        units="",
-        subnode=0,
-        idx=0x58B4,
-        subidx=0x01,
-        cyclic="CONFIG",
-        dtype=REG_DTYPE.U16,
-        access=REG_ACCESS.WO,
-    )
-
-    RPDO_ASSIGN_REGISTER_SUB_IDX_0 = EthercatRegister(
-        identifier="RPDO_ASSIGN_REGISTER",
-        units="",
-        subnode=0,
-        idx=0x1C12,
-        subidx=0x00,
-        dtype=REG_DTYPE.S32,
-        access=REG_ACCESS.RW,
-    )
-    RPDO_ASSIGN_REGISTER_SUB_IDX_1 = EthercatRegister(
-        identifier="RPDO_ASSIGN_REGISTER",
-        units="",
-        subnode=0,
-        idx=0x1C12,
-        subidx=0x01,
-        dtype=REG_DTYPE.S32,
-        access=REG_ACCESS.RW,
-    )
-    RPDO_MAP_REGISTER_SUB_IDX_0 = [
-        EthercatRegister(
-            identifier="RPDO_MAP_REGISTER",
-            units="",
-            subnode=0,
-            idx=0x1600,
-            subidx=0x00,
-            dtype=REG_DTYPE.S32,
-            access=REG_ACCESS.RW,
-        )
-    ]
-    RPDO_MAP_REGISTER_SUB_IDX_1 = [
-        EthercatRegister(
-            identifier="RPDO_MAP_REGISTER",
-            units="",
-            subnode=0,
-            idx=0x1600,
-            subidx=0x01,
-            dtype=REG_DTYPE.STR,
-            access=REG_ACCESS.RW,
-        )
-    ]
-    TPDO_ASSIGN_REGISTER_SUB_IDX_0 = EthercatRegister(
-        identifier="TPDO_ASSIGN_REGISTER",
-        units="",
-        subnode=0,
-        idx=0x1C13,
-        subidx=0x00,
-        dtype=REG_DTYPE.S32,
-        access=REG_ACCESS.RW,
-    )
-    TPDO_ASSIGN_REGISTER_SUB_IDX_1 = EthercatRegister(
-        identifier="TPDO_ASSIGN_REGISTER",
-        units="",
-        subnode=0,
-        idx=0x1C13,
-        subidx=0x01,
-        dtype=REG_DTYPE.S32,
-        access=REG_ACCESS.RW,
-    )
-    TPDO_MAP_REGISTER_SUB_IDX_0 = [
-        EthercatRegister(
-            identifier="TPDO_MAP_REGISTER",
-            units="",
-            subnode=0,
-            idx=0x1A00,
-            subidx=0x00,
-            dtype=REG_DTYPE.S32,
-            access=REG_ACCESS.RW,
-        )
-    ]
-    TPDO_MAP_REGISTER_SUB_IDX_1 = [
-        EthercatRegister(
-            identifier="TPDO_MAP_REGISTER",
-            units="",
-            subnode=0,
-            idx=0x1A00,
-            subidx=0x01,
-            dtype=REG_DTYPE.STR,
-            access=REG_ACCESS.RW,
-        )
-    ]
+    ETHERCAT_PDO_WATCHDOG = "processdata"
+    SECONDS_TO_MS_CONVERSION_FACTOR = 1000
+
+    interface = Interface.ECAT
 
     def __init__(
         self,
         slave: "CdefSlave",
         slave_id: int,
         dictionary_path: str,
         connection_timeout: float,
@@ -271,21 +174,23 @@
             }
             exc = wkc_exceptions.get(
                 exception.wkc,
                 ILIOError(f"{default_error_msg}. Wrong working counter: {exception.wkc}"),
             )
             raise exc from exception
 
-    def _monitoring_read_data(self) -> bytes:  # type: ignore [override]
+    def _monitoring_read_data(self, **kwargs: Any) -> bytes:
         """Read monitoring data frame."""
-        return self._read_raw(self.MONITORING_DATA, buffer_size=1024, complete_access=True)
+        return super()._monitoring_read_data(
+            buffer_size=self.MONITORING_DATA_BUFFER_SIZE, complete_access=True
+        )
 
-    def _disturbance_write_data(self, data: bytearray) -> None:  # type: ignore [override]
+    def _disturbance_write_data(self, data: bytes, **kwargs: Any) -> None:
         """Write disturbance data."""
-        return self._write_raw(self.DIST_DATA, bytes(data), complete_access=True)
+        super()._disturbance_write_data(data, complete_access=True)
 
     @staticmethod
     def __monitoring_disturbance_map_can_address(address: int, subnode: int) -> int:
         """Map CAN register address to IPB register address.
 
         Args:
             subnode: Subnode to be targeted.
@@ -326,26 +231,35 @@
         if self.dictionary.errors is not None:
             error_code &= 0xFFFF
             if error_code in self.dictionary.errors.errors:
                 error_description = self.dictionary.errors.errors[error_code][-1]
         return error_description
 
     def set_pdo_map_to_slave(self, rpdo_maps: List[RPDOMap], tpdo_maps: List[TPDOMap]) -> None:
-        self.reset_rpdo_mapping()
-        self.reset_tpdo_mapping()
-        self._rpdo_maps = rpdo_maps
-        self._tpdo_maps = tpdo_maps
+        self._rpdo_maps.extend(rpdo_maps)
+        self._tpdo_maps.extend(tpdo_maps)
         self.slave.config_func = self.map_pdos
 
     def process_pdo_inputs(self) -> None:
         self._process_tpdo(self.__slave.input)
 
     def generate_pdo_outputs(self) -> None:
         output = self._process_rpdo()
         if output is None:
             return
         self.__slave.output = self._process_rpdo()
 
+    def set_pdo_watchdog_time(self, timeout: float) -> None:
+        """Set the process data watchdog time.
+
+        Args:
+            timeout: Time in seconds.
+
+        """
+        self.slave.set_watchdog(
+            self.ETHERCAT_PDO_WATCHDOG, self.SECONDS_TO_MS_CONVERSION_FACTOR * timeout
+        )
+
     @property
     def slave(self) -> "CdefSlave":
         """Ethercat slave"""
         return self.__slave
```

### Comparing `ingenialink-7.2.0/ingenialink/ethernet/dictionary.py` & `ingenialink-7.3.0/ingenialink/ethernet/dictionary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 from typing import Optional, Dict, List
 import xml.etree.ElementTree as ET
 
 import ingenialogger
 
-from ingenialink.dictionary import Dictionary
-from ingenialink.ethernet.register import EthernetRegister
+from ingenialink.dictionary import DictionaryV2, Interface
+from ingenialink.ethernet.register import EthernetRegister, REG_DTYPE, REG_ACCESS, RegCyclicType
 
 logger = ingenialogger.get_logger(__name__)
 
 
-class EthernetDictionary(Dictionary):
+class EthernetDictionaryV2(DictionaryV2):
     """Contains all registers and information of a Ethernet dictionary.
 
     Args:
         dictionary_path: Path to the Ingenia dictionary.
 
     """
 
+    MONITORING_DISTURBANCE_REGISTERS: List[EthernetRegister] = [
+        EthernetRegister(
+            identifier="MONITORING_DATA",
+            units="",
+            subnode=0,
+            address=0x00B2,
+            cyclic=RegCyclicType.CONFIG,
+            dtype=REG_DTYPE.BYTE_ARRAY_512,
+            access=REG_ACCESS.RO,
+        ),
+        EthernetRegister(
+            identifier="DISTURBANCE_DATA",
+            units="",
+            subnode=0,
+            address=0x00B4,
+            cyclic=RegCyclicType.CONFIG,
+            dtype=REG_DTYPE.BYTE_ARRAY_512,
+            access=REG_ACCESS.WO,
+        ),
+    ]
+
     def __init__(self, dictionary_path: str) -> None:
-        self._registers: List[Dict[str, EthernetRegister]] = []  # type: ignore [assignment]
-        super().__init__(dictionary_path)
+        super().__init__(dictionary_path, Interface.ETH)
 
     def _read_xdf_register(self, register: ET.Element) -> Optional[EthernetRegister]:
         current_read_register = super()._read_xdf_register(register)
         if current_read_register is None:
             return None
         try:
             reg_address = int(register.attrib["address"], 16)
@@ -50,19 +70,7 @@
             return ethernet_register
 
         except KeyError as ke:
             logger.error(
                 f"Register with ID {current_read_register.identifier} has not attribute {ke}"
             )
             return None
-
-    def registers(self, subnode: int) -> Dict[str, EthernetRegister]:  # type: ignore [override]
-        """Gets the register dictionary to the targeted subnode.
-
-        Args:
-            subnode: Identifier for the subnode.
-
-        Returns:
-            Dictionary of all the registers for a subnode.
-
-        """
-        return self._registers[subnode]
```

### Comparing `ingenialink-7.2.0/ingenialink/ethernet/network.py` & `ingenialink-7.3.0/ingenialink/ethernet/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,35 +206,37 @@
         self,
         target: str,
         dictionary: str,
         port: int = 1061,
         connection_timeout: float = DEFAULT_ETH_CONNECTION_TIMEOUT,
         servo_status_listener: bool = False,
         net_status_listener: bool = False,
+        is_eoe: bool = False,
     ) -> EthernetServo:
         """Connects to a slave through the given network settings.
 
         Args:
             target: IP of the target slave.
             dictionary: Path to the target dictionary file.
             port: Port to connect to the slave.
             connection_timeout: Time in seconds of the connection timeout.
             servo_status_listener: Toggle the listener of the servo for
                 its status, errors, faults, etc.
             net_status_listener: Toggle the listener of the network
                 status, connection and disconnection.
+            is_eoe: True if communication is EoE. ``False`` by default.
 
         Returns:
             EthernetServo: Instance of the servo connected.
 
         """
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         sock.settimeout(connection_timeout)
         sock.connect((target, port))
-        servo = EthernetServo(sock, dictionary, servo_status_listener)
+        servo = EthernetServo(sock, dictionary, servo_status_listener, is_eoe)
         try:
             servo.get_state()
         except ILError as e:
             servo.stop_status_listener()
             raise ILError(f"Drive not found in IP {target}.") from e
         self.servos.append(servo)
         self._set_servo_state(target, NET_STATE.CONNECTED)
```

### Comparing `ingenialink-7.2.0/ingenialink/ethernet/register.py` & `ingenialink-7.3.0/ingenialink/ethernet/register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from ingenialink.enums.register import REG_ACCESS, REG_ADDRESS_TYPE, REG_DTYPE, REG_PHY
+from ingenialink.enums.register import (
+    REG_ACCESS,
+    REG_ADDRESS_TYPE,
+    REG_DTYPE,
+    REG_PHY,
+    RegCyclicType,
+)
 from ingenialink.register import Register
 
 
 class EthernetRegister(Register):
     """Ethernet Register.
 
     Args:
@@ -20,14 +26,16 @@
         reg_range: Range (min, max).
         labels: Register labels.
         enums: Enumeration registers.
         cat_id: Category ID.
         scat_id: Sub-category ID.
         internal_use: Internal use.
         address_type: Address Type.
+        description: Register description.
+        default: Register default value.
 
     Raises:
         TypeError: If any of the parameters has invalid type.
         ILValueError: If the register is invalid.
         ILAccessError: Register with wrong access type.
 
     """
@@ -37,27 +45,29 @@
     def __init__(
         self,
         address: int,
         dtype: REG_DTYPE,
         access: REG_ACCESS,
         identifier: Optional[str] = None,
         units: Optional[str] = None,
-        cyclic: str = "CONFIG",
+        cyclic: RegCyclicType = RegCyclicType.CONFIG,
         phy: REG_PHY = REG_PHY.NONE,
         subnode: int = 1,
         storage: Any = None,
         reg_range: Union[
             Tuple[None, None], Tuple[int, int], Tuple[float, float], Tuple[str, str]
         ] = (None, None),
         labels: Optional[Dict[str, str]] = None,
         enums: Optional[Dict[str, int]] = None,
         cat_id: Optional[str] = None,
         scat_id: Optional[str] = None,
         internal_use: int = 0,
         address_type: Optional[REG_ADDRESS_TYPE] = None,
+        description: Optional[str] = None,
+        default: Optional[bytes] = None,
     ):
         super().__init__(
             dtype,
             access,
             identifier,
             units,
             cyclic,
@@ -67,14 +77,16 @@
             reg_range,
             labels,
             enums,
             cat_id,
             scat_id,
             internal_use,
             address_type,
+            description,
+            default,
         )
 
         self.__address = address
 
     @property
     def address(self) -> int:
         """Register address."""
```

### Comparing `ingenialink-7.2.0/ingenialink/exceptions.py` & `ingenialink-7.3.0/ingenialink/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,14 @@
 
 class ILFirmwareLoadError(ILError):
     """IngeniaLink error while loading a firmware."""
 
     pass
 
 
-class ILCreationError(ILError):
-    """IngeniaLink creation error."""
-
-    pass
-
-
 class ILValueError(ILError):
     """IngeniaLink value error."""
 
     pass
 
 
 class ILTimeoutError(ILError):
@@ -99,14 +93,22 @@
 
     pass
 
 
 class ILNACKError(ILError):
     """IngeniaLink NACK error."""
 
+    pass
+
+
+class ILDictionaryParseError(ILError):
+    """IngeniaLink dictionary parse error."""
+
+    pass
+
 
 # Configuration error
 class ILIncorrectAccessType(ILConfigurationError):
     """Incorrect access type configuration error."""
 
     pass
 
@@ -184,7 +186,13 @@
     pass
 
 
 class ILCOMKITTimeout(ILConfigurationError):
     """COMKIT Timeout. CORE device is not properly connected configuration error."""
 
     pass
+
+
+class ILWrongWorkingCount(ILError):
+    """PDOs process data working count expected and received differ."""
+
+    pass
```

### Comparing `ingenialink-7.2.0/ingenialink/network.py` & `ingenialink-7.3.0/ingenialink/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/pdo.py` & `ingenialink-7.3.0/ingenialink/pdo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,78 @@
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Dict
 
 import bitarray
 
 from ingenialink.canopen.register import CanopenRegister
-from ingenialink.enums.register import REG_DTYPE
+from ingenialink.enums.register import REG_DTYPE, REG_ACCESS, RegCyclicType
 from ingenialink.ethercat.register import EthercatRegister
 from ingenialink.exceptions import ILError
 from ingenialink.servo import Servo
 from ingenialink.utils._utils import (
     convert_bytes_to_dtype,
     convert_dtype_to_bytes,
     dtype_length_bits,
 )
 
 BIT_ENDIAN = "little"
 bitarray._set_default_endian(BIT_ENDIAN)
 
+PADDING_REGISTER_IDENTIFIER = "PADDING"
+
 
 class PDOMapItem:
     """Abstract class to represent a register in the PDO mapping.
 
     Attributes:
-        register: mapped register object.
+        register: mapped register object. If None the item will padding.
         size_bits: custom register size in bits.
 
+    Raises:
+        ValueError: If the register and size_bits are not provided.
+        ValueError: If the size_bits value is invalid. Only when the register
+        is set to None.
+
     """
 
-    ACCEPTED_CYCLIC = ""
-    """Accepted cyclic: CYCLIC_TX or CYCLIC_RX."""
+    ACCEPTED_CYCLIC: RegCyclicType
+    """Accepted cyclic: CYCLIC_TX, CYCLIC_RX or CYCLIC_TXRX."""
 
     def __init__(
-        self, register: Union[EthercatRegister, CanopenRegister], size_bits: Optional[int] = None
+        self,
+        register: Union[None, EthercatRegister, CanopenRegister] = None,
+        size_bits: Optional[int] = None,
     ) -> None:
+        if register is None:
+            if size_bits is None:
+                raise ValueError("The size bits must be set when creating padding items.")
+            register = EthercatRegister(
+                identifier=PADDING_REGISTER_IDENTIFIER,
+                units="",
+                subnode=0,
+                idx=0x0000,
+                subidx=0x00,
+                cyclic=self.ACCEPTED_CYCLIC,
+                dtype=REG_DTYPE.STR,
+                access=REG_ACCESS.RW,
+            )
         self.register = register
         self.size_bits = size_bits or dtype_length_bits[register.dtype]
         self._raw_data_bits: Optional[bitarray.bitarray] = None
         self._check_if_mappable()
 
     def _check_if_mappable(self) -> None:
         """Check if the passed register is mappable. I.e., if the cyclic information is correct.
 
         Raises:
             ILError: Tf the register is not mappable.
         """
-        if not self.register.cyclic == self.ACCEPTED_CYCLIC:
+        if self.register.cyclic not in [self.ACCEPTED_CYCLIC, RegCyclicType.TXRX]:
             raise ILError(
-                f"Incorrect cyclic. It should be {self.ACCEPTED_CYCLIC}, obtained:"
-                f" {self.register.cyclic}"
+                f"Incorrect cyclic. It should be {self.ACCEPTED_CYCLIC} or {RegCyclicType.TXRX},"
+                f" obtained: {self.register.cyclic}"
             )
 
     @property
     def raw_data_bits(self) -> bitarray.bitarray:
         """Raw data in bits.
 
         Returns:
@@ -87,28 +109,34 @@
             raise ILError("Raw data is empty.")
         return self._raw_data_bits.tobytes()
 
     @raw_data_bytes.setter
     def raw_data_bytes(self, data: bytes) -> None:
         data_bits = bitarray.bitarray(endian=BIT_ENDIAN)
         data_bits.frombytes(data)
+        if self.register.identifier == PADDING_REGISTER_IDENTIFIER:
+            data_bits = data_bits[: self.size_bits]
         self.raw_data_bits = data_bits
 
     @property
     def value(self) -> Union[int, float, bool]:
         """Register value. Converts the raw data bytes into the register value.
 
         Raises:
             ILError: If the raw data is empty.
             ILError: If the register type is not int or float.
 
         Returns:
             Register value.
         """
         value: Union[bool, int, float, str]
+        if self.register.identifier == PADDING_REGISTER_IDENTIFIER:
+            raise NotImplementedError(
+                "The register value must be read by the raw_data_bytes attribute."
+            )
         if self.register.dtype == REG_DTYPE.BOOL:
             value = self.raw_data_bits.any()
         else:
             value = convert_bytes_to_dtype(self.raw_data_bytes, self.register.dtype)
         if not isinstance(value, (int, float, bool)):
             raise ILError("Wrong register value type")
         return value
@@ -126,40 +154,46 @@
         mapped_register_bytes: bytes = mapped_register.to_bytes(4, "little")
         return mapped_register_bytes
 
 
 class RPDOMapItem(PDOMapItem):
     """Class to represent RPDO mapping items."""
 
-    ACCEPTED_CYCLIC = "CYCLIC_RX"
+    ACCEPTED_CYCLIC = RegCyclicType.RX
 
     def __init__(
-        self, register: Union[EthercatRegister, CanopenRegister], size_bits: Optional[int] = None
+        self,
+        register: Union[None, EthercatRegister, CanopenRegister] = None,
+        size_bits: Optional[int] = None,
     ) -> None:
         super().__init__(register, size_bits)
 
     @property
     def value(self) -> Union[int, float]:
         return super().value
 
     @value.setter
     def value(self, value: Union[int, float, bool]) -> None:
+        if self.register.identifier == PADDING_REGISTER_IDENTIFIER:
+            raise NotImplementedError(
+                "The register value must be set by the raw_data_bytes attribute."
+            )
         if isinstance(value, bool):
             raw_data_bits = bitarray.bitarray(endian=BIT_ENDIAN)
             raw_data_bits.append(value)
             self.raw_data_bits = raw_data_bits
         else:
             raw_data_bytes = convert_dtype_to_bytes(value, self.register.dtype)
             self.raw_data_bytes = raw_data_bytes
 
 
 class TPDOMapItem(PDOMapItem):
     """Class to represent TPDO mapping items."""
 
-    ACCEPTED_CYCLIC = "CYCLIC_TX"
+    ACCEPTED_CYCLIC = RegCyclicType.TX
 
 
 class PDOMap:
     """Abstract class that contains PDO mapping information."""
 
     _PDO_MAP_ITEM_CLASS = PDOMapItem
 
@@ -349,141 +383,212 @@
 
 
 class PDOServo(Servo):
     """Abstract class to implement PDOs in a Servo class."""
 
     AVAILABLE_PDOS = 1
 
-    RPDO_ASSIGN_REGISTER_SUB_IDX_0: Union[EthercatRegister, CanopenRegister]
-    RPDO_ASSIGN_REGISTER_SUB_IDX_1: Union[EthercatRegister, CanopenRegister]
-    RPDO_MAP_REGISTER_SUB_IDX_0: List[Union[EthercatRegister, CanopenRegister]]
-    RPDO_MAP_REGISTER_SUB_IDX_1: List[Union[EthercatRegister, CanopenRegister]]
-
-    TPDO_ASSIGN_REGISTER_SUB_IDX_0: Union[EthercatRegister, CanopenRegister]
-    TPDO_ASSIGN_REGISTER_SUB_IDX_1: Union[EthercatRegister, CanopenRegister]
-    TPDO_MAP_REGISTER_SUB_IDX_0: List[Union[EthercatRegister, CanopenRegister]]
-    TPDO_MAP_REGISTER_SUB_IDX_1: List[Union[EthercatRegister, CanopenRegister]]
+    RPDO_ASSIGN_REGISTER_SUB_IDX_0 = "RPDO_ASSIGN_REGISTER_SUB_IDX_0"
+    RPDO_ASSIGN_REGISTER_SUB_IDX_1 = "RPDO_ASSIGN_REGISTER_SUB_IDX_1"
+    RPDO_MAP_REGISTER_SUB_IDX_0 = ["RPDO_MAP_REGISTER_SUB_IDX_0"]
+    RPDO_MAP_REGISTER_SUB_IDX_1 = ["RPDO_MAP_REGISTER_SUB_IDX_1"]
+
+    TPDO_ASSIGN_REGISTER_SUB_IDX_0 = "TPDO_ASSIGN_REGISTER_SUB_IDX_0"
+    TPDO_ASSIGN_REGISTER_SUB_IDX_1 = "TPDO_ASSIGN_REGISTER_SUB_IDX_1"
+    TPDO_MAP_REGISTER_SUB_IDX_0 = ["TPDO_MAP_REGISTER_SUB_IDX_0"]
+    TPDO_MAP_REGISTER_SUB_IDX_1 = ["TPDO_MAP_REGISTER_SUB_IDX_1"]
 
     def __init__(
         self,
         target: Union[int, str],
         dictionary_path: str,
         servo_status_listener: bool = False,
     ):
         super().__init__(target, dictionary_path, servo_status_listener)
         self._rpdo_maps: List[RPDOMap] = []
         self._tpdo_maps: List[TPDOMap] = []
 
     def reset_rpdo_mapping(self) -> None:
         """Delete the RPDO mapping stored in the servo slave."""
-        self.write(self.RPDO_ASSIGN_REGISTER_SUB_IDX_0, 0)
+        self.write(self.RPDO_ASSIGN_REGISTER_SUB_IDX_0, 0, subnode=0)
         for map_register in self.RPDO_MAP_REGISTER_SUB_IDX_0:
-            self.write(map_register, 0)
+            self.write(map_register, 0, subnode=0)
         self._rpdo_maps.clear()
 
     def reset_tpdo_mapping(self) -> None:
         """Delete the TPDO mapping stored in the servo slave."""
-        self.write(self.TPDO_ASSIGN_REGISTER_SUB_IDX_0, 0)
+        self.write(self.TPDO_ASSIGN_REGISTER_SUB_IDX_0, 0, subnode=0)
         for map_register in self.TPDO_MAP_REGISTER_SUB_IDX_0:
-            self.write(map_register, 0)
+            self.write(map_register, 0, subnode=0)
         self._tpdo_maps.clear()
 
     def map_rpdos(self) -> None:
         """Map the RPDO registers into the servo slave.
         It takes the first available RPDO assignment slot of the slave.
 
         Raises:
             ILError: If there are no available PDOs.
         """
         if len(self._rpdo_maps) > self.AVAILABLE_PDOS:
             raise ILError(
                 f"Could not map the RPDO maps, received {len(self._rpdo_maps)} PDOs and only"
                 f" {self.AVAILABLE_PDOS} are available"
             )
-        self.write(self.RPDO_ASSIGN_REGISTER_SUB_IDX_0, len(self._rpdo_maps))
+        self.write(self.RPDO_ASSIGN_REGISTER_SUB_IDX_0, len(self._rpdo_maps), subnode=0)
         custom_map_index = 0
         rpdo_assigns = b""
         for rpdo_map in self._rpdo_maps:
             if rpdo_map.map_register_index is None:
                 self._set_rpdo_map_register(custom_map_index, rpdo_map)
                 custom_map_index += 1
             rpdo_assigns += rpdo_map.map_register_index_bytes
         self.write(
-            self.RPDO_ASSIGN_REGISTER_SUB_IDX_1,
-            rpdo_assigns,
-            complete_access=True,
+            self.RPDO_ASSIGN_REGISTER_SUB_IDX_1, rpdo_assigns, complete_access=True, subnode=0
         )
 
     def _set_rpdo_map_register(self, rpdo_map_register_index: int, rpdo_map: RPDOMap) -> None:
         """Fill RPDO map register with PRDOMap object data
 
         Args:
             rpdo_map_register_index: custom rpdo map register index
             rpdo_map: custom rpdo data
 
         """
-        self.write(self.RPDO_MAP_REGISTER_SUB_IDX_0[rpdo_map_register_index], len(rpdo_map.items))
+        self.write(
+            self.RPDO_MAP_REGISTER_SUB_IDX_0[rpdo_map_register_index],
+            len(rpdo_map.items),
+            subnode=0,
+        )
         self.write(
             self.RPDO_MAP_REGISTER_SUB_IDX_1[rpdo_map_register_index],
             rpdo_map.items_mapping.decode("utf-8"),
             complete_access=True,
+            subnode=0,
         )
-        rpdo_map.map_register_index = self.RPDO_MAP_REGISTER_SUB_IDX_0[rpdo_map_register_index].idx
+        rpdo_map_register = self.dictionary.registers(0)[
+            self.RPDO_MAP_REGISTER_SUB_IDX_0[rpdo_map_register_index]
+        ]
+        if not isinstance(rpdo_map_register, EthercatRegister):
+            raise ValueError(
+                "Error retrieving the RPDO Map register. Expected EthercatRegister, got:"
+                f" {type(rpdo_map_register)}"
+            )
+        rpdo_map.map_register_index = rpdo_map_register.idx
 
     def map_tpdos(self) -> None:
         """Map the TPDO registers into the servo slave.
         It takes the first available TPDO assignment slot of the slave.
 
         Raises:
             ILError: If there are no available PDOs.
         """
         if len(self._tpdo_maps) > self.AVAILABLE_PDOS:
             raise ILError(
                 f"Could not map the TPDO maps, received {len(self._tpdo_maps)} PDOs and only"
                 f" {self.AVAILABLE_PDOS} are available"
             )
-        self.write(self.TPDO_ASSIGN_REGISTER_SUB_IDX_0, len(self._tpdo_maps))
+        self.write(self.TPDO_ASSIGN_REGISTER_SUB_IDX_0, len(self._tpdo_maps), subnode=0)
         custom_map_index = 0
         tpdo_assigns = b""
         for tpdo_map in self._tpdo_maps:
             if tpdo_map.map_register_index is None:
                 self._set_tpdo_map_register(custom_map_index, tpdo_map)
                 custom_map_index += 1
             tpdo_assigns += tpdo_map.map_register_index_bytes
         self.write(
-            self.TPDO_ASSIGN_REGISTER_SUB_IDX_1,
-            tpdo_assigns,
-            complete_access=True,
+            self.TPDO_ASSIGN_REGISTER_SUB_IDX_1, tpdo_assigns, complete_access=True, subnode=0
         )
 
     def _set_tpdo_map_register(self, tpdo_map_register_index: int, tpdo_map: TPDOMap) -> None:
         """Fill TPDO map register with TRDOMap object data
 
         Args:
             tpdo_map_register_index: custom tpdo map register index
             tpdo_map: custom tpdo data
 
         """
-        self.write(self.TPDO_MAP_REGISTER_SUB_IDX_0[tpdo_map_register_index], len(tpdo_map.items))
+        self.write(
+            self.TPDO_MAP_REGISTER_SUB_IDX_0[tpdo_map_register_index],
+            len(tpdo_map.items),
+            subnode=0,
+        )
         self.write(
             self.TPDO_MAP_REGISTER_SUB_IDX_1[tpdo_map_register_index],
             tpdo_map.items_mapping.decode("utf-8"),
             complete_access=True,
+            subnode=0,
         )
-        tpdo_map.map_register_index = self.TPDO_MAP_REGISTER_SUB_IDX_0[tpdo_map_register_index].idx
+        tpdo_map_register = self.dictionary.registers(0)[
+            self.TPDO_MAP_REGISTER_SUB_IDX_0[tpdo_map_register_index]
+        ]
+        if not isinstance(tpdo_map_register, EthercatRegister):
+            raise ValueError(
+                "Error retrieving the TPDO Map register. Expected EthercatRegister, got:"
+                f" {type(tpdo_map_register)}"
+            )
+        tpdo_map.map_register_index = tpdo_map_register.idx
 
     def map_pdos(self, slave_index: int) -> None:
         """Map RPDO and TPDO register into the slave.
 
         Args:
             slave_index: salve index.
         """
         self.map_tpdos()
         self.map_rpdos()
 
+    def reset_pdo_mapping(self) -> None:
+        """Reset the RPDO and TPDO mapping in the slave."""
+        self.reset_rpdo_mapping()
+        self.reset_tpdo_mapping()
+
+    def remove_rpdo_map(
+        self, rpdo_map: Optional[RPDOMap] = None, rpdo_map_index: Optional[int] = None
+    ) -> None:
+        """Remove a RPDOMap from the RPDOMap list.
+
+        Args:
+            rpdo_map: The RPDOMap instance to be removed.
+            rpdo_map_index: The index of the RPDOMap list to be removed.
+
+        Raises:
+            ValueError: If the RPDOMap instance is not in the RPDOMap list.
+            IndexError: If the index is out of range.
+
+        """
+        if rpdo_map_index is None and rpdo_map is None:
+            raise ValueError("The RPDOMap instance or the index should be provided.")
+        if rpdo_map is not None:
+            self._rpdo_maps.remove(rpdo_map)
+            return
+        if rpdo_map_index is not None:
+            self._rpdo_maps.pop(rpdo_map_index)
+
+    def remove_tpdo_map(
+        self, tpdo_map: Optional[TPDOMap] = None, tpdo_map_index: Optional[int] = None
+    ) -> None:
+        """Remove a TPDOMap from the TPDOMap list.
+
+        Args:
+            tpdo_map: The TPDOMap instance to be removed.
+            tpdo_map_index: The index of the TPDOMap list to be removed.
+
+        Raises:
+            ValueError: If the TPDOMap instance is not in the TPDOMap list.
+            IndexError: If the index is out of range.
+
+        """
+        if tpdo_map_index is None and tpdo_map is None:
+            raise ValueError("The TPDOMap instance or the index should be provided.")
+        if tpdo_map is not None:
+            self._tpdo_maps.remove(tpdo_map)
+            return
+        if tpdo_map_index is not None:
+            self._tpdo_maps.pop(tpdo_map_index)
+
     def set_pdo_map_to_slave(self, rpdo_maps: List[RPDOMap], tpdo_maps: List[TPDOMap]) -> None:
         """Callback called by the slave to configure the map.
 
         Args:
             rpdo_maps: List of RPDO maps.
             tpdo_maps: List of TPDO maps.
         """
```

### Comparing `ingenialink-7.2.0/ingenialink/poller.py` & `ingenialink-7.3.0/ingenialink/poller.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/register.py` & `ingenialink-7.3.0/ingenialink/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from abc import ABC
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from ingenialink import exceptions as exc
-from ingenialink.enums.register import REG_ACCESS, REG_ADDRESS_TYPE, REG_DTYPE, REG_PHY
-
-# CANOPEN DTYPES
-IL_REG_DTYPE_DOMAIN = 15
+from ingenialink.enums.register import (
+    REG_ACCESS,
+    REG_ADDRESS_TYPE,
+    REG_DTYPE,
+    REG_PHY,
+    RegCyclicType,
+)
+from ingenialink.utils._utils import convert_bytes_to_dtype
 
 dtypes_ranges: Dict[REG_DTYPE, Dict[str, Union[int, float]]] = {
     REG_DTYPE.U8: {"max": 255, "min": 0},
     REG_DTYPE.S8: {"max": 127, "min": -128},
     REG_DTYPE.U16: {"max": 65535, "min": 0},
     REG_DTYPE.S16: {"max": 32767, "min": -32767 - 1},
     REG_DTYPE.U32: {"max": 4294967295, "min": 0},
@@ -35,41 +39,45 @@
         reg_range: Range (min, max).
         labels: Register labels.
         enums: Enumeration registers.
         cat_id: Category ID.
         scat_id: Sub-category ID.
         internal_use: Internal use.
         address_type: Address tpye.
+        description: Register description.
+        default: Register default value.
 
     Raises:
         TypeError: If any of the parameters has invalid type.
         ILValueError: If the register is invalid.
         ILAccessError: Register with wrong access type.
 
     """
 
     def __init__(
         self,
         dtype: REG_DTYPE,
         access: REG_ACCESS,
         identifier: Optional[str] = None,
         units: Optional[str] = None,
-        cyclic: str = "CONFIG",
+        cyclic: RegCyclicType = RegCyclicType.CONFIG,
         phy: REG_PHY = REG_PHY.NONE,
         subnode: int = 1,
         storage: Any = None,
         reg_range: Union[
             Tuple[None, None], Tuple[int, int], Tuple[float, float], Tuple[str, str]
         ] = (None, None),
         labels: Optional[Dict[str, str]] = None,
         enums: Optional[Dict[str, int]] = None,
         cat_id: Optional[str] = None,
         scat_id: Optional[str] = None,
         internal_use: int = 0,
         address_type: Optional[REG_ADDRESS_TYPE] = None,
+        description: Optional[str] = None,
+        default: Optional[bytes] = None,
     ) -> None:
         if labels is None:
             labels = {}
         if enums is None:
             enums = {}
 
         self.__type_errors(dtype, access, phy)
@@ -85,14 +93,16 @@
         self._range = (None, None) if not reg_range else reg_range
         self._labels = labels
         self._cat_id = cat_id
         self._scat_id = scat_id
         self._internal_use = internal_use
         self._storage_valid = False if not storage else True
         self._address_type = address_type
+        self._description = description
+        self._default = default
         self._enums = enums
         self.__config_range(reg_range)
 
     def __type_errors(self, dtype: REG_DTYPE, access: REG_ACCESS, phy: REG_PHY) -> None:
         if not isinstance(dtype, REG_DTYPE):
             raise exc.ILValueError("Invalid data type")
 
@@ -142,15 +152,15 @@
 
     @property
     def units(self) -> Optional[str]:
         """Units of the register."""
         return self._units
 
     @property
-    def cyclic(self) -> str:
+    def cyclic(self) -> RegCyclicType:
         """Defines if the register is cyclic."""
         return self._cyclic
 
     @property
     def phy(self) -> REG_PHY:
         """Physical units of the register."""
         return REG_PHY(self._phy)
@@ -237,10 +247,22 @@
 
     @property
     def address_type(self) -> Optional[REG_ADDRESS_TYPE]:
         """Address type of the register."""
         return REG_ADDRESS_TYPE(self._address_type)
 
     @property
+    def description(self) -> Optional[str]:
+        """Register description."""
+        return self._description
+
+    @property
+    def default(self) -> Union[None, int, float, str]:
+        """Register default value"""
+        if self._default is None:
+            return self._default
+        return convert_bytes_to_dtype(self._default, self.dtype)
+
+    @property
     def mapped_address(self) -> int:
         """Register mapped address used for monitoring/disturbance."""
         raise NotImplementedError()
```

### Comparing `ingenialink-7.2.0/ingenialink/servo.py` & `ingenialink-7.3.0/ingenialink/servo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,137 @@
 import os
+import re
 import threading
 import time
 import xml.etree.ElementTree as ET
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from xml.dom import minidom
 
 import ingenialogger
 
+from ingenialink.ethernet.dictionary import EthernetDictionaryV2
+from ingenialink.ethercat.dictionary import EthercatDictionaryV2
+from ingenialink.canopen.dictionary import CanopenDictionaryV2
+from ingenialink.virtual.dictionary import VirtualDictionary
 from ingenialink.constants import (
     DEFAULT_DRIVE_NAME,
     DEFAULT_PDS_TIMEOUT,
     MONITORING_BUFFER_SIZE,
     PASSWORD_RESTORE_ALL,
     PASSWORD_STORE_ALL,
     PASSWORD_STORE_RESTORE_SUB_0,
 )
-from ingenialink.dictionary import Dictionary
+from ingenialink.dictionary import Dictionary, SubnodeType, Interface, DictionaryV3
 from ingenialink.enums.register import REG_ACCESS, REG_ADDRESS_TYPE, REG_DTYPE
 from ingenialink.enums.servo import SERVO_STATE
 from ingenialink.exceptions import (
     ILAccessError,
     ILError,
     ILIOError,
     ILRegisterNotFoundError,
     ILStateError,
     ILTimeoutError,
     ILValueError,
+    ILDictionaryParseError,
 )
 from ingenialink.register import Register
 from ingenialink.utils import constants
 from ingenialink.utils._utils import (
     convert_bytes_to_dtype,
     convert_dtype_to_bytes,
     get_drive_identification,
 )
 
 logger = ingenialogger.get_logger(__name__)
 
 OPERATION_TIME_OUT = -3
 
 
+class DictionaryFactory:
+    """Dictionary factory, creates the appropriate dictionary instance according to
+    the file version and connection interface"""
+
+    _VERSION_ABSOLUTE_PATH = "Header/Version"
+    _VERSION_REGEX = r"(\d+)\.*(\d*)"
+    _MAJOR_VERSION_GROUP = 1
+    _MINOR_VERSION_GROUP = 2
+
+    @classmethod
+    def create_dictionary(cls, dictionary_path: str, interface: Interface) -> Dictionary:
+        """Creates a dictionary instance choosing the class depending on dictionary version and
+         connection interface.
+
+        Args:
+            dictionary_path: target dictionary path
+            interface: connection interface
+
+        Returns:
+            Dictionary instance
+
+        Raises:
+            FileNotFoundError: dictionary path does not exist.
+            ILDictionaryParseError: xdf is not well-formed.
+            ILDictionaryParseError: File is not a xdf.
+            NotImplementedError: Dictionary version is not supported.
+
+        """
+        major_version, minor_version = cls.__get_dictionary_version(dictionary_path)
+        if major_version == 3:
+            return DictionaryV3(dictionary_path, interface)
+        if major_version == 2:
+            if interface == Interface.CAN:
+                return CanopenDictionaryV2(dictionary_path)
+            if interface == Interface.ECAT:
+                return EthercatDictionaryV2(dictionary_path)
+            if interface in [Interface.ETH, Interface.EoE]:
+                return EthernetDictionaryV2(dictionary_path)
+            if interface == Interface.VIRTUAL:
+                return VirtualDictionary(dictionary_path)
+        raise NotImplementedError(f"Dictionary version {major_version} is not supported")
+
+    @classmethod
+    def __get_dictionary_version(cls, dictionary_path: str) -> Tuple[int, int]:
+        """Return dictionary version, major and minor version.
+
+        Args:
+            dictionary_path: dictionary path
+
+        Returns:
+            Major and minor version
+
+        Raises:
+            FileNotFoundError: dictionary path does not exist.
+            ILDictionaryParseError: xdf is not well-formed
+            ILDictionaryParseError: File is not a xdf
+
+        """
+        try:
+            with open(dictionary_path, "r", encoding="utf-8") as xdf_file:
+                try:
+                    tree = ET.parse(xdf_file)
+                except ET.ParseError:
+                    raise ILDictionaryParseError(f"File is not a xdf: {dictionary_path}")
+        except FileNotFoundError:
+            raise FileNotFoundError(f"There is not any xdf file in the path: {dictionary_path}")
+        version_element = tree.find(cls._VERSION_ABSOLUTE_PATH)
+        if version_element is None or version_element.text is None:
+            raise ILDictionaryParseError("Version not found")
+        version_str = version_element.text.strip()
+        version_match = re.match(cls._VERSION_REGEX, version_str)
+        if version_match is None:
+            raise ILDictionaryParseError("Version has a wrong format")
+        major_version = int(version_match.group(cls._MAJOR_VERSION_GROUP))
+        if version_match.group(cls._MINOR_VERSION_GROUP):
+            minor_version = int(version_match.group(cls._MINOR_VERSION_GROUP))
+        else:
+            minor_version = 0
+        return major_version, minor_version
+
+
 class ServoStatusListener(threading.Thread):
     """Reads the status word to check if the drive is alive.
 
     Args:
         servo: Servo instance of the drive.
 
     """
@@ -54,15 +141,17 @@
         self.__servo = servo
         self.__stop = False
 
     def run(self) -> None:
         """Checks if the drive is alive by reading the status word register"""
         previous_states: Dict[int, SERVO_STATE] = {}
         while not self.__stop:
-            for subnode in range(1, self.__servo.subnodes):
+            for subnode in self.__servo.subnodes:
+                if self.__servo.subnodes[subnode] != SubnodeType.MOTION:
+                    continue
                 try:
                     current_state = self.__servo.get_state(subnode)
                     if subnode not in previous_states or previous_states[subnode] != current_state:
                         previous_states[subnode] = current_state
                         self.__servo._notify_state(current_state, subnode)
                 except ILError as e:
                     logger.error("Error getting drive status. Exception : %s", e)
@@ -79,19 +168,18 @@
     Args:
         target: Target ID of the servo.
         dictionary_path: Path to the dictionary file.
         servo_status_listener: Toggle the listener of the servo for
             its status, errors, faults, etc.
 
     Raises:
-        ILCreationError: If the servo cannot be created.
+        ILDictionaryParseError: If dictionary can not be parsed.
 
     """
 
-    DICTIONARY_CLASS = Dictionary
     MAX_WRITE_SIZE = 1
 
     STATUS_WORD_REGISTERS = "DRV_STATE_STATUS"
     RESTORE_COCO_ALL = "DRV_RESTORE_COCO_ALL"
     RESTORE_MOCO_ALL_REGISTERS = "DRV_RESTORE_MOCO_ALL"
     STORE_COCO_ALL = "DRV_STORE_COCO_ALL"
     STORE_MOCO_ALL_REGISTERS = "DRV_STORE_MOCO_ALL"
@@ -101,34 +189,36 @@
     PRODUCT_ID_REGISTERS = ["DRV_ID_PRODUCT_CODE_COCO", "DRV_ID_PRODUCT_CODE"]
     REVISION_NUMBER_REGISTERS = ["DRV_ID_REVISION_NUMBER_COCO", "DRV_ID_REVISION_NUMBER"]
     MONITORING_DIST_ENABLE = "MON_DIST_ENABLE"
     MONITORING_REMOVE_DATA = "MON_REMOVE_DATA"
     MONITORING_NUMBER_MAPPED_REGISTERS = "MON_CFG_TOTAL_MAP"
     MONITORING_BYTES_PER_BLOCK = "MON_CFG_BYTES_PER_BLOCK"
     MONITORING_ACTUAL_NUMBER_BYTES = "MON_CFG_BYTES_VALUE"
-    MONITORING_DATA: Optional[Register] = None
+    MONITORING_DATA = "MONITORING_DATA"
     MONITORING_DISTURBANCE_VERSION = "MON_DIST_VERSION"
     DISTURBANCE_ENABLE = "DIST_ENABLE"
     DISTURBANCE_REMOVE_DATA = "DIST_REMOVE_DATA"
     DISTURBANCE_NUMBER_MAPPED_REGISTERS = "DIST_CFG_MAP_REGS"
     DIST_NUMBER_SAMPLES = "DIST_CFG_SAMPLES"
-    DIST_DATA: Register
+    DIST_DATA = "DISTURBANCE_DATA"
     MONITORING_ACTUAL_NUMBER_SAMPLES = "MON_CFG_CYCLES_VALUE"
     DISTURBANCE_REMOVE_REGISTERS_OLD = "DIST_CMD_RM_REGS"
     MONITORING_REMOVE_REGISTERS_OLD = "MON_CMD_RM_REG"
     DISTURBANCE_ADD_REGISTERS_OLD = "DIST_CMD_ADD_REG"
     MONITORING_ADD_REGISTERS_OLD = "MON_OP_ADD_REG"
 
+    interface: Interface
+
     def __init__(
         self,
         target: Union[int, str],
         dictionary_path: str,
         servo_status_listener: bool = False,
     ):
-        self._dictionary = self.DICTIONARY_CLASS(dictionary_path)
+        self._dictionary = DictionaryFactory.create_dictionary(dictionary_path, self.interface)
         self.target = target
         prod_name = ""
         if self.dictionary.part_number is not None:
             prod_name = self.dictionary.part_number
         self._info = None
         self.name = DEFAULT_DRIVE_NAME
         self.full_name = f"{prod_name} {self.name} ({self.target})"
@@ -143,15 +233,15 @@
         """SERVO_UNITS_ACC: Acceleration units."""
         self._lock = threading.Lock()
         self.__observers_servo_state: List[Callable[[SERVO_STATE, None, int], Any]] = []
         self.__listener_servo_status: Optional[ServoStatusListener] = None
         self.__monitoring_data: Dict[int, List[Union[int, float]]] = {}
         self.__monitoring_size: Dict[int, int] = {}
         self.__monitoring_dtype: Dict[int, REG_DTYPE] = {}
-        self.__disturbance_data = bytearray()
+        self.__disturbance_data = bytes()
         self.__disturbance_size: Dict[int, int] = {}
         self.__disturbance_dtype: Dict[int, str] = {}
         if servo_status_listener:
             self.start_status_listener()
         else:
             self.stop_status_listener()
 
@@ -186,15 +276,15 @@
         Args:
             config_file: Path to the dictionary.
             subnode: Subnode of the axis.
 
         Raises:
             FileNotFoundError: If the configuration file cannot be found.
             ValueError: If a configuration file from a subnode different from 0
-            is attempted to be loaded to subnode 0.
+                is attempted to be loaded to subnode 0.
             ValueError: If an invalid subnode is provided.
 
         """
         if subnode is not None and (not isinstance(subnode, int) or subnode < 0):
             raise ValueError("Invalid subnode")
         _, registers = self._read_configuration_file(config_file)
 
@@ -254,23 +344,23 @@
         device.set("RevisionNumber", str(rev_number))
         device.set("firmwareVersion", str(self.dictionary.firmware_version))
 
         access_ops = {value: key for key, value in self.dictionary.access_xdf_options.items()}
         dtype_ops = {value: key for key, value in self.dictionary.dtype_xdf_options.items()}
 
         if subnode is None:
-            subnodes = list(range(self.dictionary.subnodes))
+            subnodes = list(self.dictionary.subnodes)
         else:
             subnodes = [subnode]
 
         for subnode in subnodes:
             registers_dict = self.dictionary.registers(subnode=subnode)
             for reg_id, register in registers_dict.items():
-                if (register.address_type == REG_ADDRESS_TYPE.NVM_NONE) or (
-                    register.access != REG_ACCESS.RW
+                if (register.access != REG_ACCESS.RW) or (
+                    register.address_type == REG_ADDRESS_TYPE.NVM_NONE
                 ):
                     continue
                 register_xml = ET.SubElement(registers, "Register")
                 register_xml.set("access", access_ops[register.access])
                 register_xml.set("dtype", dtype_ops[register.dtype])
                 register_xml.set("id", reg_id)
                 self.__update_register_dict(register_xml, subnode)
@@ -319,15 +409,15 @@
 
         .. note::
             The drive needs a power cycle after this
             in order for the changes to be properly applied.
 
         Args:
             subnode: Subnode of the axis. `None` by default which restores
-            all the parameters.
+                all the parameters.
 
         Raises:
             ILError: Invalid subnode.
             ILObjectNotExist: Failed to write to the registers.
 
         """
         if subnode is None:
@@ -369,21 +459,22 @@
                 try:
                     self.write(reg=self.STORE_COCO_ALL, data=PASSWORD_STORE_ALL, subnode=0)
                     logger.info("Store all successfully done.")
                 except ILError as e:
                     logger.warning(f"Store all COCO failed. Reason: {e}. Trying MOCO...")
                     r = -1
                 if r < 0:
-                    for dict_subnode in range(1, self.dictionary.subnodes):
-                        self.write(
-                            reg=self.STORE_MOCO_ALL_REGISTERS,
-                            data=PASSWORD_STORE_ALL,
-                            subnode=dict_subnode,
-                        )
-                        logger.info(f"Store axis {dict_subnode} successfully done.")
+                    for dict_subnode in self.dictionary.subnodes:
+                        if self.dictionary.subnodes[dict_subnode] == SubnodeType.MOTION:
+                            self.write(
+                                reg=self.STORE_MOCO_ALL_REGISTERS,
+                                data=PASSWORD_STORE_ALL,
+                                subnode=dict_subnode,
+                            )
+                            logger.info(f"Store axis {dict_subnode} successfully done.")
             elif subnode == 0:
                 # Store subnode 0
                 self.write(reg=self.STORE_COCO_ALL, data=PASSWORD_STORE_RESTORE_SUB_0, subnode=0)
             elif subnode > 0:
                 # Store axis
                 self.write(
                     reg=self.STORE_MOCO_ALL_REGISTERS, data=PASSWORD_STORE_ALL, subnode=subnode
@@ -693,15 +784,15 @@
     def disturbance_disable(self) -> None:
         """Disable disturbance process."""
         self.write(self.DISTURBANCE_ENABLE, data=0, subnode=0)
 
     def disturbance_remove_data(self) -> None:
         """Remove disturbance data."""
         self.write(self.DISTURBANCE_REMOVE_DATA, data=1, subnode=0)
-        self.disturbance_data = bytearray()
+        self.disturbance_data = bytes()
 
     def disturbance_set_mapped_register(
         self, channel: int, address: int, subnode: int, dtype: int, size: int
     ) -> None:
         """Set monitoring mapped register.
 
         Args:
@@ -732,15 +823,15 @@
 
     def disturbance_remove_all_mapped_registers(self) -> None:
         """Remove all disturbance mapped registers."""
         try:
             self.write(self.DISTURBANCE_NUMBER_MAPPED_REGISTERS, data=0, subnode=0)
         except ILAccessError:
             self.write(self.DISTURBANCE_REMOVE_REGISTERS_OLD, data=1, subnode=0)
-        self.__disturbance_data = bytearray()
+        self.__disturbance_data = bytes()
         self.__disturbance_size = {}
         self.__disturbance_dtype = {}
 
     def subscribe_to_status(self, callback: Callable[[SERVO_STATE, None, int], Any]) -> None:
         """Subscribe to state changes.
 
         Args:
@@ -906,17 +997,17 @@
         """Update the number of mapped monitoring registers."""
         self.write(
             self.MONITORING_NUMBER_MAPPED_REGISTERS,
             data=self.monitoring_number_mapped_registers + 1,
             subnode=0,
         )
 
-    def __monitoring_process_data(self, monitoring_data: List[bytearray]) -> None:
+    def __monitoring_process_data(self, monitoring_data: List[bytes]) -> None:
         """Arrange monitoring data."""
-        data_bytes = bytearray()
+        data_bytes = bytes()
         for i in range(len(monitoring_data)):
             data_bytes += monitoring_data[i]
         bytes_per_block = self.monitoring_get_bytes_per_block()
         number_of_blocks = len(data_bytes) // bytes_per_block
         number_of_channels = self.monitoring_get_num_mapped_registers()
         for channel in range(number_of_channels):
             self.__monitoring_data[channel] = []
@@ -953,15 +1044,15 @@
 
     def _disturbance_create_data_chunks(
         self,
         channels: Union[int, List[int]],
         dtypes: Union[REG_DTYPE, List[REG_DTYPE]],
         data_arr: Union[List[Union[int, float]], List[List[Union[int, float]]]],
         max_size: int,
-    ) -> Tuple[bytearray, List[bytearray]]:
+    ) -> Tuple[bytes, List[bytes]]:
         """Divide disturbance data into chunks.
 
         Args:
             channels: Channel identifier.
             dtypes: Data type.
             data_arr: Data array.
             max_size: Max chunk size in bytes.
@@ -977,15 +1068,15 @@
         if not isinstance(data_arr[0], list):
             num_samples = len(data_arr)
             data_arr_aux = [data_arr]  # type: ignore [list-item]
         else:
             num_samples = len(data_arr[0])
             data_arr_aux = data_arr  # type: ignore [assignment]
         self.write(self.DIST_NUMBER_SAMPLES, num_samples, subnode=0)
-        data = bytearray()
+        data = bytes()
         for sample_idx in range(num_samples):
             for channel in range(len(data_arr_aux)):
                 val = convert_dtype_to_bytes(data_arr_aux[channel][sample_idx], dtypes[channel])
                 data += val
         chunks = [data[i : i + max_size] for i in range(0, len(data), max_size)]
         return data, chunks
 
@@ -1015,15 +1106,17 @@
             raise ILAccessError("Register is Read-only")
         if not isinstance(data, bytes):
             value = convert_dtype_to_bytes(data, _reg.dtype)
         else:
             value = data
         self._write_raw(_reg, value, **kwargs)
 
-    def read(self, reg: Union[str, Register], subnode: int = 1) -> Union[int, float, str]:
+    def read(
+        self, reg: Union[str, Register], subnode: int = 1, **kwargs: Any
+    ) -> Union[int, float, str, bytes]:
         """Read a register value from servo.
 
         Args:
             reg: Register.
             subnode: Target axis of the drive.
 
         Returns:
@@ -1036,26 +1129,28 @@
 
         """
         _reg = self._get_reg(reg, subnode)
         access = _reg.access
         if access == REG_ACCESS.WO:
             raise ILAccessError("Register is Write-only")
 
-        raw_read = self._read_raw(_reg)
+        raw_read = self._read_raw(_reg, **kwargs)
+        if _reg.dtype == REG_DTYPE.BYTE_ARRAY_512:
+            return raw_read
         value = convert_bytes_to_dtype(raw_read, _reg.dtype)
         return value
 
     def replace_dictionary(self, dictionary: str) -> None:
         """Deletes and creates a new instance of the dictionary.
 
         Args:
             dictionary: Path to the dictionary.
 
         """
-        self._dictionary = self.DICTIONARY_CLASS(dictionary)
+        self._dictionary = DictionaryFactory.create_dictionary(dictionary, self.interface)
 
     def disturbance_write_data(
         self,
         channels: Union[int, List[int]],
         dtypes: Union[REG_DTYPE, List[REG_DTYPE]],
         data_arr: Union[List[Union[int, float]], List[List[Union[int, float]]]],
     ) -> None:
@@ -1063,35 +1158,49 @@
 
         Args:
             channels: Channel identifier.
             dtypes: Data type.
             data_arr: Data array.
 
         """
-        if self.DIST_DATA is None:
-            return
         try:
             data, chunks = self._disturbance_create_data_chunks(
                 channels, dtypes, data_arr, self.MAX_WRITE_SIZE
             )
         except OverflowError as e:
             raise ILValueError("Disturbance data cannot be written.") from e
         for chunk in chunks:
             self._disturbance_write_data(chunk)
         self.disturbance_data = data
 
-    def _monitoring_read_data(self) -> bytearray:
-        """Read monitoring data frame."""
-        if self.MONITORING_DATA is None:
-            return bytearray()
-        return self._read_raw(self.MONITORING_DATA)
-
-    def _disturbance_write_data(self, data: bytes) -> None:
-        """Write disturbance data."""
-        return self._write_raw(self.DIST_DATA, data=data)
+    def _monitoring_read_data(self, **kwargs: Any) -> bytes:
+        """Read monitoring data frame.
+
+        Raises:
+            NotImplementedError: If monitoring is not supported by the device.
+
+        """
+        if self.MONITORING_DATA not in self.dictionary.registers(0):
+            raise NotImplementedError("Monitoring is not supported by this device.")
+        if not isinstance(data := self.read(self.MONITORING_DATA, subnode=0, **kwargs), bytes):
+            raise ValueError(
+                f"Error reading monitoring data. Expected type bytes, got {type(data)}"
+            )
+        return data
+
+    def _disturbance_write_data(self, data: bytes, **kwargs: Any) -> None:
+        """Write disturbance data.
+
+        Raises:
+            NotImplementedError: If disturbance is not supported by the device.
+
+        """
+        if self.DIST_DATA not in self.dictionary.registers(0):
+            raise NotImplementedError("Disturbance is not supported by this device.")
+        return self.write(self.DIST_DATA, subnode=0, data=data, **kwargs)
 
     @abstractmethod
     def _write_raw(self, reg: Register, data: bytes) -> None:
         """Write raw bytes to a target register.
 
         Args:
             reg: Target register to be written.
@@ -1100,15 +1209,15 @@
         Raises:
             ILIOError: Error writing the register.
 
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _read_raw(self, reg: Register) -> bytearray:
+    def _read_raw(self, reg: Register) -> bytes:
         """Read raw bytes from a target register.
 
         Args:
             reg: Register.
 
         Returns:
             Raw bytes reading from servo.
@@ -1120,32 +1229,41 @@
         raise NotImplementedError
 
     @property
     def dictionary(self) -> Dictionary:
         """Returns dictionary object"""
         return self._dictionary
 
+    @dictionary.setter
+    def dictionary(self, dictionary: Dictionary) -> None:
+        """Sets the dictionary object"""
+        self._dictionary = dictionary
+
     @property
     def full_name(self) -> str:
         """Drive full name."""
         return self.__full_name
 
     @full_name.setter
     def full_name(self, new_name: str) -> None:
         self.__full_name = new_name
 
     @property
     def status(self) -> Dict[int, SERVO_STATE]:
         """Servo status."""
-        status = {subnode: self.get_state(subnode) for subnode in range(1, self.subnodes)}
+        status = {
+            subnode: self.get_state(subnode)
+            for subnode in self.subnodes
+            if self.subnodes[subnode] == SubnodeType.MOTION
+        }
         return status
 
     @property
-    def subnodes(self) -> int:
-        """Number of subnodes."""
+    def subnodes(self) -> Dict[int, SubnodeType]:
+        """Dictionary of subnode ids and their type"""
         return self.dictionary.subnodes
 
     @property
     def errors(self) -> Dict[int, List[Optional[str]]]:
         """Errors."""
         if self.dictionary.errors:
             return self.dictionary.errors.errors
@@ -1191,25 +1309,25 @@
             Current monitoring data size in bytes.
 
         """
         number_of_samples = int(self.read("MON_CFG_WINDOW_SAMP", subnode=0))
         return self.monitoring_get_bytes_per_block() * number_of_samples
 
     @property
-    def disturbance_data(self) -> bytearray:
+    def disturbance_data(self) -> bytes:
         """Obtain disturbance data.
 
         Returns:
             Current disturbance data.
 
         """
         return self.__disturbance_data
 
     @disturbance_data.setter
-    def disturbance_data(self, value: bytearray) -> None:
+    def disturbance_data(self, value: bytes) -> None:
         """Set disturbance data.
 
         Args:
             value: Array with the disturbance to send.
 
         """
         self.__disturbance_data = value
```

### Comparing `ingenialink-7.2.0/ingenialink/utils/_utils.py` & `ingenialink-7.3.0/ingenialink/utils/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import logging
 import struct
 import warnings
 import xml.etree.ElementTree as ET
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Union
 
 import ingenialogger
@@ -24,14 +25,15 @@
     REG_DTYPE.U16: (2, False),
     REG_DTYPE.S16: (2, True),
     REG_DTYPE.U32: (4, False),
     REG_DTYPE.S32: (4, True),
     REG_DTYPE.U64: (8, False),
     REG_DTYPE.S64: (8, True),
     REG_DTYPE.FLOAT: (4, True),
+    REG_DTYPE.BOOL: (1, False),
 }
 
 dtype_length_bits: Dict[REG_DTYPE, int] = {
     REG_DTYPE.U8: 8,
     REG_DTYPE.S8: 8,
     REG_DTYPE.U16: 16,
     REG_DTYPE.S16: 16,
@@ -39,14 +41,16 @@
     REG_DTYPE.S32: 32,
     REG_DTYPE.U64: 64,
     REG_DTYPE.S64: 64,
     REG_DTYPE.FLOAT: 32,
     REG_DTYPE.BOOL: 1,
 }
 
+VALID_BIT_REGISTER_VALUES = [0, 1, True, False]
+
 
 def deprecated(
     custom_msg: Optional[str] = None, new_func_name: Optional[str] = None
 ) -> Callable[..., Any]:
     """This is a decorator which can be used to mark functions as deprecated.
     It will result in a warning being emitted when the function is used. We use
     this decorator instead of any deprecation library because all libraries raise
@@ -68,14 +72,24 @@
             return func(*args, **kwargs)
 
         return wrapped_method
 
     return wrap
 
 
+class DisableLogger:
+    """Context manager to disable all logs."""
+
+    def __enter__(self) -> None:
+        logging.disable(logging.CRITICAL)
+
+    def __exit__(self, *args: Any) -> None:
+        logging.disable(logging.NOTSET)
+
+
 def to_ms(s: Union[int, float]) -> int:
     """Convert from seconds to milliseconds.
 
     Args:
         s: Value in seconds.
 
     Returns:
@@ -230,26 +244,34 @@
     elif dtype == REG_DTYPE.STR:
         try:
             value = data.split(b"\x00")[0].decode("utf-8")
         except UnicodeDecodeError as e:
             raise ILValueError(f"Can't decode {e.object!r} to utf-8 string") from e
     else:
         value = int.from_bytes(data, "little", signed=signed)
+    if dtype == REG_DTYPE.BOOL:
+        value = bool(value)
     if not isinstance(value, (int, float, str)):
         raise ILValueError(f"Bad data type: {type(value)}")
     return value
 
 
 def convert_dtype_to_bytes(data: Union[int, float, str, bytes], dtype: REG_DTYPE) -> bytes:
     """Convert data in dtype to bytes.
     Args:
         data: Data to convert.
         dtype: Data type.
     """
-    if dtype == REG_DTYPE.DOMAIN:
+    if (
+        dtype == REG_DTYPE.BOOL
+        and data not in VALID_BIT_REGISTER_VALUES
+        and not isinstance(data, bytes)
+    ):
+        raise ValueError(f"Invalid value. Expected values: {VALID_BIT_REGISTER_VALUES}, got {data}")
+    if dtype == REG_DTYPE.BYTE_ARRAY_512:
         if not isinstance(data, bytes):
             raise ValueError(f"Expected data of type bytes, but got {type(data)}")
         return data
     if dtype == REG_DTYPE.FLOAT:
         if not isinstance(data, (float, int)):
             raise ValueError(f"Expected data of type float, but got {type(data)}")
         return struct.pack("f", float(data))
```

### Comparing `ingenialink-7.2.0/ingenialink/utils/constants.py` & `ingenialink-7.3.0/ingenialink/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/utils/errors.py` & `ingenialink-7.3.0/ingenialink/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/utils/mcb.py` & `ingenialink-7.3.0/ingenialink/utils/mcb.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/utils/udp.py` & `ingenialink-7.3.0/ingenialink/utils/udp.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink/virtual/network.py` & `ingenialink-7.3.0/ingenialink/virtual/network.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/ingenialink.egg-info/PKG-INFO` & `ingenialink-7.3.0/ingenialink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ingenialink
-Version: 7.2.0
+Version: 7.3.0
 Summary: IngeniaLink Communications Library
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.2.0
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingenialink-python/7.3.0
 Project-URL: Source, https://github.com/ingeniamc/ingenialink-python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ingenialink-7.2.0/ingenialink.egg-info/SOURCES.txt` & `ingenialink-7.3.0/ingenialink.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ingenialink.egg-info/PKG-INFO
 ingenialink.egg-info/SOURCES.txt
 ingenialink.egg-info/dependency_links.txt
 ingenialink.egg-info/requires.txt
 ingenialink.egg-info/top_level.txt
 ingenialink/bin/__init__.py
 ingenialink/bin/FoE/__init__.py
+ingenialink/bin/FoE/linux/FoEUpdateFirmware
 ingenialink/bin/FoE/win_64x/FoEUpdateFirmware.exe
 ingenialink/canopen/__init__.py
 ingenialink/canopen/dictionary.py
 ingenialink/canopen/network.py
 ingenialink/canopen/register.py
 ingenialink/canopen/servo.py
 ingenialink/enums/__init__.py
```

### Comparing `ingenialink-7.2.0/setup.py` & `ingenialink-7.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/tests/test_mcb.py` & `ingenialink-7.3.0/tests/test_mcb.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/tests/test_servo.py` & `ingenialink-7.3.0/tests/test_servo.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,17 +162,17 @@
             elif dtype == "float":
                 assert value == pytest.approx(float(storage), 0.0001)
             else:
                 assert value == int(storage)
 
 
 @pytest.mark.no_connection
-def test_read_configuration_file(read_config):
+def test_read_configuration_file():
     test_file = "./tests/resources/test_config_file.xcf"
-    servo = CanopenServo("test", 0, read_config["canopen"]["dictionary"])
+    servo = CanopenServo("test", 0, "./tests/resources/canopen/test_dict_can.xdf")
     device, registers = servo._read_configuration_file(test_file)
 
     assert device.attrib.get("PartNumber") == "EVE-NET-C"
     assert device.attrib.get("Interface") == "CAN"
     assert device.attrib.get("firmwareVersion") == "2.3.0"
     assert device.attrib.get("ProductCode") == "493840"
     assert device.attrib.get("RevisionNumber") == "196634"
```

### Comparing `ingenialink-7.2.0/tests/test_utils.py` & `ingenialink-7.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/tests/test_virtual_drive.py` & `ingenialink-7.3.0/tests/test_virtual_drive.py`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/virtual_drive/core.py` & `ingenialink-7.3.0/virtual_drive/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pathlib
+import platform
 import socket
 import time
 from enum import Enum, IntEnum
 from threading import Thread, Timer
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
@@ -1021,15 +1022,15 @@
     """
 
     FREQ_DIVIDER_REG = "MON_DIST_FREQ_DIV"
     BUFFER_SIZE_REG = "MON_CFG_WINDOW_SAMP"
     NUMBER_MAP_REGS = "MON_CFG_TOTAL_MAP"
     MAP_REG_CFG = "MON_CFG_REG{}_MAP"
     BYTES_PER_BLOCK_REG = "MON_CFG_BYTES_PER_BLOCK"
-    DATA_REG = "MON_DATA"
+    DATA_REG = "MONITORING_DATA"
     TRIGGER_TYPE_REG = "MON_CFG_SOC_TYPE"
     AVAILABLE_BYTES_REG = "MON_CFG_BYTES_VALUE"
     STATUS_REGISTER = "MON_DIST_STATUS"
 
     def __init__(self, drive: "VirtualDrive") -> None:
         self.start_time = 0.0
         super().__init__(drive)
@@ -1109,15 +1110,15 @@
                 size = self.channels_size[channel]
                 if self.channels_dtype[channel] != REG_DTYPE.FLOAT:
                     value = int(value)
                 sample_bytes = convert_dtype_to_bytes(value, self.channels_dtype[channel])
                 if len(sample_bytes) < size:
                     sample_bytes += b"0" * (size - len(sample_bytes))
                 byte_array += sample_bytes
-        self.drive.set_value_by_id(0, "MON_DATA", byte_array)
+        self.drive.set_value_by_id(0, "MONITORING_DATA", byte_array)
 
     @property
     def trigger_type(self) -> int:
         """Trigger type Auto(0), Force (1) or Rising or Failing (2)."""
         value = self.drive.get_value_by_id(0, self.TRIGGER_TYPE_REG)
         if isinstance(value, int):
             return value
@@ -1135,15 +1136,15 @@
 
     FREQ_DIVIDER_REG = "DIST_FREQ_DIV"
     BUFFER_SIZE_REG = "DIST_CFG_SAMPLES"
     NUMBER_MAP_REGS = "DIST_CFG_MAP_REGS"
     MAP_REG_CFG = "DIST_CFG_REG{}_MAP"
     BYTES_PER_BLOCK_REG = "DIST_CFG_BYTES_PER_BLOCK"
     AVAILABLE_BYTES_REG = "DIST_CFG_BYTES"
-    DATA_REG = "DIST_DATA"
+    DATA_REG = "DISTURBANCE_DATA"
     STATUS_REGISTER = "DIST_STATUS"
 
     def __init__(self, drive: "VirtualDrive") -> None:
         self.start_time = 0.0
         self.received_bytes = bytes()
         super().__init__(drive)
 
@@ -1277,14 +1278,17 @@
         self._plant_open_loop_vol_to_curr_b = PlantOpenLoopVoltageToCurrentB(self)
         self._plant_open_loop_vol_to_curr_c = PlantOpenLoopVoltageToCurrentC(self)
 
         self.phasing = VirtualPhasing(self)
         self.internal_generator = VirtualInternalGenerator(self)
 
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        if platform.system() != "Windows":
+            # On Linux, the SO_REUSEADDR should be set to avoid keeping the socket opened.
+            self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
     def run(self) -> None:
         """Open socket, listen and decode messages."""
         server_address = (self.ip, self.port)
         self.socket.bind(server_address)
         self.socket.settimeout(2)
         while not self.__stop:
@@ -1331,15 +1335,15 @@
             data: Received data frame.
 
         Returns:
             bytes: Response to be sent.
         """
         value = self.get_value_by_id(register.subnode, str(register.identifier))
         if (
-            register.address == self.id_to_address(0, "MON_DATA")
+            register.address == self.id_to_address(0, "MONITORING_DATA")
             and isinstance(value, bytes)
             and self._monitoring
         ):
             self._monitoring.update_data()
             response = self._response_monitoring_data(value)
         else:
             data = convert_dtype_to_bytes(value, register.dtype)
@@ -1370,50 +1374,54 @@
                 continue
             self.set_value_by_id(
                 subnode,
                 element.attrib["id"],
                 cast_data.get(reg_dtype, int)(reg_data),
             )
         value: Union[str, int]
-        for subnode in range(self.__dictionary.subnodes):
+        for subnode in self.__dictionary.subnodes:
             for reg_id, reg in self.__dictionary.registers(subnode).items():
                 if reg._storage is not None:
                     continue
                 elif reg.enums_count > 0:
                     value = next(iter(reg.enums.values()))
                 elif reg.dtype == REG_DTYPE.STR:
                     value = ""
                 else:
                     value = 0
                 self.set_value_by_id(subnode, reg_id, value)
 
     def _update_registers(self) -> None:
         """Force storage_valid at each register and add registers that are not in the dictionary."""
-        for subnode in range(self.__dictionary.subnodes):
+        for subnode in self.__dictionary.subnodes:
             self.__reg_address_to_id[subnode] = {}
             for reg_id, reg in self.__dictionary.registers(subnode).items():
+                if not isinstance(reg, EthernetRegister):
+                    raise ValueError(f"Register {reg_id} is not an EthernetRegister")
                 self.__reg_address_to_id[subnode][reg.address] = reg_id
                 self.__dictionary.registers(subnode)[reg_id].storage_valid = True
 
         custom_regs = {
-            "MON_DATA": EthernetServo.MONITORING_DATA,
-            "DIST_DATA": EthernetServo.DIST_DATA,
+            "MONITORING_DATA": self.__dictionary.registers(0)[EthernetServo.MONITORING_DATA],
+            "DISTURBANCE_DATA": self.__dictionary.registers(0)[EthernetServo.DIST_DATA],
         }
         for id, reg in custom_regs.items():
+            if not isinstance(reg, EthernetRegister):
+                raise ValueError
             register = EthernetRegister(
-                reg.address, REG_DTYPE.DOMAIN, reg.access, identifier=id, subnode=reg.subnode
+                reg.address, REG_DTYPE.BYTE_ARRAY_512, reg.access, identifier=id, subnode=reg.subnode
             )
             self.__dictionary._add_register_list(register)
             self.__dictionary.registers(reg.subnode)[id].storage_valid = True
 
             self.__reg_address_to_id[reg.subnode][reg.address] = id
 
     def _init_register_signals(self) -> None:
         """Init signals, vector time and noise amplitude for each register."""
-        for subnode in range(self.__dictionary.subnodes):
+        for subnode in self.__dictionary.subnodes:
             for reg_id in self.__dictionary.registers(subnode).keys():
                 self.reg_signals[reg_id] = np.array([])
                 self.reg_time[reg_id] = np.array([])
                 self.reg_noise_amplitude[reg_id] = 0.0
 
     def __send(self, response: bytes, address: Tuple[str, int]) -> None:
         """Send a message and update log.
@@ -1433,19 +1441,19 @@
 
         Returns:
             MCB frame.
         """
         if not self._monitoring:
             return bytes(1)
         sent_cmd = self.ACK_CMD
-        reg_add = self.id_to_address(0, "MON_DATA")
+        reg_add = self.id_to_address(0, "MONITORING_DATA")
         limit = min(len(data), MONITORING_BUFFER_SIZE)
         response = MCB.build_mcb_frame(sent_cmd, 0, reg_add, data[:limit])
         data_left = data[limit:]
-        self.set_value_by_id(0, "MON_DATA", data_left)
+        self.set_value_by_id(0, "MONITORING_DATA", data_left)
         self._monitoring.available_bytes = len(data_left)
         return response
 
     def __log(self, ip_port: Tuple[str, int], message: bytes, msg_type: MSG_TYPE) -> None:
         """Updates log.
 
         Args:
@@ -1498,15 +1506,15 @@
             self._disturbance.enable()
             self.__emulate_plants()
         if reg_id == "DIST_ENABLE" and subnode == 0 and value == 0 and self._disturbance:
             self._disturbance.disable()
             self.__clean_plant_signals()
         if reg_id == "DIST_REMOVE_DATA" and subnode == 0 and value == 1 and self._disturbance:
             self._disturbance.remove_data()
-        if reg_id == "DIST_DATA" and subnode == 0 and self._disturbance:
+        if reg_id == "DISTURBANCE_DATA" and subnode == 0 and self._disturbance:
             self._disturbance.append_data(data)
         if reg_id == "DRV_OP_CMD":
             self.operation_mode = int(value)
             self.__clean_plant_signals()
         if reg_id == "DRV_STATE_CONTROL" and subnode == 1 and (int(value) & IL_MC_CW_EO):
             self.__set_motor_enable()
         if reg_id == "DRV_STATE_CONTROL" and subnode == 1 and (value == constants.IL_MC_PDS_CMD_DV):
@@ -1567,25 +1575,27 @@
             address: Register address.
 
         Returns:
             Register ID.
         """
         return self.__reg_address_to_id[subnode][address]
 
-    def id_to_address(self, subnode: int, id: str) -> int:
-        """Converts a register address into an ID.
+    def id_to_address(self, subnode: int, uid: str) -> int:
+        """Return address of Register with the target subnode and UID
 
         Args:
             subnode: Subnode.
-            id: Register ID.
+            uid: Register UID.
 
         Returns:
             Register address.
         """
-        register = self.__dictionary.registers(subnode)[id]
+        register = self.__dictionary.registers(subnode)[uid]
+        if not isinstance(register, EthernetRegister):
+            raise ValueError(f"Register {uid} is not an EthernetRegister")
         return register.address
 
     def get_value_by_id(self, subnode: int, id: str) -> Union[int, float, str, bytes]:
         """Returns a register value by its ID.
 
         Args:
             subnode: Subnode.
@@ -1633,15 +1643,15 @@
         Args:
             subnode: Subnode.
             id: Register ID.
 
         Returns:
             Register value.
         """
-        return subnode < self.__dictionary.subnodes and id in self.__dictionary.registers(subnode)
+        return subnode in self.__dictionary.subnodes and id in self.__dictionary.registers(subnode)
 
     def get_register(
         self, subnode: int, address: Optional[int] = None, id: Optional[str] = None
     ) -> EthernetRegister:
         """Returns a register by its address or ID.
 
         Args:
@@ -1656,15 +1666,18 @@
             ValueError: If both address and id are None.
         """
         if address is not None:
             id = self.address_to_id(subnode, address)
         else:
             if id is None:
                 raise ValueError("Register address or id should be passed")
-        return self.__dictionary.registers(subnode)[id]
+        register = self.__dictionary.registers(subnode)[id]
+        if not isinstance(register, EthernetRegister):
+            raise ValueError(f"Register {id} is not an EthernetRegister")
+        return register
 
     def __set_motor_enable(self) -> None:
         """Set the enabled state."""
         new_status_word = (
             self.status_word & ~constants.IL_MC_PDS_STA_OE_MSK | constants.IL_MC_PDS_STA_OE
         )
         self.status_word = new_status_word
```

### Comparing `ingenialink-7.2.0/virtual_drive/resources/virtual_drive.xcf` & `ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xcf`

 * *Files identical despite different names*

### Comparing `ingenialink-7.2.0/virtual_drive/resources/virtual_drive.xdf` & `ingenialink-7.3.0/virtual_drive/resources/virtual_drive.xdf`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (462), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -11916,4814 +11916,4813 @@
 0002e8b0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
 0002e8c0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
 0002e8d0: 206c 616e 673d 2265 6e5f 5553 223e 5573   lang="en_US">Us
 0002e8e0: 6572 206f 7665 7220 766f 6c74 6167 6520  er over voltage 
 0002e8f0: 6c65 7665 6c3c 2f4c 6162 656c 3e0d 0a20  level</Label>.. 
 0002e900: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
 0002e910: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-0002e920: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-0002e930: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-0002e940: 733d 2272 7722 2061 6464 7265 7373 5f74  s="rw" address_t
-0002e950: 7970 653d 224e 564d 5f43 4647 2220 6164  ype="NVM_CFG" ad
-0002e960: 6472 6573 733d 2230 7830 3633 3122 2064  dress="0x0631" d
-0002e970: 7479 7065 3d22 666c 6f61 7422 2069 643d  type="float" id=
-0002e980: 2244 5256 5f50 524f 545f 5553 4552 5f55  "DRV_PROT_USER_U
-0002e990: 4e44 4552 5f56 4f4c 5422 2075 6e69 7473  NDER_VOLT" units
-0002e9a0: 3d22 5622 2073 7562 6e6f 6465 3d22 3122  ="V" subnode="1"
-0002e9b0: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
-0002e9c0: 2064 6573 633d 2249 6e64 6963 6174 6573   desc="Indicates
-0002e9d0: 2074 6865 206d 696e 696d 756d 2076 6f6c   the minimum vol
-0002e9e0: 7461 6765 2072 6571 7569 7265 6420 6279  tage required by
-0002e9f0: 2074 6865 2075 7365 7220 666f 7220 6120   the user for a 
-0002ea00: 7072 6f70 6572 206f 7065 7261 7469 6f6e  proper operation
-0002ea10: 2220 6361 745f 6964 3d22 5052 4f54 4543  " cat_id="PROTEC
-0002ea20: 5449 4f4e 5322 3e0d 0a20 2020 2020 2020  TIONS">..       
-0002ea30: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-0002ea40: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-0002ea50: 6c61 6e67 3d22 656e 5f55 5322 3e55 7365  lang="en_US">Use
-0002ea60: 7220 756e 6465 7220 766f 6c74 6167 6520  r under voltage 
-0002ea70: 6c65 7665 6c3c 2f4c 6162 656c 3e0d 0a20  level</Label>.. 
-0002ea80: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-0002ea90: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-0002eaa0: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-0002eab0: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-0002eac0: 733d 2272 7722 2061 6464 7265 7373 5f74  s="rw" address_t
-0002ead0: 7970 653d 224e 564d 5f43 4647 2220 6164  ype="NVM_CFG" ad
-0002eae0: 6472 6573 733d 2230 7830 3633 3222 2064  dress="0x0632" d
-0002eaf0: 7479 7065 3d22 666c 6f61 7422 2069 643d  type="float" id=
-0002eb00: 2244 5256 5f50 524f 545f 5553 4552 5f4f  "DRV_PROT_USER_O
-0002eb10: 5645 525f 5445 4d50 2220 756e 6974 733d  VER_TEMP" units=
-0002eb20: 22c2 ba43 2220 7375 626e 6f64 653d 2231  "..C" subnode="1
-0002eb30: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-0002eb40: 2220 6465 7363 3d22 496e 6469 6361 7465  " desc="Indicate
-0002eb50: 7320 7468 6520 6d61 7869 6d75 6d20 7465  s the maximum te
-0002eb60: 6d70 6572 6174 7572 6520 6f66 2074 6865  mperature of the
-0002eb70: 2064 7269 7665 2061 6c6c 6f77 6564 2062   drive allowed b
-0002eb80: 7920 7468 6520 7573 6572 2220 6361 745f  y the user" cat_
-0002eb90: 6964 3d22 5052 4f54 4543 5449 4f4e 5322  id="PROTECTIONS"
-0002eba0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-0002ebb0: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-0002ebc0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-0002ebd0: 656e 5f55 5322 3e55 7365 7220 6f76 6572  en_US">User over
-0002ebe0: 2074 656d 7065 7261 7475 7265 206c 6576   temperature lev
-0002ebf0: 656c 3c2f 4c61 6265 6c3e 0d0a 2020 2020  el</Label>..    
-0002ec00: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-0002ec10: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-0002ec20: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-0002ec30: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-0002ec40: 7277 2220 6164 6472 6573 735f 7479 7065  rw" address_type
-0002ec50: 3d22 4e56 4d5f 4346 4722 2061 6464 7265  ="NVM_CFG" addre
-0002ec60: 7373 3d22 3078 3036 3333 2220 6474 7970  ss="0x0633" dtyp
-0002ec70: 653d 2266 6c6f 6174 2220 6964 3d22 4452  e="float" id="DR
-0002ec80: 565f 5052 4f54 5f55 5345 525f 554e 4445  V_PROT_USER_UNDE
-0002ec90: 525f 5445 4d50 2220 756e 6974 733d 22c2  R_TEMP" units=".
-0002eca0: ba43 2220 7375 626e 6f64 653d 2231 2220  .C" subnode="1" 
-0002ecb0: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
-0002ecc0: 6465 7363 3d22 496e 6469 6361 7465 7320  desc="Indicates 
-0002ecd0: 7468 6520 6d69 6e69 6d75 6d20 7465 6d70  the minimum temp
-0002ece0: 6572 6174 7572 6520 6f66 2074 6865 2064  erature of the d
-0002ecf0: 7269 7665 2061 6c6c 6f77 6564 2062 7920  rive allowed by 
-0002ed00: 7468 6520 7573 6572 2220 6361 745f 6964  the user" cat_id
-0002ed10: 3d22 5052 4f54 4543 5449 4f4e 5322 3e0d  ="PROTECTIONS">.
-0002ed20: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-0002ed30: 6c73 3e0d 0a20 2020 2020 2020 2020 2020  ls>..           
-0002ed40: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-0002ed50: 5f55 5322 3e55 7365 7220 756e 6465 7220  _US">User under 
-0002ed60: 7465 6d70 6572 6174 7572 6520 6c65 7665  temperature leve
-0002ed70: 6c3c 2f4c 6162 656c 3e0d 0a20 2020 2020  l</Label>..     
-0002ed80: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-0002ed90: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-0002eda0: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-0002edb0: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-0002edc0: 7722 2061 6464 7265 7373 5f74 7970 653d  w" address_type=
-0002edd0: 224e 564d 5f4e 4f4e 4522 2061 6464 7265  "NVM_NONE" addre
-0002ede0: 7373 3d22 3078 3036 3431 2220 6474 7970  ss="0x0641" dtyp
-0002edf0: 653d 2275 3136 2220 6964 3d22 434f 4d4d  e="u16" id="COMM
-0002ee00: 535f 5359 4e43 5f53 4947 4e41 4c5f 4346  S_SYNC_SIGNAL_CF
-0002ee10: 4722 2075 6e69 7473 3d22 2d22 2073 7562  G" units="-" sub
-0002ee20: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
-0002ee30: 2243 4f4e 4649 4722 2064 6573 633d 2249  "CONFIG" desc="I
-0002ee40: 6e64 6963 6174 6573 2074 6865 206e 756d  ndicates the num
-0002ee50: 6265 7220 6f66 2073 796e 6368 726f 6e69  ber of synchroni
-0002ee60: 7a61 7469 6f6e 2073 6967 6e61 6c73 2067  zation signals g
-0002ee70: 656e 6572 6174 6564 2062 7920 7468 6520  enerated by the 
-0002ee80: 4d43 4220 7072 6f74 6f63 6f6c 2220 6361  MCB protocol" ca
-0002ee90: 745f 6964 3d22 434f 4d4d 554e 4943 4154  t_id="COMMUNICAT
-0002eea0: 494f 4e53 223e 0d0a 2020 2020 2020 2020  IONS">..        
-0002eeb0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-0002eec0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-0002eed0: 616e 673d 2265 6e5f 5553 223e 5379 6e63  ang="en_US">Sync
-0002eee0: 2e20 7369 676e 616c 2063 6f6e 6669 6775  . signal configu
-0002eef0: 7261 7469 6f6e 3c2f 4c61 6265 6c3e 0d0a  ration</Label>..
-0002ef00: 2020 2020 2020 2020 2020 3c2f 4c61 6265            </Labe
-0002ef10: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-0002ef20: 456e 756d 6572 6174 696f 6e73 3e0d 0a20  Enumerations>.. 
-0002ef30: 2020 2020 2020 2020 2020 203c 456e 756d             <Enum
-0002ef40: 2076 616c 7565 3d22 3022 3e44 6973 6162   value="0">Disab
-0002ef50: 6c65 643c 2f45 6e75 6d3e 0d0a 2020 2020  led</Enum>..    
-0002ef60: 2020 2020 2020 2020 3c45 6e75 6d20 7661          <Enum va
-0002ef70: 6c75 653d 2231 223e 4f6e 6c79 2053 796e  lue="1">Only Syn
-0002ef80: 6320 303c 2f45 6e75 6d3e 0d0a 2020 2020  c 0</Enum>..    
-0002ef90: 2020 2020 2020 3c2f 456e 756d 6572 6174        </Enumerat
-0002efa0: 696f 6e73 3e0d 0a20 2020 2020 2020 203c  ions>..        <
-0002efb0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-0002efc0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-0002efd0: 6365 7373 3d22 7277 2220 6164 6472 6573  cess="rw" addres
-0002efe0: 735f 7479 7065 3d22 4e56 4d5f 4346 4722  s_type="NVM_CFG"
-0002eff0: 2061 6464 7265 7373 3d22 3078 3036 3433   address="0x0643
-0002f000: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
-0002f010: 3d22 434f 4d4d 535f 5359 4e43 5f53 4947  ="COMMS_SYNC_SIG
-0002f020: 4e41 4c5f 4652 4551 2220 756e 6974 733d  NAL_FREQ" units=
-0002f030: 2248 7a22 2073 7562 6e6f 6465 3d22 3122  "Hz" subnode="1"
-0002f040: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
-0002f050: 2064 6573 633d 2246 7265 7175 656e 6379   desc="Frequency
-0002f060: 2061 7420 7768 6963 6820 7468 6520 7379   at which the sy
-0002f070: 6e63 6872 6f6e 697a 6174 696f 6e20 7369  nchronization si
-0002f080: 676e 616c 2069 7320 6265 696e 6720 6765  gnal is being ge
-0002f090: 6e65 7261 7465 642e 2049 7420 7368 6f75  nerated. It shou
-0002f0a0: 6c64 2062 6520 616e 2065 7861 6374 206d  ld be an exact m
-0002f0b0: 756c 7469 706c 6520 6f66 2074 6865 2050  ultiple of the P
-0002f0c0: 574d 2066 7265 7175 656e 6379 2073 656c  WM frequency sel
-0002f0d0: 6563 7465 642e 2220 6361 745f 6964 3d22  ected." cat_id="
-0002f0e0: 4f54 4845 5253 223e 0d0a 2020 2020 2020  OTHERS">..      
-0002f0f0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-0002f100: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-0002f110: 206c 616e 673d 2265 6e5f 5553 223e 5379   lang="en_US">Sy
-0002f120: 6e63 2e20 7369 676e 616c 2066 7265 7175  nc. signal frequ
-0002f130: 656e 6379 3c2f 4c61 6265 6c3e 0d0a 2020  ency</Label>..  
-0002f140: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-0002f150: 3e0d 0a20 2020 2020 2020 2020 203c 5261  >..          <Ra
-0002f160: 6e67 6520 6d69 6e3d 2231 3022 206d 6178  nge min="10" max
-0002f170: 3d22 3230 3030 3030 222f 3e0d 0a20 2020  ="200000"/>..   
-0002f180: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-0002f190: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-0002f1a0: 7465 7220 6163 6365 7373 3d22 7277 2220  ter access="rw" 
-0002f1b0: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
-0002f1c0: 4d5f 4346 4722 2061 6464 7265 7373 3d22  M_CFG" address="
-0002f1d0: 3078 3036 3434 2220 6474 7970 653d 2275  0x0644" dtype="u
-0002f1e0: 3332 2220 6964 3d22 434f 4d4d 535f 5359  32" id="COMMS_SY
-0002f1f0: 4e43 5f50 4c4c 5f43 5554 4f46 4622 2075  NC_PLL_CUTOFF" u
-0002f200: 6e69 7473 3d22 487a 2220 7375 626e 6f64  nits="Hz" subnod
-0002f210: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-0002f220: 4e46 4947 2220 6465 7363 3d22 4375 746f  NFIG" desc="Cuto
-0002f230: 6666 2066 7265 7175 656e 6379 206f 6620  ff frequency of 
-0002f240: 7468 6520 7379 6e63 6872 6f6e 697a 6174  the synchronizat
-0002f250: 696f 6e20 7369 676e 616c 2050 4c4c 2066  ion signal PLL f
-0002f260: 696c 7465 7222 2063 6174 5f69 643d 224f  ilter" cat_id="O
-0002f270: 5448 4552 5322 3e0d 0a20 2020 2020 2020  THERS">..       
-0002f280: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-0002f290: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-0002f2a0: 6c61 6e67 3d22 656e 5f55 5322 3e53 796e  lang="en_US">Syn
-0002f2b0: 632e 2073 6967 6e61 6c20 504c 4c20 6669  c. signal PLL fi
-0002f2c0: 6c74 6572 2063 7574 6f66 6620 6672 6571  lter cutoff freq
-0002f2d0: 7565 6e63 793c 2f4c 6162 656c 3e0d 0a20  uency</Label>.. 
-0002f2e0: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-0002f2f0: 733e 0d0a 2020 2020 2020 2020 2020 3c52  s>..          <R
-0002f300: 616e 6765 206d 696e 3d22 3130 2220 6d61  ange min="10" ma
-0002f310: 783d 2232 3030 3030 3022 2f3e 0d0a 2020  x="200000"/>..  
-0002f320: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
-0002f330: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
-0002f340: 7374 6572 2061 6363 6573 733d 2272 7722  ster access="rw"
-0002f350: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-0002f360: 564d 5f43 4647 2220 6164 6472 6573 733d  VM_CFG" address=
-0002f370: 2230 7830 3634 3522 2064 7479 7065 3d22  "0x0645" dtype="
-0002f380: 666c 6f61 7422 2069 643d 2243 4f4d 4d53  float" id="COMMS
-0002f390: 5f53 594e 435f 504c 4c5f 5048 4153 4522  _SYNC_PLL_PHASE"
-0002f3a0: 2075 6e69 7473 3d22 2d22 2073 7562 6e6f   units="-" subno
-0002f3b0: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-0002f3c0: 4f4e 4649 4722 2064 6573 633d 2243 6f6e  ONFIG" desc="Con
-0002f3d0: 6669 6775 7265 7320 7068 6173 6520 6469  figures phase di
-0002f3e0: 6666 6572 656e 6365 2062 6574 7765 656e  fference between
-0002f3f0: 2074 6865 2073 796e 6368 726f 6e69 7a61   the synchroniza
-0002f400: 7469 6f6e 2073 6967 6e61 6c20 616e 6420  tion signal and 
-0002f410: 7468 6520 6765 6e65 7261 7465 6420 5057  the generated PW
-0002f420: 4d2e 2220 6361 745f 6964 3d22 4f54 4845  M." cat_id="OTHE
-0002f430: 5253 223e 0d0a 2020 2020 2020 2020 2020  RS">..          
-0002f440: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-0002f450: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-0002f460: 673d 2265 6e5f 5553 223e 5379 6e63 2e20  g="en_US">Sync. 
-0002f470: 7369 676e 616c 2050 4c4c 2070 6861 7365  signal PLL phase
-0002f480: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-0002f490: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-0002f4a0: 2020 2020 2020 2020 203c 5261 6e67 6520           <Range 
-0002f4b0: 6d69 6e3d 2230 2e30 2220 6d61 783d 2231  min="0.0" max="1
-0002f4c0: 2e30 222f 3e0d 0a20 2020 2020 2020 203c  .0"/>..        <
-0002f4d0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-0002f4e0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-0002f4f0: 6365 7373 3d22 7277 2220 6164 6472 6573  cess="rw" addres
-0002f500: 735f 7479 7065 3d22 4e56 4d5f 4346 4722  s_type="NVM_CFG"
-0002f510: 2061 6464 7265 7373 3d22 3078 3036 3436   address="0x0646
-0002f520: 2220 6474 7970 653d 2266 6c6f 6174 2220  " dtype="float" 
-0002f530: 6964 3d22 434f 4d4d 535f 5359 4e43 5f50  id="COMMS_SYNC_P
-0002f540: 4c4c 5f4b 5022 2075 6e69 7473 3d22 2d22  LL_KP" units="-"
-0002f550: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
-0002f560: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
-0002f570: 633d 2243 6f6e 6669 6775 7265 7320 7072  c="Configures pr
-0002f580: 6f70 6f72 7469 6f6e 616c 2063 6f6e 7374  oportional const
-0002f590: 616e 7420 666f 7220 7068 6173 6520 636f  ant for phase co
-0002f5a0: 7272 6563 7469 6f6e 2069 6e20 506c 6c22  rrection in Pll"
-0002f5b0: 2063 6174 5f69 643d 224f 5448 4552 5322   cat_id="OTHERS"
-0002f5c0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-0002f5d0: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-0002f5e0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-0002f5f0: 656e 5f55 5322 3e53 796e 632e 2073 6967  en_US">Sync. sig
-0002f600: 6e61 6c20 504c 4c20 4b70 3c2f 4c61 6265  nal PLL Kp</Labe
-0002f610: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
-0002f620: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-0002f630: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
-0002f640: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
-0002f650: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
-0002f660: 7373 5f74 7970 653d 224e 564d 5f4e 4f4e  ss_type="NVM_NON
-0002f670: 4522 2061 6464 7265 7373 3d22 3078 3036  E" address="0x06
-0002f680: 3444 2220 6474 7970 653d 2275 3136 2220  4D" dtype="u16" 
-0002f690: 6964 3d22 4452 565f 4449 4147 5f45 5252  id="DRV_DIAG_ERR
-0002f6a0: 4f52 5f54 4f54 414c 2220 756e 6974 733d  OR_TOTAL" units=
-0002f6b0: 222d 2220 7375 626e 6f64 653d 2231 2220  "-" subnode="1" 
-0002f6c0: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
-0002f6d0: 6465 7363 3d22 546f 7461 6c20 6e75 6d62  desc="Total numb
-0002f6e0: 6572 206f 6620 6572 726f 7273 2073 696e  er of errors sin
-0002f6f0: 6365 2070 6f77 6572 2075 7022 2063 6174  ce power up" cat
-0002f700: 5f69 643d 2252 4550 4f52 5449 4e47 223e  _id="REPORTING">
-0002f710: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-0002f720: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-0002f730: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-0002f740: 6e5f 5553 223e 4572 726f 7220 746f 7461  n_US">Error tota
-0002f750: 6c20 6e75 6d62 6572 3c2f 4c61 6265 6c3e  l number</Label>
-0002f760: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-0002f770: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-0002f780: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-0002f790: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-0002f7a0: 6365 7373 3d22 7277 2220 6164 6472 6573  cess="rw" addres
-0002f7b0: 735f 7479 7065 3d22 4e56 4d5f 4e4f 4e45  s_type="NVM_NONE
-0002f7c0: 2220 6164 6472 6573 733d 2230 7830 3634  " address="0x064
-0002f7d0: 4522 2064 7479 7065 3d22 7531 3622 2069  E" dtype="u16" i
-0002f7e0: 643d 2244 5256 5f44 4941 475f 4552 524f  d="DRV_DIAG_ERRO
-0002f7f0: 525f 4c49 5354 5f49 4458 2220 756e 6974  R_LIST_IDX" unit
-0002f800: 733d 222d 2220 7375 626e 6f64 653d 2231  s="-" subnode="1
-0002f810: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-0002f820: 2220 6465 7363 3d22 496e 6465 7820 746f  " desc="Index to
-0002f830: 2061 6363 6573 7320 746f 2074 6865 206c   access to the l
-0002f840: 6173 7420 6572 726f 7273 2220 6361 745f  ast errors" cat_
-0002f850: 6964 3d22 5245 504f 5254 494e 4722 3e0d  id="REPORTING">.
-0002f860: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-0002f870: 6c73 3e0d 0a20 2020 2020 2020 2020 2020  ls>..           
-0002f880: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-0002f890: 5f55 5322 3e45 7272 6f72 206c 6973 7420  _US">Error list 
-0002f8a0: 696e 6465 7820 7265 7175 6573 743c 2f4c  index request</L
-0002f8b0: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
-0002f8c0: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-0002f8d0: 2020 2020 2020 3c52 616e 6765 206d 696e        <Range min
-0002f8e0: 3d22 3022 206d 6178 3d22 3332 222f 3e0d  ="0" max="32"/>.
-0002f8f0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-0002f900: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-0002f910: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-0002f920: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-0002f930: 224e 564d 5f4e 4f4e 4522 2061 6464 7265  "NVM_NONE" addre
-0002f940: 7373 3d22 3078 3036 3446 2220 6474 7970  ss="0x064F" dtyp
-0002f950: 653d 2273 3332 2220 6964 3d22 4452 565f  e="s32" id="DRV_
-0002f960: 4449 4147 5f45 5252 4f52 5f4c 4953 545f  DIAG_ERROR_LIST_
-0002f970: 434f 4445 2220 756e 6974 733d 222d 2220  CODE" units="-" 
-0002f980: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-0002f990: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-0002f9a0: 3d22 436f 6e74 6169 6e73 2074 6865 2065  ="Contains the e
-0002f9b0: 7272 6f72 2063 6f64 6520 6f66 2074 6865  rror code of the
-0002f9c0: 2069 6e64 6963 6174 6564 2062 7920 7468   indicated by th
-0002f9d0: 6520 7265 7175 6573 7465 6420 6c6f 6361  e requested loca
-0002f9e0: 7469 6f6e 2072 6567 6973 7465 7222 2063  tion register" c
-0002f9f0: 6174 5f69 643d 2252 4550 4f52 5449 4e47  at_id="REPORTING
-0002fa00: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
-0002fa10: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-0002fa20: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-0002fa30: 2265 6e5f 5553 223e 4572 726f 7220 6c69  "en_US">Error li
-0002fa40: 7374 2072 6571 7565 7374 6564 2063 6f64  st requested cod
-0002fa50: 653c 2f4c 6162 656c 3e0d 0a20 2020 2020  e</Label>..     
-0002fa60: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-0002fa70: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-0002fa80: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-0002fa90: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-0002faa0: 7722 2061 6464 7265 7373 5f74 7970 653d  w" address_type=
-0002fab0: 224e 564d 5f4e 4f4e 4522 2061 6464 7265  "NVM_NONE" addre
-0002fac0: 7373 3d22 3078 3036 4442 2220 6474 7970  ss="0x06DB" dtyp
-0002fad0: 653d 2275 3332 2220 6964 3d22 4452 565f  e="u32" id="DRV_
-0002fae0: 5354 4f52 455f 4d4f 434f 5f41 4c4c 2220  STORE_MOCO_ALL" 
-0002faf0: 756e 6974 733d 222d 2220 7375 626e 6f64  units="-" subnod
-0002fb00: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-0002fb10: 4e46 4947 2220 6465 7363 3d22 2220 6361  NFIG" desc="" ca
-0002fb20: 745f 6964 3d22 4944 454e 5449 4649 4341  t_id="IDENTIFICA
-0002fb30: 5449 4f4e 223e 0d0a 2020 2020 2020 2020  TION">..        
-0002fb40: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-0002fb50: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-0002fb60: 616e 673d 2265 6e5f 5553 223e 5374 6f72  ang="en_US">Stor
-0002fb70: 6520 616c 6c3c 2f4c 6162 656c 3e0d 0a20  e all</Label>.. 
-0002fb80: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-0002fb90: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-0002fba0: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-0002fbb0: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-0002fbc0: 733d 2272 7722 2061 6464 7265 7373 5f74  s="rw" address_t
-0002fbd0: 7970 653d 224e 564d 5f4e 4f4e 4522 2061  ype="NVM_NONE" a
-0002fbe0: 6464 7265 7373 3d22 3078 3036 4443 2220  ddress="0x06DC" 
-0002fbf0: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
-0002fc00: 4452 565f 5245 5354 4f52 455f 4d4f 434f  DRV_RESTORE_MOCO
-0002fc10: 5f41 4c4c 2220 756e 6974 733d 222d 2220  _ALL" units="-" 
-0002fc20: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-0002fc30: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-0002fc40: 3d22 5573 696e 6720 7468 6520 7072 6f70  ="Using the prop
-0002fc50: 6572 2070 6173 7377 6f72 6420 616c 6c6f  er password allo
-0002fc60: 7773 2074 6f20 7265 7374 6f72 6520 7468  ws to restore th
-0002fc70: 6520 6465 6661 756c 7420 7061 7261 6d65  e default parame
-0002fc80: 7465 7273 206f 6620 7468 6520 6472 6976  ters of the driv
-0002fc90: 6520 6166 7465 7220 7468 6520 6e65 7874  e after the next
-0002fca0: 2070 6f77 6572 206f 6e22 2063 6174 5f69   power on" cat_i
-0002fcb0: 643d 2249 4445 4e54 4946 4943 4154 494f  d="IDENTIFICATIO
-0002fcc0: 4e22 3e0d 0a20 2020 2020 2020 2020 203c  N">..          <
-0002fcd0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-0002fce0: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-0002fcf0: 3d22 656e 5f55 5322 3e52 6573 746f 7265  ="en_US">Restore
-0002fd00: 2061 6c6c 3c2f 4c61 6265 6c3e 0d0a 2020   all</Label>..  
-0002fd10: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-0002fd20: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
-0002fd30: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
-0002fd40: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
-0002fd50: 3d22 7722 2061 6464 7265 7373 5f74 7970  ="w" address_typ
-0002fd60: 653d 224e 564d 5f4e 4f4e 4522 2061 6464  e="NVM_NONE" add
-0002fd70: 7265 7373 3d22 3078 3036 4446 2220 6474  ress="0x06DF" dt
-0002fd80: 7970 653d 2275 3332 2220 6964 3d22 4452  ype="u32" id="DR
-0002fd90: 565f 424f 4f54 5f52 4553 4554 2220 756e  V_BOOT_RESET" un
-0002fda0: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
-0002fdb0: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
-0002fdc0: 4947 2220 6465 7363 3d22 5769 7468 2074  IG" desc="With t
-0002fdd0: 6865 2070 726f 7065 7220 7061 7373 776f  he proper passwo
-0002fde0: 7264 2072 6573 6574 7320 7468 6520 6472  rd resets the dr
-0002fdf0: 6976 652e 2220 6361 745f 6964 3d22 494e  ive." cat_id="IN
-0002fe00: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-0002fe10: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-0002fe20: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-0002fe30: 206c 616e 673d 2265 6e5f 5553 223e 5379   lang="en_US">Sy
-0002fe40: 7374 656d 2072 6573 6574 3c2f 4c61 6265  stem reset</Labe
-0002fe50: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
-0002fe60: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-0002fe70: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
-0002fe80: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
-0002fe90: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
-0002fea0: 7373 5f74 7970 653d 224e 564d 5f4e 4f4e  ss_type="NVM_NON
-0002feb0: 4522 2061 6464 7265 7373 3d22 3078 3036  E" address="0x06
-0002fec0: 4530 2220 6474 7970 653d 2275 3332 2220  E0" dtype="u32" 
-0002fed0: 6964 3d22 4452 565f 4944 5f56 454e 444f  id="DRV_ID_VENDO
-0002fee0: 525f 4944 2220 756e 6974 733d 222d 2220  R_ID" units="-" 
-0002fef0: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-0002ff00: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-0002ff10: 3d22 4964 656e 7469 6669 6573 2074 6865  ="Identifies the
-0002ff20: 2076 656e 646f 7220 6f66 2074 6865 2070   vendor of the p
-0002ff30: 726f 6475 6374 2220 6361 745f 6964 3d22  roduct" cat_id="
-0002ff40: 4944 454e 5449 4649 4341 5449 4f4e 223e  IDENTIFICATION">
-0002ff50: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-0002ff60: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-0002ff70: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-0002ff80: 6e5f 5553 223e 5665 6e64 6f72 2049 443c  n_US">Vendor ID<
-0002ff90: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-0002ffa0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
-0002ffb0: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
-0002ffc0: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
-0002ffd0: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
-0002ffe0: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
-0002fff0: 4d5f 4e4f 4e45 2220 6164 6472 6573 733d  M_NONE" address=
-00030000: 2230 7830 3645 3122 2064 7479 7065 3d22  "0x06E1" dtype="
-00030010: 7533 3222 2069 643d 2244 5256 5f49 445f  u32" id="DRV_ID_
-00030020: 5052 4f44 5543 545f 434f 4445 2220 756e  PRODUCT_CODE" un
-00030030: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
-00030040: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
-00030050: 4947 2220 6465 7363 3d22 436f 6e74 6169  IG" desc="Contai
-00030060: 6e73 2074 6865 2070 726f 6475 6374 2063  ns the product c
-00030070: 6f64 6520 6f66 2074 6865 2064 7269 7665  ode of the drive
-00030080: 2220 6361 745f 6964 3d22 4944 454e 5449  " cat_id="IDENTI
-00030090: 4649 4341 5449 4f4e 223e 0d0a 2020 2020  FICATION">..    
-000300a0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-000300b0: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
-000300c0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-000300d0: 5072 6f64 7563 7420 636f 6465 3c2f 4c61  Product code</La
-000300e0: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
-000300f0: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
-00030100: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
-00030110: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
-00030120: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
-00030130: 7265 7373 5f74 7970 653d 224e 564d 5f4e  ress_type="NVM_N
-00030140: 4f4e 4522 2061 6464 7265 7373 3d22 3078  ONE" address="0x
-00030150: 3036 4532 2220 6474 7970 653d 2275 3332  06E2" dtype="u32
-00030160: 2220 6964 3d22 4452 565f 4944 5f52 4556  " id="DRV_ID_REV
-00030170: 4953 494f 4e5f 4e55 4d42 4552 2220 756e  ISION_NUMBER" un
-00030180: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
-00030190: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
-000301a0: 4947 2220 6465 7363 3d22 496e 6469 6361  IG" desc="Indica
-000301b0: 7465 7320 7468 6520 7265 7669 7369 6f6e  tes the revision
-000301c0: 206e 756d 6265 7220 6f66 2074 6865 2066   number of the f
-000301d0: 6972 6d77 6172 6520 7665 7273 696f 6e20  irmware version 
-000301e0: 6f6e 2074 6865 2064 7269 7665 2220 6361  on the drive" ca
-000301f0: 745f 6964 3d22 4944 454e 5449 4649 4341  t_id="IDENTIFICA
-00030200: 5449 4f4e 223e 0d0a 2020 2020 2020 2020  TION">..        
-00030210: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00030220: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00030230: 616e 673d 2265 6e5f 5553 223e 5265 7669  ang="en_US">Revi
-00030240: 7369 6f6e 206e 756d 6265 723c 2f4c 6162  sion number</Lab
-00030250: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00030260: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00030270: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00030280: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00030290: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-000302a0: 6573 735f 7479 7065 3d22 4e56 4d5f 4e4f  ess_type="NVM_NO
-000302b0: 4e45 2220 6164 6472 6573 733d 2230 7830  NE" address="0x0
-000302c0: 3645 3422 2064 7479 7065 3d22 7374 7222  6E4" dtype="str"
-000302d0: 2069 643d 2244 5256 5f49 445f 534f 4654   id="DRV_ID_SOFT
-000302e0: 5741 5245 5f56 4552 5349 4f4e 2220 756e  WARE_VERSION" un
-000302f0: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
-00030300: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
-00030310: 4947 2220 6465 7363 3d22 5075 626c 6963  IG" desc="Public
-00030320: 2073 6f66 7477 6172 6520 7265 6c65 6173   software releas
-00030330: 6520 7665 7273 696f 6e22 2063 6174 5f69  e version" cat_i
-00030340: 643d 2249 4445 4e54 4946 4943 4154 494f  d="IDENTIFICATIO
-00030350: 4e22 3e0d 0a20 2020 2020 2020 2020 203c  N">..          <
-00030360: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00030370: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-00030380: 3d22 656e 5f55 5322 3e53 6f66 7477 6172  ="en_US">Softwar
-00030390: 6520 7665 7273 696f 6e3c 2f4c 6162 656c  e version</Label
-000303a0: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-000303b0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-000303c0: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-000303d0: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-000303e0: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-000303f0: 735f 7479 7065 3d22 4e56 4d5f 4c4f 434b  s_type="NVM_LOCK
-00030400: 2220 6164 6472 6573 733d 2230 7830 3645  " address="0x06E
-00030410: 3622 2064 7479 7065 3d22 7533 3222 2069  6" dtype="u32" i
-00030420: 643d 2244 5256 5f49 445f 5345 5249 414c  d="DRV_ID_SERIAL
-00030430: 5f4e 554d 4245 5222 2075 6e69 7473 3d22  _NUMBER" units="
-00030440: 2d22 2073 7562 6e6f 6465 3d22 3122 2063  -" subnode="1" c
-00030450: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
-00030460: 6573 633d 2255 6e69 7175 6520 7365 7269  esc="Unique seri
-00030470: 616c 206e 756d 6265 7220 6964 206f 6620  al number id of 
-00030480: 7468 6520 6465 7669 6365 2220 6361 745f  the device" cat_
-00030490: 6964 3d22 4944 454e 5449 4649 4341 5449  id="IDENTIFICATI
-000304a0: 4f4e 223e 0d0a 2020 2020 2020 2020 2020  ON">..          
-000304b0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-000304c0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-000304d0: 673d 2265 6e5f 5553 223e 5365 7269 616c  g="en_US">Serial
-000304e0: 206e 756d 6265 723c 2f4c 6162 656c 3e0d   number</Label>.
-000304f0: 0a20 2020 2020 2020 2020 203c 2f4c 6162  .          </Lab
-00030500: 656c 733e 0d0a 2020 2020 2020 2020 3c2f  els>..        </
-00030510: 5265 6769 7374 6572 3e0d 0a20 2020 2020  Register>..     
-00030520: 2020 203c 5265 6769 7374 6572 2061 6363     <Register acc
-00030530: 6573 733d 2272 2220 6164 6472 6573 735f  ess="r" address_
-00030540: 7479 7065 3d22 4e56 4d5f 4857 2220 6164  type="NVM_HW" ad
-00030550: 6472 6573 733d 2230 7830 3730 3022 2064  dress="0x0700" d
-00030560: 7479 7065 3d22 7533 3222 2069 643d 2244  type="u32" id="D
-00030570: 5256 5f50 535f 4652 4551 5f31 2220 756e  RV_PS_FREQ_1" un
-00030580: 6974 733d 2248 7a22 2073 7562 6e6f 6465  its="Hz" subnode
-00030590: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-000305a0: 4649 4722 2064 6573 633d 2243 6f6e 7461  FIG" desc="Conta
-000305b0: 696e 7320 7468 6520 7365 6c65 6374 6162  ins the selectab
-000305c0: 6c65 2063 6f6d 6d75 7461 7469 6f6e 2066  le commutation f
-000305d0: 7265 7175 656e 6379 2031 2028 416c 736f  requency 1 (Also
-000305e0: 206d 696e 696d 756d 2050 574d 2066 7265   minimum PWM fre
-000305f0: 7175 656e 6379 2922 2063 6174 5f69 643d  quency)" cat_id=
-00030600: 2249 4e54 4552 4e41 4c22 3e0d 0a20 2020  "INTERNAL">..   
-00030610: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00030620: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
-00030630: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00030640: 3e50 6f77 6572 2073 7461 6765 2066 7265  >Power stage fre
-00030650: 7175 656e 6379 2031 3c2f 4c61 6265 6c3e  quency 1</Label>
-00030660: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-00030670: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-00030680: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-00030690: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-000306a0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
-000306b0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
-000306c0: 6464 7265 7373 3d22 3078 3037 3031 2220  ddress="0x0701" 
-000306d0: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
-000306e0: 4452 565f 5053 5f46 5245 515f 3222 2075  DRV_PS_FREQ_2" u
-000306f0: 6e69 7473 3d22 487a 2220 7375 626e 6f64  nits="Hz" subnod
-00030700: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-00030710: 4e46 4947 2220 6465 7363 3d22 436f 6e74  NFIG" desc="Cont
-00030720: 6169 6e73 2074 6865 2073 656c 6563 7461  ains the selecta
-00030730: 626c 6520 636f 6d6d 7574 6174 696f 6e20  ble commutation 
-00030740: 6672 6571 7565 6e63 7920 3222 2063 6174  frequency 2" cat
-00030750: 5f69 643d 2249 4e54 4552 4e41 4c22 3e0d  _id="INTERNAL">.
-00030760: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-00030770: 6c73 3e0d 0a20 2020 2020 2020 2020 2020  ls>..           
-00030780: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-00030790: 5f55 5322 3e50 6f77 6572 2073 7461 6765  _US">Power stage
-000307a0: 2066 7265 7175 656e 6379 2032 3c2f 4c61   frequency 2</La
-000307b0: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
-000307c0: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
-000307d0: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
-000307e0: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
-000307f0: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
-00030800: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
-00030810: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
-00030820: 3032 2220 6474 7970 653d 2275 3332 2220  02" dtype="u32" 
-00030830: 6964 3d22 4452 565f 5053 5f46 5245 515f  id="DRV_PS_FREQ_
-00030840: 3322 2075 6e69 7473 3d22 487a 2220 7375  3" units="Hz" su
-00030850: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-00030860: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-00030870: 436f 6e74 6169 6e73 2074 6865 2073 656c  Contains the sel
-00030880: 6563 7461 626c 6520 636f 6d6d 7574 6174  ectable commutat
-00030890: 696f 6e20 6672 6571 7565 6e63 7920 3322  ion frequency 3"
-000308a0: 2063 6174 5f69 643d 2249 4e54 4552 4e41   cat_id="INTERNA
-000308b0: 4c22 3e0d 0a20 2020 2020 2020 2020 203c  L">..          <
-000308c0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-000308d0: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-000308e0: 3d22 656e 5f55 5322 3e50 6f77 6572 2073  ="en_US">Power s
-000308f0: 7461 6765 2066 7265 7175 656e 6379 2033  tage frequency 3
-00030900: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00030910: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00030920: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-00030930: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
-00030940: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
-00030950: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-00030960: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
-00030970: 3078 3037 3033 2220 6474 7970 653d 2275  0x0703" dtype="u
-00030980: 3332 2220 6964 3d22 4452 565f 5053 5f46  32" id="DRV_PS_F
-00030990: 5245 515f 3422 2075 6e69 7473 3d22 487a  REQ_4" units="Hz
-000309a0: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
-000309b0: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
-000309c0: 7363 3d22 436f 6e74 6169 6e73 2074 6865  sc="Contains the
-000309d0: 2073 656c 6563 7461 626c 6520 636f 6d6d   selectable comm
-000309e0: 7574 6174 696f 6e20 6672 6571 7565 6e63  utation frequenc
-000309f0: 7920 3420 2841 6c73 6f20 6d61 7869 6d75  y 4 (Also maximu
-00030a00: 6d20 5057 4d20 6672 6571 7565 6e63 7929  m PWM frequency)
-00030a10: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-00030a20: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00030a30: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00030a40: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00030a50: 673d 2265 6e5f 5553 223e 506f 7765 7220  g="en_US">Power 
-00030a60: 7374 6167 6520 6672 6571 7565 6e63 7920  stage frequency 
-00030a70: 343c 2f4c 6162 656c 3e0d 0a20 2020 2020  4</Label>..     
-00030a80: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00030a90: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-00030aa0: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-00030ab0: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-00030ac0: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
-00030ad0: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
-00030ae0: 2230 7830 3730 3422 2064 7479 7065 3d22  "0x0704" dtype="
-00030af0: 7533 3222 2069 643d 2244 5256 5f50 535f  u32" id="DRV_PS_
-00030b00: 4445 4144 5f54 494d 4522 2075 6e69 7473  DEAD_TIME" units
-00030b10: 3d22 6e73 2220 7375 626e 6f64 653d 2231  ="ns" subnode="1
-00030b20: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-00030b30: 2220 6465 7363 3d22 4465 6164 2d74 696d  " desc="Dead-tim
-00030b40: 6520 6170 706c 6965 6420 746f 2050 574d  e applied to PWM
-00030b50: 2067 656e 6572 6174 696f 6e20 746f 2061   generation to a
-00030b60: 766f 6964 2073 686f 6f74 2d74 6872 6f75  void shoot-throu
-00030b70: 6768 2069 6e20 7468 6520 706f 7765 7220  gh in the power 
-00030b80: 7374 6167 6522 2063 6174 5f69 643d 2249  stage" cat_id="I
-00030b90: 4e54 4552 4e41 4c22 3e0d 0a20 2020 2020  NTERNAL">..     
-00030ba0: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00030bb0: 2020 2020 2020 2020 2020 203c 4c61 6265             <Labe
-00030bc0: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e50  l lang="en_US">P
-00030bd0: 6f77 6572 2073 7461 6765 2064 6561 642d  ower stage dead-
-00030be0: 7469 6d65 2028 6e73 293c 2f4c 6162 656c  time (ns)</Label
-00030bf0: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-00030c00: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00030c10: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-00030c20: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-00030c30: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-00030c40: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
-00030c50: 6164 6472 6573 733d 2230 7830 3730 3622  address="0x0706"
-00030c60: 2064 7479 7065 3d22 7533 3222 2069 643d   dtype="u32" id=
-00030c70: 2244 5256 5f50 535f 4d49 4e5f 4c4f 575f  "DRV_PS_MIN_LOW_
-00030c80: 5349 4445 5f4f 4e5f 5449 4d45 2220 756e  SIDE_ON_TIME" un
-00030c90: 6974 733d 226e 7322 2073 7562 6e6f 6465  its="ns" subnode
-00030ca0: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-00030cb0: 4649 4722 2064 6573 633d 224d 696e 696d  FIG" desc="Minim
-00030cc0: 756d 2074 696d 6520 7468 6520 706f 7765  um time the powe
-00030cd0: 7220 7374 6167 6520 6c6f 7720 7369 6465  r stage low side
-00030ce0: 2073 686f 756c 6420 6265 2065 6e61 626c   should be enabl
-00030cf0: 6564 2066 6f72 2061 2070 726f 7065 7220  ed for a proper 
-00030d00: 6375 7272 656e 7420 6d65 6173 7572 656d  current measurem
-00030d10: 656e 742e 2220 6361 745f 6964 3d22 494e  ent." cat_id="IN
-00030d20: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00030d30: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00030d40: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00030d50: 206c 616e 673d 2265 6e5f 5553 223e 4d69   lang="en_US">Mi
-00030d60: 6e2e 206c 6f77 2073 6964 6520 6f6e 2074  n. low side on t
-00030d70: 696d 6520 286e 7329 3c2f 4c61 6265 6c3e  ime (ns)</Label>
-00030d80: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-00030d90: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-00030da0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-00030db0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-00030dc0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
-00030dd0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
-00030de0: 6464 7265 7373 3d22 3078 3037 3037 2220  ddress="0x0707" 
-00030df0: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
-00030e00: 4452 565f 5053 5f4d 494e 5f48 4947 485f  DRV_PS_MIN_HIGH_
-00030e10: 5349 4445 5f4f 4e5f 5449 4d45 2220 756e  SIDE_ON_TIME" un
-00030e20: 6974 733d 226e 7322 2073 7562 6e6f 6465  its="ns" subnode
-00030e30: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-00030e40: 4649 4722 2064 6573 633d 2222 2063 6174  FIG" desc="" cat
-00030e50: 5f69 643d 224f 5448 4552 5322 3e0d 0a20  _id="OTHERS">.. 
-00030e60: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
-00030e70: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00030e80: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00030e90: 5322 3e4d 696e 2e20 6869 6768 2073 6964  S">Min. high sid
-00030ea0: 6520 6f6e 2074 696d 6520 286e 7329 3c2f  e on time (ns)</
-00030eb0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-00030ec0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00030ed0: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-00030ee0: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-00030ef0: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
-00030f00: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
-00030f10: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
-00030f20: 3037 3039 2220 6474 7970 653d 2275 3136  0709" dtype="u16
-00030f30: 2220 6964 3d22 4452 565f 5052 4f54 5f43  " id="DRV_PROT_C
-00030f40: 5552 525f 4f56 4552 5f52 414e 4745 5f54  URR_OVER_RANGE_T
-00030f50: 4852 4553 484f 4c44 2220 756e 6974 733d  HRESHOLD" units=
-00030f60: 2263 6e74 2220 7375 626e 6f64 653d 2231  "cnt" subnode="1
-00030f70: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-00030f80: 2220 6465 7363 3d22 4e75 6d62 6572 206f  " desc="Number o
-00030f90: 6620 636f 756e 7473 2062 656c 6f77 2041  f counts below A
-00030fa0: 4443 2063 6569 6c69 6e67 2077 6865 7265  DC ceiling where
-00030fb0: 2074 6865 2075 7070 6572 2073 6174 7572   the upper satur
-00030fc0: 6174 696f 6e20 6c69 6d69 7420 7769 6c6c  ation limit will
-00030fd0: 2062 6520 706c 6163 6564 2e20 5573 6564   be placed. Used
-00030fe0: 2066 6f72 2041 4443 2073 6174 7572 6174   for ADC saturat
-00030ff0: 696f 6e20 6572 726f 7220 6465 7465 6374  ion error detect
-00031000: 696f 6e22 2063 6174 5f69 643d 2250 524f  ion" cat_id="PRO
-00031010: 5445 4354 494f 4e53 223e 0d0a 2020 2020  TECTIONS">..    
-00031020: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-00031030: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
-00031040: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-00031050: 4375 7272 656e 7420 7361 7475 7261 7469  Current saturati
-00031060: 6f6e 2063 6f75 6e74 7320 6672 6f6d 2041  on counts from A
-00031070: 4443 2063 6569 6c69 6e67 3c2f 4c61 6265  DC ceiling</Labe
-00031080: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
-00031090: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-000310a0: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
-000310b0: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
-000310c0: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
-000310d0: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
-000310e0: 2061 6464 7265 7373 3d22 3078 3037 3041   address="0x070A
-000310f0: 2220 6474 7970 653d 2275 3136 2220 6964  " dtype="u16" id
-00031100: 3d22 4452 565f 5052 4f54 5f43 5552 525f  ="DRV_PROT_CURR_
-00031110: 554e 4445 525f 5241 4e47 455f 5448 5245  UNDER_RANGE_THRE
-00031120: 5348 4f4c 4422 2075 6e69 7473 3d22 636e  SHOLD" units="cn
-00031130: 7422 2073 7562 6e6f 6465 3d22 3122 2063  t" subnode="1" c
-00031140: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
-00031150: 6573 633d 224e 756d 6265 7220 6f66 2063  esc="Number of c
-00031160: 6f75 6e74 7320 6162 6f76 6520 4144 4320  ounts above ADC 
-00031170: 666c 6f6f 7220 7768 6572 6520 7468 6520  floor where the 
-00031180: 6c6f 7765 7220 7361 7475 7261 7469 6f6e  lower saturation
-00031190: 206c 696d 6974 2077 696c 6c20 6265 2070   limit will be p
-000311a0: 6c61 6365 642e 2055 7365 6420 666f 7220  laced. Used for 
-000311b0: 4144 4320 7361 7475 7261 7469 6f6e 2065  ADC saturation e
-000311c0: 7272 6f72 2064 6574 6563 7469 6f6e 2220  rror detection" 
-000311d0: 6361 745f 6964 3d22 5052 4f54 4543 5449  cat_id="PROTECTI
-000311e0: 4f4e 5322 3e0d 0a20 2020 2020 2020 2020  ONS">..         
-000311f0: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
-00031200: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
-00031210: 6e67 3d22 656e 5f55 5322 3e43 7572 7265  ng="en_US">Curre
-00031220: 6e74 2073 6174 7572 6174 696f 6e20 636f  nt saturation co
-00031230: 756e 7473 2066 726f 6d20 4144 4320 666c  unts from ADC fl
-00031240: 6f6f 723c 2f4c 6162 656c 3e0d 0a20 2020  oor</Label>..   
-00031250: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00031260: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
-00031270: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
-00031280: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
-00031290: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
-000312a0: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
-000312b0: 733d 2230 7830 3731 3022 2064 7479 7065  s="0x0710" dtype
-000312c0: 3d22 666c 6f61 7422 2069 643d 2244 5256  ="float" id="DRV
-000312d0: 5f50 524f 545f 4d41 4e5f 4f56 4552 5f54  _PROT_MAN_OVER_T
-000312e0: 454d 5022 2075 6e69 7473 3d22 c2ba 4322  EMP" units="..C"
-000312f0: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
-00031300: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
-00031310: 633d 2249 6e64 6963 6174 6573 2074 6865  c="Indicates the
-00031320: 206d 6178 696d 756d 2073 7570 706f 7274   maximum support
-00031330: 6564 2074 656d 7065 7261 7475 7265 206f  ed temperature o
-00031340: 6620 7468 6520 6472 6976 6522 2063 6174  f the drive" cat
-00031350: 5f69 643d 2250 524f 5445 4354 494f 4e53  _id="PROTECTIONS
-00031360: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
-00031370: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00031380: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-00031390: 2265 6e5f 5553 223e 4f76 6572 2d74 656d  "en_US">Over-tem
-000313a0: 7065 7261 7475 7265 206c 6576 656c 3c2f  perature level</
-000313b0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-000313c0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-000313d0: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-000313e0: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-000313f0: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
-00031400: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
-00031410: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
-00031420: 3037 3131 2220 6474 7970 653d 2266 6c6f  0711" dtype="flo
-00031430: 6174 2220 6964 3d22 4452 565f 5052 4f54  at" id="DRV_PROT
-00031440: 5f4d 414e 5f55 4e44 4552 5f54 454d 5022  _MAN_UNDER_TEMP"
-00031450: 2075 6e69 7473 3d22 c2ba 4322 2073 7562   units="..C" sub
-00031460: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
-00031470: 2243 4f4e 4649 4722 2064 6573 633d 2249  "CONFIG" desc="I
-00031480: 6e64 6963 6174 6573 2074 6865 206d 696e  ndicates the min
-00031490: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
-000314a0: 2061 6c6c 6f77 6564 2066 6f72 2064 7269   allowed for dri
-000314b0: 7665 206f 7065 7261 7469 6f6e 2069 6e20  ve operation in 
-000314c0: 6465 6772 6565 7320 6365 6c73 6975 7322  degrees celsius"
-000314d0: 2063 6174 5f69 643d 2250 524f 5445 4354   cat_id="PROTECT
-000314e0: 494f 4e53 223e 0d0a 2020 2020 2020 2020  IONS">..        
-000314f0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00031500: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00031510: 616e 673d 2265 6e5f 5553 223e 556e 6465  ang="en_US">Unde
-00031520: 722d 7465 6d70 6572 6174 7572 6520 6c65  r-temperature le
-00031530: 7665 6c3c 2f4c 6162 656c 3e0d 0a20 2020  vel</Label>..   
-00031540: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00031550: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
-00031560: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
-00031570: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
-00031580: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
-00031590: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
-000315a0: 733d 2230 7830 3731 3222 2064 7479 7065  s="0x0712" dtype
-000315b0: 3d22 666c 6f61 7422 2069 643d 2244 5256  ="float" id="DRV
-000315c0: 5f50 524f 545f 4d41 4e5f 4f56 4552 5f56  _PROT_MAN_OVER_V
-000315d0: 4f4c 5422 2075 6e69 7473 3d22 5622 2073  OLT" units="V" s
-000315e0: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-000315f0: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-00031600: 2249 6e64 6963 6174 6573 2074 6865 206d  "Indicates the m
-00031610: 6178 696d 756d 2073 7570 706f 7274 6564  aximum supported
-00031620: 2062 7573 2076 6f6c 7461 6765 2062 7920   bus voltage by 
-00031630: 7468 6520 6472 6976 6522 2063 6174 5f69  the drive" cat_i
-00031640: 643d 2250 524f 5445 4354 494f 4e53 223e  d="PROTECTIONS">
-00031650: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00031660: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00031670: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00031680: 6e5f 5553 223e 4f76 6572 2d76 6f6c 7461  n_US">Over-volta
-00031690: 6765 206c 6576 656c 3c2f 4c61 6265 6c3e  ge level</Label>
-000316a0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-000316b0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-000316c0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-000316d0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-000316e0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
-000316f0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
-00031700: 6464 7265 7373 3d22 3078 3037 3133 2220  ddress="0x0713" 
-00031710: 6474 7970 653d 2266 6c6f 6174 2220 6964  dtype="float" id
-00031720: 3d22 4452 565f 5052 4f54 5f4d 414e 5f55  ="DRV_PROT_MAN_U
-00031730: 4e44 4552 5f56 4f4c 5422 2075 6e69 7473  NDER_VOLT" units
-00031740: 3d22 5622 2073 7562 6e6f 6465 3d22 3122  ="V" subnode="1"
-00031750: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
-00031760: 2064 6573 633d 2249 6e64 6963 6174 6573   desc="Indicates
-00031770: 2074 6865 206d 696e 696d 756d 2076 6f6c   the minimum vol
-00031780: 7461 6765 2072 6571 7569 7265 6420 6279  tage required by
-00031790: 2074 6865 2064 7269 7665 2066 6f72 2061   the drive for a
-000317a0: 2070 726f 7065 7220 6f70 6572 6174 696f   proper operatio
-000317b0: 6e22 2063 6174 5f69 643d 2250 524f 5445  n" cat_id="PROTE
-000317c0: 4354 494f 4e53 223e 0d0a 2020 2020 2020  CTIONS">..      
-000317d0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-000317e0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-000317f0: 206c 616e 673d 2265 6e5f 5553 223e 556e   lang="en_US">Un
-00031800: 6465 722d 766f 6c74 6167 6520 6c65 7665  der-voltage leve
-00031810: 6c3c 2f4c 6162 656c 3e0d 0a20 2020 2020  l</Label>..     
-00031820: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00031830: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-00031840: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-00031850: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-00031860: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
-00031870: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
-00031880: 2230 7830 3731 4422 2064 7479 7065 3d22  "0x071D" dtype="
-00031890: 666c 6f61 7422 2069 643d 2244 5256 5f50  float" id="DRV_P
-000318a0: 524f 545f 4d41 4e5f 4d41 585f 434f 4e54  ROT_MAN_MAX_CONT
-000318b0: 5f43 5552 5245 4e54 5f56 414c 5545 2220  _CURRENT_VALUE" 
-000318c0: 756e 6974 733d 2241 2220 7375 626e 6f64  units="A" subnod
-000318d0: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-000318e0: 4e46 4947 2220 6465 7363 3d22 4d61 7869  NFIG" desc="Maxi
-000318f0: 6d75 6d20 636f 6e74 696e 756f 7573 2063  mum continuous c
-00031900: 7572 7265 6e74 206f 6e20 7468 6520 6472  urrent on the dr
-00031910: 6976 6522 2063 6174 5f69 643d 2249 4e54  ive" cat_id="INT
-00031920: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00031930: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00031940: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00031950: 6c61 6e67 3d22 656e 5f55 5322 3e4d 6178  lang="en_US">Max
-00031960: 696d 756d 2064 7269 7665 2063 7572 7265  imum drive curre
-00031970: 6e74 3c2f 4c61 6265 6c3e 0d0a 2020 2020  nt</Label>..    
-00031980: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00031990: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-000319a0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-000319b0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-000319c0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-000319d0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
-000319e0: 3d22 3078 3037 3145 2220 6474 7970 653d  ="0x071E" dtype=
-000319f0: 2275 3332 2220 6964 3d22 4452 565f 5052  "u32" id="DRV_PR
-00031a00: 4f54 5f4d 414e 5f4d 4158 5f50 4541 4b5f  OT_MAN_MAX_PEAK_
-00031a10: 4355 5252 454e 545f 5449 4d45 2220 756e  CURRENT_TIME" un
-00031a20: 6974 733d 226d 7322 2073 7562 6e6f 6465  its="ms" subnode
-00031a30: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-00031a40: 4649 4722 2064 6573 633d 224d 6178 696d  FIG" desc="Maxim
-00031a50: 756d 2074 696d 6520 696e 206d 696c 6c69  um time in milli
-00031a60: 7365 636f 6e64 7320 7468 6520 6d61 7869  seconds the maxi
-00031a70: 6d75 6d20 7065 616b 2063 7572 7265 6e74  mum peak current
-00031a80: 2063 616e 2062 6520 6472 6976 656e 2062   can be driven b
-00031a90: 7920 7468 6520 6472 6976 652e 2220 6361  y the drive." ca
-00031aa0: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
-00031ab0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00031ac0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00031ad0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00031ae0: 6e5f 5553 223e 4d61 7869 6d75 6d20 6472  n_US">Maximum dr
-00031af0: 6976 6520 7065 616b 2063 7572 7265 6e74  ive peak current
-00031b00: 2074 696d 653c 2f4c 6162 656c 3e0d 0a20   time</Label>.. 
-00031b10: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-00031b20: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-00031b30: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-00031b40: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-00031b50: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
-00031b60: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
-00031b70: 6573 733d 2230 7830 3731 4622 2064 7479  ess="0x071F" dty
-00031b80: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
-00031b90: 5256 5f50 524f 545f 4d41 4e5f 4d41 585f  RV_PROT_MAN_MAX_
-00031ba0: 5045 414b 5f43 5552 5245 4e54 5f56 414c  PEAK_CURRENT_VAL
-00031bb0: 5545 2220 756e 6974 733d 2241 2220 7375  UE" units="A" su
-00031bc0: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-00031bd0: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-00031be0: 4d61 7869 6d75 6d20 6162 736f 6c75 7465  Maximum absolute
-00031bf0: 2061 6c6c 6f77 6564 2063 7572 7265 6e74   allowed current
-00031c00: 206f 6e20 6472 6976 6522 2063 6174 5f69   on drive" cat_i
-00031c10: 643d 2249 4e54 4552 4e41 4c22 3e0d 0a20  d="INTERNAL">.. 
-00031c20: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
-00031c30: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00031c40: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00031c50: 5322 3e4d 6178 696d 756d 2064 7269 7665  S">Maximum drive
-00031c60: 2070 6561 6b20 6375 7272 656e 743c 2f4c   peak current</L
-00031c70: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
-00031c80: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-00031c90: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
-00031ca0: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
-00031cb0: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
-00031cc0: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
-00031cd0: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
-00031ce0: 3732 3022 2064 7479 7065 3d22 666c 6f61  720" dtype="floa
-00031cf0: 7422 2069 643d 2246 424b 5f43 5552 5f4d  t" id="FBK_CUR_M
-00031d00: 4541 535f 5241 4e47 4531 2220 756e 6974  EAS_RANGE1" unit
-00031d10: 733d 2241 2220 7375 626e 6f64 653d 2231  s="A" subnode="1
-00031d20: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-00031d30: 2220 6465 7363 3d22 4675 6c6c 206d 6561  " desc="Full mea
-00031d40: 7375 7269 6e67 2072 616e 6765 2066 6f72  suring range for
-00031d50: 2074 6865 2076 6172 6961 626c 6520 6761   the variable ga
-00031d60: 696e 2063 6f6e 6669 6775 7261 7469 6f6e  in configuration
-00031d70: 2031 2069 6e20 416d 7065 7265 7322 2063   1 in Amperes" c
-00031d80: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
-00031d90: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-00031da0: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-00031db0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00031dc0: 656e 5f55 5322 3e43 7572 7265 6e74 206d  en_US">Current m
-00031dd0: 6561 7375 7269 6e67 2072 616e 6765 2031  easuring range 1
-00031de0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00031df0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00031e00: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-00031e10: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
-00031e20: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
-00031e30: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-00031e40: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
-00031e50: 3078 3037 3231 2220 6474 7970 653d 2266  0x0721" dtype="f
-00031e60: 6c6f 6174 2220 6964 3d22 4642 4b5f 4355  loat" id="FBK_CU
-00031e70: 525f 4d45 4153 5f52 414e 4745 3222 2075  R_MEAS_RANGE2" u
-00031e80: 6e69 7473 3d22 4122 2073 7562 6e6f 6465  nits="A" subnode
-00031e90: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-00031ea0: 4649 4722 2064 6573 633d 2246 756c 6c20  FIG" desc="Full 
-00031eb0: 6d65 6173 7572 696e 6720 7261 6e67 6520  measuring range 
-00031ec0: 666f 7220 7468 6520 7661 7269 6162 6c65  for the variable
-00031ed0: 2067 6169 6e20 636f 6e66 6967 7572 6174   gain configurat
-00031ee0: 696f 6e20 3220 696e 2041 6d70 6572 6573  ion 2 in Amperes
-00031ef0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-00031f00: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00031f10: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00031f20: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00031f30: 673d 2265 6e5f 5553 223e 4375 7272 656e  g="en_US">Curren
-00031f40: 7420 6d65 6173 7572 696e 6720 7261 6e67  t measuring rang
-00031f50: 6520 323c 2f4c 6162 656c 3e0d 0a20 2020  e 2</Label>..   
-00031f60: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00031f70: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
-00031f80: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
-00031f90: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
-00031fa0: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
-00031fb0: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
-00031fc0: 733d 2230 7830 3732 3222 2064 7479 7065  s="0x0722" dtype
-00031fd0: 3d22 666c 6f61 7422 2069 643d 2246 424b  ="float" id="FBK
-00031fe0: 5f43 5552 5f4d 4541 535f 5241 4e47 4533  _CUR_MEAS_RANGE3
-00031ff0: 2220 756e 6974 733d 2241 2220 7375 626e  " units="A" subn
-00032000: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
-00032010: 434f 4e46 4947 2220 6465 7363 3d22 4675  CONFIG" desc="Fu
-00032020: 6c6c 206d 6561 7375 7269 6e67 2072 616e  ll measuring ran
-00032030: 6765 2066 6f72 2074 6865 2076 6172 6961  ge for the varia
-00032040: 626c 6520 6761 696e 2063 6f6e 6669 6775  ble gain configu
-00032050: 7261 7469 6f6e 2033 2069 6e20 416d 7065  ration 3 in Ampe
-00032060: 7265 7322 2063 6174 5f69 643d 2249 4e54  res" cat_id="INT
-00032070: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00032080: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00032090: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-000320a0: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
-000320b0: 7265 6e74 206d 6561 7375 7269 6e67 2072  rent measuring r
-000320c0: 616e 6765 2033 3c2f 4c61 6265 6c3e 0d0a  ange 3</Label>..
-000320d0: 2020 2020 2020 2020 2020 3c2f 4c61 6265            </Labe
-000320e0: 6c73 3e0d 0a20 2020 2020 2020 203c 2f52  ls>..        </R
-000320f0: 6567 6973 7465 723e 0d0a 2020 2020 2020  egister>..      
-00032100: 2020 3c52 6567 6973 7465 7220 6163 6365    <Register acce
-00032110: 7373 3d22 7222 2061 6464 7265 7373 5f74  ss="r" address_t
-00032120: 7970 653d 224e 564d 5f48 5722 2061 6464  ype="NVM_HW" add
-00032130: 7265 7373 3d22 3078 3037 3233 2220 6474  ress="0x0723" dt
-00032140: 7970 653d 2266 6c6f 6174 2220 6964 3d22  ype="float" id="
-00032150: 4642 4b5f 4355 525f 4d45 4153 5f52 414e  FBK_CUR_MEAS_RAN
-00032160: 4745 3422 2075 6e69 7473 3d22 4122 2073  GE4" units="A" s
-00032170: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-00032180: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-00032190: 2246 756c 6c20 6d65 6173 7572 696e 6720  "Full measuring 
-000321a0: 7261 6e67 6520 666f 7220 7468 6520 7661  range for the va
-000321b0: 7269 6162 6c65 2067 6169 6e20 636f 6e66  riable gain conf
-000321c0: 6967 7572 6174 696f 6e20 3420 696e 2041  iguration 4 in A
-000321d0: 6d70 6572 6573 2220 6361 745f 6964 3d22  mperes" cat_id="
-000321e0: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
-000321f0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-00032200: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
-00032210: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-00032220: 4375 7272 656e 7420 6d65 6173 7572 696e  Current measurin
-00032230: 6720 7261 6e67 6520 343c 2f4c 6162 656c  g range 4</Label
-00032240: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-00032250: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00032260: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-00032270: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-00032280: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-00032290: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
-000322a0: 6164 6472 6573 733d 2230 7830 3732 3822  address="0x0728"
-000322b0: 2064 7479 7065 3d22 7531 3622 2069 643d   dtype="u16" id=
-000322c0: 2246 424b 5f43 5552 5f4d 4153 4b22 2075  "FBK_CUR_MASK" u
-000322d0: 6e69 7473 3d22 2d22 2073 7562 6e6f 6465  nits="-" subnode
-000322e0: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
-000322f0: 4649 4722 2064 6573 633d 2249 6e69 6469  FIG" desc="Inidi
-00032300: 6361 7465 7320 7468 6520 6e75 6d62 6572  cates the number
-00032310: 206f 6620 6176 6169 6c61 626c 6520 7365   of available se
-00032320: 6e73 6f72 7320 666f 7220 6375 7272 656e  nsors for curren
-00032330: 7420 7365 6e73 696e 6722 2063 6174 5f69  t sensing" cat_i
-00032340: 643d 2249 4e54 4552 4e41 4c22 3e0d 0a20  d="INTERNAL">.. 
-00032350: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
-00032360: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00032370: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00032380: 5322 3e43 7572 7265 6e74 2073 656e 736f  S">Current senso
-00032390: 7273 2075 7365 6420 6d61 736b 3c2f 4c61  rs used mask</La
-000323a0: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
-000323b0: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
-000323c0: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
-000323d0: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
-000323e0: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
-000323f0: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
-00032400: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
-00032410: 3239 2220 6474 7970 653d 2275 3136 2220  29" dtype="u16" 
-00032420: 6964 3d22 4642 4b5f 4355 525f 4143 515f  id="FBK_CUR_ACQ_
-00032430: 5449 4d45 2220 756e 6974 733d 226e 7322  TIME" units="ns"
-00032440: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
-00032450: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
-00032460: 633d 2243 7572 7265 6e74 2061 6371 7569  c="Current acqui
-00032470: 7369 7469 6f6e 2028 7361 6d70 6c65 2061  sition (sample a
-00032480: 6e64 2068 6f6c 6429 2074 696d 6520 696e  nd hold) time in
-00032490: 206e 616e 6f73 6563 6f6e 6473 2220 6361   nanoseconds" ca
-000324a0: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
-000324b0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-000324c0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-000324d0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-000324e0: 6e5f 5553 223e 4375 7272 656e 7420 6163  n_US">Current ac
-000324f0: 7175 6973 6974 696f 6e20 7469 6d65 2028  quisition time (
-00032500: 6e73 293c 2f4c 6162 656c 3e0d 0a20 2020  ns)</Label>..   
-00032510: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00032520: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
-00032530: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
-00032540: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
-00032550: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
-00032560: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
-00032570: 733d 2230 7830 3732 4122 2064 7479 7065  s="0x072A" dtype
-00032580: 3d22 7531 3622 2069 643d 2246 424b 5f43  ="u16" id="FBK_C
-00032590: 5552 5f41 4351 5f41 4456 414e 4345 5f54  UR_ACQ_ADVANCE_T
-000325a0: 494d 4522 2075 6e69 7473 3d22 6e73 2220  IME" units="ns" 
-000325b0: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-000325c0: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-000325d0: 3d22 4375 7272 656e 7420 6163 7175 6973  ="Current acquis
-000325e0: 6974 696f 6e20 6164 7661 6e63 6520 7469  ition advance ti
-000325f0: 6d65 2066 726f 6d20 6365 6e74 6572 206f  me from center o
-00032600: 6620 5057 4d20 696e 206e 616e 6f73 6563  f PWM in nanosec
-00032610: 6f6e 6473 2220 6361 745f 6964 3d22 494e  onds" cat_id="IN
-00032620: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00032630: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00032640: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00032650: 206c 616e 673d 2265 6e5f 5553 223e 4375   lang="en_US">Cu
-00032660: 7272 656e 7420 6163 7175 6973 6974 696f  rrent acquisitio
-00032670: 6e20 6164 7661 6e63 6520 7469 6d65 2028  n advance time (
-00032680: 6e73 293c 2f4c 6162 656c 3e0d 0a20 2020  ns)</Label>..   
-00032690: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-000326a0: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
-000326b0: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
-000326c0: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
-000326d0: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
-000326e0: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
-000326f0: 733d 2230 7830 3732 4222 2064 7479 7065  s="0x072B" dtype
-00032700: 3d22 7533 3222 2069 643d 2244 5256 5f50  ="u32" id="DRV_P
-00032710: 535f 4d49 4e5f 4c4f 575f 5349 4445 5f4f  S_MIN_LOW_SIDE_O
-00032720: 4e5f 5449 4d45 5f32 2220 756e 6974 733d  N_TIME_2" units=
-00032730: 226e 7322 2073 7562 6e6f 6465 3d22 3122  "ns" subnode="1"
-00032740: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
-00032750: 2064 6573 633d 224d 696e 696d 756d 206c   desc="Minimum l
-00032760: 6f77 2073 6964 6520 6f6e 2074 696d 6520  ow side on time 
-00032770: 696e 206e 616e 6f73 6563 6f6e 6473 2066  in nanoseconds f
-00032780: 6f72 2066 7265 7175 656e 6379 2073 656c  or frequency sel
-00032790: 6563 7469 6f6e 2032 2220 6361 745f 6964  ection 2" cat_id
-000327a0: 3d22 494e 5445 524e 414c 223e 0d0a 2020  ="INTERNAL">..  
-000327b0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
-000327c0: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
-000327d0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-000327e0: 223e 4d69 6e2e 206c 6f77 2073 6964 6520  ">Min. low side 
-000327f0: 6f6e 2074 696d 6520 3220 286e 7329 3c2f  on time 2 (ns)</
-00032800: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-00032810: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00032820: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-00032830: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-00032840: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
-00032850: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
-00032860: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
-00032870: 3037 3243 2220 6474 7970 653d 2275 3332  072C" dtype="u32
-00032880: 2220 6964 3d22 4452 565f 5053 5f4d 494e  " id="DRV_PS_MIN
-00032890: 5f4c 4f57 5f53 4944 455f 4f4e 5f54 494d  _LOW_SIDE_ON_TIM
-000328a0: 455f 3322 2075 6e69 7473 3d22 6e73 2220  E_3" units="ns" 
-000328b0: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-000328c0: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-000328d0: 3d22 4d69 6e69 6d75 6d20 6c6f 7720 7369  ="Minimum low si
-000328e0: 6465 206f 6e20 7469 6d65 2069 6e20 6e61  de on time in na
-000328f0: 6e6f 7365 636f 6e64 7320 666f 7220 6672  noseconds for fr
-00032900: 6571 7565 6e63 7920 7365 6c65 6374 696f  equency selectio
-00032910: 6e20 3322 2063 6174 5f69 643d 2249 4e54  n 3" cat_id="INT
-00032920: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00032930: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00032940: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00032950: 6c61 6e67 3d22 656e 5f55 5322 3e4d 696e  lang="en_US">Min
-00032960: 2e20 6c6f 7720 7369 6465 206f 6e20 7469  . low side on ti
-00032970: 6d65 2033 2028 6e73 293c 2f4c 6162 656c  me 3 (ns)</Label
-00032980: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-00032990: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-000329a0: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-000329b0: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-000329c0: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-000329d0: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
-000329e0: 6164 6472 6573 733d 2230 7830 3732 4422  address="0x072D"
-000329f0: 2064 7479 7065 3d22 7533 3222 2069 643d   dtype="u32" id=
-00032a00: 2244 5256 5f50 535f 4d49 4e5f 4c4f 575f  "DRV_PS_MIN_LOW_
-00032a10: 5349 4445 5f4f 4e5f 5449 4d45 5f34 2220  SIDE_ON_TIME_4" 
-00032a20: 756e 6974 733d 226e 7322 2073 7562 6e6f  units="ns" subno
-00032a30: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00032a40: 4f4e 4649 4722 2064 6573 633d 224d 696e  ONFIG" desc="Min
-00032a50: 696d 756d 206c 6f77 2073 6964 6520 6f6e  imum low side on
-00032a60: 2074 696d 6520 696e 206e 616e 6f73 6563   time in nanosec
-00032a70: 6f6e 6473 2066 6f72 2066 7265 7175 656e  onds for frequen
-00032a80: 6379 2073 656c 6563 7469 6f6e 2034 2220  cy selection 4" 
-00032a90: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
-00032aa0: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
-00032ab0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00032ac0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-00032ad0: 2265 6e5f 5553 223e 4d69 6e2e 206c 6f77  "en_US">Min. low
-00032ae0: 2073 6964 6520 6f6e 2074 696d 6520 3420   side on time 4 
-00032af0: 286e 7329 3c2f 4c61 6265 6c3e 0d0a 2020  (ns)</Label>..  
-00032b00: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00032b10: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
-00032b20: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
-00032b30: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
-00032b40: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
-00032b50: 653d 224e 564d 5f48 5722 2061 6464 7265  e="NVM_HW" addre
-00032b60: 7373 3d22 3078 3037 3332 2220 6474 7970  ss="0x0732" dtyp
-00032b70: 653d 2266 6c6f 6174 2220 6964 3d22 4452  e="float" id="DR
-00032b80: 565f 5052 4f54 5f56 4255 535f 4d45 4153  V_PROT_VBUS_MEAS
-00032b90: 5f52 414e 4745 2220 756e 6974 733d 2256  _RANGE" units="V
-00032ba0: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
-00032bb0: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
-00032bc0: 7363 3d22 4675 6c6c 2072 616e 6765 206f  sc="Full range o
-00032bd0: 6620 6275 7320 766f 6c74 6167 6520 6d65  f bus voltage me
-00032be0: 6173 7572 656d 656e 7473 2069 6e20 766f  asurements in vo
-00032bf0: 6c74 732e 2220 6361 745f 6964 3d22 494e  lts." cat_id="IN
-00032c00: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00032c10: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00032c20: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00032c30: 206c 616e 673d 2265 6e5f 5553 223e 4275   lang="en_US">Bu
-00032c40: 7320 766f 6c74 6167 6520 6d65 6173 7572  s voltage measur
-00032c50: 696e 6720 7261 6e67 653c 2f4c 6162 656c  ing range</Label
-00032c60: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-00032c70: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00032c80: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-00032c90: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-00032ca0: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-00032cb0: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
-00032cc0: 6164 6472 6573 733d 2230 7830 3733 3322  address="0x0733"
-00032cd0: 2064 7479 7065 3d22 666c 6f61 7422 2069   dtype="float" i
-00032ce0: 643d 2244 5256 5f50 524f 545f 5642 5553  d="DRV_PROT_VBUS
-00032cf0: 5f4f 4646 5345 5422 2075 6e69 7473 3d22  _OFFSET" units="
-00032d00: 5622 2073 7562 6e6f 6465 3d22 3122 2063  V" subnode="1" c
-00032d10: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
-00032d20: 6573 633d 2243 6f6e 7374 616e 7420 6572  esc="Constant er
-00032d30: 726f 7220 696e 2076 6f6c 7473 206f 6620  ror in volts of 
-00032d40: 7468 6520 6275 7320 766f 6c74 6167 6520  the bus voltage 
-00032d50: 6d65 6173 7572 656d 656e 7473 2220 6361  measurements" ca
-00032d60: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
-00032d70: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00032d80: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00032d90: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00032da0: 6e5f 5553 223e 4275 7320 766f 6c74 6167  n_US">Bus voltag
-00032db0: 6520 7265 6164 696e 6720 6f66 6673 6574  e reading offset
-00032dc0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00032dd0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00032de0: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-00032df0: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
-00032e00: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
-00032e10: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-00032e20: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
-00032e30: 3078 3037 3334 2220 6474 7970 653d 2275  0x0734" dtype="u
-00032e40: 3136 2220 6964 3d22 4452 565f 5052 4f54  16" id="DRV_PROT
-00032e50: 5f50 5249 4d5f 5445 4d50 5f54 5950 4522  _PRIM_TEMP_TYPE"
-00032e60: 2075 6e69 7473 3d22 2d22 2073 7562 6e6f   units="-" subno
-00032e70: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00032e80: 4f4e 4649 4722 2064 6573 633d 2249 6e64  ONFIG" desc="Ind
-00032e90: 6963 6174 6573 2074 6865 2074 656d 7065  icates the tempe
-00032ea0: 7261 7475 7265 2073 656e 736f 7220 7573  rature sensor us
-00032eb0: 6564 2066 6f72 2070 7269 6d61 7279 2074  ed for primary t
-00032ec0: 656d 7065 7261 7475 7265 2072 6561 6469  emperature readi
-00032ed0: 6e67 7320 6f66 2074 6865 2070 6f77 6572  ngs of the power
-00032ee0: 2073 7461 6765 2e22 2063 6174 5f69 643d   stage." cat_id=
-00032ef0: 2249 4e54 4552 4e41 4c22 3e0d 0a20 2020  "INTERNAL">..   
-00032f00: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00032f10: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
-00032f20: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00032f30: 3e50 6f77 6572 2073 7461 6765 2074 656d  >Power stage tem
-00032f40: 702e 2073 656e 736f 7220 3120 7479 7065  p. sensor 1 type
-00032f50: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00032f60: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00032f70: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-00032f80: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
-00032f90: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
-00032fa0: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-00032fb0: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
-00032fc0: 3078 3037 3335 2220 6474 7970 653d 2275  0x0735" dtype="u
-00032fd0: 3332 2220 6964 3d22 4452 565f 5052 4f54  32" id="DRV_PROT
-00032fe0: 5f50 5249 4d5f 5445 4d50 5f52 4553 2220  _PRIM_TEMP_RES" 
-00032ff0: 756e 6974 733d 22ce a922 2073 7562 6e6f  units=".." subno
-00033000: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00033010: 4f4e 4649 4722 2064 6573 633d 224e 5443  ONFIG" desc="NTC
-00033020: 3a20 5265 7369 7374 616e 6365 2076 616c  : Resistance val
-00033030: 7565 2066 6f72 2032 3520 c2ba 4320 696e  ue for 25 ..C in
-00033040: 206f 686d 7326 2331 333b 2623 3130 3b50   ohms&#13;&#10;P
-00033050: 5443 3a20 5265 7369 7374 616e 6365 2076  TC: Resistance v
-00033060: 616c 7565 2069 6e20 6f68 6d73 2077 6865  alue in ohms whe
-00033070: 7265 2074 6865 206f 7665 722d 7465 6d70  re the over-temp
-00033080: 6572 6174 7572 6520 6d75 7374 2062 6520  erature must be 
-00033090: 6465 7465 6374 6564 2623 3133 3b26 2331  detected&#13;&#1
-000330a0: 303b 4f74 6865 7273 3a20 4e6f 7420 7573  0;Others: Not us
-000330b0: 6564 2220 6361 745f 6964 3d22 494e 5445  ed" cat_id="INTE
-000330c0: 524e 414c 223e 0d0a 2020 2020 2020 2020  RNAL">..        
-000330d0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-000330e0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-000330f0: 616e 673d 2265 6e5f 5553 223e 506f 7765  ang="en_US">Powe
-00033100: 7220 7374 6167 6520 7465 6d70 2e20 7365  r stage temp. se
-00033110: 6e73 6f72 2031 2072 6573 6973 7461 6e63  nsor 1 resistanc
-00033120: 653c 2f4c 6162 656c 3e0d 0a20 2020 2020  e</Label>..     
-00033130: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00033140: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-00033150: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-00033160: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-00033170: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
-00033180: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
-00033190: 2230 7830 3733 3622 2064 7479 7065 3d22  "0x0736" dtype="
-000331a0: 7531 3622 2069 643d 2244 5256 5f50 524f  u16" id="DRV_PRO
-000331b0: 545f 5052 494d 5f54 454d 505f 4232 3538  T_PRIM_TEMP_B258
-000331c0: 3522 2075 6e69 7473 3d22 c2ba 4b22 2073  5" units="..K" s
-000331d0: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-000331e0: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-000331f0: 224e 5443 3a20 4228 3235 2f38 3529 2070  "NTC: B(25/85) p
-00033200: 6172 616d 6574 6572 2066 726f 6d20 6461  arameter from da
-00033210: 7461 7368 6565 7426 2331 333b 2623 3130  tasheet&#13;&#10
-00033220: 3b4f 7468 6572 733a 204e 6f74 2075 7365  ;Others: Not use
-00033230: 6422 2063 6174 5f69 643d 2249 4e54 4552  d" cat_id="INTER
-00033240: 4e41 4c22 3e0d 0a20 2020 2020 2020 2020  NAL">..         
-00033250: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
-00033260: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
-00033270: 6e67 3d22 656e 5f55 5322 3e50 6f77 6572  ng="en_US">Power
-00033280: 2073 7461 6765 2074 656d 702e 2073 656e   stage temp. sen
-00033290: 736f 7220 3120 ceb2 3c2f 4c61 6265 6c3e  sor 1 ..</Label>
-000332a0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-000332b0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-000332c0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-000332d0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-000332e0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
-000332f0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
-00033300: 6464 7265 7373 3d22 3078 3037 3337 2220  ddress="0x0737" 
-00033310: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
-00033320: 4452 565f 5052 4f54 5f50 5249 4d5f 5445  DRV_PROT_PRIM_TE
-00033330: 4d50 5f45 5854 5f52 4553 2220 756e 6974  MP_EXT_RES" unit
-00033340: 733d 22ce a922 2073 7562 6e6f 6465 3d22  s=".." subnode="
-00033350: 3122 2063 7963 6c69 633d 2243 4f4e 4649  1" cyclic="CONFI
-00033360: 4722 2064 6573 633d 224e 5443 2026 616d  G" desc="NTC &am
-00033370: 703b 616d 703b 2050 5443 3a20 5265 7369  p;amp; PTC: Resi
-00033380: 7374 616e 6365 2076 616c 7565 2069 6e20  stance value in 
-00033390: 6f68 6d73 2063 6f6e 6e65 6374 6564 2074  ohms connected t
-000333a0: 6f20 7365 6e73 6f72 2066 6f72 206d 616b  o sensor for mak
-000333b0: 696e 6720 7468 6520 766f 6c74 6167 6520  ing the voltage 
-000333c0: 6469 7669 6465 7226 2331 333b 2623 3130  divider&#13;&#10
-000333d0: 3b4f 7468 6572 3a20 4e6f 7420 7573 6564  ;Other: Not used
-000333e0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-000333f0: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00033400: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00033410: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00033420: 673d 2265 6e5f 5553 223e 506f 7765 7220  g="en_US">Power 
-00033430: 7374 6167 6520 7465 6d70 2e20 7365 6e73  stage temp. sens
-00033440: 6f72 2031 2065 7874 2e20 7265 7369 7374  or 1 ext. resist
-00033450: 616e 6365 3c2f 4c61 6265 6c3e 0d0a 2020  ance</Label>..  
-00033460: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00033470: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
-00033480: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
-00033490: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
-000334a0: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
-000334b0: 653d 224e 564d 5f48 5722 2061 6464 7265  e="NVM_HW" addre
-000334c0: 7373 3d22 3078 3037 3338 2220 6474 7970  ss="0x0738" dtyp
-000334d0: 653d 2266 6c6f 6174 2220 6964 3d22 4452  e="float" id="DR
-000334e0: 565f 5052 4f54 5f50 5249 4d5f 5445 4d50  V_PROT_PRIM_TEMP
-000334f0: 5f47 4149 4e22 2075 6e69 7473 3d22 c2ba  _GAIN" units="..
-00033500: 4320 2f20 5622 2073 7562 6e6f 6465 3d22  C / V" subnode="
-00033510: 3122 2063 7963 6c69 633d 2243 4f4e 4649  1" cyclic="CONFI
-00033520: 4722 2064 6573 633d 224c 696e 6561 7220  G" desc="Linear 
-00033530: 766f 6c74 6167 6520 7365 6e73 6f72 3a20  voltage sensor: 
-00033540: 4761 696e 206f 6620 7468 6520 7365 6e73  Gain of the sens
-00033550: 6f72 2623 3133 3b26 2331 303b 4f74 6865  or&#13;&#10;Othe
-00033560: 7273 3a20 4e6f 7420 7573 6564 2220 6361  rs: Not used" ca
-00033570: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
-00033580: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00033590: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-000335a0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-000335b0: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
-000335c0: 6520 7465 6d70 2e20 7365 6e73 6f72 2031  e temp. sensor 1
-000335d0: 2067 6169 6e3c 2f4c 6162 656c 3e0d 0a20   gain</Label>.. 
-000335e0: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-000335f0: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-00033600: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-00033610: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-00033620: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
-00033630: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
-00033640: 6573 733d 2230 7830 3733 3922 2064 7479  ess="0x0739" dty
-00033650: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
-00033660: 5256 5f50 524f 545f 5052 494d 5f54 454d  RV_PROT_PRIM_TEM
-00033670: 505f 4f46 4653 4554 2220 756e 6974 733d  P_OFFSET" units=
-00033680: 22c2 ba43 2220 7375 626e 6f64 653d 2231  "..C" subnode="1
-00033690: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-000336a0: 2220 6465 7363 3d22 4e54 4320 2661 6d70  " desc="NTC &amp
-000336b0: 3b61 6d70 3b20 5054 433a 204e 6f74 2075  ;amp; PTC: Not u
-000336c0: 7365 6426 2331 333b 2623 3130 3b4c 696e  sed&#13;&#10;Lin
-000336d0: 6561 7220 7365 6e73 6f72 3a20 4f66 6673  ear sensor: Offs
-000336e0: 6574 206f 6620 7468 6520 7365 6e73 6f72  et of the sensor
-000336f0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-00033700: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00033710: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00033720: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00033730: 673d 2265 6e5f 5553 223e 506f 7765 7220  g="en_US">Power 
-00033740: 7374 6167 6520 7465 6d70 2e20 7365 6e73  stage temp. sens
-00033750: 6f72 2031 206f 6666 7365 743c 2f4c 6162  or 1 offset</Lab
-00033760: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00033770: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00033780: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00033790: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-000337a0: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-000337b0: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-000337c0: 2220 6164 6472 6573 733d 2230 7830 3734  " address="0x074
-000337d0: 3022 2064 7479 7065 3d22 7533 3222 2069  0" dtype="u32" i
-000337e0: 643d 2244 5256 5f50 524f 545f 5354 4f5f  d="DRV_PROT_STO_
-000337f0: 4346 4722 2075 6e69 7473 3d22 2d22 2073  CFG" units="-" s
-00033800: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-00033810: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-00033820: 2249 6e64 6963 6174 6573 2074 6865 2047  "Indicates the G
-00033830: 5049 2075 7365 6420 666f 7220 6465 7465  PI used for dete
-00033840: 6374 696e 6720 5354 4f20 6e6f 7469 6669  cting STO notifi
-00033850: 6361 7469 6f6e 2220 6361 745f 6964 3d22  cation" cat_id="
-00033860: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
-00033870: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-00033880: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
-00033890: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-000338a0: 5354 4f20 636f 6e66 6967 7572 6174 696f  STO configuratio
-000338b0: 6e3c 2f4c 6162 656c 3e0d 0a20 2020 2020  n</Label>..     
-000338c0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-000338d0: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
-000338e0: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
-000338f0: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
-00033900: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
-00033910: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
-00033920: 2230 7830 3734 3122 2064 7479 7065 3d22  "0x0741" dtype="
-00033930: 7533 3222 2069 643d 224d 4f54 5f42 5241  u32" id="MOT_BRA
-00033940: 4b45 5f43 4f4e 4649 4755 5241 5449 4f4e  KE_CONFIGURATION
-00033950: 2220 756e 6974 733d 222d 2220 7375 626e  " units="-" subn
-00033960: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
-00033970: 434f 4e46 4947 2220 6465 7363 3d22 496e  CONFIG" desc="In
-00033980: 6469 6361 7465 7320 7468 6520 4750 4f20  dicates the GPO 
-00033990: 7573 6564 2061 7320 6272 616b 652e 2220  used as brake." 
-000339a0: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
-000339b0: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
-000339c0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-000339d0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-000339e0: 2265 6e5f 5553 223e 4272 616b 6520 636f  "en_US">Brake co
-000339f0: 6e66 6967 7572 6174 696f 6e3c 2f4c 6162  nfiguration</Lab
-00033a00: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00033a10: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00033a20: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00033a30: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00033a40: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00033a50: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00033a60: 2220 6164 6472 6573 733d 2230 7830 3734  " address="0x074
-00033a70: 3222 2064 7479 7065 3d22 7533 3222 2069  2" dtype="u32" i
-00033a80: 643d 224d 4f54 5f42 5241 4b45 5f4d 4158  d="MOT_BRAKE_MAX
-00033a90: 5f46 5245 5122 2075 6e69 7473 3d22 487a  _FREQ" units="Hz
-00033aa0: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
-00033ab0: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
-00033ac0: 7363 3d22 496e 6469 6361 7465 7320 7468  sc="Indicates th
-00033ad0: 6520 6d61 7869 6d75 6d20 616c 6c6f 7765  e maximum allowe
-00033ae0: 6420 636f 6d6d 7574 6174 696f 6e20 6672  d commutation fr
-00033af0: 6571 7565 6e63 7920 6279 2074 6865 2062  equency by the b
-00033b00: 7261 6b65 2065 6c65 6374 726f 6e69 6373  rake electronics
-00033b10: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-00033b20: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00033b30: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00033b40: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00033b50: 673d 2265 6e5f 5553 223e 4272 616b 6520  g="en_US">Brake 
-00033b60: 6d61 782e 2066 7265 7175 656e 6379 3c2f  max. frequency</
-00033b70: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-00033b80: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00033b90: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-00033ba0: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-00033bb0: 7465 7220 6163 6365 7373 3d22 7277 2220  ter access="rw" 
-00033bc0: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
-00033bd0: 4d5f 4346 4722 2061 6464 7265 7373 3d22  M_CFG" address="
-00033be0: 3078 3037 3433 2220 6474 7970 653d 2275  0x0743" dtype="u
-00033bf0: 3332 2220 6964 3d22 4d4f 545f 4252 414b  32" id="MOT_BRAK
-00033c00: 455f 4652 4551 2220 756e 6974 733d 2248  E_FREQ" units="H
-00033c10: 7a22 2073 7562 6e6f 6465 3d22 3122 2063  z" subnode="1" c
-00033c20: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
-00033c30: 6573 633d 2242 7261 6b65 2066 7265 7175  esc="Brake frequ
-00033c40: 656e 6379 2069 6e20 6865 7274 7a2e 204f  ency in hertz. O
-00033c50: 6e6c 7920 7661 6c75 6573 206c 6f77 6572  nly values lower
-00033c60: 2074 6861 6e20 7468 6520 6d61 7869 6d75   than the maximu
-00033c70: 6d20 6272 616b 6520 6672 6571 7565 6e63  m brake frequenc
-00033c80: 7920 7769 6c6c 2062 6520 616c 6c6f 7765  y will be allowe
-00033c90: 642e 2056 616c 7565 2030 2064 6973 6162  d. Value 0 disab
-00033ca0: 6c65 7320 6d6f 6475 6c61 7465 6420 6272  les modulated br
-00033cb0: 616b 6520 6f75 7470 7574 2e22 2063 6174  ake output." cat
-00033cc0: 5f69 643d 224d 4f54 4f52 223e 0d0a 2020  _id="MOTOR">..  
-00033cd0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
-00033ce0: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
-00033cf0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-00033d00: 223e 4272 616b 6520 6672 6571 7565 6e63  ">Brake frequenc
-00033d10: 793c 2f4c 6162 656c 3e0d 0a20 2020 2020  y</Label>..     
-00033d20: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00033d30: 2020 2020 2020 2020 2020 3c52 616e 6765            <Range
-00033d40: 206d 696e 3d22 3430 3030 2220 6d61 783d   min="4000" max=
-00033d50: 2234 3030 3030 222f 3e0d 0a20 2020 2020  "40000"/>..     
-00033d60: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
-00033d70: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
-00033d80: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
-00033d90: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
-00033da0: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
-00033db0: 3436 2220 6474 7970 653d 2275 3136 2220  46" dtype="u16" 
-00033dc0: 6964 3d22 4452 565f 5052 4f54 5f52 4544  id="DRV_PROT_RED
-00033dd0: 5f54 454d 505f 5459 5045 2220 756e 6974  _TEMP_TYPE" unit
-00033de0: 733d 222d 2220 7375 626e 6f64 653d 2231  s="-" subnode="1
-00033df0: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
-00033e00: 2220 6465 7363 3d22 496e 6469 6361 7465  " desc="Indicate
-00033e10: 7320 7468 6520 7479 7065 206f 6620 7465  s the type of te
-00033e20: 6d70 6572 6174 7572 6520 7365 6e73 6f72  mperature sensor
-00033e30: 2069 7320 7573 6564 2066 6f72 2074 6865   is used for the
-00033e40: 2072 6564 756e 6461 6e74 2074 656d 7065   redundant tempe
-00033e50: 7261 7475 7265 2073 656e 736f 7220 7479  rature sensor ty
-00033e60: 7065 2220 6361 745f 6964 3d22 494e 5445  pe" cat_id="INTE
-00033e70: 524e 414c 223e 0d0a 2020 2020 2020 2020  RNAL">..        
-00033e80: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00033e90: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00033ea0: 616e 673d 2265 6e5f 5553 223e 506f 7765  ang="en_US">Powe
-00033eb0: 7220 7374 6167 6520 7465 6d70 2e20 7365  r stage temp. se
-00033ec0: 6e73 6f72 2032 2074 7970 653c 2f4c 6162  nsor 2 type</Lab
-00033ed0: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00033ee0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00033ef0: 2020 2020 3c45 6e75 6d65 7261 7469 6f6e      <Enumeration
-00033f00: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
-00033f10: 3c45 6e75 6d20 7661 6c75 653d 2230 223e  <Enum value="0">
-00033f20: 4e54 433c 2f45 6e75 6d3e 0d0a 2020 2020  NTC</Enum>..    
-00033f30: 2020 2020 2020 2020 3c45 6e75 6d20 7661          <Enum va
-00033f40: 6c75 653d 2231 223e 5054 433c 2f45 6e75  lue="1">PTC</Enu
-00033f50: 6d3e 0d0a 2020 2020 2020 2020 2020 2020  m>..            
-00033f60: 3c45 6e75 6d20 7661 6c75 653d 2232 223e  <Enum value="2">
-00033f70: 4c69 6e65 6172 2073 656e 736f 723c 2f45  Linear sensor</E
-00033f80: 6e75 6d3e 0d0a 2020 2020 2020 2020 2020  num>..          
-00033f90: 3c2f 456e 756d 6572 6174 696f 6e73 3e0d  </Enumerations>.
-00033fa0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-00033fb0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-00033fc0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-00033fd0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-00033fe0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
-00033ff0: 3d22 3078 3037 3437 2220 6474 7970 653d  ="0x0747" dtype=
-00034000: 2275 3332 2220 6964 3d22 4452 565f 5052  "u32" id="DRV_PR
-00034010: 4f54 5f52 4544 5f54 454d 505f 5245 5322  OT_RED_TEMP_RES"
-00034020: 2075 6e69 7473 3d22 cea9 2220 7375 626e   units=".." subn
-00034030: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
-00034040: 434f 4e46 4947 2220 6465 7363 3d22 4e54  CONFIG" desc="NT
-00034050: 433a 2052 6573 6973 7461 6e63 6520 7661  C: Resistance va
-00034060: 6c75 6520 666f 7220 3235 20c2 ba43 2069  lue for 25 ..C i
-00034070: 6e20 6f68 6d73 2623 3133 3b26 2331 303b  n ohms&#13;&#10;
-00034080: 5054 433a 2052 6573 6973 7461 6e63 6520  PTC: Resistance 
-00034090: 7661 6c75 6520 696e 206f 686d 7320 7768  value in ohms wh
-000340a0: 6572 6520 7468 6520 6f76 6572 2d74 656d  ere the over-tem
-000340b0: 7065 7261 7475 7265 206d 7573 7420 6265  perature must be
-000340c0: 2064 6574 6563 7465 6426 2331 333b 2623   detected&#13;&#
-000340d0: 3130 3b4f 7468 6572 733a 204e 6f74 2075  10;Others: Not u
-000340e0: 7365 6422 2063 6174 5f69 643d 2249 4e54  sed" cat_id="INT
-000340f0: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00034100: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00034110: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00034120: 6c61 6e67 3d22 656e 5f55 5322 3e50 6f77  lang="en_US">Pow
-00034130: 6572 2073 7461 6765 2074 656d 702e 2073  er stage temp. s
-00034140: 656e 736f 7220 3220 7265 7369 7374 616e  ensor 2 resistan
-00034150: 6365 3c2f 4c61 6265 6c3e 0d0a 2020 2020  ce</Label>..    
-00034160: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00034170: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-00034180: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-00034190: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-000341a0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-000341b0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
-000341c0: 3d22 3078 3037 3438 2220 6474 7970 653d  ="0x0748" dtype=
-000341d0: 2275 3136 2220 6964 3d22 4452 565f 5052  "u16" id="DRV_PR
-000341e0: 4f54 5f52 4544 5f54 454d 505f 4232 3538  OT_RED_TEMP_B258
-000341f0: 3522 2075 6e69 7473 3d22 c2ba 4b22 2073  5" units="..K" s
-00034200: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-00034210: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-00034220: 224e 5443 3a20 4228 3235 2f38 3529 2070  "NTC: B(25/85) p
-00034230: 6172 616d 6574 6572 2066 726f 6d20 6461  arameter from da
-00034240: 7461 7368 6565 7426 2331 333b 2623 3130  tasheet&#13;&#10
-00034250: 3b50 5443 3a20 4e6f 7420 7573 6564 2623  ;PTC: Not used&#
-00034260: 3133 3b26 2331 303b 4f74 6865 723a 204e  13;&#10;Other: N
-00034270: 6f74 2075 7365 6422 2063 6174 5f69 643d  ot used" cat_id=
-00034280: 2249 4e54 4552 4e41 4c22 3e0d 0a20 2020  "INTERNAL">..   
-00034290: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-000342a0: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
-000342b0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-000342c0: 3e50 6f77 6572 2073 7461 6765 2074 656d  >Power stage tem
-000342d0: 702e 2073 656e 736f 7220 3220 ceb2 3c2f  p. sensor 2 ..</
-000342e0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-000342f0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00034300: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-00034310: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-00034320: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
-00034330: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
-00034340: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
-00034350: 3037 3439 2220 6474 7970 653d 2275 3332  0749" dtype="u32
-00034360: 2220 6964 3d22 4452 565f 5052 4f54 5f52  " id="DRV_PROT_R
-00034370: 4544 5f54 454d 505f 4558 545f 5245 5322  ED_TEMP_EXT_RES"
-00034380: 2075 6e69 7473 3d22 cea9 2220 7375 626e   units=".." subn
-00034390: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
-000343a0: 434f 4e46 4947 2220 6465 7363 3d22 4e54  CONFIG" desc="NT
-000343b0: 4320 2661 6d70 3b61 6d70 3b20 5054 433a  C &amp;amp; PTC:
-000343c0: 2052 6573 6973 7461 6e63 6520 7661 6c75   Resistance valu
-000343d0: 6520 696e 206f 686d 7320 636f 6e6e 6563  e in ohms connec
-000343e0: 7465 6420 746f 2074 6865 2073 656e 736f  ted to the senso
-000343f0: 7220 666f 7220 6d61 6b69 6e67 2074 6865  r for making the
-00034400: 2076 6f6c 7461 6765 2064 6976 6964 6572   voltage divider
-00034410: 2623 3133 3b26 2331 303b 4f74 6865 7273  &#13;&#10;Others
-00034420: 3a20 4e6f 7420 7573 6564 2220 6361 745f  : Not used" cat_
-00034430: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
-00034440: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00034450: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
-00034460: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-00034470: 5553 223e 506f 7765 7220 7374 6167 6520  US">Power stage 
-00034480: 7465 6d70 2e20 7365 6e73 6f72 2032 2065  temp. sensor 2 e
-00034490: 7874 2e20 7265 7369 7374 616e 6365 3c2f  xt. resistance</
-000344a0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-000344b0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-000344c0: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
-000344d0: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
-000344e0: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
-000344f0: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
-00034500: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
-00034510: 3037 3441 2220 6474 7970 653d 2266 6c6f  074A" dtype="flo
-00034520: 6174 2220 6964 3d22 4452 565f 5052 4f54  at" id="DRV_PROT
-00034530: 5f52 4544 5f54 454d 505f 4741 494e 2220  _RED_TEMP_GAIN" 
-00034540: 756e 6974 733d 22c2 ba43 202f 2056 2220  units="..C / V" 
-00034550: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-00034560: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-00034570: 3d22 4c69 6e65 6172 2076 6f6c 7461 6765  ="Linear voltage
-00034580: 2073 656e 736f 723a 2047 6169 6e20 6f66   sensor: Gain of
-00034590: 2074 6865 2073 656e 736f 722e 2623 3133   the sensor.&#13
-000345a0: 3b26 2331 303b 4f74 6865 7273 3a20 4e6f  ;&#10;Others: No
-000345b0: 7420 7573 6564 2220 6361 745f 6964 3d22  t used" cat_id="
-000345c0: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
-000345d0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-000345e0: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
-000345f0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-00034600: 506f 7765 7220 7374 6167 6520 7465 6d70  Power stage temp
-00034610: 2e20 7365 6e73 6f72 2032 2067 6169 6e3c  . sensor 2 gain<
-00034620: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-00034630: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
-00034640: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
-00034650: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
-00034660: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
-00034670: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
-00034680: 4d5f 4857 2220 6164 6472 6573 733d 2230  M_HW" address="0
-00034690: 7830 3734 4222 2064 7479 7065 3d22 666c  x074B" dtype="fl
-000346a0: 6f61 7422 2069 643d 2244 5256 5f50 524f  oat" id="DRV_PRO
-000346b0: 545f 5245 445f 5445 4d50 5f4f 4646 5345  T_RED_TEMP_OFFSE
-000346c0: 5422 2075 6e69 7473 3d22 c2ba 4322 2073  T" units="..C" s
-000346d0: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
-000346e0: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
-000346f0: 224e 5443 2026 616d 703b 616d 703b 2050  "NTC &amp;amp; P
-00034700: 5443 3a20 4e6f 7420 7573 6564 2623 3133  TC: Not used&#13
-00034710: 3b26 2331 303b 4f74 6865 7273 3a20 4f66  ;&#10;Others: Of
-00034720: 6673 6574 206f 6620 7468 6520 7365 6e73  fset of the sens
-00034730: 6f72 2220 6361 745f 6964 3d22 494e 5445  or" cat_id="INTE
-00034740: 524e 414c 223e 0d0a 2020 2020 2020 2020  RNAL">..        
-00034750: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00034760: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00034770: 616e 673d 2265 6e5f 5553 223e 506f 7765  ang="en_US">Powe
-00034780: 7220 7374 6167 6520 7465 6d70 2e20 7365  r stage temp. se
-00034790: 6e73 6f72 2032 206f 6666 7365 743c 2f4c  nsor 2 offset</L
-000347a0: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
-000347b0: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-000347c0: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
-000347d0: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
-000347e0: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
-000347f0: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
-00034800: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
-00034810: 3735 3022 2064 7479 7065 3d22 666c 6f61  750" dtype="floa
-00034820: 7422 2069 643d 2244 5256 5f50 524f 545f  t" id="DRV_PROT_
-00034830: 4445 5241 5449 4e47 5f43 4f4e 5354 2220  DERATING_CONST" 
-00034840: 756e 6974 733d 222d 2220 7375 626e 6f64  units="-" subnod
-00034850: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-00034860: 4e46 4947 2220 6465 7363 3d22 436f 6e73  NFIG" desc="Cons
-00034870: 7461 6e74 2061 7070 6c69 6564 2069 6e20  tant applied in 
-00034880: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-00034890: 6472 6976 6520 7465 6d70 6572 6174 7572  drive temperatur
-000348a0: 6520 746f 2074 6865 206d 6178 696d 756d  e to the maximum
-000348b0: 206e 6f6d 696e 616c 2063 7572 7265 6e74   nominal current
-000348c0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-000348d0: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-000348e0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-000348f0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00034900: 673d 2265 6e5f 5553 223e 4465 7261 7469  g="en_US">Derati
-00034910: 6e67 2063 6f6e 7374 616e 743c 2f4c 6162  ng constant</Lab
-00034920: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00034930: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00034940: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00034950: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00034960: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00034970: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00034980: 2220 6164 6472 6573 733d 2230 7830 3735  " address="0x075
-00034990: 3122 2064 7479 7065 3d22 666c 6f61 7422  1" dtype="float"
-000349a0: 2069 643d 2244 5256 5f50 524f 545f 4445   id="DRV_PROT_DE
-000349b0: 5241 5449 4e47 5f46 5245 515f 434f 4e53  RATING_FREQ_CONS
-000349c0: 5431 2220 756e 6974 733d 222d 2220 7375  T1" units="-" su
-000349d0: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-000349e0: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-000349f0: 4465 7261 7469 6e67 2063 6f6e 7374 616e  Derating constan
-00034a00: 7420 666f 7220 636f 6d6d 7574 6174 696f  t for commutatio
-00034a10: 6e20 6672 6571 7565 6e63 7920 3120 7468  n frequency 1 th
-00034a20: 6174 206d 6f64 6966 6965 7320 7468 6520  at modifies the 
-00034a30: 7465 6d70 6572 6174 7572 6520 7468 7265  temperature thre
-00034a40: 7368 6f6c 6420 666f 7220 7374 6172 7469  shold for starti
-00034a50: 6e67 2063 7572 7265 6e74 2064 6572 6174  ng current derat
-00034a60: 696e 672e 2220 6361 745f 6964 3d22 494e  ing." cat_id="IN
-00034a70: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00034a80: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00034a90: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00034aa0: 206c 616e 673d 2265 6e5f 5553 223e 4672   lang="en_US">Fr
-00034ab0: 6571 7565 6e63 7920 3120 6465 7261 7469  equency 1 derati
-00034ac0: 6e67 2063 6f6e 7374 616e 743c 2f4c 6162  ng constant</Lab
-00034ad0: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00034ae0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00034af0: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00034b00: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00034b10: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00034b20: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00034b30: 2220 6164 6472 6573 733d 2230 7830 3735  " address="0x075
-00034b40: 3222 2064 7479 7065 3d22 666c 6f61 7422  2" dtype="float"
-00034b50: 2069 643d 2244 5256 5f50 524f 545f 4445   id="DRV_PROT_DE
-00034b60: 5241 5449 4e47 5f46 5245 515f 434f 4e53  RATING_FREQ_CONS
-00034b70: 5432 2220 756e 6974 733d 222d 2220 7375  T2" units="-" su
-00034b80: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-00034b90: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-00034ba0: 4465 7261 7469 6e67 2063 6f6e 7374 616e  Derating constan
-00034bb0: 7420 666f 7220 636f 6d6d 7574 6174 696f  t for commutatio
-00034bc0: 6e20 6672 6571 7565 6e63 7920 3220 7468  n frequency 2 th
-00034bd0: 6174 206d 6f64 6966 6965 7320 7468 6520  at modifies the 
-00034be0: 7465 6d70 6572 6174 7572 6520 7468 7265  temperature thre
-00034bf0: 7368 6f6c 6420 666f 7220 7374 6172 7469  shold for starti
-00034c00: 6e67 2063 7572 7265 6e74 2064 6572 6174  ng current derat
-00034c10: 696e 672e 2220 6361 745f 6964 3d22 494e  ing." cat_id="IN
-00034c20: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00034c30: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00034c40: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00034c50: 206c 616e 673d 2265 6e5f 5553 223e 4672   lang="en_US">Fr
-00034c60: 6571 7565 6e63 7920 3220 6465 7261 7469  equency 2 derati
-00034c70: 6e67 2063 6f6e 7374 616e 743c 2f4c 6162  ng constant</Lab
-00034c80: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00034c90: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00034ca0: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00034cb0: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00034cc0: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00034cd0: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00034ce0: 2220 6164 6472 6573 733d 2230 7830 3735  " address="0x075
-00034cf0: 3322 2064 7479 7065 3d22 666c 6f61 7422  3" dtype="float"
-00034d00: 2069 643d 2244 5256 5f50 524f 545f 4445   id="DRV_PROT_DE
-00034d10: 5241 5449 4e47 5f46 5245 515f 434f 4e53  RATING_FREQ_CONS
-00034d20: 5433 2220 756e 6974 733d 222d 2220 7375  T3" units="-" su
-00034d30: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-00034d40: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-00034d50: 4465 7261 7469 6e67 2063 6f6e 7374 616e  Derating constan
-00034d60: 7420 666f 7220 636f 6d6d 7574 6174 696f  t for commutatio
-00034d70: 6e20 6672 6571 7565 6e63 7920 3320 7468  n frequency 3 th
-00034d80: 6174 206d 6f64 6966 6965 7320 7468 6520  at modifies the 
-00034d90: 7465 6d70 6572 6174 7572 6520 7468 7265  temperature thre
-00034da0: 7368 6f6c 6420 666f 7220 7374 6172 7469  shold for starti
-00034db0: 6e67 2063 7572 7265 6e74 2064 6572 6174  ng current derat
-00034dc0: 696e 672e 2220 6361 745f 6964 3d22 494e  ing." cat_id="IN
-00034dd0: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00034de0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00034df0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00034e00: 206c 616e 673d 2265 6e5f 5553 223e 4672   lang="en_US">Fr
-00034e10: 6571 7565 6e63 7920 3320 6465 7261 7469  equency 3 derati
-00034e20: 6e67 2063 6f6e 7374 616e 743c 2f4c 6162  ng constant</Lab
-00034e30: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00034e40: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00034e50: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00034e60: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00034e70: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00034e80: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00034e90: 2220 6164 6472 6573 733d 2230 7830 3735  " address="0x075
-00034ea0: 3422 2064 7479 7065 3d22 666c 6f61 7422  4" dtype="float"
-00034eb0: 2069 643d 2244 5256 5f50 524f 545f 4445   id="DRV_PROT_DE
-00034ec0: 5241 5449 4e47 5f46 5245 515f 434f 4e53  RATING_FREQ_CONS
-00034ed0: 5434 2220 756e 6974 733d 222d 2220 7375  T4" units="-" su
-00034ee0: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
-00034ef0: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
-00034f00: 4465 7261 7469 6e67 2063 6f6e 7374 616e  Derating constan
-00034f10: 7420 666f 7220 636f 6d6d 7574 6174 696f  t for commutatio
-00034f20: 6e20 6672 6571 7565 6e63 7920 3420 7468  n frequency 4 th
-00034f30: 6174 206d 6f64 6966 6965 7320 7468 6520  at modifies the 
-00034f40: 7465 6d70 6572 6174 7572 6520 7468 7265  temperature thre
-00034f50: 7368 6f6c 6420 666f 7220 7374 6172 7469  shold for starti
-00034f60: 6e67 2063 7572 7265 6e74 2064 6572 6174  ng current derat
-00034f70: 696e 672e 2220 6361 745f 6964 3d22 494e  ing." cat_id="IN
-00034f80: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
-00034f90: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00034fa0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00034fb0: 206c 616e 673d 2265 6e5f 5553 223e 4672   lang="en_US">Fr
-00034fc0: 6571 7565 6e63 7920 3420 6465 7261 7469  equency 4 derati
-00034fd0: 6e67 2063 6f6e 7374 616e 743c 2f4c 6162  ng constant</Lab
-00034fe0: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
-00034ff0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00035000: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
-00035010: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
-00035020: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
-00035030: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
-00035040: 2220 6164 6472 6573 733d 2230 7830 3735  " address="0x075
-00035050: 4122 2064 7479 7065 3d22 666c 6f61 7422  A" dtype="float"
-00035060: 2069 643d 2244 5256 5f50 524f 545f 4445   id="DRV_PROT_DE
-00035070: 5241 5449 4e47 5f54 454d 505f 5448 5245  RATING_TEMP_THRE
-00035080: 5348 4f4c 445f 3122 2075 6e69 7473 3d22  SHOLD_1" units="
-00035090: 4122 2073 7562 6e6f 6465 3d22 3122 2063  A" subnode="1" c
-000350a0: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
-000350b0: 6573 633d 2254 6872 6573 686f 6c64 2074  esc="Threshold t
-000350c0: 656d 7065 7261 7475 7265 2074 6861 7420  emperature that 
-000350d0: 7374 6172 7473 2074 6865 2064 6572 6174  starts the derat
-000350e0: 696e 6720 616c 676f 7269 7468 6d20 666f  ing algorithm fo
-000350f0: 7220 7365 6c65 6374 6162 6c65 2066 7265  r selectable fre
-00035100: 7175 656e 6379 2031 2061 7420 6d69 6e69  quency 1 at mini
-00035110: 6d75 6d20 7375 7070 6c79 2076 6f6c 7461  mum supply volta
-00035120: 6765 2220 6361 745f 6964 3d22 494e 5445  ge" cat_id="INTE
-00035130: 524e 414c 223e 0d0a 2020 2020 2020 2020  RNAL">..        
-00035140: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00035150: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00035160: 616e 673d 2265 6e5f 5553 223e 506f 7765  ang="en_US">Powe
-00035170: 7220 7374 6167 6520 6465 7261 7469 6e67  r stage derating
-00035180: 2074 656d 7065 7261 7475 7265 2074 6872   temperature thr
-00035190: 6573 686f 6c64 2031 3c2f 4c61 6265 6c3e  eshold 1</Label>
-000351a0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
-000351b0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
-000351c0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
-000351d0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
-000351e0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
-000351f0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
-00035200: 6464 7265 7373 3d22 3078 3037 3542 2220  ddress="0x075B" 
-00035210: 6474 7970 653d 2266 6c6f 6174 2220 6964  dtype="float" id
-00035220: 3d22 4452 565f 5052 4f54 5f44 4552 4154  ="DRV_PROT_DERAT
-00035230: 494e 475f 5445 4d50 5f54 4852 4553 484f  ING_TEMP_THRESHO
-00035240: 4c44 5f32 2220 756e 6974 733d 2241 2220  LD_2" units="A" 
-00035250: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
-00035260: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
-00035270: 3d22 5468 7265 7368 6f6c 6420 7465 6d70  ="Threshold temp
-00035280: 6572 6174 7572 6520 7468 6174 2073 7461  erature that sta
-00035290: 7274 7320 7468 6520 6465 7261 7469 6e67  rts the derating
-000352a0: 2061 6c67 6f72 6974 686d 2066 6f72 2073   algorithm for s
-000352b0: 656c 6563 7461 626c 6520 6672 6571 7565  electable freque
-000352c0: 6e63 7920 3220 6174 206d 696e 696d 756d  ncy 2 at minimum
-000352d0: 2073 7570 706c 7920 766f 6c74 6167 6522   supply voltage"
-000352e0: 2063 6174 5f69 643d 2249 4e54 4552 4e41   cat_id="INTERNA
-000352f0: 4c22 3e0d 0a20 2020 2020 2020 2020 203c  L">..          <
-00035300: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00035310: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-00035320: 3d22 656e 5f55 5322 3e50 6f77 6572 2073  ="en_US">Power s
-00035330: 7461 6765 2064 6572 6174 696e 6720 7465  tage derating te
-00035340: 6d70 6572 6174 7572 6520 7468 7265 7368  mperature thresh
-00035350: 6f6c 6420 323c 2f4c 6162 656c 3e0d 0a20  old 2</Label>.. 
-00035360: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
-00035370: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
-00035380: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
-00035390: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
-000353a0: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
-000353b0: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
-000353c0: 6573 733d 2230 7830 3735 4322 2064 7479  ess="0x075C" dty
-000353d0: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
-000353e0: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
-000353f0: 5f54 454d 505f 5448 5245 5348 4f4c 445f  _TEMP_THRESHOLD_
-00035400: 3322 2075 6e69 7473 3d22 4122 2073 7562  3" units="A" sub
-00035410: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
-00035420: 2243 4f4e 4649 4722 2064 6573 633d 2254  "CONFIG" desc="T
-00035430: 6872 6573 686f 6c64 2074 656d 7065 7261  hreshold tempera
-00035440: 7475 7265 2074 6861 7420 7374 6172 7473  ture that starts
-00035450: 2074 6865 2064 6572 6174 696e 6720 616c   the derating al
-00035460: 676f 7269 7468 6d20 666f 7220 7365 6c65  gorithm for sele
-00035470: 6374 6162 6c65 2066 7265 7175 656e 6379  ctable frequency
-00035480: 2033 2061 7420 6d69 6e69 6d75 6d20 7375   3 at minimum su
-00035490: 7070 6c79 2076 6f6c 7461 6765 2220 6361  pply voltage" ca
-000354a0: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
-000354b0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-000354c0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-000354d0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-000354e0: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
-000354f0: 6520 6465 7261 7469 6e67 2074 656d 7065  e derating tempe
-00035500: 7261 7475 7265 2074 6872 6573 686f 6c64  rature threshold
-00035510: 2033 3c2f 4c61 6265 6c3e 0d0a 2020 2020   3</Label>..    
-00035520: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00035530: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-00035540: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-00035550: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-00035560: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-00035570: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
-00035580: 3d22 3078 3037 3544 2220 6474 7970 653d  ="0x075D" dtype=
-00035590: 2266 6c6f 6174 2220 6964 3d22 4452 565f  "float" id="DRV_
-000355a0: 5052 4f54 5f44 4552 4154 494e 475f 5445  PROT_DERATING_TE
-000355b0: 4d50 5f54 4852 4553 484f 4c44 5f34 2220  MP_THRESHOLD_4" 
-000355c0: 756e 6974 733d 2241 2220 7375 626e 6f64  units="A" subnod
-000355d0: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-000355e0: 4e46 4947 2220 6465 7363 3d22 5468 7265  NFIG" desc="Thre
-000355f0: 7368 6f6c 6420 7465 6d70 6572 6174 7572  shold temperatur
-00035600: 6520 7468 6174 2073 7461 7274 7320 7468  e that starts th
-00035610: 6520 6465 7261 7469 6e67 2061 6c67 6f72  e derating algor
-00035620: 6974 686d 2066 6f72 2073 656c 6563 7461  ithm for selecta
-00035630: 626c 6520 6672 6571 7565 6e63 7920 3420  ble frequency 4 
-00035640: 6174 206d 696e 696d 756d 2073 7570 706c  at minimum suppl
-00035650: 7920 766f 6c74 6167 6522 2063 6174 5f69  y voltage" cat_i
-00035660: 643d 2249 4e54 4552 4e41 4c22 3e0d 0a20  d="INTERNAL">.. 
-00035670: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
-00035680: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00035690: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-000356a0: 5322 3e50 6f77 6572 2073 7461 6765 2064  S">Power stage d
-000356b0: 6572 6174 696e 6720 7465 6d70 6572 6174  erating temperat
-000356c0: 7572 6520 7468 7265 7368 6f6c 6420 343c  ure threshold 4<
-000356d0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-000356e0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
-000356f0: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
-00035700: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
-00035710: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
-00035720: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
-00035730: 4d5f 4857 2220 6164 6472 6573 733d 2230  M_HW" address="0
-00035740: 7830 3736 3022 2064 7479 7065 3d22 7531  x0760" dtype="u1
-00035750: 3622 2069 643d 2244 5256 5f50 524f 545f  6" id="DRV_PROT_
-00035760: 5448 4952 445f 5445 4d50 5f54 5950 4522  THIRD_TEMP_TYPE"
-00035770: 2075 6e69 7473 3d22 2d22 2073 7562 6e6f   units="-" subno
-00035780: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00035790: 4f4e 4649 4722 2064 6573 633d 2249 6e64  ONFIG" desc="Ind
-000357a0: 6963 6174 6573 2074 6865 2074 656d 7065  icates the tempe
-000357b0: 7261 7475 7265 2073 656e 736f 7220 7573  rature sensor us
-000357c0: 6564 2066 6f72 2070 7269 6d61 7279 2074  ed for primary t
-000357d0: 656d 7065 7261 7475 7265 2072 6561 6469  emperature readi
-000357e0: 6e67 7320 6f66 2074 6865 2070 6f77 6572  ngs of the power
-000357f0: 2073 7461 6765 2e22 2063 6174 5f69 643d   stage." cat_id=
-00035800: 2249 4e54 4552 4e41 4c22 3e0d 0a20 2020  "INTERNAL">..   
-00035810: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00035820: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
-00035830: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00035840: 3e50 6f77 6572 2073 7461 6765 2074 656d  >Power stage tem
-00035850: 702e 2073 656e 736f 7220 3320 7479 7065  p. sensor 3 type
-00035860: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00035870: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00035880: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-00035890: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
-000358a0: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
-000358b0: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
-000358c0: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
-000358d0: 3078 3037 3631 2220 6474 7970 653d 2275  0x0761" dtype="u
-000358e0: 3332 2220 6964 3d22 4452 565f 5052 4f54  32" id="DRV_PROT
-000358f0: 5f54 4849 5244 5f54 454d 505f 5245 5322  _THIRD_TEMP_RES"
-00035900: 2075 6e69 7473 3d22 cea9 2220 7375 626e   units=".." subn
-00035910: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
-00035920: 434f 4e46 4947 2220 6465 7363 3d22 4e54  CONFIG" desc="NT
-00035930: 433a 2052 6573 6973 7461 6e63 6520 7661  C: Resistance va
-00035940: 6c75 6520 666f 7220 3235 20c2 ba43 2069  lue for 25 ..C i
-00035950: 6e20 6f68 6d73 2623 3133 3b26 2331 303b  n ohms&#13;&#10;
-00035960: 5054 433a 2052 6573 6973 7461 6e63 6520  PTC: Resistance 
-00035970: 7661 6c75 6520 696e 206f 686d 7320 7768  value in ohms wh
-00035980: 6572 6520 7468 6520 6f76 6572 2d74 656d  ere the over-tem
-00035990: 7065 7261 7475 7265 206d 7573 7420 6265  perature must be
-000359a0: 2064 6574 6563 7465 6426 2331 333b 2623   detected&#13;&#
-000359b0: 3130 3b4f 7468 6572 733a 204e 6f74 2075  10;Others: Not u
-000359c0: 7365 6422 2063 6174 5f69 643d 2249 4e54  sed" cat_id="INT
-000359d0: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-000359e0: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-000359f0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00035a00: 6c61 6e67 3d22 656e 5f55 5322 3e50 6f77  lang="en_US">Pow
-00035a10: 6572 2073 7461 6765 2074 656d 702e 2073  er stage temp. s
-00035a20: 656e 736f 7220 3320 7265 7369 7374 616e  ensor 3 resistan
-00035a30: 6365 3c2f 4c61 6265 6c3e 0d0a 2020 2020  ce</Label>..    
-00035a40: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00035a50: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
-00035a60: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
-00035a70: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
-00035a80: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
-00035a90: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
-00035aa0: 3d22 3078 3037 3632 2220 6474 7970 653d  ="0x0762" dtype=
-00035ab0: 2275 3136 2220 6964 3d22 4452 565f 5052  "u16" id="DRV_PR
-00035ac0: 4f54 5f54 4849 5244 5f54 454d 505f 4232  OT_THIRD_TEMP_B2
-00035ad0: 3538 3522 2075 6e69 7473 3d22 c2ba 4b22  585" units="..K"
-00035ae0: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
-00035af0: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
-00035b00: 633d 224e 5443 3a20 4228 3235 2f38 3529  c="NTC: B(25/85)
-00035b10: 2070 6172 616d 6574 6572 2066 726f 6d20   parameter from 
-00035b20: 6461 7461 7368 6565 7426 2331 333b 2623  datasheet&#13;&#
-00035b30: 3130 3b4f 7468 6572 733a 204e 6f74 2075  10;Others: Not u
-00035b40: 7365 6422 2063 6174 5f69 643d 2249 4e54  sed" cat_id="INT
-00035b50: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00035b60: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00035b70: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00035b80: 6c61 6e67 3d22 656e 5f55 5322 3e50 6f77  lang="en_US">Pow
-00035b90: 6572 2073 7461 6765 2074 656d 702e 2073  er stage temp. s
-00035ba0: 656e 736f 7220 3320 ceb2 3c2f 4c61 6265  ensor 3 ..</Labe
-00035bb0: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
-00035bc0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00035bd0: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
-00035be0: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
-00035bf0: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
-00035c00: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
-00035c10: 2061 6464 7265 7373 3d22 3078 3037 3633   address="0x0763
-00035c20: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
-00035c30: 3d22 4452 565f 5052 4f54 5f54 4849 5244  ="DRV_PROT_THIRD
-00035c40: 5f54 454d 505f 4558 545f 5245 5322 2075  _TEMP_EXT_RES" u
-00035c50: 6e69 7473 3d22 cea9 2220 7375 626e 6f64  nits=".." subnod
-00035c60: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
-00035c70: 4e46 4947 2220 6465 7363 3d22 4e54 4320  NFIG" desc="NTC 
-00035c80: 2661 6d70 3b61 6d70 3b20 5054 433a 2052  &amp;amp; PTC: R
-00035c90: 6573 6973 7461 6e63 6520 7661 6c75 6520  esistance value 
-00035ca0: 696e 206f 686d 7320 636f 6e6e 6563 7465  in ohms connecte
-00035cb0: 6420 746f 2073 656e 736f 7220 666f 7220  d to sensor for 
-00035cc0: 6d61 6b69 6e67 2074 6865 2076 6f6c 7461  making the volta
-00035cd0: 6765 2064 6976 6964 6572 2623 3133 3b26  ge divider&#13;&
-00035ce0: 2331 303b 4f74 6865 723a 204e 6f74 2075  #10;Other: Not u
-00035cf0: 7365 6422 2063 6174 5f69 643d 2249 4e54  sed" cat_id="INT
-00035d00: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
-00035d10: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00035d20: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00035d30: 6c61 6e67 3d22 656e 5f55 5322 3e50 6f77  lang="en_US">Pow
-00035d40: 6572 2073 7461 6765 2074 656d 702e 2073  er stage temp. s
-00035d50: 656e 736f 7220 3320 6578 742e 2072 6573  ensor 3 ext. res
-00035d60: 6973 7461 6e63 653c 2f4c 6162 656c 3e0d  istance</Label>.
-00035d70: 0a20 2020 2020 2020 2020 203c 2f4c 6162  .          </Lab
-00035d80: 656c 733e 0d0a 2020 2020 2020 2020 3c2f  els>..        </
-00035d90: 5265 6769 7374 6572 3e0d 0a20 2020 2020  Register>..     
-00035da0: 2020 203c 5265 6769 7374 6572 2061 6363     <Register acc
-00035db0: 6573 733d 2272 2220 6164 6472 6573 735f  ess="r" address_
-00035dc0: 7479 7065 3d22 4e56 4d5f 4857 2220 6164  type="NVM_HW" ad
-00035dd0: 6472 6573 733d 2230 7830 3736 3422 2064  dress="0x0764" d
-00035de0: 7479 7065 3d22 666c 6f61 7422 2069 643d  type="float" id=
-00035df0: 2244 5256 5f50 524f 545f 5448 4952 445f  "DRV_PROT_THIRD_
-00035e00: 5445 4d50 5f47 4149 4e22 2075 6e69 7473  TEMP_GAIN" units
-00035e10: 3d22 c2ba 4320 2f20 5622 2073 7562 6e6f  ="..C / V" subno
-00035e20: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00035e30: 4f4e 4649 4722 2064 6573 633d 224c 696e  ONFIG" desc="Lin
-00035e40: 6561 7220 766f 6c74 6167 6520 7365 6e73  ear voltage sens
-00035e50: 6f72 3a20 4761 696e 206f 6620 7468 6520  or: Gain of the 
-00035e60: 7365 6e73 6f72 2623 3133 3b26 2331 303b  sensor&#13;&#10;
-00035e70: 4f74 6865 7273 3a20 4e6f 7420 7573 6564  Others: Not used
-00035e80: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
-00035e90: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
-00035ea0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00035eb0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00035ec0: 673d 2265 6e5f 5553 223e 506f 7765 7220  g="en_US">Power 
-00035ed0: 7374 6167 6520 7465 6d70 2e20 7365 6e73  stage temp. sens
-00035ee0: 6f72 2033 2067 6169 6e3c 2f4c 6162 656c  or 3 gain</Label
-00035ef0: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
-00035f00: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00035f10: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
-00035f20: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
-00035f30: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
-00035f40: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
-00035f50: 6164 6472 6573 733d 2230 7830 3736 3522  address="0x0765"
-00035f60: 2064 7479 7065 3d22 666c 6f61 7422 2069   dtype="float" i
-00035f70: 643d 2244 5256 5f50 524f 545f 5448 4952  d="DRV_PROT_THIR
-00035f80: 445f 5445 4d50 5f4f 4646 5345 5422 2075  D_TEMP_OFFSET" u
-00035f90: 6e69 7473 3d22 c2ba 4322 2073 7562 6e6f  nits="..C" subno
-00035fa0: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
-00035fb0: 4f4e 4649 4722 2064 6573 633d 224e 5443  ONFIG" desc="NTC
-00035fc0: 2026 616d 703b 616d 703b 2050 5443 3a20   &amp;amp; PTC: 
-00035fd0: 4e6f 7420 7573 6564 2623 3133 3b26 2331  Not used&#13;&#1
-00035fe0: 303b 4c69 6e65 6172 2073 656e 736f 723a  0;Linear sensor:
-00035ff0: 204f 6666 7365 7420 6f66 2074 6865 2073   Offset of the s
-00036000: 656e 736f 7222 2063 6174 5f69 643d 2249  ensor" cat_id="I
-00036010: 4e54 4552 4e41 4c22 3e0d 0a20 2020 2020  NTERNAL">..     
-00036020: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00036030: 2020 2020 2020 2020 2020 203c 4c61 6265             <Labe
-00036040: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e50  l lang="en_US">P
-00036050: 6f77 6572 2073 7461 6765 2074 656d 702e  ower stage temp.
-00036060: 2073 656e 736f 7220 3320 6f66 6673 6574   sensor 3 offset
-00036070: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00036080: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-00036090: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
-000360a0: 723e 0d0a 2020 2020 2020 3c2f 5265 6769  r>..      </Regi
-000360b0: 7374 6572 733e 0d0a 2020 2020 3c2f 4465  sters>..    </De
-000360c0: 7669 6365 3e0d 0a20 2020 203c 4572 726f  vice>..    <Erro
-000360d0: 7273 3e0d 0a20 2020 2020 203c 4572 726f  rs>..      <Erro
-000360e0: 7220 6964 3d22 3078 3030 3030 3332 3830  r id="0x00003280
-000360f0: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-00036100: 653d 2250 6f77 6572 2073 7461 6765 2220  e="Power stage" 
-00036110: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00036120: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00036130: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00036140: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00036150: 6e5f 5553 223e 5354 4f20 4163 7469 7665  n_US">STO Active
-00036160: 2061 6e64 2050 6f77 6572 2073 7461 6765   and Power stage
-00036170: 2069 7320 7368 7574 646f 776e 3c2f 4c61   is shutdown</La
-00036180: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
-00036190: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
-000361a0: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
-000361b0: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
-000361c0: 3232 3830 2220 6166 6665 6374 6564 5f6d  2280" affected_m
-000361d0: 6f64 756c 653d 2250 6f77 6572 2073 7461  odule="Power sta
-000361e0: 6765 2220 6572 726f 725f 7479 7065 3d22  ge" error_type="
-000361f0: 6379 636c 6963 223e 0d0a 2020 2020 2020  cyclic">..      
-00036200: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00036210: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00036220: 673d 2265 6e5f 5553 223e 4857 206f 7665  g="en_US">HW ove
-00036230: 7220 6375 7272 656e 743c 2f4c 6162 656c  r current</Label
-00036240: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00036250: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-00036260: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-00036270: 6f72 2069 643d 2230 7830 3030 3032 3238  or id="0x0000228
-00036280: 3822 2061 6666 6563 7465 645f 6d6f 6475  8" affected_modu
-00036290: 6c65 3d22 506f 7765 7220 7374 6167 6522  le="Power stage"
-000362a0: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-000362b0: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-000362c0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-000362d0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-000362e0: 656e 5f55 5322 3e55 7365 7220 4932 5420  en_US">User I2T 
-000362f0: 6c69 6d69 7420 6465 7465 6374 6564 2077  limit detected w
-00036300: 6974 686f 7574 2063 7572 7265 6e74 2063  ithout current c
-00036310: 6f6e 7472 6f6c 3c2f 4c61 6265 6c3e 0d0a  ontrol</Label>..
-00036320: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00036330: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00036340: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00036350: 6964 3d22 3078 3030 3030 3332 3930 2220  id="0x00003290" 
-00036360: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00036370: 2250 6f77 6572 2073 7461 6765 2220 6572  "Power stage" er
-00036380: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
-00036390: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
-000363a0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-000363b0: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-000363c0: 5553 223e 496e 7075 7420 7374 6167 6520  US">Input stage 
-000363d0: 7072 6f62 6c65 6d3c 2f4c 6162 656c 3e0d  problem</Label>.
-000363e0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-000363f0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-00036400: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-00036410: 2069 643d 2230 7830 3030 3033 3231 3022   id="0x00003210"
-00036420: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-00036430: 3d22 506f 7765 7220 7374 6167 6522 2065  ="Power stage" e
-00036440: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
-00036450: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
-00036460: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-00036470: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-00036480: 5f55 5322 3e48 5720 4f76 6572 2d76 6f6c  _US">HW Over-vol
-00036490: 7461 6765 2064 6574 6563 7465 643c 2f4c  tage detected</L
-000364a0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
-000364b0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-000364c0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
-000364d0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
-000364e0: 3033 3231 3122 2061 6666 6563 7465 645f  03211" affected_
-000364f0: 6d6f 6475 6c65 3d22 506f 7765 7220 7374  module="Power st
-00036500: 6167 6522 2065 7272 6f72 5f74 7970 653d  age" error_type=
-00036510: 2263 7963 6c69 6322 3e0d 0a20 2020 2020  "cyclic">..     
-00036520: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00036530: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
-00036540: 6e67 3d22 656e 5f55 5322 3e46 5720 4f76  ng="en_US">FW Ov
-00036550: 6572 2d76 6f6c 7461 6765 2064 6574 6563  er-voltage detec
-00036560: 7465 643c 2f4c 6162 656c 3e0d 0a20 2020  ted</Label>..   
-00036570: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00036580: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00036590: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-000365a0: 2230 7830 3030 3033 3232 3122 2061 6666  "0x00003221" aff
-000365b0: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
-000365c0: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
-000365d0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
-000365e0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
-000365f0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-00036600: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00036610: 3e46 5720 556e 6465 722d 766f 6c74 6167  >FW Under-voltag
-00036620: 6520 6465 7465 6374 6564 3c2f 4c61 6265  e detected</Labe
-00036630: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00036640: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00036650: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00036660: 726f 7220 6964 3d22 3078 3030 3030 3433  ror id="0x000043
-00036670: 3030 2220 6166 6665 6374 6564 5f6d 6f64  00" affected_mod
-00036680: 756c 653d 2250 6f77 6572 2073 7461 6765  ule="Power stage
-00036690: 2220 6572 726f 725f 7479 7065 3d22 6379  " error_type="cy
-000366a0: 636c 6963 223e 0d0a 2020 2020 2020 2020  clic">..        
-000366b0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-000366c0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-000366d0: 2265 6e5f 5553 223e 4f76 6572 2d54 656d  "en_US">Over-Tem
-000366e0: 7065 7261 7475 7265 2064 6574 6563 7465  perature detecte
-000366f0: 6420 2869 6e74 6572 6e61 6c20 6472 6976  d (internal driv
-00036700: 6520 6c69 6d69 7429 2e3c 2f4c 6162 656c  e limit).</Label
-00036710: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00036720: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-00036730: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-00036740: 6f72 2069 643d 2230 7830 3030 3034 3330  or id="0x0000430
-00036750: 3122 2061 6666 6563 7465 645f 6d6f 6475  1" affected_modu
-00036760: 6c65 3d22 506f 7765 7220 7374 6167 6522  le="Power stage"
-00036770: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-00036780: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-00036790: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-000367a0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-000367b0: 656e 5f55 5322 3e55 6e64 6572 2d54 656d  en_US">Under-Tem
-000367c0: 7065 7261 7475 7265 2064 6574 6563 7465  perature detecte
-000367d0: 6420 2869 6e74 6572 6e61 6c20 6472 6976  d (internal driv
-000367e0: 6520 6c69 6d69 7429 3c2f 4c61 6265 6c3e  e limit)</Label>
-000367f0: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
-00036800: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
-00036810: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
-00036820: 7220 6964 3d22 3078 3030 3030 3434 3030  r id="0x00004400
-00036830: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-00036840: 653d 2250 6f77 6572 2073 7461 6765 2220  e="Power stage" 
-00036850: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00036860: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00036870: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00036880: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00036890: 6e5f 5553 223e 4d6f 746f 7220 4f76 6572  n_US">Motor Over
-000368a0: 2054 656d 7065 7261 7475 7265 2065 7272   Temperature err
-000368b0: 6f72 3c2f 4c61 6265 6c3e 0d0a 2020 2020  or</Label>..    
-000368c0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
-000368d0: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
-000368e0: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
-000368f0: 3078 3030 3030 3733 3830 2220 6166 6665  0x00007380" affe
-00036900: 6374 6564 5f6d 6f64 756c 653d 2246 6565  cted_module="Fee
-00036910: 6462 6163 6b22 2065 7272 6f72 5f74 7970  dback" error_typ
-00036920: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
-00036930: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00036940: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00036950: 6c61 6e67 3d22 656e 5f55 5322 3e54 6f6f  lang="en_US">Too
-00036960: 206d 616e 7920 6572 726f 7220 6269 7473   many error bits
-00036970: 206f 7220 696e 7661 6c69 6420 706f 7369   or invalid posi
-00036980: 7469 6f6e 2066 6c61 6773 2064 6574 6563  tion flags detec
-00036990: 7465 6420 696e 2061 6273 6f6c 7574 6520  ted in absolute 
-000369a0: 656e 636f 6465 723c 2f4c 6162 656c 3e0d  encoder</Label>.
-000369b0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-000369c0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-000369d0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-000369e0: 2069 643d 2230 7830 3030 3037 3338 3222   id="0x00007382"
-000369f0: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-00036a00: 3d22 4665 6564 6261 636b 2220 6572 726f  ="Feedback" erro
-00036a10: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
-00036a20: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
-00036a30: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
-00036a40: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-00036a50: 223e 546f 6f20 6d61 6e79 2069 6e63 6f72  ">Too many incor
-00036a60: 7265 6374 2043 5243 2063 6865 636b 7320  rect CRC checks 
-00036a70: 696e 2061 6273 6f6c 7574 6520 656e 636f  in absolute enco
-00036a80: 6465 7220 7265 6164 696e 6773 3c2f 4c61  der readings</La
-00036a90: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
-00036aa0: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
-00036ab0: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
-00036ac0: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
-00036ad0: 3733 3835 2220 6166 6665 6374 6564 5f6d  7385" affected_m
-00036ae0: 6f64 756c 653d 2243 6f6e 7472 6f6c 204c  odule="Control L
-00036af0: 6f6f 7073 2220 6572 726f 725f 7479 7065  oops" error_type
-00036b00: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
-00036b10: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00036b20: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00036b30: 616e 673d 2265 6e5f 5553 223e 506f 7369  ang="en_US">Posi
-00036b40: 7469 6f6e 206f 7574 206f 6620 6c69 6d69  tion out of limi
-00036b50: 7473 206f 7574 206f 6620 706f 7369 7469  ts out of positi
-00036b60: 6f6e 206d 6f64 6573 3c2f 4c61 6265 6c3e  on modes</Label>
-00036b70: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
-00036b80: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
-00036b90: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
-00036ba0: 7220 6964 3d22 3078 3030 3030 3733 3836  r id="0x00007386
-00036bb0: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-00036bc0: 653d 2243 6f6e 7472 6f6c 204c 6f6f 7073  e="Control Loops
-00036bd0: 2220 6572 726f 725f 7479 7065 3d22 6379  " error_type="cy
-00036be0: 636c 6963 223e 0d0a 2020 2020 2020 2020  clic">..        
-00036bf0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00036c00: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-00036c10: 2265 6e5f 5553 223e 5665 6c6f 6369 7479  "en_US">Velocity
-00036c20: 206f 7574 206f 6620 6c69 6d69 7473 206f   out of limits o
-00036c30: 7574 206f 6620 7665 6c6f 6369 7479 206f  ut of velocity o
-00036c40: 7220 706f 7369 7469 6f6e 206d 6f64 6573  r position modes
-00036c50: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00036c60: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00036c70: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
-00036c80: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
-00036c90: 3030 3030 3733 3837 2220 6166 6665 6374  00007387" affect
-00036ca0: 6564 5f6d 6f64 756c 653d 2243 6f6e 7472  ed_module="Contr
-00036cb0: 6f6c 204c 6f6f 7073 2220 6572 726f 725f  ol Loops" error_
-00036cc0: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
-00036cd0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
-00036ce0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00036cf0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-00036d00: 506f 7369 7469 6f6e 2066 6f6c 6c6f 7769  Position followi
-00036d10: 6e67 2065 7272 6f72 3c2f 4c61 6265 6c3e  ng error</Label>
-00036d20: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
-00036d30: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
-00036d40: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
-00036d50: 7220 6964 3d22 3078 3036 3031 3030 3030  r id="0x06010000
-00036d60: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-00036d70: 653d 2252 6567 6973 7465 7220 6469 6374  e="Register dict
-00036d80: 696f 6e61 7279 2220 6572 726f 725f 7479  ionary" error_ty
-00036d90: 7065 3d22 636f 6e66 6967 7572 6174 696f  pe="configuratio
-00036da0: 6e22 3e0d 0a20 2020 2020 2020 203c 4c61  n">..        <La
-00036db0: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-00036dc0: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-00036dd0: 5f55 5322 3e49 6e63 6f72 7265 6374 2061  _US">Incorrect a
-00036de0: 6363 6573 7320 7479 7065 3c2f 4c61 6265  ccess type</Labe
-00036df0: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00036e00: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00036e10: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00036e20: 726f 7220 6964 3d22 3078 3036 3032 3030  ror id="0x060200
-00036e30: 3030 2220 6166 6665 6374 6564 5f6d 6f64  00" affected_mod
-00036e40: 756c 653d 2252 6567 6973 7465 7220 6469  ule="Register di
-00036e50: 6374 696f 6e61 7279 2220 6572 726f 725f  ctionary" error_
-00036e60: 7479 7065 3d22 636f 6e66 6967 7572 6174  type="configurat
-00036e70: 696f 6e22 3e0d 0a20 2020 2020 2020 203c  ion">..        <
-00036e80: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00036e90: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00036ea0: 656e 5f55 5322 3e4f 626a 6563 7420 646f  en_US">Object do
-00036eb0: 6573 6e27 7420 6578 6973 743c 2f4c 6162  esn't exist</Lab
-00036ec0: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
-00036ed0: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
-00036ee0: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
-00036ef0: 7272 6f72 2069 643d 2230 7830 3630 3430  rror id="0x06040
-00036f00: 3034 3122 2061 6666 6563 7465 645f 6d6f  041" affected_mo
-00036f10: 6475 6c65 3d22 5265 6769 7374 6572 2064  dule="Register d
-00036f20: 6963 7469 6f6e 6172 7922 2065 7272 6f72  ictionary" error
-00036f30: 5f74 7970 653d 2263 6f6e 6669 6775 7261  _type="configura
-00036f40: 7469 6f6e 223e 0d0a 2020 2020 2020 2020  tion">..        
-00036f50: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00036f60: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-00036f70: 2265 6e5f 5553 223e 4f62 6a65 6374 2069  "en_US">Object i
-00036f80: 736e 2774 2050 444f 206d 6170 7061 626c  sn't PDO mappabl
-00036f90: 6520 6173 2072 6571 7565 7374 6564 3c2f  e as requested</
-00036fa0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-00036fb0: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
-00036fc0: 203c 2f45 7272 6f72 3e0d 0a20 2020 2020   </Error>..     
-00036fd0: 203c 4572 726f 7220 6964 3d22 3078 3036   <Error id="0x06
-00036fe0: 3037 3030 3130 2220 6166 6665 6374 6564  070010" affected
-00036ff0: 5f6d 6f64 756c 653d 2252 6567 6973 7465  _module="Registe
-00037000: 7220 6469 6374 696f 6e61 7279 2220 6572  r dictionary" er
-00037010: 726f 725f 7479 7065 3d22 636f 6e66 6967  ror_type="config
-00037020: 7572 6174 696f 6e22 3e0d 0a20 2020 2020  uration">..     
-00037030: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00037040: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
-00037050: 6e67 3d22 656e 5f55 5322 3e49 6e63 6f72  ng="en_US">Incor
-00037060: 7265 6374 2073 7065 6369 6669 6564 206f  rect specified o
-00037070: 626a 6563 7420 7369 7a65 3c2f 4c61 6265  bject size</Labe
-00037080: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00037090: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-000370a0: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-000370b0: 726f 7220 6964 3d22 3078 3036 3039 3030  ror id="0x060900
-000370c0: 3131 2220 6166 6665 6374 6564 5f6d 6f64  11" affected_mod
-000370d0: 756c 653d 2252 6567 6973 7465 7220 6469  ule="Register di
-000370e0: 6374 696f 6e61 7279 2220 6572 726f 725f  ctionary" error_
-000370f0: 7479 7065 3d22 636f 6e66 6967 7572 6174  type="configurat
-00037100: 696f 6e22 3e0d 0a20 2020 2020 2020 203c  ion">..        <
-00037110: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00037120: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00037130: 656e 5f55 5322 3e53 7562 2d49 6e64 6578  en_US">Sub-Index
-00037140: 2064 6f65 7320 6e6f 7420 6578 6973 743c   does not exist<
-00037150: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-00037160: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-00037170: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
-00037180: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
-00037190: 3630 4130 3030 3022 2061 6666 6563 7465  60A0000" affecte
-000371a0: 645f 6d6f 6475 6c65 3d22 5265 6769 7374  d_module="Regist
-000371b0: 6572 2064 6963 7469 6f6e 6172 7922 2065  er dictionary" e
-000371c0: 7272 6f72 5f74 7970 653d 2263 6f6e 6669  rror_type="confi
-000371d0: 6775 7261 7469 6f6e 223e 0d0a 2020 2020  guration">..    
-000371e0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-000371f0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00037200: 616e 673d 2265 6e5f 5553 223e 556e 7375  ang="en_US">Unsu
-00037210: 7070 6f72 7465 6420 7661 6c75 6520 696e  pported value in
-00037220: 7472 6f64 7563 6564 2069 6e20 7265 6769  troduced in regi
-00037230: 7374 6572 3c2f 4c61 6265 6c3e 0d0a 2020  ster</Label>..  
-00037240: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00037250: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
-00037260: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
-00037270: 3d22 3078 3038 3030 3030 3030 2220 6166  ="0x08000000" af
-00037280: 6665 6374 6564 5f6d 6f64 756c 653d 2252  fected_module="R
-00037290: 6567 6973 7465 7220 6469 6374 696f 6e61  egister dictiona
-000372a0: 7279 2220 6572 726f 725f 7479 7065 3d22  ry" error_type="
-000372b0: 636f 6e66 6967 7572 6174 696f 6e22 3e0d  configuration">.
-000372c0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
-000372d0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-000372e0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-000372f0: 3e52 6561 6420 2f20 5772 6974 6520 6f70  >Read / Write op
-00037300: 6572 6174 696f 6e20 6e6f 7420 6578 6563  eration not exec
-00037310: 7574 6564 3c2f 4c61 6265 6c3e 0d0a 2020  uted</Label>..  
-00037320: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-00037330: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
-00037340: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
-00037350: 3d22 3078 3030 3030 3332 3331 2220 6166  ="0x00003231" af
-00037360: 6665 6374 6564 5f6d 6f64 756c 653d 2250  fected_module="P
-00037370: 6f77 6572 2073 7461 6765 2220 6572 726f  ower stage" erro
-00037380: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
-00037390: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
-000373a0: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
-000373b0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-000373c0: 223e 5573 6572 204f 7665 722d 766f 6c74  ">User Over-volt
-000373d0: 6167 6520 6465 7465 6374 6564 3c2f 4c61  age detected</La
-000373e0: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
-000373f0: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
-00037400: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
-00037410: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
-00037420: 3332 3431 2220 6166 6665 6374 6564 5f6d  3241" affected_m
-00037430: 6f64 756c 653d 2250 6f77 6572 2073 7461  odule="Power sta
-00037440: 6765 2220 6572 726f 725f 7479 7065 3d22  ge" error_type="
-00037450: 6379 636c 6963 223e 0d0a 2020 2020 2020  cyclic">..      
-00037460: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00037470: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00037480: 673d 2265 6e5f 5553 223e 5573 6572 2055  g="en_US">User U
-00037490: 6e64 6572 2d76 6f6c 7461 6765 2064 6574  nder-voltage det
-000374a0: 6563 7465 643c 2f4c 6162 656c 3e0d 0a20  ected</Label>.. 
-000374b0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-000374c0: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
-000374d0: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
-000374e0: 643d 2230 7830 3030 3034 3330 3322 2061  d="0x00004303" a
-000374f0: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
-00037500: 506f 7765 7220 7374 6167 6522 2065 7272  Power stage" err
-00037510: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00037520: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00037530: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00037540: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00037550: 5322 3e4f 7665 722d 7465 6d70 6572 6174  S">Over-temperat
-00037560: 7572 6520 6465 7465 6374 6564 2028 7573  ure detected (us
-00037570: 6572 206c 696d 6974 293c 2f4c 6162 656c  er limit)</Label
-00037580: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00037590: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-000375a0: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-000375b0: 6f72 2069 643d 2230 7830 3030 3034 3330  or id="0x0000430
-000375c0: 3422 2061 6666 6563 7465 645f 6d6f 6475  4" affected_modu
-000375d0: 6c65 3d22 506f 7765 7220 7374 6167 6522  le="Power stage"
-000375e0: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-000375f0: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-00037600: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00037610: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00037620: 656e 5f55 5322 3e55 6e64 6572 2d74 656d  en_US">Under-tem
-00037630: 7065 7261 7475 7265 2064 6574 6563 7465  perature detecte
-00037640: 6420 2875 7365 7220 6c69 6d69 7429 3c2f  d (user limit)</
-00037650: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
-00037660: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
-00037670: 203c 2f45 7272 6f72 3e0d 0a20 2020 2020   </Error>..     
-00037680: 203c 4572 726f 7220 6964 3d22 3078 3030   <Error id="0x00
-00037690: 3030 3435 3030 2220 6166 6665 6374 6564  004500" affected
-000376a0: 5f6d 6f64 756c 653d 2250 6f77 6572 2073  _module="Power s
-000376b0: 7461 6765 2220 6572 726f 725f 7479 7065  tage" error_type
-000376c0: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
-000376d0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-000376e0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-000376f0: 616e 673d 2265 6e5f 5553 223e 4578 7465  ang="en_US">Exte
-00037700: 726e 616c 2065 7272 6f72 3c2f 4c61 6265  rnal error</Labe
-00037710: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00037720: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00037730: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00037740: 726f 7220 6964 3d22 3078 3030 3030 3733  ror id="0x000073
-00037750: 3930 2220 6166 6665 6374 6564 5f6d 6f64  90" affected_mod
-00037760: 756c 653d 2250 726f 6669 6c65 7222 2065  ule="Profiler" e
-00037770: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
-00037780: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
-00037790: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-000377a0: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-000377b0: 5f55 5322 3e49 6e74 6572 706f 6c61 7469  _US">Interpolati
-000377c0: 6f6e 2074 696d 6520 6973 2074 6f20 736d  on time is to sm
-000377d0: 616c 6c20 7768 656e 2050 5654 2069 7320  all when PVT is 
-000377e0: 656e 6162 6c65 643c 2f4c 6162 656c 3e0d  enabled</Label>.
-000377f0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-00037800: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-00037810: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-00037820: 2069 643d 2230 7830 3030 3033 3238 3122   id="0x00003281"
-00037830: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-00037840: 3d22 506f 7765 7220 7374 6167 6522 2065  ="Power stage" e
-00037850: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
-00037860: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
-00037870: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-00037880: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-00037890: 5f55 5322 3e41 626e 6f72 6d61 6c20 5354  _US">Abnormal ST
-000378a0: 4f20 5375 7070 6c79 2e20 556e 6974 2063  O Supply. Unit c
-000378b0: 6f75 6c64 2062 6520 6461 6d61 6765 643c  ould be damaged<
-000378c0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-000378d0: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-000378e0: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
-000378f0: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
-00037900: 3030 3033 3238 3222 2061 6666 6563 7465  0003282" affecte
-00037910: 645f 6d6f 6475 6c65 3d22 506f 7765 7220  d_module="Power 
-00037920: 7374 6167 6522 2065 7272 6f72 5f74 7970  stage" error_typ
-00037930: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
-00037940: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00037950: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00037960: 6c61 6e67 3d22 656e 5f55 5322 3e41 626e  lang="en_US">Abn
-00037970: 6f72 6d61 6c20 5354 4f2e 2053 544f 3120  ormal STO. STO1 
-00037980: 616e 6420 5354 4f32 2069 6e70 7574 7320  and STO2 inputs 
-00037990: 6469 6666 6572 6564 206d 6f72 6520 7468  differed more th
-000379a0: 616e 206c 6174 6368 696e 6720 7469 6d65  an latching time
-000379b0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-000379c0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-000379d0: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
-000379e0: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
-000379f0: 3030 3030 3733 3730 2220 6166 6665 6374  00007370" affect
-00037a00: 6564 5f6d 6f64 756c 653d 2246 6565 6462  ed_module="Feedb
-00037a10: 6163 6b73 2220 6572 726f 725f 7479 7065  acks" error_type
-00037a20: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
-00037a30: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00037a40: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00037a50: 616e 673d 2265 6e5f 5553 223e 4861 6c6c  ang="en_US">Hall
-00037a60: 7320 7365 7175 656e 6365 2065 7272 6f72  s sequence error
-00037a70: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00037a80: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00037a90: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
-00037aa0: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
-00037ab0: 3030 3030 3733 3731 2220 6166 6665 6374  00007371" affect
-00037ac0: 6564 5f6d 6f64 756c 653d 2246 6565 6462  ed_module="Feedb
-00037ad0: 6163 6b73 2220 6572 726f 725f 7479 7065  acks" error_type
-00037ae0: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
-00037af0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00037b00: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00037b10: 616e 673d 2265 6e5f 5553 223e 4861 6c6c  ang="en_US">Hall
-00037b20: 7320 636f 6d62 696e 6174 696f 6e20 6572  s combination er
-00037b30: 726f 723c 2f4c 6162 656c 3e0d 0a20 2020  ror</Label>..   
-00037b40: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00037b50: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00037b60: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00037b70: 2230 7830 3030 3037 3337 3222 2061 6666  "0x00007372" aff
-00037b80: 6563 7465 645f 6d6f 6475 6c65 3d22 4665  ected_module="Fe
-00037b90: 6564 6261 636b 7322 2065 7272 6f72 5f74  edbacks" error_t
-00037ba0: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
-00037bb0: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00037bc0: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-00037bd0: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e46  l lang="en_US">F
-00037be0: 6565 6462 6163 6b20 7275 6e61 7761 7920  eedback runaway 
-00037bf0: 6572 726f 723c 2f4c 6162 656c 3e0d 0a20  error</Label>.. 
-00037c00: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00037c10: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
-00037c20: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
-00037c30: 643d 2230 7830 3030 3032 3238 3922 2061  d="0x00002289" a
-00037c40: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
-00037c50: 506f 7765 7220 7374 6167 6522 2065 7272  Power stage" err
-00037c60: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00037c70: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00037c80: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00037c90: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00037ca0: 5322 3e4f 7665 7220 6375 7272 656e 7420  S">Over current 
-00037cb0: 7769 7468 6f75 7420 6375 7272 656e 7420  without current 
-00037cc0: 636f 6e74 726f 6c3c 2f4c 6162 656c 3e0d  control</Label>.
-00037cd0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-00037ce0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-00037cf0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-00037d00: 2069 643d 2230 7830 3030 3037 3339 3122   id="0x00007391"
-00037d10: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-00037d20: 3d22 5072 6f66 696c 6572 2220 6572 726f  ="Profiler" erro
-00037d30: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
-00037d40: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
-00037d50: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
-00037d60: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-00037d70: 223e 5072 6f66 696c 6572 2070 6172 616d  ">Profiler param
-00037d80: 6574 6572 7320 6e6f 7420 7661 6c69 642e  eters not valid.
-00037d90: 2054 6865 7920 7368 6f75 6c64 2061 6c6c   They should all
-00037da0: 2068 6176 6520 706f 7369 7469 7665 2076   have positive v
-00037db0: 616c 7565 732e 3c2f 4c61 6265 6c3e 0d0a  alues.</Label>..
-00037dc0: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00037dd0: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00037de0: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00037df0: 6964 3d22 3078 3030 3030 3030 3030 2220  id="0x00000000" 
-00037e00: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00037e10: 2244 7269 7665 2220 6572 726f 725f 7479  "Drive" error_ty
-00037e20: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
-00037e30: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-00037e40: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-00037e50: 206c 616e 673d 2265 6e5f 5553 223e 4e6f   lang="en_US">No
-00037e60: 2065 7272 6f72 3c2f 4c61 6265 6c3e 0d0a   error</Label>..
-00037e70: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00037e80: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00037e90: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00037ea0: 6964 3d22 3078 3030 3030 3733 3831 2220  id="0x00007381" 
-00037eb0: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00037ec0: 2246 6565 6462 6163 6b73 2220 6572 726f  "Feedbacks" erro
-00037ed0: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
-00037ee0: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
-00037ef0: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
-00037f00: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-00037f10: 223e 4269 5353 2d43 2077 6172 6e69 6e67  ">BiSS-C warning
-00037f20: 2062 6974 2061 6374 6976 653c 2f4c 6162   bit active</Lab
-00037f30: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
-00037f40: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
-00037f50: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
-00037f60: 7272 6f72 2069 643d 2230 7830 3030 3031  rror id="0x00001
-00037f70: 3030 3122 2061 6666 6563 7465 645f 6d6f  001" affected_mo
-00037f80: 6475 6c65 3d22 436f 6d6d 756e 6963 6174  dule="Communicat
-00037f90: 696f 6e73 2220 6572 726f 725f 7479 7065  ions" error_type
-00037fa0: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
-00037fb0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-00037fc0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00037fd0: 616e 673d 2265 6e5f 5553 223e 436f 6d6d  ang="en_US">Comm
-00037fe0: 756e 6963 6174 696f 6e73 2077 6174 6368  unications watch
-00037ff0: 646f 6720 6572 726f 723c 2f4c 6162 656c  dog error</Label
-00038000: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00038010: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-00038020: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-00038030: 6f72 2069 643d 2230 7830 3030 3037 3338  or id="0x0000738
-00038040: 3822 2061 6666 6563 7465 645f 6d6f 6475  8" affected_modu
-00038050: 6c65 3d22 436f 6e74 726f 6c20 6c6f 6f70  le="Control loop
-00038060: 7322 2065 7272 6f72 5f74 7970 653d 2263  s" error_type="c
-00038070: 7963 6c69 6322 3e0d 0a20 2020 2020 2020  yclic">..       
-00038080: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
-00038090: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-000380a0: 3d22 656e 5f55 5322 3e56 656c 6f63 6974  ="en_US">Velocit
-000380b0: 7920 666f 6c6c 6f77 696e 6720 6572 726f  y following erro
-000380c0: 723c 2f4c 6162 656c 3e0d 0a20 2020 2020  r</Label>..     
-000380d0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
-000380e0: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
-000380f0: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
-00038100: 7830 3030 3037 3338 3922 2061 6666 6563  x00007389" affec
-00038110: 7465 645f 6d6f 6475 6c65 3d22 436f 6d6d  ted_module="Comm
-00038120: 7574 6174 696f 6e22 2065 7272 6f72 5f74  utation" error_t
-00038130: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
-00038140: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00038150: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-00038160: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e41  l lang="en_US">A
-00038170: 6e67 6c65 2069 6e74 6567 7269 7479 2063  ngle integrity c
-00038180: 6865 636b 2031 2065 7272 6f72 3c2f 4c61  heck 1 error</La
-00038190: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
-000381a0: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
-000381b0: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
-000381c0: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
-000381d0: 3733 3841 2220 6166 6665 6374 6564 5f6d  738A" affected_m
-000381e0: 6f64 756c 653d 2243 6f6d 6d75 7461 7469  odule="Commutati
-000381f0: 6f6e 2220 6572 726f 725f 7479 7065 3d22  on" error_type="
-00038200: 6379 636c 6963 223e 0d0a 2020 2020 2020  cyclic">..      
-00038210: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
-00038220: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
-00038230: 673d 2265 6e5f 5553 223e 416e 676c 6520  g="en_US">Angle 
-00038240: 696e 7465 6772 6974 7920 6368 6563 6b20  integrity check 
-00038250: 3220 6572 726f 723c 2f4c 6162 656c 3e0d  2 error</Label>.
-00038260: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-00038270: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-00038280: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-00038290: 2069 643d 2230 7830 3030 3037 3338 4222   id="0x0000738B"
-000382a0: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-000382b0: 3d22 436f 6d6d 7574 6174 696f 6e22 2065  ="Commutation" e
-000382c0: 7272 6f72 5f74 7970 653d 2263 6f6e 6669  rror_type="confi
-000382d0: 6775 7261 7469 6f6e 223e 0d0a 2020 2020  guration">..    
-000382e0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
-000382f0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
-00038300: 616e 673d 2265 6e5f 5553 223e 5472 6170  ang="en_US">Trap
-00038310: 657a 6f69 6461 6c20 636f 6d6d 7574 6174  ezoidal commutat
-00038320: 696f 6e20 7769 7468 6f75 7420 6469 6769  ion without digi
-00038330: 7461 6c20 6861 6c6c 7320 6e6f 7420 616c  tal halls not al
-00038340: 6c6f 7765 642e 2052 6576 6965 7720 636f  lowed. Review co
-00038350: 6d6d 7574 6174 696f 6e20 7365 6e73 6f72  mmutation sensor
-00038360: 2063 6f6e 6669 6775 7261 7469 6f6e 2061   configuration a
-00038370: 6e64 2070 6861 7369 6e67 3c2f 4c61 6265  nd phasing</Labe
-00038380: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00038390: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-000383a0: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-000383b0: 726f 7220 6964 3d22 3078 3030 3030 3232  ror id="0x000022
-000383c0: 3841 2220 6166 6665 6374 6564 5f6d 6f64  8A" affected_mod
-000383d0: 756c 653d 2250 6f77 6572 2073 7461 6765  ule="Power stage
-000383e0: 2220 6572 726f 725f 7479 7065 3d22 6379  " error_type="cy
-000383f0: 636c 6963 223e 0d0a 2020 2020 2020 2020  clic">..        
-00038400: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
-00038410: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
-00038420: 2265 6e5f 5553 223e 5379 7374 656d 2049  "en_US">System I
-00038430: 3254 2064 6574 6563 7465 643c 2f4c 6162  2T detected</Lab
-00038440: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
-00038450: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
-00038460: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
-00038470: 7272 6f72 2069 643d 2230 7830 3030 3037  rror id="0x00007
-00038480: 3338 3322 2061 6666 6563 7465 645f 6d6f  383" affected_mo
-00038490: 6475 6c65 3d22 4665 6564 6261 636b 7322  dule="Feedbacks"
-000384a0: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-000384b0: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-000384c0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-000384d0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-000384e0: 656e 5f55 5322 3e4d 6178 696d 756d 2061  en_US">Maximum a
-000384f0: 6273 6f6c 7574 6520 7665 6c6f 6369 7479  bsolute velocity
-00038500: 2065 7863 6565 6465 643c 2f4c 6162 656c   exceeded</Label
-00038510: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00038520: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-00038530: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-00038540: 6f72 2069 643d 2230 7830 3030 3037 3338  or id="0x0000738
-00038550: 4422 2061 6666 6563 7465 645f 6d6f 6475  D" affected_modu
-00038560: 6c65 3d22 4665 6564 6261 636b 7322 2065  le="Feedbacks" e
-00038570: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
-00038580: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
-00038590: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
-000385a0: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
-000385b0: 5f55 5322 3e49 6e63 7265 6d65 6e74 616c  _US">Incremental
-000385c0: 2065 6e63 6f64 6572 2031 2069 6e64 6578   encoder 1 index
-000385d0: 2070 756c 7365 2069 6e74 6567 7269 7479   pulse integrity
-000385e0: 2063 6865 636b 2066 6169 6c3c 2f4c 6162   check fail</Lab
-000385f0: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
-00038600: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
-00038610: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
-00038620: 7272 6f72 2069 643d 2230 7830 3030 3037  rror id="0x00007
-00038630: 3338 4522 2061 6666 6563 7465 645f 6d6f  38E" affected_mo
-00038640: 6475 6c65 3d22 4665 6564 6261 636b 7322  dule="Feedbacks"
-00038650: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-00038660: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-00038670: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00038680: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00038690: 656e 5f55 5322 3e49 6e63 7265 6d65 6e74  en_US">Increment
-000386a0: 616c 2065 6e63 6f64 6572 2032 2069 6e64  al encoder 2 ind
-000386b0: 6578 2070 756c 7365 2069 6e74 6567 7269  ex pulse integri
-000386c0: 7479 2063 6865 636b 2066 6169 6c3c 2f4c  ty check fail</L
-000386d0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
-000386e0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-000386f0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
-00038700: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
-00038710: 3032 3238 3122 2061 6666 6563 7465 645f  02281" affected_
-00038720: 6d6f 6475 6c65 3d22 506f 7765 7220 7374  module="Power st
-00038730: 6167 6522 2065 7272 6f72 5f74 7970 653d  age" error_type=
-00038740: 2263 7963 6c69 6322 3e0d 0a20 2020 2020  "cyclic">..     
-00038750: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
-00038760: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
-00038770: 6e67 3d22 656e 5f55 5322 3e46 6175 6c74  ng="en_US">Fault
-00038780: 2064 6574 6563 7465 6420 696e 2074 6865   detected in the
-00038790: 2070 6f77 6572 2073 7461 6765 2067 6174   power stage gat
-000387a0: 6520 6472 6976 6572 3c2f 4c61 6265 6c3e  e driver</Label>
-000387b0: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
-000387c0: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
-000387d0: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
-000387e0: 7220 6964 3d22 3078 3030 3030 3232 3931  r id="0x00002291
-000387f0: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-00038800: 653d 2250 6f77 6572 2073 7461 6765 2220  e="Power stage" 
-00038810: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00038820: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00038830: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00038840: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00038850: 6e5f 5553 223e 4f70 656e 2070 6861 7365  n_US">Open phase
-00038860: 2064 6574 6563 7465 643c 2f4c 6162 656c   detected</Label
-00038870: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
-00038880: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
-00038890: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
-000388a0: 6f72 2069 643d 2230 7830 3030 3032 3239  or id="0x0000229
-000388b0: 3022 2061 6666 6563 7465 645f 6d6f 6475  0" affected_modu
-000388c0: 6c65 3d22 506f 7765 7220 7374 6167 6522  le="Power stage"
-000388d0: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
-000388e0: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
-000388f0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
-00038900: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
-00038910: 656e 5f55 5322 3e4e 6f6e 2d7a 6572 6f20  en_US">Non-zero 
-00038920: 746f 7461 6c20 7068 6173 6520 6375 7272  total phase curr
-00038930: 656e 743c 2f4c 6162 656c 3e0d 0a20 2020  ent</Label>..   
-00038940: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038950: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038960: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038970: 2230 7830 3030 3032 3238 3222 2061 6666  "0x00002282" aff
-00038980: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038990: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-000389a0: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-000389b0: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-000389c0: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-000389d0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-000389e0: 5322 3e43 7572 7265 6e74 2041 2073 656e  S">Current A sen
-000389f0: 7369 6e67 2072 6561 6368 6564 2075 7070  sing reached upp
-00038a00: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038a10: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038a20: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038a30: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038a40: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038a50: 2230 7830 3030 3032 3238 3322 2061 6666  "0x00002283" aff
-00038a60: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038a70: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-00038a80: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00038a90: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00038aa0: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00038ab0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00038ac0: 5322 3e43 7572 7265 6e74 2041 2073 656e  S">Current A sen
-00038ad0: 7369 6e67 2072 6561 6368 6564 206c 6f77  sing reached low
-00038ae0: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038af0: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038b00: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038b10: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038b20: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038b30: 2230 7830 3030 3032 3238 3422 2061 6666  "0x00002284" aff
-00038b40: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038b50: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-00038b60: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00038b70: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00038b80: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00038b90: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00038ba0: 5322 3e43 7572 7265 6e74 2042 2073 656e  S">Current B sen
-00038bb0: 7369 6e67 2072 6561 6368 6564 2075 7070  sing reached upp
-00038bc0: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038bd0: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038be0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038bf0: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038c00: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038c10: 2230 7830 3030 3032 3238 3522 2061 6666  "0x00002285" aff
-00038c20: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038c30: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-00038c40: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00038c50: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00038c60: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00038c70: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00038c80: 5322 3e43 7572 7265 6e74 2042 2073 656e  S">Current B sen
-00038c90: 7369 6e67 2072 6561 6368 6564 206c 6f77  sing reached low
-00038ca0: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038cb0: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038cc0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038cd0: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038ce0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038cf0: 2230 7830 3030 3032 3238 3622 2061 6666  "0x00002286" aff
-00038d00: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038d10: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-00038d20: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00038d30: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00038d40: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00038d50: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00038d60: 5322 3e43 7572 7265 6e74 2043 2073 656e  S">Current C sen
-00038d70: 7369 6e67 2072 6561 6368 6564 2075 7070  sing reached upp
-00038d80: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038d90: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038da0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038db0: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038dc0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038dd0: 2230 7830 3030 3032 3238 3722 2061 6666  "0x00002287" aff
-00038de0: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
-00038df0: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
-00038e00: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00038e10: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00038e20: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00038e30: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00038e40: 5322 3e43 7572 7265 6e74 2043 2073 656e  S">Current C sen
-00038e50: 7369 6e67 2072 6561 6368 6564 206c 6f77  sing reached low
-00038e60: 6572 2073 6174 7572 6174 696f 6e20 6c69  er saturation li
-00038e70: 6d69 743c 2f4c 6162 656c 3e0d 0a20 2020  mit</Label>..   
-00038e80: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-00038e90: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-00038ea0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-00038eb0: 2230 7830 3030 3037 3338 4622 2061 6666  "0x0000738F" aff
-00038ec0: 6563 7465 645f 6d6f 6475 6c65 3d22 4665  ected_module="Fe
-00038ed0: 6564 6261 636b 7322 2065 7272 6f72 5f74  edbacks" error_t
-00038ee0: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
-00038ef0: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00038f00: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-00038f10: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e44  l lang="en_US">D
-00038f20: 6967 6974 616c 2065 6e63 6f64 6572 2069  igital encoder i
-00038f30: 6e64 6578 2070 756c 7365 2069 6e74 6567  ndex pulse integ
-00038f40: 7269 7479 2063 6865 636b 2063 616c 6962  rity check calib
-00038f50: 7261 7469 6f6e 2065 7272 6f72 3c2f 4c61  ration error</La
-00038f60: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
-00038f70: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
-00038f80: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
-00038f90: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
-00038fa0: 3233 3032 2220 6166 6665 6374 6564 5f6d  2302" affected_m
-00038fb0: 6f64 756c 653d 2242 7261 6b65 2220 6572  odule="Brake" er
-00038fc0: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
-00038fd0: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
-00038fe0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00038ff0: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-00039000: 5553 223e 4272 616b 6520 6375 7272 656e  US">Brake curren
-00039010: 7420 7472 6163 6b69 6e67 2065 7272 6f72  t tracking error
-00039020: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
-00039030: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
-00039040: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
-00039050: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
-00039060: 3030 3030 3232 3842 2220 6166 6665 6374  0000228B" affect
-00039070: 6564 5f6d 6f64 756c 653d 2250 6f77 6572  ed_module="Power
-00039080: 2073 7461 6765 2220 6572 726f 725f 7479   stage" error_ty
-00039090: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
-000390a0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
-000390b0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
-000390c0: 206c 616e 673d 2265 6e5f 5553 223e 4375   lang="en_US">Cu
-000390d0: 7272 656e 7420 6465 7261 7469 6e67 2077  rrent derating w
-000390e0: 6974 686f 7574 2063 7572 7265 6e74 2063  ithout current c
-000390f0: 6f6e 7472 6f6c 3c2f 4c61 6265 6c3e 0d0a  ontrol</Label>..
-00039100: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00039110: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00039120: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00039130: 6964 3d22 3078 3030 3030 3433 3035 2220  id="0x00004305" 
-00039140: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00039150: 2250 6f77 6572 2073 7461 6765 2220 6572  "Power stage" er
-00039160: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
-00039170: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
-00039180: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00039190: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-000391a0: 5553 223e 5772 6f6e 6720 4144 4320 6d65  US">Wrong ADC me
-000391b0: 6173 7572 656d 656e 7473 2064 6574 6563  asurements detec
-000391c0: 7469 6f6e 3c2f 4c61 6265 6c3e 0d0a 2020  tion</Label>..  
-000391d0: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
-000391e0: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
-000391f0: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
-00039200: 3d22 3078 3030 3030 3433 3036 2220 6166  ="0x00004306" af
-00039210: 6665 6374 6564 5f6d 6f64 756c 653d 2250  fected_module="P
-00039220: 6f77 6572 2073 7461 6765 2220 6572 726f  ower stage" erro
-00039230: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
-00039240: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
-00039250: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
-00039260: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
-00039270: 223e 5573 6572 206f 7665 7220 7465 6d70  ">User over temp
-00039280: 6572 6174 7572 6520 7761 726e 696e 6720  erature warning 
-00039290: 7468 7265 7368 6f6c 6420 6578 6365 6564  threshold exceed
-000392a0: 6564 2e3c 2f4c 6162 656c 3e0d 0a20 2020  ed.</Label>..   
-000392b0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-000392c0: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-000392d0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-000392e0: 2230 7830 3030 3034 3330 3722 2061 6666  "0x00004307" aff
-000392f0: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
-00039300: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
-00039310: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
-00039320: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
-00039330: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-00039340: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00039350: 3e55 7365 7220 756e 6465 7220 7465 6d70  >User under temp
-00039360: 6572 6174 7572 6520 7761 726e 696e 6720  erature warning 
-00039370: 7468 7265 7368 6f6c 6420 6578 6365 6564  threshold exceed
-00039380: 6564 2e3c 2f4c 6162 656c 3e0d 0a20 2020  ed.</Label>..   
-00039390: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
-000393a0: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
-000393b0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
-000393c0: 2230 7830 3030 3033 3231 3222 2061 6666  "0x00003212" aff
-000393d0: 6563 7465 645f 6d6f 6475 6c65 3d22 5375  ected_module="Su
-000393e0: 7065 7276 6973 6f72 2220 6572 726f 725f  pervisor" error_
-000393f0: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
-00039400: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
-00039410: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
-00039420: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
-00039430: 4761 7465 2076 6f6c 7461 6765 206f 7574  Gate voltage out
-00039440: 206f 6620 6c69 6d69 7473 3c2f 4c61 6265   of limits</Labe
-00039450: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00039460: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00039470: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00039480: 726f 7220 6964 3d22 3078 3030 3030 3435  ror id="0x000045
-00039490: 3031 2220 6166 6665 6374 6564 5f6d 6f64  01" affected_mod
-000394a0: 756c 653d 2249 6e70 7574 7322 2065 7272  ule="Inputs" err
-000394b0: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-000394c0: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-000394d0: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-000394e0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-000394f0: 5322 3e4c 6f61 6420 6365 6c6c 2068 6561  S">Load cell hea
-00039500: 6c74 6820 7369 676e 616c 2065 7272 6f72  lth signal error
-00039510: 2064 6574 6563 7465 642e 3c2f 4c61 6265   detected.</Labe
-00039520: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00039530: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00039540: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00039550: 726f 7220 6964 3d22 3078 3030 3030 3435  ror id="0x000045
-00039560: 3032 2220 6166 6665 6374 6564 5f6d 6f64  02" affected_mod
-00039570: 756c 653d 2249 6e70 7574 7322 2065 7272  ule="Inputs" err
-00039580: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00039590: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-000395a0: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-000395b0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-000395c0: 5322 3e4c 6f61 6420 6365 6c6c 2061 6e61  S">Load cell ana
-000395d0: 6c6f 6720 696e 7075 7420 6f75 7420 6f66  log input out of
-000395e0: 2072 616e 6765 3c2f 4c61 6265 6c3e 0d0a   range</Label>..
-000395f0: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00039600: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00039610: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00039620: 6964 3d22 3078 3030 3030 3733 3933 2220  id="0x00007393" 
-00039630: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00039640: 2243 6f6e 7472 6f6c 206c 6f6f 7073 2220  "Control loops" 
-00039650: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00039660: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00039670: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00039680: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00039690: 6e5f 5553 223e 4375 7272 656e 7420 6469  n_US">Current di
-000396a0: 7265 6374 2066 6f6c 6c6f 7769 6e67 2065  rect following e
-000396b0: 7272 6f72 2064 6574 6563 7465 643c 2f4c  rror detected</L
-000396c0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
-000396d0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-000396e0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
-000396f0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
-00039700: 3037 3339 3222 2061 6666 6563 7465 645f  07392" affected_
-00039710: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
-00039720: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
-00039730: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
-00039740: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00039750: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00039760: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
-00039770: 7265 6e74 2071 7561 6472 6174 7572 6520  rent quadrature 
-00039780: 666f 6c6c 6f77 696e 6720 6572 726f 7220  following error 
-00039790: 6465 7465 6374 6564 3c2f 4c61 6265 6c3e  detected</Label>
-000397a0: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
-000397b0: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
-000397c0: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
-000397d0: 7220 6964 3d22 3078 3030 3030 3733 3834  r id="0x00007384
-000397e0: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
-000397f0: 653d 2246 6565 6462 6163 6b73 2220 6572  e="Feedbacks" er
-00039800: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
-00039810: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
-00039820: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00039830: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-00039840: 5553 223e 4162 736f 6c75 7465 2065 6e63  US">Absolute enc
-00039850: 6f64 6572 2065 7272 6f72 2062 6974 2061  oder error bit a
-00039860: 6374 6976 6520 7769 7468 6f75 7420 6578  ctive without ex
-00039870: 6365 6564 696e 6720 6572 726f 7220 746f  ceeding error to
-00039880: 6c65 7261 6e63 653c 2f4c 6162 656c 3e0d  lerance</Label>.
-00039890: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-000398a0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-000398b0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
-000398c0: 2069 643d 2230 7830 3530 3430 3030 3022   id="0x05040000"
-000398d0: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
-000398e0: 3d22 436f 6d6d 756e 6963 6174 696f 6e73  ="Communications
-000398f0: 2220 6572 726f 725f 7479 7065 3d22 636f  " error_type="co
-00039900: 6e66 6967 7572 6174 696f 6e22 3e0d 0a20  nfiguration">.. 
-00039910: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
-00039920: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
-00039930: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e43  l lang="en_US">C
-00039940: 4f4d 2d4b 4954 2054 696d 656f 7574 2e20  OM-KIT Timeout. 
-00039950: 434f 5245 2064 6576 6963 6520 6973 206e  CORE device is n
-00039960: 6f74 2070 726f 7065 726c 7920 636f 6e6e  ot properly conn
-00039970: 6563 7465 643c 2f4c 6162 656c 3e0d 0a20  ected</Label>.. 
-00039980: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00039990: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
-000399a0: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
-000399b0: 643d 2230 7830 3030 3046 4634 3222 2061  d="0x0000FF42" a
-000399c0: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
-000399d0: 436f 6d6d 756e 6963 6174 696f 6e73 2220  Communications" 
-000399e0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-000399f0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00039a00: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00039a10: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00039a20: 6e5f 5553 223e 4574 6865 7243 4154 2063  n_US">EtherCAT c
-00039a30: 6162 6c65 2069 7320 6469 7363 6f6e 6e65  able is disconne
-00039a40: 6374 6564 2064 7572 696e 6720 6f70 6572  cted during oper
-00039a50: 6174 696f 6e3c 2f4c 6162 656c 3e0d 0a20  ation</Label>.. 
-00039a60: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
-00039a70: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
-00039a80: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
-00039a90: 643d 2230 7830 3030 3038 3133 3022 2061  d="0x00008130" a
-00039aa0: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
-00039ab0: 436f 6d6d 756e 6963 6174 696f 6e73 2220  Communications" 
-00039ac0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00039ad0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00039ae0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00039af0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-00039b00: 6e5f 5553 223e 4c69 6665 6775 6172 6420  n_US">Lifeguard 
-00039b10: 6572 726f 7220 6f72 2068 6561 7274 6265  error or heartbe
-00039b20: 6174 2065 7272 6f72 2069 6e20 4341 4e4f  at error in CANO
-00039b30: 7065 6e20 636f 6d6d 756e 6963 6174 696f  pen communicatio
-00039b40: 6e3c 2f4c 6162 656c 3e0d 0a20 2020 2020  n</Label>..     
-00039b50: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
-00039b60: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
-00039b70: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
-00039b80: 7830 3030 3046 4634 3322 2061 6666 6563  x0000FF43" affec
-00039b90: 7465 645f 6d6f 6475 6c65 3d22 436f 6d6d  ted_module="Comm
-00039ba0: 756e 6963 6174 696f 6e22 2065 7272 6f72  unication" error
-00039bb0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
-00039bc0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
-00039bd0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
-00039be0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
-00039bf0: 3e43 7963 6c69 6320 7469 6d65 6f75 7420  >Cyclic timeout 
-00039c00: 4574 6865 7263 6174 2050 444f 206c 6966  Ethercat PDO lif
-00039c10: 6567 7561 7264 3c2f 4c61 6265 6c3e 0d0a  eguard</Label>..
-00039c20: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00039c30: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00039c40: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00039c50: 6964 3d22 3078 3030 3030 3733 3934 2220  id="0x00007394" 
-00039c60: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00039c70: 2251 7569 636b 2073 746f 7022 2065 7272  "Quick stop" err
-00039c80: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
-00039c90: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
-00039ca0: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
-00039cb0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
-00039cc0: 5322 3e45 6d65 7267 656e 6379 2070 6f73  S">Emergency pos
-00039cd0: 6974 696f 6e20 7365 742d 706f 696e 7420  ition set-point 
-00039ce0: 6e6f 7420 636f 6e66 6967 7572 6564 2e3c  not configured.<
-00039cf0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
-00039d00: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
-00039d10: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
-00039d20: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
-00039d30: 3030 3046 3031 3122 2061 6666 6563 7465  000F011" affecte
-00039d40: 645f 6d6f 6475 6c65 3d22 434f 434f 2220  d_module="COCO" 
-00039d50: 6572 726f 725f 7479 7065 3d22 636f 6e66  error_type="conf
-00039d60: 6967 7572 6174 696f 6e22 3e0d 0a20 2020  iguration">..   
-00039d70: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
-00039d80: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
-00039d90: 6c61 6e67 3d22 656e 5f55 5322 3e43 7963  lang="en_US">Cyc
-00039da0: 6c69 6320 6d6f 6465 206d 6170 7069 6e67  lic mode mapping
-00039db0: 2065 7272 6f72 3c2f 4c61 6265 6c3e 0d0a   error</Label>..
-00039dc0: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
-00039dd0: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
-00039de0: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
-00039df0: 6964 3d22 3078 3030 3030 3232 3843 2220  id="0x0000228C" 
-00039e00: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
-00039e10: 2250 6f77 6572 2073 7461 6765 2220 6572  "Power stage" er
-00039e20: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
-00039e30: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
-00039e40: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
-00039e50: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
-00039e60: 5553 223e 4375 7272 656e 7420 6361 6c69  US">Current cali
-00039e70: 6272 6174 696f 6e20 6572 726f 723c 2f4c  bration error</L
-00039e80: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
-00039e90: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
-00039ea0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
-00039eb0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
-00039ec0: 3037 3337 4522 2061 6666 6563 7465 645f  0737E" affected_
-00039ed0: 6d6f 6475 6c65 3d22 4665 6564 6261 636b  module="Feedback
-00039ee0: 7322 2065 7272 6f72 5f74 7970 653d 2263  s" error_type="c
-00039ef0: 7963 6c69 6322 3e0d 0a20 2020 2020 2020  yclic">..       
-00039f00: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
-00039f10: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
-00039f20: 3d22 656e 5f55 5322 3e41 6273 6f6c 7574  ="en_US">Absolut
-00039f30: 6520 656e 636f 6465 7220 3120 6469 7363  e encoder 1 disc
-00039f40: 6f6e 6e65 6374 696f 6e20 6f72 2066 7261  onnection or fra
-00039f50: 6d65 206f 7665 726c 6170 3c2f 4c61 6265  me overlap</Labe
-00039f60: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
-00039f70: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
-00039f80: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
-00039f90: 726f 7220 6964 3d22 3078 3030 3030 3733  ror id="0x000073
-00039fa0: 3746 2220 6166 6665 6374 6564 5f6d 6f64  7F" affected_mod
-00039fb0: 756c 653d 2246 6565 6462 6163 6b73 2220  ule="Feedbacks" 
-00039fc0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
-00039fd0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
-00039fe0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
-00039ff0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
-0003a000: 6e5f 5553 223e 4162 736f 6c75 7465 2065  n_US">Absolute e
-0003a010: 6e63 6f64 6572 2032 2064 6973 636f 6e6e  ncoder 2 disconn
-0003a020: 6563 7469 6f6e 206f 7220 6672 616d 6520  ection or frame 
-0003a030: 6f76 6572 6c61 703c 2f4c 6162 656c 3e0d  overlap</Label>.
-0003a040: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
-0003a050: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
-0003a060: 723e 0d0a 2020 2020 3c2f 4572 726f 7273  r>..    </Errors
-0003a070: 3e0d 0a20 203c 2f42 6f64 793e 0d0a 2020  >..  </Body>..  
-0003a080: 3c44 7269 7665 496d 6167 6520 656e 636f  <DriveImage enco
-0003a090: 6469 6e67 3d22 7873 3a62 6173 6536 3442  ding="xs:base64B
-0003a0a0: 696e 6172 7922 3e0d 0a20 2020 2069 5642  inary">..    iVB
-0003a0b0: 4f52 7730 4b47 676f 4141 4141 4e53 5568  ORw0KGgoAAAANSUh
-0003a0c0: 4555 6741 4141 4d67 4141 4144 4943 4159  EUgAAAMgAAADICAY
-0003a0d0: 4141 4143 7457 4b36 6541 4141 4141 584e  AAACtWK6eAAAAAXN
-0003a0e0: 5352 3049 4172 7334 6336 5141 4141 4152  SR0IArs4c6QAAAAR
-0003a0f0: 6e51 5531 4241 4143 786a 7776 3859 5155  nQU1BAACxjwv8YQU
-0003a100: 4141 4141 4a63 4568 5a63 7741 4144 734d  AAAAJcEhZcwAADsM
-0003a110: 4141 4137 4441 6364 7671 4751 4141 4663  AAA7DAcdvqGQAAFc
-0003a120: 5a53 5552 4256 4868 6537 5630 486f 4231  ZSURBVHhe7V0HoB1
-0003a130: 4631 5a37 5a33 6474 6554 6538 6b49 5130  F1Z7Z3dteTe8kIQ0
-0003a140: 496b 4143 6874 7841 3651 5a71 5141 4649  IkAChtxA6QZqQAFI
-0003a150: 6943 4b69 4149 6943 6950 3070 4152 5542  iCKiAIiCiP0pARUB
-0003a160: 4651 4552 4538 5564 4535 5366 3836 692b  FQERE8UdE5Sf86i+
-0003a170: 3968 3935 4454 3267 7870 7666 6b35 6456  9h95DT2gxpvfk5dV
-0003a180: 6264 6e66 6d50 2b66 4d7a 4f37 652b 2b35  bdnfmP+fMzO7e++5
-0003a190: 4c58 704b 5876 4276 5937 3932 6463 2b62  LXpKXvBvY792dc+b
-0003a1a0: 4d37 4d37 7337 4878 375a 7259 3946 694e  M7M7s7Hx7ZrY9FiN
-0003a1b0: 476a 4267 7859 7353 4945 534e 476a 4267  GjBgxYsSIESNGjBg
-0003a1c0: 7859 7353 4945 534e 476a 4267 7859 7353  xYsSIESNGjBgxYsS
-0003a1d0: 4945 534e 476a 4267 7859 7353 4945 534e  IESNGjBgxYsSIESN
-0003a1e0: 476a 4267 7859 7353 4945 534e 476a 4267  GjBgxYsSIESNGjBg
-0003a1f0: 7859 7353 4945 534e 476a 4267 7859 7353  xYsSIESNGjBgxYsS
-0003a200: 4945 534e 476a 4267 7859 7353 4945 534e  IESNGjBgxYsSIESN
-0003a210: 476a 4267 7859 7353 4945 534e 476a 4267  GjBgxYsSIESNGjBg
-0003a220: 7859 7353 4945 534e 476a 4267 7859 7353  xYsSIESNGjBgxYsS
-0003a230: 4945 534e 476a 4267 7859 7353 4945 534e  IESNGjBgxYsSIESN
-0003a240: 476a 4330 4772 6d57 4d72 5977 4a53 7837  GjC0GrmWMrYwJSx7
-0003a250: 7349 3277 3579 4c4f 5344 7663 4c44 596b  sI2w5yLOSDvcLDYk
-0003a260: 4279 7866 5034 6c39 3364 584b 4d43 6b46  ByxfP4l93dXKMCkF
-0003a270: 4d6b 4b32 4d76 5663 2f57 7063 5834 7475  MkK2MvVc/WpcX4tu
-0003a280: 6338 334f 6b6b 4c31 4232 6c4b 4946 736e  c83OkkL1B2lKIFsn
-0003a290: 592b 3562 774c 3331 3334 4473 664d 3336  Y+5bwL3134DsfM36
-0003a2a0: 7430 4e6c 6a64 444e 6967 6d78 466a 462f  t0NljdDNigmxFjF/
-0003a2b0: 392b 4e35 632b 6a65 4265 6941 4452 6968  9+N5c+jeBeiADRih
-0003a2c0: 494a 7255 7570 567a 486d 6678 6c6a 2f36  IJrUupVzHmfxlj/6
-0003a2d0: 314e 7a37 504a 336e 4b47 714d 3745 524e  1Nz7PJ3nKGqM7ERN
-0003a2e0: 6b4b 3243 5835 662f 7162 3976 4f4e 3445  kK2CX5f/qb9vON4E
-0003a2f0: 4c56 3348 4f6e 484c 6b43 4253 4269 6e78  LV3HOnHLkCBSBinx
-0003a300: 5a57 4f79 4b44 3137 4976 386d 6d54 7656  ZWOyKD17Iv8mmTvV
-0003a310: 5651 6f7a 7551 4579 514c 5969 4a4d 3263  VQozuQEyQLYiJM2c
-0003a320: 366a 654f 7a42 7a42 502f 6736 6165 6779  6jeOzBzBP/g6aegy
-0003a330: 3074 6855 7967 6a79 4755 6254 456e 394c  0thUygjyGUbTEn9L
-0003a340: 4231 4d69 6b2b 454f 3274 666b 6e63 3865  B1Mik+EO2tfknc8e
-0003a350: 6331 5554 4747 4673 644d 5547 3245 4361  c1UTGGFsdMUG2ECa
-0003a360: 736e 5648 7669 396f 6651 452f 2f46 6b53  snVHvi9ofQE//FkS
-0003a370: 7279 4e68 4a63 6968 4242 6761 546b 5265  ryNhJcihBBgaTkRe
-0003a380: 5939 4c2f 2f34 5a41 7676 3070 704d 6259  Y9L//4ZAvv0ppMbY
-0003a390: 7159 6f4a 304d 6162 4947 6661 2f56 3164  qYoJ0MabIGfa/V1d
-0003a3a0: 5046 4a7a 667a 7158 6351 5449 5956 4246  PFJzfzqXcQTIYVBF
-0003a3b0: 5568 7963 7451 7053 5149 4a6f 654a 6c41  UhyctQpSQIJoeJlA
-0003a3c0: 2f73 674d 4b51 4a49 626d 4d6a 6438 7347  /sgMKQJIbmMjd8sG
-0003a3d0: 774d 7872 5145 4750 7249 435a 4946 324b  wMxrQEGPrICZIF2K
-0003a3e0: 7678 662f 6f37 6159 7950 2b52 636e 6766  vxf/o7aYyP+Rcngf
-0003a3f0: 526d 7041 4870 7264 6a66 772b 4d70 7650  RmpAHprdjfw+MpvP
-0003a400: 725a 4a4e 4832 5652 5378 435a 6764 734c  rZJNH2VRSxCZgdsL
-0003a410: 6b65 7861 3376 746c 7a37 6a75 7a6e 7039  kexa3vtlz7juznp9
-0003a420: 3062 5479 4a33 7771 4943 644a 4647 4c66  0bTyJ3wqICdJFGLf
-0003a430: 716b 554d 7479 3771 5253 3759 6e64 756a  qkUMty7qRS7Ynduj
-0003a440: 4e49 5565 7844 654e 4b30 6576 4466 4554  NIUexDeNK0evDfET
-0003a450: 6556 734f 3836 3134 6265 6d71 5745 6d4a  eVsO8614bemqWEmJ
-0003a460: 734d 6351 4532 557a 6744 5438 2f6e 6667  sMcQE2UzgDT8/nfg
-0003a470: 4f39 4e34 724f 654d 4f64 5733 5473 5573  O9N4rOeMOdW3TsUs
-0003a480: 3665 576a 5747 6956 4838 6d68 3967 7a5a  6eWjWGiVH8mh9gzZ
-0003a490: 6743 6d78 6946 7066 6574 7a38 6350 7656  gCmxiFpfetz8cPvV
-0003a4a0: 3147 4d58 4639 3032 3245 474b 4362 4349  1GMXF9022EGKCbCI
-0003a4b0: 6d79 706c 4f38 2b72 4377 594c 3774 774d  myplO8+rCwYL7twM
-0003a4c0: 7878 6f44 4a30 7431 5964 2b52 4968 305a  xxoDJ0t1Yd+RIh0Z
-0003a4d0: 3732 4c6d 3167 6d70 786e 6d43 564d 4c50  72Lm1gmpxnmCVMLP
-0003a4e0: 2b6d 5151 304b 5957 4546 4531 672f 3633  +mQQ0KYWEFE1g/63
-0003a4f0: 446e 5276 6632 2f36 6b64 5a51 516f 3073  DnRvf2/6kdZQQo0s
-0003a500: 5245 3251 5441 4636 6a79 7338 6b70 384d  RE2QTAF6jys8kp8M
-0003a510: 6b2f 434b 4956 7176 4f75 776e 6b49 4555  k/CKIVqvOuwnkIEU
-0003a520: 4836 6f63 4a47 4161 7972 4530 5a64 534c  H6ocJGAayrE0ZdSL
-0003a530: 4735 6175 577a 6237 3934 6241 7062 796c  G5auWzb794bApbyl
-0003a540: 4c6a 4b35 4354 4a43 4e67 5a54 5748 7175  LjK5CTJCNgZTWHqu
-0003a550: 6650 4552 5938 685a 6f75 4633 4448 6f6f  fPERY8hZouF3DHoo
-0003a560: 2f30 3247 4e52 4777 6b4f 5149 6c59 6776  /02GNRGwkOQIlYgv
-0003a570: 794b 686e 5974 426b 5653 7049 6943 2b6f  yKhnYtBkVSpIiC+o
-0003a580: 4e43 5476 3536 3969 6264 4231 6967 6e51  NCTv569ibdB1ignQ
-0003a590: 4f66 4e39 316a 2f66 4d43 2f5a 3936 4e77  OfN91j/fMC/Z96Nw
-0003a5a0: 5877 5a43 714b 7569 6871 7363 472f 5468  XwZCqKuihqscG/Th
-0003a5b0: 5555 4456 3579 746c 3045 4552 4448 664f  UUDV5ytl0EERDHfO
-0003a5c0: 725a 4a4f 6f5a 4c46 4e42 536f 4b41 5571  rZJOoZLFNBSoKAUq
-0003a5d0: 4a39 2b48 6c42 3879 3276 7435 7677 5966  J9+HlB8y2vt5vwYf
-0003a5e0: 786c 6134 7551 4579 5154 6d44 5074 5939  xla4uQEyQTmDPtY9
-0003a5f0: 4f46 4a4c 6642 4a50 6843 5547 4844 4d51  OFJLfBJPhCUGHDMQ
-0003a600: 4779 4945 774f 6b69 3969 6771 4d4f 6443  GyIEwOki9igqMOdC
-0003a610: 5656 4371 4667 6232 7354 5564 4c74 7739  VVCqFgb2sTUdLtw9
-0003a620: 6c72 774f 5038 6c74 7656 4938 667a 3755  lrwOP8ltvVI8fz7U
-0003a630: 6d35 3156 696a 4531 4254 4a44 3159 4e64  m51VijE1BTJD1YNd
-0003a640: 3144 2f64 3070 484d 706e 4a65 2f7a 7a6c  1D/d0pHMpnJe/zzl
-0003a650: 5071 4835 6f4f 714d 4b67 6b36 4b42 704d  PqH5oOqMKgk6KBpM
-0003a660: 5547 6a45 5353 4e4c 4367 4152 5a64 5454  UGjESSNLCgARZdTT
-0003a670: 4967 3269 336e 6f6d 7277 4551 6a69 6c4a  Ig2i3nomrwEQjilJ
-0003a680: 314f 6f57 5376 6336 6c75 4f53 6a4d 5a2b  1OoWSvc6luOSjMZ+
-0003a690: 3847 5438 6876 476d 4943 5649 4765 4957  8GT8hvGmICVIGeIW
-0003a6a0: 7161 5a30 3745 5472 5862 6444 4c64 6754  qaZ07ETrXbdDLdgT
-0003a6b0: 5041 664e 7854 4e47 6455 6575 6843 514b  PAfNxTNGdUeuhCQK
-0003a6c0: 5446 4852 5967 4e46 7834 4d4e 5943 3269  TFHRYgNFx4MNYC2i
-0003a6d0: 3159 5562 3855 6144 6a53 7346 5143 7546  1YUb8UaDjSsFQCuF
-0003a6e0: 696b 5742 4c6b 6f32 5354 4e37 316b 494e  ikWBLko2STN71kIN
-0003a6f0: 5570 5154 316b 4c49 5a6b 6e39 7465 6661  UpQT1kLIZkn9tefa
-0003a700: 7635 7578 7936 6c70 6c6a 4e46 5a57 4672  v5uxy6lpljNFZWFr
-0003a710: 4730 426a 326e 356e 7070 6f62 4339 5543  G0Bj2n5nppobC9UC
-0003a720: 4f66 3046 304a 7949 4870 5a67 4f46 7753  Of0F0JyIHpZgOFwS
-0003a730: 6872 714e 684c 7755 4548 5254 3477 646c  hrqNhLwUEHRT4wdl
-0003a740: 6649 5835 5630 4773 684c 434b 4856 6967  fIX5V0GshLCKHVig
-0003a750: 5a46 706a 6a7a 4146 536e 5174 3531 7167  ZFpjjzAFSnQt51qg
-0003a760: 3154 4e34 4945 634b 5651 3574 5241 6b6b  1TN4IEcKVQ5tRAkk
-0003a770: 686b 4a4a 6435 5365 3878 3064 2f38 7566  hkJJd5Se8x0d/8uf
-0003a780: 785a 496e 5261 6351 454d 5a44 536d 7444  xZInRacQEMZDSmtD
-0003a790: 7732 4347 3936 7773 7663 6336 2b43 3836  w2CG96wsvcc6+C86
-0003a7a0: 316d 7378 4259 4b53 4b46 4864 6356 4b6e  1msxBYKSKFHdcVKn
-0003a7b0: 4c4b 2b67 4f43 6d4b 6838 4d55 3576 5162  LK+gOCmKh8MU5vQb
-0003a7c0: 556e 674f 5768 535a 2f4f 334a 456f 7753  UngOWhSZ/O3JEowS
-0003a7d0: 5a2b 3344 3479 582b 4667 374d 3336 4938  Z+3D4yX+Fg7M36I8
-0003a7e0: 4263 5743 7958 5549 4f72 5563 3852 5342  BcWCyXUIOrUc8RSB
-0003a7f0: 4a43 774d 5643 7259 5839 2b30 5878 3879  JCwMVCrYX9+0Xx8y
-0003a800: 3539 3063 6a2f 6a32 6a6e 684a 6962 4241  590cj/j2jnhJibBA
-0003a810: 7851 5141 546d 6d62 326d 6444 3439 4930  xQQATmmb2mdD49I0
-0003a820: 7745 5838 5554 7438 546c 4c57 6b6f 3455  wEX8UTt8TlLWko4U
-0003a830: 5233 5265 5672 7443 4f48 446b 5166 374d  R3ReVrtCOHDkQf7M
-0003a840: 4c2f 6e34 6644 446e 6854 3848 4c54 3542  L/n4fDDnhT8HLT5B
-0003a850: 5576 4b6f 794b 4a73 3247 676e 3459 4e67  UvKoyKJs2Ggn4YNg
-0003a860: 7038 394b 7231 3577 4133 7578 634d 4339  p89Kr15wA3uxcMC9
-0003a870: 5256 724d 435a 6931 5a42 7952 7059 6143  RVrMCZi1ZByRpYaC
-0003a880: 4554 6764 6657 4176 7538 466f 376c 3339  ETgdfWAvu8Fo7l39
-0003a890: 6831 4876 3337 6f73 5056 6c4a 436a 4137  h1Hv37osPVlJCjA7
-0003a8a0: 7878 5361 496c 4879 5074 5938 644a 4958  xxSaIlHyPtY8dJIX
-0003a8b0: 376c 4a54 6975 7a43 6179 6c42 6e43 6a6f  7lJTiuzCaylBnCjo
-0003a8c0: 6139 5337 3636 5544 334e 6155 6275 2b35  a9S766UD3NaUbu+5
-0003a8d0: 2f4b 6c47 7946 6142 394a 5446 6734 4666  /KlGyFaB9JTFg4Ff
-0003a8e0: 6647 5862 6955 7057 676f 4c49 486d 6330  fGXbiUpWgoLIHmc0
-0003a8f0: 7674 476b 5a5a 4148 4d32 7650 7237 7577  vtGkZZAHM2vPr7uw
-0003a900: 5270 2f34 4642 6c34 4851 4230 6668 4258  Rp/4FBl4HQB0fhBX
-0003a910: 555a 4c74 6b6e 5842 626b 5167 4a4d 7067  UZLtknXBbkQgJMpg
-0003a920: 496b 7a42 2b67 346e 6e4f 4d75 576a 3738  IkzB+g4nnOMuWj78
-0003a930: 334f 2f76 6a67 572f 6471 5237 466a 3145  3O/vjgW/dqR7Fj1E
-0003a940: 5758 3169 4334 4257 7133 6463 392b 5450  WX1iC4BWq3dc9+TP
-0003a950: 4a2b 5a50 5179 5862 545a 674a 314b 644f  J+ZPQyXbTZgJ1KdO
-0003a960: 7649 6f68 3258 4a4d 6532 4351 7253 4346  vIoh2XJMe2CQrSCF
-0003a970: 6e4d 4f62 732b 3936 4134 2f34 3569 2b39  nMObs+96A4/45i+9
-0003a980: 5a35 674d 4d59 655a 514c 6436 514d 5a64  Z5gMMYeZQLd6QMZd
-0003a990: 4166 6a54 696c 4157 7558 7a73 5676 4d5a  AfjTilAWuXzsVvMZ
-0003a9a0: 4655 4d37 536f 6e77 514b 534b 4342 746b  FUM7SonwQKSKCBtk
-0003a9b0: 6f71 7152 524e 5743 5978 662b 724a 7056  oqqRRNWCYxf+rJpV
-0003a9c0: 3565 7654 7350 2b2f 4470 6b2b 5052 784e  5evTsP+/Dpk+PRxN
-0003a9d0: 6c38 4956 7246 4c78 4374 5566 4445 3463  l8IVrFLxCtUfDE4c
-0003a9e0: 6d57 5049 464f 4a50 6941 345a 706e 5153  mWPIFOJPiA4ZpnQS
-0003a9f0: 6478 3369 4f49 416a 306b 4279 6747 4630  dx3iOIAj0kBygGF0
-0003aa00: 5a6f 632f 4b68 5842 6d50 6e32 4867 626d  Zoc/KhXBmPn2Hgbm
-0003aa10: 7676 4466 776d 506d 5531 6735 2b5a 4430  vvDfwmPmU1g5+ZD0
-0003aa20: 7441 6e4a 4542 4e6d 306f 5152 7a78 307a  tAnJEBNm0oQRzx0z
-0003aa30: 4f66 7a54 7131 4e38 3573 7241 5035 5067  OfzTq1N85srAP5Pg
-0003aa40: 5872 4f2f 716c 5367 3971 4353 496b 4277  XrO/qlSg9qCSIkBw
-0003aa50: 6d6a 6c49 6274 4652 4337 6963 392b 6654  mjlIbtFRC7ic9+fT
-0003aa60: 494c 772b 2f65 7363 3539 2f53 6d68 4267  ILw+/esc59/SmhBg
-0003aa70: 4276 6c41 4577 532b 4b74 4452 3676 3443  BvlAEwS+KtDR6v4C
-0003aa80: 6846 4636 6832 6757 5738 444a 3370 4850  hFF6h2gWW8DJ3pHP
-0003aa90: 7049 4e42 4e45 686b 6975 6c43 5435 2f75  pINBNEhkiulCT5/u
-0003aaa0: 6b57 7a6a 672f 6635 662b 7363 4476 4250  kWzjg/f5f+scDvBP
-0003aab0: 766a 3850 4763 424f 6169 6e70 374f 6c5a  vj8PGcBOainp7OlZ
-0003aac0: 5568 3437 7877 5a69 7a46 6d66 7474 744d  Uh47xwZizFmftttM
-0003aad0: 7379 6334 426b 717a 516d 3141 4157 5579  syc4BkqzQm1AAWUy
-0003aae0: 4f30 6d30 7271 5954 5359 5735 5341 334f  O0m0rqYTSYW5SA3O
-0003aaf0: 5471 3131 5850 6a58 7976 662f 6549 2f59  Tq11XPjXyvf/eI/Y
-0003ab00: 6d49 6234 5944 5948 5055 4948 5838 4250  mIb4YDYHPUIHX8BP
-0003ab10: 3230 7844 3544 6e53 4c6d 7144 4449 4d70  20xD5DnSLmqDDIMp
-0003ab20: 3047 7432 7254 4177 4157 6841 4275 3543  0Gt2rTAwAWhABu5C
-0003ab30: 4c49 5a7a 6d39 4276 3431 512b 324f 336d  LIZzm9Bv41Q+2O3m
-0003ab40: 7854 6c67 2f6f 4944 494a 6a53 3059 756f  xTlg/oIDIJjS0Yuo
-0003ab50: 5432 4e65 5042 6475 666b 3573 7a35 7253  T2NePBdufk5sz5rS
-0003ab60: 2f63 6a74 7845 5050 6c76 3642 4350 7135  /cjtxEPPlv6BCPq5
-0003ab70: 4c4a 5a68 7442 4e73 736c 6b6f 596d 3137  LJZhtBNsslkoYm17
-0003ab80: 6772 4d47 5a33 4a31 4c2f 757a 4945 3464  grMGZ3J1L/uzIE4d
-0003ab90: 6650 654b 744f 2b4d 7258 5944 5050 5546  fPeKtO+MrXYDPPUF
-0003aba0: 3261 3371 304c 3136 6841 6c2f 7843 4d78  2a3q0L16hAl/xCMx
-0003abb0: 5139 314a 3951 3363 4f68 4f6b 306b 6242  Q91J9Q3cOhOk0kbB
-0003abc0: 496d 4d44 5970 4d67 4c6d 4776 596c 7250  ImMDYpMgLmGvYlrP
-0003abd0: 3342 774f 4f2f 3176 3575 6359 4755 4c62  3BwOO/1v5ucYGULb
-0003abe0: 446f 6d4b 437a 742f 302f 6d6a 554b 5a2f  DomKCzt/0/mjUKZ/
-0003abf0: 7475 714e 7a73 7054 3841 7641 6d69 3030  tuqNzspT8AvAmi00
-0003ac00: 3977 2f33 5368 6949 526a 5a67 6345 4371  9w/3ShiIRjZgcECq
-0003ac10: 6c6e 6b74 784e 624f 635a 3066 4f75 6d73  lnktxNbOcZ0fOums
-0003ac20: 2f4e 754f 4c66 6158 7263 3073 5176 4951  /NuOLfaXrc0sQvIQ
-0003ac30: 3559 6531 5442 3172 4365 5261 4f2f 4f55  5Ye1TB1rCeRaO/OU
-0003ac40: 3431 7767 3667 6f46 5753 5268 7a6b 4178  41wg6goFWSRhzkAx
-0003ac50: 4b71 5532 794a 554b 7971 6437 7137 466c  KqU2yJUKyqd7q7Fl
-0003ac60: 7639 7a74 6d6d 625a 3247 7253 5a73 7553  v9ztmmbZ2GrSZsuS
-0003ac70: 4177 4567 4d4e 2f4b 6845 427a 6166 624c  AwEgMN/KhEBzafbL
-0003ac80: 6a36 5863 4c79 396b 586f 7638 4545 744e  j6XcLy9kXov8EEtN
-0003ac90: 6c35 5743 546b 5732 4835 6175 6775 4878  l5WCTkW2H5auguHx
-0003aca0: 5577 5562 6568 4f30 4238 3672 4852 3435  UwUbehO0B86rHR45
-0003acb0: 7176 6d62 5570 2f66 5736 6451 7648 4436  qvmbUp/fW6dQvHD6
-0003acc0: 5842 426e 6638 4d38 652f 3237 7338 5174  XBBnf8M8e/27s8Qt
-0003acd0: 6d73 3866 6853 4a66 4d4e 614a 536e 7a31  ms8fhSJfMNaJSnz1
-0003ace0: 4e59 4e4c 5162 6e54 734d 4979 3549 5037  NYNLQbnTsMIy5IP7
-0003acf0: 4859 6e7a 6942 774f 4f65 3344 4f4c 6c4d  HYnziBwOOe3DOLlM
-0003ad00: 4c4f 6e58 6a59 445a 7142 4d6d 6749 4257  LOnXjYDZqBMmgIBW
-0003ad10: 6136 4d59 434a 684b 6637 5844 7145 742f  a6MYCJhKf7XDqEt/
-0003ad20: 7565 546f 6331 6d39 4372 5a64 4864 6b4b  ueToc1m9CrZdHdkK
-0003ad30: 4652 6557 6266 5952 416d 3946 6754 4167  FReWbfYRAm9FgTAg
-0003ad40: 5962 7456 4a49 6134 536a 626e 4852 3735  YbtVJIa4SjbnHR75
-0003ad50: 7835 2f36 5148 7262 6a46 7753 6671 7833  x5/6QHrbjFwSfqx3
-0003ad60: 474b 3151 7436 3777 446d 5356 7667 594d  GK1Qt67wDmSVvgYM
-0003ad70: 3844 7659 4f68 7455 7154 5231 3430 784d  8DvYOhtUqTR140xM
-0003ad80: 4157 6d2f 5853 5541 4a73 3547 2b67 4450  AWm/XSUAJs5G+gDP
-0003ad90: 7269 6e66 3748 7631 3336 4953 622f 4d44  rinf7Hv136ISb/MD
-0003ada0: 6672 6776 2b63 514a 7337 5a2f 596b 384d  frgv+cQJs7Z/Yk8M
-0003adb0: 7964 4546 616a 3954 6c39 546b 6a70 3649  ydEFaj9Tl9Tkjp6I
-0003adc0: 3332 4753 4d66 7564 5067 336e 4375 6731  32GSMfudPg3nCug1
-0003add0: 4963 547a 3441 3774 3450 3556 554b 6f55  IcTz4A7t4P5VUKoU
-0003ade0: 6b74 615a 734b 6a48 4d49 3167 6231 5078  ktaZsKjHMI1gb1Px
-0003adf0: 6e57 5a48 3733 644a 3976 7255 477a 5638  nWZH73dJ9vrUGzV8
-0003ae00: 4566 4734 3879 4b37 7258 757a 5a33 4f7a  EfG48yK7rXuzZ3Oz
-0003ae10: 6642 4876 304d 4854 4338 546a 704e 4563  fBHv0MHTC8TjpNEc
-0003ae20: 384f 4d67 4775 6a4d 6f45 7752 426b 756d  8OMgGujMoEwRBkum
-0003ae30: 6b43 4a47 4869 666a 2f67 4f76 5939 3932  kCJGHifj/gOvY992
-0003ae40: 2b78 2f7a 7635 7043 6a47 4e45 7941 4c6f  +x/zv5pCjGNEyALo
-0003ae50: 4f37 6575 7965 6668 7339 3638 7545 636b  O7euyefhs968uEck
-0003ae60: 2b70 384e 7761 526f 4d43 3565 4532 3159  +p8NwaRoMC5eE21Y
-0003ae70: 464b 4655 5842 6c4a 7279 7159 5369 2f4e  FKFUXBlJryqYSi/N
-0003ae80: 7756 6957 6b2f 4847 5370 575a 752f 2b59  wViWk/HGSpWZu/+Y
-0003ae90: 6465 3339 5235 6962 6250 6b48 6b64 4776  de39R5ibbPkHkdGv
-0003aea0: 5070 6963 6e4a 717a 7345 7a43 3578 492b  PpicnJqzsEzC5xI+
-0003aeb0: 3030 544e 5535 7341 5748 5753 4536 5178  00TNU5sAWHWSE6Qx
-0003aec0: 686f 4246 3258 446a 724c 6d58 5350 7376  hoBF2XDjrLmXSPsv
-0003aed0: 7431 7a5a 7454 7638 764c 512f 3930 4762  t1zZtTv8vLQ/90Gb
-0003aee0: 436c 4530 416a 534b 6d58 424e 4831 5369  ClE0AjSKmXBNH1Si
-0003aef0: 6242 3778 764d 6e65 5873 2f2b 6173 4f78  bB7xvMneXs/+asOx
-0003af00: 4a73 4e45 4859 4c74 4563 7470 3855 4561  JsNEHYLtEctp8UEa
-0003af10: 6b54 7471 4746 744c 434c 4d5a 6977 576c  kTtqGFtLCLMZiwWl
-0003af20: 6e56 7961 734a 3759 6675 7561 6148 5636  nVyasJ7YfuuaaHV6
-0003af30: 3643 782b 452f 4678 6a6d 7959 4950 6b4f  6Cx+E/FxjmyYIPkO
-0003af40: 315a 394f 4231 384d 5a38 6e45 5954 6532  1Z9OB18MZ8nEYTe2
-0003af50: 6c68 692b 4134 4543 484f 6947 716d 364f  lhi+A4ECHOiGqm6O
-0003af60: 764d 706b 6b6d 4676 4947 556b 704a 377a  vMpkkmFvIGUkpJ7z
-0003af70: 6237 3567 4835 7642 4e6e 4774 3041 4632  b75gH5vBNnGt0AF2
-0003af80: 5543 6f72 4c44 5147 474c 6e4a 5641 5437  UCorLDQGGLnJVAT7
-0003af90: 612b 597a 5050 7676 662f 357a 4768 4c68  a+YzPPvvf/5zGhLh
-0003afa0: 5143 4c6c 5946 7736 496c 472b 554d 456b  QCLlYFw6IlG+UMEk
-0003afb0: 4639 464f 536f 504c 3167 4f6e 4956 546e  F9FOSoPL1gOnIVTn
-0003afc0: 4865 3262 6f4b 3363 6338 486d 2b62 374a  He2boK3cc8Hm+b7J
-0003afd0: 4e7a 6b46 6f72 7445 7339 2b48 5376 7773  NzkFortEs9+HSvws
-0003afe0: 4f31 7737 5275 555a 3455 4645 4e6a 4946  O1w7RuUZ4UFENjIF
-0003aff0: 655a 4663 5248 5a58 7a42 6550 6639 7671  eZFcRHZXzBePf9vq
-0003b000: 3050 4e48 5678 4544 6748 4551 4938 632b  0PNHVxEDgHEQI8c+
-0003b010: 7772 6c46 7967 424b 7877 652f 316a 3065  wrlFygBKxwe/1j0e
-0003b020: 6475 6c6c 7a6b 4c4b 4158 6a33 6976 5876  dullzkLKAXj3ivXv
-0003b030: 3751 7276 6444 7048 6a77 554c 766d 3054  7QrvdDpHjwULvm0T
-0003b040: 6249 7953 446b 6d58 496f 614b 366f 7044  bIySDkmXIoaK6opD
-0003b050: 6541 7348 4e30 7063 334c 7a7a 6f77 732f  eAsHN0pc3Lzzows/
-0003b060: 6456 782b 334f 6562 6a33 6644 575a 7639  dVx+3Oebj3fDWZv9
-0003b070: 586a 506d 5077 6668 3678 3830 6e42 7878  XjPmPwfh6x80nBxx
-0003b080: 614b 6634 6d48 4f66 5139 2f74 4f66 6d68  aKf4mHOfQ9/tOfmh
-0003b090: 4c6b 4950 6734 3031 324b 4651 5848 384c  LkIPg4012KFQXH8L
-0003b0a0: 5946 446b 4930 6270 334a 5469 5838 3359  YFDkI0bp3JTiX83Y
-0003b0b0: 3765 7957 7637 6e2b 6d5a 507a 7259 4947  7eyWv7n+mZPzrYIG
-0003b0c0: 6870 4334 4c5a 4569 4755 6f6d 7155 7054  hpC4LZEiGUomqUpT
-0003b0d0: 5a32 5048 6446 5659 4438 6970 6d79 6365  Z2PHdFVYD8ipmyce
-0003b0e0: 4876 6744 6568 4579 6648 3277 7a4f 3450  HvgDehEyfH2wzO4P
-0003b0f0: 334e 6637 5433 4f64 4147 4944 6344 4a58  3Nf7T3OdAGIDcDJX
-0003b100: 6550 5468 6353 6745 6f76 5a32 644a 4231  ePThcSgEovZ2dJB1
-0003b110: 3645 4d59 496f 437a 6959 7a44 3934 4c30  6EMYIoCziYzD94L0
-0003b120: 2b6b 2f2b 466e 5565 6e62 4248 734f 752b  +k/+FnUenbBHsOu+
-0003b130: 4245 3244 6f42 4236 6b35 4371 574b 5255  BE2DoBB6k5CqWKRU
-0003b140: 4d79 6b54 7939 5939 486e 3962 3148 7151  MykTy9Y9Hn9b1HqQ
-0003b150: 4559 3937 3661 782b 5035 3236 424d 7164  EY976ax+P526BMqd
-0003b160: 4154 306a 7143 6752 3143 6938 4c4b 366d  AT0jqCgR1Ci8LK6m
-0003b170: 5353 3278 426e 434a 5a6e 4d68 7a5a 7433  SS2xBnCJZnMhzZt3
-0003b180: 3565 6645 6d32 3451 4877 6276 682f 3237  5efEm24QHwbvh/27
-0003b190: 7539 5376 4778 6150 5176 546f 6b68 304a  u9SvGxaPQvTokh0J
-0003b1a0: 454a 326b 3648 6759 6155 725a 4338 4964  EJ2k6HgYaUrZC8Id
-0003b1b0: 436d 3333 4165 3332 5033 654c 6b4b 4d62  Cm33Ae32P3eLkKMb
-0003b1c0: 3679 5545 7739 6932 4d54 2f63 3859 3355  6yUEw9i2MT/c8Y3U
-0003b1d0: 3656 5875 7534 4777 4b6c 506b 664b 4438  6VXuu4GwKlPkfKD8
-0003b1e0: 6f4f 5651 6a6c 516e 7170 3251 524f 5653  oOVQjlQnqp2QROVS
-0003b1f0: 5141 665a 6642 7837 356c 6145 7633 3737  QAfZfBx75laEv377
-0003b200: 2f35 2b46 4b56 3255 5442 4d62 4d65 7a55  /5+FKV2UTBMbMezU
-0003b210: 3963 3744 4e6b 6b39 6154 5038 6267 6642  9c7DNkk9aTP8bgfB
-0003b220: 6761 4943 756f 3056 4a30 5569 7850 6f39  gaICuo0VJ0UixPo9
-0003b230: 6238 6a52 722f 714b 4c35 6777 3947 742f  b8jRr/qKL5gw9Gt/
-0003b240: 524e 6d74 7342 5268 796b 4b70 6c43 546b  RNmtsBRhykKplCTk
-0003b250: 4957 3639 4b65 4e4e 7a2f 6f54 7a48 7651  IW69KeNNz/oTzHvQ
-0003b260: 6363 526a 5535 452f 712f 666c 494a 6255  ccRjU5E/q/flIJbU
-0003b270: 616b 6b48 4a6f 4c6f 6b74 5931 4375 744b  akkHJoLoktY1CutK
-0003b280: 316f 2f54 3952 3466 3058 3762 4e76 3239  1o/T9R4f0X7bNv29
-0003b290: 5373 554d 7376 454c 4675 4863 706b 2f77  SsUMsvELFuHcpk/w
-0003b2a0: 7961 4844 3153 446f 6367 6544 6761 6147  yaHD1SDocgeDgaaG
-0003b2b0: 4e4b 6872 745a 4555 4845 674f 5a59 344c  NKhrtZEUHEgOZY4L
-0003b2c0: 4e79 4365 7353 2b66 3049 474a 7356 6577  NyCesS+f0IGJsVew
-0003b2d0: 4551 7977 7570 5270 6952 586f 5871 5a46  EQywupRpiRXoXqZF
-0003b2e0: 3636 2b37 352b 6964 6a54 742f 6951 3678  66+75+idjTt/iQ6x
-0003b2f0: 7947 5037 6d37 382b 4765 6c34 4436 7661  yGP7m78+Gel4D6va
-0003b300: 7155 5657 646c 4b49 4346 5958 4153 4179  qUVWdlKICFYXASAy
-0003b310: 4c62 4b69 7149 7758 6535 4655 7535 5063  LbKiqIwXe5FUu5Pc
-0003b320: 5748 584c 4a79 3176 5855 3363 4e4b 7336  WHXLJy1vXU3cNKs6
-0003b330: 4434 4255 7139 4272 6345 7139 7779 582b  D4BUq9BrcEq9wyX+
-0003b340: 7732 6553 5163 4570 6b38 6d4e 7532 6364  w2eSQcEpk8mNu2cd
-0003b350: 6166 6671 6431 7833 6b4b 454a 5154 3950  affqd1x3kKEJQT9P
-0003b360: 5251 6751 6473 5273 7866 3838 4c37 7557  RQgQdsRsxf88L7uW
-0003b370: 7576 7939 5535 732b 7735 446f 6b42 3048  uvy9U5s+w5DokB0H
-0003b380: 4a77 4261 5939 5a45 4379 526e 6644 346a  JwBaY9ZECyRnfD4j
-0003b390: 7878 4f44 6e62 7274 6d79 4373 3339 614c  xxODnbrtmyCs39aL
-0003b3a0: 3062 5167 5652 5a44 3956 2f31 6662 5775  0bQgVRZD9V/1fbWu
-0003b3b0: 7a75 466c 772b 5243 3038 4768 7358 5571  zuFlw+RC08GhsXUq
-0003b3c0: 6774 7465 7462 7736 434d 7171 6f4f 5967  gttetbw6CMqqoOYg
-0003b3d0: 4972 5a4f 6747 3250 384c 6c2b 7949 3937  IrZOgG2P8Ll+yI97
-0003b3e0: 7565 6453 7a6d 2f54 6b62 5a66 4331 444e  uedSzm/TkbZfC1DN
-0003b3f0: 4344 714d 4545 6f4f 7576 684f 7945 5144  CDqMEEoOuvhOyEQD
-0003b400: 2f4e 752b 4143 3166 3273 766c 3563 4736  /Nu+AC1f2svl5cG6
-0003b410: 5a42 7656 5a72 684a 4b79 4646 5562 5168  ZBvVZrhJKyFFUbQh
-0003b420: 3048 4133 4b5a 444a 5157 4157 622f 6148  0HA3KZDJQWAWb/aH
-0003b430: 4d57 5938 506e 6e6c 5474 336a 4754 5556  MWY8PnnlTt3jGTUV
-0003b440: 6c45 4154 6d47 684f 616e 6a6f 776e 3636  lEATmGhOanjown66
-0003b450: 5a43 5457 3647 4868 5246 3751 3443 4b30  ZCTW6GHhRF7Q4CK0
-0003b460: 564b 3445 394d 4159 7143 6a68 4d48 3350  VK4E9MAYqCjhMH3P
-0003b470: 756e 2f35 4f6e 324d 752b 4b44 5035 4d36  un/5On2Mu+KDP5M6
-0003b480: 3972 3747 6c59 6570 6e71 6878 3049 744f  9r7GlYepnqhx0ItO
-0003b490: 7064 4e43 4e2f 4444 4164 2b48 6e37 2f2f  pdNCN/DDAd+Hn7//
-0003b4a0: 4e47 6237 7654 4141 7666 4239 346b 7644  NGb7vTAAvfB94kvD
-0003b4b0: 6b6f 7575 7071 6738 4253 5653 6a2b 3247  kouupqg8BSVSj+2G
-0003b4c0: 6762 557a 4333 4954 7678 6158 317a 4f42  gbUzC3ITvxaX1zOB
-0003b4d0: 6e62 3735 7957 356d 6264 4439 4270 4c54  nb75yW5mbdD9BpLT
-0003b4e0: 3262 4a6c 3549 624f 734a 3645 4234 5743  2bJl5IbOsJ6EB4WC
-0003b4f0: 516b 5a4a 5136 4d59 4e54 4561 5052 6b4f  QkZJQ6MYNTEaPRkO
-0003b500: 4a62 2f6d 784e 6842 2f6c 465a 7576 3764  Jb/mxNhB/lFZuv7d
-0003b510: 3766 2b6b 4253 7574 656f 4266 6b7a 5066  7f+kBSuteoBfkzPf
-0003b520: 4a47 345a 446c 6c44 7171 7075 676f 7244  JG4ZDllDqqpugorD
-0003b530: 6f77 504f 5739 6b37 5930 3243 6f65 776f  owPOW9k7Y02Coewo
-0003b540: 7764 7835 4f34 716d 6570 7236 6d79 6d59  wdx5O4qmepr6mymY
-0003b550: 2f43 466f 7232 7264 4156 7345 4a34 4764  /CFor2rdAVsEJ4Gd
-0003b560: 5759 2b76 5441 7836 3974 5339 5a4b 686a  WY+vTAx69tS9ZKhj
-0003b570: 6454 7043 3957 7037 6453 584c 7845 2b67  dTpC9Wp7dSXLxE+g
-0003b580: 396d 614c 5742 4b47 3051 4145 6f6e 614a  9maLWBKG0QAEonaJ
-0003b590: 306e 4851 4353 586f 4664 7148 6c73 314f  0nHQCSXoFdqHls1O
-0003b5a0: 7458 6775 2b2b 5635 502b 734b 357a 7244  tXgu++V5P+sK5zrD
-0003b5b0: 566f 5569 6846 6a62 7569 5639 5541 666c  VoUihFjbuiV9UAfl
-0003b5c0: 5067 7370 5150 4b79 3372 7141 4a55 436f  PgspQPKy3rqAJUCo
-0003b5d0: 7864 4966 3337 396b 5459 7345 3275 6850  xdIf379kTYsE2uhP
-0003b5e0: 6b54 6661 3738 4548 7038 794f 6763 6e38  kTfa78EHp8yOgcn8
-0003b5f0: 7a56 5131 6769 4943 4948 4250 5354 4b41  zVQ1giICIHBPSTKA
-0003b600: 6c43 6678 7676 347a 7659 7965 3837 3047  lCfxvv4zvYye870G
-0003b610: 2b62 742b 2f39 6148 624b 7a65 682b 656b  +bt+/9aHbKzeh+ek
-0003b620: 2f51 7563 356c 794b 5278 6951 3156 4254  /Quc5lyKRxiQ1VBT
-0003b630: 4b48 5169 4146 5053 4330 5030 794c 7939  KHQiAFPSC0P0yLy9
-0003b640: 3964 3944 6b56 6372 6162 5368 7130 3530  9d9DkVcrabShq050
-0003b650: 2b2b 5a2f 4475 4733 3945 6d6f 3576 716a  ++Z/DuG39Emo5vqj
-0003b660: 7539 4e4f 576f 464e 7047 3061 6c7a 4d4b  u9NOWoFNpG0alzMK
-0003b670: 4f2f 634a 7662 7268 7037 7236 584e 4b76  O/cJvbrhp7r6XNKv
-0003b680: 5579 7342 324c 2f33 6d71 317a 4961 3248  UysB2L/3mq1zIa2H
-0003b690: 7950 5652 5857 6c57 7533 4834 4573 7078  yPVRXWlWu3H4Espx
-0003b6a0: 4e74 6b6d 5a48 4c72 3069 4d70 3966 4c37  NtkmZHLr0iMp9fL7
-0003b6b0: 6250 516a 3070 716d 6b6d 4961 4c68 6b70  bPQj0pqmkmIaLhkp
-0003b6c0: 5269 4241 6930 4f6b 436c 5a77 4434 3970  RiBAi0OkClZwD49p
-0003b6d0: 6a36 3371 6c76 3971 4e35 4542 536d 4955  j63qlv9qN5EBSmIU
-0003b6e0: 772b 7030 2f44 5272 3732 6630 3363 3463  w+p0/DRr72f03c4c
-0003b6f0: 2f44 4256 7552 7734 6468 5074 435a 704e  /DBVuRw4dhPtCZpN
-0003b700: 4779 4568 6d2f 5a44 5839 4878 7839 4876  GyEhm/ZDX9Hxx9Hv
-0003b710: 2f66 6544 456d 644d 6473 4257 5272 3775  /feDEmdMdsBWRr7u
-0003b720: 7736 4943 4c37 3745 4c2f 7437 6773 2b2b  w6ICL77EL/t7gs++
-0003b730: 4634 564b 5771 6c78 3250 347a 7377 435a  F4VKWqlx2P4zswCZ
-0003b740: 5a6c 5743 4651 3153 734d 7448 7442 4a47  ZlWCFQ1SsMtHtBJG
-0003b750: 4d32 3048 4442 554c 7242 7272 7856 564a  M20HDBULrBrrxVVJ
-0003b760: 5276 7055 2b35 3265 3833 6565 6f4a 344f  RvpU+52e83eeoJ4O
-0003b770: 7646 3235 3952 4473 745a 314f 6d57 4474  vF259RDstZ1OmWDt
-0003b780: 2f64 4e2f 4552 4733 6d43 575a 7876 4c6d  /dN/ERG3mCWZxvLm
-0003b790: 5a43 7659 6d32 412f 714c 6e6f 666c 4377  ZCvYm2A/qLnoflCw
-0003b7a0: 6942 2b52 544b 6b31 7378 3348 4c66 6e68  iB+RTKk1sx3HLfnh
-0003b7b0: 5a6e 2b31 7647 5058 6f72 6668 7759 6665  Zn+1vGPXorfhwYfe
-0003b7c0: 5468 4450 356e 384f 2f73 384c 7931 6c77  ThDP5n8O/s8Ly1lw
-0003b7d0: 6775 6354 7644 6974 3730 5835 6f47 3644  gucTvDit70X5oG6D
-0003b7e0: 4970 7331 6d4c 6d61 6231 784d 7146 4e30  Ips1mLmab1xMqFN0
-0003b7f0: 2f53 6163 574d 3630 5761 4f30 5543 7332  /SacWM60WaO0UCs2
-0003b800: 4249 4944 4f65 582f 4c6c 2f2f 6366 6332  BIIDOeX/Ll//cfc2
-0003b810: 6a70 2b48 3945 3532 774e 5646 456a 6831  jp+H9E52wNVFEjh1
-0003b820: 6676 3666 6e6a 6a38 3735 5763 7961 5438  fv6fnjj875WcyaT8
-0003b830: 4764 6473 5a36 6d67 4656 5134 366b 5a45  GddsZ6mgFVQ46kZE
-0003b840: 366f 4a2b 5368 4862 3551 484a 6542 3937  6oJ+ShHb5QHJeB97
-0003b850: 6b63 6a36 6b2f 746e 5237 2f33 7049 4c42  kcj6k/tnR7/3pILB
-0003b860: 6975 6431 4b6c 4d48 5033 544a 6132 4c33  iud1KlMHP3TJa2L3
-0003b870: 2f43 5058 4766 336d 7436 772b 4272 6a61  /CPXGf3mt6w+Brja
-0003b880: 6831 4b5a 6c4a 647a 7636 5379 362f 5777  h1KZlJdzv6Sy6/Ww
-0003b890: 4563 3541 3271 4152 4e30 4657 7a42 5170  Ec5A2qARN0FWzBQp
-0003b8a0: 4136 5253 4e4e 7172 576c 6344 754a 5430  A6RSNNqrWlcDuJT0
-0003b8b0: 752b 6350 435a 7065 2b31 2b50 6f42 6443  u+cPCZpe+1+PoBdC
-0003b8c0: 6849 706d 3343 4971 494d 5859 3644 482b  hIpm3CIqIMXY6DH+
-0003b8d0: 6d37 4841 6f71 334a 2b44 634f 2b55 5641  m7HAoq3J+DcO+UVA
-0003b8e0: 2b70 454f 7454 4332 4d41 714c 3062 4671  +pEOtTC2MAqL0bFq
-0003b8f0: 4f48 4947 4e6f 6852 5461 5753 4475 596b  OHIGNohRTaWSDuYk
-0003b900: 5174 3049 6e2b 3958 6350 6236 3247 7050  Qt0In+9XcPb62GpP
-0003b910: 5171 7555 5778 3542 5862 736f 774c 336b  QquUWx5BXbsowL3k
-0003b920: 6131 4f4d 6d32 4d6d 6532 6b7a 3143 2f59  a1OMm2Mme2kz1C/Y
-0003b930: 5871 304e 3665 3176 702f 6b4a 5454 5674  Xq0N6e1vp/kJTTVt
-0003b940: 7978 4f56 2f31 7061 4b51 7756 3445 4544  yxOV/1paKQwV4EED
-0003b950: 515a 7048 4730 3370 674e 3942 7178 4949  QZpHG03pgN9BqxII
-0003b960: 6646 3044 7663 534c 3378 4c50 6a56 6a31  fF0DvcSL3xLPjVj1
-0003b970: 3236 6862 304a 6b69 4d49 6e4b 4d65 7533  26hb0JkiMInKMeu3
-0003b980: 5747 6e6e 324c 722b 5547 6564 2f49 5435  WGnn2Lr+UGed/IT5
-0003b990: 616b 5150 715a 7970 6f46 4a42 6835 3143  akQPqZypoFJBh51C
-0003b9a0: 7974 4c4f 514d 4547 676f 4e41 5377 5746  ytLOQMEGgoNASwWF
-0003b9b0: 7559 6c6e 6659 3562 312b 4136 7a37 7072  uYlnfY5b1+A6z7pr
-0003b9c0: 415a 6b7a 4259 7869 7430 3561 426c 487a  AZkzBYxit05aBlHz
-0003b9d0: 3479 3738 5a5a 726d 4a2b 376d 5564 3759  4y78ZZrmJ+7mUd7Y
-0003b9e0: 6a68 3161 707a 7532 7172 5777 554e 6262  jh1apzu2qrWwUNbb
-0003b9f0: 6f50 6c55 7775 7038 6770 7546 4342 5244  oPlUwup8gpuFCBRD
-0003ba00: 5641 5559 6e71 512b 4743 5577 614b 5878  VAUYnqQ+GCUwaKXx
-0003ba10: 3769 386d 2f4e 6135 7175 3376 5831 5938  7i8m/Na5qu3vX1Y8
-0003ba20: 4f55 6659 7551 5474 6934 4c4c 544a 2f39  OUfYuQTti4LLTJ/9
-0003ba30: 7a64 4b72 7667 4f65 4245 742b 4352 662b  zdKrvgOeBEt+CRf+
-0003ba40: 3357 3669 4a4f 6669 4231 4e55 4d41 3456  3W6iJOfiB1NUMA4V
-0003ba50: 4156 5970 4b4e 6b5a 7469 3277 4441 7857  AVYpKNkZti2wDAxW
-0003ba60: 5665 4e7a 3238 4378 7235 6f6a 5252 2f39  VeNz28Cxr5ojRR/9
-0003ba70: 3468 3566 7571 6f46 3461 5232 3744 4250  4h5fuqoF4aR27DBP
-0003ba80: 7576 444d 7837 4b58 627a 2f46 392b 6172  uvDMx7KXbz/F9+ar
-0003ba90: 6b2f 4467 6f4a 7147 5473 494b 6d61 696f  k/DgoJqGTsIKmaio
-0003baa0: 6769 5761 7452 477a 4276 6756 706c 592f  giWatRGzBvgVplY/
-0003bab0: 4b6d 594d 4562 5262 714a 496f 6173 324e  KmYMEbRbqJIoas2N
-0003bac0: 7942 4e6e 5534 796c 6e57 7235 3459 397a  yBNnU4ylnWr54Y9z
-0003bad0: 4b68 3342 7545 6e35 3764 3950 516a 6868  Kh3BuEn57d9PQjhh
-0003bae0: 7735 6836 7738 397a 3766 3234 6c37 4839  w5h6w89z7f24l7H9
-0003baf0: 4b62 7530 5772 5573 3763 6743 6f31 6d47  Kbu0WrUs7cgCo1mG
-0003bb00: 5539 4e49 4f52 4c47 5364 5576 4a6f 6152  U9NIORLGSdUvJoaR
-0003bb10: 5345 5641 5a2f 4754 6f44 3777 712f 744b  SEVAZ/GToD7wq/tK
-0003bb20: 494e 2f2b 7750 3573 3548 5238 7637 7a71  IN/+wP5s5HR8v7zq
-0003bb30: 536f 4e64 3436 6263 3772 4272 722f 692f  SoNd46bc7rBrr/i/
-0003bb40: 5535 6664 6747 6167 5474 4f67 384f 5972  U5fdgGagTtOg8OYr
-0003bb50: 3352 5348 4d56 376e 6f64 6f4a 5145 3058  3RSHMV7nodoJQE0X
-0003bb60: 6243 5853 4d4b 6e73 6b6f 594f 4467 5571  bCXSMKnskoYODgUq
-0003bb70: 594c 5770 6e41 3248 6f64 632b 3635 6331  YLWpnA2Hodc+65c1
-0003bb80: 2f33 5750 6c33 7764 4370 6f33 744f 4551  /3WPl3wdCpo3tOEQ
-0003bb90: 4770 524a 6772 6a48 4632 656e 6a2b 7959  GpRJgrjHF2enj+yY
-0003bba0: 3550 6575 6659 725a 314b 5253 564c 4371  5PeufYrZ1KRSVLCq
-0003bbb0: 7a74 424e 6745 746f 6f6a 6f48 5339 5a36  ztBNgEtoojoHS9Z6
-0003bbc0: 4141 6f6c 4371 752f 3542 7573 7161 6149  AAolCqu/5BusqaaI
-0003bbd0: 714b 7754 7146 7961 4131 4272 5763 5279  qKwTqFyaA1BrWcRy
-0003bbe0: 3372 4564 4731 4778 3351 392b 5a76 3847  3rEdG1Gx3Q9+Zv8G
-0003bbf0: 7251 7156 3133 3269 4d2f 5842 4763 7568  rQqV132iM/XBGcuh
-0003bc00: 4c74 3530 7268 4867 5779 734c 5863 3957  Lt50rhHgWysLXc9W
-0003bc10: 3748 5548 3570 6a37 5243 4171 7449 4977  7HUH5pj7RCAqtIIw
-0003bc20: 7473 6f34 7842 7259 4e66 3832 3457 3145  tso4xBrYNf824W1E
-0003bc30: 5251 3677 4170 7445 514a 5472 4677 6b43  RQ6wAptEQJTrFwkC
-0003bc40: 6a50 446b 695a 3659 6b7a 416d 2b37 4976  jPDkiZ6YkzAm+7Iv
-0003bc50: 6b79 3775 7565 4f53 3069 544d 3750 5463  ky7uueOS0iTM7PTc
-0003bc60: 7049 6759 7549 3536 3673 355a 504f 2b56  pIgYuI566s5ZPO+V
-0003bc70: 6e50 4a6c 3443 4378 6a6f 5168 6f75 3744  nPJl4CCxjoQhou7D
-0003bc80: 4d6f 4934 4570 5955 574c 5547 5144 582f  MoI4EpYUWLUGQDX/
-0003bc90: 3462 464e 4438 7779 3259 4f58 5070 4f73  4bFND8wy2YOXPpOs
-0003bca0: 744e 4f6b 6b53 4b70 3878 7168 5570 5750  tNOkkSKp8xqhUpWP
-0003bcb0: 4d61 415a 6771 5963 6158 5635 626b 3370  MaAZgqYcaXV5bk3p
-0003bcc0: 712b 4f75 2f77 7974 6469 4530 6979 5859  q+Ou/wytdiE0iyXY
-0003bcd0: 7633 5471 795a 6432 4b65 356e 6b66 3441  v3TqyZd2Ke5nkf4A
-0003bce0: 7444 454a 6255 666b 677a 4837 6f43 4347  tDEJbUfkgzH7oCCG
-0003bcf0: 3059 5551 7035 636c 4251 6b63 726d 7947  0YUQp5clBQkcrmyG
-0003bd00: 6264 5a62 7043 757a 522b 4a53 2b69 7155  bdZbpCuzR+JS+iqU
-0003bd10: 626a 774c 5467 6744 5167 3168 4a59 3466  bjwLTggDQg1hJY4f
-0003bd20: 5a51 4446 3642 2f6d 462b 687a 6e33 336d  ZQDF6B/mF+hzn33m
-0003bd30: 422f 6544 3959 6366 5037 2b42 4b56 326c  B/eD9YcfP7+BKV2l
-0003bd40: 3738 4c45 7a70 6a74 7339 7830 4f5a 596e  78LEzpjts9x0OZYn
-0003bd50: 457a 5679 6f44 3053 304b 3764 736d 6470  EzVyoD0S0K7dsmdp
-0003bd60: 6d41 7670 4267 4338 6b75 6434 6936 384d  mAvpBgC8kud4i68M
-0003bd70: 4674 3972 2f65 506b 3171 3541 5859 7165  Ft9r/ePk1q5AXYqe
-0003bd80: 6839 6536 4a42 317a 4f61 6a49 4877 7867  h9e6JB1zOajIHwxg
-0003bd90: 2f5a 664c 7251 4730 794b 4453 7933 7832  /ZfLrQG0yKDSy3x2
-0003bda0: 564a 5667 6275 4b5a 6663 6465 2f62 6434  VJVgbuKZfcde/bd4
-0003bdb0: 4246 3571 6270 3261 7444 6f46 5871 4377  BF5qbp2atDoFXqCw
-0003bdc0: 2f38 5255 3462 3934 4955 6657 7645 494a  /8RU4b94IUfWvEIJ
-0003bdd0: 7436 3956 4261 4975 7942 655a 5144 2f49  t69VBaIuyBeZQD/I
-0003bde0: 4351 6f49 6f71 5151 4532 6778 7a78 6d6c  CQoIoqQQE2gxzxml
-0003bdf0: 4c6a 7635 6578 5637 4671 6743 4350 4e6b  Ljv5exV7FqgCCPNk
-0003be00: 4758 5457 4475 6d6f 3733 5849 4930 3667  GXTWDumo73XII06g
-0003be10: 5258 5563 6932 5543 4a36 4945 396b 722f  RXUci2UCJ6IE9kr/
-0003be20: 6f34 4447 786b 4174 7868 544e 3461 5053  o4DGxkAtxhTN4aPS
-0003be30: 6633 4c51 6a42 7076 432b 506a 2f75 7276  f3LQjBpvC+Pj/urv
-0003be40: 5736 3148 7a45 316a 3148 4f41 4644 4633  W61HzE1j1HOAFDF3
-0003be50: 4b6c 5675 7554 436f 7853 4663 2f2b 424f  KlVuuTCoxSFc/+BO
-0003be60: 6959 4b31 7365 7041 2f2b 4f70 6637 546d  iYK1sepA/+Opf7Tm
-0003be70: 4c36 5a31 7462 766b 776a 6247 4571 4b32  L6Z1tbvkwjbGEqK2
-0003be80: 3133 636c 3737 435a 3247 5834 6c73 2b30  13cl77CZ2GX4ls+0
-0003be90: 4273 4162 5653 5731 5362 594f 3053 426c  BsAbVSW1SbYO0SBl
-0003bea0: 476d 6977 5530 4938 4370 4f4b 4833 4266  GmiwU0I8CpOKH3Bf
-0003beb0: 6e2f 7965 2f2f 4730 3236 5670 7a71 7161  n/ye//G026Vpzqqa
-0003bec0: 6352 6343 3578 724f 3344 7856 702f 6d75  cRcC5xrO3DxVp/mu
-0003bed0: 6f34 7a47 7772 326f 5348 6d78 6272 324b  o4zGwr2oSHmxbr2K
-0003bee0: 3272 5856 7455 445a 7444 7649 434f 6952  2rXVtUDZtDvICOiR
-0003bef0: 4849 4d67 4e56 7a52 424b 6d43 5372 7144  HIMgNVzRBKmCSrqD
-0003bf00: 6153 7a63 6577 6a53 7130 6147 3170 5644  aSzcewjSq0aG1pVD
-0003bf10: 2f68 5362 4d68 5861 746f 7433 6f6b 6532  /hSbMhXatot3oke2
-0003bf20: 4575 5648 4349 766c 516e 316c 2f79 5339  EuVHCIvlQn1l/yS9
-0003bf30: 652f 4e74 526e 3936 5054 354e 4779 5945  e/NtRn96PT5NGyYE
-0003bf40: 3633 6733 6e4f 3139 3333 7a46 6566 6532  63g3nO1933zFefe2
-0003bf50: 7a34 476e 7738 6675 5375 3732 3448 5358  z4Gnw8fuSu724HSX
-0003bf60: 626c 526b 6d42 5247 7151 3935 6461 4c38  blRkmBRGqQ95daL8
-0003bf70: 3139 7966 7370 722f 2f33 706d 3971 4158  19yfspr//3pm9qAX
-0003bf80: 6355 4149 584a 7577 4567 7a47 6758 4e76  cUAIXJuwEgzGgXNv
-0003bf90: 4d6b 2f66 4e66 4d64 2b34 4d57 4c65 4550  Mk/fNfMd+4MWLeEP
-0003bfa0: 4c59 7a67 3355 5a74 5532 7941 744b 434f  LYzg3UZtU2yAtKCO
-0003bfb0: 554a 6773 4652 5a4a 5a73 4450 6a70 4755  UJgsFRZJZsDPjpGU
-0003bfc0: 394f 5377 3934 4765 392f 2b39 4776 4e4b  9OSw94Ge9/+9GvNK
-0003bfd0: 464b 4430 5a73 4f47 7633 4836 6d6e 2b49  FKD0ZsOGv3H6mn+I
-0003bfe0: 7a59 6233 6a4f 7951 4851 6573 716f 5553  zYb3jOyQHQesqoUS
-0003bff0: 6953 676f 5345 7863 7968 576c 4245 4f72  iSgoSExcyhWlBEOr
-0003c000: 7771 2f41 7053 5076 4732 7472 5959 3932  wq/ApSPvG2trYY92
-0003c010: 5462 5343 4349 525a 4236 366f 6474 5633  TbSCCIRZB66odtV3
-0003c020: 4974 5443 342b 6136 5137 4479 5966 4f38  ItTC4+a6Q7DyYfO8
-0003c030: 4c4f 6e68 6e6c 5951 3567 3955 6a32 796b  LOnhnlYQ5g9Uj2yk
-0003c040: 2b53 4243 6f58 3642 4468 6f58 4d6b 392f  +SBCoX6BDhoXMk9/
-0003c050: 4966 7254 6f32 626d 544c 7946 7673 7675  IfrTo2bmTLyFvsvu
-0003c060: 7375 7762 6b65 3956 6677 726e 3148 6369  suwbke9Vfwrn1Hci
-0003c070: 6776 2f53 424d 4758 6f64 556b 7436 5553  gv/SBMGXodUkt6US
-0003c080: 555a 4853 4b6f 4e66 4973 6458 725a 6a70  UZHSKoNfIsdXrZjp
-0003c090: 2f65 2b47 5062 4f36 7946 6d6d 425a 3043  /e+GPbO6yFmmBZ0C
-0003c0a0: 6136 3473 476e 494d 4834 516e 7749 6c7a  a64sGnIMH4QnwIlz
-0003c0b0: 3434 4567 732b 474f 3143 656c 392b 6544  44Egs+GO1Cel9+eD
-0003c0c0: 3976 5447 4476 386b 5474 7270 6333 5646  9vTGDv8kTtrpc3VF
-0003c0d0: 5a79 7167 6c69 4342 6453 5171 7875 3072  ZyqgliCBdSQqxu0r
-0003c0e0: 3541 6654 6262 7935 3863 7555 6237 4672  5AfTbby58cuUb7Fr
-0003c0f0: 6c54 5962 4e76 474f 5954 4970 7249 4f2b  lTYbNvGOYTIprIO+
-0003c100: 5a55 424d 3733 4861 7746 3846 3241 7073  ZUBM73HawF8F2Aps
-0003c110: 4a74 4454 4a32 725a 614d 506c 4c49 5034  JtDTJ2rZaMPlLIP4
-0003c120: 7873 4c32 4a4a 6f2f 2b42 5871 526a 624e  xsL2JJo/+BXqRjbN
-0003c130: 7079 2b4d 6856 7364 5142 4a48 3655 5865  py+MhVsdQBJH6UXe
-0003c140: 4162 6b41 7454 4541 4573 5331 2f59 7074  AbkAtTEAEsS1/Ypt
-0003c150: 584d 7a2f 4a73 3565 4248 5471 7775 6c6c  XMz/Js5eBHTqwull
-0003c160: 5632 696b 516f 5530 4839 4374 7279 3847  V2ikQoU0H9Ctry8G
-0003c170: 352b 6839 2b57 3974 3345 335a 695a 3547  5+h9+W9t3E3ZiZ5G
-0003c180: 7962 774d 7630 2b35 6a64 4770 7a61 6830  ybwMv0+5jdGpzah0
-0003c190: 4347 4a52 4a47 796a 4a70 454d 416e 564b  CGJRJGyjJpEMAnVK
-0003c1a0: 3437 6a4c 376c 5939 7573 5239 3759 7a5a  47jL7lY9usR97YzZ
-0003c1b0: 764c 6b67 6b42 3954 4c73 7158 4666 5743  vLkgkB9TLsqXFfWC
-0003c1c0: 4a44 5838 2b46 3867 5547 4242 426b 6931  JDX8+F8gUGBBBki1
-0003c1d0: 3978 6833 4d34 4174 702b 324c 6e37 5871  9xh3M4Atp+2Ln7Xq
-0003c1e0: 3478 2b31 3976 7179 7650 6879 5942 4754  4x+19vqyvPhyYBGT
-0003c1f0: 746f 4377 7467 6e30 4f30 6949 3272 4b39  toCwtgn0O0iI2rK9
-0003c200: 6b54 6244 6c50 7861 6176 6574 544e 6662  kTbDlPxaavetTNfb
-0003c210: 6830 7559 3377 5042 324b 4f57 4972 4575  h0uY3wPB2KOWIrEu
-0003c220: 714d 6d4b 6731 6957 7067 3841 634b 5069  qMmKg1iWpg8AcKPi
-0003c230: 6674 6c37 3368 5858 2b38 694f 2b38 2f47  ftl73hXX+8iO+8/G
-0003c240: 6770 3239 3648 4c72 576b 6253 6849 4c74  gp296HLrWkbShILt
-0003c250: 5253 6d79 4354 3174 2b62 447a 4536 6844  RSmyCT1t+bDzE6hD
-0003c260: 6867 6159 4942 5671 5967 4152 6138 5974  hgaYIBVqYgARa8Yt
-0003c270: 7563 2f70 5061 6e6d 3337 2b73 2f68 5635  uc/pPanm37+s/hV5
-0003c280: 304e 4a79 6458 3646 587a 6e55 6567 3836  0NJydX6FXznUeg86
-0003c290: 5467 3951 306e 4c32 2f59 6c64 5676 536c  Tg9Q0nL2/YldVvSl
-0003c2a0: 537a 7239 6755 7141 2b52 6863 4131 7453  Szr9gUqA+RhcA1tS
-0003c2b0: 7271 6856 516d 6a6f 6141 2b58 5336 5a67  rqhVQmjoaA+XS6Zg
-0003c2c0: 664f 7379 7974 6639 7937 6e37 7943 6d66  fOsyytf9y7n7yCmf
-0003c2d0: 4753 782b 796c 687a 4d37 3330 484e 756f  GSx+ylhzM730HNuo
-0003c2e0: 494f 464d 4c47 4664 4245 5354 4249 3449  IOFMLGFdBESTBI4I
-0003c2f0: 6457 4d48 706f 5530 5964 766d 4f4c 3144  dWMHpoU0YdvmOL1D
-0003c300: 4345 4f79 6a42 5532 5a4f 7836 3532 6635  CEOyjBU2ZOx652f5
-0003c310: 6f30 552b 5a36 366c 2f41 3033 4668 4755  o0U+Z66l/A03FhGU
-0003c320: 524d 4271 7470 4445 4837 5744 5357 4232  RMBqtpDEH7WDSWB2
-0003c330: 332b 6157 7065 7563 315a 764e 376f 5437  3+aWpeuc1ZvN7oT7
-0003c340: 6c79 5545 4931 3156 3564 4243 596c 514b  lyUEI11V5dBCYlQK
-0003c350: 7054 5841 494c 732b 6c76 574f 5748 336e  pTXAILs+lvWOWH3n
-0003c360: 7052 3354 7841 354f 4364 4232 5355 7335  pR3TxA5OCdB2SUs5
-0003c370: 5732 6169 7379 3777 6d51 714a 4531 3145  W2aisy7wmQqJE11E
-0003c380: 4376 3161 3831 2b66 6f4e 7a4c 3965 6838  Cv1a81+foNzL9eh8
-0003c390: 4f70 3939 6651 3170 4c6d 4838 3936 3056  Op99fQ1pLmH8960V
-0003c3a0: 7353 7457 4a49 4468 6e67 7947 6f4b 6c33  sStWJIDhngyGoKl3
-0003c3b0: 6652 434e 4b38 6271 4153 4565 554d 4e64  fRCNK8bqASEeUMNd
-0003c3c0: 5978 462b 652f 5750 6e35 772f 3877 5872  YxF+e/WPn5w/8wXr
-0003c3d0: 2f50 3431 4944 4e2f 6e53 4149 6768 4f39  /P41IDN/nSAIghO9
-0003c3e0: 5973 4341 5a68 4d38 634b 6268 7477 534b  YsCAZhM8cKbhtwSK
-0003c3f0: 4544 3451 4241 6b6b 6243 4953 4559 5134  ED4QBAkkbCISEYQ4
-0003c400: 5458 674a 596c 5743 4e72 637a 3579 7a4d  TXgJYlWCNrcz5yzM
-0003c410: 764a 2f38 3638 324b 2b72 7531 5a4f 436e  vJ/8682K+ru1ZOCn
-0003c420: 6f43 7775 6d54 5079 5a75 6c42 4561 5547  oCwumTPyZulBEaUG
-0003c430: 6474 4341 5a70 492b 414a 6679 5843 415a  dtCAZpI+AJfyXCAZ
-0003c440: 4744 6664 486d 5572 796b 5256 3848 7154  GDfdHmUrykRV8HqT
-0003c450: 5067 6979 546c 6831 782b 612f 5848 4867  PgiyTlh1x+a/XHHg
-0003c460: 6c76 724f 696f 664b 576c 456b 776d 3437  lvrOiofKWlEkwm47
-0003c470: 614b 686b 564d 306b 334c 5263 3061 6944  aKhkVM0k3LRc0aiD
-0003c480: 4377 312b 4b31 367a 3973 7a76 3061 3776  Cw1+K16z9szv0a7v
-0003c490: 6374 686d 2b55 2f41 326a 6256 5645 6b42  cthm+U/A2jbVVEkB
-0003c4a0: 7047 4f6f 4471 6d4c 4b44 4e49 6f43 4b30  pGOoDqmLKDNIoCK0
-0003c4b0: 4861 536f 4944 3261 5951 4b71 4a41 6f49  HaSoID2aYQKqJAoI
-0003c4c0: 7a71 5241 4674 727a 6851 5837 4851 3163  zqRAFtrzhQX7HQ1c
-0003c4d0: 3466 336c 756c 6978 6770 3166 4573 4277  4f3lulixgp1fEsBw
-0003c4e0: 6679 4947 4573 4377 4c5a 7331 6343 4273  fyIGEsCwLZs1cCBs
-0003c4f0: 567a 7057 3075 4158 7033 4a59 5170 3355  VzpW0uAXp3JYQp3U
-0003c500: 3839 4452 4145 7072 4567 7966 7866 4964  89DRAEprEgyfxfId
-0003c510: 3973 7167 352f 6475 4862 7244 656e 2f64  9sqg5/duHbrDen/d
-0003c520: 4456 7644 552f 312b 486f 734e 3955 3345  DVvDU/1+HosN9U3E
-0003c530: 5370 7234 6b7a 4834 555a 7770 7367 5a6d  Spr4kzH4UZwpsgZm
-0003c540: 325a 4249 6939 6941 6767 626c 672b 3032  2ZBIi9iAggblg+02
-0003c550: 672f 6168 674a 7739 5a64 7668 6c62 3676  g/ahgJw9Zdvhlb6v
-0003c560: 4545 706a 3139 4b71 305a 6d44 5452 704b  EEpj19Kq0ZmDTRpK
-0003c570: 5650 5532 7644 494c 6f42 6773 614d 4244  VPU2vDILoBgsaMBD
-0003c580: 6d6f 4f6d 677a 4664 7a38 642b 5076 6433  moOmgzFdz8d+Pvd3
-0003c590: 3353 3750 6351 7549 4979 5045 4c4d 4f56  3S7PcQuIIyPELMOV
-0003c5a0: 5566 6f42 5a72 7967 4f77 6877 6752 476e  UfoBZrygOwhwgRGn
-0003c5b0: 5a57 6f5a 5a6a 464c 475a 7459 742b 4775  ZWoZZjFLGZtYt+Gu
-0003c5c0: 734e 7a36 3677 6237 3537 332b 3050 6c33  sNz66wb7573+0Pl3
-0003c5d0: 5369 7030 6270 6854 6748 4c44 546f 3565  Sip0bphTgHLDTo5e
-0003c5e0: 7762 4176 6d48 6b67 4977 5955 4677 384a  wbAvmHkgIwYUFw8J
-0003c5f0: 6777 5467 754b 6833 7951 6835 4446 4f46  gwTguKh3yQh5DFOF
-0003c600: 4466 7651 6f53 4249 6364 6a57 3379 6572  DfvQoSBIcdjW3yer
-0003c610: 3758 3334 7a39 612f 584c 754f 4e62 632f  7X34z9a/XLuONbc/
-0003c620: 4166 7567 4777 6b72 6f75 6f53 5642 4551  AfugGwkrouoSVBEQ
-0003c630: 365a 5651 596d 3436 6a51 5a6c 4d42 6857  6ZVQYm46jQZlMBhW
-0003c640: 6f57 4767 6a69 3252 7651 5632 5057 504a  oWGgji2RvQV2PWPJ
-0003c650: 6934 7732 724a 6c30 4d6e 7273 3942 4652  i4w2rJl0Mnrs9BFR
-0003c660: 6135 7756 6745 4e46 4a49 674b 6c6f 6c45  a5wVgENFJIgKlolE
-0003c670: 4251 797a 5655 4e46 5169 524a 6452 7a73  BQyzVUNFQiRJdRzs
-0003c680: 4366 6958 782f 5548 4858 386d 5a6d 417a  CfiXx/UHHX8mZmAz
-0003c690: 5434 3365 564e 346d 7570 3553 4e4a 6f66  T43eVN4mup5SNJof
-0003c6a0: 5741 3574 5251 4549 524c 6c76 5439 494a  WA5tRQEIRLlvT9IJ
-0003c6b0: 3931 2b4f 5832 4839 2b39 6e58 5733 4159  91+OX2H9+9nXW3AY
-0003c6c0: 4e71 6a6f 354e 4378 3444 4548 6541 736f  Nqjo5NCx4DEHeAso
-0003c6d0: 4575 7342 6730 474d 6376 516a 3644 4c4f  EusBg0GMcvQj6DLO
-0003c6e0: 6754 646b 6868 2f51 674f 7765 4a35 4947  gTdkhh/QgOweJ5IG
-0003c6f0: 4d51 426a 7577 7841 4e76 516f 4d79 5478  MQBjuwxANvQoMyTx
-0003c700: 584a 6a7a 774b 7334 3763 3963 6b62 3333  XJjzwKs47c9ckb33
-0003c710: 7742 7576 6679 3236 526e 722f 5331 4b6e  wBuvfy26Rnr/S1Kn
-0003c720: 6376 6757 6771 4e6b 3343 4577 7947 4979  cvgWgqNk3CEwyGIy
-0003c730: 4a6f 434e 4b61 434d 4932 4859 5442 4e63  JoCNKaCMI2HYTBNc
-0003c740: 5672 4d53 6b78 5964 666a 6c66 4367 4161  VrMSkxYdfjlfCgAa
-0003c750: 6442 4b36 7656 5156 6c4b 4c5a 564a 6972  dBK6vVQVlKLZVJir
-0003c760: 4367 3142 4452 5136 4761 6272 6759 4859  Cg1BDRQ6GabrgYHY
-0003c770: 652f 4c32 424a 7a37 6e4e 7851 4f67 6e56  e/L2BJz7nNxQOgnV
-0003c780: 7667 6836 7378 3857 7744 6655 4c6f 6373  vgh6sx8WwDfULocs
-0003c790: 724c 714d 6a63 6752 4b49 4b58 7272 6252  rLqMjcgRKIKXrrbR
-0003c7a0: 656e 5031 6a2b 3772 3766 386b 2f6d 4139  enP1j+7r7f8k/mA9
-0003c7b0: 7a44 5430 424a 362b 4251 796e 6f2f 746a  zDT0BJ6+BQyno/tj
-0003c7c0: 5238 636f 5664 4834 6941 5249 4341 4c4e  R8coVdH4iARICALN
-0003c7d0: 786e 4a48 5430 6f34 7350 7441 4279 4748  xnJHT0o4sPtAByGH
-0003c7e0: 4476 6b67 5872 2f6c 7947 3132 5142 524e  DvkgXr/lyG12QBRN
-0003c7f0: 366e 4c2f 514a 4236 4759 4659 3261 7958  6nL/QJB6GYFY2ayX
-0003c800: 7665 6571 5239 5038 382f 7733 6530 7659  veeqR9P88/w3e0vY
-0003c810: 6958 6a4f 6a75 6946 3050 5a57 416f 4b78  iXjOjuiF0PZWAoKx
-0003c820: 4556 524f 4245 4b5a 726f 5944 6e41 5362  EVROBEKZroYDnASb
-0003c830: 6641 4c39 7738 4a49 5847 712f 7579 4775  fAL9w8JIXGq/uyGu
-0003c840: 3067 396d 492b 6756 366b 5970 4235 326e  0g9mI+gV6kYpB52n
-0003c850: 574c 6169 6f49 5662 5961 7362 5533 7434  WLaioIVbYasbU3t4
-0003c860: 4273 4f4e 5235 304d 355a 3565 7062 6635  BsONR50M5Z5epbf5
-0003c870: 6437 3177 4659 2f56 6a6f 584e 2f69 4b75  d71wFY/VjoXN/iKu
-0003c880: 7154 5a6a 744b 646d 2b44 414f 4947 4850  qTZjtKdm+DAOIGHP
-0003c890: 4a4f 6d41 5862 4758 6a55 3962 6454 3139  JOmAXbGXjU9bdT19
-0003c8a0: 7033 2f66 734f 7979 6668 3061 457a 6f76  p3/fsOyyfh0aEzov
-0003c8b0: 7a43 6951 486e 766b 3944 364a 6d4b 4156  zCiQHnvk9D6JmKAV
-0003c8c0: 396d 3159 4451 6d42 6e67 4e6d 354c 3451  9m1YDQmBngNm5L4Q
-0003c8d0: 3043 3861 4e6e 5941 6649 3854 374a 4237  0C8aNnYAfI8T7JB7
-0003c8e0: 5144 4169 4752 4245 4639 454b 7749 6477  QDAiGRBEF9EKwIdw
-0003c8f0: 6d36 4469 6874 3378 754a 3242 756b 7668  m6Diht3xuJ2Bukvh
-0003c900: 6b63 5850 6d7a 7365 7673 7a39 5a63 694e  kcXPmzsevsz9ZciN
-0003c910: 7365 4632 3766 5974 496f 7849 6767 3147  seF27fYtIoxIgg1G
-0003c920: 4466 514e 4c6d 4164 3077 624a 4d2b 7450  DfQNLmAd0wbJM+tP
-0003c930: 7474 747a 5253 7736 372f 4833 7747 7345  tttzRSw67/H3wGsE
-0003c940: 7136 3458 5a69 506f 4675 6c4b 4c79 3668  q64XZiPoFulKLy6h
-0003c950: 3064 4474 4269 6f59 4647 6b55 6d33 5a44  0dDtBioYFGkUm3ZD
-0003c960: 7261 5570 4444 4954 5370 7a43 6557 625a  raUpDDITSpzCeWbZ
-0003c970: 4d73 6c79 6563 7867 6171 4533 6f4c 5769  MslyecxgaqE3oLWi
-0003c980: 7068 4c47 7049 4c42 7063 3346 4641 4241  phLGpILBpc3FFABA
-0003c990: 562b 412f 3758 612f 4143 6e6e 6741 6e52  V+A/7Xa/ACnngAnR
-0003c9a0: 576e 4363 4948 3469 6850 4159 7534 4558  WnCcIH4ihPAYu4EX
-0003c9b0: 774a 6962 587a 372f 696c 7346 6232 4e44  wJibXz7/ilsFb2ND
-0003c9c0: 7646 516d 6774 2b4e 2f31 6151 4634 2b71  vFQmgt+N/1aQF4+q
-0003c9d0: 6569 4d71 4863 5279 6e6b 6566 4264 4c55  eiMqHcRynkefBdLU
-0003c9e0: 4b65 5345 7344 2b59 7252 454b 3849 6962  KeSEsD+YrREK8Iib
-0003c9f0: 416b 3641 3345 666d 437a 584b 754c 3332  Ak6A3EfmCzXKuL32
-0003ca00: 665a 6d6e 462b 3645 6b71 546f 4d4a 6344  fZmnF+6EkqToMJcD
-0003ca10: 736f 386c 6a41 7054 6777 3654 6772 6331  so8ljApTgw6Tgrc1
-0003ca20: 4c31 6b58 5038 3948 3237 6743 5133 5777  L1kXP89H27gCQ3Ww
-0003ca30: 7656 4541 6142 5248 564b 7865 5634 5545  vVEAaBRHVKxeV4UE
-0003ca40: 5131 4636 6d6b 794a 414d 5472 4b77 4234  Q1F6mkyJAMTrKwB4
-0003ca50: 4144 3551 3557 4562 6e45 7964 4f74 4862  AD5Q5WEbnEydOtHb
-0003ca60: 3731 7132 3943 7639 3131 4c57 7972 7670  71q29Cv911LWyrvp
-0003ca70: 526d 4354 6a76 792b 6d54 4759 6253 6b51  RmCTjvy+mTGYbSkQ
-0003ca80: 6a35 636c 6856 4571 6b48 3730 696d 7043  j5clhVEqkH70impC
-0003ca90: 4465 6830 727a 702f 3843 7a62 6c6b 4c31  Deh0rzp/8CzblkL1
-0003caa0: 5a4f 7045 3035 4d41 4f54 5a30 6179 5947  ZOpE05MAOTZ0ayYG
-0003cab0: 722b 6470 7241 4967 4545 5649 5942 445a  r+dprAIgEEVIYBDZ
-0003cac0: 7442 3262 686a 5153 3144 566a 5145 366b  tB2bhjQS1DVjQE6k
-0003cad0: 4c58 7041 4e68 3234 344c 3847 6846 6844  LXpANh244L8GhFhD
-0003cae0: 5474 3245 6950 3770 2f2f 3977 334a 762f  Tt2EiP7p//9w3Jv/
-0003caf0: 4148 7a66 384b 7035 772b 7258 6644 364d  AHzf8Kp5w+rXfD6M
-0003cb00: 6152 556d 6c55 716a 6a67 5646 4c51 6833  aRUmlUqjjgVFLQh3
-0003cb10: 7338 432b 7252 6778 3464 7444 4450 782f  s8C+rRgx4dtDDPx/
-0003cb20: 5070 6b2f 556c 412f 6165 774f 4962 6b73  Ppk/UlA/aewOIbks
-0003cb30: 7046 4562 4b72 5852 5579 4242 4c42 6162  pFEbKrXRUyBBLBab
-0003cb40: 6479 4742 304d 4a61 3059 2b6e 426f 6669  dyGB0MJa0Y+nBofi
-0003cb50: 554b 564f 5148 487a 7462 5265 4d39 3763  UKVOQHHztbReM97c
-0003cb60: 662b 6869 7a2b 5066 4254 6738 5945 6b6a  f+hiz+PfBTg8YEkj
-0003cb70: 6f62 5255 646f 4569 3567 597a 6b30 346c  obRUdoEi5gYzk04l
-0003cb80: 424c 5579 6568 4e50 584f 3253 584b 397a  BLUyehNPXO2SXK9z
-0003cb90: 4c54 376d 5162 6465 7646 7230 477a 5457  LT7mQbdevFr0GzTW
-0003cba0: 6755 304e 6563 4346 7176 7548 446e 4d4c  gU0NecCFqvuHDnML
-0003cbb0: 4b65 3735 4e2f 3246 712f 5543 6955 4b35  Ke75N/2Fq/UCiUK5
-0003cbc0: 7377 634f 3569 4152 4b30 505a 7771 415a  swcO5iARK0PZwqAZ
-0003cbd0: 704e 4c75 6e4b 3130 4a75 6a72 6d6e 727a  pNLunK10Jujrmnrz
-0003cbe0: 6677 626d 7648 504a 7a32 6150 3251 466a  fwbmvHPJz2aP2QFj
-0003cbf0: 4c55 5658 464f 714e 4552 5064 4478 774f  LUVXFOqNERPdDxwO
-0003cc00: 5651 6f70 514c 6d55 6b45 794b 7767 532b  VQopQLmUkEyKwgS+
-0003cc10: 445a 512b 5764 7034 5a64 4d43 582f 6d76  DZQ+Wdp4ZdMCX/mv
-0003cc20: 7339 436e 6832 3454 746a 3057 4134 7332  s9Cnh24Ttj0WA4s2
-0003cc30: 7062 536d 624e 716f 496e 5467 7147 6431  pbSmbNqoInTgqGd1
-0003cc40: 5045 4e31 5170 7433 4945 4e46 4446 5854  PEN1Qpt3IENFDFXT
-0003cc50: 5861 3063 4d48 4534 424f 646a 7372 2b31  Xa0cMHE4BOdjsr+1
-0003cc60: 6276 2b62 7562 3130 6c65 3159 3944 2f59  bv+bub10le1Y9D/Y
-0003cc70: 4a30 4945 6776 6379 3253 6735 5155 4736  J0IEgvcy2Sg5QUG6
-0003cc80: 6f71 4b51 6f53 745a 5250 2b69 3533 4571  oqKQoStZRP+i53Eq
-0003cc90: 7951 6230 6e65 7064 392b 5470 782f 4837  yQb0nepd9+Tpx/H7
-0003cca0: 6a5a 6371 3277 5234 4d70 376a 7277 6967  jZcq2wR4Mp7jrwig
-0003ccb0: 2b36 7771 556e 5152 3545 392b 4834 5748  +6wqUnQR5E9+H4WH
-0003ccc0: 4252 5749 6853 514b 6934 4d41 4c30 7232  BRWIhSQKi4MAL0r2
-0003ccd0: 5241 2f75 3058 5872 6952 6437 756f 7935  RA/u0XXriRd7uoy5
-0003cce0: 6869 5551 2f58 5447 4171 7075 4332 6266  hiUQ/XTGAqpuC2bf
-0003ccf0: 4145 4d6d 6d46 5a4d 6579 644c 4f46 6b6a  AEMmmFZMeydLOFkj
-0003cd00: 5a43 3572 376d 6f62 3939 3335 3077 434d  ZC5r7mob99350wCM
-0003cd10: 3354 6f42 326a 2f61 6449 704b 6f54 5a67  3ToB2j/adIpKoTZg
-0003cd20: 5641 575a 7a45 524f 694a 4671 5271 4141  VAWZzEROiJFqRqAA
-0003cd30: 5045 7532 5170 6955 5235 6743 6a32 7134  PEu2QpiUR5gCj2q4
-0003cd40: 7046 546c 674f 4456 7837 4c54 4570 7a38  pFTlgODVx7LTEpz8
-0003cd50: 395a 594b 3979 3468 6e34 6351 3648 524c  9ZYK9y4hn4cQ6HRL
-0003cd60: 434a 3239 4c31 772f 6951 6141 5146 7453  CJ29L1w/iQaAQFtS
-0003cd70: 2b54 4243 6b6d 5942 2b78 6f67 6d36 4c6e  +TBCkmYB+xogm6Ln
-0003cd80: 7035 4544 2f71 4432 7538 432b 6665 6a34  p5ED/qD2u8C+fej4
-0003cd90: 664f 6269 6e38 4631 7067 7865 5130 4d46  fObin8F1pgxeQ0MF
-0003cda0: 3172 6f30 4745 6f47 4931 5a4a 3175 5176  1ro0GEoGI1ZJ1uQv
-0003cdb0: 6a72 4151 3470 6171 715a 5036 6b41 2f62  jrAQ4paqqZP6kA/b
-0003cdc0: 506e 6e58 6f54 3258 2f6e 704f 6743 5744  PnnXoT2X/npOgCWD
-0003cdd0: 496f 796f 432b 556b 7152 5066 4453 4e33  IoyoC+UkqRPfDSN3
-0003cde0: 4f48 6558 4456 4a57 6832 4961 684d 6342  OHeXDVJWh2IahMcB
-0003cdf0: 4a42 3343 5935 6467 7a2b 3539 3734 3256  JB3CY5dgz+59742V
-0003ce00: 442f 2f72 3948 6d68 5669 6671 5949 4553  D//r9HmhVifqYIES
-0003ce10: 7741 567a 5a62 4e59 456f 6136 6a6c 5977  wAVzZbNYEoa6jlYw
-0003ce20: 4b47 6d4a 464a 436a 4251 5171 506c 7645  KGmJFJCjBQQqPlvE
-0003ce30: 6777 5842 7168 3750 327a 717a 3532 6e48  gwXBqh7P2zqz52nH
-0003ce40: 582b 3958 4a70 3841 3848 6734 5048 5342  X+9XJp8A8Hg4PHSB
-0003ce50: 6177 3679 6e70 5249 5147 496c 6852 4563  aw6ynpRIQGIlhREc
-0003ce60: 4552 5558 5770 634e 7238 7448 5078 4e47  ERUXWpcNr8tHPxNG
-0003ce70: 6b46 4256 7952 7737 7564 6242 3734 6248  kFBVyRw7udbB74bH
-0003ce80: 5865 4363 644d 4835 6a6d 4345 7447 3378  XeCcdMH5jmCEtG3x
-0003ce90: 4475 4768 7a41 4a6e 502b 3136 2f48 706e  DuGhzAJnP+16/Hpn
-0003cea0: 7378 6364 6335 4f30 392b 6b4b 5764 5054  sxcdc5O09+kKWdPT
-0003ceb0: 2f32 6444 6c42 2f56 5667 5970 4355 4c51  /2dDlB/VVgYpCULQ
-0003cec0: 6653 6759 774e 674c 6d56 544c 4d6f 6d78  fSgYwNgLmVTLMomx
-0003ced0: 4246 4245 6d31 7342 7336 4871 3364 2b38  BFBEm1sBs6Hq3d+8
-0003cee0: 6e2b 7a31 792f 6334 6465 7050 534d 6749  n+z1y/c4depPSMgI
-0003cef0: 524c 6165 7930 6530 4543 526f 7130 6d4c  RLaey0e0ECRoq0mL
-0003cf00: 7462 4342 4d55 2b4d 6b66 4461 4d52 4e62  tbCBMU+MkfDaMRNb
-0003cf10: 2b2f 6876 374a 5937 6137 7846 754f 5a63  +/hv7JY7a7xFuOZc
-0003cf20: 414c 3953 2f53 3141 2f43 4652 6549 3555  AL9S/S1A/CFReI5U
-0003cf30: 4945 6a45 6f73 5946 772f 5362 6f61 4635  IEjEosYFw/SboaF5
-0003cf40: 786d 556f 476d 5243 4271 6853 5648 4267  xmUoGmRCBqhSVHBg
-0003cf50: 3553 7966 372b 6f66 7666 726e 2f6f 7a50  5Syf7+ofvfrn/ozP
-0003cf60: 4f46 574f 4734 426c 3273 7943 7255 6e62  OFWOG4Bl2syCrUnb
-0003cf70: 684b 3550 3279 5639 3437 4857 6964 3933  hK5P2yV947HWid93
-0003cf80: 6563 425a 5872 7730 5837 5273 714b 6969  ecBZXrw0X7RsqKii
-0003cf90: 4f49 3354 4c42 5846 5158 6238 4238 6f6b  OI3TLBXFQXb8B8ok
-0003cfa0: 6751 6165 4675 7848 6141 6d4d 6738 5563  gQaeFuxHaAmMg8Uc
-0003cfb0: 3654 746a 3374 437a 3778 5146 6676 6547  6Ttj3tCz7xQFfveG
-0003cfc0: 5333 6e64 6459 6236 736f 6744 357a 5361  S3nddYb6sogD5zSa
-0003cfd0: 6936 775a 7245 304b 7455 6d47 7553 6e51  i6wZrE0KtUmGuSnQ
-0003cfe0: 6242 6e7a 764b 3164 4271 7759 5476 2b4b  bBnzvK1dBqwYTv+K
-0003cff0: 6867 6748 5a73 7259 6e2f 357a 6465 6268  hggHZsrYn/5zdebh
-0003d000: 766e 6237 666c 5379 5476 4232 494d 524c  vnb7flSyTvB2IMRL
-0003d010: 7373 4471 6b71 7839 7541 454d 644d 5645  ssDqkqx9uAEMdMVE
-0003d020: 6430 544b 7734 5138 662f 6c76 642b 4a4a  d0TKw4Q8f/lvd+JJ
-0003d030: 312b 3850 5838 4c62 6368 334a 6772 7848  1+8PX8Lbch3JgrxH
-0003d040: 6363 5872 5159 5454 3574 416a 7270 7449  ccXrQYTT5tAjrptI
-0003d050: 6f46 7053 6e4a 4f61 4259 5967 7436 3674  oFpSnJOaBYYgt66t
-0003d060: 4869 6233 4837 4d38 6365 7748 2f7a 3749  Hib3H7M8cewH/z7I
-0003d070: 314f 4c76 4742 4d70 5541 6f37 7252 4262  1OLvGBMpUAo7rRBb
-0003d080: 776c 4f53 4178 4f67 6850 5174 6650 2b5a  wlOSAxOghPQtfP+Z
-0003d090: 6373 6550 5130 3254 4371 6158 4d43 4d67  csePQ02TCqaXMCMg
-0003d0a0: 5443 6769 4b4a 4b71 4245 7171 5936 4973  TCgiKJKqBEqqY6Is
-0003d0b0: 3265 2b57 3668 3672 2f2f 744a 5052 4359  2e+W6h6r//tJPRCY
-0003d0c0: 3158 2f53 6f32 6f46 7869 3461 6b70 6674  1X/So2oFxi4akpft
-0003d0d0: 476d 7247 5a4a 4544 5176 556e 6776 7249  GmrGZJEDQvUngvrI
-0003d0e0: 3042 4566 594e 5658 4831 4577 3935 4b30  0BEfYNVXH1Ew95K0
-0003d0f0: 5776 2f65 4b6d 7647 447a 6f43 6a67 7363  Wv/eKmvGDzoCjgsc
-0003d100: 474e 304c 4335 4e64 4342 5367 352b 372b  GN0LC5NdCBSg5+7+
-0003d110: 322b 3535 3944 7932 5669 4c49 4862 4774  2+559Dy2ViLIHbGt
-0003d120: 692f 4b70 4877 6c64 7577 364f 4a45 5332  i/KpHwlduw6OJES2
-0003d130: 3054 636f 476d 5863 7634 306e 6e55 6a67  0TcoGmXcv40nnUjg
-0003d140: 7375 3042 6365 7a2f 5630 4a53 725a 4830  su0Bcez/V0JSrZH0
-0003d150: 5631 5461 7442 7a61 5542 5865 4e39 6570  V1TatBzaUBXeN9ep
-0003d160: 4874 3747 4858 6e6c 664e 4f66 7766 5356  Ht7GHXnlfNOfwfSV
-0003d170: 626a 4f68 664c 3038 3739 4251 7870 4f2b  bjOhfL0879BQxpO+
-0003d180: 5263 5044 3132 3357 3070 6c6f 6e6b 4344  RcPD123W0plonkCD
-0003d190: 4375 6b57 4553 5664 532b 6e36 4f4c 3172  CukWESVdS+n6OL1r
-0003d1a0: 3951 764c 655a 782b 7756 7137 466c 3850  9QvLeZx+wVq7Fl8P
-0003d1b0: 5743 7878 692b 5737 4239 5937 6662 3364  WCxxi+W7B9Y7fb3d
-0003d1c0: 7633 3533 4f5a 756e 4549 4c55 3543 674e  v353OZunEILU5CgN
-0003d1d0: 5a74 6978 556a 574c 7959 5943 7642 4f51  ZtixUjWLyYYCvBOQ
-0003d1e0: 4c53 314b 7666 7671 6235 4b73 6666 7751  LS1Kvfvqb5KsffwQ
-0003d1f0: 6578 4d57 376a 766d 7832 2f66 4f54 3972  exMW7jvmx2/fOT9r
-0003d200: 6c50 4647 5850 6869 3667 6a70 5a42 7474  lPFGXPhi6gjpZBtt
-0003d210: 5855 6d32 6741 3576 3642 5470 6b57 4164  XUm2gA5v6BTpkWAd
-0003d220: 6e6e 4676 672b 4577 4330 6b77 3032 794b  nnFvg+EwC0kw02yK
-0003d230: 4154 7245 7749 4345 744f 5733 5663 542b  ATrEwICEtOW3VcT+
-0003d240: 4d58 356a 7143 4f4e 5841 6b48 7753 2b59  MX5jqCONXAkHwS+Y
-0003d250: 6c6a 616b 6b2f 6969 4142 5938 7946 3541  ljakk/iiABY8yF5A
-0003d260: 5872 7851 7047 304c 6e4c 5632 6659 6962  XrxQpG0LnLV2fYib
-0003d270: 5155 6d57 4241 442b 3173 3662 7852 5862  QUmWBAD+1s6bxRXb
-0003d280: 2f43 2f65 7739 2b65 7468 5133 4369 5674  /C/ew9+ethQ3CiVt
-0003d290: 5965 4a39 4265 6837 6e4b 6363 5758 7a35  YeJ9Beh7nKccWXz5
-0003d2a0: 344c 376e 5044 7165 7a54 416f 3661 4c67  4L7nPDqezTAo6aLg
-0003d2b0: 4e4a 5547 5938 7251 3932 4c61 5247 4b4c  NJUGY8rQ92LaRGKL
-0003d2c0: 4141 444f 3335 6862 614c 3836 2b4c 2f48  AADO35hbaL86+L/H
-0003d2d0: 4572 412b 3538 4657 474d 7643 4744 366a  ErA+58FWGMvCGD6j
-0003d2e0: 506e 3744 6643 574a 517a 304f 684f 6b54  Pn7DfCWJQz0OhOkT
-0003d2f0: 5173 4b7a 4964 6e55 5a61 7673 6d5a 7053  QsKzIdnUZavsmZpS
-0003d300: 497a 6663 4c39 6f71 475a 3149 507a 336f  IzfcL9oqGZ1IPz3o
-0003d310: 6773 5854 314f 7039 6265 4974 6677 4c5a  gsXT1Op9beItfwLZ
-0003d320: 3976 5066 4971 6d7a 5765 7678 2b52 3776  9vPfIqmzWevx+R7v
-0003d330: 442b 7077 464e 7072 626c 4f34 6268 5561  D+pwFNprblO4bhUa
-0003d340: 5053 464a 4442 5141 4b50 514d 4870 7a7a  PSFJDBQAKPQMHpzz
-0003d350: 3163 5473 4673 4643 574d 4169 4642 494b  1cTsFsFCWMAiFBIK
-0003d360: 6347 424f 6b51 7842 4270 4d7a 6f39 714c  cGBOkQxBBpMzo9qL
-0003d370: 4756 424a 2f46 4b69 4946 7145 4e34 306f  GVBJ/FKiIFqEN40o
-0003d380: 4a44 6969 6939 4742 6f71 624a 416b 4865  JDiii9GBoqbJAkHe
-0003d390: 5873 5463 2b2b 614e 392f 7774 7665 666b  XsTc++aN9/wtvefk
-0003d3a0: 4373 4133 3669 3552 3072 3847 3259 5a4b  CsA36i5R0r8G2YZK
-0003d3b0: 4d4f 6c35 7168 6150 4d2b 2f57 7338 7334  MOl5qhaPM+/Ws8s4
-0003d3c0: 3763 716f 5930 6d63 5374 2b7a 676a 6236  7cqoY0mcSt+zgjb6
-0003d3d0: 6776 4e4a 7447 346b 6843 704e 5035 3445  gvNJtG4khCpNP54E
-0003d3e0: 7958 4776 6869 7164 5466 332f 3549 6235  yXGvhiqdTf3/5Ib5
-0003d3f0: 3454 5a4e 4f4a 4968 3077 7645 6e37 7270  4TZNOJIh0wvEn7rp
-0003d400: 5434 6343 7835 3741 6b58 7270 5643 4d75  T4cCx57AkXrpVCMu
-0003d410: 4b62 4665 5851 5149 4d4f 6955 7747 7874  KbFeXQQIMOiUwGxt
-0003d420: 7679 6331 5076 6a4c 6e76 314f 7666 5077  vyc1PvjLnv1OvfPw
-0003d430: 5a6e 6745 4533 6d37 454e 7867 6c55 4a53  ZngEE3m7ENxglUJS
-0003d440: 4941 6a4b 4244 784d 4468 7661 7261 5474  IAjKBDxMDhvaraTt
-0003d450: 3277 7356 2b62 6671 4139 7436 4577 6e44  2wsV+bfqA9t6EwnD
-0003d460: 3757 7164 5332 746c 5144 5979 6b4b 3173  7WqdS2tlQDYykK1s
-0003d470: 5168 454c 6c69 776d 7950 6f78 662b 5444  QhELliwmyPoxf+TD
-0003d480: 2b79 7a51 6159 6755 4e32 3047 6a46 6830  +yzQaYgUN20GjFh0
-0003d490: 516e 6266 5552 716f 4a74 4d53 7330 4430  QnbfURqoJtMSs0D0
-0003d4a0: 3874 7172 7852 6566 2b35 2b2b 5263 7859  8tqrxRef+5++RcxY
-0003d4b0: 3067 6848 3644 4a7a 7168 4834 7745 4f50  0ghH6DJzqhH4wEOP
-0003d4c0: 3078 4330 2b4f 4b6a 6142 5238 6d46 4d6d  0xC0+OKjaBR8mFMm
-0003d4d0: 554c 5937 6362 6179 594e 4834 6153 7955  ULY7cbayYNH4aSyU
-0003d4e0: 4777 4b62 434e 7350 7954 466b 6b6c 4178  GwKbCNsPyTFkklAx
-0003d4f0: 7367 546d 536a 7046 7359 626e 7a30 7077  sgTmSjpFsYbnz0pw
-0003d500: 2f4f 302b 2f4f 3574 376e 7643 3336 314e  /O0+/O5t7nvC361N
-0003d510: 624f 5057 674d 2f30 2b39 5876 4257 5477  bOPWgM/0+9XvBWTw
-0003d520: 6b6f 746b 4752 6255 7432 4a59 4b56 4253  kotkGRbUt2JYKVBS
-0003d530: 4369 4954 756e 6e4d 5772 586f 712f 6367  CiITunnMWrXoq/cg
-0003d540: 6244 316b 726d 6c75 4141 4a51 4b4e 6365  bD1krmluAAJQKNce
-0003d550: 4859 5941 6b6e 4f37 4c41 4563 6778 514b  HYYAknO7LAEcgxQK
-0003d560: 756f 414a 7154 6362 4b48 5435 7533 384c  uoAJqTcbKHT5u38L
-0003d570: 4967 6439 6b74 7645 6d46 474a 5156 495a  Igd9ktvEmFGJQVIZ
-0003d580: 5374 6232 7344 5541 3248 5665 4a57 6d71  Stb2sDUA2HVeJWmq
-0003d590: 3730 6d4f 4372 412f 6a56 6a78 6339 4630  70mOCrA/jVjxc9F0
-0003d5a0: 7352 4647 4849 6c6e 556f 4947 6477 704b  sRFGHIlnUoIGdwpK
-0003d5b0: 3853 6b42 677a 4b6a 6b76 5a58 3876 626e  8SkBgzKjkvZX8vbn
-0003d5c0: 3338 6e75 6666 6f6d 3146 6344 3577 3143  38nuffom1FcD5w1C
-0003d5d0: 7144 4447 6761 2b6c 314c 4736 6a44 5342  qDDGga+l1LG6jDSB
-0003d5e0: 6363 4447 4676 4f38 4e47 3141 7270 6831  ccDGFvO8NG1Arph1
-0003d5f0: 2b69 687a 5737 7968 4974 7243 676f 4b78  +ihzW7yhItrCgoKx
-0003d600: 4152 477a 4772 4f75 6c45 3069 694a 6e32  ARGzGrOulE0iiJn2
-0003d610: 5274 7865 7365 4a71 7661 467a 6737 7a72  RtxeseJqvaFzg7zr
-0003d620: 7365 4a6c 4a42 5239 6e49 4746 3070 5741  seJlJBR9nIGF0pWA
-0003d630: 5132 5a59 4f36 4b63 6b41 644f 7a68 5157  Q2ZYO6KckAdOzhQW
-0003d640: 4a56 7a2b 364a 7a58 7a2f 5939 7443 3939  JVz+6JzXz/Y9tC99
-0003d650: 394e 3043 2f41 5551 426b 6742 4270 4841  9N0C/AUQBkgBBpHA
-0003d660: 6369 5463 6b69 527a 7741 3938 4344 514b  ciTckiRzwA98CDQK
-0003d670: 3138 6d7a 6633 5856 592f 3759 4464 6a68  18mzf3XVY/7YDdjh
-0003d680: 5831 6d55 4f67 6932 7150 6b4a 6c71 4c4b  X1mUOgi2qPkJlqLK
-0003d690: 5553 7145 4336 435a 5a42 3446 655a 412b  USqEC6CZZB4FeZA+
-0003d6a0: 5351 6830 5145 3252 3949 494c 4145 4574  SQh0QE2R9IILAEEt
-0003d6b0: 484f 3963 4a55 4554 3077 4b61 4d4f 6848  HO9cJUET0wKaMOhH
-0003d6c0: 6a34 4456 574e 7237 4337 6e7a 6b64 3961  j4DVWNr7C7nzkd9a
-0003d6d0: 5331 566b 4738 7774 384b 4259 4a67 6553  S1VkG8wt8KBYJgeS
-0003d6e0: 416b 3661 6c6e 6849 4572 3446 6478 7a78  Ak6alnhIEr4Fdxzx
-0003d6f0: 5271 3846 7a72 6f41 3553 5769 4549 5a69  Rq8FzroA5SWiEIZi
-0003d700: 5963 7642 3463 6441 755a 386d 6139 4642  YcvB4cdAuZ8ma9FB
-0003d710: 6443 5630 6531 4c49 6f44 714b 6b66 6968  dCV0e1LIoDqKkfih
-0003d720: 4e46 676f 7771 6d79 3645 3670 384b 6c6e  NFgowqmy6E6p8Kln
-0003d730: 7067 5332 4936 3044 394d 4146 446d 4c7a  pgS2I60D9MAFDmLz
-0003d740: 3457 5776 7836 6d63 7966 3337 6d66 7236  4WWvx6mcyf37mfr6
-0003d750: 324f 5963 6b67 504f 4178 544a 4a78 3864  2OYckgPOAxTJJx8d
-0003d760: 4836 516b 774e 3442 3935 4443 5378 4975  H6QkwN4B95DCSxIu
-0003d770: 3836 4533 4153 4954 424b 7854 3437 685a  86E3ASITBKxT47hZ
-0003d780: 6b42 5272 4248 4333 6879 4c62 4a45 7734  kBRrBHC3hyLbJEw4
-0003d790: 706a 4f6a 2f56 6468 7664 6265 2b74 4577  pjOj/Vdhvdbe+tEw
-0003d7a0: 4536 4d6f 5742 4948 656f 5631 486c 5948  E6MoWBIHeoV1HlYH
-0003d7b0: 4842 466b 6678 6931 2f53 486b 5151 4966  HBFkfxi1/SHkQQIf
-0003d7c0: 6b30 4e48 5168 7171 784b 786e 5955 4548  k0NHQhqqxKxnYUEH
-0003d7d0: 7065 5776 6b79 782f 6434 547a 3038 7275  peWvkyx/d4Tz08ru
-0003d7e0: 694f 5565 4833 724d 3865 7034 4a58 3077  iOUeH3rM8ep4JX0w
-0003d7f0: 6955 7542 5153 6e64 2f48 4534 7044 6277  iUuBQSnd/HE4pDbw
-0003d800: 4750 7549 4251 7839 3635 4b4d 6374 7539  GPuIBQx965KMctu9
-0003d810: 6636 3531 3978 4d6c 6975 3735 4863 4276  f6519xMliu75HcBv
-0003d820: 6d4a 6c43 6f71 6f59 756e 3154 5451 6253  mJlCoqoYun1TTQbS
-0003d830: 426b 6b78 3678 4762 5367 3753 4954 6376  Bkkx6xGbSg7SITcv
-0003d840: 316b 674d 5432 334b 4c55 732b 2b2b 3373  1kgMT23KLUs+++3s
-0003d850: 5974 7333 6c5a 6537 6563 3865 7838 5836  Yts3lZe7ec8ex8X6
-0003d860: 4b6a 674a 4b76 416b 7336 4547 5941 354a  KjgJKvAks6EGYA5J
-0003d870: 4757 7844 546e 7355 6676 5633 766c 6f4e  GWxDTnsUfvV3vloN
-0003d880: 324f 682b 4758 2f76 6a38 312b 6d54 6752  2Oh+GX/vj81+mTgR
-0003d890: 5476 3468 7536 7169 4643 554b 376a 7049  Tv4hu6qiFCUK7jpI
-0003d8a0: 4264 5234 545a 4c30 6767 7341 6352 4464  BdR4TZL0ggsAcRDd
-0003d8b0: 7030 4a44 7156 3836 4761 7247 3979 4959  p0JDqV86GarG9yIY
-0003d8c0: 5875 3959 3076 6359 6565 7531 652f 7470  Xu9Y0vcYeeu1e/tp
-0003d8d0: 4879 3344 7944 5364 4643 7969 6768 6c4e  Hy3DyDSdFCyighlN
-0003d8e0: 7732 4d30 6341 386b 524a 5161 2b6e 3247  w2M0cA8kRJQa+n2G
-0003d8f0: 3135 5548 6753 3650 7268 307a 4137 4862  15UHgS6Prh0zA7Hb
-0003d900: 7177 5875 4941 3861 654c 6450 4a67 5651  qwXuIA8aeLdPJgVQ
-0003d910: 5a58 5157 7353 3147 644b 4d6d 6b52 3277  ZXQWsS1GdKMmkR2w
-0003d920: 6d50 5569 4c32 4c52 5577 7154 4456 6e51  mPUiL2LRUwqTDVnQ
-0003d930: 794b 6342 306d 5051 2f42 7050 2b66 396f  yKcB0mPQ/BpP+f9o
-0003d940: 4c56 3063 2b6d 6c41 4774 7331 3445 735a  LV0c+mlAGts14EsZ
-0003d950: 5651 4259 6b42 7049 457a 6532 4967 684e  VQBYkBpIEze2IghN
-0003d960: 3561 4442 666f 4b38 4633 625a 394c 3532  5aDBfoK8F3bZ9L52
-0003d970: 3257 6965 5050 386f 6431 4773 6173 7978  2WiePP8od1Gsasyx
-0003d980: 3150 3862 554c 3649 4864 597a 6f68 484a  1P8bUL6IHdYzohHJ
-0003d990: 326e 5251 545a 414e 5142 4e46 5873 534b  2nRQTZANQBNFXsSK
-0003d9a0: 4e70 3972 504b 4246 6232 594f 6862 444c  Np9rPKBFb2YOhbDL
-0003d9b0: 6e72 7251 2f57 6a69 442f 6547 7870 2f46  nrrQ/WjiD/eGxp/F
-0003d9c0: 7972 534b 4866 6f57 5672 6b7a 6866 4150  yrSKHfoWVrkzhfAP
-0003d9d0: 3275 534f 766b 632b 334f 2f74 7545 494e  2uSOvkc+3O/tuEIN
-0003d9e0: 3656 3776 6e48 334f 3675 744b 6c4a 7469  6V7vnH3O6utKlJti
-0003d9f0: 3668 7170 655a 6571 4a45 624c 6f4e 4356  6hqpeZeqJEbLoNCV
-0003da00: 426c 4f35 6255 6270 4b49 7873 4576 4455  BlO5bUbpKIxsEvDU
-0003da10: 374c 2f48 4368 3339 4b50 7633 6578 7831  7L/HCh39KPv3exx1
-0003da20: 3675 6849 6743 6443 6238 4b54 742b 4541  6uhIgCdCb8KTt+EA
-0003da30: 5962 5132 3843 5134 336f 616e 5573 4173  YbQ28CQ43oanUsAs
-0003da40: 3943 4179 317a 4a44 4c41 714c 6b78 6736  9CAy1zJDLAqLkxg6
-0003da50: 4275 636c 4f46 3870 4d45 7639 4674 6132  BuclOF8pMEv9Fta2
-0003da60: 7170 5974 576b 5568 564f 374b 6a4e 4170  qpYtWkUhVO7KjNAp
-0003da70: 4179 476d 7254 7234 364a 6b67 4834 4f4f  AyGmrTr46JkgH4OO
-0003da80: 5750 6451 4b4c 6159 2f48 4b63 6172 6c33  WPdQKLaY/HKcarl3
-0003da90: 4855 4761 7761 7757 6864 6254 4234 7647  HUGawawWhdbTB4vG
-0003daa0: 4731 7266 5933 3536 2b51 3336 7763 4232  G1rfY356+Q36wcB2
-0003dab0: 2b78 6866 3148 4454 584b 4345 484a 4e4b  +xhf1HDTXKCEHJNK
-0003dac0: 6846 3634 6e5a 4147 474a 5a33 735a 4f55  hF64nZAGGJZ3sZOU
-0003dad0: 6738 6237 4a6c 2f59 5a36 302f 6137 5479  g8b7Jl/YZ60/a7Ty
-0003dae0: 5a53 677a 456e 6b6a 316f 7932 617a 7145  ZSgzEnkj1oy2azqE
-0003daf0: 3354 3261 5468 6e47 6c64 4a6f 634d 4e65  3T2aThnGldJocMNe
-0003db00: 7746 3639 364b 6e58 6663 2f2b 776c 712b  wF696KnXfc/+wlq+
-0003db10: 4474 7473 3449 456b 416e 4b64 534e 6e6b  Dtts4IEkAnKdSNnk
-0003db20: 5435 416e 6573 5243 4b4b 4e51 7171 4476  T5AnesRCKKNQqqDv
-0003db30: 466e 6b51 4151 5952 742b 6149 7562 5763  FnkQAQYRt+aIubWc
-0003db40: 5048 6e75 774f 376a 5042 637a 6952 6639  PHnuwO7jPBcziRf9
-0003db50: 6c4b 6852 4b4e 3357 506d 6b67 7879 5a41  lKhRKN3WPmkgxyZA
-0003db60: 5a71 446c 7462 5155 544a 4449 7537 5262  ZqDltbQUTJDIu7Rb
-0003db70: 7766 7438 392f 5370 7739 6f6d 7731 5853  wft89/Spw9omw1XS
-0003db80: 676f 3948 4744 4241 3547 5068 6345 5a2b  go9HGDBA5GPhcEZ+
-0003db90: 7a34 4537 356d 7766 2f34 6978 6331 515a  z4E75mwf/4ixc1QZ
-0003dba0: 6445 386d 4158 7938 454f 7044 3377 4d36  dE8mAXy8EOpD3wM6
-0003dbb0: 4b30 3157 4d51 4f2f 4146 2f32 6767 3844  K01WMQO/AF/2gg8D
-0003dbc0: 4b6b 7036 344c 6668 6d65 3573 4b6a 7266  Kkp64Lfhme5sKjrf
-0003dbd0: 6350 6c71 306b 7639 3732 6574 7955 422b  cPlq0kv972etyUB+
-0003dbe0: 4831 5665 462f 3663 514d 356a 4e59 3331  H1VeF/6cQM5jNY31
-0003dbf0: 566f 4f4e 4b4b 646f 337a 4548 5269 4131  VoONKKdo3zEHRiA1
-0003dc00: 5569 7258 6c46 6961 652f 2b43 3351 4935  UirXlFiae/+C3QI5
-0003dc10: 6e72 4b5a 736d 572b 3864 4170 514d 3268  nrKZsmW+8dApQM2h
-0003dc20: 7848 392b 3467 704d 4376 6e2f 6c30 4275  xH9+4gpMCvn/l0Bu
-0003dc30: 514f 4f69 6959 7641 6c59 596e 7672 7742  QOOiiYvAlYYnvrwB
-0003dc40: 446f 4735 5948 5877 4a68 595a 6850 4f64  DoG5YHXwJhYZhPOd
-0003dc50: 3669 632b 5766 5172 6b65 4d50 7656 644f  6ic+WfQrkeMPvVdO
-0003dc60: 584f 665a 3234 5835 5153 4c6f 5242 4b4e  XOfZ24X5QSLoRBKN
-0003dc70: 4839 7450 734d 3454 2f6c 3530 784d 3337  H9tPsM4T/l50xM37
-0003dc80: 5570 4150 7758 5a63 3932 4970 7a45 476f  UpAPwXZc92IpzEGo
-0003dc90: 712b 696d 706f 4732 5268 6f30 6544 4469  q+impoG2Rho0eDDi
-0003dca0: 496a 6662 4472 3339 5050 7637 6d66 3378  IjfbDr39PPv7mf3x
-0003dcb0: 3850 3975 3248 5a68 6632 7379 4459 386c  8P9u2HZhf2syDY8l
-0003dcc0: 416c 6e67 5065 7463 4342 6841 6376 495a  AlngPetcCBhAcvIZ
-0003dcd0: 5867 4445 5944 6837 5131 7057 4155 7232  XgDEYDh7Q1pWAUr2
-0003dce0: 544a 2b37 6837 622f 6a6d 6177 7144 5a30  TJ+7h7b/jmawqDZ0
-0003dcf0: 486a 5668 5a2f 436c 4a43 5062 4447 4143  HjVhZ/ClJCPbDGAC
-0003dd00: 6c4e 684a 776c 7656 4533 6c36 7935 706e  lNhJwlvVE3l6y5pn
-0003dd10: 4d33 552f 6568 3165 6f4b 4730 7a67 5a30  M3U/eh1eoKG0zgZ0
-0003dd20: 647a 3437 6f55 4848 594a 6341 4c4d 6775  dz47oUHHYJcALMgu
-0003dd30: 6d4a 3351 2f4d 5a79 502b 4468 7073 7977  mJ3Q/MZyP+Dhpsyw
-0003dd40: 6159 766e 6753 6142 4b30 4c72 4d73 784b  aYvngSaBK0LrMsxK
-0003dd50: 4f35 3163 6c5a 644e 4a2b 2f34 4935 6d42  O51clZdNJ+/4I5mB
-0003dd60: 4867 4130 4861 5141 4964 5056 5243 5863  HgA0HaQAIdPVRCXc
-0003dd70: 7661 6764 564a 3851 655a 5033 672f 5338  vagdVJ8QeZP3g/S8
-0003dd80: 3737 5172 6f7a 576e 5666 7446 4756 4c6f  77QrozWnVftFGVLo
-0003dd90: 2b71 536b 4548 5968 435a 4864 4b62 4e39  +qSkEHYhCZHdKbN9
-0003dda0: 2f64 3936 6a5a 6f6b 7a66 3856 7133 3350  /d96jZokzf8Vq33P
-0003ddb0: 7034 314a 3035 6f4f 6a69 5a70 6541 5455  p41J05oOjiZpeATU
-0003ddc0: 5958 7348 4171 3658 6734 6855 7166 5031  YXsHAq6Xg4hUqfP1
-0003ddd0: 4f62 376c 7243 5149 6274 5759 7657 4f5a  Ob7lrCQIbtWYvWOZ
-0003dde0: 3873 7667 5662 326a 2f46 4b74 4e44 3845  8svgVb2j/FKtND8E
-0003ddf0: 7557 4859 2f79 746d 4d43 5356 5556 3762  uWHY/ytmMCSVUV7b
-0003de00: 6d46 3653 666d 4856 4c36 7538 7650 6375  mF6SfmHVL6u8vPcu
-0003de10: 6273 2b47 5853 7a59 4453 4143 5546 4944  bs+GXSzYDSACUFID
-0003de20: 2f78 4b73 5448 4339 6e67 2b66 6743 5a79  /xKsTHC9ng+fgCZy
-0003de30: 3171 656b 617a 454f 7769 7568 2b68 512f  1qekazEOwiuh+hQ/
-0003de40: 7234 4e30 6a63 432f 4354 6e43 5247 7a47  r4N0jcC/CTnCRGzG
-0003de50: 3464 3875 6834 7934 5456 636c 4459 494f  4d8uh4y4TVclDYIO
-0003de60: 4f32 6867 454a 4247 7759 6b51 5037 4747  O2hgEJBGwYkQP7GG
-0003de70: 376b 7730 6166 3062 626a 4a6b 6661 6b76  7kw0af0bbjJkfakv
-0003de80: 466f 6673 4a63 766d 7059 3644 7637 6b36  FofsJcvmpY6Dv7k6
-0003de90: 4e46 6d30 3539 5174 7452 5233 4947 4945  NFm059QttRR3IGIE
-0003dea0: 436a 6c55 6e68 7659 3953 4f34 2b73 722f  CjlUnhvY9SO4+sr/
-0003deb0: 3932 644c 3365 5650 5778 5775 5769 6952  92dL3eVPWxWuWiiR
-0003dec0: 777a 4745 416a 5638 796b 316e 5874 396f  wzGEAjV8yk1nXt9o
-0003ded0: 4b6e 7636 7147 5434 7052 4d39 546f 4b39  Knv6qGT4pRM9ToK9
-0003dee0: 424a 7548 474d 4f67 7972 4773 7432 4b39  BJuHGMOgyrGst2K9
-0003def0: 392f 4235 4d69 4f66 3767 2f72 7341 454d  9/B5MiOf7g/rsAEM
-0003df00: 5239 5538 2b7a 5834 4541 5570 744d 3061  R9U8+zX4EAUptM0a
-0003df10: 5551 4135 372f 7371 4855 2f63 2b66 6166  UQA57/sqHU/c+faf
-0003df20: 7a37 7279 6c48 4b5a 4b6d 4c6f 3551 474c  z7rylHKZKmLo5QGL
-0003df30: 6776 744a 2b6f 7748 4a59 6578 774c 7263  gvtJ+owHJYexwLrc
-0003df40: 3834 6673 7539 3245 3842 6331 6e34 5156  84fsu92E8Bc1n4QV
-0003df50: 426d 6f63 5155 6644 714f 4641 4a33 4c48  BmocQUfDqOFAJ3LH
-0003df60: 6664 4f51 6542 2b66 4744 6673 2b53 7963  fdOQeB+fGDfs+Syc
-0003df70: 6d62 4134 3577 4465 324a 727a 634a 5333  mbA45wDe2JrzcJS3
-0003df80: 2f2b 3949 4748 2b4c 734c 6e51 3351 5669  /+9IGH+LsLnQ3QVi
-0003df90: 6669 3736 386a 4e6e 3256 4f69 642b 7039  fi768jNn2VOid+p9
-0003dfa0: 7471 6761 6c68 6a53 7472 4b55 5378 7159  tqgalhjStrKUSxqY
-0003dfb0: 442b 4e45 7872 3071 5046 5076 7365 4c44  D+NExr0qPFPvseLD
-0003dfc0: 7333 574d 6c2f 326a 7855 6867 4671 5046  s3WMl/2jxUhgFqPF
-0003dfd0: 3150 752f 4c6c 6d7a 4268 756d 6d47 674f  1Pu/LlmzBhummGgO
-0003dfe0: 675a 3448 536b 4363 5170 6236 4157 396f  gZ4HSkCcQpb6AW9o
-0003dff0: 434a 4d45 686e 4456 6e30 624c 456e 4555  CJMEhnDVn0bLEnEU
-0003e000: 762b 6d4d 4739 3264 5636 6d36 3571 6a71  v+mMG92dV6m65qjq
-0003e010: 4667 517a 3244 6158 724e 6a70 5076 2f76  FgQz2DaXrNjpPv/v
-0003e020: 7a39 4a2b 6665 6370 7162 4e76 5575 5559  z9J+fecpqbNvUuUY
-0003e030: 526b 4151 6f38 5944 5464 596f 6f4f 6143  RkAQo8YDTdYooOaC
-0003e040: 6936 4744 782f 6766 5177 4f65 4676 4175  i6GDx/gfQwOeFvAu
-0003e050: 7467 6c38 4742 7548 6747 4976 7573 7564  tgl8GBuHgGIvusud
-0003e060: 3248 4e79 7664 664b 6546 336e 3936 382b  2HNyvdfKeF3n968+
-0003e070: 465a 7578 6871 7177 446a 5367 3541 4245  FZuxhqqwDjSg5ABE
-0003e080: 3961 6f5a 4d4f 4c61 3961 2b56 732b 2b2f  9aoZMOLa9a+Vs++/
-0003e090: 732b 6565 4c6b 696f 4a33 5536 5156 5166  s+eeLkioJ3U6QVQf
-0003e0a0: 7935 6630 4837 4c6f 4161 6e49 6b48 4934  y5f0H7LoAanIkHI4
-0003e0b0: 5574 694b 3156 6d6b 4869 6f51 3651 3347  UtiK1VmkHioQ6Q3G
-0003e0c0: 6e41 7343 5a72 6b59 4d37 7257 2f32 4776  nAsCZrkYM7rW/2Gv
-0003e0d0: 4d45 4c36 7363 5936 5976 366a 5267 556b  MEL6scY6Yv6jRgUk
-0003e0e0: 6c6e 4930 684c 3031 4638 4551 4947 5156  lnI0hL01F8EQIGQV
-0003e0f0: 3042 3241 476b 4949 6353 7353 6234 4759  0B2AGkIIcSsSb4GY
-0003e100: 7736 4649 3074 6862 6b77 4634 6350 4e32  w6FI0thbkwF4cPN2
-0003e110: 2b56 476a 7076 7047 4151 4a74 5a61 3235  +VGjpvpGAQJtZa25
-0003e120: 7835 7337 482f 715a 6a6d 7730 6b67 6645  x5s7H/qZjmw0kgfE
-0003e130: 6145 6f6b 4243 6848 4445 726a 4c77 4169  aEokBChHDErjLwAi
-0003e140: 3067 6166 4142 786e 4a63 5141 6859 4c77  0gafABxnJcQAhYLw
-0003e150: 7138 7249 4138 784d 7065 6c54 627a 5966  q8rIA8xMpelTbzYf
-0003e160: 7365 6d42 2b39 7845 2f6b 716e 6b4c 7268  semB+9xE/kqnkLrh
-0003e170: 4a55 2b57 6730 6b5a 6f53 5968 4553 755a  JU+Wg0kZoSYhESuZ
-0003e180: 6150 6854 3468 4244 5a43 334d 5858 3963  aPhT4hBDZC3MXX9c
-0003e190: 6c63 366f 7442 5478 3564 6939 6d6a 3556  lc6otBTx5di9mj5V
-0003e1a0: 2b71 2f73 6748 4b4f 7651 4565 6554 3831  +q/sgHKOvQEeeT81
-0003e1b0: 6f47 6a4d 7169 6d79 5273 3151 6736 626a  oGjMqimyRs1Qg6bj
-0003e1c0: 6a67 5864 3437 3771 4478 666c 4858 6d64  jgXd477qDxflHXmd
-0003e1d0: 4e4f 3259 4354 4e4a 394f 4f41 7768 4b62  NO2YCTNJ9OOAwhKb
-0003e1e0: 4a4a 3137 4352 4156 2f77 424c 3835 7a56  JJ17CRAV/wBL85zV
-0003e1f0: 7772 4b48 5434 4564 4563 444d 4f6e 5648  wrKHT4EdEcDMOnVH
-0003e200: 5667 7645 7567 3935 6538 5153 6371 6f32  VgvEug95e8QScqo2
-0003e210: 686a 6d4d 4153 7865 566a 6675 412b 344d  hjmMASxeVjfuA+4M
-0003e220: 3637 5238 735a 7439 772f 3330 314a 6365  67R8sZt9w/301Jce
-0003e230: 6e44 4b68 3977 4e39 4257 306b 597a 4d45  nDKh9wN9BW0kYzME
-0003e240: 434e 7366 3343 6f57 2b56 5537 6a79 5874  CNsf3CoW+VU7jyXt
-0003e250: 6635 6f37 7166 7957 6358 5870 682f 594b  f5o7qfyWcXXph/YK
-0003e260: 7147 6d68 6470 3541 5748 6942 5549 356d  qGmhdp5AWHiBUI5m
-0003e270: 6c64 4d47 3133 2b71 6c55 3263 3054 4c32  ldMG13+qlU2c0TL2
-0003e280: 7855 5673 7246 7431 4f6b 4832 2f4e 6a5a  xUVsrFt1OkH2/NjZ
-0003e290: 566b 3679 7830 756e 3043 3341 3650 7779  Vk6yx0un0C3A6Pwy
-0003e2a0: 3636 6a33 516e 6c6d 5661 6736 4762 6d41  66j3QnlmVag6GbmA
-0003e2b0: 5643 6473 2b56 4652 5342 444b 5a47 4f4a  VCds+VFRSBDKZGOJ
-0003e2c0: 5048 4865 7466 394f 466c 2f41 3952 7452  PHHetf9OFl/A9RtR
-0003e2d0: 4c61 654f 4278 3665 3866 6141 4845 5157  LaeOBx6e8faAHEQW
-0003e2e0: 4746 5843 734e 456b 5153 4251 5178 7131  GFXCsNEkQSBQQxq1
-0003e2f0: 3246 556d 7342 4630 3444 5464 4769 6f6d  2FUmsBF04DTdGiom
-0003e300: 426a 4a52 4375 3951 4656 3961 7737 7557  BjJRCu9QFV9aw7uW
-0003e310: 4755 3270 2f63 6664 784f 4158 7a44 5351  GU2p/cfdxOAXzDSQ
-0003e320: 4b63 6750 6142 2b66 6953 424c 6268 725a  KcgPaB+fiSBLbhrZ
-0003e330: 4b57 5837 4447 5964 4d61 6a70 6a30 7039  KWX7DGYdMajpj0p9
-0003e340: 4662 6457 6873 4449 3143 3230 6f71 4338  FbdWhsDI1C20oqC8
-0003e350: 6f57 7163 6a45 4e67 6a43 4934 644b 464a  oWqcjENgjCI4dKFJ
-0003e360: 2b41 4855 344c 5650 7458 3265 6c77 4931  +AHU4LVPtX2elwI1
-0003e370: 3377 5835 7561 5a69 2b30 4332 5949 6d66  3wX5uaZi+0C2YImf
-0003e380: 5936 377a 6174 4639 6f34 544a 6667 4b50  Y67zatF9o4TJfgKP
-0003e390: 6e35 4a4b 3533 4e4f 7578 5636 4877 376b  n5JK53NOuxV6Hw7k
-0003e3a0: 4848 4a52 6551 534e 534f 3065 4f51 4a51  HHJReQSNSO0eOQJQ
-0003e3b0: 6367 6171 5579 426d 4c73 3572 3047 4c48  cgaqUyBmLs5r0GLH
-0003e3c0: 6e6d 496d 7358 2f30 532b 392f 4c6c 3875  nmImsX/0S+9/Ll8u
-0003e3d0: 6353 312f 3874 4779 6273 7348 7743 6d2b  cS1/8tGybssHwCm+
-0003e3e0: 6351 4536 384b 6759 5250 5466 4245 5267  cQE68KgYRPTfBERg
-0003e3f0: 4e53 3241 4d41 6764 5662 5774 6a59 634d  NS2AMAgdVbWtjYcM
-0003e400: 634b 4a31 4f63 466a 3830 594d 4869 6533  cKJ1OcFj80YMHie3
-0003e410: 3637 4976 6446 4c5a 4b79 616f 4370 414c  67IvdFLZKyaoCpAL
-0003e420: 4d66 6b41 3943 6e35 442b 7256 5058 7354  MfkA9Cn5D+rVPXsT
-0003e430: 374b 7768 4b37 6953 5142 4f41 3161 4c50  7KwhK7iSQBOA1aLP
-0003e440: 4677 796e 6c4f 6641 6657 6446 4e51 5a77  FwynlOfAfWdFNQZw
-0003e450: 6857 5269 3166 4d75 7966 5879 3847 5159  hWRi1fMuyfXy8GQY
-0003e460: 2b6e 7033 6766 6d37 4379 4837 4e70 3033  +np3gfm7CyH7Np03
-0003e470: 3872 6a2b 7735 396b 7731 3144 2f32 3144  8rj+w59kw11D/21D
-0003e480: 5854 556c 455a 3353 7453 7459 4d68 642b  XTUlEZ3StStYMhd+
-0003e490: 5253 466d 585a 4f70 7150 2b59 7732 307a  RSFmXZOpqP+Yw20z
-0003e4a0: 6b6b 3162 5078 552f 4978 6e75 6578 2f38  kk1bPxU/Ixnuex/8
-0003e4b0: 2b58 4c48 6f56 672f 797a 6d63 3139 4145  +XLHoVg/yzmc19AE
-0003e4c0: 4375 3736 4732 7445 5272 7652 5356 5636  Cu76G2tERrvRSVV6
-0003e4d0: 6973 6532 4668 4a63 2f44 6737 6833 5a41  ise2FhJc/Dg7h3ZA
-0003e4e0: 4163 7768 4d56 6131 754f 7046 4230 4832  AcwhMVa1uOpFB0H2
-0003e4f0: 4d45 7367 6741 472f 6939 504d 5033 7656  MEsggAG/i9PMP3vV
-0003e500: 7139 356f 7a4c 3250 3936 784c 4144 5268  q95ozL2P96xLADRh
-0003e510: 4330 456d 5568 6866 476d 3241 6348 3962  C0EmUhhfGm2AcH9b
-0003e520: 446a 6d53 4758 5567 5358 4d69 3245 6342  DjmSGXUgSXMi2EcB
-0003e530: 3743 315a 564f 6d6b 6c48 6678 4956 6753  7C1ZVOmklHfxIVgS
-0003e540: 3654 6b48 4645 5345 3564 444b 546a 6d4d  6TkHFESE5dDKTjmM
-0003e550: 7857 4a39 6e55 7033 3633 2b35 4541 6c69  xWJ9nUp363+5EAli
-0003e560: 7772 6b58 444b 6467 6638 686f 7774 6142  wrkXDKdgf8howtaB
-0003e570: 3978 6a2f 7946 5051 4172 7738 6b6f 5745  9xj/yFPQArw8koWE
-0003e580: 5672 4f59 7978 3345 6254 3538 3073 5758  VrOYyx3EbT580sWX
-0003e590: 796e 7265 4a32 6a52 3444 6159 2f45 4b47  ynreJ2jR4DaY/EKG
-0003e5a0: 4373 4d70 6850 5475 3267 776f 4a73 4d79  CsMphPTu2gwoJsMy
-0003e5b0: 546c 6e56 4771 7462 3561 624c 6555 532b  TlnVGqtb5abLeUS+
-0003e5c0: 4a36 5946 5653 324e 5638 4332 4353 6b57  J6YFVS2NV8C2CSkW
-0003e5d0: 3345 6951 3565 7168 305a 4230 7474 6c39  3EiQ5eqh0ZB0ttl9
-0003e5e0: 4453 366f 324a 5a79 3661 696d 6243 3675  DS6o2JZy6aimbC6u
-0003e5f0: 386c 6375 765a 4156 3347 7378 4e50 6c56  8lcuvZAV3GsxNPlV
-0003e600: 746a 5775 4642 7948 6f5a 4246 7073 6c43  tjWuFByHoZBFpslC
-0003e610: 677a 5369 6873 7952 5933 3772 4476 4f76  gzSihsyRY37rDvOv
-0003e620: 502f 5a31 2f2f 7248 3738 4978 4477 7770  P/Z1//rH78IxDwwp
-0003e630: 6877 3741 4c69 4148 5455 7838 6e71 3658  hw7ALiAHTUx8nq6X
-0003e640: 444c 7578 735a 7468 6c62 4f73 4665 4132  DLuxsZthlbOsFeA2
-0003e650: 3747 6a70 3264 5359 4259 3359 3451 5563  7Gjp2dSYBY3Y4QUc
-0003e660: 386f 4b35 6e57 4738 566d 4768 5158 3631  8oK5nWG8VmGhQX61
-0003e670: 4178 2b49 736b 5568 5956 6455 704a 4277  Ax+IskUhYVdUpJBw
-0003e680: 5a79 3841 5141 3048 6b41 4642 6469 5268  Zy8AQA0HkAFBdiRh
-0003e690: 3030 342f 326a 2f61 5443 4946 6551 2f69  004/2j/aTCIFeQ/i
-0003e6a0: 3241 384d 7161 586b 772b 4850 6264 682f  2A8MqaXkw+HPbdh/
-0003e6b0: 5261 2b33 6c4a 3179 5a48 7a50 7757 756e  Ra+3lJ1yZHzPwWun
-0003e6c0: 5941 3849 3256 5546 514e 6453 4353 4b54  YA8I2VUFQNdSCSKT
-0003e6d0: 7552 585a 7778 454b 3251 6549 646a 6c4e  uRXZwxEK2QeIdjlN
-0003e6e0: 3165 4361 5465 5a6b 3167 3630 3143 6534  1eCaTeZk1g601Ce4
-0003e6f0: 7478 3457 5470 4461 5279 6654 4765 2b57  tx4WTpDaRyfTGe+W
-0003e700: 746a 4734 6c53 4f47 7a68 5545 444f 5433  tjG4lSOGzhUEDOT3
-0003e710: 7256 504f 7568 5434 4752 4547 5356 5066  rVPOuhT4GREGSVPf
-0003e720: 7037 7957 574c 482f 5561 5777 3953 6b72  p7yWWLH/UaWw9Skr
-0003e730: 784a 7867 6274 4a69 4430 4a34 632b 7669  xJxgbtJiD0J4c+vi
-0003e740: 4541 5348 4970 3230 796d 527a 7348 5442  EASHIp20ymRzsHTB
-0003e750: 3275 6e76 6456 3738 7239 687a 6445 382b  2unvdV78r9hzdE8+
-0003e760: 694d 4f43 4338 5465 6555 5a55 3377 5136  iMOCC8TeeUZU3wQ6
-0003e770: 6c76 416c 4b36 4768 4945 7433 784f 707a  lvAlK6GhIEt3xOpz
-0003e780: 4541 7a46 344d 7557 6731 3542 4f49 6d7a  EAzF4MuWg15BOImz
-0003e790: 5877 4876 4132 4131 5158 4230 4967 7268  XwHvA2A1QXB0Igrh
-0003e7a0: 5751 4271 5441 5979 5a79 4a76 4163 4331  WQBqTAYyZyJvAcC1
-0003e7b0: 4a77 7a59 4e72 4150 5770 3533 586f 4955  JwzYNrAPWp53XoIU
-0003e7c0: 3849 666b 4d33 432f 6350 3578 666b 4134  8IfkM3C/cP5xfkA4
-0003e7d0: 6541 3070 7834 632f 7a36 7174 3530 356d  eA0px4c/z6qt505m
-0003e7e0: 5444 6d30 3959 5a38 2f69 7671 7134 3343  TDm09YZ8/ivqq43C
-0003e7f0: 6a30 5462 4651 4173 5636 4353 7942 7a72  j0TbFQAsV6CSyBzr
-0003e800: 4136 4843 6734 4465 6263 2f2f 5552 4b4c  A6HCg4Debc//URKL
-0003e810: 3636 6b54 4b41 6e2f 5278 4b79 7146 4f56  66kTKAn/RxKyqFOV
-0003e820: 416b 6c41 2b41 687a 7343 6b65 3345 6754  AklA+AhzsCke3EgT
-0003e830: 6838 5361 4f43 2b6f 4253 6467 6149 456b  h8SaOC+oBSdgaIEk
-0003e840: 6550 4570 6570 6762 3345 5935 6661 4b68  ePEpepgb3EY5faKh
-0003e850: 6175 4f68 3756 7334 3948 5272 2f50 3944  auOh7Vs49HRr/P9D
-0003e860: 7056 6237 4967 6154 4453 4e45 5357 7868  pVb7IgaTDSNESWxh
-0003e870: 524d 5669 4857 3562 442b 7659 3477 7676  RMViHW5bD+vY4wvv
-0003e880: 4735 4639 3558 7a74 3641 6b38 4154 5843  G5F95Xzt6Ak8ATXC
-0003e890: 3430 5734 5344 354d 5650 4175 5847 5859  40W4SD5MVPAuXGXY
-0003e8a0: 6879 4161 7734 4353 5078 4f43 5a70 494e  hyAaw4CSPxOCZpIN
-0003e8b0: 6567 7849 5251 4137 5943 7552 524c 4648  egxIRQA7YCuRRLFH
-0003e8c0: 5644 536f 5371 6a6f 4d39 6765 3442 4456  VDSoSqjoM9ge4BDV
-0003e8d0: 5154 396c 4777 4747 345a 6d56 5335 4532  QT9lGwGG4ZmVS5E2
-0003e8e0: 7762 4349 474c 6846 696d 456d 3444 314e  wbCIGLhFimEm4D1N
-0003e8f0: 6732 6766 5948 3579 4534 3155 7043 554e  g2gfYH5yE41UpCUN
-0003e900: 4c61 424e 5053 6476 4c44 752b 6261 7672  LaBNPSdvLDu+bavr
-0003e910: 366b 5664 356f 7766 2b53 4472 7146 6474  6kVd5owf+SDrqFdt
-0003e920: 6f6d 324b 6768 5170 3045 746b 4448 6141  om2KghQp0EtkDHaA
-0003e930: 6a49 504b 5164 4176 4d35 5536 6f53 715a  jIPKQdAvM5U6oSqZ
-0003e940: 6654 6c67 7556 412f 4955 5a32 5756 6e55  fTlguVA/IUZ2WVnU
-0003e950: 4266 4655 6875 6862 6a64 5656 4638 5570  BfFUhuhbjdVVF8Up
-0003e960: 4574 7850 4549 4341 4b48 715a 6576 5a6c  EtxPEICAKHqZevZl
-0003e970: 7651 7a2f 6f57 5573 4e61 474e 4431 7461  vQz/oWUsNaGND1ta
-0003e980: 3654 7435 394b 6447 5350 7872 3637 5431  6Tt59KdGSPxr67T1
-0003e990: 774e 4e54 3163 3868 5252 4151 7479 455a  wNNT1c8hRRAQtyEZ
-0003e9a0: 5249 3148 5669 6f6b 6e6e 4548 6567 6276  RI1HVioknnEHegbv
-0003e9b0: 3870 4844 6474 472f 4c63 5350 7263 6469  8pHDdtG/LcSPrcdi
-0003e9c0: 4277 772f 6f6c 7a41 636f 5337 716b 7a63  Bww/olzAcoS7qkzc
-0003e9d0: 704d 2b78 4343 5764 6c54 6e4f 4536 6951  pM+xCCWdlTnOE6iQ
-0003e9e0: 4e70 3943 4777 4745 5663 4a69 4756 3261  Np9CGwGEVcJiGV2a
-0003e9f0: 4968 6664 6249 6855 7876 3041 504f 686d  IhfdbIhUxv0APOhm
-0003ea00: 4630 4c74 7065 475a 524c 6367 4577 504b  F0LtpeGZRLcgEwPK
-0003ea10: 6850 684b 4862 784b 4763 6544 324c 4f4d  hPhKHbxKGceD2LOM
-0003ea20: 3144 4447 7776 7551 3138 4745 6250 5a7a  1DDGwvuQ18GEbPZz
-0003ea30: 4371 314b 574c 6342 7a57 4a34 4e6e 6b4f  Cq1KWLcBzWJ4NnkO
-0003ea40: 6b55 6e37 4c74 454d 5061 7a6e 6e69 4874  kUn7LtEMPaznniHt
-0003ea50: 6c62 6671 7763 4b34 5246 4155 6f49 5565  lbfqwcK4RFAUoIUe
-0003ea60: 414d 7554 4145 355a 6b73 3647 647a 6b70  AMuTAE5Zks6Gdzkp
-0003ea70: 7735 3265 7071 716f 4748 4559 4a47 4534  w52epqqoGHEYJGE4
-0003ea80: 684f 5367 662b 4245 7a74 454b 696c 4a4b  hOSgf+BEztEKilJK
-0003ea90: 6c55 6c45 7842 436b 4654 7479 3968 6d61  lUlExBCkFTty9hma
-0003eaa0: 4f52 4d47 4639 657a 4a48 4c38 6165 7078  ORMGF9ezJHL8aepx
-0003eab0: 594b 5276 7933 3255 4637 7a52 7735 6e50  YKRvy32UF7zRw5nP
-0003eac0: 516f 394d 4b35 716a 6838 564a 4245 4363  Qo9MK5qjh8VJBECc
-0003ead0: 5253 6163 6357 734a 4264 5753 2f6e 6c39  RSaccWsJBdWS/nl9
-0003eae0: 794c 7a37 2b64 752f 636f 2f61 5550 6173  yLz7+du/co/aUPas
-0003eaf0: 3454 654a 7845 6873 5a64 6946 6873 4f38  4TeJxEhsZdiFhsO8
-0003eb00: 5a62 344a 6567 3156 584a 336b 7143 5364  Zb4Jeg1VXJ3kqCSd
-0003eb10: 7961 455a 366a 6b38 6a47 465a 4651 4b39  yaEZ6jk8jGFZFQK9
-0003eb20: 5a41 4441 584c 4371 7a55 5949 5942 456f  ZADAXLCqzUYIYBEo
-0003eb30: 7668 5345 6e48 6a43 6f6a 6d51 4f6b 4b4d  vhSEnHjCojmQOkKM
-0003eb40: 326e 6543 3151 4643 6f41 6330 3173 4a37  2neC1QFCoAc01sJ7
-0003eb50: 3452 354e 7772 4463 4d70 3942 6253 4e64  4R5NwrDcMp9BbSNd
-0003eb60: 6a48 6b7a 4359 534b 6532 324e 556e 3358  jHkzCYSKe22NUn3X
-0003eb70: 662f 7449 5043 794d 482f 416a 4769 2f33  f/tIPCyMH/AjGi/3
-0003eb80: 444b 6b54 4b42 5633 5a67 6941 556b 5777  DKkTKBV3ZgiAUkWw
-0003eb90: 5567 646b 6956 4f34 3257 3742 6a4d 306e  UgdkiVO42W7BjM0n
-0003eba0: 3761 6551 464a 7048 4869 4a41 6a43 6b57  7aeQFJpHHiJAjCkW
-0003ebb0: 6536 4643 7263 6c47 7842 4347 414a 796b  e6FCrclGxBCGAJyk
-0003ebc0: 466b 7154 617a 6e6a 4a67 7675 3831 644a  FkqTaznjJgvu81dJ
-0003ebd0: 7941 7644 6a76 2b48 6746 5873 5463 7844  yAvDjv+HgFXsTcxD
-0003ebe0: 3130 6579 4948 416f 6738 5a64 772b 7272  10eyIHAog8Zdw+rr
-0003ebf0: 3737 3378 4e34 6171 7666 4539 7350 7942  773xN4aqvfE9sPyB
-0003ec00: 4439 7751 6977 7937 7366 4854 4847 5638  D9wQiwy7sfHTHGV8
-0003ec10: 3071 7338 6b2f 4851 532f 3365 6732 6f67  0qs8k/HQS/3eg2og
-0003ec20: 462f 524d 3969 426c 376c 5941 6d32 396a  F/RM9iBl7lYAm29j
-0003ec30: 5575 6c79 316b 6972 5853 4b56 5371 434d  Uuly1kirXSKVSqCM
-0003ec40: 612b 4361 674a 6763 436e 3146 5769 736f  a+CagJgcCn1FWiso
-0003ec50: 6c38 436f 5a31 4d64 4c4a 7048 4451 6e6b  l8CoZ1MdLJpHDQnk
-0003ec60: 4e64 5538 4476 4157 5141 785a 7575 3335  NdU8DvAWQAxZuu35
-0003ec70: 5655 6a52 504f 3352 5338 2f46 3733 7946  VUjRPO3RS8/F73yF
-0003ec80: 7171 3436 4347 6b4e 7953 626b 4930 434d  qq46CGkNySbkI0CM
-0003ec90: 7842 5730 6f53 6c47 6537 5650 7735 6c4d  xBW0oSlGe7VPw5lM
-0003eca0: 534e 6661 506e 5a71 7135 7342 4441 446c  SNfaPnZqq5sBDADl
-0003ecb0: 5145 694c 6b4d 4635 4432 486d 4f69 327a  QEiLkMF5D2HmOi2z
-0003ecc0: 4374 3630 7247 3931 4c6b 4646 7773 7255  Ct60rG91LkFFwsrU
-0003ecd0: 5351 534e 4664 5150 304a 4f59 7973 4630  SQSNFdQP0JOYysF0
-0003ece0: 4838 784a 5955 4565 694a 4378 6e74 567a  H8xJYUEeiJCxntVz
-0003ecf0: 6538 6e31 6538 4c39 4b33 6751 506f 446b  e8n1e8L9K3gQPoDk
-0003ed00: 302b 7141 4835 4343 556b 4b4e 4967 4465  0+qAH5CCUkKNIgDe
-0003ed10: 4261 5462 7256 5473 702f 3930 7076 7932  BaTbrVTsp/90pvy2
-0003ed20: 6350 336c 664b 356d 6752 3733 5656 522f  cP3lfK5mgR73VVR/
-0003ed30: 774a 756d 4d78 6575 7245 6a54 3049 624c  wJumMxeurEjT0IbL
-0003ed40: 676d 5273 3643 6e5a 5733 5745 5232 4b47  gmRs6CnZW3WER2KG
-0003ed50: 6a6e 5470 4570 4879 5461 6c52 5454 7855  jnTpEpHyTalRTTxU
-0003ed60: 684e 626f 4e39 4271 3471 4167 4e71 3244  hNboN9Bq4qAgNq2D
-0003ed70: 6f42 3357 4442 636b 4c5a 3274 4c31 4654  oB3WDBckLZ2tL1FT
-0003ed80: 6267 6b4f 644a 5635 3473 4630 6f6a 5a62  bgkOdJV54sF0ojZb
-0003ed90: 4362 7476 3358 4866 7863 5438 6f6a 4f78  Cbtv3XHfxcT8ojOx
-0003eda0: 2f4c 5869 652f 7251 4e32 464b 6b4b 4956  /LXie/rQN2FKkKIV
-0003edb0: 3275 736d 4549 714a 4c32 5161 3175 7858  2usmEIqJL2Qa1uxX
-0003edc0: 3877 2b53 554c 3936 302f 4a51 5562 586c  8w+SUL960/JQUbXl
-0003edd0: 3137 4f6f 704c 4176 7948 4541 4d48 6430  17OopLAvyHEAMHd0
-0003ede0: 6d55 4245 6542 496c 526a 6879 4952 6c6d  mUBEeBIlRjhyIRlm
-0003edf0: 5175 4269 5349 4252 5261 6953 5370 4c61  QuBiSIBRRaiSSpLa
-0003ee00: 3270 3576 3033 4365 7374 7578 6b35 6b75  2p5v03Cestuxk5ku
-0003ee10: 3843 3939 714f 6873 6456 414f 7752 574c  8C99qOhsdVAOwRWL
-0003ee20: 3659 494e 4e53 354e 4968 456f 6c42 6e74  6YINNS5NIhEolBnt
-0003ee30: 376a 626d 3637 5a71 7a4c 2f50 3247 7457  7jbm67ZqzL/P2GtW
-0003ee40: 6256 6163 5937 316e 6e73 4577 4365 7156  bVacY71nnsEwCeqV
-0003ee50: 4470 4947 4a50 6e52 4c6d 4c54 4443 4133  DpIGJPnRLmLTDCA3
-0003ee60: 484e 4146 5231 4430 3651 696c 4a64 4c57  HNAFR1D06QilJdLW
-0003ee70: 4373 6f49 3642 516b 4933 4578 3763 6f41  CsoI6BQkI3Ex7coA
-0003ee80: 774a 4352 7934 4a41 4f41 4752 4144 7766  wJCRy4JAOAGRADwf
-0003ee90: 6a50 7052 566a 7652 3756 5474 6564 5a70  jPpRVjvR7VTtedZp
-0003eea0: 4a42 3639 5131 6643 5773 7736 6631 484c  JB69Q1fCWsw6f1HL
-0003eeb0: 5366 6e65 4c2b 7378 6b32 4b67 3633 6b47  SfneL+sxk2Kg63kG
-0003eec0: 3551 5244 6f37 6577 4530 4655 5543 3330  5QRDo7ewE0FUUC30
-0003eed0: 6657 4467 3177 6579 6653 7068 7273 506f  fWDg1weyfSphrsPo
-0003eee0: 3653 6f68 6570 5370 6139 4842 7157 786c  6SohepSpa9HBqWxl
-0003eef0: 536c 6149 6943 4f4c 682f 3836 4852 5565  SlaIiCOLh/86HRUe
-0003ef00: 5a41 3454 4152 5563 4a53 4249 6163 7347  ZA4TARUcJSBIacsG
-0003ef10: 4346 7766 5873 6a57 7355 5873 554a 4572  CFwfXsjWsUXsUJEr
-0003ef20: 5373 6873 7a61 2f4a 5832 4b34 3742 5937  Sshsza/JX2K47BY7
-0003ef30: 2f70 3968 3767 6d4e 734f 6941 4a43 4c52  /p9h7gmNsOiAJCLR
-0003ef40: 555a 684e 4856 5373 676f 524d 3672 472f  UZhNHVSsgoRM6rG/
-0003ef50: 644d 6536 3077 3239 3154 7a74 6b48 7866  dMe60w291TztkHxf
-0003ef60: 5030 486a 486d 6673 656e 714b 6830 304c  P0HjHmfsenqKh00L
-0003ef70: 5539 7458 4933 3864 5a50 6432 4d6f 2f55  U9tXI38dZPd2Mo/U
-0003ef80: 4e53 6444 446f 4431 4b46 464d 476c 6b38  NSdDDoD1KFFMGlk8
-0003ef90: 6954 454a 6432 5368 4736 3674 686d 7a35  iTEJd2ShG66thmz5
-0003efa0: 4d4e 6d78 4c50 5834 4f55 3479 4567 4f45  MNmxLPX4OU4yEgOE
-0003efb0: 587a 4557 6742 7342 624f 4c39 414c 6243  XzEWgBsBbOL9ALbC
-0003efc0: 4b34 4656 3631 4e6a 652b 4646 3947 6938  K4FV61Nje+FF9Gi8
-0003efd0: 3835 7366 3555 594f 7559 5259 5078 3672  85sf5UYOuYRYPx6r
-0003efe0: 5238 6b78 4275 7443 7737 4249 3753 506a  R8kxButCw7BI7SPj
-0003eff0: 4269 5966 6459 766e 4f53 616d 552f 5171  BiYfdYvnOSamU/Qq
-0003f000: 6c41 3678 7139 546b 4259 514d 4a79 6935  lA6xq9TkBYQMJyi5
-0003f010: 714f 4755 5757 6d6b 6251 7263 535a 4444  qOGUWWmkbQrcSZDD
-0003f020: 5046 4245 4439 6279 6473 664a 324e 5333  PFBED9bydsfJ2NS3
-0003f030: 6f56 5770 416d 7356 346d 766f 2b41 3269  oVWpAmsV4mvo+A2i
-0003f040: 7054 7452 5965 5669 3833 7542 3965 7652  pTtRYeVi83uB9evR
-0003f050: 6766 6f2b 3035 7a53 3176 635a 6263 3864  gfo+05zS1vcZbc8d
-0003f060: 4458 3730 4c44 6d6a 6564 4167 6c31 4a45  DX70LDmjedAgl1JE
-0003f070: 3242 7a32 4d6f 3172 5359 5855 537a 4533  2Bz2Mo1rSYXUSzE3
-0003f080: 3675 5875 4e2b 5748 686d 354d 766b 6a73  6uXuN+WHhm5Mvkjs
-0003f090: 4d71 6b4d 5049 6a77 5962 6e45 6269 514a  MqkMPIjwYbnEbiQJ
-0003f0a0: 3955 7033 426f 6576 5353 3056 3078 5173  9Up3BoevSS0V0xQs
-0003f0b0: 374e 5a49 6b4f 7579 4343 5933 6149 6b4b  7NZIkOuyCCY3aIkK
-0003f0c0: 5848 3651 4367 7649 7052 7353 414e 5942  XH6QCgvIpRsSANYB
-0003f0d0: 2b59 4d48 7657 446b 4f45 4933 2b54 6145  +YMHvWDkOEI3+TaE
-0003f0e0: 512b 486b 6548 474c 6835 576b 676a 4955  Q+HkeHGLh5WkgjIU
-0003f0f0: 5463 6966 6c34 5930 2f6b 556d 4b31 754d  Tcifl4Y0/kUmK1uM
-0003f100: 6d48 4e35 3833 4635 3369 4a72 3052 446a  mHN583F53iJr0RDj
-0003f110: 4334 5a31 3476 572b 7148 4632 514c 6c51  C4Z14vW+qHF2QLlQ
-0003f120: 4c45 3452 3254 4a4c 7951 2b67 6f5a 7a6c  LE4R2TJLyQ+goZzl
-0003f130: 322b 7670 6b54 5849 6465 6f50 5159 3253  2+vpkTXIdeoPQY2S
-0003f140: 4a43 4b68 6266 756d 5671 6649 6657 7048  JCKhbfumVqfIfWpH
-0003f150: 5a4a 4d63 467a 6e62 6155 726e 6f56 6f4c  ZJMcFznbaUrnoVoL
-0003f160: 6b46 3632 456f 397a 6137 7178 5336 6c45  kF62Eo9za7qxS6lE
-0003f170: 5169 5a61 3142 6678 335a 7261 4159 5458  QiZa1Bfx3ZraAYTX
-0003f180: 4134 7931 4143 6b6f 4b59 4e56 5753 565a  A4y1ACkoKYNVWSVZ
-0003f190: 667a 394b 4a35 6856 5757 2b4d 5075 4376  fz9KJ5hVWW+MPuCv
-0003f1a0: 5067 6f4d 376d 3777 4a48 6e46 616b 7736  PgoM7m7wJHnFakw6
-0003f1b0: 3651 6942 3142 7a48 512b 5254 416d 3167  6QiB1BzHQ+RTAm1g
-0003f1c0: 7349 5876 5648 5a45 3762 6549 7437 6e46  sIXvVHZE7beIt7nF
-0003f1d0: 3737 6335 3631 4f4c 456d 3134 6534 6e44  77c561OLEm14e4nD
-0003f1e0: 5752 704c 6757 3366 3437 6753 5242 4b7a  WRpLgW3f47gSRBKz
-0003f1f0: 6d37 4538 654a 7075 4830 7964 7a7a 5361  m7E8eJpuH0ydzzSa
-0003f200: 4438 694f 4773 4567 6370 5947 6c34 4873  D8iOGsEgcpYGl4Hs
-0003f210: 346f 7345 4e67 4276 4371 3366 6748 656a  4osENgBvCq3fgHej
-0003f220: 6450 3370 2b69 714f 6e77 4a64 6575 4f50  dP3p+iqOnwJdeuOP
-0003f230: 4b42 4f78 7067 6e6e 3573 5550 364e 4a39  KBOxpgnn5sUP6NJ9
-0003f240: 3234 4258 6530 4c36 5830 3931 7733 4b41  24BXe0L6X091w3KA
-0003f250: 7053 7865 7169 7442 4746 5448 4342 4b46  pSxeqitBGFTHCBKF
-0003f260: 6473 6959 4937 3741 5436 5338 6c30 356e  dsiYI77AT6S8l05n
-0003f270: 6e30 5346 6769 7645 6169 4367 3530 734c  n0SFgivEaiCg50sL
-0003f280: 7871 6f61 4a46 6b72 6f42 4752 4c74 7432  xqoaJFkroBGRLtt2
-0003f290: 7872 7a52 304b 3046 5332 2f57 6a68 6935  xrzR0K0FS2/Wjhi5
-0003f2a0: 4845 6753 5377 4377 7076 352b 634e 666a  HEgSSwCwpv5+cNfj
-0003f2b0: 3474 7377 486d 6261 5533 796f 6343 584d  4tswHmbaU3yocCXM
-0003f2c0: 5158 4742 7567 6776 6d46 3561 2b4b 744a  QXGBuggvmF5a+KtJ
-0003f2d0: 6a4f 4574 6b65 6f6d 6b33 664b 307a 4872  jOEtkeomk3fK0zHr
-0003f2e0: 4877 336e 346a 3343 3831 5674 7235 7441  Hw3n4j3C81Vtr5tA
-0003f2f0: 476e 5352 4344 7252 5278 4851 616b 3064  GnSRCDrRRxHQak0d
-0003f300: 6248 4c74 3359 634b 5971 2f49 5848 486d  bHLt3YcKYq/IXHHm
-0003f310: 3548 4937 2f75 4250 6d49 3942 5263 6469  5HI7/uBPmI9BRcdi
-0003f320: 4431 3442 6849 6b2b 5867 6647 4461 3351  D14BhIk+XgfGDa3Q
-0003f330: 2f4a 6538 5652 484e 6254 7541 446b 6d71  /Je8VRHNbTuADkmq
-0003f340: 4c6b 5732 5779 6942 416d 2b51 7472 546d  LkW2WyiBAm+QtrTm
-0003f350: 6538 3349 5764 4430 6b49 6842 536c 5a47  e83IWdD0kIhBSlZG
-0003f360: 4537 646f 5168 2b59 4267 7267 326b 4d53  E7doQh+YBgrg2kMS
-0003f370: 7272 6d5a 7452 2b77 2b73 6532 5158 5734  rrmZtR+w+se2QXW4
-0003f380: 5274 5a6e 4469 644b 344c 6230 3555 7761  RtZnDidK4Lb05Uwa
-0003f390: 4670 6a79 4331 6c55 4371 5671 482b 724f  FpjyC1lUCqVqH+rO
-0003f3a0: 504f 4c4e 5064 704c 574e 5935 6a42 6136  POLNPdpLWNY5jBa6
-0003f3b0: 6748 446d 6374 4332 4148 4b31 7a6a 2f6c  gHDmctC2AHK1zj/l
-0003f3c0: 3238 3977 6c61 3333 7035 4c6c 6177 6e6b  289wla33p5Llawnk
-0003f3d0: 4865 6777 3474 316d 3461 4e4d 3267 5736  Hegw4t1m4aNM2gW6
-0003f3e0: 7437 507a 356a 4356 4653 7541 4363 3071  t7Pz5jCVFSuACc0q
-0003f3f0: 6356 394b 6955 7463 7055 594c 6e4a 3033  cV9KiUtcpUYLnJ03
-0003f400: 7958 756c 7a51 6b76 6648 6d37 4f65 424d  yXulzQkvfHm7OeBM
-0003f410: 456b 7351 5356 644b 7152 5465 2f6a 7335  EksQSVdKqRTe/js5
-0003f420: 6f6c 702b 5236 5853 366f 646f 542f 7755  olp+R6XS6odoT/wU
-0003f430: 446f 484e 6854 7675 684f 7635 6d74 524a  DoHNhTvuhOv5mtRJ
-0003f440: 794b 4558 3345 5971 514a 4975 4f63 3836  yKEX3EYqQJIuOc86
-0003f450: 534d 4d59 2f71 4f33 3051 3336 5250 326e  SMMY/qO30Q36RP2n
-0003f460: 6666 5555 3645 5834 5342 3070 457a 384a  ffUU6EX4SB0pEz8J
-0003f470: 6334 5972 4735 6878 727a 6562 564a 4a70  c4YrG5hxrzebVJJp
-0003f480: 7545 384a 6d7a 4c62 3178 6f78 5152 744a  uE8JmzLb1xoxQRtJ
-0003f490: 5251 4d66 4836 6266 5073 6f57 4362 4778  RQMfH6bfPsoWCbGx
-0003f4a0: 7545 7755 6b69 7651 4565 677a 3868 7a2b  uEwUkivQEegz8hz+
-0003f4b0: 4375 7a43 766f 4355 5077 3736 576b 2f66  CuzCvoCUPw76Wk/f
-0003f4c0: 396e 7274 3976 2b39 4c32 2b71 6a43 7767  9nrt9v+9L2+qjCwg
-0003f4d0: 325a 7852 6c44 6f79 4233 7135 734b 5747  2ZxRlDoyB3q5sKWG
-0003f4e0: 7577 5739 4d73 4d52 4a79 5854 7962 6364  uwW9MsMRJyXTybcd
-0003f4f0: 4b2b 3069 4b59 4b36 4251 3672 4973 4d71  K+0iKYK6BQ6rIsMq
-0003f500: 4655 6648 435a 544f 6235 6b36 2b4a 492b  FUfHCZTOb5k6+JI+
-0003f510: 6544 6d31 5249 456e 5563 4772 6252 4c63  eDm1RIEnUcGrbRLc
-0003f520: 534a 4445 7332 3635 4245 596f 6f34 5657  SJDEs265BEYoo4VW
-0003f530: 7264 6f41 4438 6267 314f 6639 4737 324e  rdoAD8bg1Of9G72N
-0003f540: 6133 4c7a 7762 4b48 7575 4374 7655 7132  a3LzwbKHuuCtvUq2
-0003f550: 574f 7258 6773 4d74 3330 6c36 714f 6664  WOrXgsMt30l6qOfd
-0003f560: 6b4d 7365 4f67 4850 3948 6451 4a6f 4463  kMseOgHP9HdQJoDc
-0003f570: 452f 6355 6f49 4567 7a41 6632 4d45 5531  E/cUoIEgzAf2MEU1
-0003f580: 4b6f 5246 6279 686e 6b6a 6476 2b79 7262  KoRFbyhnkjdv+yrb
-0003f590: 7a6a 2f36 4732 4847 376e 6b67 4543 5364  zj/6G2HG7nkgECSd
-0003f5a0: 7a71 3757 5174 5672 6132 6d44 3658 6f44  zq7WQtVra2mD6XoD
-0003f5b0: 4245 4a33 3163 5636 4343 3630 6462 4573  BEJ31cV6CC60dbEs
-0003f5c0: 4665 6f73 556f 6a44 6c34 5277 444c 7930  FeosUojDl4RwDLy0
-0003f5d0: 7a6f 4a76 5631 4a70 6c44 546c 7770 5449  zoJvV1JplDTlwpTI
-0003f5e0: 7659 6534 4438 794c 5871 3075 786c 7150  vYe4D8yLXq0uxlqP
-0003f5f0: 3250 4c44 3173 5046 3379 4e6f 4d2f 734d  2PLD1sPF3yNoM/sM
-0003f600: 6166 5639 4472 612b 6764 496f 474f 7773  afV9Dra+gdIoGOws
-0003f610: 4939 6f4f 4541 766f 4d79 6436 4765 6378  I9oOEAvoMyd6Gecx
-0003f620: 6b32 7972 3879 6b6f 3771 364c 454b 4557  k2yr8yko7q6LEKEW
-0003f630: 614a 6232 6c50 5a4e 4e71 795a 6433 4d4b  aJb2lPZNNqyZd3MK
-0003f640: 6d50 6c44 7531 716a 4365 7237 3379 4776  mPlDu1qjCer73yGv
-0003f650: 4b62 3775 5355 4248 7544 6a31 4275 5355  Kb7uSUBHuDj1BuSU
-0003f660: 5952 6e56 4546 7568 4537 7738 3871 6a58  YRnVEFuhE7w88qjX
-0003f670: 544f 3975 4752 476d 426f 5a63 7461 6d42  TO9uGRGmBoZctamB
-0003f680: 6464 652b 6b41 624b 3075 6930 696d 785a  dde+kAbK0ui0imxZ
-0003f690: 2b4d 6d4f 4c6a 4633 4932 7174 6266 2b52  +MmOLjF3I2qtbf+R
-0003f6a0: 342f 7064 6745 5045 2b39 5854 5453 3043  4/pdgEPE+9XTTS0C
-0003f6b0: 456e 5576 4a6f 7335 6d4f 6c56 6749 4e69  EnUvJos5mOlVgINi
-0003f6c0: 7964 2b33 6b37 416e 372f 5449 3765 612f  yd+3k7An7/TI7ea/
-0003f6d0: 786c 7574 6e65 5336 6267 3831 3634 414c  xlutneS6bg8164AL
-0003f6e0: 6f33 676d 5268 4235 5a4b 5371 4970 424a  o3gmRhB5ZKSqIpBJ
-0003f6f0: 5273 3035 4444 3449 6551 2b44 6a49 6568  Rs05DD4IeQ+DjIeh
-0003f700: 5362 5a65 3768 5278 6630 3978 7335 3978  SbZe7hRxf09xs59x
-0003f710: 5762 2b54 412b 705a 5444 3772 6147 3948  Wb+TA+pZTD7raG9H
-0003f720: 2f4b 6d5a 6276 6658 4b74 4771 4969 4d32  /KmZbvfXKtGqIiM2
-0003f730: 5567 6442 7161 4d46 4d73 6847 3677 7256  UgdBqaMFMshG6wrV
-0003f740: 4f57 7079 595a 4f77 444f 316b 6e38 4b59  OWpyYZOwDO1kn8KY
-0003f750: 6539 3951 3970 3361 6f59 396c 3568 312f  e99Q9p3aoY9l5h1/
-0003f760: 5178 5062 3865 746d 7672 4842 6156 792b  QxPb8etmvrHBaVy+
-0003f770: 5a63 4d45 7262 6268 5148 4e4c 6968 7855  ZcMErbbhQHNLihxU
-0003f780: 3345 7559 7146 5334 594e 3053 6878 5058  3EuYqFS4YN0ShxPX
-0003f790: 6765 5437 4a65 332f 416b 5732 356c 6759  geT7Je3/AkW25lgY
-0003f7a0: 5848 3533 585a 6d62 6833 4554 666a 572b  XH53XZmbh3ETfjW+
-0003f7b0: 7371 354b 3456 5064 4d65 6a56 6376 474d  sq5K4VPdMejVcvGM
-0003f7c0: 5857 6b2b 4572 6e73 7a64 4f61 4336 6b67  XWk+ErnszdOaC6kg
-0003f7d0: 5541 434c 5349 4343 4843 5642 7147 3072  UACLSICCHCVBqG0r
-0003f7e0: 4836 7550 7450 754a 4872 6438 3536 544a  H6uPtPuJHrd856TJ
-0003f7f0: 7668 7947 3164 4364 6253 4872 5567 2b35  vhyG1dCdbSHrUg+5
-0003f800: 506f 4350 425a 3030 7772 3936 4946 676f  PoCPBZ00wr96IFgo
-0003f810: 6d59 754b 6730 5231 785a 6e73 7576 6176  mYuKg0R1xZnsuvav
-0003f820: 6875 6441 5458 5743 3474 3237 4b41 5965  hudATXWC4t27KAYe
-0003f830: 3148 7248 724c 534b 5432 6839 4f45 4935  1HrHrLSKT2h9OEI5
-0003f840: 5a54 3630 6132 595a 5254 5279 6844 6145  ZT60a2YZRTRyhDaE
-0003f850: 6441 7348 656c 7479 6136 6c54 582f 735a  dAsHeltya6lTX/sZ
-0003f860: 6956 6131 346b 594f 3842 6b6a 7070 4971  iVa14kYO8BkjppIq
-0003f870: 4752 766c 5571 6a41 7931 6453 3065 502f  GRvlUqjAy1dS0eP/
-0003f880: 4c73 2b6a 4674 626b 7338 4f61 6856 6b6d  Ls+jFtbks8OahVkm
-0003f890: 504c 7471 4d7a 3652 5750 4371 4749 4959  PLtqMz6RWPCqGIIY
-0003f8a0: 5542 7445 346b 6d53 4a57 3334 3446 6741  UBtE4kmSJW344FgA
-0003f8b0: 4f32 494c 747a 386b 4e37 724f 304c 6566  O2ILtz8kN7rO0Lef
-0003f8c0: 6166 7654 635a 4f75 4848 6846 4945 7053  afvTcZOuHHhFIEpS
-0003f8d0: 3154 6d70 744a 7576 2b31 4337 496b 2b42  1TmptJuv+1C7Ik+B
-0003f8e0: 732f 3137 5159 5852 4f45 7a55 4770 5a70  s/17QYXROEzUGpZp
-0003f8f0: 4562 644e 5254 4952 7063 564c 3071 6a32  EbdNRTIRpcVL0qj2
-0003f900: 3639 5776 482f 4335 3735 7353 392f 4e71  69WvH/C575sS9/Nq
-0003f910: 4d51 432b 417a 3358 5265 7963 7767 6465  MQC+Az3XReycwgde
-0003f920: 3569 3765 744a 516d 434d 7144 5877 4163  5i7etJQmCMqDXwAc
-0003f930: 4c62 6364 7842 617a 7637 624e 5433 2b5a  LbcdxBazv7bNT3+Z
-0003f940: 766e 3343 3174 3332 2f48 7a48 4848 6d7a  vn3C1t32/HzHHHmz
-0003f950: 5730 3739 4156 3271 3737 576b 5249 5963  W079AV2q77WkRIYc
-0003f960: 556a 6444 4174 3067 6e63 577a 4734 6d2f  UjdDAt0gncWzG4m/
-0003f970: 536e 4b32 4434 5a51 4473 3732 467a 5734  SnK2D4ZQDs72FzW4
-0003f980: 6244 7165 656e 3354 7442 7438 414c 434a  bDqeen3TtBt8ALCJ
-0003f990: 424f 6343 7743 7938 5463 377a 7157 4f47  BOcCwCy8Tc7zqWOG
-0003f9a0: 6f43 494c 6b37 5878 5144 3770 3871 3446  oCILk7XxQD7p8q4F
-0003f9b0: 3273 7778 4f5a 496f 4931 4245 6534 4650  2swxOZIoI1BEe4FP
-0003f9c0: 3939 7763 6331 5a62 7333 5a4b 7a38 6559  99wcc1Zbs3ZKz8eY
-0003f9d0: 694d 4d56 7677 456c 6962 315a 7670 3368  iMMVvwElib1Zvp3h
-0003f9e0: 3171 3264 354d 4d48 4568 5334 4a65 2b36  1q2d5MMHEhS4Je+6
-0003f9f0: 7247 5748 6a32 3473 2f68 2b35 4449 3262  rGWHj24s/h+5DI2b
-0003fa00: 7152 6e54 6f6a 4552 564b 3058 6b4d 4f6c  qRnTojERVK0XkMOl
-0003fa10: 4b6b 7570 592f 6430 4a6f 3337 6165 7357  KkupY/d0Jo37aesW
-0003fa20: 4a50 3344 4844 3638 5845 755a 4951 4253  JP3DHD68XEuZIQBS
-0003fa30: 5949 7441 7a77 4f57 3262 614c 4768 7464  YItAzwOW2baLGhtd
-0003fa40: 324a 5467 4e6d 4c63 5576 4e70 6131 6e4c  2JTgNmLcUvNpa1nL
-0003fa50: 4f59 5965 3048 7266 6e33 5835 3939 5751  OYYe0Hrfn3X599WQ
-0003fa60: 5966 7445 6277 6d48 6555 4663 4946 4643  YftEbwmHeUFcIFFC
-0003fa70: 3154 6b4b 5441 2b63 6154 4c77 4446 5433  1TkKTA+caTLwDFT3
-0003fa80: 6159 716e 7255 6f35 646f 5073 615a 6369  aYqnrUo5doPsaZci
-0003fa90: 4251 7979 3377 6337 5463 416f 6e34 5a33  BQyy3wc7TcAon4Z3
-0003faa0: 4271 7032 4437 5551 3952 7651 6d6f 626d  Bqp2D7UQ9RvQmobm
-0003fab0: 4873 6932 6757 776e 694c 7341 6268 5330  Hsi2gWwniLsAbhS0
-0003fac0: 774b 4530 456c 3350 5262 7654 6f48 4751  wKE0El3PRbvToHGQ
-0003fad0: 2b72 6446 4a77 4268 2b44 7039 6173 4663  +rdFJwBh+Dp9asFc
-0003fae0: 5536 4b44 5732 7930 6346 3954 4e35 4231  U6KDW2y0cF9TN5B1
-0003faf0: 314f 6d76 4352 4e48 4b35 3170 5348 7238  1OmvCRNHK51pSHr8
-0003fb00: 5268 6b56 6e53 695a 6d6d 7736 6c4a 5059  RhkVnSiZmmw6lJPY
-0003fb10: 7a6f 3268 526c 4b36 4d53 6c55 3674 3368  zo2hRlK6MSlU6t3h
-0003fb20: 4339 4b67 3950 4866 4770 4674 627a 7a6e  C9Kg9PHfGpFtbzzn
-0003fb30: 7951 476e 6251 4241 4751 3662 6964 5242  yQGnbQBAGQ6bidRB
-0003fb40: 6c79 596a 7a46 5366 6874 6f30 6256 7466  lyYjzFSfhto0bVtf
-0003fb50: 3872 614e 2b34 6f38 5a39 4a50 6f58 4d4e  8raN+4o8Z9JPoXMN
-0003fb60: 4171 5647 6230 696c 6156 4764 4644 7469  AqVGb0ilaVGdFDti
-0003fb70: 504c 457a 2b72 2b65 7031 4d6e 4a56 4f4a  PLEz+r+ep1MnJVOJ
-0003fb80: 544f 4565 4963 684e 7863 3655 7156 2f44  TOEeIchNxc6UqV/D
-0003fb90: 635a 6364 2f76 5731 4477 366e 4f59 494e  cZcd/vW1Dw6nOYIN
-0003fba0: 6570 554c 5276 5235 6b4f 4277 4d49 4165  epULRvR5kOBwMIAe
-0003fbb0: 714b 4d76 706d 3454 7030 3631 3946 3936  qKMvpm4Tp0619F96
-0003fbc0: 6679 5752 5978 6843 6a46 4959 6b43 4352  fyWRYxhCjFIYkCCR
-0003fbd0: 4a49 754f 496d 6b54 7968 5653 6250 414b  JIuOImkTyhVSbPAK
-0003fbe0: 3677 322b 6852 3947 5856 5972 4a59 5659  6w2+hR9GXVYrJYVY
-0003fbf0: 4247 6179 4e65 5367 6b6e 5744 5568 4c32  BGayNeSgknWDUhL2
-0003fc00: 6476 3876 7761 3571 2b39 2b56 762b 5431  dv8vwa5q+9+Vv+T1
-0003fc10: 7269 6d38 626d 3356 4d58 6931 5665 6478  rim8bm3VMXi1Vedx
-0003fc20: 704f 5876 5377 5731 5444 3771 5831 6151  pOXvSwW1TD7qX1aQ
-0003fc30: 5042 592b 6950 7535 7438 6f4a 6971 6858  PBY+iPu5t8oJiqhX
-0003fc40: 6141 435a 4c31 4162 5130 6263 7479 7a6b  aACZL1AbQ0bctyzk
-0003fc50: 326b 557a 646c 4a44 346c 682f 7364 786d  2kUzdlJD4lh/sdxm
-0003fc60: 7667 6354 514b 6f4e 3871 6434 7633 5667  vgcTQKoN8qd4v3Vg
-0003fc70: 3763 6562 3054 7230 582f 336e 4570 6e66  7ceb0Tr0X/3nEpnf
-0003fc80: 434c 7341 774f 544e 6431 3967 612f 5075  CLsAwOTNd19ga/Pu
-0003fc90: 3139 6147 3671 5458 3332 7442 5439 6565  19aG6qTX32tBT9ee
-0003fca0: 414f 6744 3070 416e 734c 6164 787a 6370  AOgD0pAnsLadxzcp
-0003fcb0: 4d64 584d 3462 4450 416a 304a 6f6c 5458  MdXM4bDPAj0JolTX
-0003fcc0: 3634 5255 616f 522b 3739 7547 5557 7465  64RUaoR+79uGUWte
-0003fcd0: 5335 586d 594f 5868 4a66 3579 7772 5a75  S5XmYOXhJf5ywrZu
-0003fce0: 674a 3436 485a 6f4a 306c 5a30 3663 4c43  gJ46HZoJ0lZ06cLC
-0003fcf0: 6d36 6167 5247 7869 554b 6367 4542 6341  m6agRGxiUKcgEBcA
-0003fd00: 7352 346f 4335 3159 717a 4276 7435 456f  sR4oC51YqzBvt5Eo
-0003fd10: 4a79 5368 3965 6b77 4648 784f 6837 4252  JySh9ekwFHxOh7BR
-0003fd20: 6f74 462b 5041 4472 4677 6f41 456c 4e77  otF+PADrFwoAElNw
-0003fd30: 674f 6238 396b 6642 2f7a 3279 377a 616f  gOb89kfB/z2y7zao
-0003fd40: 7550 704f 6256 3244 526d 3570 3747 3658  uPpObV2DRm5p7G6X
-0003fd50: 414e 4659 334a 4c74 3476 366d 3544 5871  ANFY3JLt4v6m5DXq
-0003fd60: 5447 5450 7349 5857 4c31 764e 4d62 3468  TGTPsIXWL1vNMb4h
-0003fd70: 737a 6e50 586e 486a 6c65 6934 4564 7a2b  sznPXnHjlei4Edz+
-0003fd80: 3631 3450 4d6e 3838 7336 5570 6374 4958  614PMn88s6UpctIX
-0003fd90: 6957 7430 3453 476d 4e57 2f35 456c 5464  iWt04SGmNW/5ElTd
-0003fda0: 2f55 5457 5341 386c 5175 7569 6342 4a79  /UTWSA8lQuuicBJy
-0003fdb0: 5061 4a56 5a65 754a 7551 3064 6f78 6376  PaJVZeuJuQ0doxcv
-0003fdc0: 424c 4f6e 5646 6a4a 764a 2f4f 464c 3850  BLOnVFjJvJ/OFL8P
-0003fdd0: 552b 7065 7763 5a68 6f59 7848 5254 5a69  U+pewcZhoYxHRTZi
-0003fde0: 4f69 676c 6b77 4178 4b6a 655a 4447 3077  OiglkwAxKjeZDG0w
-0003fdf0: 6d4f 6953 4858 6c6d 7661 5742 3352 4935  mOiSHXlmvaWB3RI5
-0003fe00: 414c 7931 4471 3045 4745 764a 3949 4d57  ALy1Dq0EGEvJ9IMW
-0003fe10: 7064 7233 384e 5a4b 4473 566f 6952 4853  pdr38NZKDsVoiRHS
-0003fe20: 6876 4943 4f79 4948 414e 4e47 3673 6d72  hvICOyIHANNG6smr
-0003fe30: 4530 7a66 5773 6266 7537 4b49 766b 5451  E0zfWsbfu7KIvkTQ
-0003fe40: 786d 597a 6642 2b6b 306f 6b51 704a 5177  xmYzfB+k0okQpJQw
-0003fe50: 7579 337a 3157 456f 3753 4d6c 4866 6670  uy3z1WEo7SMlHffp
-0003fe60: 6f61 7538 316a 3955 6b32 6871 6455 694a  oau81j9Uk2hqdUiJ
-0003fe70: 3046 6f59 6b69 4f62 6167 7351 6c49 326f  0FoYkiObagsQlI2o
-0003fe80: 6236 6872 6b39 637a 3354 7746 7976 452b  b6hrk9cz3TwFyvE+
-0003fe90: 4a6c 4d74 3063 416a 4d57 7161 546d 6a69  JlMt0cAjMWqaTmji
-0003fea0: 6979 4161 4254 6c50 7249 6b4a 624b 4530  iyAaBTlPrIkJbKE0
-0003feb0: 6d2f 426b 6a67 677a 6145 7247 624d 6844  m/BkjggzaErGbMhD
-0003fec0: 4275 7249 5a74 462f 376a 6a6a 6172 6e4c  BurIZtF/7jjjarnL
-0003fed0: 6534 5468 5a4c 7645 636d 3449 6371 3359  e4ThZLvEcm4Icq3Y
-0003fee0: 474e 6179 7036 7a74 7a65 6732 624d 5957  GNayp6ztzeg2bMYW
-0003fef0: 654d 3934 3046 5032 4c2b 4970 4778 5241  eM940FP2L+IpGxRA
-0003ff00: 6b43 7079 5534 2b4d 6e55 614b 5577 3051  kCpyU4+MnUaKUw0Q
-0003ff10: 3530 396e 3773 372f 5556 6966 7947 622b  509n7s7/UVifyGb+
-0003ff20: 7868 5466 364e 524b 587a 7041 4562 7949  xhTf6NRKXzpAEbyI
-0003ff30: 4b38 434c 5242 562f 724e 5173 4f74 3962  K8CLRBV/rNQsOt9b
-0003ff40: 3167 454d 354f 434e 7270 6656 434b 7373  1gEM5OCNrpfVCKss
-0003ff50: 6e77 3744 6e52 706a 454e 3674 2b43 4945  nw7DnRpjEN6t+CIE
-0003ff60: 704a 6470 4a6a 575a 734a 676a 4d57 696c  pJdpJjWZsJgjMWil
-0003ff70: 6e43 3949 7779 6468 306f 4836 4272 7452  nC9Iwydh0oH6BrtR
-0003ff80: 3235 4d42 7256 4739 4b32 7a71 534a 3533  25MBrVG9K2zqSJ53
-0003ff90: 726b 7233 7143 7877 7670 336f 7047 6655  rkr3qCxwvp3opGfU
-0003ffa0: 5747 774e 3870 6b71 7267 5a37 7755 716d  WGwN8pkqrgZ7wUqm
-0003ffb0: 6841 2f65 6f47 3362 3339 4453 5532 366e  hA/eoG3b39DSU26n
-0003ffc0: 7434 6774 5634 514c 7444 5974 4f71 6d68  t4gtV4QLtDYtOqmh
-0003ffd0: 304b 3045 5377 2f71 5876 5575 7562 6734  0K0ESw/qXvUuubg4
-0003ffe0: 3245 4647 3071 5267 7743 5a2b 7735 4d47  2EFG0qRgwCZ+w5MG
-0003fff0: 7137 4a70 7346 6232 7672 6847 3957 6f58  q7JpsFb2vrhG9WoX
-00040000: 7772 4154 4852 5563 706a 684c 4a55 5175  wrATHRUcpjhLJUQu
-00040010: 3657 6442 6d77 5a77 6b61 7573 4235 4b69  6WdBmwZwkausB5Ki
-00040020: 7a73 7877 5866 4575 7571 6e65 364e 5a50  zsxwXfEuuqne6NZP
-00040030: 3166 3248 3739 4133 6875 6267 4f49 644b  1f2H79A3hubgOIdK
-00040040: 7041 3931 3058 424d 5973 3147 6974 6d41  pA910XBMYs1GitmA
-00040050: 644a 5244 464e 676a 554c 3943 5657 6b77  dJRDFNgjUL9CVWkw
-00040060: 4f30 4173 7756 376f 4269 4847 716e 5848  O0AswV7oBiHGqnXH
-00040070: 6d32 6a33 5336 7647 506b 704d 3176 6736  m2j3S6vGPkpM1vg6
-00040080: 4c44 7866 7136 4362 4479 306e 4c48 3168  LDxfq6CbDy0nLH1h
-00040090: 5831 6575 7858 3965 7954 6b37 6936 626d  X1euxX9eyTk7i6bm
-000400a0: 7379 414f 4d32 774b 3631 344e 414e 7974  syAOM2wK614NANyt
-000400b0: 3370 317a 644a 4e54 2f2f 6736 6657 5454  3p1zdJNT//g6fWTT
-000400c0: 504c 6349 6b66 4b79 636b 647a 3757 2f76  PLcIkfKyckdz7W/v
-000400d0: 5565 4155 2f69 5635 4470 7752 6b69 4335  UeAU/iV5DpwRkiC5
-000400e0: 6f78 3263 6254 4279 6639 6733 7462 5252  ox2cbTByf9g3tbRR
-000400f0: 3371 3178 7633 676a 574d 6e66 306d 6331  3q1xv3gjWMnf0mc1
-00040100: 7237 454a 6565 5239 5449 4d34 3131 5877  r7EJeeR9TIM411Xw
-00040110: 544c 646b 2b4e 5834 4e74 312f 4f63 4459  TLdk+NX4Nt1/OcDY
-00040120: 524f 7556 766f 5350 545a 5754 6167 5569  ROuVvoSPTZWTagUi
-00040130: 6e56 7646 6f42 4557 6f42 375a 5349 6d42  nVvFoBEWoB7ZSImB
-00040140: 596c 4163 4339 5174 3070 5261 5441 2f43  YlAcC9Qt0pRaTA/C
-00040150: 3278 6551 4a56 7256 7a73 3558 6b7a 6567  2xeQJVrVzs5Xkzeg
-00040160: 314b 4331 4344 7679 4141 6a35 5975 4869  1KC1CDvyAAj5YuHi
-00040170: 2f70 6e55 4c6e 3137 5269 4872 7755 5958  /pnULn17RiHrwUYX
-00040180: 3141 4c32 5065 7143 716d 5234 6855 5659  1AL2PeqCqmR4hUVY
-00040190: 386f 6167 7971 697a 5047 6572 3072 7833  8oagyqizPGer0rx3
-000401a0: 7979 6b30 5a50 4846 5234 7563 4933 6372  yyk0ZPHFR4ucI3cr
-000401b0: 6d55 654c 5256 5032 3642 5031 6645 484d  mUeLRVP26BP1fEHM
-000401c0: 5070 4231 3058 3357 5364 7147 6c43 6161  PpB10X3WSdqGlCaa
-000401d0: 4c56 5136 6472 6643 3561 556f 4149 416c  LVQ6drfC5aUoAIAl
-000401e0: 5147 7075 4a4b 7a51 7950 2f4a 7543 6437  QGpuJKzQyP/JuCd7
-000401f0: 5978 7164 2b55 3235 4b2b 4b4d 585a 5766  Yxqd+U25K+KMXZWf
-00040200: 786b 7565 4a35 4852 7237 4f79 6471 3443  xkueJ5HRr7Oydq4C
-00040210: 3477 5751 556e 7842 7557 4278 652f 7179  4wWQUnxBuWBxe/qy
-00040220: 7867 5842 4a59 626b 7468 6430 394c 6e38  xgXBJYbkthd09Ln8
-00040230: 4f70 6e47 7730 4132 386f 4f74 6978 7a57  OpnGw0A28oOtixzW
-00040240: 7153 7441 5270 5641 5935 4e45 326f 3064  qStARpVAY5NE2o0d
-00040250: 734b 6d70 7343 4b56 6a56 4172 5241 4e50  sKmpsCKVjVArRANP
-00040260: 2f33 7957 712b 5738 4663 3349 424d 5241  /3yWq+W8Fc3IBMRA
-00040270: 5263 7542 2f53 3674 6574 6135 747a 7452  RcuB/S6teta5tztR
-00040280: 7269 2f37 5843 4636 2b58 5a4c 7456 6457  ri/7XCF6+XZLtVdW
-00040290: 5773 4459 7738 5134 764e 4b33 7666 6f61  WsDYw8Q4vNK3vfoa
-000402a0: 6473 6f53 2f55 7554 686e 464c 6d79 6d51  dsoS/UuThnFLmymQ
-000402b0: 5444 4c4f 5574 3765 7138 6849 2f35 7042  TDLOUt7eq8hI/5pB
-000402c0: 4e56 5658 3856 6178 4952 3972 3636 4967  NVVX8VaxIR9r66Ig
-000402d0: 675a 6d6a 6c52 5478 4546 4d55 4543 4945  gZmjlRTxEFMUECIE
-000402e0: 454b 5357 4867 5345 4a45 6953 3571 6a59  EKSWHgSEJEiS5qjY
-000402f0: 2f36 3646 5a4f 5862 7474 5230 4e4e 666a  /66FZOXbttR0NNfj
-00040300: 5944 3263 6b38 4435 4b6f 6457 316d 6f41  YD2ck8D5KodW1moA
-00040310: 6764 6331 7161 4f43 3374 5045 5733 3555  gdc1qaOC3tPEW35U
-00040320: 314f 5052 6964 5379 667a 2f63 7157 5034  1OPRidSyfz/cqWP4
-00040330: 336f 484e 2f47 354a 5652 394d 6b55 4232  3oHN/G5JVR9MkUB2
-00040340: 5a41 6831 5853 7541 3545 4947 4e51 744b  ZAh1XSuA5EIGNQtK
-00040350: 5667 4544 3949 4e42 3259 314d 622b 4143  VgED9INB2Y1Mb+AC
-00040360: 4379 336e 4365 5438 5954 686c 6f63 6967  Cy3nCeT8YThlocig
-00040370: 5030 5a52 6476 4e39 6c48 562b 6568 546e  P0ZRdvN9lHV+ehTn
-00040380: 4573 4439 646b 384c 6855 766b 7257 6172  EsD9dk8LhUvkrWar
-00040390: 2f62 7436 4e76 7043 747a 5635 6131 674b  /bt6NvpCtzV5a1gK
-000403a0: 5859 344a 3041 6e6a 3171 5663 766c 6b4b  XY4J0Anj1qVcvlkK
-000403b0: 3939 466b 734e 564e 5138 4272 6245 3649  99FksNVNQ8BrbE6I
-000403c0: 6a6b 6f52 5135 4542 7651 516f 676c 2b4e  jkoRQ5EBvQQogl+N
-000403d0: 2b54 6575 4b33 4b77 4f6e 6b4a 7442 7867  +TeuK3KwOnkJtBxg
-000403e0: 7944 506e 6132 4654 5335 636c 7149 4971  yDPna2FTS5clqIIq
-000403f0: 3273 735a 4774 5733 304a 4368 4661 3435  2ssZGtW30JChFa45
-00040400: 6e4c 572b 695a 316e 5867 4746 5830 3545  nLW+iZ1nXgGFX05E
-00040410: 7843 5074 3232 4c39 4b68 3159 7157 6d7a  xCPt22L9Kh1YqWmz
-00040420: 5450 7769 3048 5145 364d 4272 2f72 2f7a  TPwi0HQE6MBr/r/z
-00040430: 7648 5976 664a 4449 6c58 734d 412b 6d50  vHYvfJDIlXsMA+mP
-00040440: 4f46 6537 617a 4e6f 3231 6f6c 6e70 7767  OFe7azNo21olnpwg
-00040450: 7a70 7469 396b 3374 5770 6171 726b 746f  zpti9k3tWpaqrkto
-00040460: 4336 4a67 632b 4c52 7635 7a37 456f 4d69  C6Jgc+LRv5z7EoMi
-00040470: 4278 4341 6c41 7365 7a76 4a67 6736 7748  BxCAlAsezvJgg6wH
-00040480: 4f4a 2f7a 5653 5349 496f 7036 3362 3344  OJ/zVSSIIop63b3D
-00040490: 6655 6c34 4548 3246 4845 6b57 3953 6a6d  fUl4EH2FHEkW9Sjm
-000404a0: 5352 4964 6542 7130 776e 414b 526e 7a74  SRIdeBq0wnAKRnzt
-000404b0: 6d63 7565 654a 7971 466e 4747 506e 6330  mcueeJyqFnGGPnc0
-000404c0: 7972 5735 7230 5753 304f 7574 5a36 4531  yrW5r0WS0OutZ6E1
-000404d0: 5172 326e 4e38 6e77 6d58 5a32 5833 7158  Qr2nN8nwmXZ2X3qX
-000404e0: 4d46 2b64 4279 3961 4766 5273 5572 6265  MF+dBy9aGfRsUrbe
-000404f0: 6264 3943 766e 4131 5662 5566 6776 5559  bd9CvnA1VbUfgvUY
-00040500: 7033 7843 4d58 2b35 554f 352f 6171 5872  p3xCMX+5UO5/aqXr
-00040510: 7966 734b 4773 3745 4733 7442 4c4a 6d76  yfsKGs7EG3tBLJmv
-00040520: 3839 4c79 6c32 644c 6856 4b63 7859 3370  89Lyl2dLhVKcxY3p
-00040530: 7952 4d39 4d70 7541 6e67 7375 3477 6665  yRM9MpuAngsu4wfe
-00040540: 7349 6f54 6f48 4547 6179 684c 4459 4673  sIoToHEGayhLDYFs
-00040550: 6753 4556 4e71 7377 6e66 7567 4c4a 6762  gSEVNqswnfugLJgb
-00040560: 6f53 4743 6870 334d 6247 7568 7575 4c6d  oSGChp3MbGuhuuLm
-00040570: 4d57 3434 4d70 5a43 4e7a 6537 6330 612b  MW44MpZCNze7c0a+
-00040580: 3362 4449 3545 4879 7150 3266 6e71 6133  3bDI5EHyqP2fnqa3
-00040590: 5669 656f 3276 4a6d 6f72 6179 6c4a 7652  Vieo2vJmoraylJvR
-000405a0: 4f4c 6455 5a6d 5538 6b57 394e 577a 6657  OLdUZmU8kW9NWzfW
-000405b0: 3262 5a38 4b76 666b 7a78 5162 3151 3454  2bZ8KvfkzxQb1Q4T
-000405c0: 6b51 476d 536a 4530 4836 6765 4274 674f  kQGmSjE0H6geBtgO
-000405d0: 4147 316b 682b 5932 634f 6164 6c36 7573  AG1kh+Y2cOadl6us
-000405e0: 2b53 6a68 5676 7157 4a61 5744 3561 656b  +SjhVvqWJaWD5aek
-000405f0: 6e61 334c 7a48 6c72 6176 4d6e 6b51 4d43  na3LzHlravMnkQMC
-00040600: 3638 3137 4b4e 754d 3748 3067 4351 3435  6817KNuM7H0gCQ45
-00040610: 4e67 6255 6563 6d77 7232 4d41 5a59 4d75  NgbUecmwr2MAZYMu
-00040620: 6931 494d 6762 4645 4154 3648 4f54 4d61  i1IMgbFEAT6HOTMa
-00040630: 6a46 4c31 5755 2f4b 4f44 5637 574e 5665  jFL1WU/KODV7WNVe
-00040640: 6d6f 736a 5677 4843 717a 3544 634c 4c35  mosjVwHCqz5DcLL5
-00040650: 6e35 345a 546e 5957 5531 6f53 6c44 3656  n54ZTnYWU1oSlD6V
-00040660: 5872 576b 7571 7265 4175 596c 5743 5a61  XrWkuqreAuYlWCZa
-00040670: 6272 6663 382f 7849 5944 6e30 546f 736c  brfc8/xIYDn0Tosl
-00040680: 6963 6969 5539 7961 6872 7455 336d 4f54  iciiU9yahrtU3mOT
-00040690: 5472 5654 6d7a 644b 7254 7567 3930 4774  TrVTmzdKrTug90Gt
-000406a0: 6b52 6230 3750 4f31 3366 756a 5957 6341  kRb07PO13fujYWcA
-000406b0: 6b76 6e64 6a56 5361 5464 7470 4e34 6a66  kvndjVSaTdtpN4jf
-000406c0: 6b51 5441 396e 4147 5752 7a7a 4532 6742  kQTA9nAGWRzzE2gB
-000406d0: 7744 6d4c 334c 4554 4776 4d55 454d 6644  wDmL3LETGvMUEMfD
-000406e0: 4e30 4b75 4548 4170 7269 6834 6251 5351  N0KuEHAprih4bQSQ
-000406f0: 5373 7644 6164 7166 4378 4454 6f5a 6c30  SsvDadqfCxDToZl0
-00040700: 4f76 456d 3535 5058 4656 5844 5370 6d46  OvEm55PXFVXDSpmF
-00040710: 5869 3537 7249 4646 7139 4c42 6e58 5635  Xi57rIFFq9LBnXV5
-00040720: 5976 4f44 7542 6833 3835 3043 5538 5442  YvODuBh3850CU8TB
-00040730: 5270 6e63 4645 6533 4967 6148 5256 5851  RpncFEe3IgaHRVXQ
-00040740: 644b 4839 494f 4e57 3379 4a70 3032 5839  dKH9IONW3yJp02X9
-00040750: 3061 5764 6142 4676 5849 3764 6730 6a6c  0aWdaBFvXI7dg0jl
-00040760: 6239 6839 6850 6e70 7261 6b51 696e 5337  b9h9hPnprakQinS7
-00040770: 344c 5556 337a 3431 334b 5231 366f 6477  4LUV3z413KR16odw
-00040780: 514f 5244 4a74 7079 3761 7571 314c 5470  QORDJtpy7auq1LTp
-00040790: 616b 656a 6549 6459 6f6e 4f69 7162 3135  akejeIdYonOiqb15
-000407a0: 7043 3877 3532 702b 5638 4c30 4f65 7265  pC8w52p+V8L0Oere
-000407b0: 6a41 3567 4844 3933 6d65 6d2f 454c 4e5a  jA5gHD93mem/ELNZ
-000407c0: 4344 7a56 7551 5849 6738 4333 4775 6675  CDzVuQXIg8C3Gufu
-000407d0: 6332 647a 5556 4a64 7469 517a 314c 4268  c2dzUVJdtiQz1LBh
-000407e0: 3234 5a6b 6570 365a 5779 684a 3246 5a2f  24Zkep6ZWyhJ2FZ/
-000407f0: 6c5a 4a78 544f 4f4d 3334 3141 4a38 3279  lZJxTOOM341AJ82y
-00040800: 4148 5069 5934 6a76 5363 7237 4d4d 7a31  AHPiY4jvScr7MMz1
-00040810: 2f58 6f34 634f 4c78 796d 3150 3542 6275  /Xo4cOLxym1P5Bbu
-00040820: 7461 3972 6935 4542 4d76 6951 2f37 3657  ta9ri5EBMviQ/76W
-00040830: 6c7a 5836 684b 6466 526b 4176 7447 304d  lzX6hKdfRkAvtG0M
-00040840: 4f35 7562 4b62 7166 5330 4b34 7a62 6b31  O5ubKbqfS0K4zbk1
-00040850: 4572 324a 4635 7830 3474 454a 6e30 5245  Er2JF5x04tEJn0RE
-00040860: 7031 4174 5143 5058 4f70 7670 6649 6e58  p1AtQCPXOpvpfInX
-00040870: 354f 6274 4d37 5a4c 2f4b 6237 526f 456e  5ObtM7ZL/Kb7RoEn
-00040880: 3853 6a69 6639 7977 5a69 6852 3346 5739  8Sjif9ywZihR3FW9
-00040890: 6c37 6b44 7069 5a38 784c 6e65 4a6b 6b50  l7kDpiZ8xLneJkkP
-000408a0: 7841 6749 6858 6641 794e 7a74 4a35 3963  xAgIhXfAyNztJ59c
-000408b0: 7770 476f 5464 6f4c 6a4d 4d6f 7032 4d4c  wpGoTdoLjMMop2ML
-000408c0: 6f56 564b 3439 5534 3632 2b58 4471 6337  oVVK49U462+XDqc7
-000408d0: 697a 6a73 544f 2f52 666c 3834 366f 757a  izjsTO/Rfl846ouz
-000408e0: 6438 7732 5349 304b 4d70 4d75 3853 7663  d8w2SI0KMpMu8Svc
-000408f0: 6733 5571 5173 522f 4f53 4c4b 2b44 495a  g3UqQsR/OSLK+DIZ
-00040900: 5966 5748 7972 636a 6757 6667 6d71 4546  YfWHyrcjgWfgmqEF
-00040910: 664c 5131 5742 5237 4762 326a 6d53 4978  fLQ1WBR7Gb2jmSIx
-00040920: 6332 6e59 5844 5039 7132 552f 4f62 4733  c2nYXDP9q2U/ObG3
-00040930: 672f 6853 532b 6254 6236 6c6d 5337 704f  g/hSS+bTb6lmS7pO
-00040940: 3068 392f 6d56 7675 4e68 5975 4144 7965  0h9/mVvuNhYuADye
-00040950: 4232 7867 4170 6778 495a 5072 3756 7372  B2xgApgxIZPr7Vsr
-00040960: 2b73 5a57 702f 3968 4d77 4a45 554b 4447  +sZWp/9hMwJEUKDG
-00040970: 4f58 7744 7873 3276 7a36 3732 6e73 6658  OXwDxs2vz672nsfX
-00040980: 4168 3978 2f61 5472 5a71 3339 796a 6637  Ah9x/aTrZq39yjf7
-00040990: 3457 3438 6550 6469 3631 7643 4b47 7147  4W48ePdi61vCKGqG
-000409a0: 4d6c 3742 6339 5136 4b53 4752 3554 4a41  Ml7Bc9Q6KSGR5TJA
-000409b0: 4e59 494a 384b 2b45 7558 314d 3042 3047  NYIJ8K+EuX1M0B0G
-000409c0: 434f 4b4a 2b50 5231 6742 6552 522f 3975  COKJ+PR1gBeRR/9u
-000409d0: 7530 4c6a 4d6e 5476 366b 734b 5748 6b35  u0LjMnTv6ksKWHk5
-000409e0: 7446 4b54 6b51 3136 646b 6259 7a53 314d  tFKTkQ16dkbYzS1M
-000409f0: 5335 6b62 637a 3068 4446 7451 7043 3359  S5kbcz0hDFtQpC3Y
-00040a00: 7134 6658 7773 3236 6462 2b48 4c55 4c78  q4fXws26db+HLULx
-00040a10: 5656 7166 5770 5044 7269 3257 5139 5953  VVqfWpPDri2WQ9YS
-00040a20: 3761 6c57 2f4c 4a73 3674 6550 5036 3351  7alW/LJs6tePP63Q
-00040a30: 4833 726f 7a30 624f 686f 5170 5630 596d  H3roz0bOhoQpV0Ym
-00040a40: 764a 4270 7949 474b 4364 4149 546f 4948  vJBpyIGKCdAIToIH
-00040a50: 6477 634f 4c43 4c4a 6872 4b44 516b 4b53  dwcOLCLJhrKDQkKS
-00040a60: 3172 6456 624d 4877 2b6b 4b54 4475 2b4c  1rdVbMHw+kKTDu+L
-00040a70: 6467 356e 546e 6246 392b 365a 6233 6570  dg5nTnbF9+6Zb3ep
-00040a80: 4f50 636a 4831 706e 6e76 7854 7769 794c  OPcjH1pnnvxTwiyL
-00040a90: 3473 5954 3077 4a37 5a62 6873 3664 6753  4sYT0wJ7Zbhs6dgS
-00040aa0: 382b 2f37 634e 616e 6d4c 4576 4b52 495a  8+/7cNanmLEvKRIZ
-00040ab0: 3368 687a 6c6b 4736 7563 5665 6366 5557  3hhzlkG6ucVecfUW
-00040ac0: 726a 6c59 6b75 7055 6730 4e42 3079 6453  rjlYkupUg0NB0ydS
-00040ad0: 3155 6e7a 446e 674f 6879 4247 4674 7962  1UnzDngOhyBGFtyb
-00040ae0: 4e6e 6434 356d 5267 7774 6a43 4c54 6641  Nnd45mRgwtjCLTfA
-00040af0: 7159 6167 5678 6168 4862 3032 7858 7231  qYagVxahHb02xXr1
-00040b00: 5362 7372 722b 494b 494a 6f66 357a 4936  Sbsrr+IKIJof5zI6
-00040b10: 5473 5845 3237 7936 6263 4d45 4750 362b  TsXE27y6bcMEGP6+
-00040b20: 7a6c 6348 5a6e 5263 3476 6675 5054 4976  zlcHZnRc4vfuPTIv
-00040b30: 7138 424f 6947 794a 4931 484e 4530 6343  q8BOiGyJI1HNE0cC
-00040b40: 7934 4255 3334 3537 4e56 6b44 3345 6751  y4BU3457NVkD3EgQ
-00040b50: 7751 6436 5a59 4573 484a 7041 6b47 452b  wQd6ZYEsHJpAkGE+
-00040b60: 4938 4656 5959 314e 6f54 3434 6f6b 4369  I8FVYY1NoT44okCi
-00040b70: 5a58 4672 4d6d 7043 442b 5569 4644 5558  ZXFrMmpCD+UiFDUX
-00040b80: 6b64 4775 486c 3765 7239 7031 574c 7079  kdGuHl7er9p1WLpy
-00040b90: 4f2f 2f57 786c 3455 4246 3877 3146 7578  O//Wxl4UBF8w1Fux
-00040ba0: 5733 5679 4a2b 3944 2f79 5a70 4d77 664c  W3VyJ+9D/yZpMwfL
-00040bb0: 6265 3854 7771 5341 614f 6d6d 3151 3249  be8TwqSAaOmm1Q2I
-00040bc0: 676b 6a6e 6271 3354 7667 6568 3267 6942  gkjnbq3Tvgeh2giB
-00040bd0: 7763 7576 3072 7163 7251 4647 4347 4c6a  wcuv0rqcrQFGCGLj
-00040be0: 574f 6b32 6548 6d55 6233 4b51 6a6b 4369  WOk2eHmUb3KQjkCi
-00040bf0: 7471 3244 5964 5568 6c54 4e77 4a6b 7646  tq2DYdUhlTNwJkvF
-00040c00: 7837 2f32 6971 6932 482f 3839 7777 3569  x7/2iqi2H/89ww5i
-00040c10: 377a 3766 782f 2f35 5652 7430 4236 4158  7z7fx//5VRt0B6AX
-00040c20: 5873 7255 7048 4535 7055 3467 494f 5972  XsrUpHE5pU4gIOYr
-00040c30: 5277 4868 4e2b 7a76 7076 4641 6c4d 336e  RwHhN+zvpvFAlM3n
-00040c40: 4857 7a79 3149 6934 3262 4241 5651 5241  HWzy1Ii42bBAVQRA
-00040c50: 436e 4b46 4779 5830 5366 5259 3374 7875  CnKFGyX0SfRY3txu
-00040c60: 4b75 5061 4776 346c 464a 4e46 4f78 6f4f  KuPaGv4lFJNFOxoO
-00040c70: 7a74 4f50 4273 4d76 4c46 6d5a 4e2b 446f  ztOPBsMvLFmZN+Do
-00040c80: 4d75 3770 3545 722f 5242 4c6b 4543 4649  Mu7p5Er/RBLkECFI
-00040c90: 4246 7835 6748 7455 5870 6770 2b4e 7278  BFx5gHtUXpgp+Nrx
-00040ca0: 6668 6830 635a 5566 766b 3576 3055 6c6a  fhh0cZUfvk5v0Ulj
-00040cb0: 314d 4359 725a 4f57 4b5a 4575 2b30 7739  1MCYrZOWKZEu+0w9
-00040cc0: 5156 6741 7168 7941 6155 2b51 4d2b 3433  QVgAqhyAaU+QM+43
-00040cd0: 3572 596d 4264 7456 3636 3759 596c 7634  5rYmBdtV667YYlv4
-00040ce0: 6445 4d64 6446 5871 5574 5730 7073 5869  dEMddFXqUtW0psXi
-00040cf0: 2f4f 6542 4e75 6e45 5372 776d 5362 2b6c  /OeBNunESrwmSb+l
-00040d00: 5a52 4837 627a 556b 2f30 5837 4939 636b  ZRH7bzUk/0X7I9ck
-00040d10: 4235 3756 304b 3047 6d54 3763 4754 6d44  B57V0K0GmT7cGTmD
-00040d20: 7076 4b50 2b2b 5536 3030 3175 464e 744c  pvKP++U6001uFNtL
-00040d30: 3947 6d5a 4679 574a 306b 3436 6666 5258  9GmZFyWJ0k46ffRX
-00040d40: 3677 564c 5565 7a65 3275 484f 6d58 4950  6wVLUeze2uHOmXIP
-00040d50: 3365 594a 7462 5174 5962 7966 734e 6b6a  3eYJtbQtYbyfsNkj
-00040d60: 4a4a 3742 5a54 6d4c 5276 3874 6541 554a  JJ7BZTmLRv8teAUJ
-00040d70: 796c 454e 4868 4748 4c47 4d75 6d63 3936  ylENHhGHLGMumc96
-00040d80: 636e 6164 307a 7748 437a 7848 4e75 6a4f  cnad0zwHCzxHNujO
-00040d90: 5462 5134 666d 5565 7330 7249 5571 7736  TbQ4fmUes0rIUqw6
-00040da0: 3575 4c57 3743 494a 5846 6866 4f57 356f  5uLW7CIJXFhfOW5o
-00040db0: 5379 6641 455a 5470 394f 5743 2b61 4470  SyfAEZTp9OWC+aDp
-00040dc0: 3944 396c 6778 584a 7750 7a58 2b67 7571  9D9lgxXJwPzX+guq
-00040dd0: 6433 5971 3752 4e31 4a56 435a 424e 4e43  d3Yq7RN1JVCZBNNC
-00040de0: 6276 5050 5a4d 7164 5065 6b44 5173 546f  bvPPZMqdPekDQsTo
-00040df0: 6952 7a6b 4d67 5957 475a 3041 515a 4d6e  iRzkMgYWGZ0AQZMn
-00040e00: 7133 6b6d 7859 4867 316b 4751 7248 7977  q3kmxYHg1kGQrHyw
-00040e10: 6b79 454e 416b 4e71 5149 4232 5241 3945  kyENAkNqQIB2RA9E
-00040e20: 7442 4945 6837 7041 5a64 616c 3876 7959  tBIEh7pAZdal8vyY
-00040e30: 6142 6c71 4644 7234 4845 4947 5662 3645  aBlqFDr4HEIGVb6E
-00040e40: 3849 6c58 4472 5478 2b4e 4877 7078 4161  8IlXDrTx+NHwpxAa
-00040e50: 6869 646e 5a46 6a6d 7958 3550 626d 572f  hidnZFjmyX5PbmW/
-00040e60: 3556 6a49 716d 6941 4267 4369 6a50 7176  5VjIqmiABgCijPqv
-00040e70: 5a34 5030 454e 3747 434a 397a 2b64 4e42  Z4P0EN7GCJ9z+dNB
-00040e80: 514a 7950 4168 2b47 6137 5964 6e75 6572  QJyPAh+Ga7Ydnuer
-00040e90: 5761 7246 5676 516b 515a 4d69 7239 3666  WarFVvQkQZMir96f
-00040ea0: 6471 756a 4837 4e53 4553 5451 6f72 3466  dqujH7NSESTQor4f
-00040eb0: 6a63 7a49 4156 6878 3552 6474 5749 776a  jczIAVhx5RdtWIwj
-00040ec0: 556a 6332 656e 6867 344c 2f4b 2f44 4463  Ujc2enhg4L/K/DDc
-00040ed0: 4264 6a62 3871 7637 6964 5455 6575 2b43  Bdjb8qv7idTUeu+C
-00040ee0: 4369 7276 6b76 696e 594e 6769 4377 4748  CirvkvinYNgiCwGH
-00040ef0: 5872 4e38 376a 5858 6246 5131 546b 6756  XrN87jXXbFQ1TkgV
-00040f00: 3146 6b4d 556b 6a56 6c39 7964 4b46 674d  1FkMUkjVl9ydKFgM
-00040f10: 6b30 7477 6c72 2f74 6261 634c 4968 3832  k0twlr/tbacLIh82
-00040f20: 384f 3157 6f4c 5254 5676 534d 7332 2f50  8O1WoLRTVvSMs2/P
-00040f30: 722b 4644 6a46 7539 6355 3262 4166 4b39  r+FDjFu9cU2bAfK9
-00040f40: 3164 734b 7671 7574 6b50 3044 2f6a 5834  1dsKvqutkP0D/jX4
-00040f50: 5a43 4e47 7653 666f 7231 5870 4754 3963  ZCNGvSfor1XpGT9c
-00040f60: 3659 7537 7261 3933 3176 4d71 387a 5748  6Yu7ra931vMq8zWH
-00040f70: 6249 5967 4244 4155 6d7a 4270 6b5a 394d  bIYgBDAUmzBpkZ9M
-00040f80: 394f 3678 374b 5648 4b45 6352 4165 5a50  9O6x7KVHKEcRAeZP
-00040f90: 5a63 4c62 626f 6765 5643 4f4b 6e31 6e49  ZcLbbogeVCOKn1nI
-00040fa0: 6636 6d59 4471 5575 6c7a 6b64 5976 502f  f6mYDqUulzkdYvP/
-00040fb0: 6c2b 4954 756c 694d 496e 477a 4750 6e42  l+ITuliMInGzGPnB
-00040fc0: 4e6f 7256 7631 7a7a 4e6e 636a 326b 6e4d  NorVv1zzNncj2knM
-00040fd0: 7a61 3766 5779 5761 7259 7473 6a69 4161  za7fWyWarYtsjiAa
-00040fe0: 652f 6561 4e61 4b41 446a 4754 4a35 4271  e/eaNaKADjGTJ5Bq
-00040ff0: 4b4f 7454 3643 4653 4b51 6e49 5a72 322f  KOtT6CFSKQnIZr2/
-00041000: 436d 3478 6237 4a49 7748 2f58 7072 636e  Cm4xb7JIwH/Xprcn
-00041010: 6336 765a 3330 3545 674b 4b4d 6b32 5949  c6vZ305EgKKMk2YI
-00041020: 4534 577a 6d64 4876 5534 4635 3237 7033  E4WzmdHvU4F527p3
-00041030: 6975 7141 5830 476f 3749 4146 5175 706d  iuqAX0Go7IAFQupm
-00041040: 3137 6471 3065 6855 5432 2b4c 5671 6335  17dq0ehUT2+LVqc5
-00041050: 696d 7955 4941 6336 456a 4431 6e54 356a  imyUIAc6EjD1nT5j
-00041060: 3161 6276 3932 4269 4347 4344 4a5a 6b31  1abv92BiCGCDJZk1
-00041070: 5936 6d38 4262 384a 4850 5870 7230 7332  Y6m8Bb8JHPXpr0s2
-00041080: 3048 3871 6756 3748 7a71 674f 696a 6e4b  0H8qgV7HzqgOijnK
-00041090: 4c45 4151 3837 3967 486d 464f 6f36 5556  LEAQ879gHmFOo6UV
-000410a0: 6c55 4765 6644 3532 2f76 796f 6259 5167  lUGefD52/vyobYQg
-000410b0: 514a 5954 5279 3248 754d 5443 6371 7252  QJYTRy2HuMTCcqrR
-000410c0: 6e34 4c6f 5958 654a 6975 7731 3431 754b  n4LoYXeJiuw141uK
-000410d0: 5476 466b 5051 6164 6544 3071 3953 3064  TvFkPQadeD0q9S0d
-000410e0: 4155 6f32 6476 624f 4462 7773 7138 6e55  AUo2dvbODbwsq8nU
-000410f0: 5a5a 4c4a 6c72 5578 6b6d 344a 4632 356b  ZZLJlrUxkm4JF25k
-00041100: 6842 774a 3148 6539 5566 5473 4633 492b  hBwJ1He9UfTsF3I+
-00041110: 5a30 3531 526a 2f56 4b47 4849 6738 4d78  Z051Rj/VKGHIg8Mx
-00041120: 6658 6330 4531 7373 735a 494d 4664 6378  fXc0E1sssZIMFdcx
-00041130: 546a 687a 4a6c 6f45 306e 464c 2f31 6662  TjhzJloE0nFL/1fb
-00041140: 7a54 5135 4556 3361 4337 6756 515a 5171  zTQ5EV3aC7gVQZQq
-00041150: 6259 6332 6231 5744 564e 4938 704f 7241  bYc2b1WDVNI8pOrA
-00041160: 7474 6530 3954 4763 7761 304a 5077 6668  tte09TGcwa0JPwfh
-00041170: 5537 4153 6233 5748 487a 7069 656a 4862  U7ASb3WHHzpiejHb
-00041180: 5139 5945 3658 3164 6778 6852 374c 4275  Q9YE6X1dgxhR7LBu
-00041190: 3733 7276 3370 6b36 4746 4f76 446e 495a  73rv3pk6GFOvDnIZ
-000411a0: 4238 764e 7964 6171 7a2b 5077 5178 4144  B8vNydaqz+PwQxAD
-000411b0: 4f6d 4650 5941 3962 4b35 2f71 3232 7a63  OmFPYA9bK5/q22zc
-000411c0: 6b69 6948 5078 7043 4750 4e52 6d58 706e  kiiHPxpCGPNRmXpn
-000411d0: 7069 4344 4a6f 5774 6c59 5745 766a 6c4b  piCDJoWtlYWEvjlK
-000411e0: 6232 4a78 644e 764d 4a56 3269 4443 622f  b2JxdNvMJV2iDCb/
-000411f0: 2f76 5a50 7475 5451 6f62 3834 4936 4e77  /vZPtuTQob84I6Nw
-00041200: 6159 2b65 4639 7334 6741 3853 5974 5854  aY+eF9s4gA8SYtXT
-00041210: 7a32 3242 6278 4559 3131 4461 4639 5243  z22BbxEY11DaF9RC
-00041220: 6c50 5a37 544d 6b52 4c37 6143 6939 5561  lPZ7TMkRL7aCi9Ua
-00041230: 414e 336d 4154 5147 5073 6d6c 6e54 3778  AN3mATQGPsmlnT7x
-00041240: 4472 655a 4673 3757 6c59 3277 4751 5469  DreZFs7WlY2wGQTi
-00041250: 624d 634d 6179 3259 4858 694e 4b6a 4535  bMcMay2YHXiNKjE5
-00041260: 686c 7059 4750 6347 4c54 7530 614c 376f  hlpYGPcGLTu0aL7o
-00041270: 7434 764e 4c45 414f 596e 4c49 4864 7559  t4vNLEAOYnLIHduY
-00041280: 542b 2f62 6c7a 3639 614a 5647 6947 5856  T+/blz69aJVGiGXV
-00041290: 4b42 307a 734f 3774 5437 5943 6b32 6452  KB0zsO7tT7YCk2dR
-000412a0: 4a2f 4d53 5a4d 3533 4f65 7131 4e65 7438  J/MSZM53Oeq1Net8
-000412b0: 6350 7878 3943 4d77 7053 3467 646f 486e  cPxx9CMwpS4gdoHn
-000412c0: 7078 6e56 772f 4765 6355 7a62 3968 5042  pxnVw/GecUzb9hPB
-000412d0: 3577 6565 6649 4169 6371 4437 7777 4159  5weefIAicqD7wwAY
-000412e0: 7653 4853 574b 5030 4f32 566c 7574 4465  vSHSWKP0O2VlutDe
-000412f0: 524d 327a 3258 4f65 3276 3148 3345 3879  RM2z2XOe2v1H3E8y
-00041300: 2b64 624c 7552 5541 536c 454e 4d6a 4142  +dbLuRUASlENMjAB
-00041310: 6644 4949 5934 466c 3235 3530 3375 4d2b  fDIIY4Fl25503uM+
-00041320: 644a 6372 7a7a 7a48 5236 5848 3544 4342  dJcrzzzHR6XH5DCB
-00041330: 495a 7a74 785a 776e 5347 5849 6743 5443  IZztxZwnSGXIgCTC
-00041340: 3949 7a4a 454d 5875 322f 434c 4f4d 3961  9IzJEMXu2/CLOM9a
-00041350: 484c 785a 4246 4c6a 7557 4632 3337 3530  HLxZBFLjuWF23750
-00041360: 3534 794a 424f 6f73 4e50 666d 4b39 622f  54yJBOosNPfmK9b/
-00041370: 6d47 7434 5a73 6e63 6173 6463 6f69 3233  mGt4Zsncasdcoi23
-00041380: 3750 7369 6d51 554a 4845 4e51 6875 6770  7PsimQUJHENQhugp
-00041390: 3446 7066 684f 3970 6246 4667 4f6c 7464  4FpfhO9pbFFgOltd
-000413a0: 5635 4d42 3251 454c 4735 4369 4c4c 794a  V5MB2QELG5CiLLyJ
-000413b0: 4246 4c42 4459 4d66 4159 5556 5841 4430  BFLBDYMfAYUVXAD0
-000413c0: 5365 6f6b 7439 562b 5730 4776 6739 7276  Seokt9V+W0Gvg9rv
-000413d0: 4b38 2b46 2b78 3135 6a67 2f67 6944 7248  K8+F+x15jg/giDrH
-000413e0: 6141 782f 3578 6e2f 5776 4357 4858 5a73  aAx/5xn/WvCWHXZs
-000413f0: 3678 4971 4855 3932 4b4c 3634 4869 5149  6xIqHU92KL64HiQI
-00041400: 6655 4e77 6977 3637 4e39 4362 6f6a 6270  fUNwiw67N9Cbojbp
-00041410: 794f 4956 6549 7835 4f62 5252 6944 3149  yOIVeIx5ObRRiD1I
-00041420: 4b38 6962 5477 5a74 3038 526b 624f 3370  K8ibTwZt08RkbO3p
-00041430: 6e6f 5969 3639 5338 6b78 4769 486d 4341  noYi69S8kxGiHmCA
-00041440: 6441 5963 3258 6431 4a75 774d 784d 5459  dAYc2Xd1JuwMxMTY
-00041450: 4c38 5243 7249 3243 6e77 6d46 5856 3033  L8RCrI2CnwmFXV03
-00041460: 6974 7a62 6934 5653 5849 5059 676e 6347  itzbi4VSXIPYgncG
-00041470: 5747 485a 7453 5879 426e 3533 7161 7351  WGHZtSXyBn53qasQ
-00041480: 4532 5269 6f47 3479 5636 3358 5261 3852  E2RioG4yV63XRa8R
-00041490: 3377 7273 554d 5545 3242 666f 4253 4233  3wrsUMUE2BfoBSB3
-000414a0: 7266 6968 696f 4d65 4976 5559 5849 7962  rfihioMeIvUYXIyb
-000414b0: 4970 6f4d 4455 6270 2f32 4256 5077 7263  IpoMDUbp/2BVPwrc
-000414c0: 6f34 6b6e 3670 674e 6d4a 6a43 6336 6135  o4kn6pgNmJjCc6a5
-000414d0: 4a66 4477 4a33 7971 4950 5568 5859 5773  JfDwJ3yqIPUhXYWs
-000414e0: 4e75 365a 4d77 6174 7238 5842 714b 7945  Nu6ZMwatr8XBqKyE
-000414f0: 6d53 4664 6953 302f 6934 2b48 5556 6b63  mSFdiS0/i4+HUVkc
-00041500: 3878 4f70 4b59 4f66 7479 6763 6744 6452  8xOpKYOftygcgDdR
-00041510: 774b 695a 484e 7944 3249 4673 536e 5878  wKiZHNyD2IFsSnXx
-00041520: 4261 3732 4976 5561 3349 6962 496c 7361  Ba72IvUa3IibIlsa
-00041530: 6d44 7276 5570 6476 346e 6b61 3367 7248  mDrvUpdv4nka3grH
-00041540: 2f42 7964 7955 7967 4534 6f6b 5641 4141  /BydyUygE4okVAAA
-00041550: 4141 456c 4654 6b53 7551 6d43 430d 0a20  AAElFTkSuQmCC.. 
-00041560: 203c 2f44 7269 7665 496d 6167 653e 0d0a   </DriveImage>..
-00041570: 3c2f 496e 6765 6e69 6144 6963 7469 6f6e  </IngeniaDiction
-00041580: 6172 793e 0d0a                           ary>..
+0002e920: 6769 7374 6572 3e0d 0a09 093c 5265 6769  gister>....<Regi
+0002e930: 7374 6572 2061 6363 6573 733d 2272 7722  ster access="rw"
+0002e940: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
+0002e950: 564d 5f43 4647 2220 6164 6472 6573 733d  VM_CFG" address=
+0002e960: 2230 7830 3633 3122 2064 7479 7065 3d22  "0x0631" dtype="
+0002e970: 666c 6f61 7422 2069 643d 2244 5256 5f50  float" id="DRV_P
+0002e980: 524f 545f 5553 4552 5f55 4e44 4552 5f56  ROT_USER_UNDER_V
+0002e990: 4f4c 5422 2075 6e69 7473 3d22 5622 2073  OLT" units="V" s
+0002e9a0: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
+0002e9b0: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
+0002e9c0: 2249 6e64 6963 6174 6573 2074 6865 206d  "Indicates the m
+0002e9d0: 696e 696d 756d 2076 6f6c 7461 6765 2072  inimum voltage r
+0002e9e0: 6571 7569 7265 6420 6279 2074 6865 2075  equired by the u
+0002e9f0: 7365 7220 666f 7220 6120 7072 6f70 6572  ser for a proper
+0002ea00: 206f 7065 7261 7469 6f6e 2220 6361 745f   operation" cat_
+0002ea10: 6964 3d22 5052 4f54 4543 5449 4f4e 5322  id="PROTECTIONS"
+0002ea20: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+0002ea30: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+0002ea40: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+0002ea50: 656e 5f55 5322 3e55 7365 7220 756e 6465  en_US">User unde
+0002ea60: 7220 766f 6c74 6167 6520 6c65 7665 6c3c  r voltage level<
+0002ea70: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+0002ea80: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+0002ea90: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
+0002eaa0: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
+0002eab0: 7374 6572 2061 6363 6573 733d 2272 7722  ster access="rw"
+0002eac0: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
+0002ead0: 564d 5f43 4647 2220 6164 6472 6573 733d  VM_CFG" address=
+0002eae0: 2230 7830 3633 3222 2064 7479 7065 3d22  "0x0632" dtype="
+0002eaf0: 666c 6f61 7422 2069 643d 2244 5256 5f50  float" id="DRV_P
+0002eb00: 524f 545f 5553 4552 5f4f 5645 525f 5445  ROT_USER_OVER_TE
+0002eb10: 4d50 2220 756e 6974 733d 22c2 ba43 2220  MP" units="..C" 
+0002eb20: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+0002eb30: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+0002eb40: 3d22 496e 6469 6361 7465 7320 7468 6520  ="Indicates the 
+0002eb50: 6d61 7869 6d75 6d20 7465 6d70 6572 6174  maximum temperat
+0002eb60: 7572 6520 6f66 2074 6865 2064 7269 7665  ure of the drive
+0002eb70: 2061 6c6c 6f77 6564 2062 7920 7468 6520   allowed by the 
+0002eb80: 7573 6572 2220 6361 745f 6964 3d22 5052  user" cat_id="PR
+0002eb90: 4f54 4543 5449 4f4e 5322 3e0d 0a20 2020  OTECTIONS">..   
+0002eba0: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+0002ebb0: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
+0002ebc0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+0002ebd0: 3e55 7365 7220 6f76 6572 2074 656d 7065  >User over tempe
+0002ebe0: 7261 7475 7265 206c 6576 656c 3c2f 4c61  rature level</La
+0002ebf0: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
+0002ec00: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+0002ec10: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+0002ec20: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+0002ec30: 7220 6163 6365 7373 3d22 7277 2220 6164  r access="rw" ad
+0002ec40: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+0002ec50: 4346 4722 2061 6464 7265 7373 3d22 3078  CFG" address="0x
+0002ec60: 3036 3333 2220 6474 7970 653d 2266 6c6f  0633" dtype="flo
+0002ec70: 6174 2220 6964 3d22 4452 565f 5052 4f54  at" id="DRV_PROT
+0002ec80: 5f55 5345 525f 554e 4445 525f 5445 4d50  _USER_UNDER_TEMP
+0002ec90: 2220 756e 6974 733d 22c2 ba43 2220 7375  " units="..C" su
+0002eca0: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
+0002ecb0: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
+0002ecc0: 496e 6469 6361 7465 7320 7468 6520 6d69  Indicates the mi
+0002ecd0: 6e69 6d75 6d20 7465 6d70 6572 6174 7572  nimum temperatur
+0002ece0: 6520 6f66 2074 6865 2064 7269 7665 2061  e of the drive a
+0002ecf0: 6c6c 6f77 6564 2062 7920 7468 6520 7573  llowed by the us
+0002ed00: 6572 2220 6361 745f 6964 3d22 5052 4f54  er" cat_id="PROT
+0002ed10: 4543 5449 4f4e 5322 3e0d 0a20 2020 2020  ECTIONS">..     
+0002ed20: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+0002ed30: 2020 2020 2020 2020 2020 203c 4c61 6265             <Labe
+0002ed40: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e55  l lang="en_US">U
+0002ed50: 7365 7220 756e 6465 7220 7465 6d70 6572  ser under temper
+0002ed60: 6174 7572 6520 6c65 7665 6c3c 2f4c 6162  ature level</Lab
+0002ed70: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+0002ed80: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+0002ed90: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+0002eda0: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+0002edb0: 2061 6363 6573 733d 2272 7722 2061 6464   access="rw" add
+0002edc0: 7265 7373 5f74 7970 653d 224e 564d 5f4e  ress_type="NVM_N
+0002edd0: 4f4e 4522 2061 6464 7265 7373 3d22 3078  ONE" address="0x
+0002ede0: 3036 3431 2220 6474 7970 653d 2275 3136  0641" dtype="u16
+0002edf0: 2220 6964 3d22 434f 4d4d 535f 5359 4e43  " id="COMMS_SYNC
+0002ee00: 5f53 4947 4e41 4c5f 4346 4722 2075 6e69  _SIGNAL_CFG" uni
+0002ee10: 7473 3d22 2d22 2073 7562 6e6f 6465 3d22  ts="-" subnode="
+0002ee20: 3122 2063 7963 6c69 633d 2243 4f4e 4649  1" cyclic="CONFI
+0002ee30: 4722 2064 6573 633d 2249 6e64 6963 6174  G" desc="Indicat
+0002ee40: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
+0002ee50: 2073 796e 6368 726f 6e69 7a61 7469 6f6e   synchronization
+0002ee60: 2073 6967 6e61 6c73 2067 656e 6572 6174   signals generat
+0002ee70: 6564 2062 7920 7468 6520 4d43 4220 7072  ed by the MCB pr
+0002ee80: 6f74 6f63 6f6c 2220 6361 745f 6964 3d22  otocol" cat_id="
+0002ee90: 434f 4d4d 554e 4943 4154 494f 4e53 223e  COMMUNICATIONS">
+0002eea0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+0002eeb0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+0002eec0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+0002eed0: 6e5f 5553 223e 5379 6e63 2e20 7369 676e  n_US">Sync. sign
+0002eee0: 616c 2063 6f6e 6669 6775 7261 7469 6f6e  al configuration
+0002eef0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+0002ef00: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+0002ef10: 2020 2020 2020 2020 203c 456e 756d 6572           <Enumer
+0002ef20: 6174 696f 6e73 3e0d 0a20 2020 2020 2020  ations>..       
+0002ef30: 2020 2020 203c 456e 756d 2076 616c 7565       <Enum value
+0002ef40: 3d22 3022 3e44 6973 6162 6c65 643c 2f45  ="0">Disabled</E
+0002ef50: 6e75 6d3e 0d0a 2020 2020 2020 2020 2020  num>..          
+0002ef60: 2020 3c45 6e75 6d20 7661 6c75 653d 2231    <Enum value="1
+0002ef70: 223e 4f6e 6c79 2053 796e 6320 303c 2f45  ">Only Sync 0</E
+0002ef80: 6e75 6d3e 0d0a 2020 2020 2020 2020 2020  num>..          
+0002ef90: 3c2f 456e 756d 6572 6174 696f 6e73 3e0d  </Enumerations>.
+0002efa0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+0002efb0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+0002efc0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+0002efd0: 7277 2220 6164 6472 6573 735f 7479 7065  rw" address_type
+0002efe0: 3d22 4e56 4d5f 4346 4722 2061 6464 7265  ="NVM_CFG" addre
+0002eff0: 7373 3d22 3078 3036 3433 2220 6474 7970  ss="0x0643" dtyp
+0002f000: 653d 2275 3332 2220 6964 3d22 434f 4d4d  e="u32" id="COMM
+0002f010: 535f 5359 4e43 5f53 4947 4e41 4c5f 4652  S_SYNC_SIGNAL_FR
+0002f020: 4551 2220 756e 6974 733d 2248 7a22 2073  EQ" units="Hz" s
+0002f030: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
+0002f040: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
+0002f050: 2246 7265 7175 656e 6379 2061 7420 7768  "Frequency at wh
+0002f060: 6963 6820 7468 6520 7379 6e63 6872 6f6e  ich the synchron
+0002f070: 697a 6174 696f 6e20 7369 676e 616c 2069  ization signal i
+0002f080: 7320 6265 696e 6720 6765 6e65 7261 7465  s being generate
+0002f090: 642e 2049 7420 7368 6f75 6c64 2062 6520  d. It should be 
+0002f0a0: 616e 2065 7861 6374 206d 756c 7469 706c  an exact multipl
+0002f0b0: 6520 6f66 2074 6865 2050 574d 2066 7265  e of the PWM fre
+0002f0c0: 7175 656e 6379 2073 656c 6563 7465 642e  quency selected.
+0002f0d0: 2220 6361 745f 6964 3d22 4f54 4845 5253  " cat_id="OTHERS
+0002f0e0: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+0002f0f0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+0002f100: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+0002f110: 2265 6e5f 5553 223e 5379 6e63 2e20 7369  "en_US">Sync. si
+0002f120: 676e 616c 2066 7265 7175 656e 6379 3c2f  gnal frequency</
+0002f130: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+0002f140: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+0002f150: 2020 2020 2020 203c 5261 6e67 6520 6d69         <Range mi
+0002f160: 6e3d 2231 3022 206d 6178 3d22 3230 3030  n="10" max="2000
+0002f170: 3030 222f 3e0d 0a20 2020 2020 2020 203c  00"/>..        <
+0002f180: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+0002f190: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+0002f1a0: 6365 7373 3d22 7277 2220 6164 6472 6573  cess="rw" addres
+0002f1b0: 735f 7479 7065 3d22 4e56 4d5f 4346 4722  s_type="NVM_CFG"
+0002f1c0: 2061 6464 7265 7373 3d22 3078 3036 3434   address="0x0644
+0002f1d0: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
+0002f1e0: 3d22 434f 4d4d 535f 5359 4e43 5f50 4c4c  ="COMMS_SYNC_PLL
+0002f1f0: 5f43 5554 4f46 4622 2075 6e69 7473 3d22  _CUTOFF" units="
+0002f200: 487a 2220 7375 626e 6f64 653d 2231 2220  Hz" subnode="1" 
+0002f210: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+0002f220: 6465 7363 3d22 4375 746f 6666 2066 7265  desc="Cutoff fre
+0002f230: 7175 656e 6379 206f 6620 7468 6520 7379  quency of the sy
+0002f240: 6e63 6872 6f6e 697a 6174 696f 6e20 7369  nchronization si
+0002f250: 676e 616c 2050 4c4c 2066 696c 7465 7222  gnal PLL filter"
+0002f260: 2063 6174 5f69 643d 224f 5448 4552 5322   cat_id="OTHERS"
+0002f270: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+0002f280: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+0002f290: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+0002f2a0: 656e 5f55 5322 3e53 796e 632e 2073 6967  en_US">Sync. sig
+0002f2b0: 6e61 6c20 504c 4c20 6669 6c74 6572 2063  nal PLL filter c
+0002f2c0: 7574 6f66 6620 6672 6571 7565 6e63 793c  utoff frequency<
+0002f2d0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+0002f2e0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+0002f2f0: 2020 2020 2020 2020 3c52 616e 6765 206d          <Range m
+0002f300: 696e 3d22 3130 2220 6d61 783d 2232 3030  in="10" max="200
+0002f310: 3030 3022 2f3e 0d0a 2020 2020 2020 2020  000"/>..        
+0002f320: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
+0002f330: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
+0002f340: 6363 6573 733d 2272 7722 2061 6464 7265  ccess="rw" addre
+0002f350: 7373 5f74 7970 653d 224e 564d 5f43 4647  ss_type="NVM_CFG
+0002f360: 2220 6164 6472 6573 733d 2230 7830 3634  " address="0x064
+0002f370: 3522 2064 7479 7065 3d22 666c 6f61 7422  5" dtype="float"
+0002f380: 2069 643d 2243 4f4d 4d53 5f53 594e 435f   id="COMMS_SYNC_
+0002f390: 504c 4c5f 5048 4153 4522 2075 6e69 7473  PLL_PHASE" units
+0002f3a0: 3d22 2d22 2073 7562 6e6f 6465 3d22 3122  ="-" subnode="1"
+0002f3b0: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+0002f3c0: 2064 6573 633d 2243 6f6e 6669 6775 7265   desc="Configure
+0002f3d0: 7320 7068 6173 6520 6469 6666 6572 656e  s phase differen
+0002f3e0: 6365 2062 6574 7765 656e 2074 6865 2073  ce between the s
+0002f3f0: 796e 6368 726f 6e69 7a61 7469 6f6e 2073  ynchronization s
+0002f400: 6967 6e61 6c20 616e 6420 7468 6520 6765  ignal and the ge
+0002f410: 6e65 7261 7465 6420 5057 4d2e 2220 6361  nerated PWM." ca
+0002f420: 745f 6964 3d22 4f54 4845 5253 223e 0d0a  t_id="OTHERS">..
+0002f430: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+0002f440: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+0002f450: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+0002f460: 5553 223e 5379 6e63 2e20 7369 676e 616c  US">Sync. signal
+0002f470: 2050 4c4c 2070 6861 7365 3c2f 4c61 6265   PLL phase</Labe
+0002f480: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+0002f490: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+0002f4a0: 2020 203c 5261 6e67 6520 6d69 6e3d 2230     <Range min="0
+0002f4b0: 2e30 2220 6d61 783d 2231 2e30 222f 3e0d  .0" max="1.0"/>.
+0002f4c0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+0002f4d0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+0002f4e0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+0002f4f0: 7277 2220 6164 6472 6573 735f 7479 7065  rw" address_type
+0002f500: 3d22 4e56 4d5f 4346 4722 2061 6464 7265  ="NVM_CFG" addre
+0002f510: 7373 3d22 3078 3036 3436 2220 6474 7970  ss="0x0646" dtyp
+0002f520: 653d 2266 6c6f 6174 2220 6964 3d22 434f  e="float" id="CO
+0002f530: 4d4d 535f 5359 4e43 5f50 4c4c 5f4b 5022  MMS_SYNC_PLL_KP"
+0002f540: 2075 6e69 7473 3d22 2d22 2073 7562 6e6f   units="-" subno
+0002f550: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
+0002f560: 4f4e 4649 4722 2064 6573 633d 2243 6f6e  ONFIG" desc="Con
+0002f570: 6669 6775 7265 7320 7072 6f70 6f72 7469  figures proporti
+0002f580: 6f6e 616c 2063 6f6e 7374 616e 7420 666f  onal constant fo
+0002f590: 7220 7068 6173 6520 636f 7272 6563 7469  r phase correcti
+0002f5a0: 6f6e 2069 6e20 506c 6c22 2063 6174 5f69  on in Pll" cat_i
+0002f5b0: 643d 224f 5448 4552 5322 3e0d 0a20 2020  d="OTHERS">..   
+0002f5c0: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+0002f5d0: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
+0002f5e0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+0002f5f0: 3e53 796e 632e 2073 6967 6e61 6c20 504c  >Sync. signal PL
+0002f600: 4c20 4b70 3c2f 4c61 6265 6c3e 0d0a 2020  L Kp</Label>..  
+0002f610: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+0002f620: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
+0002f630: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
+0002f640: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
+0002f650: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
+0002f660: 653d 224e 564d 5f4e 4f4e 4522 2061 6464  e="NVM_NONE" add
+0002f670: 7265 7373 3d22 3078 3036 3444 2220 6474  ress="0x064D" dt
+0002f680: 7970 653d 2275 3136 2220 6964 3d22 4452  ype="u16" id="DR
+0002f690: 565f 4449 4147 5f45 5252 4f52 5f54 4f54  V_DIAG_ERROR_TOT
+0002f6a0: 414c 2220 756e 6974 733d 222d 2220 7375  AL" units="-" su
+0002f6b0: 626e 6f64 653d 2231 2220 6379 636c 6963  bnode="1" cyclic
+0002f6c0: 3d22 434f 4e46 4947 2220 6465 7363 3d22  ="CONFIG" desc="
+0002f6d0: 546f 7461 6c20 6e75 6d62 6572 206f 6620  Total number of 
+0002f6e0: 6572 726f 7273 2073 696e 6365 2070 6f77  errors since pow
+0002f6f0: 6572 2075 7022 2063 6174 5f69 643d 2252  er up" cat_id="R
+0002f700: 4550 4f52 5449 4e47 223e 0d0a 2020 2020  EPORTING">..    
+0002f710: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+0002f720: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+0002f730: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+0002f740: 4572 726f 7220 746f 7461 6c20 6e75 6d62  Error total numb
+0002f750: 6572 3c2f 4c61 6265 6c3e 0d0a 2020 2020  er</Label>..    
+0002f760: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+0002f770: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+0002f780: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+0002f790: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+0002f7a0: 7277 2220 6164 6472 6573 735f 7479 7065  rw" address_type
+0002f7b0: 3d22 4e56 4d5f 4e4f 4e45 2220 6164 6472  ="NVM_NONE" addr
+0002f7c0: 6573 733d 2230 7830 3634 4522 2064 7479  ess="0x064E" dty
+0002f7d0: 7065 3d22 7531 3622 2069 643d 2244 5256  pe="u16" id="DRV
+0002f7e0: 5f44 4941 475f 4552 524f 525f 4c49 5354  _DIAG_ERROR_LIST
+0002f7f0: 5f49 4458 2220 756e 6974 733d 222d 2220  _IDX" units="-" 
+0002f800: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+0002f810: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+0002f820: 3d22 496e 6465 7820 746f 2061 6363 6573  ="Index to acces
+0002f830: 7320 746f 2074 6865 206c 6173 7420 6572  s to the last er
+0002f840: 726f 7273 2220 6361 745f 6964 3d22 5245  rors" cat_id="RE
+0002f850: 504f 5254 494e 4722 3e0d 0a20 2020 2020  PORTING">..     
+0002f860: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+0002f870: 2020 2020 2020 2020 2020 203c 4c61 6265             <Labe
+0002f880: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e45  l lang="en_US">E
+0002f890: 7272 6f72 206c 6973 7420 696e 6465 7820  rror list index 
+0002f8a0: 7265 7175 6573 743c 2f4c 6162 656c 3e0d  request</Label>.
+0002f8b0: 0a20 2020 2020 2020 2020 203c 2f4c 6162  .          </Lab
+0002f8c0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+0002f8d0: 3c52 616e 6765 206d 696e 3d22 3022 206d  <Range min="0" m
+0002f8e0: 6178 3d22 3332 222f 3e0d 0a20 2020 2020  ax="32"/>..     
+0002f8f0: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+0002f900: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+0002f910: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+0002f920: 7265 7373 5f74 7970 653d 224e 564d 5f4e  ress_type="NVM_N
+0002f930: 4f4e 4522 2061 6464 7265 7373 3d22 3078  ONE" address="0x
+0002f940: 3036 3446 2220 6474 7970 653d 2273 3332  064F" dtype="s32
+0002f950: 2220 6964 3d22 4452 565f 4449 4147 5f45  " id="DRV_DIAG_E
+0002f960: 5252 4f52 5f4c 4953 545f 434f 4445 2220  RROR_LIST_CODE" 
+0002f970: 756e 6974 733d 222d 2220 7375 626e 6f64  units="-" subnod
+0002f980: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+0002f990: 4e46 4947 2220 6465 7363 3d22 436f 6e74  NFIG" desc="Cont
+0002f9a0: 6169 6e73 2074 6865 2065 7272 6f72 2063  ains the error c
+0002f9b0: 6f64 6520 6f66 2074 6865 2069 6e64 6963  ode of the indic
+0002f9c0: 6174 6564 2062 7920 7468 6520 7265 7175  ated by the requ
+0002f9d0: 6573 7465 6420 6c6f 6361 7469 6f6e 2072  ested location r
+0002f9e0: 6567 6973 7465 7222 2063 6174 5f69 643d  egister" cat_id=
+0002f9f0: 2252 4550 4f52 5449 4e47 223e 0d0a 2020  "REPORTING">..  
+0002fa00: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+0002fa10: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
+0002fa20: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+0002fa30: 223e 4572 726f 7220 6c69 7374 2072 6571  ">Error list req
+0002fa40: 7565 7374 6564 2063 6f64 653c 2f4c 6162  uested code</Lab
+0002fa50: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+0002fa60: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+0002fa70: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+0002fa80: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+0002fa90: 2061 6363 6573 733d 2272 7722 2061 6464   access="rw" add
+0002faa0: 7265 7373 5f74 7970 653d 224e 564d 5f4e  ress_type="NVM_N
+0002fab0: 4f4e 4522 2061 6464 7265 7373 3d22 3078  ONE" address="0x
+0002fac0: 3036 4442 2220 6474 7970 653d 2275 3332  06DB" dtype="u32
+0002fad0: 2220 6964 3d22 4452 565f 5354 4f52 455f  " id="DRV_STORE_
+0002fae0: 4d4f 434f 5f41 4c4c 2220 756e 6974 733d  MOCO_ALL" units=
+0002faf0: 222d 2220 7375 626e 6f64 653d 2231 2220  "-" subnode="1" 
+0002fb00: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+0002fb10: 6465 7363 3d22 2220 6361 745f 6964 3d22  desc="" cat_id="
+0002fb20: 4944 454e 5449 4649 4341 5449 4f4e 223e  IDENTIFICATION">
+0002fb30: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+0002fb40: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+0002fb50: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+0002fb60: 6e5f 5553 223e 5374 6f72 6520 616c 6c3c  n_US">Store all<
+0002fb70: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+0002fb80: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+0002fb90: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
+0002fba0: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
+0002fbb0: 7374 6572 2061 6363 6573 733d 2272 7722  ster access="rw"
+0002fbc0: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
+0002fbd0: 564d 5f4e 4f4e 4522 2061 6464 7265 7373  VM_NONE" address
+0002fbe0: 3d22 3078 3036 4443 2220 6474 7970 653d  ="0x06DC" dtype=
+0002fbf0: 2275 3332 2220 6964 3d22 4452 565f 5245  "u32" id="DRV_RE
+0002fc00: 5354 4f52 455f 4d4f 434f 5f41 4c4c 2220  STORE_MOCO_ALL" 
+0002fc10: 756e 6974 733d 222d 2220 7375 626e 6f64  units="-" subnod
+0002fc20: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+0002fc30: 4e46 4947 2220 6465 7363 3d22 5573 696e  NFIG" desc="Usin
+0002fc40: 6720 7468 6520 7072 6f70 6572 2070 6173  g the proper pas
+0002fc50: 7377 6f72 6420 616c 6c6f 7773 2074 6f20  sword allows to 
+0002fc60: 7265 7374 6f72 6520 7468 6520 6465 6661  restore the defa
+0002fc70: 756c 7420 7061 7261 6d65 7465 7273 206f  ult parameters o
+0002fc80: 6620 7468 6520 6472 6976 6520 6166 7465  f the drive afte
+0002fc90: 7220 7468 6520 6e65 7874 2070 6f77 6572  r the next power
+0002fca0: 206f 6e22 2063 6174 5f69 643d 2249 4445   on" cat_id="IDE
+0002fcb0: 4e54 4946 4943 4154 494f 4e22 3e0d 0a20  NTIFICATION">.. 
+0002fcc0: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
+0002fcd0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+0002fce0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+0002fcf0: 5322 3e52 6573 746f 7265 2061 6c6c 3c2f  S">Restore all</
+0002fd00: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+0002fd10: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+0002fd20: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
+0002fd30: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
+0002fd40: 7465 7220 6163 6365 7373 3d22 7722 2061  ter access="w" a
+0002fd50: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
+0002fd60: 5f4e 4f4e 4522 2061 6464 7265 7373 3d22  _NONE" address="
+0002fd70: 3078 3036 4446 2220 6474 7970 653d 2275  0x06DF" dtype="u
+0002fd80: 3332 2220 6964 3d22 4452 565f 424f 4f54  32" id="DRV_BOOT
+0002fd90: 5f52 4553 4554 2220 756e 6974 733d 222d  _RESET" units="-
+0002fda0: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
+0002fdb0: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
+0002fdc0: 7363 3d22 5769 7468 2074 6865 2070 726f  sc="With the pro
+0002fdd0: 7065 7220 7061 7373 776f 7264 2072 6573  per password res
+0002fde0: 6574 7320 7468 6520 6472 6976 652e 2220  ets the drive." 
+0002fdf0: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+0002fe00: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+0002fe10: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+0002fe20: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+0002fe30: 2265 6e5f 5553 223e 5379 7374 656d 2072  "en_US">System r
+0002fe40: 6573 6574 3c2f 4c61 6265 6c3e 0d0a 2020  eset</Label>..  
+0002fe50: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+0002fe60: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
+0002fe70: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
+0002fe80: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
+0002fe90: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
+0002fea0: 653d 224e 564d 5f4e 4f4e 4522 2061 6464  e="NVM_NONE" add
+0002feb0: 7265 7373 3d22 3078 3036 4530 2220 6474  ress="0x06E0" dt
+0002fec0: 7970 653d 2275 3332 2220 6964 3d22 4452  ype="u32" id="DR
+0002fed0: 565f 4944 5f56 454e 444f 525f 4944 2220  V_ID_VENDOR_ID" 
+0002fee0: 756e 6974 733d 222d 2220 7375 626e 6f64  units="-" subnod
+0002fef0: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+0002ff00: 4e46 4947 2220 6465 7363 3d22 4964 656e  NFIG" desc="Iden
+0002ff10: 7469 6669 6573 2074 6865 2076 656e 646f  tifies the vendo
+0002ff20: 7220 6f66 2074 6865 2070 726f 6475 6374  r of the product
+0002ff30: 2220 6361 745f 6964 3d22 4944 454e 5449  " cat_id="IDENTI
+0002ff40: 4649 4341 5449 4f4e 223e 0d0a 2020 2020  FICATION">..    
+0002ff50: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+0002ff60: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+0002ff70: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+0002ff80: 5665 6e64 6f72 2049 443c 2f4c 6162 656c  Vendor ID</Label
+0002ff90: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
+0002ffa0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+0002ffb0: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
+0002ffc0: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
+0002ffd0: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
+0002ffe0: 735f 7479 7065 3d22 4e56 4d5f 4e4f 4e45  s_type="NVM_NONE
+0002fff0: 2220 6164 6472 6573 733d 2230 7830 3645  " address="0x06E
+00030000: 3122 2064 7479 7065 3d22 7533 3222 2069  1" dtype="u32" i
+00030010: 643d 2244 5256 5f49 445f 5052 4f44 5543  d="DRV_ID_PRODUC
+00030020: 545f 434f 4445 2220 756e 6974 733d 222d  T_CODE" units="-
+00030030: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
+00030040: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
+00030050: 7363 3d22 436f 6e74 6169 6e73 2074 6865  sc="Contains the
+00030060: 2070 726f 6475 6374 2063 6f64 6520 6f66   product code of
+00030070: 2074 6865 2064 7269 7665 2220 6361 745f   the drive" cat_
+00030080: 6964 3d22 4944 454e 5449 4649 4341 5449  id="IDENTIFICATI
+00030090: 4f4e 223e 0d0a 2020 2020 2020 2020 2020  ON">..          
+000300a0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+000300b0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+000300c0: 673d 2265 6e5f 5553 223e 5072 6f64 7563  g="en_US">Produc
+000300d0: 7420 636f 6465 3c2f 4c61 6265 6c3e 0d0a  t code</Label>..
+000300e0: 2020 2020 2020 2020 2020 3c2f 4c61 6265            </Labe
+000300f0: 6c73 3e0d 0a20 2020 2020 2020 203c 2f52  ls>..        </R
+00030100: 6567 6973 7465 723e 0d0a 2020 2020 2020  egister>..      
+00030110: 2020 3c52 6567 6973 7465 7220 6163 6365    <Register acce
+00030120: 7373 3d22 7222 2061 6464 7265 7373 5f74  ss="r" address_t
+00030130: 7970 653d 224e 564d 5f4e 4f4e 4522 2061  ype="NVM_NONE" a
+00030140: 6464 7265 7373 3d22 3078 3036 4532 2220  ddress="0x06E2" 
+00030150: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
+00030160: 4452 565f 4944 5f52 4556 4953 494f 4e5f  DRV_ID_REVISION_
+00030170: 4e55 4d42 4552 2220 756e 6974 733d 222d  NUMBER" units="-
+00030180: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
+00030190: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
+000301a0: 7363 3d22 496e 6469 6361 7465 7320 7468  sc="Indicates th
+000301b0: 6520 7265 7669 7369 6f6e 206e 756d 6265  e revision numbe
+000301c0: 7220 6f66 2074 6865 2066 6972 6d77 6172  r of the firmwar
+000301d0: 6520 7665 7273 696f 6e20 6f6e 2074 6865  e version on the
+000301e0: 2064 7269 7665 2220 6361 745f 6964 3d22   drive" cat_id="
+000301f0: 4944 454e 5449 4649 4341 5449 4f4e 223e  IDENTIFICATION">
+00030200: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00030210: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00030220: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00030230: 6e5f 5553 223e 5265 7669 7369 6f6e 206e  n_US">Revision n
+00030240: 756d 6265 723c 2f4c 6162 656c 3e0d 0a20  umber</Label>.. 
+00030250: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00030260: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00030270: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00030280: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00030290: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+000302a0: 7065 3d22 4e56 4d5f 4e4f 4e45 2220 6164  pe="NVM_NONE" ad
+000302b0: 6472 6573 733d 2230 7830 3645 3422 2064  dress="0x06E4" d
+000302c0: 7479 7065 3d22 7374 7222 2069 643d 2244  type="str" id="D
+000302d0: 5256 5f49 445f 534f 4654 5741 5245 5f56  RV_ID_SOFTWARE_V
+000302e0: 4552 5349 4f4e 2220 756e 6974 733d 222d  ERSION" units="-
+000302f0: 2220 7375 626e 6f64 653d 2231 2220 6379  " subnode="1" cy
+00030300: 636c 6963 3d22 434f 4e46 4947 2220 6465  clic="CONFIG" de
+00030310: 7363 3d22 5075 626c 6963 2073 6f66 7477  sc="Public softw
+00030320: 6172 6520 7265 6c65 6173 6520 7665 7273  are release vers
+00030330: 696f 6e22 2063 6174 5f69 643d 2249 4445  ion" cat_id="IDE
+00030340: 4e54 4946 4943 4154 494f 4e22 3e0d 0a20  NTIFICATION">.. 
+00030350: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
+00030360: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00030370: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+00030380: 5322 3e53 6f66 7477 6172 6520 7665 7273  S">Software vers
+00030390: 696f 6e3c 2f4c 6162 656c 3e0d 0a20 2020  ion</Label>..   
+000303a0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+000303b0: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+000303c0: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+000303d0: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+000303e0: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+000303f0: 3d22 4e56 4d5f 4c4f 434b 2220 6164 6472  ="NVM_LOCK" addr
+00030400: 6573 733d 2230 7830 3645 3622 2064 7479  ess="0x06E6" dty
+00030410: 7065 3d22 7533 3222 2069 643d 2244 5256  pe="u32" id="DRV
+00030420: 5f49 445f 5345 5249 414c 5f4e 554d 4245  _ID_SERIAL_NUMBE
+00030430: 5222 2075 6e69 7473 3d22 2d22 2073 7562  R" units="-" sub
+00030440: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
+00030450: 2243 4f4e 4649 4722 2064 6573 633d 2255  "CONFIG" desc="U
+00030460: 6e69 7175 6520 7365 7269 616c 206e 756d  nique serial num
+00030470: 6265 7220 6964 206f 6620 7468 6520 6465  ber id of the de
+00030480: 7669 6365 2220 6361 745f 6964 3d22 4944  vice" cat_id="ID
+00030490: 454e 5449 4649 4341 5449 4f4e 223e 0d0a  ENTIFICATION">..
+000304a0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+000304b0: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+000304c0: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+000304d0: 5553 223e 5365 7269 616c 206e 756d 6265  US">Serial numbe
+000304e0: 723c 2f4c 6162 656c 3e0d 0a20 2020 2020  r</Label>..     
+000304f0: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00030500: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
+00030510: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
+00030520: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
+00030530: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
+00030540: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
+00030550: 2230 7830 3730 3022 2064 7479 7065 3d22  "0x0700" dtype="
+00030560: 7533 3222 2069 643d 2244 5256 5f50 535f  u32" id="DRV_PS_
+00030570: 4652 4551 5f31 2220 756e 6974 733d 2248  FREQ_1" units="H
+00030580: 7a22 2073 7562 6e6f 6465 3d22 3122 2063  z" subnode="1" c
+00030590: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+000305a0: 6573 633d 2243 6f6e 7461 696e 7320 7468  esc="Contains th
+000305b0: 6520 7365 6c65 6374 6162 6c65 2063 6f6d  e selectable com
+000305c0: 6d75 7461 7469 6f6e 2066 7265 7175 656e  mutation frequen
+000305d0: 6379 2031 2028 416c 736f 206d 696e 696d  cy 1 (Also minim
+000305e0: 756d 2050 574d 2066 7265 7175 656e 6379  um PWM frequency
+000305f0: 2922 2063 6174 5f69 643d 2249 4e54 4552  )" cat_id="INTER
+00030600: 4e41 4c22 3e0d 0a20 2020 2020 2020 2020  NAL">..         
+00030610: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00030620: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00030630: 6e67 3d22 656e 5f55 5322 3e50 6f77 6572  ng="en_US">Power
+00030640: 2073 7461 6765 2066 7265 7175 656e 6379   stage frequency
+00030650: 2031 3c2f 4c61 6265 6c3e 0d0a 2020 2020   1</Label>..    
+00030660: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00030670: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+00030680: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+00030690: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+000306a0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
+000306b0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
+000306c0: 3d22 3078 3037 3031 2220 6474 7970 653d  ="0x0701" dtype=
+000306d0: 2275 3332 2220 6964 3d22 4452 565f 5053  "u32" id="DRV_PS
+000306e0: 5f46 5245 515f 3222 2075 6e69 7473 3d22  _FREQ_2" units="
+000306f0: 487a 2220 7375 626e 6f64 653d 2231 2220  Hz" subnode="1" 
+00030700: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+00030710: 6465 7363 3d22 436f 6e74 6169 6e73 2074  desc="Contains t
+00030720: 6865 2073 656c 6563 7461 626c 6520 636f  he selectable co
+00030730: 6d6d 7574 6174 696f 6e20 6672 6571 7565  mmutation freque
+00030740: 6e63 7920 3222 2063 6174 5f69 643d 2249  ncy 2" cat_id="I
+00030750: 4e54 4552 4e41 4c22 3e0d 0a20 2020 2020  NTERNAL">..     
+00030760: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00030770: 2020 2020 2020 2020 2020 203c 4c61 6265             <Labe
+00030780: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e50  l lang="en_US">P
+00030790: 6f77 6572 2073 7461 6765 2066 7265 7175  ower stage frequ
+000307a0: 656e 6379 2032 3c2f 4c61 6265 6c3e 0d0a  ency 2</Label>..
+000307b0: 2020 2020 2020 2020 2020 3c2f 4c61 6265            </Labe
+000307c0: 6c73 3e0d 0a20 2020 2020 2020 203c 2f52  ls>..        </R
+000307d0: 6567 6973 7465 723e 0d0a 2020 2020 2020  egister>..      
+000307e0: 2020 3c52 6567 6973 7465 7220 6163 6365    <Register acce
+000307f0: 7373 3d22 7222 2061 6464 7265 7373 5f74  ss="r" address_t
+00030800: 7970 653d 224e 564d 5f48 5722 2061 6464  ype="NVM_HW" add
+00030810: 7265 7373 3d22 3078 3037 3032 2220 6474  ress="0x0702" dt
+00030820: 7970 653d 2275 3332 2220 6964 3d22 4452  ype="u32" id="DR
+00030830: 565f 5053 5f46 5245 515f 3322 2075 6e69  V_PS_FREQ_3" uni
+00030840: 7473 3d22 487a 2220 7375 626e 6f64 653d  ts="Hz" subnode=
+00030850: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+00030860: 4947 2220 6465 7363 3d22 436f 6e74 6169  IG" desc="Contai
+00030870: 6e73 2074 6865 2073 656c 6563 7461 626c  ns the selectabl
+00030880: 6520 636f 6d6d 7574 6174 696f 6e20 6672  e commutation fr
+00030890: 6571 7565 6e63 7920 3322 2063 6174 5f69  equency 3" cat_i
+000308a0: 643d 2249 4e54 4552 4e41 4c22 3e0d 0a20  d="INTERNAL">.. 
+000308b0: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
+000308c0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+000308d0: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+000308e0: 5322 3e50 6f77 6572 2073 7461 6765 2066  S">Power stage f
+000308f0: 7265 7175 656e 6379 2033 3c2f 4c61 6265  requency 3</Labe
+00030900: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00030910: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00030920: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+00030930: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
+00030940: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
+00030950: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
+00030960: 2061 6464 7265 7373 3d22 3078 3037 3033   address="0x0703
+00030970: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
+00030980: 3d22 4452 565f 5053 5f46 5245 515f 3422  ="DRV_PS_FREQ_4"
+00030990: 2075 6e69 7473 3d22 487a 2220 7375 626e   units="Hz" subn
+000309a0: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
+000309b0: 434f 4e46 4947 2220 6465 7363 3d22 436f  CONFIG" desc="Co
+000309c0: 6e74 6169 6e73 2074 6865 2073 656c 6563  ntains the selec
+000309d0: 7461 626c 6520 636f 6d6d 7574 6174 696f  table commutatio
+000309e0: 6e20 6672 6571 7565 6e63 7920 3420 2841  n frequency 4 (A
+000309f0: 6c73 6f20 6d61 7869 6d75 6d20 5057 4d20  lso maximum PWM 
+00030a00: 6672 6571 7565 6e63 7929 2220 6361 745f  frequency)" cat_
+00030a10: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+00030a20: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00030a30: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00030a40: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00030a50: 5553 223e 506f 7765 7220 7374 6167 6520  US">Power stage 
+00030a60: 6672 6571 7565 6e63 7920 343c 2f4c 6162  frequency 4</Lab
+00030a70: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+00030a80: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00030a90: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+00030aa0: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+00030ab0: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
+00030ac0: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
+00030ad0: 2220 6164 6472 6573 733d 2230 7830 3730  " address="0x070
+00030ae0: 3422 2064 7479 7065 3d22 7533 3222 2069  4" dtype="u32" i
+00030af0: 643d 2244 5256 5f50 535f 4445 4144 5f54  d="DRV_PS_DEAD_T
+00030b00: 494d 4522 2075 6e69 7473 3d22 6e73 2220  IME" units="ns" 
+00030b10: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+00030b20: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+00030b30: 3d22 4465 6164 2d74 696d 6520 6170 706c  ="Dead-time appl
+00030b40: 6965 6420 746f 2050 574d 2067 656e 6572  ied to PWM gener
+00030b50: 6174 696f 6e20 746f 2061 766f 6964 2073  ation to avoid s
+00030b60: 686f 6f74 2d74 6872 6f75 6768 2069 6e20  hoot-through in 
+00030b70: 7468 6520 706f 7765 7220 7374 6167 6522  the power stage"
+00030b80: 2063 6174 5f69 643d 2249 4e54 4552 4e41   cat_id="INTERNA
+00030b90: 4c22 3e0d 0a20 2020 2020 2020 2020 203c  L">..          <
+00030ba0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00030bb0: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00030bc0: 3d22 656e 5f55 5322 3e50 6f77 6572 2073  ="en_US">Power s
+00030bd0: 7461 6765 2064 6561 642d 7469 6d65 2028  tage dead-time (
+00030be0: 6e73 293c 2f4c 6162 656c 3e0d 0a20 2020  ns)</Label>..   
+00030bf0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00030c00: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+00030c10: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+00030c20: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+00030c30: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+00030c40: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
+00030c50: 733d 2230 7830 3730 3622 2064 7479 7065  s="0x0706" dtype
+00030c60: 3d22 7533 3222 2069 643d 2244 5256 5f50  ="u32" id="DRV_P
+00030c70: 535f 4d49 4e5f 4c4f 575f 5349 4445 5f4f  S_MIN_LOW_SIDE_O
+00030c80: 4e5f 5449 4d45 2220 756e 6974 733d 226e  N_TIME" units="n
+00030c90: 7322 2073 7562 6e6f 6465 3d22 3122 2063  s" subnode="1" c
+00030ca0: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+00030cb0: 6573 633d 224d 696e 696d 756d 2074 696d  esc="Minimum tim
+00030cc0: 6520 7468 6520 706f 7765 7220 7374 6167  e the power stag
+00030cd0: 6520 6c6f 7720 7369 6465 2073 686f 756c  e low side shoul
+00030ce0: 6420 6265 2065 6e61 626c 6564 2066 6f72  d be enabled for
+00030cf0: 2061 2070 726f 7065 7220 6375 7272 656e   a proper curren
+00030d00: 7420 6d65 6173 7572 656d 656e 742e 2220  t measurement." 
+00030d10: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00030d20: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00030d30: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00030d40: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00030d50: 2265 6e5f 5553 223e 4d69 6e2e 206c 6f77  "en_US">Min. low
+00030d60: 2073 6964 6520 6f6e 2074 696d 6520 286e   side on time (n
+00030d70: 7329 3c2f 4c61 6265 6c3e 0d0a 2020 2020  s)</Label>..    
+00030d80: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00030d90: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+00030da0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+00030db0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+00030dc0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
+00030dd0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
+00030de0: 3d22 3078 3037 3037 2220 6474 7970 653d  ="0x0707" dtype=
+00030df0: 2275 3332 2220 6964 3d22 4452 565f 5053  "u32" id="DRV_PS
+00030e00: 5f4d 494e 5f48 4947 485f 5349 4445 5f4f  _MIN_HIGH_SIDE_O
+00030e10: 4e5f 5449 4d45 2220 756e 6974 733d 226e  N_TIME" units="n
+00030e20: 7322 2073 7562 6e6f 6465 3d22 3122 2063  s" subnode="1" c
+00030e30: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+00030e40: 6573 633d 2222 2063 6174 5f69 643d 224f  esc="" cat_id="O
+00030e50: 5448 4552 5322 3e0d 0a20 2020 2020 2020  THERS">..       
+00030e60: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00030e70: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00030e80: 6c61 6e67 3d22 656e 5f55 5322 3e4d 696e  lang="en_US">Min
+00030e90: 2e20 6869 6768 2073 6964 6520 6f6e 2074  . high side on t
+00030ea0: 696d 6520 286e 7329 3c2f 4c61 6265 6c3e  ime (ns)</Label>
+00030eb0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+00030ec0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+00030ed0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+00030ee0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+00030ef0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
+00030f00: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
+00030f10: 6464 7265 7373 3d22 3078 3037 3039 2220  ddress="0x0709" 
+00030f20: 6474 7970 653d 2275 3136 2220 6964 3d22  dtype="u16" id="
+00030f30: 4452 565f 5052 4f54 5f43 5552 525f 4f56  DRV_PROT_CURR_OV
+00030f40: 4552 5f52 414e 4745 5f54 4852 4553 484f  ER_RANGE_THRESHO
+00030f50: 4c44 2220 756e 6974 733d 2263 6e74 2220  LD" units="cnt" 
+00030f60: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+00030f70: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+00030f80: 3d22 4e75 6d62 6572 206f 6620 636f 756e  ="Number of coun
+00030f90: 7473 2062 656c 6f77 2041 4443 2063 6569  ts below ADC cei
+00030fa0: 6c69 6e67 2077 6865 7265 2074 6865 2075  ling where the u
+00030fb0: 7070 6572 2073 6174 7572 6174 696f 6e20  pper saturation 
+00030fc0: 6c69 6d69 7420 7769 6c6c 2062 6520 706c  limit will be pl
+00030fd0: 6163 6564 2e20 5573 6564 2066 6f72 2041  aced. Used for A
+00030fe0: 4443 2073 6174 7572 6174 696f 6e20 6572  DC saturation er
+00030ff0: 726f 7220 6465 7465 6374 696f 6e22 2063  ror detection" c
+00031000: 6174 5f69 643d 2250 524f 5445 4354 494f  at_id="PROTECTIO
+00031010: 4e53 223e 0d0a 2020 2020 2020 2020 2020  NS">..          
+00031020: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+00031030: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+00031040: 673d 2265 6e5f 5553 223e 4375 7272 656e  g="en_US">Curren
+00031050: 7420 7361 7475 7261 7469 6f6e 2063 6f75  t saturation cou
+00031060: 6e74 7320 6672 6f6d 2041 4443 2063 6569  nts from ADC cei
+00031070: 6c69 6e67 3c2f 4c61 6265 6c3e 0d0a 2020  ling</Label>..  
+00031080: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+00031090: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
+000310a0: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
+000310b0: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
+000310c0: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
+000310d0: 653d 224e 564d 5f48 5722 2061 6464 7265  e="NVM_HW" addre
+000310e0: 7373 3d22 3078 3037 3041 2220 6474 7970  ss="0x070A" dtyp
+000310f0: 653d 2275 3136 2220 6964 3d22 4452 565f  e="u16" id="DRV_
+00031100: 5052 4f54 5f43 5552 525f 554e 4445 525f  PROT_CURR_UNDER_
+00031110: 5241 4e47 455f 5448 5245 5348 4f4c 4422  RANGE_THRESHOLD"
+00031120: 2075 6e69 7473 3d22 636e 7422 2073 7562   units="cnt" sub
+00031130: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
+00031140: 2243 4f4e 4649 4722 2064 6573 633d 224e  "CONFIG" desc="N
+00031150: 756d 6265 7220 6f66 2063 6f75 6e74 7320  umber of counts 
+00031160: 6162 6f76 6520 4144 4320 666c 6f6f 7220  above ADC floor 
+00031170: 7768 6572 6520 7468 6520 6c6f 7765 7220  where the lower 
+00031180: 7361 7475 7261 7469 6f6e 206c 696d 6974  saturation limit
+00031190: 2077 696c 6c20 6265 2070 6c61 6365 642e   will be placed.
+000311a0: 2055 7365 6420 666f 7220 4144 4320 7361   Used for ADC sa
+000311b0: 7475 7261 7469 6f6e 2065 7272 6f72 2064  turation error d
+000311c0: 6574 6563 7469 6f6e 2220 6361 745f 6964  etection" cat_id
+000311d0: 3d22 5052 4f54 4543 5449 4f4e 5322 3e0d  ="PROTECTIONS">.
+000311e0: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+000311f0: 6c73 3e0d 0a20 2020 2020 2020 2020 2020  ls>..           
+00031200: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
+00031210: 5f55 5322 3e43 7572 7265 6e74 2073 6174  _US">Current sat
+00031220: 7572 6174 696f 6e20 636f 756e 7473 2066  uration counts f
+00031230: 726f 6d20 4144 4320 666c 6f6f 723c 2f4c  rom ADC floor</L
+00031240: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
+00031250: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00031260: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
+00031270: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
+00031280: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
+00031290: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+000312a0: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
+000312b0: 3731 3022 2064 7479 7065 3d22 666c 6f61  710" dtype="floa
+000312c0: 7422 2069 643d 2244 5256 5f50 524f 545f  t" id="DRV_PROT_
+000312d0: 4d41 4e5f 4f56 4552 5f54 454d 5022 2075  MAN_OVER_TEMP" u
+000312e0: 6e69 7473 3d22 c2ba 4322 2073 7562 6e6f  nits="..C" subno
+000312f0: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
+00031300: 4f4e 4649 4722 2064 6573 633d 2249 6e64  ONFIG" desc="Ind
+00031310: 6963 6174 6573 2074 6865 206d 6178 696d  icates the maxim
+00031320: 756d 2073 7570 706f 7274 6564 2074 656d  um supported tem
+00031330: 7065 7261 7475 7265 206f 6620 7468 6520  perature of the 
+00031340: 6472 6976 6522 2063 6174 5f69 643d 2250  drive" cat_id="P
+00031350: 524f 5445 4354 494f 4e53 223e 0d0a 2020  ROTECTIONS">..  
+00031360: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00031370: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
+00031380: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+00031390: 223e 4f76 6572 2d74 656d 7065 7261 7475  ">Over-temperatu
+000313a0: 7265 206c 6576 656c 3c2f 4c61 6265 6c3e  re level</Label>
+000313b0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+000313c0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+000313d0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+000313e0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+000313f0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
+00031400: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
+00031410: 6464 7265 7373 3d22 3078 3037 3131 2220  ddress="0x0711" 
+00031420: 6474 7970 653d 2266 6c6f 6174 2220 6964  dtype="float" id
+00031430: 3d22 4452 565f 5052 4f54 5f4d 414e 5f55  ="DRV_PROT_MAN_U
+00031440: 4e44 4552 5f54 454d 5022 2075 6e69 7473  NDER_TEMP" units
+00031450: 3d22 c2ba 4322 2073 7562 6e6f 6465 3d22  ="..C" subnode="
+00031460: 3122 2063 7963 6c69 633d 2243 4f4e 4649  1" cyclic="CONFI
+00031470: 4722 2064 6573 633d 2249 6e64 6963 6174  G" desc="Indicat
+00031480: 6573 2074 6865 206d 696e 696d 756d 2074  es the minimum t
+00031490: 656d 7065 7261 7475 7265 2061 6c6c 6f77  emperature allow
+000314a0: 6564 2066 6f72 2064 7269 7665 206f 7065  ed for drive ope
+000314b0: 7261 7469 6f6e 2069 6e20 6465 6772 6565  ration in degree
+000314c0: 7320 6365 6c73 6975 7322 2063 6174 5f69  s celsius" cat_i
+000314d0: 643d 2250 524f 5445 4354 494f 4e53 223e  d="PROTECTIONS">
+000314e0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+000314f0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00031500: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00031510: 6e5f 5553 223e 556e 6465 722d 7465 6d70  n_US">Under-temp
+00031520: 6572 6174 7572 6520 6c65 7665 6c3c 2f4c  erature level</L
+00031530: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
+00031540: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00031550: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
+00031560: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
+00031570: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
+00031580: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+00031590: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
+000315a0: 3731 3222 2064 7479 7065 3d22 666c 6f61  712" dtype="floa
+000315b0: 7422 2069 643d 2244 5256 5f50 524f 545f  t" id="DRV_PROT_
+000315c0: 4d41 4e5f 4f56 4552 5f56 4f4c 5422 2075  MAN_OVER_VOLT" u
+000315d0: 6e69 7473 3d22 5622 2073 7562 6e6f 6465  nits="V" subnode
+000315e0: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+000315f0: 4649 4722 2064 6573 633d 2249 6e64 6963  FIG" desc="Indic
+00031600: 6174 6573 2074 6865 206d 6178 696d 756d  ates the maximum
+00031610: 2073 7570 706f 7274 6564 2062 7573 2076   supported bus v
+00031620: 6f6c 7461 6765 2062 7920 7468 6520 6472  oltage by the dr
+00031630: 6976 6522 2063 6174 5f69 643d 2250 524f  ive" cat_id="PRO
+00031640: 5445 4354 494f 4e53 223e 0d0a 2020 2020  TECTIONS">..    
+00031650: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00031660: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+00031670: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00031680: 4f76 6572 2d76 6f6c 7461 6765 206c 6576  Over-voltage lev
+00031690: 656c 3c2f 4c61 6265 6c3e 0d0a 2020 2020  el</Label>..    
+000316a0: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+000316b0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+000316c0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+000316d0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+000316e0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
+000316f0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
+00031700: 3d22 3078 3037 3133 2220 6474 7970 653d  ="0x0713" dtype=
+00031710: 2266 6c6f 6174 2220 6964 3d22 4452 565f  "float" id="DRV_
+00031720: 5052 4f54 5f4d 414e 5f55 4e44 4552 5f56  PROT_MAN_UNDER_V
+00031730: 4f4c 5422 2075 6e69 7473 3d22 5622 2073  OLT" units="V" s
+00031740: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
+00031750: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
+00031760: 2249 6e64 6963 6174 6573 2074 6865 206d  "Indicates the m
+00031770: 696e 696d 756d 2076 6f6c 7461 6765 2072  inimum voltage r
+00031780: 6571 7569 7265 6420 6279 2074 6865 2064  equired by the d
+00031790: 7269 7665 2066 6f72 2061 2070 726f 7065  rive for a prope
+000317a0: 7220 6f70 6572 6174 696f 6e22 2063 6174  r operation" cat
+000317b0: 5f69 643d 2250 524f 5445 4354 494f 4e53  _id="PROTECTIONS
+000317c0: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+000317d0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+000317e0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+000317f0: 2265 6e5f 5553 223e 556e 6465 722d 766f  "en_US">Under-vo
+00031800: 6c74 6167 6520 6c65 7665 6c3c 2f4c 6162  ltage level</Lab
+00031810: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+00031820: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00031830: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+00031840: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+00031850: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
+00031860: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
+00031870: 2220 6164 6472 6573 733d 2230 7830 3731  " address="0x071
+00031880: 4422 2064 7479 7065 3d22 666c 6f61 7422  D" dtype="float"
+00031890: 2069 643d 2244 5256 5f50 524f 545f 4d41   id="DRV_PROT_MA
+000318a0: 4e5f 4d41 585f 434f 4e54 5f43 5552 5245  N_MAX_CONT_CURRE
+000318b0: 4e54 5f56 414c 5545 2220 756e 6974 733d  NT_VALUE" units=
+000318c0: 2241 2220 7375 626e 6f64 653d 2231 2220  "A" subnode="1" 
+000318d0: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+000318e0: 6465 7363 3d22 4d61 7869 6d75 6d20 636f  desc="Maximum co
+000318f0: 6e74 696e 756f 7573 2063 7572 7265 6e74  ntinuous current
+00031900: 206f 6e20 7468 6520 6472 6976 6522 2063   on the drive" c
+00031910: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+00031920: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00031930: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00031940: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00031950: 656e 5f55 5322 3e4d 6178 696d 756d 2064  en_US">Maximum d
+00031960: 7269 7665 2063 7572 7265 6e74 3c2f 4c61  rive current</La
+00031970: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
+00031980: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00031990: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+000319a0: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+000319b0: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+000319c0: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
+000319d0: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
+000319e0: 3145 2220 6474 7970 653d 2275 3332 2220  1E" dtype="u32" 
+000319f0: 6964 3d22 4452 565f 5052 4f54 5f4d 414e  id="DRV_PROT_MAN
+00031a00: 5f4d 4158 5f50 4541 4b5f 4355 5252 454e  _MAX_PEAK_CURREN
+00031a10: 545f 5449 4d45 2220 756e 6974 733d 226d  T_TIME" units="m
+00031a20: 7322 2073 7562 6e6f 6465 3d22 3122 2063  s" subnode="1" c
+00031a30: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+00031a40: 6573 633d 224d 6178 696d 756d 2074 696d  esc="Maximum tim
+00031a50: 6520 696e 206d 696c 6c69 7365 636f 6e64  e in millisecond
+00031a60: 7320 7468 6520 6d61 7869 6d75 6d20 7065  s the maximum pe
+00031a70: 616b 2063 7572 7265 6e74 2063 616e 2062  ak current can b
+00031a80: 6520 6472 6976 656e 2062 7920 7468 6520  e driven by the 
+00031a90: 6472 6976 652e 2220 6361 745f 6964 3d22  drive." cat_id="
+00031aa0: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
+00031ab0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00031ac0: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+00031ad0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00031ae0: 4d61 7869 6d75 6d20 6472 6976 6520 7065  Maximum drive pe
+00031af0: 616b 2063 7572 7265 6e74 2074 696d 653c  ak current time<
+00031b00: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+00031b10: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+00031b20: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
+00031b30: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
+00031b40: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
+00031b50: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
+00031b60: 4d5f 4857 2220 6164 6472 6573 733d 2230  M_HW" address="0
+00031b70: 7830 3731 4622 2064 7479 7065 3d22 666c  x071F" dtype="fl
+00031b80: 6f61 7422 2069 643d 2244 5256 5f50 524f  oat" id="DRV_PRO
+00031b90: 545f 4d41 4e5f 4d41 585f 5045 414b 5f43  T_MAN_MAX_PEAK_C
+00031ba0: 5552 5245 4e54 5f56 414c 5545 2220 756e  URRENT_VALUE" un
+00031bb0: 6974 733d 2241 2220 7375 626e 6f64 653d  its="A" subnode=
+00031bc0: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+00031bd0: 4947 2220 6465 7363 3d22 4d61 7869 6d75  IG" desc="Maximu
+00031be0: 6d20 6162 736f 6c75 7465 2061 6c6c 6f77  m absolute allow
+00031bf0: 6564 2063 7572 7265 6e74 206f 6e20 6472  ed current on dr
+00031c00: 6976 6522 2063 6174 5f69 643d 2249 4e54  ive" cat_id="INT
+00031c10: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
+00031c20: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00031c30: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00031c40: 6c61 6e67 3d22 656e 5f55 5322 3e4d 6178  lang="en_US">Max
+00031c50: 696d 756d 2064 7269 7665 2070 6561 6b20  imum drive peak 
+00031c60: 6375 7272 656e 743c 2f4c 6162 656c 3e0d  current</Label>.
+00031c70: 0a20 2020 2020 2020 2020 203c 2f4c 6162  .          </Lab
+00031c80: 656c 733e 0d0a 2020 2020 2020 2020 3c2f  els>..        </
+00031c90: 5265 6769 7374 6572 3e0d 0a20 2020 2020  Register>..     
+00031ca0: 2020 203c 5265 6769 7374 6572 2061 6363     <Register acc
+00031cb0: 6573 733d 2272 2220 6164 6472 6573 735f  ess="r" address_
+00031cc0: 7479 7065 3d22 4e56 4d5f 4857 2220 6164  type="NVM_HW" ad
+00031cd0: 6472 6573 733d 2230 7830 3732 3022 2064  dress="0x0720" d
+00031ce0: 7479 7065 3d22 666c 6f61 7422 2069 643d  type="float" id=
+00031cf0: 2246 424b 5f43 5552 5f4d 4541 535f 5241  "FBK_CUR_MEAS_RA
+00031d00: 4e47 4531 2220 756e 6974 733d 2241 2220  NGE1" units="A" 
+00031d10: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+00031d20: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+00031d30: 3d22 4675 6c6c 206d 6561 7375 7269 6e67  ="Full measuring
+00031d40: 2072 616e 6765 2066 6f72 2074 6865 2076   range for the v
+00031d50: 6172 6961 626c 6520 6761 696e 2063 6f6e  ariable gain con
+00031d60: 6669 6775 7261 7469 6f6e 2031 2069 6e20  figuration 1 in 
+00031d70: 416d 7065 7265 7322 2063 6174 5f69 643d  Amperes" cat_id=
+00031d80: 2249 4e54 4552 4e41 4c22 3e0d 0a20 2020  "INTERNAL">..   
+00031d90: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00031da0: 0a20 2020 2020 2020 2020 2020 203c 4c61  .            <La
+00031db0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00031dc0: 3e43 7572 7265 6e74 206d 6561 7375 7269  >Current measuri
+00031dd0: 6e67 2072 616e 6765 2031 3c2f 4c61 6265  ng range 1</Labe
+00031de0: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00031df0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00031e00: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+00031e10: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
+00031e20: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
+00031e30: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
+00031e40: 2061 6464 7265 7373 3d22 3078 3037 3231   address="0x0721
+00031e50: 2220 6474 7970 653d 2266 6c6f 6174 2220  " dtype="float" 
+00031e60: 6964 3d22 4642 4b5f 4355 525f 4d45 4153  id="FBK_CUR_MEAS
+00031e70: 5f52 414e 4745 3222 2075 6e69 7473 3d22  _RANGE2" units="
+00031e80: 4122 2073 7562 6e6f 6465 3d22 3122 2063  A" subnode="1" c
+00031e90: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+00031ea0: 6573 633d 2246 756c 6c20 6d65 6173 7572  esc="Full measur
+00031eb0: 696e 6720 7261 6e67 6520 666f 7220 7468  ing range for th
+00031ec0: 6520 7661 7269 6162 6c65 2067 6169 6e20  e variable gain 
+00031ed0: 636f 6e66 6967 7572 6174 696f 6e20 3220  configuration 2 
+00031ee0: 696e 2041 6d70 6572 6573 2220 6361 745f  in Amperes" cat_
+00031ef0: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+00031f00: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00031f10: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00031f20: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00031f30: 5553 223e 4375 7272 656e 7420 6d65 6173  US">Current meas
+00031f40: 7572 696e 6720 7261 6e67 6520 323c 2f4c  uring range 2</L
+00031f50: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
+00031f60: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00031f70: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
+00031f80: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
+00031f90: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
+00031fa0: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+00031fb0: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
+00031fc0: 3732 3222 2064 7479 7065 3d22 666c 6f61  722" dtype="floa
+00031fd0: 7422 2069 643d 2246 424b 5f43 5552 5f4d  t" id="FBK_CUR_M
+00031fe0: 4541 535f 5241 4e47 4533 2220 756e 6974  EAS_RANGE3" unit
+00031ff0: 733d 2241 2220 7375 626e 6f64 653d 2231  s="A" subnode="1
+00032000: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
+00032010: 2220 6465 7363 3d22 4675 6c6c 206d 6561  " desc="Full mea
+00032020: 7375 7269 6e67 2072 616e 6765 2066 6f72  suring range for
+00032030: 2074 6865 2076 6172 6961 626c 6520 6761   the variable ga
+00032040: 696e 2063 6f6e 6669 6775 7261 7469 6f6e  in configuration
+00032050: 2033 2069 6e20 416d 7065 7265 7322 2063   3 in Amperes" c
+00032060: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+00032070: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00032080: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00032090: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+000320a0: 656e 5f55 5322 3e43 7572 7265 6e74 206d  en_US">Current m
+000320b0: 6561 7375 7269 6e67 2072 616e 6765 2033  easuring range 3
+000320c0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+000320d0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+000320e0: 2020 2020 2020 203c 2f52 6567 6973 7465         </Registe
+000320f0: 723e 0d0a 2020 2020 2020 2020 3c52 6567  r>..        <Reg
+00032100: 6973 7465 7220 6163 6365 7373 3d22 7222  ister access="r"
+00032110: 2061 6464 7265 7373 5f74 7970 653d 224e   address_type="N
+00032120: 564d 5f48 5722 2061 6464 7265 7373 3d22  VM_HW" address="
+00032130: 3078 3037 3233 2220 6474 7970 653d 2266  0x0723" dtype="f
+00032140: 6c6f 6174 2220 6964 3d22 4642 4b5f 4355  loat" id="FBK_CU
+00032150: 525f 4d45 4153 5f52 414e 4745 3422 2075  R_MEAS_RANGE4" u
+00032160: 6e69 7473 3d22 4122 2073 7562 6e6f 6465  nits="A" subnode
+00032170: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+00032180: 4649 4722 2064 6573 633d 2246 756c 6c20  FIG" desc="Full 
+00032190: 6d65 6173 7572 696e 6720 7261 6e67 6520  measuring range 
+000321a0: 666f 7220 7468 6520 7661 7269 6162 6c65  for the variable
+000321b0: 2067 6169 6e20 636f 6e66 6967 7572 6174   gain configurat
+000321c0: 696f 6e20 3420 696e 2041 6d70 6572 6573  ion 4 in Amperes
+000321d0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
+000321e0: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
+000321f0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+00032200: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+00032210: 673d 2265 6e5f 5553 223e 4375 7272 656e  g="en_US">Curren
+00032220: 7420 6d65 6173 7572 696e 6720 7261 6e67  t measuring rang
+00032230: 6520 343c 2f4c 6162 656c 3e0d 0a20 2020  e 4</Label>..   
+00032240: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00032250: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+00032260: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+00032270: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+00032280: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+00032290: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
+000322a0: 733d 2230 7830 3732 3822 2064 7479 7065  s="0x0728" dtype
+000322b0: 3d22 7531 3622 2069 643d 2246 424b 5f43  ="u16" id="FBK_C
+000322c0: 5552 5f4d 4153 4b22 2075 6e69 7473 3d22  UR_MASK" units="
+000322d0: 2d22 2073 7562 6e6f 6465 3d22 3122 2063  -" subnode="1" c
+000322e0: 7963 6c69 633d 2243 4f4e 4649 4722 2064  yclic="CONFIG" d
+000322f0: 6573 633d 2249 6e69 6469 6361 7465 7320  esc="Inidicates 
+00032300: 7468 6520 6e75 6d62 6572 206f 6620 6176  the number of av
+00032310: 6169 6c61 626c 6520 7365 6e73 6f72 7320  ailable sensors 
+00032320: 666f 7220 6375 7272 656e 7420 7365 6e73  for current sens
+00032330: 696e 6722 2063 6174 5f69 643d 2249 4e54  ing" cat_id="INT
+00032340: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
+00032350: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00032360: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00032370: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00032380: 7265 6e74 2073 656e 736f 7273 2075 7365  rent sensors use
+00032390: 6420 6d61 736b 3c2f 4c61 6265 6c3e 0d0a  d mask</Label>..
+000323a0: 2020 2020 2020 2020 2020 3c2f 4c61 6265            </Labe
+000323b0: 6c73 3e0d 0a20 2020 2020 2020 203c 2f52  ls>..        </R
+000323c0: 6567 6973 7465 723e 0d0a 2020 2020 2020  egister>..      
+000323d0: 2020 3c52 6567 6973 7465 7220 6163 6365    <Register acce
+000323e0: 7373 3d22 7222 2061 6464 7265 7373 5f74  ss="r" address_t
+000323f0: 7970 653d 224e 564d 5f48 5722 2061 6464  ype="NVM_HW" add
+00032400: 7265 7373 3d22 3078 3037 3239 2220 6474  ress="0x0729" dt
+00032410: 7970 653d 2275 3136 2220 6964 3d22 4642  ype="u16" id="FB
+00032420: 4b5f 4355 525f 4143 515f 5449 4d45 2220  K_CUR_ACQ_TIME" 
+00032430: 756e 6974 733d 226e 7322 2073 7562 6e6f  units="ns" subno
+00032440: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
+00032450: 4f4e 4649 4722 2064 6573 633d 2243 7572  ONFIG" desc="Cur
+00032460: 7265 6e74 2061 6371 7569 7369 7469 6f6e  rent acquisition
+00032470: 2028 7361 6d70 6c65 2061 6e64 2068 6f6c   (sample and hol
+00032480: 6429 2074 696d 6520 696e 206e 616e 6f73  d) time in nanos
+00032490: 6563 6f6e 6473 2220 6361 745f 6964 3d22  econds" cat_id="
+000324a0: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
+000324b0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+000324c0: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+000324d0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+000324e0: 4375 7272 656e 7420 6163 7175 6973 6974  Current acquisit
+000324f0: 696f 6e20 7469 6d65 2028 6e73 293c 2f4c  ion time (ns)</L
+00032500: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
+00032510: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00032520: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
+00032530: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
+00032540: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
+00032550: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+00032560: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
+00032570: 3732 4122 2064 7479 7065 3d22 7531 3622  72A" dtype="u16"
+00032580: 2069 643d 2246 424b 5f43 5552 5f41 4351   id="FBK_CUR_ACQ
+00032590: 5f41 4456 414e 4345 5f54 494d 4522 2075  _ADVANCE_TIME" u
+000325a0: 6e69 7473 3d22 6e73 2220 7375 626e 6f64  nits="ns" subnod
+000325b0: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+000325c0: 4e46 4947 2220 6465 7363 3d22 4375 7272  NFIG" desc="Curr
+000325d0: 656e 7420 6163 7175 6973 6974 696f 6e20  ent acquisition 
+000325e0: 6164 7661 6e63 6520 7469 6d65 2066 726f  advance time fro
+000325f0: 6d20 6365 6e74 6572 206f 6620 5057 4d20  m center of PWM 
+00032600: 696e 206e 616e 6f73 6563 6f6e 6473 2220  in nanoseconds" 
+00032610: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00032620: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00032630: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00032640: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00032650: 2265 6e5f 5553 223e 4375 7272 656e 7420  "en_US">Current 
+00032660: 6163 7175 6973 6974 696f 6e20 6164 7661  acquisition adva
+00032670: 6e63 6520 7469 6d65 2028 6e73 293c 2f4c  nce time (ns)</L
+00032680: 6162 656c 3e0d 0a20 2020 2020 2020 2020  abel>..         
+00032690: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+000326a0: 2020 2020 3c2f 5265 6769 7374 6572 3e0d      </Register>.
+000326b0: 0a20 2020 2020 2020 203c 5265 6769 7374  .        <Regist
+000326c0: 6572 2061 6363 6573 733d 2272 2220 6164  er access="r" ad
+000326d0: 6472 6573 735f 7479 7065 3d22 4e56 4d5f  dress_type="NVM_
+000326e0: 4857 2220 6164 6472 6573 733d 2230 7830  HW" address="0x0
+000326f0: 3732 4222 2064 7479 7065 3d22 7533 3222  72B" dtype="u32"
+00032700: 2069 643d 2244 5256 5f50 535f 4d49 4e5f   id="DRV_PS_MIN_
+00032710: 4c4f 575f 5349 4445 5f4f 4e5f 5449 4d45  LOW_SIDE_ON_TIME
+00032720: 5f32 2220 756e 6974 733d 226e 7322 2073  _2" units="ns" s
+00032730: 7562 6e6f 6465 3d22 3122 2063 7963 6c69  ubnode="1" cycli
+00032740: 633d 2243 4f4e 4649 4722 2064 6573 633d  c="CONFIG" desc=
+00032750: 224d 696e 696d 756d 206c 6f77 2073 6964  "Minimum low sid
+00032760: 6520 6f6e 2074 696d 6520 696e 206e 616e  e on time in nan
+00032770: 6f73 6563 6f6e 6473 2066 6f72 2066 7265  oseconds for fre
+00032780: 7175 656e 6379 2073 656c 6563 7469 6f6e  quency selection
+00032790: 2032 2220 6361 745f 6964 3d22 494e 5445   2" cat_id="INTE
+000327a0: 524e 414c 223e 0d0a 2020 2020 2020 2020  RNAL">..        
+000327b0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
+000327c0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+000327d0: 616e 673d 2265 6e5f 5553 223e 4d69 6e2e  ang="en_US">Min.
+000327e0: 206c 6f77 2073 6964 6520 6f6e 2074 696d   low side on tim
+000327f0: 6520 3220 286e 7329 3c2f 4c61 6265 6c3e  e 2 (ns)</Label>
+00032800: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+00032810: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+00032820: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+00032830: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+00032840: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
+00032850: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
+00032860: 6464 7265 7373 3d22 3078 3037 3243 2220  ddress="0x072C" 
+00032870: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
+00032880: 4452 565f 5053 5f4d 494e 5f4c 4f57 5f53  DRV_PS_MIN_LOW_S
+00032890: 4944 455f 4f4e 5f54 494d 455f 3322 2075  IDE_ON_TIME_3" u
+000328a0: 6e69 7473 3d22 6e73 2220 7375 626e 6f64  nits="ns" subnod
+000328b0: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+000328c0: 4e46 4947 2220 6465 7363 3d22 4d69 6e69  NFIG" desc="Mini
+000328d0: 6d75 6d20 6c6f 7720 7369 6465 206f 6e20  mum low side on 
+000328e0: 7469 6d65 2069 6e20 6e61 6e6f 7365 636f  time in nanoseco
+000328f0: 6e64 7320 666f 7220 6672 6571 7565 6e63  nds for frequenc
+00032900: 7920 7365 6c65 6374 696f 6e20 3322 2063  y selection 3" c
+00032910: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+00032920: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00032930: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00032940: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00032950: 656e 5f55 5322 3e4d 696e 2e20 6c6f 7720  en_US">Min. low 
+00032960: 7369 6465 206f 6e20 7469 6d65 2033 2028  side on time 3 (
+00032970: 6e73 293c 2f4c 6162 656c 3e0d 0a20 2020  ns)</Label>..   
+00032980: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00032990: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+000329a0: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+000329b0: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+000329c0: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+000329d0: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
+000329e0: 733d 2230 7830 3732 4422 2064 7479 7065  s="0x072D" dtype
+000329f0: 3d22 7533 3222 2069 643d 2244 5256 5f50  ="u32" id="DRV_P
+00032a00: 535f 4d49 4e5f 4c4f 575f 5349 4445 5f4f  S_MIN_LOW_SIDE_O
+00032a10: 4e5f 5449 4d45 5f34 2220 756e 6974 733d  N_TIME_4" units=
+00032a20: 226e 7322 2073 7562 6e6f 6465 3d22 3122  "ns" subnode="1"
+00032a30: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00032a40: 2064 6573 633d 224d 696e 696d 756d 206c   desc="Minimum l
+00032a50: 6f77 2073 6964 6520 6f6e 2074 696d 6520  ow side on time 
+00032a60: 696e 206e 616e 6f73 6563 6f6e 6473 2066  in nanoseconds f
+00032a70: 6f72 2066 7265 7175 656e 6379 2073 656c  or frequency sel
+00032a80: 6563 7469 6f6e 2034 2220 6361 745f 6964  ection 4" cat_id
+00032a90: 3d22 494e 5445 524e 414c 223e 0d0a 2020  ="INTERNAL">..  
+00032aa0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00032ab0: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
+00032ac0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+00032ad0: 223e 4d69 6e2e 206c 6f77 2073 6964 6520  ">Min. low side 
+00032ae0: 6f6e 2074 696d 6520 3420 286e 7329 3c2f  on time 4 (ns)</
+00032af0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+00032b00: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00032b10: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
+00032b20: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
+00032b30: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
+00032b40: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
+00032b50: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
+00032b60: 3037 3332 2220 6474 7970 653d 2266 6c6f  0732" dtype="flo
+00032b70: 6174 2220 6964 3d22 4452 565f 5052 4f54  at" id="DRV_PROT
+00032b80: 5f56 4255 535f 4d45 4153 5f52 414e 4745  _VBUS_MEAS_RANGE
+00032b90: 2220 756e 6974 733d 2256 2220 7375 626e  " units="V" subn
+00032ba0: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
+00032bb0: 434f 4e46 4947 2220 6465 7363 3d22 4675  CONFIG" desc="Fu
+00032bc0: 6c6c 2072 616e 6765 206f 6620 6275 7320  ll range of bus 
+00032bd0: 766f 6c74 6167 6520 6d65 6173 7572 656d  voltage measurem
+00032be0: 656e 7473 2069 6e20 766f 6c74 732e 2220  ents in volts." 
+00032bf0: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00032c00: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00032c10: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00032c20: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00032c30: 2265 6e5f 5553 223e 4275 7320 766f 6c74  "en_US">Bus volt
+00032c40: 6167 6520 6d65 6173 7572 696e 6720 7261  age measuring ra
+00032c50: 6e67 653c 2f4c 6162 656c 3e0d 0a20 2020  nge</Label>..   
+00032c60: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00032c70: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+00032c80: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+00032c90: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+00032ca0: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+00032cb0: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
+00032cc0: 733d 2230 7830 3733 3322 2064 7479 7065  s="0x0733" dtype
+00032cd0: 3d22 666c 6f61 7422 2069 643d 2244 5256  ="float" id="DRV
+00032ce0: 5f50 524f 545f 5642 5553 5f4f 4646 5345  _PROT_VBUS_OFFSE
+00032cf0: 5422 2075 6e69 7473 3d22 5622 2073 7562  T" units="V" sub
+00032d00: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
+00032d10: 2243 4f4e 4649 4722 2064 6573 633d 2243  "CONFIG" desc="C
+00032d20: 6f6e 7374 616e 7420 6572 726f 7220 696e  onstant error in
+00032d30: 2076 6f6c 7473 206f 6620 7468 6520 6275   volts of the bu
+00032d40: 7320 766f 6c74 6167 6520 6d65 6173 7572  s voltage measur
+00032d50: 656d 656e 7473 2220 6361 745f 6964 3d22  ements" cat_id="
+00032d60: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
+00032d70: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00032d80: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+00032d90: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00032da0: 4275 7320 766f 6c74 6167 6520 7265 6164  Bus voltage read
+00032db0: 696e 6720 6f66 6673 6574 3c2f 4c61 6265  ing offset</Labe
+00032dc0: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00032dd0: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00032de0: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+00032df0: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
+00032e00: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
+00032e10: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
+00032e20: 2061 6464 7265 7373 3d22 3078 3037 3334   address="0x0734
+00032e30: 2220 6474 7970 653d 2275 3136 2220 6964  " dtype="u16" id
+00032e40: 3d22 4452 565f 5052 4f54 5f50 5249 4d5f  ="DRV_PROT_PRIM_
+00032e50: 5445 4d50 5f54 5950 4522 2075 6e69 7473  TEMP_TYPE" units
+00032e60: 3d22 2d22 2073 7562 6e6f 6465 3d22 3122  ="-" subnode="1"
+00032e70: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00032e80: 2064 6573 633d 2249 6e64 6963 6174 6573   desc="Indicates
+00032e90: 2074 6865 2074 656d 7065 7261 7475 7265   the temperature
+00032ea0: 2073 656e 736f 7220 7573 6564 2066 6f72   sensor used for
+00032eb0: 2070 7269 6d61 7279 2074 656d 7065 7261   primary tempera
+00032ec0: 7475 7265 2072 6561 6469 6e67 7320 6f66  ture readings of
+00032ed0: 2074 6865 2070 6f77 6572 2073 7461 6765   the power stage
+00032ee0: 2e22 2063 6174 5f69 643d 2249 4e54 4552  ." cat_id="INTER
+00032ef0: 4e41 4c22 3e0d 0a20 2020 2020 2020 2020  NAL">..         
+00032f00: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00032f10: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00032f20: 6e67 3d22 656e 5f55 5322 3e50 6f77 6572  ng="en_US">Power
+00032f30: 2073 7461 6765 2074 656d 702e 2073 656e   stage temp. sen
+00032f40: 736f 7220 3120 7479 7065 3c2f 4c61 6265  sor 1 type</Labe
+00032f50: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00032f60: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00032f70: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+00032f80: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
+00032f90: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
+00032fa0: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
+00032fb0: 2061 6464 7265 7373 3d22 3078 3037 3335   address="0x0735
+00032fc0: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
+00032fd0: 3d22 4452 565f 5052 4f54 5f50 5249 4d5f  ="DRV_PROT_PRIM_
+00032fe0: 5445 4d50 5f52 4553 2220 756e 6974 733d  TEMP_RES" units=
+00032ff0: 22ce a922 2073 7562 6e6f 6465 3d22 3122  ".." subnode="1"
+00033000: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00033010: 2064 6573 633d 224e 5443 3a20 5265 7369   desc="NTC: Resi
+00033020: 7374 616e 6365 2076 616c 7565 2066 6f72  stance value for
+00033030: 2032 3520 c2ba 4320 696e 206f 686d 7326   25 ..C in ohms&
+00033040: 2331 333b 2623 3130 3b50 5443 3a20 5265  #13;&#10;PTC: Re
+00033050: 7369 7374 616e 6365 2076 616c 7565 2069  sistance value i
+00033060: 6e20 6f68 6d73 2077 6865 7265 2074 6865  n ohms where the
+00033070: 206f 7665 722d 7465 6d70 6572 6174 7572   over-temperatur
+00033080: 6520 6d75 7374 2062 6520 6465 7465 6374  e must be detect
+00033090: 6564 2623 3133 3b26 2331 303b 4f74 6865  ed&#13;&#10;Othe
+000330a0: 7273 3a20 4e6f 7420 7573 6564 2220 6361  rs: Not used" ca
+000330b0: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
+000330c0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+000330d0: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+000330e0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+000330f0: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
+00033100: 6520 7465 6d70 2e20 7365 6e73 6f72 2031  e temp. sensor 1
+00033110: 2072 6573 6973 7461 6e63 653c 2f4c 6162   resistance</Lab
+00033120: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+00033130: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00033140: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+00033150: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+00033160: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
+00033170: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
+00033180: 2220 6164 6472 6573 733d 2230 7830 3733  " address="0x073
+00033190: 3622 2064 7479 7065 3d22 7531 3622 2069  6" dtype="u16" i
+000331a0: 643d 2244 5256 5f50 524f 545f 5052 494d  d="DRV_PROT_PRIM
+000331b0: 5f54 454d 505f 4232 3538 3522 2075 6e69  _TEMP_B2585" uni
+000331c0: 7473 3d22 c2ba 4b22 2073 7562 6e6f 6465  ts="..K" subnode
+000331d0: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+000331e0: 4649 4722 2064 6573 633d 224e 5443 3a20  FIG" desc="NTC: 
+000331f0: 4228 3235 2f38 3529 2070 6172 616d 6574  B(25/85) paramet
+00033200: 6572 2066 726f 6d20 6461 7461 7368 6565  er from datashee
+00033210: 7426 2331 333b 2623 3130 3b4f 7468 6572  t&#13;&#10;Other
+00033220: 733a 204e 6f74 2075 7365 6422 2063 6174  s: Not used" cat
+00033230: 5f69 643d 2249 4e54 4552 4e41 4c22 3e0d  _id="INTERNAL">.
+00033240: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+00033250: 6c73 3e0d 0a20 2020 2020 2020 2020 2020  ls>..           
+00033260: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
+00033270: 5f55 5322 3e50 6f77 6572 2073 7461 6765  _US">Power stage
+00033280: 2074 656d 702e 2073 656e 736f 7220 3120   temp. sensor 1 
+00033290: ceb2 3c2f 4c61 6265 6c3e 0d0a 2020 2020  ..</Label>..    
+000332a0: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+000332b0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+000332c0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+000332d0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+000332e0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
+000332f0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
+00033300: 3d22 3078 3037 3337 2220 6474 7970 653d  ="0x0737" dtype=
+00033310: 2275 3332 2220 6964 3d22 4452 565f 5052  "u32" id="DRV_PR
+00033320: 4f54 5f50 5249 4d5f 5445 4d50 5f45 5854  OT_PRIM_TEMP_EXT
+00033330: 5f52 4553 2220 756e 6974 733d 22ce a922  _RES" units=".."
+00033340: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
+00033350: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
+00033360: 633d 224e 5443 2026 616d 703b 616d 703b  c="NTC &amp;amp;
+00033370: 2050 5443 3a20 5265 7369 7374 616e 6365   PTC: Resistance
+00033380: 2076 616c 7565 2069 6e20 6f68 6d73 2063   value in ohms c
+00033390: 6f6e 6e65 6374 6564 2074 6f20 7365 6e73  onnected to sens
+000333a0: 6f72 2066 6f72 206d 616b 696e 6720 7468  or for making th
+000333b0: 6520 766f 6c74 6167 6520 6469 7669 6465  e voltage divide
+000333c0: 7226 2331 333b 2623 3130 3b4f 7468 6572  r&#13;&#10;Other
+000333d0: 3a20 4e6f 7420 7573 6564 2220 6361 745f  : Not used" cat_
+000333e0: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+000333f0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00033400: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00033410: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00033420: 5553 223e 506f 7765 7220 7374 6167 6520  US">Power stage 
+00033430: 7465 6d70 2e20 7365 6e73 6f72 2031 2065  temp. sensor 1 e
+00033440: 7874 2e20 7265 7369 7374 616e 6365 3c2f  xt. resistance</
+00033450: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+00033460: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00033470: 2020 2020 203c 2f52 6567 6973 7465 723e       </Register>
+00033480: 0d0a 2020 2020 2020 2020 3c52 6567 6973  ..        <Regis
+00033490: 7465 7220 6163 6365 7373 3d22 7222 2061  ter access="r" a
+000334a0: 6464 7265 7373 5f74 7970 653d 224e 564d  ddress_type="NVM
+000334b0: 5f48 5722 2061 6464 7265 7373 3d22 3078  _HW" address="0x
+000334c0: 3037 3338 2220 6474 7970 653d 2266 6c6f  0738" dtype="flo
+000334d0: 6174 2220 6964 3d22 4452 565f 5052 4f54  at" id="DRV_PROT
+000334e0: 5f50 5249 4d5f 5445 4d50 5f47 4149 4e22  _PRIM_TEMP_GAIN"
+000334f0: 2075 6e69 7473 3d22 c2ba 4320 2f20 5622   units="..C / V"
+00033500: 2073 7562 6e6f 6465 3d22 3122 2063 7963   subnode="1" cyc
+00033510: 6c69 633d 2243 4f4e 4649 4722 2064 6573  lic="CONFIG" des
+00033520: 633d 224c 696e 6561 7220 766f 6c74 6167  c="Linear voltag
+00033530: 6520 7365 6e73 6f72 3a20 4761 696e 206f  e sensor: Gain o
+00033540: 6620 7468 6520 7365 6e73 6f72 2623 3133  f the sensor&#13
+00033550: 3b26 2331 303b 4f74 6865 7273 3a20 4e6f  ;&#10;Others: No
+00033560: 7420 7573 6564 2220 6361 745f 6964 3d22  t used" cat_id="
+00033570: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
+00033580: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00033590: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+000335a0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+000335b0: 506f 7765 7220 7374 6167 6520 7465 6d70  Power stage temp
+000335c0: 2e20 7365 6e73 6f72 2031 2067 6169 6e3c  . sensor 1 gain<
+000335d0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+000335e0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+000335f0: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
+00033600: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
+00033610: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
+00033620: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
+00033630: 4d5f 4857 2220 6164 6472 6573 733d 2230  M_HW" address="0
+00033640: 7830 3733 3922 2064 7479 7065 3d22 666c  x0739" dtype="fl
+00033650: 6f61 7422 2069 643d 2244 5256 5f50 524f  oat" id="DRV_PRO
+00033660: 545f 5052 494d 5f54 454d 505f 4f46 4653  T_PRIM_TEMP_OFFS
+00033670: 4554 2220 756e 6974 733d 22c2 ba43 2220  ET" units="..C" 
+00033680: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+00033690: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+000336a0: 3d22 4e54 4320 2661 6d70 3b61 6d70 3b20  ="NTC &amp;amp; 
+000336b0: 5054 433a 204e 6f74 2075 7365 6426 2331  PTC: Not used&#1
+000336c0: 333b 2623 3130 3b4c 696e 6561 7220 7365  3;&#10;Linear se
+000336d0: 6e73 6f72 3a20 4f66 6673 6574 206f 6620  nsor: Offset of 
+000336e0: 7468 6520 7365 6e73 6f72 2220 6361 745f  the sensor" cat_
+000336f0: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+00033700: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00033710: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00033720: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00033730: 5553 223e 506f 7765 7220 7374 6167 6520  US">Power stage 
+00033740: 7465 6d70 2e20 7365 6e73 6f72 2031 206f  temp. sensor 1 o
+00033750: 6666 7365 743c 2f4c 6162 656c 3e0d 0a20  ffset</Label>.. 
+00033760: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00033770: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00033780: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00033790: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+000337a0: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+000337b0: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+000337c0: 6573 733d 2230 7830 3734 3022 2064 7479  ess="0x0740" dty
+000337d0: 7065 3d22 7533 3222 2069 643d 2244 5256  pe="u32" id="DRV
+000337e0: 5f50 524f 545f 5354 4f5f 4346 4722 2075  _PROT_STO_CFG" u
+000337f0: 6e69 7473 3d22 2d22 2073 7562 6e6f 6465  nits="-" subnode
+00033800: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+00033810: 4649 4722 2064 6573 633d 2249 6e64 6963  FIG" desc="Indic
+00033820: 6174 6573 2074 6865 2047 5049 2075 7365  ates the GPI use
+00033830: 6420 666f 7220 6465 7465 6374 696e 6720  d for detecting 
+00033840: 5354 4f20 6e6f 7469 6669 6361 7469 6f6e  STO notification
+00033850: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
+00033860: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
+00033870: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+00033880: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+00033890: 673d 2265 6e5f 5553 223e 5354 4f20 636f  g="en_US">STO co
+000338a0: 6e66 6967 7572 6174 696f 6e3c 2f4c 6162  nfiguration</Lab
+000338b0: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+000338c0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+000338d0: 2020 3c2f 5265 6769 7374 6572 3e0d 0a20    </Register>.. 
+000338e0: 2020 2020 2020 203c 5265 6769 7374 6572         <Register
+000338f0: 2061 6363 6573 733d 2272 2220 6164 6472   access="r" addr
+00033900: 6573 735f 7479 7065 3d22 4e56 4d5f 4857  ess_type="NVM_HW
+00033910: 2220 6164 6472 6573 733d 2230 7830 3734  " address="0x074
+00033920: 3122 2064 7479 7065 3d22 7533 3222 2069  1" dtype="u32" i
+00033930: 643d 224d 4f54 5f42 5241 4b45 5f43 4f4e  d="MOT_BRAKE_CON
+00033940: 4649 4755 5241 5449 4f4e 2220 756e 6974  FIGURATION" unit
+00033950: 733d 222d 2220 7375 626e 6f64 653d 2231  s="-" subnode="1
+00033960: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
+00033970: 2220 6465 7363 3d22 496e 6469 6361 7465  " desc="Indicate
+00033980: 7320 7468 6520 4750 4f20 7573 6564 2061  s the GPO used a
+00033990: 7320 6272 616b 652e 2220 6361 745f 6964  s brake." cat_id
+000339a0: 3d22 494e 5445 524e 414c 223e 0d0a 2020  ="INTERNAL">..  
+000339b0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+000339c0: 0d0a 2020 2020 2020 2020 2020 2020 3c4c  ..            <L
+000339d0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+000339e0: 223e 4272 616b 6520 636f 6e66 6967 7572  ">Brake configur
+000339f0: 6174 696f 6e3c 2f4c 6162 656c 3e0d 0a20  ation</Label>.. 
+00033a00: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00033a10: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00033a20: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00033a30: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00033a40: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00033a50: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00033a60: 6573 733d 2230 7830 3734 3222 2064 7479  ess="0x0742" dty
+00033a70: 7065 3d22 7533 3222 2069 643d 224d 4f54  pe="u32" id="MOT
+00033a80: 5f42 5241 4b45 5f4d 4158 5f46 5245 5122  _BRAKE_MAX_FREQ"
+00033a90: 2075 6e69 7473 3d22 487a 2220 7375 626e   units="Hz" subn
+00033aa0: 6f64 653d 2231 2220 6379 636c 6963 3d22  ode="1" cyclic="
+00033ab0: 434f 4e46 4947 2220 6465 7363 3d22 496e  CONFIG" desc="In
+00033ac0: 6469 6361 7465 7320 7468 6520 6d61 7869  dicates the maxi
+00033ad0: 6d75 6d20 616c 6c6f 7765 6420 636f 6d6d  mum allowed comm
+00033ae0: 7574 6174 696f 6e20 6672 6571 7565 6e63  utation frequenc
+00033af0: 7920 6279 2074 6865 2062 7261 6b65 2065  y by the brake e
+00033b00: 6c65 6374 726f 6e69 6373 2220 6361 745f  lectronics" cat_
+00033b10: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+00033b20: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00033b30: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00033b40: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00033b50: 5553 223e 4272 616b 6520 6d61 782e 2066  US">Brake max. f
+00033b60: 7265 7175 656e 6379 3c2f 4c61 6265 6c3e  requency</Label>
+00033b70: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+00033b80: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+00033b90: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+00033ba0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+00033bb0: 6365 7373 3d22 7277 2220 6164 6472 6573  cess="rw" addres
+00033bc0: 735f 7479 7065 3d22 4e56 4d5f 4346 4722  s_type="NVM_CFG"
+00033bd0: 2061 6464 7265 7373 3d22 3078 3037 3433   address="0x0743
+00033be0: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
+00033bf0: 3d22 4d4f 545f 4252 414b 455f 4652 4551  ="MOT_BRAKE_FREQ
+00033c00: 2220 756e 6974 733d 2248 7a22 2073 7562  " units="Hz" sub
+00033c10: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
+00033c20: 2243 4f4e 4649 4722 2064 6573 633d 2242  "CONFIG" desc="B
+00033c30: 7261 6b65 2066 7265 7175 656e 6379 2069  rake frequency i
+00033c40: 6e20 6865 7274 7a2e 204f 6e6c 7920 7661  n hertz. Only va
+00033c50: 6c75 6573 206c 6f77 6572 2074 6861 6e20  lues lower than 
+00033c60: 7468 6520 6d61 7869 6d75 6d20 6272 616b  the maximum brak
+00033c70: 6520 6672 6571 7565 6e63 7920 7769 6c6c  e frequency will
+00033c80: 2062 6520 616c 6c6f 7765 642e 2056 616c   be allowed. Val
+00033c90: 7565 2030 2064 6973 6162 6c65 7320 6d6f  ue 0 disables mo
+00033ca0: 6475 6c61 7465 6420 6272 616b 6520 6f75  dulated brake ou
+00033cb0: 7470 7574 2e22 2063 6174 5f69 643d 224d  tput." cat_id="M
+00033cc0: 4f54 4f52 223e 0d0a 2020 2020 2020 2020  OTOR">..        
+00033cd0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
+00033ce0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+00033cf0: 616e 673d 2265 6e5f 5553 223e 4272 616b  ang="en_US">Brak
+00033d00: 6520 6672 6571 7565 6e63 793c 2f4c 6162  e frequency</Lab
+00033d10: 656c 3e0d 0a20 2020 2020 2020 2020 203c  el>..          <
+00033d20: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00033d30: 2020 2020 3c52 616e 6765 206d 696e 3d22      <Range min="
+00033d40: 3430 3030 2220 6d61 783d 2234 3030 3030  4000" max="40000
+00033d50: 222f 3e0d 0a20 2020 2020 2020 203c 2f52  "/>..        </R
+00033d60: 6567 6973 7465 723e 0d0a 2020 2020 2020  egister>..      
+00033d70: 2020 3c52 6567 6973 7465 7220 6163 6365    <Register acce
+00033d80: 7373 3d22 7222 2061 6464 7265 7373 5f74  ss="r" address_t
+00033d90: 7970 653d 224e 564d 5f48 5722 2061 6464  ype="NVM_HW" add
+00033da0: 7265 7373 3d22 3078 3037 3436 2220 6474  ress="0x0746" dt
+00033db0: 7970 653d 2275 3136 2220 6964 3d22 4452  ype="u16" id="DR
+00033dc0: 565f 5052 4f54 5f52 4544 5f54 454d 505f  V_PROT_RED_TEMP_
+00033dd0: 5459 5045 2220 756e 6974 733d 222d 2220  TYPE" units="-" 
+00033de0: 7375 626e 6f64 653d 2231 2220 6379 636c  subnode="1" cycl
+00033df0: 6963 3d22 434f 4e46 4947 2220 6465 7363  ic="CONFIG" desc
+00033e00: 3d22 496e 6469 6361 7465 7320 7468 6520  ="Indicates the 
+00033e10: 7479 7065 206f 6620 7465 6d70 6572 6174  type of temperat
+00033e20: 7572 6520 7365 6e73 6f72 2069 7320 7573  ure sensor is us
+00033e30: 6564 2066 6f72 2074 6865 2072 6564 756e  ed for the redun
+00033e40: 6461 6e74 2074 656d 7065 7261 7475 7265  dant temperature
+00033e50: 2073 656e 736f 7220 7479 7065 2220 6361   sensor type" ca
+00033e60: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
+00033e70: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00033e80: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00033e90: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00033ea0: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
+00033eb0: 6520 7465 6d70 2e20 7365 6e73 6f72 2032  e temp. sensor 2
+00033ec0: 2074 7970 653c 2f4c 6162 656c 3e0d 0a20   type</Label>.. 
+00033ed0: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00033ee0: 733e 0d0a 2020 2020 2020 2020 2020 3c45  s>..          <E
+00033ef0: 6e75 6d65 7261 7469 6f6e 733e 0d0a 2020  numerations>..  
+00033f00: 2020 2020 2020 2020 2020 3c45 6e75 6d20            <Enum 
+00033f10: 7661 6c75 653d 2230 223e 4e54 433c 2f45  value="0">NTC</E
+00033f20: 6e75 6d3e 0d0a 2020 2020 2020 2020 2020  num>..          
+00033f30: 2020 3c45 6e75 6d20 7661 6c75 653d 2231    <Enum value="1
+00033f40: 223e 5054 433c 2f45 6e75 6d3e 0d0a 2020  ">PTC</Enum>..  
+00033f50: 2020 2020 2020 2020 2020 3c45 6e75 6d20            <Enum 
+00033f60: 7661 6c75 653d 2232 223e 4c69 6e65 6172  value="2">Linear
+00033f70: 2073 656e 736f 723c 2f45 6e75 6d3e 0d0a   sensor</Enum>..
+00033f80: 2020 2020 2020 2020 2020 3c2f 456e 756d            </Enum
+00033f90: 6572 6174 696f 6e73 3e0d 0a20 2020 2020  erations>..     
+00033fa0: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+00033fb0: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+00033fc0: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+00033fd0: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
+00033fe0: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
+00033ff0: 3437 2220 6474 7970 653d 2275 3332 2220  47" dtype="u32" 
+00034000: 6964 3d22 4452 565f 5052 4f54 5f52 4544  id="DRV_PROT_RED
+00034010: 5f54 454d 505f 5245 5322 2075 6e69 7473  _TEMP_RES" units
+00034020: 3d22 cea9 2220 7375 626e 6f64 653d 2231  =".." subnode="1
+00034030: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
+00034040: 2220 6465 7363 3d22 4e54 433a 2052 6573  " desc="NTC: Res
+00034050: 6973 7461 6e63 6520 7661 6c75 6520 666f  istance value fo
+00034060: 7220 3235 20c2 ba43 2069 6e20 6f68 6d73  r 25 ..C in ohms
+00034070: 2623 3133 3b26 2331 303b 5054 433a 2052  &#13;&#10;PTC: R
+00034080: 6573 6973 7461 6e63 6520 7661 6c75 6520  esistance value 
+00034090: 696e 206f 686d 7320 7768 6572 6520 7468  in ohms where th
+000340a0: 6520 6f76 6572 2d74 656d 7065 7261 7475  e over-temperatu
+000340b0: 7265 206d 7573 7420 6265 2064 6574 6563  re must be detec
+000340c0: 7465 6426 2331 333b 2623 3130 3b4f 7468  ted&#13;&#10;Oth
+000340d0: 6572 733a 204e 6f74 2075 7365 6422 2063  ers: Not used" c
+000340e0: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+000340f0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00034100: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00034110: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00034120: 656e 5f55 5322 3e50 6f77 6572 2073 7461  en_US">Power sta
+00034130: 6765 2074 656d 702e 2073 656e 736f 7220  ge temp. sensor 
+00034140: 3220 7265 7369 7374 616e 6365 3c2f 4c61  2 resistance</La
+00034150: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
+00034160: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00034170: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+00034180: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+00034190: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+000341a0: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
+000341b0: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
+000341c0: 3438 2220 6474 7970 653d 2275 3136 2220  48" dtype="u16" 
+000341d0: 6964 3d22 4452 565f 5052 4f54 5f52 4544  id="DRV_PROT_RED
+000341e0: 5f54 454d 505f 4232 3538 3522 2075 6e69  _TEMP_B2585" uni
+000341f0: 7473 3d22 c2ba 4b22 2073 7562 6e6f 6465  ts="..K" subnode
+00034200: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+00034210: 4649 4722 2064 6573 633d 224e 5443 3a20  FIG" desc="NTC: 
+00034220: 4228 3235 2f38 3529 2070 6172 616d 6574  B(25/85) paramet
+00034230: 6572 2066 726f 6d20 6461 7461 7368 6565  er from datashee
+00034240: 7426 2331 333b 2623 3130 3b50 5443 3a20  t&#13;&#10;PTC: 
+00034250: 4e6f 7420 7573 6564 2623 3133 3b26 2331  Not used&#13;&#1
+00034260: 303b 4f74 6865 723a 204e 6f74 2075 7365  0;Other: Not use
+00034270: 6422 2063 6174 5f69 643d 2249 4e54 4552  d" cat_id="INTER
+00034280: 4e41 4c22 3e0d 0a20 2020 2020 2020 2020  NAL">..         
+00034290: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+000342a0: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+000342b0: 6e67 3d22 656e 5f55 5322 3e50 6f77 6572  ng="en_US">Power
+000342c0: 2073 7461 6765 2074 656d 702e 2073 656e   stage temp. sen
+000342d0: 736f 7220 3220 ceb2 3c2f 4c61 6265 6c3e  sor 2 ..</Label>
+000342e0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+000342f0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+00034300: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+00034310: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+00034320: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
+00034330: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
+00034340: 6464 7265 7373 3d22 3078 3037 3439 2220  ddress="0x0749" 
+00034350: 6474 7970 653d 2275 3332 2220 6964 3d22  dtype="u32" id="
+00034360: 4452 565f 5052 4f54 5f52 4544 5f54 454d  DRV_PROT_RED_TEM
+00034370: 505f 4558 545f 5245 5322 2075 6e69 7473  P_EXT_RES" units
+00034380: 3d22 cea9 2220 7375 626e 6f64 653d 2231  =".." subnode="1
+00034390: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
+000343a0: 2220 6465 7363 3d22 4e54 4320 2661 6d70  " desc="NTC &amp
+000343b0: 3b61 6d70 3b20 5054 433a 2052 6573 6973  ;amp; PTC: Resis
+000343c0: 7461 6e63 6520 7661 6c75 6520 696e 206f  tance value in o
+000343d0: 686d 7320 636f 6e6e 6563 7465 6420 746f  hms connected to
+000343e0: 2074 6865 2073 656e 736f 7220 666f 7220   the sensor for 
+000343f0: 6d61 6b69 6e67 2074 6865 2076 6f6c 7461  making the volta
+00034400: 6765 2064 6976 6964 6572 2623 3133 3b26  ge divider&#13;&
+00034410: 2331 303b 4f74 6865 7273 3a20 4e6f 7420  #10;Others: Not 
+00034420: 7573 6564 2220 6361 745f 6964 3d22 494e  used" cat_id="IN
+00034430: 5445 524e 414c 223e 0d0a 2020 2020 2020  TERNAL">..      
+00034440: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+00034450: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00034460: 206c 616e 673d 2265 6e5f 5553 223e 506f   lang="en_US">Po
+00034470: 7765 7220 7374 6167 6520 7465 6d70 2e20  wer stage temp. 
+00034480: 7365 6e73 6f72 2032 2065 7874 2e20 7265  sensor 2 ext. re
+00034490: 7369 7374 616e 6365 3c2f 4c61 6265 6c3e  sistance</Label>
+000344a0: 0d0a 2020 2020 2020 2020 2020 3c2f 4c61  ..          </La
+000344b0: 6265 6c73 3e0d 0a20 2020 2020 2020 203c  bels>..        <
+000344c0: 2f52 6567 6973 7465 723e 0d0a 2020 2020  /Register>..    
+000344d0: 2020 2020 3c52 6567 6973 7465 7220 6163      <Register ac
+000344e0: 6365 7373 3d22 7222 2061 6464 7265 7373  cess="r" address
+000344f0: 5f74 7970 653d 224e 564d 5f48 5722 2061  _type="NVM_HW" a
+00034500: 6464 7265 7373 3d22 3078 3037 3441 2220  ddress="0x074A" 
+00034510: 6474 7970 653d 2266 6c6f 6174 2220 6964  dtype="float" id
+00034520: 3d22 4452 565f 5052 4f54 5f52 4544 5f54  ="DRV_PROT_RED_T
+00034530: 454d 505f 4741 494e 2220 756e 6974 733d  EMP_GAIN" units=
+00034540: 22c2 ba43 202f 2056 2220 7375 626e 6f64  "..C / V" subnod
+00034550: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+00034560: 4e46 4947 2220 6465 7363 3d22 4c69 6e65  NFIG" desc="Line
+00034570: 6172 2076 6f6c 7461 6765 2073 656e 736f  ar voltage senso
+00034580: 723a 2047 6169 6e20 6f66 2074 6865 2073  r: Gain of the s
+00034590: 656e 736f 722e 2623 3133 3b26 2331 303b  ensor.&#13;&#10;
+000345a0: 4f74 6865 7273 3a20 4e6f 7420 7573 6564  Others: Not used
+000345b0: 2220 6361 745f 6964 3d22 494e 5445 524e  " cat_id="INTERN
+000345c0: 414c 223e 0d0a 2020 2020 2020 2020 2020  AL">..          
+000345d0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+000345e0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+000345f0: 673d 2265 6e5f 5553 223e 506f 7765 7220  g="en_US">Power 
+00034600: 7374 6167 6520 7465 6d70 2e20 7365 6e73  stage temp. sens
+00034610: 6f72 2032 2067 6169 6e3c 2f4c 6162 656c  or 2 gain</Label
+00034620: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
+00034630: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00034640: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
+00034650: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
+00034660: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
+00034670: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
+00034680: 6164 6472 6573 733d 2230 7830 3734 4222  address="0x074B"
+00034690: 2064 7479 7065 3d22 666c 6f61 7422 2069   dtype="float" i
+000346a0: 643d 2244 5256 5f50 524f 545f 5245 445f  d="DRV_PROT_RED_
+000346b0: 5445 4d50 5f4f 4646 5345 5422 2075 6e69  TEMP_OFFSET" uni
+000346c0: 7473 3d22 c2ba 4322 2073 7562 6e6f 6465  ts="..C" subnode
+000346d0: 3d22 3122 2063 7963 6c69 633d 2243 4f4e  ="1" cyclic="CON
+000346e0: 4649 4722 2064 6573 633d 224e 5443 2026  FIG" desc="NTC &
+000346f0: 616d 703b 616d 703b 2050 5443 3a20 4e6f  amp;amp; PTC: No
+00034700: 7420 7573 6564 2623 3133 3b26 2331 303b  t used&#13;&#10;
+00034710: 4f74 6865 7273 3a20 4f66 6673 6574 206f  Others: Offset o
+00034720: 6620 7468 6520 7365 6e73 6f72 2220 6361  f the sensor" ca
+00034730: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
+00034740: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00034750: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00034760: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00034770: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
+00034780: 6520 7465 6d70 2e20 7365 6e73 6f72 2032  e temp. sensor 2
+00034790: 206f 6666 7365 743c 2f4c 6162 656c 3e0d   offset</Label>.
+000347a0: 0a20 2020 2020 2020 2020 203c 2f4c 6162  .          </Lab
+000347b0: 656c 733e 0d0a 2020 2020 2020 2020 3c2f  els>..        </
+000347c0: 5265 6769 7374 6572 3e0d 0a20 2020 2020  Register>..     
+000347d0: 2020 203c 5265 6769 7374 6572 2061 6363     <Register acc
+000347e0: 6573 733d 2272 2220 6164 6472 6573 735f  ess="r" address_
+000347f0: 7479 7065 3d22 4e56 4d5f 4857 2220 6164  type="NVM_HW" ad
+00034800: 6472 6573 733d 2230 7830 3735 3022 2064  dress="0x0750" d
+00034810: 7479 7065 3d22 666c 6f61 7422 2069 643d  type="float" id=
+00034820: 2244 5256 5f50 524f 545f 4445 5241 5449  "DRV_PROT_DERATI
+00034830: 4e47 5f43 4f4e 5354 2220 756e 6974 733d  NG_CONST" units=
+00034840: 222d 2220 7375 626e 6f64 653d 2231 2220  "-" subnode="1" 
+00034850: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+00034860: 6465 7363 3d22 436f 6e73 7461 6e74 2061  desc="Constant a
+00034870: 7070 6c69 6564 2069 6e20 6675 6e63 7469  pplied in functi
+00034880: 6f6e 206f 6620 7468 6520 6472 6976 6520  on of the drive 
+00034890: 7465 6d70 6572 6174 7572 6520 746f 2074  temperature to t
+000348a0: 6865 206d 6178 696d 756d 206e 6f6d 696e  he maximum nomin
+000348b0: 616c 2063 7572 7265 6e74 2220 6361 745f  al current" cat_
+000348c0: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+000348d0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+000348e0: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+000348f0: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00034900: 5553 223e 4465 7261 7469 6e67 2063 6f6e  US">Derating con
+00034910: 7374 616e 743c 2f4c 6162 656c 3e0d 0a20  stant</Label>.. 
+00034920: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00034930: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00034940: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00034950: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00034960: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00034970: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00034980: 6573 733d 2230 7830 3735 3122 2064 7479  ess="0x0751" dty
+00034990: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
+000349a0: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
+000349b0: 5f46 5245 515f 434f 4e53 5431 2220 756e  _FREQ_CONST1" un
+000349c0: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
+000349d0: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+000349e0: 4947 2220 6465 7363 3d22 4465 7261 7469  IG" desc="Derati
+000349f0: 6e67 2063 6f6e 7374 616e 7420 666f 7220  ng constant for 
+00034a00: 636f 6d6d 7574 6174 696f 6e20 6672 6571  commutation freq
+00034a10: 7565 6e63 7920 3120 7468 6174 206d 6f64  uency 1 that mod
+00034a20: 6966 6965 7320 7468 6520 7465 6d70 6572  ifies the temper
+00034a30: 6174 7572 6520 7468 7265 7368 6f6c 6420  ature threshold 
+00034a40: 666f 7220 7374 6172 7469 6e67 2063 7572  for starting cur
+00034a50: 7265 6e74 2064 6572 6174 696e 672e 2220  rent derating." 
+00034a60: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00034a70: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00034a80: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00034a90: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00034aa0: 2265 6e5f 5553 223e 4672 6571 7565 6e63  "en_US">Frequenc
+00034ab0: 7920 3120 6465 7261 7469 6e67 2063 6f6e  y 1 derating con
+00034ac0: 7374 616e 743c 2f4c 6162 656c 3e0d 0a20  stant</Label>.. 
+00034ad0: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00034ae0: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00034af0: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00034b00: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00034b10: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00034b20: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00034b30: 6573 733d 2230 7830 3735 3222 2064 7479  ess="0x0752" dty
+00034b40: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
+00034b50: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
+00034b60: 5f46 5245 515f 434f 4e53 5432 2220 756e  _FREQ_CONST2" un
+00034b70: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
+00034b80: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+00034b90: 4947 2220 6465 7363 3d22 4465 7261 7469  IG" desc="Derati
+00034ba0: 6e67 2063 6f6e 7374 616e 7420 666f 7220  ng constant for 
+00034bb0: 636f 6d6d 7574 6174 696f 6e20 6672 6571  commutation freq
+00034bc0: 7565 6e63 7920 3220 7468 6174 206d 6f64  uency 2 that mod
+00034bd0: 6966 6965 7320 7468 6520 7465 6d70 6572  ifies the temper
+00034be0: 6174 7572 6520 7468 7265 7368 6f6c 6420  ature threshold 
+00034bf0: 666f 7220 7374 6172 7469 6e67 2063 7572  for starting cur
+00034c00: 7265 6e74 2064 6572 6174 696e 672e 2220  rent derating." 
+00034c10: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00034c20: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00034c30: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00034c40: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00034c50: 2265 6e5f 5553 223e 4672 6571 7565 6e63  "en_US">Frequenc
+00034c60: 7920 3220 6465 7261 7469 6e67 2063 6f6e  y 2 derating con
+00034c70: 7374 616e 743c 2f4c 6162 656c 3e0d 0a20  stant</Label>.. 
+00034c80: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00034c90: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00034ca0: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00034cb0: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00034cc0: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00034cd0: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00034ce0: 6573 733d 2230 7830 3735 3322 2064 7479  ess="0x0753" dty
+00034cf0: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
+00034d00: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
+00034d10: 5f46 5245 515f 434f 4e53 5433 2220 756e  _FREQ_CONST3" un
+00034d20: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
+00034d30: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+00034d40: 4947 2220 6465 7363 3d22 4465 7261 7469  IG" desc="Derati
+00034d50: 6e67 2063 6f6e 7374 616e 7420 666f 7220  ng constant for 
+00034d60: 636f 6d6d 7574 6174 696f 6e20 6672 6571  commutation freq
+00034d70: 7565 6e63 7920 3320 7468 6174 206d 6f64  uency 3 that mod
+00034d80: 6966 6965 7320 7468 6520 7465 6d70 6572  ifies the temper
+00034d90: 6174 7572 6520 7468 7265 7368 6f6c 6420  ature threshold 
+00034da0: 666f 7220 7374 6172 7469 6e67 2063 7572  for starting cur
+00034db0: 7265 6e74 2064 6572 6174 696e 672e 2220  rent derating." 
+00034dc0: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00034dd0: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00034de0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00034df0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00034e00: 2265 6e5f 5553 223e 4672 6571 7565 6e63  "en_US">Frequenc
+00034e10: 7920 3320 6465 7261 7469 6e67 2063 6f6e  y 3 derating con
+00034e20: 7374 616e 743c 2f4c 6162 656c 3e0d 0a20  stant</Label>.. 
+00034e30: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00034e40: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00034e50: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00034e60: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00034e70: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00034e80: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00034e90: 6573 733d 2230 7830 3735 3422 2064 7479  ess="0x0754" dty
+00034ea0: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
+00034eb0: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
+00034ec0: 5f46 5245 515f 434f 4e53 5434 2220 756e  _FREQ_CONST4" un
+00034ed0: 6974 733d 222d 2220 7375 626e 6f64 653d  its="-" subnode=
+00034ee0: 2231 2220 6379 636c 6963 3d22 434f 4e46  "1" cyclic="CONF
+00034ef0: 4947 2220 6465 7363 3d22 4465 7261 7469  IG" desc="Derati
+00034f00: 6e67 2063 6f6e 7374 616e 7420 666f 7220  ng constant for 
+00034f10: 636f 6d6d 7574 6174 696f 6e20 6672 6571  commutation freq
+00034f20: 7565 6e63 7920 3420 7468 6174 206d 6f64  uency 4 that mod
+00034f30: 6966 6965 7320 7468 6520 7465 6d70 6572  ifies the temper
+00034f40: 6174 7572 6520 7468 7265 7368 6f6c 6420  ature threshold 
+00034f50: 666f 7220 7374 6172 7469 6e67 2063 7572  for starting cur
+00034f60: 7265 6e74 2064 6572 6174 696e 672e 2220  rent derating." 
+00034f70: 6361 745f 6964 3d22 494e 5445 524e 414c  cat_id="INTERNAL
+00034f80: 223e 0d0a 2020 2020 2020 2020 2020 3c4c  ">..          <L
+00034f90: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00034fa0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00034fb0: 2265 6e5f 5553 223e 4672 6571 7565 6e63  "en_US">Frequenc
+00034fc0: 7920 3420 6465 7261 7469 6e67 2063 6f6e  y 4 derating con
+00034fd0: 7374 616e 743c 2f4c 6162 656c 3e0d 0a20  stant</Label>.. 
+00034fe0: 2020 2020 2020 2020 203c 2f4c 6162 656c           </Label
+00034ff0: 733e 0d0a 2020 2020 2020 2020 3c2f 5265  s>..        </Re
+00035000: 6769 7374 6572 3e0d 0a20 2020 2020 2020  gister>..       
+00035010: 203c 5265 6769 7374 6572 2061 6363 6573   <Register acces
+00035020: 733d 2272 2220 6164 6472 6573 735f 7479  s="r" address_ty
+00035030: 7065 3d22 4e56 4d5f 4857 2220 6164 6472  pe="NVM_HW" addr
+00035040: 6573 733d 2230 7830 3735 4122 2064 7479  ess="0x075A" dty
+00035050: 7065 3d22 666c 6f61 7422 2069 643d 2244  pe="float" id="D
+00035060: 5256 5f50 524f 545f 4445 5241 5449 4e47  RV_PROT_DERATING
+00035070: 5f54 454d 505f 5448 5245 5348 4f4c 445f  _TEMP_THRESHOLD_
+00035080: 3122 2075 6e69 7473 3d22 4122 2073 7562  1" units="A" sub
+00035090: 6e6f 6465 3d22 3122 2063 7963 6c69 633d  node="1" cyclic=
+000350a0: 2243 4f4e 4649 4722 2064 6573 633d 2254  "CONFIG" desc="T
+000350b0: 6872 6573 686f 6c64 2074 656d 7065 7261  hreshold tempera
+000350c0: 7475 7265 2074 6861 7420 7374 6172 7473  ture that starts
+000350d0: 2074 6865 2064 6572 6174 696e 6720 616c   the derating al
+000350e0: 676f 7269 7468 6d20 666f 7220 7365 6c65  gorithm for sele
+000350f0: 6374 6162 6c65 2066 7265 7175 656e 6379  ctable frequency
+00035100: 2031 2061 7420 6d69 6e69 6d75 6d20 7375   1 at minimum su
+00035110: 7070 6c79 2076 6f6c 7461 6765 2220 6361  pply voltage" ca
+00035120: 745f 6964 3d22 494e 5445 524e 414c 223e  t_id="INTERNAL">
+00035130: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00035140: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00035150: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00035160: 6e5f 5553 223e 506f 7765 7220 7374 6167  n_US">Power stag
+00035170: 6520 6465 7261 7469 6e67 2074 656d 7065  e derating tempe
+00035180: 7261 7475 7265 2074 6872 6573 686f 6c64  rature threshold
+00035190: 2031 3c2f 4c61 6265 6c3e 0d0a 2020 2020   1</Label>..    
+000351a0: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+000351b0: 0a20 2020 2020 2020 203c 2f52 6567 6973  .        </Regis
+000351c0: 7465 723e 0d0a 2020 2020 2020 2020 3c52  ter>..        <R
+000351d0: 6567 6973 7465 7220 6163 6365 7373 3d22  egister access="
+000351e0: 7222 2061 6464 7265 7373 5f74 7970 653d  r" address_type=
+000351f0: 224e 564d 5f48 5722 2061 6464 7265 7373  "NVM_HW" address
+00035200: 3d22 3078 3037 3542 2220 6474 7970 653d  ="0x075B" dtype=
+00035210: 2266 6c6f 6174 2220 6964 3d22 4452 565f  "float" id="DRV_
+00035220: 5052 4f54 5f44 4552 4154 494e 475f 5445  PROT_DERATING_TE
+00035230: 4d50 5f54 4852 4553 484f 4c44 5f32 2220  MP_THRESHOLD_2" 
+00035240: 756e 6974 733d 2241 2220 7375 626e 6f64  units="A" subnod
+00035250: 653d 2231 2220 6379 636c 6963 3d22 434f  e="1" cyclic="CO
+00035260: 4e46 4947 2220 6465 7363 3d22 5468 7265  NFIG" desc="Thre
+00035270: 7368 6f6c 6420 7465 6d70 6572 6174 7572  shold temperatur
+00035280: 6520 7468 6174 2073 7461 7274 7320 7468  e that starts th
+00035290: 6520 6465 7261 7469 6e67 2061 6c67 6f72  e derating algor
+000352a0: 6974 686d 2066 6f72 2073 656c 6563 7461  ithm for selecta
+000352b0: 626c 6520 6672 6571 7565 6e63 7920 3220  ble frequency 2 
+000352c0: 6174 206d 696e 696d 756d 2073 7570 706c  at minimum suppl
+000352d0: 7920 766f 6c74 6167 6522 2063 6174 5f69  y voltage" cat_i
+000352e0: 643d 2249 4e54 4552 4e41 4c22 3e0d 0a20  d="INTERNAL">.. 
+000352f0: 2020 2020 2020 2020 203c 4c61 6265 6c73           <Labels
+00035300: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00035310: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+00035320: 5322 3e50 6f77 6572 2073 7461 6765 2064  S">Power stage d
+00035330: 6572 6174 696e 6720 7465 6d70 6572 6174  erating temperat
+00035340: 7572 6520 7468 7265 7368 6f6c 6420 323c  ure threshold 2<
+00035350: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+00035360: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+00035370: 2020 2020 2020 3c2f 5265 6769 7374 6572        </Register
+00035380: 3e0d 0a20 2020 2020 2020 203c 5265 6769  >..        <Regi
+00035390: 7374 6572 2061 6363 6573 733d 2272 2220  ster access="r" 
+000353a0: 6164 6472 6573 735f 7479 7065 3d22 4e56  address_type="NV
+000353b0: 4d5f 4857 2220 6164 6472 6573 733d 2230  M_HW" address="0
+000353c0: 7830 3735 4322 2064 7479 7065 3d22 666c  x075C" dtype="fl
+000353d0: 6f61 7422 2069 643d 2244 5256 5f50 524f  oat" id="DRV_PRO
+000353e0: 545f 4445 5241 5449 4e47 5f54 454d 505f  T_DERATING_TEMP_
+000353f0: 5448 5245 5348 4f4c 445f 3322 2075 6e69  THRESHOLD_3" uni
+00035400: 7473 3d22 4122 2073 7562 6e6f 6465 3d22  ts="A" subnode="
+00035410: 3122 2063 7963 6c69 633d 2243 4f4e 4649  1" cyclic="CONFI
+00035420: 4722 2064 6573 633d 2254 6872 6573 686f  G" desc="Thresho
+00035430: 6c64 2074 656d 7065 7261 7475 7265 2074  ld temperature t
+00035440: 6861 7420 7374 6172 7473 2074 6865 2064  hat starts the d
+00035450: 6572 6174 696e 6720 616c 676f 7269 7468  erating algorith
+00035460: 6d20 666f 7220 7365 6c65 6374 6162 6c65  m for selectable
+00035470: 2066 7265 7175 656e 6379 2033 2061 7420   frequency 3 at 
+00035480: 6d69 6e69 6d75 6d20 7375 7070 6c79 2076  minimum supply v
+00035490: 6f6c 7461 6765 2220 6361 745f 6964 3d22  oltage" cat_id="
+000354a0: 494e 5445 524e 414c 223e 0d0a 2020 2020  INTERNAL">..    
+000354b0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+000354c0: 2020 2020 2020 2020 2020 2020 3c4c 6162              <Lab
+000354d0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+000354e0: 506f 7765 7220 7374 6167 6520 6465 7261  Power stage dera
+000354f0: 7469 6e67 2074 656d 7065 7261 7475 7265  ting temperature
+00035500: 2074 6872 6573 686f 6c64 2033 3c2f 4c61   threshold 3</La
+00035510: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
+00035520: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00035530: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+00035540: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+00035550: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+00035560: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
+00035570: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
+00035580: 3544 2220 6474 7970 653d 2266 6c6f 6174  5D" dtype="float
+00035590: 2220 6964 3d22 4452 565f 5052 4f54 5f44  " id="DRV_PROT_D
+000355a0: 4552 4154 494e 475f 5445 4d50 5f54 4852  ERATING_TEMP_THR
+000355b0: 4553 484f 4c44 5f34 2220 756e 6974 733d  ESHOLD_4" units=
+000355c0: 2241 2220 7375 626e 6f64 653d 2231 2220  "A" subnode="1" 
+000355d0: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+000355e0: 6465 7363 3d22 5468 7265 7368 6f6c 6420  desc="Threshold 
+000355f0: 7465 6d70 6572 6174 7572 6520 7468 6174  temperature that
+00035600: 2073 7461 7274 7320 7468 6520 6465 7261   starts the dera
+00035610: 7469 6e67 2061 6c67 6f72 6974 686d 2066  ting algorithm f
+00035620: 6f72 2073 656c 6563 7461 626c 6520 6672  or selectable fr
+00035630: 6571 7565 6e63 7920 3420 6174 206d 696e  equency 4 at min
+00035640: 696d 756d 2073 7570 706c 7920 766f 6c74  imum supply volt
+00035650: 6167 6522 2063 6174 5f69 643d 2249 4e54  age" cat_id="INT
+00035660: 4552 4e41 4c22 3e0d 0a20 2020 2020 2020  ERNAL">..       
+00035670: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00035680: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00035690: 6c61 6e67 3d22 656e 5f55 5322 3e50 6f77  lang="en_US">Pow
+000356a0: 6572 2073 7461 6765 2064 6572 6174 696e  er stage deratin
+000356b0: 6720 7465 6d70 6572 6174 7572 6520 7468  g temperature th
+000356c0: 7265 7368 6f6c 6420 343c 2f4c 6162 656c  reshold 4</Label
+000356d0: 3e0d 0a20 2020 2020 2020 2020 203c 2f4c  >..          </L
+000356e0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+000356f0: 3c2f 5265 6769 7374 6572 3e0d 0a20 2020  </Register>..   
+00035700: 2020 2020 203c 5265 6769 7374 6572 2061       <Register a
+00035710: 6363 6573 733d 2272 2220 6164 6472 6573  ccess="r" addres
+00035720: 735f 7479 7065 3d22 4e56 4d5f 4857 2220  s_type="NVM_HW" 
+00035730: 6164 6472 6573 733d 2230 7830 3736 3022  address="0x0760"
+00035740: 2064 7479 7065 3d22 7531 3622 2069 643d   dtype="u16" id=
+00035750: 2244 5256 5f50 524f 545f 5448 4952 445f  "DRV_PROT_THIRD_
+00035760: 5445 4d50 5f54 5950 4522 2075 6e69 7473  TEMP_TYPE" units
+00035770: 3d22 2d22 2073 7562 6e6f 6465 3d22 3122  ="-" subnode="1"
+00035780: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00035790: 2064 6573 633d 2249 6e64 6963 6174 6573   desc="Indicates
+000357a0: 2074 6865 2074 656d 7065 7261 7475 7265   the temperature
+000357b0: 2073 656e 736f 7220 7573 6564 2066 6f72   sensor used for
+000357c0: 2070 7269 6d61 7279 2074 656d 7065 7261   primary tempera
+000357d0: 7475 7265 2072 6561 6469 6e67 7320 6f66  ture readings of
+000357e0: 2074 6865 2070 6f77 6572 2073 7461 6765   the power stage
+000357f0: 2e22 2063 6174 5f69 643d 2249 4e54 4552  ." cat_id="INTER
+00035800: 4e41 4c22 3e0d 0a20 2020 2020 2020 2020  NAL">..         
+00035810: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00035820: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00035830: 6e67 3d22 656e 5f55 5322 3e50 6f77 6572  ng="en_US">Power
+00035840: 2073 7461 6765 2074 656d 702e 2073 656e   stage temp. sen
+00035850: 736f 7220 3320 7479 7065 3c2f 4c61 6265  sor 3 type</Labe
+00035860: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00035870: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00035880: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+00035890: 2020 2020 2020 3c52 6567 6973 7465 7220        <Register 
+000358a0: 6163 6365 7373 3d22 7222 2061 6464 7265  access="r" addre
+000358b0: 7373 5f74 7970 653d 224e 564d 5f48 5722  ss_type="NVM_HW"
+000358c0: 2061 6464 7265 7373 3d22 3078 3037 3631   address="0x0761
+000358d0: 2220 6474 7970 653d 2275 3332 2220 6964  " dtype="u32" id
+000358e0: 3d22 4452 565f 5052 4f54 5f54 4849 5244  ="DRV_PROT_THIRD
+000358f0: 5f54 454d 505f 5245 5322 2075 6e69 7473  _TEMP_RES" units
+00035900: 3d22 cea9 2220 7375 626e 6f64 653d 2231  =".." subnode="1
+00035910: 2220 6379 636c 6963 3d22 434f 4e46 4947  " cyclic="CONFIG
+00035920: 2220 6465 7363 3d22 4e54 433a 2052 6573  " desc="NTC: Res
+00035930: 6973 7461 6e63 6520 7661 6c75 6520 666f  istance value fo
+00035940: 7220 3235 20c2 ba43 2069 6e20 6f68 6d73  r 25 ..C in ohms
+00035950: 2623 3133 3b26 2331 303b 5054 433a 2052  &#13;&#10;PTC: R
+00035960: 6573 6973 7461 6e63 6520 7661 6c75 6520  esistance value 
+00035970: 696e 206f 686d 7320 7768 6572 6520 7468  in ohms where th
+00035980: 6520 6f76 6572 2d74 656d 7065 7261 7475  e over-temperatu
+00035990: 7265 206d 7573 7420 6265 2064 6574 6563  re must be detec
+000359a0: 7465 6426 2331 333b 2623 3130 3b4f 7468  ted&#13;&#10;Oth
+000359b0: 6572 733a 204e 6f74 2075 7365 6422 2063  ers: Not used" c
+000359c0: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+000359d0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+000359e0: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+000359f0: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00035a00: 656e 5f55 5322 3e50 6f77 6572 2073 7461  en_US">Power sta
+00035a10: 6765 2074 656d 702e 2073 656e 736f 7220  ge temp. sensor 
+00035a20: 3320 7265 7369 7374 616e 6365 3c2f 4c61  3 resistance</La
+00035a30: 6265 6c3e 0d0a 2020 2020 2020 2020 2020  bel>..          
+00035a40: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00035a50: 2020 203c 2f52 6567 6973 7465 723e 0d0a     </Register>..
+00035a60: 2020 2020 2020 2020 3c52 6567 6973 7465          <Registe
+00035a70: 7220 6163 6365 7373 3d22 7222 2061 6464  r access="r" add
+00035a80: 7265 7373 5f74 7970 653d 224e 564d 5f48  ress_type="NVM_H
+00035a90: 5722 2061 6464 7265 7373 3d22 3078 3037  W" address="0x07
+00035aa0: 3632 2220 6474 7970 653d 2275 3136 2220  62" dtype="u16" 
+00035ab0: 6964 3d22 4452 565f 5052 4f54 5f54 4849  id="DRV_PROT_THI
+00035ac0: 5244 5f54 454d 505f 4232 3538 3522 2075  RD_TEMP_B2585" u
+00035ad0: 6e69 7473 3d22 c2ba 4b22 2073 7562 6e6f  nits="..K" subno
+00035ae0: 6465 3d22 3122 2063 7963 6c69 633d 2243  de="1" cyclic="C
+00035af0: 4f4e 4649 4722 2064 6573 633d 224e 5443  ONFIG" desc="NTC
+00035b00: 3a20 4228 3235 2f38 3529 2070 6172 616d  : B(25/85) param
+00035b10: 6574 6572 2066 726f 6d20 6461 7461 7368  eter from datash
+00035b20: 6565 7426 2331 333b 2623 3130 3b4f 7468  eet&#13;&#10;Oth
+00035b30: 6572 733a 204e 6f74 2075 7365 6422 2063  ers: Not used" c
+00035b40: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+00035b50: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00035b60: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00035b70: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00035b80: 656e 5f55 5322 3e50 6f77 6572 2073 7461  en_US">Power sta
+00035b90: 6765 2074 656d 702e 2073 656e 736f 7220  ge temp. sensor 
+00035ba0: 3320 ceb2 3c2f 4c61 6265 6c3e 0d0a 2020  3 ..</Label>..  
+00035bb0: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+00035bc0: 3e0d 0a20 2020 2020 2020 203c 2f52 6567  >..        </Reg
+00035bd0: 6973 7465 723e 0d0a 2020 2020 2020 2020  ister>..        
+00035be0: 3c52 6567 6973 7465 7220 6163 6365 7373  <Register access
+00035bf0: 3d22 7222 2061 6464 7265 7373 5f74 7970  ="r" address_typ
+00035c00: 653d 224e 564d 5f48 5722 2061 6464 7265  e="NVM_HW" addre
+00035c10: 7373 3d22 3078 3037 3633 2220 6474 7970  ss="0x0763" dtyp
+00035c20: 653d 2275 3332 2220 6964 3d22 4452 565f  e="u32" id="DRV_
+00035c30: 5052 4f54 5f54 4849 5244 5f54 454d 505f  PROT_THIRD_TEMP_
+00035c40: 4558 545f 5245 5322 2075 6e69 7473 3d22  EXT_RES" units="
+00035c50: cea9 2220 7375 626e 6f64 653d 2231 2220  .." subnode="1" 
+00035c60: 6379 636c 6963 3d22 434f 4e46 4947 2220  cyclic="CONFIG" 
+00035c70: 6465 7363 3d22 4e54 4320 2661 6d70 3b61  desc="NTC &amp;a
+00035c80: 6d70 3b20 5054 433a 2052 6573 6973 7461  mp; PTC: Resista
+00035c90: 6e63 6520 7661 6c75 6520 696e 206f 686d  nce value in ohm
+00035ca0: 7320 636f 6e6e 6563 7465 6420 746f 2073  s connected to s
+00035cb0: 656e 736f 7220 666f 7220 6d61 6b69 6e67  ensor for making
+00035cc0: 2074 6865 2076 6f6c 7461 6765 2064 6976   the voltage div
+00035cd0: 6964 6572 2623 3133 3b26 2331 303b 4f74  ider&#13;&#10;Ot
+00035ce0: 6865 723a 204e 6f74 2075 7365 6422 2063  her: Not used" c
+00035cf0: 6174 5f69 643d 2249 4e54 4552 4e41 4c22  at_id="INTERNAL"
+00035d00: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00035d10: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00035d20: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00035d30: 656e 5f55 5322 3e50 6f77 6572 2073 7461  en_US">Power sta
+00035d40: 6765 2074 656d 702e 2073 656e 736f 7220  ge temp. sensor 
+00035d50: 3320 6578 742e 2072 6573 6973 7461 6e63  3 ext. resistanc
+00035d60: 653c 2f4c 6162 656c 3e0d 0a20 2020 2020  e</Label>..     
+00035d70: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00035d80: 2020 2020 2020 2020 3c2f 5265 6769 7374          </Regist
+00035d90: 6572 3e0d 0a20 2020 2020 2020 203c 5265  er>..        <Re
+00035da0: 6769 7374 6572 2061 6363 6573 733d 2272  gister access="r
+00035db0: 2220 6164 6472 6573 735f 7479 7065 3d22  " address_type="
+00035dc0: 4e56 4d5f 4857 2220 6164 6472 6573 733d  NVM_HW" address=
+00035dd0: 2230 7830 3736 3422 2064 7479 7065 3d22  "0x0764" dtype="
+00035de0: 666c 6f61 7422 2069 643d 2244 5256 5f50  float" id="DRV_P
+00035df0: 524f 545f 5448 4952 445f 5445 4d50 5f47  ROT_THIRD_TEMP_G
+00035e00: 4149 4e22 2075 6e69 7473 3d22 c2ba 4320  AIN" units="..C 
+00035e10: 2f20 5622 2073 7562 6e6f 6465 3d22 3122  / V" subnode="1"
+00035e20: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00035e30: 2064 6573 633d 224c 696e 6561 7220 766f   desc="Linear vo
+00035e40: 6c74 6167 6520 7365 6e73 6f72 3a20 4761  ltage sensor: Ga
+00035e50: 696e 206f 6620 7468 6520 7365 6e73 6f72  in of the sensor
+00035e60: 2623 3133 3b26 2331 303b 4f74 6865 7273  &#13;&#10;Others
+00035e70: 3a20 4e6f 7420 7573 6564 2220 6361 745f  : Not used" cat_
+00035e80: 6964 3d22 494e 5445 524e 414c 223e 0d0a  id="INTERNAL">..
+00035e90: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00035ea0: 733e 0d0a 2020 2020 2020 2020 2020 2020  s>..            
+00035eb0: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00035ec0: 5553 223e 506f 7765 7220 7374 6167 6520  US">Power stage 
+00035ed0: 7465 6d70 2e20 7365 6e73 6f72 2033 2067  temp. sensor 3 g
+00035ee0: 6169 6e3c 2f4c 6162 656c 3e0d 0a20 2020  ain</Label>..   
+00035ef0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00035f00: 0d0a 2020 2020 2020 2020 3c2f 5265 6769  ..        </Regi
+00035f10: 7374 6572 3e0d 0a20 2020 2020 2020 203c  ster>..        <
+00035f20: 5265 6769 7374 6572 2061 6363 6573 733d  Register access=
+00035f30: 2272 2220 6164 6472 6573 735f 7479 7065  "r" address_type
+00035f40: 3d22 4e56 4d5f 4857 2220 6164 6472 6573  ="NVM_HW" addres
+00035f50: 733d 2230 7830 3736 3522 2064 7479 7065  s="0x0765" dtype
+00035f60: 3d22 666c 6f61 7422 2069 643d 2244 5256  ="float" id="DRV
+00035f70: 5f50 524f 545f 5448 4952 445f 5445 4d50  _PROT_THIRD_TEMP
+00035f80: 5f4f 4646 5345 5422 2075 6e69 7473 3d22  _OFFSET" units="
+00035f90: c2ba 4322 2073 7562 6e6f 6465 3d22 3122  ..C" subnode="1"
+00035fa0: 2063 7963 6c69 633d 2243 4f4e 4649 4722   cyclic="CONFIG"
+00035fb0: 2064 6573 633d 224e 5443 2026 616d 703b   desc="NTC &amp;
+00035fc0: 616d 703b 2050 5443 3a20 4e6f 7420 7573  amp; PTC: Not us
+00035fd0: 6564 2623 3133 3b26 2331 303b 4c69 6e65  ed&#13;&#10;Line
+00035fe0: 6172 2073 656e 736f 723a 204f 6666 7365  ar sensor: Offse
+00035ff0: 7420 6f66 2074 6865 2073 656e 736f 7222  t of the sensor"
+00036000: 2063 6174 5f69 643d 2249 4e54 4552 4e41   cat_id="INTERNA
+00036010: 4c22 3e0d 0a20 2020 2020 2020 2020 203c  L">..          <
+00036020: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00036030: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00036040: 3d22 656e 5f55 5322 3e50 6f77 6572 2073  ="en_US">Power s
+00036050: 7461 6765 2074 656d 702e 2073 656e 736f  tage temp. senso
+00036060: 7220 3320 6f66 6673 6574 3c2f 4c61 6265  r 3 offset</Labe
+00036070: 6c3e 0d0a 2020 2020 2020 2020 2020 3c2f  l>..          </
+00036080: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00036090: 203c 2f52 6567 6973 7465 723e 0d0a 2020   </Register>..  
+000360a0: 2020 2020 3c2f 5265 6769 7374 6572 733e      </Registers>
+000360b0: 0d0a 2020 2020 3c2f 4465 7669 6365 3e0d  ..    </Device>.
+000360c0: 0a20 2020 203c 4572 726f 7273 3e0d 0a20  .    <Errors>.. 
+000360d0: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+000360e0: 3078 3030 3030 3332 3830 2220 6166 6665  0x00003280" affe
+000360f0: 6374 6564 5f6d 6f64 756c 653d 2250 6f77  cted_module="Pow
+00036100: 6572 2073 7461 6765 2220 6572 726f 725f  er stage" error_
+00036110: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00036120: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00036130: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00036140: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00036150: 5354 4f20 4163 7469 7665 2061 6e64 2050  STO Active and P
+00036160: 6f77 6572 2073 7461 6765 2069 7320 7368  ower stage is sh
+00036170: 7574 646f 776e 3c2f 4c61 6265 6c3e 0d0a  utdown</Label>..
+00036180: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+00036190: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
+000361a0: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
+000361b0: 6964 3d22 3078 3030 3030 3232 3830 2220  id="0x00002280" 
+000361c0: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
+000361d0: 2250 6f77 6572 2073 7461 6765 2220 6572  "Power stage" er
+000361e0: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
+000361f0: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
+00036200: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00036210: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00036220: 5553 223e 4857 206f 7665 7220 6375 7272  US">HW over curr
+00036230: 656e 743c 2f4c 6162 656c 3e0d 0a20 2020  ent</Label>..   
+00036240: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00036250: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+00036260: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+00036270: 2230 7830 3030 3032 3238 3822 2061 6666  "0x00002288" aff
+00036280: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
+00036290: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
+000362a0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+000362b0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+000362c0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+000362d0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+000362e0: 3e55 7365 7220 4932 5420 6c69 6d69 7420  >User I2T limit 
+000362f0: 6465 7465 6374 6564 2077 6974 686f 7574  detected without
+00036300: 2063 7572 7265 6e74 2063 6f6e 7472 6f6c   current control
+00036310: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00036320: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00036330: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00036340: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00036350: 3030 3030 3332 3930 2220 6166 6665 6374  00003290" affect
+00036360: 6564 5f6d 6f64 756c 653d 2250 6f77 6572  ed_module="Power
+00036370: 2073 7461 6765 2220 6572 726f 725f 7479   stage" error_ty
+00036380: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
+00036390: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+000363a0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+000363b0: 206c 616e 673d 2265 6e5f 5553 223e 496e   lang="en_US">In
+000363c0: 7075 7420 7374 6167 6520 7072 6f62 6c65  put stage proble
+000363d0: 6d3c 2f4c 6162 656c 3e0d 0a20 2020 2020  m</Label>..     
+000363e0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+000363f0: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+00036400: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+00036410: 7830 3030 3033 3231 3022 2061 6666 6563  x00003210" affec
+00036420: 7465 645f 6d6f 6475 6c65 3d22 506f 7765  ted_module="Powe
+00036430: 7220 7374 6167 6522 2065 7272 6f72 5f74  r stage" error_t
+00036440: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
+00036450: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00036460: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+00036470: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e48  l lang="en_US">H
+00036480: 5720 4f76 6572 2d76 6f6c 7461 6765 2064  W Over-voltage d
+00036490: 6574 6563 7465 643c 2f4c 6162 656c 3e0d  etected</Label>.
+000364a0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
+000364b0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
+000364c0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
+000364d0: 2069 643d 2230 7830 3030 3033 3231 3122   id="0x00003211"
+000364e0: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
+000364f0: 3d22 506f 7765 7220 7374 6167 6522 2065  ="Power stage" e
+00036500: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
+00036510: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
+00036520: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00036530: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
+00036540: 5f55 5322 3e46 5720 4f76 6572 2d76 6f6c  _US">FW Over-vol
+00036550: 7461 6765 2064 6574 6563 7465 643c 2f4c  tage detected</L
+00036560: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00036570: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00036580: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00036590: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+000365a0: 3033 3232 3122 2061 6666 6563 7465 645f  03221" affected_
+000365b0: 6d6f 6475 6c65 3d22 506f 7765 7220 7374  module="Power st
+000365c0: 6167 6522 2065 7272 6f72 5f74 7970 653d  age" error_type=
+000365d0: 2263 7963 6c69 6322 3e0d 0a20 2020 2020  "cyclic">..     
+000365e0: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+000365f0: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00036600: 6e67 3d22 656e 5f55 5322 3e46 5720 556e  ng="en_US">FW Un
+00036610: 6465 722d 766f 6c74 6167 6520 6465 7465  der-voltage dete
+00036620: 6374 6564 3c2f 4c61 6265 6c3e 0d0a 2020  cted</Label>..  
+00036630: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00036640: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00036650: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00036660: 3d22 3078 3030 3030 3433 3030 2220 6166  ="0x00004300" af
+00036670: 6665 6374 6564 5f6d 6f64 756c 653d 2250  fected_module="P
+00036680: 6f77 6572 2073 7461 6765 2220 6572 726f  ower stage" erro
+00036690: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
+000366a0: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
+000366b0: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
+000366c0: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+000366d0: 223e 4f76 6572 2d54 656d 7065 7261 7475  ">Over-Temperatu
+000366e0: 7265 2064 6574 6563 7465 6420 2869 6e74  re detected (int
+000366f0: 6572 6e61 6c20 6472 6976 6520 6c69 6d69  ernal drive limi
+00036700: 7429 2e3c 2f4c 6162 656c 3e0d 0a20 2020  t).</Label>..   
+00036710: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00036720: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+00036730: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+00036740: 2230 7830 3030 3034 3330 3122 2061 6666  "0x00004301" aff
+00036750: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
+00036760: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
+00036770: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+00036780: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+00036790: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+000367a0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+000367b0: 3e55 6e64 6572 2d54 656d 7065 7261 7475  >Under-Temperatu
+000367c0: 7265 2064 6574 6563 7465 6420 2869 6e74  re detected (int
+000367d0: 6572 6e61 6c20 6472 6976 6520 6c69 6d69  ernal drive limi
+000367e0: 7429 3c2f 4c61 6265 6c3e 0d0a 2020 2020  t)</Label>..    
+000367f0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+00036800: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
+00036810: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+00036820: 3078 3030 3030 3434 3030 2220 6166 6665  0x00004400" affe
+00036830: 6374 6564 5f6d 6f64 756c 653d 2250 6f77  cted_module="Pow
+00036840: 6572 2073 7461 6765 2220 6572 726f 725f  er stage" error_
+00036850: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00036860: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00036870: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00036880: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00036890: 4d6f 746f 7220 4f76 6572 2054 656d 7065  Motor Over Tempe
+000368a0: 7261 7475 7265 2065 7272 6f72 3c2f 4c61  rature error</La
+000368b0: 6265 6c3e 0d0a 2020 2020 2020 2020 3c2f  bel>..        </
+000368c0: 4c61 6265 6c73 3e0d 0a20 2020 2020 203c  Labels>..      <
+000368d0: 2f45 7272 6f72 3e0d 0a20 2020 2020 203c  /Error>..      <
+000368e0: 4572 726f 7220 6964 3d22 3078 3030 3030  Error id="0x0000
+000368f0: 3733 3830 2220 6166 6665 6374 6564 5f6d  7380" affected_m
+00036900: 6f64 756c 653d 2246 6565 6462 6163 6b22  odule="Feedback"
+00036910: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
+00036920: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
+00036930: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00036940: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00036950: 656e 5f55 5322 3e54 6f6f 206d 616e 7920  en_US">Too many 
+00036960: 6572 726f 7220 6269 7473 206f 7220 696e  error bits or in
+00036970: 7661 6c69 6420 706f 7369 7469 6f6e 2066  valid position f
+00036980: 6c61 6773 2064 6574 6563 7465 6420 696e  lags detected in
+00036990: 2061 6273 6f6c 7574 6520 656e 636f 6465   absolute encode
+000369a0: 723c 2f4c 6162 656c 3e0d 0a20 2020 2020  r</Label>..     
+000369b0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+000369c0: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+000369d0: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+000369e0: 7830 3030 3037 3338 3222 2061 6666 6563  x00007382" affec
+000369f0: 7465 645f 6d6f 6475 6c65 3d22 4665 6564  ted_module="Feed
+00036a00: 6261 636b 2220 6572 726f 725f 7479 7065  back" error_type
+00036a10: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
+00036a20: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+00036a30: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+00036a40: 616e 673d 2265 6e5f 5553 223e 546f 6f20  ang="en_US">Too 
+00036a50: 6d61 6e79 2069 6e63 6f72 7265 6374 2043  many incorrect C
+00036a60: 5243 2063 6865 636b 7320 696e 2061 6273  RC checks in abs
+00036a70: 6f6c 7574 6520 656e 636f 6465 7220 7265  olute encoder re
+00036a80: 6164 696e 6773 3c2f 4c61 6265 6c3e 0d0a  adings</Label>..
+00036a90: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+00036aa0: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
+00036ab0: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
+00036ac0: 6964 3d22 3078 3030 3030 3733 3835 2220  id="0x00007385" 
+00036ad0: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
+00036ae0: 2243 6f6e 7472 6f6c 204c 6f6f 7073 2220  "Control Loops" 
+00036af0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
+00036b00: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
+00036b10: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00036b20: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00036b30: 6e5f 5553 223e 506f 7369 7469 6f6e 206f  n_US">Position o
+00036b40: 7574 206f 6620 6c69 6d69 7473 206f 7574  ut of limits out
+00036b50: 206f 6620 706f 7369 7469 6f6e 206d 6f64   of position mod
+00036b60: 6573 3c2f 4c61 6265 6c3e 0d0a 2020 2020  es</Label>..    
+00036b70: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+00036b80: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
+00036b90: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+00036ba0: 3078 3030 3030 3733 3836 2220 6166 6665  0x00007386" affe
+00036bb0: 6374 6564 5f6d 6f64 756c 653d 2243 6f6e  cted_module="Con
+00036bc0: 7472 6f6c 204c 6f6f 7073 2220 6572 726f  trol Loops" erro
+00036bd0: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
+00036be0: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
+00036bf0: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
+00036c00: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+00036c10: 223e 5665 6c6f 6369 7479 206f 7574 206f  ">Velocity out o
+00036c20: 6620 6c69 6d69 7473 206f 7574 206f 6620  f limits out of 
+00036c30: 7665 6c6f 6369 7479 206f 7220 706f 7369  velocity or posi
+00036c40: 7469 6f6e 206d 6f64 6573 3c2f 4c61 6265  tion modes</Labe
+00036c50: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
+00036c60: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
+00036c70: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
+00036c80: 726f 7220 6964 3d22 3078 3030 3030 3733  ror id="0x000073
+00036c90: 3837 2220 6166 6665 6374 6564 5f6d 6f64  87" affected_mod
+00036ca0: 756c 653d 2243 6f6e 7472 6f6c 204c 6f6f  ule="Control Loo
+00036cb0: 7073 2220 6572 726f 725f 7479 7065 3d22  ps" error_type="
+00036cc0: 6379 636c 6963 223e 0d0a 2020 2020 2020  cyclic">..      
+00036cd0: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
+00036ce0: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+00036cf0: 673d 2265 6e5f 5553 223e 506f 7369 7469  g="en_US">Positi
+00036d00: 6f6e 2066 6f6c 6c6f 7769 6e67 2065 7272  on following err
+00036d10: 6f72 3c2f 4c61 6265 6c3e 0d0a 2020 2020  or</Label>..    
+00036d20: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+00036d30: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
+00036d40: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+00036d50: 3078 3036 3031 3030 3030 2220 6166 6665  0x06010000" affe
+00036d60: 6374 6564 5f6d 6f64 756c 653d 2252 6567  cted_module="Reg
+00036d70: 6973 7465 7220 6469 6374 696f 6e61 7279  ister dictionary
+00036d80: 2220 6572 726f 725f 7479 7065 3d22 636f  " error_type="co
+00036d90: 6e66 6967 7572 6174 696f 6e22 3e0d 0a20  nfiguration">.. 
+00036da0: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00036db0: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+00036dc0: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e49  l lang="en_US">I
+00036dd0: 6e63 6f72 7265 6374 2061 6363 6573 7320  ncorrect access 
+00036de0: 7479 7065 3c2f 4c61 6265 6c3e 0d0a 2020  type</Label>..  
+00036df0: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00036e00: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00036e10: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00036e20: 3d22 3078 3036 3032 3030 3030 2220 6166  ="0x06020000" af
+00036e30: 6665 6374 6564 5f6d 6f64 756c 653d 2252  fected_module="R
+00036e40: 6567 6973 7465 7220 6469 6374 696f 6e61  egister dictiona
+00036e50: 7279 2220 6572 726f 725f 7479 7065 3d22  ry" error_type="
+00036e60: 636f 6e66 6967 7572 6174 696f 6e22 3e0d  configuration">.
+00036e70: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+00036e80: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00036e90: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00036ea0: 3e4f 626a 6563 7420 646f 6573 6e27 7420  >Object doesn't 
+00036eb0: 6578 6973 743c 2f4c 6162 656c 3e0d 0a20  exist</Label>.. 
+00036ec0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00036ed0: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
+00036ee0: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
+00036ef0: 643d 2230 7830 3630 3430 3034 3122 2061  d="0x06040041" a
+00036f00: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
+00036f10: 5265 6769 7374 6572 2064 6963 7469 6f6e  Register diction
+00036f20: 6172 7922 2065 7272 6f72 5f74 7970 653d  ary" error_type=
+00036f30: 2263 6f6e 6669 6775 7261 7469 6f6e 223e  "configuration">
+00036f40: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
+00036f50: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
+00036f60: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+00036f70: 223e 4f62 6a65 6374 2069 736e 2774 2050  ">Object isn't P
+00036f80: 444f 206d 6170 7061 626c 6520 6173 2072  DO mappable as r
+00036f90: 6571 7565 7374 6564 3c2f 4c61 6265 6c3e  equested</Label>
+00036fa0: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
+00036fb0: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
+00036fc0: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
+00036fd0: 7220 6964 3d22 3078 3036 3037 3030 3130  r id="0x06070010
+00036fe0: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
+00036ff0: 653d 2252 6567 6973 7465 7220 6469 6374  e="Register dict
+00037000: 696f 6e61 7279 2220 6572 726f 725f 7479  ionary" error_ty
+00037010: 7065 3d22 636f 6e66 6967 7572 6174 696f  pe="configuratio
+00037020: 6e22 3e0d 0a20 2020 2020 2020 203c 4c61  n">..        <La
+00037030: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00037040: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
+00037050: 5f55 5322 3e49 6e63 6f72 7265 6374 2073  _US">Incorrect s
+00037060: 7065 6369 6669 6564 206f 626a 6563 7420  pecified object 
+00037070: 7369 7a65 3c2f 4c61 6265 6c3e 0d0a 2020  size</Label>..  
+00037080: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00037090: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+000370a0: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+000370b0: 3d22 3078 3036 3039 3030 3131 2220 6166  ="0x06090011" af
+000370c0: 6665 6374 6564 5f6d 6f64 756c 653d 2252  fected_module="R
+000370d0: 6567 6973 7465 7220 6469 6374 696f 6e61  egister dictiona
+000370e0: 7279 2220 6572 726f 725f 7479 7065 3d22  ry" error_type="
+000370f0: 636f 6e66 6967 7572 6174 696f 6e22 3e0d  configuration">.
+00037100: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+00037110: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00037120: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00037130: 3e53 7562 2d49 6e64 6578 2064 6f65 7320  >Sub-Index does 
+00037140: 6e6f 7420 6578 6973 743c 2f4c 6162 656c  not exist</Label
+00037150: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
+00037160: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
+00037170: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
+00037180: 6f72 2069 643d 2230 7830 3630 4130 3030  or id="0x060A000
+00037190: 3022 2061 6666 6563 7465 645f 6d6f 6475  0" affected_modu
+000371a0: 6c65 3d22 5265 6769 7374 6572 2064 6963  le="Register dic
+000371b0: 7469 6f6e 6172 7922 2065 7272 6f72 5f74  tionary" error_t
+000371c0: 7970 653d 2263 6f6e 6669 6775 7261 7469  ype="configurati
+000371d0: 6f6e 223e 0d0a 2020 2020 2020 2020 3c4c  on">..        <L
+000371e0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+000371f0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00037200: 6e5f 5553 223e 556e 7375 7070 6f72 7465  n_US">Unsupporte
+00037210: 6420 7661 6c75 6520 696e 7472 6f64 7563  d value introduc
+00037220: 6564 2069 6e20 7265 6769 7374 6572 3c2f  ed in register</
+00037230: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+00037240: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00037250: 203c 2f45 7272 6f72 3e0d 0a20 2020 2020   </Error>..     
+00037260: 203c 4572 726f 7220 6964 3d22 3078 3038   <Error id="0x08
+00037270: 3030 3030 3030 2220 6166 6665 6374 6564  000000" affected
+00037280: 5f6d 6f64 756c 653d 2252 6567 6973 7465  _module="Registe
+00037290: 7220 6469 6374 696f 6e61 7279 2220 6572  r dictionary" er
+000372a0: 726f 725f 7479 7065 3d22 636f 6e66 6967  ror_type="config
+000372b0: 7572 6174 696f 6e22 3e0d 0a20 2020 2020  uration">..     
+000372c0: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+000372d0: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+000372e0: 6e67 3d22 656e 5f55 5322 3e52 6561 6420  ng="en_US">Read 
+000372f0: 2f20 5772 6974 6520 6f70 6572 6174 696f  / Write operatio
+00037300: 6e20 6e6f 7420 6578 6563 7574 6564 3c2f  n not executed</
+00037310: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+00037320: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+00037330: 203c 2f45 7272 6f72 3e0d 0a20 2020 2020   </Error>..     
+00037340: 203c 4572 726f 7220 6964 3d22 3078 3030   <Error id="0x00
+00037350: 3030 3332 3331 2220 6166 6665 6374 6564  003231" affected
+00037360: 5f6d 6f64 756c 653d 2250 6f77 6572 2073  _module="Power s
+00037370: 7461 6765 2220 6572 726f 725f 7479 7065  tage" error_type
+00037380: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
+00037390: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+000373a0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+000373b0: 616e 673d 2265 6e5f 5553 223e 5573 6572  ang="en_US">User
+000373c0: 204f 7665 722d 766f 6c74 6167 6520 6465   Over-voltage de
+000373d0: 7465 6374 6564 3c2f 4c61 6265 6c3e 0d0a  tected</Label>..
+000373e0: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+000373f0: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
+00037400: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
+00037410: 6964 3d22 3078 3030 3030 3332 3431 2220  id="0x00003241" 
+00037420: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
+00037430: 2250 6f77 6572 2073 7461 6765 2220 6572  "Power stage" er
+00037440: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
+00037450: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
+00037460: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00037470: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00037480: 5553 223e 5573 6572 2055 6e64 6572 2d76  US">User Under-v
+00037490: 6f6c 7461 6765 2064 6574 6563 7465 643c  oltage detected<
+000374a0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+000374b0: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+000374c0: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
+000374d0: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
+000374e0: 3030 3034 3330 3322 2061 6666 6563 7465  0004303" affecte
+000374f0: 645f 6d6f 6475 6c65 3d22 506f 7765 7220  d_module="Power 
+00037500: 7374 6167 6522 2065 7272 6f72 5f74 7970  stage" error_typ
+00037510: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00037520: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00037530: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00037540: 6c61 6e67 3d22 656e 5f55 5322 3e4f 7665  lang="en_US">Ove
+00037550: 722d 7465 6d70 6572 6174 7572 6520 6465  r-temperature de
+00037560: 7465 6374 6564 2028 7573 6572 206c 696d  tected (user lim
+00037570: 6974 293c 2f4c 6162 656c 3e0d 0a20 2020  it)</Label>..   
+00037580: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00037590: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+000375a0: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+000375b0: 2230 7830 3030 3034 3330 3422 2061 6666  "0x00004304" aff
+000375c0: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
+000375d0: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
+000375e0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+000375f0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+00037600: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00037610: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00037620: 3e55 6e64 6572 2d74 656d 7065 7261 7475  >Under-temperatu
+00037630: 7265 2064 6574 6563 7465 6420 2875 7365  re detected (use
+00037640: 7220 6c69 6d69 7429 3c2f 4c61 6265 6c3e  r limit)</Label>
+00037650: 0d0a 2020 2020 2020 2020 3c2f 4c61 6265  ..        </Labe
+00037660: 6c73 3e0d 0a20 2020 2020 203c 2f45 7272  ls>..      </Err
+00037670: 6f72 3e0d 0a20 2020 2020 203c 4572 726f  or>..      <Erro
+00037680: 7220 6964 3d22 3078 3030 3030 3435 3030  r id="0x00004500
+00037690: 2220 6166 6665 6374 6564 5f6d 6f64 756c  " affected_modul
+000376a0: 653d 2250 6f77 6572 2073 7461 6765 2220  e="Power stage" 
+000376b0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
+000376c0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
+000376d0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+000376e0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+000376f0: 6e5f 5553 223e 4578 7465 726e 616c 2065  n_US">External e
+00037700: 7272 6f72 3c2f 4c61 6265 6c3e 0d0a 2020  rror</Label>..  
+00037710: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00037720: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00037730: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00037740: 3d22 3078 3030 3030 3733 3930 2220 6166  ="0x00007390" af
+00037750: 6665 6374 6564 5f6d 6f64 756c 653d 2250  fected_module="P
+00037760: 726f 6669 6c65 7222 2065 7272 6f72 5f74  rofiler" error_t
+00037770: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
+00037780: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00037790: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+000377a0: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e49  l lang="en_US">I
+000377b0: 6e74 6572 706f 6c61 7469 6f6e 2074 696d  nterpolation tim
+000377c0: 6520 6973 2074 6f20 736d 616c 6c20 7768  e is to small wh
+000377d0: 656e 2050 5654 2069 7320 656e 6162 6c65  en PVT is enable
+000377e0: 643c 2f4c 6162 656c 3e0d 0a20 2020 2020  d</Label>..     
+000377f0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+00037800: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+00037810: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+00037820: 7830 3030 3033 3238 3122 2061 6666 6563  x00003281" affec
+00037830: 7465 645f 6d6f 6475 6c65 3d22 506f 7765  ted_module="Powe
+00037840: 7220 7374 6167 6522 2065 7272 6f72 5f74  r stage" error_t
+00037850: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
+00037860: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00037870: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+00037880: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e41  l lang="en_US">A
+00037890: 626e 6f72 6d61 6c20 5354 4f20 5375 7070  bnormal STO Supp
+000378a0: 6c79 2e20 556e 6974 2063 6f75 6c64 2062  ly. Unit could b
+000378b0: 6520 6461 6d61 6765 643c 2f4c 6162 656c  e damaged</Label
+000378c0: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
+000378d0: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
+000378e0: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
+000378f0: 6f72 2069 643d 2230 7830 3030 3033 3238  or id="0x0000328
+00037900: 3222 2061 6666 6563 7465 645f 6d6f 6475  2" affected_modu
+00037910: 6c65 3d22 506f 7765 7220 7374 6167 6522  le="Power stage"
+00037920: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
+00037930: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
+00037940: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00037950: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00037960: 656e 5f55 5322 3e41 626e 6f72 6d61 6c20  en_US">Abnormal 
+00037970: 5354 4f2e 2053 544f 3120 616e 6420 5354  STO. STO1 and ST
+00037980: 4f32 2069 6e70 7574 7320 6469 6666 6572  O2 inputs differ
+00037990: 6564 206d 6f72 6520 7468 616e 206c 6174  ed more than lat
+000379a0: 6368 696e 6720 7469 6d65 3c2f 4c61 6265  ching time</Labe
+000379b0: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
+000379c0: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
+000379d0: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
+000379e0: 726f 7220 6964 3d22 3078 3030 3030 3733  ror id="0x000073
+000379f0: 3730 2220 6166 6665 6374 6564 5f6d 6f64  70" affected_mod
+00037a00: 756c 653d 2246 6565 6462 6163 6b73 2220  ule="Feedbacks" 
+00037a10: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
+00037a20: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
+00037a30: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00037a40: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00037a50: 6e5f 5553 223e 4861 6c6c 7320 7365 7175  n_US">Halls sequ
+00037a60: 656e 6365 2065 7272 6f72 3c2f 4c61 6265  ence error</Labe
+00037a70: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
+00037a80: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
+00037a90: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
+00037aa0: 726f 7220 6964 3d22 3078 3030 3030 3733  ror id="0x000073
+00037ab0: 3731 2220 6166 6665 6374 6564 5f6d 6f64  71" affected_mod
+00037ac0: 756c 653d 2246 6565 6462 6163 6b73 2220  ule="Feedbacks" 
+00037ad0: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
+00037ae0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
+00037af0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00037b00: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00037b10: 6e5f 5553 223e 4861 6c6c 7320 636f 6d62  n_US">Halls comb
+00037b20: 696e 6174 696f 6e20 6572 726f 723c 2f4c  ination error</L
+00037b30: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00037b40: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00037b50: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00037b60: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00037b70: 3037 3337 3222 2061 6666 6563 7465 645f  07372" affected_
+00037b80: 6d6f 6475 6c65 3d22 4665 6564 6261 636b  module="Feedback
+00037b90: 7322 2065 7272 6f72 5f74 7970 653d 2263  s" error_type="c
+00037ba0: 7963 6c69 6322 3e0d 0a20 2020 2020 2020  yclic">..       
+00037bb0: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00037bc0: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00037bd0: 3d22 656e 5f55 5322 3e46 6565 6462 6163  ="en_US">Feedbac
+00037be0: 6b20 7275 6e61 7761 7920 6572 726f 723c  k runaway error<
+00037bf0: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+00037c00: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00037c10: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
+00037c20: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
+00037c30: 3030 3032 3238 3922 2061 6666 6563 7465  0002289" affecte
+00037c40: 645f 6d6f 6475 6c65 3d22 506f 7765 7220  d_module="Power 
+00037c50: 7374 6167 6522 2065 7272 6f72 5f74 7970  stage" error_typ
+00037c60: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00037c70: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00037c80: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00037c90: 6c61 6e67 3d22 656e 5f55 5322 3e4f 7665  lang="en_US">Ove
+00037ca0: 7220 6375 7272 656e 7420 7769 7468 6f75  r current withou
+00037cb0: 7420 6375 7272 656e 7420 636f 6e74 726f  t current contro
+00037cc0: 6c3c 2f4c 6162 656c 3e0d 0a20 2020 2020  l</Label>..     
+00037cd0: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+00037ce0: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+00037cf0: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+00037d00: 7830 3030 3037 3339 3122 2061 6666 6563  x00007391" affec
+00037d10: 7465 645f 6d6f 6475 6c65 3d22 5072 6f66  ted_module="Prof
+00037d20: 696c 6572 2220 6572 726f 725f 7479 7065  iler" error_type
+00037d30: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
+00037d40: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+00037d50: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+00037d60: 616e 673d 2265 6e5f 5553 223e 5072 6f66  ang="en_US">Prof
+00037d70: 696c 6572 2070 6172 616d 6574 6572 7320  iler parameters 
+00037d80: 6e6f 7420 7661 6c69 642e 2054 6865 7920  not valid. They 
+00037d90: 7368 6f75 6c64 2061 6c6c 2068 6176 6520  should all have 
+00037da0: 706f 7369 7469 7665 2076 616c 7565 732e  positive values.
+00037db0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00037dc0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00037dd0: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00037de0: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00037df0: 3030 3030 3030 3030 2220 6166 6665 6374  00000000" affect
+00037e00: 6564 5f6d 6f64 756c 653d 2244 7269 7665  ed_module="Drive
+00037e10: 2220 6572 726f 725f 7479 7065 3d22 6379  " error_type="cy
+00037e20: 636c 6963 223e 0d0a 2020 2020 2020 2020  clic">..        
+00037e30: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+00037e40: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+00037e50: 2265 6e5f 5553 223e 4e6f 2065 7272 6f72  "en_US">No error
+00037e60: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00037e70: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00037e80: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00037e90: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00037ea0: 3030 3030 3733 3831 2220 6166 6665 6374  00007381" affect
+00037eb0: 6564 5f6d 6f64 756c 653d 2246 6565 6462  ed_module="Feedb
+00037ec0: 6163 6b73 2220 6572 726f 725f 7479 7065  acks" error_type
+00037ed0: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
+00037ee0: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+00037ef0: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+00037f00: 616e 673d 2265 6e5f 5553 223e 4269 5353  ang="en_US">BiSS
+00037f10: 2d43 2077 6172 6e69 6e67 2062 6974 2061  -C warning bit a
+00037f20: 6374 6976 653c 2f4c 6162 656c 3e0d 0a20  ctive</Label>.. 
+00037f30: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00037f40: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
+00037f50: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
+00037f60: 643d 2230 7830 3030 3031 3030 3122 2061  d="0x00001001" a
+00037f70: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
+00037f80: 436f 6d6d 756e 6963 6174 696f 6e73 2220  Communications" 
+00037f90: 6572 726f 725f 7479 7065 3d22 6379 636c  error_type="cycl
+00037fa0: 6963 223e 0d0a 2020 2020 2020 2020 3c4c  ic">..        <L
+00037fb0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+00037fc0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00037fd0: 6e5f 5553 223e 436f 6d6d 756e 6963 6174  n_US">Communicat
+00037fe0: 696f 6e73 2077 6174 6368 646f 6720 6572  ions watchdog er
+00037ff0: 726f 723c 2f4c 6162 656c 3e0d 0a20 2020  ror</Label>..   
+00038000: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00038010: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+00038020: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+00038030: 2230 7830 3030 3037 3338 3822 2061 6666  "0x00007388" aff
+00038040: 6563 7465 645f 6d6f 6475 6c65 3d22 436f  ected_module="Co
+00038050: 6e74 726f 6c20 6c6f 6f70 7322 2065 7272  ntrol loops" err
+00038060: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
+00038070: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
+00038080: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
+00038090: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+000380a0: 5322 3e56 656c 6f63 6974 7920 666f 6c6c  S">Velocity foll
+000380b0: 6f77 696e 6720 6572 726f 723c 2f4c 6162  owing error</Lab
+000380c0: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
+000380d0: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
+000380e0: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
+000380f0: 7272 6f72 2069 643d 2230 7830 3030 3037  rror id="0x00007
+00038100: 3338 3922 2061 6666 6563 7465 645f 6d6f  389" affected_mo
+00038110: 6475 6c65 3d22 436f 6d6d 7574 6174 696f  dule="Commutatio
+00038120: 6e22 2065 7272 6f72 5f74 7970 653d 2263  n" error_type="c
+00038130: 7963 6c69 6322 3e0d 0a20 2020 2020 2020  yclic">..       
+00038140: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00038150: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00038160: 3d22 656e 5f55 5322 3e41 6e67 6c65 2069  ="en_US">Angle i
+00038170: 6e74 6567 7269 7479 2063 6865 636b 2031  ntegrity check 1
+00038180: 2065 7272 6f72 3c2f 4c61 6265 6c3e 0d0a   error</Label>..
+00038190: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+000381a0: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
+000381b0: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
+000381c0: 6964 3d22 3078 3030 3030 3733 3841 2220  id="0x0000738A" 
+000381d0: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
+000381e0: 2243 6f6d 6d75 7461 7469 6f6e 2220 6572  "Commutation" er
+000381f0: 726f 725f 7479 7065 3d22 6379 636c 6963  ror_type="cyclic
+00038200: 223e 0d0a 2020 2020 2020 2020 3c4c 6162  ">..        <Lab
+00038210: 656c 733e 0d0a 2020 2020 2020 2020 2020  els>..          
+00038220: 3c4c 6162 656c 206c 616e 673d 2265 6e5f  <Label lang="en_
+00038230: 5553 223e 416e 676c 6520 696e 7465 6772  US">Angle integr
+00038240: 6974 7920 6368 6563 6b20 3220 6572 726f  ity check 2 erro
+00038250: 723c 2f4c 6162 656c 3e0d 0a20 2020 2020  r</Label>..     
+00038260: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+00038270: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+00038280: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+00038290: 7830 3030 3037 3338 4222 2061 6666 6563  x0000738B" affec
+000382a0: 7465 645f 6d6f 6475 6c65 3d22 436f 6d6d  ted_module="Comm
+000382b0: 7574 6174 696f 6e22 2065 7272 6f72 5f74  utation" error_t
+000382c0: 7970 653d 2263 6f6e 6669 6775 7261 7469  ype="configurati
+000382d0: 6f6e 223e 0d0a 2020 2020 2020 2020 3c4c  on">..        <L
+000382e0: 6162 656c 733e 0d0a 2020 2020 2020 2020  abels>..        
+000382f0: 2020 3c4c 6162 656c 206c 616e 673d 2265    <Label lang="e
+00038300: 6e5f 5553 223e 5472 6170 657a 6f69 6461  n_US">Trapezoida
+00038310: 6c20 636f 6d6d 7574 6174 696f 6e20 7769  l commutation wi
+00038320: 7468 6f75 7420 6469 6769 7461 6c20 6861  thout digital ha
+00038330: 6c6c 7320 6e6f 7420 616c 6c6f 7765 642e  lls not allowed.
+00038340: 2052 6576 6965 7720 636f 6d6d 7574 6174   Review commutat
+00038350: 696f 6e20 7365 6e73 6f72 2063 6f6e 6669  ion sensor confi
+00038360: 6775 7261 7469 6f6e 2061 6e64 2070 6861  guration and pha
+00038370: 7369 6e67 3c2f 4c61 6265 6c3e 0d0a 2020  sing</Label>..  
+00038380: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00038390: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+000383a0: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+000383b0: 3d22 3078 3030 3030 3232 3841 2220 6166  ="0x0000228A" af
+000383c0: 6665 6374 6564 5f6d 6f64 756c 653d 2250  fected_module="P
+000383d0: 6f77 6572 2073 7461 6765 2220 6572 726f  ower stage" erro
+000383e0: 725f 7479 7065 3d22 6379 636c 6963 223e  r_type="cyclic">
+000383f0: 0d0a 2020 2020 2020 2020 3c4c 6162 656c  ..        <Label
+00038400: 733e 0d0a 2020 2020 2020 2020 2020 3c4c  s>..          <L
+00038410: 6162 656c 206c 616e 673d 2265 6e5f 5553  abel lang="en_US
+00038420: 223e 5379 7374 656d 2049 3254 2064 6574  ">System I2T det
+00038430: 6563 7465 643c 2f4c 6162 656c 3e0d 0a20  ected</Label>.. 
+00038440: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00038450: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
+00038460: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
+00038470: 643d 2230 7830 3030 3037 3338 3322 2061  d="0x00007383" a
+00038480: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
+00038490: 4665 6564 6261 636b 7322 2065 7272 6f72  Feedbacks" error
+000384a0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+000384b0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+000384c0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+000384d0: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+000384e0: 3e4d 6178 696d 756d 2061 6273 6f6c 7574  >Maximum absolut
+000384f0: 6520 7665 6c6f 6369 7479 2065 7863 6565  e velocity excee
+00038500: 6465 643c 2f4c 6162 656c 3e0d 0a20 2020  ded</Label>..   
+00038510: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00038520: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+00038530: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+00038540: 2230 7830 3030 3037 3338 4422 2061 6666  "0x0000738D" aff
+00038550: 6563 7465 645f 6d6f 6475 6c65 3d22 4665  ected_module="Fe
+00038560: 6564 6261 636b 7322 2065 7272 6f72 5f74  edbacks" error_t
+00038570: 7970 653d 2263 7963 6c69 6322 3e0d 0a20  ype="cyclic">.. 
+00038580: 2020 2020 2020 203c 4c61 6265 6c73 3e0d         <Labels>.
+00038590: 0a20 2020 2020 2020 2020 203c 4c61 6265  .          <Labe
+000385a0: 6c20 6c61 6e67 3d22 656e 5f55 5322 3e49  l lang="en_US">I
+000385b0: 6e63 7265 6d65 6e74 616c 2065 6e63 6f64  ncremental encod
+000385c0: 6572 2031 2069 6e64 6578 2070 756c 7365  er 1 index pulse
+000385d0: 2069 6e74 6567 7269 7479 2063 6865 636b   integrity check
+000385e0: 2066 6169 6c3c 2f4c 6162 656c 3e0d 0a20   fail</Label>.. 
+000385f0: 2020 2020 2020 203c 2f4c 6162 656c 733e         </Labels>
+00038600: 0d0a 2020 2020 2020 3c2f 4572 726f 723e  ..      </Error>
+00038610: 0d0a 2020 2020 2020 3c45 7272 6f72 2069  ..      <Error i
+00038620: 643d 2230 7830 3030 3037 3338 4522 2061  d="0x0000738E" a
+00038630: 6666 6563 7465 645f 6d6f 6475 6c65 3d22  ffected_module="
+00038640: 4665 6564 6261 636b 7322 2065 7272 6f72  Feedbacks" error
+00038650: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+00038660: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+00038670: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00038680: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00038690: 3e49 6e63 7265 6d65 6e74 616c 2065 6e63  >Incremental enc
+000386a0: 6f64 6572 2032 2069 6e64 6578 2070 756c  oder 2 index pul
+000386b0: 7365 2069 6e74 6567 7269 7479 2063 6865  se integrity che
+000386c0: 636b 2066 6169 6c3c 2f4c 6162 656c 3e0d  ck fail</Label>.
+000386d0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
+000386e0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
+000386f0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
+00038700: 2069 643d 2230 7830 3030 3032 3238 3122   id="0x00002281"
+00038710: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
+00038720: 3d22 506f 7765 7220 7374 6167 6522 2065  ="Power stage" e
+00038730: 7272 6f72 5f74 7970 653d 2263 7963 6c69  rror_type="cycli
+00038740: 6322 3e0d 0a20 2020 2020 2020 203c 4c61  c">..        <La
+00038750: 6265 6c73 3e0d 0a20 2020 2020 2020 2020  bels>..         
+00038760: 203c 4c61 6265 6c20 6c61 6e67 3d22 656e   <Label lang="en
+00038770: 5f55 5322 3e46 6175 6c74 2064 6574 6563  _US">Fault detec
+00038780: 7465 6420 696e 2074 6865 2070 6f77 6572  ted in the power
+00038790: 2073 7461 6765 2067 6174 6520 6472 6976   stage gate driv
+000387a0: 6572 3c2f 4c61 6265 6c3e 0d0a 2020 2020  er</Label>..    
+000387b0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+000387c0: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
+000387d0: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+000387e0: 3078 3030 3030 3232 3931 2220 6166 6665  0x00002291" affe
+000387f0: 6374 6564 5f6d 6f64 756c 653d 2250 6f77  cted_module="Pow
+00038800: 6572 2073 7461 6765 2220 6572 726f 725f  er stage" error_
+00038810: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00038820: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00038830: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00038840: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00038850: 4f70 656e 2070 6861 7365 2064 6574 6563  Open phase detec
+00038860: 7465 643c 2f4c 6162 656c 3e0d 0a20 2020  ted</Label>..   
+00038870: 2020 2020 203c 2f4c 6162 656c 733e 0d0a       </Labels>..
+00038880: 2020 2020 2020 3c2f 4572 726f 723e 0d0a        </Error>..
+00038890: 2020 2020 2020 3c45 7272 6f72 2069 643d        <Error id=
+000388a0: 2230 7830 3030 3032 3239 3022 2061 6666  "0x00002290" aff
+000388b0: 6563 7465 645f 6d6f 6475 6c65 3d22 506f  ected_module="Po
+000388c0: 7765 7220 7374 6167 6522 2065 7272 6f72  wer stage" error
+000388d0: 5f74 7970 653d 2263 7963 6c69 6322 3e0d  _type="cyclic">.
+000388e0: 0a20 2020 2020 2020 203c 4c61 6265 6c73  .        <Labels
+000388f0: 3e0d 0a20 2020 2020 2020 2020 203c 4c61  >..          <La
+00038900: 6265 6c20 6c61 6e67 3d22 656e 5f55 5322  bel lang="en_US"
+00038910: 3e4e 6f6e 2d7a 6572 6f20 746f 7461 6c20  >Non-zero total 
+00038920: 7068 6173 6520 6375 7272 656e 743c 2f4c  phase current</L
+00038930: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038940: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038950: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038960: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038970: 3032 3238 3222 2061 6666 6563 7465 645f  02282" affected_
+00038980: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038990: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+000389a0: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+000389b0: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+000389c0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+000389d0: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+000389e0: 7265 6e74 2041 2073 656e 7369 6e67 2072  rent A sensing r
+000389f0: 6561 6368 6564 2075 7070 6572 2073 6174  eached upper sat
+00038a00: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038a10: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038a20: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038a30: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038a40: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038a50: 3032 3238 3322 2061 6666 6563 7465 645f  02283" affected_
+00038a60: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038a70: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+00038a80: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00038a90: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00038aa0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00038ab0: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00038ac0: 7265 6e74 2041 2073 656e 7369 6e67 2072  rent A sensing r
+00038ad0: 6561 6368 6564 206c 6f77 6572 2073 6174  eached lower sat
+00038ae0: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038af0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038b00: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038b10: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038b20: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038b30: 3032 3238 3422 2061 6666 6563 7465 645f  02284" affected_
+00038b40: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038b50: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+00038b60: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00038b70: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00038b80: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00038b90: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00038ba0: 7265 6e74 2042 2073 656e 7369 6e67 2072  rent B sensing r
+00038bb0: 6561 6368 6564 2075 7070 6572 2073 6174  eached upper sat
+00038bc0: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038bd0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038be0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038bf0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038c00: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038c10: 3032 3238 3522 2061 6666 6563 7465 645f  02285" affected_
+00038c20: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038c30: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+00038c40: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00038c50: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00038c60: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00038c70: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00038c80: 7265 6e74 2042 2073 656e 7369 6e67 2072  rent B sensing r
+00038c90: 6561 6368 6564 206c 6f77 6572 2073 6174  eached lower sat
+00038ca0: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038cb0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038cc0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038cd0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038ce0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038cf0: 3032 3238 3622 2061 6666 6563 7465 645f  02286" affected_
+00038d00: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038d10: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+00038d20: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00038d30: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00038d40: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00038d50: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00038d60: 7265 6e74 2043 2073 656e 7369 6e67 2072  rent C sensing r
+00038d70: 6561 6368 6564 2075 7070 6572 2073 6174  eached upper sat
+00038d80: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038d90: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038da0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038db0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038dc0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038dd0: 3032 3238 3722 2061 6666 6563 7465 645f  02287" affected_
+00038de0: 6d6f 6475 6c65 3d22 436f 6e74 726f 6c20  module="Control 
+00038df0: 6c6f 6f70 7322 2065 7272 6f72 5f74 7970  loops" error_typ
+00038e00: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00038e10: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00038e20: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00038e30: 6c61 6e67 3d22 656e 5f55 5322 3e43 7572  lang="en_US">Cur
+00038e40: 7265 6e74 2043 2073 656e 7369 6e67 2072  rent C sensing r
+00038e50: 6561 6368 6564 206c 6f77 6572 2073 6174  eached lower sat
+00038e60: 7572 6174 696f 6e20 6c69 6d69 743c 2f4c  uration limit</L
+00038e70: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00038e80: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+00038e90: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+00038ea0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+00038eb0: 3037 3338 4622 2061 6666 6563 7465 645f  0738F" affected_
+00038ec0: 6d6f 6475 6c65 3d22 4665 6564 6261 636b  module="Feedback
+00038ed0: 7322 2065 7272 6f72 5f74 7970 653d 2263  s" error_type="c
+00038ee0: 7963 6c69 6322 3e0d 0a20 2020 2020 2020  yclic">..       
+00038ef0: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00038f00: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00038f10: 3d22 656e 5f55 5322 3e44 6967 6974 616c  ="en_US">Digital
+00038f20: 2065 6e63 6f64 6572 2069 6e64 6578 2070   encoder index p
+00038f30: 756c 7365 2069 6e74 6567 7269 7479 2063  ulse integrity c
+00038f40: 6865 636b 2063 616c 6962 7261 7469 6f6e  heck calibration
+00038f50: 2065 7272 6f72 3c2f 4c61 6265 6c3e 0d0a   error</Label>..
+00038f60: 2020 2020 2020 2020 3c2f 4c61 6265 6c73          </Labels
+00038f70: 3e0d 0a20 2020 2020 203c 2f45 7272 6f72  >..      </Error
+00038f80: 3e0d 0a20 2020 2020 203c 4572 726f 7220  >..      <Error 
+00038f90: 6964 3d22 3078 3030 3030 3233 3032 2220  id="0x00002302" 
+00038fa0: 6166 6665 6374 6564 5f6d 6f64 756c 653d  affected_module=
+00038fb0: 2242 7261 6b65 2220 6572 726f 725f 7479  "Brake" error_ty
+00038fc0: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
+00038fd0: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00038fe0: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00038ff0: 206c 616e 673d 2265 6e5f 5553 223e 4272   lang="en_US">Br
+00039000: 616b 6520 6375 7272 656e 7420 7472 6163  ake current trac
+00039010: 6b69 6e67 2065 7272 6f72 3c2f 4c61 6265  king error</Labe
+00039020: 6c3e 0d0a 2020 2020 2020 2020 3c2f 4c61  l>..        </La
+00039030: 6265 6c73 3e0d 0a20 2020 2020 203c 2f45  bels>..      </E
+00039040: 7272 6f72 3e0d 0a20 2020 2020 203c 4572  rror>..      <Er
+00039050: 726f 7220 6964 3d22 3078 3030 3030 3232  ror id="0x000022
+00039060: 3842 2220 6166 6665 6374 6564 5f6d 6f64  8B" affected_mod
+00039070: 756c 653d 2250 6f77 6572 2073 7461 6765  ule="Power stage
+00039080: 2220 6572 726f 725f 7479 7065 3d22 6379  " error_type="cy
+00039090: 636c 6963 223e 0d0a 2020 2020 2020 2020  clic">..        
+000390a0: 3c4c 6162 656c 733e 0d0a 2020 2020 2020  <Labels>..      
+000390b0: 2020 2020 3c4c 6162 656c 206c 616e 673d      <Label lang=
+000390c0: 2265 6e5f 5553 223e 4375 7272 656e 7420  "en_US">Current 
+000390d0: 6465 7261 7469 6e67 2077 6974 686f 7574  derating without
+000390e0: 2063 7572 7265 6e74 2063 6f6e 7472 6f6c   current control
+000390f0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00039100: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00039110: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00039120: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00039130: 3030 3030 3433 3035 2220 6166 6665 6374  00004305" affect
+00039140: 6564 5f6d 6f64 756c 653d 2250 6f77 6572  ed_module="Power
+00039150: 2073 7461 6765 2220 6572 726f 725f 7479   stage" error_ty
+00039160: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
+00039170: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00039180: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00039190: 206c 616e 673d 2265 6e5f 5553 223e 5772   lang="en_US">Wr
+000391a0: 6f6e 6720 4144 4320 6d65 6173 7572 656d  ong ADC measurem
+000391b0: 656e 7473 2064 6574 6563 7469 6f6e 3c2f  ents detection</
+000391c0: 4c61 6265 6c3e 0d0a 2020 2020 2020 2020  Label>..        
+000391d0: 3c2f 4c61 6265 6c73 3e0d 0a20 2020 2020  </Labels>..     
+000391e0: 203c 2f45 7272 6f72 3e0d 0a20 2020 2020   </Error>..     
+000391f0: 203c 4572 726f 7220 6964 3d22 3078 3030   <Error id="0x00
+00039200: 3030 3433 3036 2220 6166 6665 6374 6564  004306" affected
+00039210: 5f6d 6f64 756c 653d 2250 6f77 6572 2073  _module="Power s
+00039220: 7461 6765 2220 6572 726f 725f 7479 7065  tage" error_type
+00039230: 3d22 6379 636c 6963 223e 0d0a 2020 2020  ="cyclic">..    
+00039240: 2020 2020 3c4c 6162 656c 733e 0d0a 2020      <Labels>..  
+00039250: 2020 2020 2020 2020 3c4c 6162 656c 206c          <Label l
+00039260: 616e 673d 2265 6e5f 5553 223e 5573 6572  ang="en_US">User
+00039270: 206f 7665 7220 7465 6d70 6572 6174 7572   over temperatur
+00039280: 6520 7761 726e 696e 6720 7468 7265 7368  e warning thresh
+00039290: 6f6c 6420 6578 6365 6564 6564 2e3c 2f4c  old exceeded.</L
+000392a0: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+000392b0: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+000392c0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+000392d0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+000392e0: 3034 3330 3722 2061 6666 6563 7465 645f  04307" affected_
+000392f0: 6d6f 6475 6c65 3d22 506f 7765 7220 7374  module="Power st
+00039300: 6167 6522 2065 7272 6f72 5f74 7970 653d  age" error_type=
+00039310: 2263 7963 6c69 6322 3e0d 0a20 2020 2020  "cyclic">..     
+00039320: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00039330: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00039340: 6e67 3d22 656e 5f55 5322 3e55 7365 7220  ng="en_US">User 
+00039350: 756e 6465 7220 7465 6d70 6572 6174 7572  under temperatur
+00039360: 6520 7761 726e 696e 6720 7468 7265 7368  e warning thresh
+00039370: 6f6c 6420 6578 6365 6564 6564 2e3c 2f4c  old exceeded.</L
+00039380: 6162 656c 3e0d 0a20 2020 2020 2020 203c  abel>..        <
+00039390: 2f4c 6162 656c 733e 0d0a 2020 2020 2020  /Labels>..      
+000393a0: 3c2f 4572 726f 723e 0d0a 2020 2020 2020  </Error>..      
+000393b0: 3c45 7272 6f72 2069 643d 2230 7830 3030  <Error id="0x000
+000393c0: 3033 3231 3222 2061 6666 6563 7465 645f  03212" affected_
+000393d0: 6d6f 6475 6c65 3d22 5375 7065 7276 6973  module="Supervis
+000393e0: 6f72 2220 6572 726f 725f 7479 7065 3d22  or" error_type="
+000393f0: 6379 636c 6963 223e 0d0a 2020 2020 2020  cyclic">..      
+00039400: 2020 3c4c 6162 656c 733e 0d0a 2020 2020    <Labels>..    
+00039410: 2020 2020 2020 3c4c 6162 656c 206c 616e        <Label lan
+00039420: 673d 2265 6e5f 5553 223e 4761 7465 2076  g="en_US">Gate v
+00039430: 6f6c 7461 6765 206f 7574 206f 6620 6c69  oltage out of li
+00039440: 6d69 7473 3c2f 4c61 6265 6c3e 0d0a 2020  mits</Label>..  
+00039450: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00039460: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00039470: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00039480: 3d22 3078 3030 3030 3435 3031 2220 6166  ="0x00004501" af
+00039490: 6665 6374 6564 5f6d 6f64 756c 653d 2249  fected_module="I
+000394a0: 6e70 7574 7322 2065 7272 6f72 5f74 7970  nputs" error_typ
+000394b0: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+000394c0: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+000394d0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+000394e0: 6c61 6e67 3d22 656e 5f55 5322 3e4c 6f61  lang="en_US">Loa
+000394f0: 6420 6365 6c6c 2068 6561 6c74 6820 7369  d cell health si
+00039500: 676e 616c 2065 7272 6f72 2064 6574 6563  gnal error detec
+00039510: 7465 642e 3c2f 4c61 6265 6c3e 0d0a 2020  ted.</Label>..  
+00039520: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00039530: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00039540: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00039550: 3d22 3078 3030 3030 3435 3032 2220 6166  ="0x00004502" af
+00039560: 6665 6374 6564 5f6d 6f64 756c 653d 2249  fected_module="I
+00039570: 6e70 7574 7322 2065 7272 6f72 5f74 7970  nputs" error_typ
+00039580: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00039590: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+000395a0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+000395b0: 6c61 6e67 3d22 656e 5f55 5322 3e4c 6f61  lang="en_US">Loa
+000395c0: 6420 6365 6c6c 2061 6e61 6c6f 6720 696e  d cell analog in
+000395d0: 7075 7420 6f75 7420 6f66 2072 616e 6765  put out of range
+000395e0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+000395f0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00039600: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00039610: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00039620: 3030 3030 3733 3933 2220 6166 6665 6374  00007393" affect
+00039630: 6564 5f6d 6f64 756c 653d 2243 6f6e 7472  ed_module="Contr
+00039640: 6f6c 206c 6f6f 7073 2220 6572 726f 725f  ol loops" error_
+00039650: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00039660: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00039670: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00039680: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00039690: 4375 7272 656e 7420 6469 7265 6374 2066  Current direct f
+000396a0: 6f6c 6c6f 7769 6e67 2065 7272 6f72 2064  ollowing error d
+000396b0: 6574 6563 7465 643c 2f4c 6162 656c 3e0d  etected</Label>.
+000396c0: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
+000396d0: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
+000396e0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
+000396f0: 2069 643d 2230 7830 3030 3037 3339 3222   id="0x00007392"
+00039700: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
+00039710: 3d22 436f 6e74 726f 6c20 6c6f 6f70 7322  ="Control loops"
+00039720: 2065 7272 6f72 5f74 7970 653d 2263 7963   error_type="cyc
+00039730: 6c69 6322 3e0d 0a20 2020 2020 2020 203c  lic">..        <
+00039740: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00039750: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00039760: 656e 5f55 5322 3e43 7572 7265 6e74 2071  en_US">Current q
+00039770: 7561 6472 6174 7572 6520 666f 6c6c 6f77  uadrature follow
+00039780: 696e 6720 6572 726f 7220 6465 7465 6374  ing error detect
+00039790: 6564 3c2f 4c61 6265 6c3e 0d0a 2020 2020  ed</Label>..    
+000397a0: 2020 2020 3c2f 4c61 6265 6c73 3e0d 0a20      </Labels>.. 
+000397b0: 2020 2020 203c 2f45 7272 6f72 3e0d 0a20       </Error>.. 
+000397c0: 2020 2020 203c 4572 726f 7220 6964 3d22       <Error id="
+000397d0: 3078 3030 3030 3733 3834 2220 6166 6665  0x00007384" affe
+000397e0: 6374 6564 5f6d 6f64 756c 653d 2246 6565  cted_module="Fee
+000397f0: 6462 6163 6b73 2220 6572 726f 725f 7479  dbacks" error_ty
+00039800: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
+00039810: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00039820: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00039830: 206c 616e 673d 2265 6e5f 5553 223e 4162   lang="en_US">Ab
+00039840: 736f 6c75 7465 2065 6e63 6f64 6572 2065  solute encoder e
+00039850: 7272 6f72 2062 6974 2061 6374 6976 6520  rror bit active 
+00039860: 7769 7468 6f75 7420 6578 6365 6564 696e  without exceedin
+00039870: 6720 6572 726f 7220 746f 6c65 7261 6e63  g error toleranc
+00039880: 653c 2f4c 6162 656c 3e0d 0a20 2020 2020  e</Label>..     
+00039890: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+000398a0: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+000398b0: 2020 2020 3c45 7272 6f72 2069 643d 2230      <Error id="0
+000398c0: 7830 3530 3430 3030 3022 2061 6666 6563  x05040000" affec
+000398d0: 7465 645f 6d6f 6475 6c65 3d22 436f 6d6d  ted_module="Comm
+000398e0: 756e 6963 6174 696f 6e73 2220 6572 726f  unications" erro
+000398f0: 725f 7479 7065 3d22 636f 6e66 6967 7572  r_type="configur
+00039900: 6174 696f 6e22 3e0d 0a20 2020 2020 2020  ation">..       
+00039910: 203c 4c61 6265 6c73 3e0d 0a20 2020 2020   <Labels>..     
+00039920: 2020 2020 203c 4c61 6265 6c20 6c61 6e67       <Label lang
+00039930: 3d22 656e 5f55 5322 3e43 4f4d 2d4b 4954  ="en_US">COM-KIT
+00039940: 2054 696d 656f 7574 2e20 434f 5245 2064   Timeout. CORE d
+00039950: 6576 6963 6520 6973 206e 6f74 2070 726f  evice is not pro
+00039960: 7065 726c 7920 636f 6e6e 6563 7465 643c  perly connected<
+00039970: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+00039980: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00039990: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
+000399a0: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
+000399b0: 3030 3046 4634 3222 2061 6666 6563 7465  000FF42" affecte
+000399c0: 645f 6d6f 6475 6c65 3d22 436f 6d6d 756e  d_module="Commun
+000399d0: 6963 6174 696f 6e73 2220 6572 726f 725f  ications" error_
+000399e0: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+000399f0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00039a00: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00039a10: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00039a20: 4574 6865 7243 4154 2063 6162 6c65 2069  EtherCAT cable i
+00039a30: 7320 6469 7363 6f6e 6e65 6374 6564 2064  s disconnected d
+00039a40: 7572 696e 6720 6f70 6572 6174 696f 6e3c  uring operation<
+00039a50: 2f4c 6162 656c 3e0d 0a20 2020 2020 2020  /Label>..       
+00039a60: 203c 2f4c 6162 656c 733e 0d0a 2020 2020   </Labels>..    
+00039a70: 2020 3c2f 4572 726f 723e 0d0a 2020 2020    </Error>..    
+00039a80: 2020 3c45 7272 6f72 2069 643d 2230 7830    <Error id="0x0
+00039a90: 3030 3038 3133 3022 2061 6666 6563 7465  0008130" affecte
+00039aa0: 645f 6d6f 6475 6c65 3d22 436f 6d6d 756e  d_module="Commun
+00039ab0: 6963 6174 696f 6e73 2220 6572 726f 725f  ications" error_
+00039ac0: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00039ad0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00039ae0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00039af0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+00039b00: 4c69 6665 6775 6172 6420 6572 726f 7220  Lifeguard error 
+00039b10: 6f72 2068 6561 7274 6265 6174 2065 7272  or heartbeat err
+00039b20: 6f72 2069 6e20 4341 4e4f 7065 6e20 636f  or in CANOpen co
+00039b30: 6d6d 756e 6963 6174 696f 6e3c 2f4c 6162  mmunication</Lab
+00039b40: 656c 3e0d 0a20 2020 2020 2020 203c 2f4c  el>..        </L
+00039b50: 6162 656c 733e 0d0a 2020 2020 2020 3c2f  abels>..      </
+00039b60: 4572 726f 723e 0d0a 2020 2020 2020 3c45  Error>..      <E
+00039b70: 7272 6f72 2069 643d 2230 7830 3030 3046  rror id="0x0000F
+00039b80: 4634 3322 2061 6666 6563 7465 645f 6d6f  F43" affected_mo
+00039b90: 6475 6c65 3d22 436f 6d6d 756e 6963 6174  dule="Communicat
+00039ba0: 696f 6e22 2065 7272 6f72 5f74 7970 653d  ion" error_type=
+00039bb0: 2263 7963 6c69 6322 3e0d 0a20 2020 2020  "cyclic">..     
+00039bc0: 2020 203c 4c61 6265 6c73 3e0d 0a20 2020     <Labels>..   
+00039bd0: 2020 2020 2020 203c 4c61 6265 6c20 6c61         <Label la
+00039be0: 6e67 3d22 656e 5f55 5322 3e43 7963 6c69  ng="en_US">Cycli
+00039bf0: 6320 7469 6d65 6f75 7420 4574 6865 7263  c timeout Etherc
+00039c00: 6174 2050 444f 206c 6966 6567 7561 7264  at PDO lifeguard
+00039c10: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00039c20: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00039c30: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00039c40: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00039c50: 3030 3030 3733 3934 2220 6166 6665 6374  00007394" affect
+00039c60: 6564 5f6d 6f64 756c 653d 2251 7569 636b  ed_module="Quick
+00039c70: 2073 746f 7022 2065 7272 6f72 5f74 7970   stop" error_typ
+00039c80: 653d 2263 7963 6c69 6322 3e0d 0a20 2020  e="cyclic">..   
+00039c90: 2020 2020 203c 4c61 6265 6c73 3e0d 0a20       <Labels>.. 
+00039ca0: 2020 2020 2020 2020 203c 4c61 6265 6c20           <Label 
+00039cb0: 6c61 6e67 3d22 656e 5f55 5322 3e45 6d65  lang="en_US">Eme
+00039cc0: 7267 656e 6379 2070 6f73 6974 696f 6e20  rgency position 
+00039cd0: 7365 742d 706f 696e 7420 6e6f 7420 636f  set-point not co
+00039ce0: 6e66 6967 7572 6564 2e3c 2f4c 6162 656c  nfigured.</Label
+00039cf0: 3e0d 0a20 2020 2020 2020 203c 2f4c 6162  >..        </Lab
+00039d00: 656c 733e 0d0a 2020 2020 2020 3c2f 4572  els>..      </Er
+00039d10: 726f 723e 0d0a 2020 2020 2020 3c45 7272  ror>..      <Err
+00039d20: 6f72 2069 643d 2230 7830 3030 3046 3031  or id="0x0000F01
+00039d30: 3122 2061 6666 6563 7465 645f 6d6f 6475  1" affected_modu
+00039d40: 6c65 3d22 434f 434f 2220 6572 726f 725f  le="COCO" error_
+00039d50: 7479 7065 3d22 636f 6e66 6967 7572 6174  type="configurat
+00039d60: 696f 6e22 3e0d 0a20 2020 2020 2020 203c  ion">..        <
+00039d70: 4c61 6265 6c73 3e0d 0a20 2020 2020 2020  Labels>..       
+00039d80: 2020 203c 4c61 6265 6c20 6c61 6e67 3d22     <Label lang="
+00039d90: 656e 5f55 5322 3e43 7963 6c69 6320 6d6f  en_US">Cyclic mo
+00039da0: 6465 206d 6170 7069 6e67 2065 7272 6f72  de mapping error
+00039db0: 3c2f 4c61 6265 6c3e 0d0a 2020 2020 2020  </Label>..      
+00039dc0: 2020 3c2f 4c61 6265 6c73 3e0d 0a20 2020    </Labels>..   
+00039dd0: 2020 203c 2f45 7272 6f72 3e0d 0a20 2020     </Error>..   
+00039de0: 2020 203c 4572 726f 7220 6964 3d22 3078     <Error id="0x
+00039df0: 3030 3030 3232 3843 2220 6166 6665 6374  0000228C" affect
+00039e00: 6564 5f6d 6f64 756c 653d 2250 6f77 6572  ed_module="Power
+00039e10: 2073 7461 6765 2220 6572 726f 725f 7479   stage" error_ty
+00039e20: 7065 3d22 6379 636c 6963 223e 0d0a 2020  pe="cyclic">..  
+00039e30: 2020 2020 2020 3c4c 6162 656c 733e 0d0a        <Labels>..
+00039e40: 2020 2020 2020 2020 2020 3c4c 6162 656c            <Label
+00039e50: 206c 616e 673d 2265 6e5f 5553 223e 4375   lang="en_US">Cu
+00039e60: 7272 656e 7420 6361 6c69 6272 6174 696f  rrent calibratio
+00039e70: 6e20 6572 726f 723c 2f4c 6162 656c 3e0d  n error</Label>.
+00039e80: 0a20 2020 2020 2020 203c 2f4c 6162 656c  .        </Label
+00039e90: 733e 0d0a 2020 2020 2020 3c2f 4572 726f  s>..      </Erro
+00039ea0: 723e 0d0a 2020 2020 2020 3c45 7272 6f72  r>..      <Error
+00039eb0: 2069 643d 2230 7830 3030 3037 3337 4522   id="0x0000737E"
+00039ec0: 2061 6666 6563 7465 645f 6d6f 6475 6c65   affected_module
+00039ed0: 3d22 4665 6564 6261 636b 7322 2065 7272  ="Feedbacks" err
+00039ee0: 6f72 5f74 7970 653d 2263 7963 6c69 6322  or_type="cyclic"
+00039ef0: 3e0d 0a20 2020 2020 2020 203c 4c61 6265  >..        <Labe
+00039f00: 6c73 3e0d 0a20 2020 2020 2020 2020 203c  ls>..          <
+00039f10: 4c61 6265 6c20 6c61 6e67 3d22 656e 5f55  Label lang="en_U
+00039f20: 5322 3e41 6273 6f6c 7574 6520 656e 636f  S">Absolute enco
+00039f30: 6465 7220 3120 6469 7363 6f6e 6e65 6374  der 1 disconnect
+00039f40: 696f 6e20 6f72 2066 7261 6d65 206f 7665  ion or frame ove
+00039f50: 726c 6170 3c2f 4c61 6265 6c3e 0d0a 2020  rlap</Label>..  
+00039f60: 2020 2020 2020 3c2f 4c61 6265 6c73 3e0d        </Labels>.
+00039f70: 0a20 2020 2020 203c 2f45 7272 6f72 3e0d  .      </Error>.
+00039f80: 0a20 2020 2020 203c 4572 726f 7220 6964  .      <Error id
+00039f90: 3d22 3078 3030 3030 3733 3746 2220 6166  ="0x0000737F" af
+00039fa0: 6665 6374 6564 5f6d 6f64 756c 653d 2246  fected_module="F
+00039fb0: 6565 6462 6163 6b73 2220 6572 726f 725f  eedbacks" error_
+00039fc0: 7479 7065 3d22 6379 636c 6963 223e 0d0a  type="cyclic">..
+00039fd0: 2020 2020 2020 2020 3c4c 6162 656c 733e          <Labels>
+00039fe0: 0d0a 2020 2020 2020 2020 2020 3c4c 6162  ..          <Lab
+00039ff0: 656c 206c 616e 673d 2265 6e5f 5553 223e  el lang="en_US">
+0003a000: 4162 736f 6c75 7465 2065 6e63 6f64 6572  Absolute encoder
+0003a010: 2032 2064 6973 636f 6e6e 6563 7469 6f6e   2 disconnection
+0003a020: 206f 7220 6672 616d 6520 6f76 6572 6c61   or frame overla
+0003a030: 703c 2f4c 6162 656c 3e0d 0a20 2020 2020  p</Label>..     
+0003a040: 2020 203c 2f4c 6162 656c 733e 0d0a 2020     </Labels>..  
+0003a050: 2020 2020 3c2f 4572 726f 723e 0d0a 2020      </Error>..  
+0003a060: 2020 3c2f 4572 726f 7273 3e0d 0a20 203c    </Errors>..  <
+0003a070: 2f42 6f64 793e 0d0a 2020 3c44 7269 7665  /Body>..  <Drive
+0003a080: 496d 6167 6520 656e 636f 6469 6e67 3d22  Image encoding="
+0003a090: 7873 3a62 6173 6536 3442 696e 6172 7922  xs:base64Binary"
+0003a0a0: 3e0d 0a20 2020 2069 5642 4f52 7730 4b47  >..    iVBORw0KG
+0003a0b0: 676f 4141 4141 4e53 5568 4555 6741 4141  goAAAANSUhEUgAAA
+0003a0c0: 4d67 4141 4144 4943 4159 4141 4143 7457  MgAAADICAYAAACtW
+0003a0d0: 4b36 6541 4141 4141 584e 5352 3049 4172  K6eAAAAAXNSR0IAr
+0003a0e0: 7334 6336 5141 4141 4152 6e51 5531 4241  s4c6QAAAARnQU1BA
+0003a0f0: 4143 786a 7776 3859 5155 4141 4141 4a63  ACxjwv8YQUAAAAJc
+0003a100: 4568 5a63 7741 4144 734d 4141 4137 4441  EhZcwAADsMAAA7DA
+0003a110: 6364 7671 4751 4141 4663 5a53 5552 4256  cdvqGQAAFcZSURBV
+0003a120: 4868 6537 5630 486f 4231 4631 5a37 5a33  Hhe7V0HoB1F1Z7Z3
+0003a130: 6474 6554 6538 6b49 5130 496b 4143 6874  dteTe8kIQ0IkACht
+0003a140: 7841 3651 5a71 5141 4649 6943 4b69 4149  xA6QZqQAFIiCKiAI
+0003a150: 6943 6950 3070 4152 5542 4651 4552 4538  iCiP0pARUBFQERE8
+0003a160: 5564 4535 5366 3836 692b 3968 3935 4454  UdE5Sf86i+9h95DT
+0003a170: 3267 7870 7666 6b35 6456 6264 6e66 6d50  2gxpvfk5dVbdnfmP
+0003a180: 2b66 4d7a 4f37 652b 2b35 4c58 704b 5876  +fMzO7e++5LXpKXv
+0003a190: 4276 5937 3932 6463 2b62 4d37 4d37 7337  BvY792dc+bM7M7s7
+0003a1a0: 4878 375a 7259 3946 694e 476a 4267 7859  Hx7ZrY9FiNGjBgxY
+0003a1b0: 7353 4945 534e 476a 4267 7859 7353 4945  sSIESNGjBgxYsSIE
+0003a1c0: 534e 476a 4267 7859 7353 4945 534e 476a  SNGjBgxYsSIESNGj
+0003a1d0: 4267 7859 7353 4945 534e 476a 4267 7859  BgxYsSIESNGjBgxY
+0003a1e0: 7353 4945 534e 476a 4267 7859 7353 4945  sSIESNGjBgxYsSIE
+0003a1f0: 534e 476a 4267 7859 7353 4945 534e 476a  SNGjBgxYsSIESNGj
+0003a200: 4267 7859 7353 4945 534e 476a 4267 7859  BgxYsSIESNGjBgxY
+0003a210: 7353 4945 534e 476a 4267 7859 7353 4945  sSIESNGjBgxYsSIE
+0003a220: 534e 476a 4267 7859 7353 4945 534e 476a  SNGjBgxYsSIESNGj
+0003a230: 4267 7859 7353 4945 534e 476a 4330 4772  BgxYsSIESNGjC0Gr
+0003a240: 6d57 4d72 5977 4a53 7837 7349 3277 3579  mWMrYwJSx7sI2w5y
+0003a250: 4c4f 5344 7663 4c44 596b 4279 7866 5034  LOSDvcLDYkByxfP4
+0003a260: 6c39 3364 584b 4d43 6b46 4d6b 4b32 4d76  l93dXKMCkFMkK2Mv
+0003a270: 5663 2f57 7063 5834 7475 6338 334f 6b6b  Vc/WpcX4tuc83Okk
+0003a280: 4c31 4232 6c4b 4946 736e 592b 3562 774c  L1B2lKIFsnY+5bwL
+0003a290: 3331 3334 4473 664d 3336 7430 4e6c 6a64  3134DsfM36t0Nljd
+0003a2a0: 444e 6967 6d78 466a 462f 392b 4e35 632b  DNigmxFjF/9+N5c+
+0003a2b0: 6a65 4265 6941 4452 6968 494a 7255 7570  jeBeiADRihIJrUup
+0003a2c0: 567a 486d 6678 6c6a 2f36 314e 7a37 504a  VzHmfxlj/61Nz7PJ
+0003a2d0: 336e 4b47 714d 3745 524e 6b4b 3243 5835  3nKGqM7ERNkK2CX5
+0003a2e0: 662f 7162 3976 4f4e 3445 4c56 3348 4f6e  f/qb9vON4ELV3HOn
+0003a2f0: 484c 6b43 4253 4269 6e78 5a57 4f79 4b44  HLkCBSBinxZWOyKD
+0003a300: 3137 4976 386d 6d54 7656 5651 6f7a 7551  17Iv8mmTvVVQozuQ
+0003a310: 4579 514c 5969 4a4d 3263 366a 654f 7a42  EyQLYiJM2c6jeOzB
+0003a320: 7a42 502f 6736 6165 6779 3074 6855 7967  zBP/g6aegy0thUyg
+0003a330: 6a79 4755 6254 456e 394c 4231 4d69 6b2b  jyGUbTEn9LB1Mik+
+0003a340: 454f 3274 666b 6e63 3865 6331 5554 4747  EO2tfknc8ec1UTGG
+0003a350: 4673 644d 5547 3245 4361 736e 5648 7669  FsdMUG2ECasnVHvi
+0003a360: 396f 6651 452f 2f46 6b53 7279 4e68 4a63  9ofQE//FkSryNhJc
+0003a370: 6968 4242 6761 546b 5265 5939 4c2f 2f34  ihBBgaTkReY9L//4
+0003a380: 5a41 7676 3070 704d 6259 7159 6f4a 304d  ZAvv0ppMbYqYoJ0M
+0003a390: 6162 4947 6661 2f56 3164 5046 4a7a 667a  abIGfa/V1dPFJzfz
+0003a3a0: 7158 6351 5449 5956 4246 5568 7963 7451  qXcQTIYVBFUhyctQ
+0003a3b0: 7053 5149 4a6f 654a 6c41 2f73 674d 4b51  pSQIJoeJlA/sgMKQ
+0003a3c0: 4a49 626d 4d6a 6438 7347 774d 7872 5145  JIbmMjd8sGwMxrQE
+0003a3d0: 4750 7249 435a 4946 324b 7678 662f 6f37  GPrICZIF2Kvxf/o7
+0003a3e0: 6159 7950 2b52 636e 6766 526d 7041 4870  aYyP+RcngfRmpAHp
+0003a3f0: 7264 6a66 772b 4d70 7650 725a 4a4e 4832  rdjfw+MpvPrZJNH2
+0003a400: 5652 5378 435a 6764 734c 6b65 7861 3376  VRSxCZgdsLkexa3v
+0003a410: 746c 7a37 6a75 7a6e 7039 3062 5479 4a33  tlz7juznp90bTyJ3
+0003a420: 7771 4943 644a 4647 4c66 716b 554d 7479  wqICdJFGLfqkUMty
+0003a430: 3771 5253 3759 6e64 756a 4e49 5565 7844  7qRS7YndujNIUexD
+0003a440: 654e 4b30 6576 4466 4554 6556 734f 3836  eNK0evDfETeVsO86
+0003a450: 3134 6265 6d71 5745 6d4a 734d 6351 4532  14bemqWEmJsMcQE2
+0003a460: 557a 6744 5438 2f6e 6667 4f39 4e34 724f  UzgDT8/nfgO9N4rO
+0003a470: 654d 4f64 5733 5473 5573 3665 576a 5747  eMOdW3TsUs6eWjWG
+0003a480: 6956 4838 6d68 3967 7a5a 6743 6d78 6946  iVH8mh9gzZgCmxiF
+0003a490: 7066 6574 7a38 6350 7656 3147 4d58 4639  pfetz8cPvV1GMXF9
+0003a4a0: 3032 3245 474b 4362 4349 6d79 706c 4f38  022EGKCbCImyplO8
+0003a4b0: 2b72 4377 594c 3774 774d 7878 6f44 4a30  +rCwYL7twMxxoDJ0
+0003a4c0: 7431 5964 2b52 4968 305a 3732 4c6d 3167  t1Yd+RIh0Z72Lm1g
+0003a4d0: 6d70 786e 6d43 564d 4c50 2b6d 5151 304b  mpxnmCVMLP+mQQ0K
+0003a4e0: 5957 4546 4531 672f 3633 446e 5276 6632  YWEFE1g/63DnRvf2
+0003a4f0: 2f36 6b64 5a51 516f 3073 5245 3251 5441  /6kdZQQo0sRE2QTA
+0003a500: 4636 6a79 7338 6b70 384d 6b2f 434b 4956  F6jys8kp8Mk/CKIV
+0003a510: 7176 4f75 776e 6b49 4555 4836 6f63 4a47  qvOuwnkIEUH6ocJG
+0003a520: 4161 7972 4530 5a64 534c 4735 6175 577a  AayrE0ZdSLG5auWz
+0003a530: 6237 3934 6241 7062 796c 4c6a 4b35 4354  b794bApbylLjK5CT
+0003a540: 4a43 4e67 5a54 5748 7175 6650 4552 5938  JCNgZTWHqufPERY8
+0003a550: 685a 6f75 4633 4448 6f6f 2f30 3247 4e52  hZouF3DHoo/02GNR
+0003a560: 4777 6b4f 5149 6c59 6776 794b 686e 5974  GwkOQIlYgvyKhnYt
+0003a570: 426b 5653 7049 6943 2b6f 4e43 5476 3536  BkVSpIiC+oNCTv56
+0003a580: 3969 6264 4231 6967 6e51 4f66 4e39 316a  9ibdB1ignQOfN91j
+0003a590: 2f66 4d43 2f5a 3936 4e77 5877 5a43 714b  /fMC/Z96NwXwZCqK
+0003a5a0: 7569 6871 7363 472f 5468 5555 4456 3579  uihqscG/ThUUDV5y
+0003a5b0: 746c 3045 4552 4448 664f 725a 4a4f 6f5a  tl0EERDHfOrZJOoZ
+0003a5c0: 4c46 4e42 536f 4b41 5571 4a39 2b48 6c42  LFNBSoKAUqJ9+HlB
+0003a5d0: 3879 3276 7435 7677 5966 786c 6134 7551  8y2vt5vwYfxla4uQ
+0003a5e0: 4579 5154 6d44 5074 5939 4f46 4a4c 6642  EyQTmDPtY9OFJLfB
+0003a5f0: 4a50 6843 5547 4844 4d51 4779 4945 774f  JPhCUGHDMQGyIEwO
+0003a600: 6b69 3969 6771 4d4f 6443 5656 4371 4667  ki9igqMOdCVVCqFg
+0003a610: 6232 7354 5564 4c74 7739 6c72 774f 5038  b2sTUdLtw9lrwOP8
+0003a620: 6c74 7656 4938 667a 3755 6d35 3156 696a  ltvVI8fz7Um51Vij
+0003a630: 4531 4254 4a44 3159 4e64 3144 2f64 3070  E1BTJD1YNd1D/d0p
+0003a640: 484d 706e 4a65 2f7a 7a6c 5071 4835 6f4f  HMpnJe/zzlPqH5oO
+0003a650: 714d 4b67 6b36 4b42 704d 5547 6a45 5353  qMKgk6KBpMUGjESS
+0003a660: 4e4c 4367 4152 5a64 5454 4967 3269 336e  NLCgARZdTTIg2i3n
+0003a670: 6f6d 7277 4551 6a69 6c4a 314f 6f57 5376  omrwEQjilJ1OoWSv
+0003a680: 6336 6c75 4f53 6a4d 5a2b 3847 5438 6876  c6luOSjMZ+8GT8hv
+0003a690: 476d 4943 5649 4765 4957 7161 5a30 3745  GmICVIGeIWqaZ07E
+0003a6a0: 5472 5862 6444 4c64 6754 5041 664e 7854  TrXbdDLdgTPAfNxT
+0003a6b0: 4e47 6455 6575 6843 514b 5446 4852 5967  NGdUeuhCQKTFHRYg
+0003a6c0: 4e46 7834 4d4e 5943 3269 3159 5562 3855  NFx4MNYC2i1YUb8U
+0003a6d0: 6144 6a53 7346 5143 7546 696b 5742 4c6b  aDjSsFQCuFikWBLk
+0003a6e0: 6f32 5354 4e37 316b 494e 5570 5154 316b  o2STN71kINUpQT1k
+0003a6f0: 4c49 5a6b 6e39 7465 6661 7635 7578 7936  LIZkn9tefav5uxy6
+0003a700: 6c70 6c6a 4e46 5a57 4672 4730 426a 326e  lpljNFZWFrG0Bj2n
+0003a710: 356e 7070 6f62 4339 5543 4f66 3046 304a  5nppobC9UCOf0F0J
+0003a720: 7949 4870 5a67 4f46 7753 6872 714e 684c  yIHpZgOFwShrqNhL
+0003a730: 7755 4548 5254 3477 646c 6649 5835 5630  wUEHRT4wdlfIX5V0
+0003a740: 4773 684c 434b 4856 6967 5a46 706a 6a7a  GshLCKHVigZFpjjz
+0003a750: 4146 536e 5174 3531 7167 3154 4e34 4945  AFSnQt51qg1TN4IE
+0003a760: 634b 5651 3574 5241 6b6b 686b 4a4a 6435  cKVQ5tRAkkhkJJd5
+0003a770: 5365 3878 3064 2f38 7566 785a 496e 5261  Se8x0d/8ufxZInRa
+0003a780: 6351 454d 5a44 536d 7444 7732 4347 3936  cQEMZDSmtDw2CG96
+0003a790: 7773 7663 6336 2b43 3836 316d 7378 4259  wsvcc6+C861msxBY
+0003a7a0: 4b53 4b46 4864 6356 4b6e 4c4b 2b67 4f43  KSKFHdcVKnLK+gOC
+0003a7b0: 6d4b 6838 4d55 3576 5162 556e 674f 5768  mKh8MU5vQbUngOWh
+0003a7c0: 535a 2f4f 334a 456f 7753 5a2b 3344 3479  SZ/O3JEowSZ+3D4y
+0003a7d0: 582b 4667 374d 3336 4938 4263 5743 7958  X+Fg7M36I8BcWCyX
+0003a7e0: 5549 4f72 5563 3852 5342 4a43 774d 5643  UIOrUc8RSBJCwMVC
+0003a7f0: 7259 5839 2b30 5878 3879 3539 3063 6a2f  rYX9+0Xx8y590cj/
+0003a800: 6a32 6a6e 684a 6962 4241 7851 5141 546d  j2jnhJibBAxQQATm
+0003a810: 6d62 326d 6444 3439 4930 7745 5838 5554  mb2mdD49I0wEX8UT
+0003a820: 7438 546c 4c57 6b6f 3455 5233 5265 5672  t8TlLWko4UR3ReVr
+0003a830: 7443 4f48 446b 5166 374d 4c2f 6e34 6644  tCOHDkQf7ML/n4fD
+0003a840: 446e 6854 3848 4c54 3542 5576 4b6f 794b  DnhT8HLT5BUvKoyK
+0003a850: 4a73 3247 676e 3459 4e67 7038 394b 7231  Js2Ggn4YNgp89Kr1
+0003a860: 3577 4133 7578 634d 4339 5256 724d 435a  5wA3uxcMC9RVrMCZ
+0003a870: 6931 5a42 7952 7059 6143 4554 6764 6657  i1ZByRpYaCETgdfW
+0003a880: 4176 7538 466f 376c 3339 6831 4876 3337  Avu8Fo7l39h1Hv37
+0003a890: 6f73 5056 6c4a 436a 4137 7878 5361 496c  osPVlJCjA7xxSaIl
+0003a8a0: 4879 5074 5938 644a 4958 376c 4a54 6975  HyPtY8dJIX7lJTiu
+0003a8b0: 7a43 6179 6c42 6e43 6a6f 6139 5337 3636  zCaylBnCjoa9S766
+0003a8c0: 5544 334e 6155 6275 2b35 2f4b 6c47 7946  UD3NaUbu+5/KlGyF
+0003a8d0: 6142 394a 5446 6734 4666 6647 5862 6955  aB9JTFg4FffGXbiU
+0003a8e0: 7057 676f 4c49 486d 6330 7674 476b 5a5a  pWgoLIHmc0vtGkZZ
+0003a8f0: 4148 4d32 7650 7237 7577 5270 2f34 4642  AHM2vPr7uwRp/4FB
+0003a900: 6c34 4851 4230 6668 4258 555a 4c74 6b6e  l4HQB0fhBXUZLtkn
+0003a910: 5842 626b 5167 4a4d 7067 496b 7a42 2b67  XBbkQgJMpgIkzB+g
+0003a920: 346e 6e4f 4d75 576a 3738 334f 2f76 6a67  4nnOMuWj783O/vjg
+0003a930: 572f 6471 5237 466a 3145 5758 3169 4334  W/dqR7Fj1EWX1iC4
+0003a940: 4257 7133 6463 392b 5450 4a2b 5a50 5179  BWq3dc9+TPJ+ZPQy
+0003a950: 5862 545a 674a 314b 644f 7649 6f68 3258  XbTZgJ1KdOvIoh2X
+0003a960: 4a4d 6532 4351 7253 4346 6e4d 4f62 732b  JMe2CQrSCFnMObs+
+0003a970: 3936 4134 2f34 3569 2b39 5a35 674d 4d59  96A4/45i+9Z5gMMY
+0003a980: 655a 514c 6436 514d 5a64 4166 6a54 696c  eZQLd6QMZdAfjTil
+0003a990: 4157 7558 7a73 5676 4d5a 4655 4d37 536f  AWuXzsVvMZFUM7So
+0003a9a0: 6e77 514b 534b 4342 746b 6f71 7152 524e  nwQKSKCBtkoqqRRN
+0003a9b0: 5743 5978 662b 724a 7056 3565 7654 7350  WCYxf+rJpV5evTsP
+0003a9c0: 2b2f 4470 6b2b 5052 784e 6c38 4956 7246  +/Dpk+PRxNl8IVrF
+0003a9d0: 4c78 4374 5566 4445 3463 6d57 5049 464f  LxCtUfDE4cmWPIFO
+0003a9e0: 4a50 6941 345a 706e 5153 6478 3369 4f49  JPiA4ZpnQSdx3iOI
+0003a9f0: 416a 306b 4279 6747 4630 5a6f 632f 4b68  Aj0kBygGF0Zoc/Kh
+0003aa00: 5842 6d50 6e32 4867 626d 7676 4466 776d  XBmPn2HgbmvvDfwm
+0003aa10: 506d 5531 6735 2b5a 4430 7441 6e4a 4542  PmU1g5+ZD0tAnJEB
+0003aa20: 4e6d 306f 5152 7a78 307a 4f66 7a54 7131  Nm0oQRzx0zOfzTq1
+0003aa30: 4e38 3573 7241 5035 5067 5872 4f2f 716c  N85srAP5PgXrO/ql
+0003aa40: 5367 3971 4353 496b 4277 6d6a 6c49 6274  Sg9qCSIkBwmjlIbt
+0003aa50: 4652 4337 6963 392b 6654 494c 772b 2f65  FRC7ic9+fTILw+/e
+0003aa60: 7363 3539 2f53 6d68 4267 4276 6c41 4577  sc59/SmhBgBvlAEw
+0003aa70: 532b 4b74 4452 3676 3443 6846 4636 6832  S+KtDR6v4ChFF6h2
+0003aa80: 6757 5738 444a 3370 4850 7049 4e42 4e45  gWW8DJ3pHPpINBNE
+0003aa90: 686b 6975 6c43 5435 2f75 6b57 7a6a 672f  hkiulCT5/ukWzjg/
+0003aaa0: 6635 662b 7363 4476 4250 766a 3850 4763  f5f+scDvBPvj8PGc
+0003aab0: 424f 6169 6e70 374f 6c5a 5568 3437 7877  BOainp7OlZUh47xw
+0003aac0: 5a69 7a46 6d66 7474 744d 7379 6334 426b  ZizFmftttMsyc4Bk
+0003aad0: 717a 516d 3141 4157 5579 4f30 6d30 7271  qzQm1AAWUyO0m0rq
+0003aae0: 5954 5359 5735 5341 334f 5471 3131 5850  YTSYW5SA3OTq11XP
+0003aaf0: 6a58 7976 662f 6549 2f59 6d49 6234 5944  jXyvf/eI/YmIb4YD
+0003ab00: 5948 5055 4948 5838 4250 3230 7844 3544  YHPUIHX8BP20xD5D
+0003ab10: 6e53 4c6d 7144 4449 4d70 3047 7432 7254  nSLmqDDIMp0Gt2rT
+0003ab20: 4177 4157 6841 4275 3543 4c49 5a7a 6d39  AwAWhABu5CLIZzm9
+0003ab30: 4276 3431 512b 324f 336d 7854 6c67 2f6f  Bv41Q+2O3mxTlg/o
+0003ab40: 4944 494a 6a53 3059 756f 5432 4e65 5042  IDIJjS0YuoT2NePB
+0003ab50: 6475 666b 3573 7a35 7253 2f63 6a74 7845  dufk5sz5rS/cjtxE
+0003ab60: 5050 6c76 3642 4350 7135 4c4a 5a68 7442  PPlv6BCPq5LJZhtB
+0003ab70: 4e73 736c 6b6f 596d 3137 6772 4d47 5a33  NsslkoYm17grMGZ3
+0003ab80: 4a31 4c2f 757a 4945 3464 6650 654b 744f  J1L/uzIE4dfPeKtO
+0003ab90: 2b4d 7258 5944 5050 5546 3261 3371 304c  +MrXYDPPUF2a3q0L
+0003aba0: 3136 6841 6c2f 7843 4d78 5139 314a 3951  16hAl/xCMxQ91J9Q
+0003abb0: 3363 4f68 4f6b 306b 6242 496d 4d44 5970  3cOhOk0kbBImMDYp
+0003abc0: 4d67 4c6d 4776 596c 7250 3342 774f 4f2f  MgLmGvYlrP3BwOO/
+0003abd0: 3176 3575 6359 4755 4c62 446f 6d4b 437a  1v5ucYGULbDomKCz
+0003abe0: 742f 302f 6d6a 554b 5a2f 7475 714e 7a73  t/0/mjUKZ/tuqNzs
+0003abf0: 7054 3841 7641 6d69 3030 3977 2f33 5368  pT8AvAmi009w/3Sh
+0003ac00: 6949 526a 5a67 6345 4371 6c6e 6b74 784e  iIRjZgcECqlnktxN
+0003ac10: 624f 635a 3066 4f75 6d73 2f4e 754f 4c66  bOcZ0fOums/NuOLf
+0003ac20: 6158 7263 3073 5176 4951 3559 6531 5442  aXrc0sQvIQ5Ye1TB
+0003ac30: 3172 4365 5261 4f2f 4f55 3431 7767 3667  1rCeRaO/OU41wg6g
+0003ac40: 6f46 5753 5268 7a6b 4178 4b71 5532 794a  oFWSRhzkAxKqU2yJ
+0003ac50: 554b 7971 6437 7137 466c 7639 7a74 6d6d  UKyqd7q7Flv9ztmm
+0003ac60: 625a 3247 7253 5a73 7553 4177 4567 4d4e  bZ2GrSZsuSAwEgMN
+0003ac70: 2f4b 6845 427a 6166 624c 6a36 5863 4c79  /KhEBzafbLj6XcLy
+0003ac80: 396b 586f 7638 4545 744e 6c35 5743 546b  9kXov8EEtNl5WCTk
+0003ac90: 5732 4835 6175 6775 4878 5577 5562 6568  W2H5auguHxUwUbeh
+0003aca0: 4f30 4238 3672 4852 3435 7176 6d62 5570  O0B86rHR45qvmbUp
+0003acb0: 2f66 5736 6451 7648 4436 5842 426e 6638  /fW6dQvHD6XBBnf8
+0003acc0: 4d38 652f 3237 7338 5174 6d73 3866 6853  M8e/27s8Qtms8fhS
+0003acd0: 4a66 4d4e 614a 536e 7a31 4e59 4e4c 5162  JfMNaJSnz1NYNLQb
+0003ace0: 6e54 734d 4979 3549 5037 4859 6e7a 6942  nTsMIy5IP7HYnziB
+0003acf0: 774f 4f65 3344 4f4c 6c4d 4c4f 6e58 6a59  wOOe3DOLlMLOnXjY
+0003ad00: 445a 7142 4d6d 6749 4257 6136 4d59 434a  DZqBMmgIBWa6MYCJ
+0003ad10: 684b 6637 5844 7145 742f 7565 546f 6331  hKf7XDqEt/ueToc1
+0003ad20: 6d39 4372 5a64 4864 6b4b 4652 6557 6266  m9CrZdHdkKFReWbf
+0003ad30: 5952 416d 3946 6754 4167 5962 7456 4a49  YRAm9FgTAgYbtVJI
+0003ad40: 6134 536a 626e 4852 3735 7835 2f36 5148  a4SjbnHR75x5/6QH
+0003ad50: 7262 6a46 7753 6671 7833 474b 3151 7436  rbjFwSfqx3GK1Qt6
+0003ad60: 3777 446d 5356 7667 594d 3844 7659 4f68  7wDmSVvgYM8DvYOh
+0003ad70: 7455 7154 5231 3430 784d 4157 6d2f 5853  tUqTR140xMAWm/XS
+0003ad80: 5541 4a73 3547 2b67 4450 7269 6e66 3748  UAJs5G+gDPrinf7H
+0003ad90: 7631 3336 4953 622f 4d44 6672 6776 2b63  v136ISb/MDfrgv+c
+0003ada0: 514a 7337 5a2f 596b 384d 7964 4546 616a  QJs7Z/Yk8MydEFaj
+0003adb0: 3954 6c39 546b 6a70 3649 3332 4753 4d66  9Tl9Tkjp6I32GSMf
+0003adc0: 7564 5067 336e 4375 6731 4963 547a 3441  udPg3nCug1IcTz4A
+0003add0: 3774 3450 3556 554b 6f55 6b74 615a 734b  7t4P5VUKoUktaZsK
+0003ade0: 6a48 4d49 3167 6231 5078 6e57 5a48 3733  jHMI1gb1PxnWZH73
+0003adf0: 644a 3976 7255 477a 5638 4566 4734 3879  dJ9vrUGzV8EfG48y
+0003ae00: 4b37 7258 757a 5a33 4f7a 6642 4876 304d  K7rXuzZ3OzfBHv0M
+0003ae10: 4854 4338 546a 704e 4563 384f 4d67 4775  HTC8TjpNEc8OMgGu
+0003ae20: 6a4d 6f45 7752 426b 756d 6b43 4a47 4869  jMoEwRBkumkCJGHi
+0003ae30: 666a 2f67 4f76 5939 3932 2b78 2f7a 7635  fj/gOvY992+x/zv5
+0003ae40: 7043 6a47 4e45 7941 4c6f 4f37 6575 7965  pCjGNEyALoO7euye
+0003ae50: 6668 7339 3638 7545 636b 2b70 384e 7761  fhs968uEck+p8Nwa
+0003ae60: 526f 4d43 3565 4532 3159 464b 4655 5842  RoMC5eE21YFKFUXB
+0003ae70: 6c4a 7279 7159 5369 2f4e 7756 6957 6b2f  lJryqYSi/NwViWk/
+0003ae80: 4847 5370 575a 752f 2b59 6465 3339 5235  HGSpWZu/+Yde39R5
+0003ae90: 6962 6250 6b48 6b64 4776 5070 6963 6e4a  ibbPkHkdGvPpicnJ
+0003aea0: 717a 7345 7a43 3578 492b 3030 544e 5535  qzsEzC5xI+00TNU5
+0003aeb0: 7341 5748 5753 4536 5178 686f 4246 3258  sAWHWSE6QxhoBF2X
+0003aec0: 446a 724c 6d58 5350 7376 7431 7a5a 7454  DjrLmXSPsvt1zZtT
+0003aed0: 7638 764c 512f 3930 4762 436c 4530 416a  v8vLQ/90GbClE0Aj
+0003aee0: 534b 6d58 424e 4831 5369 6242 3778 764d  SKmXBNH1SibB7xvM
+0003aef0: 6e65 5873 2f2b 6173 4f78 4a73 4e45 4859  neXs/+asOxJsNEHY
+0003af00: 4c74 4563 7470 3855 4561 6b54 7471 4746  LtEctp8UEakTtqGF
+0003af10: 744c 434c 4d5a 6977 576c 6e56 7961 734a  tLCLMZiwWlnVyasJ
+0003af20: 3759 6675 7561 6148 5636 3643 782b 452f  7YfuuaaHV66Cx+E/
+0003af30: 4678 6a6d 7959 4950 6b4f 315a 394f 4231  FxjmyYIPkO1Z9OB1
+0003af40: 384d 5a38 6e45 5954 6532 6c68 692b 4134  8MZ8nEYTe2lhi+A4
+0003af50: 4543 484f 6947 716d 364f 764d 706b 6b6d  ECHOiGqm6OvMpkkm
+0003af60: 4676 4947 556b 704a 377a 6237 3567 4835  FvIGUkpJ7zb75gH5
+0003af70: 7642 4e6e 4774 3041 4632 5543 6f72 4c44  vBNnGt0AF2UCorLD
+0003af80: 5147 474c 6e4a 5641 5437 612b 597a 5050  QGGLnJVAT7a+YzPP
+0003af90: 7676 662f 357a 4768 4c68 5143 4c6c 5946  vvf/5zGhLhQCLlYF
+0003afa0: 7736 496c 472b 554d 456b 4639 464f 536f  w6IlG+UMEkF9FOSo
+0003afb0: 504c 3167 4f6e 4956 546e 4865 3262 6f4b  PL1gOnIVTnHe2boK
+0003afc0: 3363 6338 486d 2b62 374a 4e7a 6b46 6f72  3cc8Hm+b7JNzkFor
+0003afd0: 7445 7339 2b48 5376 7773 4f31 7737 5275  tEs9+HSvwsO1w7Ru
+0003afe0: 555a 3455 4645 4e6a 4946 655a 4663 5248  UZ4UFENjIFeZFcRH
+0003aff0: 5a58 7a42 6550 6639 7671 3050 4e48 5678  ZXzBePf9vq0PNHVx
+0003b000: 4544 6748 4551 4938 632b 7772 6c46 7967  EDgHEQI8c+wrlFyg
+0003b010: 424b 7877 652f 316a 3065 6475 6c6c 7a6b  BKxwe/1j0edullzk
+0003b020: 4c4b 4158 6a33 6976 5876 3751 7276 6444  LKAXj3ivXv7QrvdD
+0003b030: 7048 6a77 554c 766d 3054 6249 7953 446b  pHjwULvm0TbIySDk
+0003b040: 6d58 496f 614b 366f 7044 6541 7348 4e30  mXIoaK6opDeAsHN0
+0003b050: 7063 334c 7a7a 6f77 732f 6456 782b 334f  pc3Lzzows/dVx+3O
+0003b060: 6562 6a33 6644 575a 7639 586a 506d 5077  ebj3fDWZv9XjPmPw
+0003b070: 6668 3678 3830 6e42 7878 614b 6634 6d48  fh6x80nBxxaKf4mH
+0003b080: 4f66 5139 2f74 4f66 6d68 4c6b 4950 6734  OfQ9/tOfmhLkIPg4
+0003b090: 3031 324b 4651 5848 384c 5946 446b 4930  012KFQXH8LYFDkI0
+0003b0a0: 6270 334a 5469 5838 3359 3765 7957 7637  bp3JTiX83Y7eyWv7
+0003b0b0: 6e2b 6d5a 507a 7259 4947 6870 4334 4c5a  n+mZPzrYIGhpC4LZ
+0003b0c0: 4569 4755 6f6d 7155 7054 5a32 5048 6446  EiGUomqUpTZ2PHdF
+0003b0d0: 5659 4438 6970 6d79 6365 4876 6744 6568  VYD8ipmyceHvgDeh
+0003b0e0: 4579 6648 3277 7a4f 3450 334e 6637 5433  EyfH2wzO4P3Nf7T3
+0003b0f0: 4f64 4147 4944 6344 4a58 6550 5468 6353  OdAGIDcDJXePThcS
+0003b100: 6745 6f76 5a32 644a 4231 3645 4d59 496f  gEovZ2dJB16EMYIo
+0003b110: 437a 6959 7a44 3934 4c30 2b6b 2f2b 466e  CziYzD94L0+k/+Fn
+0003b120: 5565 6e62 4248 734f 752b 4245 3244 6f42  UenbBHsOu+BE2DoB
+0003b130: 4236 6b35 4371 574b 5255 4d79 6b54 7939  B6k5CqWKRUMykTy9
+0003b140: 5939 486e 3962 3148 7151 4559 3937 3661  Y9Hn9b1HqQEY976a
+0003b150: 782b 5035 3236 424d 7164 4154 306a 7143  x+P526BMqdAT0jqC
+0003b160: 6752 3143 6938 4c4b 366d 5353 3278 426e  gR1Ci8LK6mSS2xBn
+0003b170: 434a 5a6e 4d68 7a5a 7433 3565 6645 6d32  CJZnMhzZt35efEm2
+0003b180: 3451 4877 6276 682f 3237 7539 5376 4778  4QHwbvh/27u9SvGx
+0003b190: 6150 5176 546f 6b68 304a 454a 326b 3648  aPQvTokh0JEJ2k6H
+0003b1a0: 6759 6155 725a 4338 4964 436d 3333 4165  gYaUrZC8IdCm33Ae
+0003b1b0: 3332 5033 654c 6b4b 4d62 3679 5545 7739  32P3eLkKMb6yUEw9
+0003b1c0: 6932 4d54 2f63 3859 3355 3656 5875 7534  i2MT/c8Y3U6VXuu4
+0003b1d0: 4777 4b6c 506b 664b 4438 6f4f 5651 6a6c  GwKlPkfKD8oOVQjl
+0003b1e0: 516e 7170 3251 524f 5653 5141 665a 6642  Qnqp2QROVSQAfZfB
+0003b1f0: 7837 356c 6145 7633 3737 2f35 2b46 4b56  x75laEv377/5+FKV
+0003b200: 3255 5442 4d62 4d65 7a55 3963 3744 4e6b  2UTBMbMezU9c7DNk
+0003b210: 6b39 6154 5038 6267 6642 6761 4943 756f  k9aTP8bgfBgaICuo
+0003b220: 3056 4a30 5569 7850 6f39 6238 6a52 722f  0VJ0UixPo9b8jRr/
+0003b230: 714b 4c35 6777 3947 742f 524e 6d74 7342  qKL5gw9Gt/RNmtsB
+0003b240: 5268 796b 4b70 6c43 546b 4957 3639 4b65  RhykKplCTkIW69Ke
+0003b250: 4e4e 7a2f 6f54 7a48 7651 6363 526a 5535  NNz/oTzHvQccRjU5
+0003b260: 452f 712f 666c 494a 6255 616b 6b48 4a6f  E/q/flIJbUakkHJo
+0003b270: 4c6f 6b74 5931 4375 744b 316f 2f54 3952  LoktY1CutK1o/T9R
+0003b280: 3466 3058 3762 4e76 3239 5373 554d 7376  4f0X7bNv29SsUMsv
+0003b290: 454c 4675 4863 706b 2f77 7961 4844 3153  ELFuHcpk/wyaHD1S
+0003b2a0: 446f 6367 6544 6761 6147 4e4b 6872 745a  DocgeDgaaGNKhrtZ
+0003b2b0: 4555 4845 674f 5a59 344c 4e79 4365 7353  EUHEgOZY4LNyCesS
+0003b2c0: 2b66 3049 474a 7356 6577 4551 7977 7570  +f0IGJsVewEQywup
+0003b2d0: 5270 6952 586f 5871 5a46 3636 2b37 352b  RpiRXoXqZF66+75+
+0003b2e0: 6964 6a54 742f 6951 3678 7947 5037 6d37  idjTt/iQ6xyGP7m7
+0003b2f0: 382b 4765 6c34 4436 7661 7155 5657 646c  8+Gel4D6vaqUVWdl
+0003b300: 4b49 4346 5958 4153 4179 4c62 4b69 7149  KICFYXASAyLbKiqI
+0003b310: 7758 6535 4655 7535 5063 5748 584c 4a79  wXe5FUu5PcWHXLJy
+0003b320: 3176 5855 3363 4e4b 7336 4434 4255 7139  1vXU3cNKs6D4BUq9
+0003b330: 4272 6345 7139 7779 582b 7732 6553 5163  BrcEq9wyX+w2eSQc
+0003b340: 4570 6b38 6d4e 7532 6364 6166 6671 6431  Epk8mNu2cdaffqd1
+0003b350: 7833 6b4b 454a 5154 3950 5251 6751 6473  x3kKEJQT9PRQgQds
+0003b360: 5273 7866 3838 4c37 7557 7576 7939 5535  Rsxf88L7uWuvy9U5
+0003b370: 732b 7735 446f 6b42 3048 4a77 4261 5939  s+w5DokB0HJwBaY9
+0003b380: 5a45 4379 526e 6644 346a 7878 4f44 6e62  ZECyRnfD4jxxODnb
+0003b390: 7274 6d79 4373 3339 614c 3062 5167 5652  rtmyCs39aL0bQgVR
+0003b3a0: 5a44 3956 2f31 6662 5775 7a75 466c 772b  ZD9V/1fbWuzuFlw+
+0003b3b0: 5243 3038 4768 7358 5571 6774 7465 7462  RC08GhsXUqgttetb
+0003b3c0: 7736 434d 7171 6f4f 5967 4972 5a4f 6747  w6CMqqoOYgIrZOgG
+0003b3d0: 3250 384c 6c2b 7949 3937 7565 6453 7a6d  2P8Ll+yI97uedSzm
+0003b3e0: 2f54 6b62 5a66 4331 444e 4344 714d 4545  /TkbZfC1DNCDqMEE
+0003b3f0: 6f4f 7576 684f 7945 5144 2f4e 752b 4143  oOuvhOyEQD/Nu+AC
+0003b400: 3166 3273 766c 3563 4736 5a42 7656 5a72  1f2svl5cG6ZBvVZr
+0003b410: 684a 4b79 4646 5562 5168 3048 4133 4b5a  hJKyFFUbQh0HA3KZ
+0003b420: 444a 5157 4157 622f 6148 4d57 5938 506e  DJQWAWb/aHMWY8Pn
+0003b430: 6e6c 5474 336a 4754 5556 6c45 4154 6d47  nlTt3jGTUVlEATmG
+0003b440: 684f 616e 6a6f 776e 3636 5a43 5457 3647  hOanjown66ZCTW6G
+0003b450: 4868 5246 3751 3443 4b30 564b 3445 394d  HhRF7Q4CK0VK4E9M
+0003b460: 4159 7143 6a68 4d48 3350 756e 2f35 4f6e  AYqCjhMH3Pun/5On
+0003b470: 324d 752b 4b44 5035 4d36 3972 3747 6c59  2Mu+KDP5M69r7GlY
+0003b480: 6570 6e71 6878 3049 744f 7064 4e43 4e2f  epnqhx0ItOpdNCN/
+0003b490: 4444 4164 2b48 6e37 2f2f 4e47 6237 7654  DDAd+Hn7//NGb7vT
+0003b4a0: 4141 7666 4239 346b 7644 6b6f 7575 7071  AAvfB94kvDkouupq
+0003b4b0: 6738 4253 5653 6a2b 3247 6762 557a 4333  g8BSVSj+2GgbUzC3
+0003b4c0: 4954 7678 6158 317a 4f42 6e62 3735 7957  ITvxaX1zOBnb75yW
+0003b4d0: 356d 6264 4439 4270 4c54 3262 4a6c 3549  5mbdD9BpLT2bJl5I
+0003b4e0: 624f 734a 3645 4234 5743 516b 5a4a 5136  bOsJ6EB4WCQkZJQ6
+0003b4f0: 4d59 4e54 4561 5052 6b4f 4a62 2f6d 784e  MYNTEaPRkOJb/mxN
+0003b500: 6842 2f6c 465a 7576 3764 3766 2b6b 4253  hB/lFZuv7d7f+kBS
+0003b510: 7574 656f 4266 6b7a 5066 4a47 345a 446c  uteoBfkzPfJG4ZDl
+0003b520: 6c44 7171 7075 676f 7244 6f77 504f 5739  lDqqpugorDowPOW9
+0003b530: 6b37 5930 3243 6f65 776f 7764 7835 4f34  k7Y02Coewowdx5O4
+0003b540: 716d 6570 7236 6d79 6d59 2f43 466f 7232  qmepr6mymY/CFor2
+0003b550: 7264 4156 7345 4a34 4764 5759 2b76 5441  rdAVsEJ4GdWY+vTA
+0003b560: 7836 3974 5339 5a4b 686a 6454 7043 3957  x69tS9ZKhjdTpC9W
+0003b570: 7037 6453 584c 7845 2b67 396d 614c 5742  p7dSXLxE+g9maLWB
+0003b580: 4b47 3051 4145 6f6e 614a 306e 4851 4353  KG0QAEonaJ0nHQCS
+0003b590: 586f 4664 7148 6c73 314f 7458 6775 2b2b  XoFdqHls1OtXgu++
+0003b5a0: 5635 502b 734b 357a 7244 566f 5569 6846  V5P+sK5zrDVoUihF
+0003b5b0: 6a62 7569 5639 5541 666c 5067 7370 5150  jbuiV9UAflPgspQP
+0003b5c0: 4b79 3372 7141 4a55 436f 7864 4966 3337  Ky3rqAJUCoxdIf37
+0003b5d0: 396b 5459 7345 3275 6850 6b54 6661 3738  9kTYsE2uhPkTfa78
+0003b5e0: 4548 7038 794f 6763 6e38 7a56 5131 6769  EHp8yOgcn8zVQ1gi
+0003b5f0: 4943 4948 4250 5354 4b41 6c43 6678 7676  ICIHBPSTKAlCfxvv
+0003b600: 347a 7659 7965 3837 3047 2b62 742b 2f39  4zvYye870G+bt+/9
+0003b610: 6148 624b 7a65 682b 656b 2f51 7563 356c  aHbKzeh+ek/Quc5l
+0003b620: 794b 5278 6951 3156 4254 4b48 5169 4146  yKRxiQ1VBTKHQiAF
+0003b630: 5053 4330 5030 794c 7939 3964 3944 6b56  PSC0P0yLy99d9DkV
+0003b640: 6372 6162 5368 7130 3530 2b2b 5a2f 4475  crabShq050++Z/Du
+0003b650: 4733 3945 6d6f 3576 716a 7539 4e4f 576f  G39Emo5vqju9NOWo
+0003b660: 464e 7047 3061 6c7a 4d4b 4f2f 634a 7662  FNpG0alzMKO/cJvb
+0003b670: 7268 7037 7236 584e 4b76 5579 7342 324c  rhp7r6XNKvUysB2L
+0003b680: 2f33 6d71 317a 4961 3248 7950 5652 5857  /3mq1zIa2HyPVRXW
+0003b690: 6c57 7533 4834 4573 7078 4e74 6b6d 5a48  lWu3H4EspxNtkmZH
+0003b6a0: 4c72 3069 4d70 3966 4c37 6250 516a 3070  Lr0iMp9fL7bPQj0p
+0003b6b0: 716d 6b6d 4961 4c68 6b70 5269 4241 6930  qmkmIaLhkpRiBAi0
+0003b6c0: 4f6b 436c 5a77 4434 3970 6a36 3371 6c76  OkClZwD49pj63qlv
+0003b6d0: 3971 4e35 4542 536d 4955 772b 7030 2f44  9qN5EBSmIUw+p0/D
+0003b6e0: 5272 3732 6630 3363 3463 2f44 4256 7552  Rr72f03c4c/DBVuR
+0003b6f0: 7734 6468 5074 435a 704e 4779 4568 6d2f  w4dhPtCZpNGyEhm/
+0003b700: 5a44 5839 4878 7839 4876 2f66 6544 456d  ZDX9Hxx9Hv/feDEm
+0003b710: 644d 6473 4257 5272 3775 7736 4943 4c37  dMdsBWRr7uw6ICL7
+0003b720: 3745 4c2f 7437 6773 2b2b 4634 564b 5771  7EL/t7gs++F4VKWq
+0003b730: 6c78 3250 347a 7377 435a 5a6c 5743 4651  lx2P4zswCZZlWCFQ
+0003b740: 3153 734d 7448 7442 4a47 4d32 3048 4442  1SsMtHtBJGM20HDB
+0003b750: 554c 7242 7272 7856 564a 5276 7055 2b35  ULrBrrxVVJRvpU+5
+0003b760: 3265 3833 6565 6f4a 344f 7646 3235 3952  2e83eeoJ4OvF259R
+0003b770: 4473 745a 314f 6d57 4474 2f64 4e2f 4552  DstZ1OmWDt/dN/ER
+0003b780: 4733 6d43 575a 7876 4c6d 5a43 7659 6d32  G3mCWZxvLmZCvYm2
+0003b790: 412f 714c 6e6f 666c 4377 6942 2b52 544b  A/qLnoflCwiB+RTK
+0003b7a0: 6b31 7378 3348 4c66 6e68 5a6e 2b31 7647  k1sx3HLfnhZn+1vG
+0003b7b0: 5058 6f72 6668 7759 6665 5468 4450 356e  PXorfhwYfeThDP5n
+0003b7c0: 384f 2f73 384c 7931 6c77 6775 6354 7644  8O/s8Ly1lwgucTvD
+0003b7d0: 6974 3730 5835 6f47 3644 4970 7331 6d4c  it70X5oG6DIps1mL
+0003b7e0: 6d61 6231 784d 7146 4e30 2f53 6163 574d  mab1xMqFN0/SacWM
+0003b7f0: 3630 5761 4f30 5543 7332 4249 4944 4f65  60WaO0UCs2BIIDOe
+0003b800: 582f 4c6c 2f2f 6366 6332 6a70 2b48 3945  X/Ll//cfc2jp+H9E
+0003b810: 3532 774e 5646 456a 6831 6676 3666 6e6a  52wNVFEjh1fv6fnj
+0003b820: 6a38 3735 5763 7961 5438 4764 6473 5a36  j875WcyaT8GddsZ6
+0003b830: 6d67 4656 5134 366b 5a45 366f 4a2b 5368  mgFVQ46kZE6oJ+Sh
+0003b840: 4862 3551 484a 6542 3937 6b63 6a36 6b2f  Hb5QHJeB97kcj6k/
+0003b850: 746e 5237 2f33 7049 4c42 6975 6431 4b6c  tnR7/3pILBiud1Kl
+0003b860: 4d48 5033 544a 6132 4c33 2f43 5058 4766  MHP3TJa2L3/CPXGf
+0003b870: 336d 7436 772b 4272 6a61 6831 4b5a 6c4a  3mt6w+Brjah1KZlJ
+0003b880: 647a 7636 5379 362f 5777 4563 3541 3271  dzv6Sy6/WwEc5A2q
+0003b890: 4152 4e30 4657 7a42 5170 4136 5253 4e4e  ARN0FWzBQpA6RSNN
+0003b8a0: 7172 576c 6344 754a 5430 752b 6350 435a  qrWlcDuJT0u+cPCZ
+0003b8b0: 7065 2b31 2b50 6f42 6443 6849 706d 3343  pe+1+PoBdChIpm3C
+0003b8c0: 4971 494d 5859 3644 482b 6d37 4841 6f71  IqIMXY6DH+m7HAoq
+0003b8d0: 334a 2b44 634f 2b55 5641 2b70 454f 7454  3J+DcO+UVA+pEOtT
+0003b8e0: 4332 4d41 714c 3062 4671 4f48 4947 4e6f  C2MAqL0bFqOHIGNo
+0003b8f0: 6852 5461 5753 4475 596b 5174 3049 6e2b  hRTaWSDuYkQt0In+
+0003b900: 3958 6350 6236 3247 7050 5171 7555 5778  9XcPb62GpPQquUWx
+0003b910: 3542 5862 736f 774c 336b 6131 4f4d 6d32  5BXbsowL3ka1OMm2
+0003b920: 4d6d 6532 6b7a 3143 2f59 5871 304e 3665  Mme2kz1C/YXq0N6e
+0003b930: 3176 702f 6b4a 5454 5674 7978 4f56 2f31  1vp/kJTTVtyxOV/1
+0003b940: 7061 4b51 7756 3445 4544 515a 7048 4730  paKQwV4EEDQZpHG0
+0003b950: 3370 674e 3942 7178 4949 6646 3044 7663  3pgN9BqxIIfF0Dvc
+0003b960: 534c 3378 4c50 6a56 6a31 3236 6862 304a  SL3xLPjVj126hb0J
+0003b970: 6b69 4d49 6e4b 4d65 7533 5747 6e6e 324c  kiMInKMeu3WGnn2L
+0003b980: 722b 5547 6564 2f49 5435 616b 5150 715a  r+UGed/IT5akQPqZ
+0003b990: 7970 6f46 4a42 6835 3143 7974 4c4f 514d  ypoFJBh51CytLOQM
+0003b9a0: 4547 676f 4e41 5377 5746 7559 6c6e 6659  EGgoNASwWFuYlnfY
+0003b9b0: 3562 312b 4136 7a37 7072 415a 6b7a 4259  5b1+A6z7prAZkzBY
+0003b9c0: 7869 7430 3561 426c 487a 3479 3738 5a5a  xit05aBlHz4y78ZZ
+0003b9d0: 726d 4a2b 376d 5564 3759 6a68 3161 707a  rmJ+7mUd7Yjh1apz
+0003b9e0: 7532 7172 5777 554e 6262 6f50 6c55 7775  u2qrWwUNbboPlUwu
+0003b9f0: 7038 6770 7546 4342 5244 5641 5559 6e71  p8gpuFCBRDVAUYnq
+0003ba00: 512b 4743 5577 614b 5878 3769 386d 2f4e  Q+GCUwaKXx7i8m/N
+0003ba10: 6135 7175 3376 5831 5938 4f55 6659 7551  a5qu3vX1Y8OUfYuQ
+0003ba20: 5474 6934 4c4c 544a 2f39 7a64 4b72 7667  Tti4LLTJ/9zdKrvg
+0003ba30: 4f65 4245 742b 4352 662b 3357 3669 4a4f  OeBEt+CRf+3W6iJO
+0003ba40: 6669 4231 4e55 4d41 3456 4156 5970 4b4e  fiB1NUMA4VAVYpKN
+0003ba50: 6b5a 7469 3277 4441 7857 5665 4e7a 3238  kZti2wDAxWVeNz28
+0003ba60: 4378 7235 6f6a 5252 2f39 3468 3566 7571  Cxr5ojRR/94h5fuq
+0003ba70: 6f46 3461 5232 3744 4250 7576 444d 7837  oF4aR27DBPuvDMx7
+0003ba80: 4b58 627a 2f46 392b 6172 6b2f 4467 6f4a  KXbz/F9+ark/DgoJ
+0003ba90: 7147 5473 494b 6d61 696f 6769 5761 7452  qGTsIKmaiogiWatR
+0003baa0: 477a 4276 6756 706c 592f 4b6d 594d 4562  GzBvgVplY/KmYMEb
+0003bab0: 5262 714a 496f 6173 324e 7942 4e6e 5534  RbqJIoas2NyBNnU4
+0003bac0: 796c 6e57 7235 3459 397a 4b68 3342 7545  ylnWr54Y9zKh3BuE
+0003bad0: 6e35 3764 3950 516a 6868 7735 6836 7738  n57d9PQjhhw5h6w8
+0003bae0: 397a 3766 3234 6c37 4839 4b62 7530 5772  9z7f24l7H9Kbu0Wr
+0003baf0: 5573 3763 6743 6f31 6d47 5539 4e49 4f52  Us7cgCo1mGU9NIOR
+0003bb00: 4c47 5364 5576 4a6f 6152 5345 5641 5a2f  LGSdUvJoaRSEVAZ/
+0003bb10: 4754 6f44 3777 712f 744b 494e 2f2b 7750  GToD7wq/tKIN/+wP
+0003bb20: 3573 3548 5238 7637 7a71 536f 4e64 3436  5s5HR8v7zqSoNd46
+0003bb30: 6263 3772 4272 722f 692f 5535 6664 6747  bc7rBrr/i/U5fdgG
+0003bb40: 6167 5474 4f67 384f 5972 3352 5348 4d56  agTtOg8OYr3RSHMV
+0003bb50: 376e 6f64 6f4a 5145 3058 6243 5853 4d4b  7nodoJQE0XbCXSMK
+0003bb60: 6e73 6b6f 594f 4467 5571 594c 5770 6e41  nskoYODgUqYLWpnA
+0003bb70: 3248 6f64 632b 3635 6331 2f33 5750 6c33  2Hodc+65c1/3WPl3
+0003bb80: 7764 4370 6f33 744f 4551 4770 524a 6772  wdCpo3tOEQGpRJgr
+0003bb90: 6a48 4632 656e 6a2b 7959 3550 6575 6659  jHF2enj+yY5PeufY
+0003bba0: 725a 314b 5253 564c 4371 7a74 424e 6745  rZ1KRSVLCqztBNgE
+0003bbb0: 746f 6f6a 6f48 5339 5a36 4141 6f6c 4371  toojoHS9Z6AAolCq
+0003bbc0: 752f 3542 7573 7161 6149 714b 7754 7146  u/5BusqaaIqKwTqF
+0003bbd0: 7961 4131 4272 5763 5279 3372 4564 4731  yaA1BrWcRy3rEdG1
+0003bbe0: 4778 3351 392b 5a76 3847 7251 7156 3133  Gx3Q9+Zv8GrQqV13
+0003bbf0: 3269 4d2f 5842 4763 7568 4c74 3530 7268  2iM/XBGcuhLt50rh
+0003bc00: 4867 5779 734c 5863 3957 3748 5548 3570  HgWysLXc9W7HUH5p
+0003bc10: 6a37 5243 4171 7449 4977 7473 6f34 7842  j7RCAqtIIwtso4xB
+0003bc20: 7259 4e66 3832 3457 3145 5251 3677 4170  rYNf824W1ERQ6wAp
+0003bc30: 7445 514a 5472 4677 6b43 6a50 446b 695a  tEQJTrFwkCjPDkiZ
+0003bc40: 3659 6b7a 416d 2b37 4976 6b79 3775 7565  6YkzAm+7Ivky7uue
+0003bc50: 4f53 3069 544d 3750 5463 7049 6759 7549  OS0iTM7PTcpIgYuI
+0003bc60: 3536 3673 355a 504f 2b56 6e50 4a6c 3443  566s5ZPO+VnPJl4C
+0003bc70: 4378 6a6f 5168 6f75 3744 4d6f 4934 4570  CxjoQhou7DMoI4Ep
+0003bc80: 5955 574c 5547 5144 582f 3462 464e 4438  YUWLUGQDX/4bFND8
+0003bc90: 7779 3259 4f58 5070 4f73 744e 4f6b 6b53  wy2YOXPpOstNOkkS
+0003bca0: 4b70 3878 7168 5570 5750 4d61 415a 6771  Kp8xqhUpWPMaAZgq
+0003bcb0: 5963 6158 5635 626b 3370 712b 4f75 2f77  YcaXV5bk3pq+Ou/w
+0003bcc0: 7974 6469 4530 6979 5859 7633 5471 795a  ytdiE0iyXYv3TqyZ
+0003bcd0: 6432 4b65 356e 6b66 3441 7444 454a 6255  d2Ke5nkf4AtDEJbU
+0003bce0: 666b 677a 4837 6f43 4347 3059 5551 7035  fkgzH7oCCG0YUQp5
+0003bcf0: 636c 4251 6b63 726d 7947 6264 5a62 7043  clBQkcrmyGbdZbpC
+0003bd00: 757a 522b 4a53 2b69 7155 626a 774c 5467  uzR+JS+iqUbjwLTg
+0003bd10: 6744 5167 3168 4a59 3466 5a51 4446 3642  gDQg1hJY4fZQDF6B
+0003bd20: 2f6d 462b 687a 6e33 336d 422f 6544 3959  /mF+hzn33mB/eD9Y
+0003bd30: 6366 5037 2b42 4b56 326c 3738 4c45 7a70  cfP7+BKV2l78LEzp
+0003bd40: 6a74 7339 7830 4f5a 596e 457a 5679 6f44  jts9x0OZYnEzVyoD
+0003bd50: 3053 304b 3764 736d 6470 6d41 7670 4267  0S0K7dsmdpmAvpBg
+0003bd60: 4338 6b75 6434 6936 384d 4674 3972 2f65  C8kud4i68MFt9r/e
+0003bd70: 506b 3171 3541 5859 7165 6839 6536 4a42  Pk1q5AXYqeh9e6JB
+0003bd80: 317a 4f61 6a49 4877 7867 2f5a 664c 7251  1zOajIHwxg/ZfLrQ
+0003bd90: 4730 794b 4453 7933 7832 564a 5667 6275  G0yKDSy3x2VJVgbu
+0003bda0: 4b5a 6663 6465 2f62 6434 4246 3571 6270  KZfcde/bd4BF5qbp
+0003bdb0: 3261 7444 6f46 5871 4377 2f38 5255 3462  2atDoFXqCw/8RU4b
+0003bdc0: 3934 4955 6657 7645 494a 7436 3956 4261  94IUfWvEIJt69VBa
+0003bdd0: 4975 7942 655a 5144 2f49 4351 6f49 6f71  IuyBeZQD/ICQoIoq
+0003bde0: 5151 4532 6778 7a78 6d6c 4c6a 7635 6578  QQE2gxzxmlLjv5ex
+0003bdf0: 5637 4671 6743 4350 4e6b 4758 5457 4475  V7FqgCCPNkGXTWDu
+0003be00: 6d6f 3733 5849 4930 3667 5258 5563 6932  mo73XII06gRXUci2
+0003be10: 5543 4a36 4945 396b 722f 6f34 4447 786b  UCJ6IE9kr/o4DGxk
+0003be20: 4174 7868 544e 3461 5053 6633 4c51 6a42  AtxhTN4aPSf3LQjB
+0003be30: 7076 432b 506a 2f75 7276 5736 3148 7a45  pvC+Pj/urvW61HzE
+0003be40: 316a 3148 4f41 4644 4633 4b6c 5675 7554  1j1HOAFDF3KlVuuT
+0003be50: 436f 7853 4663 2f2b 424f 6959 4b31 7365  CoxSFc/+BOiYK1se
+0003be60: 7041 2f2b 4f70 6637 546d 4c36 5a31 7462  pA/+Opf7TmL6Z1tb
+0003be70: 766b 776a 6247 4571 4b32 3133 636c 3737  vkwjbGEqK213cl77
+0003be80: 435a 3247 5834 6c73 2b30 4273 4162 5653  CZ2GX4ls+0BsAbVS
+0003be90: 5731 5362 594f 3053 426c 476d 6977 5530  W1SbYO0SBlGmiwU0
+0003bea0: 4938 4370 4f4b 4833 4266 6e2f 7965 2f2f  I8CpOKH3Bfn/ye//
+0003beb0: 4730 3236 5670 7a71 7161 6352 6343 3578  G026VpzqqacRcC5x
+0003bec0: 724f 3344 7856 702f 6d75 6f34 7a47 7772  rO3DxVp/muo4zGwr
+0003bed0: 326f 5348 6d78 6272 324b 3272 5856 7455  2oSHmxbr2K2rXVtU
+0003bee0: 445a 7444 7649 434f 6952 4849 4d67 4e56  DZtDvICOiRHIMgNV
+0003bef0: 7a52 424b 6d43 5372 7144 6153 7a63 6577  zRBKmCSrqDaSzcew
+0003bf00: 6a53 7130 6147 3170 5644 2f68 5362 4d68  jSq0aG1pVD/hSbMh
+0003bf10: 5861 746f 7433 6f6b 6532 4575 5648 4349  Xatot3oke2EuVHCI
+0003bf20: 766c 516e 316c 2f79 5339 652f 4e74 526e  vlQn1l/yS9e/NtRn
+0003bf30: 3936 5054 354e 4779 5945 3633 6733 6e4f  96PT5NGyYE63g3nO
+0003bf40: 3139 3333 7a46 6566 6532 7a34 476e 7738  1933zFefe2z4Gnw8
+0003bf50: 6675 5375 3732 3448 5358 626c 526b 6d42  fuSu724HSXblRkmB
+0003bf60: 5247 7151 3935 6461 4c38 3139 7966 7370  RGqQ95daL819yfsp
+0003bf70: 722f 2f33 706d 3971 4158 6355 4149 584a  r//3pm9qAXcUAIXJ
+0003bf80: 7577 4567 7a47 6758 4e76 4d6b 2f66 4e66  uwEgzGgXNvMk/fNf
+0003bf90: 4d64 2b34 4d57 4c65 4550 4c59 7a67 3355  Md+4MWLeEPLYzg3U
+0003bfa0: 5a74 5532 7941 744b 434f 554a 6773 4652  ZtU2yAtKCOUJgsFR
+0003bfb0: 5a4a 5a73 4450 6a70 4755 394f 5377 3934  ZJZsDPjpGU9OSw94
+0003bfc0: 4765 392f 2b39 4776 4e4b 464b 4430 5a73  Ge9/+9GvNKFKD0Zs
+0003bfd0: 4f47 7633 4836 6d6e 2b49 7a59 6233 6a4f  OGv3H6mn+IzYb3jO
+0003bfe0: 7951 4851 6573 716f 5553 6953 676f 5345  yQHQesqoUSiSgoSE
+0003bff0: 7863 7968 576c 4245 4f72 7771 2f41 7053  xcyhWlBEOrwq/ApS
+0003c000: 5076 4732 7472 5959 3932 5462 5343 4349  PvG2trYY92TbSCCI
+0003c010: 525a 4236 366f 6474 5633 4974 5443 342b  RZB66odtV3ItTC4+
+0003c020: 6136 5137 4479 5966 4f38 4c4f 6e68 6e6c  a6Q7DyYfO8LOnhnl
+0003c030: 5951 3567 3955 6a32 796b 2b53 4243 6f58  YQ5g9Uj2yk+SBCoX
+0003c040: 3642 4468 6f58 4d6b 392f 4966 7254 6f32  6BDhoXMk9/IfrTo2
+0003c050: 626d 544c 7946 7673 7675 7375 7762 6b65  bmTLyFvsvusuwbke
+0003c060: 3956 6677 726e 3148 6369 6776 2f53 424d  9Vfwrn1Hcigv/SBM
+0003c070: 4758 6f64 556b 7436 5553 555a 4853 4b6f  GXodUkt6USUZHSKo
+0003c080: 4e66 4973 6458 725a 6a70 2f65 2b47 5062  NfIsdXrZjp/e+GPb
+0003c090: 4f36 7946 6d6d 425a 3043 6136 3473 476e  O6yFmmBZ0Ca64sGn
+0003c0a0: 494d 4834 516e 7749 6c7a 3434 4567 732b  IMH4QnwIlz44Egs+
+0003c0b0: 474f 3143 656c 392b 6544 3976 5447 4476  GO1Cel9+eD9vTGDv
+0003c0c0: 386b 5474 7270 6333 5646 5a79 7167 6c69  8kTtrpc3VFZyqgli
+0003c0d0: 4342 6453 5171 7875 3072 3541 6654 6262  CBdSQqxu0r5AfTbb
+0003c0e0: 7935 3863 7555 6237 4672 6c54 5962 4e76  y58cuUb7FrlTYbNv
+0003c0f0: 474f 5954 4970 7249 4f2b 5a55 424d 3733  GOYTIprIO+ZUBM73
+0003c100: 4861 7746 3846 3241 7073 4a74 4454 4a32  HawF8F2ApsJtDTJ2
+0003c110: 725a 614d 506c 4c49 5034 7873 4c32 4a4a  rZaMPlLIP4xsL2JJ
+0003c120: 6f2f 2b42 5871 526a 624e 7079 2b4d 6856  o/+BXqRjbNpy+MhV
+0003c130: 7364 5142 4a48 3655 5865 4162 6b41 7454  sdQBJH6UXeAbkAtT
+0003c140: 4541 4573 5331 2f59 7074 584d 7a2f 4a73  EAEsS1/YptXMz/Js
+0003c150: 3565 4248 5471 7775 6c6c 5632 696b 516f  5eBHTqwullV2ikQo
+0003c160: 5530 4839 4374 7279 3847 352b 6839 2b57  U0H9Ctry8G5+h9+W
+0003c170: 3974 3345 335a 695a 3547 7962 774d 7630  9t3E3ZiZ5GybwMv0
+0003c180: 2b35 6a64 4770 7a61 6830 4347 4a52 4a47  +5jdGpzah0CGJRJG
+0003c190: 796a 4a70 454d 416e 564b 3437 6a4c 376c  yjJpEMAnVK47jL7l
+0003c1a0: 5939 7573 5239 3759 7a5a 764c 6b67 6b42  Y9usR97YzZvLkgkB
+0003c1b0: 3954 4c73 7158 4666 5743 4a44 5838 2b46  9TLsqXFfWCJDX8+F
+0003c1c0: 3867 5547 4242 426b 6931 3978 6833 4d34  8gUGBBBki19xh3M4
+0003c1d0: 4174 702b 324c 6e37 5871 3478 2b31 3976  Atp+2Ln7Xq4x+19v
+0003c1e0: 7179 7650 6879 5942 4754 746f 4377 7467  qyvPhyYBGTtoCwtg
+0003c1f0: 6e30 4f30 6949 3272 4b39 6b54 6244 6c50  n0O0iI2rK9kTbDlP
+0003c200: 7861 6176 6574 544e 6662 6830 7559 3377  xaavetTNfbh0uY3w
+0003c210: 5042 324b 4f57 4972 4575 714d 6d4b 6731  PB2KOWIrEuqMmKg1
+0003c220: 6957 7067 3841 634b 5069 6674 6c37 3368  iWpg8AcKPiftl73h
+0003c230: 5858 2b38 694f 2b38 2f47 6770 3239 3648  XX+8iO+8/Ggp296H
+0003c240: 4c72 576b 6253 6849 4c74 5253 6d79 4354  LrWkbShILtRSmyCT
+0003c250: 3174 2b62 447a 4536 6844 6867 6159 4942  1t+bDzE6hDhgaYIB
+0003c260: 5671 5967 4152 6138 5974 7563 2f70 5061  VqYgARa8Ytuc/pPa
+0003c270: 6e6d 3337 2b73 2f68 5635 304e 4a79 6458  nm37+s/hV50NJydX
+0003c280: 3646 587a 6e55 6567 3836 5467 3951 306e  6FXznUeg86Tg9Q0n
+0003c290: 4c32 2f59 6c64 5676 536c 537a 7239 6755  L2/YldVvSlSzr9gU
+0003c2a0: 7141 2b52 6863 4131 7453 7271 6856 516d  qA+RhcA1tSrqhVQm
+0003c2b0: 6a6f 6141 2b58 5336 5a67 664f 7379 7974  joaA+XS6ZgfOsyyt
+0003c2c0: 6639 7937 6e37 7943 6d66 4753 782b 796c  f9y7n7yCmfGSx+yl
+0003c2d0: 687a 4d37 3330 484e 756f 494f 464d 4c47  hzM730HNuoIOFMLG
+0003c2e0: 4664 4245 5354 4249 3449 6457 4d48 706f  FdBESTBI4IdWMHpo
+0003c2f0: 5530 5964 766d 4f4c 3144 4345 4f79 6a42  U0YdvmOL1DCEOyjB
+0003c300: 5532 5a4f 7836 3532 6635 6f30 552b 5a36  U2ZOx652f5o0U+Z6
+0003c310: 366c 2f41 3033 4668 4755 524d 4271 7470  6l/A03FhGURMBqtp
+0003c320: 4445 4837 5744 5357 4232 332b 6157 7065  DEH7WDSWB23+aWpe
+0003c330: 7563 315a 764e 376f 5437 6c79 5545 4931  uc1ZvN7oT7lyUEI1
+0003c340: 3156 3564 4243 596c 514b 7054 5841 494c  1V5dBCYlQKpTXAIL
+0003c350: 732b 6c76 574f 5748 336e 7052 3354 7841  s+lvWOWH3npR3TxA
+0003c360: 354f 4364 4232 5355 7335 5732 6169 7379  5OCdB2SUs5W2aisy
+0003c370: 3777 6d51 714a 4531 3145 4376 3161 3831  7wmQqJE11ECv1a81
+0003c380: 2b66 6f4e 7a4c 3965 6838 4f70 3939 6651  +foNzL9eh8Op99fQ
+0003c390: 3170 4c6d 4838 3936 3056 7353 7457 4a49  1pLmH8960VsStWJI
+0003c3a0: 4468 6e67 7947 6f4b 6c33 6652 434e 4b38  DhngyGoKl3fRCNK8
+0003c3b0: 6271 4153 4565 554d 4e64 5978 462b 652f  bqASEeUMNdYxF+e/
+0003c3c0: 5750 6e35 772f 3877 5872 2f50 3431 4944  WPn5w/8wXr/P41ID
+0003c3d0: 4e2f 6e53 4149 6768 4f39 5973 4341 5a68  N/nSAIghO9YsCAZh
+0003c3e0: 4d38 634b 6268 7477 534b 4544 3451 4241  M8cKbhtwSKED4QBA
+0003c3f0: 6b6b 6243 4953 4559 5134 5458 674a 596c  kkbCISEYQ4TXgJYl
+0003c400: 5743 4e72 637a 3579 7a4d 764a 2f38 3638  WCNrcz5yzMvJ/868
+0003c410: 324b 2b72 7531 5a4f 436e 6f43 7775 6d54  2K+ru1ZOCnoCwumT
+0003c420: 5079 5a75 6c42 4561 5547 6474 4341 5a70  PyZulBEaUGdtCAZp
+0003c430: 492b 414a 6679 5843 415a 4744 6664 486d  I+AJfyXCAZGDfdHm
+0003c440: 5572 796b 5256 3848 7154 5067 6979 546c  UrykRV8HqTPgiyTl
+0003c450: 6831 782b 612f 5848 4867 6c76 724f 696f  h1x+a/XHHglvrOio
+0003c460: 664b 576c 456b 776d 3437 614b 686b 564d  fKWlEkwm47aKhkVM
+0003c470: 306b 334c 5263 3061 6944 4377 312b 4b31  0k3LRc0aiDCw1+K1
+0003c480: 367a 3973 7a76 3061 3776 6374 686d 2b55  6z9szv0a7vcthm+U
+0003c490: 2f41 326a 6256 5645 6b42 7047 4f6f 4471  /A2jbVVEkBpGOoDq
+0003c4a0: 6d4c 4b44 4e49 6f43 4b30 4861 536f 4944  mLKDNIoCK0HaSoID
+0003c4b0: 3261 5951 4b71 4a41 6f49 7a71 5241 4674  2aYQKqJAoIzqRAFt
+0003c4c0: 727a 6851 5837 4851 3163 3466 336c 756c  rzhQX7HQ1c4f3lul
+0003c4d0: 6978 6770 3166 4573 4277 6679 4947 4573  ixgp1fEsBwfyIGEs
+0003c4e0: 4377 4c5a 7331 6343 4273 567a 7057 3075  CwLZs1cCBsVzpW0u
+0003c4f0: 4158 7033 4a59 5170 3355 3839 4452 4145  AXp3JYQp3U89DRAE
+0003c500: 7072 4567 7966 7866 4964 3973 7167 352f  prEgyfxfId9sqg5/
+0003c510: 6475 4862 7244 656e 2f64 4456 7644 552f  duHbrDen/dDVvDU/
+0003c520: 312b 486f 734e 3955 3345 5370 7234 6b7a  1+HosN9U3ESpr4kz
+0003c530: 4834 555a 7770 7367 5a6d 325a 4249 6939  H4UZwpsgZm2ZBIi9
+0003c540: 6941 6767 626c 672b 3032 672f 6168 674a  iAggblg+02g/ahgJ
+0003c550: 7739 5a64 7668 6c62 3676 4545 706a 3139  w9Zdvhlb6vEEpj19
+0003c560: 4b71 305a 6d44 5452 704b 5650 5532 7644  Kq0ZmDTRpKVPU2vD
+0003c570: 494c 6f42 6773 614d 4244 6d6f 4f6d 677a  ILoBgsaMBDmoOmgz
+0003c580: 4664 7a38 642b 5076 6433 3353 3750 6351  Fdz8d+Pvd33S7PcQ
+0003c590: 7549 4979 5045 4c4d 4f56 5566 6f42 5a72  uIIyPELMOVUfoBZr
+0003c5a0: 7967 4f77 6877 6752 476e 5a57 6f5a 5a6a  ygOwhwgRGnZWoZZj
+0003c5b0: 464c 475a 7459 742b 4775 734e 7a36 3677  FLGZtYt+GusNz66w
+0003c5c0: 6237 3537 332b 3050 6c33 5369 7030 6270  b7573+0Pl3Sip0bp
+0003c5d0: 6854 6748 4c44 546f 3565 7762 4176 6d48  hTgHLDTo5ewbAvmH
+0003c5e0: 6b67 4977 5955 4677 384a 6777 5467 754b  kgIwYUFw8JgwTguK
+0003c5f0: 6833 7951 6835 4446 4f46 4466 7651 6f53  h3yQh5DFOFDfvQoS
+0003c600: 4249 6364 6a57 3379 6572 3758 3334 7a39  BIcdjW3yer7X34z9
+0003c610: 612f 584c 754f 4e62 632f 4166 7567 4777  a/XLuONbc/AfugGw
+0003c620: 6b72 6f75 6f53 5642 4551 365a 5651 596d  krouoSVBEQ6ZVQYm
+0003c630: 3436 6a51 5a6c 4d42 6857 6f57 4767 6a69  46jQZlMBhWoWGgji
+0003c640: 3252 7651 5632 5057 504a 6934 7732 724a  2RvQV2PWPJi4w2rJ
+0003c650: 6c30 4d6e 7273 3942 4652 6135 7756 6745  l0Mnrs9BFRa5wVgE
+0003c660: 4e46 4a49 674b 6c6f 6c45 4251 797a 5655  NFJIgKlolEBQyzVU
+0003c670: 4e46 5169 524a 6452 7a73 4366 6958 782f  NFQiRJdRzsCfiXx/
+0003c680: 5548 4858 386d 5a6d 417a 5434 3365 564e  UHHX8mZmAzT43eVN
+0003c690: 346d 7570 3553 4e4a 6f66 5741 3574 5251  4mup5SNJofWA5tRQ
+0003c6a0: 4549 524c 6c76 5439 494a 3931 2b4f 5832  EIRLlvT9IJ91+OX2
+0003c6b0: 4839 2b39 6e58 5733 4159 4e71 6a6f 354e  H9+9nXW3AYNqjo5N
+0003c6c0: 4378 3444 4548 6541 736f 4575 7342 6730  Cx4DEHeAsoEusBg0
+0003c6d0: 474d 6376 516a 3644 4c4f 6754 646b 6868  GMcvQj6DLOgTdkhh
+0003c6e0: 2f51 674f 7765 4a35 4947 4d51 426a 7577  /QgOweJ5IGMQBjuw
+0003c6f0: 7841 4e76 516f 4d79 5478 584a 6a7a 774b  xANvQoMyTxXJjzwK
+0003c700: 7334 3763 3963 6b62 3333 7742 7576 6679  s47c9ckb33wBuvfy
+0003c710: 3236 526e 722f 5331 4b6e 6376 6757 6771  26Rnr/S1KncvgWgq
+0003c720: 4e6b 3343 4577 7947 4979 4a6f 434e 4b61  Nk3CEwyGIyJoCNKa
+0003c730: 434d 4932 4859 5442 4e63 5672 4d53 6b78  CMI2HYTBNcVrMSkx
+0003c740: 5964 666a 6c66 4367 4161 6442 4b36 7656  YdfjlfCgAadBK6vV
+0003c750: 5156 6c4b 4c5a 564a 6972 4367 3142 4452  QVlKLZVJirCg1BDR
+0003c760: 5136 4761 6272 6759 4859 652f 4c32 424a  Q6GabrgYHYe/L2BJ
+0003c770: 7a37 6e4e 7851 4f67 6e56 7667 6836 7378  z7nNxQOgnVvgh6sx
+0003c780: 3857 7744 6655 4c6f 6373 724c 714d 6a63  8WwDfULocsrLqMjc
+0003c790: 6752 4b49 4b58 7272 6252 656e 5031 6a2b  gRKIKXrrbRenP1j+
+0003c7a0: 3772 3766 386b 2f6d 4139 7a44 5430 424a  7r7f8k/mA9zDT0BJ
+0003c7b0: 362b 4251 796e 6f2f 746a 5238 636f 5664  6+BQyno/tjR8coVd
+0003c7c0: 4834 6941 5249 4341 4c4e 786e 4a48 5430  H4iARICALNxnJHT0
+0003c7d0: 6f34 7350 7441 4279 4748 4476 6b67 5872  o4sPtAByGHDvkgXr
+0003c7e0: 2f6c 7947 3132 5142 524e 366e 4c2f 514a  /lyG12QBRN6nL/QJ
+0003c7f0: 4236 4759 4659 3261 7958 7665 6571 5239  B6GYFY2ayXveeqR9
+0003c800: 5038 382f 7733 6530 7659 6958 6a4f 6a75  P88/w3e0vYiXjOju
+0003c810: 6946 3050 5a57 416f 4b78 4556 524f 4245  iF0PZWAoKxEVROBE
+0003c820: 4b5a 726f 5944 6e41 5362 6641 4c39 7738  KZroYDnASbfAL9w8
+0003c830: 4a49 5847 712f 7579 4775 3067 396d 492b  JIXGq/uyGu0g9mI+
+0003c840: 6756 366b 5970 4235 326e 574c 6169 6f49  gV6kYpB52nWLaioI
+0003c850: 5662 5961 7362 5533 7434 4273 4f4e 5235  VbYasbU3t4BsONR5
+0003c860: 304d 355a 3565 7062 6635 6437 3177 4659  0M5Z5epbf5d71wFY
+0003c870: 2f56 6a6f 584e 2f69 4b75 7154 5a6a 744b  /VjoXN/iKuqTZjtK
+0003c880: 646d 2b44 414f 4947 4850 4a4f 6d41 5862  dm+DAOIGHPJOmAXb
+0003c890: 4758 6a55 3962 6454 3139 7033 2f66 734f  GXjU9bdT19p3/fsO
+0003c8a0: 7979 6668 3061 457a 6f76 7a43 6951 486e  yyfh0aEzovzCiQHn
+0003c8b0: 766b 3944 364a 6d4b 4156 396d 3159 4451  vk9D6JmKAV9m1YDQ
+0003c8c0: 6d42 6e67 4e6d 354c 3451 3043 3861 4e6e  mBngNm5L4Q0C8aNn
+0003c8d0: 5941 6649 3854 374a 4237 5144 4169 4752  YAfI8T7JB7QDAiGR
+0003c8e0: 4245 4639 454b 7749 6477 6d36 4469 6874  BEF9EKwIdwm6Diht
+0003c8f0: 3378 754a 3242 756b 7668 6b63 5850 6d7a  3xuJ2BukvhkcXPmz
+0003c900: 7365 7673 7a39 5a63 694e 7365 4632 3766  sevsz9ZciNseF27f
+0003c910: 5974 496f 7849 6767 3147 4466 514e 4c6d  YtIoxIgg1GDfQNLm
+0003c920: 4164 3077 624a 4d2b 7450 7474 747a 5253  Ad0wbJM+tPtttzRS
+0003c930: 7736 372f 4833 7747 7345 7136 3458 5a69  w67/H3wGsEq64XZi
+0003c940: 506f 4675 6c4b 4c79 3668 3064 4474 4269  PoFulKLy6h0dDtBi
+0003c950: 6f59 4647 6b55 6d33 5a44 7261 5570 4444  oYFGkUm3ZDraUpDD
+0003c960: 4954 5370 7a43 6557 625a 4d73 6c79 6563  ITSpzCeWbZMslyec
+0003c970: 7867 6171 4533 6f4c 5769 7068 4c47 7049  xgaqE3oLWiphLGpI
+0003c980: 4c42 7063 3346 4641 4241 562b 412f 3758  LBpc3FFABAV+A/7X
+0003c990: 612f 4143 6e6e 6741 6e52 576e 4363 4948  a/ACnngAnRWnCcIH
+0003c9a0: 3469 6850 4159 7534 4558 774a 6962 587a  4ihPAYu4EXwJibXz
+0003c9b0: 372f 696c 7346 6232 4e44 7646 516d 6774  7/ilsFb2NDvFQmgt
+0003c9c0: 2b4e 2f31 6151 4634 2b71 6569 4d71 4863  +N/1aQF4+qeiMqHc
+0003c9d0: 5279 6e6b 6566 4264 4c55 4b65 5345 7344  RynkefBdLUKeSEsD
+0003c9e0: 2b59 7252 454b 3849 6962 416b 3641 3345  +YrREK8IibAk6A3E
+0003c9f0: 666d 437a 584b 754c 3332 665a 6d6e 462b  fmCzXKuL32fZmnF+
+0003ca00: 3645 6b71 546f 4d4a 6344 736f 386c 6a41  6EkqToMJcDso8ljA
+0003ca10: 7054 6777 3654 6772 6331 4c31 6b58 5038  pTgw6Tgrc1L1kXP8
+0003ca20: 3948 3237 6743 5133 5777 7656 4541 6142  9H27gCQ3WwvVEAaB
+0003ca30: 5248 564b 7865 5634 5545 5131 4636 6d6b  RHVKxeV4UEQ1F6mk
+0003ca40: 794a 414d 5472 4b77 4234 4144 3551 3557  yJAMTrKwB4AD5Q5W
+0003ca50: 4562 6e45 7964 4f74 4862 3731 7132 3943  EbnEydOtHb71q29C
+0003ca60: 7639 3131 4c57 7972 7670 526d 4354 6a76  v911LWyrvpRmCTjv
+0003ca70: 792b 6d54 4759 6253 6b51 6a35 636c 6856  y+mTGYbSkQj5clhV
+0003ca80: 4571 6b48 3730 696d 7043 4465 6830 727a  EqkH70impCDeh0rz
+0003ca90: 702f 3843 7a62 6c6b 4c31 5a4f 7045 3035  p/8CzblkL1ZOpE05
+0003caa0: 4d41 4f54 5a30 6179 5947 722b 6470 7241  MAOTZ0ayYGr+dprA
+0003cab0: 4967 4545 5649 5942 445a 7442 3262 686a  IgEEVIYBDZtB2bhj
+0003cac0: 5153 3144 566a 5145 366b 4c58 7041 4e68  QS1DVjQE6kLXpANh
+0003cad0: 3234 344c 3847 6846 6844 5474 3245 6950  244L8GhFhDTt2EiP
+0003cae0: 3770 2f2f 3977 334a 762f 4148 7a66 384b  7p//9w3Jv/AHzf8K
+0003caf0: 7035 772b 7258 6644 364d 6152 556d 6c55  p5w+rXfD6MaRUmlU
+0003cb00: 716a 6a67 5646 4c51 6833 7338 432b 7252  qjjgVFLQh3s8C+rR
+0003cb10: 6778 3464 7444 4450 782f 5070 6b2f 556c  gx4dtDDPx/Ppk/Ul
+0003cb20: 412f 6165 774f 4962 6b73 7046 4562 4b72  A/aewOIbkspFEbKr
+0003cb30: 5852 5579 4242 4c42 6162 6479 4742 304d  XRUyBBLBabdyGB0M
+0003cb40: 4a61 3059 2b6e 426f 6669 554b 564f 5148  Ja0Y+nBofiUKVOQH
+0003cb50: 487a 7462 5265 4d39 3763 662b 6869 7a2b  HztbReM97cf+hiz+
+0003cb60: 5066 4254 6738 5945 6b6a 6f62 5255 646f  PfBTg8YEkjobRUdo
+0003cb70: 4569 3567 597a 6b30 346c 424c 5579 6568  Ei5gYzk04lBLUyeh
+0003cb80: 4e50 584f 3253 584b 397a 4c54 376d 5162  NPXO2SXK9zLT7mQb
+0003cb90: 6465 7646 7230 477a 5457 6755 304e 6563  devFr0GzTWgU0Nec
+0003cba0: 4346 7176 7548 446e 4d4c 4b65 3735 4e2f  CFqvuHDnMLKe75N/
+0003cbb0: 3246 712f 5543 6955 4b35 7377 634f 3569  2Fq/UCiUK5swcO5i
+0003cbc0: 4152 4b30 505a 7771 415a 704e 4c75 6e4b  ARK0PZwqAZpNLunK
+0003cbd0: 3130 4a75 6a72 6d6e 727a 6677 626d 7648  10JujrmnrzfwbmvH
+0003cbe0: 504a 7a32 6150 3251 466a 4c55 5658 464f  PJz2aP2QFjLUVXFO
+0003cbf0: 714e 4552 5064 4478 774f 5651 6f70 514c  qNERPdDxwOVQopQL
+0003cc00: 6d55 6b45 794b 7767 532b 445a 512b 5764  mUkEyKwgS+DZQ+Wd
+0003cc10: 7034 5a64 4d43 582f 6d76 7339 436e 6832  p4ZdMCX/mvs9Cnh2
+0003cc20: 3454 746a 3057 4134 7332 7062 536d 624e  4Ttj0WA4s2pbSmbN
+0003cc30: 716f 496e 5467 7147 6431 5045 4e31 5170  qoInTgqGd1PEN1Qp
+0003cc40: 7433 4945 4e46 4446 5854 5861 3063 4d48  t3IENFDFXTXa0cMH
+0003cc50: 4534 424f 646a 7372 2b31 6276 2b62 7562  E4BOdjsr+1bv+bub
+0003cc60: 3130 6c65 3159 3944 2f59 4a30 4945 6776  10le1Y9D/YJ0IEgv
+0003cc70: 6379 3253 6735 5155 4736 6f71 4b51 6f53  cy2Sg5QUG6oqKQoS
+0003cc80: 745a 5250 2b69 3533 4571 7951 6230 6e65  tZRP+i53EqyQb0ne
+0003cc90: 7064 392b 5470 782f 4837 6a5a 6371 3277  pd9+Tpx/H7jZcq2w
+0003cca0: 5234 4d70 376a 7277 6967 2b36 7771 556e  R4Mp7jrwig+6wqUn
+0003ccb0: 5152 3545 392b 4834 5748 4252 5749 6853  QR5E9+H4WHBRWIhS
+0003ccc0: 514b 6934 4d41 4c30 7232 5241 2f75 3058  QKi4MAL0r2RA/u0X
+0003ccd0: 5872 6952 6437 756f 7935 6869 5551 2f58  XriRd7uoy5hiUQ/X
+0003cce0: 5447 4171 7075 4332 6266 4145 4d6d 6d46  TGAqpuC2bfAEMmmF
+0003ccf0: 5a4d 6579 644c 4f46 6b6a 5a43 3572 376d  ZMeydLOFkjZC5r7m
+0003cd00: 6f62 3939 3335 3077 434d 3354 6f42 326a  ob99350wCM3ToB2j
+0003cd10: 2f61 6449 704b 6f54 5a67 5641 575a 7a45  /adIpKoTZgVAWZzE
+0003cd20: 524f 694a 4671 5271 4141 5045 7532 5170  ROiJFqRqAAPEu2Qp
+0003cd30: 6955 5235 6743 6a32 7134 7046 546c 674f  iUR5gCj2q4pFTlgO
+0003cd40: 4456 7837 4c54 4570 7a38 395a 594b 3979  DVx7LTEpz89ZYK9y
+0003cd50: 3468 6e34 6351 3648 524c 434a 3239 4c31  4hn4cQ6HRLCJ29L1
+0003cd60: 772f 6951 6141 5146 7453 2b54 4243 6b6d  w/iQaAQFtS+TBCkm
+0003cd70: 5942 2b78 6f67 6d36 4c6e 7035 4544 2f71  YB+xogm6Lnp5ED/q
+0003cd80: 4432 7538 432b 6665 6a34 664f 6269 6e38  D2u8C+fej4fObin8
+0003cd90: 4631 7067 7865 5130 4d46 3172 6f30 4745  F1pgxeQ0MF1ro0GE
+0003cda0: 6f47 4931 5a4a 3175 5176 6a72 4151 3470  oGI1ZJ1uQvjrAQ4p
+0003cdb0: 6171 715a 5036 6b41 2f62 506e 6e58 6f54  aqqZP6kA/bPnnXoT
+0003cdc0: 3258 2f6e 704f 6743 5744 496f 796f 432b  2X/npOgCWDIoyoC+
+0003cdd0: 556b 7152 5066 4453 4e33 4f48 6558 4456  UkqRPfDSN3OHeXDV
+0003cde0: 4a57 6832 4961 684d 6342 4a42 3343 5935  JWh2IahMcBJB3CY5
+0003cdf0: 6467 7a2b 3539 3734 3256 442f 2f72 3948  dgz+59742VD//r9H
+0003ce00: 6d68 5669 6671 5949 4553 7741 567a 5a62  mhVifqYIESwAVzZb
+0003ce10: 4e59 456f 6136 6a6c 5977 4b47 6d4a 464a  NYEoa6jlYwKGmJFJ
+0003ce20: 436a 4251 5171 506c 7645 6777 5842 7168  CjBQQqPlvEgwXBqh
+0003ce30: 3750 327a 717a 3532 6e48 582b 3958 4a70  7P2zqz52nHX+9XJp
+0003ce40: 3841 3848 6734 5048 5342 6177 3679 6e70  8A8Hg4PHSBaw6ynp
+0003ce50: 5249 5147 496c 6852 4563 4552 5558 5770  RIQGIlhREcERUXWp
+0003ce60: 634e 7238 7448 5078 4e47 6b46 4256 7952  cNr8tHPxNGkFBVyR
+0003ce70: 7737 7564 6242 3734 6248 5865 4363 644d  w7udbB74bHXeCcdM
+0003ce80: 4835 6a6d 4345 7447 3378 4475 4768 7a41  H5jmCEtG3xDuGhzA
+0003ce90: 4a6e 502b 3136 2f48 706e 7378 6364 6335  JnP+16/Hpnsxcdc5
+0003cea0: 4f30 392b 6b4b 5764 5054 2f32 6444 6c42  O09+kKWdPT/2dDlB
+0003ceb0: 2f56 5667 5970 4355 4c51 6653 6759 774e  /VVgYpCULQfSgYwN
+0003cec0: 674c 6d56 544c 4d6f 6d78 4246 4245 6d31  gLmVTLMomxBFBEm1
+0003ced0: 7342 7336 4871 3364 2b38 6e2b 7a31 792f  sBs6Hq3d+8n+z1y/
+0003cee0: 6334 6465 7050 534d 6749 524c 6165 7930  c4depPSMgIRLaey0
+0003cef0: 6530 4543 526f 7130 6d4c 7462 4342 4d55  e0ECRoq0mLtbCBMU
+0003cf00: 2b4d 6b66 4461 4d52 4e62 2b2f 6876 374a  +MkfDaMRNb+/hv7J
+0003cf10: 5937 6137 7846 754f 5a63 414c 3953 2f53  Y7a7xFuOZcAL9S/S
+0003cf20: 3141 2f43 4652 6549 3555 4945 6a45 6f73  1A/CFReI5UIEjEos
+0003cf30: 5946 772f 5362 6f61 4635 786d 556f 476d  YFw/SboaF5xmUoGm
+0003cf40: 5243 4271 6853 5648 4267 3553 7966 372b  RCBqhSVHBg5Syf7+
+0003cf50: 6f66 7666 726e 2f6f 7a50 4f46 574f 4734  ofvfrn/ozPOFWOG4
+0003cf60: 426c 3273 7943 7255 6e62 684b 3550 3279  Bl2syCrUnbhK5P2y
+0003cf70: 5639 3437 4857 6964 3933 6563 425a 5872  V947HWid93ecBZXr
+0003cf80: 7730 5837 5273 714b 6969 4f49 3354 4c42  w0X7RsqKiiOI3TLB
+0003cf90: 5846 5158 6238 4238 6f6b 6751 6165 4675  XFQXb8B8okgQaeFu
+0003cfa0: 7848 6141 6d4d 6738 5563 3654 746a 3374  xHaAmMg8Uc6Ttj3t
+0003cfb0: 437a 3778 5146 6676 6547 5333 6e64 6459  Cz7xQFfveGS3nddY
+0003cfc0: 6236 736f 6744 357a 5361 6936 775a 7245  b6sogD5zSai6wZrE
+0003cfd0: 304b 7455 6d47 7553 6e51 6242 6e7a 764b  0KtUmGuSnQbBnzvK
+0003cfe0: 3164 4271 7759 5476 2b4b 6867 6748 5a73  1dBqwYTv+KhggHZs
+0003cff0: 7259 6e2f 357a 6465 6268 766e 6237 666c  rYn/5zdebhvnb7fl
+0003d000: 5379 5476 4232 494d 524c 7373 4471 6b71  SyTvB2IMRLssDqkq
+0003d010: 7839 7541 454d 644d 5645 6430 544b 7734  x9uAEMdMVEd0TKw4
+0003d020: 5138 662f 6c76 642b 4a4a 312b 3850 5838  Q8f/lvd+JJ1+8PX8
+0003d030: 4c62 6368 334a 6772 7848 6363 5872 5159  Lbch3JgrxHccXrQY
+0003d040: 5454 3574 416a 7270 7449 6f46 7053 6e4a  TT5tAjrptIoFpSnJ
+0003d050: 4f61 4259 5967 7436 3674 4869 6233 4837  OaBYYgt66tHib3H7
+0003d060: 4d38 6365 7748 2f7a 3749 314f 4c76 4742  M8cewH/z7I1OLvGB
+0003d070: 4d70 5541 6f37 7252 4262 776c 4f53 4178  MpUAo7rRBbwlOSAx
+0003d080: 4f67 6850 5174 6650 2b5a 6373 6550 5130  OghPQtfP+ZcsePQ0
+0003d090: 3254 4371 6158 4d43 4d67 5443 6769 4b4a  2TCqaXMCMgTCgiKJ
+0003d0a0: 4b71 4245 7171 5936 4973 3265 2b57 3668  KqBEqqY6Is2e+W6h
+0003d0b0: 3672 2f2f 744a 5052 4359 3158 2f53 6f32  6r//tJPRCY1X/So2
+0003d0c0: 6f46 7869 3461 6b70 6674 476d 7247 5a4a  oFxi4akpftGmrGZJ
+0003d0d0: 4544 5176 556e 6776 7249 3042 4566 594e  EDQvUngvrI0BEfYN
+0003d0e0: 5658 4831 4577 3935 4b30 5776 2f65 4b6d  VXH1Ew95K0Wv/eKm
+0003d0f0: 7647 447a 6f43 6a67 7363 474e 304c 4335  vGDzoCjgscGN0LC5
+0003d100: 4e64 4342 5367 352b 372b 322b 3535 3944  NdCBSg5+7+2+559D
+0003d110: 7932 5669 4c49 4862 4774 692f 4b70 4877  y2ViLIHbGti/KpHw
+0003d120: 6c64 7577 364f 4a45 5332 3054 636f 476d  lduw6OJES20TcoGm
+0003d130: 5863 7634 306e 6e55 6a67 7375 3042 6365  Xcv40nnUjgsu0Bce
+0003d140: 7a2f 5630 4a53 725a 4830 5631 5461 7442  z/V0JSrZH0V1TatB
+0003d150: 7a61 5542 5865 4e39 6570 4874 3747 4858  zaUBXeN9epHt7GHX
+0003d160: 6e6c 664e 4f66 7766 5356 626a 4f68 664c  nlfNOfwfSVbjOhfL
+0003d170: 3038 3739 4251 7870 4f2b 5263 5044 3132  0879BQxpO+RcPD12
+0003d180: 3357 3070 6c6f 6e6b 4344 4375 6b57 4553  3W0plonkCDCukWES
+0003d190: 5664 532b 6e36 4f4c 3172 3951 764c 655a  VdS+n6OL1r9QvLeZ
+0003d1a0: 782b 7756 7137 466c 3850 5743 7878 692b  x+wVq7Fl8PWCxxi+
+0003d1b0: 5737 4239 5937 6662 3364 7633 3533 4f5a  W7B9Y7fb3dv353OZ
+0003d1c0: 756e 4549 4c55 3543 674e 5a74 6978 556a  unEILU5CgNZtixUj
+0003d1d0: 574c 7959 5943 7642 4f51 4c53 314b 7666  WLyYYCvBOQLS1Kvf
+0003d1e0: 7671 6235 4b73 6666 7751 6578 4d57 376a  vqb5KsffwQexMW7j
+0003d1f0: 766d 7832 2f66 4f54 3972 6c50 4647 5850  vmx2/fOT9rlPFGXP
+0003d200: 6869 3667 6a70 5a42 7474 5855 6d32 6741  hi6gjpZBttXUm2gA
+0003d210: 3576 3642 5470 6b57 4164 6e6e 4676 672b  5v6BTpkWAdnnFvg+
+0003d220: 4577 4330 6b77 3032 794b 4154 7245 7749  EwC0kw02yKATrEwI
+0003d230: 4345 744f 5733 5663 542b 4d58 356a 7143  CEtOW3VcT+MX5jqC
+0003d240: 4f4e 5841 6b48 7753 2b59 6c6a 616b 6b2f  ONXAkHwS+Yljakk/
+0003d250: 6969 4142 5938 7946 3541 5872 7851 7047  iiABY8yF5AXrxQpG
+0003d260: 304c 6e4c 5632 6659 6962 5155 6d57 4241  0LnLV2fYibQUmWBA
+0003d270: 442b 3173 3662 7852 5862 2f43 2f65 7739  D+1s6bxRXb/C/ew9
+0003d280: 2b65 7468 5133 4369 5674 5965 4a39 4265  +ethQ3CiVtYeJ9Be
+0003d290: 6837 6e4b 6363 5758 7a35 344c 376e 5044  h7nKccWXz54L7nPD
+0003d2a0: 7165 7a54 416f 3661 4c67 4e4a 5547 5938  qezTAo6aLgNJUGY8
+0003d2b0: 7251 3932 4c61 5247 4b4c 4141 444f 3335  rQ92LaRGKLAADO35
+0003d2c0: 6862 614c 3836 2b4c 2f48 4572 412b 3538  hbaL86+L/HErA+58
+0003d2d0: 4657 474d 7643 4744 366a 506e 3744 6643  FWGMvCGD6jPn7DfC
+0003d2e0: 574a 517a 304f 684f 6b54 5173 4b7a 4964  WJQz0OhOkTQsKzId
+0003d2f0: 6e55 5a61 7673 6d5a 7053 497a 6663 4c39  nUZavsmZpSIzfcL9
+0003d300: 6f71 475a 3149 507a 336f 6773 5854 314f  oqGZ1IPz3ogsXT1O
+0003d310: 7039 6265 4974 6677 4c5a 3976 5066 4971  p9beItfwLZ9vPfIq
+0003d320: 6d7a 5765 7678 2b52 3776 442b 7077 464e  mzWevx+R7vD+pwFN
+0003d330: 7072 626c 4f34 6268 5561 5053 464a 4442  prblO4bhUaPSFJDB
+0003d340: 5141 4b50 514d 4870 7a7a 3163 5473 4673  QAKPQMHpzz1cTsFs
+0003d350: 4643 574d 4169 4642 494b 6347 424f 6b51  FCWMAiFBIKcGBOkQ
+0003d360: 7842 4270 4d7a 6f39 714c 4756 424a 2f46  xBBpMzo9qLGVBJ/F
+0003d370: 4b69 4946 7145 4e34 306f 4a44 6969 6939  KiIFqEN40oJDiii9
+0003d380: 4742 6f71 624a 416b 4865 5873 5463 2b2b  GBoqbJAkHeXsTc++
+0003d390: 614e 392f 7774 7665 666b 4373 4133 3669  aN9/wtvefkCsA36i
+0003d3a0: 3552 3072 3847 3259 5a4b 4d4f 6c35 7168  5R0r8G2YZKMOl5qh
+0003d3b0: 6150 4d2b 2f57 7338 7334 3763 716f 5930  aPM+/Ws8s47cqoY0
+0003d3c0: 6d63 5374 2b7a 676a 6236 6776 4e4a 7447  mcSt+zgjb6gvNJtG
+0003d3d0: 346b 6843 704e 5035 3445 7958 4776 6869  4khCpNP54EyXGvhi
+0003d3e0: 7164 5466 332f 3549 6235 3454 5a4e 4f4a  qdTf3/5Ib54TZNOJ
+0003d3f0: 4968 3077 7645 6e37 7270 5434 6343 7835  Ih0wvEn7rpT4cCx5
+0003d400: 3741 6b58 7270 5643 4d75 4b62 4665 5851  7AkXrpVCMuKbFeXQ
+0003d410: 5149 4d4f 6955 7747 7874 7679 6331 5076  QIMOiUwGxtvyc1Pv
+0003d420: 6a4c 6e76 314f 7666 5077 5a6e 6745 4533  jLnv1OvfPwZngEE3
+0003d430: 6d37 454e 7867 6c55 4a53 4941 6a4b 4244  m7ENxglUJSIAjKBD
+0003d440: 784d 4468 7661 7261 5474 3277 7356 2b62  xMDhvaraTt2wsV+b
+0003d450: 6671 4139 7436 4577 6e44 3757 7164 5332  fqA9t6EwnD7WqdS2
+0003d460: 746c 5144 5979 6b4b 3173 5168 454c 6c69  tlQDYykK1sQhELli
+0003d470: 776d 7950 6f78 662b 5444 2b79 7a51 6159  wmyPoxf+TD+yzQaY
+0003d480: 6755 4e32 3047 6a46 6830 516e 6266 5552  gUN20GjFh0QnbfUR
+0003d490: 716f 4a74 4d53 7330 4430 3874 7172 7852  qoJtMSs0D08tqrxR
+0003d4a0: 6566 2b35 2b2b 5263 7859 3067 6848 3644  ef+5++RcxY0ghH6D
+0003d4b0: 4a7a 7168 4834 7745 4f50 3078 4330 2b4f  JzqhH4wEOP0xC0+O
+0003d4c0: 4b6a 6142 5238 6d46 4d6d 554c 5937 6362  KjaBR8mFMmULY7cb
+0003d4d0: 6179 594e 4834 6153 7955 4777 4b62 434e  ayYNH4aSyUGwKbCN
+0003d4e0: 7350 7954 466b 6b6c 4178 7367 546d 536a  sPyTFkklAxsgTmSj
+0003d4f0: 7046 7359 626e 7a30 7077 2f4f 302b 2f4f  pFsYbnz0pw/O0+/O
+0003d500: 3574 376e 7643 3336 314e 624f 5057 674d  5t7nvC361NbOPWgM
+0003d510: 2f30 2b39 5876 4257 5477 6b6f 746b 4752  /0+9XvBWTwkotkGR
+0003d520: 6255 7432 4a59 4b56 4253 4369 4954 756e  bUt2JYKVBSCiITun
+0003d530: 6e4d 5772 586f 712f 6367 6244 316b 726d  nMWrXoq/cgbD1krm
+0003d540: 6c75 4141 4a51 4b4e 6365 4859 5941 6b6e  luAAJQKNceHYYAkn
+0003d550: 4f37 4c41 4563 6778 514b 756f 414a 7154  O7LAEcgxQKuoAJqT
+0003d560: 6362 4b48 5435 7533 384c 4967 6439 6b74  cbKHT5u38LIgd9kt
+0003d570: 7645 6d46 474a 5156 495a 5374 6232 7344  vEmFGJQVIZStb2sD
+0003d580: 5541 3248 5665 4a57 6d71 3730 6d4f 4372  UA2HVeJWmq70mOCr
+0003d590: 412f 6a56 6a78 6339 4630 7352 4647 4849  A/jVjxc9F0sRFGHI
+0003d5a0: 6c6e 556f 4947 6477 704b 3853 6b42 677a  lnUoIGdwpK8SkBgz
+0003d5b0: 4b6a 6b76 5a58 3876 626e 3338 6e75 6666  KjkvZX8vbn38nuff
+0003d5c0: 6f6d 3146 6344 3577 3143 7144 4447 6761  om1FcD5w1CqDDGga
+0003d5d0: 2b6c 314c 4736 6a44 5342 6363 4447 4676  +l1LG6jDSBccDGFv
+0003d5e0: 4f38 4e47 3141 7270 6831 2b69 687a 5737  O8NG1Arph1+ihzW7
+0003d5f0: 7968 4974 7243 676f 4b78 4152 477a 4772  yhItrCgoKxARGzGr
+0003d600: 4f75 6c45 3069 694a 6e32 5274 7865 7365  OulE0iiJn2Rtxese
+0003d610: 4a71 7661 467a 6737 7a72 7365 4a6c 4a42  JqvaFzg7zrseJlJB
+0003d620: 5239 6e49 4746 3070 5741 5132 5a59 4f36  R9nIGF0pWAQ2ZYO6
+0003d630: 4b63 6b41 644f 7a68 5157 4a56 7a2b 364a  KckAdOzhQWJVz+6J
+0003d640: 7a58 7a2f 5939 7443 3939 394e 3043 2f41  zXz/Y9tC999N0C/A
+0003d650: 5551 426b 6742 4270 4841 6369 5463 6b69  UQBkgBBpHAciTcki
+0003d660: 527a 7741 3938 4344 514b 3138 6d7a 6633  RzwA98CDQK18mzf3
+0003d670: 5856 592f 3759 4464 6a68 5831 6d55 4f67  XVY/7YDdjhX1mUOg
+0003d680: 6932 7150 6b4a 6c71 4c4b 5553 7145 4336  i2qPkJlqLKUSqEC6
+0003d690: 435a 5a42 3446 655a 412b 5351 6830 5145  CZZB4FeZA+SQh0QE
+0003d6a0: 3252 3949 494c 4145 4574 484f 3963 4a55  2R9IILAEEtHO9cJU
+0003d6b0: 4554 3077 4b61 4d4f 6848 6a34 4456 574e  ET0wKaMOhHj4DVWN
+0003d6c0: 7237 4337 6e7a 6b64 3961 5331 566b 4738  r7C7nzkd9aS1VkG8
+0003d6d0: 7774 384b 4259 4a67 6553 416b 3661 6c6e  wt8KBYJgeSAk6aln
+0003d6e0: 6849 4572 3446 6478 7a78 5271 3846 7a72  hIEr4FdxzxRq8Fzr
+0003d6f0: 6f41 3553 5769 4549 5a69 5963 7642 3463  oA5SWiEIZiYcvB4c
+0003d700: 6441 755a 386d 6139 4642 6443 5630 6531  dAuZ8ma9FBdCV0e1
+0003d710: 4c49 6f44 714b 6b66 6968 4e46 676f 7771  LIoDqKkfihNFgowq
+0003d720: 6d79 3645 3670 384b 6c6e 7067 5332 4936  my6E6p8KlnpgS2I6
+0003d730: 3044 394d 4146 446d 4c7a 3457 5776 7836  0D9MAFDmLz4WWvx6
+0003d740: 6d63 7966 3337 6d66 7236 324f 5963 6b67  mcyf37mfr62OYckg
+0003d750: 504f 4178 544a 4a78 3864 4836 516b 774e  POAxTJJx8dH6QkwN
+0003d760: 3442 3935 4443 5378 4975 3836 4533 4153  4B95DCSxIu86E3AS
+0003d770: 4954 424b 7854 3437 685a 6b42 5272 4248  ITBKxT47hZkBRrBH
+0003d780: 4333 6879 4c62 4a45 7734 706a 4f6a 2f56  C3hyLbJEw4pjOj/V
+0003d790: 6468 7664 6265 2b74 4577 4536 4d6f 5742  dhvdbe+tEwE6MoWB
+0003d7a0: 4948 656f 5631 486c 5948 4842 466b 6678  IHeoV1HlYHHBFkfx
+0003d7b0: 6931 2f53 486b 5151 4966 6b30 4e48 5168  i1/SHkQQIfk0NHQh
+0003d7c0: 7171 784b 786e 5955 4548 7065 5776 6b79  qqxKxnYUEHpeWvky
+0003d7d0: 782f 6434 547a 3038 7275 694f 5565 4833  x/d4Tz08ruiOUeH3
+0003d7e0: 724d 3865 7034 4a58 3077 6955 7542 5153  rM8ep4JX0wiUuBQS
+0003d7f0: 6e64 2f48 4534 7044 6277 4750 7549 4251  nd/HE4pDbwGPuIBQ
+0003d800: 7839 3635 4b4d 6374 7539 6636 3531 3978  x965KMctu9f6519x
+0003d810: 4d6c 6975 3735 4863 4276 6d4a 6c43 6f71  Mliu75HcBvmJlCoq
+0003d820: 6f59 756e 3154 5451 6253 426b 6b78 3678  oYun1TTQbSBkkx6x
+0003d830: 4762 5367 3753 4954 6376 316b 674d 5432  GbSg7SITcv1kgMT2
+0003d840: 334b 4c55 732b 2b2b 3373 5974 7333 6c5a  3KLUs+++3sYts3lZ
+0003d850: 6537 6563 3865 7838 5836 4b6a 674a 4b76  e7ec8ex8X6KjgJKv
+0003d860: 416b 7336 4547 5941 354a 4757 7844 546e  Aks6EGYA5JGWxDTn
+0003d870: 7355 6676 5633 766c 6f4e 324f 682b 4758  sUfvV3vloN2Oh+GX
+0003d880: 2f76 6a38 312b 6d54 6752 5476 3468 7536  /vj81+mTgRTv4hu6
+0003d890: 7169 4643 554b 376a 7049 4264 5234 545a  qiFCUK7jpIBdR4TZ
+0003d8a0: 4c30 6767 7341 6352 4464 7030 4a44 7156  L0ggsAcRDdp0JDqV
+0003d8b0: 3836 4761 7247 3979 4959 5875 3959 3076  86GarG9yIYXu9Y0v
+0003d8c0: 6359 6565 7531 652f 7470 4879 3344 7944  cYeeu1e/tpHy3DyD
+0003d8d0: 5364 4643 7969 6768 6c4e 7732 4d30 6341  SdFCyighlNw2M0cA
+0003d8e0: 386b 524a 5161 2b6e 3247 3135 5548 6753  8kRJQa+n2G15UHgS
+0003d8f0: 3650 7268 307a 4137 4862 7177 5875 4941  6Prh0zA7HbqwXuIA
+0003d900: 3861 654c 6450 4a67 5651 5a58 5157 7353  8aeLdPJgVQZXQWsS
+0003d910: 3147 644b 4d6d 6b52 3277 6d50 5569 4c32  1GdKMmkR2wmPUiL2
+0003d920: 4c52 5577 7154 4456 6e51 794b 6342 306d  LRUwqTDVnQyKcB0m
+0003d930: 5051 2f42 7050 2b66 396f 4c56 3063 2b6d  PQ/BpP+f9oLV0c+m
+0003d940: 6c41 4774 7331 3445 735a 5651 4259 6b42  lAGts14EsZVQBYkB
+0003d950: 7049 457a 6532 4967 684e 3561 4442 666f  pIEze2IghN5aDBfo
+0003d960: 4b38 4633 625a 394c 3532 3257 6965 5050  K8F3bZ9L522WiePP
+0003d970: 386f 6431 4773 6173 7978 3150 3862 554c  8od1Gsasyx1P8bUL
+0003d980: 3649 4864 597a 6f68 484a 326e 5251 545a  6IHdYzohHJ2nRQTZ
+0003d990: 414e 5142 4e46 5873 534b 4e70 3972 504b  ANQBNFXsSKNp9rPK
+0003d9a0: 4246 6232 594f 6862 444c 6e72 7251 2f57  BFb2YOhbDLnrrQ/W
+0003d9b0: 6a69 442f 6547 7870 2f46 7972 534b 4866  jiD/eGxp/FyrSKHf
+0003d9c0: 6f57 5672 6b7a 6866 4150 3275 534f 766b  oWVrkzhfAP2uSOvk
+0003d9d0: 632b 334f 2f74 7545 494e 3656 3776 6e48  c+3O/tuEIN6V7vnH
+0003d9e0: 334f 3675 744b 6c4a 7469 3668 7170 655a  3O6utKlJti6hqpeZ
+0003d9f0: 6571 4a45 624c 6f4e 4356 426c 4f35 6255  eqJEbLoNCVBlO5bU
+0003da00: 6270 4b49 7873 4576 4455 374c 2f48 4368  bpKIxsEvDU7L/HCh
+0003da10: 3339 4b50 7633 6578 7831 3675 6849 6743  39KPv3exx16uhIgC
+0003da20: 6443 6238 4b54 742b 4541 5962 5132 3843  dCb8KTt+EAYbQ28C
+0003da30: 5134 336f 616e 5573 4173 3943 4179 317a  Q43oanUsAs9CAy1z
+0003da40: 4a44 4c41 714c 6b78 6736 4275 636c 4f46  JDLAqLkxg6BuclOF
+0003da50: 3870 4d45 7639 4674 6132 7170 5974 576b  8pMEv9Fta2qpYtWk
+0003da60: 5568 564f 374b 6a4e 4170 4179 476d 7254  UhVO7KjNApAyGmrT
+0003da70: 7234 364a 6b67 4834 4f4f 5750 6451 4b4c  r46JkgH4OOWPdQKL
+0003da80: 6159 2f48 4b63 6172 6c33 4855 4761 7761  aY/HKcarl3HUGawa
+0003da90: 7757 6864 6254 4234 7647 4731 7266 5933  wWhdbTB4vGG1rfY3
+0003daa0: 3536 2b51 3336 7763 4232 2b78 6866 3148  56+Q36wcB2+xhf1H
+0003dab0: 4454 584b 4345 484a 4e4b 6846 3634 6e5a  DTXKCEHJNKhF64nZ
+0003dac0: 4147 474a 5a33 735a 4f55 6738 6237 4a6c  AGGJZ3sZOUg8b7Jl
+0003dad0: 2f59 5a36 302f 6137 5479 5a53 677a 456e  /YZ60/a7TyZSgzEn
+0003dae0: 6b6a 316f 7932 617a 7145 3354 3261 5468  kj1oy2azqE3T2aTh
+0003daf0: 6e47 6c64 4a6f 634d 4e65 7746 3639 364b  nGldJocMNewF696K
+0003db00: 6e58 6663 2f2b 776c 712b 4474 7473 3449  nXfc/+wlq+Dtts4I
+0003db10: 456b 416e 4b64 534e 6e6b 5435 416e 6573  EkAnKdSNnkT5Anes
+0003db20: 5243 4b4b 4e51 7171 4476 466e 6b51 4151  RCKKNQqqDvFnkQAQ
+0003db30: 5952 742b 6149 7562 5763 5048 6e75 774f  YRt+aIubWcPHnuwO
+0003db40: 376a 5042 637a 6952 6639 6c4b 6852 4b4e  7jPBcziRf9lKhRKN
+0003db50: 3357 506d 6b67 7879 5a41 5a71 446c 7462  3WPmkgxyZAZqDltb
+0003db60: 5155 544a 4449 7537 5262 7766 7438 392f  QUTJDIu7Rbwft89/
+0003db70: 5370 7739 6f6d 7731 5853 676f 3948 4744  Spw9omw1XSgo9HGD
+0003db80: 4241 3547 5068 6345 5a2b 7a34 4537 356d  BA5GPhcEZ+z4E75m
+0003db90: 7766 2f34 6978 6331 515a 6445 386d 4158  wf/4ixc1QZdE8mAX
+0003dba0: 7938 454f 7044 3377 4d36 4b30 3157 4d51  y8EOpD3wM6K01WMQ
+0003dbb0: 4f2f 4146 2f32 6767 3844 4b6b 7036 344c  O/AF/2gg8DKkp64L
+0003dbc0: 6668 6d65 3573 4b6a 7266 6350 6c71 306b  fhme5sKjrfcPlq0k
+0003dbd0: 7639 3732 6574 7955 422b 4831 5665 462f  v972etyUB+H1VeF/
+0003dbe0: 3663 514d 356a 4e59 3331 566f 4f4e 4b4b  6cQM5jNY31VoONKK
+0003dbf0: 646f 337a 4548 5269 4131 5569 7258 6c46  do3zEHRiA1UirXlF
+0003dc00: 6961 652f 2b43 3351 4935 6e72 4b5a 736d  iae/+C3QI5nrKZsm
+0003dc10: 572b 3864 4170 514d 3268 7848 392b 3467  W+8dApQM2hxH9+4g
+0003dc20: 704d 4376 6e2f 6c30 4275 514f 4f69 6959  pMCvn/l0BuQOOiiY
+0003dc30: 7641 6c59 596e 7672 7742 446f 4735 5948  vAlYYnvrwBDoG5YH
+0003dc40: 5877 4a68 595a 6850 4f64 3669 632b 5766  XwJhYZhPOd6ic+Wf
+0003dc50: 5172 6b65 4d50 7656 644f 584f 665a 3234  QrkeMPvVdOXOfZ24
+0003dc60: 5835 5153 4c6f 5242 4b4e 4839 7450 734d  X5QSLoRBKNH9tPsM
+0003dc70: 3454 2f6c 3530 784d 3337 5570 4150 7758  4T/l50xM37UpAPwX
+0003dc80: 5a63 3932 4970 7a45 476f 712b 696d 706f  Zc92IpzEGoq+impo
+0003dc90: 4732 5268 6f30 6544 4469 496a 6662 4472  G2Rho0eDDiIjfbDr
+0003dca0: 3339 5050 7637 6d66 3378 3850 3975 3248  39PPv7mf3x8P9u2H
+0003dcb0: 5a68 6632 7379 4459 386c 416c 6e67 5065  Zhf2syDY8lAlngPe
+0003dcc0: 7463 4342 6841 6376 495a 5867 4445 5944  tcCBhAcvIZXgDEYD
+0003dcd0: 6837 5131 7057 4155 7232 544a 2b37 6837  h7Q1pWAUr2TJ+7h7
+0003dce0: 622f 6a6d 6177 7144 5a30 486a 5668 5a2f  b/jmawqDZ0HjVhZ/
+0003dcf0: 436c 4a43 5062 4447 4143 6c4e 684a 776c  ClJCPbDGAClNhJwl
+0003dd00: 7656 4533 6c36 7935 706e 4d33 552f 6568  vVE3l6y5pnM3U/eh
+0003dd10: 3165 6f4b 4730 7a67 5a30 647a 3437 6f55  1eoKG0zgZ0dz47oU
+0003dd20: 4848 594a 6341 4c4d 6775 6d4a 3351 2f4d  HHYJcALMgumJ3Q/M
+0003dd30: 5a79 502b 4468 7073 7977 6159 766e 6753  ZyP+DhpsywaYvngS
+0003dd40: 6142 4b30 4c72 4d73 784b 4f35 3163 6c5a  aBK0LrMsxKO51clZ
+0003dd50: 644e 4a2b 2f34 4935 6d42 4867 4130 4861  dNJ+/4I5mBHgA0Ha
+0003dd60: 5141 4964 5056 5243 5863 7661 6764 564a  QAIdPVRCXcvagdVJ
+0003dd70: 3851 655a 5033 672f 5338 3737 5172 6f7a  8QeZP3g/S877Qroz
+0003dd80: 576e 5666 7446 4756 4c6f 2b71 536b 4548  WnVftFGVLo+qSkEH
+0003dd90: 5968 435a 4864 4b62 4e39 2f64 3936 6a5a  YhCZHdKbN9/d96jZ
+0003dda0: 6f6b 7a66 3856 7133 3350 7034 314a 3035  okzf8Vq33Pp41J05
+0003ddb0: 6f4f 6a69 5a70 6541 5455 5958 7348 4171  oOjiZpeATUYXsHAq
+0003ddc0: 3658 6734 6855 7166 5031 4f62 376c 7243  6Xg4hUqfP1Ob7lrC
+0003ddd0: 5149 6274 5759 7657 4f5a 3873 7667 5662  QIbtWYvWOZ8svgVb
+0003dde0: 326a 2f46 4b74 4e44 3845 7557 4859 2f79  2j/FKtND8EuWHY/y
+0003ddf0: 746d 4d43 5356 5556 3762 6d46 3653 666d  tmMCSVUV7bmF6Sfm
+0003de00: 4856 4c36 7538 7650 6375 6273 2b47 5853  HVL6u8vPcubs+GXS
+0003de10: 7a59 4453 4143 5546 4944 2f78 4b73 5448  zYDSACUFID/xKsTH
+0003de20: 4339 6e67 2b66 6743 5a79 3171 656b 617a  C9ng+fgCZy1qekaz
+0003de30: 454f 7769 7568 2b68 512f 7234 4e30 6a63  EOwiuh+hQ/r4N0jc
+0003de40: 432f 4354 6e43 5247 7a47 3464 3875 6834  C/CTnCRGzG4d8uh4
+0003de50: 7934 5456 636c 4459 494f 4f32 6867 454a  y4TVclDYIOO2hgEJ
+0003de60: 4247 7759 6b51 5037 4747 376b 7730 6166  BGwYkQP7GG7kw0af
+0003de70: 3062 626a 4a6b 6661 6b76 466f 6673 4a63  0bbjJkfakvFofsJc
+0003de80: 766d 7059 3644 7637 6b36 4e46 6d30 3539  vmpY6Dv7k6NFm059
+0003de90: 5174 7452 5233 4947 4945 436a 6c55 6e68  QttRR3IGIECjlUnh
+0003dea0: 7659 3953 4f34 2b73 722f 3932 644c 3365  vY9SO4+sr/92dL3e
+0003deb0: 5650 5778 5775 5769 6952 777a 4745 416a  VPWxWuWiiRwzGEAj
+0003dec0: 5638 796b 316e 5874 396f 4b6e 7636 7147  V8yk1nXt9oKnv6qG
+0003ded0: 5434 7052 4d39 546f 4b39 424a 7548 474d  T4pRM9ToK9BJuHGM
+0003dee0: 4f67 7972 4773 7432 4b39 392f 4235 4d69  OgyrGst2K99/B5Mi
+0003def0: 4f66 3767 2f72 7341 454d 5239 5538 2b7a  Of7g/rsAEMR9U8+z
+0003df00: 5834 4541 5570 744d 3061 5551 4135 372f  X4EAUptM0aUQA57/
+0003df10: 7371 4855 2f63 2b66 6166 7a37 7279 6c48  sqHU/c+fafz7rylH
+0003df20: 4b5a 4b6d 4c6f 3551 474c 6776 744a 2b6f  KZKmLo5QGLgvtJ+o
+0003df30: 7748 4a59 6578 774c 7263 3834 6673 7539  wHJYexwLrc84fsu9
+0003df40: 3245 3842 6331 6e34 5156 426d 6f63 5155  2E8Bc1n4QVBmocQU
+0003df50: 6644 714f 4641 4a33 4c48 6664 4f51 6542  fDqOFAJ3LHfdOQeB
+0003df60: 2b66 4744 6673 2b53 7963 6d62 4134 3577  +fGDfs+SycmbA45w
+0003df70: 4465 324a 727a 634a 5333 2f2b 3949 4748  De2JrzcJS3/+9IGH
+0003df80: 2b4c 734c 6e51 3351 5669 6669 3736 386a  +LsLnQ3QVifi768j
+0003df90: 4e6e 3256 4f69 642b 7039 7471 6761 6c68  Nn2VOid+p9tqgalh
+0003dfa0: 6a53 7472 4b55 5378 7159 442b 4e45 7872  jStrKUSxqYD+NExr
+0003dfb0: 3071 5046 5076 7365 4c44 7333 574d 6c2f  0qPFPvseLDs3WMl/
+0003dfc0: 326a 7855 6867 4671 5046 3150 752f 4c6c  2jxUhgFqPF1Pu/Ll
+0003dfd0: 6d7a 4268 756d 6d47 674f 675a 3448 536b  mzBhummGgOgZ4HSk
+0003dfe0: 4363 5170 6236 4157 396f 434a 4d45 686e  CcQpb6AW9oCJMEhn
+0003dff0: 4456 6e30 624c 456e 4555 762b 6d4d 4739  DVn0bLEnEUv+mMG9
+0003e000: 3264 5636 6d36 3571 6a71 4667 517a 3244  2dV6m65qjqFgQz2D
+0003e010: 6158 724e 6a70 5076 2f76 7a39 4a2b 6665  aXrNjpPv/vz9J+fe
+0003e020: 6370 7162 4e76 5575 5559 526b 4151 6f38  cpqbNvUuUYRkAQo8
+0003e030: 5944 5464 596f 6f4f 6143 6936 4744 782f  YDTdYooOaCi6GDx/
+0003e040: 6766 5177 4f65 4676 4175 7467 6c38 4742  gfQwOeFvAutgl8GB
+0003e050: 7548 6747 4976 7573 7564 3248 4e79 7664  uHgGIvusud2HNyvd
+0003e060: 664b 6546 336e 3936 382b 465a 7578 6871  fKeF3n968+FZuxhq
+0003e070: 7177 446a 5367 3541 4245 3961 6f5a 4d4f  qwDjSg5ABE9aoZMO
+0003e080: 4c61 3961 2b56 732b 2b2f 732b 6565 4c6b  La9a+Vs++/s+eeLk
+0003e090: 696f 4a33 5536 5156 5166 7935 6630 4837  ioJ3U6QVQfy5f0H7
+0003e0a0: 4c6f 4161 6e49 6b48 4934 5574 694b 3156  LoAanIkHI4UtiK1V
+0003e0b0: 6d6b 4869 6f51 3651 3347 6e41 7343 5a72  mkHioQ6Q3GnAsCZr
+0003e0c0: 6b59 4d37 7257 2f32 4776 4d45 4c36 7363  kYM7rW/2GvMEL6sc
+0003e0d0: 5936 5976 366a 5267 556b 6c6e 4930 684c  Y6Yv6jRgUklnI0hL
+0003e0e0: 3031 4638 4551 4947 5156 3042 3241 476b  01F8EQIGQV0B2AGk
+0003e0f0: 4949 6353 7353 6234 4759 7736 4649 3074  IIcSsSb4GYw6FI0t
+0003e100: 6862 6b77 4634 6350 4e32 2b56 476a 7076  hbkwF4cPN2+VGjpv
+0003e110: 7047 4151 4a74 5a61 3235 7835 7337 482f  pGAQJtZa25x5s7H/
+0003e120: 715a 6a6d 7730 6b67 6645 6145 6f6b 4243  qZjmw0kgfEaEokBC
+0003e130: 6848 4445 726a 4c77 4169 3067 6166 4142  hHDErjLwAi0gafAB
+0003e140: 786e 4a63 5141 6859 4c77 7138 7249 4138  xnJcQAhYLwq8rIA8
+0003e150: 784d 7065 6c54 627a 5966 7365 6d42 2b39  xMpelTbzYfsemB+9
+0003e160: 7845 2f6b 716e 6b4c 7268 4a55 2b57 6730  xE/kqnkLrhJU+Wg0
+0003e170: 6b5a 6f53 5968 4553 755a 6150 6854 3468  kZoSYhESuZaPhT4h
+0003e180: 4244 5a43 334d 5858 3963 6c63 366f 7442  BDZC3MXX9clc6otB
+0003e190: 5478 3564 6939 6d6a 3556 2b71 2f73 6748  Tx5di9mj5V+q/sgH
+0003e1a0: 4b4f 7651 4565 6554 3831 6f47 6a4d 7169  KOvQEeeT81oGjMqi
+0003e1b0: 6d79 5273 3151 6736 626a 6a67 5864 3437  myRs1Qg6bjjgXd47
+0003e1c0: 3771 4478 666c 4858 6d64 4e4f 3259 4354  7qDxflHXmdNO2YCT
+0003e1d0: 4e4a 394f 4f41 7768 4b62 4a4a 3137 4352  NJ9OOAwhKbJJ17CR
+0003e1e0: 4156 2f77 424c 3835 7a56 7772 4b48 5434  AV/wBL85zVwrKHT4
+0003e1f0: 4564 4563 444d 4f6e 5648 5667 7645 7567  EdEcDMOnVHVgvEug
+0003e200: 3935 6538 5153 6371 6f32 686a 6d4d 4153  95e8QScqo2hjmMAS
+0003e210: 7865 566a 6675 412b 344d 3637 5238 735a  xeVjfuA+4M67R8sZ
+0003e220: 7439 772f 3330 314a 6365 6e44 4b68 3977  t9w/301JcenDKh9w
+0003e230: 4e39 4257 306b 597a 4d45 434e 7366 3343  N9BW0kYzMECNsf3C
+0003e240: 6f57 2b56 5537 6a79 5874 6635 6f37 7166  oW+VU7jyXtf5o7qf
+0003e250: 7957 6358 5870 682f 594b 7147 6d68 6470  yWcXXph/YKqGmhdp
+0003e260: 3541 5748 6942 5549 356d 6c64 4d47 3133  5AWHiBUI5mldMG13
+0003e270: 2b71 6c55 3263 3054 4c32 7855 5673 7246  +qlU2c0TL2xUVsrF
+0003e280: 7431 4f6b 4832 2f4e 6a5a 566b 3679 7830  t1OkH2/NjZVk6yx0
+0003e290: 756e 3043 3341 3650 7779 3636 6a33 516e  un0C3A6Pwy66j3Qn
+0003e2a0: 6c6d 5661 6736 4762 6d41 5643 6473 2b56  lmVag6GbmAVCds+V
+0003e2b0: 4652 5342 444b 5a47 4f4a 5048 4865 7466  FRSBDKZGOJPHHetf
+0003e2c0: 394f 466c 2f41 3952 7452 4c61 654f 4278  9OFl/A9RtRLaeOBx
+0003e2d0: 3665 3866 6141 4845 5157 4746 5843 734e  6e8faAHEQWGFXCsN
+0003e2e0: 456b 5153 4251 5178 7131 3246 556d 7342  EkQSBQQxq12FUmsB
+0003e2f0: 4630 3444 5464 4769 6f6d 426a 4a52 4375  F04DTdGiomBjJRCu
+0003e300: 3951 4656 3961 7737 7557 4755 3270 2f63  9QFV9aw7uWGU2p/c
+0003e310: 6664 784f 4158 7a44 5351 4b63 6750 6142  fdxOAXzDSQKcgPaB
+0003e320: 2b66 6953 424c 6268 725a 4b57 5837 4447  +fiSBLbhrZKWX7DG
+0003e330: 5964 4d61 6a70 6a30 7039 4662 6457 6873  YdMajpj0p9FbdWhs
+0003e340: 4449 3143 3230 6f71 4338 6f57 7163 6a45  DI1C20oqC8oWqcjE
+0003e350: 4e67 6a43 4934 644b 464a 2b41 4855 344c  NgjCI4dKFJ+AHU4L
+0003e360: 5650 7458 3265 6c77 4931 3377 5835 7561  VPtX2elwI13wX5ua
+0003e370: 5a69 2b30 4332 5949 6d66 5936 377a 6174  Zi+0C2YImfY67zat
+0003e380: 4639 6f34 544a 6667 4b50 6e35 4a4b 3533  F9o4TJfgKPn5JK53
+0003e390: 4e4f 7578 5636 4877 376b 4848 4a52 6551  NOuxV6Hw7kHHJReQ
+0003e3a0: 534e 534f 3065 4f51 4a51 6367 6171 5579  SNSO0eOQJQcgaqUy
+0003e3b0: 426d 4c73 3572 3047 4c48 6e6d 496d 7358  BmLs5r0GLHnmImsX
+0003e3c0: 2f30 532b 392f 4c6c 3875 6353 312f 3874  /0S+9/Ll8ucS1/8t
+0003e3d0: 4779 6273 7348 7743 6d2b 6351 4536 384b  GybssHwCm+cQE68K
+0003e3e0: 6759 5250 5466 4245 5267 4e53 3241 4d41  gYRPTfBERgNS2AMA
+0003e3f0: 6764 5662 5774 6a59 634d 634b 4a31 4f63  gdVbWtjYcMcKJ1Oc
+0003e400: 466a 3830 594d 4869 6533 3637 4976 6446  Fj80YMHie367IvdF
+0003e410: 4c5a 4b79 616f 4370 414c 4d66 6b41 3943  LZKyaoCpALMfkA9C
+0003e420: 6e35 442b 7256 5058 7354 374b 7768 4b37  n5D+rVPXsT7KwhK7
+0003e430: 6953 5142 4f41 3161 4c50 4677 796e 6c4f  iSQBOA1aLPFwynlO
+0003e440: 6641 6657 6446 4e51 5a77 6857 5269 3166  fAfWdFNQZwhWRi1f
+0003e450: 4d75 7966 5879 3847 5159 2b6e 7033 6766  MuyfXy8GQY+np3gf
+0003e460: 6d37 4379 4837 4e70 3033 3872 6a2b 7735  m7CyH7Np038rj+w5
+0003e470: 396b 7731 3144 2f32 3144 5854 556c 455a  9kw11D/21DXTUlEZ
+0003e480: 3353 7453 7459 4d68 642b 5253 466d 585a  3StStYMhd+RSFmXZ
+0003e490: 4f70 7150 2b59 7732 307a 6b6b 3162 5078  OpqP+Yw20zkk1bPx
+0003e4a0: 552f 4978 6e75 6578 2f38 2b58 4c48 6f56  U/Ixnuex/8+XLHoV
+0003e4b0: 672f 797a 6d63 3139 4145 4375 3736 4732  g/yzmc19AECu76G2
+0003e4c0: 7445 5272 7652 5356 5636 6973 6532 4668  tERrvRSVV6ise2Fh
+0003e4d0: 4a63 2f44 6737 6833 5a41 4163 7768 4d56  Jc/Dg7h3ZAAcwhMV
+0003e4e0: 6131 754f 7046 4230 4832 4d45 7367 6741  a1uOpFB0H2MEsggA
+0003e4f0: 472f 6939 504d 5033 7656 7139 356f 7a4c  G/i9PMP3vVq95ozL
+0003e500: 3250 3936 784c 4144 5268 4330 456d 5568  2P96xLADRhC0EmUh
+0003e510: 6866 476d 3241 6348 3962 446a 6d53 4758  hfGm2AcH9bDjmSGX
+0003e520: 5567 5358 4d69 3245 6342 3743 315a 564f  UgSXMi2EcB7C1ZVO
+0003e530: 6d6b 6c48 6678 4956 6753 3654 6b48 4645  mklHfxIVgS6TkHFE
+0003e540: 5345 3564 444b 546a 6d4d 7857 4a39 6e55  SE5dDKTjmMxWJ9nU
+0003e550: 7033 3633 2b35 4541 6c69 7772 6b58 444b  p363+5EAliwrkXDK
+0003e560: 6467 6638 686f 7774 6142 3978 6a2f 7946  dgf8howtaB9xj/yF
+0003e570: 5051 4172 7738 6b6f 5745 5672 4f59 7978  PQArw8koWEVrOYyx
+0003e580: 3345 6254 3538 3073 5758 796e 7265 4a32  3EbT580sWXynreJ2
+0003e590: 6a52 3444 6159 2f45 4b47 4373 4d70 6850  jR4DaY/EKGCsMphP
+0003e5a0: 5475 3267 776f 4a73 4d79 546c 6e56 4771  Tu2gwoJsMyTlnVGq
+0003e5b0: 7462 3561 624c 6555 532b 4a36 5946 5653  tb5abLeUS+J6YFVS
+0003e5c0: 324e 5638 4332 4353 6b57 3345 6951 3565  2NV8C2CSkW3EiQ5e
+0003e5d0: 7168 305a 4230 7474 6c39 4453 366f 324a  qh0ZB0ttl9DS6o2J
+0003e5e0: 5a79 3661 696d 6243 3675 386c 6375 765a  Zy6aimbC6u8lcuvZ
+0003e5f0: 4156 3347 7378 4e50 6c56 746a 5775 4642  AV3GsxNPlVtjWuFB
+0003e600: 7948 6f5a 4246 7073 6c43 677a 5369 6873  yHoZBFpslCgzSihs
+0003e610: 7952 5933 3772 4476 4f76 502f 5a31 2f2f  yRY37rDvOvP/Z1//
+0003e620: 7248 3738 4978 4477 7770 6877 3741 4c69  rH78IxDwwphw7ALi
+0003e630: 4148 5455 7838 6e71 3658 444c 7578 735a  AHTUx8nq6XDLuxsZ
+0003e640: 7468 6c62 4f73 4665 4132 3747 6a70 3264  thlbOsFeA27Gjp2d
+0003e650: 5359 4259 3359 3451 5563 386f 4b35 6e57  SYBY3Y4QUc8oK5nW
+0003e660: 4738 566d 4768 5158 3631 4178 2b49 736b  G8VmGhQX61Ax+Isk
+0003e670: 5568 5956 6455 704a 4277 5a79 3841 5141  UhYVdUpJBwZy8AQA
+0003e680: 3048 6b41 4642 6469 5268 3030 342f 326a  0HkAFBdiRh004/2j
+0003e690: 2f61 5443 4946 6551 2f69 3241 384d 7161  /aTCIFeQ/i2A8Mqa
+0003e6a0: 586b 772b 4850 6264 682f 5261 2b33 6c4a  Xkw+HPbdh/Ra+3lJ
+0003e6b0: 3179 5a48 7a50 7757 756e 5941 3849 3256  1yZHzPwWunYA8I2V
+0003e6c0: 5546 514e 6453 4353 4b54 7552 585a 7778  UFQNdSCSKTuRXZwx
+0003e6d0: 454b 3251 6549 646a 6c4e 3165 4361 5465  EK2QeIdjlN1eCaTe
+0003e6e0: 5a6b 3167 3630 3143 6534 7478 3457 5470  Zk1g601Ce4tx4WTp
+0003e6f0: 4461 5279 6654 4765 2b57 746a 4734 6c53  DaRyfTGe+WtjG4lS
+0003e700: 4f47 7a68 5545 444f 5433 7256 504f 7568  OGzhUEDOT3rVPOuh
+0003e710: 5434 4752 4547 5356 5066 7037 7957 574c  T4GREGSVPfp7yWWL
+0003e720: 482f 5561 5777 3953 6b72 784a 7867 6274  H/UaWw9SkrxJxgbt
+0003e730: 4a69 4430 4a34 632b 7669 4541 5348 4970  JiD0J4c+viEASHIp
+0003e740: 3230 796d 527a 7348 5442 3275 6e76 6456  20ymRzsHTB2unvdV
+0003e750: 3738 7239 687a 6445 382b 694d 4f43 4338  78r9hzdE8+iMOCC8
+0003e760: 5465 6555 5a55 3377 5136 6c76 416c 4b36  TeeUZU3wQ6lvAlK6
+0003e770: 4768 4945 7433 784f 707a 4541 7a46 344d  GhIEt3xOpzEAzF4M
+0003e780: 7557 6731 3542 4f49 6d7a 5877 4876 4132  uWg15BOImzXwHvA2
+0003e790: 4131 5158 4230 4967 7268 5751 4271 5441  A1QXB0IgrhWQBqTA
+0003e7a0: 5979 5a79 4a76 4163 4331 4a77 7a59 4e72  YyZyJvAcC1JwzYNr
+0003e7b0: 4150 5770 3533 586f 4955 3849 666b 4d33  APWp53XoIU8IfkM3
+0003e7c0: 432f 6350 3578 666b 4134 6541 3070 7834  C/cP5xfkA4eA0px4
+0003e7d0: 632f 7a36 7174 3530 356d 5444 6d30 3959  c/z6qt505mTDm09Y
+0003e7e0: 5a38 2f69 7671 7134 3343 6a30 5462 4651  Z8/ivqq43Cj0TbFQ
+0003e7f0: 4173 5636 4353 7942 7a72 4136 4843 6734  AsV6CSyBzrA6HCg4
+0003e800: 4465 6263 2f2f 5552 4b4c 3636 6b54 4b41  Debc//URKL66kTKA
+0003e810: 6e2f 5278 4b79 7146 4f56 416b 6c41 2b41  n/RxKyqFOVAklA+A
+0003e820: 687a 7343 6b65 3345 6754 6838 5361 4f43  hzsCke3EgTh8SaOC
+0003e830: 2b6f 4253 6467 6149 456b 6550 4570 6570  +oBSdgaIEkePEpep
+0003e840: 6762 3345 5935 6661 4b68 6175 4f68 3756  gb3EY5faKhauOh7V
+0003e850: 7334 3948 5272 2f50 3944 7056 6237 4967  s49HRr/P9DpVb7Ig
+0003e860: 6154 4453 4e45 5357 7868 524d 5669 4857  aTDSNESWxhRMViHW
+0003e870: 3562 442b 7659 3477 7676 4735 4639 3558  5bD+vY4wvvG5F95X
+0003e880: 7a74 3641 6b38 4154 5843 3430 5734 5344  zt6Ak8ATXC40W4SD
+0003e890: 354d 5650 4175 5847 5859 6879 4161 7734  5MVPAuXGXYhyAaw4
+0003e8a0: 4353 5078 4f43 5a70 494e 6567 7849 5251  CSPxOCZpINegxIRQ
+0003e8b0: 4137 5943 7552 524c 4648 5644 536f 5371  A7YCuRRLFHVDSoSq
+0003e8c0: 6a6f 4d39 6765 3442 4456 5154 396c 4777  joM9ge4BDVQT9lGw
+0003e8d0: 4747 345a 6d56 5335 4532 7762 4349 474c  GG4ZmVS5E2wbCIGL
+0003e8e0: 6846 696d 456d 3444 314e 6732 6766 5948  hFimEm4D1Ng2gfYH
+0003e8f0: 3579 4534 3155 7043 554e 4c61 424e 5053  5yE41UpCUNLaBNPS
+0003e900: 6476 4c44 752b 6261 7672 366b 5664 356f  dvLDu+bavr6kVd5o
+0003e910: 7766 2b53 4472 7146 6474 6f6d 324b 6768  wf+SDrqFdtom2Kgh
+0003e920: 5170 3045 746b 4448 6141 6a49 504b 5164  Qp0EtkDHaAjIPKQd
+0003e930: 4176 4d35 5536 6f53 715a 6654 6c67 7556  AvM5U6oSqZfTlguV
+0003e940: 412f 4955 5a32 5756 6e55 4266 4655 6875  A/IUZ2WVnUBfFUhu
+0003e950: 6862 6a64 5656 4638 5570 4574 7850 4549  hbjdVVF8UpEtxPEI
+0003e960: 4341 4b48 715a 6576 5a6c 7651 7a2f 6f57  CAKHqZevZlvQz/oW
+0003e970: 5573 4e61 474e 4431 7461 3654 7435 394b  UsNaGND1ta6Tt59K
+0003e980: 6447 5350 7872 3637 5431 774e 4e54 3163  dGSPxr67T1wNNT1c
+0003e990: 3868 5252 4151 7479 455a 5249 3148 5669  8hRRAQtyEZRI1HVi
+0003e9a0: 6f6b 6e6e 4548 6567 6276 3870 4844 6474  oknnEHegbv8pHDdt
+0003e9b0: 472f 4c63 5350 7263 6469 4277 772f 6f6c  G/LcSPrcdiBww/ol
+0003e9c0: 7a41 636f 5337 716b 7a63 704d 2b78 4343  zAcoS7qkzcpM+xCC
+0003e9d0: 5764 6c54 6e4f 4536 6951 4e70 3943 4777  WdlTnOE6iQNp9CGw
+0003e9e0: 4745 5663 4a69 4756 3261 4968 6664 6249  GEVcJiGV2aIhfdbI
+0003e9f0: 6855 7876 3041 504f 686d 4630 4c74 7065  hUxv0APOhmF0Ltpe
+0003ea00: 475a 524c 6367 4577 504b 6850 684b 4862  GZRLcgEwPKhPhKHb
+0003ea10: 784b 4763 6544 324c 4f4d 3144 4447 7776  xKGceD2LOM1DDGwv
+0003ea20: 7551 3138 4745 6250 5a7a 4371 314b 574c  uQ18GEbPZzCq1KWL
+0003ea30: 6342 7a57 4a34 4e6e 6b4f 6b55 6e37 4c74  cBzWJ4NnkOkUn7Lt
+0003ea40: 454d 5061 7a6e 6e69 4874 6c62 6671 7763  EMPaznniHtlbfqwc
+0003ea50: 4b34 5246 4155 6f49 5565 414d 7554 4145  K4RFAUoIUeAMuTAE
+0003ea60: 355a 6b73 3647 647a 6b70 7735 3265 7071  5Zks6Gdzkpw52epq
+0003ea70: 716f 4748 4559 4a47 4534 684f 5367 662b  qoGHEYJGE4hOSgf+
+0003ea80: 4245 7a74 454b 696c 4a4b 6c55 6c45 7842  BEztEKilJKlUlExB
+0003ea90: 436b 4654 7479 3968 6d61 4f52 4d47 4639  CkFTty9hmaORMGF9
+0003eaa0: 657a 4a48 4c38 6165 7078 594b 5276 7933  ezJHL8aepxYKRvy3
+0003eab0: 3255 4637 7a52 7735 6e50 516f 394d 4b35  2UF7zRw5nPQo9MK5
+0003eac0: 716a 6838 564a 4245 4363 5253 6163 6357  qjh8VJBECcRSaccW
+0003ead0: 734a 4264 5753 2f6e 6c39 794c 7a37 2b64  sJBdWS/nl9yLz7+d
+0003eae0: 752f 636f 2f61 5550 6173 3454 654a 7845  u/co/aUPas4TeJxE
+0003eaf0: 6873 5a64 6946 6873 4f38 5a62 344a 6567  hsZdiFhsO8Zb4Jeg
+0003eb00: 3156 584a 336b 7143 5364 7961 455a 366a  1VXJ3kqCSdyaEZ6j
+0003eb10: 6b38 6a47 465a 4651 4b39 5a41 4441 584c  k8jGFZFQK9ZADAXL
+0003eb20: 4371 7a55 5949 5942 456f 7668 5345 6e48  CqzUYIYBEovhSEnH
+0003eb30: 6a43 6f6a 6d51 4f6b 4b4d 326e 6543 3151  jCojmQOkKM2neC1Q
+0003eb40: 4643 6f41 6330 3173 4a37 3452 354e 7772  FCoAc01sJ74R5Nwr
+0003eb50: 4463 4d70 3942 6253 4e64 6a48 6b7a 4359  DcMp9BbSNdjHkzCY
+0003eb60: 534b 6532 324e 556e 3358 662f 7449 5043  SKe22NUn3Xf/tIPC
+0003eb70: 794d 482f 416a 4769 2f33 444b 6b54 4b42  yMH/AjGi/3DKkTKB
+0003eb80: 5633 5a67 6941 556b 5777 5567 646b 6956  V3ZgiAUkWwUgdkiV
+0003eb90: 4f34 3257 3742 6a4d 306e 3761 6551 464a  O42W7BjM0n7aeQFJ
+0003eba0: 7048 4869 4a41 6a43 6b57 6536 4643 7263  pHHiJAjCkWe6FCrc
+0003ebb0: 6c47 7842 4347 414a 796b 466b 7154 617a  lGxBCGAJykFkqTaz
+0003ebc0: 6e6a 4a67 7675 3831 644a 7941 7644 6a76  njJgvu81dJyAvDjv
+0003ebd0: 2b48 6746 5873 5463 7844 3130 6579 4948  +HgFXsTcxD10eyIH
+0003ebe0: 416f 6738 5a64 772b 7272 3737 3378 4e34  Aog8Zdw+rr773xN4
+0003ebf0: 6171 7666 4539 7350 7942 4439 7751 6977  aqvfE9sPyBD9wQiw
+0003ec00: 7937 7366 4854 4847 5638 3071 7338 6b2f  y7sfHTHGV80qs8k/
+0003ec10: 4851 532f 3365 6732 6f67 462f 524d 3969  HQS/3eg2ogF/RM9i
+0003ec20: 426c 376c 5941 6d32 396a 5575 6c79 316b  Bl7lYAm29jUuly1k
+0003ec30: 6972 5853 4b56 5371 434d 612b 4361 674a  irXSKVSqCMa+CagJ
+0003ec40: 6763 436e 3146 5769 736f 6c38 436f 5a31  gcCn1FWisol8CoZ1
+0003ec50: 4d64 4c4a 7048 4451 6e6b 4e64 5538 4476  MdLJpHDQnkNdU8Dv
+0003ec60: 4157 5141 785a 7575 3335 5655 6a52 504f  AWQAxZuu35VUjRPO
+0003ec70: 3352 5338 2f46 3733 7946 7171 3436 4347  3RS8/F73yFqq46CG
+0003ec80: 6b4e 7953 626b 4930 434d 7842 5730 6f53  kNySbkI0CMxBW0oS
+0003ec90: 6c47 6537 5650 7735 6c4d 534e 6661 506e  lGe7VPw5lMSNfaPn
+0003eca0: 5a71 7135 7342 4441 446c 5145 694c 6b4d  Zqq5sBDADlQEiLkM
+0003ecb0: 4635 4432 486d 4f69 327a 4374 3630 7247  F5D2HmOi2zCt60rG
+0003ecc0: 3931 4c6b 4646 7773 7255 5351 534e 4664  91LkFFwsrUSQSNFd
+0003ecd0: 5150 304a 4f59 7973 4630 4838 784a 5955  QP0JOYysF0H8xJYU
+0003ece0: 4565 694a 4378 6e74 567a 6538 6e31 6538  EeiJCxntVze8n1e8
+0003ecf0: 4c39 4b33 6751 506f 446b 302b 7141 4835  L9K3gQPoDk0+qAH5
+0003ed00: 4343 556b 4b4e 4967 4465 4261 5462 7256  CCUkKNIgDeBaTbrV
+0003ed10: 5473 702f 3930 7076 7932 6350 336c 664b  Tsp/90pvy2cP3lfK
+0003ed20: 356d 6752 3733 5656 522f 774a 756d 4d78  5mgR73VVR/wJumMx
+0003ed30: 6575 7245 6a54 3049 624c 676d 5273 3643  eurEjT0IbLgmRs6C
+0003ed40: 6e5a 5733 5745 5232 4b47 6a6e 5470 4570  nZW3WER2KGjnTpEp
+0003ed50: 4879 5461 6c52 5454 7855 684e 626f 4e39  HyTalRTTxUhNboN9
+0003ed60: 4271 3471 4167 4e71 3244 6f42 3357 4442  Bq4qAgNq2DoB3WDB
+0003ed70: 636b 4c5a 3274 4c31 4654 6267 6b4f 644a  ckLZ2tL1FTbgkOdJ
+0003ed80: 5635 3473 4630 6f6a 5a62 4362 7476 3358  V54sF0ojZbCbtv3X
+0003ed90: 4866 7863 5438 6f6a 4f78 2f4c 5869 652f  HfxcT8ojOx/LXie/
+0003eda0: 7251 4e32 464b 6b4b 4956 3275 736d 4549  rQN2FKkKIV2usmEI
+0003edb0: 714a 4c32 5161 3175 7858 3877 2b53 554c  qJL2Qa1uxX8w+SUL
+0003edc0: 3936 302f 4a51 5562 586c 3137 4f6f 704c  960/JQUbXl17OopL
+0003edd0: 4176 7948 4541 4d48 6430 6d55 4245 6542  AvyHEAMHd0mUBEeB
+0003ede0: 496c 526a 6879 4952 6c6d 5175 4269 5349  IlRjhyIRlmQuBiSI
+0003edf0: 4252 5261 6953 5370 4c61 3270 3576 3033  BRRaiSSpLa2p5v03
+0003ee00: 4365 7374 7578 6b35 6b75 3843 3939 714f  Cestuxk5ku8C99qO
+0003ee10: 6873 6456 414f 7752 574c 3659 494e 4e53  hsdVAOwRWL6YINNS
+0003ee20: 354e 4968 456f 6c42 6e74 376a 626d 3637  5NIhEolBnt7jbm67
+0003ee30: 5a71 7a4c 2f50 3247 7457 6256 6163 5937  ZqzL/P2GtWbVacY7
+0003ee40: 316e 6e73 4577 4365 7156 4470 4947 4a50  1nnsEwCeqVDpIGJP
+0003ee50: 6e52 4c6d 4c54 4443 4133 484e 4146 5231  nRLmLTDCA3HNAFR1
+0003ee60: 4430 3651 696c 4a64 4c57 4373 6f49 3642  D06QilJdLWCsoI6B
+0003ee70: 516b 4933 4578 3763 6f41 774a 4352 7934  QkI3Ex7coAwJCRy4
+0003ee80: 4a41 4f41 4752 4144 7766 6a50 7052 566a  JAOAGRADwfjPpRVj
+0003ee90: 7652 3756 5474 6564 5a70 4a42 3639 5131  vR7VTtedZpJB69Q1
+0003eea0: 6643 5773 7736 6631 484c 5366 6e65 4c2b  fCWsw6f1HLSfneL+
+0003eeb0: 7378 6b32 4b67 3633 6b47 3551 5244 6f37  sxk2Kg63kG5QRDo7
+0003eec0: 6577 4530 4655 5543 3330 6657 4467 3177  ewE0FUUC30fWDg1w
+0003eed0: 6579 6653 7068 7273 506f 3653 6f68 6570  eyfSphrsPo6Sohep
+0003eee0: 5370 6139 4842 7157 786c 536c 6149 6943  Spa9HBqWxlSlaIiC
+0003eef0: 4f4c 682f 3836 4852 5565 5a41 3454 4152  OLh/86HRUeZA4TAR
+0003ef00: 5563 4a53 4249 6163 7347 4346 7766 5873  UcJSBIacsGCFwfXs
+0003ef10: 6a57 7355 5873 554a 4572 5373 6873 7a61  jWsUXsUJErSshsza
+0003ef20: 2f4a 5832 4b34 3742 5937 2f70 3968 3767  /JX2K47BY7/p9h7g
+0003ef30: 6d4e 734f 6941 4a43 4c52 555a 684e 4856  mNsOiAJCLRUZhNHV
+0003ef40: 5373 676f 524d 3672 472f 644d 6536 3077  SsgoRM6rG/dMe60w
+0003ef50: 3239 3154 7a74 6b48 7866 5030 486a 486d  291TztkHxfP0HjHm
+0003ef60: 6673 656e 714b 6830 304c 5539 7458 4933  fsenqKh00LU9tXI3
+0003ef70: 3864 5a50 6432 4d6f 2f55 4e53 6444 446f  8dZPd2Mo/UNSdDDo
+0003ef80: 4431 4b46 464d 476c 6b38 6954 454a 6432  D1KFFMGlk8iTEJd2
+0003ef90: 5368 4736 3674 686d 7a35 4d4e 6d78 4c50  ShG66thmz5MNmxLP
+0003efa0: 5834 4f55 3479 4567 4f45 587a 4557 6742  X4OU4yEgOEXzEWgB
+0003efb0: 7342 624f 4c39 414c 6243 4b34 4656 3631  sBbOL9ALbCK4FV61
+0003efc0: 4e6a 652b 4646 3947 6938 3835 7366 3555  Nje+FF9Gi885sf5U
+0003efd0: 594f 7559 5259 5078 3672 5238 6b78 4275  YOuYRYPx6rR8kxBu
+0003efe0: 7443 7737 4249 3753 506a 4269 5966 6459  tCw7BI7SPjBiYfdY
+0003eff0: 766e 4f53 616d 552f 5171 6c41 3678 7139  vnOSamU/QqlA6xq9
+0003f000: 546b 4259 514d 4a79 6935 714f 4755 5757  TkBYQMJyi5qOGUWW
+0003f010: 6d6b 6251 7263 535a 4444 5046 4245 4439  mkbQrcSZDDPFBED9
+0003f020: 6279 6473 664a 324e 5333 6f56 5770 416d  bydsfJ2NS3oVWpAm
+0003f030: 7356 346d 766f 2b41 3269 7054 7452 5965  sV4mvo+A2ipTtRYe
+0003f040: 5669 3833 7542 3965 7652 6766 6f2b 3035  Vi83uB9evRgfo+05
+0003f050: 7a53 3176 635a 6263 3864 4458 3730 4c44  zS1vcZbc8dDX70LD
+0003f060: 6d6a 6564 4167 6c31 4a45 3242 7a32 4d6f  mjedAgl1JE2Bz2Mo
+0003f070: 3172 5359 5855 537a 4533 3675 5875 4e2b  1rSYXUSzE36uXuN+
+0003f080: 5748 686d 354d 766b 6a73 4d71 6b4d 5049  WHhm5MvkjsMqkMPI
+0003f090: 6a77 5962 6e45 6269 514a 3955 7033 426f  jwYbnEbiQJ9Up3Bo
+0003f0a0: 6576 5353 3056 3078 5173 374e 5a49 6b4f  evSS0V0xQs7NZIkO
+0003f0b0: 7579 4343 5933 6149 6b4b 5848 3651 4367  uyCCY3aIkKXH6QCg
+0003f0c0: 7649 7052 7353 414e 5942 2b59 4d48 7657  vIpRsSANYB+YMHvW
+0003f0d0: 446b 4f45 4933 2b54 6145 512b 486b 6548  DkOEI3+TaEQ+HkeH
+0003f0e0: 474c 6835 576b 676a 4955 5463 6966 6c34  GLh5WkgjIUTcifl4
+0003f0f0: 5930 2f6b 556d 4b31 754d 6d48 4e35 3833  Y0/kUmK1uMmHN583
+0003f100: 4635 3369 4a72 3052 446a 4334 5a31 3476  F53iJr0RDjC4Z14v
+0003f110: 572b 7148 4632 514c 6c51 4c45 3452 3254  W+qHF2QLlQLE4R2T
+0003f120: 4a4c 7951 2b67 6f5a 7a6c 322b 7670 6b54  JLyQ+goZzl2+vpkT
+0003f130: 5849 6465 6f50 5159 3253 4a43 4b68 6266  XIdeoPQY2SJCKhbf
+0003f140: 756d 5671 6649 6657 7048 5a4a 4d63 467a  umVqfIfWpHZJMcFz
+0003f150: 6e62 6155 726e 6f56 6f4c 6b46 3632 456f  nbaUrnoVoLkF62Eo
+0003f160: 397a 6137 7178 5336 6c45 5169 5a61 3142  9za7qxS6lEQiZa1B
+0003f170: 6678 335a 7261 4159 5458 4134 7931 4143  fx3ZraAYTXA4y1AC
+0003f180: 6b6f 4b59 4e56 5753 565a 667a 394b 4a35  koKYNVWSVZfz9KJ5
+0003f190: 6856 5757 2b4d 5075 4376 5067 6f4d 376d  hVWW+MPuCvPgoM7m
+0003f1a0: 3777 4a48 6e46 616b 7736 3651 6942 3142  7wJHnFakw66QiB1B
+0003f1b0: 7a48 512b 5254 416d 3167 7349 5876 5648  zHQ+RTAm1gsIXvVH
+0003f1c0: 5a45 3762 6549 7437 6e46 3737 6335 3631  ZE7beIt7nF77c561
+0003f1d0: 4f4c 456d 3134 6534 6e44 5752 704c 6757  OLEm14e4nDWRpLgW
+0003f1e0: 3366 3437 6753 5242 4b7a 6d37 4538 654a  3f47gSRBKzm7E8eJ
+0003f1f0: 7075 4830 7964 7a7a 5361 4438 694f 4773  puH0ydzzSaD8iOGs
+0003f200: 4567 6370 5947 6c34 4873 346f 7345 4e67  EgcpYGl4Hs4osENg
+0003f210: 4276 4371 3366 6748 656a 6450 3370 2b69  BvCq3fgHejdP3p+i
+0003f220: 714f 6e77 4a64 6575 4f50 4b42 4f78 7067  qOnwJdeuOPKBOxpg
+0003f230: 6e6e 3573 5550 364e 4a39 3234 4258 6530  nn5sUP6NJ924BXe0
+0003f240: 4c36 5830 3931 7733 4b41 7053 7865 7169  L6X091w3KApSxeqi
+0003f250: 7442 4746 5448 4342 4b46 6473 6959 4937  tBGFTHCBKFdsiYI7
+0003f260: 3741 5436 5338 6c30 356e 6e30 5346 6769  7AT6S8l05nn0SFgi
+0003f270: 7645 6169 4367 3530 734c 7871 6f61 4a46  vEaiCg50sLxqoaJF
+0003f280: 6b72 6f42 4752 4c74 7432 7872 7a52 304b  kroBGRLtt2xrzR0K
+0003f290: 3046 5332 2f57 6a68 6935 4845 6753 5377  0FS2/Wjhi5HEgSSw
+0003f2a0: 4377 7076 352b 634e 666a 3474 7377 486d  Cwpv5+cNfj4tswHm
+0003f2b0: 6261 5533 796f 6343 584d 5158 4742 7567  baU3yocCXMQXGBug
+0003f2c0: 6776 6d46 3561 2b4b 744a 6a4f 4574 6b65  gvmF5a+KtJjOEtke
+0003f2d0: 6f6d 6b33 664b 307a 4872 4877 336e 346a  omk3fK0zHrHw3n4j
+0003f2e0: 3343 3831 5674 7235 7441 476e 5352 4344  3C81Vtr5tAGnSRCD
+0003f2f0: 7252 5278 4851 616b 3064 6248 4c74 3359  rRRxHQak0dbHLt3Y
+0003f300: 634b 5971 2f49 5848 486d 3548 4937 2f75  cKYq/IXHHm5HI7/u
+0003f310: 4250 6d49 3942 5263 6469 4431 3442 6849  BPmI9BRcdiD14BhI
+0003f320: 6b2b 5867 6647 4461 3351 2f4a 6538 5652  k+XgfGDa3Q/Je8VR
+0003f330: 484e 6254 7541 446b 6d71 4c6b 5732 5779  HNbTuADkmqLkW2Wy
+0003f340: 6942 416d 2b51 7472 546d 6538 3349 5764  iBAm+QtrTme83IWd
+0003f350: 4430 6b49 6842 536c 5a47 4537 646f 5168  D0kIhBSlZGE7doQh
+0003f360: 2b59 4267 7267 326b 4d53 7272 6d5a 7452  +YBgrg2kMSrrmZtR
+0003f370: 2b77 2b73 6532 5158 5734 5274 5a6e 4469  +w+se2QXW4RtZnDi
+0003f380: 644b 344c 6230 3555 7761 4670 6a79 4331  dK4Lb05UwaFpjyC1
+0003f390: 6c55 4371 5671 482b 724f 504f 4c4e 5064  lUCqVqH+rOPOLNPd
+0003f3a0: 704c 574e 5935 6a42 6136 6748 446d 6374  pLWNY5jBa6gHDmct
+0003f3b0: 4332 4148 4b31 7a6a 2f6c 3238 3977 6c61  C2AHK1zj/l289wla
+0003f3c0: 3333 7035 4c6c 6177 6e6b 4865 6777 3474  33p5LlawnkHegw4t
+0003f3d0: 316d 3461 4e4d 3267 5736 7437 507a 356a  1m4aNM2gW6t7Pz5j
+0003f3e0: 4356 4653 7541 4363 3071 6356 394b 6955  CVFSuACc0qcV9KiU
+0003f3f0: 7463 7055 594c 6e4a 3033 7958 756c 7a51  tcpUYLnJ03yXulzQ
+0003f400: 6b76 6648 6d37 4f65 424d 456b 7351 5356  kvfHm7OeBMEksQSV
+0003f410: 644b 7152 5465 2f6a 7335 6f6c 702b 5236  dKqRTe/js5olp+R6
+0003f420: 5853 366f 646f 542f 7755 446f 484e 6854  XS6odoT/wUDoHNhT
+0003f430: 7675 684f 7635 6d74 524a 794b 4558 3345  vuhOv5mtRJyKEX3E
+0003f440: 5971 514a 4975 4f63 3836 534d 4d59 2f71  YqQJIuOc86SMMY/q
+0003f450: 4f33 3051 3336 5250 326e 6666 5555 3645  O30Q36RP2nffUU6E
+0003f460: 5834 5342 3070 457a 384a 6334 5972 4735  X4SB0pEz8Jc4YrG5
+0003f470: 6878 727a 6562 564a 4a70 7545 384a 6d7a  hxrzebVJJpuE8Jmz
+0003f480: 4c62 3178 6f78 5152 744a 5251 4d66 4836  Lb1xoxQRtJRQMfH6
+0003f490: 6266 5073 6f57 4362 4778 7545 7755 6b69  bfPsoWCbGxuEwUki
+0003f4a0: 7651 4565 677a 3868 7a2b 4375 7a43 766f  vQEegz8hz+CuzCvo
+0003f4b0: 4355 5077 3736 576b 2f66 396e 7274 3976  CUPw76Wk/f9nrt9v
+0003f4c0: 2b39 4c32 2b71 6a43 7767 325a 7852 6c44  +9L2+qjCwg2ZxRlD
+0003f4d0: 6f79 4233 7135 734b 5747 7577 5739 4d73  oyB3q5sKWGuwW9Ms
+0003f4e0: 4d52 4a79 5854 7962 6364 4b2b 3069 4b59  MRJyXTybcdK+0iKY
+0003f4f0: 4b36 4251 3672 4973 4d71 4655 6648 435a  K6BQ6rIsMqFUfHCZ
+0003f500: 544f 6235 6b36 2b4a 492b 6544 6d31 5249  TOb5k6+JI+eDm1RI
+0003f510: 456e 5563 4772 6252 4c63 534a 4445 7332  EnUcGrbRLcSJDEs2
+0003f520: 3635 4245 596f 6f34 5657 7264 6f41 4438  65BEYoo4VWrdoAD8
+0003f530: 6267 314f 6639 4737 324e 6133 4c7a 7762  bg1Of9G72Na3Lzwb
+0003f540: 4b48 7575 4374 7655 7132 574f 7258 6773  KHuuCtvUq2WOrXgs
+0003f550: 4d74 3330 6c36 714f 6664 6b4d 7365 4f67  Mt30l6qOfdkMseOg
+0003f560: 4850 3948 6451 4a6f 4463 452f 6355 6f49  HP9HdQJoDcE/cUoI
+0003f570: 4567 7a41 6632 4d45 5531 4b6f 5246 6279  EgzAf2MEU1KoRFby
+0003f580: 686e 6b6a 6476 2b79 7262 7a6a 2f36 4732  hnkjdv+yrbzj/6G2
+0003f590: 4847 376e 6b67 4543 5364 7a71 3757 5174  HG7nkgECSdzq7WQt
+0003f5a0: 5672 6132 6d44 3658 6f44 4245 4a33 3163  Vra2mD6XoDBEJ31c
+0003f5b0: 5636 4343 3630 6462 4573 4665 6f73 556f  V6CC60dbEsFeosUo
+0003f5c0: 6a44 6c34 5277 444c 7930 7a6f 4a76 5631  jDl4RwDLy0zoJvV1
+0003f5d0: 4a70 6c44 546c 7770 5449 7659 6534 4438  JplDTlwpTIvYe4D8
+0003f5e0: 794c 5871 3075 786c 7150 3250 4c44 3173  yLXq0uxlqP2PLD1s
+0003f5f0: 5046 3379 4e6f 4d2f 734d 6166 5639 4472  PF3yNoM/sMafV9Dr
+0003f600: 612b 6764 496f 474f 7773 4939 6f4f 4541  a+gdIoGOwsI9oOEA
+0003f610: 766f 4d79 6436 4765 6378 6b32 7972 3879  voMyd6Gecxk2yr8y
+0003f620: 6b6f 3771 364c 454b 4557 614a 6232 6c50  ko7q6LEKEWaJb2lP
+0003f630: 5a4e 4e71 795a 6433 4d4b 6d50 6c44 7531  ZNNqyZd3MKmPlDu1
+0003f640: 716a 4365 7237 3379 4776 4b62 3775 5355  qjCer73yGvKb7uSU
+0003f650: 4248 7544 6a31 4275 5355 5952 6e56 4546  BHuDj1BuSUYRnVEF
+0003f660: 7568 4537 7738 3871 6a58 544f 3975 4752  uhE7w88qjXTO9uGR
+0003f670: 476d 426f 5a63 7461 6d42 6464 652b 6b41  GmBoZctamBdde+kA
+0003f680: 624b 3075 6930 696d 785a 2b4d 6d4f 4c6a  bK0ui0imxZ+MmOLj
+0003f690: 4633 4932 7174 6266 2b52 342f 7064 6745  F3I2qtbf+R4/pdgE
+0003f6a0: 5045 2b39 5854 5453 3043 456e 5576 4a6f  PE+9XTTS0CEnUvJo
+0003f6b0: 7335 6d4f 6c56 6749 4e69 7964 2b33 6b37  s5mOlVgINiyd+3k7
+0003f6c0: 416e 372f 5449 3765 612f 786c 7574 6e65  An7/TI7ea/xlutne
+0003f6d0: 5336 6267 3831 3634 414c 6f33 676d 5268  S6bg8164ALo3gmRh
+0003f6e0: 4235 5a4b 5371 4970 424a 5273 3035 4444  B5ZKSqIpBJRs05DD
+0003f6f0: 3449 6551 2b44 6a49 6568 5362 5a65 3768  4IeQ+DjIehSbZe7h
+0003f700: 5278 6630 3978 7335 3978 5762 2b54 412b  Rxf09xs59xWb+TA+
+0003f710: 705a 5444 3772 6147 3948 2f4b 6d5a 6276  pZTD7raG9H/KmZbv
+0003f720: 6658 4b74 4771 4969 4d32 5567 6442 7161  fXKtGqIiM2UgdBqa
+0003f730: 4d46 4d73 6847 3677 7256 4f57 7079 595a  MFMshG6wrVOWpyYZ
+0003f740: 4f77 444f 316b 6e38 4b59 6539 3951 3970  OwDO1kn8KYe99Q9p
+0003f750: 3361 6f59 396c 3568 312f 5178 5062 3865  3aoY9l5h1/QxPb8e
+0003f760: 746d 7672 4842 6156 792b 5a63 4d45 7262  tmvrHBaVy+ZcMErb
+0003f770: 6268 5148 4e4c 6968 7855 3345 7559 7146  bhQHNLihxU3EuYqF
+0003f780: 5334 594e 3053 6878 5058 6765 5437 4a65  S4YN0ShxPXgeT7Je
+0003f790: 332f 416b 5732 356c 6759 5848 3533 585a  3/AkW25lgYXH53XZ
+0003f7a0: 6d62 6833 4554 666a 572b 7371 354b 3456  mbh3ETfjW+sq5K4V
+0003f7b0: 5064 4d65 6a56 6376 474d 5857 6b2b 4572  PdMejVcvGMXWk+Er
+0003f7c0: 6e73 7a64 4f61 4336 6b67 5541 434c 5349  nszdOaC6kgUACLSI
+0003f7d0: 4343 4843 5642 7147 3072 4836 7550 7450  CCHCVBqG0rH6uPtP
+0003f7e0: 754a 4872 6438 3536 544a 7668 7947 3164  uJHrd856TJvhyG1d
+0003f7f0: 4364 6253 4872 5567 2b35 506f 4350 425a  CdbSHrUg+5PoCPBZ
+0003f800: 3030 7772 3936 4946 676f 6d59 754b 6730  00wr96IFgomYuKg0
+0003f810: 5231 785a 6e73 7576 6176 6875 6441 5458  R1xZnsuvavhudATX
+0003f820: 5743 3474 3237 4b41 5965 3148 7248 724c  WC4t27KAYe1HrHrL
+0003f830: 534b 5432 6839 4f45 4935 5a54 3630 6132  SKT2h9OEI5ZT60a2
+0003f840: 595a 5254 5279 6844 6145 6441 7348 656c  YZRTRyhDaEdAsHel
+0003f850: 7479 6136 6c54 582f 735a 6956 6131 346b  tya6lTX/sZiVa14k
+0003f860: 594f 3842 6b6a 7070 4971 4752 766c 5571  YO8BkjppIqGRvlUq
+0003f870: 6a41 7931 6453 3065 502f 4c73 2b6a 4674  jAy1dS0eP/Ls+jFt
+0003f880: 626b 7338 4f61 6856 6b6d 504c 7471 4d7a  bks8OahVkmPLtqMz
+0003f890: 3652 5750 4371 4749 4959 5542 7445 346b  6RWPCqGIIYUBtE4k
+0003f8a0: 6d53 4a57 3334 3446 6741 4f32 494c 747a  mSJW344FgAO2ILtz
+0003f8b0: 386b 4e37 724f 304c 6566 6166 7654 635a  8kN7rO0LefafvTcZ
+0003f8c0: 4f75 4848 6846 4945 7053 3154 6d70 744a  OuHHhFIEpS1TmptJ
+0003f8d0: 7576 2b31 4337 496b 2b42 732f 3137 5159  uv+1C7Ik+Bs/17QY
+0003f8e0: 5852 4f45 7a55 4770 5a70 4562 644e 5254  XROEzUGpZpEbdNRT
+0003f8f0: 4952 7063 564c 3071 6a32 3639 5776 482f  IRpcVL0qj269WvH/
+0003f900: 4335 3735 7353 392f 4e71 4d51 432b 417a  C575sS9/NqMQC+Az
+0003f910: 3358 5265 7963 7767 6465 3569 3765 744a  3XReycwgde5i7etJ
+0003f920: 516d 434d 7144 5877 4163 4c62 6364 7842  QmCMqDXwAcLbcdxB
+0003f930: 617a 7637 624e 5433 2b5a 766e 3343 3174  azv7bNT3+Zvn3C1t
+0003f940: 3332 2f48 7a48 4848 6d7a 5730 3739 4156  32/HzHHHmzW079AV
+0003f950: 3271 3737 576b 5249 5963 556a 6444 4174  2q77WkRIYcUjdDAt
+0003f960: 3067 6e63 577a 4734 6d2f 536e 4b32 4434  0gncWzG4m/SnK2D4
+0003f970: 5a51 4473 3732 467a 5734 6244 7165 656e  ZQDs72FzW4bDqeen
+0003f980: 3354 7442 7438 414c 434a 424f 6343 7743  3TtBt8ALCJBOcCwC
+0003f990: 7938 5463 377a 7157 4f47 6f43 494c 6b37  y8Tc7zqWOGoCILk7
+0003f9a0: 5878 5144 3770 3871 3446 3273 7778 4f5a  XxQD7p8q4F2swxOZ
+0003f9b0: 496f 4931 4245 6534 4650 3939 7763 6331  IoI1BEe4FP99wcc1
+0003f9c0: 5a62 7333 5a4b 7a38 6559 694d 4d56 7677  Zbs3ZKz8eYiMMVvw
+0003f9d0: 456c 6962 315a 7670 3368 3171 3264 354d  Elib1Zvp3h1q2d5M
+0003f9e0: 4d48 4568 5334 4a65 2b36 7247 5748 6a32  MHEhS4Je+6rGWHj2
+0003f9f0: 3473 2f68 2b35 4449 3262 7152 6e54 6f6a  4s/h+5DI2bqRnToj
+0003fa00: 4552 564b 3058 6b4d 4f6c 4b6b 7570 592f  ERVK0XkMOlKkupY/
+0003fa10: 6430 4a6f 3337 6165 7357 4a50 3344 4844  d0Jo37aesWJP3DHD
+0003fa20: 3638 5845 755a 4951 4253 5949 7441 7a77  68XEuZIQBSYItAzw
+0003fa30: 4f57 3262 614c 4768 7464 324a 5467 4e6d  OW2baLGhtd2JTgNm
+0003fa40: 4c63 5576 4e70 6131 6e4c 4f59 5965 3048  LcUvNpa1nLOYYe0H
+0003fa50: 7266 6e33 5835 3939 5751 5966 7445 6277  rfn3X599WQYftEbw
+0003fa60: 6d48 6555 4663 4946 4643 3154 6b4b 5441  mHeUFcIFFC1TkKTA
+0003fa70: 2b63 6154 4c77 4446 5433 6159 716e 7255  +caTLwDFT3aYqnrU
+0003fa80: 6f35 646f 5073 615a 6369 4251 7979 3377  o5doPsaZciBQyy3w
+0003fa90: 6337 5463 416f 6e34 5a33 4271 7032 4437  c7TcAon4Z3Bqp2D7
+0003faa0: 5551 3952 7651 6d6f 626d 4873 6932 6757  UQ9RvQmobmHsi2gW
+0003fab0: 776e 694c 7341 6268 5330 774b 4530 456c  wniLsAbhS0wKE0El
+0003fac0: 3350 5262 7654 6f48 4751 2b72 6446 4a77  3PRbvToHGQ+rdFJw
+0003fad0: 4268 2b44 7039 6173 4663 5536 4b44 5732  Bh+Dp9asFcU6KDW2
+0003fae0: 7930 6346 3954 4e35 4231 314f 6d76 4352  y0cF9TN5B11OmvCR
+0003faf0: 4e48 4b35 3170 5348 7238 5268 6b56 6e53  NHK51pSHr8RhkVnS
+0003fb00: 695a 6d6d 7736 6c4a 5059 7a6f 3268 526c  iZmmw6lJPYzo2hRl
+0003fb10: 4b36 4d53 6c55 3674 3368 4339 4b67 3950  K6MSlU6t3hC9Kg9P
+0003fb20: 4866 4770 4674 627a 7a6e 7951 476e 6251  HfGpFtbzznyQGnbQ
+0003fb30: 4241 4751 3662 6964 5242 6c79 596a 7a46  BAGQ6bidRBlyYjzF
+0003fb40: 5366 6874 6f30 6256 7466 3872 614e 2b34  Sfhto0bVtf8raN+4
+0003fb50: 6f38 5a39 4a50 6f58 4d4e 4171 5647 6230  o8Z9JPoXMNAqVGb0
+0003fb60: 696c 6156 4764 4644 7469 504c 457a 2b72  ilaVGdFDtiPLEz+r
+0003fb70: 2b65 7031 4d6e 4a56 4f4a 544f 4565 4963  +ep1MnJVOJTOEeIc
+0003fb80: 684e 7863 3655 7156 2f44 635a 6364 2f76  hNxc6UqV/DcZcd/v
+0003fb90: 5731 4477 366e 4f59 494e 6570 554c 5276  W1Dw6nOYINepULRv
+0003fba0: 5235 6b4f 4277 4d49 4165 714b 4d76 706d  R5kOBwMIAeqKMvpm
+0003fbb0: 3454 7030 3631 3946 3936 6679 5752 5978  4Tp0619F96fyWRYx
+0003fbc0: 6843 6a46 4959 6b43 4352 4a49 754f 496d  hCjFIYkCCRJIuOIm
+0003fbd0: 6b54 7968 5653 6250 414b 3677 322b 6852  kTyhVSbPAK6w2+hR
+0003fbe0: 3947 5856 5972 4a59 5659 4247 6179 4e65  9GXVYrJYVYBGayNe
+0003fbf0: 5367 6b6e 5744 5568 4c32 6476 3876 7761  SgknWDUhL2dv8vwa
+0003fc00: 3571 2b39 2b56 762b 5431 7269 6d38 626d  5q+9+Vv+T1rim8bm
+0003fc10: 3356 4d58 6931 5665 6478 704f 5876 5377  3VMXi1VedxpOXvSw
+0003fc20: 5731 5444 3771 5831 6151 5042 592b 6950  W1TD7qX1aQPBY+iP
+0003fc30: 7535 7438 6f4a 6971 6858 6141 435a 4c31  u5t8oJiqhXaACZL1
+0003fc40: 4162 5130 6263 7479 7a6b 326b 557a 646c  AbQ0bctyzk2kUzdl
+0003fc50: 4a44 346c 682f 7364 786d 7667 6354 514b  JD4lh/sdxmvgcTQK
+0003fc60: 6f4e 3871 6434 7633 5667 3763 6562 3054  oN8qd4v3Vg7ceb0T
+0003fc70: 7230 582f 336e 4570 6e66 434c 7341 774f  r0X/3nEpnfCLsAwO
+0003fc80: 544e 6431 3967 612f 5075 3139 6147 3671  TNd19ga/Pu19aG6q
+0003fc90: 5458 3332 7442 5439 6565 414f 6744 3070  TX32tBT9eeAOgD0p
+0003fca0: 416e 734c 6164 787a 6370 4d64 584d 3462  AnsLadxzcpMdXM4b
+0003fcb0: 4450 416a 304a 6f6c 5458 3634 5255 616f  DPAj0JolTX64RUao
+0003fcc0: 522b 3739 7547 5557 7465 5335 586d 594f  R+79uGUWteS5XmYO
+0003fcd0: 5868 4a66 3579 7772 5a75 674a 3436 485a  XhJf5ywrZugJ46HZ
+0003fce0: 6f4a 306c 5a30 3663 4c43 6d36 6167 5247  oJ0lZ06cLCm6agRG
+0003fcf0: 7869 554b 6367 4542 6341 7352 346f 4335  xiUKcgEBcAsR4oC5
+0003fd00: 3159 717a 4276 7435 456f 4a79 5368 3965  1YqzBvt5EoJySh9e
+0003fd10: 6b77 4648 784f 6837 4252 6f74 462b 5041  kwFHxOh7BRotF+PA
+0003fd20: 4472 4677 6f41 456c 4e77 674f 6238 396b  DrFwoAElNwgOb89k
+0003fd30: 6642 2f7a 3279 377a 616f 7550 704f 6256  fB/z2y7zaouPpObV
+0003fd40: 3244 526d 3570 3747 3658 414e 4659 334a  2DRm5p7G6XANFY3J
+0003fd50: 4c74 3476 366d 3544 5871 5447 5450 7349  Lt4v6m5DXqTGTPsI
+0003fd60: 5857 4c31 764e 4d62 3468 737a 6e50 586e  XWL1vNMb4hsznPXn
+0003fd70: 486a 6c65 6934 4564 7a2b 3631 3450 4d6e  Hjlei4Edz+614PMn
+0003fd80: 3838 7336 5570 6374 4958 6957 7430 3453  88s6UpctIXiWt04S
+0003fd90: 476d 4e57 2f35 456c 5464 2f55 5457 5341  GmNW/5ElTd/UTWSA
+0003fda0: 386c 5175 7569 6342 4a79 5061 4a56 5a65  8lQuuicBJyPaJVZe
+0003fdb0: 754a 7551 3064 6f78 6376 424c 4f6e 5646  uJuQ0doxcvBLOnVF
+0003fdc0: 6a4a 764a 2f4f 464c 3850 552b 7065 7763  jJvJ/OFL8PU+pewc
+0003fdd0: 5a68 6f59 7848 5254 5a69 4f69 676c 6b77  ZhoYxHRTZiOiglkw
+0003fde0: 4178 4b6a 655a 4447 3077 6d4f 6953 4858  AxKjeZDG0wmOiSHX
+0003fdf0: 6c6d 7661 5742 3352 4935 414c 7931 4471  lmvaWB3RI5ALy1Dq
+0003fe00: 3045 4745 764a 3949 4d57 7064 7233 384e  0EGEvJ9IMWpdr38N
+0003fe10: 5a4b 4473 566f 6952 4853 6876 4943 4f79  ZKDsVoiRHShvICOy
+0003fe20: 4948 414e 4e47 3673 6d72 4530 7a66 5773  IHANNG6smrE0zfWs
+0003fe30: 6266 7537 4b49 766b 5451 786d 597a 6642  bfu7KIvkTQxmYzfB
+0003fe40: 2b6b 306f 6b51 704a 5177 7579 337a 3157  +k0okQpJQwuy3z1W
+0003fe50: 456f 3753 4d6c 4866 6670 6f61 7538 316a  Eo7SMlHffpoau81j
+0003fe60: 3955 6b32 6871 6455 694a 3046 6f59 6b69  9Uk2hqdUiJ0FoYki
+0003fe70: 4f62 6167 7351 6c49 326f 6236 6872 6b39  ObagsQlI2ob6hrk9
+0003fe80: 637a 3354 7746 7976 452b 4a6c 4d74 3063  cz3TwFyvE+JlMt0c
+0003fe90: 416a 4d57 7161 546d 6a69 6979 4161 4254  AjMWqaTmjiiyAaBT
+0003fea0: 6c50 7249 6b4a 624b 4530 6d2f 426b 6a67  lPrIkJbKE0m/Bkjg
+0003feb0: 677a 6145 7247 624d 6844 4275 7249 5a74  gzaErGbMhDBurIZt
+0003fec0: 462f 376a 6a6a 6172 6e4c 6534 5468 5a4c  F/7jjjarnLe4ThZL
+0003fed0: 7645 636d 3449 6371 3359 474e 6179 7036  vEcm4Icq3YGNayp6
+0003fee0: 7a74 7a65 6732 624d 5957 654d 3934 3046  ztzeg2bMYWeM940F
+0003fef0: 5032 4c2b 4970 4778 5241 6b43 7079 5534  P2L+IpGxRAkCpyU4
+0003ff00: 2b4d 6e55 614b 5577 3051 3530 396e 3773  +MnUaKUw0Q509n7s
+0003ff10: 372f 5556 6966 7947 622b 7868 5466 364e  7/UVifyGb+xhTf6N
+0003ff20: 524b 587a 7041 4562 7949 4b38 434c 5242  RKXzpAEbyIK8CLRB
+0003ff30: 562f 724e 5173 4f74 3962 3167 454d 354f  V/rNQsOt9b1gEM5O
+0003ff40: 434e 7270 6656 434b 7373 6e77 3744 6e52  CNrpfVCKssnw7DnR
+0003ff50: 706a 454e 3674 2b43 4945 704a 6470 4a6a  pjEN6t+CIEpJdpJj
+0003ff60: 575a 734a 676a 4d57 696c 6e43 3949 7779  WZsJgjMWilnC9Iwy
+0003ff70: 6468 306f 4836 4272 7452 3235 4d42 7256  dh0oH6BrtR25MBrV
+0003ff80: 4739 4b32 7a71 534a 3533 726b 7233 7143  G9K2zqSJ53rkr3qC
+0003ff90: 7877 7670 336f 7047 6655 5747 774e 3870  xwvp3opGfUWGwN8p
+0003ffa0: 6b71 7267 5a37 7755 716d 6841 2f65 6f47  kqrgZ7wUqmhA/eoG
+0003ffb0: 3362 3339 4453 5532 366e 7434 6774 5634  3b39DSU26nt4gtV4
+0003ffc0: 514c 7444 5974 4f71 6d68 304b 3045 5377  QLtDYtOqmh0K0ESw
+0003ffd0: 2f71 5876 5575 7562 6734 3245 4647 3071  /qXvUuubg42EFG0q
+0003ffe0: 5267 7743 5a2b 7735 4d47 7137 4a70 7346  RgwCZ+w5MGq7JpsF
+0003fff0: 6232 7672 6847 3957 6f58 7772 4154 4852  b2vrhG9WoXwrATHR
+00040000: 5563 706a 684c 4a55 5175 3657 6442 6d77  UcpjhLJUQu6WdBmw
+00040010: 5a77 6b61 7573 4235 4b69 7a73 7877 5866  ZwkausB5KizsxwXf
+00040020: 4575 7571 6e65 364e 5a50 3166 3248 3739  Euuqne6NZP1f2H79
+00040030: 4133 6875 6267 4f49 644b 7041 3931 3058  A3hubgOIdKpA910X
+00040040: 424d 5973 3147 6974 6d41 644a 5244 464e  BMYs1GitmAdJRDFN
+00040050: 676a 554c 3943 5657 6b77 4f30 4173 7756  gjUL9CVWkwO0AswV
+00040060: 376f 4269 4847 716e 5848 6d32 6a33 5336  7oBiHGqnXHm2j3S6
+00040070: 7647 506b 704d 3176 6736 4c44 7866 7136  vGPkpM1vg6LDxfq6
+00040080: 4362 4479 306e 4c48 3168 5831 6575 7858  CbDy0nLH1hX1euxX
+00040090: 3965 7954 6b37 6936 626d 7379 414f 4d32  9eyTk7i6bmsyAOM2
+000400a0: 774b 3631 344e 414e 7974 3370 317a 644a  wK614NANyt3p1zdJ
+000400b0: 4e54 2f2f 6736 6657 5454 504c 6349 6b66  NT//g6fWTTPLcIkf
+000400c0: 4b79 636b 647a 3757 2f76 5565 4155 2f69  Kyckdz7W/vUeAU/i
+000400d0: 5635 4470 7752 6b69 4335 6f78 3263 6254  V5DpwRkiC5ox2cbT
+000400e0: 4279 6639 6733 7462 5252 3371 3178 7633  Byf9g3tbRR3q1xv3
+000400f0: 676a 574d 6e66 306d 6331 7237 454a 6565  gjWMnf0mc1r7EJee
+00040100: 5239 5449 4d34 3131 5877 544c 646b 2b4e  R9TIM411XwTLdk+N
+00040110: 5834 4e74 312f 4f63 4459 524f 7556 766f  X4Nt1/OcDYROuVvo
+00040120: 5350 545a 5754 6167 5569 6e56 7646 6f42  SPTZWTagUinVvFoB
+00040130: 4557 6f42 375a 5349 6d42 596c 4163 4339  EWoB7ZSImBYlAcC9
+00040140: 5174 3070 5261 5441 2f43 3278 6551 4a56  Qt0pRaTA/C2xeQJV
+00040150: 7256 7a73 3558 6b7a 6567 314b 4331 4344  rVzs5Xkzeg1KC1CD
+00040160: 7679 4141 6a35 5975 4869 2f70 6e55 4c6e  vyAAj5YuHi/pnULn
+00040170: 3137 5269 4872 7755 5958 3141 4c32 5065  17RiHrwUYX1AL2Pe
+00040180: 7143 716d 5234 6855 5659 386f 6167 7971  qCqmR4hUVY8oagyq
+00040190: 697a 5047 6572 3072 7833 7979 6b30 5a50  izPGer0rx3yyk0ZP
+000401a0: 4846 5234 7563 4933 6372 6d55 654c 5256  HFR4ucI3crmUeLRV
+000401b0: 5032 3642 5031 6645 484d 5070 4231 3058  P26BP1fEHMPpB10X
+000401c0: 3357 5364 7147 6c43 6161 4c56 5136 6472  3WSdqGlCaaLVQ6dr
+000401d0: 6643 3561 556f 4149 416c 5147 7075 4a4b  fC5aUoAIAlQGpuJK
+000401e0: 7a51 7950 2f4a 7543 6437 5978 7164 2b55  zQyP/JuCd7Yxqd+U
+000401f0: 3235 4b2b 4b4d 585a 5766 786b 7565 4a35  25K+KMXZWfxkueJ5
+00040200: 4852 7237 4f79 6471 3443 3477 5751 556e  HRr7Oydq4C4wWQUn
+00040210: 7842 7557 4278 652f 7179 7867 5842 4a59  xBuWBxe/qyxgXBJY
+00040220: 626b 7468 6430 394c 6e38 4f70 6e47 7730  bkthd09Ln8OpnGw0
+00040230: 4132 386f 4f74 6978 7a57 7153 7441 5270  A28oOtixzWqStARp
+00040240: 5641 5935 4e45 326f 3064 734b 6d70 7343  VAY5NE2o0dsKmpsC
+00040250: 4b56 6a56 4172 5241 4e50 2f33 7957 712b  KVjVArRANP/3yWq+
+00040260: 5738 4663 3349 424d 5241 5263 7542 2f53  W8Fc3IBMRARcuB/S
+00040270: 3674 6574 6135 747a 7452 7269 2f37 5843  6teta5tztRri/7XC
+00040280: 4636 2b58 5a4c 7456 6457 5773 4459 7738  F6+XZLtVdWWsDYw8
+00040290: 5134 764e 4b33 7666 6f61 6473 6f53 2f55  Q4vNK3vfoadsoS/U
+000402a0: 7554 686e 464c 6d79 6d51 5444 4c4f 5574  uThnFLmymQTDLOUt
+000402b0: 3765 7138 6849 2f35 7042 4e56 5658 3856  7eq8hI/5pBNVVX8V
+000402c0: 6178 4952 3972 3636 4967 675a 6d6a 6c52  axIR9r66IggZmjlR
+000402d0: 5478 4546 4d55 4543 4945 454b 5357 4867  TxEFMUECIEEKSWHg
+000402e0: 5345 4a45 6953 3571 6a59 2f36 3646 5a4f  SEJEiS5qjY/66FZO
+000402f0: 5862 7474 5230 4e4e 666a 5944 3263 6b38  XbttR0NNfjYD2ck8
+00040300: 4435 4b6f 6457 316d 6f41 6764 6331 7161  D5KodW1moAgdc1qa
+00040310: 4f43 3374 5045 5733 3555 314f 5052 6964  OC3tPEW35U1OPRid
+00040320: 5379 667a 2f63 7157 5034 336f 484e 2f47  Syfz/cqWP43oHN/G
+00040330: 354a 5652 394d 6b55 4232 5a41 6831 5853  5JVR9MkUB2ZAh1XS
+00040340: 7541 3545 4947 4e51 744b 5667 4544 3949  uA5EIGNQtKVgED9I
+00040350: 4e42 3259 314d 622b 4143 4379 336e 4365  NB2Y1Mb+ACCy3nCe
+00040360: 5438 5954 686c 6f63 6967 5030 5a52 6476  T8YThlocigP0ZRdv
+00040370: 4e39 6c48 562b 6568 546e 4573 4439 646b  N9lHV+ehTnEsD9dk
+00040380: 384c 6855 766b 7257 6172 2f62 7436 4e76  8LhUvkrWar/bt6Nv
+00040390: 7043 747a 5635 6131 674b 5859 344a 3041  pCtzV5a1gKXY4J0A
+000403a0: 6e6a 3171 5663 766c 6b4b 3939 466b 734e  nj1qVcvlkK99FksN
+000403b0: 564e 5138 4272 6245 3649 6a6b 6f52 5135  VNQ8BrbE6IjkoRQ5
+000403c0: 4542 7651 516f 676c 2b4e 2b54 6575 4b33  EBvQQogl+N+TeuK3
+000403d0: 4b77 4f6e 6b4a 7442 7867 7944 506e 6132  KwOnkJtBxgyDPna2
+000403e0: 4654 5335 636c 7149 4971 3273 735a 4774  FTS5clqIIq2ssZGt
+000403f0: 5733 304a 4368 4661 3435 6e4c 572b 695a  W30JChFa45nLW+iZ
+00040400: 316e 5867 4746 5830 3545 7843 5074 3232  1nXgGFX05ExCPt22
+00040410: 4c39 4b68 3159 7157 6d7a 5450 7769 3048  L9Kh1YqWmzTPwi0H
+00040420: 5145 364d 4272 2f72 2f7a 7648 5976 664a  QE6MBr/r/zvHYvfJ
+00040430: 4449 6c58 734d 412b 6d50 4f46 6537 617a  DIlXsMA+mPOFe7az
+00040440: 4e6f 3231 6f6c 6e70 7767 7a70 7469 396b  No21olnpwgzpti9k
+00040450: 3374 5770 6171 726b 746f 4336 4a67 632b  3tWpaqrktoC6Jgc+
+00040460: 4c52 7635 7a37 456f 4d69 4278 4341 6c41  LRv5z7EoMiBxCAlA
+00040470: 7365 7a76 4a67 6736 7748 4f4a 2f7a 5653  sezvJgg6wHOJ/zVS
+00040480: 5349 496f 7036 3362 3344 6655 6c34 4548  SIIop63b3DfUl4EH
+00040490: 3246 4845 6b57 3953 6a6d 5352 4964 6542  2FHEkW9SjmSRIdeB
+000404a0: 7130 776e 414b 526e 7a74 6d63 7565 654a  q0wnAKRnztmcueeJ
+000404b0: 7971 466e 4747 506e 6330 7972 5735 7230  yqFnGGPnc0yrW5r0
+000404c0: 5753 304f 7574 5a36 4531 5172 326e 4e38  WS0OutZ6E1Qr2nN8
+000404d0: 6e77 6d58 5a32 5833 7158 4d46 2b64 4279  nwmXZ2X3qXMF+dBy
+000404e0: 3961 4766 5273 5572 6265 6264 3943 766e  9aGfRsUrbebd9Cvn
+000404f0: 4131 5662 5566 6776 5559 7033 7843 4d58  A1VbUfgvUYp3xCMX
+00040500: 2b35 554f 352f 6171 5872 7966 734b 4773  +5UO5/aqXryfsKGs
+00040510: 3745 4733 7442 4c4a 6d76 3839 4c79 6c32  7EG3tBLJmv89Lyl2
+00040520: 644c 6856 4b63 7859 3370 7952 4d39 4d70  dLhVKcxY3pyRM9Mp
+00040530: 7541 6e67 7375 3477 6665 7349 6f54 6f48  uAngsu4wfesIoToH
+00040540: 4547 6179 684c 4459 4673 6753 4556 4e71  EGayhLDYFsgSEVNq
+00040550: 7377 6e66 7567 4c4a 6762 6f53 4743 6870  swnfugLJgboSGChp
+00040560: 334d 6247 7568 7575 4c6d 4d57 3434 4d70  3MbGuhuuLmMW44Mp
+00040570: 5a43 4e7a 6537 6330 612b 3362 4449 3545  ZCNze7c0a+3bDI5E
+00040580: 4879 7150 3266 6e71 6133 5669 656f 3276  HyqP2fnqa3Vieo2v
+00040590: 4a6d 6f72 6179 6c4a 7652 4f4c 6455 5a6d  JmoraylJvROLdUZm
+000405a0: 5538 6b57 394e 577a 6657 3262 5a38 4b76  U8kW9NWzfW2bZ8Kv
+000405b0: 666b 7a78 5162 3151 3454 6b51 476d 536a  fkzxQb1Q4TkQGmSj
+000405c0: 4530 4836 6765 4274 674f 4147 316b 682b  E0H6geBtgOAG1kh+
+000405d0: 5932 634f 6164 6c36 7573 2b53 6a68 5676  Y2cOadl6us+SjhVv
+000405e0: 7157 4a61 5744 3561 656b 6e61 334c 7a48  qWJaWD5aekna3LzH
+000405f0: 6c72 6176 4d6e 6b51 4d43 3638 3137 4b4e  lravMnkQMC6817KN
+00040600: 754d 3748 3067 4351 3435 4e67 6255 6563  uM7H0gCQ45NgbUec
+00040610: 6d77 7232 4d41 5a59 4d75 6931 494d 6762  mwr2MAZYMui1IMgb
+00040620: 4645 4154 3648 4f54 4d61 6a46 4c31 5755  FEAT6HOTMajFL1WU
+00040630: 2f4b 4f44 5637 574e 5665 6d6f 736a 5677  /KODV7WNVemosjVw
+00040640: 4843 717a 3544 634c 4c35 6e35 345a 546e  HCqz5DcLL5n54ZTn
+00040650: 5957 5531 6f53 6c44 3656 5872 576b 7571  YWU1oSlD6VXrWkuq
+00040660: 7265 4175 596c 5743 5a61 6272 6663 382f  reAuYlWCZabrfc8/
+00040670: 7849 5944 6e30 546f 736c 6963 6969 5539  xIYDn0TosliciiU9
+00040680: 7961 6872 7455 336d 4f54 5472 5654 6d7a  yahrtU3mOTTrVTmz
+00040690: 644b 7254 7567 3930 4774 6b52 6230 3750  dKrTug90GtkRb07P
+000406a0: 4f31 3366 756a 5957 6341 6b76 6e64 6a56  O13fujYWcAkvndjV
+000406b0: 5361 5464 7470 4e34 6a66 6b51 5441 396e  SaTdtpN4jfkQTA9n
+000406c0: 4147 5752 7a7a 4532 6742 7744 6d4c 334c  AGWRzzE2gBwDmL3L
+000406d0: 4554 4776 4d55 454d 6644 4e30 4b75 4548  ETGvMUEMfDN0KuEH
+000406e0: 4170 7269 6834 6251 5351 5373 7644 6164  Aprih4bQSQSsvDad
+000406f0: 7166 4378 4454 6f5a 6c30 4f76 456d 3535  qfCxDToZl0OvEm55
+00040700: 5058 4656 5844 5370 6d46 5869 3537 7249  PXFVXDSpmFXi57rI
+00040710: 4646 7139 4c42 6e58 5635 5976 4f44 7542  FFq9LBnXV5YvODuB
+00040720: 6833 3835 3043 5538 5442 5270 6e63 4645  h3850CU8TBRpncFE
+00040730: 6533 4967 6148 5256 5851 644b 4839 494f  e3IgaHRVXQdKH9IO
+00040740: 4e57 3379 4a70 3032 5839 3061 5764 6142  NW3yJp02X90aWdaB
+00040750: 4676 5849 3764 6730 6a6c 6239 6839 6850  FvXI7dg0jlb9h9hP
+00040760: 6e70 7261 6b51 696e 5337 344c 5556 337a  nprakQinS74LUV3z
+00040770: 3431 334b 5231 366f 6477 514f 5244 4a74  413KR16odwQORDJt
+00040780: 7079 3761 7571 314c 5470 616b 656a 6549  py7auq1LTpakejeI
+00040790: 6459 6f6e 4f69 7162 3135 7043 3877 3532  dYonOiqb15pC8w52
+000407a0: 702b 5638 4c30 4f65 7265 6a41 3567 4844  p+V8L0OerejA5gHD
+000407b0: 3933 6d65 6d2f 454c 4e5a 4344 7a56 7551  93mem/ELNZCDzVuQ
+000407c0: 5849 6738 4333 4775 6675 6332 647a 5556  XIg8C3Gufuc2dzUV
+000407d0: 4a64 7469 517a 314c 4268 3234 5a6b 6570  JdtiQz1LBh24Zkep
+000407e0: 365a 5779 684a 3246 5a2f 6c5a 4a78 544f  6ZWyhJ2FZ/lZJxTO
+000407f0: 4f4d 3334 3141 4a38 3279 4148 5069 5934  OM341AJ82yAHPiY4
+00040800: 6a76 5363 7237 4d4d 7a31 2f58 6f34 634f  jvScr7MMz1/Xo4cO
+00040810: 4c78 796d 3150 3542 6275 7461 3972 6935  Lxym1P5Bbuta9ri5
+00040820: 4542 4d76 6951 2f37 3657 6c7a 5836 684b  EBMviQ/76WlzX6hK
+00040830: 6466 526b 4176 7447 304d 4f35 7562 4b62  dfRkAvtG0MO5ubKb
+00040840: 7166 5330 4b34 7a62 6b31 4572 324a 4635  qfS0K4zbk1Er2JF5
+00040850: 7830 3474 454a 6e30 5245 7031 4174 5143  x04tEJn0REp1AtQC
+00040860: 5058 4f70 7670 6649 6e58 354f 6274 4d37  PXOpvpfInX5ObtM7
+00040870: 5a4c 2f4b 6237 526f 456e 3853 6a69 6639  ZL/Kb7RoEn8Sjif9
+00040880: 7977 5a69 6852 3346 5739 6c37 6b44 7069  ywZihR3FW9l7kDpi
+00040890: 5a38 784c 6e65 4a6b 6b50 7841 6749 6858  Z8xLneJkkPxAgIhX
+000408a0: 6641 794e 7a74 4a35 3963 7770 476f 5464  fAyNztJ59cwpGoTd
+000408b0: 6f4c 6a4d 4d6f 7032 4d4c 6f56 564b 3439  oLjMMop2MLoVVK49
+000408c0: 5534 3632 2b58 4471 6337 697a 6a73 544f  U462+XDqc7izjsTO
+000408d0: 2f52 666c 3834 366f 757a 6438 7732 5349  /Rfl846ouzd8w2SI
+000408e0: 304b 4d70 4d75 3853 7663 6733 5571 5173  0KMpMu8Svcg3UqQs
+000408f0: 522f 4f53 4c4b 2b44 495a 5966 5748 7972  R/OSLK+DIZYfWHyr
+00040900: 636a 6757 6667 6d71 4546 664c 5131 5742  cjgWfgmqEFfLQ1WB
+00040910: 5237 4762 326a 6d53 4978 6332 6e59 5844  R7Gb2jmSIxc2nYXD
+00040920: 5039 7132 552f 4f62 4733 672f 6853 532b  P9q2U/ObG3g/hSS+
+00040930: 6254 6236 6c6d 5337 704f 3068 392f 6d56  bTb6lmS7pO0h9/mV
+00040940: 7675 4e68 5975 4144 7965 4232 7867 4170  vuNhYuADyeB2xgAp
+00040950: 6778 495a 5072 3756 7372 2b73 5a57 702f  gxIZPr7Vsr+sZWp/
+00040960: 3968 4d77 4a45 554b 4447 4f58 7744 7873  9hMwJEUKDGOXwDxs
+00040970: 3276 7a36 3732 6e73 6658 4168 3978 2f61  2vz672nsfXAh9x/a
+00040980: 5472 5a71 3339 796a 6637 3457 3438 6550  TrZq39yjf74W48eP
+00040990: 6469 3631 7643 4b47 7147 4d6c 3742 6339  di61vCKGqGMl7Bc9
+000409a0: 5136 4b53 4752 3554 4a41 4e59 494a 384b  Q6KSGR5TJANYIJ8K
+000409b0: 2b45 7558 314d 3042 3047 434f 4b4a 2b50  +EuX1M0B0GCOKJ+P
+000409c0: 5231 6742 6552 522f 3975 7530 4c6a 4d6e  R1gBeRR/9uu0LjMn
+000409d0: 5476 366b 734b 5748 6b35 7446 4b54 6b51  Tv6ksKWHk5tFKTkQ
+000409e0: 3136 646b 6259 7a53 314d 5335 6b62 637a  16dkbYzS1MS5kbcz
+000409f0: 3068 4446 7451 7043 3359 7134 6658 7773  0hDFtQpC3Yq4fXws
+00040a00: 3236 6462 2b48 4c55 4c78 5656 7166 5770  26db+HLULxVVqfWp
+00040a10: 5044 7269 3257 5139 5953 3761 6c57 2f4c  PDri2WQ9YS7alW/L
+00040a20: 4a73 3674 6550 5036 3351 4833 726f 7a30  Js6tePP63QH3roz0
+00040a30: 624f 686f 5170 5630 596d 764a 4270 7949  bOhoQpV0YmvJBpyI
+00040a40: 474b 4364 4149 546f 4948 6477 634f 4c43  GKCdAIToIHdwcOLC
+00040a50: 4c4a 6872 4b44 516b 4b53 3172 6456 624d  LJhrKDQkKS1rdVbM
+00040a60: 4877 2b6b 4b54 4475 2b4c 6467 356e 546e  Hw+kKTDu+Ldg5nTn
+00040a70: 6246 392b 365a 6233 6570 4f50 636a 4831  bF9+6Zb3epOPcjH1
+00040a80: 706e 6e76 7854 7769 794c 3473 5954 3077  pnnvxTwiyL4sYT0w
+00040a90: 4a37 5a62 6873 3664 6753 382b 2f37 634e  J7Zbhs6dgS8+/7cN
+00040aa0: 616e 6d4c 4576 4b52 495a 3368 687a 6c6b  anmLEvKRIZ3hhzlk
+00040ab0: 4736 7563 5665 6366 5557 726a 6c59 6b75  G6ucVecfUWrjlYku
+00040ac0: 7055 6730 4e42 3079 6453 3155 6e7a 446e  pUg0NB0ydS1UnzDn
+00040ad0: 674f 6879 4247 4674 7962 4e6e 6434 356d  gOhyBGFtybNnd45m
+00040ae0: 5267 7774 6a43 4c54 6641 7159 6167 5678  RgwtjCLTfAqYagVx
+00040af0: 6168 4862 3032 7858 7231 5362 7372 722b  ahHb02xXr1Sbsrr+
+00040b00: 494b 494a 6f66 357a 4936 5473 5845 3237  IKIJof5zI6TsXE27
+00040b10: 7936 6263 4d45 4750 362b 7a6c 6348 5a6e  y6bcMEGP6+zlcHZn
+00040b20: 5263 3476 6675 5054 4976 7138 424f 6947  Rc4vfuPTIvq8BOiG
+00040b30: 794a 4931 484e 4530 6343 7934 4255 3334  yJI1HNE0cCy4BU34
+00040b40: 3537 4e56 6b44 3345 6751 7751 6436 5a59  57NVkD3EgQwQd6ZY
+00040b50: 4573 484a 7041 6b47 452b 4938 4656 5959  EsHJpAkGE+I8FVYY
+00040b60: 314e 6f54 3434 6f6b 4369 5a58 4672 4d6d  1NoT44okCiZXFrMm
+00040b70: 7043 442b 5569 4644 5558 6b64 4775 486c  pCD+UiFDUXkdGuHl
+00040b80: 3765 7239 7031 574c 7079 4f2f 2f57 786c  7er9p1WLpyO//Wxl
+00040b90: 3455 4246 3877 3146 7578 5733 5679 4a2b  4UBF8w1FuxW3VyJ+
+00040ba0: 3944 2f79 5a70 4d77 664c 6265 3854 7771  9D/yZpMwfLbe8Twq
+00040bb0: 5341 614f 6d6d 3151 3249 676b 6a6e 6271  SAaOmm1Q2Igkjnbq
+00040bc0: 3354 7667 6568 3267 6942 7763 7576 3072  3Tvgeh2giBwcuv0r
+00040bd0: 7163 7251 4647 4347 4c6a 574f 6b32 6548  qcrQFGCGLjWOk2eH
+00040be0: 6d55 6233 4b51 6a6b 4369 7471 3244 5964  mUb3KQjkCitq2DYd
+00040bf0: 5568 6c54 4e77 4a6b 7646 7837 2f32 6971  UhlTNwJkvFx7/2iq
+00040c00: 6932 482f 3839 7777 3569 377a 3766 782f  i2H/89ww5i7z7fx/
+00040c10: 2f35 5652 7430 4236 4158 5873 7255 7048  /5VRt0B6AXXsrUpH
+00040c20: 4535 7055 3467 494f 5972 5277 4868 4e2b  E5pU4gIOYrRwHhN+
+00040c30: 7a76 7076 4641 6c4d 336e 4857 7a79 3149  zvpvFAlM3nHWzy1I
+00040c40: 6934 3262 4241 5651 5241 436e 4b46 4779  i42bBAVQRACnKFGy
+00040c50: 5830 5366 5259 3374 7875 4b75 5061 4776  X0SfRY3txuKuPaGv
+00040c60: 346c 464a 4e46 4f78 6f4f 7a74 4f50 4273  4lFJNFOxoOztOPBs
+00040c70: 4d76 4c46 6d5a 4e2b 446f 4d75 3770 3545  MvLFmZN+DoMu7p5E
+00040c80: 722f 5242 4c6b 4543 4649 4246 7835 6748  r/RBLkECFIBFx5gH
+00040c90: 7455 5870 6770 2b4e 7278 6668 6830 635a  tUXpgp+Nrxfhh0cZ
+00040ca0: 5566 766b 3576 3055 6c6a 314d 4359 725a  Ufvk5v0Ulj1MCYrZ
+00040cb0: 4f57 4b5a 4575 2b30 7739 5156 6741 7168  OWKZEu+0w9QVgAqh
+00040cc0: 7941 6155 2b51 4d2b 3433 3572 596d 4264  yAaU+QM+435rYmBd
+00040cd0: 7456 3636 3759 596c 7634 6445 4d64 6446  tV667YYlv4dEMddF
+00040ce0: 5871 5574 5730 7073 5869 2f4f 6542 4e75  XqUtW0psXi/OeBNu
+00040cf0: 6e45 5372 776d 5362 2b6c 5a52 4837 627a  nESrwmSb+lZRH7bz
+00040d00: 556b 2f30 5837 4939 636b 4235 3756 304b  Uk/0X7I9ckB57V0K
+00040d10: 3047 6d54 3763 4754 6d44 7076 4b50 2b2b  0GmT7cGTmDpvKP++
+00040d20: 5536 3030 3175 464e 744c 3947 6d5a 4679  U6001uFNtL9GmZFy
+00040d30: 574a 306b 3436 6666 5258 3677 564c 5565  WJ0k46ffRX6wVLUe
+00040d40: 7a65 3275 484f 6d58 4950 3365 594a 7462  ze2uHOmXIP3eYJtb
+00040d50: 5174 5962 7966 734e 6b6a 4a4a 3742 5a54  QtYbyfsNkjJJ7BZT
+00040d60: 6d4c 5276 3874 6541 554a 796c 454e 4868  mLRv8teAUJylENHh
+00040d70: 4748 4c47 4d75 6d63 3936 636e 6164 307a  GHLGMumc96cnad0z
+00040d80: 7748 437a 7848 4e75 6a4f 5462 5134 666d  wHCzxHNujOTbQ4fm
+00040d90: 5565 7330 7249 5571 7736 3575 4c57 3743  Ues0rIUqw65uLW7C
+00040da0: 494a 5846 6866 4f57 356f 5379 6641 455a  IJXFhfOW5oSyfAEZ
+00040db0: 5470 394f 5743 2b61 4470 3944 396c 6778  Tp9OWC+aDp9D9lgx
+00040dc0: 584a 7750 7a58 2b67 7571 6433 5971 3752  XJwPzX+guqd3Yq7R
+00040dd0: 4e31 4a56 435a 424e 4e43 6276 5050 5a4d  N1JVCZBNNCbvPPZM
+00040de0: 7164 5065 6b44 5173 546f 6952 7a6b 4d67  qdPekDQsToiRzkMg
+00040df0: 5957 475a 3041 515a 4d6e 7133 6b6d 7859  YWGZ0AQZMnq3kmxY
+00040e00: 4867 316b 4751 7248 7977 6b79 454e 416b  Hg1kGQrHywkyENAk
+00040e10: 4e71 5149 4232 5241 3945 7442 4945 6837  NqQIB2RA9EtBIEh7
+00040e20: 7041 5a64 616c 3876 7959 6142 6c71 4644  pAZdal8vyYaBlqFD
+00040e30: 7234 4845 4947 5662 3645 3849 6c58 4472  r4HEIGVb6E8IlXDr
+00040e40: 5478 2b4e 4877 7078 4161 6869 646e 5a46  Tx+NHwpxAahidnZF
+00040e50: 6a6d 7958 3550 626d 572f 3556 6a49 716d  jmyX5PbmW/5VjIqm
+00040e60: 6941 4267 4369 6a50 7176 5a34 5030 454e  iABgCijPqvZ4P0EN
+00040e70: 3747 434a 397a 2b64 4e42 514a 7950 4168  7GCJ9z+dNBQJyPAh
+00040e80: 2b47 6137 5964 6e75 6572 5761 7246 5676  +Ga7YdnuerWarFVv
+00040e90: 516b 515a 4d69 7239 3666 6471 756a 4837  QkQZMir96fdqujH7
+00040ea0: 4e53 4553 5451 6f72 3466 6a63 7a49 4156  NSESTQor4fjczIAV
+00040eb0: 6878 3552 6474 5749 776a 556a 6332 656e  hx5RdtWIwjUjc2en
+00040ec0: 6867 344c 2f4b 2f44 4463 4264 6a62 3871  hg4L/K/DDcBdjb8q
+00040ed0: 7637 6964 5455 6575 2b43 4369 7276 6b76  v7idTUeu+CCirvkv
+00040ee0: 696e 594e 6769 4377 4748 5872 4e38 376a  inYNgiCwGHXrN87j
+00040ef0: 5858 6246 5131 546b 6756 3146 6b4d 556b  XXbFQ1TkgV1FkMUk
+00040f00: 6a56 6c39 7964 4b46 674d 6b30 7477 6c72  jVl9ydKFgMk0twlr
+00040f10: 2f74 6261 634c 4968 3832 384f 3157 6f4c  /tbacLIh828O1WoL
+00040f20: 5254 5676 534d 7332 2f50 722b 4644 6a46  RTVvSMs2/Pr+FDjF
+00040f30: 7539 6355 3262 4166 4b39 3164 734b 7671  u9cU2bAfK91dsKvq
+00040f40: 7574 6b50 3044 2f6a 5834 5a43 4e47 7653  utkP0D/jX4ZCNGvS
+00040f50: 666f 7231 5870 4754 3963 3659 7537 7261  for1XpGT9c6Yu7ra
+00040f60: 3933 3176 4d71 387a 5748 6249 5967 4244  931vMq8zWHbIYgBD
+00040f70: 4155 6d7a 4270 6b5a 394d 394f 3678 374b  AUmzBpkZ9M9O6x7K
+00040f80: 5648 4b45 6352 4165 5a50 5a63 4c62 626f  VHKEcRAeZPZcLbbo
+00040f90: 6765 5643 4f4b 6e31 6e49 6636 6d59 4471  geVCOKn1nIf6mYDq
+00040fa0: 5575 6c7a 6b64 5976 502f 6c2b 4954 756c  UulzkdYvP/l+ITul
+00040fb0: 694d 496e 477a 4750 6e42 4e6f 7256 7631  iMInGzGPnBNorVv1
+00040fc0: 7a7a 4e6e 636a 326b 6e4d 7a61 3766 5779  zzNncj2knMza7fWy
+00040fd0: 5761 7259 7473 6a69 4161 652f 6561 4e61  WarYtsjiAae/eaNa
+00040fe0: 4b41 446a 4754 4a35 4271 4b4f 7454 3643  KADjGTJ5BqKOtT6C
+00040ff0: 4653 4b51 6e49 5a72 322f 436d 3478 6237  FSKQnIZr2/Cm4xb7
+00041000: 4a49 7748 2f58 7072 636e 6336 765a 3330  JIwH/Xprcnc6vZ30
+00041010: 3545 674b 4b4d 6b32 5949 4534 577a 6d64  5EgKKMk2YIE4Wzmd
+00041020: 4876 5534 4635 3237 7033 6975 7141 5830  HvU4F527p3iuqAX0
+00041030: 476f 3749 4146 5175 706d 3137 6471 3065  Go7IAFQupm17dq0e
+00041040: 6855 5432 2b4c 5671 6335 696d 7955 4941  hUT2+LVqc5imyUIA
+00041050: 6336 456a 4431 6e54 356a 3161 6276 3932  c6EjD1nT5j1abv92
+00041060: 4269 4347 4344 4a5a 6b31 5936 6d38 4262  BiCGCDJZk1Y6m8Bb
+00041070: 384a 4850 5870 7230 7332 3048 3871 6756  8JHPXpr0s20H8qgV
+00041080: 3748 7a71 674f 696a 6e4b 4c45 4151 3837  7HzqgOijnKLEAQ87
+00041090: 3967 486d 464f 6f36 5556 6c55 4765 6644  9gHmFOo6UVlUGefD
+000410a0: 3532 2f76 796f 6259 5167 514a 5954 5279  52/vyobYQgQJYTRy
+000410b0: 3248 754d 5443 6371 7252 6e34 4c6f 5958  2HuMTCcqrRn4LoYX
+000410c0: 654a 6975 7731 3431 754b 5476 466b 5051  eJiuw141uKTvFkPQ
+000410d0: 6164 6544 3071 3953 3064 4155 6f32 6476  adeD0q9S0dAUo2dv
+000410e0: 624f 4462 7773 7138 6e55 5a5a 4c4a 6c72  bODbwsq8nUZZLJlr
+000410f0: 5578 6b6d 344a 4632 356b 6842 774a 3148  Uxkm4JF25khBwJ1H
+00041100: 6539 5566 5473 4633 492b 5a30 3531 526a  e9UfTsF3I+Z051Rj
+00041110: 2f56 4b47 4849 6738 4d78 6658 6330 4531  /VKGHIg8MxfXc0E1
+00041120: 7373 735a 494d 4664 6378 546a 687a 4a6c  sssZIMFdcxTjhzJl
+00041130: 6f45 306e 464c 2f31 6662 7a54 5135 4556  oE0nFL/1fbzTQ5EV
+00041140: 3361 4337 6756 515a 5171 6259 6332 6231  3aC7gVQZQqbYc2b1
+00041150: 5744 564e 4938 704f 7241 7474 6530 3954  WDVNI8pOrAtte09T
+00041160: 4763 7761 304a 5077 6668 5537 4153 6233  Gcwa0JPwfhU7ASb3
+00041170: 5748 487a 7069 656a 4862 5139 5945 3658  WHHzpiejHbQ9YE6X
+00041180: 3164 6778 6852 374c 4275 3733 7276 3370  1dgxhR7LBu73rv3p
+00041190: 6b36 4746 4f76 446e 495a 4238 764e 7964  k6GFOvDnIZB8vNyd
+000411a0: 6171 7a2b 5077 5178 4144 4f6d 4650 5941  aqz+PwQxADOmFPYA
+000411b0: 3962 4b35 2f71 3232 7a63 6b69 6948 5078  9bK5/q22zckiiHPx
+000411c0: 7043 4750 4e52 6d58 706e 7069 4344 4a6f  pCGPNRmXpnpiCDJo
+000411d0: 5774 6c59 5745 766a 6c4b 6232 4a78 644e  WtlYWEvjlKb2JxdN
+000411e0: 764d 4a56 3269 4443 622f 2f76 5a50 7475  vMJV2iDCb//vZPtu
+000411f0: 5451 6f62 3834 4936 4e77 6159 2b65 4639  TQob84I6NwaY+eF9
+00041200: 7334 6741 3853 5974 5854 7a32 3242 6278  s4gA8SYtXTz22Bbx
+00041210: 4559 3131 4461 4639 5243 6c50 5a37 544d  EY11DaF9RClPZ7TM
+00041220: 6b52 4c37 6143 6939 5561 414e 336d 4154  kRL7aCi9UaAN3mAT
+00041230: 5147 5073 6d6c 6e54 3778 4472 655a 4673  QGPsmlnT7xDreZFs
+00041240: 3757 6c59 3277 4751 5469 624d 634d 6179  7WlY2wGQTibMcMay
+00041250: 3259 4858 694e 4b6a 4535 686c 7059 4750  2YHXiNKjE5hlpYGP
+00041260: 6347 4c54 7530 614c 376f 7434 764e 4c45  cGLTu0aL7ot4vNLE
+00041270: 414f 596e 4c49 4864 7559 542b 2f62 6c7a  AOYnLIHduYT+/blz
+00041280: 3639 614a 5647 6947 5856 4b42 307a 734f  69aJVGiGXVKB0zsO
+00041290: 3774 5437 5943 6b32 6452 4a2f 4d53 5a4d  7tT7YCk2dRJ/MSZM
+000412a0: 3533 4f65 7131 4e65 7438 6350 7878 3943  53Oeq1Net8cPxx9C
+000412b0: 4d77 7053 3467 646f 486e 7078 6e56 772f  MwpS4gdoHnpxnVw/
+000412c0: 4765 6355 7a62 3968 5042 3577 6565 6649  GecUzb9hPB5weefI
+000412d0: 4169 6371 4437 7777 4159 7653 4853 574b  AicqD7wwAYvSHSWK
+000412e0: 5030 4f32 566c 7574 4465 524d 327a 3258  P0O2VlutDeRM2z2X
+000412f0: 4f65 3276 3148 3345 3879 2b64 624c 7552  Oe2v1H3E8y+dbLuR
+00041300: 5541 536c 454e 4d6a 4142 6644 4949 5934  UASlENMjABfDIIY4
+00041310: 466c 3235 3530 3375 4d2b 644a 6372 7a7a  Fl25503uM+dJcrzz
+00041320: 7a48 5236 5848 3544 4342 495a 7a74 785a  zHR6XH5DCBIZztxZ
+00041330: 776e 5347 5849 6743 5443 3949 7a4a 454d  wnSGXIgCTC9IzJEM
+00041340: 5875 322f 434c 4f4d 3961 484c 785a 4246  Xu2/CLOM9aHLxZBF
+00041350: 4c6a 7557 4632 3337 3530 3534 794a 424f  LjuWF2375054yJBO
+00041360: 6f73 4e50 666d 4b39 622f 6d47 7434 5a73  osNPfmK9b/mGt4Zs
+00041370: 6e63 6173 6463 6f69 3233 3750 7369 6d51  ncasdcoi237PsimQ
+00041380: 554a 4845 4e51 6875 6770 3446 7066 684f  UJHENQhugp4FpfhO
+00041390: 3970 6246 4667 4f6c 7464 5635 4d42 3251  9pbFFgOltdV5MB2Q
+000413a0: 454c 4735 4369 4c4c 794a 4246 4c42 4459  ELG5CiLLyJBFLBDY
+000413b0: 4d66 4159 5556 5841 4430 5365 6f6b 7439  MfAYUVXAD0Seokt9
+000413c0: 562b 5730 4776 6739 7276 4b38 2b46 2b78  V+W0Gvg9rvK8+F+x
+000413d0: 3135 6a67 2f67 6944 7248 6141 782f 3578  15jg/giDrHaAx/5x
+000413e0: 6e2f 5776 4357 4858 5a73 3678 4971 4855  n/WvCWHXZs6xIqHU
+000413f0: 3932 4b4c 3634 4869 5149 6655 4e77 6977  92KL64HiQIfUNwiw
+00041400: 3637 4e39 4362 6f6a 6270 794f 4956 6549  67N9CbojbpyOIVeI
+00041410: 7835 4f62 5252 6944 3149 4b38 6962 5477  x5ObRRiD1IK8ibTw
+00041420: 5a74 3038 526b 624f 3370 6e6f 5969 3639  Zt08RkbO3pnoYi69
+00041430: 5338 6b78 4769 486d 4341 6441 5963 3258  S8kxGiHmCAdAYc2X
+00041440: 6431 4a75 774d 784d 5459 4c38 5243 7249  d1JuwMxMTYL8RCrI
+00041450: 3243 6e77 6d46 5856 3033 6974 7a62 6934  2CnwmFXV03itzbi4
+00041460: 5653 5849 5059 676e 6347 5747 485a 7453  VSXIPYgncGWGHZtS
+00041470: 5879 426e 3533 7161 7351 4532 5269 6f47  XyBn53qasQE2RioG
+00041480: 3479 5636 3358 5261 3852 3377 7273 554d  4yV63XRa8R3wrsUM
+00041490: 5545 3242 666f 4253 4233 7266 6968 696f  UE2BfoBSB3rfihio
+000414a0: 4d65 4976 5559 5849 7962 4970 6f4d 4455  MeIvUYXIybIpoMDU
+000414b0: 6270 2f32 4256 5077 7263 6f34 6b6e 3670  bp/2BVPwrco4kn6p
+000414c0: 674e 6d4a 6a43 6336 6135 4a66 4477 4a33  gNmJjCc6a5JfDwJ3
+000414d0: 7971 4950 5568 5859 5773 4e75 365a 4d77  yqIPUhXYWsNu6ZMw
+000414e0: 6174 7238 5842 714b 7945 6d53 4664 6953  atr8XBqKyEmSFdiS
+000414f0: 302f 6934 2b48 5556 6b63 3878 4f70 4b59  0/i4+HUVkc8xOpKY
+00041500: 4f66 7479 6763 6744 6452 774b 695a 484e  OftygcgDdRwKiZHN
+00041510: 7944 3249 4673 536e 5878 4261 3732 4976  yD2IFsSnXxBa72Iv
+00041520: 5561 3349 6962 496c 7361 6d44 7276 5570  Ua3IibIlsamDrvUp
+00041530: 6476 346e 6b61 3367 7248 2f42 7964 7955  dv4nka3grH/BydyU
+00041540: 7967 4534 6f6b 5641 4141 4141 456c 4654  ygE4okVAAAAAElFT
+00041550: 6b53 7551 6d43 430d 0a20 203c 2f44 7269  kSuQmCC..  </Dri
+00041560: 7665 496d 6167 653e 0d0a 3c2f 496e 6765  veImage>..</Inge
+00041570: 6e69 6144 6963 7469 6f6e 6172 793e 0d0a  niaDictionary>..
```

