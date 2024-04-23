# Comparing `tmp/puma-hep-0.3.4.tar.gz` & `tmp/puma_hep-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puma-hep-0.3.4.tar", last modified: Fri Mar  8 17:38:49 2024, max compression
+gzip compressed data, was "puma_hep-0.3.5.tar", last modified: Tue Apr 23 12:32:49 2024, max compression
```

## Comparing `puma-hep-0.3.4.tar` & `puma_hep-0.3.5.tar`

### file list

```diff
@@ -1,69 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.777568 puma-hep-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-03-08 17:38:42.000000 puma-hep-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:38:42.000000 puma-hep-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-08 17:38:49.777568 puma-hep-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-08 17:38:42.000000 puma-hep-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.773568 puma-hep-0.3.4/puma/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/fraction_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.773568 puma-hep-0.3.4/puma/hlplots/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/aux_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    32221 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/yuma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/hlplots/yutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/integrated_eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/line_plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.773568 puma-hep-0.3.4/puma/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.777568 puma-hep-0.3.4/puma/tests/hlplots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/hlplots/test_aux_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/hlplots/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/hlplots/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/hlplots/test_yuma.py
--rw-r--r--   0 runner    (1001) docker     (127)    29954 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_integrated_eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_plot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18627 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_var_vs_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/test_var_vs_vtx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.777568 puma-hep-0.3.4/puma/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/test_histogram_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/tests/utils/test_vertexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.777568 puma-hep-0.3.4/puma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/aux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/utils/vertexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17532 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/var_vs_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-03-08 17:38:42.000000 puma-hep-0.3.4/puma/var_vs_vtx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:38:49.777568 puma-hep-0.3.4/puma_hep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-08 17:38:49.000000 puma-hep-0.3.4/puma_hep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-08 17:38:42.000000 puma-hep-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-08 17:38:42.000000 puma-hep-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-08 17:38:49.781568 puma-hep-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-03-08 17:38:42.000000 puma-hep-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.284340 puma_hep-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-23 12:32:44.000000 puma_hep-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:32:44.000000 puma_hep-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-23 12:32:49.284340 puma_hep-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-23 12:32:44.000000 puma_hep-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.276340 puma_hep-0.3.5/puma/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/fraction_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31008 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.276340 puma_hep-0.3.5/puma/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16875 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/aux_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/yuma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/hlplots/yutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/integrated_eff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/line_plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/matshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.280340 puma_hep-0.3.5/puma/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.280340 puma_hep-0.3.5/puma/tests/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/hlplots/test_aux_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/hlplots/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/hlplots/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/hlplots/test_yuma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29954 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_integrated_eff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_matshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18627 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_var_vs_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/test_var_vs_vtx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.280340 puma_hep-0.3.5/puma/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_histogram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/tests/utils/test_vertexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.280340 puma_hep-0.3.5/puma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/utils/vertexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17532 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/var_vs_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-23 12:32:44.000000 puma_hep-0.3.5/puma/var_vs_vtx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:32:49.284340 puma_hep-0.3.5/puma_hep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 12:32:49.000000 puma_hep-0.3.5/puma_hep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 12:32:44.000000 puma_hep-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 12:32:44.000000 puma_hep-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 12:32:49.284340 puma_hep-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-04-23 12:32:44.000000 puma_hep-0.3.5/setup.py
```

### Comparing `puma-hep-0.3.4/LICENSE` & `puma_hep-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/PKG-INFO` & `puma_hep-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.3.4
+Version: 0.3.5
 Summary: ATLAS Flavour Tagging Plotting Code
 Home-page: https://github.com/umami-hep/puma
 Project-URL: Homepage, https://github.com/umami-hep/puma
 Project-URL: Issue Tracker, https://github.com/umami-hep/puma/issues
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.3.4/README.md` & `puma_hep-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/__init__.py` & `puma_hep-0.3.5/puma/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """puma framework - Plotting UMami Api."""
 
 # flake8: noqa
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 from puma.histogram import Histogram, HistogramPlot
 from puma.integrated_eff import IntegratedEfficiency, IntegratedEfficiencyPlot
 from puma.line_plot_2d import Line2D, Line2DPlot
 from puma.pie import PiePlot
 from puma.plot_base import PlotBase, PlotLineObject, PlotObject
 from puma.roc import Roc, RocPlot
