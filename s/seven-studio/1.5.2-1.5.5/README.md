# Comparing `tmp/seven_studio-1.5.2.tar.gz` & `tmp/seven_studio-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_studio-1.5.2.tar", last modified: Thu Oct 19 09:06:00 2023, max compression
+gzip compressed data, was "dist/seven_studio-1.5.5.tar", last modified: Tue Apr 23 02:58:41 2024, max compression
```

## Comparing `seven_studio-1.5.2.tar` & `seven_studio-1.5.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.286006 seven_studio-1.5.2/
--rw-r--r--   0 root         (0) root         (0)     3171 2023-10-19 09:06:00.286006 seven_studio-1.5.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1664 2023-10-19 09:04:44.000000 seven_studio-1.5.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-19 09:06:00.286006 seven_studio-1.5.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1262 2023-10-19 09:04:44.000000 seven_studio-1.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.255006 seven_studio-1.5.2/seven_studio/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.258006 seven_studio-1.5.2/seven_studio/handlers/
--rwxrwxrwx   0 root         (0) root         (0)      132 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26840 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/studio_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.262006 seven_studio-1.5.2/seven_studio/handlers/system/
--rwxrwxrwx   0 root         (0) root         (0)      224 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9452 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/core.py
--rwxrwxrwx   0 root         (0) root         (0)    22072 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/file.py
--rwxrwxrwx   0 root         (0) root         (0)    17655 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/menu.py
--rwxrwxrwx   0 root         (0) root         (0)    32373 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/power.py
--rwxrwxrwx   0 root         (0) root         (0)     6678 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/product.py
--rwxrwxrwx   0 root         (0) root         (0)     2636 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/handlers/system/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.263006 seven_studio-1.5.2/seven_studio/libs/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.267006 seven_studio-1.5.2/seven_studio/libs/file/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8612 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/bos.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/cos.py
--rwxrwxrwx   0 root         (0) root         (0)    19074 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/ks3.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/oss2.py
--rwxrwxrwx   0 root         (0) root         (0)     8593 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/s3.py
--rwxrwxrwx   0 root         (0) root         (0)    14037 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/file/upload.py
--rwxrwxrwx   0 root         (0) root         (0)     6306 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/libs/geetest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.269006 seven_studio-1.5.2/seven_studio/models/
--rwxrwxrwx   0 root         (0) root         (0)      180 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.270006 seven_studio-1.5.2/seven_studio/models/db_models/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.273006 seven_studio-1.5.2/seven_studio/models/db_models/file/
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1492 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_history_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_resource_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2433 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_restrict_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_restrict_pic_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1451 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_storage_path_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/file/file_water_image_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.274006 seven_studio-1.5.2/seven_studio/models/db_models/log/
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/log/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1298 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/log/log_action_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.276006 seven_studio-1.5.2/seven_studio/models/db_models/menu/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/menu/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1583 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_cote_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2174 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)    19404 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_info_model_ex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.278006 seven_studio-1.5.2/seven_studio/models/db_models/product/
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/product/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/product/product_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/product/product_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.280006 seven_studio-1.5.2/seven_studio/models/db_models/role/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/role/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/role/role_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1014 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/role/role_power_model.py
--rwxrwxrwx   0 root         (0) root         (0)      952 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/role/role_power_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/role/role_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.282006 seven_studio-1.5.2/seven_studio/models/db_models/settings/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/settings/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/settings/settings_base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.283006 seven_studio-1.5.2/seven_studio/models/db_models/user/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/user/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2025 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/user/user_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/user/user_info_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1035 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/db_models/user/user_login_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/dto_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/enum.py
--rwxrwxrwx   0 root         (0) root         (0)    37633 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/power_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2689 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/models/seven_model.py
--rwxrwxrwx   0 root         (0) root         (0)     4391 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.285006 seven_studio-1.5.2/seven_studio/utils/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1959 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/utils/dict.py
--rwxrwxrwx   0 root         (0) root         (0)      637 2023-10-19 09:04:44.000000 seven_studio-1.5.2/seven_studio/utils/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 09:06:00.258006 seven_studio-1.5.2/seven_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3171 2023-10-19 09:05:59.000000 seven_studio-1.5.2/seven_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2636 2023-10-19 09:06:00.000000 seven_studio-1.5.2/seven_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-19 09:05:59.000000 seven_studio-1.5.2/seven_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-10-19 09:05:59.000000 seven_studio-1.5.2/seven_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-19 09:05:59.000000 seven_studio-1.5.2/seven_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.045914 seven_studio-1.5.5/
+-rw-r--r--   0 root         (0) root         (0)     3251 2024-04-23 02:58:41.045914 seven_studio-1.5.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1720 2024-04-23 02:46:57.000000 seven_studio-1.5.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 02:58:41.045914 seven_studio-1.5.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1262 2024-04-23 02:46:57.000000 seven_studio-1.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.037914 seven_studio-1.5.5/seven_studio/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.038914 seven_studio-1.5.5/seven_studio/handlers/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26840 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/studio_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.039914 seven_studio-1.5.5/seven_studio/handlers/system/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9452 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    22072 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/file.py
+-rwxrwxrwx   0 root         (0) root         (0)    17655 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/menu.py
+-rwxrwxrwx   0 root         (0) root         (0)    32373 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/power.py
+-rwxrwxrwx   0 root         (0) root         (0)     6678 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/product.py
+-rwxrwxrwx   0 root         (0) root         (0)     2636 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/handlers/system/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.039914 seven_studio-1.5.5/seven_studio/libs/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.040914 seven_studio-1.5.5/seven_studio/libs/file/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8612 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/bos.py
+-rwxrwxrwx   0 root         (0) root         (0)     8613 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/cos.py
+-rwxrwxrwx   0 root         (0) root         (0)    19074 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/ks3.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/oss2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8593 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/s3.py
+-rwxrwxrwx   0 root         (0) root         (0)    14037 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/file/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6306 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/libs/geetest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.041914 seven_studio-1.5.5/seven_studio/models/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.041914 seven_studio-1.5.5/seven_studio/models/db_models/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.042914 seven_studio-1.5.5/seven_studio/models/db_models/file/
+-rwxrwxrwx   0 root         (0) root         (0)      308 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_history_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_resource_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2433 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_restrict_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_restrict_pic_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1451 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_storage_path_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/file/file_water_image_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.042914 seven_studio-1.5.5/seven_studio/models/db_models/log/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/log/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/log/log_action_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.043914 seven_studio-1.5.5/seven_studio/models/db_models/menu/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/menu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_cote_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2174 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    19404 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_info_model_ex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.043914 seven_studio-1.5.5/seven_studio/models/db_models/product/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/product/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/product/product_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/product/product_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.044914 seven_studio-1.5.5/seven_studio/models/db_models/role/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/role/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/role/role_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1014 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/role/role_power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      952 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/role/role_power_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/role/role_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.044914 seven_studio-1.5.5/seven_studio/models/db_models/settings/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/settings/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/settings/settings_base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.044914 seven_studio-1.5.5/seven_studio/models/db_models/user/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/user/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/user/user_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/user/user_info_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1035 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/db_models/user/user_login_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/dto_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/enum.py
+-rwxrwxrwx   0 root         (0) root         (0)    37640 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/models/seven_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.045914 seven_studio-1.5.5/seven_studio/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1959 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/utils/dict.py
+-rwxrwxrwx   0 root         (0) root         (0)      637 2024-04-23 02:36:20.000000 seven_studio-1.5.5/seven_studio/utils/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:58:41.038914 seven_studio-1.5.5/seven_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3251 2024-04-23 02:58:40.000000 seven_studio-1.5.5/seven_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-23 02:58:41.000000 seven_studio-1.5.5/seven_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 02:58:40.000000 seven_studio-1.5.5/seven_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-23 02:58:40.000000 seven_studio-1.5.5/seven_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-23 02:58:40.000000 seven_studio-1.5.5/seven_studio.egg-info/top_level.txt
```

### Comparing `seven_studio-1.5.2/PKG-INFO` & `seven_studio-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_studio
-Version: 1.5.2
+Version: 1.5.5
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: <!--
          * @Author: ChenXiaolei
