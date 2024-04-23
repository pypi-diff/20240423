# Comparing `tmp/phenocv-0.1.3.tar.gz` & `tmp/phenocv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenocv-0.1.3.tar", last modified: Tue Feb 20 04:41:01 2024, max compression
+gzip compressed data, was "phenocv-0.1.4.tar", last modified: Tue Apr 23 05:27:08 2024, max compression
```

## Comparing `phenocv-0.1.3.tar` & `phenocv-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.607360 phenocv-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-02-20 04:39:34.000000 phenocv-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-02-20 04:41:01.607360 phenocv-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-20 04:39:34.000000 phenocv-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.595360 phenocv-0.1.3/phenocv/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.599360 phenocv-0.1.3/phenocv/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/analysis/traits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.599360 phenocv-0.1.3/phenocv/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.595360 phenocv-0.1.3/phenocv/configs/mmdet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.599360 phenocv-0.1.3/phenocv/configs/mmdet/_base_/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/custom_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.599360 phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/cascade-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/faster-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/mask-rcnn_r50_fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.599360 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_100e_onecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_1x.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_20e.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_2x.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_3x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.603360 phenocv-0.1.3/phenocv/configs/mmdet/panicle/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/cascade-rcnn_convnext-t-p4-w7_fpn_2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/cascade-rcnn_r101_fpn_2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/cascade-rcnn_r50_fpn_2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/dino-4scale_r50_8xb2-2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/dino-5scale_swim-l_8xb2-2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_convnext-t-p4-w7_fpn_3x_ms_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_r101_fpn_2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_r50-scratch_fpn_fn-all_6x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_r50_fpn_2x_panicle-full.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/sahi_panicle_headingdate.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/sahi_panicle_num.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/configs/test.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.603360 phenocv-0.1.3/phenocv/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/convert/coco2ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/convert/yolo2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.603360 phenocv-0.1.3/phenocv/predict/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/predict/base_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/predict/yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.603360 phenocv-0.1.3/phenocv/process/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/process/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-20 04:39:34.000000 phenocv-0.1.3/phenocv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 04:41:01.603360 phenocv-0.1.3/phenocv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-02-20 04:41:01.000000 phenocv-0.1.3/phenocv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-20 04:41:01.000000 phenocv-0.1.3/phenocv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 04:41:01.000000 phenocv-0.1.3/phenocv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-20 04:41:01.000000 phenocv-0.1.3/phenocv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 04:41:01.000000 phenocv-0.1.3/phenocv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-02-20 04:39:34.000000 phenocv-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 04:41:01.607360 phenocv-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.318023 phenocv-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-04-23 05:25:32.000000 phenocv-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-23 05:27:08.318023 phenocv-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 05:25:32.000000 phenocv-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.310023 phenocv-0.1.4/phenocv/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.310023 phenocv-0.1.4/phenocv/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/analysis/traits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.310023 phenocv-0.1.4/phenocv/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.306023 phenocv-0.1.4/phenocv/configs/mmdet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.310023 phenocv-0.1.4/phenocv/configs/mmdet/_base_/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/custom_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.310023 phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/cascade-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/faster-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/mask-rcnn_r50_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.314023 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_100e_onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_1x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_20e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_2x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_3x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.314023 phenocv-0.1.4/phenocv/configs/mmdet/panicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/cascade-rcnn_convnext-t-p4-w7_fpn_2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/cascade-rcnn_r101_fpn_2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/cascade-rcnn_r50_fpn_2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/dino-4scale_r50_8xb2-2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/dino-5scale_swim-l_8xb2-2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_convnext-t-p4-w7_fpn_3x_ms_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_r101_fpn_2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_r50-scratch_fpn_fn-all_6x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_r50_fpn_2x_panicle-full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/sahi_panicle_headingdate.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/sahi_panicle_num.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/configs/test.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.314023 phenocv-0.1.4/phenocv/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/convert/coco2ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/convert/yolo2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.314023 phenocv-0.1.4/phenocv/predict/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/predict/base_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/predict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/predict/yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.318023 phenocv-0.1.4/phenocv/process/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/process/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 05:25:32.000000 phenocv-0.1.4/phenocv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 05:27:08.318023 phenocv-0.1.4/phenocv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-23 05:27:08.000000 phenocv-0.1.4/phenocv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-23 05:27:08.000000 phenocv-0.1.4/phenocv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 05:27:08.000000 phenocv-0.1.4/phenocv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 05:27:08.000000 phenocv-0.1.4/phenocv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 05:27:08.000000 phenocv-0.1.4/phenocv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-23 05:25:32.000000 phenocv-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 05:27:08.318023 phenocv-0.1.4/setup.cfg
```

### Comparing `phenocv-0.1.3/LICENSE` & `phenocv-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/PKG-INFO` & `phenocv-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenocv
-Version: 0.1.3
+Version: 0.1.4
 Summary: Rice High Throughput Phenotyping Computer Vision Toolkit
 Author-email: RuLei Chen <chenrulei@cemps.ac.cn>
 Maintainer-email: RuLei Chen <chenrulei@cemps.ac.cn>
 License: AGPL-3.0
 Keywords: machine-learning,deep-learning,computer-vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,16 +50,14 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