```

### Comparing `puma-hep-0.3.4/puma/fraction_scan.py` & `puma_hep-0.3.5/puma/fraction_scan.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/histogram.py` & `puma_hep-0.3.5/puma/histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/hlplots/aux_results.py` & `puma_hep-0.3.5/puma/hlplots/aux_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from pathlib import Path
 
 import numpy as np
 from ftag import Cuts, Flavour, Flavours
 from ftag.hdf5 import H5Reader
 
 from puma.hlplots.tagger import Tagger
+from puma.matshow import MatshowPlot
 from puma.utils import logger
-from puma.utils.aux import get_aux_labels
+from puma.utils.aux import get_aux_labels, get_trackOrigin_classNames
+from puma.utils.confusion_matrix import confusion_matrix
 from puma.utils.vertexing import calculate_vertex_metrics
 from puma.var_vs_vtx import VarVsVtx, VarVsVtxPlot
 
 
 @dataclass
 class AuxResults:
     """Store information about several taggers and plot auxiliary task results."""
@@ -38,14 +40,15 @@
         if isinstance(self.perf_vars, str):
             self.perf_vars = [self.perf_vars]
         if self.atlas_second_tag is not None and self.atlas_third_tag is not None:
             self.atlas_second_tag = f"{self.atlas_second_tag}\n{self.atlas_third_tag}"
 
         self.plot_funcs = {
             "vertexing": self.plot_var_vtx_perf,
+            "track_origin": self.plot_track_origin_confmat,
         }
 
     def add(self, tagger):
         """Add tagger to class.
 
         Parameters
         ----------
@@ -131,17 +134,17 @@
         aux_labels = get_aux_labels()
 
         aux_var_list = sum([list(t.aux_variables.values()) for t in taggers], [])
         aux_var_list += sum([list(aux_labels.values()) for t in taggers], [])
         aux_var_list = list(set(aux_var_list))
 
         # load data
-        reader = H5Reader(file_path, precision="full")
+        reader = H5Reader(file_path, precision="full", shuffle=False)
         data = reader.load({key: var_list}, num_jets)[key]
-        aux_reader = H5Reader(file_path, precision="full", jets_name=aux_key)
+        aux_reader = H5Reader(file_path, precision="full", jets_name=aux_key, shuffle=False)
         aux_data = aux_reader.load({aux_key: aux_var_list}, num_jets)[aux_key]
 
         # check for nan values
         data = check_nan(data)
         # apply common cuts
         if cuts:
             idx, data = cuts(data)
@@ -382,7 +385,55 @@
                     **kwargs,
                 )
 
                 plot_vtx_fakes.add(vtx_perf, reference=tagger.reference)
 
             plot_vtx_fakes.draw()
             plot_vtx_fakes.savefig(self.get_filename(f"{flav}_vtx_fakes_vs_{perf_var}", suffix))
+
+    def plot_track_origin_confmat(
+        self,
+        normalize: str | None = "rownorm",
+        atlas_offset: float = 1.5,
+        **kwargs,
+    ):
+        """Plot Track Origin Aux Task confusion matrix.
+
+        Parameters
+        ----------
+        normalize : str | None, optional
+            Normalization of the confusion matrix. Can be:
+            None: Give raw counts;
+            "rownorm": Normalize across the prediction class, i.e. such that the rows add to one;
+            "colnorm": Normalize across the target class, i.e. such that the columns add to one;
+            "all" : Normalize across all examples, i.e. such that all matrix entries add to one.
+            Defaults to "rownorm".
+        atlas_offset : float, optional
+            Space at the top of the plot reserved to the Atlasify text. by default 1.5
+        **kwargs : kwargs
+            Keyword arguments for `puma.MatshowPlot` and `puma.PlotObject`
+        """
+        for tagger in self.taggers.values():
+            # Reading tagger's target and predicted labels
+            # and flattening them so that they have shape (Ntracks,)
+            target = tagger.aux_labels["track_origin"].reshape(-1)
+            predictions = tagger.aux_scores["track_origin"].reshape(-1)
+
+            # Computing the confusion matrix
+            cm = confusion_matrix(target, predictions, normalize=normalize)
+
+            class_names = get_trackOrigin_classNames()
+
+            # Plotting the confusion matrix
+            plot_cm = MatshowPlot(
+                x_ticklabels=class_names,
+                y_ticklabels=class_names,
+                title="Track Origin Auxiliary Task\nConfusion Matrix",
+                xlabel="Predicted Classes",
+                ylabel="Target Classes",
+                atlas_offset=atlas_offset,
+                atlas_second_tag=self.atlas_second_tag,
+                **kwargs,
+            )
+            plot_cm.draw(cm)
+            base = tagger.name + "_trackOrigin_cm"
+            plot_cm.savefig(self.get_filename(base))
```

### Comparing `puma-hep-0.3.4/puma/hlplots/results.py` & `puma_hep-0.3.5/puma/hlplots/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,17 @@
             List of background flavours, by default None, will use self.backgrounds
         **kwargs
             Keyword arguments for `puma.Line2DPlot
         """
         if self.signal not in {Flavours.bjets, Flavours.cjets}:
             raise ValueError("Signal flavour must be bjets or cjets")
 
