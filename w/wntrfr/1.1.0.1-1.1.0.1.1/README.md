# Comparing `tmp/wntrfr-1.1.0.1.tar.gz` & `tmp/wntrfr-1.1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wntrfr-1.1.0.1.tar", last modified: Thu Apr 18 01:02:30 2024, max compression
+gzip compressed data, was "wntrfr-1.1.0.1.1.tar", last modified: Tue Apr 23 00:30:47 2024, max compression
```

## Comparing `wntrfr-1.1.0.1.tar` & `wntrfr-1.1.0.1.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.668003 wntrfr-1.1.0.1/
--rw-rw-rw-   0        0        0     4787 2024-04-12 18:43:38.000000 wntrfr-1.1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      343 2024-04-18 00:54:57.000000 wntrfr-1.1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4705 2024-04-18 01:02:30.668003 wntrfr-1.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1/README.md
--rw-rw-rw-   0        0        0      210 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 01:02:30.668003 wntrfr-1.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4384 2024-04-13 00:40:09.000000 wntrfr-1.1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.615293 wntrfr-1.1.0.1/wntrfr/
--rw-rw-rw-   0        0        0      570 2024-04-18 01:02:14.000000 wntrfr-1.1.0.1/wntrfr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.621854 wntrfr-1.1.0.1/wntrfr/epanet/
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.622856 wntrfr-1.1.0.1/wntrfr/epanet/Darwin/
--rw-rw-rw-   0        0        0   302216 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1/wntrfr/epanet/Darwin/libepanet.dylib
--rw-rw-rw-   0        0        0   325828 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1/wntrfr/epanet/Darwin/libepanet22.dylib
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.625152 wntrfr-1.1.0.1/wntrfr/epanet/Linux/
--rw-rw-rw-   0        0        0   385808 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1/wntrfr/epanet/Linux/libepanet22_amd64.so
--rw-rw-rw-   0        0        0   505379 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1/wntrfr/epanet/Linux/libepanet2_amd64.so
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.630613 wntrfr-1.1.0.1/wntrfr/epanet/Windows/
--rw-rw-rw-   0        0        0     8758 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.bas
--rw-rw-rw-   0        0        0     4106 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.def
--rw-rw-rw-   0        0        0   217088 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.dll
--rw-rw-rw-   0        0        0    22614 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.lib
--rw-rw-rw-   0        0        0     9910 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.pas
--rw-rw-rw-   0        0        0   349184 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet22_amd64.dll
--rw-rw-rw-   0        0        0   285696 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet22_win32.dll
--rw-rw-rw-   0        0        0   315904 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2_amd64.dll
--rw-rw-rw-   0        0        0      249 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/epanet/__init__.py
--rw-rw-rw-   0        0        0     7865 2024-04-12 18:43:46.000000 wntrfr-1.1.0.1/wntrfr/epanet/exceptions.py
--rw-rw-rw-   0        0        0   152416 2024-03-28 23:47:01.000000 wntrfr-1.1.0.1/wntrfr/epanet/io.py
--rw-rw-rw-   0        0        0    27944 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/epanet/toolkit.py
--rw-rw-rw-   0        0        0    46112 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/epanet/util.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.632636 wntrfr-1.1.0.1/wntrfr/gis/
--rw-rw-rw-   0        0        0      271 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/gis/__init__.py
--rw-rw-rw-   0        0        0    12741 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/gis/geospatial.py
--rw-rw-rw-   0        0        0    19214 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/gis/network.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.635629 wntrfr-1.1.0.1/wntrfr/graphics/
--rw-rw-rw-   0        0        0      394 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/graphics/__init__.py
--rw-rw-rw-   0        0        0     1779 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1/wntrfr/graphics/color.py
--rw-rw-rw-   0        0        0     6745 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/graphics/curve.py
--rw-rw-rw-   0        0        0     3543 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/graphics/layer.py
--rw-rw-rw-   0        0        0    31670 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/graphics/network.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.639627 wntrfr-1.1.0.1/wntrfr/metrics/
--rw-rw-rw-   0        0        0      939 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/__init__.py
--rw-rw-rw-   0        0        0    15315 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/economic.py
--rw-rw-rw-   0        0        0    15710 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/hydraulic.py
--rw-rw-rw-   0        0        0     2761 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/misc.py
--rw-rw-rw-   0        0        0    16807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/topographic.py
--rw-rw-rw-   0        0        0     5236 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/metrics/water_security.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.641757 wntrfr-1.1.0.1/wntrfr/morph/
--rw-rw-rw-   0        0        0      573 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/morph/__init__.py
--rw-rw-rw-   0        0        0    12684 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/morph/link.py
--rw-rw-rw-   0        0        0    11032 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/morph/node.py
--rw-rw-rw-   0        0        0    16912 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/morph/skel.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.647756 wntrfr-1.1.0.1/wntrfr/network/
--rw-rw-rw-   0        0        0      874 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/__init__.py
--rw-rw-rw-   0        0        0    25793 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/base.py
--rw-rw-rw-   0        0        0    83473 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/controls.py
--rw-rw-rw-   0        0        0    83834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/elements.py
--rw-rw-rw-   0        0        0    24487 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/io.py
--rw-rw-rw-   0        0        0     2311 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/layer.py
--rw-rw-rw-   0        0        0    88834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/model.py
--rw-rw-rw-   0        0        0    31476 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/network/options.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.648754 wntrfr-1.1.0.1/wntrfr/scenario/
--rw-rw-rw-   0        0        0      222 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/scenario/__init__.py
--rw-rw-rw-   0        0        0     7818 2024-04-13 00:44:11.000000 wntrfr-1.1.0.1/wntrfr/scenario/earthquake.py
--rw-rw-rw-   0        0        0     3706 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/scenario/fragility_curve.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.652281 wntrfr-1.1.0.1/wntrfr/sim/
--rw-rw-rw-   0        0        0      329 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.657280 wntrfr-1.1.0.1/wntrfr/sim/aml/
--rw-rw-rw-   0        0        0      254 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/__init__.py
--rw-rw-rw-   0        0        0    16045 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/aml.py
--rw-rw-rw-   0        0        0    14245 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.cpp
--rw-rw-rw-   0        0        0     3707 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.hpp
--rw-rw-rw-   0        0        0      938 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.i
--rw-rw-rw-   0        0        0     2121 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.py
--rw-rw-rw-   0        0        0   359034 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator_wrap.cpp
--rw-rw-rw-   0        0        0    37825 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/expr.py
--rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/aml/numpy.i
--rw-rw-rw-   0        0        0    76807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/core.py
--rw-rw-rw-   0        0        0     5097 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/epanet.py
--rw-rw-rw-   0        0        0    14911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/hydraulics.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.660970 wntrfr-1.1.0.1/wntrfr/sim/models/
--rw-rw-rw-   0        0        0      108 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/__init__.py
--rw-rw-rw-   0        0        0      911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/constants.py
--rw-rw-rw-   0        0        0    29038 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/constraint.py
--rw-rw-rw-   0        0        0    17287 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/param.py
--rw-rw-rw-   0        0        0      938 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/utils.py
--rw-rw-rw-   0        0        0     2412 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/models/var.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.663997 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/
--rw-rw-rw-   0        0        0      148 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/__init__.py
--rw-rw-rw-   0        0        0     1647 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.cpp
--rw-rw-rw-   0        0        0      332 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.hpp
--rw-rw-rw-   0        0        0      634 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.i
--rw-rw-rw-   0        0        0     2129 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.py
--rw-rw-rw-   0        0        0   154827 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp
--rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1/wntrfr/sim/network_isolation/numpy.i
--rw-rw-rw-   0        0        0      415 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1/wntrfr/sim/results.py
--rw-rw-rw-   0        0        0     7259 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/sim/solvers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.666997 wntrfr-1.1.0.1/wntrfr/utils/
--rw-rw-rw-   0        0        0       93 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1/wntrfr/utils/__init__.py
--rw-rw-rw-   0        0        0     1058 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1/wntrfr/utils/doc_inheritor.py
--rw-rw-rw-   0        0        0     1167 2024-04-13 00:45:48.000000 wntrfr-1.1.0.1/wntrfr/utils/logger.py
--rw-rw-rw-   0        0        0     1876 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1/wntrfr/utils/ordered_set.py
--rw-rw-rw-   0        0        0      972 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1/wntrfr/utils/polynomial_interpolation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 01:02:30.618292 wntrfr-1.1.0.1/wntrfr.egg-info/
--rw-rw-rw-   0        0        0     4705 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 01:02:28.000000 wntrfr-1.1.0.1/wntrfr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/
+-rw-rw-rw-   0        0        0     4787 2024-04-12 18:43:38.000000 wntrfr-1.1.0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      343 2024-04-18 00:54:57.000000 wntrfr-1.1.0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4707 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.1/README.md
+-rw-rw-rw-   0        0        0      210 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 00:30:47.996694 wntrfr-1.1.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4384 2024-04-13 00:40:09.000000 wntrfr-1.1.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.907229 wntrfr-1.1.0.1.1/wntrfr/
+-rw-rw-rw-   0        0        0      572 2024-04-23 00:30:40.000000 wntrfr-1.1.0.1.1/wntrfr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.914737 wntrfr-1.1.0.1.1/wntrfr/epanet/
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.915732 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/
+-rw-rw-rw-   0        0        0   302216 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet.dylib
+-rw-rw-rw-   0        0        0   325828 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet22.dylib
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.917738 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/
+-rw-rw-rw-   0        0        0   385808 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet22_amd64.so
+-rw-rw-rw-   0        0        0   505379 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet2_amd64.so
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.923747 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/
+-rw-rw-rw-   0        0        0     8758 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.bas
+-rw-rw-rw-   0        0        0     4106 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.def
+-rw-rw-rw-   0        0        0   217088 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.dll
+-rw-rw-rw-   0        0        0    22614 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.lib
+-rw-rw-rw-   0        0        0     9910 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.pas
+-rw-rw-rw-   0        0        0   349184 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_amd64.dll
+-rw-rw-rw-   0        0        0   285696 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_win32.dll
+-rw-rw-rw-   0        0        0   315904 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2_amd64.dll
+-rw-rw-rw-   0        0        0      249 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/__init__.py
+-rw-rw-rw-   0        0        0     7865 2024-04-12 18:43:46.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/exceptions.py
+-rw-rw-rw-   0        0        0   152460 2024-04-23 00:30:11.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/io.py
+-rw-rw-rw-   0        0        0    27944 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/toolkit.py
+-rw-rw-rw-   0        0        0    46112 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/util.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.924749 wntrfr-1.1.0.1.1/wntrfr/gis/
+-rw-rw-rw-   0        0        0      271 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/__init__.py
+-rw-rw-rw-   0        0        0    12741 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/geospatial.py
+-rw-rw-rw-   0        0        0    19214 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/network.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.927744 wntrfr-1.1.0.1.1/wntrfr/graphics/
+-rw-rw-rw-   0        0        0      394 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/__init__.py
+-rw-rw-rw-   0        0        0     1779 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/color.py
+-rw-rw-rw-   0        0        0     6745 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/curve.py
+-rw-rw-rw-   0        0        0     3543 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/layer.py
+-rw-rw-rw-   0        0        0    31670 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/network.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.932167 wntrfr-1.1.0.1.1/wntrfr/metrics/
+-rw-rw-rw-   0        0        0      939 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/__init__.py
+-rw-rw-rw-   0        0        0    15315 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/economic.py
+-rw-rw-rw-   0        0        0    15710 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/hydraulic.py
+-rw-rw-rw-   0        0        0     2761 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/misc.py
+-rw-rw-rw-   0        0        0    16807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/topographic.py
+-rw-rw-rw-   0        0        0     5236 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/water_security.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.937692 wntrfr-1.1.0.1.1/wntrfr/morph/
+-rw-rw-rw-   0        0        0      573 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/__init__.py
+-rw-rw-rw-   0        0        0    12684 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/link.py
+-rw-rw-rw-   0        0        0    11032 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/node.py
+-rw-rw-rw-   0        0        0    16912 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/skel.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.946694 wntrfr-1.1.0.1.1/wntrfr/network/
+-rw-rw-rw-   0        0        0      874 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/__init__.py
+-rw-rw-rw-   0        0        0    25793 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/base.py
+-rw-rw-rw-   0        0        0    83473 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/controls.py
+-rw-rw-rw-   0        0        0    83834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/elements.py
+-rw-rw-rw-   0        0        0    24487 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/io.py
+-rw-rw-rw-   0        0        0     2311 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/layer.py
+-rw-rw-rw-   0        0        0    88834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/model.py
+-rw-rw-rw-   0        0        0    31476 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/options.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.951691 wntrfr-1.1.0.1.1/wntrfr/scenario/
+-rw-rw-rw-   0        0        0      222 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/__init__.py
+-rw-rw-rw-   0        0        0     7818 2024-04-13 00:44:11.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/earthquake.py
+-rw-rw-rw-   0        0        0     3706 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/fragility_curve.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.960690 wntrfr-1.1.0.1.1/wntrfr/sim/
+-rw-rw-rw-   0        0        0      329 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.972690 wntrfr-1.1.0.1.1/wntrfr/sim/aml/
+-rw-rw-rw-   0        0        0      254 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/__init__.py
+-rw-rw-rw-   0        0        0    16045 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/aml.py
+-rw-rw-rw-   0        0        0    14245 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.cpp
+-rw-rw-rw-   0        0        0     3707 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.hpp
+-rw-rw-rw-   0        0        0      938 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.i
+-rw-rw-rw-   0        0        0     2121 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.py
+-rw-rw-rw-   0        0        0   359034 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator_wrap.cpp
+-rw-rw-rw-   0        0        0    37825 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/expr.py
+-rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/numpy.i
+-rw-rw-rw-   0        0        0    76807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/core.py
+-rw-rw-rw-   0        0        0     5097 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/epanet.py
+-rw-rw-rw-   0        0        0    14911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/hydraulics.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.980690 wntrfr-1.1.0.1.1/wntrfr/sim/models/
+-rw-rw-rw-   0        0        0      108 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/__init__.py
+-rw-rw-rw-   0        0        0      911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/constants.py
+-rw-rw-rw-   0        0        0    29038 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/constraint.py
+-rw-rw-rw-   0        0        0    17287 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/param.py
+-rw-rw-rw-   0        0        0      938 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/utils.py
+-rw-rw-rw-   0        0        0     2412 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/var.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.985690 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/
+-rw-rw-rw-   0        0        0      148 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/__init__.py
+-rw-rw-rw-   0        0        0     1647 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.cpp
+-rw-rw-rw-   0        0        0      332 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.hpp
+-rw-rw-rw-   0        0        0      634 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.i
+-rw-rw-rw-   0        0        0     2129 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.py
+-rw-rw-rw-   0        0        0   154827 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp
+-rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/numpy.i
+-rw-rw-rw-   0        0        0      415 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/results.py
+-rw-rw-rw-   0        0        0     7259 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/solvers.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/wntrfr/utils/
+-rw-rw-rw-   0        0        0       93 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/utils/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/doc_inheritor.py
+-rw-rw-rw-   0        0        0     1167 2024-04-13 00:45:48.000000 wntrfr-1.1.0.1.1/wntrfr/utils/logger.py
+-rw-rw-rw-   0        0        0     1876 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/ordered_set.py
+-rw-rw-rw-   0        0        0      972 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/polynomial_interpolation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.910229 wntrfr-1.1.0.1.1/wntrfr.egg-info/
+-rw-rw-rw-   0        0        0     4707 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2787 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 00:30:27.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/top_level.txt
```

### Comparing `wntrfr-1.1.0.1/LICENSE.md` & `wntrfr-1.1.0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/PKG-INFO` & `wntrfr-1.1.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wntrfr
-Version: 1.1.0.1
+Version: 1.1.0.1.1
 Summary: Water Network Tool for Resilience
 Home-page: https://github.com/snaeimi/WNTR
 Author: WNTR Developers
 Maintainer-email: snaeimi@udel.edu
 License: Revised BSD
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `wntrfr-1.1.0.1/README.md` & `wntrfr-1.1.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/setup.py` & `wntrfr-1.1.0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/__init__.py` & `wntrfr-1.1.0.1.1/wntrfr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from wntrfr import metrics
 from wntrfr import sim
 from wntrfr import scenario
 from wntrfr import graphics
 from wntrfr import gis
 from wntrfr import utils
 
-__version__ = '1.1.0.1'
+__version__ = '1.1.0.1.1'
 
 __copyright__ = """Copyright 2023 National Technology & Engineering 
 Solutions of Sandia, LLC (NTESS). Under the terms of Contract DE-NA0003525 
 with NTESS, the U.S. Government retains certain rights in this software."""
 
 __license__ = "Revised BSD License"
```

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Darwin/libepanet.dylib` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet.dylib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Darwin/libepanet22.dylib` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet22.dylib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Linux/libepanet22_amd64.so` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet22_amd64.so`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Linux/libepanet2_amd64.so` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet2_amd64.so`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.bas` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.bas`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.def` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.def`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.dll` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.lib` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.lib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2.pas` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.pas`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet22_amd64.dll` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_amd64.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet22_win32.dll` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_win32.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/Windows/epanet2_amd64.dll` & `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2_amd64.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/exceptions.py` & `wntrfr-1.1.0.1.1/wntrfr/epanet/exceptions.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/io.py` & `wntrfr-1.1.0.1.1/wntrfr/epanet/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The wntr.epanet.io module contains methods for reading/writing EPANET input and output files.
+The wntrfr.epanet.io module contains methods for reading/writing EPANET input and output files.
 """
 from __future__ import absolute_import
 
 import datetime
 import difflib
 import io
 import logging
@@ -13,24 +13,24 @@
 import warnings
 from collections import OrderedDict
 
 import numpy as np
 import pandas as pd
 import six
 import wntr
-import wntr.network
-from wntr.network.base import Link
-from wntr.network.controls import (AndCondition, Comparison, Control,
+import wntrfr.network
+from wntrfr.network.base import Link
+from wntrfr.network.controls import (AndCondition, Comparison, Control,
                                    ControlAction, OrCondition, Rule,
                                    SimTimeCondition, TimeOfDayCondition,
                                    ValueCondition, _ControlType)
-from wntr.network.elements import Junction, Pipe, Pump, Reservoir, Tank, Valve
-from wntr.network.model import (Curve, Demands, LinkStatus, Pattern, Source,
+from wntrfr.network.elements import Junction, Pipe, Pump, Reservoir, Tank, Valve
+from wntrfr.network.model import (Curve, Demands, LinkStatus, Pattern, Source,
                                 WaterNetworkModel)
-from wntr.network.options import Options
+from wntrfr.network.options import Options
 
 from .util import (EN, FlowUnits, HydParam, MassUnits, MixType, PressureUnits,
                    QualParam, QualType, ResultType, StatisticsType, from_si,
                    to_si)
 
 #from .time_utils import run_lineprofile
 sys_default_enc = sys.getdefaultencoding()
@@ -402,15 +402,15 @@
 
     def write(self, filename, wn, units=None, version=2.2, force_coordinates=False):
         """
         Write a water network model into an EPANET INP file.
 
         .. note::
 
