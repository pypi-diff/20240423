# Comparing `tmp/trajectopy_core-2.7.0.tar.gz` & `tmp/trajectopy_core-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy_core-2.7.0.tar", max compression
+gzip compressed data, was "trajectopy_core-3.0.0.tar", max compression
```

## Comparing `trajectopy_core-2.7.0.tar` & `trajectopy_core-3.0.0.tar`

### file list

```diff
@@ -1,78 +1,72 @@
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-2.7.0/LICENSE
--rw-r--r--   0        0        0     1049 2024-04-18 14:05:54.819712 trajectopy_core-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    33078 2024-02-02 14:24:47.281805 trajectopy_core-2.7.0/README.md
--rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-2.7.0/trajectopy_core/__init__.py
--rw-r--r--   0        0        0       49 2023-11-08 14:24:59.343660 trajectopy_core-2.7.0/trajectopy_core/alignment/__init__.py
--rw-r--r--   0        0        0    10137 2024-04-18 14:05:54.820715 trajectopy_core-2.7.0/trajectopy_core/alignment/actions.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.344660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/__init__.py
--rw-r--r--   0        0        0     2435 2023-11-29 11:29:09.869840 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/helmert_transformation.py
--rw-r--r--   0        0        0     5318 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/leverarm.py
--rw-r--r--   0        0        0     2163 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/direct/timeshift.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.345660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/__init__.py
--rw-r--r--   0        0        0    19496 2024-04-18 14:05:54.821747 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/data.py
--rw-r--r--   0        0        0    36416 2024-04-18 14:05:54.821747 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/estimation.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/__init__.py
--rw-r--r--   0        0        0    16133 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/equations.py
--rw-r--r--   0        0        0     8549 2023-11-08 14:24:59.347660 trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/interface.py
--rw-r--r--   0        0        0    23827 2023-11-29 11:29:09.870840 trajectopy_core-2.7.0/trajectopy_core/alignment/parameters.py
--rw-r--r--   0        0        0     2833 2023-11-08 14:24:59.349660 trajectopy_core-2.7.0/trajectopy_core/alignment/result.py
--rw-r--r--   0        0        0     1021 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/alignment/rotation_alignment.py
--rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-2.7.0/trajectopy_core/alignment/utils.py
--rw-r--r--   0        0        0        0 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/approximation/__init__.py
--rw-r--r--   0        0        0     9308 2023-11-29 11:29:09.871841 trajectopy_core-2.7.0/trajectopy_core/approximation/cubic_approximation.py
--rw-r--r--   0        0        0     6608 2023-11-29 11:29:09.872840 trajectopy_core-2.7.0/trajectopy_core/approximation/math_utils.py
--rw-r--r--   0        0        0     3880 2023-11-29 11:29:09.872840 trajectopy_core-2.7.0/trajectopy_core/approximation/mls_approximation.py
--rw-r--r--   0        0        0     2151 2023-11-29 11:29:09.873840 trajectopy_core-2.7.0/trajectopy_core/approximation/rot_approximation.py
--rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-2.7.0/trajectopy_core/approximation/voxelizer.py
--rw-r--r--   0        0        0     2001 2024-04-18 14:05:54.822747 trajectopy_core-2.7.0/trajectopy_core/definitions.py
--rw-r--r--   0        0        0      112 2023-11-08 14:24:59.350662 trajectopy_core-2.7.0/trajectopy_core/evaluation/__init__.py
--rw-r--r--   0        0        0    15142 2023-12-04 13:28:15.723893 trajectopy_core-2.7.0/trajectopy_core/evaluation/ate_result.py
--rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-2.7.0/trajectopy_core/evaluation/comparison.py
--rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-2.7.0/trajectopy_core/evaluation/deviations.py
--rw-r--r--   0        0        0     9981 2023-12-04 09:19:20.545163 trajectopy_core-2.7.0/trajectopy_core/evaluation/rpe_result.py
--rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-2.7.0/trajectopy_core/evaluation/utils.py
--rw-r--r--   0        0        0        0 2023-10-09 11:26:32.327576 trajectopy_core-2.7.0/trajectopy_core/io/__init__.py
--rw-r--r--   0        0        0     5273 2023-11-29 11:29:09.876841 trajectopy_core-2.7.0/trajectopy_core/io/header.py
--rw-r--r--   0        0        0     3021 2023-11-29 11:29:09.877841 trajectopy_core-2.7.0/trajectopy_core/io/rosbag.py
--rw-r--r--   0        0        0     1197 2023-10-09 11:26:32.328577 trajectopy_core-2.7.0/trajectopy_core/io/rosmsg.py
--rw-r--r--   0        0        0    11291 2023-11-29 11:29:09.877841 trajectopy_core-2.7.0/trajectopy_core/io/trajectory_io.py
--rw-r--r--   0        0        0     1118 2023-11-29 11:29:09.878841 trajectopy_core-2.7.0/trajectopy_core/io/utils.py
--rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-2.7.0/trajectopy_core/kml.py
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-2.7.0/trajectopy_core/LICENSE
--rw-r--r--   0        0        0     9635 2024-04-18 14:05:54.822747 trajectopy_core-2.7.0/trajectopy_core/matching.py
--rw-r--r--   0        0        0     6433 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/pipelines.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-2.7.0/trajectopy_core/plotting/__init__.py
--rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-2.7.0/trajectopy_core/plotting/bar_plots.py
--rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-2.7.0/trajectopy_core/plotting/heatmaps.py
--rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-2.7.0/trajectopy_core/plotting/histograms.py
--rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-2.7.0/trajectopy_core/plotting/line_plots.py
--rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-2.7.0/trajectopy_core/plotting/multi_line_plots.py
--rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-2.7.0/trajectopy_core/plotting/scatter_plots.py
--rw-r--r--   0        0        0     1626 2023-11-29 11:29:09.880840 trajectopy_core-2.7.0/trajectopy_core/plotting/tables.py
--rw-r--r--   0        0        0     1727 2023-12-04 13:28:15.725896 trajectopy_core-2.7.0/trajectopy_core/plotting/utils.py
--rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-2.7.0/trajectopy_core/report/__init__.py
--rw-r--r--   0        0        0     2441 2024-02-02 14:24:47.286809 trajectopy_core-2.7.0/trajectopy_core/report/alignment.py
--rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-2.7.0/trajectopy_core/report/assets/icon.png
--rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-2.7.0/trajectopy_core/report/assets/style.css
--rw-r--r--   0        0        0     6220 2024-02-02 14:24:47.287810 trajectopy_core-2.7.0/trajectopy_core/report/data.py
--rw-r--r--   0        0        0     3640 2024-02-02 14:24:47.287810 trajectopy_core-2.7.0/trajectopy_core/report/multi.py
--rw-r--r--   0        0        0     5286 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/single.py
--rw-r--r--   0        0        0     4660 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/templates/generic.html
--rw-r--r--   0        0        0     5616 2024-02-02 14:24:47.288807 trajectopy_core-2.7.0/trajectopy_core/report/templates/multi_template.html
--rw-r--r--   0        0        0     7282 2024-02-02 14:24:47.289808 trajectopy_core-2.7.0/trajectopy_core/report/templates/single_template.html
--rw-r--r--   0        0        0     1999 2024-01-22 14:08:45.548680 trajectopy_core-2.7.0/trajectopy_core/report/trajectory.py
--rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-2.7.0/trajectopy_core/report/utils.py
--rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-2.7.0/trajectopy_core/rotationset.py
--rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-2.7.0/trajectopy_core/settings/__init__.py
--rw-r--r--   0        0        0     8889 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/settings/alignment.py
--rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-2.7.0/trajectopy_core/settings/approximation.py
--rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-2.7.0/trajectopy_core/settings/base.py
--rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-2.7.0/trajectopy_core/settings/comparison.py
--rw-r--r--   0        0        0     1164 2024-04-18 14:05:54.823745 trajectopy_core-2.7.0/trajectopy_core/settings/matching.py
--rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-2.7.0/trajectopy_core/settings/processing.py
--rw-r--r--   0        0        0     6091 2024-02-02 14:24:47.289808 trajectopy_core-2.7.0/trajectopy_core/settings/report.py
--rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-2.7.0/trajectopy_core/settings/sorting.py
--rw-r--r--   0        0        0    10908 2023-12-04 09:19:20.551570 trajectopy_core-2.7.0/trajectopy_core/spatialsorter.py
--rw-r--r--   0        0        0    22734 2024-02-02 14:24:47.290806 trajectopy_core-2.7.0/trajectopy_core/trajectory.py
--rw-r--r--   0        0        0     6322 2023-11-29 11:29:09.888841 trajectopy_core-2.7.0/trajectopy_core/utils.py
--rw-r--r--   0        0        0    33953 1970-01-01 00:00:00.000000 trajectopy_core-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1049 2024-04-23 15:04:24.291777 trajectopy_core-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    33059 2024-04-23 15:04:24.287780 trajectopy_core-3.0.0/README.md
+-rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-3.0.0/trajectopy_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.294777 trajectopy_core-3.0.0/trajectopy_core/alignment/__init__.py
+-rw-r--r--   0        0        0    20272 2024-04-23 15:04:24.295777 trajectopy_core-3.0.0/trajectopy_core/alignment/data.py
+-rw-r--r--   0        0        0    10299 2024-04-23 15:04:24.295777 trajectopy_core-3.0.0/trajectopy_core/alignment/direct.py
+-rw-r--r--   0        0        0     8526 2024-04-23 15:04:24.296780 trajectopy_core-3.0.0/trajectopy_core/alignment/egrad_interface.py
+-rw-r--r--   0        0        0    16133 2024-04-23 15:04:24.296780 trajectopy_core-3.0.0/trajectopy_core/alignment/equations.py
+-rw-r--r--   0        0        0    32369 2024-04-23 15:04:24.296780 trajectopy_core-3.0.0/trajectopy_core/alignment/estimation.py
+-rw-r--r--   0        0        0    23829 2024-04-23 15:04:24.297810 trajectopy_core-3.0.0/trajectopy_core/alignment/parameters.py
+-rw-r--r--   0        0        0     2845 2024-04-23 15:04:24.297810 trajectopy_core-3.0.0/trajectopy_core/alignment/result.py
+-rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-3.0.0/trajectopy_core/alignment/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 13:30:20.272430 trajectopy_core-3.0.0/trajectopy_core/approximation/__init__.py
+-rw-r--r--   0        0        0     9308 2023-11-29 11:29:09.871841 trajectopy_core-3.0.0/trajectopy_core/approximation/cubic_approximation.py
+-rw-r--r--   0        0        0     6608 2023-11-29 11:29:09.872840 trajectopy_core-3.0.0/trajectopy_core/approximation/math_utils.py
+-rw-r--r--   0        0        0     3880 2023-11-29 11:29:09.872840 trajectopy_core-3.0.0/trajectopy_core/approximation/mls_approximation.py
+-rw-r--r--   0        0        0     2151 2023-11-29 11:29:09.873840 trajectopy_core-3.0.0/trajectopy_core/approximation/rot_approximation.py
+-rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-3.0.0/trajectopy_core/approximation/voxelizer.py
+-rw-r--r--   0        0        0     2001 2024-04-18 14:05:54.822747 trajectopy_core-3.0.0/trajectopy_core/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.298782 trajectopy_core-3.0.0/trajectopy_core/evaluation/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-23 15:04:24.298782 trajectopy_core-3.0.0/trajectopy_core/evaluation/ate_result.py
+-rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-3.0.0/trajectopy_core/evaluation/comparison.py
+-rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-3.0.0/trajectopy_core/evaluation/deviations.py
+-rw-r--r--   0        0        0     2277 2024-04-23 15:04:24.299809 trajectopy_core-3.0.0/trajectopy_core/evaluation/metrics.py
+-rw-r--r--   0        0        0     9993 2024-04-23 15:04:24.299809 trajectopy_core-3.0.0/trajectopy_core/evaluation/rpe_result.py
+-rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-3.0.0/trajectopy_core/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.299809 trajectopy_core-3.0.0/trajectopy_core/input_output/__init__.py
+-rw-r--r--   0        0        0     5273 2024-04-23 15:04:24.300806 trajectopy_core-3.0.0/trajectopy_core/input_output/header.py
+-rw-r--r--   0        0        0     3033 2024-04-23 15:04:24.300806 trajectopy_core-3.0.0/trajectopy_core/input_output/rosbag.py
+-rw-r--r--   0        0        0     1197 2024-04-23 15:04:24.300806 trajectopy_core-3.0.0/trajectopy_core/input_output/rosmsg.py
+-rw-r--r--   0        0        0    11313 2024-04-23 15:04:24.301809 trajectopy_core-3.0.0/trajectopy_core/input_output/trajectory_io.py
+-rw-r--r--   0        0        0     1118 2024-04-23 15:04:24.301809 trajectopy_core-3.0.0/trajectopy_core/input_output/utils.py
+-rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-3.0.0/trajectopy_core/kml.py
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-3.0.0/trajectopy_core/LICENSE
+-rw-r--r--   0        0        0     9635 2024-04-23 13:24:51.703124 trajectopy_core-3.0.0/trajectopy_core/matching.py
+-rw-r--r--   0        0        0     1756 2024-04-23 15:04:24.301809 trajectopy_core-3.0.0/trajectopy_core/merging.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-3.0.0/trajectopy_core/plotting/__init__.py
+-rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-3.0.0/trajectopy_core/plotting/bar_plots.py
+-rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-3.0.0/trajectopy_core/plotting/heatmaps.py
+-rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-3.0.0/trajectopy_core/plotting/histograms.py
+-rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-3.0.0/trajectopy_core/plotting/line_plots.py
+-rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-3.0.0/trajectopy_core/plotting/multi_line_plots.py
+-rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-3.0.0/trajectopy_core/plotting/scatter_plots.py
+-rw-r--r--   0        0        0     1626 2024-04-23 13:05:40.251467 trajectopy_core-3.0.0/trajectopy_core/plotting/tables.py
+-rw-r--r--   0        0        0     1660 2024-04-23 15:04:24.302811 trajectopy_core-3.0.0/trajectopy_core/plotting/utils.py
+-rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-3.0.0/trajectopy_core/report/__init__.py
+-rw-r--r--   0        0        0     2441 2024-04-23 13:05:41.738081 trajectopy_core-3.0.0/trajectopy_core/report/alignment.py
+-rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-3.0.0/trajectopy_core/report/assets/icon.png
+-rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-3.0.0/trajectopy_core/report/assets/style.css
+-rw-r--r--   0        0        0     6220 2024-02-02 14:24:47.287810 trajectopy_core-3.0.0/trajectopy_core/report/data.py
+-rw-r--r--   0        0        0     3640 2024-02-02 14:24:47.287810 trajectopy_core-3.0.0/trajectopy_core/report/multi.py
+-rw-r--r--   0        0        0     5286 2024-02-02 14:24:47.288807 trajectopy_core-3.0.0/trajectopy_core/report/single.py
+-rw-r--r--   0        0        0     4660 2024-02-02 14:24:47.288807 trajectopy_core-3.0.0/trajectopy_core/report/templates/generic.html
+-rw-r--r--   0        0        0     5616 2024-02-02 14:24:47.288807 trajectopy_core-3.0.0/trajectopy_core/report/templates/multi_template.html
+-rw-r--r--   0        0        0     7282 2024-02-02 14:24:47.289808 trajectopy_core-3.0.0/trajectopy_core/report/templates/single_template.html
+-rw-r--r--   0        0        0     2010 2024-04-23 15:04:24.302811 trajectopy_core-3.0.0/trajectopy_core/report/trajectory.py
+-rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-3.0.0/trajectopy_core/report/utils.py
+-rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-3.0.0/trajectopy_core/rotationset.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-3.0.0/trajectopy_core/settings/__init__.py
+-rw-r--r--   0        0        0     8782 2024-04-23 15:04:24.303809 trajectopy_core-3.0.0/trajectopy_core/settings/alignment.py
+-rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-3.0.0/trajectopy_core/settings/approximation.py
+-rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-3.0.0/trajectopy_core/settings/base.py
+-rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-3.0.0/trajectopy_core/settings/comparison.py
+-rw-r--r--   0        0        0     1164 2024-04-18 14:05:54.823745 trajectopy_core-3.0.0/trajectopy_core/settings/matching.py
+-rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-3.0.0/trajectopy_core/settings/processing.py
+-rw-r--r--   0        0        0     6091 2024-02-02 14:24:47.289808 trajectopy_core-3.0.0/trajectopy_core/settings/report.py
+-rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-3.0.0/trajectopy_core/settings/sorting.py
+-rw-r--r--   0        0        0    10910 2024-04-23 15:04:24.303809 trajectopy_core-3.0.0/trajectopy_core/sorting.py
+-rw-r--r--   0        0        0    30134 2024-04-23 15:04:24.304809 trajectopy_core-3.0.0/trajectopy_core/trajectory.py
+-rw-r--r--   0        0        0     6322 2023-11-29 11:29:09.888841 trajectopy_core-3.0.0/trajectopy_core/utils.py
+-rw-r--r--   0        0        0    33934 1970-01-01 00:00:00.000000 trajectopy_core-3.0.0/PKG-INFO
```

### Comparing `trajectopy_core-2.7.0/LICENSE` & `trajectopy_core-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/pyproject.toml` & `trajectopy_core-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy-core"
-version = "2.7.0"
+version = "3.0.0"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 maintainers = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "MIT"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy-core"
```

### Comparing `trajectopy_core-2.7.0/README.md` & `trajectopy_core-3.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 This section shows how to use trajectopy to evaluate two trajectories. The example data can be found in the example_data folder. The full code can be found in the example_scripts folder.
 
 ### Absolute Trajectory Error (ATE)
 
     
 ```python
-from trajectopy_core.pipelines import ate
+from trajectopy_core.evaluation.metrics import ate
 from trajectopy_core.settings.processing import ProcessingSettings
 from trajectopy_core.trajectory import Trajectory
 
 # Import
 gt_traj = Trajectory.from_file("./example_data/KITTI_gt.traj")
 est_traj = Trajectory.from_file("./example_data/KITTI_ORB.traj")
 
@@ -99,15 +99,15 @@
 ate_result = ate(trajectory_gt=gt_traj, trajectory_est=est_traj, settings=settings)
 
 ```
 
 ### Relative Pose Error (RPE)
 
 ```python
-from trajectopy_core.pipelines import rpe
+from trajectopy_core.evaluation.metrics import rpe
 from trajectopy_core.settings.processing import ProcessingSettings
 from trajectopy_core.trajectory import Trajectory
 
 # Import
 gt_traj = Trajectory.from_file("./example_data/KITTI_gt.traj")
 est_traj = Trajectory.from_file("./example_data/KITTI_ORB.traj")
 
@@ -179,26 +179,26 @@
 - `use_x_speed` (boolean): Enable or disable the use of X-axis speed for time shift estimation.
 - `use_y_speed` (boolean): Enable or disable the use of Y-axis speed for time shift estimation.
 - `use_z_speed` (boolean): Enable or disable the use of Z-axis speed for time shift estimation.
 - `lever_x` (boolean): Enable or disable estimation of lever arm in the X-axis.
 - `lever_y` (boolean): Enable or disable estimation of lever arm in the Y-axis.
 - `lever_z` (boolean): Enable or disable estimation of lever arm in the Z-axis.
 - `sensor_rotation` (boolean): Enable or disable estimation of sensor rotation. Independent of the least squares adjustment, a constant rotational offset can be computed between the rotations of both trajectories after the alignment.
-- `auto_update` (boolean): If set to `True`, the estimation settings are automatically updated and parameters are disabled if they are not significant (experimental).
 
 ### Stochastics Settings
 
 - `std_xy_from` (float): Standard deviation of XY source position components in meters.
 - `std_z_from` (float): Standard deviation of Z source position component in meters.
 - `std_xy_to` (float): Standard deviation of XY target position components in meters.
 - `std_z_to` (float): Standard deviation of Z target position component in meters.
 - `std_roll_pitch` (float): Standard deviation of roll and pitch in radians.
 - `std_yaw` (float): Standard deviation of yaw in radians.
 - `std_speed_to` (float): Standard deviation of platform speed in (meters per second).
 - `error_probability` (float): Probability of error used for stochastic testing.
+- `variance_estimation` (boolean): Enable or disable the estimation of the variance factor for a-posteriori variance computation.
 
 ### Threshold Settings
 
 Usually, these settings can be left at their default values.
 
 - `metric_threshold` (float): Iteration threshold for the least squares adjustment regarding the metric parameters.
 - `time_threshold` (float): Iteration threshold for the least squares adjustment regarding the time shift parameter.
```

