# Comparing `tmp/nonebot_plugin_game_collection-3.0.2.tar.gz` & `tmp/nonebot_plugin_game_collection-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-3.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_game_collection-3.0.3.tar", max compression
```

## Comparing `nonebot_plugin_game_collection-3.0.2.tar` & `nonebot_plugin_game_collection-3.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.2/LICENSE
--rw-r--r--   0        0        0      931 2024-04-16 11:46:27.481877 nonebot_plugin_game_collection-3.0.2/nonebot_plugin_game_collection/__init__.py
--rw-r--r--   0        0        0      362 2024-04-16 11:49:48.962958 nonebot_plugin_game_collection-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.2/README.md
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.3/LICENSE
+-rw-r--r--   0        0        0      931 2024-04-16 11:46:27.481877 nonebot_plugin_game_collection-3.0.3/nonebot_plugin_game_collection/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-23 16:24:35.218578 nonebot_plugin_game_collection-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.3/README.md
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_game_collection-3.0.2/LICENSE` & `nonebot_plugin_game_collection-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.2/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-3.0.3/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.2/README.md` & `nonebot_plugin_game_collection-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.2/PKG-INFO` & `nonebot_plugin_game_collection-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-game-collection
-Version: 3.0.2
+Version: 3.0.3
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers-leafgame (>=0.1.2,<0.2.0)
-Requires-Dist: nonebot-plugin-clovers (>=0.1.2,<0.2.0)
+Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0)
+Requires-Dist: nonebot-plugin-clovers[onebot] (==0.1.2r2)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.2
+Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.3
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: clovers-leafgame (>=0.1.2,<0.2.0) Requires-Dist:
-nonebot-plugin-clovers (>=0.1.2,<0.2.0) Description-Content-Type: text/markdown
+Python :: 3.11 Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0) Requires-Dist:
+nonebot-plugin-clovers[onebot] (==0.1.2r2) Description-Content-Type: text/
+markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # nonebot-plugin-game-collection _â¨ æ¹èª [nonebot_plugin_russian](https://
   github.com/HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace]
 (https://github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
```