-            Please note that by default, an EPANET 2.2 formatted file is written by WNTR. An INP file
+            Please note that by default, an EPANET 2.2 formatted file is written by wntrfr. An INP file
             with version 2.2 options *will not* work with EPANET 2.0 (neither command line nor GUI). 
             By default, WNTR will use the EPANET 2.2 toolkit.
         
 
         Parameters
         ----------
         filename : str
@@ -493,15 +493,15 @@
                 continue
             lines.append(line)
         self.wn.title = lines
 
     def _write_title(self, f, wn):
         if wn.name is not None:
             f.write('; Filename: {0}\n'.format(wn.name).encode(sys_default_enc))
-            f.write('; WNTR: {}\n; Created: {:%Y-%m-%d %H:%M:%S}\n'.format(wntr.__version__, datetime.datetime.now()).encode(sys_default_enc))
+            f.write('; WNTR: {}\n; Created: {:%Y-%m-%d %H:%M:%S}\n'.format(wntrfr.__version__, datetime.datetime.now()).encode(sys_default_enc))
         f.write('[TITLE]\n'.encode(sys_default_enc))
         if hasattr(wn, 'title'):
             for line in wn.title:
                 f.write('{}\n'.format(line).encode(sys_default_enc))
         f.write('\n'.encode(sys_default_enc))
 
     def _read_junctions(self):
