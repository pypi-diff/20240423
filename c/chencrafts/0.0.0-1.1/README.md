# Comparing `tmp/chencrafts-0.0.0.tar.gz` & `tmp/chencrafts-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chencrafts-0.0.0.tar", last modified: Tue Apr 23 17:37:21 2024, max compression
+gzip compressed data, was "chencrafts-1.1.tar", last modified: Thu Apr 18 06:13:08 2024, max compression
```

## Comparing `chencrafts-0.0.0.tar` & `chencrafts-1.1.tar`

### file list

```diff
@@ -1,76 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.219647 chencrafts-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.203647 chencrafts-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.207647 chencrafts-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-23 17:37:16.000000 chencrafts-0.0.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 17:37:16.000000 chencrafts-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-23 17:37:16.000000 chencrafts-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 17:37:16.000000 chencrafts-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-23 17:37:21.219647 chencrafts-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-23 17:37:16.000000 chencrafts-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 17:37:16.000000 chencrafts-0.0.0/_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.207647 chencrafts-0.0.0/chencrafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.211647 chencrafts-0.0.0/chencrafts/bsqubits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.211647 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30405 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/cat_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/batched_custom_sweeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/cat_ideal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/cat_real.py
--rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/derive_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/error_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/pulse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/bsqubits/systems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/chencrafts/cqed/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/block_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/crit_photon_num.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/crit_photon_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/flexible_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/mode_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/pulses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/qt_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/scq_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/spec_poly_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/special_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/cqed/symbolic_bosons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/chencrafts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/projects/fluxonium_tunable_coupler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/projects/protomon_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/projects/protomon_full_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/chencrafts/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/gadgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-23 17:37:16.000000 chencrafts-0.0.0/chencrafts/toolbox/useless.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/chencrafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:37:21.000000 chencrafts-0.0.0/chencrafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 17:37:16.000000 chencrafts-0.0.0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 17:37:16.000000 chencrafts-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 17:37:16.000000 chencrafts-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:37:21.219647 chencrafts-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:37:21.215647 chencrafts-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-23 17:37:16.000000 chencrafts-0.0.0/tests/test_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.612922 chencrafts-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-18 06:12:52.000000 chencrafts-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 06:12:52.000000 chencrafts-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-18 06:13:08.612922 chencrafts-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 06:12:52.000000 chencrafts-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.600922 chencrafts-1.1/chencrafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.604922 chencrafts-1.1/chencrafts/bsqubits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.604922 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30405 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/cat_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/batched_custom_sweeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/cat_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/cat_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/derive_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/error_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/pulse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/systems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/cqed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/block_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/crit_photon_num.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/cqed/custom_sweeps/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/crit_photon_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/flexible_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/mode_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/pulses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/qt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/scq_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/spec_poly_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/special_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/symbolic_bosons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/fluxonium_tunable_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/protomon_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/protomon_full_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/gadgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/useless.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.612922 chencrafts-1.1/chencrafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 06:12:52.000000 chencrafts-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 06:12:52.000000 chencrafts-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:13:08.612922 chencrafts-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 06:12:52.000000 chencrafts-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-18 06:12:52.000000 chencrafts-1.1/tests/test_optimization.py
```

### Comparing `chencrafts-0.0.0/LICENSE` & `chencrafts-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/PKG-INFO` & `chencrafts-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 0.0.0
-Summary: A personal toolbox for superconducting qubits and quantum mechanics.
-Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
+Version: 1.1
+Summary: CHEN CRAFTS, my personal toolbox!
+Home-page: https://github.com/Harrinive/chencrafts
+Author: Danyang Chen
+Author-email: DanyangChen2026@u.northwestern.edu
 License: MIT
-Project-URL: Homepage, https://github.com/Harrinive/chencrafts
-Project-URL: Repository, https://github.com/Harrinive/chencrafts
 Keywords: personal toolbox,superconducting qubits,quantum mechanics
+Platform: Linux
+Platform: Mac OSX
+Platform: Unix
+Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
 Requires-Dist: matplotlib
+Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pandas
 Requires-Dist: tqdm
+Requires-Dist: pandas
 Requires-Dist: dill
 Requires-Dist: pathos
 Requires-Dist: scqubits
 Requires-Dist: IPython
 Provides-Extra: cqed
-Requires-Dist: torch>=1.7; extra == "cqed"
+Requires-Dist: torch; extra == "cqed"
 Requires-Dist: multiprocess; extra == "cqed"
 Provides-Extra: bsqubits
-Requires-Dist: networkx>=2.4; extra == "bsqubits"
+Requires-Dist: networkx; extra == "bsqubits"
 
