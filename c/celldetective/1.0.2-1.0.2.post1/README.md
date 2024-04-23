# Comparing `tmp/celldetective-1.0.2.tar.gz` & `tmp/celldetective-1.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celldetective-1.0.2.tar", last modified: Tue Apr 23 14:38:09 2024, max compression
+gzip compressed data, was "celldetective-1.0.2.post1.tar", last modified: Tue Apr 23 15:50:24 2024, max compression
```

## Comparing `celldetective-1.0.2.tar` & `celldetective-1.0.2.post1.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 14:38:01.000000 celldetective-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-23 14:38:09.643888 celldetective-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    10795 2024-04-23 14:38:01.000000 celldetective-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.631888 celldetective-1.0.2/celldetective/
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14033 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.627888 celldetective-1.0.2/celldetective/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.635888 celldetective-1.0.2/celldetective/datasets/segmentation_annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/datasets/segmentation_annotations/blank
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.635888 celldetective-1.0.2/celldetective/datasets/signal_annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/datasets/signal_annotations/blank
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/extra_properties.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.639888 celldetective-1.0.2/celldetective/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)      921 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/about.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24199 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/analyze_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/btrack_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/classifier_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18931 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/configure_new_exp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15688 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/control_panel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15584 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/gui_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3620 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/json_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    68074 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/measurement_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/neighborhood_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    43616 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/plot_signals_ui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41764 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/process_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    27208 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/retrain_segmentation_model_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    24206 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/retrain_signal_model_options.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17167 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/seg_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    98494 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/signal_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/signal_annotator_options.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3874 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32711 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/survival_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/tableUI.py
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/gui/thresholds_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.639888 celldetective-1.0.2/celldetective/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    36631 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/signals_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/splash-test.png
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/splash0.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/survival2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/vignette_signals2.png
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/icons/vignette_signals2.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    73349 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.639888 celldetective-1.0.2/celldetective/links/
--rw-r--r--   0 runner    (1001) docker     (127)    22728 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/links/zenodo.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    57027 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/measure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.627888 celldetective-1.0.2/celldetective/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/models/segmentation_effectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/segmentation_effectors/blank
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/models/segmentation_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/segmentation_generic/blank
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/models/segmentation_targets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/segmentation_targets/blank
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/models/signal_detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/signal_detection/blank
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/models/tracking_configs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/tracking_configs/mcf7.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     2727 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/tracking_configs/ricm.json
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/models/tracking_configs/ricm2.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    30880 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/neighborhood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/analyze_signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10240 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/measure_cells.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7494 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/segment_cells.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4998 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/segment_cells_thresholds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7510 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/track_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/train_segmentation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/scripts/train_signal_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28496 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/segmentation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   104258 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37570 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/tracking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59280 2024-04-23 14:38:01.000000 celldetective-1.0.2/celldetective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:09.643888 celldetective-1.0.2/celldetective.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 14:38:09.000000 celldetective-1.0.2/celldetective.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:38:09.643888 celldetective-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-23 14:38:01.000000 celldetective-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10825 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.364762 celldetective-1.0.2.post1/celldetective/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14033 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.356762 celldetective-1.0.2.post1/celldetective/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.364762 celldetective-1.0.2.post1/celldetective/datasets/segmentation_annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/datasets/segmentation_annotations/blank
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.364762 celldetective-1.0.2.post1/celldetective/datasets/signal_annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/datasets/signal_annotations/blank
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/extra_properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.368762 celldetective-1.0.2.post1/celldetective/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      921 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/about.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24199 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/analyze_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/btrack_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/classifier_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18931 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/configure_new_exp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15688 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/control_panel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15584 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/gui_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3620 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/json_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68074 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/measurement_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/neighborhood_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43616 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/plot_signals_ui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41764 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/process_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27208 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/retrain_segmentation_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24206 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/retrain_signal_model_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17167 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/seg_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98494 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/signal_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/signal_annotator_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3874 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32711 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/survival_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/tableUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/gui/thresholds_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    36631 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/signals_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/splash-test.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/splash0.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/survival2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/vignette_signals2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/icons/vignette_signals2.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73349 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/links/
+-rw-r--r--   0 runner    (1001) docker     (127)    22728 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/links/zenodo.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57027 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/measure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.360762 celldetective-1.0.2.post1/celldetective/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/models/segmentation_effectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/segmentation_effectors/blank
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/models/segmentation_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/segmentation_generic/blank
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/models/segmentation_targets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/segmentation_targets/blank
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/models/signal_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/signal_detection/blank
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/models/tracking_configs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/tracking_configs/mcf7.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2727 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/tracking_configs/ricm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/models/tracking_configs/ricm2.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30880 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/neighborhood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/analyze_signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10240 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/measure_cells.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7494 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/segment_cells.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4998 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/segment_cells_thresholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7510 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/track_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/train_segmentation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/scripts/train_signal_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28496 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/segmentation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104258 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37570 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/tracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59280 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/celldetective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/celldetective.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 15:50:24.000000 celldetective-1.0.2.post1/celldetective.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:50:24.372762 celldetective-1.0.2.post1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1419 2024-04-23 15:50:20.000000 celldetective-1.0.2.post1/setup.py
```

### Comparing `celldetective-1.0.2/LICENSE` & `celldetective-1.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/PKG-INFO` & `celldetective-1.0.2.post1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: celldetective
-Version: 1.0.2
-Summary: description
-Home-page: http://github.com/remyeltorro/celldetective
-Author: Rémy Torro
-Author-email: remy.torro@inserm.fr
-License: GPL-3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Celldetective
+=============
 
 .. raw:: html
 
 	<embed>
 		<p align="center">
 		<img src="https://github.com/remyeltorro/celldetective/blob/main/celldetective/icons/logo-large.png" width="33%" />
 		</p>
 	</embed>
 
 |ico1| |ico2| |ico3|