@@ -1095,15 +1095,15 @@
             if (current[1].upper() == 'OPEN' or
                     current[1].upper() == 'CLOSED' or
                     current[1].upper() == 'ACTIVE'):
                 new_status = LinkStatus[current[1].upper()]
                 link.initial_status = new_status
                 link._user_status = new_status
             else:
-                if isinstance(link, wntr.network.Valve):
+                if isinstance(link, wntrfr.network.Valve):
                     new_status = LinkStatus.Active
                     valve_type = link.valve_type
                     if valve_type in ['PRV', 'PSV', 'PBV']:
                         setting = to_si(self.flow_units, float(current[1]), HydParam.Pressure)
                     elif valve_type == 'FCV':
                         setting = to_si(self.flow_units, float(current[1]), HydParam.Flow)
                     elif valve_type == 'TCV':
@@ -2413,17 +2413,17 @@
                     value = to_si(self.inp_units, value, HydParam.HydraulicHead)
                 elif attr.lower() in ['flow']:
                     value = to_si(self.inp_units, value, HydParam.Flow)
                 elif attr.lower() in ['pressure']:
                     value = to_si(self.inp_units, value, HydParam.Pressure)
                 elif attr.lower() in ['setting']:
                     link = model.get_link(words[2])
-                    if isinstance(link, wntr.network.Pump):
+                    if isinstance(link, wntrfr.network.Pump):
                         value = value
