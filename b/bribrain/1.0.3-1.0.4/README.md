# Comparing `tmp/bribrain-1.0.3.tar.gz` & `tmp/bribrain-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bribrain-1.0.3.tar", last modified: Wed Apr  3 07:51:03 2024, max compression
+gzip compressed data, was "dist/bribrain-1.0.4.tar", last modified: Tue Apr 23 08:53:07 2024, max compression
```

## Comparing `bribrain-1.0.3.tar` & `bribrain-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 07:51:03.000000 bribrain-1.0.3/
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain/
--rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-03-20 04:25:35.000000 bribrain-1.0.3/bribrain/__init__.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     2456 2024-03-14 14:03:41.000000 bribrain-1.0.3/bribrain/config.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     4330 2024-04-03 02:49:31.000000 bribrain-1.0.3/bribrain/function.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    80247 2024-04-03 03:09:21.000000 bribrain-1.0.3/bribrain/ingestion.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    16561 2024-04-03 07:48:47.000000 bribrain-1.0.3/bribrain/load.py
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       40 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-04-03 07:51:03.000000 bribrain-1.0.3/bribrain.egg-info/top_level.txt
--rwx------   0 cdsw      (8536) cdsw      (8536)      647 2024-04-03 07:50:54.000000 bribrain-1.0.3/setup.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-03 07:51:03.000000 bribrain-1.0.3/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-04-03 07:51:03.000000 bribrain-1.0.3/setup.cfg
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain/
+-rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/__init__.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     2456 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/config.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     4330 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/function.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    81374 2024-04-23 08:52:31.000000 bribrain-1.0.4/bribrain/ingestion.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    16561 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/load.py
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       40 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/top_level.txt
+-rwx------   0 cdsw      (8536) cdsw      (8536)      647 2024-04-23 08:52:51.000000 bribrain-1.0.4/setup.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-23 08:53:07.000000 bribrain-1.0.4/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-04-23 08:53:07.000000 bribrain-1.0.4/setup.cfg
```

### Comparing `bribrain-1.0.3/bribrain/config.py` & `bribrain-1.0.4/bribrain/config.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.3/bribrain/function.py` & `bribrain-1.0.4/bribrain/function.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.3/bribrain/ingestion.py` & `bribrain-1.0.4/bribrain/ingestion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #=============================================================#
 ###  CREATED AT     : 18 MARET 2024                         ###
-###  UPDATED AT     : 03 APRIL 2024                         ###
+###  UPDATED AT     : 23 APRIL 2024                         ###
 ###  COPYRIGHT      : ANDRI ARIYANTO                        ###
 ###  DESCRIPTION    : Module untuk melakukan ingest data    ###
 #=============================================================#
 
 import os # memungkinkan pengguna untuk berinteraksi dengan sistem operasi yang dijalankan sekarang
 import re # membantu mencocokkan atau menemukan string atau set string lainnya, menggunakan sintaksis khusus yang dimiliki suatu pola.
 import json # untuk mengubah kamus python menjadi string JSON yang dapat ditulis menjadi file
@@ -13,17 +13,25 @@
 from pytz import timezone # memasukkan zona waktu
 from pyspark.sql import functions as F # memasukkan fungsi dari pyspark
 from datetime import datetime, timedelta # Durasi yang mengekspresikan perbedaan antara dua tanggal, waktu, atau instance waktu ke resolusi mikrodetik.
 from dateutil.relativedelta import relativedelta # Menerapkan pada datetime yang ada dan dapat menggantikan komponen spesifik dari datetime, atau mewakili interval waktu
 from pyspark.sql.types import StructType, StructField, StringType, TimestampType # memasukkan struktur tipe yang berada pada pyspark
 
 
-
+# 1 ===================================================================================================================================================================================================
 def ingest_to_hive(spark, params):  
+  """Orchestrator untuk proses standard ingestion
   
+  Parameters:
+      df: Spark DataFrame input
+      params: parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
+  
+  Return:
+      dict: parameter-parameter hasil yang disimpan dalam bentuk dictionaries
+  """  
   t0 = set_ingest_timer()
   dt0 = set_datetime()
 
   params = get_additional_attributes(params)
   params["formatted_source_schema"] = params["source_schema"]
   params["formatted_source_table"] = params["source_table"]
   params["hive_partition_date"] = params["hive_partition_ingest"]
@@ -84,18 +92,33 @@
     params["status_desc"] = ": "+str(e).replace("\n","|")
   finally:
     params = update_additional_attributes(spark, params)
     params["job_period"] = None
     params["running_time"] = get_ingest_timer_string(t0)
     
     return params
