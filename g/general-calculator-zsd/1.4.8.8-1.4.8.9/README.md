# Comparing `tmp/general_calculator_zsd-1.4.8.8.tar.gz` & `tmp/general_calculator_zsd-1.4.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_calculator_zsd-1.4.8.8.tar", last modified: Mon Feb 26 03:07:41 2024, max compression
+gzip compressed data, was "general_calculator_zsd-1.4.8.9.tar", last modified: Mon Feb 26 05:15:57 2024, max compression
```

## Comparing `general_calculator_zsd-1.4.8.8.tar` & `general_calculator_zsd-1.4.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 03:07:41.504890 general_calculator_zsd-1.4.8.8/
--rw-rw-rw-   0        0        0      424 2024-02-26 03:07:41.503893 general_calculator_zsd-1.4.8.8/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-02-23 09:01:36.000000 general_calculator_zsd-1.4.8.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 03:07:41.473973 general_calculator_zsd-1.4.8.8/general_calculator_zsd/
--rw-rw-rw-   0        0        0        0 2022-11-16 09:26:24.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd/__init__.py
--rw-rw-rw-   0        0        0    53199 2023-11-17 08:46:37.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd/general_calculator.py
--rw-rw-rw-   0        0        0    80378 2024-02-26 03:02:30.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd/mysql_transmit_data4all.py
-drwxrwxrwx   0        0        0        0 2024-02-26 03:07:41.500899 general_calculator_zsd-1.4.8.8/general_calculator_zsd.egg-info/
--rw-rw-rw-   0        0        0      424 2024-02-26 03:07:41.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-02-26 03:07:41.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 03:07:41.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-02-26 03:07:41.000000 general_calculator_zsd-1.4.8.8/general_calculator_zsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 03:07:41.504890 general_calculator_zsd-1.4.8.8/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-02-26 03:07:35.000000 general_calculator_zsd-1.4.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-26 05:15:57.214395 general_calculator_zsd-1.4.8.9/
+-rw-rw-rw-   0        0        0      424 2024-02-26 05:15:57.213397 general_calculator_zsd-1.4.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-02-23 09:01:36.000000 general_calculator_zsd-1.4.8.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-26 05:15:57.201429 general_calculator_zsd-1.4.8.9/general_calculator_zsd/
+-rw-rw-rw-   0        0        0        0 2022-11-16 09:26:24.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd/__init__.py
+-rw-rw-rw-   0        0        0    53199 2023-11-17 08:46:37.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd/general_calculator.py
+-rw-rw-rw-   0        0        0    80373 2024-02-26 05:14:50.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd/mysql_transmit_data4all.py
+drwxrwxrwx   0        0        0        0 2024-02-26 05:15:57.212401 general_calculator_zsd-1.4.8.9/general_calculator_zsd.egg-info/
+-rw-rw-rw-   0        0        0      424 2024-02-26 05:15:57.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-02-26 05:15:57.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-26 05:15:57.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-02-26 05:15:57.000000 general_calculator_zsd-1.4.8.9/general_calculator_zsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-26 05:15:57.214395 general_calculator_zsd-1.4.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-02-26 05:15:53.000000 general_calculator_zsd-1.4.8.9/setup.py
```

### Comparing `general_calculator_zsd-1.4.8.8/README.md` & `general_calculator_zsd-1.4.8.9/README.md`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.4.8.8/general_calculator_zsd/general_calculator.py` & `general_calculator_zsd-1.4.8.9/general_calculator_zsd/general_calculator.py`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.4.8.8/general_calculator_zsd/mysql_transmit_data4all.py` & `general_calculator_zsd-1.4.8.9/general_calculator_zsd/mysql_transmit_data4all.py`

 * *Files 0% similar despite different names*

```diff
@@ -1169,15 +1169,15 @@
         insert_data["user_id"] = json_data["user_id"]
         insert_data["user_nickname"] = json_data["user_name"]
         # insert_data["user_gender"] = json_data["user_gender"]
         insert_data["user_country"] = json_data["user_country"]
         insert_data["user_province"] = json_data["user_province"]
         # insert_data["user_city"] = json_data["user_city"]
         # insert_data["user_work"] = json_data["user_work"]
-        insert_data["user_summary"] = json_data["user_summary"]
+        insert_data["user_summary"] = json_data["summary"]
         # insert_data["verified_flag"] = json_data["verified_flag"]
         # insert_data["verified_reason"] = json_data["verified_reason"]
         # insert_data["user_post_count"] = json_data["note_count"]
         # insert_data["following_count"] = json_data["following_count"]
         # insert_data["follower_count"] = json_data["follower_count"]
         # insert_data["user_level"] = json_data["level"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
```