#### html2text {}

```diff
@@ -22,22 +22,22 @@
 ```console .\.venv\Scripts\activate ``` #### Installation via pip Update pip:
 ```console pip install --upgrade pip ``` Install trajectopy: ```console pip
 install trajectopy-core ``` ### Or using the repository: ```console pip install
 git+https://github.com/gereon-t/trajectopy-core.git@main ``` ## Exemplary
 Evaluation This section shows how to use trajectopy to evaluate two
 trajectories. The example data can be found in the example_data folder. The
 full code can be found in the example_scripts folder. ### Absolute Trajectory
-Error (ATE) ```python from trajectopy_core.pipelines import ate from
+Error (ATE) ```python from trajectopy_core.evaluation.metrics import ate from
 trajectopy_core.settings.processing import ProcessingSettings from
 trajectopy_core.trajectory import Trajectory # Import gt_traj =
 Trajectory.from_file("./example_data/KITTI_gt.traj") est_traj =
 Trajectory.from_file("./example_data/KITTI_ORB.traj") # default settings
 settings = ProcessingSettings() ate_result = ate(trajectory_gt=gt_traj,
 trajectory_est=est_traj, settings=settings) ``` ### Relative Pose Error (RPE)
-```python from trajectopy_core.pipelines import rpe from
+```python from trajectopy_core.evaluation.metrics import rpe from
 trajectopy_core.settings.processing import ProcessingSettings from
 trajectopy_core.trajectory import Trajectory # Import gt_traj =
 Trajectory.from_file("./example_data/KITTI_gt.traj") est_traj =
 Trajectory.from_file("./example_data/KITTI_ORB.traj") # default settings
 settings = ProcessingSettings() rpe_result = rpe(trajectory_gt=gt_traj,
 trajectory_est=est_traj, settings=settings) ``` ## Importing Trajectories
 Trajectory files must be ASCII files with a csv-like layout. The default column
