# Comparing `tmp/robust_extraction-0.1.8.tar.gz` & `tmp/robust_extraction-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robust_extraction-0.1.8.tar", last modified: Sun Apr 21 17:16:53 2024, max compression
+gzip compressed data, was "robust_extraction-0.1.9.tar", last modified: Mon Apr 22 10:40:02 2024, max compression
```

## Comparing `robust_extraction-0.1.8.tar` & `robust_extraction-0.1.9.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust_extraction-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      706 2024-04-21 17:16:50.000000 robust_extraction-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.169880 robust_extraction-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:34:41.000000 robust_extraction-0.1.8/src/robust_extraction/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      327 2024-04-21 16:41:44.000000 robust_extraction-0.1.8/src/robust_extraction/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/contours/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:18:52.000000 robust_extraction-0.1.8/src/robust_extraction/contours/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-21 16:41:39.000000 robust_extraction-0.1.8/src/robust_extraction/contours/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3294 2024-04-21 17:14:36.000000 robust_extraction-0.1.8/src/robust_extraction/contours/contours.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-04-21 16:41:32.000000 robust_extraction-0.1.8/src/robust_extraction/contours/rois.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      135 2024-04-21 16:19:36.000000 robust_extraction-0.1.8/src/robust_extraction/contours/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/lines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/clustering.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/metrics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/segmentation.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1594 2024-04-21 17:16:09.000000 robust_extraction-0.1.8/src/robust_extraction/lines/cluster/inclination.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/lines/coverage/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/coverage/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/coverage/coverage.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/directions.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.179880 robust_extraction-0.1.8/src/robust_extraction/lines/draw/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/draw/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      349 2024-04-21 17:15:37.000000 robust_extraction-0.1.8/src/robust_extraction/lines/draw/clustered.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust_extraction-0.1.8/src/robust_extraction/lines/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3738 2024-04-21 17:14:56.000000 robust_extraction-0.1.8/src/robust_extraction/lines/instersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1270 2024-04-21 16:29:37.000000 robust_extraction-0.1.8/src/robust_extraction/lines/points.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/lines/poly/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/poly/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/lines/poly/intersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust_extraction-0.1.8/src/robust_extraction/lines/poly/poly.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/manual/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       83 2024-04-21 16:41:01.000000 robust_extraction-0.1.8/src/robust_extraction/manual/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      445 2024-04-21 16:40:14.000000 robust_extraction-0.1.8/src/robust_extraction/manual/_correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1282 2024-04-21 16:40:29.000000 robust_extraction-0.1.8/src/robust_extraction/manual/_extract.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/match1d/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/match1d/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust_extraction-0.1.8/src/robust_extraction/match1d/st_lap.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/perspective/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:22:50.000000 robust_extraction-0.1.8/src/robust_extraction/perspective/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-04-21 16:28:05.000000 robust_extraction-0.1.8/src/robust_extraction/perspective/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3766 2024-04-11 16:09:23.000000 robust_extraction-0.1.8/src/robust_extraction/perspective/perspective.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4545 2024-04-21 16:21:59.000000 robust_extraction-0.1.8/src/robust_extraction/perspective/perspective2.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:22:10.000000 robust_extraction-0.1.8/src/robust_extraction/perspective/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/pipeline/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:41:20.000000 robust_extraction-0.1.8/src/robust_extraction/pipeline/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      963 2024-04-17 13:41:53.000000 robust_extraction-0.1.8/src/robust_extraction/pipeline/ret.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2633 2024-04-21 16:34:11.000000 robust_extraction-0.1.8/src/robust_extraction/pipeline/v6.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3124 2024-04-21 16:41:18.000000 robust_extraction-0.1.8/src/robust_extraction/pipeline/v7.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/templates/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-01-25 18:20:54.000000 robust_extraction-0.1.8/src/robust_extraction/templates/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/templates/_models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/templates/_models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      238 2024-01-25 18:23:21.000000 robust_extraction-0.1.8/src/robust_extraction/templates/_models/_models.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/templates/_models/fcde.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/templates/_models/llobregat23.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust_extraction-0.1.8/src/robust_extraction/templates/templates.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction/vectors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust_extraction-0.1.8/src/robust_extraction/vectors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-04-21 16:17:53.000000 robust_extraction-0.1.8/src/robust_extraction/vectors/vectors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 17:16:53.189880 robust_extraction-0.1.8/src/robust_extraction.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-21 17:16:53.000000 robust_extraction-0.1.8/src/robust_extraction.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2365 2024-04-21 17:16:53.000000 robust_extraction-0.1.8/src/robust_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 17:16:53.000000 robust_extraction-0.1.8/src/robust_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      117 2024-04-21 17:16:53.000000 robust_extraction-0.1.8/src/robust_extraction.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-21 17:16:53.000000 robust_extraction-0.1.8/src/robust_extraction.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.945235 robust_extraction-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-22 10:40:02.945235 robust_extraction-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust_extraction-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      706 2024-04-22 10:39:59.000000 robust_extraction-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:40:02.945235 robust_extraction-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.905235 robust_extraction-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.915235 robust_extraction-0.1.9/src/robust_extraction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:34:41.000000 robust_extraction-0.1.9/src/robust_extraction/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      373 2024-04-22 10:39:43.000000 robust_extraction-0.1.9/src/robust_extraction/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/contours/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:18:52.000000 robust_extraction-0.1.9/src/robust_extraction/contours/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-21 16:41:39.000000 robust_extraction-0.1.9/src/robust_extraction/contours/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3294 2024-04-21 17:14:36.000000 robust_extraction-0.1.9/src/robust_extraction/contours/contours.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-04-21 16:41:32.000000 robust_extraction-0.1.9/src/robust_extraction/contours/rois.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      135 2024-04-21 16:19:36.000000 robust_extraction-0.1.9/src/robust_extraction/contours/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/clustering.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/metrics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/segmentation.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1594 2024-04-21 17:16:09.000000 robust_extraction-0.1.9/src/robust_extraction/lines/cluster/inclination.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/coverage/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/coverage/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/coverage/coverage.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/directions.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/draw/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/draw/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      349 2024-04-21 17:15:37.000000 robust_extraction-0.1.9/src/robust_extraction/lines/draw/clustered.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust_extraction-0.1.9/src/robust_extraction/lines/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3738 2024-04-21 17:14:56.000000 robust_extraction-0.1.9/src/robust_extraction/lines/instersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1270 2024-04-21 16:29:37.000000 robust_extraction-0.1.9/src/robust_extraction/lines/points.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/lines/poly/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/poly/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/lines/poly/intersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust_extraction-0.1.9/src/robust_extraction/lines/poly/poly.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/manual/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       83 2024-04-21 16:41:01.000000 robust_extraction-0.1.9/src/robust_extraction/manual/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      445 2024-04-21 16:40:14.000000 robust_extraction-0.1.9/src/robust_extraction/manual/_correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1282 2024-04-21 16:40:29.000000 robust_extraction-0.1.9/src/robust_extraction/manual/_extract.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.925235 robust_extraction-0.1.9/src/robust_extraction/match1d/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/match1d/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust_extraction-0.1.9/src/robust_extraction/match1d/st_lap.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.935235 robust_extraction-0.1.9/src/robust_extraction/perspective/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 16:22:50.000000 robust_extraction-0.1.9/src/robust_extraction/perspective/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-04-21 16:28:05.000000 robust_extraction-0.1.9/src/robust_extraction/perspective/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3766 2024-04-11 16:09:23.000000 robust_extraction-0.1.9/src/robust_extraction/perspective/perspective.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4545 2024-04-21 16:21:59.000000 robust_extraction-0.1.9/src/robust_extraction/perspective/perspective2.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:22:10.000000 robust_extraction-0.1.9/src/robust_extraction/perspective/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.935235 robust_extraction-0.1.9/src/robust_extraction/pipeline/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-04-21 16:41:20.000000 robust_extraction-0.1.9/src/robust_extraction/pipeline/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      963 2024-04-17 13:41:53.000000 robust_extraction-0.1.9/src/robust_extraction/pipeline/ret.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2633 2024-04-21 16:34:11.000000 robust_extraction-0.1.9/src/robust_extraction/pipeline/v6.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3124 2024-04-21 16:41:18.000000 robust_extraction-0.1.9/src/robust_extraction/pipeline/v7.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.935235 robust_extraction-0.1.9/src/robust_extraction/templates/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 10:39:18.000000 robust_extraction-0.1.9/src/robust_extraction/templates/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      210 2024-04-22 10:39:22.000000 robust_extraction-0.1.9/src/robust_extraction/templates/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.935235 robust_extraction-0.1.9/src/robust_extraction/templates/_models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 10:38:59.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-04-22 10:38:48.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      193 2024-04-22 10:38:24.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/_models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/fcde.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-22 10:37:39.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/id.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/templates/_models/llobregat23.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust_extraction-0.1.9/src/robust_extraction/templates/templates.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.935235 robust_extraction-0.1.9/src/robust_extraction/vectors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust_extraction-0.1.9/src/robust_extraction/vectors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-04-21 16:17:53.000000 robust_extraction-0.1.9/src/robust_extraction/vectors/vectors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:40:02.945235 robust_extraction-0.1.9/src/robust_extraction.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-22 10:40:02.000000 robust_extraction-0.1.9/src/robust_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2509 2024-04-22 10:40:02.000000 robust_extraction-0.1.9/src/robust_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:40:02.000000 robust_extraction-0.1.9/src/robust_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      117 2024-04-22 10:40:02.000000 robust_extraction-0.1.9/src/robust_extraction.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-22 10:40:02.000000 robust_extraction-0.1.9/src/robust_extraction.egg-info/top_level.txt
```

### Comparing `robust_extraction-0.1.8/PKG-INFO` & `robust_extraction-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/robust-extraction.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
```

### Comparing `robust_extraction-0.1.8/pyproject.toml` & `robust_extraction-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robust-extraction"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Automatic preprocessing of chess scoresheets"
 dependencies = [
   "ramda", "numpy", "haskellian", "pure-cv", "pydantic",
   "networkx", "scipy", "opencv-python", "scikit-learn", "py_jaxtyping", "jaxtyping", "lazy-loader"
```

### Comparing `robust_extraction-0.1.8/src/robust_extraction/contours/contours.py` & `robust_extraction-0.1.9/src/robust_extraction/contours/contours.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/contours/rois.py` & `robust_extraction-0.1.9/src/robust_extraction/contours/rois.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/__init__.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/clustering.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/clustering.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/metrics.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/metrics.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/cluster/collinear/segmentation.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/cluster/collinear/segmentation.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/cluster/inclination.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/cluster/inclination.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/coverage/coverage.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/directions.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/directions.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/extract.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/extract.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/instersections.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/instersections.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/points.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/points.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/poly/intersections.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/poly/intersections.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/lines/poly/poly.py` & `robust_extraction-0.1.9/src/robust_extraction/lines/poly/poly.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/manual/_extract.py` & `robust_extraction-0.1.9/src/robust_extraction/manual/_extract.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/match1d/st_lap.py` & `robust_extraction-0.1.9/src/robust_extraction/match1d/st_lap.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/perspective/perspective.py` & `robust_extraction-0.1.9/src/robust_extraction/perspective/perspective.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/perspective/perspective2.py` & `robust_extraction-0.1.9/src/robust_extraction/perspective/perspective2.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/pipeline/ret.py` & `robust_extraction-0.1.9/src/robust_extraction/pipeline/ret.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/pipeline/v6.py` & `robust_extraction-0.1.9/src/robust_extraction/pipeline/v6.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/pipeline/v7.py` & `robust_extraction-0.1.9/src/robust_extraction/pipeline/v7.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction/templates/templates.py` & `robust_extraction-0.1.9/src/robust_extraction/templates/templates.py`

 * *Files identical despite different names*

### Comparing `robust_extraction-0.1.8/src/robust_extraction.egg-info/PKG-INFO` & `robust_extraction-0.1.9/src/robust_extraction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/robust-extraction.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
```

### Comparing `robust_extraction-0.1.8/src/robust_extraction.egg-info/SOURCES.txt` & `robust_extraction-0.1.9/src/robust_extraction.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 src/robust_extraction/perspective/perspective2.py
 src/robust_extraction/perspective/types.py
 src/robust_extraction/pipeline/__init__.py
 src/robust_extraction/pipeline/ret.py
 src/robust_extraction/pipeline/v6.py
 src/robust_extraction/pipeline/v7.py
 src/robust_extraction/templates/__init__.py
+src/robust_extraction/templates/__init__.pyi
 src/robust_extraction/templates/templates.py
 src/robust_extraction/templates/_models/__init__.py
+src/robust_extraction/templates/_models/__init__.pyi
 src/robust_extraction/templates/_models/_models.py
 src/robust_extraction/templates/_models/fcde.py
+src/robust_extraction/templates/_models/id.py
 src/robust_extraction/templates/_models/llobregat23.py
 src/robust_extraction/vectors/__init__.py
 src/robust_extraction/vectors/vectors.py
```