-                    elif isinstance(link, wntr.network.Valve):
+                    elif isinstance(link, wntrfr.network.Valve):
                         if link.valve_type.upper() in ['PRV', 'PBV', 'PSV']:
                             value = to_si(self.inp_units, value, HydParam.Pressure)
                         elif link.valve_type.upper() in ['FCV']:
                             value = to_si(self.inp_units, value, HydParam.Flow)
                 if words[1].upper() in ['NODE', 'JUNCTION', 'RESERVOIR', 'TANK']:
                     condition = ValueCondition(model.get_node(words[2]), words[3].lower(), words[4].lower(), value)
                 elif words[1].upper() in ['LINK', 'PIPE', 'PUMP', 'VALVE']:
@@ -2557,15 +2557,15 @@
         self.report_start = None
         self.report_step = None
         self.duration = None
         self.chemical = None
         self.chem_units = None
         self.inp_file = None
         self.report_file = None
-        self.results = wntr.sim.SimulationResults()
+        self.results = wntrfr.sim.SimulationResults()
         if result_types is None:
             self.items = [ member for name, member in ResultType.__members__.items() ]
         else:
             self.items = result_types
         self.create_network = network
         self.keep_energy = energy
         self.keep_statistics = statistics
@@ -2645,15 +2645,15 @@
             if the simulation does not converge.  Default = False.
 
         Returns
         -------
         object
             returns a WaterNetworkResults object    
         """
-        self.results = wntr.sim.SimulationResults()
+        self.results = wntrfr.sim.SimulationResults()
         
         logger.debug('Read binary EPANET data from %s',filename)
         dt_str = 'u1'  #.format(self.idlen)
         with open(filename, 'rb') as fin:
             ftype = self.ftype
             idlen = self.idlen
             logger.debug('... read prolog information ...')
@@ -2815,15 +2815,15 @@
                     logger.error('Simulation did not converge at time ' + self._get_time(t) + '.')
                     raise RuntimeError('Simulation did not converge at time ' + self._get_time(t) + '.')
                 else:
                     data = data[0:N*(4*nnodes+8*nlinks)]
                     data = np.reshape(data, (N, (4*nnodes+8*nlinks)))
                     reporttimes = reporttimes[0:N]
                     warnings.warn('Simulation did not converge at time ' + self._get_time(t) + '.')
-                    self.results.error_code = wntr.sim.results.ResultsStatus.error
+                    self.results.error_code = wntrfr.sim.results.ResultsStatus.error
             else:
                 data = np.reshape(data, (nrptsteps, (4*nnodes+8*nlinks)))
                 self.results.error_code = None
 
             df = pd.DataFrame(data.transpose(), index =index, columns = reporttimes)
             df = df.transpose()
             
@@ -3054,15 +3054,15 @@
     return True
 
 
 def _clean_line(wn, sec, line):  # pragma: no cover
     """
     Parameters
     ----------
