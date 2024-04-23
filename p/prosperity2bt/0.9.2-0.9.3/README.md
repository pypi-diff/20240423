# Comparing `tmp/prosperity2bt-0.9.2.tar.gz` & `tmp/prosperity2bt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.9.2.tar", last modified: Tue Apr 23 14:29:56 2024, max compression
+gzip compressed data, was "prosperity2bt-0.9.3.tar", last modified: Tue Apr 23 15:27:38 2024, max compression
```

## Comparing `prosperity2bt-0.9.2.tar` & `prosperity2bt-0.9.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.672711 prosperity2bt-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-23 14:29:56.672711 prosperity2bt-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.624711 prosperity2bt-0.9.2/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.624711 prosperity2bt-0.9.2/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.624711 prosperity2bt-0.9.2/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.632711 prosperity2bt-0.9.2/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.644711 prosperity2bt-0.9.2/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.652711 prosperity2bt-0.9.2/prosperity2bt/resources/round4/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.656711 prosperity2bt-0.9.2/prosperity2bt/resources/round6/
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   122003 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   193189 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   447246 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)   563765 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)   564184 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_5.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.664711 prosperity2bt-0.9.2/prosperity2bt/resources/round7/
--rw-r--r--   0 runner    (1001) docker     (127)  1238622 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1956167 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4508145 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)  5728020 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-23 14:29:52.000000 prosperity2bt-0.9.2/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:56.672711 prosperity2bt-0.9.2/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 14:29:56.000000 prosperity2bt-0.9.2/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-23 14:29:54.000000 prosperity2bt-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:29:56.672711 prosperity2bt-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:38.000719 prosperity2bt-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-23 15:27:38.000719 prosperity2bt-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.952719 prosperity2bt-0.9.3/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.952719 prosperity2bt-0.9.3/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.956719 prosperity2bt-0.9.3/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.960719 prosperity2bt-0.9.3/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.972719 prosperity2bt-0.9.3/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.980719 prosperity2bt-0.9.3/prosperity2bt/resources/round4/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.984719 prosperity2bt-0.9.3/prosperity2bt/resources/round6/
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122003 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   193189 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   447246 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   563765 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   564184 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_5.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:37.992719 prosperity2bt-0.9.3/prosperity2bt/resources/round7/
+-rw-r--r--   0 runner    (1001) docker     (127)  1238622 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1956167 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4508145 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  5728020 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-23 15:27:33.000000 prosperity2bt-0.9.3/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:27:38.000719 prosperity2bt-0.9.3/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 15:27:37.000000 prosperity2bt-0.9.3/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 15:27:35.000000 prosperity2bt-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:27:38.000719 prosperity2bt-0.9.3/setup.cfg
```

### Comparing `prosperity2bt-0.9.2/LICENSE` & `prosperity2bt-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/PKG-INFO` & `prosperity2bt-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.9.2
+Version: 0.9.3
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
-Requires-Dist: multiprocess
 Requires-Dist: orjson
 Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
```

### Comparing `prosperity2bt-0.9.2/README.md` & `prosperity2bt-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/__main__.py` & `prosperity2bt-0.9.3/prosperity2bt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from argparse import ArgumentParser
 from collections import defaultdict
 from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime
 from functools import partial, reduce
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 from importlib import import_module, metadata
-from multiprocess import Manager, Queue
+from multiprocessing import Manager, Queue
 from pathlib import Path
 from prosperity2bt.data import has_day_data
 from prosperity2bt.file_reader import FileReader, FileSystemReader, PackageResourcesReader
 from prosperity2bt.models import BacktestResult
 from prosperity2bt.runner import run_backtest
 from tqdm import tqdm
 from typing import Any, Optional
```

### Comparing `prosperity2bt-0.9.2/prosperity2bt/data.py` & `prosperity2bt-0.9.3/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/datamodel.py` & `prosperity2bt-0.9.3/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/file_reader.py` & `prosperity2bt-0.9.3/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/models.py` & `prosperity2bt-0.9.3/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_1.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/prices_round_4_day_3.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/prices_round_4_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_0.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_1.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_3.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_4.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_4.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round6/prices_round_6_day_5.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round6/prices_round_6_day_5.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_1.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_2.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_3.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/resources/round7/prices_round_7_day_4.csv` & `prosperity2bt-0.9.3/prosperity2bt/resources/round7/prices_round_7_day_4.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/prosperity2bt/runner.py` & `prosperity2bt-0.9.3/prosperity2bt/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from contextlib import closing, redirect_stdout
 from io import StringIO
 from IPython.utils.io import Tee
-from multiprocess import Queue
+from multiprocessing import Queue
 from prosperity2bt.data import BacktestData, LIMITS, read_day_data
 from prosperity2bt.datamodel import Observation, Order, OrderDepth, Symbol, Trade, TradingState
 from prosperity2bt.file_reader import FileReader
 from prosperity2bt.models import ActivityLogRow, BacktestResult, MarketTrade, SandboxLogRow, TradeRow
 from typing import Any
 
 def prepare_state(state: TradingState, data: BacktestData) -> None:
```

### Comparing `prosperity2bt-0.9.2/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.9.3/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.9.2
+Version: 0.9.3
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
-Requires-Dist: multiprocess
 Requires-Dist: orjson
 Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
```

### Comparing `prosperity2bt-0.9.2/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.9.3/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.2/pyproject.toml` & `prosperity2bt-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.9.2"
+version = "0.9.3"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">= 3.9"
-dependencies = ["ipython", "jsonpickle", "multiprocess", "orjson", "tqdm"]
+dependencies = ["ipython", "jsonpickle", "orjson", "tqdm"]
 
 [project.scripts]
 prosperity2bt = "prosperity2bt.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/jmerle/imc-prosperity-2-backtester"
 Issues = "https://github.com/jmerle/imc-prosperity-2-backtester/issues"
```

