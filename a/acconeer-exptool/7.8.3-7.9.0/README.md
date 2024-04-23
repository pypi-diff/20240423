# Comparing `tmp/acconeer-exptool-7.8.3.tar.gz` & `tmp/acconeer-exptool-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-7.8.3.tar", last modified: Wed Mar 20 10:08:06 2024, max compression
+gzip compressed data, was "acconeer-exptool-7.9.0.tar", last modified: Wed Mar 27 13:09:10 2024, max compression
```

## Comparing `acconeer-exptool-7.8.3.tar` & `acconeer-exptool-7.9.0.tar`

### file list

```diff
@@ -1,724 +1,728 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.200218 acconeer-exptool-7.8.3/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.120218 acconeer-exptool-7.8.3/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      415 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      206 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18217 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/CHANGELOG.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16194 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10709 2024-03-20 10:08:06.200218 acconeer-exptool-7.8.3/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8238 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2024-03-20 09:25:07.000000 acconeer-exptool-7.8.3/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1895 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-7.8.3/docker/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1613 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.120218 acconeer-exptool-7.8.3/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.120218 acconeer-exptool-7.8.3/examples/a121/algo/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8169 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2318 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/breathing/breathing.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14865 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/breathing/breathing_with_gui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-10-11 21:09:39.000000 acconeer-exptool-7.8.3/examples/a121/algo/distance/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2108 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/examples/a121/algo/distance/post_process_distance_result.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-10-11 21:09:39.000000 acconeer-exptool-7.8.3/examples/a121/algo/distance/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/algo/hand_motion/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1414 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/hand_motion/hand_motion_example_app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.132218 acconeer-exptool-7.8.3/examples/a121/algo/obstacle/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13857 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/obstacle/detector.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5803 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/phase_tracking/phase_tracking.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-10-11 21:09:39.000000 acconeer-exptool-7.8.3/examples/a121/algo/presence/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11023 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10428 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/smart_presence/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17511 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/smart_presence/ref_app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/speed/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9028 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/speed/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9176 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/speed/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/surface_velocity/example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8863 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/algo/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2388 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/examples/a121/algo/tank_level/tank_level.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9918 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/examples/a121/algo/tank_level/tank_level_with_gui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11882 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/algo/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8404 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/examples/a121/algo/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/algo/waste_level/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15674 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/examples/a121/algo/waste_level/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/examples/a121/basic.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/examples/a121/load_record_h5.m
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/examples/a121/plot.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4561 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/post_process_sparse_iq.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/examples/a121/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/record_data/with_cli.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/examples/a121/reuse_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4252 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/examples/a121/stress.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/gui/main.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7006 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/portable/package/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      592 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/portable/package/README.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/portable/package/update.bat
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2703 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2612 2024-03-20 10:08:06.200218 acconeer-exptool-7.8.3/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.128218 acconeer-exptool-7.8.3/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.120218 acconeer-exptool-7.8.3/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      327 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.136218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      350 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      123 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1398 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/attrs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5435 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/descriptors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1183 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/enum.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      405 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/formatting.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      404 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7126 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10074 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/comm_devices.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      148 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      367 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      614 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1107 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      645 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      679 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      972 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      718 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1329 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/protocol.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1369 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/buffered_link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3507 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/helpers.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      881 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/null_link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10450 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/serial_link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2461 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/socket_link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2770 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/usb_link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3231 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/message_stream.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2047 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/unwrap_ticks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      937 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/docstrings.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      313 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8835 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/client_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1089 2024-03-19 22:08:53.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/validation_result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1110 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/int_16_complex.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      167 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.140218 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      133 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6609 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3530 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/saver.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      940 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_session_schema.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1374 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2476 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_core/version_parsing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5888 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4262 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2020 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18332 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/json/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.144218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24890 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9857 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11317 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4935 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21419 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.148218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      588 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2533 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9165 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.152218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15249 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14234 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.156218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10410 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3129 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4665 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1383 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      944 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      380 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6295 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12704 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5868 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4308 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1078 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11309 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/mock_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      758 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      550 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.160218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      238 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3636 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22122 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10940 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9624 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      534 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4808 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8247 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2319 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2977 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2248 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      725 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      320 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      234 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8265 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3035 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3504 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6874 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/saver.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3582 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      961 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11976 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5167 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7915 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_perf_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      879 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3558 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      404 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7291 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      729 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3671 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      378 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11298 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1060 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6619 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20270 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26990 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17502 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.164218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      303 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      759 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20282 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8660 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    33221 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5798 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    61875 2024-03-19 11:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28471 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5836 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_pidget_mapping.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    29382 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      232 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13243 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20944 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9984 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_mode_handler.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      279 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      853 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30732 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27106 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_detector_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23850 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      385 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1364 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12100 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_processors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21128 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    33044 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_ref_app_plugin.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1066 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10153 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7799 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.168218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      252 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2856 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15929 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25864 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7315 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_pidget_mapping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18396 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8375 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6606 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18518 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    33100 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      949 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15561 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3686 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      213 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      345 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14721 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22726 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4802 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      181 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11623 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24450 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14019 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-06-27 15:00:16.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29808 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7432 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6316 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      381 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1176 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1325 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2333 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19663 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17865 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.172218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      419 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1115 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13255 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12595 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      239 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      808 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20369 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7077 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       56 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7408 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/memory.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9290 2024-03-20 10:00:03.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/algo.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14738 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/api.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      312 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/dependency_injection.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4824 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/domain.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7844 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/lookup.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      336 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4761 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      898 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_argument_parser.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1718 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      987 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2838 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.176218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      174 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    29439 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      981 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      317 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2094 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      598 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3818 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1614 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2234 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2012 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4618 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3195 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_rate_calc.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_tasks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2151 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      290 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3293 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1330 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1928 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1560 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/visual_policies.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      360 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2226 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/app_model_viewer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      590 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6258 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3719 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/perf_calc_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2022 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/range_help_view.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13690 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/sensor_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17155 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/session_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8434 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/subsweep_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7156 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1358 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/collapsible_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      590 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/goto_resource_tab_button.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4117 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/group_box.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.180218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      262 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7950 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/buttons.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      282 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2650 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/load_dialog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2851 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/preview.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1775 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/save_dialog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/set_config_presenter.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3423 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/syntax_highlight.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1424 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/misc_error_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      802 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3845 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/hooks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2055 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/pidget_groups.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    28216 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/pidgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2519 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/tab_pg_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1657 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/two_sensor_ids_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2687 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       94 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14431 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4604 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17705 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2979 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/icons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4748 2024-01-12 11:00:48.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/main_window.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1994 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1271 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/animation.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5482 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/event_system.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      723 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/_preset_selection.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5180 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/distance_config_input.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4403 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/memory_breakdown_output.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16800 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/power_consumption_vs_rate_output.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14258 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/power_curve_output.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5594 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/presence_config_input.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4014 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/session_config_input.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18599 2024-03-20 10:06:00.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9636 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.184218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       98 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11165 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4912 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13917 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4721 2023-10-11 21:09:39.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3623 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1807 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84004 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/modules.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/loader.gif
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   183522 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/new_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/old_gui.png
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.128218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.188218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6060 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3656 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4287 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13021 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_mcumgruart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      148 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_mcumgruart/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14409 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_mcumgruart/_mcumgrflasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      127 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_mcumgruart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1078 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.192218 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6663 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9146 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9444 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/mpl_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      206 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1411 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11251 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/builtin_persistors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11966 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/core.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13233 2023-11-29 08:00:18.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/optimizing_persistors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3536 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/opser/registry_persistor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3917 2024-03-15 14:00:20.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/pg_process.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/setup_group.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2952 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       96 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      329 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/linux.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1211 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/ubuntu_22_04.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13147 2024-03-19 22:08:55.000000 acconeer-exptool-7.8.3/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10709 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30118 2024-03-20 10:08:06.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      566 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2024-03-20 10:08:05.000000 acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/tools/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/tools/check_changelog.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13869 2024-03-19 22:08:52.000000 acconeer-exptool-7.8.3/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/tools/check_permissions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-10-11 21:09:38.000000 acconeer-exptool-7.8.3/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-7.8.3/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2073 2024-01-16 22:00:08.000000 acconeer-exptool-7.8.3/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-20 10:08:06.196218 acconeer-exptool-7.8.3/utils/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    31174 2024-03-19 22:08:54.000000 acconeer-exptool-7.8.3/utils/convert_h5.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.020107 acconeer-exptool-7.9.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      415 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      206 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18455 2024-03-27 13:04:59.000000 acconeer-exptool-7.9.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16194 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10709 2024-03-27 13:09:10.020107 acconeer-exptool-7.9.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8238 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2024-03-27 13:04:59.000000 acconeer-exptool-7.9.0/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1895 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/docker/requirements-dev.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1613 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/examples/a121/algo/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8169 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2318 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/breathing/breathing.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14865 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/breathing/breathing_with_gui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4522 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/distance/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2108 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/distance/post_process_distance_result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/distance/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/hand_motion/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1414 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/hand_motion/hand_motion_example_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/obstacle/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13857 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/obstacle/detector.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5803 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/phase_tracking/phase_tracking.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11241 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/presence/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11023 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10428 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/smart_presence/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17511 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/smart_presence/ref_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9028 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/speed/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9176 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/speed/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/surface_velocity/example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8863 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2388 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/tank_level/tank_level.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9918 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/tank_level/tank_level_with_gui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11882 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8404 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/algo/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.956108 acconeer-exptool-7.9.0/examples/a121/algo/waste_level/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15674 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/examples/a121/algo/waste_level/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1222 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      776 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/load_record_h5.m
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/plot.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4561 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/post_process_sparse_iq.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/examples/a121/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/record_data/with_cli.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1140 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/reuse_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4252 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/stress.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/examples/app/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/examples/app/new/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/examples/app/new/plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7289 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/examples/app/new/plugins/my_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/gui/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7006 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      592 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/package/README.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/portable/package/update.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2703 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2612 2024-03-27 13:09:10.020107 acconeer-exptool-7.9.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.944108 acconeer-exptool-7.9.0/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      327 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      350 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      123 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1398 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/attrs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5435 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/descriptors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1183 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/enum.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      405 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/formatting.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      404 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7126 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10074 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/comm_devices.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.960108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      148 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      614 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1107 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      645 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      679 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      972 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      718 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1329 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/protocol.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1369 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/buffered_link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3507 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/helpers.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      881 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/null_link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10450 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/serial_link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2461 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/socket_link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2770 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/usb_link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3231 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/message_stream.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2047 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/unwrap_ticks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      937 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/docstrings.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      313 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8835 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/client_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1089 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/validation_result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1110 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/int_16_complex.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      167 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      133 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6609 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3530 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/saver.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      940 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1374 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2476 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_core/version_parsing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5888 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4262 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.964108 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2020 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18332 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/json/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24890 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9857 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.968108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11317 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4935 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21419 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      588 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2533 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.972108 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9165 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15249 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14234 2024-03-26 22:08:51.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.976107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10410 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3129 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4665 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1383 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      944 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      380 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6295 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12704 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.980107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5868 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4308 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1078 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11309 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/mock_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      758 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      550 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      238 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3636 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22122 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10940 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9624 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      534 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4808 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8247 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2319 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2977 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2248 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      725 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      320 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      234 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8265 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3035 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3504 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6874 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/saver.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3582 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      961 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11976 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5167 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7915 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_perf_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      879 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3558 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      404 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7291 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      729 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3671 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.984107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      378 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11298 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1060 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6619 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20270 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26990 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17502 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20282 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8660 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    33221 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      507 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      855 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5798 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    61892 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28471 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5836 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_pidget_mapping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29382 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      232 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13243 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20944 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9984 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_mode_handler.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      279 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      853 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30732 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27106 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    23850 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.988107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      385 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1364 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12100 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_processors.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21128 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_ref_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    33044 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_ref_app_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1066 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10153 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7799 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      252 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2856 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15929 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25864 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7315 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_pidget_mapping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18396 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8375 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6606 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18518 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    33100 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      949 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15561 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3686 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      345 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14721 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22726 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4802 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      181 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11623 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24450 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14019 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.992107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29808 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7432 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6316 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      381 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1176 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1325 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2333 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19663 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17865 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      419 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1115 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13255 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12595 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      239 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      808 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_configs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20369 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7077 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       56 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7408 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/memory.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9290 2024-03-27 08:15:16.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/algo.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14738 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/api.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      312 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/dependency_injection.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4824 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/domain.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7844 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/lookup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      336 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4761 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.996107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      941 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1578 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1759 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      987 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3019 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.000107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      174 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29439 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      317 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2094 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.000107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      598 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3818 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1614 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2234 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2012 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4618 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3195 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_rate_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_tasks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3777 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.000107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      290 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3293 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1330 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1928 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1560 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/visual_policies.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.000107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      360 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2226 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.000107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      590 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6258 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3719 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/perf_calc_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2022 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/range_help_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13690 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/sensor_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17155 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/session_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8434 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/subsweep_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7156 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1358 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/collapsible_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      590 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/goto_resource_tab_button.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4117 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/group_box.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      262 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7950 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/buttons.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      282 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2650 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/load_dialog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2851 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/preview.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1775 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/save_dialog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/set_config_presenter.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3423 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/syntax_highlight.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1424 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/misc_error_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      844 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3845 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/hooks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2055 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/pidget_groups.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29106 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2519 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/tab_pg_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1657 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/two_sensor_ids_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2687 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14431 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4604 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17705 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2979 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/icons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4748 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1994 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1271 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/animation.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5482 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/event_system.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      723 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/_preset_selection.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5180 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/distance_config_input.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4403 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/memory_breakdown_output.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16800 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/power_consumption_vs_rate_output.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14258 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/power_curve_output.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5594 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/presence_config_input.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4014 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/session_config_input.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18599 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9636 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.004107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11165 2024-03-27 08:16:36.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4912 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14127 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4721 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3623 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1807 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84004 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/loader.gif
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   183522 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/new_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/old_gui.png
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:09.952108 acconeer-exptool-7.9.0/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.008107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6060 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3656 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4287 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13021 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_mcumgruart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      148 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_mcumgruart/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14409 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_mcumgruart/_mcumgrflasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      127 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_mcumgruart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1078 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.012107 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6663 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9146 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9444 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/mpl_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      206 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1411 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/api.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11251 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/builtin_persistors.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11966 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/core.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13233 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/optimizing_persistors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3536 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/opser/registry_persistor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3917 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/pg_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/setup_group.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2952 2024-03-26 22:08:51.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       96 2024-03-26 22:08:51.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      329 2024-03-26 22:08:51.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/linux.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1211 2024-03-26 22:08:51.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/ubuntu_22_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13147 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10709 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30156 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      566 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2024-03-27 13:09:09.000000 acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/check_changelog.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13869 2024-03-26 22:08:50.000000 acconeer-exptool-7.9.0/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/check_permissions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4237 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2073 2024-03-25 16:02:38.000000 acconeer-exptool-7.9.0/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 13:09:10.016107 acconeer-exptool-7.9.0/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31174 2024-03-27 12:59:59.000000 acconeer-exptool-7.9.0/utils/convert_h5.py
```

### Comparing `acconeer-exptool-7.8.3/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/CHANGELOG.md` & `acconeer-exptool-7.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## v7.9.0
+
+### Added
+Plugin system! You are now able to write your own plugins for
+the new Exploration Tool.
+
+Head over to docs.acconeer.com and navigate to
+
+Exploration Tool > Algorithms > A121 > Adding your own plugin
+
+to get started!
+
 ## v7.8.3
 
 ### Changed
 - Bump SDK version for A111 and A121
 
 ## v7.8.2
