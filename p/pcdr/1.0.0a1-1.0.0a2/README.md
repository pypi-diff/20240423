# Comparing `tmp/pcdr-1.0.0a1.tar.gz` & `tmp/pcdr-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdr-1.0.0a1.tar", last modified: Mon Apr 15 23:29:26 2024, max compression
+gzip compressed data, was "pcdr-1.0.0a2.tar", last modified: Tue Apr 23 15:55:17 2024, max compression
```

## Comparing `pcdr-1.0.0a1.tar` & `pcdr-1.0.0a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/
--rw-r--r--   0 j         (1000) j         (1000)    35149 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1191 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/README.md
--rw-r--r--   0 j         (1000) j         (1000)      613 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/pyproject.toml
--rw-r--r--   0 j         (1000) j         (1000)       38 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/setup.cfg
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.762252 pcdr-1.0.0a1/src/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.766252 pcdr-1.0.0a1/src/pcdr/
--rw-r--r--   0 j         (1000) j         (1000)      768 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/__init__.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.766252 pcdr-1.0.0a1/src/pcdr/_beta/
--rw-r--r--   0 j         (1000) j         (1000)     3106 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_receiver.py
--rw-r--r--   0 j         (1000) j         (1000)     7122 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_sendlike.py
--rw-r--r--   0 j         (1000) j         (1000)     1774 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3866 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     9152 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_flow_impl.py
--rw-r--r--   0 j         (1000) j         (1000)     2807 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_helpers.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr/_internal/
--rw-r--r--   0 j         (1000) j         (1000)     3989 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/basictermplot.py
--rw-r--r--   0 j         (1000) j         (1000)     1565 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/fileio.py
--rw-r--r--   0 j         (1000) j         (1000)    13243 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/misc.py
--rw-r--r--   0 j         (1000) j         (1000)     7650 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/our_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     2456 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/queue_to_guisink_flowgraph.py
--rwxr-xr-x   0 j         (1000) j         (1000)     5357 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/queue_to_waterfall_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)      657 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/types_and_contracts.py
--rw-r--r--   0 j         (1000) j         (1000)     3013 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/vector_to_guisink_flowgraph.py
--rw-r--r--   0 j         (1000) j         (1000)     3430 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/vector_tx_flowgraphs.py
--rw-r--r--   0 j         (1000) j         (1000)     1451 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_internal/wrapped_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     5022 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_modulators.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr/_queue/
--rw-r--r--   0 j         (1000) j         (1000)       51 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     6343 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/sink.py
--rw-r--r--   0 j         (1000) j         (1000)     1199 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_queue/source.py
--rw-r--r--   0 j         (1000) j         (1000)    45382 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/_wavegen.py
--rw-r--r--   0 j         (1000) j         (1000)      141 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/src/pcdr/flow.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/src/pcdr.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1189 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       40 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2024-04-15 23:29:26.000000 pcdr-1.0.0a1/src/pcdr.egg-info/top_level.txt
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-15 23:29:26.770252 pcdr-1.0.0a1/tests/
--rw-r--r--   0 j         (1000) j         (1000)      838 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_gnuradio_vector_tx_flowgraphs.py
--rw-r--r--   0 j         (1000) j         (1000)      939 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_gnuradio_write_file_and_read_file.py
--rw-r--r--   0 j         (1000) j         (1000)      308 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_helpers.py
--rw-r--r--   0 j         (1000) j         (1000)     2988 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_multiple.py
--rw-r--r--   0 j         (1000) j         (1000)     5648 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_other__blocks_for_testing.py
--rw-r--r--   0 j         (1000) j         (1000)     2498 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_our_GR_blocks.py
--rw-r--r--   0 j         (1000) j         (1000)     1705 2024-04-15 23:29:19.000000 pcdr-1.0.0a1/tests/test_simple.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/
+-rw-r--r--   0 j         (1000) j         (1000)    35149 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1191 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/README.md
+-rw-r--r--   0 j         (1000) j         (1000)      613 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/pyproject.toml
+-rw-r--r--   0 j         (1000) j         (1000)       38 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/setup.cfg
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.992619 pcdr-1.0.0a2/src/
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.992619 pcdr-1.0.0a2/src/pcdr/
+-rw-r--r--   0 j         (1000) j         (1000)      781 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/__init__.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_beta/
+-rw-r--r--   0 j         (1000) j         (1000)     3106 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_receiver.py
+-rw-r--r--   0 j         (1000) j         (1000)     7098 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_sendlike.py
+-rw-r--r--   0 j         (1000) j         (1000)     1774 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3866 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     9152 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_flow_impl.py
+-rw-r--r--   0 j         (1000) j         (1000)     2766 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_helpers.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_internal/
+-rw-r--r--   0 j         (1000) j         (1000)     3989 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/basictermplot.py
+-rw-r--r--   0 j         (1000) j         (1000)     1565 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/fileio.py
+-rw-r--r--   0 j         (1000) j         (1000)    16005 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/misc.py
+-rw-r--r--   0 j         (1000) j         (1000)     7650 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     2456 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/queue_to_guisink_flowgraph.py
+-rwxr-xr-x   0 j         (1000) j         (1000)     5357 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/queue_to_waterfall_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)      657 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/types_and_contracts.py
+-rw-r--r--   0 j         (1000) j         (1000)     3013 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/vector_to_guisink_flowgraph.py
+-rw-r--r--   0 j         (1000) j         (1000)     3471 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)     1451 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_internal/wrapped_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     5185 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_modulators.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:16.996619 pcdr-1.0.0a2/src/pcdr/_queue/
+-rw-r--r--   0 j         (1000) j         (1000)       51 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     6343 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/sink.py
+-rw-r--r--   0 j         (1000) j         (1000)     1199 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_queue/source.py
+-rw-r--r--   0 j         (1000) j         (1000)    46825 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/_wavegen.py
+-rw-r--r--   0 j         (1000) j         (1000)      141 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/src/pcdr/flow.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/src/pcdr.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     1757 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1189 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       40 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2024-04-23 15:55:16.000000 pcdr-1.0.0a2/src/pcdr.egg-info/top_level.txt
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2024-04-23 15:55:17.000619 pcdr-1.0.0a2/tests/
+-rw-r--r--   0 j         (1000) j         (1000)      838 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_gnuradio_vector_tx_flowgraphs.py
+-rw-r--r--   0 j         (1000) j         (1000)      939 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_gnuradio_write_file_and_read_file.py
+-rw-r--r--   0 j         (1000) j         (1000)      308 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_helpers.py
+-rw-r--r--   0 j         (1000) j         (1000)     2988 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_multiple.py
+-rw-r--r--   0 j         (1000) j         (1000)     5648 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_other__blocks_for_testing.py
+-rw-r--r--   0 j         (1000) j         (1000)     2498 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_our_GR_blocks.py
+-rw-r--r--   0 j         (1000) j         (1000)     1705 2024-04-23 15:55:07.000000 pcdr-1.0.0a2/tests/test_simple.py
```

### Comparing `pcdr-1.0.0a1/LICENSE` & `pcdr-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/PKG-INFO` & `pcdr-1.0.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pcdr
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: GNU Radio-based transmit and receive wrappers and more
 Author: james-pcdr
 Project-URL: Homepage, https://github.com/python-can-define-radio/pcdr
 Project-URL: Bug Tracker, https://github.com/python-can-define-radio/pcdr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: termcolor
 Requires-Dist: typeguard
