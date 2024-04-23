# Comparing `tmp/cellpy-1.0.1b4.tar.gz` & `tmp/cellpy-1.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.1b4.tar", last modified: Wed Feb 28 12:28:53 2024, max compression
+gzip compressed data, was "cellpy-1.0.1b5.tar", last modified: Thu Mar  7 14:24:51 2024, max compression
```

## Comparing `cellpy-1.0.1b4.tar` & `cellpy-1.0.1b5.tar`

### file list

```diff
@@ -1,104 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.602062 cellpy-1.0.1b4/
--rw-rw-rw-   0        0        0      459 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/AUTHORS.md
--rw-rw-rw-   0        0        0     3406 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     5515 2024-02-28 11:17:20.000000 cellpy-1.0.1b4/HISTORY.md
--rw-rw-rw-   0        0        0     1087 2024-02-25 13:53:46.000000 cellpy-1.0.1b4/LICENSE.md
--rw-rw-rw-   0        0        0      521 2024-02-28 11:32:42.000000 cellpy-1.0.1b4/MANIFEST.in
--rw-rw-rw-   0        0        0     9199 2024-02-28 12:28:53.600053 cellpy-1.0.1b4/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2024-02-28 12:27:31.000000 cellpy-1.0.1b4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.411002 cellpy-1.0.1b4/cellpy/
--rw-rw-rw-   0        0        0     1163 2024-02-25 13:53:46.000000 cellpy-1.0.1b4/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2024-02-28 12:28:10.000000 cellpy-1.0.1b4/cellpy/_version.py
--rw-rw-rw-   0        0        0    63696 2024-02-25 13:53:46.000000 cellpy-1.0.1b4/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.430996 cellpy-1.0.1b4/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    29493 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4833 2024-02-27 19:45:44.000000 cellpy-1.0.1b4/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.442999 cellpy-1.0.1b4/cellpy/parameters/
--rw-rw-rw-   0        0        0     3513 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    24966 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.446997 cellpy-1.0.1b4/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24148 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    14964 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    13581 2024-02-28 10:14:22.000000 cellpy-1.0.1b4/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.467000 cellpy-1.0.1b4/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   280560 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    43072 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    23045 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0      495 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/do.py
--rw-rw-rw-   0        0        0    18236 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.506260 cellpy-1.0.1b4/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    50060 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    20270 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21106 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11088 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     9389 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9921 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27792 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    24693 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.521827 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6631 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4080 2024-02-19 09:55:29.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10400 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3798 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.525401 cellpy-1.0.1b4/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.1b4/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22114 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1210 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12894 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    17041 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/instruments/neware_xlsx.py
--rw-rw-rw-   0        0        0    15935 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.532400 cellpy-1.0.1b4/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.1b4/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15822 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1448 2024-02-25 22:55:02.000000 cellpy-1.0.1b4/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26858 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.562270 cellpy-1.0.1b4/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    64651 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.593060 cellpy-1.0.1b4/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19592 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    42419 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14268 2024-02-27 12:28:16.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    28926 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    46212 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3404 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0    10200 2024-02-19 12:52:17.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    75591 2024-02-27 12:28:16.000000 cellpy-1.0.1b4/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.1b4/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    78981 2024-02-27 12:28:16.000000 cellpy-1.0.1b4/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     7653 2024-02-28 10:18:22.000000 cellpy-1.0.1b4/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    46309 2024-02-19 09:55:29.000000 cellpy-1.0.1b4/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    39839 2024-02-27 12:28:16.000000 cellpy-1.0.1b4/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.1b4/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    32747 2024-02-18 15:23:05.000000 cellpy-1.0.1b4/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    23662 2024-02-27 12:34:26.000000 cellpy-1.0.1b4/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1789 2024-02-20 19:45:17.000000 cellpy-1.0.1b4/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2024-02-28 12:28:53.596058 cellpy-1.0.1b4/cellpy.egg-info/
--rw-rw-rw-   0        0        0     9199 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3086 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-28 12:28:52.000000 cellpy-1.0.1b4/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-28 12:28:53.000000 cellpy-1.0.1b4/cellpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2024-02-28 11:28:30.000000 cellpy-1.0.1b4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 12:28:53.602062 cellpy-1.0.1b4/setup.cfg
--rw-rw-rw-   0        0        0     3150 2024-02-28 11:24:48.000000 cellpy-1.0.1b4/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.418329 cellpy-1.0.1b5/
+-rw-rw-rw-   0        0        0      459 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/AUTHORS.md
+-rw-rw-rw-   0        0        0     3406 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     5515 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/HISTORY.md
+-rw-rw-rw-   0        0        0     1087 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/LICENSE.md
+-rw-rw-rw-   0        0        0      521 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9199 2024-03-07 14:24:51.417329 cellpy-1.0.1b5/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/README.md
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.230387 cellpy-1.0.1b5/cellpy/
+-rw-rw-rw-   0        0        0     1163 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-03-07 14:24:27.000000 cellpy-1.0.1b5/cellpy/_version.py
+-rw-rw-rw-   0        0        0    63696 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.250306 cellpy-1.0.1b5/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    29493 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4833 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.260813 cellpy-1.0.1b5/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3513 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    24966 2024-03-07 14:13:43.000000 cellpy-1.0.1b5/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.264812 cellpy-1.0.1b5/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24148 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    14964 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    13581 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.281331 cellpy-1.0.1b5/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   281279 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    46853 2024-03-03 20:04:34.000000 cellpy-1.0.1b5/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    23045 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0      594 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/do.py
+-rw-rw-rw-   0        0        0    18255 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.319329 cellpy-1.0.1b5/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    50060 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    20270 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21106 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11088 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     9389 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9921 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    28999 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    26718 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.332331 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6631 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     4332 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     2020 2024-03-04 20:37:20.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1961 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10627 2024-03-06 09:48:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3798 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.337331 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    49457 2024-03-07 14:23:42.000000 cellpy-1.0.1b5/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1430 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    14739 2024-03-03 15:12:15.000000 cellpy-1.0.1b5/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3519 2024-03-03 20:04:34.000000 cellpy-1.0.1b5/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    17041 2024-02-28 15:42:13.000000 cellpy-1.0.1b5/cellpy/readers/instruments/neware_xlsx.py
+-rw-rw-rw-   0        0        0    15973 2024-02-29 16:05:35.000000 cellpy-1.0.1b5/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.345332 cellpy-1.0.1b5/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    16213 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1448 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    27486 2024-02-29 08:50:08.000000 cellpy-1.0.1b5/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.379329 cellpy-1.0.1b5/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    64651 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.411331 cellpy-1.0.1b5/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19592 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    42419 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14268 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    28926 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    46212 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3404 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0    10200 2024-02-19 12:52:17.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    82304 2024-03-06 15:48:16.000000 cellpy-1.0.1b5/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    78981 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     9123 2024-03-06 08:45:46.000000 cellpy-1.0.1b5/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    46313 2024-03-06 15:48:16.000000 cellpy-1.0.1b5/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    39839 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.1b5/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    32747 2024-02-18 15:23:05.000000 cellpy-1.0.1b5/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    23825 2024-02-29 16:05:35.000000 cellpy-1.0.1b5/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1789 2024-02-28 15:42:14.000000 cellpy-1.0.1b5/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2024-03-07 14:24:51.414330 cellpy-1.0.1b5/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     9199 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3025 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-07 14:24:50.000000 cellpy-1.0.1b5/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-07 14:24:51.000000 cellpy-1.0.1b5/cellpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2024-02-28 15:42:19.000000 cellpy-1.0.1b5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-07 14:24:51.418329 cellpy-1.0.1b5/setup.cfg
+-rw-rw-rw-   0        0        0     3150 2024-02-28 15:42:19.000000 cellpy-1.0.1b5/setup.py
```

### Comparing `cellpy-1.0.1b4/CONTRIBUTING.md` & `cellpy-1.0.1b5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/HISTORY.md` & `cellpy-1.0.1b5/HISTORY.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/LICENSE.md` & `cellpy-1.0.1b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/MANIFEST.in` & `cellpy-1.0.1b5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/PKG-INFO` & `cellpy-1.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.1b4
+Version: 1.0.1b5
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.1b4/README.md` & `cellpy-1.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/__init__.py` & `cellpy-1.0.1b5/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/cli.py` & `cellpy-1.0.1b5/cellpy/cli.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/exceptions.py` & `cellpy-1.0.1b5/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/internals/core.py` & `cellpy-1.0.1b5/cellpy/internals/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/log.py` & `cellpy-1.0.1b5/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/logging.json` & `cellpy-1.0.1b5/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.1b5/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/parameters/internal_settings.py` & `cellpy-1.0.1b5/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.1b5/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/parameters/prmreader.py` & `cellpy-1.0.1b5/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/parameters/prms.py` & `cellpy-1.0.1b5/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/cellreader.py` & `cellpy-1.0.1b5/cellpy/readers/cellreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -759,20 +759,22 @@
             instrument, instrument_file=instrument_file, model=model, **kwargs
         )
 
     @staticmethod
     def _parse_instrument_str(instrument, custom_instrument_splitter="::"):
         if not instrument:
             return None, None
-
-        _instrument = instrument.split(custom_instrument_splitter)
-        if len(_instrument) < 2:
-            return instrument, None
-
-        return _instrument
+        try:
+            _instrument = instrument.split(custom_instrument_splitter)
+            if len(_instrument) < 2:
+                return instrument, None
+            else:
+                return _instrument
+        except AttributeError:
+            return str(instrument), None
 
     @property
     def cycle_mode(self):
         # TODO: v2.0 edit this from scalar to list
         try:
             data = self.data
             m = data.meta_test_dependent.cycle_mode
@@ -1284,15 +1286,16 @@
                 data.raw_data_files_length.extend(new_data.raw_data_files_length)
 
         logging.debug("finished loading the raw-files")
 
         if not prms.Reader.sorted_data:
             logging.debug("sorting data")
             data = self._sort_data(data)
-            data.raw_units = self._set_raw_units()
+
+        data.raw_units = self._set_raw_units()
 
         self.data = data
         self._invent_a_cell_name(self.file_names)  # TODO (v1.0.0): fix me
         return self
 
     def _validate_cell(self, level=0):
         logging.debug("validating test")
@@ -1338,15 +1341,15 @@
 
         Args:
             cellpy_file (OtherPath, str): Full path to the cellpy file.
             parent_level (str, optional): Parent level. Warning! Deprecating this soon!
             return_cls (bool): Return the class.
             accept_old (bool): Accept loading old cellpy-file versions.
                 Instead of raising WrongFileVersion it only issues a warning.
-            selector (): under development
+            selector (str): Experimental feature - select specific ranges of data.
 
         Returns:
             cellpy.CellpyCell class if return_cls is True
         """
 
         # This is what happens:
         # 1) (this is not implemented yet, using only hdf5) chose what file format to load from
@@ -4154,18 +4157,18 @@
         self,
         cycle=None,
         converter=None,
         mode="gravimetric",
         as_frame=True,
         **kwargs,
     ):
-        """Returns discharge-capacity and voltage for the selected cycle.
+        """Returns discharge capacity and voltage for the selected cycle.
 
         Args:
-           cycle (int): cycle number.
+            cycle (int): cycle number.
             converter (float): a multiplication factor that converts the values to
                 specific values (i.e. from Ah to mAh/g). If not provided (or None),
                 the factor is obtained from the self.get_converter_to_specific() method.
             mode (string): 'gravimetric', 'areal' or 'absolute'. Defaults to 'gravimetric'. Used
                 if converter is not provided (or None).
             as_frame (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
             **kwargs (dict): additional keyword arguments sent to the internal _get_cap method.
@@ -4247,19 +4250,21 @@
     ):
         """Gets the capacity for the run.
 
         Args:
             cycle (int, list): cycle number (s).
             cycles (list): list of cycle numbers.
             method (string): how the curves are given
-                "back-and-forth" - standard back and forth; discharge
-                (or charge) reversed from where charge (or discharge) ends.
-                "forth" - discharge (or charge) continues along x-axis.
-                "forth-and-forth" - discharge (or charge) also starts at 0
-                (or shift if not shift=0.0)
+
+                - "back-and-forth" - standard back and forth; discharge
+                  (or charge) reversed from where charge (or discharge) ends.
+                - "forth" - discharge (or charge) continues along x-axis.
+                - "forth-and-forth" - discharge (or charge) also starts at 0
+                  (or shift if not shift=0.0)
+
             insert_nan (bool): insert a np.nan between the charge and discharge curves.
                 Defaults to True for "forth-and-forth", else False
             shift: start-value for charge (or discharge) (typically used when
                 plotting shifted-capacity).
             categorical_column: add a categorical column showing if it is
                 charge or discharge.
             label_cycle_number (bool): add column for cycle number
@@ -5858,15 +5863,18 @@
                 self.headers_normal.data_point_txt,
                 self.headers_normal.datetime_txt,
                 self.headers_normal.discharge_capacity_txt,
                 self.headers_normal.test_time_txt,
             ]
             for cn in column_names:
                 if not columns_to_keep.count(cn):
