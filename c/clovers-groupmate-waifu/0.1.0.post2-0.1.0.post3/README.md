# Comparing `tmp/clovers_groupmate_waifu-0.1.0.post2.tar.gz` & `tmp/clovers_groupmate_waifu-0.1.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_groupmate_waifu-0.1.0.post2.tar", max compression
+gzip compressed data, was "clovers_groupmate_waifu-0.1.0.post3.tar", max compression
```

## Comparing `clovers_groupmate_waifu-0.1.0.post2.tar` & `clovers_groupmate_waifu-0.1.0.post3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14844 2024-04-23 13:29:58.828804 clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-23 16:19:41.580219 clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/clovers.py
--rw-r--r--   0        0        0     2696 2024-04-23 10:14:52.156708 clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/config.py
--rw-r--r--   0        0        0     1763 2024-04-23 04:39:50.328249 clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/data.py
--rw-r--r--   0        0        0      627 2024-04-19 18:04:26.925322 clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/utils.py
--rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 clovers_groupmate_waifu-0.1.0.post2/LICENSE
--rw-r--r--   0        0        0      391 2024-04-23 16:18:21.944939 clovers_groupmate_waifu-0.1.0.post2/pyproject.toml
--rw-r--r--   0        0        0     3209 2023-11-06 04:36:06.281170 clovers_groupmate_waifu-0.1.0.post2/README.md
--rw-r--r--   0        0        0     3479 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    14844 2024-04-23 13:29:58.828804 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-23 16:19:41.580219 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/clovers.py
+-rw-r--r--   0        0        0     2696 2024-04-23 10:14:52.156708 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/config.py
+-rw-r--r--   0        0        0     1763 2024-04-23 04:39:50.328249 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/data.py
+-rw-r--r--   0        0        0      627 2024-04-19 18:04:26.925322 clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/utils.py
+-rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 clovers_groupmate_waifu-0.1.0.post3/LICENSE
+-rw-r--r--   0        0        0      391 2024-04-23 16:43:50.889424 clovers_groupmate_waifu-0.1.0.post3/pyproject.toml
+-rw-r--r--   0        0        0     3209 2023-11-06 04:36:06.281170 clovers_groupmate_waifu-0.1.0.post3/README.md
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 clovers_groupmate_waifu-0.1.0.post3/PKG-INFO
```

### Comparing `clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/__init__.py` & `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/clovers.py` & `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/config.py` & `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/config.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/data.py` & `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/data.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/clovers_groupmate_waifu/utils.py` & `clovers_groupmate_waifu-0.1.0.post3/clovers_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/LICENSE` & `clovers_groupmate_waifu-0.1.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/README.md` & `clovers_groupmate_waifu-0.1.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `clovers_groupmate_waifu-0.1.0.post2/PKG-INFO` & `clovers_groupmate_waifu-0.1.0.post3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: clovers-groupmate-waifu
-Version: 0.1.0.post2
+Version: 0.1.0.post3
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
 Requires-Dist: clovers[linecard,tools] (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.0.post2
+Metadata-Version: 2.1 Name: clovers-groupmate-waifu Version: 0.1.0.post3
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
->=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Requires-Dist:
-clovers-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers[linecard,tools]
-(>=0.1.4,<0.2.0) Description-Content-Type: text/markdown
+>=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0) Requires-
+Dist: clovers[linecard,tools] (>=0.1.4,<0.2.0) Description-Content-Type: text/
+markdown
                                    _[_n_o_n_e_b_o_t_]
                   # nonebot_plugin_groupmate_waifu å¨¶ç¾¤å
 ## éè¦å®è£ [pil-utils](https://github.com/MeetWq/pil-utils)
 PILå·¥å·æä»¶ï¼æ¹ä¾¿å¾çæä½ï¼æ¯ææå­è½¬å¾ç
 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)
 APScheduler å®æ¶ä»»å¡æä»¶ ## å®è£ pip install
 nonebot_plugin_groupmate_waifu ## ä½¿ç¨ nonebot.load_plugin
```