```

### Comparing `acconeer-exptool-7.8.3/Jenkinsfile` & `acconeer-exptool-7.9.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/LICENSE.md` & `acconeer-exptool-7.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/PKG-INFO` & `acconeer-exptool-7.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.8.3
+Version: 7.9.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.8.3/README.md` & `acconeer-exptool-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/docker/Dockerfile` & `acconeer-exptool-7.9.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/dodo.py` & `acconeer-exptool-7.9.0/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/basic.py` & `acconeer-exptool-7.9.0/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/basic_continuous.py` & `acconeer-exptool-7.9.0/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/load_record.py` & `acconeer-exptool-7.9.0/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/load_record_h5.m` & `acconeer-exptool-7.9.0/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.9.0/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.9.0/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.9.0/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.9.0/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.9.0/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/services/envelope.py` & `acconeer-exptool-7.9.0/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/services/iq.py` & `acconeer-exptool-7.9.0/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/services/power_bins.py` & `acconeer-exptool-7.9.0/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/services/sparse.py` & `acconeer-exptool-7.9.0/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/utils/ping.py` & `acconeer-exptool-7.9.0/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.9.0/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/bilateration/bilaterator.py` & `acconeer-exptool-7.9.0/examples/a121/algo/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/breathing/breathing.py` & `acconeer-exptool-7.9.0/examples/a121/algo/breathing/breathing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/breathing/breathing_with_gui.py` & `acconeer-exptool-7.9.0/examples/a121/algo/breathing/breathing_with_gui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/distance/detector.py` & `acconeer-exptool-7.9.0/examples/a121/algo/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/distance/post_process_distance_result.py` & `acconeer-exptool-7.9.0/examples/a121/algo/distance/post_process_distance_result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/distance/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/hand_motion/hand_motion_example_app.py` & `acconeer-exptool-7.9.0/examples/a121/algo/hand_motion/hand_motion_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/obstacle/detector.py` & `acconeer-exptool-7.9.0/examples/a121/algo/obstacle/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.9.0/examples/a121/algo/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/presence/detector.py` & `acconeer-exptool-7.9.0/examples/a121/algo/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/presence/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/smart_presence/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/smart_presence/ref_app.py` & `acconeer-exptool-7.9.0/examples/a121/algo/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/speed/detector.py` & `acconeer-exptool-7.9.0/examples/a121/algo/speed/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/speed/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/speed/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/surface_velocity/example_app.py` & `acconeer-exptool-7.9.0/examples/a121/algo/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/surface_velocity/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/tank_level/tank_level.py` & `acconeer-exptool-7.9.0/examples/a121/algo/tank_level/tank_level.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/tank_level/tank_level_with_gui.py` & `acconeer-exptool-7.9.0/examples/a121/algo/tank_level/tank_level_with_gui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/touchless_button/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/vibration/vibration.py` & `acconeer-exptool-7.9.0/examples/a121/algo/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/algo/waste_level/processor.py` & `acconeer-exptool-7.9.0/examples/a121/algo/waste_level/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/basic.py` & `acconeer-exptool-7.9.0/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/extended_config.py` & `acconeer-exptool-7.9.0/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/load_record.py` & `acconeer-exptool-7.9.0/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/load_record_h5.m` & `acconeer-exptool-7.9.0/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/plot.py` & `acconeer-exptool-7.9.0/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/post_process_sparse_iq.py` & `acconeer-exptool-7.9.0/examples/a121/post_process_sparse_iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.9.0/examples/a121/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.9.0/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.9.0/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/stress.py` & `acconeer-exptool-7.9.0/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/examples/a121/subsweeps.py` & `acconeer-exptool-7.9.0/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/gui/main.py` & `acconeer-exptool-7.9.0/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/noxfile.py` & `acconeer-exptool-7.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/portable/make.py` & `acconeer-exptool-7.9.0/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/portable/package/README.txt` & `acconeer-exptool-7.9.0/portable/package/README.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/portable/package/tools/update.py` & `acconeer-exptool-7.9.0/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/pyproject.toml` & `acconeer-exptool-7.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/setup.cfg` & `acconeer-exptool-7.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/attrs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/attrs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/descriptors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/descriptors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/class_creation/enum.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/class_creation/enum.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/comm_devices.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/comm_devices.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/log_message.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/message.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/messages/system_info_response.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/communication_protocol/protocol.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/communication_protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/buffered_link.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/buffered_link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/helpers.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/helpers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/null_link.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/null_link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/serial_link.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/serial_link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/socket_link.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/socket_link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/links/usb_link.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/links/usb_link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/message_stream.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/message_stream.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/communication/unwrap_ticks.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/communication/unwrap_ticks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/docstrings.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/docstrings.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/client_info.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/entities/validation_result.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/entities/validation_result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/int_16_complex.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/int_16_complex.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/recorder.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/saver.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/saver.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_record/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/h5_session_schema.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/h5_session_schema.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/recording/recorder.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/recording/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_core/version_parsing.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_core/version_parsing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/mock_client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/mock_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/communication/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/record.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/record_io.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/recorder.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/h5_record/saver.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/h5_record/saver.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/im_record/im_record.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/recording/recorder.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/recording/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_ref_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,22 +1593,22 @@
 
     context_group = algo_group.create_group("context")
     context.to_h5(context_group)
 
 
 def _load_algo_data(
     algo_group: h5py.Group,
-) -> Tuple[int, DetectorConfig, DetectorContext]:
-    sensor_id = algo_group["sensor_ids"][()]
+) -> Tuple[list[int], DetectorConfig, DetectorContext]:
+    sensor_ids = algo_group["sensor_ids"][()].tolist()
     config = DetectorConfig.from_json(algo_group["detector_config"][()])
 
     context_group = algo_group["context"]
     context = DetectorContext.from_h5(context_group)
 