@@ -143,29 +143,28 @@
 axis speed for time shift estimation. - `use_z_speed` (boolean): Enable or
 disable the use of Z-axis speed for time shift estimation. - `lever_x`
 (boolean): Enable or disable estimation of lever arm in the X-axis. - `lever_y`
 (boolean): Enable or disable estimation of lever arm in the Y-axis. - `lever_z`
 (boolean): Enable or disable estimation of lever arm in the Z-axis. -
 `sensor_rotation` (boolean): Enable or disable estimation of sensor rotation.
 Independent of the least squares adjustment, a constant rotational offset can
-be computed between the rotations of both trajectories after the alignment. -
-`auto_update` (boolean): If set to `True`, the estimation settings are
-automatically updated and parameters are disabled if they are not significant
-(experimental). ### Stochastics Settings - `std_xy_from` (float): Standard
-deviation of XY source position components in meters. - `std_z_from` (float):
-Standard deviation of Z source position component in meters. - `std_xy_to`
-(float): Standard deviation of XY target position components in meters. -
-`std_z_to` (float): Standard deviation of Z target position component in
-meters. - `std_roll_pitch` (float): Standard deviation of roll and pitch in
-radians. - `std_yaw` (float): Standard deviation of yaw in radians. -
-`std_speed_to` (float): Standard deviation of platform speed in (meters per
-second). - `error_probability` (float): Probability of error used for
-stochastic testing. ### Threshold Settings Usually, these settings can be left
-at their default values. - `metric_threshold` (float): Iteration threshold for
-the least squares adjustment regarding the metric parameters. -
+be computed between the rotations of both trajectories after the alignment. ###
+Stochastics Settings - `std_xy_from` (float): Standard deviation of XY source
+position components in meters. - `std_z_from` (float): Standard deviation of Z
+source position component in meters. - `std_xy_to` (float): Standard deviation
+of XY target position components in meters. - `std_z_to` (float): Standard
+deviation of Z target position component in meters. - `std_roll_pitch` (float):
+Standard deviation of roll and pitch in radians. - `std_yaw` (float): Standard
+deviation of yaw in radians. - `std_speed_to` (float): Standard deviation of
+platform speed in (meters per second). - `error_probability` (float):
+Probability of error used for stochastic testing. - `variance_estimation`
+(boolean): Enable or disable the estimation of the variance factor for a-
+posteriori variance computation. ### Threshold Settings Usually, these settings
+can be left at their default values. - `metric_threshold` (float): Iteration
+threshold for the least squares adjustment regarding the metric parameters. -
 `time_threshold` (float): Iteration threshold for the least squares adjustment
 regarding the time shift parameter. ## Matching Settings - `method`
 (`MatchingMethod`): The method used for trajectory matching. Choices:
 `MatchingMethod.NEAREST_SPATIAL`, `MatchingMethod.NEAREST_TEMPORAL`,
 `MatchingMethod.INTERPOLATION`, `MatchingMethod.NEAREST_SPATIAL_INTERPOLATED`.
 The methods are described below. - `max_time_diff` (float): Maximum allowed
 time difference when matching two trajectories using their timestamps. -
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/data.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,14 +503,32 @@
         thresholds[:3] *= self.alignment_settings.metric_threshold
         thresholds[3:7] *= scale_and_angle_th
         thresholds[7] *= self.alignment_settings.time_threshold
         thresholds[8:] *= self.alignment_settings.metric_threshold
         return thresholds
 
     def get_variance_estimation_subset(self, num_obs: int = 200) -> "AlignmentData":
+        """Returns a subset of the alignment data for variance estimation
+
+        This method will return a subset of the alignment data
+        that contains 'num_obs' observations. The subset is selected
+        by finding the epoch with the highest standard deviation of
+        the observations. The idea is that a higher variance in the
+        observations will lead to a better estimation of the variances.
+
+        The motivation behind this is that the variance estimation
+        is memory and time consuming. Therefore, a subset of the
+        observations is used for the estimation.
+
+        Args:
+            num_obs (int, optional): Subet size. Defaults to 200.
+
+        Returns:
+            AlignmentData: Cropped alignment data
+        """
         obs_matrix = np.reshape(self.obs_vector, (len(self), self.num_obs_per_epoch))
         if len(obs_matrix) <= num_obs:
             return copy.deepcopy(self)
 
         obs_norm = np.linalg.norm(obs_matrix, axis=1)
         obs_series = pd.Series(obs_norm)
         max_idx = obs_series.rolling(window=num_obs).std().idxmax()
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/estimation.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/estimation.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,108 @@
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
 
 import logging
-from typing import Dict, Union
+from typing import Dict
 
 import numpy as np
 from numpy import matlib
-from scipy.sparse import csc_matrix, spdiags
+from scipy.sparse import csc_matrix
 from scipy.sparse.linalg import spsolve
 from scipy.stats.distributions import chi2
 
-from trajectopy_core.alignment.direct.helmert_transformation import direct_helmert_transformation
-from trajectopy_core.alignment.direct.leverarm import direct_leverarm
-from trajectopy_core.alignment.direct.timeshift import direct_timeshift
-from trajectopy_core.alignment.ghm.data import AlignmentData
-from trajectopy_core.alignment.ghm.functional_model.interface import FunctionalRelationship
-from trajectopy_core.alignment.parameters import AlignmentParameters, HelmertTransformation, Leverarm, Parameter
+from trajectopy_core.alignment.data import AlignmentData
+from trajectopy_core.alignment.direct import (
+    align_rotations,
+    direct_helmert_transformation,
+    direct_leverarm,
+    direct_timeshift,
+)
+from trajectopy_core.alignment.egrad_interface import FunctionalRelationship
+from trajectopy_core.alignment.parameters import (
+    AlignmentParameters,
+    HelmertTransformation,
+    Leverarm,
+    Parameter,
+    SensorRotationParameters,
+)
+from trajectopy_core.alignment.result import AlignmentResult
 from trajectopy_core.alignment.utils import dict2table
 from trajectopy_core.definitions import Unit
-from trajectopy_core.settings.alignment import AlignmentEstimationSettings, AlignmentSettings
+from trajectopy_core.settings.alignment import AlignmentSettings
+from trajectopy_core.settings.matching import MatchingSettings
+from trajectopy_core.trajectory import Trajectory
 
 logger = logging.getLogger("root")
 
 
-class Alignment:
+def compute_alignment(
+    traj_from: Trajectory,
+    traj_to: Trajectory,
+    alignment_settings: AlignmentSettings = AlignmentSettings(),
+    matching_settings: MatchingSettings = MatchingSettings(),
+) -> AlignmentResult:
+    """Aligns two trajectories
+
+    Performs a
+    - Helmert
+    - Leverarm
+    - Time shift
+
+    estimation depending on the configuration.
+    After this, the estimated parameters are applied
+    to the 'traj_from' trajectory.
+
+    Args:
+        traj_from (Trajectory)
+        traj_to (Trajectory)
+        alignment_settings (AlignmentSettings, optional): Settings for the alignment process. Defaults to AlignmentSettings().
+        matching_settings (MatchingSettings, optional): Settings for the matching process. Defaults to MatchingSettings().
+
+    Returns:
+        AlignmentResult: Result of the alignment process
+    """
+    logger.info("Aligning trajectory positions ...")
+
+    alignment_data = AlignmentData(
+        traj_from=traj_from,
+        traj_to=traj_to,
+        alignment_settings=alignment_settings,
+        matching_settings=matching_settings,
+    )
+    ghm_alignment = AlignmentEstimation(alignment_data=alignment_data)
+    estimated_parameters = ghm_alignment.estimate_parameters()
+
+    if (
+        alignment_data.traj_from.rot is not None
+        and alignment_data.traj_to.rot is not None
+        and alignment_settings.estimation_settings.sensor_rotation
+    ):
+        pre_aligned_trajectory = alignment_data.traj_from.apply_transformation(
+            estimated_parameters.sim3_matrix, inplace=False
+        )
+        logger.info("Aligning rotations ...")
+        sensor_rot_params = align_rotations(rot_from=pre_aligned_trajectory.rot, rot_to=alignment_data.traj_to.rot)
+        print(sensor_rot_params)
+    else:
+        sensor_rot_params = SensorRotationParameters(enabled=False)
+
+    return AlignmentResult(
+        name=f"{alignment_data.traj_from.name} to {alignment_data.traj_to.name}",
+        position_parameters=estimated_parameters,
+        rotation_parameters=sensor_rot_params,
+        estimation_of=ghm_alignment.settings.estimation_settings,
+        converged=ghm_alignment.has_results,
+    )
+
+
+class AlignmentEstimation:
     """Class representing the alignment of two trajectories
 
     This class will align two trajectories using a combination
     of a 3d Helmert-transformation, a leverarm estimation and a
     time-shift estimation.
 
     It can fully align two trajectories their separation can be
@@ -60,124 +132,24 @@
             error_probability (float, optional): Used for the stochastic global test.
                                                  Defaults to 0.05.
         """
         self.funcrel = FunctionalRelationship()
         self.data = alignment_data
 
         self._est_params = self.init_parameters()
