# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.25.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.25.tar", last modified: Thu Apr 18 19:05:24 2024, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.26.tar", last modified: Tue Apr 23 00:59:47 2024, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.25.tar` & `nonebot_plugin_simulator_xiuxian-0.5.26.tar`

### file list

```diff
@@ -1,25 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.225834 nonebot_plugin_simulator_xiuxian-0.5.25/
--rw-rw-rw-   0        0        0      265 2024-04-18 19:05:24.225834 nonebot_plugin_simulator_xiuxian-0.5.25/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.208930 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0     2040 2024-04-17 16:39:11.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/cd_manager.py
--rw-rw-rw-   0        0        0      358 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/config.py
--rw-rw-rw-   0        0        0     2849 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/data_source.py
--rw-rw-rw-   0        0        0     1787 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/exp_util.py
--rw-rw-rw-   0        0        0     1354 2024-04-18 19:00:35.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/help.py
--rw-rw-rw-   0        0        0     4430 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/item_json.py
--rw-rw-rw-   0        0        0    50728 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/player_fight.py
--rw-rw-rw-   0        0        0     8141 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/read_buff.py
--rw-rw-rw-   0        0        0     8555 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/utils.py
--rw-rw-rw-   0        0        0    54291 2024-04-18 18:05:50.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
--rw-rw-rw-   0        0        0     5780 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
--rw-rw-rw-   0        0        0      787 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
--rw-rw-rw-   0        0        0     2477 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.224834 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0      265 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      951 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 19:05:24.226836 nonebot_plugin_simulator_xiuxian-0.5.25/setup.cfg
--rw-rw-rw-   0        0        0      593 2024-04-18 19:04:58.000000 nonebot_plugin_simulator_xiuxian-0.5.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:59:47.294168 nonebot_plugin_simulator_xiuxian-0.5.26/
+-rw-rw-rw-   0        0        0     5386 2024-04-23 00:59:47.294168 nonebot_plugin_simulator_xiuxian-0.5.26/PKG-INFO
+-rw-rw-rw-   0        0        0     4958 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.26/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 00:59:47.277166 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0      175 2024-04-22 23:40:10.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:59:47.293168 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0     5386 2024-04-23 00:59:47.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-23 00:59:47.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 00:59:47.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-04-23 00:59:47.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-23 00:59:47.000000 nonebot_plugin_simulator_xiuxian-0.5.26/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-23 00:59:47.295168 nonebot_plugin_simulator_xiuxian-0.5.26/setup.cfg
+-rw-rw-rw-   0        0        0      980 2024-04-23 00:59:43.000000 nonebot_plugin_simulator_xiuxian-0.5.26/setup.py
```

