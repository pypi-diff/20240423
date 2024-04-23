# Comparing `tmp/dtps_http-1.3.4-py3-none-any.whl.zip` & `tmp/dtps_http-1.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 152734 bytes, number of entries: 40
+Zip file size: 152736 bytes, number of entries: 40
 -rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 dtps/__init__.py
 -rw-r--r--  2.0 unx     6709 b- defN 80-Jan-01 00:00 dtps/config.py
--rw-r--r--  2.0 unx     3733 b- defN 80-Jan-01 00:00 dtps/dtps_utils.py
+-rw-r--r--  2.0 unx     3735 b- defN 80-Jan-01 00:00 dtps/dtps_utils.py
 -rw-r--r--  2.0 unx    11921 b- defN 80-Jan-01 00:00 dtps/ergo_create.py
 -rw-r--r--  2.0 unx     7597 b- defN 80-Jan-01 00:00 dtps/ergo_ui.py
 -rw-r--r--  2.0 unx    12733 b- defN 80-Jan-01 00:00 dtps/ergo_use.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dtps/py.typed
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dtps/structures.py
 -rw-r--r--  2.0 unx      655 b- defN 80-Jan-01 00:00 dtps_http/__init__.py
 -rw-r--r--  2.0 unx     4860 b- defN 80-Jan-01 00:00 dtps_http/blob_manager.py
@@ -30,13 +30,13 @@
 -rw-r--r--  2.0 unx     1338 b- defN 80-Jan-01 00:00 dtps_http_programs/dtps_send_continuous.py
 -rw-r--r--  2.0 unx     3112 b- defN 80-Jan-01 00:00 dtps_http_programs/dtps_stats.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dtps_http_programs/py.typed
 -rw-r--r--  2.0 unx     1789 b- defN 80-Jan-01 00:00 dtps_http_programs/server_clock.py
 -rw-r--r--  2.0 unx     1270 b- defN 80-Jan-01 00:00 static/favicon.png
 -rw-r--r--  2.0 unx     7885 b- defN 80-Jan-01 00:00 static/send.js
 -rw-r--r--  2.0 unx     1472 b- defN 80-Jan-01 00:00 static/style.css
--rw-r--r--  2.0 unx    75933 b- defN 80-Jan-01 00:00 dtps_http-1.3.4.dist-info/LICENSE.pdf
--rw-r--r--  2.0 unx     1040 b- defN 80-Jan-01 00:00 dtps_http-1.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dtps_http-1.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 dtps_http-1.3.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3186 b- defN 16-Jan-01 00:00 dtps_http-1.3.4.dist-info/RECORD
-40 files, 370233 bytes uncompressed, 147728 bytes compressed:  60.1%
+-rw-r--r--  2.0 unx    75933 b- defN 80-Jan-01 00:00 dtps_http-1.3.5.dist-info/LICENSE.pdf
+-rw-r--r--  2.0 unx     1040 b- defN 80-Jan-01 00:00 dtps_http-1.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dtps_http-1.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 dtps_http-1.3.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3186 b- defN 16-Jan-01 00:00 dtps_http-1.3.5.dist-info/RECORD
+40 files, 370235 bytes uncompressed, 147730 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: static/send.js
 Comment: 
 
 Filename: static/style.css
 Comment: 
 
-Filename: dtps_http-1.3.4.dist-info/LICENSE.pdf
+Filename: dtps_http-1.3.5.dist-info/LICENSE.pdf
 Comment: 
 
-Filename: dtps_http-1.3.4.dist-info/METADATA
+Filename: dtps_http-1.3.5.dist-info/METADATA
 Comment: 
 
-Filename: dtps_http-1.3.4.dist-info/WHEEL
+Filename: dtps_http-1.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: dtps_http-1.3.4.dist-info/entry_points.txt
+Filename: dtps_http-1.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: dtps_http-1.3.4.dist-info/RECORD
+Filename: dtps_http-1.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dtps/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 from logging import DEBUG, getLogger
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 from .config import *
```

## dtps/dtps_utils.py

```diff
@@ -47,15 +47,15 @@
             msgs.append(q.get_nowait())
         except asyncio.QueueEmpty:
             break
     return msgs
 
 
 class ExpensiveCallbackSubscription(SubscriptionInterface):
