# Comparing `tmp/prosperity2bt-0.9.0.tar.gz` & `tmp/prosperity2bt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.9.0.tar", last modified: Tue Apr 23 11:52:49 2024, max compression
+gzip compressed data, was "prosperity2bt-0.9.1.tar", last modified: Tue Apr 23 12:03:18 2024, max compression
```

## Comparing `prosperity2bt-0.9.0.tar` & `prosperity2bt-0.9.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.618055 prosperity2bt-0.9.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.630055 prosperity2bt-0.9.0/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.638055 prosperity2bt-0.9.0/prosperity2bt/resources/round4/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.638055 prosperity2bt-0.9.0/prosperity2bt/resources/round6/
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   122003 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   193189 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   447246 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)   563765 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)   564184 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_5.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.650055 prosperity2bt-0.9.0/prosperity2bt/resources/round7/
--rw-r--r--   0 runner    (1001) docker     (127)  1238622 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1956167 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4508145 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)  5728020 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 11:52:47.000000 prosperity2bt-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.680317 prosperity2bt-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-23 12:03:18.680317 prosperity2bt-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.628318 prosperity2bt-0.9.1/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.628318 prosperity2bt-0.9.1/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.632318 prosperity2bt-0.9.1/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.640318 prosperity2bt-0.9.1/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.652318 prosperity2bt-0.9.1/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.656318 prosperity2bt-0.9.1/prosperity2bt/resources/round4/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.660318 prosperity2bt-0.9.1/prosperity2bt/resources/round6/
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122003 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   193189 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   447246 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   563765 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   564184 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_5.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.672318 prosperity2bt-0.9.1/prosperity2bt/resources/round7/
+-rw-r--r--   0 runner    (1001) docker     (127)  1238622 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1956167 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4508145 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  5728020 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-23 12:03:14.000000 prosperity2bt-0.9.1/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:03:18.676318 prosperity2bt-0.9.1/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 12:03:18.000000 prosperity2bt-0.9.1/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 12:03:16.000000 prosperity2bt-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:03:18.680317 prosperity2bt-0.9.1/setup.cfg
```

### Comparing `prosperity2bt-0.9.0/LICENSE` & `prosperity2bt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/PKG-INFO` & `prosperity2bt-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -105,10 +105,26 @@
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
+## Data Files
+
+Data for the following round is included:
+- Round 0: prices and anonymized trades data on AMETHYSTS and STARFRUIT that was used during tutorial submission runs.
+- Round 1: prices, anonymized trades, and de-anonymized trades data on AMETHYSTS and STARFRUIT.
+- Round 3: prices, anonymized trades, and de-anonymized trades data on CHOCOLATE, STRAWBERRIES, ROSES, and GIFT_BASKET.
+- Round 4: prices, anonymized trades, and de-anonymized trades data on COCONUT and COCONUT_COUPON.
+- Round 6: prices data that was used during submission runs. Round 6 day X represents the submission data of round X, where X = 0 means the tutorial round.
+- Round 7: prices data that was used during end-of-round runs. Round 7 day Y represents the end-of-round data of round Y.
+
+Round 2 (ORCHIDS and conversion observations) is not supported. By default de-anonymized trades data is used if it is available, except when the `--no-names` flag is used.
+
+## Environment Variables
+
+During backtests two environment variables are set for the trader to know the round and day it's being backtested on. The environment variable named `PROSPERITY2BT_ROUND` contains the round number and `PROSPERITY2BT_DAY` contains the day number. Note that these environment variables do not exist in the official submission environment, so make sure the code you submit doesn't require them to be defined.
+
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.9.0/prosperity2bt/__main__.py` & `prosperity2bt-0.9.1/prosperity2bt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
     parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
     parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("--no-out", action="store_true", help="skip saving the output log to a file")
     parser.add_argument("--no-progress", action="store_true", help="don't show progress bars")
     parser.add_argument("--vis-requests", type=int, default=2, help="number of requests the visualizer is expected to make to the backtester's HTTP server when using --vis")
     parser.add_argument("--original-timestamps", action="store_true", help="preserve original timestamps in output log rather than making them increase across days")
     parser.add_argument("--max-workers", type=int, default=None, help="maximum number of worker processes to use")
+    parser.add_argument("--no-names", action="store_true", help="don't use de-anonymized trades data, even if it exists")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     if args.vis and args.no_out:
         print("Error: --vis and --no-out are mutually exclusive")
         sys.exit(1)
@@ -271,14 +272,15 @@
                 run_backtest,
                 trader_module.Trader(),
                 file_reader,
                 round_num,
                 day_num,
                 args.print,
                 args.no_trades_matching,
+                args.no_names,
                 progress_queue,
                 i,
             )
 
             if show_live_results:
                 result = future.result()
                 print_day_summary(result)