-
+ 
 .. |ico1| image:: https://img.shields.io/readthedocs/celldetective?link=https%3A%2F%2Fcelldetective.readthedocs.io%2Fen%2Flatest%2Findex.html
 
 .. |ico2| image:: https://img.shields.io/github/forks/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fforks
 
 .. |ico3| image:: https://img.shields.io/github/stars/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fstargazers
```

### Comparing `celldetective-1.0.2/README.rst` & `celldetective-1.0.2.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,58 @@
+Metadata-Version: 2.1
+Name: celldetective
+Version: 1.0.2.post1
+Summary: description
+Home-page: http://github.com/remyeltorro/celldetective
+Author: Rémy Torro
+Author-email: remy.torro@inserm.fr
+License: GPL-3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: wheel
+Requires-Dist: nbsphinx
+Requires-Dist: nbsphinx_link
+Requires-Dist: sphinx_rtd_theme
+Requires-Dist: sphinx==5.0.2
+Requires-Dist: jinja2<3.1
+Requires-Dist: ipykernel
+Requires-Dist: stardist
+Requires-Dist: cellpose<3
+Requires-Dist: scikit-learn
+Requires-Dist: btrack
+Requires-Dist: tensorflow<=2.12.1
+Requires-Dist: napari
+Requires-Dist: tqdm
+Requires-Dist: mahotas
+Requires-Dist: fonticon-materialdesignicons6
+Requires-Dist: art
+Requires-Dist: lifelines
+Requires-Dist: setuptools
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: liblapack
+Requires-Dist: gputools
+Requires-Dist: lmfit~=1.2.2
+Requires-Dist: superqt>=0.6.1
+Requires-Dist: setuptools
+
+Celldetective
+=============
+
 .. raw:: html
 
 	<embed>
 		<p align="center">
 		<img src="https://github.com/remyeltorro/celldetective/blob/main/celldetective/icons/logo-large.png" width="33%" />
 		</p>
 	</embed>
 
 |ico1| |ico2| |ico3|
-
+ 
 .. |ico1| image:: https://img.shields.io/readthedocs/celldetective?link=https%3A%2F%2Fcelldetective.readthedocs.io%2Fen%2Flatest%2Findex.html
 
 .. |ico2| image:: https://img.shields.io/github/forks/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fforks
 
 .. |ico3| image:: https://img.shields.io/github/stars/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fstargazers