-Requires-Dist: attrs>=21.1.0
+Requires-Dist: attrs>=21.3.0
 
 # pcdr
 
 pcdr module: https://pypi.org/project/pcdr/
 
 ### Installation
```

### Comparing `pcdr-1.0.0a1/README.md` & `pcdr-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/pyproject.toml` & `pcdr-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=42.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pcdr"
-version = "1.0.0a1"
+version = "1.0.0a2"
 authors = [
   { name="james-pcdr" },
 ]
 description = "GNU Radio-based transmit and receive wrappers and more"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["numpy", "termcolor", "typeguard", "attrs>=21.1.0"]
+dependencies = ["numpy", "termcolor", "typeguard", "attrs>=21.3.0"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/python-can-define-radio/pcdr"
```

### Comparing `pcdr-1.0.0a1/src/pcdr/__init__.py` & `pcdr-1.0.0a2/src/pcdr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     generate_ook_modulated_example_file,
     makeWave,
     make_wave,
     multiply_by_complex_wave,
     multiply_by_real_wave,
     make_fft,
     make_fft_positive_freqs_only,
+    noisify,
 )
 
 from pcdr._helpers import (
     str_to_bin_list,
     int_to_bin_list,
 )
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_receiver.py` & `pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_receiver.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_beta/gnuradio_sendlike.py` & `pcdr-1.0.0a2/src/pcdr/_beta/gnuradio_sendlike.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 from gnuradio import gr
 
 from pcdr._beta.osmocom_queued_tx_flowgraph import queue_to_osmocom_sink, queue_to_print_sink, queue_to_string_file_sink, queue_to_file_sink, queue_to_zmqpub_sink
 from pcdr._internal.misc import SimpleQueueTypeWrapped, queue_to_list, prepend_zeros_, configure_graceful_exit
