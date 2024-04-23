# Comparing `tmp/diplomat_track-0.1.3.tar.gz` & `tmp/diplomat_track-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diplomat_track-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "diplomat_track-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `diplomat_track-0.1.3.tar` & `diplomat_track-0.1.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     6853 2024-04-18 17:00:47.958715 diplomat_track-0.1.3/README.md
--rw-r--r--   0        0        0     2548 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/__init__.py
--rw-r--r--   0        0        0       45 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/__main__.py
--rw-r--r--   0        0        0     2456 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/_cli_runner.py
--rw-r--r--   0        0        0    23069 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/core_ops.py
--rw-r--r--   0        0        0     1432 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontend_ops.py
--rw-r--r--   0        0        0     7089 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/__init__.py
--rw-r--r--   0        0        0      901 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/csv/__init__.py
--rw-r--r--   0        0        0      475 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/csv/_verify_func.py
--rw-r--r--   0        0        0      938 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/csv/csv_utils.py
--rw-r--r--   0        0        0     5436 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/csv/label_videos.py
--rw-r--r--   0        0        0     3049 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/csv/tweak_results.py
--rw-r--r--   0        0        0     1464 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/__init__.py
--rw-r--r--   0        0        0      980 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/_verify_func.py
--rw-r--r--   0        0        0     2879 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/convert_results_dlc.py
--rw-r--r--   0        0        0      679 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/dlc_importer.py
--rw-r--r--   0        0        0    10254 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/label_videos_dlc.py
--rw-r--r--   0        0        0    13430 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/predict_frames_dlc.py
--rw-r--r--   0        0        0    19593 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/predict_videos_dlc.py
--rw-r--r--   0        0        0     1806 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/save_from_restore.py
--rw-r--r--   0        0        0     4185 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/deeplabcut/tweak_results.py
--rw-r--r--   0        0        0     1391 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/__init__.py
--rw-r--r--   0        0        0      458 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/_verify_func.py
--rw-r--r--   0        0        0     1704 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/convert_results_sleap.py
--rw-r--r--   0        0        0     5323 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/label_videos_sleap.py
--rw-r--r--   0        0        0     8744 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/predict_frames_sleap.py
--rw-r--r--   0        0        0     6413 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/predict_videos_sleap.py
--rw-r--r--   0        0        0     9260 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/run_utils.py
--rw-r--r--   0        0        0     1355 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/save_from_restore.py
--rw-r--r--   0        0        0      590 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/sleap_importer.py
--rw-r--r--   0        0        0    12331 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/sleap_providers.py
--rw-r--r--   0        0        0     2539 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/tweak_results_sleap.py
--rw-r--r--   0        0        0     2277 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/frontends/sleap/visual_settings.py
--rw-r--r--   0        0        0     5416 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictor_ops.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/__init__.py
--rw-r--r--   0        0        0      699 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/argmax.py
--rw-r--r--   0        0        0    14516 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fastplotter.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/__init__.py
--rw-r--r--   0        0        0     4917 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/arr_utils.py
--rw-r--r--   0        0        0     1319 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_help.py
--rw-r--r--   0        0        0     7374 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_math.py
--rw-r--r--   0        0        0    24838 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_test_data.py
--rw-r--r--   0        0        0     4284 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass.py
--rw-r--r--   0        0        0    23216 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass_engine.py
--rw-r--r--   0        0        0     1530 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass_loader.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/__init__.py
--rw-r--r--   0        0        0    11011 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/cluster_frames.py
--rw-r--r--   0        0        0     9363 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/create_skeleton.py
--rw-r--r--   0        0        0    26266 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/fix_frame.py
--rw-r--r--   0        0        0    48985 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
--rw-r--r--   0        0        0     5120 2024-04-18 17:00:47.962715 diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/optimize_std.py
--rw-r--r--   0        0        0    13500 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/fpe/skeleton_structures.py
--rw-r--r--   0        0        0    29594 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/fpe/sparse_storage.py
--rw-r--r--   0        0        0     5863 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/frame_exporter.py
--rw-r--r--   0        0        0    11920 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/plotter.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/__init__.py
--rw-r--r--   0        0        0      767 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/assignment.py
--rw-r--r--   0        0        0    14995 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/avl_tree.py
--rw-r--r--   0        0        0     9344 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/disk_sparse_storage.py
--rw-r--r--   0        0        0    18778 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/file_io.py
--rw-r--r--   0        0        0     1361 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/growable_numpy_array.py
--rw-r--r--   0        0        0     4263 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/segmentation.py
--rw-r--r--   0        0        0    70601 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/__init__.py
--rw-r--r--   0        0        0    20059 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/labelers.py
--rw-r--r--   0        0        0     6622 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/scorers.py
--rw-r--r--   0        0        0    18822 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_sfpe/__init__.py
--rw-r--r--   0        0        0    28291 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
--rw-r--r--   0        0        0     2168 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/__init__.py
--rw-r--r--   0        0        0     3523 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/containers.py
--rw-r--r--   0        0        0    11144 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/pose.py
--rw-r--r--   0        0        0    13781 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/predictor.py
--rw-r--r--   0        0        0     3749 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/progress_bar.py
--rw-r--r--   0        0        0    18651 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/track_data.py
--rw-r--r--   0        0        0    21853 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/processing/type_casters.py
--rw-r--r--   0        0        0       96 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/__init__.py
--rw-r--r--   0        0        0      360 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/_bit_or.py
--rw-r--r--   0        0        0      874 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/_function_tools.py
--rw-r--r--   0        0        0    11484 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/cli_tools.py
--rw-r--r--   0        0        0     3153 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/colormaps.py
--rw-r--r--   0        0        0    11695 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/extract_frames.py
--rw-r--r--   0        0        0    10794 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/frame_store_api.py
--rw-r--r--   0        0        0    28484 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/frame_store_fmt.py
--rw-r--r--   0        0        0     8442 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/graph_ops.py
--rw-r--r--   0        0        0     3980 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/lazy_import.py
--rw-r--r--   0        0        0     4284 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/pluginloader.py
--rw-r--r--   0        0        0     1690 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/pretty_printer.py
--rw-r--r--   0        0        0     6965 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/shapes.py
--rw-r--r--   0        0        0     2816 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/track_formats.py
--rw-r--r--   0        0        0    11520 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/tweak_ui.py
--rw-r--r--   0        0        0      925 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/video_info.py
--rw-r--r--   0        0        0     1596 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/video_io.py
--rw-r--r--   0        0        0     6823 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/utils/video_splitter.py
--rw-r--r--   0        0        0      403 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/wx_gui/__init__.py
--rw-r--r--   0        0        0    37702 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/wx_gui/fpe_editor.py
--rw-r--r--   0        0        0     4670 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/wx_gui/helpdialog.py
--rw-r--r--   0        0        0    14468 2024-04-18 17:00:47.966715 diplomat_track-0.1.3/diplomat/wx_gui/icons.py
--rw-r--r--   0        0        0    14402 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/id_swap_dialog.py
--rw-r--r--   0        0        0     2026 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/identity_swapper.py
--rw-r--r--   0        0        0    15199 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/labeler_lib.py
--rw-r--r--   0        0        0    46523 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/point_edit.py
--rw-r--r--   0        0        0    25981 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/probability_displayer.py
--rw-r--r--   0        0        0     7308 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/progress_bar.py
--rw-r--r--   0        0        0     2382 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/progress_dialog.py
--rw-r--r--   0        0        0     6002 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/score_lib.py
--rw-r--r--   0        0        0     8477 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/scroll_image_list.py
--rw-r--r--   0        0        0     4380 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/settings_dialog.py
--rw-r--r--   0        0        0    35348 2024-04-18 17:00:47.970715 diplomat_track-0.1.3/diplomat/wx_gui/video_player.py
--rw-r--r--   0        0        0     1119 2024-04-18 17:00:48.010715 diplomat_track-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 diplomat_track-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6853 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/README.md
+-rw-r--r--   0        0        0     2548 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/__main__.py
+-rw-r--r--   0        0        0     2456 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/_cli_runner.py
+-rw-r--r--   0        0        0    23434 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/core_ops.py
+-rw-r--r--   0        0        0     1432 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontend_ops.py
+-rw-r--r--   0        0        0     7089 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/csv/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/csv/_verify_func.py
+-rw-r--r--   0        0        0      938 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/csv/csv_utils.py
+-rw-r--r--   0        0        0     5436 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/csv/label_videos.py
+-rw-r--r--   0        0        0     3049 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/csv/tweak_results.py
+-rw-r--r--   0        0        0     1464 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/__init__.py
+-rw-r--r--   0        0        0      980 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/_verify_func.py
+-rw-r--r--   0        0        0     2879 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/convert_results_dlc.py
+-rw-r--r--   0        0        0      679 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/dlc_importer.py
+-rw-r--r--   0        0        0    10254 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/label_videos_dlc.py
+-rw-r--r--   0        0        0    13430 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/predict_frames_dlc.py
+-rw-r--r--   0        0        0    19583 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/predict_videos_dlc.py
+-rw-r--r--   0        0        0     1806 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/save_from_restore.py
+-rw-r--r--   0        0        0     4185 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/deeplabcut/tweak_results.py
+-rw-r--r--   0        0        0     1391 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/sleap/__init__.py
+-rw-r--r--   0        0        0      458 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/sleap/_verify_func.py
+-rw-r--r--   0        0        0     1704 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/sleap/convert_results_sleap.py
+-rw-r--r--   0        0        0     5323 2024-04-22 19:10:48.967755 diplomat_track-0.1.4/diplomat/frontends/sleap/label_videos_sleap.py
+-rw-r--r--   0        0        0     8744 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/predict_frames_sleap.py
+-rw-r--r--   0        0        0     6418 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/predict_videos_sleap.py
+-rw-r--r--   0        0        0     9260 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/run_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/save_from_restore.py
+-rw-r--r--   0        0        0      590 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/sleap_importer.py
+-rw-r--r--   0        0        0    12331 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/sleap_providers.py
+-rw-r--r--   0        0        0     2539 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/tweak_results_sleap.py
+-rw-r--r--   0        0        0     2277 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/frontends/sleap/visual_settings.py
+-rw-r--r--   0        0        0     5416 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictor_ops.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/argmax.py
+-rw-r--r--   0        0        0    14516 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fastplotter.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/__init__.py
+-rw-r--r--   0        0        0     4917 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/arr_utils.py
+-rw-r--r--   0        0        0     1319 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_help.py
+-rw-r--r--   0        0        0     7374 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_math.py
+-rw-r--r--   0        0        0    24838 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_test_data.py
+-rw-r--r--   0        0        0     4284 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass.py
+-rw-r--r--   0        0        0    23216 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass_engine.py
+-rw-r--r--   0        0        0     1530 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass_loader.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/__init__.py
+-rw-r--r--   0        0        0    11011 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/cluster_frames.py
+-rw-r--r--   0        0        0     9363 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/create_skeleton.py
+-rw-r--r--   0        0        0    26266 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/fix_frame.py
+-rw-r--r--   0        0        0    48985 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
+-rw-r--r--   0        0        0     5120 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/optimize_std.py
+-rw-r--r--   0        0        0    13500 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/skeleton_structures.py
+-rw-r--r--   0        0        0    30391 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/fpe/sparse_storage.py
+-rw-r--r--   0        0        0     5863 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/frame_exporter.py
+-rw-r--r--   0        0        0    11920 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/plotter.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/__init__.py
+-rw-r--r--   0        0        0      767 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/assignment.py
+-rw-r--r--   0        0        0    14995 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/avl_tree.py
+-rw-r--r--   0        0        0     9344 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/disk_sparse_storage.py
+-rw-r--r--   0        0        0    18778 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/file_io.py
+-rw-r--r--   0        0        0     1361 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/growable_numpy_array.py
+-rw-r--r--   0        0        0     4263 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/segmentation.py
+-rw-r--r--   0        0        0    70649 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/__init__.py
+-rw-r--r--   0        0        0    26301 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/labelers.py
+-rw-r--r--   0        0        0     6622 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/scorers.py
+-rw-r--r--   0        0        0    18822 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_sfpe/__init__.py
+-rw-r--r--   0        0        0    28291 2024-04-22 19:10:48.971755 diplomat_track-0.1.4/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0     2168 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/__init__.py
+-rw-r--r--   0        0        0     3523 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/containers.py
+-rw-r--r--   0        0        0    11144 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/pose.py
+-rw-r--r--   0        0        0    13781 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/predictor.py
+-rw-r--r--   0        0        0     3749 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/progress_bar.py
+-rw-r--r--   0        0        0    18651 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/track_data.py
+-rw-r--r--   0        0        0    21853 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/processing/type_casters.py
+-rw-r--r--   0        0        0       96 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/_bit_or.py
+-rw-r--r--   0        0        0      874 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/_function_tools.py
+-rw-r--r--   0        0        0    11484 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/cli_tools.py
+-rw-r--r--   0        0        0     3153 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/colormaps.py
+-rw-r--r--   0        0        0    11695 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/extract_frames.py
+-rw-r--r--   0        0        0    10794 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/frame_store_api.py
+-rw-r--r--   0        0        0    28484 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/frame_store_fmt.py
+-rw-r--r--   0        0        0     8442 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/graph_ops.py
+-rw-r--r--   0        0        0     3980 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/lazy_import.py
+-rw-r--r--   0        0        0     4284 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/pluginloader.py
+-rw-r--r--   0        0        0     1690 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/pretty_printer.py
+-rw-r--r--   0        0        0     6965 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/shapes.py
+-rw-r--r--   0        0        0     2816 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/track_formats.py
+-rw-r--r--   0        0        0    11520 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/tweak_ui.py
+-rw-r--r--   0        0        0      925 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/video_info.py
+-rw-r--r--   0        0        0     1596 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/video_io.py
+-rw-r--r--   0        0        0     6823 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/utils/video_splitter.py
+-rw-r--r--   0        0        0      403 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/__init__.py
+-rw-r--r--   0        0        0    37702 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/fpe_editor.py
+-rw-r--r--   0        0        0     4670 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/helpdialog.py
+-rw-r--r--   0        0        0    14468 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/icons.py
+-rw-r--r--   0        0        0    14402 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/id_swap_dialog.py
+-rw-r--r--   0        0        0     2026 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/identity_swapper.py
+-rw-r--r--   0        0        0    15199 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/labeler_lib.py
+-rw-r--r--   0        0        0    46523 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/point_edit.py
+-rw-r--r--   0        0        0    25981 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/probability_displayer.py
+-rw-r--r--   0        0        0     7308 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/progress_bar.py
+-rw-r--r--   0        0        0     2382 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/progress_dialog.py
+-rw-r--r--   0        0        0     6002 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/score_lib.py
+-rw-r--r--   0        0        0     8477 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/scroll_image_list.py
+-rw-r--r--   0        0        0     4380 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/settings_dialog.py
+-rw-r--r--   0        0        0    35348 2024-04-22 19:10:48.975756 diplomat_track-0.1.4/diplomat/wx_gui/video_player.py
+-rw-r--r--   0        0        0     1119 2024-04-22 19:10:49.019756 diplomat_track-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 diplomat_track-0.1.4/PKG-INFO
```

### Comparing `diplomat_track-0.1.3/README.md` & `diplomat_track-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/__init__.py` & `diplomat_track-0.1.4/diplomat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 """
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 # Can be used by functions to determine if diplomat was invoked through it's CLI interface.
 CLI_RUN = False
 
 from diplomat.predictor_ops import list_predictor_plugins, get_predictor_settings, test_predictor_plugin
 from diplomat.frontend_ops import list_all_frontends, list_loaded_frontends
 from diplomat.utils.video_splitter import split_videos
 from diplomat.core_ops import track_with, track, track_and_interact, annotate, tweak, yaml, convert, interact
```

### Comparing `diplomat_track-0.1.3/diplomat/_cli_runner.py` & `diplomat_track-0.1.4/diplomat/_cli_runner.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/core_ops.py` & `diplomat_track-0.1.4/diplomat/core_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,28 @@
     config: Union[List[os.PathLike], os.PathLike],
     **kwargs: typing.Any
 ) -> typing.Tuple[str, ModuleType]:
     from diplomat import _LOADED_FRONTENDS
 
     contracts = [contracts] if(isinstance(contracts, DIPLOMATContract)) else contracts
 
+    print(f"Loaded frontends: {_LOADED_FRONTENDS}")
+
+    print(f"Config: {config}")
+
+
+
     for name, funcs in _LOADED_FRONTENDS.items():
+        print(f"Checking frontend '{name}'...")
+
+        for contract in contracts:
+            print(f"Verifying contract '{contract}'...")
+            verified = funcs.verify(contract=contract, config=config, **kwargs)
+            print(f"Verified: {verified}")
+        
         if(all(funcs.verify(
             contract=c,
             config=config,
             **kwargs
         ) for c in contracts)):
             print(f"Frontend '{name}' selected.")
             return (name, funcs)
@@ -216,15 +229,15 @@
 
     if(videos is None and frame_stores is None):
         print("No frame stores or videos passed, terminating.")
         return
 
     # If some videos are supplied, run the frontends video analysis function.
     if(videos is not None):
-        print("Running on videos...")
+        print("Running on videos... TEST")
         selected_frontend.analyze_videos(
             config=config,
             videos=videos,
             num_outputs=num_outputs,
             predictor=predictor,
             predictor_settings=predictor_settings,
             **_get_casted_args(selected_frontend.analyze_videos, extra_args)
```

### Comparing `diplomat_track-0.1.3/diplomat/frontend_ops.py` & `diplomat_track-0.1.4/diplomat/frontend_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/__init__.py` & `diplomat_track-0.1.4/diplomat/frontends/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/csv/__init__.py` & `diplomat_track-0.1.4/diplomat/frontends/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/csv/csv_utils.py` & `diplomat_track-0.1.4/diplomat/frontends/csv/csv_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/csv/label_videos.py` & `diplomat_track-0.1.4/diplomat/frontends/csv/label_videos.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/csv/tweak_results.py` & `diplomat_track-0.1.4/diplomat/frontends/csv/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/__init__.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/_verify_func.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/_verify_func.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/convert_results_dlc.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/convert_results_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/dlc_importer.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/dlc_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/label_videos_dlc.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/label_videos_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/predict_frames_dlc.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/predict_frames_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/predict_videos_dlc.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/predict_videos_dlc.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,20 +38,21 @@
     destination_folder: tc.Optional[str] = None,
     batch_size: tc.Optional[int] = None,
     cropping: tc.Optional[tc.Tuple[int, int, int, int]] = None,
     model_prefix: str = "",
     num_outputs: tc.Optional[int] = None,
     multi_output_format: tc.Literal["default", "separate"] = "default",
     predictor: tc.Optional[str] = None,
-    predictor_settings: tc.Optional[tc.Dict[str, tc.Any]] = None
+    predictor_settings: tc.Optional[tc.Dict[str, tc.Any]] = None,
 ):
     """
     Run DIPLOMAT tracking on videos using a DEEPLABCUT project and trained network.
 
     :param config: The path to the DLC config for the DEEPLABCUT project.
