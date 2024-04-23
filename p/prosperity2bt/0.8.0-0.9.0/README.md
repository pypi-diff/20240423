# Comparing `tmp/prosperity2bt-0.8.0.tar.gz` & `tmp/prosperity2bt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.8.0.tar", last modified: Mon Apr 22 12:31:33 2024, max compression
+gzip compressed data, was "prosperity2bt-0.9.0.tar", last modified: Tue Apr 23 11:52:49 2024, max compression
```

## Comparing `prosperity2bt-0.8.0.tar` & `prosperity2bt-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.397024 prosperity2bt-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-22 12:31:33.397024 prosperity2bt-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.369023 prosperity2bt-0.8.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.369023 prosperity2bt-0.8.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.369023 prosperity2bt-0.8.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.377023 prosperity2bt-0.8.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.389023 prosperity2bt-0.8.0/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.397024 prosperity2bt-0.8.0/prosperity2bt/resources/round4/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-22 12:31:29.000000 prosperity2bt-0.8.0/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:33.397024 prosperity2bt-0.8.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 12:31:33.000000 prosperity2bt-0.8.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 12:31:31.000000 prosperity2bt-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:31:33.397024 prosperity2bt-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.610055 prosperity2bt-0.9.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.618055 prosperity2bt-0.9.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   272730 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   277553 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   270052 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.630055 prosperity2bt-0.9.0/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   191502 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   184609 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   189148 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.638055 prosperity2bt-0.9.0/prosperity2bt/resources/round4/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92981 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91029 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.638055 prosperity2bt-0.9.0/prosperity2bt/resources/round6/
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122003 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   193189 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   447246 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   563765 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   564184 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round6/prices_round_6_day_5.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.650055 prosperity2bt-0.9.0/prosperity2bt/resources/round7/
+-rw-r--r--   0 runner    (1001) docker     (127)  1238622 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1956167 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4508145 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  5728020 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/resources/round7/prices_round_7_day_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-23 11:52:45.000000 prosperity2bt-0.9.0/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 11:52:49.000000 prosperity2bt-0.9.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 11:52:47.000000 prosperity2bt-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:52:49.658055 prosperity2bt-0.9.0/setup.cfg
```

### Comparing `prosperity2bt-0.8.0/LICENSE` & `prosperity2bt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/PKG-INFO` & `prosperity2bt-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
+Requires-Dist: orjson
 Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
```

### Comparing `prosperity2bt-0.8.0/README.md` & `prosperity2bt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/__main__.py` & `prosperity2bt-0.9.0/prosperity2bt/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 import sys
 import webbrowser
 from argparse import ArgumentParser
 from collections import defaultdict
+from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime
 from functools import partial, reduce
 from http.server import HTTPServer, SimpleHTTPRequestHandler
-from importlib import import_module, metadata, reload
+from importlib import import_module, metadata
+from multiprocessing import Manager, Queue
 from pathlib import Path
-from prosperity2bt.data import BacktestData, read_day_data
-from prosperity2bt.file_reader import FileSystemReader, PackageResourcesReader
+from prosperity2bt.data import has_day_data
+from prosperity2bt.file_reader import FileReader, FileSystemReader, PackageResourcesReader
 from prosperity2bt.models import BacktestResult
 from prosperity2bt.runner import run_backtest
+from tqdm import tqdm
 from typing import Any, Optional
 
 def parse_algorithm(algorithm: str) -> Any:
     algorithm_path = Path(algorithm).expanduser().resolve()
     if not algorithm_path.is_file():
         raise ModuleNotFoundError(f"{algorithm_path} is not a file")
 
     sys.path.append(str(algorithm_path.parent))
     return import_module(algorithm_path.stem)
 
-def parse_days(days: list[str], data_root: Optional[str]) -> list[BacktestData]:
+def parse_data(data_root: Optional[str]) -> FileReader:
     if data_root is not None:
-        file_reader = FileSystemReader(Path(data_root).expanduser().resolve())
+        return FileSystemReader(Path(data_root).expanduser().resolve())
     else:
-        file_reader = PackageResourcesReader()
+        return PackageResourcesReader()
 
+def parse_days(file_reader: FileReader, days: list[str]) -> list[tuple[int, int]]:
     parsed_days = []
 