-Requires-Dist: mkdocs-redirects; extra == "dev"
-Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
 Provides-Extra: label-studio
 Requires-Dist: label_studio_converter==0.0.55; extra == "label-studio"
 Requires-Dist: label_studio_ml==1.0.9; extra == "label-studio"
 Requires-Dist: label_studio_tools==0.0.3; extra == "label-studio"
 
 # phenocv
 
@@ -91,14 +89,19 @@
 
 ```shell
 git clone https://github.com/r1cheu/phenocv.git
 cd phenocv
 pip install -e .
 ```
 
+## Tutorial
+
+| Getting Start | [![Open In GitHub](https://img.shields.io/badge/Open%20in-GitHub-blue?logo=GitHub)](https://github.com/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) |
+| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+
 ## License
 
 This project is released under the [AGPL 3.0 license](LICENSE).
 
 ## Citation
 
 If you find this project useful in your research, please consider cite:
```

### Comparing `phenocv-0.1.3/README.md` & `phenocv-0.1.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
 ```shell
 git clone https://github.com/r1cheu/phenocv.git
 cd phenocv
 pip install -e .
 ```
 
+## Tutorial
+
+| Getting Start | [![Open In GitHub](https://img.shields.io/badge/Open%20in-GitHub-blue?logo=GitHub)](https://github.com/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) |
+| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+
 ## License
 
 This project is released under the [AGPL 3.0 license](LICENSE).
 
 ## Citation
 
 If you find this project useful in your research, please consider cite:
```

### Comparing `phenocv-0.1.3/phenocv/analysis/traits.py` & `phenocv-0.1.4/phenocv/analysis/traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,9 +191,7 @@
         _img = result_dir / f'{_id}.png'
 
         self.process_images(img_paths, classes, pred_dir=pred_dir)
 
         self.traits = self.postprocess(raw_csv, interp_csv, self.save_file)
         self.extractor.plot(_img)
         self.clear()
-
-        return self.traits
```

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/custom_runtime.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/custom_runtime.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/cascade-rcnn_r50_fpn.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/cascade-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/faster-rcnn_r50_fpn.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/faster-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/models/mask-rcnn_r50_fpn.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/models/mask-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_100e_onecycle.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_100e_onecycle.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_1x.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_1x.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_20e.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_20e.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_2x.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_2x.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/_base_/schedules/schedule_3x.py` & `phenocv-0.1.4/phenocv/configs/mmdet/_base_/schedules/schedule_3x.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/cascade-rcnn_convnext-t-p4-w7_fpn_2x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/cascade-rcnn_convnext-t-p4-w7_fpn_2x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/cascade-rcnn_r50_fpn_2x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/cascade-rcnn_r50_fpn_2x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/dino-4scale_r50_8xb2-2x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/dino-4scale_r50_8xb2-2x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/dino-5scale_swim-l_8xb2-2x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/dino-5scale_swim-l_8xb2-2x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_convnext-t-p4-w7_fpn_3x_ms_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_convnext-t-p4-w7_fpn_3x_ms_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_r50-scratch_fpn_fn-all_6x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_r50-scratch_fpn_fn-all_6x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/mmdet/panicle/faster-rcnn_r50_fpn_2x_panicle-full.py` & `phenocv-0.1.4/phenocv/configs/mmdet/panicle/faster-rcnn_r50_fpn_2x_panicle-full.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/configs/sahi_panicle_headingdate.cfg` & `phenocv-0.1.4/phenocv/configs/sahi_panicle_headingdate.cfg`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/convert/base.py` & `phenocv-0.1.4/phenocv/convert/base.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/convert/coco2ls.py` & `phenocv-0.1.4/phenocv/convert/coco2ls.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/convert/yolo2coco.py` & `phenocv-0.1.4/phenocv/convert/yolo2coco.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/predict/base_yolo.py` & `phenocv-0.1.4/phenocv/predict/base_yolo.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/predict/utils.py` & `phenocv-0.1.4/phenocv/predict/utils.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/predict/yolo.py` & `phenocv-0.1.4/phenocv/predict/yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         # If old box exists, adjust boxes
         if old_box is not None:
             boxes = self._adjust_boxes_with_old_box(boxes, old_box)
 
         return Results(orig_img=orig_img, path=path, names=names, boxes=boxes)
 
     def _prepare_from_results(self, source):
-        img = source.crop_img()[:, :, ::-1]  # convert to RGB
+        img = source.crop_img()  # convert to RGB
         orig_img = source.orig_img
         path = source.path
         old_box, names = self.update_old_box(source)
         return img, orig_img, path, old_box, names
 
     def _prepare_from_path(self, source):
         img = read_image(source, order='RGB')
```

### Comparing `phenocv-0.1.3/phenocv/process/base.py` & `phenocv-0.1.4/phenocv/process/base.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/process/extractor.py` & `phenocv-0.1.4/phenocv/process/extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,33 +121,35 @@
         impute_index = self.data['interpolate'].values
 
         def _plot(ax, x, y, index, color='black'):
             ax.plot(x[~index], y[~index], 'o', color=color)
             ax.plot(x, y, color=color, linestyle='-')
             ax.plot(
                 x[index], y[index], 'o', color=color, markerfacecolor='white')
-            ax.plot(x, self.logistic(x), color='b', linestyle='--')
+            ax.plot(x, self.logistic(x), color='#55A5FF', linestyle='--')
 
-        def _format_ticks(ax, days, dates):
+        def _format_ticks(ax: plt.axes, days, dates):
             selected_days = days[::2]
             selected_dates = dates[::2]
 
-            axes.set_xticks(selected_days)
-            axes.set_xticklabels(
+            ax.set_xticks(selected_days)
+            ax.set_xticklabels(
                 pd.to_datetime(selected_dates).dt.strftime('%m-%d'),
                 rotation=45)
 
             ax.xaxis.set_minor_locator(mdates.DayLocator(interval=1))
             ax.tick_params(axis='x', which='minor', length=2)
 
-            ax.set_xlim(34, 127)
+            ax.set_xlabel('Date')
+            ax.set_ylabel('Number of Panicles')
+
 
         _plot(axes, self.data['days'], self.data['value'], impute_index)
         _format_ticks(axes, self.data['days'], self.data['date'])
         axes.set_title(self.data['id'].iloc[0])
 
         for key in [f"{int(i * 100)}%" for i in self.percents]:
-            axes.axvline(self.result[key], color='b', linestyle='--')
+            axes.axvline(self.result[key], color='#55A5FF', linestyle='--')
 
         plt.tight_layout()
         plt.savefig(save_path, dpi=300)
         plt.close()
```

### Comparing `phenocv-0.1.3/phenocv/process/formatter.py` & `phenocv-0.1.4/phenocv/process/formatter.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/process/postprocessor.py` & `phenocv-0.1.4/phenocv/process/postprocessor.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv/process/preprocess.py` & `phenocv-0.1.4/phenocv/process/preprocess.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,27 +13,56 @@
 
     preprocessor = PanicleUavPreprocessor()
     results = preprocessor('path/to/image')
     or,
     results = preprocessor.results
 
 """
+import logging
 from pathlib import Path
-from typing import Union
+from typing import Tuple, Union
 
 import numpy as np
 import torch
 
 from phenocv.utils import Results, read_image
 
 from .base import Processor
-from .utils import binarize_cive, min_sum, moving_average
+from .utils import binarize_cive, find_min
 
 
-class PanicleUavPreprocessor(Processor):
+class Preprocessor(Processor):
+
+    def __init__(self,
+                 names: Tuple | str = None):
+        super().__init__()
+
+        if names is None:
+            logging.warning('No names provided, using default names')
+            self.names = {0: "NoName"}
+        if isinstance(names, str):
+            self.names = {0: names}
+        if isinstance(names, tuple):
+            self.names = {i: name for i, name in enumerate(names)}
+
+    def __call__(self, img_path: Union[str, Path]):
+        img = read_image(img_path, order='RGB')
+        boxes = self.process(img)
+
+        self._result = Results(
+            orig_img=img,
+            names=self.names,
+            path=img_path,
+            boxes=boxes,
+        )
+
+        return self.result
+
+
+class PrePanicleUavHW(Preprocessor):
     """Preprocess the image from the UAV, which need to locate the central
     plot of the image. The image is first binarized with CIVE, then the
     image is cropped to the region of interest.
 
     Attributes:
         height (int): The expected height of the plot.
         width (int): The expected width of the plot.
@@ -43,47 +72,55 @@
     """
 
     def __init__(
         self,
         width: int = 3800,
         height: int = 2000,
         window_size: int = 100,
+        names: Tuple[str] = ('plot', ),
     ):
-        super().__init__()
+        super().__init__(names=names)
         self.height = height
         self.width = width
         self.window_size = window_size
-        self.names = {0: "plot"}
 
-    def __call__(self, img_path: Union[str, Path]):
-        """using the CIVE to binarize the image, then find the minimum
-        sum of the binarized image to locate the plot.
+    def process(self, img: np.ndarray):
+        bin_image = binarize_cive(img)
 
-        Args:
-            img_path (str or Path): The path to the image.
-        """
-        img = read_image(img_path)
-        boxes = self.process(img)
+        x1, x2 = find_min(bin_image, 0, self.window_size, self.width)
+        y1, y2 = find_min(bin_image, 1, self.window_size, self.height)
 
-        self._result = Results(
-            orig_img=img,
-            names=self.names,
-            path=img_path,
-            boxes=boxes,
-        )
+        return torch.tensor([[x1, y1, x2, y2, 0, 0]])
 
-        return self.result
+
+class PrePanicleUav(Preprocessor):
+
+    def __init__(self,
+                 window_size: int = 100,
+                 w_ratio: float = 2,
+                 names: Tuple[str] = ('plot', )):
+        super().__init__(names=names)
+        self.window_size = window_size
+        self.w_ratio = w_ratio
 
     def process(self, img: np.ndarray):
+
         bin_image = binarize_cive(img)
 
-        x = np.apply_along_axis(np.sum, 0, bin_image)
-        x = moving_average(x, self.window_size)
-        x1, x2 = min_sum(x, self.width, self.window_size)
+        up, down = self.cut_2_image(bin_image)
+
+        y1 = find_min(up, 1, self.window_size)
+        y2 = find_min(down, 1, self.window_size) + bin_image.shape[0] // 2
+        width = int((y2 - y1) * self.w_ratio)
+        x1, x2 = find_min(bin_image, 0, self.window_size, width)
+
+        return torch.tensor([[x1, y1, x2, y2, 0, 0]])
+
+    @staticmethod
+    def cut_2_image(img):
 
-        y = np.apply_along_axis(np.sum, 1, bin_image)
-        y = moving_average(y, self.window_size)
-        y1, y2 = min_sum(y, self.height, self.window_size)
+        half_h = img.shape[0] // 2
 
-        boxes = torch.tensor([[x1, y1, x2, y2, 0, 0]])
+        up = img[:half_h, :]
+        down = img[half_h:, :]
 
-        return boxes
+        return up, down
```

### Comparing `phenocv-0.1.3/phenocv/process/utils.py` & `phenocv-0.1.4/phenocv/process/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
     Returns:
     numpy.ndarray: The binarize image.
     """
     r, g, b = cv2.split(img)
     cive = 0.441 * r - 0.811 * g + 0.385 * b + 18.78745
     gray = cive.astype('uint8')
-    _, th = cv2.threshold(gray, 0, 1, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+    _, th = cv2.threshold(gray, 0, 1,
+                          cv2.THRESH_BINARY + cv2.THRESH_OTSU)
     return th
 
 
 def moving_average(interval, window_size):
     """Calculate the moving average of a given interval.
 
     Parameters:
@@ -48,29 +49,46 @@
     array-like: The moving average of the path interval.
     """
     window = np.ones(int(window_size)) / float(window_size)
     re = np.convolve(interval, window, 'valid')
     return re
 
 
-def min_sum(x, length, window_size):
+def min_sum(x, window_size, board_interval=None):
     """Calculate the index range with the minimum sum of a given array.
 
     Parameters:
     x (array-like): The path array.
     length (int): The length of the index range.
     window_size (int): The window size for moving average.
 
     Returns:
     tuple: A tuple containing the start and end index of the range with
         the minimum sum.
     """
-    i_sum = x[:-length] + x[length:]
-    index = np.argmin(i_sum) + window_size
-    return index, index + length
+    if board_interval:
+        i_sum = x[:-board_interval] + x[board_interval:]
+        index = np.argmin(i_sum) + window_size
+        return index, index + board_interval
+    else:
+        index = np.argmin(x) + window_size
+        return index
+
+
+def find_min(bin_image, axis, window_size, board_interval=None) -> tuple[int, int] | int :
+
+    bin_image = np.apply_along_axis(np.sum, axis, bin_image)
+    bin_image = moving_average(bin_image, window_size)
+
+    if board_interval:
+        start, end = min_sum(bin_image, window_size, board_interval)
+        return start, end
+    else:
+        start = min_sum(bin_image, window_size)
+        return start
 
 
 def cut_up_curve(df: pd.DataFrame):
     start_idx = df[df['value'] == 0].index.max()
     end_idx = df['value'].idxmax()
     assert (start_idx < end_idx), 'start_idx should be smaller than ' \
                                   'end_idx'
```

### Comparing `phenocv-0.1.3/phenocv/registry.py` & `phenocv-0.1.4/phenocv/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 from typing import Tuple, Union
 
 import catalogue
 from confection import Config, registry
 
 from phenocv.predict import YoloSahiPanicleUavPredictor
 from phenocv.process import (IdDateFormatter, NaiveFormatter, PanicleExtractor,
-                             PaniclePostprocessor, PanicleUavPreprocessor)
+                             PaniclePostprocessor, PrePanicleUav,
+                             PrePanicleUavHW)
 
 registry.preprocessor = catalogue.create("phenocv", "preprocessor")
 registry.predictor = catalogue.create("phenocv", "predictor")
 registry.formatter = catalogue.create("phenocv", "formatter")
 registry.postprocessor = catalogue.create("phenocv", "postprocessor")
 registry.extractor = catalogue.create("phenocv", "extractor")
 
 
-@registry.preprocessor.register('panicle_uav')
-def panicle_uav_preprocessor(
+@registry.preprocessor.register('panicle_uav_hw')
+def panicle_uav_hw_pre(
     width: int = 3800,
     height: int = 2000,
     window_size: int = 100,
-) -> PanicleUavPreprocessor:
-    return PanicleUavPreprocessor(
+    names: Tuple[str] | str = 'plot'
+) -> PrePanicleUavHW:
+    return PrePanicleUavHW(
         width=width,
         height=height,
         window_size=window_size,
+        names=names
     )
 
 
+@registry.preprocessor.register('panicle_uav')
+def panicle_uav_pre(
+    window_size: int = 100,
+    w_ratio: float = 1.8,
+    names: Tuple[str] | str = 'plot'
+) -> PrePanicleUav:
+    return PrePanicleUav(
+        window_size=window_size,
+        w_ratio=w_ratio,
+        names=names)
+
+
 @registry.predictor.register('yolo_sahi_panicle_uav')
 def yolo_sahi_panicle_uav_predictor(
     model_type: str,
     model_weight: str,
     device: int | Tuple[int] = 0,
     conf=0.25,
     iou=0.7,
```

### Comparing `phenocv-0.1.3/phenocv/utils.py` & `phenocv-0.1.4/phenocv/utils.py`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/phenocv.egg-info/PKG-INFO` & `phenocv-0.1.4/phenocv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenocv
-Version: 0.1.3
+Version: 0.1.4
 Summary: Rice High Throughput Phenotyping Computer Vision Toolkit
 Author-email: RuLei Chen <chenrulei@cemps.ac.cn>
 Maintainer-email: RuLei Chen <chenrulei@cemps.ac.cn>
 License: AGPL-3.0
 Keywords: machine-learning,deep-learning,computer-vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,16 +50,14 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
-Requires-Dist: mkdocs-redirects; extra == "dev"
-Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
 Provides-Extra: label-studio
 Requires-Dist: label_studio_converter==0.0.55; extra == "label-studio"
 Requires-Dist: label_studio_ml==1.0.9; extra == "label-studio"
 Requires-Dist: label_studio_tools==0.0.3; extra == "label-studio"
 
 # phenocv
 
@@ -91,14 +89,19 @@
 
 ```shell
 git clone https://github.com/r1cheu/phenocv.git
 cd phenocv
 pip install -e .
 ```
 
+## Tutorial
+
+| Getting Start | [![Open In GitHub](https://img.shields.io/badge/Open%20in-GitHub-blue?logo=GitHub)](https://github.com/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/r1cheu/phenocv/blob/main/tutorial/getting_start.ipynb) |
+| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+
 ## License
 
 This project is released under the [AGPL 3.0 license](LICENSE).
 
 ## Citation
 
 If you find this project useful in your research, please consider cite:
```

### Comparing `phenocv-0.1.3/phenocv.egg-info/SOURCES.txt` & `phenocv-0.1.4/phenocv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenocv-0.1.3/pyproject.toml` & `phenocv-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -68,16 +68,14 @@
     "pre-commit",
     "pytest",
     "pytest-cov",
     "coverage[toml]",
     "mkdocs-material",
     "mkdocstrings[python]",
     "mkdocs-jupyter", # for notebooks
-    "mkdocs-redirects", # for 301 redirects
-    "mkdocs-ultralytics-plugin>=0.0.42", # for meta descriptions and test_images, dates and authors
 ]
 
 label_studio = [
     "label_studio_converter==0.0.55",
     "label_studio_ml==1.0.9",
     "label_studio_tools==0.0.3",
 ]
```

