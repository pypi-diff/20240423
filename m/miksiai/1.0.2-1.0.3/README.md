# Comparing `tmp/miksiai-1.0.2-cp310-cp310-macosx_11_0_arm64.whl.zip` & `tmp/miksiai-1.0.3-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 381140 bytes, number of entries: 16
+Zip file size: 381111 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 15:56 miksiai/__init__.py
 -rwxr-xr-x  2.0 unx   136184 b- defN 24-Apr-23 12:34 miksiai/agent.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   117142 b- defN 24-Apr-23 12:34 miksiai/api.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx    77353 b- defN 24-Apr-23 12:34 miksiai/master.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   100653 b- defN 24-Apr-23 12:34 miksiai/pythontool.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx    75227 b- defN 24-Apr-23 12:34 miksiai/settings.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   172602 b- defN 24-Apr-23 12:34 miksiai/sqltool.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx    78168 b- defN 24-Apr-23 12:34 miksiai/utils.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   118093 b- defN 24-Apr-23 12:34 miksiai/sql_graph/custom_sql.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   136972 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_graph.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx    72260 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so
 -rwxr-xr-x  2.0 unx   239248 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_runnables.cpython-310-darwin.so
--rw-r--r--  2.0 unx     7454 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1479 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/RECORD
-16 files, 1332953 bytes uncompressed, 378682 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx     7431 b- defN 24-Apr-23 12:51 miksiai-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 24-Apr-23 12:51 miksiai-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-23 12:51 miksiai-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1479 b- defN 24-Apr-23 12:51 miksiai-1.0.3.dist-info/RECORD
+16 files, 1332922 bytes uncompressed, 378653 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so
 Comment: 
 
 Filename: miksiai/sql_graph/sql_runnables.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai-1.0.2.dist-info/METADATA
+Filename: miksiai-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: miksiai-1.0.2.dist-info/WHEEL
+Filename: miksiai-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: miksiai-1.0.2.dist-info/top_level.txt
+Filename: miksiai-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: miksiai-1.0.2.dist-info/RECORD
+Filename: miksiai-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `miksiai-1.0.2.dist-info/METADATA` & `miksiai-1.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: miksiai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Miksi-AI empowers your BI
 Home-page: https://github.com/Miksi-io/Custom-Agent
-Author: RichardKaranuMbuti
-Author-email: officialforrichardk@gmail.com
+Author: miksiai
+Author-email: miksiai@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `miksiai-1.0.2.dist-info/RECORD` & `miksiai-1.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 miksiai/settings.cpython-310-darwin.so,sha256=lxgn4A5o0gm-co9UDBveRzOzirguPwJ6-S3i_q5vgE4,75227
 miksiai/sqltool.cpython-310-darwin.so,sha256=AhTJbq3nhqq9tYK2azQqTgkfvzxG8fmEjNr3lT8l2XE,172602
 miksiai/utils.cpython-310-darwin.so,sha256=HfCX5rtdAlc-ApvOEl31aykQVKyA4O0UeWGq4ss45cA,78168
 miksiai/sql_graph/custom_sql.cpython-310-darwin.so,sha256=7VBcfA0gVlyXtcQgZRoL8lRGgKa3F_yii4MmegFkFmM,118093
 miksiai/sql_graph/sql_graph.cpython-310-darwin.so,sha256=1WmRzSjJUloSxgx_V-i4irSuFW6R5mcNuIDxXBVR-T4,136972
 miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so,sha256=TaX5tUGdjfdr0kJnprsWFJ_CYCIJqlEHB9bFKtQJpNQ,72260
 miksiai/sql_graph/sql_runnables.cpython-310-darwin.so,sha256=VUgwdHHY8g-Wv02wqz-K8MAWvXGWrxQn9C9aUuRZqQQ,239248
-miksiai-1.0.2.dist-info/METADATA,sha256=4chQCUxSkgEboINTuRXNxlWWV2zDPbqMJZUnvlLYAck,7454
-miksiai-1.0.2.dist-info/WHEEL,sha256=ReeDLt7JoWNv8uQs9jcofmiBOX-MvocIgD8kJPMfr7M,110
-miksiai-1.0.2.dist-info/top_level.txt,sha256=ZFs4wEgKwJOgH1c2Yw9pkvibLpluMlWlMeBx9YztSFI,8
-miksiai-1.0.2.dist-info/RECORD,,
+miksiai-1.0.3.dist-info/METADATA,sha256=gBNjPNOM8hurtBIkVITRcpcaEcAWL29dnP1iBlqviwc,7431
+miksiai-1.0.3.dist-info/WHEEL,sha256=yrvteVAZzxQvtDnzdCRh4dP01sPIxYhLXIXplC7o50E,102
+miksiai-1.0.3.dist-info/top_level.txt,sha256=ZFs4wEgKwJOgH1c2Yw9pkvibLpluMlWlMeBx9YztSFI,8
+miksiai-1.0.3.dist-info/RECORD,,
```