-        self._reestimation_required = True
         self._has_results = False
         self._converged = False
         self._group_redundancies = {}
 
         logger.info("Initialized Alignment!")
         logger.info(self)
 
     def __str__(self) -> str:
         return settings_str(self)
 
-    @property
-    def settings(self) -> AlignmentSettings:
-        return self.data.alignment_settings
-
-    def update_estimation_settings(self) -> Union[AlignmentEstimationSettings, None]:
-        """Checks if enabled parameters are actually needed and returns the updated settings"""
-
-        def default_check(parameter: Parameter) -> bool:
-            return abs(parameter.value) <= 3 * np.sqrt(parameter.variance)
-
-        def scale_check(parameter: Parameter) -> bool:
-            return abs(parameter.value - 1) <= 3 * np.sqrt(parameter.variance)
-
-        if not self.has_results:
-            logger.warning("No results available. Returning None.")
-            return None
-
-        logger.info("Checking if enabled parameters are needed...")
-
-        check_mapping = {Unit.SCALE: scale_check}
-
-        settings_changed = False
-        for parameter in self.est_params:
-            if not parameter.enabled:
-                continue
-
-            if check_mapping.get(parameter.unit, default_check)(parameter):
-                logger.info("Parameter %s is enabled but not needed. Disabling.", parameter.name)
-                parameter.enabled = False
-                settings_changed = True
-
-        if not settings_changed:
-            logger.info("No settings changed.")
-            return None
-
-        return self.est_params.to_estimation_settings()
-
-    def estimate(self) -> AlignmentParameters:
-        """Handles the estimation of the parameters
-
-        Calls either robust reweighting or variance
-        estimation methods.
-        """
-        logger.info("Performing alignment...")
-        if self.settings.estimation_settings.all_lq_disabled:
-            logger.warning("Nothing to estimate since all parameters are disabled")
-            return AlignmentParameters()
-
-        max_recomputations = 5
-        cnt = 0
-        while self._reestimation_required:
-            if cnt > max_recomputations:
-                logger.warning("Maximum number of recomputations reached. Aborting.")
-                break
-
-            self._reestimation_required = False
-            self._estimate_parameters()
-
-            if self.data.alignment_settings.stochastics.variance_component_estimation:
-                self.variance_component_estimation()
-
-            # after adjusting the group variances, the parameters need to be re-estimated before performing the global test
-            # we only want to change one thing at a time
-            if self._reestimation_required:
-                self._estimate_parameters()
-
-            self.variance_estimation()
-
-            cnt += 1
-
-        if not self._converged:
-            logger.info("Adjustment did not converge. Returning initial parameters.")
-            return self.init_parameters()
-
-        self._has_results = True
-        print_summary(self)
-
-        return self._est_params
-
-    @property
-    def has_results(self) -> bool:
-        return self._has_results
-
-    @property
-    def est_params(self) -> AlignmentParameters:
-        return self._est_params
-
-    @property
-    def group_redundancies(self) -> Dict[str, bool]:
-        return self._group_redundancies
-
-    @property
-    def num_of_equations(self) -> int:
-        return self.data.number_of_epochs * 3
-
-    @property
-    def redundancy(self) -> int:
-        return self.num_of_equations - self._est_params.num_enabled
-
     def init_parameters(self) -> AlignmentParameters:
         """This method computes initial parameters
         for the iterative adjustment
 
         For this, the helmert transformation and
         the leverarm estimation are done separatetly
         using methods that do not require inital
@@ -232,220 +204,135 @@
             lever_z=leverarm_init.z,
         )
 
         alignparams.apply_settings(self.settings.estimation_settings)
         logger.debug("Applied settings: %s \n", str(self.settings.estimation_settings))
         return alignparams
 
-    @property
-    def variance_factor(self) -> float:
-        return (
-            self.data.res_vector.T @ spsolve(csc_matrix(self.data.sigma_ll), self.data.res_vector)
-        ) / self.redundancy
+    def estimate_parameters(self) -> AlignmentParameters:
+        """Handles the estimation of the parameters"""
 
-    @property
-    def _condition_xyz_to(self) -> list:
-        """
-        Helper function returning the constant xyz_to component of
-        the condition matrix
-        """
-        return [
-            np.c_[
-                -np.ones((self.data.number_of_epochs, 1)),
-                np.zeros((self.data.number_of_epochs, 1)),
-                np.zeros((self.data.number_of_epochs, 1)),
-            ],
-            np.c_[
-                np.zeros((self.data.number_of_epochs, 1)),
-                -np.ones((self.data.number_of_epochs, 1)),
-                np.zeros((self.data.number_of_epochs, 1)),
-            ],
-            np.c_[
-                np.zeros((self.data.number_of_epochs, 1)),
-                np.zeros((self.data.number_of_epochs, 1)),
-                -np.ones((self.data.number_of_epochs, 1)),
-            ],
-        ]
+        logger.info("Performing alignment...")
+        if self.settings.estimation_settings.all_lq_disabled:
+            logger.warning("Nothing to estimate since all parameters are disabled")
+            return AlignmentParameters()
 
-    def variance_component_estimation(self) -> Dict[str, bool]:
-        """Performs an estimation of the variances for different observation groups
+        cnt = 0
+        max_recomputations = 5
+        var_fac_diff = float("inf")
+        var_fac_tol = 1e-3
 
-        The observations groups are:
-            - x and y components of xyz_from
-            - z component of xyz_from
-            - x and y components of xyz_to
-            - z component of xyz_to
-            - roll / pitch components of rpy_body
-            - yaw component of rpy_body
-            - speed (at target positions)
+        while var_fac_diff > var_fac_tol and cnt < max_recomputations:
+            self._estimate_parameters()
+            self._global_test(variance_factor=self.variance_factor, redundancy=self.redundancy)
 
