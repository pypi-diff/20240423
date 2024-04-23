# Comparing `tmp/peracotta-2.3.0.tar.gz` & `tmp/peracotta-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peracotta-2.3.0.tar", last modified: Fri Mar 15 15:05:29 2024, max compression
+gzip compressed data, was "peracotta-2.3.1.tar", last modified: Tue Apr 23 12:33:06 2024, max compression
```

## Comparing `peracotta-2.3.0.tar` & `peracotta-2.3.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.735980 peracotta-2.3.0/
--rw-r--r--   0 basilef   (1000) users      (100)     1066 2024-02-28 15:11:29.000000 peracotta-2.3.0/LICENSE
--rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-03-15 15:05:29.735980 peracotta-2.3.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) users      (100)     7847 2024-02-28 15:11:32.000000 peracotta-2.3.0/README.md
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.734980 peracotta-2.3.0/peracotta.egg-info/
--rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) users      (100)     1614 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) users      (100)        1 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) users      (100)       95 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) users      (100)      174 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) users      (100)       10 2024-03-15 15:05:29.000000 peracotta-2.3.0/peracotta.egg-info/top_level.txt
--rw-r--r--   0 basilef   (1000) users      (100)     1071 2024-03-15 14:46:03.000000 peracotta-2.3.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) users      (100)       38 2024-03-15 15:05:29.735980 peracotta-2.3.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.731979 peracotta-2.3.0/src/
--rw-r--r--   0 basilef   (1000) users      (100)     4259 2024-03-15 14:41:00.000000 peracotta-2.3.0/src/__init__.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.731979 peracotta-2.3.0/src/assets/
--rw-r--r--   0 basilef   (1000) users      (100)     8050 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/Installing.gif
--rw-r--r--   0 basilef   (1000) users      (100)     2651 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/error.ui
--rw-r--r--   0 basilef   (1000) users      (100)    13414 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/interface.ui
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.731979 peracotta-2.3.0/src/assets/themes/
--rw-r--r--   0 basilef   (1000) users      (100)     5952 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/themes/Dark.css
--rw-r--r--   0 basilef   (1000) users      (100)     6478 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/themes/WEEE Open.css
--rw-r--r--   0 basilef   (1000) users      (100)       33 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/themes/default.css
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.732980 peracotta-2.3.0/src/assets/toolbox/
--rw-r--r--   0 basilef   (1000) users      (100)     9745 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/case.png
--rw-r--r--   0 basilef   (1000) users      (100)    14546 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/cpu.png
--rw-r--r--   0 basilef   (1000) users      (100)    16694 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/gpu.png
--rw-r--r--   0 basilef   (1000) users      (100)    20523 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/hdd.png
--rw-r--r--   0 basilef   (1000) users      (100)    13943 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/keyboard.png
--rw-r--r--   0 basilef   (1000) users      (100)     6966 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/monitor.png
--rw-r--r--   0 basilef   (1000) users      (100)    17156 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/motherboard.png
--rw-r--r--   0 basilef   (1000) users      (100)     9567 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/mouse.png
--rw-r--r--   0 basilef   (1000) users      (100)    10348 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/odd.png
--rw-r--r--   0 basilef   (1000) users      (100)    28645 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/psu.png
--rw-r--r--   0 basilef   (1000) users      (100)     8639 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/ram.png
--rw-r--r--   0 basilef   (1000) users      (100)    10601 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/ssd.png
--rw-r--r--   0 basilef   (1000) users      (100)    11950 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/toolbox/wifi-card.png
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.733980 peracotta-2.3.0/src/assets/ui/
--rw-r--r--   0 basilef   (1000) users      (100)     1444 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/ui/light_down_arrow.png
--rw-r--r--   0 basilef   (1000) users      (100)     6790 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/ui/light_split_handle.png
--rw-r--r--   0 basilef   (1000) users      (100)    28552 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/ui/pear_emoji.png
--rw-r--r--   0 basilef   (1000) users      (100)    14674 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/ui/radio_ckd.png
--rw-r--r--   0 basilef   (1000) users      (100)    12489 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/ui/radio_unckd.png
--rw-r--r--   0 basilef   (1000) users      (100)     5226 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/assets/uploadTaralloDialog.ui
--rw-r--r--   0 basilef   (1000) users      (100)    16567 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/commons.py
--rw-r--r--   0 basilef   (1000) users      (100)     2362 2024-03-05 12:25:23.000000 peracotta-2.3.0/src/config.py
--rw-r--r--   0 basilef   (1000) users      (100)      307 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/config.toml
--rw-r--r--   0 basilef   (1000) users      (100)     1223 2024-03-15 15:05:24.000000 peracotta-2.3.0/src/constants.py
--rw-r--r--   0 basilef   (1000) users      (100)    43091 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/features.json
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.734980 peracotta-2.3.0/src/gui/
--rw-r--r--   0 basilef   (1000) users      (100)     3273 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/gui/PeraThread.py
--rw-r--r--   0 basilef   (1000) users      (100)    26699 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/gui/Toolbox.py
--rw-r--r--   0 basilef   (1000) users      (100)      102 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/gui/__init__.py
--rw-r--r--   0 basilef   (1000) users      (100)     1108 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/gui/exception_handler.py
--rw-r--r--   0 basilef   (1000) users      (100)       48 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/gui/exceptions.py
--rw-r--r--   0 basilef   (1000) users      (100)    20845 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/gui/gui.py
--rw-r--r--   0 basilef   (1000) users      (100)     2989 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/gui/prettyprinter.py
--rw-r--r--   0 basilef   (1000) users      (100)     1362 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/gui/widgets.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.734980 peracotta-2.3.0/src/parsers/
--rwxr-xr-x   0 basilef   (1000) users      (100)     5274 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/read_decode_dimms.py
--rw-r--r--   0 basilef   (1000) users      (100)    14087 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/read_dmidecode.py
--rwxr-xr-x   0 basilef   (1000) users      (100)     4008 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/read_lscpu.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    10890 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/read_lspci_and_glxinfo.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    26973 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/read_smartctl.py
--rw-r--r--   0 basilef   (1000) users      (100)     3766 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/parsers/windows_parser.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    12449 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/peracruda.py
--rw-r--r--   0 basilef   (1000) users      (100)      639 2024-03-15 14:49:31.000000 peracotta-2.3.0/src/peralog.py
--rw-r--r--   0 basilef   (1000) users      (100)      337 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/reporter.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-03-15 15:05:29.734980 peracotta-2.3.0/src/scripts/
--rwxr-xr-x   0 basilef   (1000) users      (100)     1628 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/scripts/check_dependencies.sh
--rwxr-xr-x   0 basilef   (1000) users      (100)     1718 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/scripts/generate_files.sh
--rw-r--r--   0 basilef   (1000) users      (100)     2694 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/scripts/get_windows_specs.py
--rwxr-xr-x   0 basilef   (1000) users      (100)      172 2024-02-28 15:11:29.000000 peracotta-2.3.0/src/scripts/install_dependencies_all.sh
--rw-r--r--   0 basilef   (1000) users      (100)     3216 2024-03-15 14:40:38.000000 peracotta-2.3.0/src/tarallo.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/
+-rw-r--r--   0 basilef   (1000) users      (100)     1066 2024-02-28 15:11:29.000000 peracotta-2.3.1/LICENSE
+-rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-04-23 12:33:06.634646 peracotta-2.3.1/PKG-INFO
+-rw-r--r--   0 basilef   (1000) users      (100)     7847 2024-02-28 15:11:32.000000 peracotta-2.3.1/README.md
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/peracotta.egg-info/
+-rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) users      (100)     1614 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) users      (100)        1 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) users      (100)       95 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) users      (100)      174 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) users      (100)       10 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/top_level.txt
+-rw-r--r--   0 basilef   (1000) users      (100)     1071 2024-03-15 15:08:55.000000 peracotta-2.3.1/pyproject.toml
+-rw-r--r--   0 basilef   (1000) users      (100)       38 2024-04-23 12:33:06.634646 peracotta-2.3.1/setup.cfg
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.631646 peracotta-2.3.1/src/
+-rw-r--r--   0 basilef   (1000) users      (100)     4432 2024-03-27 15:00:33.000000 peracotta-2.3.1/src/__init__.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/
+-rw-r--r--   0 basilef   (1000) users      (100)     8050 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/Installing.gif
+-rw-r--r--   0 basilef   (1000) users      (100)     2651 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/error.ui
+-rw-r--r--   0 basilef   (1000) users      (100)    13414 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/interface.ui
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/themes/
+-rw-r--r--   0 basilef   (1000) users      (100)     5952 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/Dark.css
+-rw-r--r--   0 basilef   (1000) users      (100)     6478 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/WEEE Open.css
+-rw-r--r--   0 basilef   (1000) users      (100)       33 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/default.css
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/toolbox/
+-rw-r--r--   0 basilef   (1000) users      (100)     9745 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/case.png
+-rw-r--r--   0 basilef   (1000) users      (100)    14546 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/cpu.png
+-rw-r--r--   0 basilef   (1000) users      (100)    16694 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/gpu.png
+-rw-r--r--   0 basilef   (1000) users      (100)    20523 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/hdd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    13943 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/keyboard.png
+-rw-r--r--   0 basilef   (1000) users      (100)     6966 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/monitor.png
+-rw-r--r--   0 basilef   (1000) users      (100)    17156 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/motherboard.png
+-rw-r--r--   0 basilef   (1000) users      (100)     9567 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/mouse.png
+-rw-r--r--   0 basilef   (1000) users      (100)    10348 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/odd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    28645 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/psu.png
+-rw-r--r--   0 basilef   (1000) users      (100)     8639 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/ram.png
+-rw-r--r--   0 basilef   (1000) users      (100)    10601 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/ssd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    11950 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/wifi-card.png
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/assets/ui/
+-rw-r--r--   0 basilef   (1000) users      (100)     1444 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/light_down_arrow.png
+-rw-r--r--   0 basilef   (1000) users      (100)     6790 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/light_split_handle.png
+-rw-r--r--   0 basilef   (1000) users      (100)    28552 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/pear_emoji.png
+-rw-r--r--   0 basilef   (1000) users      (100)    14674 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/radio_ckd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    12489 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/radio_unckd.png
+-rw-r--r--   0 basilef   (1000) users      (100)     5226 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/uploadTaralloDialog.ui
+-rw-r--r--   0 basilef   (1000) users      (100)    16567 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/commons.py
+-rw-r--r--   0 basilef   (1000) users      (100)     2361 2024-03-27 15:00:33.000000 peracotta-2.3.1/src/config.py
+-rw-r--r--   0 basilef   (1000) users      (100)      307 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/config.toml
+-rw-r--r--   0 basilef   (1000) users      (100)     1360 2024-04-23 12:31:03.000000 peracotta-2.3.1/src/constants.py
+-rw-r--r--   0 basilef   (1000) users      (100)    43091 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/features.json
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/gui/
+-rw-r--r--   0 basilef   (1000) users      (100)     3273 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/PeraThread.py
+-rw-r--r--   0 basilef   (1000) users      (100)    26699 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/Toolbox.py
+-rw-r--r--   0 basilef   (1000) users      (100)      102 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/__init__.py
+-rw-r--r--   0 basilef   (1000) users      (100)     1108 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/exception_handler.py
+-rw-r--r--   0 basilef   (1000) users      (100)       48 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/exceptions.py
+-rw-r--r--   0 basilef   (1000) users      (100)    20818 2024-04-23 12:16:45.000000 peracotta-2.3.1/src/gui/gui.py
+-rw-r--r--   0 basilef   (1000) users      (100)     2989 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/prettyprinter.py
+-rw-r--r--   0 basilef   (1000) users      (100)     1362 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/widgets.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/parsers/
+-rwxr-xr-x   0 basilef   (1000) users      (100)     5274 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_decode_dimms.py
+-rw-r--r--   0 basilef   (1000) users      (100)    14087 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_dmidecode.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)     4008 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_lscpu.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    10890 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_lspci_and_glxinfo.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    26973 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_smartctl.py
+-rw-r--r--   0 basilef   (1000) users      (100)     3766 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/windows_parser.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    12449 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/peracruda.py
+-rw-r--r--   0 basilef   (1000) users      (100)      639 2024-03-15 15:10:11.000000 peracotta-2.3.1/src/peralog.py
+-rw-r--r--   0 basilef   (1000) users      (100)      337 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/reporter.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/src/scripts/
+-rwxr-xr-x   0 basilef   (1000) users      (100)     1628 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/check_dependencies.sh
+-rwxr-xr-x   0 basilef   (1000) users      (100)     1718 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/generate_files.sh
+-rw-r--r--   0 basilef   (1000) users      (100)     2694 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/get_windows_specs.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)      172 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/install_dependencies_all.sh
+-rw-r--r--   0 basilef   (1000) users      (100)     3216 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/tarallo.py
```

### Comparing `peracotta-2.3.0/LICENSE` & `peracotta-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/PKG-INFO` & `peracotta-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peracotta
-Version: 2.3.0
+Version: 2.3.1
 License: MIT License
         
         Copyright (c) 2018 WEEE Open
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `peracotta-2.3.0/README.md` & `peracotta-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/peracotta.egg-info/PKG-INFO` & `peracotta-2.3.1/peracotta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peracotta
-Version: 2.3.0
+Version: 2.3.1
 License: MIT License
         
         Copyright (c) 2018 WEEE Open
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `peracotta-2.3.0/peracotta.egg-info/SOURCES.txt` & `peracotta-2.3.1/peracotta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/pyproject.toml` & `peracotta-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/__init__.py` & `peracotta-2.3.1/src/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,7 +88,17 @@
 
 
 def main_cli():
     """.. todo::Entrypoint for the CLI version"""
     print("Sorry, peracruda isn't implemented in v2 yet! Use the old one at https://github.com/WEEE-Open/peracotta")
     parse_common_args()
     # peracruda.__main() # Doesn't seem to prompt for sudo password and gets stuck