-from pcdr._internal.vector_tx_flowgraphs import vector_to_file_sink, vector_to_osmocom_sink
+from pcdr._internal.vector_tx_flowgraphs import vector_to_file_sink
 from pcdr._internal.types_and_contracts import TRealNum, TRealOrComplexNum
 from pcdr._internal.queue_to_guisink_flowgraph import queue_to_guisink
 from pcdr._internal.vector_to_guisink_flowgraph import vector_to_guisink
 
 
 
 try:
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py` & `pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_rx_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py` & `pcdr-1.0.0a2/src/pcdr/_beta/osmocom_queued_tx_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_flow_impl.py` & `pcdr-1.0.0a2/src/pcdr/_flow_impl.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_helpers.py` & `pcdr-1.0.0a2/src/pcdr/_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, TypeVar, Union
 from typeguard import typechecked
 
 import numpy as np
+from numpy.typing import NDArray
 
 
 
 @typechecked
 def bytes_to_bin_list(b: Union[bytes, List[int]]) -> List[int]:
     """
     Converts each item in b to bits.
@@ -55,37 +56,37 @@
     numeric = [ord(c) for c in message]
     if any(map(lambda x: x > 256, numeric)):
         raise ValueError(_NON_ASCII_ERR)
     return bytes_to_bin_list(numeric)
 
 
 @typechecked
-def int_to_bin_list(message: np.ndarray) -> List[int]:
+def int_to_bin_list(message: NDArray) -> List[int]:
     """
     Converts a numpy array of integers to a list of bits. Capable handling of a variety of dtypes.
 
     Examples:
 
-    >>> int_to_bin_list(np.array([0x43],dtype='uint8'))
+    >>> int_to_bin_list(np.array([0x43], dtype=np.uint8))
     [0, 1, 0, 0, 0, 0, 1, 1]
     
-    >>> int_to_bin_list(np.array([0x43,0x42],dtype='uint8'))
+    >>> int_to_bin_list(np.array([0x43, 0x42], dtype=np.uint8))
     [0, 1, 0, 0, 0, 0, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0]
     
