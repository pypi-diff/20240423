# Comparing `tmp/udata_piwik-4.0.0-py2.py3-none-any.whl.zip` & `tmp/udata_piwik-4.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9746 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-20 16:13 udata_piwik/__init__.py
--rw-r--r--  2.0 unx     2643 b- defN 23-Nov-20 16:13 udata_piwik/client.py
--rw-r--r--  2.0 unx      428 b- defN 23-Nov-20 16:13 udata_piwik/factories.py
--rw-r--r--  2.0 unx      339 b- defN 23-Nov-20 16:13 udata_piwik/models.py
--rw-r--r--  2.0 unx      692 b- defN 23-Nov-20 16:13 udata_piwik/settings.py
--rw-r--r--  2.0 unx     2175 b- defN 23-Nov-20 16:13 udata_piwik/tasks.py
--rw-r--r--  2.0 unx      279 b- defN 23-Nov-20 16:13 udata_piwik/views.py
--rw-r--r--  2.0 unx      199 b- defN 23-Nov-20 16:13 udata_piwik/migrations/2015-10-01-fix-resources-metrics.js
--rw-r--r--  2.0 unx     2015 b- defN 23-Nov-20 16:13 udata_piwik/templates/piwik.html
--rw-r--r--  2.0 unx     9084 b- defN 23-Nov-20 16:13 udata_piwik-4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Nov-20 16:13 udata_piwik-4.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      124 b- defN 23-Nov-20 16:13 udata_piwik-4.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Nov-20 16:13 udata_piwik-4.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1162 b- defN 23-Nov-20 16:13 udata_piwik-4.0.0.dist-info/RECORD
-14 files, 19262 bytes uncompressed, 7800 bytes compressed:  59.5%
+Zip file size: 9826 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:51 udata_piwik/__init__.py
+-rw-r--r--  2.0 unx     2717 b- defN 24-Apr-23 13:51 udata_piwik/client.py
+-rw-r--r--  2.0 unx      428 b- defN 24-Apr-23 13:51 udata_piwik/factories.py
+-rw-r--r--  2.0 unx      339 b- defN 24-Apr-23 13:51 udata_piwik/models.py
+-rw-r--r--  2.0 unx      692 b- defN 24-Apr-23 13:51 udata_piwik/settings.py
+-rw-r--r--  2.0 unx     2175 b- defN 24-Apr-23 13:51 udata_piwik/tasks.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-23 13:51 udata_piwik/views.py
+-rw-r--r--  2.0 unx      199 b- defN 24-Apr-23 13:51 udata_piwik/migrations/2015-10-01-fix-resources-metrics.js
+-rw-r--r--  2.0 unx     2015 b- defN 24-Apr-23 13:51 udata_piwik/templates/piwik.html
+-rw-r--r--  2.0 unx     9321 b- defN 24-Apr-23 13:52 udata_piwik-4.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-23 13:52 udata_piwik-4.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-23 13:52 udata_piwik-4.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-23 13:52 udata_piwik-4.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-23 13:52 udata_piwik-4.1.0.dist-info/RECORD
+14 files, 19573 bytes uncompressed, 7880 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: udata_piwik/migrations/2015-10-01-fix-resources-metrics.js
 Comment: 
 
 Filename: udata_piwik/templates/piwik.html
 Comment: 
 
-Filename: udata_piwik-4.0.0.dist-info/METADATA
+Filename: udata_piwik-4.1.0.dist-info/METADATA
 Comment: 
 
-Filename: udata_piwik-4.0.0.dist-info/WHEEL
+Filename: udata_piwik-4.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: udata_piwik-4.0.0.dist-info/entry_points.txt
+Filename: udata_piwik-4.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: udata_piwik-4.0.0.dist-info/top_level.txt
+Filename: udata_piwik-4.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: udata_piwik-4.0.0.dist-info/RECORD
+Filename: udata_piwik-4.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## udata_piwik/client.py

```diff
@@ -1,11 +1,14 @@
 import logging
 import requests
 
-from simplejson.errors import JSONDecodeError
+try:
+    from simplejson.errors import JSONDecodeError
+except ImportError:
+    from json.decoder import JSONDecodeError
 from urllib.parse import urlencode
 
 from flask import current_app
 
 from . import settings
 
 # Prevent max headers error by raising the hardcoded limit
```

## Comparing `udata_piwik-4.0.0.dist-info/METADATA` & `udata_piwik-4.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-piwik
-Version: 4.0.0
+Version: 4.1.0
 Summary: Piwik/Matomo support for uData
 Home-page: https://github.com/opendatateam/udata-piwik
 Author: OpenDataTeam
 Author-email: contact@opendata.team
 License: LGPL
 Keywords: udata piwik
 Classifier: Development Status :: 3 - Alpha
