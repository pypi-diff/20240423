# Comparing `tmp/mobio-media-sdk-0.2.8.tar.gz` & `tmp/mobio-media-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-media-sdk-0.2.8.tar", last modified: Fri Jan 13 02:12:03 2023, max compression
+gzip compressed data, was "mobio-media-sdk-0.2.9.tar", last modified: Wed Apr  5 08:31:59 2023, max compression
```

## Comparing `mobio-media-sdk-0.2.8.tar` & `mobio-media-sdk-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 tungdd     (502) staff       (20)        0 2023-01-13 02:12:03.696555 mobio-media-sdk-0.2.8/
--rwxr-xr-x   0 tungdd     (502) staff       (20)     1073 2021-07-08 08:00:49.000000 mobio-media-sdk-0.2.8/LICENSE
--rw-r--r--   0 tungdd     (502) staff       (20)     3454 2023-01-13 02:12:03.696705 mobio-media-sdk-0.2.8/PKG-INFO
--rwxr-xr-x   0 tungdd     (502) staff       (20)       82 2021-09-07 21:54:01.000000 mobio-media-sdk-0.2.8/README.md
-drwxr-xr-x   0 tungdd     (502) staff       (20)        0 2023-01-13 02:12:03.683956 mobio-media-sdk-0.2.8/mobio/
-drwxr-xr-x   0 tungdd     (502) staff       (20)        0 2023-01-13 02:12:03.684077 mobio-media-sdk-0.2.8/mobio/sdks/
-drwxr-xr-x   0 tungdd     (502) staff       (20)        0 2023-01-13 02:12:03.693029 mobio-media-sdk-0.2.8/mobio/sdks/media/
--rwxr-xr-x   0 tungdd     (502) staff       (20)        0 2021-07-08 08:00:49.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/__init__.py
--rwxr-xr-x   0 tungdd     (502) staff       (20)     1737 2022-01-14 11:39:45.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/config.py
--rw-r--r--   0 tungdd     (502) staff       (20)     4351 2022-07-03 23:33:21.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/constant.py
--rw-r--r--   0 tungdd     (502) staff       (20)    38208 2021-09-10 10:18:59.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/custom_mimetypes.py
--rwxr-xr-x   0 tungdd     (502) staff       (20)      338 2021-07-08 08:00:49.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/dir.py
--rw-r--r--   0 tungdd     (502) staff       (20)     2419 2022-11-11 14:14:51.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/merchant_config.py
--rwxr-xr-x   0 tungdd     (502) staff       (20)    20755 2023-01-13 01:55:46.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/mobio_media_sdk.py
--rw-r--r--   0 tungdd     (502) staff       (20)     1083 2022-11-11 14:14:51.000000 mobio-media-sdk-0.2.8/mobio/sdks/media/utils.py
-drwxr-xr-x   0 tungdd     (502) staff       (20)        0 2023-01-13 02:12:03.695979 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/
--rw-r--r--   0 tungdd     (502) staff       (20)     3454 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/PKG-INFO
--rw-r--r--   0 tungdd     (502) staff       (20)      537 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 tungdd     (502) staff       (20)        1 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 tungdd     (502) staff       (20)        6 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 tungdd     (502) staff       (20)       98 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/requires.txt
--rw-r--r--   0 tungdd     (502) staff       (20)        6 2023-01-13 02:12:03.000000 mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/top_level.txt
--rwxr-xr-x   0 tungdd     (502) staff       (20)      104 2021-07-08 08:00:49.000000 mobio-media-sdk-0.2.8/pyproject.toml
--rwxr-xr-x   0 tungdd     (502) staff       (20)       38 2023-01-13 02:12:03.697249 mobio-media-sdk-0.2.8/setup.cfg
--rwxr-xr-x   0 tungdd     (502) staff       (20)     9113 2023-01-13 02:11:56.000000 mobio-media-sdk-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:31:59.886800 mobio-media-sdk-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-04-05 08:31:59.887800 mobio-media-sdk-0.2.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     2650 2023-04-05 08:26:46.000000 mobio-media-sdk-0.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:31:59.869799 mobio-media-sdk-0.2.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:31:59.869799 mobio-media-sdk-0.2.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:31:59.880800 mobio-media-sdk-0.2.9/mobio/sdks/media/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1737 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/config.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/constant.py
+-rw-r--r--   0 root         (0) root         (0)    38208 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/custom_mimetypes.py
+-rwxr-xr-x   0 root         (0) root         (0)      338 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/dir.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/merchant_config.py
+-rwxr-xr-x   0 root         (0) root         (0)    20755 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/mobio_media_sdk.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/mobio/sdks/media/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:31:59.885800 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      104 2023-04-05 07:33:40.000000 mobio-media-sdk-0.2.9/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-04-05 08:31:59.888800 mobio-media-sdk-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9320 2023-04-05 08:31:59.000000 mobio-media-sdk-0.2.9/setup.py
```

### Comparing `mobio-media-sdk-0.2.8/PKG-INFO` & `mobio-media-sdk-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 Metadata-Version: 2.1
 Name: mobio-media-sdk