-    q: Queue[RawData]
+    q: "Queue[RawData]"
     sub: Optional[SubscriptionInterface]
     task: Optional[asyncio.Task]
 
     def __init__(self, expensive_callback: Callable[[RawData], Awaitable[None]]):
         self.expensive_callback = expensive_callback
         self.q = Queue()
         self.sub = None
```

## dtps_http/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 import coloredlogs  # type: ignore
 
 coloredlogs.install(level="DEBUG")  # type: ignore
 
 from logging import getLogger, INFO, WARNING
```

## dtps_http_programs/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 from logging import DEBUG, getLogger
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 from .server_clock import *
```

## Comparing `dtps_http-1.3.4.dist-info/LICENSE.pdf` & `dtps_http-1.3.5.dist-info/LICENSE.pdf`

 * *Files identical despite different names*

## Comparing `dtps_http-1.3.4.dist-info/METADATA` & `dtps_http-1.3.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtps-http
-Version: 1.3.4
+Version: 1.3.5
 Summary: 
 Author: Andrea Censi
 Author-email: AndreaCensi@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `dtps_http-1.3.4.dist-info/RECORD` & `dtps_http-1.3.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-dtps/__init__.py,sha256=wdqTEDQSlQlLQfPDGuktsVFBTw8H5meL2ntSrX28n2o,260
+dtps/__init__.py,sha256=NMx2F1XK_EzBVjjTkS0_yKbPKQdDOTrmJmpLGSzqJeM,260
 dtps/config.py,sha256=pX8NyQFRER6sxKxiCCNW7rTjUR2lQyg7yi-wcTzwlDA,6709
-dtps/dtps_utils.py,sha256=IFMm9DkKd4FBXGX41Ps0FaA83GfSaLzyOhuVJUVagjk,3733
+dtps/dtps_utils.py,sha256=ap3nmQzbHdeFiC-9YRCCZXwujZAaQtJOy4KimtGvB_E,3735
 dtps/ergo_create.py,sha256=awaOjfX8eVBzK_y2us3WcOTxiS3v3j7XqTVf55UKPk4,11921
 dtps/ergo_ui.py,sha256=lnP4ChQcc2hQkOxDDQEj_FG_SQc2aCEiICEPtRL2dSI,7597
 dtps/ergo_use.py,sha256=GmiZkjqiT4QhA0WprJe4N1tfKaRGD1ND3rgUOmvY4sc,12733
 dtps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dtps/structures.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dtps_http/__init__.py,sha256=3HkCKWG0fHbKBLP7Me9FGHSytTsU3O8WT54nAXsqcGo,655
+dtps_http/__init__.py,sha256=TgMmfqBQ5ktgv7K60pGMTj9kGhLionDOQjh_1B113R0,655
 dtps_http/blob_manager.py,sha256=cHg_4nU1_X7KjBUK6meX0pZkEJ8MCzOw6k1gh1DefzM,4860
 dtps_http/client.py,sha256=hsF32Mw-4zHExK5POp5wKdCDBLL0Yx0aqvfOn7spIwc,62659
 dtps_http/constants.py,sha256=iWSaL75cxZI62Q1oWqzLl9vAK_aaUgBQarFf3bChbbc,3721
 dtps_http/ergo_utils.py,sha256=tVW797yywqleDm9f0yoo8pZXHk5yb-8gr3j9yJQjakI,1365
 dtps_http/exceptions.py,sha256=4w-Yrx-MedOytS_QIpNCiIZRQbFTjyjID-MO-JL_skw,420
 dtps_http/link_headers.py,sha256=ADp5tF-pKU1N7W3M4SISASYTTisL086lTHKYpwDPEo0,1672
 dtps_http/object_queue.py,sha256=MzAERV5fgwtxrFCOwASljEY0rQHaYJwfxoBl4RapHII,10426
@@ -19,22 +19,22 @@
 dtps_http/server_start.py,sha256=fK1pNHPveSCeEw8AV5M6WfVqKHz4nyq4xW1tP9JZCtI,9695
 dtps_http/structures.py,sha256=wjq_7U4Zn9V1h9yJgpZ82ssU6hHgw84miyafCWun4ps,17307
 dtps_http/types.py,sha256=0izHqzwhIqABEFg6lPuf9-fzu8VvxjsukOOlepl9nhQ,3555
 dtps_http/types_of_source.py,sha256=ucrDpQCXlk6QAqKxCNh_E06H6Hn692u3oTpQ-KuI-ZE,21464
 dtps_http/urls.py,sha256=NmGcqCpanRrco1JhPQGNvn-rLG2jIQ9W7J2G9YyisGQ,4336
 dtps_http/utils.py,sha256=V31fI0dQSMuG5UcWuQZcuSlol9oC92ZonN_bx6REHDI,6139
 dtps_http/utils_every_once_in_a_while.py,sha256=nvZsWa1dnK0i8bSkOciUw-VrLxMpT25QZ6pOcXQICig,838
-dtps_http_programs/__init__.py,sha256=hLXtJDTTv68ZeG8AfAU6DVHPcy-HDnoPjYAumPqA-Hc,257
+dtps_http_programs/__init__.py,sha256=ciRD_PR34dCRRlh6qgT5tiD9j92C0IpysGm1UU5hBXc,257
 dtps_http_programs/dtps_listen.py,sha256=2T-CxSAqnC7mdT5AD-bsYqWBggPABefadL_TjxGrBR0,3671
 dtps_http_programs/dtps_proxy.py,sha256=luhDbyOQeFuQOeAXhIB8CjsYhjW8260rHVN2vVWKiTM,1721
 dtps_http_programs/dtps_send_continuous.py,sha256=M4QHRoAUrZ04Rshm11n-g4CUsEeDjvW_UpdRqUHccvo,1338
 dtps_http_programs/dtps_stats.py,sha256=oC8uEjPFhUN1soZ6wkyzmffPPRLuZxrjESsbqfVBN9A,3112
 dtps_http_programs/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dtps_http_programs/server_clock.py,sha256=r7aJJjsXN6Gy26Iy6qw_gs0xQ7RbMlgJBcAhZYFZt7M,1789
 static/favicon.png,sha256=SuoDecEFzJG3RabXtOofSBcIPjDhKVLjFB0UX_LW4tI,1270
 static/send.js,sha256=_dvhwM61lpyrlIDd0-3xeJ59RCPgeLzBcMpeDlNqEms,7885
 static/style.css,sha256=hYKy8n6jh47vqXRg-ljM1x3Ket2rtMhH08TpOIHaW_s,1472
-dtps_http-1.3.4.dist-info/LICENSE.pdf,sha256=V1TBclYda54_miAikuVMwqHoWjwkjHw_yoF2zEqpc_k,75933
-dtps_http-1.3.4.dist-info/METADATA,sha256=7NfSlf35Y5vgheTVZICldsBidXZHBYjreOWmO9B9yDQ,1040
-dtps_http-1.3.4.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-dtps_http-1.3.4.dist-info/entry_points.txt,sha256=0f8h-Ls_gnf01ABr2FNt1iv2hZqrTfchBMIq-hJs6Uc,379
-dtps_http-1.3.4.dist-info/RECORD,,
+dtps_http-1.3.5.dist-info/LICENSE.pdf,sha256=V1TBclYda54_miAikuVMwqHoWjwkjHw_yoF2zEqpc_k,75933
+dtps_http-1.3.5.dist-info/METADATA,sha256=rlCkG0cN8qy1nsh0f-RxvmBHUkoNzcGQzio9wRd3yM0,1040
+dtps_http-1.3.5.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+dtps_http-1.3.5.dist-info/entry_points.txt,sha256=0f8h-Ls_gnf01ABr2FNt1iv2hZqrTfchBMIq-hJs6Uc,379
+dtps_http-1.3.5.dist-info/RECORD,,
```