-    return sensor_id, config, context
+    return sensor_ids, config, context
 
 
 def _get_group_items(group: h5py.Group) -> list[npt.NDArray[Any]]:
     group_items = []
 
     i = 0
     while True:
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_pidget_mapping.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_pidget_mapping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_example_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_example_app_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_example_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/hand_motion/_mode_handler.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/hand_motion/_mode_handler.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_detector.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_detector_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/obstacle/_processors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/obstacle/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_processors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_ref_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/parking/_ref_app_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/parking/_ref_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_pidget_mapping.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_pidget_mapping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_detector.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/speed/_processors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/speed/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_configs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/algo/waste_level/_processor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/algo/waste_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/memory.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/memory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/algo.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/algo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/api.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/api.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/domain.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/domain.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/a121/model/power/lookup.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/a121/model/power/lookup.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2022-2024
 # All rights reserved
 
 from ._enums import (
     ConnectionInterface,
     ConnectionState,
     PluginFamily,
     PluginGeneration,
@@ -17,14 +17,15 @@
     BackendLogger,
     BackendPlugin,
     GeneralMessage,
     Message,
     PluginStateMessage,
     is_task,
 )
+from .plugin_loader import register_plugin
 from .pluginbase import (
     PgPlotPlugin,
     PlotPluginBase,
     PluginPresetBase,
     PluginSpecBase,
     ViewPluginBase,
     visual_policies,
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2022-2024
 # All rights reserved
 
 from enum import Enum, auto
 
 
 class ConnectionState(Enum):
     DISCONNECTED = auto()
@@ -62,12 +62,13 @@
 
 
 class PluginFamily(Enum):
     SERVICE = "Services"
     DETECTOR = "Detectors"
     REF_APP = "Reference apps"
     EXAMPLE_APP = "Example apps"
+    EXTERNAL_PLUGIN = "External Plugins"
 
 
 class PluginGeneration(Enum):
     A111 = "a111"
     A121 = "a121"
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2022-2024
 # All rights reserved
 
 import ctypes
 import importlib.resources
 import sys
 import typing as t
 
@@ -15,15 +15,15 @@
 
 from acconeer.exptool.app import resources
 from acconeer.exptool.utils import config_logging
 
 from ._argument_parser import ExptoolArgumentParser
 from .app_model import AppModel
 from .backend import Backend
-from .plugin_loader import load_default_plugins
+from .plugin_loader import import_and_register_plugin_module, load_plugins
 from .storage import remove_config_dir, remove_temp_dir
 from .ui import AppModelViewer, MainWindow
 
 
 def main() -> None:
     parser = ExptoolArgumentParser()
     args = parser.parse_args()
@@ -44,18 +44,22 @@
 
     # The cast necessitated of a miss in the typing stubs.
     app: QApplication = t.cast(QApplication, QApplication.instance()) or QApplication(sys.argv)
 
     app.setStyleSheet(qdarktheme.load_stylesheet("light"))
     app.setAttribute(QtCore.Qt.ApplicationAttribute.AA_UseHighDpiPixmaps)
 
+    if args.plugin_modules is not None:
+        for plugin_module_name in args.plugin_modules:
+            import_and_register_plugin_module(plugin_module_name)
+
     backend = Backend()
     backend.start()
 
-    model = AppModel(backend, load_default_plugins())
+    model = AppModel(backend, load_plugins())
     model.start()
 
     app.aboutToQuit.connect(model.stop)
     app.aboutToQuit.connect(backend.stop)
 
     pg.setConfigOption("background", "w")
     pg.setConfigOption("foreground", "k")
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_rate_calc.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/backend/_tasks.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/backend/_tasks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/pluginbase/visual_policies.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/pluginbase/visual_policies.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/metadata_view.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/metadata_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/perf_calc_view.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/perf_calc_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/range_help_view.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/sensor_config_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/sensor_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/session_config_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/session_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/a121/subsweep_config_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/a121/subsweep_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/attrs_config_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/attrs_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/collapsible_widget.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/data_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/goto_resource_tab_button.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/goto_resource_tab_button.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/group_box.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/group_box.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/buttons.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/buttons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/load_dialog.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/load_dialog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/preview.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/preview.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/save_dialog.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/save_dialog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/set_config_presenter.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/set_config_presenter.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/syntax_highlight.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/json_save_load_buttons/dialogs/syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/misc_error_view.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/__init__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2023
+# Copyright (c) Acconeer AB, 2023-2024
 # All rights reserved
 
 from . import hooks
 from .pidget_groups import CollapsiblePidgetGroup, FlatPidgetGroup, PidgetGroup, WidgetHook
 from .pidgets import (
     WIDGET_WIDTH,
     CheckboxPidget,
@@ -27,8 +27,10 @@
     OptionalPidgetFactory,
     Pidget,
     PidgetComboBox,
     PidgetFactory,
     PidgetHook,
     SensorIdPidget,
     SensorIdPidgetFactory,
+    StrPidget,
+    StrPidgetFactory,
 )
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/hooks.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/hooks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/pidget_groups.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/pidgets/pidgets.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/pidgets/pidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     QCheckBox,
     QComboBox,
     QDoubleSpinBox,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLayout,
+    QLineEdit,
     QSlider,
     QSpinBox,
     QStackedWidget,
     QVBoxLayout,
     QWidget,
 )
 