```

### Comparing `prosperity2bt-0.9.0/prosperity2bt/data.py` & `prosperity2bt-0.9.1/prosperity2bt/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         profit_loss=profit_loss,
     )
 
 def has_day_data(file_reader: FileReader, round_num: int, day_num: int) -> bool:
     with file_reader.file([f"round{round_num}", f"prices_round_{round_num}_day_{day_num}.csv"]) as file:
         return file is not None
 
-def read_day_data(file_reader: FileReader, round_num: int, day_num: int) -> Optional[BacktestData]:
+def read_day_data(file_reader: FileReader, round_num: int, day_num: int, no_names: bool) -> Optional[BacktestData]:
     prices = []
     with file_reader.file([f"round{round_num}", f"prices_round_{round_num}_day_{day_num}.csv"]) as file:
         if file is None:
             return None
 
         for line in file.read_text(encoding="utf-8").splitlines()[1:]:
             columns = line.split(";")
@@ -98,15 +98,17 @@
                 ask_prices=get_column_values(columns, [9, 11, 13]),
                 ask_volumes=get_column_values(columns, [10, 12, 14]),
                 mid_price=float(columns[15]),
                 profit_loss=float(columns[16]),
             ))
 
     trades = []
-    for suffix in ["wn", "nn"]:
+    trades_suffixes = ["nn"] if no_names else ["wn", "nn"]
+
+    for suffix in trades_suffixes:
         with file_reader.file([f"round{round_num}", f"trades_round_{round_num}_day_{day_num}_{suffix}.csv"]) as file:
             if file is None:
                 continue
 
             for line in file.read_text(encoding="utf-8").splitlines()[1:]:
                 columns = line.split(";")
```

### Comparing `prosperity2bt-0.9.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.9.1/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/file_reader.py` & `prosperity2bt-0.9.1/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/models.py` & `prosperity2bt-0.9.1/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/prices_round_4_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_0.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_1.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_3.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_4.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_4.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_5.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round6/prices_round_6_day_5.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_1.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_2.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_3.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_4.csv` & `prosperity2bt-0.9.1/prosperity2bt/resources/round7/prices_round_7_day_4.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/prosperity2bt/runner.py` & `prosperity2bt-0.9.1/prosperity2bt/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,18 +216,19 @@
 def run_backtest(
     trader: Any,
     file_reader: FileReader,
     round_num: int,
     day_num: int,
     print_output: bool,
     disable_trades_matching: bool,
+    no_names: bool,
     progress_queue: Queue,
     progress_id: int,
 ) -> BacktestResult:
-    data = read_day_data(file_reader, round_num, day_num)
+    data = read_day_data(file_reader, round_num, day_num, no_names)
 
     os.environ["PROSPERITY2BT_ROUND"] = str(round_num)
     os.environ["PROSPERITY2BT_DAY"] = str(day_num)
 
     trader_data = ""
     state = TradingState(
         traderData=trader_data,
```

### Comparing `prosperity2bt-0.9.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.9.1/prosperity2bt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -105,10 +105,26 @@
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
 
+## Data Files
+
+Data for the following round is included:
+- Round 0: prices and anonymized trades data on AMETHYSTS and STARFRUIT that was used during tutorial submission runs.
+- Round 1: prices, anonymized trades, and de-anonymized trades data on AMETHYSTS and STARFRUIT.
+- Round 3: prices, anonymized trades, and de-anonymized trades data on CHOCOLATE, STRAWBERRIES, ROSES, and GIFT_BASKET.
+- Round 4: prices, anonymized trades, and de-anonymized trades data on COCONUT and COCONUT_COUPON.
+- Round 6: prices data that was used during submission runs. Round 6 day X represents the submission data of round X, where X = 0 means the tutorial round.
+- Round 7: prices data that was used during end-of-round runs. Round 7 day Y represents the end-of-round data of round Y.
+
+Round 2 (ORCHIDS and conversion observations) is not supported. By default de-anonymized trades data is used if it is available, except when the `--no-names` flag is used.
+
+## Environment Variables
+
+During backtests two environment variables are set for the trader to know the round and day it's being backtested on. The environment variable named `PROSPERITY2BT_ROUND` contains the round number and `PROSPERITY2BT_DAY` contains the day number. Note that these environment variables do not exist in the official submission environment, so make sure the code you submit doesn't require them to be defined.
+
 ## Development
 
 If you want to make changes to the backtester, clone (or fork and clone) this repository and run `pip install -e .` in the project's root. This installs the project in editable mode, so any changes you make are automatically taken into account the next time you run `prosperity2bt`.
```

### Comparing `prosperity2bt-0.9.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.9.1/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.9.0/pyproject.toml` & `prosperity2bt-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.9.0"
+version = "0.9.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