-    >>> int_to_bin_list(np.array([0x4342],dtype='uint16'))
+    >>> int_to_bin_list(np.array([0x4342], dtype=np.uint16))
     [0, 1, 0, 0, 0, 0, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0]
 	"""
 
-    if ((message.dtype == 'int8')|(message.dtype == 'uint8')):
+    if message.dtype in [np.int8, np.uint8]:
         bitlength = 8
-    elif (((message.dtype == 'int16')|(message.dtype == 'uint16'))):
+    elif message.dtype in [np.int16, np.uint16]:
         bitlength = 16
-    elif (((message.dtype == 'int32')|(message.dtype == 'uint32'))):
+    elif message.dtype in [np.int32, np.uint32]:
         bitlength = 32
-    elif (((message.dtype == 'int64')|(message.dtype == 'uint64'))):
+    elif message.dtype in [np.int64, np.uint64]:
         bitlength = 64
     else:
         raise ValueError("Unsupported dtype")
 
     ret = [0]*bitlength*len(message)
     bitlist_index = 0
     shift_list = list(reversed(range(0,bitlength)))
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/basictermplot.py` & `pcdr-1.0.0a2/src/pcdr/_internal/basictermplot.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/fileio.py` & `pcdr-1.0.0a2/src/pcdr/_internal/fileio.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/misc.py` & `pcdr-1.0.0a2/src/pcdr/_internal/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from queue import SimpleQueue, Empty, Queue
 import signal
 import sys
-from typing import Union, Type, overload
+from typing import (
+    Union, Type, overload,
+    Literal, Callable, Type, Optional
+)
 
 import attrs
 from attrs import field, validators
 from gnuradio import gr
 import numpy as np
 import osmosdr
 from typeguard import typechecked
@@ -426,7 +429,95 @@
     """Sends `data` to osmocom sink."""
     from pcdr._internal.vector_tx_flowgraphs import vector_to_osmocom_sink
     normal_py_data = list(map(complex, data))  # GNURadio type issues. Eventually, fix this for efficiency
     tb = vector_to_osmocom_sink(normal_py_data, center_freq, samp_rate, if_gain, device_args, repeat)
     configure_graceful_exit(tb)
     tb.start()
     tb.wait()
+
+
+@typechecked
+def blockify(category: Literal["source", "sink", "whatever_you_call_the_others"],
+             func: Callable,
+             in_type: Optional[type],
+             out_type: Optional[type]):
+    """Turns a function into a (relatively inefficient) gnuradio block.
+    Mostly useful for testing.
+    
+    Example:
+    >>> import time
+    >>> state = {"current": np.int64(0)}
+    >>> def count_up() -> np.int64:
+    ...     what_it_was = state["current"]
+    ...     state["current"] += np.int64(1)
+    ...     time.sleep(0.1)
+    ...     return what_it_was
+    >>> srcblk = blockify("source", count_up, in_type=None, out_type=np.int64)
+    >>> snkblk = blockify("sink", print, in_type=np.int64, out_type=None)
+    >>> tb = gr.top_block()
+    >>> tb.connect(srcblk, snkblk)
+    >>> tb.start()
+    >>> time.sleep(0.5)
+    0
+    1
+    2
+    3
+    4
+    >>> tb.stop()
+    >>> tb.wait()
+    """
+    if category == "source":
+        class Blockify_Blk(gr.sync_block):
+            @typechecked
+            def __init__(self):
+                gr.sync_block.__init__(
+                    self,
+                    name='',
+                    in_sig=[],
+                    out_sig=[out_type]
+                )
+
+            def work(self, input_items, output_items):  
+                output_items[0][0] = func()
+                return 1        
+        return Blockify_Blk()
+    
+    elif category == "sink":
+        class Blockify_Blk(gr.sync_block):
+            @typechecked
+            def __init__(self):
+                gr.sync_block.__init__(
+                    self,
+                    name='',
+                    in_sig=[in_type],
+                    out_sig=[]
+                )
+                self._in_type = in_type
+
+            def work(self, input_items, output_items): 
+                # This may be a redundant check, but that's ok
+                #  because this is not meant to be performant
+                indat = input_items[0][0]
+                assert isinstance(indat, self._in_type)
+                func(indat)
+                return 1        
+        return Blockify_Blk()
+    
+    elif category == "whatever_you_call_the_others":
+        class Blockify_Blk(gr.sync_block):
+            @typechecked
+            def __init__(self):
+                gr.sync_block.__init__(
+                    self,
+                    name='',
+                    in_sig=[in_type],
+                    out_sig=[out_type]
+                )
+
+            def work(self, input_items, output_items):  
+                output_items[0][0] = func(input_items[0][0])
+                return 1        
+        return Blockify_Blk()
+    
+    else:
+        raise ValueError("not possible because of typechecked")
+
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/our_GR_blocks.py` & `pcdr-1.0.0a2/src/pcdr/_internal/our_GR_blocks.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/queue_to_guisink_flowgraph.py` & `pcdr-1.0.0a2/src/pcdr/_internal/queue_to_guisink_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/queue_to_waterfall_flowgraph.py` & `pcdr-1.0.0a2/src/pcdr/_internal/queue_to_waterfall_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/types_and_contracts.py` & `pcdr-1.0.0a2/src/pcdr/_internal/types_and_contracts.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/vector_to_guisink_flowgraph.py` & `pcdr-1.0.0a2/src/pcdr/_internal/vector_to_guisink_flowgraph.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/vector_tx_flowgraphs.py` & `pcdr-1.0.0a2/src/pcdr/_internal/vector_tx_flowgraphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # SPDX-License-Identifier: GPL-3.0
 #
 # GNU Radio Python Flow Graph
 # Title: Osmocom helper
 # GNU Radio version: 3.8.1.0
 
 import numpy as np
+from numpy.typing import NDArray
 from gnuradio import gr
 from gnuradio import blocks
 import osmosdr
 from pcdr._internal.our_GR_blocks import print_sink, string_file_sink
 from gnuradio import zeromq
 from typing import List
 from pcdr._internal.misc import validate_hack_rf_transmit
@@ -29,15 +30,15 @@
 # _queue_to_zmqpub_sink__queue_source = queue_source
 
 
 class vector_to_osmocom_sink(gr.top_block):
 
     @typechecked
     def __init__(self,
-                 data: List[complex],
+                 data: NDArray[np.complex64],
                  center_freq: float,
                  samp_rate: float,
                  if_gain: int,
                  device_args: str,
                  repeat: bool):
         """device_args: "hackrf=0" is common."""
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_internal/wrapped_GR_blocks.py` & `pcdr-1.0.0a2/src/pcdr/_internal/wrapped_GR_blocks.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_modulators.py` & `pcdr-1.0.0a2/src/pcdr/_modulators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Iterable, TypeVar, Tuple
 
 import numpy as np
+from numpy.typing import NDArray
 
 
 T = TypeVar('T')
 
 
 
 def __repeat_each_item(original: List[T], numtimes: int) -> List[T]:
@@ -41,15 +42,15 @@
     pcdr._modulators.NonBitError: ...
     """
     if not all(map(lambda x: x in [1, 0], bits)):
         raise NonBitError('`bits` must be of type List[int], and all of those integers'
                          ' must be either 0 or 1. It cannot be a string, such as "1010".')
 
 