+
     :param videos: A single path or list of paths, to the location of video files to run analysis on. Can also be a directory.
     :param video_type: Optional string, the video extension to search for if the 'videos' argument is a directory
                        to search inside ('.avi', '.mp4', ...).
     :param shuffle: int, optional. Integer specifying which TrainingsetFraction to use. By default, the first
                     (note that TrainingFraction is a list in config.yaml).
     :param training_set_index: int, optional. Integer specifying which TrainingsetFraction to use. By default the first
                                (note that TrainingFraction is a list in config.yaml).
@@ -166,15 +167,14 @@
                 inputs,
                 outputs,
                 table_header,
                 save_as_csv,
                 destination_folder,
                 predictor_cls,
                 predictor_settings,
-                dipui_file=None
             )
     else:
         print("No videos found!")
 
     model_config["num_outputs"] = old_num_outputs
     os.chdir(this_dir)
 
@@ -193,14 +193,15 @@
     inputs: tf.compat.v1.Tensor,
     outputs: List[tf.compat.v1.Tensor],
     table_header,
     save_as_csv,
     dest_folder=None,
     predictor_cls=None,
     predictor_settings=None,
+    dipui_file=None
 ) -> str:
     print(f"Analyzing video: {video}")
 
     dest_folder = Path(Path(video).resolve().parent if(dest_folder is None) else dest_folder)
     dest_folder.mkdir(exist_ok=True)
 
     video_name = Path(video).stem