-        backgrounds = backgrounds if backgrounds is not None else self.backgrounds
+        backgrounds = (
+            [Flavours[b] for b in backgrounds] if backgrounds is not None else self.backgrounds
+        )
         if len(backgrounds) != 2:
             raise ValueError("Only two background flavours are supported")
 
         frac = "fc" if self.signal == Flavours.bjets else "fb"
         back_str = "_".join([f.name for f in backgrounds])
         plot_name = f"{frac}_scan"
         suffix = combine_suffixes([f"{back_str}_eff{int(efficiency * 100)}", suffix])
```

### Comparing `puma-hep-0.3.4/puma/hlplots/tagger.py` & `puma_hep-0.3.5/puma/hlplots/tagger.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/hlplots/yuma.py` & `puma_hep-0.3.5/puma/hlplots/yuma.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,32 @@
 
     @classmethod
     def load_config(cls, path: Path, **kwargs) -> YumaConfig:
         if not path.exists():
             raise FileNotFoundError(f"Config at {path} does not exist")
         with open(path) as f:
             config = yaml.safe_load(f)
-        return cls(config_path=path, **config, **kwargs)
+
+        config = cls(config_path=path, **config, **kwargs)
+        config.check_config()
+        return config
+
+    def check_config(self):
+        """Checks the config for any issues, raises an error if any are found."""
+        allowed_keys = ["signal", "plot_kwargs", "include_taggers", "exclude_taggers", "reference"]
+        for plots in self.plots.values():
+            for p in plots:
+                for k in p:
+                    if k not in allowed_keys:
+                        raise ValueError(
+                            f"Unknown key {k} in plot config. Maybe '{k}' belongs"
+                            "under 'plot_kwargs'?"
+                        )
+
+        return True
 
     def get_results(self):
         """
         Create the high-level 'Results' object from the config file, using the
         previously set signal and sample. Iterates and loads all models in the config
         file, and adds them.
         """
```

### Comparing `puma-hep-0.3.4/puma/hlplots/yutils.py` & `puma_hep-0.3.5/puma/hlplots/yutils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/integrated_eff.py` & `puma_hep-0.3.5/puma/integrated_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/line_plot_2d.py` & `puma_hep-0.3.5/puma/line_plot_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/metrics.py` & `puma_hep-0.3.5/puma/metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/pie.py` & `puma_hep-0.3.5/puma/pie.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/plot_base.py` & `puma_hep-0.3.5/puma/plot_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,18 +425,18 @@
         ymin, ymax = self.axis_top.get_ylim()
         self.axis_top.set_ylim(
             ymin if self.ymin is None else self.ymin,
             ymin + (ymax - ymin) * self.y_scale if self.ymax is None else self.ymax,
         )
 
         for i, ratio_axis in enumerate(self.ratio_axes):