-def ook_modulate(bits: List[int], bit_length: int, dtype=np.uint8) -> np.ndarray:
+def ook_modulate(bits: List[int], bit_length: int, dtype=np.uint8) -> NDArray:
     """
     OOK Modulate. This is equivalent to simply repeating the bits, that is,
     >>> ook_modulate([1, 0], 3)
     array([1, 1, 1, 0, 0, 0], dtype=uint8)
 
     It also converts the data to a numpy array.
 
@@ -61,15 +62,16 @@
     """ 
     __must_be_binary(bits)
     result = np.array(__repeat_each_item(bits, bit_length), dtype=dtype)
     assert result.dtype == dtype
     return result
 
 
-def ook_modulate_at_frequency(bits: List[int], bit_length: int, samp_rate: float, freq: float) -> Tuple[np.ndarray, np.ndarray]:
+def ook_modulate_at_frequency(bits: List[int], bit_length: int, samp_rate: float, freq: float
+                ) -> Tuple[NDArray[np.float64], NDArray[np.complex64]]:
     """
     OOK Modulate at a given frequency. Returns the timestamps and the modulated data.
 
     Examples:
     >>> from pcdr._internal.basictermplot import plot
     >>> timestamps, data = ook_modulate_at_frequency([1, 0, 1, 1], bit_length=20, samp_rate=40, freq=2)
     >>> plot(timestamps, data.real, 80, 10)
@@ -91,13 +93,13 @@
     __must_be_binary(bits)
     ## TODO: place this import better.
     ## For now, this import must be here due to circular imports
     from pcdr._wavegen import multiply_by_complex_wave
 
     baseband_sig = ook_modulate(bits, bit_length)
     result = multiply_by_complex_wave(baseband_sig, samp_rate, freq)
-    assert result[0].dtype == np.float64
+    assert result[0].dtype == np.float64    # TODO: these may be unnecessary now that I know how to do NDArray type annotations properly
     assert result[1].dtype == np.complex64
     assert len(result[0]) == len(result[1]) == (len(bits) * bit_length)
     return result
```

### Comparing `pcdr-1.0.0a1/src/pcdr/_queue/sink.py` & `pcdr-1.0.0a2/src/pcdr/_queue/sink.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_queue/source.py` & `pcdr-1.0.0a2/src/pcdr/_queue/source.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/src/pcdr/_wavegen.py` & `pcdr-1.0.0a2/src/pcdr/_wavegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import random
 from typing import Optional, List, Tuple, Literal
 
 import numpy as np
+from numpy.typing import NDArray
 from typeguard import typechecked
 
 from pcdr._internal.fileio import writeRealCSV, writeComplexCSV
 from pcdr._modulators import ook_modulate
 from pcdr._helpers import str_to_bin_list
 
 
 
-def make_timestamps_seconds(seconds: float, num_samples: int, dtype=np.float64) -> np.ndarray:
+@typechecked
+def make_timestamps_seconds(seconds: float, num_samples: int, dtype=np.float64) -> NDArray:
     """Creates timestamps from zero up to the given maximum number of seconds.
     Implemented using np.linspace().
     
     Note: We use np.float64 as the default dtype because np.float32 was causing float rounding issues
     that became worse with larger time values (as float rounding issues usually do).
     
     Example:
@@ -32,15 +34,16 @@
     )
     assert result.dtype == dtype
     assert len(result) == num_samples
     assert (0 <= result).all()
     return result
 
 
-def make_timestamps_samprate(samp_rate: float, num_samples: int, dtype=np.float64) -> np.ndarray:
+@typechecked
+def make_timestamps_samprate(samp_rate: float, num_samples: int, dtype=np.float64) -> NDArray:
     """Creates `num_samples` timestamps spaced by `1/samp_rate`.
     Implemented using np.linspace().
     
     Examples:
     >>> make_timestamps_samprate(5, 10)
     array([0. , 0.2, 0.4, 0.6, 0.8, 1. , 1.2, 1.4, 1.6, 1.8])
 
@@ -71,27 +74,28 @@
     raise NotImplementedError("Intended purpose: run either make_timestamps_seconds or make_timestamps_samprate based on provided arguments")
 
 #### This is something we may do eventually.
 # @overload
 # def makeRealWave(samp_rate: float,
 #                  freq: float,
 #                  num_samples: int,
-#                  allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]: ...
+#                  allowAliasing: bool = False) -> Tuple[NDArray, NDArray]: ...
 # @overload
 # def makeRealWave(samp_rate: float,
 #                  freq: float,
 #                  seconds: float,
-#                  allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]: ...
+#                  allowAliasing: bool = False) -> Tuple[NDArray, NDArray]: ...
 # def makeRealWave(samp_rate: float,
 #                  freq: float,
 #                  **kwargs):
 #     return something
 
 
-def makeRealWave_basic(timestamps: np.ndarray, freq: float) -> np.ndarray:
+@typechecked
+def makeRealWave_basic(timestamps: NDArray, freq: float) -> NDArray[np.float32]:
     """Return a sine wave.
     
     Example:
     >>> from pcdr._internal.basictermplot import plot
     >>> timestamps = make_timestamps_seconds(1, 50)
     >>> wave = makeRealWave_basic(timestamps, 2)
     >>> plot(timestamps, wave)