```

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/save_from_restore.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/deeplabcut/tweak_results.py` & `diplomat_track-0.1.4/diplomat/frontends/deeplabcut/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/__init__.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/convert_results_sleap.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/convert_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/label_videos_sleap.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/label_videos_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/predict_frames_sleap.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/predict_frames_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/predict_videos_sleap.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/predict_videos_sleap.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     _setup_gpus(use_cpu, gpu_index)
 
     import sleap
     batch_size = _get_default_value(sleap.load_model, "batch_size", 4) if(batch_size is None) else batch_size
     if(num_outputs is None):
         raise ValueError("'num_outputs' is not set! Please set it to the number of bodies you are tracking.")
 
-    print("Loading Model...")
+    print("Loading Model... TEST")
     model = sleap.load_model(_paths_to_str(config), batch_size=batch_size)
     # Get the model extractor...
     mdl_extractor = PredictorExtractor(model, refinement_kernel_size)
     mdl_metadata = mdl_extractor.get_metadata()
 
     predictor_cls = get_predictor("SegmentedFramePassEngine" if(predictor is None) else predictor)
     print(f"Using predictor: '{predictor_cls.get_name()}'")
```

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/run_utils.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/run_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/save_from_restore.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/sleap_importer.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/sleap_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/sleap_providers.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/sleap_providers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/tweak_results_sleap.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/tweak_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/frontends/sleap/visual_settings.py` & `diplomat_track-0.1.4/diplomat/frontends/sleap/visual_settings.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictor_ops.py` & `diplomat_track-0.1.4/diplomat/predictor_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/argmax.py` & `diplomat_track-0.1.4/diplomat/predictors/argmax.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fastplotter.py` & `diplomat_track-0.1.4/diplomat/predictors/fastplotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/arr_utils.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/arr_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_help.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_help.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_math.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_math.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/fpe_test_data.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/fpe_test_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass_engine.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_pass_loader.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_pass_loader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/cluster_frames.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/cluster_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/create_skeleton.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/create_skeleton.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/fix_frame.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/fix_frame.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/mit_viterbi.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/mit_viterbi.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/frame_passes/optimize_std.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/frame_passes/optimize_std.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/skeleton_structures.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/skeleton_structures.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/fpe/sparse_storage.py` & `diplomat_track-0.1.4/diplomat/predictors/fpe/sparse_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,30 @@
             self._off_access = None
             self._coords_access = None
             self._prob_access = None
             return self, 4
 
         float_offset = 4 + length * 2 * np.dtype(int_dtype).itemsize
 