-        """
-        group_global_tests: Dict[str, bool] = {}
-        group_variance_factors = []
+            if not self.data.alignment_settings.stochastics.variance_estimation:
+                break
 
-        for group_key in self.data.variance_groups:
-            group_variances = np.c_[self.data.get_var_group(key=group_key)]
-            group_residuals = np.c_[self.data.get_res_group(key=group_key)]
-
-            group_redundancy = self.group_redundancies[group_key]
-            group_variance_factor = (
-                np.sum(group_residuals * np.reciprocal(group_variances) * group_residuals) / group_redundancy
-            )
+            var_fac_diff = abs(self.variance_factor - 1)
 
-            if np.allclose(group_variance_factor, 0):
-                logger.warning("Variance factor is 0 for group %s. Skipping.", group_key)
-                continue
+            logger.info("Adjusting variance vector by factor %.3f", self.variance_factor)
+            self.data._var_vector *= self.variance_factor
 
-            group_global_test = self._global_test(
-                variance_factor=group_variance_factor, redundancy=group_redundancy, description=group_key
-            )
+            if var_fac_diff > var_fac_tol:
+                logger.info("Variance component is different from 1, re-estimation required.")
+            else:
+                logger.info("Finished with variance estimation. Re-estimation not required.")
 
-            # global test for group
-            self.data.set_var_group(values=group_variances * group_variance_factor, key=group_key)
-            logger.info("Adjusted variance for group %s by factor %.3f", group_key, group_variance_factor)
-
-            group_global_tests[group_key] = group_global_test
-            group_variance_factors.append(group_variance_factor)
-
-        if any((abs(factor - 1)) > 0.1 for factor in group_variance_factors):
-            logger.info("Group variance components are different from 1, re-estimation required.")
-            self._reestimation_required = True
-        else:
-            logger.info("Finished with variance component estimation. Re-estimation not required.")
+            cnt += 1
 
-        logging.info(dict2table(group_global_tests, title="Group Stochastic Test Results"))
-        return group_global_tests
+        if not self._converged:
+            logger.info("Adjustment did not converge. Returning initial parameters.")
+            return self.init_parameters()
 
-    def variance_estimation(self) -> None:
-        """
-        Tests the consistency of the functional and stochastic model and
-        adjusts the variance vector if necessary.
-        """
-        self._global_test(variance_factor=self.variance_factor, redundancy=self.redundancy)
+        self._has_results = True
+        print_summary(self)
 
-        if not self.data.alignment_settings.stochastics.variance_estimation:
-            return
+        return self._est_params
 
-        logger.info("Adjusting variance vector by factor %.3f", self.variance_factor)
+    @property
+    def settings(self) -> AlignmentSettings:
+        return self.data.alignment_settings
 
-        if np.allclose(self.variance_factor, 0):
-            logger.warning("Variance factor is 0. Aborting.")
-            return
+    @property
+    def has_results(self) -> bool:
+        return self._has_results
 
-        if abs(self.variance_factor - 1) > 0.1:
-            logger.info("Variance component is different from 1, re-estimation required.")
-            self._reestimation_required = True
-        else:
-            logger.info("Finished with variance estimation. Re-estimation not required.")
+    @property
+    def est_params(self) -> AlignmentParameters:
+        return self._est_params
 
-        self.data._var_vector *= self.variance_factor
+    @property
+    def group_redundancies(self) -> Dict[str, bool]:
+        return self._group_redundancies
 
-    def _global_test(self, variance_factor: float, redundancy: int, description: str = "global") -> bool:
-        tau = variance_factor * redundancy
-        quantile = chi2.ppf(1 - self.settings.stochastics.error_probability, redundancy)
+    @property
+    def num_of_equations(self) -> int:
+        return self.data.number_of_epochs * 3
 
-        logger.info(
-            "Stochastic test passed (%s): %s, quantile: %.3f, test value: %.3f, variance factor: %.3f",
-            description,
-            str(tau <= quantile),
-            quantile,
-            tau,
-            variance_factor,
-        )
-        return tau <= quantile
+    @property
+    def redundancy(self) -> int:
+        return self.num_of_equations - self._est_params.num_enabled
+
+    @property
+    def variance_factor(self) -> float:
+        return (
+            self.data.res_vector.T @ spsolve(csc_matrix(self.data.sigma_ll), self.data.res_vector)
+        ) / self.redundancy
 
     def _estimate_parameters(self) -> None:
         """Helmert-Leverarm-Time Transformation using the Gauß-Helmert-Model
 
         The observation-equations are sorted in the following way:
         [X, Y, Z, X, Y, Z, ..., X, Y, Z]
         """
         # obs = [x_from, y_from, z_from, x_to, y_to, z_to, roll_body, pitch_body, yaw_body]
 
         # preparation for iterative adjustment
         delta_params = np.ones((len(self._est_params),)) * np.Inf
         self.data.res_vector = np.zeros_like(self.data.obs_vector)
 
-        contradiction_w = self._auto_functional_relationship()
+        contradiction_w = self._eval_functional_relationship()
 
         it_counter = 0
         max_iterations = 15
         self._converged = True
         while any(abs(value) > threshold for value, threshold in zip(delta_params, self.data.thresholds)):
             if it_counter > max_iterations:
                 logger.error(
                     "Adjustment did not converge after %i iterations. Maximum parameter update: %.3e",
                     it_counter,
                     np.max(np.abs(delta_params)),
                 )
                 self._converged = False
                 break
 
-            a_design = self.auto_design_matrix()
+            a_design = self._get_design_matrix()
 
             # filter design matrix
             a_design = a_design[:, self.settings.estimation_settings.lq_parameter_filter]
-            b_cond = self._condition_matrix()
+            b_cond = self._get_condition_matrix()
 
             bbt = b_cond @ self.data.sigma_ll @ b_cond.T
 
             # solve normal equations
             delta_params = self._compute_parameter_deltas(contradiction_w, a_design, bbt)
             correlates_k = -spsolve(bbt, a_design @ delta_params + contradiction_w)
             self.data.res_vector = self.data.sigma_ll @ b_cond.T @ correlates_k
 
             # update
             self._est_params.values_enabled += delta_params
-            contradiction_w = self._auto_functional_relationship() - b_cond @ self.data.res_vector.ravel()
+            contradiction_w = self._eval_functional_relationship() - b_cond @ self.data.res_vector.ravel()
             it_counter += 1
 
         if self._converged:
             logger.info("Adjustment did converge after %i iterations", it_counter)
 
         self._compute_parameter_variances(a_design, bbt)
 
-        if self.data.alignment_settings.stochastics.variance_component_estimation:
-            self._compute_group_redundancies(a_design, b_cond, bbt)
-
-    def _compute_group_redundancies(self, a_design: csc_matrix, b_cond: csc_matrix, bbt: csc_matrix) -> None:
-        q_22 = -self.est_params.get_covariance_matrix()
-        q_12 = -spsolve(bbt, a_design @ q_22)
-        q_21 = q_12.T if q_12.ndim == 2 else q_12[None, :]
-        q_11 = spsolve(
-            bbt, spdiags(np.ones(a_design.shape[0]), 0, a_design.shape[0], a_design.shape[0]) - a_design @ q_21
-        )
-        red_components = (
-            self.data.sigma_ll @ b_cond.T @ q_11 @ b_cond @ self.data.sigma_ll
-        ).diagonal() * np.reciprocal(self.data.var_vector)
-
-        group_redundancies = {
-            "XY_FROM": (
-                sum(red_components[0 :: self.data.num_obs_per_epoch])
-                + sum(red_components[1 :: self.data.num_obs_per_epoch])
-            ),
-            "Z_FROM": sum(red_components[2 :: self.data.num_obs_per_epoch]),
-            "XY_TO": (
-                sum(red_components[3 :: self.data.num_obs_per_epoch])
-                + sum(red_components[4 :: self.data.num_obs_per_epoch])
-            ),
-            "Z_TO": sum(red_components[5 :: self.data.num_obs_per_epoch]),
-            "ROLL_PITCH": (
-                sum(red_components[6 :: self.data.num_obs_per_epoch])
-                + sum(red_components[7 :: self.data.num_obs_per_epoch])
-            ),
-            "YAW": sum(red_components[8 :: self.data.num_obs_per_epoch]),
-            "SPEED": (
-                sum(red_components[9 :: self.data.num_obs_per_epoch])
-                + sum(red_components[10 :: self.data.num_obs_per_epoch])
-                + sum(red_components[11 :: self.data.num_obs_per_epoch])
-            ),
-        }
-
-        self._group_redundancies = group_redundancies
-
     def _compute_parameter_variances(self, a_design: csc_matrix, bbt: csc_matrix) -> None:
         sigma_xx_inv: csc_matrix = a_design.T @ spsolve(bbt, a_design)
         if sigma_xx_inv.size == 1:
             self._est_params.set_covariance_matrix(np.reciprocal(sigma_xx_inv[:, None]))
         else:
             self._est_params.set_covariance_matrix(np.linalg.pinv(sigma_xx_inv.toarray()))
 
@@ -458,22 +345,37 @@
         # quasi vermittelnd
         # spsolve(-a_design.T @ spsolve(bbt, -a_design), -a_design.T @ spsolve(bbt, contradiction_w))
         return -spsolve(
             a_design.T @ spsolve(bbt, a_design),
             a_design.T @ spsolve(bbt, contradiction_w),
         )
 
-    def auto_design_matrix(self) -> csc_matrix:
+    def _global_test(self, variance_factor: float, redundancy: int, description: str = "global") -> bool:
+        tau = variance_factor * redundancy
+        quantile = chi2.ppf(1 - self.settings.stochastics.error_probability, redundancy)
+
+        logger.info(
+            "Stochastic test passed (%s): %s, quantile: %.3f, test value: %.3f, variance factor: %.3f, redundancy: %i",
+            description,
+            str(tau <= quantile),
+            quantile,
+            tau,
+            variance_factor,
+            redundancy,
+        )
+        return tau <= quantile
+
+    def _get_design_matrix(self) -> csc_matrix:
         a_design = np.zeros((self.data.number_of_epochs * 3, 11))
-        a_design[0::3, :] = self._auto_design_x()
-        a_design[1::3, :] = self._auto_design_y()
-        a_design[2::3, :] = self._auto_design_z()
+        a_design[0::3, :] = self._get_design_x()
+        a_design[1::3, :] = self._get_design_y()
+        a_design[2::3, :] = self._get_design_z()
         return csc_matrix(a_design)
 
-    def _auto_design_z(self) -> np.ndarray:
+    def _get_design_z(self) -> np.ndarray:
         return np.c_[
             np.zeros((self.data.number_of_epochs, 1)),
             np.zeros((self.data.number_of_epochs, 1)),
             self.funcrel.eval(
                 func=self.funcrel.dz_dsim_trans_z,
                 parameters=self.est_params,
                 observations=self.data,
@@ -512,15 +414,15 @@
             self.funcrel.eval(
                 func=self.funcrel.dz_dlever_z,
                 parameters=self.est_params,
                 observations=self.data,
             ),
         ]
 
-    def _auto_design_y(self) -> np.ndarray:
+    def _get_design_y(self) -> np.ndarray:
         return np.c_[
             np.zeros((self.data.number_of_epochs, 1)),
             self.funcrel.eval(
                 func=self.funcrel.dy_dsim_trans_y,
                 parameters=self.est_params,
                 observations=self.data,
             ),
@@ -563,15 +465,15 @@
             self.funcrel.eval(
                 func=self.funcrel.dy_dlever_z,
                 parameters=self.est_params,
                 observations=self.data,
             ),
         ]
 
-    def _auto_design_x(self) -> np.ndarray:
+    def _get_design_x(self) -> np.ndarray:
         return np.c_[
             self.funcrel.eval(
                 func=self.funcrel.dx_dsim_trans_x,
                 parameters=self.est_params,
                 observations=self.data,
             ),
             np.zeros((self.data.number_of_epochs, 1)),
@@ -614,23 +516,23 @@
             self.funcrel.eval(
                 func=self.funcrel.dx_dlever_z,
                 parameters=self.est_params,
                 observations=self.data,
             ),
         ]
 
-    def _auto_functional_relationship(self) -> np.ndarray:
+    def _eval_functional_relationship(self) -> np.ndarray:
         # accounting for the time shift not by using the velocity model but by shifting the time stamps and re-interpolating
         func_xyz = np.zeros((self.data.number_of_epochs * 3,))
         func_xyz[::3] = self.funcrel.eval(func=self.funcrel.x, parameters=self.est_params, observations=self.data)
         func_xyz[1::3] = self.funcrel.eval(func=self.funcrel.y, parameters=self.est_params, observations=self.data)
         func_xyz[2::3] = self.funcrel.eval(func=self.funcrel.z, parameters=self.est_params, observations=self.data)
         return func_xyz
 
-    def _condition_matrix(self) -> csc_matrix:
+    def _get_condition_matrix(self) -> csc_matrix:
         """Computes the condition-matrix for the Gauß-Helmert-Model
 
         The matrix contains the derivatives of the
         observation equations with respect to the observations.
 
         Depending on whether the lever arm is to be estimated,
         additional columns are added to the condition matrix