@@ -109,15 +113,16 @@
     ~████████████████oooooo███████████████████oooooo███
     """
     result = np.float32(np.sin(freq * 2 * np.pi * timestamps))
     assert timestamps.shape == result.shape
     return result
 
 
-def makeComplexWave_basic(timestamps: np.ndarray, freq: float) -> np.ndarray:
+@typechecked
+def makeComplexWave_basic(timestamps: NDArray, freq: float) -> NDArray[np.complex64]:
     """Return a complex wave.
     
     The real part is cosine (starts at 1); the imaginary part is sine (starts at 0).
     
     Example:
     >>> from pcdr._internal.basictermplot import plot
     >>> timestamps = make_timestamps_seconds(1, 50)
@@ -159,15 +164,15 @@
 
 
 
 class AliasError(ValueError):
     pass
 
 
-
+@typechecked
 def _isAliasingWhenDisallowed(allowAliasing: bool, freq: float, samp_rate: float) -> bool:
     """
     Examples:
 
     >>> allowAliasing = False
     >>> samp_rate = 5
     >>> too_high_freq = 4
@@ -181,22 +186,24 @@
     False
     >>> _isAliasingWhenDisallowed(allowAliasing, acceptable_freq, samp_rate)
     False
     """
     return (not allowAliasing) and (abs(freq) > samp_rate/2)
 
 
+@typechecked
 def _aliasingError(allowAliasing: bool, freq: float, samp_rate: float) -> None:
     """Gives a detailed Aliasing error message if it's aliasing when it shouldn't.
     :raises AliasError:"""
     if _isAliasingWhenDisallowed(allowAliasing, freq, samp_rate):
         raise AliasError(f"For a sample rate of {samp_rate}, the highest frequency that can be faithfully represented is {samp_rate/2}. The specified freq, {freq}, is greater than the limit specified by Shannon/Nyquist/Kotelnikov/Whittaker (commonly called the Nyquist frequency).")
 
 
-def makeComplexWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+@typechecked
+def makeComplexWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.complex64]]:
     """
     Returns a tuple (timestamps, wave).
     
     The real part of the wave is cosine (starts at 1); the imaginary part is sine (starts at 0).
 
     :raises AliasError: if _isAliasingWhenDisallowed
     
@@ -236,15 +243,16 @@
     t = num_samples / samp_rate
     timestamps = make_timestamps_seconds(seconds=t, num_samples=num_samples)
     wave = makeComplexWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
-def makeRealWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+@typechecked
+def makeRealWave_numsamps(num_samples: int, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.float32]]:
     """
     Return a Real wave.
 
     :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
     >>> from pcdr._internal.basictermplot import plot
@@ -269,15 +277,15 @@
     t = num_samples / samp_rate
     timestamps = make_timestamps_seconds(seconds=t, num_samples=num_samples)
     wave = makeRealWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
-def makeComplexWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+def makeComplexWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.complex64]]:
     """
     Returns a tuple (timestamps, wave).
     
     The real part of the wave is cosine (starts at 1); the imaginary part is sine (starts at 0).
 
     :raises AliasError: if _isAliasingWhenDisallowed
     
@@ -316,15 +324,15 @@
     num_samples = int(samp_rate * seconds)
     timestamps = make_timestamps_seconds(seconds, num_samples)
     wave = makeComplexWave_basic(timestamps, freq)
     assert len(timestamps) == len(wave) == num_samples
     return timestamps, wave
 
 
-def makeRealWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+def makeRealWave_time(seconds: float, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.float32]]:
     """
     Return a Real wave.
 
     :raises AliasError: if _isAliasingWhenDisallowed
     
     Example:
     >>> from pcdr._internal.basictermplot import plot