+
+
+if __name__ == "__main__":
+    try:
+        if sys.argv[1] == "gui":
+            main_gui()
+        else:
+            main_cli()
+    except IndexError:
+        main_cli()
```

### Comparing `peracotta-2.3.0/src/assets/Installing.gif` & `peracotta-2.3.1/src/assets/Installing.gif`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/error.ui` & `peracotta-2.3.1/src/assets/error.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/interface.ui` & `peracotta-2.3.1/src/assets/interface.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/themes/Dark.css` & `peracotta-2.3.1/src/assets/themes/Dark.css`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/themes/WEEE Open.css` & `peracotta-2.3.1/src/assets/themes/WEEE Open.css`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/case.png` & `peracotta-2.3.1/src/assets/toolbox/case.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/cpu.png` & `peracotta-2.3.1/src/assets/toolbox/cpu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/gpu.png` & `peracotta-2.3.1/src/assets/toolbox/gpu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/hdd.png` & `peracotta-2.3.1/src/assets/toolbox/hdd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/keyboard.png` & `peracotta-2.3.1/src/assets/toolbox/keyboard.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/monitor.png` & `peracotta-2.3.1/src/assets/toolbox/monitor.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/motherboard.png` & `peracotta-2.3.1/src/assets/toolbox/motherboard.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/mouse.png` & `peracotta-2.3.1/src/assets/toolbox/mouse.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/odd.png` & `peracotta-2.3.1/src/assets/toolbox/odd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/psu.png` & `peracotta-2.3.1/src/assets/toolbox/psu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/ram.png` & `peracotta-2.3.1/src/assets/toolbox/ram.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/ssd.png` & `peracotta-2.3.1/src/assets/toolbox/ssd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/toolbox/wifi-card.png` & `peracotta-2.3.1/src/assets/toolbox/wifi-card.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/ui/light_down_arrow.png` & `peracotta-2.3.1/src/assets/ui/light_down_arrow.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/ui/light_split_handle.png` & `peracotta-2.3.1/src/assets/ui/light_split_handle.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/ui/pear_emoji.png` & `peracotta-2.3.1/src/assets/ui/pear_emoji.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/ui/radio_ckd.png` & `peracotta-2.3.1/src/assets/ui/radio_ckd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/ui/radio_unckd.png` & `peracotta-2.3.1/src/assets/ui/radio_unckd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/assets/uploadTaralloDialog.ui` & `peracotta-2.3.1/src/assets/uploadTaralloDialog.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/commons.py` & `peracotta-2.3.1/src/commons.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/config.py` & `peracotta-2.3.1/src/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 
 AUTOMATIC_REPORT_ERRORS = true
 REPORT_URL = "http://127.0.0.1:9999"
 ```
 This configuration can be overridden by `~/.config/WEEE Open/peracotta/.env`
 and/or environment variables. If both are used, the latter take precedence.
 