-    wn: wntr.network.WaterNetworkModel
+    wn: wntrfr.network.WaterNetworkModel
     sec: str
     line: list of str
 
     Returns
     -------
     new_list: list of str
 	
@@ -3081,15 +3081,15 @@
 
 
 def _read_control_line(line, wn, flow_units, control_name):
     """
     Parameters
     ----------
     line: str
-    wn: wntr.network.WaterNetworkModel
+    wn: wntrfr.network.WaterNetworkModel
     flow_units: str
     control_name: str
 
     Returns
     -------
     control_obj: Control
 	
@@ -3106,30 +3106,30 @@
     current[1] = link_name # don't capitalize the link name
 
     # Create the control action object
 
     status = current[2].upper()
     if status == 'OPEN' or status == 'OPENED' or status == 'CLOSED' or status == 'ACTIVE':
         setting = LinkStatus[status].value
-        action_obj = wntr.network.ControlAction(link, 'status', setting)
+        action_obj = wntrfr.network.ControlAction(link, 'status', setting)
     else:
-        if isinstance(link, wntr.network.Pump):
-            action_obj = wntr.network.ControlAction(link, 'base_speed', float(current[2]))
-        elif isinstance(link, wntr.network.Valve):
+        if isinstance(link, wntrfr.network.Pump):
+            action_obj = wntrfr.network.ControlAction(link, 'base_speed', float(current[2]))
+        elif isinstance(link, wntrfr.network.Valve):
             if link.valve_type == 'PRV' or link.valve_type == 'PSV' or link.valve_type == 'PBV':
                 setting = to_si(flow_units, float(current[2]), HydParam.Pressure)
             elif link.valve_type == 'FCV':
                 setting = to_si(flow_units, float(current[2]), HydParam.Flow)
             elif link.valve_type == 'TCV':
                 setting = float(current[2])
             elif link.valve_type == 'GPV':
                 setting = current[2]
             else:
                 raise ValueError('Unrecognized valve type {0} while parsing control {1}'.format(link.valve_type, line))
-            action_obj = wntr.network.ControlAction(link, 'setting', setting)
+            action_obj = wntrfr.network.ControlAction(link, 'setting', setting)
         else:
             raise RuntimeError(('Links of type {0} can only have controls that change\n'.format(type(link))+
                                 'the link status. Control: {0}'.format(line)))
 
     # Create the control object
     #control_count += 1
     #control_name = 'control '+str(control_count)
```

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/toolkit.py` & `wntrfr-1.1.0.1.1/wntrfr/epanet/toolkit.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/epanet/util.py` & `wntrfr-1.1.0.1.1/wntrfr/epanet/util.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/gis/geospatial.py` & `wntrfr-1.1.0.1.1/wntrfr/gis/geospatial.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/gis/network.py` & `wntrfr-1.1.0.1.1/wntrfr/gis/network.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/graphics/color.py` & `wntrfr-1.1.0.1.1/wntrfr/graphics/color.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/graphics/curve.py` & `wntrfr-1.1.0.1.1/wntrfr/graphics/curve.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/graphics/layer.py` & `wntrfr-1.1.0.1.1/wntrfr/graphics/layer.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/graphics/network.py` & `wntrfr-1.1.0.1.1/wntrfr/graphics/network.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/__init__.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/economic.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/economic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/hydraulic.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/hydraulic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/misc.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/misc.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/topographic.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/topographic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/metrics/water_security.py` & `wntrfr-1.1.0.1.1/wntrfr/metrics/water_security.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/morph/__init__.py` & `wntrfr-1.1.0.1.1/wntrfr/morph/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/morph/link.py` & `wntrfr-1.1.0.1.1/wntrfr/morph/link.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/morph/node.py` & `wntrfr-1.1.0.1.1/wntrfr/morph/node.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/morph/skel.py` & `wntrfr-1.1.0.1.1/wntrfr/morph/skel.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/__init__.py` & `wntrfr-1.1.0.1.1/wntrfr/network/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/base.py` & `wntrfr-1.1.0.1.1/wntrfr/network/base.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/controls.py` & `wntrfr-1.1.0.1.1/wntrfr/network/controls.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/elements.py` & `wntrfr-1.1.0.1.1/wntrfr/network/elements.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/io.py` & `wntrfr-1.1.0.1.1/wntrfr/network/io.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/layer.py` & `wntrfr-1.1.0.1.1/wntrfr/network/layer.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/model.py` & `wntrfr-1.1.0.1.1/wntrfr/network/model.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/network/options.py` & `wntrfr-1.1.0.1.1/wntrfr/network/options.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/scenario/earthquake.py` & `wntrfr-1.1.0.1.1/wntrfr/scenario/earthquake.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/scenario/fragility_curve.py` & `wntrfr-1.1.0.1.1/wntrfr/scenario/fragility_curve.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/aml.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/aml.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.cpp` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.hpp` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.hpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.i` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/evaluator_wrap.cpp` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator_wrap.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/expr.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/expr.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/aml/numpy.i` & `wntrfr-1.1.0.1.1/wntrfr/sim/aml/numpy.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/core.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/core.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/epanet.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/epanet.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/hydraulics.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/hydraulics.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/models/constants.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/models/constants.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/models/constraint.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/models/constraint.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/models/param.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/models/param.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/models/utils.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/models/utils.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/models/var.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/models/var.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.cpp` & `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.i` & `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp` & `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/network_isolation/numpy.i` & `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/numpy.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/sim/solvers.py` & `wntrfr-1.1.0.1.1/wntrfr/sim/solvers.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/utils/doc_inheritor.py` & `wntrfr-1.1.0.1.1/wntrfr/utils/doc_inheritor.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/utils/logger.py` & `wntrfr-1.1.0.1.1/wntrfr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/utils/ordered_set.py` & `wntrfr-1.1.0.1.1/wntrfr/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr/utils/polynomial_interpolation.py` & `wntrfr-1.1.0.1.1/wntrfr/utils/polynomial_interpolation.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1/wntrfr.egg-info/PKG-INFO` & `wntrfr-1.1.0.1.1/wntrfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wntrfr
-Version: 1.1.0.1
+Version: 1.1.0.1.1
 Summary: Water Network Tool for Resilience
 Home-page: https://github.com/snaeimi/WNTR
 Author: WNTR Developers
 Maintainer-email: snaeimi@udel.edu
 License: Revised BSD
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `wntrfr-1.1.0.1/wntrfr.egg-info/SOURCES.txt` & `wntrfr-1.1.0.1.1/wntrfr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 ./wntrfr/sim/aml/evaluator.cpp
 ./wntrfr/sim/aml/evaluator_wrap.cpp
 ./wntrfr/sim/network_isolation/network_isolation.cpp
 ./wntrfr/sim/network_isolation/network_isolation_wrap.cpp
 wntrfr/__init__.py
 wntrfr.egg-info/PKG-INFO
```