@@ -354,24 +362,55 @@
 
 @typechecked
 def make_wave(samp_rate: float,
              freq: float,
              type_: Literal["real", "complex"],
              *, seconds: Optional[float] = None,
              num: Optional[float] = None,
-             allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+             allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray]:
     """
-    TODO:
-     - finish writing tests
-     - Write implementation that makes these tests pass
-     - Change lessons to use makeWave
-     - Add @typechecked to all funcs in this file
+    Generate a sine wave and the associated timestamps.
+
+    Parameters:
+    -----------
+    samp_rate :
+        Measured in samples per second.
+    freq :
+        Frequency in Hz of the generated wave.
+    type_ :
+        "real" will have no imaginary part. "complex" will have an imaginary part that is 90 degrees out of phase from the real part.
+    seconds : 
+        The length of the signal will be this many seconds. See example 1.
+        
+
+    Examples:
+    ---------
+
+    Example 1: Demonstrating `seconds`.
     
-    >>> from pcdr._internal.basictermplot import plot
+    If we set our sample rate...   
+    >>> samp_rate = 50
+
+    ...and our number of seconds...  
+    >>> seconds = 2
+
+    ...the return value will have the length that we expect, which is samp_rate * seconds samples:
+    >>> timestamps, wave = makeWave(samp_rate, freq=3, "real", seconds=seconds)
+    >>> print(len(timestamps))
+    100
+    >>> print(len(wave))
+    100
+    
+
+    Example 2: Plotting a result.
+    Generate one second of data of a 3 Hz wave. The sample rate is 50 samples per second, and it is a real wave (no imaginary part).
     >>> timestamps, wave = makeWave(50, 3, "real", seconds=1)
+
+    Plot that wave. (Note, matplotlib would generate a superior plot; this is a simplified textual plot.)
+    >>> from pcdr._internal.basictermplot import plot
     >>> plot(timestamps, wave)
     xmin: 0.00
     xmax: 0.98
     ymin: -1.00
     ymax: 1.00
     ~████o████████████████o████████████████████████████
     ~███o█oo████████████oo█o█████████████oooo██████████
@@ -487,16 +526,16 @@
             return makeComplexWave_numsamps(num, samp_rate, freq, allowAliasing)
         else:
             raise ValueError("This will never happen if the @typechecked works")
     else:
         raise Exception("Impossible case")
 
 
-makeWave = make_wave
-
+def makeWave(*args, **kwargs):
+    print("Use make_wave instead.")
 
 
 def wave_and_write(basename: str, timestamps: np.ndarray, freq, complex_or_real: Literal["c", "r"]):
     if complex_or_real == "r":
         data = makeRealWave_basic(timestamps, freq)
         writeRealCSV(basename + ".csv", data)
         data.tofile(basename + ".float32")
@@ -553,15 +592,16 @@
         raise ValueError(f"The number of samples would be {num_samples}, but a partial sample is meaningless.\nPlease pick a sample rate and an amount of time whose product is an integer.")
 
     timestamps = make_timestamps_seconds(max_time, num_samples)
 
     wave_and_write(filename, timestamps, freq, complex_or_real)
 
 
-def multiply_by_complex_wave(baseband_sig: np.ndarray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+@typechecked
+def multiply_by_complex_wave(baseband_sig: NDArray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.complex64]]:
     """
     Returns a tuple (timestamps, mult).
 
     >>> from pcdr._internal.basictermplot import plot
     >>> from pcdr import multiply_by_complex_wave, ook_modulate
     >>> baseband_sig = ook_modulate([1, 0], 32)
     >>> timestamps, mult = multiply_by_complex_wave(baseband_sig, 64, 2)
@@ -583,15 +623,16 @@
     mult = np.complex64(baseband_sig) * wave
     assert len(timestamps) == len(mult) == len(baseband_sig)
     assert timestamps.dtype == np.float64
     assert mult.dtype == np.complex64
     return timestamps, mult
 
 