-Version: 0.2.8
-Summary: Mobio media SDK
+Version: 0.2.9
+Summary: Mobio Media SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Keywords: mobio,media,file
+Description: ##  Thư viện Media.
+        
+        ### Cài đặt:
+        
+        ```bash
+         $ pip3 install mobio-media-sdk
+         ```
+        
+        #### Log:
+        
+        - Version: 0.1.1: Thêm mobio token.
+        - Version: 0.1.2: Add json.dums by func finish_save_file_by_filepath
+        - Version: 0.1.3: Add func get_path_by_url, get_binary_by_url
+            + Hướng dẫn sử dụng:
+                + func get_path_by_url -> kết quả trả về là path của url.
+                  ```python3
+                  from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+                  MobioMediaSDK().get_path_by_url(url)
+                  ```
+                + func get_binary_by_url -> kết quả trả về là binary của url
+                  ```python3
+                  from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+                  MobioMediaSDK().get_binary_by_url(url)
+                  ```
+        - Version: 0.1.4: Add func get_filename_by_url
+          + Hướng dẫn sử dụng:
+            + func get_filename_by_url -> kết quả trả về là filename của url
+              ```python3
+              from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+              MobioMediaSDK().get_filename_by_url(url)
+              ```
+        - Version: 0.1.5: Delete system_config
+        - Version: 0.1.6: Rename get_local_path_by_url -> get_path_by_url
+        - Version: 0.1.7: Option read file "r" -> "rb"
+        - Version: 0.1.8: Update lại token call từ Admin
+        - Version: 0.1.9: Bổ sung tính năng:
+          - Tạo public link khi chưa có file upload.
+              ```python3
+              from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+              MobioMediaSDK().create_public_url_without_file(
+                    merchant_id="merchant_id",
+                    filename="filename",
+                    mimetype_str="mimetype_str"
+              )
+        
+              result = {
+                'url': '',
+                'local_path': '',
+                'filename': ''
+              }
+              ```
+              Sau khi xử lý nghiệp vụ xong có thể dùng func sau để Lưu file được lấy path từ URL
+              ```python3
+               from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+               MobioMediaSDK().finish_save_file_by_public_url(filepath="filepath", url="url")
+              ```
+          - Thêm option **file_byte** khi upload file. Option này phục vụ cho nhu cầu upload file bằng bytes.
+        
+        - Version: 0.2.0: Bổ sung option display, group_ids
+        - Version: 0.2.1: Bổ sung merchant_id
+        - Version: 0.2.2: Sửa từ get public-host từ module media sang module Admin.
+        - Version: 0.2.2 và 0.2.3: Bổ sung phần tính dung lượng file khi trả về.
+        - Version: 0.2.5: Chuyển việc lấy public-host sang admin-sdk
+        - Version: 0.2.6: Apply libs m-kafka-sdk-v2
+        - Version: 0.2.7: Bỏ m-kafka-sdk
+        - Version: 0.2.8: Fix lỗi encode url với những tên file đặc biệt
+        - Version: 0.2.9: Nâng cấp confluent_kafka
+        
+Keywords: mobio,media,upload
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-##  Thư viện Media.
-
-### Cài đặt:
-
-```bash
- $ pip3 install mobio-media-sdk
- ```
-
-#### Log:
-
-- Version: 0.1.1: Thêm mobio token.
-- Version: 0.1.2: Add json.dums by func finish_save_file_by_filepath
-- Version: 0.1.3: Add func get_path_by_url, get_binary_by_url
-    + Hướng dẫn sử dụng:
-        + func get_path_by_url -> kết quả trả về là path của url.
-          ```python3
-          from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-          MobioMediaSDK().get_path_by_url(url)
-          ```
-        + func get_binary_by_url -> kết quả trả về là binary của url
-          ```python3
-          from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-          MobioMediaSDK().get_binary_by_url(url)
-          ```
-- Version: 0.1.4: Add func get_filename_by_url
-  + Hướng dẫn sử dụng:
-    + func get_filename_by_url -> kết quả trả về là filename của url
-      ```python3
-      from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-      MobioMediaSDK().get_filename_by_url(url)
-      ```
-- Version: 0.1.5: Delete system_config
-- Version: 0.1.6: Rename get_local_path_by_url -> get_path_by_url
-- Version: 0.1.7: Option read file "r" -> "rb"
-- Version: 0.1.8: Update lại token call từ Admin
-- Version: 0.1.9: Bổ sung tính năng:
-  - Tạo public link khi chưa có file upload.
-      ```python3
-      from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-      MobioMediaSDK().create_public_url_without_file(
-            merchant_id="merchant_id",
-            filename="filename",
-            mimetype_str="mimetype_str"
-      )
-  
-      result = {
-        'url': '',
-        'local_path': '',
-        'filename': ''
-      }
-      ```
-      Sau khi xử lý nghiệp vụ xong có thể dùng func sau để Lưu file được lấy path từ URL
-      ```python3
-       from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-       MobioMediaSDK().finish_save_file_by_public_url(filepath="filepath", url="url")
-      ```
-  - Thêm option **file_byte** khi upload file. Option này phục vụ cho nhu cầu upload file bằng bytes.
-    
-- Version: 0.2.0: Bổ sung option display, group_ids
-- Version: 0.2.1: Bổ sung merchant_id
-- Version: 0.2.2: Sửa từ get public-host từ module media sang module Admin.
-- Version: 0.2.2 và 0.2.3: Bổ sung phần tính dung lượng file khi trả về.
-- Version: 0.2.5: Chuyển việc lấy public-host sang admin-sdk
-- Version: 0.2.6: Apply libs m-kafka-sdk-v2
-- Version: 0.2.7: Bỏ m-kafka-sdk
-- Version: 0.2.8: Fix lỗi encode url với những tên file đặc biệt
```

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/config.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/config.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/constant.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/constant.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/custom_mimetypes.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/custom_mimetypes.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/merchant_config.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/merchant_config.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/mobio_media_sdk.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/mobio_media_sdk.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio/sdks/media/utils.py` & `mobio-media-sdk-0.2.9/mobio/sdks/media/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/PKG-INFO` & `mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 Metadata-Version: 2.1
 Name: mobio-media-sdk
-Version: 0.2.8
-Summary: Mobio media SDK
+Version: 0.2.9
+Summary: Mobio Media SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Keywords: mobio,media,file
+Description: ##  Thư viện Media.
+        
+        ### Cài đặt:
+        
+        ```bash
+         $ pip3 install mobio-media-sdk
+         ```
+        
+        #### Log:
+        
+        - Version: 0.1.1: Thêm mobio token.
+        - Version: 0.1.2: Add json.dums by func finish_save_file_by_filepath
+        - Version: 0.1.3: Add func get_path_by_url, get_binary_by_url
+            + Hướng dẫn sử dụng:
+                + func get_path_by_url -> kết quả trả về là path của url.
+                  ```python3
+                  from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+                  MobioMediaSDK().get_path_by_url(url)
+                  ```
+                + func get_binary_by_url -> kết quả trả về là binary của url
+                  ```python3
+                  from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+                  MobioMediaSDK().get_binary_by_url(url)
+                  ```
+        - Version: 0.1.4: Add func get_filename_by_url
+          + Hướng dẫn sử dụng:
+            + func get_filename_by_url -> kết quả trả về là filename của url
+              ```python3
+              from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+              MobioMediaSDK().get_filename_by_url(url)
+              ```
+        - Version: 0.1.5: Delete system_config
+        - Version: 0.1.6: Rename get_local_path_by_url -> get_path_by_url
+        - Version: 0.1.7: Option read file "r" -> "rb"
+        - Version: 0.1.8: Update lại token call từ Admin
+        - Version: 0.1.9: Bổ sung tính năng:
+          - Tạo public link khi chưa có file upload.
+              ```python3
+              from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+              MobioMediaSDK().create_public_url_without_file(
+                    merchant_id="merchant_id",
+                    filename="filename",
+                    mimetype_str="mimetype_str"
+              )
+        
+              result = {
+                'url': '',
+                'local_path': '',
+                'filename': ''
+              }
+              ```
+              Sau khi xử lý nghiệp vụ xong có thể dùng func sau để Lưu file được lấy path từ URL
+              ```python3
+               from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK
+               MobioMediaSDK().finish_save_file_by_public_url(filepath="filepath", url="url")
+              ```
+          - Thêm option **file_byte** khi upload file. Option này phục vụ cho nhu cầu upload file bằng bytes.
+        
+        - Version: 0.2.0: Bổ sung option display, group_ids
+        - Version: 0.2.1: Bổ sung merchant_id
+        - Version: 0.2.2: Sửa từ get public-host từ module media sang module Admin.
+        - Version: 0.2.2 và 0.2.3: Bổ sung phần tính dung lượng file khi trả về.
+        - Version: 0.2.5: Chuyển việc lấy public-host sang admin-sdk
+        - Version: 0.2.6: Apply libs m-kafka-sdk-v2
+        - Version: 0.2.7: Bỏ m-kafka-sdk
+        - Version: 0.2.8: Fix lỗi encode url với những tên file đặc biệt
+        - Version: 0.2.9: Nâng cấp confluent_kafka
+        
+Keywords: mobio,media,upload
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-##  Thư viện Media.
-
-### Cài đặt:
-
-```bash
- $ pip3 install mobio-media-sdk
- ```
-
-#### Log:
-
-- Version: 0.1.1: Thêm mobio token.
-- Version: 0.1.2: Add json.dums by func finish_save_file_by_filepath
-- Version: 0.1.3: Add func get_path_by_url, get_binary_by_url
-    + Hướng dẫn sử dụng:
-        + func get_path_by_url -> kết quả trả về là path của url.
-          ```python3
-          from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-          MobioMediaSDK().get_path_by_url(url)
-          ```
-        + func get_binary_by_url -> kết quả trả về là binary của url
-          ```python3
-          from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-          MobioMediaSDK().get_binary_by_url(url)
-          ```
-- Version: 0.1.4: Add func get_filename_by_url
-  + Hướng dẫn sử dụng:
-    + func get_filename_by_url -> kết quả trả về là filename của url
-      ```python3
-      from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-      MobioMediaSDK().get_filename_by_url(url)
-      ```
-- Version: 0.1.5: Delete system_config
-- Version: 0.1.6: Rename get_local_path_by_url -> get_path_by_url
-- Version: 0.1.7: Option read file "r" -> "rb"
-- Version: 0.1.8: Update lại token call từ Admin
-- Version: 0.1.9: Bổ sung tính năng:
-  - Tạo public link khi chưa có file upload.
-      ```python3
-      from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-      MobioMediaSDK().create_public_url_without_file(
-            merchant_id="merchant_id",
-            filename="filename",
-            mimetype_str="mimetype_str"
-      )
-  
-      result = {
-        'url': '',
-        'local_path': '',
-        'filename': ''
-      }
-      ```
-      Sau khi xử lý nghiệp vụ xong có thể dùng func sau để Lưu file được lấy path từ URL
-      ```python3
-       from mobio.sdks.media.mobio_media_sdk import MobioMediaSDK 
-       MobioMediaSDK().finish_save_file_by_public_url(filepath="filepath", url="url")
-      ```
-  - Thêm option **file_byte** khi upload file. Option này phục vụ cho nhu cầu upload file bằng bytes.
-    
-- Version: 0.2.0: Bổ sung option display, group_ids
-- Version: 0.2.1: Bổ sung merchant_id
-- Version: 0.2.2: Sửa từ get public-host từ module media sang module Admin.
-- Version: 0.2.2 và 0.2.3: Bổ sung phần tính dung lượng file khi trả về.
-- Version: 0.2.5: Chuyển việc lấy public-host sang admin-sdk
-- Version: 0.2.6: Apply libs m-kafka-sdk-v2
-- Version: 0.2.7: Bỏ m-kafka-sdk
-- Version: 0.2.8: Fix lỗi encode url với những tên file đặc biệt
```