-    if data_root is not None:
-        data_root = Path(data_root).expanduser().resolve()
-
     for arg in days:
         if "-" in arg:
             round_num, day_num = map(int, arg.split("-", 1))
 
-            day_data = read_day_data(file_reader, round_num, day_num)
-            if day_data is None:
+            if not has_day_data(file_reader, round_num, day_num):
                 print(f"Warning: no data found for round {round_num} day {day_num}")
                 continue
 
-            parsed_days.append(day_data)
+            parsed_days.append((round_num, day_num))
         else:
             round_num = int(arg)
 
             parsed_days_in_round = []
             for day_num in range(-5, 6):
-                day_data = read_day_data(file_reader, round_num, day_num)
-                if day_data is not None:
-                    parsed_days_in_round.append(day_data)
+                if has_day_data(file_reader, round_num, day_num):
+                    parsed_days_in_round.append((round_num, day_num))
 
             if len(parsed_days_in_round) == 0:
                 print(f"Warning: no data found for round {round_num}")
                 continue
 
             parsed_days.extend(parsed_days_in_round)
 
@@ -69,14 +68,41 @@
 
     if no_out:
         return None
 
     timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
     return Path.cwd() / "backtests" / f"{timestamp}.log"
 
+def update_progress_bars(days: list[tuple[int, int]], queue: Queue) -> None:
+    bars = [tqdm(
+        desc=f"Round {round_num} day {day_num}",
+        position=i,
+        ascii=True,
+    ) for i, (round_num, day_num) in enumerate(days)]
+
+    completed = 0
+
+    while completed < len(days):
+        bar_id, operation, amount = queue.get()
+        bar = bars[bar_id]
+
+        if operation == "total":
+            bar.total = amount
+        elif operation == "update":
+            bar.n = amount
+            bar.refresh()
+
+            if bar.n == bar.total:
+                completed += 1
+
+    for bar in bars:
+        bar.close()
+
+    print()
+
 def print_day_summary(result: BacktestResult) -> None:
     last_timestamp = result.activity_logs[-1].timestamp
 
     product_lines = []
     total_profit = 0
 
     for row in reversed(result.activity_logs):
@@ -85,24 +111,28 @@
 
         product = row.columns[2]
         profit = row.columns[-1]
 
         product_lines.append(f"{product}: {profit:,.0f}")
         total_profit += profit
 
+    print(f"Round {result.round_num} day {result.day_num}:")
     print(*reversed(product_lines), sep="\n")
-    print(f"Total profit: {total_profit:,.0f}\n")
+    print(f"Total profit: {total_profit:,.0f}")
 
-def merge_results(a: BacktestResult, b: BacktestResult, merge_profit_loss: bool) -> BacktestResult:
+def merge_results(a: BacktestResult, b: BacktestResult, merge_profit_loss: bool, merge_timestamps: bool) -> BacktestResult:
     sandbox_logs = a.sandbox_logs[:]
     activity_logs = a.activity_logs[:]
     trades = a.trades[:]
 
-    a_last_timestamp = a.activity_logs[-1].timestamp
-    timestamp_offset = a_last_timestamp + 100
+    if merge_timestamps:
+        a_last_timestamp = a.activity_logs[-1].timestamp
+        timestamp_offset = a_last_timestamp + 100
+    else:
+        timestamp_offset = 0
 
     sandbox_logs.extend([row.with_offset(timestamp_offset) for row in b.sandbox_logs])
     trades.extend([row.with_offset(timestamp_offset) for row in b.trades])
 
     if merge_profit_loss:
         profit_loss_offsets = defaultdict(float)
         for row in reversed(a.activity_logs):
@@ -120,17 +150,18 @@
 
     return BacktestResult(a.round_num, a.day_num, sandbox_logs, activity_logs, trades)
 
 def write_output(output_file: Path, merged_results: BacktestResult) -> None:
     output_file.parent.mkdir(parents=True, exist_ok=True)
     with output_file.open("w+", encoding="utf-8") as file:
         file.write("Sandbox logs:\n")
-        file.write("\n".join(map(str, merged_results.sandbox_logs)))
+        for row in merged_results.sandbox_logs:
+            file.write(str(row))
 