@@ -13,14 +13,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.5.5 更新内容
+        * 栏目条件挂载缺少where
+        
         ### 1.5.2 更新内容
         * 限制弱密码输入
         
         ### 1.5.0 更新内容
         * 修改登录过滤器login_filter
         
         ### 1.4.0 更新内容
```

### Comparing `seven_studio-1.5.2/README.md` & `seven_studio-1.5.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 # seven_studio
 
 ## 天志互联Python公共基础后台管理平台
 
+### 1.5.5 更新内容
+* 栏目条件挂载缺少where
+
 ### 1.5.2 更新内容
 * 限制弱密码输入
 
 ### 1.5.0 更新内容
 * 修改登录过滤器login_filter
 
 ### 1.4.0 更新内容
```

### Comparing `seven_studio-1.5.2/setup.py` & `seven_studio-1.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_studio",
-    version="1.5.2",
+    version="1.5.5",
     author="seven",
     author_email="tech@gao7.com",
     description="seven studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_studio",
```

### Comparing `seven_studio-1.5.2/seven_studio/handlers/studio_base.py` & `seven_studio-1.5.5/seven_studio/handlers/studio_base.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/core.py` & `seven_studio-1.5.5/seven_studio/handlers/system/core.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/file.py` & `seven_studio-1.5.5/seven_studio/handlers/system/file.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/menu.py` & `seven_studio-1.5.5/seven_studio/handlers/system/menu.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/power.py` & `seven_studio-1.5.5/seven_studio/handlers/system/power.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/product.py` & `seven_studio-1.5.5/seven_studio/handlers/system/product.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/handlers/system/settings.py` & `seven_studio-1.5.5/seven_studio/handlers/system/settings.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/bos.py` & `seven_studio-1.5.5/seven_studio/libs/file/bos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/cos.py` & `seven_studio-1.5.5/seven_studio/libs/file/cos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/ks3.py` & `seven_studio-1.5.5/seven_studio/libs/file/ks3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/oss2.py` & `seven_studio-1.5.5/seven_studio/libs/file/oss2.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/s3.py` & `seven_studio-1.5.5/seven_studio/libs/file/s3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/file/upload.py` & `seven_studio-1.5.5/seven_studio/libs/file/upload.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/libs/geetest.py` & `seven_studio-1.5.5/seven_studio/libs/geetest.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_history_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_history_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_resource_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_resource_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_restrict_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_restrict_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_restrict_pic_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_restrict_pic_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_storage_path_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_storage_path_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/file/file_water_image_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/file/file_water_image_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/log/log_action_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/log/log_action_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_cote_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_cote_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_info_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/menu/menu_info_model_ex.py` & `seven_studio-1.5.5/seven_studio/models/db_models/menu/menu_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/product/product_info_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/product/product_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/product/product_user_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/product/product_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/role/role_info_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/role/role_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/role/role_power_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/role/role_power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/role/role_power_model_ex.py` & `seven_studio-1.5.5/seven_studio/models/db_models/role/role_power_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/role/role_user_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/role/role_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/settings/settings_base_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/settings/settings_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/user/user_info_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/user/user_info_model_ex.py` & `seven_studio-1.5.5/seven_studio/models/db_models/user/user_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/db_models/user/user_login_model.py` & `seven_studio-1.5.5/seven_studio/models/db_models/user/user_login_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/dto_model.py` & `seven_studio-1.5.5/seven_studio/models/dto_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/enum.py` & `seven_studio-1.5.5/seven_studio/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/models/power_model.py` & `seven_studio-1.5.5/seven_studio/models/power_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         if menu_cote.IDPathName.strip() != "":
             field_parms += f",{menu_cote.IDPathName}"
 
         condition = ""
         if menu_cote.Condtion.strip() == "":
             condition = f" ORDER BY {menu_cote.SortExpression}"
         else:
-            condition = f"{menu_cote.Condtion} ORDER BY {menu_cote.SortExpression}"
+            condition = f" WHERE {menu_cote.Condtion} ORDER BY {menu_cote.SortExpression}"
 
         sql = f"SELECT {field_parms} FROM {menu_cote.CoteTableName}{condition}"
         return MySQLHelper(config.get_value(menu_cote.ConnectionStringName)).fetch_all_rows(sql)
 
     def __check_menu_power(self, is_power, menu_id, cote_id):
         """
         :description: 菜单权限判断
```

### Comparing `seven_studio-1.5.2/seven_studio/models/seven_model.py` & `seven_studio-1.5.5/seven_studio/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/route.py` & `seven_studio-1.5.5/seven_studio/route.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/utils/dict.py` & `seven_studio-1.5.5/seven_studio/utils/dict.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio/utils/random.py` & `seven_studio-1.5.5/seven_studio/utils/random.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.5.2/seven_studio.egg-info/PKG-INFO` & `seven_studio-1.5.5/seven_studio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-studio
-Version: 1.5.2
+Version: 1.5.5
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: <!--
          * @Author: ChenXiaolei
@@ -13,14 +13,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.5.5 更新内容
+        * 栏目条件挂载缺少where
+        
         ### 1.5.2 更新内容
         * 限制弱密码输入
         
         ### 1.5.0 更新内容
         * 修改登录过滤器login_filter
         
         ### 1.4.0 更新内容
```

### Comparing `seven_studio-1.5.2/seven_studio.egg-info/SOURCES.txt` & `seven_studio-1.5.5/seven_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