### Comparing `mobio-media-sdk-0.2.8/mobio_media_sdk.egg-info/SOURCES.txt` & `mobio-media-sdk-0.2.9/mobio_media_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 mobio/sdks/media/__init__.py
 mobio/sdks/media/config.py
 mobio/sdks/media/constant.py
```

### Comparing `mobio-media-sdk-0.2.8/setup.py` & `mobio-media-sdk-0.2.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 from setuptools import find_namespace_packages, setup
 
 
 class Readme(object):
-    __readme_path = "/Users/tungdd/workspace/mobio/media/media_sdks/README_NEW.md"
+    __readme_path = "README.md"
 
     @staticmethod
     def get():
         """get content README.md
         :param filename:
         :return:
         """
         long_description = ""
-        with open(Readme().__readme_path, "r", encoding="utf-8") as req_file:
+        with open(Readme.__readme_path, "r", encoding="utf-8") as req_file:
             long_description = req_file.read()
         return long_description
 
 
 class Requirements(object):
-    __requirements_path = "/Users/tungdd/workspace/mobio/media/media_sdks/requirements_sdk.txt"
 
     @staticmethod
     def get():
         """Retrieve all dependencies for this project
         :param filename:
         :return:
         """
-        requirements = []
-        with open(Requirements.__requirements_path) as req_file:
-            for line in req_file.read().splitlines():
-                if not line.strip().startswith("#"):
-                    requirements.append(line)
+        requirements = ["m-singleton", "Werkzeug", "Flask", "m-caching", "requests", "confluent_kafka==1.7.0", "python-magic", "mobio-admin-sdk"]
         return requirements
 
 
-version = "0.2.8"
+version_dev='0.2.10'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='0.2.9'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+
+run_mode=''
+
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
     #
     # And where it will live on PyPI: https://pypi.org/project/sampleproject/
     #
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
-    name="mobio-media-sdk",  # Required
+    name="mobio-media-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version=version,  # Required
+    version='0.2.9',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description="Mobio media SDK",  # Optional
+    description="Mobio Media SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
@@ -115,18 +114,18 @@
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
-    keywords="mobio, media, file",  # Optional
+    keywords="mobio, media, upload",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
-    # package_dir={"": "src"},  # Optional
+    # package_dir={"": "mobio"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
@@ -194,8 +193,8 @@
         # "Bug Reports": "https://github.com/mobiovn",
         # "Funding": "https://mobio.vn/",
         # "Say Thanks!": "https://mobio.vn/",
         # 'Documentation': 'https://packaging.python.org/tutorials/distributing-packages/',
         "Source": "https://github.com/mobiovn",
     },
     license="MIT",
-)
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