-        self._coords = np.frombuffer(data, np.dtype(int_dtype), length * 2, 4).reshape((length, 2))
+        # Calculate the expected size of the data based on `length` and `int_dtype`
+        int_dtype_size = np.dtype(int_dtype).itemsize  # Size of int_dtype in bytes
+        expected_data_size = length * 2 * int_dtype_size + 4  # +4 for the offset
+
+        # Check if the actual data buffer is smaller than expected
+        if len(data) < expected_data_size:
+            print(f"Error: The data buffer length {len(data)} is smaller than the expected size {expected_data_size}.")
+
+        # Proceed with the original line, wrapped in a try-except block for safety
+        try:
+            self._coords = np.frombuffer(data, np.dtype(int_dtype), length * 2, 4).reshape((length, 2))
+        except ValueError as e:
+            print(f"Encountered an error when trying to reshape the data: {e}")
+
+
+        #self._coords = np.frombuffer(data, np.dtype(int_dtype), length * 2, 4).reshape((length, 2))
         self._coords_access = self.NumpyAccessor(self._coords)
         self._offsets_probs = np.frombuffer(data, np.dtype(float_dtype), length * 3, float_offset).reshape((length, 3))
         self._off_access = self.NumpyAccessor(self._offsets_probs, (slice(1, 3),))
         self._prob_access = self.NumpyAccessor(self._offsets_probs, (0,))
 
         return self, float_offset + length * 3 * np.dtype(float_dtype).itemsize