-        file.write("\n\n\n\nActivities log:\n")
+        file.write("\n\n\nActivities log:\n")
         file.write("day;timestamp;product;bid_price_1;bid_volume_1;bid_price_2;bid_volume_2;bid_price_3;bid_volume_3;ask_price_1;ask_volume_1;ask_price_2;ask_volume_2;ask_price_3;ask_volume_3;mid_price;profit_and_loss\n")
         file.write("\n".join(map(str, merged_results.activity_logs)))
 
         file.write("\n\n\n\n\nTrade History:\n")
         file.write("[\n")
         file.write(",\n".join(map(str, merged_results.trades)))
         file.write("]")
@@ -189,57 +220,90 @@
     parser.add_argument("--out", type=str, help="path to save output log to (defaults to backtests/<timestamp>.log)")
     parser.add_argument("--data", type=str, help="path to data directory (must look similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources)")
     parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
     parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("--no-out", action="store_true", help="skip saving the output log to a file")
     parser.add_argument("--no-progress", action="store_true", help="don't show progress bars")
     parser.add_argument("--vis-requests", type=int, default=2, help="number of requests the visualizer is expected to make to the backtester's HTTP server when using --vis")
+    parser.add_argument("--original-timestamps", action="store_true", help="preserve original timestamps in output log rather than making them increase across days")
+    parser.add_argument("--max-workers", type=int, default=None, help="maximum number of worker processes to use")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     if args.vis and args.no_out:
         print("Error: --vis and --no-out are mutually exclusive")
         sys.exit(1)
 
     if args.out is not None and args.no_out:
         print("Error: --out and --no-out are mutually exclusive")
         sys.exit(1)
 
+    if args.max_workers is not None and args.max_workers < 1:
+        print("Error: --max-workers must be greater than 0")
+        sys.exit(1)
+
     try:
         trader_module = parse_algorithm(args.algorithm)
     except ModuleNotFoundError as e:
         print(f"{args.algorithm} is not a valid algorithm file: {e}")
         sys.exit(1)
 
     if not hasattr(trader_module, "Trader"):
         print(f"{args.algorithm} does not expose a Trader class")
         sys.exit(1)
 
-    days = parse_days(args.days, args.data)
+    file_reader = parse_data(args.data)
+    days = parse_days(file_reader, args.days)
     output_file = parse_out(args.out, args.no_out)
 
-    results = []
-    for day in days:
-        print(f"Backtesting {args.algorithm} on round {day.round_num} day {day.day_num}")
-
-        reload(trader_module)
-        trader = trader_module.Trader()
-
-        result = run_backtest(trader, day, args.print, args.no_trades_matching, args.no_progress)
-        print_day_summary(result)
-
-        results.append(result)
+    progress_queue = Manager().Queue()
 
-    merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
+    with ProcessPoolExecutor(args.max_workers) as executor:
+        show_progress_bars = not args.no_progress and not args.print and executor._max_workers > 1
+        show_live_results = args.print or executor._max_workers == 1
+
+        if show_progress_bars:
+            executor.submit(update_progress_bars, days, progress_queue)
+
+        futures = []
+        for i, (round_num, day_num) in enumerate(days):
+            future = executor.submit(
+                run_backtest,
+                trader_module.Trader(),
+                file_reader,
+                round_num,
+                day_num,
+                args.print,
+                args.no_trades_matching,
+                progress_queue,
+                i,
+            )
+
+            if show_live_results:
+                result = future.result()
+                print_day_summary(result)
+                if len(days) > 1:
+                    print()
+
+            futures.append(future)
+
+        results = [future.result() for future in futures]
+
+    if not show_live_results:
+        for result in results:
+            print_day_summary(result)
+            if len(days) > 1:
+                print()
 
     if len(days) > 1:
         print_overall_summary(results)
 
     if output_file is not None:
+        merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl, not args.original_timestamps), results)
         write_output(output_file, merged_results)
         print(f"\nSuccessfully saved backtest results to {format_path(output_file)}")
 
     if args.vis:
         open_visualizer(output_file, args.vis_requests)
 
 if __name__ == "__main__":