-            if self.ymin_ratio[i] or self.ymax_ratio[i]:
+            if self.ymin_ratio[i] is not None or self.ymax_ratio[i] is not None:
                 ymin, ymax = ratio_axis.get_ylim()
-                ymin = self.ymin_ratio[i] if self.ymin_ratio[i] else ymin
-                ymax = self.ymax_ratio[i] if self.ymax_ratio[i] else ymax
+                ymin = self.ymin_ratio[i] if self.ymin_ratio[i] is not None else ymin
+                ymax = self.ymax_ratio[i] if self.ymax_ratio[i] is not None else ymax
                 ratio_axis.set_ylim(bottom=ymin, top=ymax)
 
     def set_ylabel(self, ax_mpl, label: str | None = None, align_right: bool = True, **kwargs):
         """Set y-axis label.
 
         Parameters
         ----------
```

### Comparing `puma-hep-0.3.4/puma/roc.py` & `puma_hep-0.3.5/puma/roc.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/hlplots/test_aux_results.py` & `puma_hep-0.3.5/puma/tests/hlplots/test_aux_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,14 +190,22 @@
             auxresults.add(self.dummy_tagger)
             auxresults.plot_var_vtx_perf(vtx_flavours=["bjets"])
             self.assertIsFile(auxresults.get_filename("bjets_vtx_eff_vs_pt"))
             self.assertIsFile(auxresults.get_filename("bjets_vtx_purity_vs_pt"))
             self.assertIsFile(auxresults.get_filename("bjets_vtx_trk_eff_vs_pt"))
             self.assertIsFile(auxresults.get_filename("bjets_vtx_trk_purity_vs_pt"))
 
+    def test_plot_trackorigin_cm(self):
+        self.dummy_tagger.reference = True
+        with tempfile.TemporaryDirectory() as tmp_file:
+            auxresults = AuxResults(sample="test", output_dir=tmp_file)
+            auxresults.add(self.dummy_tagger)
+            auxresults.plot_track_origin_confmat()
+            self.assertIsFile(auxresults.get_filename(self.dummy_tagger.name + "_trackOrigin_cm"))
+
     def test_plot_var_vtx_perf_ujets(self):
         """Test that png files are being created for tagger with aux tasks."""
         self.dummy_tagger.reference = True
         with tempfile.TemporaryDirectory() as tmp_file:
             auxresults = AuxResults(sample="test", output_dir=tmp_file)
             auxresults.add(self.dummy_tagger)
             auxresults.plot_var_vtx_perf(no_vtx_flavours=["ujets"])
```

### Comparing `puma-hep-0.3.4/puma/tests/hlplots/test_results.py` & `puma_hep-0.3.5/puma/tests/hlplots/test_results.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/hlplots/test_tagger.py` & `puma_hep-0.3.5/puma/tests/hlplots/test_tagger.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/hlplots/test_yuma.py` & `puma_hep-0.3.5/puma/tests/hlplots/test_yuma.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,14 +93,37 @@
 class TestYumaPlots(unittest.TestCase):
     def testArgs(self):
         config_path = str(EXAMPLES / "plt_cfg.yaml")
         args = ["--config", config_path, "--signals", "bjets", "--plots", "not_valid"]
         with self.assertRaises(SystemExit):
             main(args)
 
+    def testCheckConfig(self):
+        with tempfile.TemporaryDirectory() as tmp_file:
+            cpath = Path(tmp_file) / "dummyconfig.yaml"
+            tmp_config = {
+                "plot_dir": "test/dir",
+                "taggers_config": {"tagger1": {"sample_path": "dummy1"}},
+                "results_config": {"sample": "ttbar"},
+                "plots": {
+                    "roc": [
+                        {
+                            "signal": "bjets",
+                            "include_taggers": ["tagger1"],
+                            "efficiency": 0.8,  # Shouldn't be here
+                        }
+                    ]
+                },
+            }
+            with open(cpath, "w") as f:
+                yaml.dump(tmp_config, f)
+            args = ["--config", cpath.as_posix(), "--signals", "bjets"]
+            with self.assertRaises(ValueError):
+                main(args)
+
     def testAllPlots(self):
         plt_cfg = EXAMPLES / "plt_cfg.yaml"
         taggers = EXAMPLES / "taggers.yaml"
         plt_cfg, taggers = load_no_include(plt_cfg, taggers)
 
         with tempfile.TemporaryDirectory() as tmp_file:
             fpath1, _file = get_mock_file(fname=(Path(tmp_file) / "file1.h5").as_posix())
```

### Comparing `puma-hep-0.3.4/puma/tests/test_histogram.py` & `puma_hep-0.3.5/puma/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_integrated_eff.py` & `puma_hep-0.3.5/puma/tests/test_integrated_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_line_2d.py` & `puma_hep-0.3.5/puma/tests/test_line_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_metrics.py` & `puma_hep-0.3.5/puma/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_pie_chart.py` & `puma_hep-0.3.5/puma/tests/test_pie_chart.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_plot_base.py` & `puma_hep-0.3.5/puma/tests/test_plot_base.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_roc.py` & `puma_hep-0.3.5/puma/tests/test_roc.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_var_vs_eff.py` & `puma_hep-0.3.5/puma/tests/test_var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_var_vs_var.py` & `puma_hep-0.3.5/puma/tests/test_var_vs_var.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/test_var_vs_vtx.py` & `puma_hep-0.3.5/puma/tests/test_var_vs_vtx.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/utils/test_generate.py` & `puma_hep-0.3.5/puma/tests/utils/test_generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/utils/test_histogram_utils.py` & `puma_hep-0.3.5/puma/tests/utils/test_histogram_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/utils/test_utils.py` & `puma_hep-0.3.5/puma/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/tests/utils/test_vertexing.py` & `puma_hep-0.3.5/puma/tests/utils/test_vertexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,24 +345,24 @@
         np.testing.assert_array_equal(metrics["test_vertex_size"], [[2, -1]])
         np.testing.assert_array_equal(metrics["ref_vertex_size"], [[2, -1]])
 
 
 class CleanTruthVerticesTestCase(unittest.TestCase):
     """Test case for clean_truth_vertices function."""
 
-    def test_track_removal(self):
-        """Check case where PV, PU and fake tracks are removed."""
-        vtx_indices = np.array([1, 0, 1, 0, 0, 1, 2, 0, 2, 2])
-        trk_origin = np.array([2, 0, 2, 1, 1, 2, 2, 0, 4, 4])
+    def test_non_hf_vtx_removal(self):
+        """Check case where non-pure HF vertices are removed."""
+        vtx_indices = np.array([1, 0, 1, 0, 0, 1, 2, 0, 2, 2, 3, 3])
+        trk_origin = np.array([2, 0, 2, 1, 1, 2, 2, 0, 4, 4, 3, 3])
         cleaned_indices = clean_truth_vertices(vtx_indices, trk_origin)
-        expected_result = np.array([-99, -99, -99, -99, -99, -99, -99, -99, 2, 2])
+        expected_result = np.array([-99, -99, -99, -99, -99, -99, -99, -99, -99, -99, 3, 3])
         np.testing.assert_array_equal(cleaned_indices, expected_result)
 
-    def test_incl_track_merging(self):
-        """Check case in inclusive vertexing where HF tracks are merged."""
+    def test_incl_hf_vtx_merging(self):
+        """Check case in inclusive vertexing where HF vertices are merged."""
         vtx_indices = np.array([0, 0, 1, 2, 1, 2, 2, 2])
         trk_origin = np.array([2, 2, 3, 4, 3, 4, 4, 4])
         cleaned_indices = clean_truth_vertices(vtx_indices, trk_origin, incl_vertexing=True)
         expected_result = np.array([-99, -99, 3, 3, 3, 3, 3, 3])
         np.testing.assert_array_equal(cleaned_indices, expected_result)
 
 
@@ -373,14 +373,22 @@
         """Check case where PV in model with track origin prediction is removed."""
         vtx_indices = np.array([0, 0, 0, 0, 0, 1, 1, 1, 1])
         trk_origin = np.array([2, 4, 2, 2, 2, 2, 3, 3, 4])
         cleaned_indices = clean_reco_vertices(vtx_indices, trk_origin)
         expected_result = np.array([-99, -99, -99, -99, -99, 1, 1, 1, 1])
         np.testing.assert_array_equal(cleaned_indices, expected_result)
 
+    def test_non_hf_vtx_removal(self):
+        """Check case where vertices without HF track are removed."""
+        vtx_indices = np.array([1, 0, 1, 0, 0, 1, 2, 0, 2, 2, 3, 3])
+        trk_origin = np.array([2, 0, 2, 1, 1, 2, 2, 0, 4, 4, 3, 3])
+        cleaned_indices = clean_reco_vertices(vtx_indices, trk_origin)
+        expected_result = np.array([-99, -99, -99, -99, -99, -99, 2, -99, 2, 2, 3, 3])
+        np.testing.assert_array_equal(cleaned_indices, expected_result)
+
     def test_incl_track_merging_hf(self):
         """Check case in incl vertexing w track origin prediction where HF vertices are merged."""
         vtx_indices = np.array([0, 0, 1, 2, 1, 2, 2, 1, 3, 3])
         trk_origin = np.array([2, 2, 3, 3, 3, 5, 7, 5, 7, 7])
         cleaned_indices = clean_reco_vertices(vtx_indices, trk_origin, incl_vertexing=True)
         expected_result = np.array([-99, -99, 3, 3, 3, 3, 3, 3, -99, -99])
         np.testing.assert_array_equal(cleaned_indices, expected_result)
```

### Comparing `puma-hep-0.3.4/puma/utils/__init__.py` & `puma_hep-0.3.5/puma/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/utils/generate.py` & `puma_hep-0.3.5/puma/utils/generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/utils/histogram.py` & `puma_hep-0.3.5/puma/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/utils/logging.py` & `puma_hep-0.3.5/puma/utils/logging.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/utils/vertexing.py` & `puma_hep-0.3.5/puma/utils/vertexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,16 +234,16 @@
 
     return metrics
 
 
 def clean_truth_vertices(truth_vertices, truth_track_origin, incl_vertexing=False):
     """
     Clean truth vertices for each track in a single jet. This function removes