```

### Comparing `celldetective-1.0.2/celldetective/__main__.py` & `celldetective-1.0.2.post1/celldetective/__main__.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/events.py` & `celldetective-1.0.2.post1/celldetective/events.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/extra_properties.py` & `celldetective-1.0.2.post1/celldetective/extra_properties.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/filters.py` & `celldetective-1.0.2.post1/celldetective/filters.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/__init__.py` & `celldetective-1.0.2.post1/celldetective/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/about.py` & `celldetective-1.0.2.post1/celldetective/gui/about.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/analyze_block.py` & `celldetective-1.0.2.post1/celldetective/gui/analyze_block.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/btrack_options.py` & `celldetective-1.0.2.post1/celldetective/gui/btrack_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/classifier_widget.py` & `celldetective-1.0.2.post1/celldetective/gui/classifier_widget.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/configure_new_exp.py` & `celldetective-1.0.2.post1/celldetective/gui/configure_new_exp.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/control_panel.py` & `celldetective-1.0.2.post1/celldetective/gui/control_panel.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/gui_utils.py` & `celldetective-1.0.2.post1/celldetective/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/json_readers.py` & `celldetective-1.0.2.post1/celldetective/gui/json_readers.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/measurement_options.py` & `celldetective-1.0.2.post1/celldetective/gui/measurement_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/neighborhood_options.py` & `celldetective-1.0.2.post1/celldetective/gui/neighborhood_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/plot_signals_ui.py` & `celldetective-1.0.2.post1/celldetective/gui/plot_signals_ui.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/process_block.py` & `celldetective-1.0.2.post1/celldetective/gui/process_block.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/retrain_segmentation_model_options.py` & `celldetective-1.0.2.post1/celldetective/gui/retrain_segmentation_model_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/retrain_signal_model_options.py` & `celldetective-1.0.2.post1/celldetective/gui/retrain_signal_model_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/seg_model_loader.py` & `celldetective-1.0.2.post1/celldetective/gui/seg_model_loader.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/signal_annotator.py` & `celldetective-1.0.2.post1/celldetective/gui/signal_annotator.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/signal_annotator_options.py` & `celldetective-1.0.2.post1/celldetective/gui/signal_annotator_options.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/styles.py` & `celldetective-1.0.2.post1/celldetective/gui/styles.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/survival_ui.py` & `celldetective-1.0.2.post1/celldetective/gui/survival_ui.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/tableUI.py` & `celldetective-1.0.2.post1/celldetective/gui/tableUI.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/gui/thresholds_gui.py` & `celldetective-1.0.2.post1/celldetective/gui/thresholds_gui.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/logo-large.png` & `celldetective-1.0.2.post1/celldetective/icons/logo-large.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/logo.png` & `celldetective-1.0.2.post1/celldetective/icons/logo.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/signals_icon.png` & `celldetective-1.0.2.post1/celldetective/icons/signals_icon.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/splash-test.png` & `celldetective-1.0.2.post1/celldetective/icons/splash-test.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/splash.png` & `celldetective-1.0.2.post1/celldetective/icons/splash.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/splash0.png` & `celldetective-1.0.2.post1/celldetective/icons/splash0.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/survival2.png` & `celldetective-1.0.2.post1/celldetective/icons/survival2.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/vignette_signals2.png` & `celldetective-1.0.2.post1/celldetective/icons/vignette_signals2.png`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/icons/vignette_signals2.svg` & `celldetective-1.0.2.post1/celldetective/icons/vignette_signals2.svg`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/io.py` & `celldetective-1.0.2.post1/celldetective/io.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/links/zenodo.json` & `celldetective-1.0.2.post1/celldetective/links/zenodo.json`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/measure.py` & `celldetective-1.0.2.post1/celldetective/measure.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/models/tracking_configs/mcf7.json` & `celldetective-1.0.2.post1/celldetective/models/tracking_configs/mcf7.json`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/models/tracking_configs/ricm.json` & `celldetective-1.0.2.post1/celldetective/models/tracking_configs/ricm.json`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/models/tracking_configs/ricm2.json` & `celldetective-1.0.2.post1/celldetective/models/tracking_configs/ricm2.json`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/neighborhood.py` & `celldetective-1.0.2.post1/celldetective/neighborhood.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/analyze_signals.py` & `celldetective-1.0.2.post1/celldetective/scripts/analyze_signals.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/measure_cells.py` & `celldetective-1.0.2.post1/celldetective/scripts/measure_cells.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/segment_cells.py` & `celldetective-1.0.2.post1/celldetective/scripts/segment_cells.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/segment_cells_thresholds.py` & `celldetective-1.0.2.post1/celldetective/scripts/segment_cells_thresholds.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/track_cells.py` & `celldetective-1.0.2.post1/celldetective/scripts/track_cells.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/train_segmentation_model.py` & `celldetective-1.0.2.post1/celldetective/scripts/train_segmentation_model.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/scripts/train_signal_model.py` & `celldetective-1.0.2.post1/celldetective/scripts/train_signal_model.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/segmentation.py` & `celldetective-1.0.2.post1/celldetective/segmentation.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/signals.py` & `celldetective-1.0.2.post1/celldetective/signals.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/tracking.py` & `celldetective-1.0.2.post1/celldetective/tracking.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective/utils.py` & `celldetective-1.0.2.post1/celldetective/utils.py`

 * *Files identical despite different names*

### Comparing `celldetective-1.0.2/celldetective.egg-info/PKG-INFO` & `celldetective-1.0.2.post1/celldetective.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 Metadata-Version: 2.1
 Name: celldetective