-                    summary.pop(cn)
+                    try:
+                        summary.pop(cn)
+                    except KeyError:
+                        logging.debug(f"could not pop {cn}")
 
         data.summary = summary
 
         # ----------------- calculated values -----------------------
 
         if self.cycle_mode == "anode":
             logging.info(
@@ -6708,65 +6716,64 @@
     initialize=False,
     debug=False,
     **kwargs,
 ):
     """Create a CellpyCell object
 
     Args:
-        filename (str, os.PathLike, OtherPath, or list of raw-file names): path to file(s) to load
-        instrument (str): instrument to use (defaults to the one in your cellpy config file)
-        instrument_file (str or path): yaml file for custom file type
+        filename (str, os.PathLike, OtherPath, or list of raw-file names): path to file(s) or data-set(s) to load.
+        instrument (str): instrument to use (defaults to the one in your cellpy config file).
+        instrument_file (str or path): yaml file for custom file type.
         cellpy_file (str, os.PathLike, or OtherPath): if both filename (a raw-file) and cellpy_file (a cellpy file)
             is provided, cellpy will try to check if the raw-file is has been updated since the
             creation of the cellpy-file and select this instead of the raw file if cellpy thinks
             they are similar (use with care!).
-        logging_mode (str): "INFO" or "DEBUG"
-        cycle_mode (str): the cycle mode (e.g. "anode" or "full_cell")
-        mass (float): mass of active material (mg) (defaults to mass given in cellpy-file or 1.0)
-        nominal_capacity (float): nominal capacity for the cell (e.g. used for finding C-rates)
+        logging_mode (str): "INFO" or "DEBUG".
+        cycle_mode (str): the cycle mode (e.g. "anode" or "full_cell").
+        mass (float): mass of active material (mg) (defaults to mass given in cellpy-file or 1.0).
+        nominal_capacity (float): nominal capacity for the cell (e.g. used for finding C-rates).
         nom_cap_specifics (str): either "gravimetric" (pr mass), or "areal" (per area).
             ("volumetric" is not fully implemented yet - let us know if you need it).
-        loading (float): loading in units [mass] / [area]
-        area (float): active electrode area (e.g. used for finding the areal capacity)
-        estimate_area (bool): calculate area from loading if given (defaults to True)
+        loading (float): loading in units [mass] / [area].
+        area (float): active electrode area (e.g. used for finding the areal capacity).
+        estimate_area (bool): calculate area from loading if given (defaults to True).
         auto_pick_cellpy_format (bool): decide if it is a cellpy-file based on suffix.
         auto_summary (bool): (re-) create summary.
         units (dict): update cellpy units (used after the file is loaded, e.g. when creating summary).
-        step_kwargs (dict): sent to make_steps
-        summary_kwargs (dict): sent to make_summary
+        step_kwargs (dict): sent to make_steps.
+        summary_kwargs (dict): sent to make_summary.
         selector (dict): passed to load (when loading cellpy-files).
         testing (bool): set to True if testing (will for example prevent making .log files)
         refuse_copying (bool): set to True if you do not want to copy the raw-file before loading.
         initialize (bool): set to True if you want to initialize the CellpyCell object (probably only
-            useful if you want to return a cellpy-file with no data in it)
+            useful if you want to return a cellpy-file with no data in it).
         debug (bool): set to True if you want to debug the loader.
-        **kwargs: sent to the loader
+        **kwargs: sent to the loader.
 
-    Keyword args ("arbin_res"):
-        bad_steps (list of tuples): (c, s) tuples of steps s (in cycle c) to skip loading [arbin_res].
+    Transferred Parameters:
+        bad_steps (list of tuples): (c, s) tuples of steps s (in cycle c) to skip loading ("arbin_res").
         dataset_number (int): the data set number ('Test-ID') to select if you are dealing
-            with arbin files with more than one data-set. Defaults to selecting all data-sets and merging them.
+            with arbin files with more than one data-set. Defaults to selecting all data-sets
+            and merging them ("arbin_res").
         data_points (tuple of ints): load only data from data_point[0] to
-                data_point[1] (use None for infinite).
-        increment_cycle_index (bool): increment the cycle index if merging several datasets (default True).
-
-    Keyword args ("maccor_txt", "neware_txt", "local_instrument", "custom"):
-        sep (str): separator used in the file.
-        skip_rows (int): number of rows to skip in the beginning of the file.
-        header (int): row number of the header.
-        encoding (str): encoding of the file.
-        decimal (str): decimal separator.
-        thousand (str): thousand separator.
-        pre_processor_hook (callable): pre-processors to use.
-
-    Keyword args ("pec_csv"):
-        bad_steps (list): separator used in the file (not implemented yet).
+            data_point[1] (use None for infinite) ("arbin_res").
+        increment_cycle_index (bool): increment the cycle index if merging several datasets (default True)
+        ("arbin_res").
+        sep (str): separator used in the file ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        skip_rows (int): number of rows to skip in the beginning of the file
+            ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        header (int): row number of the header ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        encoding (str): encoding of the file ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        decimal (str): decimal separator ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        thousand (str): thousand separator ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        pre_processor_hook (callable): pre-processors to use ("maccor_txt", "neware_txt", "local_instrument", "custom").
+        bad_steps (list): separator used in the file (not implemented yet) ("pec_csv").
 
     Returns:
-        CellpyCell object (if successful, None if not)
+        CellpyCell object (if successful, None if not).
 
     Examples:
         >>> # read an arbin .res file and create a cellpy object with
         >>> # populated summary and step-table:
         >>> c = cellpy.get("my_data.res", instrument="arbin_res", mass=1.14, area=2.12, loading=1.2, nom_cap=155.2)
         >>>
         >>> # load a cellpy-file:
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/core.py` & `cellpy-1.0.1b5/cellpy/readers/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 It also contains functions that are used by readers and utils.
 And it has the file version definitions.
 """
 
 import abc
 import datetime
 import importlib
+import inspect
 import logging
 import os
 import pathlib
 import pickle
 import sys
 import time
 import warnings
-from typing import Any, Tuple, Dict, List, Union, TypeVar
+from typing import Any, Tuple, Dict, List, Union, TypeVar, Optional
 
 import numpy as np
 import pandas as pd
 import pint
 from scipy import interpolate
 
 from cellpy.exceptions import NullData
@@ -33,14 +34,17 @@
     CellpyMetaIndividualTest,
 )
 
 HEADERS_NORMAL = get_headers_normal()  # TODO @jepe refactor this (not needed)
 HEADERS_SUMMARY = get_headers_summary()  # TODO @jepe refactor this (not needed)
 HEADERS_STEP_TABLE = get_headers_step_table()  # TODO @jepe refactor this (not needed)
 
+LOADERS_NOT_READY_FOR_PROD = [
+    "ext_nda_reader"
+]  # used by the instruments_configurations helper function (move?)
 
 # pint (https://pint.readthedocs.io/en/stable/)
 ureg = pint.UnitRegistry()
 ureg.default_format = "~P"
 Q = ureg.Quantity
 
 
@@ -625,15 +629,25 @@
 
 
 class InstrumentFactory:
     """Factory for instrument loaders."""
 
     def __init__(self):
         self._builders = {}
-        self._kwargs = {}
+        self._kwargs = {}  # stored kwargs for the builders (not used yet)
+
+    def __str__(self):
+        txt = "<InstrumentFactory>\n"
+        for key in self._builders:
+            txt += f"  {key}\n"
+        return txt
+
+    @property
+    def builders(self):
+        return self._builders
 
     def register_builder(self, key: str, builder: Tuple[str, Any], **kwargs) -> None:
         """register an instrument loader module.
 
         Args:
             key: instrument id
             builder: (module_name, module_path)
@@ -641,25 +655,83 @@
                defaults to the builders to allow for using .query).
         """
 
         logging.debug(f"Registering instrument {key}")
         self._builders[key] = builder
         self._kwargs[key] = kwargs
 
+    def unregister_builder(self, key: str) -> None:
+        """unregister an instrument loader module.
+
+        Args:
+            key: instrument id
+        """
+        logging.debug(f"Unregistering instrument {key}")
+        self._builders.pop(key, None)
+        self._kwargs.pop(key, None)
+
+    def get_registered_builders(self):
+        return list(self._builders.keys())
+
+    def get_registered_kwargs(self):
+        return self._kwargs
+
+    def get_registered_builder(self, key):
+        return self._builders.get(key, None)
+
+    def create_all(self, **kwargs):
+        """Create all the instrument loader modules.
+
+        Args:
+            **kwargs: sent to the initializer of the loader class.
+
+        Returns:
+            dict of instances of loader classes.
+        """
+        loaders = {}
+        for key in self._builders:
+            bargs = self._kwargs.get(key, {})
+            bargs.update(kwargs)
+            try:
+                models = {}
+                loader = self.create(key, **bargs)
+                models["default"] = loader
+
+                if available_models := self._get_models(loader):
+                    for model in available_models:
+                        bargs["model"] = model
+                        models[model] = self.create(key, **bargs)
+
+                loaders[key] = models
+            except Exception as e:
+                logging.critical(f"Could not create loader for {key}: {e}")
+        return loaders
+
+    @staticmethod
+    def _get_models(loader):
+
+        try:
+            models = loader.get_params("supported_models")
+            return models
+
+        except Exception as e:
+            logging.debug(f"COULD NOT RETRIEVE supported_models for {loader}: {e}")
+
+        return
+
     def create(self, key: Union[str, None], **kwargs):
         """Create the instrument loader module and initialize the loader class.
 
         Args:
             key: instrument id
             **kwargs: sent to the initializer of the loader class.
 
         Returns:
             instance of loader class.
         """
-
         module_name, module_path = self._builders.get(key, (None, None))
 
         # constant:
         instrument_class = "DataLoader"
 
         if not module_name:
             raise ValueError(key)
@@ -689,17 +761,59 @@
         try:
             value = loader.get_params(variable)
             logging.debug(f"GOT {variable}={value} for {key}")
             return value
 
         except (AttributeError, NotImplementedError, KeyError):
             logging.debug(f"COULD NOT RETRIEVE {variable} for {key}")
+
+        except Exception as e:
+            logging.debug(f"COULD NOT RETRIEVE {variable} for {key}: {e}")
+
         return
 
 
+def instrument_configurations(search_text: str = "") -> Dict[str, Any]:
+    """This function returns a dictionary with information about the available
+    instrument loaders and their models.
+
+    Args:
+        search_text: string to search for in the instrument names.
+
+    Returns:
+        dict: nested dictionary with information about the available instrument loaders and their models.
+
+    """
+    instruments = {}
+    _instruments = find_all_instruments(search_text)
+    factory = InstrumentFactory()
+
+    for instrument, instrument_settings in _instruments.items():
+        if instrument not in LOADERS_NOT_READY_FOR_PROD:
+            factory.register_builder(instrument, instrument_settings)
+
+    loaders = factory.create_all()
+
+    for loader, loader_instance in loaders.items():
+        _info = {"__all__": []}
+        for model, model_instance in loader_instance.items():
+            _info["__all__"].append(model)
+            _model_info = {}
+            if hasattr(model_instance, "config_params"):
+                _model_info["config_params"] = model_instance.config_params
+            else:
+                _model_info["config_params"] = None
+
+            _model_info["doc"] = inspect.getdoc(model_instance)
+
+            _info[model] = _model_info
+        instruments[loader] = _info
+    return instruments
+
+
 def generate_default_factory():
     """This function searches for all available instrument readers
     and registers them in an InstrumentFactory instance.
 
     Returns:
         InstrumentFactory
     """
@@ -707,28 +821,35 @@
     instruments = find_all_instruments()
     for instrument_id, instrument in instruments.items():
         instrument_factory.register_builder(instrument_id, instrument)
     return instrument_factory
 
 
 # TODO: v1.1.0 - implement plugins and local instrument readers
-def find_all_instruments() -> Dict[str, Tuple[str, pathlib.Path]]:
+def find_all_instruments(
+    name_contains: Optional[str] = None,
+) -> Dict[str, Tuple[str, pathlib.Path]]:
     """finds all the supported instruments"""
 
+    if name_contains:
+        glob_txt = f"*{name_contains}*.py"
+    else:
+        glob_txt = "*.py"
+
     import cellpy.readers.instruments as hard_coded_instruments_site
 
     instruments_found = {}
     logging.debug("Searching for modules in base instrument folder:")
 
     hard_coded_instruments_site = pathlib.Path(
         hard_coded_instruments_site.__file__
     ).parent
     modules_in_hard_coded_instruments_site = [
         s
-        for s in hard_coded_instruments_site.glob("*.py")
+        for s in hard_coded_instruments_site.glob(glob_txt)
         if not (
             str(s.name).startswith("_")
             or str(s.name).startswith("dev_")
             or str(s.name).startswith("base")
             or str(s.name).startswith("backup")
             or str(s.name).startswith("registered_loaders")
         )
@@ -1039,15 +1160,15 @@
     header_name="Unit",
     dx=10.0,
     generate_new_x=True,
 ):
     """Do a pandas.DataFrame.group_by and perform interpolation for all groups.
 
     This function is a wrapper around an internal interpolation function in
-    cellpy (that uses scipy.interpolate.interp1d) that combines doing a group-by
+    cellpy (that uses ``scipy.interpolate.interp1d``) that combines doing a group-by
     operation and interpolation.
 
     Args:
         df (pandas.DataFrame): the dataframe to morph.
         x (str): the header for the x-value
             (defaults to normal header step_time_txt) (remark that the default
             group_by column is the cycle column, and each cycle normally
@@ -1065,23 +1186,21 @@
             applies for xy xy xy ... data) (defaults to "Unit").
         dx (float): if generating new x-column and number_of_points is None or
             zero, distance between the generated values.
         generate_new_x (bool): create a new x-column by
             using the x-min and x-max values from the original dataframe where
             the method is set by the number_of_points key-word:
 
-            1)  if number_of_points is not None (default is 100):
+            1)  if number_of_points is not None (default is 100)::
+
+                    new_x = np.linspace(x_max, x_min, number_of_points)
+
+            2)  else::
 
-                ```
-                new_x = np.linspace(x_max, x_min, number_of_points)
-                ```
-            2)  else:
-                ```
-                new_x = np.arange(x_max, x_min, dx)
-                ```
+                    new_x = np.arange(x_max, x_min, dx)
 
 
     Returns: pandas.DataFrame with interpolated x- and y-values. The returned
         dataframe is in tidy (long) format for tidy=True.
 
     """
     # TODO: @jepe - create more tests
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/dbreader.py` & `cellpy-1.0.1b5/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/filefinder.py` & `cellpy-1.0.1b5/cellpy/readers/filefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,25 @@
             not given, all files will be listed.
         glob_txt (str, optional): optional, glob pattern to use when searching for files.
 
     Returns:
         list of str: list of file paths.
 
     Examples:
-        # find all files in your raw-file directory:
+        >>> # find all files in your raw-file directory:
         >>> filelist_1 = filefinder.find_in_raw_file_directory()
 
-        # find all files in your raw-file directory in the subdirectory 'MY-PROJECT':
+        >>> # find all files in your raw-file directory in the subdirectory 'MY-PROJECT':
         >>> filelist_2 = filefinder.find_in_raw_file_directory(raw_file_dir=rawdatadir/"MY-PROJECT")
 
-        # find all files in your raw-file directory with the extension '.raw' in the subdirectory 'MY-PROJECT':
+        >>> # find all files in your raw-file directory with the extension '.raw' in the subdirectory 'MY-PROJECT':
         >>> filelist_3 = filefinder.find_in_raw_file_directory(raw_file_dir=rawdatadir/"MY-PROJECT", extension="raw")
 
-        # find all files in your raw-file directory with the extension '.raw' in the subdirectory 'MY-PROJECT'
-        # that contains the string 'good' in the file name:
+        >>> # find all files in your raw-file directory with the extension '.raw' in the subdirectory 'MY-PROJECT'
+        >>> # that contains the string 'good' in the file name
         >>> filelist_4 = filefinder.find_in_raw_file_directory(
         >>>     raw_file_dir=rawdatadir/"MY-PROJECT",
         >>>     glob_txt="*good*",
         >>>     extension="raw"
         >>>)
 
     Notes:
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/base.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import shutil
 import tempfile
 from abc import ABC
 from typing import List, Union
 
 import pandas as pd
 