-  
-  
+# 2 ===================================================================================================================================================================================================
+def try_or(func, default=None, expected_exc=(Exception,)):
+  """Menangkap error dan memberikan keluaran sesuai parameter
+
+  Args:
+      func (function): python function
+        (notes is ditambahkan lambda pada sebelum nama function, ex: try_or(lambda:func))
+      default (object): keluaran yang diharapkan ketika terjadi error
+      expected_exc (Exception): Exception yang diharapkan
     
-# 1 ===================================================================================================================================================================================================
+  Returns:
+      object: keluaran dari function atau mengembalikan keluaran sesuai input jika terdapat error
+  """
+  
+  try:
+    return func()
+  except expected_exc:
+    return default
+# 3 ===================================================================================================================================================================================================
 def add_partition_column(df, params):
   """Menambahkan kolom yang akan digunakan sebagai partisi pada Spark DataFrame
   
   Parameters:
       df: Spark DataFrame input
       params: parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
   
@@ -118,15 +141,14 @@
       i += 1 # menambahkan 1 nilai pencacah
   else: # kondisi ketika hive_partition_source tidak memiliki value
     # melakukan perulangan untuk menambahkan kolom partisi sebanyak list input
     while i < len(hive_partition_col): # kondisi perulangan true ketika variable pencacah lebih kecil dari panjang list hive_partition_col
       df = df.withColumn(hive_partition_col[i], F.lit(hive_partition_date[i])) # proses penambahan kolom dan nilainya yang mengacu pada hive_partition_date
       i += 1# menambahkan 1 nilai pencacah
   return df # return Spark DataFrame yang ditambahkan kolom partisi
-# 2 ===================================================================================================================================================================================================
 # 4 ===================================================================================================================================================================================================
 def drop_hive_table(spark, params):  
   """Menghapus tabel pada hive 
   
   Parameters:
       spark: objek SparkSession
       params: parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
@@ -517,14 +539,15 @@
       spark : Objek SparkSession
       df  : Spark DataFrame yang akan dicari jumlah row-nya
       params : parameter-parameter pendukung yang disimpan dalam bentuk dictionaries
 
   Return : Hasil partisi number
 
   """
+  hive_schema = params["hive_schema"] # menyimpan nama hive schema
   hive_table = params["hive_table"] # menyimpan nama hive tabel
   params["hive_blocksize"] = int(params["repartition_size"])*1024*1024 # update hive_blocksize dengan integer partisi size
   params["sample_schema"] = params["hive_schema"] # update sample schema dengan temporary
   params["sample_table"] = "sample_" + hive_table # update sampel tabel dengan hive tabel
   
   if hive_schema.startswith("dev"):
     hdfs_path = "/dev/"
@@ -1180,15 +1203,15 @@
   params["created_by"] = get_describe_formatted(spark, params, "Owner") # update value dengan informasi metadata pembuat tabel target
   
   # melakukan kondisional tabel target memiliki partisi ingest atau tidak
   if params["hive_partition_date"] != None: # kondisi ketika tabel target memiliki partisi terakhir
     partition_date = params["hive_partition_date"].split("|") # membuat list hive_partition_date
     partition_col = params["hive_partition_col"].split("|") # membuat list hive_partition_date
     params["partition_ingest"] = "/".join(["{}={}".format(partition_col[i], partition_date[i]) for i in range(len(partition_date))]) # membuat parameter partition_ingest dari partition_date dan partition_col
-    params["partition_path"] = params["storage_path"] + "/" + params["partition_ingest"] # menetapkan lokasi partisi ter-ingest di hive direktori
+    params["partition_path"] = try_or(lambda: params["storage_path"] + "/" + params["partition_ingest"]) # menetapkan lokasi partisi ter-ingest di hive direktori
   else: # kondisi ketika tabel target tidak memiliki partisi terakhir
     params["partition_path"] = params["storage_path"] # menetapkan lokasi data ter-ingest di hive direktori
   params["total_rows"] = get_total_count(spark, params) # mendapatkan jumlah keseluruhan data dari tabel target
   return params # return params yang telah ter-update
   #except:
   #  return params # return params yang telah ter-update
 # 34 ==================================================================================================================================================================================================
```

### Comparing `bribrain-1.0.3/bribrain/load.py` & `bribrain-1.0.4/bribrain/load.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.3/setup.py` & `bribrain-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'Standard code for Dept BRIBrain'
 
 # Setting up
 setup(
     name="bribrain",
     version=VERSION,
     author="Andri Ariyanto",
```