-For compatibility with the old M.I.S.O.'s martello.sh script, it's also possible to configure it by placing a .env file in the src directory. For the same reasons, there's a .env.example in the source code at the appropriate place
+For compatibility with the old M.I.S.O.'s martello.sh script, it's also possible to configure it by placing a .env file in the src directory. This file is only checked if peracotta is being launched directly from source instead of being installed.
+For this reasons, there's a .env.example in the source code at the appropriate place
 """
+
 import os
 from pathlib import Path
 
 import toml
 from dotenv import load_dotenv
 
 from .commons import parse_from_env
+from .constants import basedir
 
 HOME_DIR = Path().home()
 
 CONF_DIR = HOME_DIR.joinpath(".config/WEEE Open/peracotta")
 CONFIG = {}
 
 keys = [
@@ -38,36 +41,31 @@
     "TARALLO_FEATURES_AUTO_DOWNLOAD",
     "GENERATE_FILES_USE_SUDO",
     "GENERATE_FILES_ASK_SUDO_PASSWORD",
     "REPORT_URL",
     "AUTOMATIC_REPORT_ERRORS",
 ]
 
-# 1) local environment
-for key in keys:
-    CONFIG[key] = parse_from_env(os.environ.get(key))
+# 1) src's .env, for compatibility with old M.I.S.O.
+if isinstance(basedir, str):  # If the app is installed as a package basedir is a PosixPath object
+    try:
+        load_dotenv(basedir + "/../.env")  # doesn't override already defined variables
+    except FileNotFoundError:
+        pass
 
-# 1.1) src's .env, for compatibility with old M.I.S.O.
-try:
-    load_dotenv(".env")
-    for key in keys:
-        if key not in CONFIG.keys() or CONFIG[key] is None:
-            CONFIG[key] = parse_from_env(os.environ.get(key))
-except FileNotFoundError:
-    pass
 
 # 2) CONF_DIR's .env
 try:
     load_dotenv(CONF_DIR.joinpath(".env"))
-    for key in keys:
-        if key not in CONFIG.keys() or CONFIG[key] is None:
-            CONFIG[key] = parse_from_env(os.environ.get(key))
 except FileNotFoundError:
     pass
 
+for key in keys:
+    CONFIG[key] = parse_from_env(os.environ.get(key))
+
 # 3) CONF_DIR's toml
 try:
     _toml_conf = toml.load(CONF_DIR.joinpath("config.toml"))
     for k in _toml_conf:
         if k not in CONFIG.keys() or CONFIG[k] is None:
             CONFIG[k] = _toml_conf[k]
 except FileNotFoundError:
```

### Comparing `peracotta-2.3.0/src/constants.py` & `peracotta-2.3.1/src/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import importlib.resources
 import os
 
-basedir = importlib.resources.files("peracotta")
+try:
+    basedir = importlib.resources.files("peracotta")
+except ModuleNotFoundError:  # in case it's being called without installing the package
+    basedir = os.path.dirname(__file__)
 
 URL = {
     "website": "https://weeeopen.polito.it",
     "source_code": "https://github.com/WEEE-Open/peracotta",
 }
 
-VERSION = "2.3.0"
+VERSION = "2.3.1"
 
 PATH = {
     "UI": "assets/interface.ui",
     "TARALLOUPLOADDIALOG": "assets/uploadTaralloDialog.ui",
     "ERRORDIALOG": "assets/error.ui",
     "JSON": "copy_this_to_tarallo.json",
     "FEATURES": "features.json",
```

### Comparing `peracotta-2.3.0/src/features.json` & `peracotta-2.3.1/src/features.json`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/gui/PeraThread.py` & `peracotta-2.3.1/src/gui/PeraThread.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/gui/Toolbox.py` & `peracotta-2.3.1/src/gui/Toolbox.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/gui/exception_handler.py` & `peracotta-2.3.1/src/gui/exception_handler.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/gui/gui.py` & `peracotta-2.3.1/src/gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.features = dict()
         self.encountered_types_count = defaultdict(lambda: 0)
         self.active_theme = str()
 
         self.setWindowIcon(QtGui.QIcon(PATH["ICON"]))
 
         # shortcuts
-        self.refreshThemeShortcut = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+R"), self)
+        self.refreshThemeShortcut = QtWidgets.QShortcut(QtGui.QKeySequence("Ctrl+R"), self)
         self.refreshThemeShortcut.activated.connect(self.refresh_theme)
 
         # Output toolbox
         self.outputScrollArea = self.findChild(QtWidgets.QScrollArea, "outputScrollArea")
         self.itemToolBox = None
 
         # App settings
@@ -105,41 +105,41 @@
         self.saveJsonBtn.clicked.connect(self.save_json)
 
         # Upload to tarallo button
         self.uploadBtn = self.findChild(QtWidgets.QPushButton, "uploadBtn")
         self.uploadBtn.clicked.connect(self.tarallo_dialog)
 
         # File actions
-        self.actionOpen = self.findChild(QtGui.QAction, "actionOpen")
+        self.actionOpen = self.findChild(QtWidgets.QAction, "actionOpen")
         self.actionOpen.triggered.connect(self.open_json)
-        self.actionOpenLastJson = self.findChild(QtGui.QAction, "actionOpenLastJson")
+        self.actionOpenLastJson = self.findChild(QtWidgets.QAction, "actionOpenLastJson")
         self.actionOpenLastJson.triggered.connect(self.open_latest_json)
-        self.actionOpenJson = self.findChild(QtGui.QAction, "actionOpenJson")
+        self.actionOpenJson = self.findChild(QtWidgets.QAction, "actionOpenJson")
         self.actionOpenJson.triggered.connect(self.show_json)
-        self.actionLoadRawFiles = self.findChild(QtGui.QAction, "actionLoadRawFiles")
+        self.actionLoadRawFiles = self.findChild(QtWidgets.QAction, "actionLoadRawFiles")
         self.actionLoadRawFiles.triggered.connect(self._load_raw_files)
-        self.actionExit = self.findChild(QtGui.QAction, "actionExit")
+        self.actionExit = self.findChild(QtWidgets.QAction, "actionExit")
         self.actionExit.triggered.connect(self.close)
 
         # Options actions
         self.menuTheme = self.findChild(QtWidgets.QMenu, "menuTheme")
         action = list()
         action.append(self.menuTheme.addAction("Default"))
         action[-1].triggered.connect(lambda: self.set_theme("default"))
         for theme_file in os.listdir(PATH["THEMES"]):
             theme = theme_file.rstrip(".css")
             action.append(self.menuTheme.addAction(theme))
             action[-1].triggered.connect((lambda t: lambda: self.set_theme(t))(theme))
 
         # Help actions
-        self.actionAboutUs = self.findChild(QtGui.QAction, "actionAboutUs")
+        self.actionAboutUs = self.findChild(QtWidgets.QAction, "actionAboutUs")
         self.actionAboutUs.triggered.connect(self.open_website)
-        self.actionSourceCode = self.findChild(QtGui.QAction, "actionSourceCode")
+        self.actionSourceCode = self.findChild(QtWidgets.QAction, "actionSourceCode")
         self.actionSourceCode.triggered.connect(self.open_source_code)
-        self.actionVersion = self.findChild(QtGui.QAction, "actionVersion")
+        self.actionVersion = self.findChild(QtWidgets.QAction, "actionVersion")
         self.actionVersion.triggered.connect(self.show_version)
 
         # Status bar widgets
         self.progressBar = QtWidgets.QProgressBar()
         self.statusBar().addPermanentWidget(self.progressBar)
         self.progressBar.hide()
         # self.statusBar().setStyleSheet(DEFAULT_PROGRESS_BAR_STYLE)
@@ -181,19 +181,19 @@
             if item in niy:
                 checkbox.setEnabled(False)
             layout.addWidget(checkbox)
         self.reset_setup_group()
 
     @staticmethod
     def backup_features_json():
-        shutil.copy2(CONF_DIR.joinpath("features.json"), CONF_DIR.joinpath("features.json.bak"))
+        shutil.copy2(PATH["FEATURES"], PATH["FEATURES"] + ".bak")
 
     @staticmethod
     def restore_features_json():
-        shutil.move(CONF_DIR.joinpath("features.json.bak"), CONF_DIR.joinpath("features.json"))
+        shutil.move(PATH["FEATURES"] + ".bak", PATH["FEATURES"])
 
     def load_features_file(self, auto_update: bool):
         self.features = {}
         has_file = False
 
         try:
             mtime = os.path.getmtime(PATH["FEATURES"])
@@ -201,15 +201,14 @@
             has_file = True
         except FileNotFoundError:
             mtime = 0
 
         if auto_update and time.time() - mtime > 60 * 60 * 12:
             try:
                 response = requests.get(f"{CONFIG['TARALLO_URL']}/features.json", headers={"User-Agent": "peracotta", "Accept": "application/json"})
-
                 with open(CONF_DIR.joinpath("features.json"), "w") as fs:
                     json.dump(response.json(), fs)
 
                 has_file = True
             except requests.exceptions.ConnectionError as e:
                 logger.exception("Couldn't connect to TARALLO")
                 QtWidgets.QMessageBox.warning(None, "Error", f"Couldn't connect to TARALLO to update features.json")
```

### Comparing `peracotta-2.3.0/src/gui/prettyprinter.py` & `peracotta-2.3.1/src/gui/prettyprinter.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/gui/widgets.py` & `peracotta-2.3.1/src/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/read_decode_dimms.py` & `peracotta-2.3.1/src/parsers/read_decode_dimms.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/read_dmidecode.py` & `peracotta-2.3.1/src/parsers/read_dmidecode.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/read_lscpu.py` & `peracotta-2.3.1/src/parsers/read_lscpu.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/read_lspci_and_glxinfo.py` & `peracotta-2.3.1/src/parsers/read_lspci_and_glxinfo.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/read_smartctl.py` & `peracotta-2.3.1/src/parsers/read_smartctl.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/parsers/windows_parser.py` & `peracotta-2.3.1/src/parsers/windows_parser.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/peracruda.py` & `peracotta-2.3.1/src/peracruda.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/peralog.py` & `peracotta-2.3.1/src/peralog.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/scripts/check_dependencies.sh` & `peracotta-2.3.1/src/scripts/check_dependencies.sh`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/scripts/generate_files.sh` & `peracotta-2.3.1/src/scripts/generate_files.sh`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/scripts/get_windows_specs.py` & `peracotta-2.3.1/src/scripts/get_windows_specs.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.0/src/tarallo.py` & `peracotta-2.3.1/src/tarallo.py`

 * *Files identical despite different names*