```

### Comparing `diplomat_track-0.1.3/diplomat/predictors/frame_exporter.py` & `diplomat_track-0.1.4/diplomat/predictors/frame_exporter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/plotter.py` & `diplomat_track-0.1.4/diplomat/predictors/plotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/assignment.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/assignment.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/avl_tree.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/avl_tree.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/disk_sparse_storage.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/disk_sparse_storage.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/file_io.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/file_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/growable_numpy_array.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/growable_numpy_array.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/segmentation.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/segmentation.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/sfpe/segmented_frame_pass_engine.py` & `diplomat_track-0.1.4/diplomat/predictors/sfpe/segmented_frame_pass_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 import os
+from datetime import datetime
 import shutil
 from enum import Enum
 from datetime import datetime
 from pathlib import Path
 from typing import List, Tuple, Optional, Any, Callable, Sequence, Iterable, BinaryIO
 import numpy as np
 from diplomat.processing import *
@@ -132,15 +133,17 @@
             self._internal_prog_data[self.PROGRESS] + amt,
             self._internal_prog_data[self.TOTAL]
         )
         self.rate_limit_update()
 
     def rate_limit_update(self):
         new_time = time.monotonic()
-        if(new_time - self._last_update > self._refresh_rate):
+        if(new_time - self._last_update 
+           
+           self._refresh_rate):
             self._last_update = new_time
             self.update_shared_mem(self._internal_prog_data)
 
     def update_shared_mem(self, data: list):
         self._prog_data[:] = data
 
     def get_prog_info(self) -> Tuple[int, int, int]:
@@ -463,18 +466,18 @@
 
         Returns:
             DiskBackedForwardBackwardData: An object that holds and manages access to the frames data.
         """
         timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
         output_path = Path(self.video_metadata["output-file-path"]).resolve()
         if self.settings.dipui_file is not None:
-            dipui_path = str(self.settings.dipui_file)
-            if os.path.exists(dipui_path):
-                output_path = dipui_path.replace(".dipui","") + f"_{timestamp}.dipui"
-            output_path = Path(output_path).resolve()
+            output_path = Path(self.settings.dipui_file).resolve()
+            if os.path.exists(output_path):
+                timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
+                output_path += timestamp
         else:
             output_path = output_path.parent / f"{output_path.stem}_{timestamp}{output_path.suffix}"
 
         video_path = Path(self.video_metadata["orig-video-path"]).resolve()
         disk_path = output_path.parent / (output_path.stem + ".dipui")
 
         self._file_obj = disk_path.open("w+b")
@@ -1591,15 +1594,17 @@
                 "Location to store frames while the algorithm is running."
             ),
             "memory_cache_size": (
                 100,
                 type_casters.RangedInteger(1, np.inf),
                 "Size of lifo cache used to temporarily store frames loaded from disk if running in disk storage_mode."
             ),
-            "dipui_file": (None, type_casters.Union(type_casters.Literal(None), str), "A path specifying where to save the dipui file"),
+            "dipui_file": (None, type_casters.Union(type_casters.Literal(None), str), "A path specifying where to save the dipui file"
+            )
+
         }
 
     @classmethod
     def get_tests(cls) -> Optional[List[TestFunction]]:
         return [
             cls.test_plotting,
             cls.test_sparsification,
```

### Comparing `diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/scorers.py` & `diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/scorers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py` & `diplomat_track-0.1.4/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py` & `diplomat_track-0.1.4/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/__init__.py` & `diplomat_track-0.1.4/diplomat/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/containers.py` & `diplomat_track-0.1.4/diplomat/processing/containers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/pose.py` & `diplomat_track-0.1.4/diplomat/processing/pose.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/predictor.py` & `diplomat_track-0.1.4/diplomat/processing/predictor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/progress_bar.py` & `diplomat_track-0.1.4/diplomat/processing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/track_data.py` & `diplomat_track-0.1.4/diplomat/processing/track_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/processing/type_casters.py` & `diplomat_track-0.1.4/diplomat/processing/type_casters.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/_function_tools.py` & `diplomat_track-0.1.4/diplomat/utils/_function_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/cli_tools.py` & `diplomat_track-0.1.4/diplomat/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/colormaps.py` & `diplomat_track-0.1.4/diplomat/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/extract_frames.py` & `diplomat_track-0.1.4/diplomat/utils/extract_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/frame_store_api.py` & `diplomat_track-0.1.4/diplomat/utils/frame_store_api.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/frame_store_fmt.py` & `diplomat_track-0.1.4/diplomat/utils/frame_store_fmt.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/graph_ops.py` & `diplomat_track-0.1.4/diplomat/utils/graph_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/lazy_import.py` & `diplomat_track-0.1.4/diplomat/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/pluginloader.py` & `diplomat_track-0.1.4/diplomat/utils/pluginloader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/pretty_printer.py` & `diplomat_track-0.1.4/diplomat/utils/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/shapes.py` & `diplomat_track-0.1.4/diplomat/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/track_formats.py` & `diplomat_track-0.1.4/diplomat/utils/track_formats.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/tweak_ui.py` & `diplomat_track-0.1.4/diplomat/utils/tweak_ui.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/video_info.py` & `diplomat_track-0.1.4/diplomat/utils/video_info.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/video_io.py` & `diplomat_track-0.1.4/diplomat/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/utils/video_splitter.py` & `diplomat_track-0.1.4/diplomat/utils/video_splitter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/fpe_editor.py` & `diplomat_track-0.1.4/diplomat/wx_gui/fpe_editor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/helpdialog.py` & `diplomat_track-0.1.4/diplomat/wx_gui/helpdialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/icons.py` & `diplomat_track-0.1.4/diplomat/wx_gui/icons.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/id_swap_dialog.py` & `diplomat_track-0.1.4/diplomat/wx_gui/id_swap_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/identity_swapper.py` & `diplomat_track-0.1.4/diplomat/wx_gui/identity_swapper.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/labeler_lib.py` & `diplomat_track-0.1.4/diplomat/wx_gui/labeler_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/point_edit.py` & `diplomat_track-0.1.4/diplomat/wx_gui/point_edit.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/probability_displayer.py` & `diplomat_track-0.1.4/diplomat/wx_gui/probability_displayer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/progress_bar.py` & `diplomat_track-0.1.4/diplomat/wx_gui/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/progress_dialog.py` & `diplomat_track-0.1.4/diplomat/wx_gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/score_lib.py` & `diplomat_track-0.1.4/diplomat/wx_gui/score_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/scroll_image_list.py` & `diplomat_track-0.1.4/diplomat/wx_gui/scroll_image_list.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/settings_dialog.py` & `diplomat_track-0.1.4/diplomat/wx_gui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/diplomat/wx_gui/video_player.py` & `diplomat_track-0.1.4/diplomat/wx_gui/video_player.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/pyproject.toml` & `diplomat_track-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.3/PKG-INFO` & `diplomat_track-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diplomat-track
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 Author-email: Isaac Robinson <isaac.k.robinson2000@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

