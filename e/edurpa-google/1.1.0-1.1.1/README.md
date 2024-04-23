# Comparing `tmp/edurpa_google-1.1.0-py3-none-any.whl.zip` & `tmp/edurpa_google-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9370 bytes, number of entries: 11
+Zip file size: 9363 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-17 16:24 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat    13103 b- defN 24-Apr-18 09:37 EduRPA/Google/Classroom.py
--rw-rw-rw-  2.0 fat     1549 b- defN 24-Apr-18 09:37 EduRPA/Google/CustomOAuth.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-23 16:12 EduRPA/Google/CustomOAuth.py
 -rw-rw-rw-  2.0 fat    11964 b- defN 24-Apr-18 09:38 EduRPA/Google/Form.py
 -rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-21 05:45 EduRPA/Google/Utils.py
 -rw-rw-rw-  2.0 fat      469 b- defN 24-Apr-21 13:23 EduRPA/Google/__init__.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-21 13:23 edurpa_google-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      670 b- defN 24-Apr-21 13:23 edurpa_google-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 13:23 edurpa_google-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-21 13:23 edurpa_google-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      893 b- defN 24-Apr-21 13:23 edurpa_google-1.1.0.dist-info/RECORD
-11 files, 30149 bytes uncompressed, 7854 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-23 16:13 edurpa_google-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      692 b- defN 24-Apr-23 16:13 edurpa_google-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 16:13 edurpa_google-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-23 16:13 edurpa_google-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      893 b- defN 24-Apr-23 16:13 edurpa_google-1.1.1.dist-info/RECORD
+11 files, 30133 bytes uncompressed, 7847 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: EduRPA/Google/Utils.py
 Comment: 
 
 Filename: EduRPA/Google/__init__.py
 Comment: 
 
-Filename: edurpa_google-1.1.0.dist-info/LICENSE
+Filename: edurpa_google-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_google-1.1.0.dist-info/METADATA
+Filename: edurpa_google-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_google-1.1.0.dist-info/WHEEL
+Filename: edurpa_google-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_google-1.1.0.dist-info/top_level.txt
+Filename: edurpa_google-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_google-1.1.0.dist-info/RECORD
+Filename: edurpa_google-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Google/CustomOAuth.py

```diff
@@ -1,15 +1,15 @@
 import base64
 import pickle
 import google.oauth2.credentials
 import io
 import json
-import os.path
 
-VAULT_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), '../devdata/vault.json'))
+# Get the current working directory
+VAULT_PATH = './devdata/vault.json'
 
 class CustomOAuth():
     def __init__(self):
         pass
 
     def _create_credentials(self, token_file_path):
         credentials = None
```

## Comparing `edurpa_google-1.1.0.dist-info/LICENSE` & `edurpa_google-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_google-1.1.0.dist-info/METADATA` & `edurpa_google-1.1.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: edurpa-google
-Version: 1.1.0
+Version: 1.1.1
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edurpa-google
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: robotframework (==6.1.1)
 Requires-Dist: rpaframework (==27.7.0)
 Requires-Dist: google-api-python-client
 Requires-Dist: PyPDF2
+Requires-Dist: gdown
 
 # EduRPA
 EduRPA is an robotframework librabry that support feature in education field
```

## Comparing `edurpa_google-1.1.0.dist-info/RECORD` & `edurpa_google-1.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 EduRPA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 EduRPA/Google/Classroom.py,sha256=ZUMo0Dlc46bFwAUnUHKrbOl_RzvOvVHWAQtfa3hJPqQ,13103
-EduRPA/Google/CustomOAuth.py,sha256=mdcF-tqze2HulL4QZ6K-dl-dr-Am8qLSB3opr2F9PkM,1549
+EduRPA/Google/CustomOAuth.py,sha256=zyN2Iq8wwoXtwI9bBAtgecA7R9aZr3rfzswlsf8Bf4o,1511
 EduRPA/Google/Form.py,sha256=K4SdXFT6VKbreHnNebTjGtEDuJoPC7JnKD4t1xSB55Y,11964
 EduRPA/Google/Utils.py,sha256=oELOV-TFTQz_NDf9i0usZfXC9kbY4Xa_Kb1T7D8ssOw,314
 EduRPA/Google/__init__.py,sha256=q9wb2yVj8rKIsGf7UelAixwVKWk9CCKsQCzmUtCVzDM,469
-edurpa_google-1.1.0.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_google-1.1.0.dist-info/METADATA,sha256=iQSxZjFW7FHqyaQ9j1-stIv51vNJRfbhGmR4pQ3lOGU,670
-edurpa_google-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_google-1.1.0.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_google-1.1.0.dist-info/RECORD,,
+edurpa_google-1.1.1.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_google-1.1.1.dist-info/METADATA,sha256=8CQoxcQ0kt2cdsJMgyOgH3TlkSXI8BPcpiewuOjRm38,692
+edurpa_google-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_google-1.1.1.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_google-1.1.1.dist-info/RECORD,,
```

