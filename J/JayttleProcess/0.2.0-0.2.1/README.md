# Comparing `tmp/JayttleProcess-0.2.0-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 51041 bytes, number of entries: 13
+Zip file size: 51174 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2602 b- defN 24-Apr-22 05:39 JayttleProcess/CommonDecorator.py
 -rw-rw-rw-  2.0 fat     4727 b- defN 24-Mar-19 06:31 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat     5978 b- defN 24-Apr-22 10:17 JayttleProcess/FTPCommonUse.py
+-rw-rw-rw-  2.0 fat     6334 b- defN 24-Apr-22 12:47 JayttleProcess/FTPCommonUse.py
 -rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-22 05:39 JayttleProcess/JsonCommonManage.py
 -rw-rw-rw-  2.0 fat    35197 b- defN 24-Apr-22 10:17 JayttleProcess/RinexCommonManage.py
 -rw-rw-rw-  2.0 fat    30819 b- defN 24-Apr-22 05:38 JayttleProcess/SQLCommonUse.py
 -rw-rw-rw-  2.0 fat   117788 b- defN 24-Apr-22 05:38 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-22 10:18 JayttleProcess-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 10:18 JayttleProcess-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-22 10:18 JayttleProcess-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1132 b- defN 24-Apr-22 10:18 JayttleProcess-0.2.0.dist-info/RECORD
-13 files, 205167 bytes uncompressed, 49131 bytes compressed:  76.1%
+-rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-22 12:48 JayttleProcess-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 12:48 JayttleProcess-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-22 12:48 JayttleProcess-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1132 b- defN 24-Apr-22 12:48 JayttleProcess-0.2.1.dist-info/RECORD
+13 files, 205523 bytes uncompressed, 49264 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.2.0.dist-info/METADATA
+Filename: JayttleProcess-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.2.0.dist-info/WHEEL
+Filename: JayttleProcess-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.2.0.dist-info/top_level.txt
+Filename: JayttleProcess-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.2.0.dist-info/RECORD
+Filename: JayttleProcess-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/FTPCommonUse.py

```diff
@@ -133,30 +133,40 @@
         return False
 
     finally:
         # 关闭FTP连接
         ftp.quit()
 
 
+def process_string(s: str) -> str:
+    if len(s) == 4:
+        if s.startswith('B'):
+            return 'towerbase' + s[2]
+        elif s.startswith('R'):
+            return 'tower' + s[2]
+    return None
+
+
 
 def download_files_from_ftp_by_txt(ftp_config: FTPConfig, txt_file_path: str, local_save_path: str) -> bool:
     # 读取指定的 txt 文件
     with open(txt_file_path, 'r') as txt_file:
         files_to_download = txt_file.readlines()
     # 去除每行末尾的换行符
     files_to_download = [file.strip() for file in files_to_download]
-
+    # 获取文件名的前四个字符并处理
+    target_folder = process_string(os.path.basename(txt_file_path)[:4])
     # 使用 FTPConfig 对象下载文件
-    success = download_files_from_ftp(ftp_config, remote_folder='towerbase2', files_to_download=files_to_download, local_save_path=local_save_path)
+    success = download_files_from_ftp(ftp_config, remote_folder=target_folder, files_to_download=files_to_download, local_save_path=local_save_path)
     return success
 
 
-# 示例使用
-json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\options.json'
-ftp_config = FTPConfig(json_file_path)
-txt_file_path = r'D:\Ropeway\GNSS\R031_output_B021.txt'
-local_save_path = r'D:\Ropeway\GNSS\FTP\B021'
-
-if download_files_from_ftp_by_txt(ftp_config, txt_file_path, local_save_path):
-    print("文件下载成功！")
-else:
-    print("文件下载失败。")
+# # 示例使用
+# json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\options.json'
+# ftp_config = FTPConfig(json_file_path)
+# txt_file_path = r'D:\Ropeway\GNSS\R031_output_B021.txt'
+# local_save_path = r'D:\Ropeway\GNSS\FTP\B021'
+
+# if download_files_from_ftp_by_txt(ftp_config, txt_file_path, local_save_path):
+#     print("文件下载成功！")
+# else:
+#     print("文件下载失败。")
```

## Comparing `JayttleProcess-0.2.0.dist-info/METADATA` & `JayttleProcess-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.2.0
-Summary: modifty time:2024-04-22 18:00
+Version: 0.2.1
+Summary: modifty time:2024-04-22 21:00
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
```

## Comparing `JayttleProcess-0.2.0.dist-info/RECORD` & `JayttleProcess-0.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 JayttleProcess/CommonDecorator.py,sha256=JbmL5wFuJ1bxNh-ka2drELVX8Y4InzNJ-_sXKDyiMvU,2602
 JayttleProcess/ComputerControl.py,sha256=S-glg1n5thtd-GxeemZVKIJT2ibXkyw71qUTYDxmG6A,4727
 JayttleProcess/EntertainmentCode.py,sha256=KR-nFHjwIjfl8E_IMuRl44p2Xwkw6UMZYuvkdL9NFck,613
-JayttleProcess/FTPCommonUse.py,sha256=-XVBbtvAbJOghuWvscs9R7Gp2Eh5qXdEs8DnqNHF0bQ,5978
+JayttleProcess/FTPCommonUse.py,sha256=nyRub8LQJmTTSEpAioImC94XZbGF519-4WWyY9y0Gg4,6334
 JayttleProcess/JsonCommonManage.py,sha256=KJtfAxPUGktFMocoFKFd8E_VtGW-vyhAMPPz--34mkA,5650
 JayttleProcess/RinexCommonManage.py,sha256=JbAf3GSUJ_gLIq0cQQPDn3NY_ROeRYhweWWgN2HU2lA,35197
 JayttleProcess/SQLCommonUse.py,sha256=7QVASTQ-AjPLz8E52ZAbdBOQumbEllEnpQbJ-H4qKo0,30819
 JayttleProcess/TimeSeriesDataMethod.py,sha256=HUmf2RjkcNRAcjS4XkTwDqQNc-6mGhVcufjGo82D4rk,117788
 JayttleProcess/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-JayttleProcess-0.2.0.dist-info/METADATA,sha256=_LO_OtCLzbiHPF3348Aw3gsnNdJBV53NmKoiKdKMizY,554
-JayttleProcess-0.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-JayttleProcess-0.2.0.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
-JayttleProcess-0.2.0.dist-info/RECORD,,
+JayttleProcess-0.2.1.dist-info/METADATA,sha256=H-6KQOh7Q8PMwp-yANuElPEoT-3hhdgaiV0qwqbGCX4,554
+JayttleProcess-0.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+JayttleProcess-0.2.1.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
+JayttleProcess-0.2.1.dist-info/RECORD,,
```