@@ -90,14 +90,19 @@
 [circleci-badge]: https://circleci.com/gh/opendatateam/udata-piwik.svg?style=shield
 [gitter-badge]: https://badges.gitter.im/Join%20Chat.svg
 [gitter-url]: https://gitter.im/opendatateam/udata
 [udata]: https://github.com/opendatateam/udata
 
 # Changelog
 
+## 4.1.0 (2024-04-23)
+
+- Do not import simplejson [#287](https://github.com/opendatateam/udata-piwik/pull/287)
+- Migrate to Python 3.11 following `udata` dependencies upgrade [#286](https://github.com/opendatateam/udata-piwik/pull/286)
+
 ## 4.0.0 (2023-11-20)
 
 - [BREAKING] Remove metrics computation with Matomo as a source (cf below) [#273](https://github.com/opendatateam/udata-piwik/pull/273)
 - Replace mongo legacy image in CI [#266](https://github.com/opendatateam/udata-piwik/pull/266)
 - Upgrade test and develop deps [#284](https://github.com/opendatateam/udata-piwik/pull/284)
 
 Up until this version, metrics were tentatively computed from Matomo for pretty much every object of a udata instance. We found this method to be pretty inaccurate, since Matomo limits the number of records stored to roughly the most visited 1000 for a given "namespace". There's a way around that by using the data from the Live module of Matomo but it's not enabled on our instance for privacy reasons. We also needed to count hits that Matomo could not know of: resources (files) downloads made directly on our server.
```

## Comparing `udata_piwik-4.0.0.dist-info/RECORD` & `udata_piwik-4.1.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 udata_piwik/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-udata_piwik/client.py,sha256=KMRQbEpmsAYZUAxiNu9WiSJXEdtNlQCOKpMfdDTJmV0,2643
+udata_piwik/client.py,sha256=LSLZLlR8PBtaJjRKBUwwrN0p1372hDGu3TIrSalU22U,2717
 udata_piwik/factories.py,sha256=iZ5SrUIRry2ukb8nedYEBzBXY2wYtIWdMq3Rb-PRfMA,428
 udata_piwik/models.py,sha256=OO2kvB15NriorzJ5xq72sEZvhxGSZWheKHVFfivixV8,339
 udata_piwik/settings.py,sha256=-qGt0tFVrkZJMjompnjjmQX73olNvGI6ceVeix1Auww,692
 udata_piwik/tasks.py,sha256=lGOSHvnLw3ZAWHA5EZWppOpeFqj2Rn6YUZl11waiRgU,2175
 udata_piwik/views.py,sha256=AMBHivXLIDkNPmwLovD794iaSjQo_Bnl6zZvpT0hTdc,279
 udata_piwik/migrations/2015-10-01-fix-resources-metrics.js,sha256=8GWUKfLxMsXwXT3t5OO0pvlJCl8J6hpP-BUML99DFWw,199
 udata_piwik/templates/piwik.html,sha256=1KA-Yl_VS4gsq8WpGD5mIbVtxApK1gPztaK8xDs2poM,2015
-udata_piwik-4.0.0.dist-info/METADATA,sha256=VkpGzdl6KiZIEqyCKBTht7MAQ-kOrUCdHDIL4op01a4,9084
-udata_piwik-4.0.0.dist-info/WHEEL,sha256=P2T-6epvtXQ2cBOE_U1K4_noqlJFN3tj15djMgEu4NM,110
-udata_piwik-4.0.0.dist-info/entry_points.txt,sha256=0KSxhYoKumJP8GU4qqzIrh5gELrWRyMv4lUxXb8tvfs,124
-udata_piwik-4.0.0.dist-info/top_level.txt,sha256=OzcCbU-GK4Jh-6lVOLkGQjNDcwtsupESGM_aqCNoPbY,12
-udata_piwik-4.0.0.dist-info/RECORD,,
+udata_piwik-4.1.0.dist-info/METADATA,sha256=YOKSXHUMB21vzyMWqbIAjvQk2o2VOba6Ny9l63gbuys,9321
+udata_piwik-4.1.0.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+udata_piwik-4.1.0.dist-info/entry_points.txt,sha256=0KSxhYoKumJP8GU4qqzIrh5gELrWRyMv4lUxXb8tvfs,124
+udata_piwik-4.1.0.dist-info/top_level.txt,sha256=OzcCbU-GK4Jh-6lVOLkGQjNDcwtsupESGM_aqCNoPbY,12
+udata_piwik-4.1.0.dist-info/RECORD,,
```