-CHENCRAFTS, Danyang's personal toolbox!
-=================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-0.0.0/README.md` & `chencrafts-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CHENCRAFTS, Danyang's personal toolbox!
+CHEN CRAFTS, my personal toolbox!
 =================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-0.0.0/_setup.py` & `chencrafts-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/__init__.py` & `chencrafts-1.1/chencrafts/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/__init__.py` & `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/cat_tree.py` & `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/cat_tree.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/edge.py` & `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/edge.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/graph.py` & `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/graph.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/QEC_graph/node.py` & `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/node.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/__init__.py` & `chencrafts-1.1/chencrafts/bsqubits/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/batched_custom_sweeps.py` & `chencrafts-1.1/chencrafts/bsqubits/batched_custom_sweeps.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/cat_ideal.py` & `chencrafts-1.1/chencrafts/bsqubits/cat_ideal.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/cat_real.py` & `chencrafts-1.1/chencrafts/bsqubits/cat_real.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/derive_var.py` & `chencrafts-1.1/chencrafts/bsqubits/derive_var.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/error_rates.py` & `chencrafts-1.1/chencrafts/bsqubits/error_rates.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/pulse_utils.py` & `chencrafts-1.1/chencrafts/bsqubits/pulse_utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/bsqubits/systems.py` & `chencrafts-1.1/chencrafts/bsqubits/systems.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/__init__.py` & `chencrafts-1.1/chencrafts/cqed/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/block_diag.py` & `chencrafts-1.1/chencrafts/cqed/block_diag.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/crit_photon_num.py` & `chencrafts-1.1/chencrafts/cqed/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/crit_photon_num.py` & `chencrafts-1.1/chencrafts/cqed/custom_sweeps/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/decoherence.py` & `chencrafts-1.1/chencrafts/cqed/custom_sweeps/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/custom_sweeps/utils.py` & `chencrafts-1.1/chencrafts/cqed/custom_sweeps/utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/decoherence.py` & `chencrafts-1.1/chencrafts/cqed/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/flexible_sweep.py` & `chencrafts-1.1/chencrafts/cqed/flexible_sweep.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/mode_assignment.py` & `chencrafts-1.1/chencrafts/cqed/mode_assignment.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/pulses.py` & `chencrafts-1.1/chencrafts/cqed/pulses.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/qt_helper.py` & `chencrafts-1.1/chencrafts/cqed/qt_helper.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/scq_helper.py` & `chencrafts-1.1/chencrafts/cqed/scq_helper.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/spec_poly_fit.py` & `chencrafts-1.1/chencrafts/cqed/spec_poly_fit.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/special_states.py` & `chencrafts-1.1/chencrafts/cqed/special_states.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/cqed/symbolic_bosons.py` & `chencrafts-1.1/chencrafts/cqed/symbolic_bosons.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/projects/fluxonium_tunable_coupler.py` & `chencrafts-1.1/chencrafts/projects/fluxonium_tunable_coupler.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/projects/protomon_disorder.py` & `chencrafts-1.1/chencrafts/projects/protomon_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/projects/protomon_full_disorder.py` & `chencrafts-1.1/chencrafts/projects/protomon_full_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/settings.py` & `chencrafts-1.1/chencrafts/settings.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/__init__.py` & `chencrafts-1.1/chencrafts/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/data_processing.py` & `chencrafts-1.1/chencrafts/toolbox/data_processing.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/gadgets.py` & `chencrafts-1.1/chencrafts/toolbox/gadgets.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/optimize.py` & `chencrafts-1.1/chencrafts/toolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/plot.py` & `chencrafts-1.1/chencrafts/toolbox/plot.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/save.py` & `chencrafts-1.1/chencrafts/toolbox/save.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts/toolbox/useless.py` & `chencrafts-1.1/chencrafts/toolbox/useless.py`

 * *Files identical despite different names*

### Comparing `chencrafts-0.0.0/chencrafts.egg-info/PKG-INFO` & `chencrafts-1.1/chencrafts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 0.0.0
-Summary: A personal toolbox for superconducting qubits and quantum mechanics.
-Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
+Version: 1.1
+Summary: CHEN CRAFTS, my personal toolbox!
+Home-page: https://github.com/Harrinive/chencrafts
+Author: Danyang Chen
+Author-email: DanyangChen2026@u.northwestern.edu
 License: MIT
-Project-URL: Homepage, https://github.com/Harrinive/chencrafts
-Project-URL: Repository, https://github.com/Harrinive/chencrafts
 Keywords: personal toolbox,superconducting qubits,quantum mechanics
+Platform: Linux
+Platform: Mac OSX
+Platform: Unix
+Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
 Requires-Dist: matplotlib
+Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pandas
 Requires-Dist: tqdm
+Requires-Dist: pandas
 Requires-Dist: dill
 Requires-Dist: pathos
 Requires-Dist: scqubits
 Requires-Dist: IPython
 Provides-Extra: cqed
-Requires-Dist: torch>=1.7; extra == "cqed"
+Requires-Dist: torch; extra == "cqed"
 Requires-Dist: multiprocess; extra == "cqed"
 Provides-Extra: bsqubits
-Requires-Dist: networkx>=2.4; extra == "bsqubits"
+Requires-Dist: networkx; extra == "bsqubits"
 
-CHENCRAFTS, Danyang's personal toolbox!
-=================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-0.0.0/chencrafts.egg-info/SOURCES.txt` & `chencrafts-1.1/chencrafts.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-.gitignore
 LICENSE
 MANIFEST.in
 README.md
-_setup.py
-meta.yaml
 pyproject.toml
 requirements.txt
-.github/workflows/publish_to_pypi.yml
+setup.py
 chencrafts/__init__.py
 chencrafts/py.typed
-chencrafts/pyrightconfig.json
 chencrafts/settings.py
 chencrafts/version.py
 chencrafts.egg-info/PKG-INFO
 chencrafts.egg-info/SOURCES.txt
 chencrafts.egg-info/dependency_links.txt
+chencrafts.egg-info/not-zip-safe
 chencrafts.egg-info/requires.txt
 chencrafts.egg-info/top_level.txt
 chencrafts/bsqubits/__init__.py
 chencrafts/bsqubits/batched_custom_sweeps.py
 chencrafts/bsqubits/cat_ideal.py
 chencrafts/bsqubits/cat_real.py
 chencrafts/bsqubits/derive_var.py
```

### Comparing `chencrafts-0.0.0/tests/test_optimization.py` & `chencrafts-1.1/tests/test_optimization.py`

 * *Files identical despite different names*

