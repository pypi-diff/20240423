# Comparing `tmp/nxtomomill-1.0.5.tar.gz` & `tmp/nxtomomill-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxtomomill-1.0.5.tar", last modified: Thu Mar 21 04:39:23 2024, max compression
+gzip compressed data, was "nxtomomill-1.0.6.tar", last modified: Tue Apr 23 13:15:54 2024, max compression
```

## Comparing `nxtomomill-1.0.5.tar` & `nxtomomill-1.0.6.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/
--rw-r--r--   0 payno     (1000) payno     (1000)     1257 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     2130 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     1173 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/README.md
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.992654 nxtomomill-1.0.5/nxtomomill/
--rw-r--r--   0 payno     (1000) payno     (1000)      278 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8734 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/__main__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/app/
--rw-r--r--   0 payno     (1000) payno     (1000)       30 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8600 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/dxfile2nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5976 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/edf2nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4103 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/edf2nx_check.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2494 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/edfconfig.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2364 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/fscan2nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16200 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/app/h52nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14979 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/app/h5_3dxrd2nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4141 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/h5config.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2448 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/nxcopy.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14923 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/patch_nx.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5156 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/app/split_nxfile.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16992 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/app/z_concatenate_scans.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9511 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/app/zstages2nxs.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/
--rw-r--r--   0 payno     (1000) payno     (1000)      484 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      189 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/baseconverter.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/dxfile/
--rw-r--r--   0 payno     (1000) payno     (1000)      237 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/dxfile/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    27310 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/converter/dxfile/dxfileconverter.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5022 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/converter/dxfile/test_dxfile.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/edf/
--rw-r--r--   0 payno     (1000) payno     (1000)      117 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/edf/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2329 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/converter/edf/checks.py
--rw-r--r--   0 payno     (1000) payno     (1000)    45229 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/converter/edf/edfconverter.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/fscan/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/fscan/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4947 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/fscan/fscanconverter.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/hdf5/
--rw-r--r--   0 payno     (1000) payno     (1000)     1470 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    26157 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/baseacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5067 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/blisstomoconfig.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15312 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)    47110 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/standardacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10937 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4603 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2515 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6070 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py
--rw-r--r--   0 payno     (1000) payno     (1000)    37501 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/hdf5converter.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4698 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/hdf5/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1589 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/converter/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill/io/
--rw-r--r--   0 payno     (1000) payno     (1000)       91 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3548 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/acquisitionstep.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/nxtomomill/io/config/
--rw-r--r--   0 payno     (1000) payno     (1000)     1611 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/config/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8422 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/config/configbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13649 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/config/confighandler.py
--rw-r--r--   0 payno     (1000) payno     (1000)    45355 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/io/config/edfconfig.py
--rw-r--r--   0 payno     (1000) payno     (1000)    57219 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/io/config/hdf5config.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12436 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/io/framegroup.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5316 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/io/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/nxtomomill/nexus/
--rw-r--r--   0 payno     (1000) payno     (1000)      365 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      297 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      303 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      294 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)      318 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/nxtransformations.py
--rw-r--r--   0 payno     (1000) payno     (1000)      284 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/nexus/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5435 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/settings.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/nxtomomill/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     1476 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/test/test_version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/nxtomomill/test/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/test/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    26897 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/test/utils/bliss.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3253 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/test/utils/dxfile.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/nxtomomill/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)      705 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    13180 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/flat_reducer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    16832 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/frameappender.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3246 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/h5pyutils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3361 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/hdf5.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3205 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/nxtomomill/utils/io.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4102 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/nexus.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3396 2024-03-20 17:53:03.000000 nxtomomill-1.0.5/nxtomomill/utils/progress.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19189 2024-03-21 04:37:37.000000 nxtomomill-1.0.5/nxtomomill/utils/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4345 2024-03-21 04:39:10.000000 nxtomomill-1.0.5/nxtomomill/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-21 04:39:22.996654 nxtomomill-1.0.5/nxtomomill.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     2130 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     2755 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       56 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      260 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       11 2024-03-21 04:39:22.000000 nxtomomill-1.0.5/nxtomomill.egg-info/top_level.txt
--rw-r--r--   0 payno     (1000) payno     (1000)     1361 2024-03-21 04:39:23.000654 nxtomomill-1.0.5/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)     1486 2024-03-14 18:41:23.000000 nxtomomill-1.0.5/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.833346 nxtomomill-1.0.6/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1257 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     2879 2024-04-23 13:15:54.833346 nxtomomill-1.0.6/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     1173 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/README.md
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.825345 nxtomomill-1.0.6/nxtomomill/
+-rw-r--r--   0 payno     (1000) payno     (1000)      278 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8734 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/__main__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)       30 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8600 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/dxfile2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5976 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/edf2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4103 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/edf2nx_check.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2494 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/edfconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2364 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/fscan2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16200 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/app/h52nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14979 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/app/h5_3dxrd2nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4141 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/h5config.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2448 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/nxcopy.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14923 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/patch_nx.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5156 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/app/split_nxfile.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16992 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/app/z_concatenate_scans.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9511 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/app/zstages2nxs.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/
+-rw-r--r--   0 payno     (1000) payno     (1000)      484 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      189 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/baseconverter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/dxfile/
+-rw-r--r--   0 payno     (1000) payno     (1000)      237 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/dxfile/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    27310 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/converter/dxfile/dxfileconverter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5022 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/converter/dxfile/test_dxfile.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/edf/
+-rw-r--r--   0 payno     (1000) payno     (1000)      117 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/edf/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2329 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/converter/edf/checks.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    45229 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/converter/edf/edfconverter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/fscan/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/fscan/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4947 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/fscan/fscanconverter.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/hdf5/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1470 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    26157 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/baseacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5067 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/blisstomoconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15312 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    47110 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/standardacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10937 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4603 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2515 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6070 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    37501 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/hdf5converter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4698 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/hdf5/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1589 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/converter/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/io/
+-rw-r--r--   0 payno     (1000) payno     (1000)       91 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3548 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/acquisitionstep.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/io/config/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1611 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/config/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8422 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/config/configbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13649 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/config/confighandler.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    45355 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/io/config/edfconfig.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    57219 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/io/config/hdf5config.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12436 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/io/framegroup.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5316 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/io/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/nexus/
+-rw-r--r--   0 payno     (1000) payno     (1000)      365 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      297 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      303 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      294 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      291 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      318 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/nxtransformations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      284 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/nexus/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5435 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/settings.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1476 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/test/test_version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.829345 nxtomomill-1.0.6/nxtomomill/test/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/test/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    26897 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/test/utils/bliss.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3253 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/test/utils/dxfile.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.833346 nxtomomill-1.0.6/nxtomomill/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)      705 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13180 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/utils/flat_reducer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    16832 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/utils/frameappender.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3246 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/utils/h5pyutils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3361 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/utils/hdf5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3205 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/nxtomomill/utils/io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4102 2024-03-21 04:37:37.000000 nxtomomill-1.0.6/nxtomomill/utils/nexus.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3396 2024-03-20 17:53:03.000000 nxtomomill-1.0.6/nxtomomill/utils/progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19261 2024-04-23 13:15:21.000000 nxtomomill-1.0.6/nxtomomill/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4345 2024-04-23 13:15:41.000000 nxtomomill-1.0.6/nxtomomill/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 13:15:54.833346 nxtomomill-1.0.6/nxtomomill.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2879 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2755 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       56 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      260 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       11 2024-04-23 13:15:54.000000 nxtomomill-1.0.6/nxtomomill.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     1361 2024-04-23 13:15:54.833346 nxtomomill-1.0.6/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1486 2024-03-14 18:41:23.000000 nxtomomill-1.0.6/setup.py
```

### Comparing `nxtomomill-1.0.5/LICENSE` & `nxtomomill-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/README.md` & `nxtomomill-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/__main__.py` & `nxtomomill-1.0.6/nxtomomill/__main__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/dxfile2nx.py` & `nxtomomill-1.0.6/nxtomomill/app/dxfile2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/edf2nx.py` & `nxtomomill-1.0.6/nxtomomill/app/edf2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/edf2nx_check.py` & `nxtomomill-1.0.6/nxtomomill/app/edf2nx_check.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/edfconfig.py` & `nxtomomill-1.0.6/nxtomomill/app/edfconfig.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/fscan2nx.py` & `nxtomomill-1.0.6/nxtomomill/app/fscan2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/h52nx.py` & `nxtomomill-1.0.6/nxtomomill/app/h52nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/h5_3dxrd2nx.py` & `nxtomomill-1.0.6/nxtomomill/app/h5_3dxrd2nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/h5config.py` & `nxtomomill-1.0.6/nxtomomill/app/h5config.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/nxcopy.py` & `nxtomomill-1.0.6/nxtomomill/app/nxcopy.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/patch_nx.py` & `nxtomomill-1.0.6/nxtomomill/app/patch_nx.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/split_nxfile.py` & `nxtomomill-1.0.6/nxtomomill/app/split_nxfile.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/z_concatenate_scans.py` & `nxtomomill-1.0.6/nxtomomill/app/z_concatenate_scans.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/app/zstages2nxs.py` & `nxtomomill-1.0.6/nxtomomill/app/zstages2nxs.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/dxfile/dxfileconverter.py` & `nxtomomill-1.0.6/nxtomomill/converter/dxfile/dxfileconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/dxfile/test_dxfile.py` & `nxtomomill-1.0.6/nxtomomill/converter/dxfile/test_dxfile.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/edf/checks.py` & `nxtomomill-1.0.6/nxtomomill/converter/edf/checks.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/edf/edfconverter.py` & `nxtomomill-1.0.6/nxtomomill/converter/edf/edfconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/fscan/fscanconverter.py` & `nxtomomill-1.0.6/nxtomomill/converter/fscan/fscanconverter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/__init__.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/baseacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/baseacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/blisstomoconfig.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/blisstomoconfig.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/pcotomoacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/standardacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/standardacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/utils.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/xrd3dacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/xrdctacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/acquisition/zseriesacquisition.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/hdf5converter.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/hdf5converter.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/hdf5/utils.py` & `nxtomomill-1.0.6/nxtomomill/converter/hdf5/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/converter/version.py` & `nxtomomill-1.0.6/nxtomomill/converter/version.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/acquisitionstep.py` & `nxtomomill-1.0.6/nxtomomill/io/acquisitionstep.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/config/__init__.py` & `nxtomomill-1.0.6/nxtomomill/io/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/config/configbase.py` & `nxtomomill-1.0.6/nxtomomill/io/config/configbase.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/config/confighandler.py` & `nxtomomill-1.0.6/nxtomomill/io/config/confighandler.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/config/edfconfig.py` & `nxtomomill-1.0.6/nxtomomill/io/config/edfconfig.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/config/hdf5config.py` & `nxtomomill-1.0.6/nxtomomill/io/config/hdf5config.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/framegroup.py` & `nxtomomill-1.0.6/nxtomomill/io/framegroup.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/io/utils.py` & `nxtomomill-1.0.6/nxtomomill/io/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/settings.py` & `nxtomomill-1.0.6/nxtomomill/settings.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/test/test_version.py` & `nxtomomill-1.0.6/nxtomomill/test/test_version.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/test/utils/bliss.py` & `nxtomomill-1.0.6/nxtomomill/test/utils/bliss.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/test/utils/dxfile.py` & `nxtomomill-1.0.6/nxtomomill/test/utils/dxfile.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/__init__.py` & `nxtomomill-1.0.6/nxtomomill/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/flat_reducer.py` & `nxtomomill-1.0.6/nxtomomill/utils/flat_reducer.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/frameappender.py` & `nxtomomill-1.0.6/nxtomomill/utils/frameappender.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/h5pyutils.py` & `nxtomomill-1.0.6/nxtomomill/utils/h5pyutils.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/hdf5.py` & `nxtomomill-1.0.6/nxtomomill/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/io.py` & `nxtomomill-1.0.6/nxtomomill/utils/io.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/nexus.py` & `nxtomomill-1.0.6/nxtomomill/utils/nexus.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/progress.py` & `nxtomomill-1.0.6/nxtomomill/utils/progress.py`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/nxtomomill/utils/utils.py` & `nxtomomill-1.0.6/nxtomomill/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,16 @@
     )
     wheres = "start", "end", "end", "start"  # warning: order import
 
     for d_n, data, key, where in zip(data_names, datas, keys_value, wheres):
         if data is None:
             continue
         n_frames_to_insert = 1
+        if isinstance(data, str):
+            data = DataUrl(path=data)
         if isinstance(data, numpy.ndarray) and data.ndim == 3:
             n_frames_to_insert = data.shape[0]
         elif isinstance(data, DataUrl):
             with open_hdf5(data.file_path()) as h5s:
                 if data.data_path() not in h5s:
                     raise KeyError(
                         f"Path given ({data.data_path()}) is not in {data.file_path}"
```

### Comparing `nxtomomill-1.0.5/nxtomomill/version.py` & `nxtomomill-1.0.6/nxtomomill/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     "gamma": 12,
     "rc": 13,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 0
-MICRO = 5
+MICRO = 6
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
```

### Comparing `nxtomomill-1.0.5/nxtomomill.egg-info/SOURCES.txt` & `nxtomomill-1.0.6/nxtomomill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/setup.cfg` & `nxtomomill-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nxtomomill-1.0.5/setup.py` & `nxtomomill-1.0.6/setup.py`

 * *Files identical despite different names*