```

### Comparing `prosperity2bt-0.8.0/prosperity2bt/data.py` & `prosperity2bt-0.9.0/prosperity2bt/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,20 +46,25 @@
     day_num: int
 
     prices: dict[int, dict[Symbol, PriceRow]]
     trades: dict[int, dict[Symbol, list[Trade]]]
     products: list[Symbol]
     profit_loss: dict[Symbol, int]
 
+# We need to be able to pickle BacktestData for the multiprocessing module
+# defaultdict(<lambda>) does not support this because lambdas cannot be pickled
+def create_defaultdict_of_lists() -> dict:
+    return defaultdict(list)
+
 def create_backtest_data(round_num: int, day_num: int, prices: list[PriceRow], trades: list[Trade]) -> BacktestData:
     prices_by_timestamp: dict[int, dict[Symbol, PriceRow]] = defaultdict(dict)
     for row in prices:
         prices_by_timestamp[row.timestamp][row.product] = row
 
-    trades_by_timestamp: dict[int, dict[Symbol, list[Trade]]] = defaultdict(lambda: defaultdict(list))
+    trades_by_timestamp: dict[int, dict[Symbol, list[Trade]]] = defaultdict(create_defaultdict_of_lists)
     for trade in trades:
         trades_by_timestamp[trade.timestamp][trade.symbol].append(trade)
 
     products = sorted(set(row.product for row in prices))
     profit_loss = {product: 0 for product in products}
 
     return BacktestData(
@@ -67,14 +72,18 @@
         day_num=day_num,
         prices=prices_by_timestamp,
         trades=trades_by_timestamp,
         products=products,
         profit_loss=profit_loss,
     )
 
+def has_day_data(file_reader: FileReader, round_num: int, day_num: int) -> bool:
+    with file_reader.file([f"round{round_num}", f"prices_round_{round_num}_day_{day_num}.csv"]) as file:
+        return file is not None
+
 def read_day_data(file_reader: FileReader, round_num: int, day_num: int) -> Optional[BacktestData]:
     prices = []
     with file_reader.file([f"round{round_num}", f"prices_round_{round_num}_day_{day_num}.csv"]) as file:
         if file is None:
             return None
 
         for line in file.read_text(encoding="utf-8").splitlines()[1:]:
```

### Comparing `prosperity2bt-0.8.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.9.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/file_reader.py` & `prosperity2bt-0.9.0/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/models.py` & `prosperity2bt-0.9.0/prosperity2bt/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import orjson
 from dataclasses import dataclass
 from prosperity2bt.datamodel import Trade
 from typing import Any
 
 @dataclass
 class SandboxLogRow:
     timestamp: int
@@ -13,19 +13,19 @@
         return SandboxLogRow(
             self.timestamp + timestamp_offset,
             self.sandbox_log,
             self.lambda_log.replace(f"[[{self.timestamp},", f"[[{self.timestamp + timestamp_offset},"),
         )
 
     def __str__(self) -> str:
-        return json.dumps({
+        return orjson.dumps({
             "sandboxLog": self.sandbox_log,
             "lambdaLog": self.lambda_log,
             "timestamp": self.timestamp,
-        }, indent=2)
+        }, option=orjson.OPT_APPEND_NEWLINE | orjson.OPT_INDENT_2).decode("utf-8")
 
 @dataclass
 class ActivityLogRow:
     columns: list[Any]
 
     @property
     def timestamp(self) -> int:
```

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_-2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round1/trades_round_1_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_0_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round3/trades_round_3_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv` & `prosperity2bt-0.9.0/prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.8.0/prosperity2bt/runner.py` & `prosperity2bt-0.9.0/prosperity2bt/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 from contextlib import closing, redirect_stdout
 from io import StringIO
 from IPython.utils.io import Tee
-from prosperity2bt.data import BacktestData, LIMITS
+from multiprocessing import Queue
+from prosperity2bt.data import BacktestData, LIMITS, read_day_data
 from prosperity2bt.datamodel import Observation, Order, OrderDepth, Symbol, Trade, TradingState
+from prosperity2bt.file_reader import FileReader
 from prosperity2bt.models import ActivityLogRow, BacktestResult, MarketTrade, SandboxLogRow, TradeRow
-from tqdm import tqdm
 from typing import Any
 
 def prepare_state(state: TradingState, data: BacktestData) -> None:
     for product in data.products:
         order_depth = OrderDepth()
         row = data.prices[state.timestamp][product]
 
@@ -209,19 +211,27 @@
         remaining_market_trades = [t.trade for t in trades if t.trade.quantity > 0]
 
         state.market_trades[product] = remaining_market_trades
         result.trades.extend([TradeRow(trade) for trade in remaining_market_trades])
 
 def run_backtest(
     trader: Any,
-    data: BacktestData,
+    file_reader: FileReader,
+    round_num: int,
+    day_num: int,
     print_output: bool,
     disable_trades_matching: bool,
-    disable_progress_bar: bool,
+    progress_queue: Queue,
+    progress_id: int,
 ) -> BacktestResult:
+    data = read_day_data(file_reader, round_num, day_num)
+
+    os.environ["PROSPERITY2BT_ROUND"] = str(round_num)
+    os.environ["PROSPERITY2BT_DAY"] = str(day_num)
+
     trader_data = ""
     state = TradingState(
         traderData=trader_data,
         timestamp=0,
         listings={},
         order_depths={},
         own_trades={},
@@ -234,18 +244,18 @@
         round_num=data.round_num,
         day_num=data.day_num,
         sandbox_logs=[],
         activity_logs=[],
         trades=[],
     )
 
-    sorted_timestamps = sorted(data.prices.keys())
-    timestamps_iterator = sorted_timestamps if disable_progress_bar else tqdm(sorted_timestamps, ascii=True)
+    timestamps = sorted(data.prices.keys())
+    progress_queue.put_nowait([progress_id, "total", len(timestamps)])
 
-    for timestamp in timestamps_iterator:
+    for i, timestamp in enumerate(timestamps):
         state.timestamp = timestamp
         state.traderData = trader_data
 
         prepare_state(state, data)
 
         stdout = StringIO()
 
@@ -268,8 +278,11 @@
 
         result.sandbox_logs.append(sandbox_row)
 
         create_activity_logs(state, data, result)
         enforce_limits(state, data, orders, sandbox_row)
         match_orders(state, data, orders, result, disable_trades_matching)
 
+        if i % 100 == 0 or i == len(timestamps) - 1:
+            progress_queue.put_nowait([progress_id, "update", i + 1])
+
     return result
```

### Comparing `prosperity2bt-0.8.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.9.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jsonpickle
+Requires-Dist: orjson
 Requires-Dist: tqdm
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
```

### Comparing `prosperity2bt-0.8.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.9.0/prosperity2bt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -43,8 +43,18 @@
 prosperity2bt/resources/round4/prices_round_4_day_2.csv
 prosperity2bt/resources/round4/prices_round_4_day_3.csv
 prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
 prosperity2bt/resources/round4/trades_round_4_day_1_wn.csv
 prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
 prosperity2bt/resources/round4/trades_round_4_day_2_wn.csv
 prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
-prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
+prosperity2bt/resources/round4/trades_round_4_day_3_wn.csv
+prosperity2bt/resources/round6/prices_round_6_day_0.csv
+prosperity2bt/resources/round6/prices_round_6_day_1.csv
+prosperity2bt/resources/round6/prices_round_6_day_2.csv
+prosperity2bt/resources/round6/prices_round_6_day_3.csv
+prosperity2bt/resources/round6/prices_round_6_day_4.csv
+prosperity2bt/resources/round6/prices_round_6_day_5.csv
+prosperity2bt/resources/round7/prices_round_7_day_1.csv
+prosperity2bt/resources/round7/prices_round_7_day_2.csv
+prosperity2bt/resources/round7/prices_round_7_day_3.csv
+prosperity2bt/resources/round7/prices_round_7_day_4.csv
```

### Comparing `prosperity2bt-0.8.0/pyproject.toml` & `prosperity2bt-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.8.0"
+version = "0.9.0"
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
-dependencies = ["ipython", "jsonpickle", "tqdm"]
+dependencies = ["ipython", "jsonpickle", "orjson", "tqdm"]
 
 [project.scripts]
 prosperity2bt = "prosperity2bt.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/jmerle/imc-prosperity-2-backtester"
 Issues = "https://github.com/jmerle/imc-prosperity-2-backtester/issues"
```