@@ -171,14 +172,42 @@
         return int(self._spin_box.value())
 
     def __on_changed(self) -> None:
         self.sig_update.emit(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
+class StrPidgetFactory(PidgetFactory):
+    def create(self, parent: QWidget) -> StrPidget:
+        return StrPidget(self, parent)
+
+
+class StrPidget(Pidget):
+    def __init__(self, factory: StrPidgetFactory, parent: QWidget) -> None:
+        super().__init__(factory, parent)
+
+        self._line_edit = QLineEdit(self._body_widget)
+        self._line_edit.setMaximumWidth(WIDGET_WIDTH)
+        self._line_edit.editingFinished.connect(self.__on_changed)
+        self._body_layout.addWidget(self._line_edit)
+
+    def set_data(self, value: Any) -> None:
+        assert isinstance(value, str)
+
+        with QtCore.QSignalBlocker(self):
+            self._line_edit.setText(value)
+
+    def get_data(self) -> str:
+        return str(self._line_edit.text())
+
+    def __on_changed(self) -> None:
+        self.sig_update.emit(self.get_data())
+
+
+@attrs.frozen(kw_only=True, slots=False)
 class FloatPidgetFactory(PidgetFactory):
     limits: Optional[Tuple[Optional[float], Optional[float]]] = None
     suffix: Optional[str] = None
     decimals: int = 1
 
     def create(self, parent: QWidget) -> FloatPidget:
         return FloatPidget(self, parent)
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/tab_pg_widget.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/tab_pg_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/components/two_sensor_ids_editor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/components/two_sensor_ids_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/animation.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/animation.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/event_system.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/event_system.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/_preset_selection.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/_preset_selection.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/distance_config_input.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/distance_config_input.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/memory_breakdown_output.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/memory_breakdown_output.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/power_consumption_vs_rate_output.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/power_consumption_vs_rate_output.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/power_curve_output.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/power_curve_output.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/presence_config_input.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/presence_config_input.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/services/session_config_input.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/services/session_config_input.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/resource_tab/widgets.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/resource_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2022-2024
 # All rights reserved
 
 from __future__ import annotations
 
 import importlib.resources
 import logging
 from enum import Enum
@@ -131,29 +131,37 @@
                 button.clicked.connect(partial(self._on_preset_click, preset.preset_id))
 
     def _on_app_model_update(self, app_model: AppModel) -> None:
         self.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
 
 class PluginSelection(QWidget):
+    PLUGIN_FAMILY_ORDER = [
+        PluginFamily.EXTERNAL_PLUGIN,
+        PluginFamily.SERVICE,
+        PluginFamily.DETECTOR,
+        PluginFamily.REF_APP,
+        PluginFamily.EXAMPLE_APP,
+    ]
+
     def __init__(
         self, app_model: AppModel, plugins: list[PluginSpecBase], parent: QWidget
     ) -> None:
         super().__init__(parent)
 
         self.app_model = app_model
 
         app_model.sig_notify.connect(self._on_app_model_update)
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(11)
 
         group_boxes = {}
-        for family in PluginFamily:
+        for family in self.PLUGIN_FAMILY_ORDER:
             group_box = QGroupBox(self)
             group_box.setTitle(family.value)
             group_box.setHidden(True)
             group_box.setLayout(QVBoxLayout(group_box))
             self.layout().addWidget(group_box)
             group_boxes[family] = group_box
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/new_gui.png` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/new_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/app/resources/old_gui.png` & `acconeer-exptool-7.9.0/src/acconeer/exptool/app/resources/old_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.9.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_mcumgruart/_mcumgrflasher.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_mcumgruart/_mcumgrflasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/opser/api.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/opser/api.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/opser/builtin_persistors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/opser/builtin_persistors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/opser/core.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/opser/core.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/opser/optimizing_persistors.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/opser/optimizing_persistors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/opser/registry_persistor.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/opser/registry_persistor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/setup/platforms/ubuntu_22_04.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/setup/platforms/ubuntu_22_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.9.0/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.8.3
+Version: 7.9.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 examples/a121/algo/tank_level/tank_level.py
 examples/a121/algo/tank_level/tank_level_with_gui.py
 examples/a121/algo/touchless_button/processor.py
 examples/a121/algo/vibration/vibration.py
 examples/a121/algo/waste_level/processor.py
 examples/a121/record_data/barebones.py
 examples/a121/record_data/with_cli.py
+examples/app/new/plugins/my_plugin.py
 gui/main.py
 portable/.gitignore
 portable/make.py
 portable/package/README.txt
 portable/package/cmd_with_path.bat
 portable/package/run_app.bat
 portable/package/update.bat
```

### Comparing `acconeer-exptool-7.8.3/src/acconeer_exptool.egg-info/requires.txt` & `acconeer-exptool-7.9.0/src/acconeer_exptool.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_changelog.py` & `acconeer-exptool-7.9.0/tools/check_changelog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_copyright.py` & `acconeer-exptool-7.9.0/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_line_length.py` & `acconeer-exptool-7.9.0/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_permissions.py` & `acconeer-exptool-7.9.0/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_sdk_mentions.py` & `acconeer-exptool-7.9.0/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/check_whitespace.py` & `acconeer-exptool-7.9.0/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/tools/update_regmap.py` & `acconeer-exptool-7.9.0/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.8.3/utils/convert_h5.py` & `acconeer-exptool-7.9.0/utils/convert_h5.py`

 * *Files identical despite different names*