+from cellpy.exceptions import WrongFileVersion
 import cellpy.internals.core
 import cellpy.readers.core as core
 from cellpy.parameters.internal_settings import headers_normal
 from cellpy.readers.instruments.configurations import (
     ModelParameters,
     register_configuration_from_module,
 )
@@ -604,20 +605,28 @@
             data.raw.rename(index=str, columns=new_aux_headers, inplace=True)
         return data
 
     def _post_process(self, data):
         # ordered post-processing steps:
         for processor_name in ORDERED_POST_PROCESSING_STEPS:
             if processor_name in self.post_processors:
-                data = self._perform_post_process_step(data, processor_name)
+                try:
+                    data = self._perform_post_process_step(data, processor_name)
+                except Exception as e:
+                    logging.error(f"failed to run {processor_name}: {e}")
+                    raise WrongFileVersion(f"failed to run {processor_name}: {e}")
 
         # non-ordered post-processing steps
         for processor_name in self.post_processors:
             if processor_name not in ORDERED_POST_PROCESSING_STEPS:
-                data = self._perform_post_process_step(data, processor_name)
+                try:
+                    data = self._perform_post_process_step(data, processor_name)
+                except Exception as e:
+                    logging.error(f"failed to run {processor_name}: {e}")
+                    raise WrongFileVersion(f"failed to run {processor_name}: {e}")
         return data
 
     def _perform_post_process_step(self, data, processor_name):
         if self.post_processors[processor_name]:
             if hasattr(post_processors, processor_name):
                 logging.critical(f"running post-processor: {processor_name}")
                 processor = getattr(post_processors, processor_name)