@@ -684,22 +586,22 @@
 
         Args:
             parameters (AlignmentParameters): (current) estimated parameters
 
         Returns:
             np.ndarray: condition matrix data
         """
-        xyz_from_component = self._auto_condition_xyz_from()
+        xyz_from_component = self._get_condition_xyz_from()
 
         rpy_body_component = (
-            self._auto_condition_rpy_body() if self.settings.estimation_settings.leverarm_enabled else None
+            self._get_condition_rpy_body() if self.settings.estimation_settings.leverarm_enabled else None
         )
 
         speed_to_component = (
-            self._auto_condition_speed_to() if self.settings.estimation_settings.time_shift_enabled else None
+            self._get_condition_speed_to() if self.settings.estimation_settings.time_shift_enabled else None
         )
 
         if (
             self.settings.estimation_settings.leverarm_enabled
             and not self.settings.estimation_settings.time_shift_enabled
             and rpy_body_component is not None
         ):
@@ -754,15 +656,15 @@
                     xyz_from_component[i],
                     self._condition_xyz_to[i],
                 ]
                 for i in range(3)
             ]
         )
 
-    def _auto_condition_rpy_body(self) -> list:
+    def _get_condition_rpy_body(self) -> list:
         return [
             np.c_[
                 self.funcrel.eval(
                     func=self.funcrel.dx_deuler_x,
                     parameters=self.est_params,
                     observations=self.data,
                 ),
@@ -809,15 +711,15 @@
                     func=self.funcrel.dz_deuler_z,
                     parameters=self.est_params,
                     observations=self.data,
                 ),
             ],
         ]
 
-    def _auto_condition_xyz_from(self) -> list:
+    def _get_condition_xyz_from(self) -> list:
         return [
             np.c_[
                 self.funcrel.eval(
                     func=self.funcrel.dx_dx_from,
                     parameters=self.est_params,
                     observations=self.data,
                 ),
@@ -864,15 +766,39 @@
                     func=self.funcrel.dz_dz_from,
                     parameters=self.est_params,
                     observations=self.data,
                 ),
             ],
         ]
 
-    def _auto_condition_speed_to(self) -> list:
+    @property
+    def _condition_xyz_to(self) -> list:
+        """
+        Helper function returning the constant xyz_to component of
+        the condition matrix
+        """
+        return [
+            np.c_[
+                -np.ones((self.data.number_of_epochs, 1)),
+                np.zeros((self.data.number_of_epochs, 1)),
+                np.zeros((self.data.number_of_epochs, 1)),
+            ],
+            np.c_[
+                np.zeros((self.data.number_of_epochs, 1)),
+                -np.ones((self.data.number_of_epochs, 1)),
+                np.zeros((self.data.number_of_epochs, 1)),
+            ],
+            np.c_[
+                np.zeros((self.data.number_of_epochs, 1)),
+                np.zeros((self.data.number_of_epochs, 1)),
+                -np.ones((self.data.number_of_epochs, 1)),
+            ],
+        ]
+
+    def _get_condition_speed_to(self) -> list:
         return [
             np.c_[
                 self.funcrel.eval(
                     func=self.funcrel.dx_dspeed_x,
                     parameters=self.est_params,
                     observations=self.data,
                 ),
@@ -920,20 +846,20 @@
                     parameters=self.est_params,
                     observations=self.data,
                 ),
             ],
         ]
 
 
-def print_summary(alignment: Alignment) -> None:
+def print_summary(alignment: AlignmentEstimation) -> None:
     logger.info(dict2table(alignment.data.group_stds, title="Group Standard Deviations"))
     logger.info(alignment.est_params)
 
 
-def settings_str(alignment: Alignment) -> str:
+def settings_str(alignment: AlignmentEstimation) -> str:
     return (
         f"\n _____________________________________________________________________\n"
         f"| ---------------------------- Alignment ---------------------------- |\n"
         f"| Estimation of:           {alignment.settings.estimation_settings.short_mode_str:<42} |\n"
         f"| Error probability [%]:   {alignment.settings.stochastics.error_probability*100:<42} |\n"
         f"|_____________________________________________________________________|\n"
     )
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/equations.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/ghm/functional_model/interface.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/egrad_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 from typing import Callable
 
 import autograd.numpy as np
 from autograd import elementwise_grad as egrad
 
-from trajectopy_core.alignment.ghm.data import AlignmentData
-from trajectopy_core.alignment.ghm.functional_model.equations import (
+from trajectopy_core.alignment.data import AlignmentData
+from trajectopy_core.alignment.equations import (
     functional_relationship_x,
     functional_relationship_y,
     functional_relationship_z,
 )
 from trajectopy_core.alignment.parameters import AlignmentParameters
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/parameters.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 from abc import ABC
 from dataclasses import dataclass, field, fields
 from typing import Dict, List
 
 import numpy as np
 import pandas as pd
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/result.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 from dataclasses import dataclass, field
 
 import numpy as np
 
 from trajectopy_core.alignment.parameters import AlignmentParameters, SensorRotationParameters
-from trajectopy_core.io.header import HeaderData
+from trajectopy_core.input_output.header import HeaderData
 from trajectopy_core.settings.alignment import AlignmentEstimationSettings
 
 
 @dataclass
 class AlignmentResult:
     name: str = "Alignment Result"
     position_parameters: AlignmentParameters = field(default_factory=AlignmentParameters)
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/alignment/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/approximation/cubic_approximation.py` & `trajectopy_core-3.0.0/trajectopy_core/approximation/cubic_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/approximation/math_utils.py` & `trajectopy_core-3.0.0/trajectopy_core/approximation/math_utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/approximation/mls_approximation.py` & `trajectopy_core-3.0.0/trajectopy_core/approximation/mls_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/approximation/rot_approximation.py` & `trajectopy_core-3.0.0/trajectopy_core/approximation/rot_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/approximation/voxelizer.py` & `trajectopy_core-3.0.0/trajectopy_core/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/definitions.py` & `trajectopy_core-3.0.0/trajectopy_core/definitions.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/evaluation/ate_result.py` & `trajectopy_core-3.0.0/trajectopy_core/evaluation/ate_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 from functools import cached_property
 from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 from pointset import PointSet
 
 from trajectopy_core.evaluation.deviations import AbsoluteTrajectoryDeviations
 from trajectopy_core.evaluation.utils import rms
-from trajectopy_core.io.header import HeaderData
+from trajectopy_core.input_output.header import HeaderData
 from trajectopy_core.rotationset import RotationSet
 from trajectopy_core.trajectory import Trajectory
 
 
 class ATEResult:
     """
     This class represents a set of absolute trajectory deviations
@@ -58,26 +59,26 @@
             "RMS Z [m]": f"{self.pos_rms_z:.4f}",
             "Bias Along-Track [m]": f"{self.pos_bias_along:.4f}",
             "Bias Horizontal Cross-Track [m]": f"{self.pos_bias_cross_h:.4f}",
             "Bias Vertical Cross-Track [m]": f"{self.pos_bias_cross_v:.4f}",
             "RMS Along-Track [m]": f"{self.pos_rms_along:.4f}",
             "RMS Horizontal Cross-Track [m]": f"{self.pos_rms_cross_h:.4f}",
             "RMS Vertical Cross-Track [m]": f"{self.pos_rms_cross_v:.4f}",