-    all truth PV, PU and fake tracks from truth vertices. If inclusive vertexing
-    is enabled, it also merges HF tracks into a single vertex.
+    all truth vertices that are not entirely from HF. If inclusive vertexing
+    is enabled, it also merges remaining vertices into a single vertex.
 
     Parameters
     ----------
     truth_vertices: np.ndarray
         Array containing truth vertex indices for each track in a jet.
     truth_track_origin: np.ndarray
         Array containing truth track origin labels for each track in a jet.
@@ -251,34 +251,27 @@
         Whether to merge all vertex indices, by default False.
 
     Returns
     -------
     truth_vertices: np.ndarray
         Array containing cleaned truth vertex indices for each track in a jet.
     """
-    # clean truth vertex indices - remove indices from true PV, PU, fake
-    truth_removal_cond = np.logical_or(
-        truth_vertices == 0,
-        np.isin(truth_track_origin, [0, 1, 2]),
-    )
+    # remove vertices that aren't purely HF
+    removal_indices = np.unique(truth_vertices[np.isin(truth_track_origin, [3, 4, 5], invert=True)])
     truth_vertices = clean_indices(
         truth_vertices,
-        truth_removal_cond,
+        np.isin(truth_vertices, removal_indices),
         mode="remove",
     )
 
     # merge truth vertices from HF for inclusive performance
     if incl_vertexing:
-        truth_merge_cond = np.logical_and(
-            truth_vertices > 0,
-            np.isin(truth_track_origin, [3, 4, 5]),
-        )
         truth_vertices = clean_indices(
             truth_vertices,
-            truth_merge_cond,
+            truth_vertices > 0,
             mode="merge",
         )
 
     return truth_vertices
 
 
 def clean_reco_vertices(reco_vertices, reco_track_origin=None, incl_vertexing=False):
@@ -313,25 +306,27 @@
             pv_index = pv_candidate_indices[np.argmax(pv_candidate_counts)]
             reco_vertices = clean_indices(
                 reco_vertices,
                 reco_vertices == pv_index,
                 mode="remove",
             )
 
-        # merge vertices with > 0 tracks from HF and remove others
+        # remove vertices with no tracks from HF
+        hf_vertex_indices = np.unique(reco_vertices[np.isin(reco_track_origin, [3, 4, 5])])
+        reco_vertices = clean_indices(
+            reco_vertices,
+            np.isin(reco_vertices, hf_vertex_indices, invert=True),
+            mode="remove",
+        )
+
+        # merge remaining vertices for inclusive performance
         if incl_vertexing:
-            hf_vertex_indices = np.unique(reco_vertices[np.isin(reco_track_origin, [3, 4, 5, 6])])
-            reco_vertices = clean_indices(
-                reco_vertices,
-                np.isin(reco_vertices, hf_vertex_indices, invert=True),
-                mode="remove",
-            )
             reco_vertices = clean_indices(
                 reco_vertices,
-                np.isin(reco_vertices, hf_vertex_indices),
+                reco_vertices >= 0,
                 mode="merge",
             )
 
     # merge all reco vertices if track origin predictions are not available
     elif incl_vertexing:
         reco_vertices = clean_indices(
             reco_vertices,
```

### Comparing `puma-hep-0.3.4/puma/var_vs_eff.py` & `puma_hep-0.3.5/puma/var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/var_vs_var.py` & `puma_hep-0.3.5/puma/var_vs_var.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma/var_vs_vtx.py` & `puma_hep-0.3.5/puma/var_vs_vtx.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.3.4/puma_hep.egg-info/PKG-INFO` & `puma_hep-0.3.5/puma_hep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.3.4
+Version: 0.3.5
 Summary: ATLAS Flavour Tagging Plotting Code
 Home-page: https://github.com/umami-hep/puma
 Project-URL: Homepage, https://github.com/umami-hep/puma
 Project-URL: Issue Tracker, https://github.com/umami-hep/puma/issues
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.3.4/puma_hep.egg-info/SOURCES.txt` & `puma_hep-0.3.5/puma_hep.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.cfg
 setup.py
 puma/__init__.py
 puma/fraction_scan.py
 puma/histogram.py
 puma/integrated_eff.py
 puma/line_plot_2d.py
+puma/matshow.py
 puma/metrics.py
 puma/pie.py
 puma/plot_base.py
 puma/roc.py
 puma/var_vs_eff.py
 puma/var_vs_var.py
 puma/var_vs_vtx.py
@@ -23,34 +24,37 @@
 puma/hlplots/tagger.py
 puma/hlplots/yuma.py
 puma/hlplots/yutils.py
 puma/tests/__init__.py
 puma/tests/test_histogram.py
 puma/tests/test_integrated_eff.py
 puma/tests/test_line_2d.py
+puma/tests/test_matshow.py
 puma/tests/test_metrics.py
 puma/tests/test_pie_chart.py
 puma/tests/test_plot_base.py
 puma/tests/test_roc.py
 puma/tests/test_var_vs_eff.py
 puma/tests/test_var_vs_var.py
 puma/tests/test_var_vs_vtx.py
 puma/tests/hlplots/__init__.py
 puma/tests/hlplots/test_aux_results.py
 puma/tests/hlplots/test_results.py
 puma/tests/hlplots/test_tagger.py
 puma/tests/hlplots/test_yuma.py
 puma/tests/utils/__init__.py
+puma/tests/utils/test_confusion_matrix.py
 puma/tests/utils/test_generate.py
 puma/tests/utils/test_histogram_utils.py
 puma/tests/utils/test_logging.py
 puma/tests/utils/test_utils.py
 puma/tests/utils/test_vertexing.py
 puma/utils/__init__.py
 puma/utils/aux.py
+puma/utils/confusion_matrix.py
 puma/utils/generate.py
 puma/utils/histogram.py
 puma/utils/logging.py
 puma/utils/vertexing.py
 puma_hep.egg-info/PKG-INFO
 puma_hep.egg-info/SOURCES.txt
 puma_hep.egg-info/dependency_links.txt
```

### Comparing `puma-hep-0.3.4/pyproject.toml` & `puma_hep-0.3.5/pyproject.toml`

 * *Files identical despite different names*