@@ -666,23 +675,17 @@
 
     """
 
     instrument_name = "txt_loader"
     raw_ext = "*"
 
     # override this if needed
-    def parse_loader_parameters(self, **kwargs):
-        sep = kwargs.get("sep", None)
-        if sep is not None:
-            self.sep = sep
-        if self.sep is None:
-            self._auto_formatter()
-
-    # override this if needed
     def parse_formatter_parameters(self, **kwargs):
+        """Parse the formatter parameters."""
+
         logging.debug(f"model: {self.model}")
         if not self.config_params.formatters:
             # Setting defaults if formatter is not loaded
             logging.debug("No formatter given - using default values.")
             self.sep = kwargs.pop("sep", None)
             self.skiprows = kwargs.pop("skiprows", 0)
             self.header = kwargs.pop("header", 0)
@@ -710,15 +713,37 @@
         logging.debug(
             f"Formatters: self.sep={self.sep} self.skiprows={self.skiprows} self.header={self.header} self.encoding={self.encoding}"
         )
         logging.debug(
             f"Formatters (cont.): self.decimal={self.decimal} self.thousands={self.thousands}"
         )
 
+    # TODO: need to implement the possibility to override the configuration parameters from the
+    #  configuration file (config_params), e.g.
+    #  c = cellpy.get(filename, instrument="xxx", model="yyy", raw_units={"voltage": "mV"})
+    # override this if needed
+    def parse_loader_parameters(self, auto_formatter=None, **kwargs):
+        """Parse the loader parameters.
+
+        Args:
+            auto_formatter: if True, the formatter will be set to auto-formatting.
+            **kwargs: keyword arguments.
+        """
+        if auto_formatter:
+            self._auto_formatter()
+        else:
+            # backup option - do auto-formatting if sep is not given
+            sep = kwargs.get("sep", None)
+            if sep is not None:
+                self.sep = sep
+            if self.sep is None:
+                self._auto_formatter()
+
     def _auto_formatter(self):
+        print("auto-formatting")
         separator, first_index = find_delimiter_and_start(
             self.name,
             separators=None,
             checking_length_header=100,
             checking_length_whole=200,
         )
         self.encoding = "UTF-8"  # consider adding a find_encoding function
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/biologics_mpr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-"""This file contains methods for importing Bio-Logic mpr-type files"""
-# This is based on the work by Chris Kerr
-# (https://github.com/chatcannon/galvani/blob/master/galvani/BioLogic.py)
+"""This file contains methods for importing Bio-Logic mpr-type files.
+This is based on the work by Chris Kerr
+(https://github.com/chatcannon/galvani/blob/master/galvani/BioLogic.py)
+
+"""
+
 import datetime
 import dateparser
 import shutil
 import tempfile
 import time
 import warnings
 import logging
@@ -57,18 +60,17 @@
     "Discharge_Capacity",
     "Internal_Resistance",
 ]
 
 
 def _read_modules(fileobj):
     module_magic = fileobj.read(len(b"MODULE"))
+    logging.debug(f"-")
     hdr_bytes = fileobj.read(hdr_dtype.itemsize)
-    hdr = np.fromstring(
-        hdr_bytes, dtype=hdr_dtype, count=1
-    )  # TODO: change to frombuffer
+    hdr = np.fromstring(hdr_bytes, dtype=hdr_dtype, count=1)
     hdr_dict = dict(((n, hdr[n][0]) for n in hdr_dtype.names))
     hdr_dict["offset"] = fileobj.tell()
     hdr_dict["data"] = fileobj.read(hdr_dict["length"])
     fileobj.seek(hdr_dict["offset"] + hdr_dict["length"], SEEK_SET)
     hdr_dict["end"] = fileobj.tell()
     return hdr_dict
 
@@ -102,16 +104,16 @@
 
         Returns: dictionary containing the unit-fractions for current, charge,
         and mass
 
         """
 
         raw_units = dict()
-        raw_units["current"] = "A"
-        raw_units["charge"] = "Ah"
+        raw_units["current"] = "mA"
+        raw_units["charge"] = "mAh"
         raw_units["mass"] = "g"
         raw_units["voltage"] = "V"
         return raw_units
 
     @staticmethod
     def get_raw_limits():
         """Include the settings for how to decide what kind of
@@ -174,16 +176,16 @@
             file_name (str): path to .res file.
             bad_steps (list of tuples): (c, s) tuples of steps s
              (in cycle c) to skip loading.
 
         Returns:
             new test
         """
-        print("bad steps: %s" % bad_steps)
-        print(f"kwargs: {kwargs}")
+        # print("bad steps: %s" % bad_steps)
+        # print(f"kwargs: {kwargs}")
         # self.name = file_name
 
         # creating temporary file and connection
         # self.copy_to_temporary()
         temp_filename = self.temp_file_path
 
         filesize = os.path.getsize(self.temp_file_path)
@@ -211,46 +213,41 @@
 
         # --------- read raw-data (normal-data) -------------------------
         self.logger.debug("reading raw-data")
         self.mpr_data = None
         self.mpr_log = None
         self.mpr_settings = None
 
+        # print(" loading mpr-data ".center(80, "-"))
         self._load_mpr_data(temp_filename, bad_steps)
+
         length_of_test = self.mpr_data.shape[0]
         logging.debug(f"length of test: {length_of_test}")
 
         self.logger.debug("renaming columns")
         self._rename_headers()
         # ---------  stats-data (summary-data) -------------------------
         summary_df = self._create_summary_data()
 
         if summary_df.empty:
             txt = "\nCould not find any summary (stats-file)!"
             txt += " (summary_df.empty = True)"
             txt += "\n -> issue make_summary(use_cellpy_stat_file=False)"
-            warnings.warn(txt)
+            logging.debug(txt)
 
         data.summary = summary_df
         data.raw = self.mpr_data
 
         data.raw_data_files_length.append(length_of_test)
         self._clean_up(temp_filename)
         return data
 
     def _parse_mpr_log_data(self):
         if not self.mpr_log:
-            print("no mpr_log")
-            # self.mpr_log["end_date"] = self.mpr_settings["start_date"]
-            # self.mpr_log["length2"] = 0
-            # self.mpr_log["end2"] = 0
-            # self.mpr_log["offset2"] = 0
-            # self.mpr_log["version2"] = 0
-            # self.mpr_log["data"] = None
-            # self.mpr_log["file"] = None
+            logging.debug("OBS! No mpr_log!")
 
         for value in bl_log_pos_dtype:
             # print(value)
             key, start, end, dtype = value
             if key not in self.mpr_log:
                 continue
             self.mpr_log[key] = np.frombuffer(  # replaced np.fromstring
@@ -272,31 +269,31 @@
         mpr_settings = dict()
         mpr_settings["start_date"] = start_date
         mpr_settings["length"] = settings_mod["length"]
         mpr_settings["end"] = settings_mod["end"]
         mpr_settings["offset"] = settings_mod["offset"]
         mpr_settings["version"] = settings_mod["version"]
         mpr_settings["data"] = settings_mod["data"]
-        # print(f"mpr_settings: {mpr_settings}")
         self.mpr_settings = mpr_settings
-        return None
 
     def _get_flag(self, flag_name):
-        print(f"flag_name: {flag_name}")
+        # TODO: next, find out what where the Ns changes are and Ns
+        #  seems to be a method there to get the cycle number as well
+        # print(f"flag_name: {flag_name}")
         if flag_name in self.flags_dict:
             mask, dtype = self.flags_dict[flag_name]
-            print(f"flag: {flag_name}, mask: {mask}, dtype: {dtype}")
+            # print(f"flag: {flag_name}, mask: {mask}, dtype: {dtype}")
             bin_str = f"{mask:010b}"
-            print(f"bin_str: {bin_str}")
-            print([int(x) for x in bin_str])
-            print(self.mpr_data["flags"])
+            # print(f"bin_str: {bin_str}")
+            # print([int(x) for x in bin_str])
+            # print(self.mpr_data["flags"])
             stuff = np.array(
                 self.mpr_data["flags"] & mask, dtype=dtype
             )  # need to fix this!
-            print(f"stuff: {stuff}")
+            # print(f"stuff: {stuff}")
             return np.array(
                 self.mpr_data["flags"] & mask, dtype=dtype
             )  # need to fix this!
         # elif flag_name in self.flags2_dict:
         #     mask, dtype = self.flags2_dict[flag_name]
         #     return np.array(self.mpr_data['flags2'] & mask, dtype=dtype)
         else:
@@ -306,17 +303,17 @@
     def _load_mpr_data(self, filename, bad_steps):
         if bad_steps is not None:
             warnings.warn("Exluding bad steps is not implemented")
 
         stats_info = os.stat(filename)
         mpr_modules = []
 
-        mpr_log = None
-        mpr_data = None
-        mpr_settings = None
+        # VMP LOG: log module
+        # VMP data: data module
+        # VMP Set: settings module
         with open(filename, mode="rb") as file_obj:
             label = file_obj.read(len(mpr_label))
             self.logger.debug(f"label: {label}")
             counter = 0
             while True:
                 counter += 1
                 new_module = _read_modules(file_obj)
@@ -325,15 +322,15 @@
                 if position >= stats_info.st_size:
                     txt = "-reached end of file"
                     if position == stats_info.st_size:
                         txt += " --exactly at end of file"
                     self.logger.info(txt)
                     break
 
-        # ------------- set -----------------------------------
+        # ------------- settings -------------------------------
         settings_mod = None
         for m in mpr_modules:
             if m["shortname"].strip().decode() == "VMP Set":
                 settings_mod = m
                 break
         if settings_mod is None:
             raise IOError("No settings-module found!")
@@ -350,15 +347,15 @@
 
         data_version = data_module["version"]
         n_data_points = np.fromstring(data_module["data"][:4], dtype="<u4")
         n_data_points = n_data_points[0]
         n_columns = np.fromstring(data_module["data"][4:5], dtype="u1")
         n_columns = n_columns[0]
 
-        # print(f"data (points, cols): {n_data_points}, {n_columns}")
+        logging.debug(f"data (points, cols): {n_data_points}, {n_columns}")
 
         if data_version == 0:
             logging.debug("data version 0")
             column_types = np.fromstring(
                 data_module["data"][5:], dtype="u1", count=n_columns
             )
 
@@ -374,49 +371,38 @@
             remaining_headers = data_module["data"][5 + 2 * n_columns : 405]
 
         else:
             raise IOError("Unrecognised version for data module: %d" % data_version)
 
         whats_left = remaining_headers.strip(b"\x00").decode("utf8")
         if whats_left:
-            self.logger.debug("UPS! you have some columns left")
+            self.logger.debug(" *** UPS! you have some columns left")
             self.logger.debug(whats_left)
 
+        self.cols = []
         dtype_dict = OrderedDict()
         flags_dict = OrderedDict()
-
         for col in column_types:
-            print(f"{col=}")
+            # print(f"col: {col} - {bl_dtypes[col]}")
+            self.cols.append(col)
             if col in bl_flags.keys():
                 flags_dict[bl_flags[col][0]] = bl_flags[col][1]
-
             dtype_dict[bl_dtypes[col][1]] = bl_dtypes[col][0]
-
         self.dtype_dict = dtype_dict
         self.flags_dict = flags_dict
 
         dtype = np.dtype(list(dtype_dict.items()))
-
         p = dtype.itemsize
         if not p == (len(main_data) / n_data_points):
             self.logger.info(
-                "WARNING! You have defined %i bytes, "
-                "but it seems it should be %i" % (p, len(main_data) / n_data_points)
+                f"WARNING! You have defined {p} bytes, but it seems it should be [{len(main_data) / n_data_points}]"
             )
         bulk = main_data
         bulk_data = np.fromstring(bulk, dtype=dtype)
-        print(bulk_data)
         mpr_data = pd.DataFrame(bulk_data)
-        print(mpr_data.head())
-        print(self.flags_dict)
-        print(mpr_data.columns)
-        print(mpr_data["flags"].unique())
-        print(mpr_data["flags2"].unique())
-        logging.debug(mpr_data.columns)
-        self.logger.debug(mpr_data.head())
 
         # ------------- log  -----------------------------------
         log_module = None
         for m in mpr_modules:
             if m["shortname"].strip().decode() == "VMP LOG":
                 log_module = m
 
@@ -433,120 +419,220 @@
             mpr_log["version2"] = log_module["version"]
             mpr_log["data"] = log_module[
                 "data"
             ]  # Not sure if I will ever need it, but just in case....
         self.mpr_log = mpr_log
         self._parse_mpr_log_data()
         self.mpr_data = mpr_data
+        self._unpack_flags()
+
+        # # temporary export while developing
+        # temp = self.mpr_data.copy()
+        #
+        # temp.to_csv(
+        #     r"C:\scripting\cellpy_dev_resources\dev_data\biologic\out\intermediate.csv",
+        #     sep=";",
+        # )
+
+    def _unpack_flags(self):
+
+        df = self.mpr_data
+        flags_dict = self.flags_dict
+
+        for flag_name, (mask, dtype) in flags_dict.items():
+            if flag_name in df.columns:
+                continue
+            df[flag_name] = np.array(df["flags"] & mask, dtype=dtype)
+            if dtype == np.bool_:  # bool, but we prefer 0 and 1
+                df[flag_name] = df[flag_name].astype(int)
+        self.mpr_data = df
 
     def _rename_header(self, h_old, h_new):
         try:
             self.mpr_data.rename(
                 columns={h_new: self.cellpy_headers[h_old]}, inplace=True
             )
         except KeyError as e:
-            # warnings.warn(f"KeyError {e}")
             self.logger.info(f"Problem during conversion to cellpy-format ({e})")
 
-    def _generate_cycle_index(self):
+    def _generate_cycle_index(self, cellpy_header_lookup=None, b_header=None):
+        if "half_cycle" in self.mpr_data.columns:
+            self.mpr_data[self.cellpy_headers["cycle_index_txt"]] = (
+                np.floor(self.mpr_data["half_cycle"] + 1) / 2
+            ).astype(int) + 1
+            return
+
+        if "cycleno" in self.mpr_data.columns:
+            self.mpr_data[self.cellpy_headers["cycle_index_txt"]] = (
+                np.floor(self.mpr_data["cycleno"] + 1) / 2
+            ).astype(int) + 1
+            return
+
+        logging.debug("No Ns - must generate from flags")
         flag = "Ns changes"
+        self.mpr_data[self.cellpy_headers["cycle_index_txt"]] = 1
+
         n = self._get_flag(flag)
-        print(f"n: {n}")
         if n is None:
             return
-        self.mpr_data[self.cellpy_headers["cycle_index_txt"]] = 1
+
         ns_changes = self.mpr_data[n].index.values
         for i in ns_changes:
             self.mpr_data.loc[i:, self.cellpy_headers["cycle_index_txt"]] += 1
 
-    def _generate_datetime(self):
-        start_date = self.mpr_settings["start_date"]
-        # TODO: convert to datetime:
+    def _generate_datetime(self, cellpy_header_lookup=None, b_header=None):
+        if b_header is None:
+            b_header = self.cellpy_headers["test_time_txt"]
         start_datetime = self.mpr_log["Start"]
-        cellpy_header_txt = "datetime_txt"
-        date_format = "%Y-%m-%d %H:%M:%S"  # without microseconds
-        self.mpr_data[self.cellpy_headers[cellpy_header_txt]] = [
+        self.mpr_data[self.cellpy_headers[cellpy_header_lookup]] = [
             start_datetime + datetime.timedelta(seconds=n)
-            for n in self.mpr_data["time"].values
+            for n in self.mpr_data[b_header].values
         ]
-        # self.mpr_data[self.cellpy_headers[cellpy_header_txt]]
-        # .start_date.strftime(date_format)
-        # TODO: @jepe - currently storing as datetime object
-        # (while for arbindata it is stored as str)
-
-    def _generate_step_index(self):
-        # TODO: @jepe - check and optionally fix me
-        cellpy_header_txt = "step_index_txt"
-        biologics_header_txt = "flags2"
-        self._rename_header(cellpy_header_txt, biologics_header_txt)
-        self.mpr_data[self.cellpy_headers[cellpy_header_txt]] += 1
-
-    def _generate_step_time(self):
-        k = self.cellpy_headers["step_time_txt"]
-        if k in self.mpr_data.columns:
-            self.mpr_data[self.cellpy_headers["step_time_txt"]] = np.nan
-
-    def _generate_sub_step_time(self):
-        # TODO: @jepe - fix me
-        k = self.cellpy_headers["sub_step_time_txt"]
-        if k in self.mpr_data.columns:
-            self.mpr_data[self.cellpy_headers["sub_step_time_txt"]] = np.nan
 
-    def _generate_capacities(self):
-        cap_col = self.mpr_data.get("QChargeDischarge")
+    def _generate_step_index(self, cellpy_header_lookup=None, b_header=None):
+
+        if b_header in self.mpr_data.columns:
+            self.mpr_data[self.cellpy_headers["step_index_txt"]] = (
+                self.mpr_data[b_header].astype(int) + 1
+            )
+            return
+
+        logging.debug("No Ns - must generate from flags")
+        self.mpr_data[self.cellpy_headers["step_index_txt"]] = 1
+        flag = "Ns changes"
+
+        n = self._get_flag(flag)
+        if n is None:
+            return
+
+        ns_changes = self.mpr_data[n].index.values
+        for i in ns_changes:
+            self.mpr_data.loc[i:, self.cellpy_headers["step_index_txt"]] += 1
+
+    def _generate_step_time(self, cellpy_header_lookup=None, b_header=None):
+
+        self.mpr_data[self.cellpy_headers["step_time_txt"]] = np.nan
+        if b_header is not None:
+            logging.debug("Not implemented yet")
+            return
+
+        try:
+            g = self.mpr_data.groupby(self.cellpy_headers["step_index_txt"])
+            for name, group in g:
+                t = group[self.cellpy_headers["test_time_txt"]].values
+                t = t - t[0]
+                self.mpr_data.loc[group.index, self.cellpy_headers["step_time_txt"]] = t
+
+        except Exception as e:
+            logging.debug(f"could not group by step_index_txt: {e}")
+            return
+
+    def _generate_capacities(self, cellpy_header_lookup=None, b_header=None):
+        if b_header is None:
+            b_header = "QChargeDischarge"
+
+        cap_col = self.mpr_data[b_header]
         if cap_col is None:
             return
-        k = self.cellpy_headers["charge_capacity_txt"]
-        if k in self.mpr_data.columns:
-            self.mpr_data[self.cellpy_headers["discharge_capacity_txt"]] = [
-                0.0 if x < 0 else x for x in cap_col
-            ]
-            self.mpr_data[self.cellpy_headers["charge_capacity_txt"]] = [
-                0.0 if x >= 0 else x for x in cap_col
-            ]
+        self.mpr_data[self.cellpy_headers["discharge_capacity_txt"]] = [
+            0.0 if x < 0 else x for x in cap_col
+        ]
+        self.mpr_data[self.cellpy_headers["charge_capacity_txt"]] = [
+            0.0 if x >= 0 else -x for x in cap_col
+        ]
 
     def _rename_headers(self):
         # should ideally use the info from bl_dtypes, will do that later
 
-        self.mpr_data[self.cellpy_headers["internal_resistance_txt"]] = np.nan
+        protected = [
+            "datetime_txt",
+            "step_time_txt",
+            "step_index_txt",
+            "cycle_index_txt",
+            "step_time_txt",
+            "sub_step_time_txt",
+            "charge_capacity_txt",
+            "discharge_capacity_txt",
+            "data_point_txt",
+            # "internal_resistance_txt",
+        ]
+
+        # self.mpr_data[self.cellpy_headers["internal_resistance_txt"]] = np.nan
         self.mpr_data[self.cellpy_headers["data_point_txt"]] = np.arange(
             1, self.mpr_data.shape[0] + 1, 1
         )
-        self._generate_datetime()
-        self._generate_cycle_index()
-
-        self._generate_step_time()
-        self._generate_sub_step_time()
-        self._generate_step_index()
-        self._generate_capacities()
-
-        # simple renaming of column headers for the rest
-        self._rename_header("frequency_txt", "freq")
-        self._rename_header("voltage_txt", "Ewe")
-        self._rename_header("current_txt", "I")
-        self._rename_header("aci_phase_angle_txt", "phaseZ")
-        self._rename_header("amplitude_txt", "absZ")
-        self._rename_header("ref_voltage_txt", "Ece")
-        self._rename_header("ref_aci_phase_angle_txt", "phaseZce")
-        self._rename_header("test_time_txt", "time")
 
-        self.mpr_data[self.cellpy_headers["sub_step_index_txt"]] = self.mpr_data[
-            self.cellpy_headers["step_index_txt"]
-        ]
+        cycle_index_made = False
+        step_index_made = False
+        sub_step_index_made = False
+        step_time_made = False
+        sub_step_time_made = False
+        capacity_made = False
+        datetime_made = False
+
+        for key in self.cols:
+            cellpy_header_lookup = bl_dtypes[key][-1]
+            b_header = bl_dtypes[key][1]
+
+            if cellpy_header_lookup:
+
+                if cellpy_header_lookup not in protected:
+                    self._rename_header(cellpy_header_lookup, b_header)
+
+                if cellpy_header_lookup == "charge_capacity_txt":
+                    self._generate_capacities(cellpy_header_lookup, b_header)
+                    capacity_made = True
+
+                if cellpy_header_lookup == "datetime_txt":
+                    self._generate_datetime(cellpy_header_lookup, b_header)
+                    datetime_made = True
+
+                if cellpy_header_lookup == "cycle_index_txt":
+                    self._generate_cycle_index(cellpy_header_lookup, b_header)
+                    cycle_index_made = True
+
+                if cellpy_header_lookup == "step_index_txt":
+                    self._generate_step_index(cellpy_header_lookup, b_header)
+                    step_index_made = True
+
+                if cellpy_header_lookup == "step_time_txt":
+                    self._generate_step_time(cellpy_header_lookup, b_header)
+                    step_time_made = True
+
+        if not capacity_made:
+            self._generate_capacities()
+        if not datetime_made:
+            self._generate_datetime("datetime_txt")
+        if not cycle_index_made:
+            self._generate_cycle_index()
+        if not step_index_made:
+            self._generate_step_index()
+
+        if not step_time_made:
+            self._generate_step_time()
+
+        if not sub_step_time_made:
+            self.mpr_data[self.cellpy_headers["sub_step_time_txt"]] = self.mpr_data[
+                self.cellpy_headers["step_time_txt"]
+            ]
+        if not sub_step_index_made:
+            self.mpr_data[self.cellpy_headers["sub_step_index_txt"]] = self.mpr_data[
+                self.cellpy_headers["step_index_txt"]
+            ]
 
     def _create_summary_data(self):
         # Summary data should contain datapoint-number
         # for last point in the cycle. It must also contain
         # capacity
         df_summary = pd.DataFrame()
         mpr_log = self.mpr_log
         mpr_settings = self.mpr_settings
         # TODO: @jepe - finalise making summary of mpr-files
         # after figuring out steps etc
-        warnings.warn(
+        logging.debug(
             "Creating summary data for biologics mpr-files" " is not implemented yet"
         )
         self.logger.info(mpr_settings)
         self.logger.info(mpr_log)
         start_date = mpr_settings["start_date"]
         self.logger.info(start_date)
         return df_summary
@@ -571,91 +657,83 @@
         pass
 
 
 def _main():
     # This is just for testing
     import logging
     import os
+    import pathlib
+    import sys
+
+    import pandas as pd
+
+    import cellpy
+    from cellpy import cellreader, log
+
+    # -------- defining overall path-names etc ----------
+    # galvanostatic with steps (but only one cycle): Bec_03_02_formation_20170314_C02.mpr
+    # with several cycles (at least one) [VSP]: Mel495_GEIS_cycle4_all_temps.mpr
+
+    mpr_file_path = pathlib.Path(r"C:\scripting\cellpy_dev_resources\dev_data\biologic")
+    mpr_file = mpr_file_path / "Bec_03_02_formation_20170314_C02.mpr"
+
+    out_dir = pathlib.Path(r"C:\scripting\cellpy_dev_resources\dev_data\biologic\out")
+
+    print("\n======================mpr-dev===========================")
+    print(f"Test-file: {mpr_file}")
+    log.setup_logging(default_level="DEBUG")
+    instrument = "biologics_mpr"
+
+    c = cellpy.get(mpr_file, instrument=instrument, mass=0.1, area=0.785)
+    c.to_csv(out_dir, sep=";")
+
+
+def _main0():
+    # This is just for testing
+    import logging
+    import os
+    import pathlib
     import sys
 
+    import pandas as pd
+
+    import cellpy
     from cellpy import cellreader, log
 
     # -------- defining overall path-names etc ----------
-    current_file_path = os.path.dirname(os.path.realpath(__file__))
-    # relative_test_data_dir = "../cellpy/data_ex"
-    relative_test_data_dir = "../../../testdata"
-    relative_out_data_dir = "../../../dev_data"
-    test_data_dir = os.path.abspath(
-        os.path.join(current_file_path, relative_test_data_dir)
-    )
-    test_data_dir_out = os.path.abspath(
-        os.path.join(current_file_path, relative_out_data_dir)
-    )
-    test_data_dir_raw = os.path.join(test_data_dir, "data")
-    if not os.path.isdir(test_data_dir_raw):
-        print(f"Could not find {test_data_dir_raw}")
-        sys.exit(-23)
-    if not os.path.isdir(test_data_dir_out):
-        sys.exit(-24)
-
-    if not os.path.isdir(os.path.join(test_data_dir_out, "out")):
-        os.mkdir(os.path.join(test_data_dir_out, "out"))
-    test_data_dir_out = os.path.join(test_data_dir_out, "out")
-
-    test_raw_file = "biol.mpr"
-    test_raw_file_full = os.path.join(test_data_dir_raw, test_raw_file)
-
-    test_data_dir_cellpy = os.path.join(test_data_dir, "hdf5")
-    test_cellpy_file = "geis.h5"
-    test_cellpy_file_tmp = "tmpfile.h5"
-    test_cellpy_file_full = os.path.join(test_data_dir_cellpy, test_cellpy_file)
-    test_cellpy_file_tmp_full = os.path.join(test_data_dir_cellpy, test_cellpy_file_tmp)
+    # galvanostatic with steps (but only one cycle): Bec_03_02_formation_20170314_C02.mpr
+    # with several cycles (at least one) [VSP]: Mel495_GEIS_cycle4_all_temps.mpr
+
+    mpr_file_path = pathlib.Path(r"C:\scripting\cellpy_dev_resources\dev_data\biologic")
+    mpr_file = mpr_file_path / "Mel495_GEIS_cycle4_all_temps.mpr"
+
+    out_dir = pathlib.Path(r"C:\scripting\cellpy_dev_resources\dev_data\biologic\out")
 
-    raw_file_name = test_raw_file_full
     print("\n======================mpr-dev===========================")
-    print(f"Test-file: {raw_file_name}")
+    print(f"Test-file: {mpr_file}")
     log.setup_logging(default_level="DEBUG")
     instrument = "biologics_mpr"
     cellpy_data_instance = cellreader.CellpyCell()
     cellpy_data_instance.set_instrument(instrument=instrument)
     print("starting to load the file")
-    cellpy_data_instance.from_raw(raw_file_name)
+    cellpy_data_instance.from_raw(mpr_file, mass=0.1, area=0.785)
     print("printing cellpy instance:")
-    print(cellpy_data_instance)
+    raw = cellpy_data_instance.data.raw
+    print(raw.head())
+    out_name = f"{mpr_file.stem}_cellpy.csv"
+    raw.to_csv(out_dir / out_name, sep=";")
 
     print("---make step table")
     cellpy_data_instance.make_step_table()
+    steps = cellpy_data_instance.data.steps
+    out_name = f"{mpr_file.stem}_cellpy_steps.csv"
+    steps.to_csv(out_dir / out_name, sep=";")
 
     print("---make summary")
     cellpy_data_instance.make_summary()
-
-    print("---saving to csv")
-    try:
-        temp_dir = tempfile.mkdtemp()
-        cellpy_data_instance.to_csv(datadir=temp_dir)
-        cellpy_data_instance.to_csv(datadir=test_data_dir_out)
-        print("---saving to hdf5")
-        print("NOT YET")
-    finally:
-        shutil.rmtree(temp_dir)
-
-    # dtype = dtype([('flags', 'u1'), ('time/s', '<f8'), ('Ewe/V', '<f4'), ('dQ/mA.h', '<f8'),
-    #        ('I/mA', '<f4'), ('Ece/V', '<f4'), ('(Q-Qo)/mA.h', '<f8'), ('20', '<f8'),
-    #        ('freq/Hz', '<f4'), ('Phase(Z)/deg', '<f4'), ('|Z|/Ohm', '<f4'),
-    #        ('I Range', '<u2'), ('74', '<f8'), ('96', '<f8'), ('98', '<f8'),
-    #        ('99', '<f8'), ('100', '<f8'), ('101', '<f8'), ('123', '<f8'),
-    #        ('124', '<f8'), ('Capacitance charge/µF', '<f8'), ('Capacitance discharge/µF', '<f8'),
-    #        ('Ns', '<u2'), ('430', '<f8'), ('431', '<f8'), ('432', '<f8'), ('433', '<f8'),
-    #        ('Q charge/discharge/mA.h', '<f8'), ('half cycle', '<u4'), ('469', '<f8'),
-    #        ('471', '<f8')])
-    #
-    # flags = OrderedDict(
-    #     [
-    #         ('mode', (3, <class 'numpy.uint8'>)),('ox/red', (4, <class 'numpy.bool_'>)),
-    #         ('error', (8, <class 'numpy.bool_'>)), ('control changes', (16, <class 'numpy.bool_'>)),
-    #         ('Ns changes', (32, <class 'numpy.bool_'>)), ('counter inc.', (128, <class 'numpy.bool_'>))]
-    # )
-    # flags2 = OrderedDict()
+    summary = cellpy_data_instance.data.summary
+    out_name = f"{mpr_file.stem}_cellpy_summary.csv"
+    summary.to_csv(out_dir / out_name, sep=";")
 
 
 if __name__ == "__main__":
     _main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# Works for data from KIT (SIMBA project)
+"""Configuration for tab-delimited Maccor txt files with 12 comment rows (used by KIT in the SIMBA project)."""
 
-file_info = {"raw_extension": "txt"}
+# currently skips the comment rows instead of parsing them (change this by modifying the formatters
+# and add preprocessing step for parsing them)
 
 unit_labels = {
     "resistance": "Ohms",
     "time": "s",
     "current": "A",
     "voltage": "V",
     "power": "W",
     "capacity": "Ah",
     "energy": "Wh",
     "temperature": "C",
 }
 
+file_info = {"raw_extension": "txt"}
+
 normal_headers_renaming_dict = {
     "data_point_txt": "Rec",
     "cycle_index_txt": "Cycle C",
     "step_index_txt": "Step",
     "test_time_txt": "TestTime",
     "step_time_txt": "StepTime",
     "charge_capacity_txt": "Cap. [Ah]",
@@ -63,9 +66,10 @@
 
 post_processors = {
     "split_capacity": True,
     "split_current": True,
     "set_index": True,
     "rename_headers": True,
     "remove_last_if_bad": True,
+    "set_cycle_number_not_zero": True,
     "convert_date_time_to_datetime": True,
 }
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# not updated yet
+"""Configuration for tab-delimited Maccor txt files with three comment rows (used by UBham in the SIMBA project)."""
+
+# currently skips the comment rows instead of parsing them (change this by modifying the formatters
+# and add preprocessing step for parsing them)
+
 unit_labels = {
     "resistance": "Ohms",
     # not observed yet:
     "time": "s",
     "current": "A",
     "voltage": "V",
     "power": "W",
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,78 @@
-# Works for data from WMG and UBham (SIMBA project)
+"""Configuration for tab-delimited Maccor txt files with two comment rows (used by WMG in the SIMBA project)."""
 
+# currently skips the comment rows instead of parsing them (change this by modifying the formatters
+# and add preprocessing step for parsing them)
+
+file_info = {"raw_extension": "txt"}
+
+# not used yet:
 unit_labels = {
     "resistance": "Ohms",
     "time": "s",
-    "current": "Amps",
-    "voltage": "Volts",
-    "power": "Watt-hr",
-    "capacity": "Amp-hr",
-    "energy": "Wh",
+    "current": "mA",
+    "voltage": "mV",
+    "power": "mW",
+    "capacity": "mAh",
+    "energy": "mWh",
     "temperature": "C",
 }
 
-prefixes = {
-    "G": 1000_000_000,
-    "M": 1000_000,
-    "k": 1000.0,
-    "h": 100.0,
-    "d": 10.0,
-    "c": 0.01,
-    "m": 0.001,
-    "micro": 0.000_001,
-    "n": 0.000_000_001,
-}
-
 normal_headers_renaming_dict = {
-    "data_point_txt": f"Rec#",
-    "datetime_txt": f"DPt Time",
-    "test_time_txt": f"TestTime",
-    "step_time_txt": f"StepTime",
-    "cycle_index_txt": f"Cyc#",
-    "step_index_txt": f"Step",
+    "data_point_txt": "Rec#",
+    "cycle_index_txt": "Cyc#",
+    "step_index_txt": "Step",
+    "test_time_txt": "TestTime",
+    "step_time_txt": "StepTime",
+    "charge_capacity_txt": "mAmp-hr",
+    "charge_energy_txt": "mWatt-hr",
+    "current_txt": "mAmps",
+    "voltage_txt": "Volts",
+    "datetime_txt": "DPt Time",
 }
 
-file_info = {"raw_extension": "txt"}
+raw_units = {"current": "mA", "charge": "mAh", "mass": "g", "voltage": "mV"}
 
 states = {
     "column_name": "State",
     "charge_keys": ["C"],
     "discharge_keys": ["D"],
     "rest_keys": ["R"],
 }
 
-raw_units = {"current": "A", "charge": "Ah", "mass": "g", "voltage": "V"}
 
-# raw_limits = {
-#     "current_hard": 0.000_000_000_000_1,
-#     "current_soft": 0.000_01,
-#     "stable_current_hard": 2.0,
-#     "stable_current_soft": 4.0,
-#     "stable_voltage_hard": 2.0,
-#     "stable_voltage_soft": 4.0,
-#     "stable_charge_hard": 0.001,
-#     "stable_charge_soft": 5.0,
-#     "ir_change": 0.00001,
-# }
+raw_limits = {
+    "current_hard": 0.000_000_000_000_1,
+    "current_soft": 0.000_01,
+    "stable_current_hard": 2.0,
+    "stable_current_soft": 4.0,
+    "stable_voltage_hard": 2.0,
+    "stable_voltage_soft": 4.0,
+    "stable_charge_hard": 0.001,
+    "stable_charge_soft": 5.0,
+    "ir_change": 0.00001,
+}
 
 formatters = {
-    "skiprows": 3,  # 12 for other file
+    "skiprows": 2,
     "sep": "\t",
-    "header": 0,  # 0 for other file
+    "header": 0,
     "encoding": "ISO-8859-1",  # options: "ISO-8859-1", "utf-8", "cp1252"
-    "decimal": ".",
-    "thousands": ",",
+    "decimal": ",",
+    "thousands": None,
 }
 
-pre_processors = {}
+pre_processors = {
+    "remove_empty_lines": True,
+}
 
 post_processors = {
-    "get_column_names": True,
     "split_capacity": True,
-    "split_current": False,
+    "split_current": True,
     "set_index": True,
     "rename_headers": True,
-    "remove_last_if_bad": True,
     "set_cycle_number_not_zero": True,
+    "remove_last_if_bad": True,
     "convert_date_time_to_datetime": True,
     "convert_step_time_to_timedelta": True,
     "convert_test_time_to_timedelta": True,
-    "convert_units": True,
-    "select_columns_to_keep": True,
 }
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/custom.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module is used for loading data using the ``instrument="custom"`` method.
 If no ``instrument_file`` is given (either directly or through the use
-of the ``::`` separator), the default instrument file (yaml) will be used."""
+of the ``::`` separator), the default instrument file (yaml) will be used.
+"""
 
 # This module works, but is by no means finished. The module is meant to
 # be developed further allowing for example
 # to provide custom parsers. At the moment, we anticipate that it only should
-# work with txt-files (so the class is called CustomTxtLoader), however, it is
+# work with "simple" files (txt-files, xlsx, ...), however, it is
 # possible to extend the scope to allow for providing parsers that also can read
 # binary files. The future will show.
 
 import logging
 import sys
 from abc import ABC
 from pathlib import Path
@@ -27,15 +28,18 @@
     """Class for loading data from txt files."""
 
     instrument_name = "custom"
     raw_ext = "*"
 
     def __init__(self, instrument_file=None, **kwargs):
         if instrument_file is None:
-            logging.debug("No instrument_file provided - checking default")
+            logging.debug("No instrument_file provided - checking default for one")
+            # currently using the name custom_instrument_definitions_file for this also
+            # consider adding a separate config parameter for the default instrument file
+            # e.g. local_instrument_default_file
             instrument_file = prms.Instruments.custom_instrument_definitions_file
         if not instrument_file:
             raise FileExistsError(
                 "Missing instrument definition file "
                 "(not given and not defined in config)"
             )
         if not Path(instrument_file).is_file():
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/local_instrument.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """This module is used for loading data using the corresponding local
 yaml file with definitions on how the data should be loaded. This loader
-is based on the ``TxtLoader`` and can only be used to load csv-type files"""
+is based on the ``TxtLoader`` and can only be used to load csv-type files.
+As a "short-cut", this loader will be used if you set the ``instrument``
+to the name of the instrument file (with the ``.yml`` extension) e.g.
+``c = cellpy.get(rawfile, instrument="instrumentfile.yml")``.
+The default instrument file is defined in the cellpy configuration file
+(available through ``prms.Instruments.custom_instrument_definitions_file``)."""
 
 from cellpy.readers.instruments.base import TxtLoader
 from cellpy.readers.instruments.configurations import (
     register_local_configuration_from_yaml_file,
 )
 
 
@@ -24,13 +29,10 @@
         super().__init__()
 
     default_model = None
     supported_models = None
 
     def pre_init(self):
         self.auto_register_config = False
-        print("---------------------------")
-        print(f"{self.local_instrument_file}")
-        print("---------------------------")
         self.config_params = register_local_configuration_from_yaml_file(
             self.local_instrument_file
         )
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/maccor_txt.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,26 +10,21 @@
     base_columns_int,
     headers_normal,
 )
 from cellpy.readers.instruments.base import TxtLoader
 
 
 SUPPORTED_MODELS = {
-    "ZERO": "maccor_txt_zero",
+    "ZERO": "maccor_txt_zero",  # needs to be updated (does no postprocessing at the moment)
     "ONE": "maccor_txt_one",
     "TWO": "maccor_txt_two",
     "THREE": "maccor_txt_three",
-    "FOUR": "maccor_txt_four",
-    "WMG_SIMBA": "maccor_txt_three",
-    "KIT_SIMBA": "maccor_txt_four",
-    "KIT_COMMA_SIMBA": "maccor_txt_two",
-    "UBHAM_SIMBA": "maccor_txt_three",
-    "S4000-WMG": "maccor_txt_four",
-    "S4000-KIT": "maccor_txt_four",
-    "S4000-UBHAM": "maccor_txt_three",
+    "S4000-UBHAM": "maccor_txt_one",
+    "S4000-KIT": "maccor_txt_two",
+    "S4000-WMG": "maccor_txt_three",
 }
 
 
 MUST_HAVE_RAW_COLUMNS = [
     headers_normal.test_time_txt,
     headers_normal.step_time_txt,
     headers_normal.current_txt,
@@ -420,11 +415,78 @@
     plt.legend()
     plt.show()
 
     outfile = out / "test_out"
     c.save(outfile)
 
 
+def _fix_bugs_now():
+    import pathlib
+
+    import cellpy
+    import pandas as pd
+    import matplotlib.pyplot as plt
+
+    DATADIR = r"C:\scripting\cellpy_dev_resources\dev_data\simba_Maccor\S4000"
+    FILENAME = "01_UBham_CD_M50_Validation_0deg_01.txt"
+    INSTRUMENT = "maccor_txt"
+    MODEL = "ONE"
+
+    pd.options.display.max_columns = 100
+    datadir = pathlib.Path(DATADIR)
+    name = datadir / FILENAME
+    out = pathlib.Path(r"C:\scripting\trash")
+    print(f"File exists? {name.is_file()}")
+    if not name.is_file():
+        print(f"could not find {name} ")
+        return
+
+    c = cellpy.get(
+        filename=name,
+        instrument=INSTRUMENT,
+        model=MODEL,
+        mass=1.0,
+        auto_summary=False,
+        # auto_formatter=True,  # does not work for UBHAM (finds only two comment rows, but should be three)
+        # post_processors={"another_param": False},  # This parameter will be available in the post-processors
+    )
+    print(f"loaded the file - now lets see what we got")
+    raw = c.data.raw
+    raw.to_clipboard()
+    print(raw.head())
+    c.make_step_table()
+    steps = c.data.steps
+    summary = c.data.summary
+
+    raw.to_csv(out / "raw.csv", sep=";")
+    steps.to_csv(out / "steps.csv", sep=";")
+    summary.to_csv(out / "summary.csv", sep=";")
+
+    fig_1, (ax1, ax2, ax3, ax4) = plt.subplots(
+        4,
+        1,
+        figsize=(6, 10),
+        constrained_layout=True,
+        sharex=True,
+    )
+    raw.plot(x="test_time", y="voltage", ax=ax1, xlabel="")
+    raw.plot(x="test_time", y="current", ax=ax2, xlabel="")
+    raw.plot(
+        x="test_time", y=["charge_capacity", "discharge_capacity"], ax=ax3, xlabel=""
+    )
+    raw.plot(x="test_time", y="cycle_index", ax=ax4)
+    fig_1.suptitle(f"{name.name}", fontsize=16)
+
+    n = c.get_number_of_cycles()
+    print(f"Number of cycles: {n}")
+
+    plt.legend()
+    plt.show()
+
+    outfile = out / "test_out"
+    c.save(outfile)
+
+
 if __name__ == "__main__":
     # check_dev_loader2(model="two")
     # check_loader(number=2, model="two")
-    _check_loader_from_outside_with_get()
+    _fix_bugs_now()
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/neware_txt.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     base_columns_int,
     headers_normal,
 )
 from cellpy.readers.instruments.base import TxtLoader
 
 
 SUPPORTED_MODELS = {
+    "ONE": "neware_txt_zero",
     "UIO": "neware_txt_zero",
 }
 
 
 MUST_HAVE_RAW_COLUMNS = [
     headers_normal.test_time_txt,
     headers_normal.step_time_txt,
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/neware_xlsx.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/neware_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/pec_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         raw_units = dict()
         raw_units["current"] = "A"
         raw_units["charge"] = "Ah"
         raw_units["mass"] = "mg"
         raw_units["voltage"] = "V"
         raw_units["energy"] = "Wh"
         raw_units["time"] = "s"
+        raw_units["capacity"] = "Ah"
 
         return raw_units
 
     @staticmethod
     def _raw_units_for_internal_calculations():
         raw_units = dict()
         raw_units["current"] = 1.0
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/processors/post_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 the ``config_params.post_processor[<name of post processor>]``.
 
 """
 
 import datetime
 import logging
 import sys
+import warnings
 
 import pandas as pd
 import numpy as np
 
 from cellpy.parameters.internal_settings import headers_normal
 from cellpy.parameters.prms import _minimum_columns_to_keep_for_raw_if_exists
 from cellpy.readers.core import Data
@@ -77,15 +78,16 @@
         logging.debug("converting time - not implemented yet")
 
     return data
 
 
 def set_cycle_number_not_zero(data: Data, config_params: ModelParameters) -> Data:
     """Set cycle number to start from 1 instead of 0."""
-    data.raw[headers_normal.cycle_index_txt] += 1
+    if data.raw[headers_normal.cycle_index_txt].min() == 0:
+        data.raw[headers_normal.cycle_index_txt] += 1
     return data
 
 
 def select_columns_to_keep(data: Data, config_params: ModelParameters) -> Data:
     """Select columns to keep in the raw data."""
     config_params.columns_to_keep.extend(
         headers_normal[h] for h in _minimum_columns_to_keep_for_raw_if_exists
@@ -154,15 +156,23 @@
             )
     return data
 
 
 def convert_date_time_to_datetime(data: Data, config_params: ModelParameters) -> Data:
     """Convert date_time column to datetime."""
     hdr_date_time = headers_normal.datetime_txt
-    data.raw[hdr_date_time] = pd.to_datetime(data.raw[hdr_date_time])
+    try:
+        data.raw[hdr_date_time] = pd.to_datetime(data.raw[hdr_date_time])
+    except ValueError as e:
+        warnings.warn(
+            f"Could not convert date_time to datetime. Will try mixed format (slow)."
+        )
+        data.raw[hdr_date_time] = pd.to_datetime(
+            data.raw[hdr_date_time], format="mixed"
+        )
     return data
 
 
 def date_time_from_test_time(data: Data, config_params: ModelParameters) -> Data:
     """Add a date_time column (based on the test_time column)."""
     hdr_date_time = headers_normal.datetime_txt
     hdr_test_time = headers_normal.test_time_txt
@@ -246,14 +256,15 @@
     print(config_params.post_processors["replace"])
 
 
 def rename_headers(data: Data, config_params: ModelParameters) -> Data:
     """Rename headers to the correct Cellpy headers."""
     columns = {}
     renaming_dict = config_params.normal_headers_renaming_dict
+    print(data.raw.columns)
     # ---- special cases ----
     # 1. datetime_txt and test_time_txt same column
     if "datetime_txt" in renaming_dict and "test_time_txt" in renaming_dict:
         datetime_hdr = renaming_dict["datetime_txt"]
         test_time_hdr = renaming_dict["test_time_txt"]
         if datetime_hdr == test_time_hdr:
             logging.debug("both test_time and datetime assigned to same column")
```

### Comparing `cellpy-1.0.1b4/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.1b5/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.1b5/cellpy/readers/sql_dbreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,30 @@
 
 # ------------------- USED BY NEW CELLPY DB --------------------------
 DB_URI = f"sqlite:///cellpy.db"
 hdr_journal = get_headers_journal()
 
 
 class Base(DeclarativeBase):
+    """Base class for the database models."""
+
     pass
 
 
 batch_cell_association_table = Table(
     "batch_cell_association_table",
     Base.metadata,
     Column("batches_pk", ForeignKey("batches.pk"), primary_key=True),
     Column("cells_pk", ForeignKey("cells.pk"), primary_key=True),
 )
 
 
 class Cell(Base):
+    """Model for cell objects in the database."""
+
     __tablename__ = "cells"
     pk: Mapped[int] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column()  # cell_name
     test_date: Mapped[Optional[str]] = mapped_column()
     label: Mapped[Optional[str]] = mapped_column()  # label
     project: Mapped[Optional[str]] = mapped_column()  # project
     cell_group: Mapped[Optional[str]] = mapped_column()  # cell_group
@@ -70,17 +74,17 @@
     area: Mapped[Optional[float]] = mapped_column()  # area
     mass_total: Mapped[Optional[float]] = mapped_column()  # total_material
     loading_active: Mapped[Optional[float]] = mapped_column()  # loading
     nominal_capacity: Mapped[Optional[float]] = mapped_column()  # nom_cap
     comment_slurry: Mapped[Optional[str]] = mapped_column()  # comment_slurry
     comment_cell: Mapped[Optional[str]] = mapped_column()  # comment_cell
     comment_general: Mapped[Optional[str]] = mapped_column()  # comment_general
-    comment_history: Mapped[
-        Optional[str]
-    ] = mapped_column()  # div information from legacy Excel file
+    comment_history: Mapped[Optional[str]] = (
+        mapped_column()
+    )  # div information from legacy Excel file
     selected: Mapped[Optional[bool]] = mapped_column()  # selected
     frozen: Mapped[Optional[bool]] = mapped_column()  # freeze
     argument: Mapped[Optional[str]] = mapped_column()  # argument
     cell_exists: Mapped[Optional[bool]] = mapped_column()  # cell_exists
     active_material_mass_fraction: Mapped[Optional[float]] = mapped_column()
     pasting_thickness: Mapped[Optional[str]] = mapped_column()
     solvent_solid_ratio: Mapped[Optional[str]] = mapped_column()
@@ -119,26 +123,30 @@
         )
 
     def __str__(self) -> str:
         return f"cell: '{self.name}' (#{self.pk})"
 
 
 class RawData(Base):
+    """Model for raw data objects in the database."""
+
     __tablename__ = "raw_data"
     pk: Mapped[int] = mapped_column(primary_key=True)
     cell_pk: Mapped[int] = mapped_column(ForeignKey("cells.pk"))
     cell: Mapped["Cell"] = relationship(back_populates="raw_data")
     is_file: Mapped[bool] = mapped_column()
     name: Mapped[str] = mapped_column()
 
     def __repr__(self) -> str:
         return f"RawData(pk={self.pk!r}, name={self.name!r}, cell={self.cell_pk!r})"
 
 
 class Batch(Base):
+    """Model for batch objects in the database."""
+
     __tablename__ = "batches"
     pk: Mapped[int] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column()
     comment: Mapped[Optional[str]] = mapped_column()
     cells: Mapped[List["Cell"]] = relationship(
         secondary=batch_cell_association_table, back_populates="batches"
     )
@@ -147,14 +155,16 @@
         return f"Batch(pk={self.pk!r}, name={self.name!r}, cells={self.cells!r})"
 
     def __str__(self) -> str:
         return f"batch: '{self.name}' (#{self.pk})"
 
 
 class SQLReader(BaseDbReader):
+    """A custom database reader for the batch utility in cellpy."""
+
     def __init__(self, db_connection: str = None, batch: str = None, **kwargs) -> None:
         """Initialize the SQLReader."""
         self.db_connection = db_connection
         self.batch = batch  # not used - only here for compatibility with BaseDbReader
         self.engine = None
         self.kwargs = kwargs  # not used at the moment
 
@@ -207,15 +217,15 @@
         with Session(self.engine) as session:
             session.add(cell)
 
     def add_batch_object(self, batch: Batch) -> None:
         """Add a batch object to the database.
 
         For this to work, you will have to create a batch object first, then populate it with
-        data (including the cell objects that the batch refers to, see .add_cell_object),
+        data (including the cell objects that the batch refers to, see ``.add_cell_object``),
         and finally add it to the database using this method.
 
         Examples:
             >>> from cellpy.readers import sql_dbreader
             >>> db = sql_dbreader.SQLReader()
             >>> db.open_db("my_db.sqlite")
 
@@ -249,14 +259,24 @@
 
     def from_batch(
         self,
         batch_name: str,
         include_key: bool = False,
         include_individual_arguments: bool = False,
     ) -> dict:
+        """Get a dictionary with the data from a batch for the journal.
+
+        Args:
+            batch_name: name of the batch.
+            include_key: include the key (the cell ids).
+            include_individual_arguments: include the individual arguments.
+
+        Returns:
+            dict: dictionary with the data.
+        """
         pages_dict = defaultdict(list)
         arguments = []
         with Session(self.engine) as session:
             stmt = select(Cell).where(Cell.batches.any(name=batch_name))
             result = session.execute(stmt)
             for cell in result.scalars():
                 pages_dict[hdr_journal["filename"]].append(cell.name)
@@ -591,16 +611,15 @@
             date = datetime.strptime(datestr, strf)
         except ValueError as e:
             logging.debug(e)
             return None
 
         return date
 
-    def extract_date_from_cell_name(self, force=False):
-        ...
+    def extract_date_from_cell_name(self, force=False): ...
 
 
 def _check_import_cells_from_excel_sqlite(cellpy_db_uri, sqlite_path):
     reader = SQLReader()
     reader.create_db(cellpy_db_uri, echo=False)
     reader.load_excel_sqlite(sqlite_path)
     # 2023.04.06 missing in test excel file:
```

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch.py` & `cellpy-1.0.1b5/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.1b5/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/collectors.py` & `cellpy-1.0.1b5/cellpy/utils/collectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         elevated_plotter_arguments=None,
         data_collector_arguments: dict = None,
         plotter_arguments: dict = None,
         experimental: bool = False,
         **kwargs,
     ):
         """Update both the collected data and the plot(s).
+
         Args:
             b (cellpy.utils.Batch): the batch object.
             data_collector (callable): method that collects the data.
             plotter (callable): method that crates the plots.
             collector_name (str): name of collector.
             name (str or bool): name used for auto-generating filenames etc.
             autorun (bool): run collector and plotter immediately if True.
@@ -179,15 +180,17 @@
             backend (str): name of plotting backend to use ("plotly" or "matplotlib").
             elevated_data_collector_arguments (dict): arguments picked up by the child class' initializer.
             elevated_plotter_arguments (dict): arguments picked up by the child class' initializer.
             data_collector_arguments (dict): keyword arguments sent to the data collector.
             plotter_arguments (dict): keyword arguments sent to the plotter.
             update_name (bool): update the name (using automatic name generation) based on new settings.
             **kwargs: set Collector attributes.
+
         """
+
         self.b = b
         self.data_collector = data_collector
         self.plotter = plotter
         self.nick = nick
         self.experimental = experimental
         if backend != "plotly" and not self.experimental:
             print(f"{backend=}")
@@ -348,14 +351,16 @@
         self.sep = kwargs.get("sep", ";")
         self.csv_include_index = kwargs.get("csv_include_index", True)
         self.csv_layout = kwargs.get("csv_layout", "long")
         self.dpi = kwargs.get("dpi", 200)
         self.toolbar = kwargs.get("toolbar", True)
 
     def generate_name(self):
+        """Generate a name for the collection."""
+
         names = ["collector", self.collector_name]
         if self.nick:
             names.insert(0, self.nick)
         name = "_".join(names)
         return name
 
     def render(self):
@@ -382,15 +387,14 @@
 
         if plotter_arguments is not None:
             logging.info(f"Updating elevated arguments")
             elevated_plotter_arguments = {}
             for k, v in plotter_arguments.items():
                 if v is not None:
                     elevated_plotter_arguments[k] = v
-
             self._update_arguments(
                 None, elevated_plotter_arguments, set_as_defaults=True
             )
 
     def _update_arguments(
         self,
         data_collector_arguments: dict = None,
@@ -426,24 +430,27 @@
             print("*** 'plot_type' TRANSLATED TO 'method'")
             self.plotter_arguments["method"] = self.plotter_arguments.pop("plot_type")
 
     def reset_arguments(
         self, data_collector_arguments: dict = None, plotter_arguments: dict = None
     ):
         """Reset the arguments to the defaults.
+
         Args:
             data_collector_arguments (dict): optional additional keyword arguments for the data collector.
             plotter_arguments (dict): optional additional keyword arguments for the plotter.
+
         """
         self._data_collector_arguments = self._default_data_collector_arguments.copy()
         self._plotter_arguments = self._default_plotter_arguments.copy()
         self._update_arguments(data_collector_arguments, plotter_arguments)
 
     def parse_units(self, **kwargs):
         """Look through your cellpy objects and search for units."""
+
         b = self.b
         c_units = []
         r_units = []
         c_unit = None
         r_unit = None
         for c in b:
             cu = c.cellpy_units
@@ -469,21 +476,23 @@
         plotter_arguments: dict = None,
         reset: bool = False,
         update_data: bool = False,
         update_name: bool = False,
         update_plot: bool = True,
     ):
         """Update both the collected data and the plot(s).
+
         Args:
             data_collector_arguments (dict): keyword arguments sent to the data collector.
             plotter_arguments (dict): keyword arguments sent to the plotter.
             reset (bool): reset the arguments first.
             update_data (bool): update the data before updating the plot even if data has been collected before.
             update_name (bool): update the name (using automatic name generation) based on new settings.
             update_plot (bool): update the plot.
+
         """
         if reset:
             self.reset_arguments(data_collector_arguments, plotter_arguments)
         else:
             self._update_arguments(data_collector_arguments, plotter_arguments)
         if update_data or self.data is None:
             try:
@@ -513,26 +522,28 @@
             print("No figure to show!")
             return False
         return True
 
     def show(self, **kwargs):
         """Show the figure.
 
-        Note that show returns the `figure` object and  if the `backend` used
-        does not provide automatic rendering in the editor / running environment you
-        are using, you might have to issue the rendering yourself. For example, if you
-        are using `plotly` and running it as a script in a typical command shell,
-        you will have to issue `.show()` on the returned `figure` object.
+        Notes:
+            The ``show`` method returns the ``figure`` object and  if the ``backend`` used
+            does not provide automatic rendering in the editor / running environment you
+            are using, you might have to issue the rendering yourself. For example, if you
+            are using `plotly` and running it as a script in a typical command shell,
+            you will have to issue ``.show()`` on the returned ``figure`` object.
 
         Args:
             **kwargs: sent to the plotter.
 
         Returns:
             Figure object
         """
+
         if not self._figure_valid():
             return
 
         print(f"figure name: {self.name}")
         if kwargs:
             logging.info(f"updating figure with {kwargs}")
             self._update_arguments(plotter_arguments=kwargs)
@@ -544,14 +555,21 @@
             return self.figure
 
     def preprocess_data_for_csv(self):
         logging.debug(f"the data layout {self.csv_layout} is not supported yet!")
         return self.data
 
     def to_csv(self, serial_number=None):
+        """Save to csv file.
+
+        Args:
+            serial_number (int): serial number to append to the filename.
+
+        """
+
         filename = self._output_path(serial_number)
         filename = filename.with_suffix(".csv")
         if self.csv_layout != "long":
             data = self.preprocess_data_for_csv()
         else:
             data = self.data
 
@@ -559,14 +577,21 @@
             filename,
             sep=self.sep,
             index=self.csv_include_index,
         )
         print(f"saved csv file: {filename}")
 
     def to_hdf5(self, serial_number=None):
+        """Save to hdf5 file.
+
+        Args:
+            serial_number (int): serial number to append to the filename.
+
+        """
+
         filename = self._output_path(serial_number)
         filename = filename.with_suffix(".h5")
         data = self.data
 
         data.to_hdf(filename, key=HDF_KEY, mode="w")
         print(f"saved hdf5 file: {filename}")
 
@@ -582,14 +607,27 @@
         p.terminate()
         if p.exitcode is None:
             print(f"Oops, {p} timeouts! Could not save {filename}")
         if p.exitcode == 0:
             print(f"saved image file: {filename}")
 
     def to_image_files(self, serial_number=None):
+        """Save to image files (png, svg, json).
+
+        Notes:
+            This method requires ``kaleido`` for the plotly backend.
+
+        Notes:
+            Exporting to json is only applicable for the plotly backend.
+
+        Args:
+            serial_number (int): serial number to append to the filename.
+
+        """
+
         if not self._figure_valid():
             return
         filename_pre = self._output_path(serial_number)
         filename_png = filename_pre.with_suffix(".png")
         filename_svg = filename_pre.with_suffix(".svg")
         filename_json = filename_pre.with_suffix(".json")
 
@@ -604,14 +642,21 @@
             print(f"TODO: implement saving {filename_json}")
         else:
             print(f"TODO: implement saving {filename_png}")
             print(f"TODO: implement saving {filename_svg}")
             print(f"TODO: implement saving {filename_json}")
 
     def save(self, serial_number=None):
+        """Save to csv, hdf5 and image files.
+
+        Args:
+            serial_number (int): serial number to append to the filename.
+
+        """
+
         self.to_csv(serial_number=serial_number)
         self.to_hdf5(serial_number=serial_number)
 
         if self._figure_valid():
             self.to_image_files(serial_number=serial_number)
 
     def _output_path(self, serial_number=None):
@@ -654,15 +699,15 @@
         rate_std=None,
         rate_column=None,
         inverse=None,
         inverted: bool = None,
         key_index_bounds=None,
         backend: str = "plotly",
         title: str = None,
-        points: bool = None,
+        markers: bool = None,
         line: bool = None,
         width: int = None,
         height: int = None,
         legend_title: str = None,
         marker_size: int = None,
         cmap=None,
         spread: bool = None,
@@ -670,50 +715,50 @@
         *args,
         **kwargs,
     ):
         """Collects and shows summaries.
 
         Arguments:
             backend (str): what plotting backend to use (currently only 'plotly' is supported)
-
-        Elevated data collector args:
-            max_cycle (int): drop all cycles above this value.
-            rate (float): filter on rate (C-rate)
+            max_cycle (int): drop all cycles above this value (elevated data collector argument).
+            rate (float): filter on rate (C-rate) (elevated data collector argument).
             on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
-            columns (list): selected column(s) (using cellpy attribute name)
-                [defaults to "charge_capacity_gravimetric"]
-            column_names (list): selected column(s) (using exact column name)
+                (elevated data collector argument).
+            columns (list): selected column(s) (using cellpy attribute name). Defaults to "charge_capacity_gravimetric".
+                (elevated data collector argument).
+            column_names (list): selected column(s) (using exact column name) (elevated data collector argument)
             normalize_capacity_on (list): list of cycle numbers that will be used for setting the basis of the
-                normalization (typically the first few cycles after formation)
+                normalization (typically the first few cycles after formation) (elevated data collector argument)
             scale_by (float or str): scale the normalized data with nominal capacity if "nom_cap",
-                or given value (defaults to one).
-            nom_cap (float): nominal capacity of the cell
+                or given value (defaults to one) (elevated data collector argument).
+            nom_cap (float): nominal capacity of the cell (elevated data collector argument)
             normalize_cycles (bool): perform a normalization of the cycle numbers (also called equivalent cycle index)
-            group_it (bool): if True, average pr group.
+                (elevated data collector argument).
+            group_it (bool): if True, average pr group (elevated data collector argument).
             rate_std (float): allow for this inaccuracy when selecting cycles based on rate
-            rate_column (str): name of the column containing the C-rates.
-            inverse (bool): select steps that do not have the given C-rate.
-            inverted (bool): select cycles that do not have the steps filtered by given C-rate.
+                (elevated data collector argument)
+            rate_column (str): name of the column containing the C-rates (elevated data collector argument).
+            inverse (bool): select steps that do not have the given C-rate (elevated data collector argument).
+            inverted (bool): select cycles that do not have the steps filtered by given C-rate
+                (elevated data collector argument).
             key_index_bounds (list): used when creating a common label for the cells in a group
                 (when group_it is set to True) by splitting and combining from key_index_bound[0] to key_index_bound[1].
                 For example, if your cells are called "cell_01_01" and "cell_01_02" and you set
                 key_index_bounds=[0, 2], the common label will be "cell_01". Or if they are called
                 "20230101_cell_01_01_01" and "20230101_cell_01_01_02" and you set key_index_bounds=[1, 3],
-                the common label will be "cell_01_01".
-
-        Elevated plotter args:
-            points (bool): plot points if True
-            line (bool): plot line if True
-            width: width of plot
-            height: height of plot
-            legend_title: title to put over the legend
-            marker_size: size of the markers used
-            cmap: color-map to use
-            spread (bool): plot error-bands instead of error-bars if True
-            fig_title (str): title of the figure
+                the common label will be "cell_01_01" (elevated data collector argument).
+            markers (bool): plot points if True (elevated plotter argument).
+            line (bool): plot line if True (elevated plotter argument).
+            width: width of plot (elevated plotter argument).
+            height: height of plot (elevated plotter argument).
+            legend_title: title to put over the legend (elevated plotter argument).
+            marker_size: size of the markers used (elevated plotter argument).
+            cmap: color-map to use (elevated plotter argument).
+            spread (bool): plot error-bands instead of error-bars if True (elevated plotter argument).
+            fig_title (str): title of the figure (elevated plotter argument).
         """
 
         # TODO: include option for error-bands (spread) (https://plotly.com/python/continuous-error-bars/)
 
         elevated_data_collector_arguments = dict(
             max_cycle=max_cycle,
             rate=rate,
@@ -731,15 +776,15 @@
             inverted=inverted,
             key_index_bounds=key_index_bounds,
         )
 
         elevated_plotter_arguments = {
             "fig_title": fig_title,
             "title": title,
-            "points": points,
+            "markers": markers,
             "line": line,
             "width": width,
             "height": height,
             "legend_title": legend_title,
             "marker_size": marker_size,
             "cmap": cmap,
             "spread": spread,
@@ -861,15 +906,46 @@
         legend_position=None,
         fig_title=None,
         cols=None,
         group_legend_muting=True,
         *args,
         **kwargs,
     ):
-        """Create a collection of ica (dQ/dV) plots."""
+        """Create a collection of ica (dQ/dV) plots.
+
+        Args:
+            b: cellpy batch object
+            plot_type (str): either 'fig_pr_cell' or 'fig_pr_cycle'
+            backend (str): what plotting backend to use (currently only 'plotly' is supported)
+            cycles (list): select these cycles (elevated data collector argument).
+            max_cycle (int): drop all cycles above this value (elevated data collector argument).
+            rate (float): filter on rate (C-rate) (elevated data collector argument).
+            rate_on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge")
+                (elevated data collector argument).
+            rate_std (float): allow for this inaccuracy when selecting cycles based on rate
+                (elevated data collector argument).
+            rate_agg (str): how to aggregate the rate (e.g. "mean", "max", "min", "first", "last")
+                (elevated data collector argument).
+            inverse (bool): select steps that do not have the given C-rate (elevated data collector argument).
+            label_mapper (callable or dict): function (or dict) that changes the cell names
+                (elevated data collector argument).
+                The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
+                Similarly, if it is a function it takes the cell label as input and returns the new label.
+                Remark! No check are performed to ensure that the new cell labels are unique.
+            cycles_to_plot (int): plot points if True (elevated plotter argument).
+            width (float): width of plot (elevated plotter argument).
+            palette (str): color-map to use (elevated plotter argument).
+            legend_position (str): position of the legend (elevated plotter argument).
+            show_legend (bool): set to False if you don't want to show legend (elevated plotter argument).
+            fig_title (str): title (will be put above the figure) (elevated plotter argument).
+            cols (int): number of columns (elevated plotter argument).
+            group_legend_muting (bool): if True, the legend will be interactive (elevated plotter argument).
+
+
+        """
 
         self.plot_type = plot_type
         self._default_plotter_arguments["method"] = plot_type
 
         elevated_data_collector_arguments = dict(
             cycles=cycles,
             max_cycle=max_cycle,
@@ -954,46 +1030,48 @@
         group_legend_muting=True,
         *args,
         **kwargs,
     ):
         """Create a collection of capacity plots.
 
         Args:
-            b:
+            b: cellpy batch object
             plot_type (str): either 'fig_pr_cell' or 'fig_pr_cycle'
             backend (str): what plotting backend to use (currently only 'plotly' is supported)
             collector_type (str): how the curves are given
-                "back-and-forth" - standard back and forth; discharge
-                    (or charge) reversed from where charge (or discharge) ends.
-                "forth" - discharge (or charge) continues along x-axis.
-                "forth-and-forth" - discharge (or charge) also starts at 0
+
+                - "back-and-forth" - standard back and forth; discharge
+                  (or charge) reversed from where charge (or discharge) ends.
+                - "forth" - discharge (or charge) continues along x-axis.
+                - "forth-and-forth" - discharge (or charge) also starts at 0.
+
             data_collector_arguments (dict) - arguments transferred to the plotter
             plotter_arguments (dict) - arguments transferred to the plotter
-
-        Elevated data collector args:
-            cycles (list): select these cycles.
-            max_cycle (int): drop all cycles above this value.
-            rate (float): filter on rate (C-rate)
-            rate_on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
+            cycles (list): select these cycles (elevated data collector argument).
+            max_cycle (int): drop all cycles above this value (elevated data collector argument).
+            rate (float): filter on rate (C-rate) (elevated data collector argument).
+            rate_on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge")
+                (elevated data collector argument).
             rate_std (float): allow for this inaccuracy when selecting cycles based on rate
+                (elevated data collector argument).
             rate_agg (str): how to aggregate the rate (e.g. "mean", "max", "min", "first", "last")
-            inverse (bool): select steps that do not have the given C-rate.
-            label_mapper (callable or dict): function (or dict) that changes the cell names.
+                (elevated data collector argument).
+            inverse (bool): select steps that do not have the given C-rate (elevated data collector argument).
+            label_mapper (callable or dict): function (or dict) that changes the cell names
+                (elevated data collector argument).
                 The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
                 Similarly, if it is a function it takes the cell label as input and returns the new label.
                 Remark! No check are performed to ensure that the new cell labels are unique.
-
-        Elevated plotter args:
-            cycles_to_plot (int): plot points if True
-            width (float): width of plot
-            legend_position (str): position of the legend
-            show_legend (bool): set to False if you don't want to show legend
-            fig_title (str): title (will be put above the figure)
-            palette (str): color-map to use
-            cols (int): number of columns
+            cycles_to_plot (int): plot points if True (elevated plotter argument).
+            width (float): width of plot (elevated plotter argument).
+            legend_position (str): position of the legend (elevated plotter argument).
+            show_legend (bool): set to False if you don't want to show legend (elevated plotter argument).
+            fig_title (str): title (will be put above the figure) (elevated plotter argument).
+            palette (str): color-map to use (elevated plotter argument).
+            cols (int): number of columns (elevated plotter argument).
         """
 
         elevated_data_collector_arguments = dict(
             cycles=cycles,
             max_cycle=max_cycle,
             label_mapper=label_mapper,
             rate=rate,
@@ -1061,15 +1139,15 @@
             names.insert(0, self.nick)
 
         name = "_".join(names)
         return name
 
 
 def pick_named_cell(b, label_mapper=None):
-    """generator that picks a cell from the batch object, yields its label and the cell itself.
+    """Generator that picks a cell from the batch object, yields its label and the cell itself.
 
     Args:
         b (cellpy.batch object): your batch object
         label_mapper (callable or dict): function (or dict) that changes the cell names.
             The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
             Similarly, if it is a function it takes the cell label as input and returns the new label.
             Remark! No check are performed to ensure that the new cell labels are unique.
@@ -1129,14 +1207,35 @@
     interpolated=True,
     number_of_points=100,
     max_cycle=50,
     abort_on_missing=False,
     method="back-and-forth",
     label_mapper=None,
 ):
+    """
+    Collects cycles from all the cells in the batch object.
+
+    Args:
+        b: cellpy batch object
+        cycles: list of cycle numbers to collect
+        rate: filter on rate (C-rate)
+        rate_on: only select cycles if based on the rate of this step-type (e.g. on="charge").
+        rate_std: allow for this inaccuracy when selecting cycles based on rate
+        rate_agg: how to aggregate the rate (e.g. "mean", "max", "min", "first", "last")
+        inverse: select steps that do not have the given C-rate.
+        interpolated: if True, interpolate the data
+        number_of_points: number of points to interpolate to
+        max_cycle: drop all cycles above this value
+        abort_on_missing: if True, abort if a cell is empty
+        method: how the voltage curves are given (back-and-forth, forth, forth-and-forth)
+        label_mapper: function (or dict) that changes the cell names.
+
+    Returns:
+        pd.DataFrame: collected data
+    """
     if cycles is None:
         cycles = list(range(1, max_cycle + 1))
     all_curves = []
     keys = []
     for n, g, sg, c in pick_named_cell(b, label_mapper):
         if rate is not None:
             filtered_cycles = c.get_cycle_numbers(
@@ -1181,14 +1280,37 @@
     max_cycle=50,
     abort_on_missing=False,
     label_direction=True,
     number_of_points=None,
     label_mapper=None,
     **kwargs,
 ):
+    """
+    Collects ica (dQ/dV) curves from all the cells in the batch object.
+
+    Args:
+        b: cellpy batch object
+        cycles: list of cycle numbers to collect
+        rate: filter on rate (C-rate)
+        rate_on: only select cycles if based on the rate of this step-type (e.g. on="charge").
+        rate_std: allow for this inaccuracy when selecting cycles based on rate
+        rate_agg: how to aggregate the rate (e.g. "mean", "max", "min", "first", "last")
+        inverse: select steps that do not have the given C-rate.
+        voltage_resolution: smoothing of the voltage curve
+        number_of_points: number of points to interpolate to
+        max_cycle: drop all cycles above this value
+        abort_on_missing: if True, abort if a cell is empty
+        label_direction: how the voltage curves are given (back-and-forth, forth, forth-and-forth)
+        label_mapper: function (or dict) that changes the cell names.
+        **kwargs: passed on to ica.dqdv
+
+    Returns:
+        pd.DataFrame: collected data
+    """
+
     if cycles is None:
         cycles = list(range(1, max_cycle + 1))
     all_curves = []
     keys = []
     for n, g, sg, c in pick_named_cell(b, label_mapper):
         if rate is not None:
             filtered_cycles = c.get_cycle_numbers(
@@ -1222,30 +1344,35 @@
     return collected_curves
 
 
 # plotter functions (consider moving to plotutils)
 
 
 def remove_markers(trace):
+    """Remove markers from a plotly trace."""
+
     trace.update(marker=None, mode="lines")
     return trace
 
 
 def _hist_eq(trace):
     z = histogram_equalization(trace.z)
     trace.update(z=z)
     return trace
 
 
 def y_axis_replacer(ax, label):
+    """Replace y-axis label in matplotlib plots."""
     ax.update(title_text=label)
     return ax
 
 
 def legend_replacer(trace, df, group_legends=True):
+    """Replace legend labels with cell names in plotly plots."""
+
     name = trace.name
     parts = name.split(",")
     if len(parts) == 2:
         group = int(parts[0])
         subgroup = int(parts[1])
     else:
         print(
@@ -1373,15 +1500,15 @@
     palette_continuous: str = "Viridis",
     palette_range: tuple = None,
     height: float = None,
     width: float = None,
     spread: bool = False,
     **kwargs,
 ) -> Any:
-    """create a plot made up of sequences of data (voltage curves, dQ/dV, etc).
+    """Create a plot made up of sequences of data (voltage curves, dQ/dV, etc).
 
     This method contains the "common" operations done for all the sequence plots,
     currently supporting filtering out the specific cycles, selecting either
     dividing into subplots by cell or by cycle, and creating the (most basic) figure object.
 
     Args:
         collected_curves (pd.DataFrame): collected data in long format.
@@ -1547,19 +1674,19 @@
     if backend == "plotly":
         if method == "fig_pr_cell":
             start, end = 0.0, 1.0
             if palette_range is not None:
                 start, end = palette_range
             unique_cycle_numbers = curves[z].unique()
             number_of_colors = len(unique_cycle_numbers)
-
-            selected_colors = px.colors.sample_colorscale(
-                palette_continuous, number_of_colors, low=start, high=end
-            )
-            plotly_arguments["color_discrete_sequence"] = selected_colors
+            if number_of_colors > 1:
+                selected_colors = px.colors.sample_colorscale(
+                    palette_continuous, number_of_colors, low=start, high=end
+                )
+                plotly_arguments["color_discrete_sequence"] = selected_colors
         elif method == "fig_pr_cycle":
             if palette_discrete is not None:
                 # plotly_arguments["color_discrete_sequence"] = getattr(px.colors.sequential, palette_discrete)
                 logging.debug(
                     f"palette_discrete is not implemented yet ({palette_discrete})"
                 )
 
@@ -2116,18 +2243,16 @@
         method=method,
         cycles=cycles_to_plot,
         **kwargs,
     )
 
 
 def histogram_equalization(image: np.array) -> np.array:
-    """Perform histogram equalization on a numpy array.
-
+    """Perform histogram equalization on a numpy array."""
     # from http://www.janeriksolem.net/histogram-equalization-with-python-and.html
-    """
     number_bins = 256
     scale = 100
     image[np.isnan(image)] = 0.0
     image_histogram, bins = np.histogram(image.flatten(), number_bins, density=True)
     cdf = image_histogram.cumsum()  # cumulative distribution function
     cdf = (scale - 1) * cdf / cdf[-1]  # normalize
     # use linear interpolation of cdf to find new pixel values
```

### Comparing `cellpy-1.0.1b4/cellpy/utils/easyplot.py` & `cellpy-1.0.1b5/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/example_data.py` & `cellpy-1.0.1b5/cellpy/utils/example_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,20 +69,24 @@
     # CV = "cv.h5"
     # EIS = "eis.h5"
     # BUGGY_FILE = "buggy.h5"
     # PLATING = "plating.h5"
     ARBIN = "20160805_test001_45_cc_01.res"
     AUX_MULTI_X = "aux_multi_x.res"
     PEC_CSV = "pec.csv"
-    # CUSTOM = "custom.csv"
-    # CUSTOM_EXCEL = "custom.xlsx"
+    CUSTOM = "custom_data.csv"
+    CUSTOM_EXCEL = "custom_data.xlsx"
     # BIOL_MPR = "biol.mpr"
-    # MACCOR_TXT = "maccor.txt"
-    # NEWARE_CSV = "neware.csv"
+    MACCOR_TXT_TYPE_ONE = "maccor_one.txt"
+    MACCOR_TXT_TYPE_TWO = "maccor_two.txt"
+    MACCOR_TXT_TYPE_THREE = "maccor_three.txt"
+    NEWARE_CSV = "neware_uio.csv"
     # --------------------------------
+    LOCAL_INSTRUMENT = "local_instrument.yml"
+    CUSTOM_INSTRUMENT = "custom_instrument.yml"
     # DB = "cellpy_db.sqlite"
     # SIMPLE_DB = "simple_db.xlsx"
     # STEPS = "steps.csv"
     # STEPS_SHORT = "steps_short.csv"
 
 
 def download_file(url, local_filename):
@@ -230,15 +234,30 @@
 def arbin_multi_file_path() -> Path:
     """Get the path to an example arbin res file"""
     return _download_if_missing(ExampleData.AUX_MULTI_X.value)
 
 
 def maccor_file_path() -> Path:
     """Get the path to an example maccor txt file"""
-    return _download_if_missing(ExampleData.MACCOR_TXT.value)
+    return _download_if_missing(ExampleData.MACCOR_TXT_TYPE_THREE.value)
+
+
+def maccor_file_path_type_one() -> Path:
+    """Get the path to an example maccor txt file"""
+    return _download_if_missing(ExampleData.MACCOR_TXT_TYPE_ONE.value)
+
+
+def maccor_file_path_type_two() -> Path:
+    """Get the path to an example maccor txt file"""
+    return _download_if_missing(ExampleData.MACCOR_TXT_TYPE_TWO.value)
+
+
+def maccor_file_path_type_three() -> Path:
+    """Get the path to an example maccor txt file"""
+    return _download_if_missing(ExampleData.MACCOR_TXT_TYPE_THREE.value)
 
 
 def neware_file_path() -> Path:
     """Get the path to an example neware csv file"""
     return _download_if_missing(ExampleData.NEWARE_CSV.value)
 
 
@@ -248,12 +267,33 @@
 
 
 def biologics_file_path() -> Path:
     """Get the path to an example biologics mpr file"""
     return _download_if_missing(ExampleData.BIOL_MPR.value)
 
 
+def custom_file_path() -> Path:
+    """Get the path to an example custom data csv file"""
+    return _download_if_missing(ExampleData.CUSTOM.value)
+
+
+def custom_xlsx_file_path() -> Path:
+    """Get the path to an example custom data Excel file"""
+    return _download_if_missing(ExampleData.CUSTOM_EXCEL.value)
+
+
+def custom_instrument_path() -> Path:
+    """Get the path to an example custom instrument definition yaml file"""
+    return _download_if_missing(ExampleData.CUSTOM_INSTRUMENT.value)
+
+
+def local_instrument_path() -> Path:
+    """Get the path to an example local-instrument definition yaml file
+    for loading csv-type files"""
+    return _download_if_missing(ExampleData.LOCAL_INSTRUMENT.value)
+
+
 if __name__ == "__main__":
     # This is used for making a new version of the cellpy file
     _a = raw_file()
     print("Saving new version of the cellpy file!")
     _a.save(cellpy_file_path())
```

### Comparing `cellpy-1.0.1b4/cellpy/utils/helpers.py` & `cellpy-1.0.1b5/cellpy/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,15 +934,15 @@
         g = pages.groupby("group")
         # this ensures that order is kept and grouping is correct
         # it is therefore ok to assume from now on that all the cells within a list belongs to the same group
         for gno, b_sub in g:
             cell_names_nest.append(list(b_sub.index))
             group_nest.append(gno)
     else:
-        cell_names_nest.append(list(b.index))
+        cell_names_nest.append(list(pages.index))
         group_nest.append(pages.group.to_list())
 
     default_columns = [hdr_summary["charge_capacity_gravimetric"]]
     hdr_norm_cycle = hdr_summary["normalized_cycle_index"]
 
     if columns is None:
         columns = []
```

### Comparing `cellpy-1.0.1b4/cellpy/utils/ica.py` & `cellpy-1.0.1b5/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.1b5/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy/utils/plotutils.py` & `cellpy-1.0.1b5/cellpy/utils/plotutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,15 @@
     )
 
     x_columns = ([hdr.cycle_index, hdr.data_point, hdr.test_time, hdr.datetime],)
     y_cols = dict(
         voltages=[hdr.end_voltage_charge, hdr.end_voltage_discharge],
         capacities_gravimetric=_capacities_gravimetric,
         capacities_areal=_capacities_areal,
+        capacities=_cap_cols,
         capacities_gravimetric_split_constant_voltage=_capacities_gravimetric_split,
         capacities_areal_split_constant_voltage=_capacities_areal_split,
     )
     return x_columns, y_cols
 
 
 def create_label_dict(c):
@@ -248,18 +249,21 @@
     _cap_gravimetric_label = (
         f"Capacity ({c.cellpy_units.charge}/{c.cellpy_units.specific_gravimetric})"
     )
     _cap_areal_label = (
         f"Capacity ({c.cellpy_units.charge}/{c.cellpy_units.specific_areal})"
     )
 
+    _cap_label = f"Capacity ({c.cellpy_units.charge})"
+
     y_axis_label = {
         "voltages": f"Voltage ({c.cellpy_units.voltage})",
         "capacities_gravimetric": _cap_gravimetric_label,
         "capacities_areal": _cap_areal_label,
+        "capacities": _cap_label,
         "capacities_gravimetric_split_constant_voltage": _cap_gravimetric_label,
         "capacities_areal_split_constant_voltage": _cap_areal_label,
     }
     return x_axis_labels, y_axis_label
 
 
 def summary_plot(
@@ -281,16 +285,16 @@
 
 
     Args:
         c: cellpy object
         x: x-axis column (default: 'cycle_index')
         y: y-axis column or column set. Currently, the following predefined sets exists:
 
-            - "voltages", "capacities_gravimetric", "capacities_areal", "capacities_gravimetric_split_constant_voltage",
-              "capacities_areal_split_constant_voltage"
+            - "voltages", "capacities_gravimetric", "capacities_areal", "capacities",
+              "capacities_gravimetric_split_constant_voltage", "capacities_areal_split_constant_voltage"
 
         height: height of the plot
         markers: use markers
         title: title of the plot
         x_range: limits for x-axis
         y_range: limits for y-axis
         split: split the plot
@@ -642,20 +646,19 @@
     ]
     m_cycle_data = data[cycle_hdr].isin(cycle)
     data = data.loc[m_cycle_data, :]
 
     data[time_hdr] = data[time_hdr] * t_scaler
     data[voltage_hdr] = data[voltage_hdr] * v_scaler
     data[current_hdr] = data[current_hdr] * i_scaler
-
     data = data.merge(
         table,
         left_on=(cycle_hdr, step_number_hdr),
         right_on=(cycle_, step_),
-    )
+    ).sort_values(by=[time_hdr])
 
     fig = go.Figure()
 
     grouped_data = data.groupby(cycle_hdr)
     for cycle_number, group in grouped_data:
         x = group[time_hdr]
         y = group[voltage_hdr]
```

### Comparing `cellpy-1.0.1b4/cellpy/utils/processor.py` & `cellpy-1.0.1b5/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.1b4/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.1b5/cellpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.1b4
+Version: 1.0.1b5
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.1b4/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.1b5/cellpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 cellpy/readers/instruments/ext_nda_reader.py
 cellpy/readers/instruments/local_instrument.py
 cellpy/readers/instruments/maccor_txt.py
 cellpy/readers/instruments/neware_txt.py
 cellpy/readers/instruments/neware_xlsx.py
 cellpy/readers/instruments/pec_csv.py
 cellpy/readers/instruments/configurations/__init__.py
-cellpy/readers/instruments/configurations/maccor_txt_four.py
 cellpy/readers/instruments/configurations/maccor_txt_one.py
 cellpy/readers/instruments/configurations/maccor_txt_three.py
 cellpy/readers/instruments/configurations/maccor_txt_two.py
 cellpy/readers/instruments/configurations/maccor_txt_zero.py
 cellpy/readers/instruments/configurations/neware_txt_zero.py
 cellpy/readers/instruments/loader_specific_modules/__init__.py
 cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
```

### Comparing `cellpy-1.0.1b4/setup.py` & `cellpy-1.0.1b5/setup.py`

 * *Files identical despite different names*

