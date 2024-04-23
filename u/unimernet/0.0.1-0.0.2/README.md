# Comparing `tmp/unimernet-0.0.1-py2.py3-none-any.whl.zip` & `tmp/unimernet-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2226198 bytes, number of entries: 69
+Zip file size: 2226225 bytes, number of entries: 69
 -rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 test.py
 -rw-r--r--  2.0 unx     2750 b- defN 80-Jan-01 00:00 train.py
 -rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 unimernet/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/common/__init__.py
 -rw-r--r--  2.0 unx    15074 b- defN 80-Jan-01 00:00 unimernet/common/config.py
 -rw-r--r--  2.0 unx     3614 b- defN 80-Jan-01 00:00 unimernet/common/dist_utils.py
 -rw-r--r--  2.0 unx      815 b- defN 80-Jan-01 00:00 unimernet/common/gradcam.py
@@ -59,13 +59,13 @@
 -rw-r--r--  2.0 unx    11292 b- defN 80-Jan-01 00:00 unimernet/processors/randaugment.py
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 unimernet/runners/__init__.py
 -rw-r--r--  2.0 unx    23307 b- defN 80-Jan-01 00:00 unimernet/runners/runner_base.py
 -rw-r--r--  2.0 unx    11842 b- defN 80-Jan-01 00:00 unimernet/runners/runner_iter.py
 -rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 unimernet/tasks/__init__.py
 -rw-r--r--  2.0 unx     9180 b- defN 80-Jan-01 00:00 unimernet/tasks/base_task.py
 -rw-r--r--  2.0 unx     6318 b- defN 80-Jan-01 00:00 unimernet/tasks/unimernet_train.py
--rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7565 b- defN 80-Jan-01 00:00 unimernet-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 unimernet-0.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6544 b- defN 16-Jan-01 00:00 unimernet-0.0.1.dist-info/RECORD
-69 files, 2619997 bytes uncompressed, 2215592 bytes compressed:  15.4%
+-rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7646 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 unimernet-0.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6544 b- defN 16-Jan-01 00:00 unimernet-0.0.2.dist-info/RECORD
+69 files, 2620078 bytes uncompressed, 2215619 bytes compressed:  15.4%
```

## zipnote {}

```diff
@@ -186,23 +186,23 @@
 
 Filename: unimernet/tasks/base_task.py
 Comment: 
 
 Filename: unimernet/tasks/unimernet_train.py
 Comment: 
 
-Filename: unimernet-0.0.1.dist-info/LICENSE
+Filename: unimernet-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: unimernet-0.0.1.dist-info/METADATA
+Filename: unimernet-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: unimernet-0.0.1.dist-info/WHEEL
+Filename: unimernet-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: unimernet-0.0.1.dist-info/entry_points.txt
+Filename: unimernet-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: unimernet-0.0.1.dist-info/RECORD
+Filename: unimernet-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `unimernet-0.0.1.dist-info/LICENSE` & `unimernet-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unimernet-0.0.1.dist-info/METADATA` & `unimernet-0.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimernet
-Version: 0.0.1
+Version: 0.0.2
 Summary: UniMERNet: A Universal Network for Real-World Mathematical Expression Recognition
 Home-page: https://github.com/xxx
 License: Apache-2.0
 Keywords: MER,latex,markdown,pdf
 Author: Bin Wang
 Author-email: ictwangbin@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,14 +26,16 @@
 Requires-Dist: fairscale (>=0.4.13,<0.5.0)
 Requires-Dist: ftfy (>=6.2.0,<7.0.0)
 Requires-Dist: iopath (>=0.1.10,<0.2.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.9.0,<5.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: timm (>=0.9.16,<0.10.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: torchtext (>=0.17.2,<0.18.0)
 Requires-Dist: torchvision (>=0.17.2,<0.18.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
 Requires-Dist: wand (>=0.6.13,<0.7.0)
```

## Comparing `unimernet-0.0.1.dist-info/RECORD` & `unimernet-0.0.2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -58,12 +58,12 @@
 unimernet/processors/randaugment.py,sha256=mNaXux-SCMNBYIubeG9k9YRxIkv7p6JMecTJqq4AabM,11292
 unimernet/runners/__init__.py,sha256=RXvSvxFZ2_Q5Lq_0OHe8x53uiLC6vO-SgVmtiKZnEeY,368
 unimernet/runners/runner_base.py,sha256=XN1OLAq5t68u5-BCVnALXnhZSVFDLur7z0CyIpSSti8,23307
 unimernet/runners/runner_iter.py,sha256=tz88ZTLymApeEe5A-wVynscWuc7uTymQFngCxI2Tqes,11842
 unimernet/tasks/__init__.py,sha256=5_T40TR9RVIURJDppFO-fgQjUxygtlvEtZpoZFEKLp4,717
 unimernet/tasks/base_task.py,sha256=FujbWh9o6a4tnDIR3pSYPqSnkTppGPhmdg9648AsVcE,9180
 unimernet/tasks/unimernet_train.py,sha256=ut8QUVOPgnLbiuGfIpHbM4SJwbmVr2SbVvR_q46AzjQ,6318
-unimernet-0.0.1.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
-unimernet-0.0.1.dist-info/METADATA,sha256=VjYq4eRUh7VqBPh2FBooT4RxEnQtMJ3v7neRW0w2zTI,7565
-unimernet-0.0.1.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
-unimernet-0.0.1.dist-info/entry_points.txt,sha256=_OsnCi4ChrM_8ss-TzUkaPxwqMLI2I5ve5SoCcCKc-w,104
-unimernet-0.0.1.dist-info/RECORD,,
+unimernet-0.0.2.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
+unimernet-0.0.2.dist-info/METADATA,sha256=BrwJVMOHVVCt6Zz3STpe9pNQKaPqHobkrizGTukgc6c,7646
+unimernet-0.0.2.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
+unimernet-0.0.2.dist-info/entry_points.txt,sha256=_OsnCi4ChrM_8ss-TzUkaPxwqMLI2I5ve5SoCcCKc-w,104
+unimernet-0.0.2.dist-info/RECORD,,
```