-            "Maximum rotation deviation [°]": f"{np.rad2deg(self.rot_dev_max):.4f}"
-            if self.abs_dev.rot_dev is not None
-            else "-",
-            "Mean rotation deviation [°]": f"{np.rad2deg(self.rot_ate):.4f}"
-            if self.abs_dev.rot_dev is not None
-            else "-",
-            "Median rotation deviation [°]": f"{np.rad2deg(self.rot_dev_median):.4f}"
-            if self.abs_dev.rot_dev is not None
-            else "-",
-            "Minimum rotation deviation [°]": f"{np.rad2deg(self.rot_dev_min):.4f}"
-            if self.abs_dev.rot_dev is not None
-            else "-",
+            "Maximum rotation deviation [°]": (
+                f"{np.rad2deg(self.rot_dev_max):.4f}" if self.abs_dev.rot_dev is not None else "-"
+            ),
+            "Mean rotation deviation [°]": (
+                f"{np.rad2deg(self.rot_ate):.4f}" if self.abs_dev.rot_dev is not None else "-"
+            ),
+            "Median rotation deviation [°]": (
+                f"{np.rad2deg(self.rot_dev_median):.4f}" if self.abs_dev.rot_dev is not None else "-"
+            ),
+            "Minimum rotation deviation [°]": (
+                f"{np.rad2deg(self.rot_dev_min):.4f}" if self.abs_dev.rot_dev is not None else "-"
+            ),
             "RMS Rotation [°]": f"{np.rad2deg(self.rot_dev_rms):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "STD Rotation [°]": f"{np.rad2deg(self.rot_dev_std):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "RMS Roll [°]": f"{np.rad2deg(self.rot_rms_x):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "RMS Pitch [°]": f"{np.rad2deg(self.rot_rms_y):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "RMS Yaw [°]": f"{np.rad2deg(self.rot_rms_z):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "Bias Roll [°]": f"{np.rad2deg(self.rot_bias_x):.4f}" if self.abs_dev.rot_dev is not None else "-",
             "Bias Pitch [°]": f"{np.rad2deg(self.rot_bias_y):.4f}" if self.abs_dev.rot_dev is not None else "-",
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/evaluation/comparison.py` & `trajectopy_core-3.0.0/trajectopy_core/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/evaluation/deviations.py` & `trajectopy_core-3.0.0/trajectopy_core/evaluation/deviations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/evaluation/rpe_result.py` & `trajectopy_core-3.0.0/trajectopy_core/evaluation/rpe_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import csv
 from typing import Any, Callable, Dict, List
 
 import numpy as np
 import pandas as pd
 
 from trajectopy_core.definitions import Unit
 from trajectopy_core.evaluation.deviations import RelativeTrajectoryDeviations
-from trajectopy_core.io.header import HeaderData
+from trajectopy_core.input_output.header import HeaderData
 
 
 class RPEResult:
     """
     This class represents a set of relative trajectory deviations
 
     Relative trajectory deviations describe relative pose deviations between
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/evaluation/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/io/header.py` & `trajectopy_core-3.0.0/trajectopy_core/input_output/header.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/io/rosbag.py` & `trajectopy_core-3.0.0/trajectopy_core/input_output/rosbag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from pathlib import Path
 from typing import Any, Dict, List
 
 import numpy as np
 from pointset import PointSet
 from rosbags.highlevel import AnyReader
 
-from trajectopy_core.io.rosmsg import geometry_pose_stamped_handler
+from trajectopy_core.input_output.rosmsg import geometry_pose_stamped_handler
 from trajectopy_core.rotationset import RotationSet
 from trajectopy_core.trajectory import Trajectory
 
 ROS_MESSAGE_HANDLERS = {"geometry_msgs/msg/PoseStamped": geometry_pose_stamped_handler}
 
 logger = logging.getLogger("root")
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/io/rosmsg.py` & `trajectopy_core-3.0.0/trajectopy_core/input_output/rosmsg.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/io/trajectory_io.py` & `trajectopy_core-3.0.0/trajectopy_core/input_output/trajectory_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from io import StringIO
 from typing import List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pointset import PointSet
 
 from trajectopy_core.definitions import GPS_LEAP_SECONDS, GPS_WEEK_ZERO, TimeFormat
-from trajectopy_core.io.header import HeaderData
-from trajectopy_core.io.utils import get_rot_matrix
+from trajectopy_core.input_output.header import HeaderData
+from trajectopy_core.input_output.utils import get_rot_matrix
 from trajectopy_core.rotationset import RotationSet
 
 logger = logging.getLogger("root")
 
 
 def read_data(filename: str, dtype=float) -> Tuple[HeaderData, np.ndarray]:
     """Reads the header and the data from a file
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/io/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/input_output/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/kml.py` & `trajectopy_core-3.0.0/trajectopy_core/kml.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/LICENSE` & `trajectopy_core-3.0.0/trajectopy_core/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/matching.py` & `trajectopy_core-3.0.0/trajectopy_core/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/bar_plots.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/bar_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/heatmaps.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/heatmaps.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/histograms.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/line_plots.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/multi_line_plots.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/multi_line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/scatter_plots.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/scatter_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/tables.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/tables.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/plotting/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/plotting/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from typing import List, Tuple
 
-from trajectopy_core.spatialsorter import Sorting
-from trajectopy_core.trajectory import Trajectory
+from trajectopy_core.sorting import Sorting
 
 logger = logging.getLogger("root")
 
 
 def derive_xlabel_from_sortings(sort_by_list: List[str]) -> str:
     if all(sorting == Sorting.ARC_LENGTH for sorting in sort_by_list):
         return "trajectory length [m]"
@@ -20,15 +20,15 @@
     if all(sorting == Sorting.TIME for sorting in sort_by_list):
         return "time [s]"
 
     logger.warning("Data is diffently sorted, weird things might happen.")
     return "time [s] / trajectory length [m]"
 
 
-def get_axis_label(trajectories: List[Trajectory]) -> Tuple[str, str, str]:
+def get_axis_label(trajectories: List) -> Tuple[str, str, str]:
     """Returns the unit of the axis"""
     if all(traj.pos.epsg == 0 for traj in trajectories):
         return "x [m]", "y [m]", "z [m]"
 
     unit_set = {traj.pos.crs.axis_info[0].unit_name if traj.pos.crs else "unknown" for traj in trajectories}
     unit_name = unit_set.pop().replace("metre", "m").replace("degree", "°")
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/alignment.py` & `trajectopy_core-3.0.0/trajectopy_core/report/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/assets/icon.png` & `trajectopy_core-3.0.0/trajectopy_core/report/assets/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/assets/style.css` & `trajectopy_core-3.0.0/trajectopy_core/report/assets/style.css`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/data.py` & `trajectopy_core-3.0.0/trajectopy_core/report/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/multi.py` & `trajectopy_core-3.0.0/trajectopy_core/report/multi.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/single.py` & `trajectopy_core-3.0.0/trajectopy_core/report/single.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/templates/generic.html` & `trajectopy_core-3.0.0/trajectopy_core/report/templates/generic.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/templates/multi_template.html` & `trajectopy_core-3.0.0/trajectopy_core/report/templates/multi_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/templates/single_template.html` & `trajectopy_core-3.0.0/trajectopy_core/report/templates/single_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/trajectory.py` & `trajectopy_core-3.0.0/trajectopy_core/report/trajectory.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 logger = logging.getLogger("root")
 
 
 def render_one_line_plots(
     trajectories: List[Trajectory], report_settings: ReportSettings = ReportSettings()
 ) -> List[str]:
     one_line_plots = [
-        scatter_plots.render_trajectories_mapbox(trajectories, report_settings)
-        if report_settings.scatter_mapbox
-        else scatter_plots.render_trajectories(trajectories, report_settings)
+        (
+            scatter_plots.render_trajectories_mapbox(trajectories, report_settings)
+            if report_settings.scatter_mapbox
+            else scatter_plots.render_trajectories(trajectories, report_settings)
+        )
     ]
     one_line_plots.append(multi_line_plots.render_pos_plot(trajectories, report_settings))
 
-    rot_trajectories = [traj for traj in trajectories if traj.has_orientation]
-
-    if rot_trajectories:
+    if rot_trajectories := [traj for traj in trajectories if traj.has_orientation]:
         one_line_plots.append(multi_line_plots.render_rot_plot(rot_trajectories, report_settings))
 
     return one_line_plots
 
 
 def render_trajectories(*, trajectories: List[Trajectory], report_settings: ReportSettings = ReportSettings()) -> str:
     """
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/report/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/report/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/rotationset.py` & `trajectopy_core-3.0.0/trajectopy_core/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/alignment.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,16 +225,14 @@
     std_xy_to: float = 1.0
     std_z_to: float = 1.0
     std_roll_pitch: float = float(np.deg2rad(1.0))
     std_yaw: float = float(np.deg2rad(1.0))
     std_speed: float = 1.0
     error_probability: float = 0.05
     variance_estimation: bool = False
-    variance_component_estimation: bool = False
-    variance_component_estimation_subset_size: int = 200
 
     @property
     def var_xy_from(self) -> float:
         return self.std_xy_from**2
 
     @property
     def var_z_from(self) -> float:
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/base.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/base.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/comparison.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/matching.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/processing.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/processing.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/settings/report.py` & `trajectopy_core-3.0.0/trajectopy_core/settings/report.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/trajectopy_core/spatialsorter.py` & `trajectopy_core-3.0.0/trajectopy_core/sorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 spatialsorter 
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import logging
 from enum import Enum
 from typing import List, Tuple
 
 import matplotlib.tri as mtri
 import networkx as nx
 import numpy as np
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/trajectory.py` & `trajectopy_core-3.0.0/trajectopy_core/trajectory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
+
 import copy
 import logging
-from typing import List, Union
+from typing import List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pointset import PointSet
 from scipy.spatial.transform import Slerp
 
-import trajectopy_core.io.trajectory_io as trajectory_io
+import trajectopy_core.input_output.trajectory_io as trajectory_io
+from trajectopy_core.alignment.equations import leverarm_time_component
+from trajectopy_core.alignment.parameters import AlignmentParameters
+from trajectopy_core.alignment.result import AlignmentResult
+from trajectopy_core.approximation.cubic_approximation import piecewise_cubic
+from trajectopy_core.approximation.rot_approximation import rot_average_window
 from trajectopy_core.rotationset import RotationSet
-from trajectopy_core.spatialsorter import Sorting
+from trajectopy_core.settings.approximation import ApproximationSettings
+from trajectopy_core.settings.sorting import SortingSettings
+from trajectopy_core.sorting import Sorting, sort_mls
 from trajectopy_core.utils import common_time_span, gradient_3d, lengths_from_xyz
 
 # logger configuration
 logger = logging.getLogger("root")
 
 
 class TrajectoryError(Exception):
@@ -605,7 +613,185 @@
         Returns:
             Trajectory: Transformed trajectory
 
         """
         traj_self = self if inplace else self.copy()
         traj_self.se3 = [np.dot(transformation, p) for p in traj_self.se3]
         return traj_self
+
+    def apply_alignment(self, alignment_result: AlignmentResult, inplace: bool = True) -> "Trajectory":
+        """Transforms trajectory using alignment parameters.
+
+        After computing the alignment parameters needed to align
+        two trajectories, they can be applied to arbitrary trajectories.
+
+        Args:
+            alignment_result (AlignmentResult)
+            inplace (bool, optional): Perform in-place. Defaults to True.
+
+        Returns:
+            Trajectory: Aligned trajectory
+        """
+
+        def _prepare_alignment_application(
+            trajectory: Trajectory, alignment_parameters: AlignmentParameters
+        ) -> Tuple[float, ...]:
+            if trajectory.rot is not None:
+                rpy = trajectory.rot.as_euler("xyz", degrees=False)
+                euler_x, euler_y, euler_z = rpy[:, 0], rpy[:, 1], rpy[:, 2]
+                lever_x, lever_y, lever_z = (
+                    alignment_parameters.lever_x.value,
+                    alignment_parameters.lever_y.value,
+                    alignment_parameters.lever_z.value,
+                )
+            else:
+                logger.error("Trajectory has no orientations. Cannot apply leverarm.")
+                euler_x, euler_y, euler_z = 0, 0, 0
+                lever_x, lever_y, lever_z = 0, 0, 0
+
+            return euler_x, euler_y, euler_z, lever_x, lever_y, lever_z
+
+        trajectory = trajectory if inplace else self.copy()
+
+        # leverarm and time
+        (
+            euler_x,
+            euler_y,
+            euler_z,
+            lever_x,
+            lever_y,
+            lever_z,
+        ) = _prepare_alignment_application(trajectory, alignment_result.position_parameters)
+
+        speed_3d = trajectory.speed_3d
+        speed_x, speed_y, speed_z = speed_3d[:, 0], speed_3d[:, 1], speed_3d[:, 2]
+
+        trafo_x, trafo_y, trafo_z = leverarm_time_component(
+            euler_x=euler_x,
+            euler_y=euler_y,
+            euler_z=euler_z,
+            lever_x=lever_x,
+            lever_y=lever_y,
+            lever_z=lever_z,
+            time_shift=alignment_result.position_parameters.time_shift.value,
+            speed_x=speed_x,
+            speed_y=speed_y,
+            speed_z=speed_z,
+        )
+        trajectory.pos.xyz += np.c_[trafo_x, trafo_y, trafo_z]
+
+        # similiarity transformation
+        trajectory.apply_transformation(alignment_result.position_parameters.sim3_matrix)
+
+        logger.info("Applied alignment parameters to positions.")
+
+        # sensor orientation
+        if trajectory.rot is not None:
+            trajectory.rot = alignment_result.rotation_parameters.rotation_set * trajectory.rot
+            logger.info("Applied alignment parameters to orientations.")
+
+        return trajectory
+
+    def sort_spatially(
+        self, sorting_settings: SortingSettings = SortingSettings(), inplace: bool = True
+    ) -> "Trajectory":
+        """
+        Sorts the trajectory spatially.
+
+        Args:
+            sorting_settings (SortingSettings): Sorting settings.
+            inplace (bool, optional): Whether to sort the trajectory in-place. Defaults to True.
+
+        Returns:
+            Trajectory: Sorted trajectory.
+
+        """
+        sort_idx, arc_lengths = sort_mls(xyz_unsorted=self.pos.xyz, settings=sorting_settings)
+        arg_sort_sort_idx = np.argsort(sort_idx)
+        trajectory = self.apply_index(sorted(sort_idx), inplace=inplace)
+        trajectory.arc_lengths = arc_lengths[arg_sort_sort_idx]
+        trajectory.sorting = Sorting.ARC_LENGTH
+        return trajectory
+
+    def approximate(
+        self, approximation_settings: ApproximationSettings = ApproximationSettings(), inplace: bool = True
+    ) -> "Trajectory":
+        """
+        Approximates the trajectory using piecewise cubic polynomial.
+
+        Args:
+            approximation_settings (ApproximationSettings): Approximation settings.
+
+        Returns:
+            Trajectory: Approximated trajectory.
+
+        """
+        xyz_approx = piecewise_cubic(
+            function_of=self.function_of,
+            values=self.xyz,
+            int_size=approximation_settings.fe_int_size,
+            min_obs=approximation_settings.fe_min_obs,
+        )
+
+        traj_approx = self if inplace else self.copy()
+        traj_approx.pos.xyz = xyz_approx[self.sort_switching_index, :]
+
+        if not traj_approx.has_orientation:
+            return traj_approx
+
+        quat_approx = rot_average_window(
+            function_of=self.function_of,
+            quat=self.quat,
+            win_size=approximation_settings.rot_approx_win_size,
+        )
+        traj_approx.rot = RotationSet.from_quat(quat_approx[self.sort_switching_index, :])
+
+        return traj_approx
+
+    def adopt_first_pose(self, trajectory: "Trajectory", inplace: bool = True) -> "Trajectory":
+        """Transform trajectory so that the first pose is identical in both
+
+        Args:
+            trajectory (Trajectory): Target Trajectory
+            inplace (bool, optional): Perform in-place. Defaults to True.
+
+        Returns:
+            Trajectory: Transformed trajectory
+        """
+        trajectory = self if inplace else self.copy()
+        trajectory.adopt_first_position(trajectory)
+        trajectory.adopt_first_orientation(trajectory)
+        return trajectory
+
+    def adopt_first_position(self, trajectory: "Trajectory", inplace: bool = True) -> "Trajectory":
+        """Transform trajectory so that the first position is identical in both
+
+        Args:
+            trajectory (Trajectory): Target Trajectory
+            inplace (bool, optional): Perform in-place. Defaults to True.
+
+        Returns:
+            Trajectory: Transformed trajectory
+        """
+        trajectory = self if inplace else self.copy()
+        position_difference = trajectory.pos.xyz[0, :] - trajectory.pos.xyz[0, :]
+        trajectory.pos.xyz += position_difference
+        return trajectory
+
+    def adopt_first_orientation(self, trajectory: "Trajectory", inplace: bool = True) -> "Trajectory":
+        """Transform trajectory so that the first orientation is identical in both
+
+        Args:
+            trajectory (Trajectory): Target Trajectory
+            inplace (bool, optional): Perform in-place. Defaults to True.
+
+        Returns:
+            Trajectory: Transformed trajectory
+        """
+        trajectory = self if inplace else self.copy()
+        if self.rot is not None and trajectory.rot is not None:
+            rpy_from = trajectory.rot.as_euler(seq="xyz")
+            rotation_difference = trajectory.rot.as_euler(seq="xyz")[0, :] - rpy_from[0, :]
+
+            trajectory.rot = RotationSet.from_euler(seq="xyz", angles=rpy_from + rotation_difference)
+
+        return trajectory
```

### Comparing `trajectopy_core-2.7.0/trajectopy_core/utils.py` & `trajectopy_core-3.0.0/trajectopy_core/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-2.7.0/PKG-INFO` & `trajectopy_core-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy-core
-Version: 2.7.0
+Version: 3.0.0
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 Maintainer: Gereon Tombrink
@@ -112,15 +112,15 @@
 
 This section shows how to use trajectopy to evaluate two trajectories. The example data can be found in the example_data folder. The full code can be found in the example_scripts folder.
 
 ### Absolute Trajectory Error (ATE)
 
     
 ```python
-from trajectopy_core.pipelines import ate
+from trajectopy_core.evaluation.metrics import ate
 from trajectopy_core.settings.processing import ProcessingSettings
 from trajectopy_core.trajectory import Trajectory
 
 # Import
 gt_traj = Trajectory.from_file("./example_data/KITTI_gt.traj")
 est_traj = Trajectory.from_file("./example_data/KITTI_ORB.traj")
 
@@ -130,15 +130,15 @@
 ate_result = ate(trajectory_gt=gt_traj, trajectory_est=est_traj, settings=settings)
 
 ```
 
 ### Relative Pose Error (RPE)
 
 ```python
-from trajectopy_core.pipelines import rpe
+from trajectopy_core.evaluation.metrics import rpe
 from trajectopy_core.settings.processing import ProcessingSettings
 from trajectopy_core.trajectory import Trajectory
 
 # Import
 gt_traj = Trajectory.from_file("./example_data/KITTI_gt.traj")
 est_traj = Trajectory.from_file("./example_data/KITTI_ORB.traj")
 
@@ -210,26 +210,26 @@
 - `use_x_speed` (boolean): Enable or disable the use of X-axis speed for time shift estimation.
 - `use_y_speed` (boolean): Enable or disable the use of Y-axis speed for time shift estimation.
 - `use_z_speed` (boolean): Enable or disable the use of Z-axis speed for time shift estimation.
 - `lever_x` (boolean): Enable or disable estimation of lever arm in the X-axis.
 - `lever_y` (boolean): Enable or disable estimation of lever arm in the Y-axis.
 - `lever_z` (boolean): Enable or disable estimation of lever arm in the Z-axis.
 - `sensor_rotation` (boolean): Enable or disable estimation of sensor rotation. Independent of the least squares adjustment, a constant rotational offset can be computed between the rotations of both trajectories after the alignment.
-- `auto_update` (boolean): If set to `True`, the estimation settings are automatically updated and parameters are disabled if they are not significant (experimental).
 
 ### Stochastics Settings
 
 - `std_xy_from` (float): Standard deviation of XY source position components in meters.
 - `std_z_from` (float): Standard deviation of Z source position component in meters.
 - `std_xy_to` (float): Standard deviation of XY target position components in meters.
 - `std_z_to` (float): Standard deviation of Z target position component in meters.
 - `std_roll_pitch` (float): Standard deviation of roll and pitch in radians.
 - `std_yaw` (float): Standard deviation of yaw in radians.
 - `std_speed_to` (float): Standard deviation of platform speed in (meters per second).
 - `error_probability` (float): Probability of error used for stochastic testing.
+- `variance_estimation` (boolean): Enable or disable the estimation of the variance factor for a-posteriori variance computation.
 
 ### Threshold Settings
 
 Usually, these settings can be left at their default values.
 
 - `metric_threshold` (float): Iteration threshold for the least squares adjustment regarding the metric parameters.
 - `time_threshold` (float): Iteration threshold for the least squares adjustment regarding the time shift parameter.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trajectopy-core Version: 2.7.0 Summary: Trajectory
+Metadata-Version: 2.1 Name: trajectopy-core Version: 3.0.0 Summary: Trajectory
 Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT Keywords:
 trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Author:
 Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de Maintainer: Gereon
 Tombrink Maintainer-email: tombrink@igg.uni-bonn.de Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -39,22 +39,22 @@
 ```console .\.venv\Scripts\activate ``` #### Installation via pip Update pip:
 ```console pip install --upgrade pip ``` Install trajectopy: ```console pip
 install trajectopy-core ``` ### Or using the repository: ```console pip install
 git+https://github.com/gereon-t/trajectopy-core.git@main ``` ## Exemplary
 Evaluation This section shows how to use trajectopy to evaluate two
 trajectories. The example data can be found in the example_data folder. The
 full code can be found in the example_scripts folder. ### Absolute Trajectory
-Error (ATE) ```python from trajectopy_core.pipelines import ate from
+Error (ATE) ```python from trajectopy_core.evaluation.metrics import ate from
 trajectopy_core.settings.processing import ProcessingSettings from
 trajectopy_core.trajectory import Trajectory # Import gt_traj =
 Trajectory.from_file("./example_data/KITTI_gt.traj") est_traj =
 Trajectory.from_file("./example_data/KITTI_ORB.traj") # default settings
 settings = ProcessingSettings() ate_result = ate(trajectory_gt=gt_traj,
 trajectory_est=est_traj, settings=settings) ``` ### Relative Pose Error (RPE)
-```python from trajectopy_core.pipelines import rpe from
+```python from trajectopy_core.evaluation.metrics import rpe from
 trajectopy_core.settings.processing import ProcessingSettings from
 trajectopy_core.trajectory import Trajectory # Import gt_traj =
 Trajectory.from_file("./example_data/KITTI_gt.traj") est_traj =
 Trajectory.from_file("./example_data/KITTI_ORB.traj") # default settings
 settings = ProcessingSettings() rpe_result = rpe(trajectory_gt=gt_traj,
 trajectory_est=est_traj, settings=settings) ``` ## Importing Trajectories
 Trajectory files must be ASCII files with a csv-like layout. The default column
@@ -160,29 +160,28 @@
 axis speed for time shift estimation. - `use_z_speed` (boolean): Enable or
 disable the use of Z-axis speed for time shift estimation. - `lever_x`
 (boolean): Enable or disable estimation of lever arm in the X-axis. - `lever_y`
 (boolean): Enable or disable estimation of lever arm in the Y-axis. - `lever_z`
 (boolean): Enable or disable estimation of lever arm in the Z-axis. -
 `sensor_rotation` (boolean): Enable or disable estimation of sensor rotation.
 Independent of the least squares adjustment, a constant rotational offset can
-be computed between the rotations of both trajectories after the alignment. -
-`auto_update` (boolean): If set to `True`, the estimation settings are
-automatically updated and parameters are disabled if they are not significant
-(experimental). ### Stochastics Settings - `std_xy_from` (float): Standard
-deviation of XY source position components in meters. - `std_z_from` (float):
-Standard deviation of Z source position component in meters. - `std_xy_to`
-(float): Standard deviation of XY target position components in meters. -
-`std_z_to` (float): Standard deviation of Z target position component in
-meters. - `std_roll_pitch` (float): Standard deviation of roll and pitch in
-radians. - `std_yaw` (float): Standard deviation of yaw in radians. -
-`std_speed_to` (float): Standard deviation of platform speed in (meters per
-second). - `error_probability` (float): Probability of error used for
-stochastic testing. ### Threshold Settings Usually, these settings can be left
-at their default values. - `metric_threshold` (float): Iteration threshold for
-the least squares adjustment regarding the metric parameters. -
+be computed between the rotations of both trajectories after the alignment. ###
+Stochastics Settings - `std_xy_from` (float): Standard deviation of XY source
+position components in meters. - `std_z_from` (float): Standard deviation of Z
+source position component in meters. - `std_xy_to` (float): Standard deviation
+of XY target position components in meters. - `std_z_to` (float): Standard
+deviation of Z target position component in meters. - `std_roll_pitch` (float):
+Standard deviation of roll and pitch in radians. - `std_yaw` (float): Standard
+deviation of yaw in radians. - `std_speed_to` (float): Standard deviation of
+platform speed in (meters per second). - `error_probability` (float):
+Probability of error used for stochastic testing. - `variance_estimation`
+(boolean): Enable or disable the estimation of the variance factor for a-
+posteriori variance computation. ### Threshold Settings Usually, these settings
+can be left at their default values. - `metric_threshold` (float): Iteration
+threshold for the least squares adjustment regarding the metric parameters. -
 `time_threshold` (float): Iteration threshold for the least squares adjustment
 regarding the time shift parameter. ## Matching Settings - `method`
 (`MatchingMethod`): The method used for trajectory matching. Choices:
 `MatchingMethod.NEAREST_SPATIAL`, `MatchingMethod.NEAREST_TEMPORAL`,
 `MatchingMethod.INTERPOLATION`, `MatchingMethod.NEAREST_SPATIAL_INTERPOLATED`.
 The methods are described below. - `max_time_diff` (float): Maximum allowed
 time difference when matching two trajectories using their timestamps. -
```