-def multiply_by_real_wave(baseband_sig: np.ndarray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+@typechecked
+def multiply_by_real_wave(baseband_sig: NDArray, samp_rate: float, freq: float, allowAliasing: bool = False) -> Tuple[NDArray[np.float64], NDArray[np.float32]]:
     """
     Returns a tuple (timestamps, mult).
 
     >>> from pcdr._internal.basictermplot import plot
     >>> from pcdr import multiply_by_real_wave, ook_modulate
     >>> baseband_sig = ook_modulate([1, 0], 32)
     >>> timestamps, wave = multiply_by_real_wave(baseband_sig, 64, 2)
@@ -613,15 +654,16 @@
     mult = np.float32(baseband_sig) * wave
     assert len(timestamps) == len(mult) == len(baseband_sig)
     assert timestamps.dtype == np.float64
     assert mult.dtype == np.float32
     return timestamps, mult
 
 
-def random_normal(size: int, dtype=np.float32, seed=None) -> np.ndarray:
+@typechecked
+def random_normal(size: int, dtype=np.float32, seed=None) -> NDArray:
     """A wrapper of numpy's `standard_normal()` function;
     returns a numpy array of length `size` containing normally distributed noise.
 
     `seed` is optional, and mostly just used for testing the function.
     
     TODO >>> random_normal(size=3, seed=0)
     array([ 1.117622 , -1.3871249, -0.4265716], dtype=float32)
@@ -640,15 +682,16 @@
         raise NotImplementedError()
     assert isinstance(result, np.ndarray)
     assert len(result) == size
     assert result.dtype == dtype
     return result
 
 
-def noisify(data: np.ndarray, amplitude=1, seed=None) -> np.ndarray:
+@typechecked
+def noisify(data: NDArray, amplitude=1, seed=None) -> NDArray:
     """
     Returns a copy of `data` with random normally distributed noise added.
     `seed` is optional, and mostly just used for testing the function.
 
     TODO >>> dat = np.array([10, 100, 1000], dtype=np.float32)
     TODO >>> noisify(dat, amplitude=0.1, seed=0)
     array([ 11.117622,  98.61288 , 999.5734  ], dtype=float32)
@@ -667,15 +710,16 @@
         raise NotImplementedError("Currently, this only works for these dtypes: float32, complex64.")
     assert randnoise.dtype == data.dtype
     result = data + amplitude * randnoise
     assert result.dtype == data.dtype
     return result
 
 
-def generate_ook_modulated_example_data(noise: bool = False, message_delay: bool = False, text_source: Optional[str] = None) -> np.ndarray:
+@typechecked
+def generate_ook_modulated_example_data(noise: bool = False, message_delay: bool = False, text_source: Optional[str] = None) -> NDArray[np.complex64]:
     """
     Generate a file with the given `output_filename`.
 
     if `noise` is True, random noise will be added to the generated signal.
     if `message_delay` is True, there will be a pause before the meaningful data starts.
     if `text_source` is any string, a random sentence from it will be used as the message.
     
@@ -708,14 +752,17 @@
     if noise:
         fully_modded = noisify(fully_modded)
     
     assert fully_modded.dtype == np.complex64
     return fully_modded
 
 
+## TODO: 2024 APRIL 18: FINISH ADDING TYPECHECKED AND ALSO CONVERT NDARRAY
+
+@typechecked
 def generate_ook_modulated_example_file(output_filename: str, noise: bool = False, message_delay: bool = False, text_source: Optional[str] = None):
     """
     Generate a file with the given `output_filename`.
 
     if `noise` is True, random noise will be added to the generated signal.
     if `message_delay` is True, there will be a pause before the meaningful data starts.
     if `text_source` is any string, a random sentence from it will be used as the message.
@@ -726,15 +773,16 @@
     generate_ook_modulated_example_file("generated_example_file.complex", text_source=text_content)
     """
     
     data = generate_ook_modulated_example_data(noise, message_delay, text_source)
     data.tofile(output_filename)
 
 
-def make_fft_positive_freqs_only(sig: np.ndarray, samp_rate: float) -> Tuple[np.ndarray, np.ndarray]:
+@typechecked
+def make_fft_positive_freqs_only(sig: NDArray, samp_rate: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     Computes an fft, returns only the positive frequencies.
     Return value is a tuple: (sample_freqs, fft_mag).
     `sample_freqs` ranges from 0 to approximately samp_rate/2
 
     >>> from pcdr._internal.basictermplot import plot
     >>> from pcdr import make_wave, make_fft_positive_freqs_only
```

### Comparing `pcdr-1.0.0a1/src/pcdr.egg-info/PKG-INFO` & `pcdr-1.0.0a2/src/pcdr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pcdr
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: GNU Radio-based transmit and receive wrappers and more
 Author: james-pcdr
 Project-URL: Homepage, https://github.com/python-can-define-radio/pcdr
 Project-URL: Bug Tracker, https://github.com/python-can-define-radio/pcdr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: termcolor
 Requires-Dist: typeguard
-Requires-Dist: attrs>=21.1.0
+Requires-Dist: attrs>=21.3.0
 
 # pcdr
 
 pcdr module: https://pypi.org/project/pcdr/
 
 ### Installation
```

### Comparing `pcdr-1.0.0a1/src/pcdr.egg-info/SOURCES.txt` & `pcdr-1.0.0a2/src/pcdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_gnuradio_vector_tx_flowgraphs.py` & `pcdr-1.0.0a2/tests/test_gnuradio_vector_tx_flowgraphs.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_gnuradio_write_file_and_read_file.py` & `pcdr-1.0.0a2/tests/test_gnuradio_write_file_and_read_file.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_multiple.py` & `pcdr-1.0.0a2/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_other__blocks_for_testing.py` & `pcdr-1.0.0a2/tests/test_other__blocks_for_testing.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_our_GR_blocks.py` & `pcdr-1.0.0a2/tests/test_our_GR_blocks.py`

 * *Files identical despite different names*

### Comparing `pcdr-1.0.0a1/tests/test_simple.py` & `pcdr-1.0.0a2/tests/test_simple.py`

 * *Files identical despite different names*