-Version: 1.0.2
+Version: 1.0.2.post1
 Summary: description
 Home-page: http://github.com/remyeltorro/celldetective
 Author: Rémy Torro
 Author-email: remy.torro@inserm.fr
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: wheel
+Requires-Dist: nbsphinx
+Requires-Dist: nbsphinx_link
+Requires-Dist: sphinx_rtd_theme
+Requires-Dist: sphinx==5.0.2
+Requires-Dist: jinja2<3.1
+Requires-Dist: ipykernel
+Requires-Dist: stardist
+Requires-Dist: cellpose<3
+Requires-Dist: scikit-learn
+Requires-Dist: btrack
+Requires-Dist: tensorflow<=2.12.1
+Requires-Dist: napari
+Requires-Dist: tqdm
+Requires-Dist: mahotas
+Requires-Dist: fonticon-materialdesignicons6
+Requires-Dist: art
+Requires-Dist: lifelines
+Requires-Dist: setuptools
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: liblapack
+Requires-Dist: gputools
+Requires-Dist: lmfit~=1.2.2
+Requires-Dist: superqt>=0.6.1
+Requires-Dist: setuptools
+
+Celldetective
+=============
 
 .. raw:: html
 
 	<embed>
 		<p align="center">
 		<img src="https://github.com/remyeltorro/celldetective/blob/main/celldetective/icons/logo-large.png" width="33%" />
 		</p>
 	</embed>
 
 |ico1| |ico2| |ico3|
-
+ 
 .. |ico1| image:: https://img.shields.io/readthedocs/celldetective?link=https%3A%2F%2Fcelldetective.readthedocs.io%2Fen%2Flatest%2Findex.html
 
 .. |ico2| image:: https://img.shields.io/github/forks/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fforks
 
 .. |ico3| image:: https://img.shields.io/github/stars/remyeltorro/celldetective?link=https%3A%2F%2Fgithub.com%2Fremyeltorro%2Fcelldetective%2Fstargazers
```

### Comparing `celldetective-1.0.2/celldetective.egg-info/SOURCES.txt` & `celldetective-1.0.2.post1/celldetective.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 celldetective/tracking.py
 celldetective/utils.py
 celldetective.egg-info/PKG-INFO
 celldetective.egg-info/SOURCES.txt
 celldetective.egg-info/dependency_links.txt
 celldetective.egg-info/entry_points.txt
 celldetective.egg-info/not-zip-safe
+celldetective.egg-info/requires.txt
 celldetective.egg-info/top_level.txt
 celldetective/datasets/segmentation_annotations/blank
 celldetective/datasets/signal_annotations/blank
 celldetective/gui/__init__.py
 celldetective/gui/about.py
 celldetective/gui/analyze_block.py
 celldetective/gui/btrack_options.py
```

