# Comparing `tmp/evox-0.8.0.tar.gz` & `tmp/evox-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evox-0.8.0.tar", last modified: Mon Apr 22 12:07:45 2024, max compression
+gzip compressed data, was "evox-0.8.1.tar", last modified: Tue Apr 23 13:55:44 2024, max compression
```

## Comparing `evox-0.8.0.tar` & `evox-0.8.1.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.729981 evox-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 12:07:37.000000 evox-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 12:07:37.000000 evox-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-22 12:07:45.729981 evox-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-22 12:07:37.000000 evox-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-22 12:07:37.000000 evox-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:07:45.729981 evox-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.685980 evox-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.689980 evox-0.8.0/src/evox/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.689980 evox-0.8.0/src/evox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.689980 evox-0.8.0/src/evox/algorithms/containers/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/containers/clustered_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/containers/coevolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/containers/tree_algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.693981 evox-0.8.0/src/evox/algorithms/mo/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/bce_ibea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/bige.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/eagmoead.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/gde3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/hype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/ibea.py
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/im_moea.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/knea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/lmocso.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/moead.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/moeaddra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/moeadm2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/nsga3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/rvea.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/rveaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/spea2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/sra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/mo/tdea.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.693981 evox-0.8.0/src/evox/algorithms/so/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.697980 evox-0.8.0/src/evox/algorithms/so/de_variants/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/de.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/jade.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/sade.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/de_variants/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.697980 evox-0.8.0/src/evox/algorithms/so/es_variants/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/amalgam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/ars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/asebo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/cma_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/cr_fm_nes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/des.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/esmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/guided_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/les.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/ma_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/nes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/noise_reuse_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/open_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/persistent_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/pgpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/rmes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/snes.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/es_variants/sort_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.701981 evox-0.8.0/src/evox/algorithms/so/pso_variants/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/clpso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/cso.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/dms_pso_el.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/fips.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/fs_pso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/pso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/sl_pso_gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/sl_pso_us.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/swmmpso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/topology_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/algorithms/so/pso_variants/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.701981 evox-0.8.0/src/evox/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.701981 evox-0.8.0/src/evox/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/metrics/gd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/metrics/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/metrics/igd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/eval_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/evoxvis_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/pop_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/std_mo_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/monitors/std_so_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/operators/crossover/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/differential_evolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/one_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/sbx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/simulated_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/crossover/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/operators/gaussian_process/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/gaussian_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/gaussian_process/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/gaussian_process/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/operators/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/mutation/bitflip.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/mutation/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/mutation/pm_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.705981 evox-0.8.0/src/evox/operators/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/sampling/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/sampling/latin_hypercude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/sampling/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/operators/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/find_pbest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/non_dominate.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/roulette_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/rvea_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/topk_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/tournament.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/operators/selection/uniform_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/problems/evoxbench/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/evoxbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/evoxbench/evoxbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/problems/neuroevolution/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/brax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/env_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/gym.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.709981 evox-0.8.0/src/evox/problems/neuroevolution/supervised_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/supervised_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/neuroevolution/supervised_learning/torchvision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.713981 evox-0.8.0/src/evox/problems/numerical/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/ackley.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.721981 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_1_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_1_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_1_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_2_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_2_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_2_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_3_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_3_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_3_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_4_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_4_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_4_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_5_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_5_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_5_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_6_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_6_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_6_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_7_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_7_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_7_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_8_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_8_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_8_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/Rand_Seeds.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_6.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_7.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_8.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_9.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_6_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_6_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D10.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D20.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21614 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/cec2022_so.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/dtlz.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/griewank.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/lsmop.py
--rw-r--r--   0 runner    (1001) docker     (127)    36810 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/maf.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/rastrigin.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/schwefel.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/problems/numerical/zdt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.721981 evox-0.8.0/src/evox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.721981 evox-0.8.0/src/evox/vis_tools/
--rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/vis_tools/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.721981 evox-0.8.0/src/evox/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/workflows/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/workflows/non_jit_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-04-22 12:07:37.000000 evox-0.8.0/src/evox/workflows/std_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.725981 evox-0.8.0/src/evox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-22 12:07:45.000000 evox-0.8.0/src/evox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-04-22 12:07:45.000000 evox-0.8.0/src/evox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:07:45.000000 evox-0.8.0/src/evox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-22 12:07:45.000000 evox-0.8.0/src/evox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 12:07:45.000000 evox-0.8.0/src/evox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:07:45.725981 evox-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_classic_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_crowding_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_envpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_evoxbench.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_lsmop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_maf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_multi_objective_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_neuroevolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_non_dominated_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_single_objective_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_test_suit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-22 12:07:37.000000 evox-0.8.0/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.961266 evox-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 13:55:39.000000 evox-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-23 13:55:39.000000 evox-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-23 13:55:44.961266 evox-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 13:55:39.000000 evox-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-23 13:55:39.000000 evox-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:55:44.961266 evox-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.913266 evox-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.917266 evox-0.8.1/src/evox/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.917266 evox-0.8.1/src/evox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.917266 evox-0.8.1/src/evox/algorithms/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/containers/clustered_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/containers/coevolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/containers/tree_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.921266 evox-0.8.1/src/evox/algorithms/mo/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/bce_ibea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/bige.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/eagmoead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/gde3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/hype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/ibea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/im_moea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/knea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/lmocso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/moead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/moeaddra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/moeadm2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/nsga3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/rvea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/rveaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/spea2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/sra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/mo/tdea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.921266 evox-0.8.1/src/evox/algorithms/so/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.925266 evox-0.8.1/src/evox/algorithms/so/de_variants/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/jade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/sade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/de_variants/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.929266 evox-0.8.1/src/evox/algorithms/so/es_variants/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/amalgam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/ars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/asebo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/cr_fm_nes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/des.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/esmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/guided_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/les.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/ma_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/nes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/noise_reuse_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/open_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/persistent_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/pgpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/rmes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/snes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/es_variants/sort_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.929266 evox-0.8.1/src/evox/algorithms/so/pso_variants/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/clpso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/cso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/dms_pso_el.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/fips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/fs_pso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/pso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/sl_pso_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/sl_pso_us.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/swmmpso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/topology_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/algorithms/so/pso_variants/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.929266 evox-0.8.1/src/evox/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.933266 evox-0.8.1/src/evox/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/metrics/gd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/metrics/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/metrics/igd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.933266 evox-0.8.1/src/evox/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/eval_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/evoxvis_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/pop_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/std_mo_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/monitors/std_so_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.933266 evox-0.8.1/src/evox/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.933266 evox-0.8.1/src/evox/operators/crossover/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/differential_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/one_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/sbx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/simulated_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/crossover/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.933266 evox-0.8.1/src/evox/operators/gaussian_process/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/gaussian_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/gaussian_process/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/gaussian_process/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/operators/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/mutation/bitflip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/mutation/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/mutation/pm_mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/operators/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/sampling/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/sampling/latin_hypercude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/sampling/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/operators/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/find_pbest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/non_dominate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/roulette_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/rvea_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/topk_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/tournament.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/operators/selection/uniform_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/problems/evoxbench/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/evoxbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/evoxbench/evoxbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/problems/neuroevolution/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.937266 evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/brax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/env_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/gym.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.941266 evox-0.8.1/src/evox/problems/neuroevolution/supervised_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/supervised_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/neuroevolution/supervised_learning/tfds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.941266 evox-0.8.1/src/evox/problems/numerical/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/ackley.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.953266 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_1_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_1_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_1_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_2_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_2_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_2_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_3_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_3_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_3_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_4_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_4_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_4_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_5_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_5_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_5_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_6_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_6_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_6_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_7_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_7_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_7_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_8_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_8_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_8_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100200 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/Rand_Seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_6_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_6_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21614 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/cec2022_so.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/dtlz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/griewank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/lsmop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36810 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/rastrigin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/schwefel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/problems/numerical/zdt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.953266 evox-0.8.1/src/evox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.953266 evox-0.8.1/src/evox/vis_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/vis_tools/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.953266 evox-0.8.1/src/evox/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/workflows/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/workflows/non_jit_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-04-23 13:55:39.000000 evox-0.8.1/src/evox/workflows/std_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.957266 evox-0.8.1/src/evox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-23 13:55:44.000000 evox-0.8.1/src/evox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-23 13:55:44.000000 evox-0.8.1/src/evox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:55:44.000000 evox-0.8.1/src/evox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 13:55:44.000000 evox-0.8.1/src/evox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 13:55:44.000000 evox-0.8.1/src/evox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:55:44.957266 evox-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_classic_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_crowding_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_envpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_evoxbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_lsmop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_multi_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_neuroevolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_non_dominated_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_single_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_test_suit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-23 13:55:39.000000 evox-0.8.1/tests/test_workflows.py
```

### Comparing `evox-0.8.0/LICENSE` & `evox-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/PKG-INFO` & `evox-0.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6576 6f78  : 2.1.Name: evox
-00000020: 0a56 6572 7369 6f6e 3a20 302e 382e 300a  .Version: 0.8.0.
+00000020: 0a56 6572 7369 6f6e 3a20 302e 382e 310a  .Version: 0.8.1.
 00000030: 5375 6d6d 6172 793a 2065 766f 780a 4175  Summary: evox.Au
 00000040: 7468 6f72 2d65 6d61 696c 3a20 4269 6c6c  thor-email: Bill
 00000050: 2048 7561 6e67 203c 6269 6c6c 2e68 7561   Huang <bill.hua
 00000060: 6e67 3230 3031 4067 6d61 696c 2e63 6f6d  ng2001@gmail.com
 00000070: 3e2c 2043 6872 6973 7469 6e61 204c 6565  >, Christina Lee
 00000080: 203c 3133 3135 3535 3239 3932 4071 712e   <1315552992@qq.
 00000090: 636f 6d3e 2c20 5a68 656e 7975 204c 6961  com>, Zhenyu Lia
@@ -161,552 +161,568 @@
 00000a00: 4469 7374 3a20 6368 6578 3e3d 302e 312e  Dist: chex>=0.1.
 00000a10: 303b 2065 7874 7261 203d 3d20 2274 6573  0; extra == "tes
 00000a20: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
 00000a30: 3a20 666c 6178 3e3d 302e 352e 303b 2065  : flax>=0.5.0; e
 00000a40: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
 00000a50: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
 00000a60: 7465 7374 3e3d 362e 302e 303b 2065 7874  test>=6.0.0; ext
-00000a70: 7261 203d 3d20 2274 6573 7422 0a50 726f  ra == "test".Pro
-00000a80: 7669 6465 732d 4578 7472 613a 2076 6973  vides-Extra: vis
-00000a90: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000aa0: 706c 6f74 6c79 3e3d 352e 302e 303b 2065  plotly>=5.0.0; e
-00000ab0: 7874 7261 203d 3d20 2276 6973 220a 5265  xtra == "vis".Re
-00000ac0: 7175 6972 6573 2d44 6973 743a 2070 616e  quires-Dist: pan
-00000ad0: 6461 733e 3d32 2e30 2e30 3b20 6578 7472  das>=2.0.0; extr
-00000ae0: 6120 3d3d 2022 7669 7322 0a50 726f 7669  a == "vis".Provi
-00000af0: 6465 732d 4578 7472 613a 2067 796d 6e61  des-Extra: gymna
-00000b00: 7369 756d 0a52 6571 7569 7265 732d 4469  sium.Requires-Di
-00000b10: 7374 3a20 6779 6d6e 6173 6975 6d3e 3d30  st: gymnasium>=0
-00000b20: 2e32 392e 303b 2065 7874 7261 203d 3d20  .29.0; extra == 
-00000b30: 2267 796d 6e61 7369 756d 220a 5072 6f76  "gymnasium".Prov
-00000b40: 6964 6573 2d45 7874 7261 3a20 656e 7670  ides-Extra: envp
-00000b50: 6f6f 6c0a 5265 7175 6972 6573 2d44 6973  ool.Requires-Dis
-00000b60: 743a 2065 6e76 706f 6f6c 3e3d 302e 382e  t: envpool>=0.8.
-00000b70: 303b 2065 7874 7261 203d 3d20 2265 6e76  0; extra == "env
-00000b80: 706f 6f6c 220a 5072 6f76 6964 6573 2d45  pool".Provides-E
-00000b90: 7874 7261 3a20 6e65 7572 6f65 766f 6c75  xtra: neuroevolu
-00000ba0: 7469 6f6e 0a52 6571 7569 7265 732d 4469  tion.Requires-Di
-00000bb0: 7374 3a20 746f 7263 683e 3d31 2e30 2e30  st: torch>=1.0.0
-00000bc0: 3b20 6578 7472 6120 3d3d 2022 6e65 7572  ; extra == "neur
-00000bd0: 6f65 766f 6c75 7469 6f6e 220a 5265 7175  oevolution".Requ
-00000be0: 6972 6573 2d44 6973 743a 2074 6f72 6368  ires-Dist: torch
-00000bf0: 7669 7369 6f6e 3e3d 302e 312e 303b 2065  vision>=0.1.0; e
-00000c00: 7874 7261 203d 3d20 226e 6575 726f 6576  xtra == "neuroev
-00000c10: 6f6c 7574 696f 6e22 0a50 726f 7669 6465  olution".Provide
-00000c20: 732d 4578 7472 613a 2064 6973 7472 6962  s-Extra: distrib
-00000c30: 7574 6564 0a52 6571 7569 7265 732d 4469  uted.Requires-Di
-00000c40: 7374 3a20 7261 793e 3d32 2e30 2e30 3b20  st: ray>=2.0.0; 
-00000c50: 6578 7472 6120 3d3d 2022 6469 7374 7269  extra == "distri
-00000c60: 6275 7465 6422 0a50 726f 7669 6465 732d  buted".Provides-
-00000c70: 4578 7472 613a 2066 756c 6c0a 5265 7175  Extra: full.Requ
-00000c80: 6972 6573 2d44 6973 743a 2067 796d 6e61  ires-Dist: gymna
-00000c90: 7369 756d 3e3d 302e 3239 2e30 3b20 6578  sium>=0.29.0; ex
-00000ca0: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000cb0: 7175 6972 6573 2d44 6973 743a 2072 6179  quires-Dist: ray
-00000cc0: 3e3d 322e 302e 303b 2065 7874 7261 203d  >=2.0.0; extra =
-00000cd0: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
-00000ce0: 732d 4469 7374 3a20 746f 7263 683e 3d31  s-Dist: torch>=1
-00000cf0: 2e30 2e30 3b20 6578 7472 6120 3d3d 2022  .0.0; extra == "
-00000d00: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
-00000d10: 6973 743a 2074 6f72 6368 7669 7369 6f6e  ist: torchvision
-00000d20: 3e3d 302e 312e 303b 2065 7874 7261 203d  >=0.1.0; extra =
-00000d30: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
-00000d40: 732d 4469 7374 3a20 656e 7670 6f6f 6c3e  s-Dist: envpool>
-00000d50: 3d30 2e38 2e30 3b20 6578 7472 6120 3d3d  =0.8.0; extra ==
-00000d60: 2022 6675 6c6c 220a 5265 7175 6972 6573   "full".Requires
-00000d70: 2d44 6973 743a 2067 706a 6178 3e3d 302e  -Dist: gpjax>=0.
-00000d80: 382e 303b 2065 7874 7261 203d 3d20 2266  8.0; extra == "f
-00000d90: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
-00000da0: 7374 3a20 706c 6f74 6c79 3e3d 352e 302e  st: plotly>=5.0.
-00000db0: 303b 2065 7874 7261 203d 3d20 2266 756c  0; extra == "ful
-00000dc0: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000dd0: 3a20 7061 6e64 6173 3e3d 322e 302e 303b  : pandas>=2.0.0;
-00000de0: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-00000df0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000e00: 2067 700a 5265 7175 6972 6573 2d44 6973   gp.Requires-Dis
-00000e10: 743a 2067 706a 6178 3e3d 302e 382e 303b  t: gpjax>=0.8.0;
-00000e20: 2065 7874 7261 203d 3d20 2267 7022 0a0a   extra == "gp"..
-00000e30: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000e40: 7222 3e0a 2020 3c70 6963 7475 7265 3e0a  r">.  <picture>.
-00000e50: 2020 2020 3c73 6f75 7263 6520 6d65 6469      <source medi
-00000e60: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
-00000e70: 722d 7363 6865 6d65 3a20 6461 726b 2922  r-scheme: dark)"
-00000e80: 2073 7263 7365 743d 2264 6f63 732f 736f   srcset="docs/so
-00000e90: 7572 6365 2f5f 7374 6174 6963 2f65 766f  urce/_static/evo
-00000ea0: 785f 6c6f 676f 5f64 6172 6b2e 706e 6722  x_logo_dark.png"
-00000eb0: 3e0a 2020 2020 3c73 6f75 7263 6520 6d65  >.    <source me
-00000ec0: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
-00000ed0: 6c6f 722d 7363 6865 6d65 3a20 6c69 6768  lor-scheme: ligh
-00000ee0: 7429 2220 7372 6373 6574 3d22 646f 6373  t)" srcset="docs
-00000ef0: 2f73 6f75 7263 652f 5f73 7461 7469 632f  /source/_static/
-00000f00: 6576 6f78 5f6c 6f67 6f5f 6c69 6768 742e  evox_logo_light.
-00000f10: 706e 6722 3e0a 2020 2020 3c69 6d67 2061  png">.    <img a
-00000f20: 6c74 3d22 4576 6f58 204c 6f67 6f22 2068  lt="EvoX Logo" h
-00000f30: 6569 6768 743d 2231 3238 2220 7769 6474  eight="128" widt
-00000f40: 683d 2235 3030 7078 2220 7372 633d 2264  h="500px" src="d
-00000f50: 6f63 732f 736f 7572 6365 2f5f 7374 6174  ocs/source/_stat
-00000f60: 6963 2f65 766f 785f 6c6f 676f 5f6c 6967  ic/evox_logo_lig
-00000f70: 6874 2e70 6e67 223e 0a20 203c 2f70 6963  ht.png">.  </pic
-00000f80: 7475 7265 3e0a 3c2f 6831 3e0a 0a3c 7020  ture>.</h1>..<p 
-00000f90: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000fa0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000fb0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-00000fc0: 2f32 3330 312e 3132 3435 3722 3e0a 2020  /2301.12457">.  
-00000fd0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000fe0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000ff0: 696f 2f62 6164 6765 2f70 6170 6572 2d61  io/badge/paper-a
-00001000: 7278 6976 2d72 6564 3f73 7479 6c65 3d66  rxiv-red?style=f
-00001010: 6f72 2d74 6865 2d62 6164 6765 2220 616c  or-the-badge" al
-00001020: 743d 2245 766f 5820 5061 7065 7220 6f6e  t="EvoX Paper on
-00001030: 2061 7258 6976 223e 0a20 203c 2f61 3e0a   arXiv">.  </a>.
-00001040: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00001050: 733a 2f2f 6576 6f78 2e72 6561 6474 6865  s://evox.readthe
-00001060: 646f 6373 2e69 6f2f 223e 0a20 2020 203c  docs.io/">.    <
-00001070: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001080: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001090: 6261 6467 652f 646f 6373 2d72 6561 6474  badge/docs-readt
-000010a0: 6865 646f 6373 2d62 6c75 653f 7374 796c  hedocs-blue?styl
-000010b0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000010c0: 2061 6c74 3d22 4576 6f58 2044 6f63 756d   alt="EvoX Docum
-000010d0: 656e 7461 7469 6f6e 223e 0a20 203c 2f61  entation">.  </a
-000010e0: 3e0a 3c2f 703e 0a0a 3c70 2061 6c69 676e  >.</p>..<p align
-000010f0: 3d22 6365 6e74 6572 223e 0a20 203c 623e  ="center">.  <b>
-00001100: f09f 8c9f 4469 7374 7269 6275 7465 6420  ....Distributed 
-00001110: 4750 552d 6163 6365 6c65 7261 7465 6420  GPU-accelerated 
-00001120: 4672 616d 6577 6f72 6b20 666f 7220 5363  Framework for Sc
-00001130: 616c 6162 6c65 2045 766f 6c75 7469 6f6e  alable Evolution
-00001140: 6172 7920 436f 6d70 7574 6174 696f 6ef0  ary Computation.
-00001150: 9f8c 9f3c 2f62 3e0a 3c2f 703e 0a0a 2d2d  ...</b>.</p>..--
-00001160: 2d0a 0a23 230a 4275 696c 6469 6e67 2075  -..##.Building u
-00001170: 706f 6e20 5b4a 4158 5d28 6874 7470 733a  pon [JAX](https:
-00001180: 2f2f 6769 7468 7562 2e63 6f6d 2f67 6f6f  //github.com/goo
-00001190: 676c 652f 6a61 7829 2061 6e64 205b 5261  gle/jax) and [Ra
-000011a0: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000011b0: 622e 636f 6d2f 7261 792d 7072 6f6a 6563  b.com/ray-projec
-000011c0: 742f 7261 7929 2c20 4576 6f58 206f 6666  t/ray), EvoX off
-000011d0: 6572 7320 6120 636f 6d70 7265 6865 6e73  ers a comprehens
-000011e0: 6976 6520 7375 6974 6520 6f66 202a 2a35  ive suite of **5
-000011f0: 302b 2045 766f 6c75 7469 6f6e 6172 7920  0+ Evolutionary 
-00001200: 416c 676f 7269 7468 6d73 2028 4541 7329  Algorithms (EAs)
-00001210: 2a2a 2061 6e64 2061 2077 6964 6520 7261  ** and a wide ra
-00001220: 6e67 6520 6f66 202a 2a31 3030 2b20 4265  nge of **100+ Be
-00001230: 6e63 686d 6172 6b20 5072 6f62 6c65 6d73  nchmark Problems
-00001240: 2a2a 2c20 616c 6c20 6265 6e65 6669 7469  **, all benefiti
-00001250: 6e67 2066 726f 6d20 6469 7374 7269 6275  ng from distribu
-00001260: 7465 6420 4750 552d 6163 6365 6c65 7261  ted GPU-accelera
-00001270: 7469 6f6e 2e20 4974 2066 6163 696c 6974  tion. It facilit
-00001280: 6174 6573 2065 6666 6963 6965 6e74 2065  ates efficient e
-00001290: 7870 6c6f 7261 7469 6f6e 206f 6620 636f  xploration of co
-000012a0: 6d70 6c65 7820 6f70 7469 6d69 7a61 7469  mplex optimizati
-000012b0: 6f6e 206c 616e 6473 6361 7065 732c 2065  on landscapes, e
-000012c0: 6666 6563 7469 7665 2074 6163 6b6c 696e  ffective tacklin
-000012d0: 6720 6f66 2062 6c61 636b 2d62 6f78 206f  g of black-box o
-000012e0: 7074 696d 697a 6174 696f 6e20 6368 616c  ptimization chal
-000012f0: 6c65 6e67 6573 2c20 616e 6420 6465 6570  lenges, and deep
-00001300: 2064 6976 6573 2069 6e74 6f20 6e65 7572   dives into neur
-00001310: 6f65 766f 6c75 7469 6f6e 2077 6974 6820  oevolution with 
-00001320: 5b42 7261 785d 2868 7474 7073 3a2f 2f67  [Brax](https://g
-00001330: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
-00001340: 2f62 7261 7829 2e20 5769 7468 2061 2066  /brax). With a f
-00001350: 6f75 6e64 6174 696f 6e20 696e 2066 756e  oundation in fun
-00001360: 6374 696f 6e61 6c20 7072 6f67 7261 6d6d  ctional programm
-00001370: 696e 6720 616e 6420 6869 6572 6172 6368  ing and hierarch
-00001380: 6963 616c 2073 7461 7465 206d 616e 6167  ical state manag
-00001390: 656d 656e 742c 2045 766f 5820 6f66 6665  ement, EvoX offe
-000013a0: 7273 2061 2075 7365 722d 6672 6965 6e64  rs a user-friend
-000013b0: 6c79 2061 6e64 206d 6f64 756c 6172 2065  ly and modular e
-000013c0: 7870 6572 6965 6e63 652e 2046 6f72 206d  xperience. For m
-000013d0: 6f72 6520 6465 7461 696c 732c 2070 6c65  ore details, ple
-000013e0: 6173 6520 7265 6665 7220 746f 206f 7572  ase refer to our
-000013f0: 205b 5061 7065 725d 2868 7474 7073 3a2f   [Paper](https:/
-00001400: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00001410: 3330 312e 3132 3435 3729 2061 6e64 205b  301.12457) and [
-00001420: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00001430: 7474 7073 3a2f 2f65 766f 782e 7265 6164  ttps://evox.read
-00001440: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00001450: 7465 7374 2f29 202f 205b e696 87e6 a1a3  test/) / [......
-00001460: 5d28 6874 7470 733a 2f2f 6576 6f78 2e72  ](https://evox.r
-00001470: 6561 6474 6865 646f 6373 2e69 6f2f 7a68  eadthedocs.io/zh
-00001480: 2f6c 6174 6573 742f 292e 0a0a 2d2d 2d0a  /latest/)...---.
-00001490: 0a23 2320 4b65 7920 4665 6174 7572 6573  .## Key Features
-000014a0: 0a0a 2d20 f09f 9a80 202a 2a46 6173 7420  ..- .... **Fast 
-000014b0: 5065 7266 6f72 6d61 6e63 652a 2a3a 0a20  Performance**:. 
-000014c0: 202d 2045 7870 6572 6965 6e63 6520 2a2a   - Experience **
-000014d0: 4750 552d 4163 6365 6c65 7261 7465 642a  GPU-Accelerated*
-000014e0: 2a20 6f70 7469 6d69 7a61 7469 6f6e 2c20  * optimization, 
-000014f0: 6163 6869 6576 696e 6720 7370 6565 6473  achieving speeds
-00001500: 206f 7665 7220 3130 3078 2066 6173 7465   over 100x faste
-00001510: 7220 7468 616e 2074 7261 6469 7469 6f6e  r than tradition
-00001520: 616c 206d 6574 686f 6473 2e0a 2020 2d20  al methods..  - 
-00001530: 4c65 7665 7261 6765 2074 6865 2070 6f77  Leverage the pow
-00001540: 6572 206f 6620 2a2a 4469 7374 7269 6275  er of **Distribu
-00001550: 7465 6420 576f 726b 666c 6f77 732a 2a20  ted Workflows** 
-00001560: 666f 7220 6576 656e 206d 6f72 6520 7261  for even more ra
-00001570: 7069 6420 6f70 7469 6d69 7a61 7469 6f6e  pid optimization
-00001580: 2e0a 0a2d 20f0 9f8c 9020 2a2a 5665 7273  ...- .... **Vers
-00001590: 6174 696c 6520 4f70 7469 6d69 7a61 7469  atile Optimizati
-000015a0: 6f6e 2053 7569 7465 2a2a 3a0a 2020 2d20  on Suite**:.  - 
-000015b0: 4361 7465 7220 746f 2061 6c6c 2079 6f75  Cater to all you
-000015c0: 7220 6e65 6564 7320 7769 7468 2062 6f74  r needs with bot
-000015d0: 6820 2a2a 5369 6e67 6c65 2d6f 626a 6563  h **Single-objec
-000015e0: 7469 7665 2a2a 2061 6e64 202a 2a4d 756c  tive** and **Mul
-000015f0: 7469 2d6f 626a 6563 7469 7665 2a2a 206f  ti-objective** o
-00001600: 7074 696d 697a 6174 696f 6e20 6361 7061  ptimization capa
-00001610: 6269 6c69 7469 6573 2e0a 2020 2d20 4469  bilities..  - Di
-00001620: 7665 2069 6e74 6f20 6120 636f 6d70 7265  ve into a compre
-00001630: 6865 6e73 6976 6520 6c69 6272 6172 7920  hensive library 
-00001640: 6f66 202a 2a42 656e 6368 6d61 726b 2050  of **Benchmark P
-00001650: 726f 626c 656d 732a 2a2c 2065 6e73 7572  roblems**, ensur
-00001660: 696e 6720 726f 6275 7374 2074 6573 7469  ing robust testi
-00001670: 6e67 2061 6e64 2065 7661 6c75 6174 696f  ng and evaluatio
-00001680: 6e2e 0a20 202d 2045 7870 6c6f 7265 2074  n..  - Explore t
-00001690: 6865 2066 726f 6e74 6965 7220 6f66 2041  he frontier of A
-000016a0: 4920 7769 7468 2065 7874 656e 7369 7665  I with extensive
-000016b0: 2074 6f6f 6c73 2066 6f72 202a 2a4e 6575   tools for **Neu
-000016c0: 726f 6576 6f6c 7574 696f 6e2a 2a20 7461  roevolution** ta
-000016d0: 736b 732e 0a0a 2d20 f09f 9ba0 efb8 8f20  sks...- ....... 
-000016e0: 2a2a 4465 7369 676e 6564 2066 6f72 2053  **Designed for S
-000016f0: 696d 706c 6963 6974 792a 2a3a 0a20 202d  implicity**:.  -
-00001700: 2045 6d62 7261 6365 2074 6865 2065 6c65   Embrace the ele
-00001710: 6761 6e63 6520 6f66 202a 2a46 756e 6374  gance of **Funct
-00001720: 696f 6e61 6c20 5072 6f67 7261 6d6d 696e  ional Programmin
-00001730: 672a 2a2c 2073 696d 706c 6966 7969 6e67  g**, simplifying
-00001740: 2063 6f6d 706c 6578 2061 6c67 6f72 6974   complex algorit
-00001750: 686d 6963 2063 6f6d 706f 7369 7469 6f6e  hmic composition
-00001760: 732e 0a20 202d 2042 656e 6566 6974 2066  s..  - Benefit f
-00001770: 726f 6d20 2a2a 4869 6572 6172 6368 6963  rom **Hierarchic
-00001780: 616c 2053 7461 7465 204d 616e 6167 656d  al State Managem
-00001790: 656e 742a 2a2c 2065 6e73 7572 696e 6720  ent**, ensuring 
-000017a0: 6d6f 6475 6c61 7220 616e 6420 636c 6561  modular and clea
-000017b0: 6e20 7072 6f67 7261 6d6d 696e 672e 0a20  n programming.. 
-000017c0: 202d 204a 756d 7073 7461 7274 2079 6f75   - Jumpstart you
-000017d0: 7220 6a6f 7572 6e65 7920 7769 7468 206f  r journey with o
-000017e0: 7572 205b 4465 7461 696c 6564 2054 7574  ur [Detailed Tut
-000017f0: 6f72 6961 6c5d 2868 7474 7073 3a2f 2f65  orial](https://e
-00001800: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
-00001810: 696f 2f65 6e2f 6c61 7465 7374 2f67 7569  io/en/latest/gui
-00001820: 6465 2f62 6173 6963 732f 696e 6465 782e  de/basics/index.
-00001830: 6874 6d6c 292e 0a0a 2d2d 2d0a 0a23 2320  html)...---..## 
-00001840: 436f 6d70 7265 6865 6e73 6976 6520 4576  Comprehensive Ev
-00001850: 6f6c 7574 696f 6e61 7279 2041 6c67 6f72  olutionary Algor
-00001860: 6974 686d 730a 0a23 2323 2053 696e 676c  ithms..### Singl
-00001870: 652d 4f62 6a65 6374 6976 6520 4f70 7469  e-Objective Opti
-00001880: 6d69 7a61 7469 6f6e 0a0a 7c20 4361 7465  mization..| Cate
-00001890: 676f 7279 2020 2020 2020 2020 2020 2020  gory            
-000018a0: 2020 2020 2020 2020 7c20 416c 676f 7269          | Algori
-000018b0: 7468 6d20 4e61 6d65 7320 2020 2020 2020  thm Names       
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d        |.| ------
-000018e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000018f0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-00001900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001920: 2d2d 207c 0a7c 2044 6966 6665 7265 6e74  -- |.| Different
-00001930: 6961 6c20 4576 6f6c 7574 696f 6e20 2020  ial Evolution   
-00001940: 2020 207c 2043 6f44 452c 204a 6144 452c     | CoDE, JaDE,
-00001950: 2053 6144 452c 2053 4841 4445 2c20 494d   SaDE, SHADE, IM
-00001960: 4f44 452c 202e 2e2e 2020 2020 2020 2020  ODE, ...        
-00001970: 7c0a 7c20 4576 6f6c 7574 696f 6e20 5374  |.| Evolution St
-00001980: 7261 7465 6779 2020 2020 2020 2020 7c20  rategy        | 
-00001990: 434d 412d 4553 2c20 5047 5045 2c20 4f70  CMA-ES, PGPE, Op
-000019a0: 656e 4553 2c20 4352 2d46 4d2d 4e45 532c  enES, CR-FM-NES,
-000019b0: 2078 4e45 532c 202e 2e2e 207c 0a7c 2050   xNES, ... |.| P
-000019c0: 6172 7469 636c 6520 5377 6172 6d20 4f70  article Swarm Op
-000019d0: 7469 6d69 7a61 7469 6f6e 207c 2046 4950  timization | FIP
-000019e0: 532c 2043 534f 2c20 4350 534f 2c20 434c  S, CSO, CPSO, CL
-000019f0: 5053 4f2c 2053 4c2d 5053 4f2c 202e 2e2e  PSO, SL-PSO, ...
-00001a00: 2020 2020 2020 2020 7c0a 0a23 2323 204d          |..### M
-00001a10: 756c 7469 2d4f 626a 6563 7469 7665 204f  ulti-Objective O
-00001a20: 7074 696d 697a 6174 696f 6e0a 0a7c 2043  ptimization..| C
-00001a30: 6174 6567 6f72 7920 2020 2020 2020 2020  ategory         
-00001a40: 2020 7c20 416c 676f 7269 7468 6d20 4e61    | Algorithm Na
-00001a50: 6d65 7320 2020 2020 2020 2020 2020 2020  mes             
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d      |.| --------
-00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
-00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a 7c20  ----------- |.| 
-00001ac0: 446f 6d69 6e61 6e63 652d 6261 7365 6420  Dominance-based 
-00001ad0: 2020 207c 204e 5347 412d 4949 2c20 4e53     | NSGA-II, NS
-00001ae0: 4741 2d49 4949 2c20 5350 4541 322c 2042  GA-III, SPEA2, B
-00001af0: 6947 452c 204b 6e45 412c 202e 2e2e 2020  iGE, KnEA, ...  
-00001b00: 2020 2020 7c0a 7c20 4465 636f 6d70 6f73      |.| Decompos
-00001b10: 6974 696f 6e2d 6261 7365 647c 204d 4f45  ition-based| MOE
-00001b20: 412f 442c 2052 5645 412c 2074 2d44 4541  A/D, RVEA, t-DEA
-00001b30: 2c20 4d4f 4541 442d 4d32 4d2c 2045 4147  , MOEAD-M2M, EAG
-00001b40: 2d4d 4f45 4144 2c20 2e2e 2e20 7c0a 7c20  -MOEAD, ... |.| 
-00001b50: 496e 6469 6361 746f 722d 6261 7365 6420  Indicator-based 
-00001b60: 2020 207c 2049 4245 412c 2048 7970 452c     | IBEA, HypE,
-00001b70: 2053 5241 2c20 4d61 4f45 412d 4947 442c   SRA, MaOEA-IGD,
-00001b80: 2041 522d 4d4f 4541 2c20 2e2e 2e20 2020   AR-MOEA, ...   
-00001b90: 2020 2020 7c0a 0a46 6f72 2061 2063 6f6d      |..For a com
-00001ba0: 7072 6568 656e 7369 7665 206c 6973 7420  prehensive list 
-00001bb0: 616e 6420 6675 7274 6865 7220 6465 7461  and further deta
-00001bc0: 696c 7320 6f66 2061 6c6c 2061 6c67 6f72  ils of all algor
-00001bd0: 6974 686d 732c 2070 6c65 6173 6520 6368  ithms, please ch
-00001be0: 6563 6b20 7468 6520 5b41 5049 2044 6f63  eck the [API Doc
-00001bf0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001c00: 733a 2f2f 6576 6f78 2e72 6561 6474 6865  s://evox.readthe
-00001c10: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00001c20: 742f 6170 692f 616c 676f 7269 7468 6d73  t/api/algorithms
-00001c30: 2f69 6e64 6578 2e68 746d 6c29 2e0a 0a23  /index.html)...#
-00001c40: 2320 4469 7665 7273 6520 4265 6e63 686d  # Diverse Benchm
-00001c50: 6172 6b20 5072 6f62 6c65 6d73 0a0a 7c20  ark Problems..| 
-00001c60: 4361 7465 676f 7279 2020 2020 2020 7c20  Category      | 
-00001c70: 5072 6f62 6c65 6d20 4e61 6d65 7320 2020  Problem Names   
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2020 2020 7c0a 7c20 2d2d 2d2d          |.| ----
-00001ca0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00001cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cd0: 2d2d 2d20 7c0a 7c20 4e75 6d65 7269 6361  --- |.| Numerica
-00001ce0: 6c20 2020 2020 7c20 4454 4c5a 2c20 4c53  l     | DTLZ, LS
-00001cf0: 4d4f 502c 204d 6146 2c20 5a44 542c 2043  MOP, MaF, ZDT, C
-00001d00: 4543 2732 322c 2020 2e2e 2e20 2020 207c  EC'22,  ...    |
-00001d10: 0a7c 204e 6575 726f 6576 6f6c 7574 696f  .| Neuroevolutio
-00001d20: 6e7c 2042 7261 782c 2047 796d 2c20 546f  n| Brax, Gym, To
-00001d30: 7263 6856 6973 696f 6e20 4461 7461 7365  rchVision Datase
-00001d40: 742c 202e 2e2e 2020 2020 7c0a 0a46 6f72  t, ...    |..For
-00001d50: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
-00001d60: 206c 6973 7420 616e 6420 6675 7274 6865   list and furthe
-00001d70: 7220 6465 7461 696c 7320 6f66 2061 6c6c  r details of all
-00001d80: 2062 656e 6368 6d61 726b 2070 726f 626c   benchmark probl
-00001d90: 656d 732c 2070 6c65 6173 6520 6368 6563  ems, please chec
-00001da0: 6b20 7468 6520 5b41 5049 2044 6f63 756d  k the [API Docum
-00001db0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00001dc0: 2f2f 6576 6f78 2e72 6561 6474 6865 646f  //evox.readthedo
-00001dd0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001de0: 6170 692f 7072 6f62 6c65 6d73 2f69 6e64  api/problems/ind
-00001df0: 6578 2e68 746d 6c29 2e0a 0a0a 2323 2053  ex.html)....## S
-00001e00: 6574 7469 6e67 2055 7020 4576 6f58 0a0a  etting Up EvoX..
-00001e10: 496e 7374 616c 6c20 6065 766f 7860 2065  Install `evox` e
-00001e20: 6666 6f72 746c 6573 736c 7920 7669 6120  ffortlessly via 
-00001e30: 6070 6970 603a 0a60 6060 6261 7368 0a70  `pip`:.```bash.p
-00001e40: 6970 2069 6e73 7461 6c6c 2065 766f 780a  ip install evox.
-00001e50: 6060 600a 0a2a 2a4e 6f74 652a 2a3a 2054  ```..**Note**: T
-00001e60: 6f20 696e 7374 616c 6c20 4576 6f58 2077  o install EvoX w
-00001e70: 6974 6820 4a41 5820 616e 6420 6861 7264  ith JAX and hard
-00001e80: 7761 7265 2061 6363 656c 6572 6174 696f  ware acceleratio
-00001e90: 6e20 6361 7061 6269 6c69 7469 6573 2c20  n capabilities, 
-00001ea0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-00001eb0: 6f75 7220 636f 6d70 7265 6865 6e73 6976  our comprehensiv
-00001ec0: 6520 5b49 6e73 7461 6c6c 6174 696f 6e20  e [Installation 
-00001ed0: 4775 6964 655d 2868 7474 7073 3a2f 2f65  Guide](https://e
-00001ee0: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
-00001ef0: 696f 2f65 6e2f 6c61 7465 7374 2f67 7569  io/en/latest/gui
-00001f00: 6465 2f69 6e73 7461 6c6c 2e68 746d 6c29  de/install.html)
-00001f10: 2e0a 0a0a 2323 2051 7569 636b 2053 7461  ....## Quick Sta
-00001f20: 7274 0a0a 4b69 636b 7374 6172 7420 796f  rt..Kickstart yo
-00001f30: 7572 206a 6f75 726e 6579 2077 6974 6820  ur journey with 
-00001f40: 4576 6f58 2069 6e20 6a75 7374 2061 2066  EvoX in just a f
-00001f50: 6577 2073 696d 706c 6520 7374 6570 733a  ew simple steps:
-00001f60: 0a31 2e20 2a2a 496d 706f 7274 206e 6563  .1. **Import nec
-00001f70: 6573 7361 7279 206d 6f64 756c 6573 2a2a  essary modules**
-00001f80: 3a0a 6060 6070 7974 686f 6e0a 696d 706f  :.```python.impo
-00001f90: 7274 2065 766f 780a 6672 6f6d 2065 766f  rt evox.from evo
-00001fa0: 7820 696d 706f 7274 2061 6c67 6f72 6974  x import algorit
-00001fb0: 686d 732c 2070 726f 626c 656d 732c 2077  hms, problems, w
-00001fc0: 6f72 6b66 6c6f 7773 0a60 6060 0a32 2e20  orkflows.```.2. 
-00001fd0: 2a2a 436f 6e66 6967 7572 6520 616e 2061  **Configure an a
-00001fe0: 6c67 6f72 6974 686d 2061 6e64 2064 6566  lgorithm and def
-00001ff0: 696e 6520 6120 7072 6f62 6c65 6d2a 2a3a  ine a problem**:
-00002000: 0a60 6060 7079 7468 6f6e 0a70 736f 203d  .```python.pso =
-00002010: 2061 6c67 6f72 6974 686d 732e 5053 4f28   algorithms.PSO(
-00002020: 0a20 2020 206c 623d 6a6e 702e 6675 6c6c  .    lb=jnp.full
-00002030: 2873 6861 7065 3d28 322c 292c 2066 696c  (shape=(2,), fil
-00002040: 6c5f 7661 6c75 653d 2d33 3229 2c0a 2020  l_value=-32),.  
-00002050: 2020 7562 3d6a 6e70 2e66 756c 6c28 7368    ub=jnp.full(sh
-00002060: 6170 653d 2832 2c29 2c20 6669 6c6c 5f76  ape=(2,), fill_v
-00002070: 616c 7565 3d33 3229 2c0a 2020 2020 706f  alue=32),.    po
-00002080: 705f 7369 7a65 3d31 3030 2c0a 290a 6163  p_size=100,.).ac
-00002090: 6b6c 6579 203d 2070 726f 626c 656d 732e  kley = problems.
-000020a0: 6e75 6d65 7269 6361 6c2e 4163 6b6c 6579  numerical.Ackley
-000020b0: 2829 0a60 6060 0a33 2e20 2a2a 436f 6d70  ().```.3. **Comp
-000020c0: 6f73 6520 616e 6420 696e 6974 6961 6c69  ose and initiali
-000020d0: 7a65 2074 6865 2077 6f72 6b66 6c6f 772a  ze the workflow*
-000020e0: 2a3a 0a60 6060 7079 7468 6f6e 0a77 6f72  *:.```python.wor
-000020f0: 6b66 6c6f 7720 3d20 776f 726b 666c 6f77  kflow = workflow
-00002100: 732e 5374 6457 6f72 6b66 6c6f 7728 7073  s.StdWorkflow(ps
-00002110: 6f2c 2061 636b 6c65 7929 0a6b 6579 203d  o, ackley).key =
-00002120: 206a 6178 2e72 616e 646f 6d2e 5052 4e47   jax.random.PRNG
-00002130: 4b65 7928 3432 290a 7374 6174 6520 3d20  Key(42).state = 
-00002140: 776f 726b 666c 6f77 2e69 6e69 7428 6b65  workflow.init(ke
-00002150: 7929 0a60 6060 0a34 2e20 2a2a 5275 6e20  y).```.4. **Run 
-00002160: 7468 6520 776f 726b 666c 6f77 2a2a 3a0a  the workflow**:.
-00002170: 6060 6070 7974 686f 6e0a 2320 4578 6563  ```python.# Exec
-00002180: 7574 6520 7468 6520 776f 726b 666c 6f77  ute the workflow
-00002190: 2066 6f72 2031 3030 2069 7465 7261 7469   for 100 iterati
-000021a0: 6f6e 730a 666f 7220 6920 696e 2072 616e  ons.for i in ran
-000021b0: 6765 2831 3030 293a 0a20 2020 2073 7461  ge(100):.    sta
-000021c0: 7465 203d 2077 6f72 6b66 6c6f 772e 7374  te = workflow.st
-000021d0: 6570 2873 7461 7465 290a 6060 600a 0a23  ep(state).```..#
-000021e0: 2320 5573 652d 6361 7365 7320 616e 6420  # Use-cases and 
-000021f0: 4170 706c 6963 6174 696f 6e73 0a0a 5472  Applications..Tr
-00002200: 7920 6f75 7420 7265 6164 792d 746f 2d70  y out ready-to-p
-00002210: 6c61 7920 6578 616d 706c 6573 2069 6e20  lay examples in 
-00002220: 796f 7572 2062 726f 7773 6572 2077 6974  your browser wit
-00002230: 6820 436f 6c61 623a 0a0a 7c20 4578 616d  h Colab:..| Exam
-00002240: 706c 6520 7c20 4c69 6e6b 207c 0a7c 202d  ple | Link |.| -
-00002250: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d20 7c0a  ------ | ---- |.
-00002260: 7c20 4261 7369 6320 5573 6167 6520 7c20  | Basic Usage | 
-00002270: 5b21 5b4f 7065 6e20 696e 2043 6f6c 6162  [![Open in Colab
-00002280: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00002290: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-000022a0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
-000022b0: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
-000022c0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-000022d0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
-000022e0: 6974 6875 622f 454d 492d 4772 6f75 702f  ithub/EMI-Group/
-000022f0: 6576 6f78 2f62 6c6f 622f 6d61 696e 2f64  evox/blob/main/d
-00002300: 6f63 732f 736f 7572 6365 2f67 7569 6465  ocs/source/guide
-00002310: 2f62 6173 6963 732f 312d 7374 6172 742e  /basics/1-start.
-00002320: 6970 796e 6229 207c 0a7c 204e 756d 6572  ipynb) |.| Numer
-00002330: 6963 616c 204f 7074 696d 697a 6174 696f  ical Optimizatio
-00002340: 6e20 7c20 5b21 5b4f 7065 6e20 696e 2043  n | [![Open in C
-00002350: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
-00002360: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002370: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00002380: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
-00002390: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-000023a0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-000023b0: 6f6d 2f67 6974 6875 622f 454d 492d 4772  om/github/EMI-Gr
-000023c0: 6f75 702f 6576 6f78 2f62 6c6f 622f 6d61  oup/evox/blob/ma
-000023d0: 696e 2f64 6f63 732f 736f 7572 6365 2f65  in/docs/source/e
-000023e0: 7861 6d70 6c65 2f70 736f 5f61 636b 6c65  xample/pso_ackle
-000023f0: 792e 6970 796e 6229 207c 0a7c 204e 6575  y.ipynb) |.| Neu
-00002400: 726f 6576 6f6c 7574 696f 6e20 7769 7468  roevolution with
-00002410: 2047 796d 207c 205b 215b 4f70 656e 2069   Gym | [![Open i
-00002420: 6e20 436f 6c61 625d 2868 7474 7073 3a2f  n Colab](https:/
-00002430: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00002440: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
-00002450: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
-00002460: 6729 5d28 6874 7470 733a 2f2f 636f 6c61  g)](https://cola
-00002470: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00002480: 652e 636f 6d2f 6769 7468 7562 2f45 4d49  e.com/github/EMI
-00002490: 2d47 726f 7570 2f65 766f 782f 626c 6f62  -Group/evox/blob
-000024a0: 2f6d 6169 6e2f 646f 6373 2f73 6f75 7263  /main/docs/sourc
-000024b0: 652f 6578 616d 706c 652f 6779 6d5f 636c  e/example/gym_cl
-000024c0: 6173 7369 635f 636f 6e74 726f 6c2e 6970  assic_control.ip
-000024d0: 796e 6229 207c 0a7c 204e 6575 726f 6576  ynb) |.| Neuroev
-000024e0: 6f6c 7574 696f 6e20 7769 7468 2042 7261  olution with Bra
-000024f0: 7820 7c20 5b21 5b4f 7065 6e20 696e 2043  x | [![Open in C
-00002500: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
-00002510: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002520: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00002530: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
-00002540: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00002550: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00002560: 6f6d 2f67 6974 6875 622f 454d 492d 4772  om/github/EMI-Gr
-00002570: 6f75 702f 6576 6f78 2f62 6c6f 622f 6d61  oup/evox/blob/ma
-00002580: 696e 2f64 6f63 732f 736f 7572 6365 2f67  in/docs/source/g
-00002590: 7569 6465 2f62 6173 6963 732f 322d 7072  uide/basics/2-pr
-000025a0: 6f62 6c65 6d73 2e69 7079 6e62 2920 7c0a  oblems.ipynb) |.
-000025b0: 7c20 4375 7374 6f6d 2041 6c67 6f72 6974  | Custom Algorit
-000025c0: 686d 2f50 726f 626c 656d 207c 205b 215b  hm/Problem | [![
-000025d0: 4f70 656e 2069 6e20 436f 6c61 625d 2868  Open in Colab](h
-000025e0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-000025f0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00002600: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00002610: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00002620: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00002630: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00002640: 7562 2f45 4d49 2d47 726f 7570 2f65 766f  ub/EMI-Group/evo
-00002650: 782f 626c 6f62 2f6d 6169 6e2f 646f 6373  x/blob/main/docs
-00002660: 2f73 6f75 7263 652f 6578 616d 706c 652f  /source/example/
-00002670: 6375 7374 6f6d 5f61 6c67 6f72 6974 686d  custom_algorithm
-00002680: 5f61 6e64 5f70 726f 626c 656d 2e69 7079  _and_problem.ipy
-00002690: 6e62 2920 7c0a 0a46 6f72 206d 6f72 6520  nb) |..For more 
-000026a0: 7573 652d 6361 7365 7320 616e 6420 6170  use-cases and ap
-000026b0: 706c 6963 6174 696f 6e73 2c20 706c 6561  plications, plea
-000026c0: 6520 6368 6563 6b20 6f75 7420 5b45 7861  e check out [Exa
-000026d0: 6d70 6c65 2044 6972 6563 746f 7279 5d28  mple Directory](
-000026e0: 6874 7470 733a 2f2f 6576 6f78 2e72 6561  https://evox.rea
-000026f0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00002700: 6174 6573 742f 6578 616d 706c 652f 696e  atest/example/in
-00002710: 6465 782e 6874 6d6c 292e 0a0a 2323 2043  dex.html)...## C
-00002720: 6f6d 6d75 6e69 7479 2026 2053 7570 706f  ommunity & Suppo
-00002730: 7274 0a0a 2d20 456e 6761 6765 2069 6e20  rt..- Engage in 
-00002740: 6469 7363 7573 7369 6f6e 7320 616e 6420  discussions and 
-00002750: 7368 6172 6520 796f 7572 2065 7870 6572  share your exper
-00002760: 6965 6e63 6573 206f 6e20 5b47 6974 4875  iences on [GitHu
-00002770: 6220 4469 7363 7573 7369 6f6e 2042 6f61  b Discussion Boa
-00002780: 7264 5d28 6874 7470 733a 2f2f 6769 7468  rd](https://gith
-00002790: 7562 2e63 6f6d 2f45 4d49 2d47 726f 7570  ub.com/EMI-Group
-000027a0: 2f65 766f 782f 6469 7363 7573 7369 6f6e  /evox/discussion
-000027b0: 7329 2e0a 2d20 4a6f 696e 206f 7572 2051  s)..- Join our Q
-000027c0: 5120 6772 6f75 7020 2849 443a 2032 3937  Q group (ID: 297
-000027d0: 3936 3937 3137 292e 0a2d 2048 656c 7020  969717)..- Help 
-000027e0: 7769 7468 2074 6865 2074 7261 6e73 6c61  with the transla
-000027f0: 7469 6f6e 206f 6620 7468 6520 646f 6375  tion of the docu
-00002800: 6d65 6e74 6174 696f 6e20 6f6e 205b 5765  mentation on [We
-00002810: 626c 6174 655d 2868 7474 7073 3a2f 2f68  blate](https://h
-00002820: 6f73 7465 642e 7765 626c 6174 652e 6f72  osted.weblate.or
-00002830: 672f 7072 6f6a 6563 7473 2f65 766f 782f  g/projects/evox/
-00002840: 6576 6f78 2f29 2e0a 5765 2063 7572 7265  evox/)..We curre
-00002850: 6e74 6c79 2073 7570 706f 7274 2074 7261  ntly support tra
-00002860: 6e73 6c61 7469 6f6e 7320 696e 2074 776f  nslations in two
-00002870: 206c 616e 6775 6167 6573 2c20 5b45 6e67   languages, [Eng
-00002880: 6c69 7368 5d28 6874 7470 733a 2f2f 6576  lish](https://ev
-00002890: 6f78 2e72 6561 6474 6865 646f 6373 2e69  ox.readthedocs.i
-000028a0: 6f2f 656e 2f6c 6174 6573 742f 2920 2f20  o/en/latest/) / 
-000028b0: 5be4 b8ad e696 875d 2868 7474 7073 3a2f  [......](https:/
-000028c0: 2f65 766f 782e 7265 6164 7468 6564 6f63  /evox.readthedoc
-000028d0: 732e 696f 2f7a 682f 6c61 7465 7374 2f29  s.io/zh/latest/)
-000028e0: 2e0a 2d20 4f66 6669 6369 616c 2057 6562  ..- Official Web
-000028f0: 7369 7465 3a20 6874 7470 733a 2f2f 6576  site: https://ev
-00002900: 6f78 2e67 726f 7570 2f0a 0a23 2320 5369  ox.group/..## Si
-00002910: 7374 6572 2050 726f 6a65 6374 730a 0a2d  ster Projects..-
-00002920: 2045 766f 5842 656e 6368 3a20 4120 6265   EvoXBench: A be
-00002930: 6e63 686d 6172 6b20 706c 6174 666f 726d  nchmark platform
-00002940: 2066 6f72 204e 6575 7261 6c20 4172 6368   for Neural Arch
-00002950: 6974 6563 7574 7265 2053 6561 7263 6820  itecutre Search 
-00002960: 284e 4153 2920 7769 7468 6f75 7420 7468  (NAS) without th
-00002970: 6520 7265 7175 6972 656d 656e 7420 6f66  e requirement of
-00002980: 2047 5055 732f 5079 546f 7263 682f 5465   GPUs/PyTorch/Te
-00002990: 6e73 6f72 666c 6f77 2c20 7375 7070 6f72  nsorflow, suppor
-000029a0: 7469 6e67 2076 6172 696f 7573 2070 726f  ting various pro
-000029b0: 6772 616d 6d69 6e67 206c 616e 6775 6167  gramming languag
-000029c0: 6573 2073 7563 6820 6173 204a 6176 612c  es such as Java,
-000029d0: 204d 6174 6c61 622c 2050 7974 686f 6e2c   Matlab, Python,
-000029e0: 2065 6374 2e20 4368 6563 6b20 6f75 7420   ect. Check out 
-000029f0: 5b68 6572 655d 2868 7474 7073 3a2f 2f67  [here](https://g
-00002a00: 6974 6875 622e 636f 6d2f 454d 492d 4772  ithub.com/EMI-Gr
-00002a10: 6f75 702f 6576 6f78 6265 6e63 6829 2e0a  oup/evoxbench)..
-00002a20: 0a23 2320 4369 7469 6e67 2045 766f 580a  .## Citing EvoX.
-00002a30: 0a49 6620 796f 7520 7573 6520 4576 6f58  .If you use EvoX
-00002a40: 2069 6e20 796f 7572 2072 6573 6561 7263   in your researc
-00002a50: 6820 616e 6420 7761 6e74 2074 6f20 6369  h and want to ci
-00002a60: 7465 2069 7420 696e 2079 6f75 7220 776f  te it in your wo
-00002a70: 726b 2c20 706c 6561 7365 2075 7365 3a0a  rk, please use:.
-00002a80: 6060 600a 4061 7274 6963 6c65 7b65 766f  ```.@article{evo
-00002a90: 782c 0a20 2074 6974 6c65 203d 207b 7b45  x,.  title = {{E
-00002aa0: 766f 587d 3a20 7b41 7d20 7b44 6973 7472  voX}: {A} {Distr
-00002ab0: 6962 7574 6564 7d20 7b47 5055 7d2d 6163  ibuted} {GPU}-ac
-00002ac0: 6365 6c65 7261 7465 6420 7b46 7261 6d65  celerated {Frame
-00002ad0: 776f 726b 7d20 666f 7220 7b53 6361 6c61  work} for {Scala
-00002ae0: 626c 657d 207b 4576 6f6c 7574 696f 6e61  ble} {Evolutiona
-00002af0: 7279 7d20 7b43 6f6d 7075 7461 7469 6f6e  ry} {Computation
-00002b00: 7d7d 2c0a 2020 6175 7468 6f72 203d 207b  }},.  author = {
-00002b10: 4875 616e 672c 2042 6569 6368 656e 2061  Huang, Beichen a
-00002b20: 6e64 2043 6865 6e67 2c20 5261 6e20 616e  nd Cheng, Ran an
-00002b30: 6420 4c69 2c20 5a68 756f 7a68 616f 2061  d Li, Zhuozhao a
-00002b40: 6e64 204a 696e 2c20 5961 6f63 6875 2061  nd Jin, Yaochu a
-00002b50: 6e64 2054 616e 2c20 4b61 7920 4368 656e  nd Tan, Kay Chen
-00002b60: 7d2c 0a20 206a 6f75 726e 616c 203d 207b  },.  journal = {
-00002b70: 4945 4545 2054 7261 6e73 6163 7469 6f6e  IEEE Transaction
-00002b80: 7320 6f6e 2045 766f 6c75 7469 6f6e 6172  s on Evolutionar
-00002b90: 7920 436f 6d70 7574 6174 696f 6e7d 2c0a  y Computation},.
-00002ba0: 2020 7965 6172 203d 2032 3032 342c 0a20    year = 2024,. 
-00002bb0: 2064 6f69 203d 207b 3130 2e31 3130 392f   doi = {10.1109/
-00002bc0: 5445 5643 2e32 3032 342e 3333 3838 3535  TEVC.2024.338855
-00002bd0: 307d 0a7d 0a60 6060 0a0a 2323 2053 7461  0}.}.```..## Sta
-00002be0: 7220 4869 7374 6f72 790a 0a5b 215b 5374  r History..[![St
-00002bf0: 6172 2048 6973 746f 7279 2043 6861 7274  ar History Chart
-00002c00: 5d28 6874 7470 733a 2f2f 6170 692e 7374  ](https://api.st
-00002c10: 6172 2d68 6973 746f 7279 2e63 6f6d 2f73  ar-history.com/s
-00002c20: 7667 3f72 6570 6f73 3d45 4d49 2d47 726f  vg?repos=EMI-Gro
-00002c30: 7570 2f65 766f 7826 7479 7065 3d44 6174  up/evox&type=Dat
-00002c40: 6529 5d28 6874 7470 733a 2f2f 7374 6172  e)](https://star
-00002c50: 2d68 6973 746f 7279 2e63 6f6d 2f23 454d  -history.com/#EM
-00002c60: 492d 4772 6f75 702f 6576 6f78 2644 6174  I-Group/evox&Dat
-00002c70: 6529 0a0a 0a0a                           e)....
+00000a70: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
+00000a80: 7569 7265 732d 4469 7374 3a20 7465 6e73  uires-Dist: tens
+00000a90: 6f72 666c 6f77 3e3d 322e 3132 2e30 3b20  orflow>=2.12.0; 
+00000aa0: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
+00000ab0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000ac0: 7669 730a 5265 7175 6972 6573 2d44 6973  vis.Requires-Dis
+00000ad0: 743a 2070 6c6f 746c 793e 3d35 2e30 2e30  t: plotly>=5.0.0
+00000ae0: 3b20 6578 7472 6120 3d3d 2022 7669 7322  ; extra == "vis"
+00000af0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000b00: 7061 6e64 6173 3e3d 322e 302e 303b 2065  pandas>=2.0.0; e
+00000b10: 7874 7261 203d 3d20 2276 6973 220a 5072  xtra == "vis".Pr
+00000b20: 6f76 6964 6573 2d45 7874 7261 3a20 6779  ovides-Extra: gy
+00000b30: 6d6e 6173 6975 6d0a 5265 7175 6972 6573  mnasium.Requires
+00000b40: 2d44 6973 743a 2067 796d 6e61 7369 756d  -Dist: gymnasium
+00000b50: 3e3d 302e 3239 2e30 3b20 6578 7472 6120  >=0.29.0; extra 
+00000b60: 3d3d 2022 6779 6d6e 6173 6975 6d22 0a50  == "gymnasium".P
+00000b70: 726f 7669 6465 732d 4578 7472 613a 2065  rovides-Extra: e
+00000b80: 6e76 706f 6f6c 0a52 6571 7569 7265 732d  nvpool.Requires-
+00000b90: 4469 7374 3a20 656e 7670 6f6f 6c3e 3d30  Dist: envpool>=0
+00000ba0: 2e38 2e30 3b20 6578 7472 6120 3d3d 2022  .8.0; extra == "
+00000bb0: 656e 7670 6f6f 6c22 0a50 726f 7669 6465  envpool".Provide
+00000bc0: 732d 4578 7472 613a 206e 6575 726f 6576  s-Extra: neuroev
+00000bd0: 6f6c 7574 696f 6e0a 5265 7175 6972 6573  olution.Requires
+00000be0: 2d44 6973 743a 2074 656e 736f 7266 6c6f  -Dist: tensorflo
+00000bf0: 772d 6461 7461 7365 7473 3e3d 342e 302e  w-datasets>=4.0.
+00000c00: 303b 2065 7874 7261 203d 3d20 226e 6575  0; extra == "neu
+00000c10: 726f 6576 6f6c 7574 696f 6e22 0a52 6571  roevolution".Req
+00000c20: 7569 7265 732d 4469 7374 3a20 6772 6169  uires-Dist: grai
+00000c30: 6e3e 3d30 2e31 2e30 3b20 6578 7472 6120  n>=0.1.0; extra 
+00000c40: 3d3d 2022 6e65 7572 6f65 766f 6c75 7469  == "neuroevoluti
+00000c50: 6f6e 220a 5265 7175 6972 6573 2d44 6973  on".Requires-Dis
+00000c60: 743a 2062 7261 783e 3d30 2e31 2e30 3b20  t: brax>=0.1.0; 
+00000c70: 6578 7472 6120 3d3d 2022 6e65 7572 6f65  extra == "neuroe
+00000c80: 766f 6c75 7469 6f6e 220a 5072 6f76 6964  volution".Provid
+00000c90: 6573 2d45 7874 7261 3a20 6469 7374 7269  es-Extra: distri
+00000ca0: 6275 7465 640a 5265 7175 6972 6573 2d44  buted.Requires-D
+00000cb0: 6973 743a 2072 6179 3e3d 322e 302e 303b  ist: ray>=2.0.0;
+00000cc0: 2065 7874 7261 203d 3d20 2264 6973 7472   extra == "distr
+00000cd0: 6962 7574 6564 220a 5072 6f76 6964 6573  ibuted".Provides
+00000ce0: 2d45 7874 7261 3a20 6675 6c6c 0a52 6571  -Extra: full.Req
+00000cf0: 7569 7265 732d 4469 7374 3a20 6779 6d6e  uires-Dist: gymn
+00000d00: 6173 6975 6d3e 3d30 2e32 392e 303b 2065  asium>=0.29.0; e
+00000d10: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
+00000d20: 6571 7569 7265 732d 4469 7374 3a20 7261  equires-Dist: ra
+00000d30: 793e 3d32 2e30 2e30 3b20 6578 7472 6120  y>=2.0.0; extra 
+00000d40: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000d50: 6573 2d44 6973 743a 2065 6e76 706f 6f6c  es-Dist: envpool
+00000d60: 3e3d 302e 382e 303b 2065 7874 7261 203d  >=0.8.0; extra =
+00000d70: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
+00000d80: 732d 4469 7374 3a20 6770 6a61 783e 3d30  s-Dist: gpjax>=0
+00000d90: 2e38 2e30 3b20 6578 7472 6120 3d3d 2022  .8.0; extra == "
+00000da0: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+00000db0: 6973 743a 2070 6c6f 746c 793e 3d35 2e30  ist: plotly>=5.0
+00000dc0: 2e30 3b20 6578 7472 6120 3d3d 2022 6675  .0; extra == "fu
+00000dd0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000de0: 743a 2070 616e 6461 733e 3d32 2e30 2e30  t: pandas>=2.0.0
+00000df0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+00000e00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000e10: 2074 656e 736f 7266 6c6f 772d 6461 7461   tensorflow-data
+00000e20: 7365 7473 3e3d 342e 302e 303b 2065 7874  sets>=4.0.0; ext
+00000e30: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+00000e40: 7569 7265 732d 4469 7374 3a20 6772 6169  uires-Dist: grai
+00000e50: 6e3e 3d30 2e31 2e30 3b20 6578 7472 6120  n>=0.1.0; extra 
+00000e60: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000e70: 6573 2d44 6973 743a 2062 7261 783e 3d30  es-Dist: brax>=0
+00000e80: 2e31 2e30 3b20 6578 7472 6120 3d3d 2022  .1.0; extra == "
+00000e90: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+00000ea0: 6973 743a 2070 6c6f 746c 793e 3d35 2e30  ist: plotly>=5.0
+00000eb0: 2e30 3b20 6578 7472 6120 3d3d 2022 6675  .0; extra == "fu
+00000ec0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000ed0: 743a 2070 616e 6461 733e 3d32 2e30 2e30  t: pandas>=2.0.0
+00000ee0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+00000ef0: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
+00000f00: 3a20 6770 0a52 6571 7569 7265 732d 4469  : gp.Requires-Di
+00000f10: 7374 3a20 6770 6a61 783e 3d30 2e38 2e30  st: gpjax>=0.8.0
+00000f20: 3b20 6578 7472 6120 3d3d 2022 6770 220a  ; extra == "gp".
+00000f30: 0a3c 6831 2061 6c69 676e 3d22 6365 6e74  .<h1 align="cent
+00000f40: 6572 223e 0a20 203c 7069 6374 7572 653e  er">.  <picture>
+00000f50: 0a20 2020 203c 736f 7572 6365 206d 6564  .    <source med
+00000f60: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
+00000f70: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
+00000f80: 2220 7372 6373 6574 3d22 646f 6373 2f73  " srcset="docs/s
+00000f90: 6f75 7263 652f 5f73 7461 7469 632f 6576  ource/_static/ev
+00000fa0: 6f78 5f6c 6f67 6f5f 6461 726b 2e70 6e67  ox_logo_dark.png
+00000fb0: 223e 0a20 2020 203c 736f 7572 6365 206d  ">.    <source m
+00000fc0: 6564 6961 3d22 2870 7265 6665 7273 2d63  edia="(prefers-c
+00000fd0: 6f6c 6f72 2d73 6368 656d 653a 206c 6967  olor-scheme: lig
+00000fe0: 6874 2922 2073 7263 7365 743d 2264 6f63  ht)" srcset="doc
+00000ff0: 732f 736f 7572 6365 2f5f 7374 6174 6963  s/source/_static
+00001000: 2f65 766f 785f 6c6f 676f 5f6c 6967 6874  /evox_logo_light
+00001010: 2e70 6e67 223e 0a20 2020 203c 696d 6720  .png">.    <img 
+00001020: 616c 743d 2245 766f 5820 4c6f 676f 2220  alt="EvoX Logo" 
+00001030: 6865 6967 6874 3d22 3132 3822 2077 6964  height="128" wid
+00001040: 7468 3d22 3530 3070 7822 2073 7263 3d22  th="500px" src="
+00001050: 646f 6373 2f73 6f75 7263 652f 5f73 7461  docs/source/_sta
+00001060: 7469 632f 6576 6f78 5f6c 6f67 6f5f 6c69  tic/evox_logo_li
+00001070: 6768 742e 706e 6722 3e0a 2020 3c2f 7069  ght.png">.  </pi
+00001080: 6374 7572 653e 0a3c 2f68 313e 0a0a 3c70  cture>.</h1>..<p
+00001090: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000010a0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000010b0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000010c0: 732f 3233 3031 2e31 3234 3537 223e 0a20  s/2301.12457">. 
+000010d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000010e0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000010f0: 2e69 6f2f 6261 6467 652f 7061 7065 722d  .io/badge/paper-
+00001100: 6172 7869 762d 7265 643f 7374 796c 653d  arxiv-red?style=
+00001110: 666f 722d 7468 652d 6261 6467 6522 2061  for-the-badge" a
+00001120: 6c74 3d22 4576 6f58 2050 6170 6572 206f  lt="EvoX Paper o
+00001130: 6e20 6172 5869 7622 3e0a 2020 3c2f 613e  n arXiv">.  </a>
+00001140: 0a0a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+00001150: 7073 3a2f 2f65 766f 782e 7265 6164 7468  ps://evox.readth
+00001160: 6564 6f63 732e 696f 2f22 3e0a 2020 2020  edocs.io/">.    
+00001170: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001180: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001190: 2f62 6164 6765 2f64 6f63 732d 7265 6164  /badge/docs-read
+000011a0: 7468 6564 6f63 732d 626c 7565 3f73 7479  thedocs-blue?sty
+000011b0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+000011c0: 2220 616c 743d 2245 766f 5820 446f 6375  " alt="EvoX Docu
+000011d0: 6d65 6e74 6174 696f 6e22 3e0a 2020 3c2f  mentation">.  </
+000011e0: 613e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  a>.</p>..<p alig
+000011f0: 6e3d 2263 656e 7465 7222 3e0a 2020 3c62  n="center">.  <b
+00001200: 3ef0 9f8c 9f44 6973 7472 6962 7574 6564  >....Distributed
+00001210: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
+00001220: 2046 7261 6d65 776f 726b 2066 6f72 2053   Framework for S
+00001230: 6361 6c61 626c 6520 4576 6f6c 7574 696f  calable Evolutio
+00001240: 6e61 7279 2043 6f6d 7075 7461 7469 6f6e  nary Computation
+00001250: f09f 8c9f 3c2f 623e 0a3c 2f70 3e0a 0a2d  ....</b>.</p>..-
+00001260: 2d2d 0a0a 2323 0a42 7569 6c64 696e 6720  --..##.Building 
+00001270: 7570 6f6e 205b 4a41 585d 2868 7474 7073  upon [JAX](https
+00001280: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
+00001290: 6f67 6c65 2f6a 6178 2920 616e 6420 5b52  ogle/jax) and [R
+000012a0: 6179 5d28 6874 7470 733a 2f2f 6769 7468  ay](https://gith
+000012b0: 7562 2e63 6f6d 2f72 6179 2d70 726f 6a65  ub.com/ray-proje
+000012c0: 6374 2f72 6179 292c 2045 766f 5820 6f66  ct/ray), EvoX of
+000012d0: 6665 7273 2061 2063 6f6d 7072 6568 656e  fers a comprehen
+000012e0: 7369 7665 2073 7569 7465 206f 6620 2a2a  sive suite of **
+000012f0: 3530 2b20 4576 6f6c 7574 696f 6e61 7279  50+ Evolutionary
+00001300: 2041 6c67 6f72 6974 686d 7320 2845 4173   Algorithms (EAs
+00001310: 292a 2a20 616e 6420 6120 7769 6465 2072  )** and a wide r
+00001320: 616e 6765 206f 6620 2a2a 3130 302b 2042  ange of **100+ B
+00001330: 656e 6368 6d61 726b 2050 726f 626c 656d  enchmark Problem
+00001340: 732a 2a2c 2061 6c6c 2062 656e 6566 6974  s**, all benefit
+00001350: 696e 6720 6672 6f6d 2064 6973 7472 6962  ing from distrib
+00001360: 7574 6564 2047 5055 2d61 6363 656c 6572  uted GPU-acceler
+00001370: 6174 696f 6e2e 2049 7420 6661 6369 6c69  ation. It facili
+00001380: 7461 7465 7320 6566 6669 6369 656e 7420  tates efficient 
+00001390: 6578 706c 6f72 6174 696f 6e20 6f66 2063  exploration of c
+000013a0: 6f6d 706c 6578 206f 7074 696d 697a 6174  omplex optimizat
+000013b0: 696f 6e20 6c61 6e64 7363 6170 6573 2c20  ion landscapes, 
+000013c0: 6566 6665 6374 6976 6520 7461 636b 6c69  effective tackli
+000013d0: 6e67 206f 6620 626c 6163 6b2d 626f 7820  ng of black-box 
+000013e0: 6f70 7469 6d69 7a61 7469 6f6e 2063 6861  optimization cha
+000013f0: 6c6c 656e 6765 732c 2061 6e64 2064 6565  llenges, and dee
+00001400: 7020 6469 7665 7320 696e 746f 206e 6575  p dives into neu
+00001410: 726f 6576 6f6c 7574 696f 6e20 7769 7468  roevolution with
+00001420: 205b 4272 6178 5d28 6874 7470 733a 2f2f   [Brax](https://
+00001430: 6769 7468 7562 2e63 6f6d 2f67 6f6f 676c  github.com/googl
+00001440: 652f 6272 6178 292e 2057 6974 6820 6120  e/brax). With a 
+00001450: 666f 756e 6461 7469 6f6e 2069 6e20 6675  foundation in fu
+00001460: 6e63 7469 6f6e 616c 2070 726f 6772 616d  nctional program
+00001470: 6d69 6e67 2061 6e64 2068 6965 7261 7263  ming and hierarc
+00001480: 6869 6361 6c20 7374 6174 6520 6d61 6e61  hical state mana
+00001490: 6765 6d65 6e74 2c20 4576 6f58 206f 6666  gement, EvoX off
+000014a0: 6572 7320 6120 7573 6572 2d66 7269 656e  ers a user-frien
+000014b0: 646c 7920 616e 6420 6d6f 6475 6c61 7220  dly and modular 
+000014c0: 6578 7065 7269 656e 6365 2e20 466f 7220  experience. For 
+000014d0: 6d6f 7265 2064 6574 6169 6c73 2c20 706c  more details, pl
+000014e0: 6561 7365 2072 6566 6572 2074 6f20 6f75  ease refer to ou
+000014f0: 7220 5b50 6170 6572 5d28 6874 7470 733a  r [Paper](https:
+00001500: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00001510: 3233 3031 2e31 3234 3537 2920 616e 6420  2301.12457) and 
+00001520: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
+00001530: 6874 7470 733a 2f2f 6576 6f78 2e72 6561  https://evox.rea
+00001540: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001550: 6174 6573 742f 2920 2f20 5be6 9687 e6a1  atest/) / [.....
+00001560: a35d 2868 7474 7073 3a2f 2f65 766f 782e  .](https://evox.
+00001570: 7265 6164 7468 6564 6f63 732e 696f 2f7a  readthedocs.io/z
+00001580: 682f 6c61 7465 7374 2f29 2e0a 0a2d 2d2d  h/latest/)...---
+00001590: 0a0a 2323 204b 6579 2046 6561 7475 7265  ..## Key Feature
+000015a0: 730a 0a2d 20f0 9f9a 8020 2a2a 4661 7374  s..- .... **Fast
+000015b0: 2050 6572 666f 726d 616e 6365 2a2a 3a0a   Performance**:.
+000015c0: 2020 2d20 4578 7065 7269 656e 6365 202a    - Experience *
+000015d0: 2a47 5055 2d41 6363 656c 6572 6174 6564  *GPU-Accelerated
+000015e0: 2a2a 206f 7074 696d 697a 6174 696f 6e2c  ** optimization,
+000015f0: 2061 6368 6965 7669 6e67 2073 7065 6564   achieving speed
+00001600: 7320 6f76 6572 2031 3030 7820 6661 7374  s over 100x fast
+00001610: 6572 2074 6861 6e20 7472 6164 6974 696f  er than traditio
+00001620: 6e61 6c20 6d65 7468 6f64 732e 0a20 202d  nal methods..  -
+00001630: 204c 6576 6572 6167 6520 7468 6520 706f   Leverage the po
+00001640: 7765 7220 6f66 202a 2a44 6973 7472 6962  wer of **Distrib
+00001650: 7574 6564 2057 6f72 6b66 6c6f 7773 2a2a  uted Workflows**
+00001660: 2066 6f72 2065 7665 6e20 6d6f 7265 2072   for even more r
+00001670: 6170 6964 206f 7074 696d 697a 6174 696f  apid optimizatio
+00001680: 6e2e 0a0a 2d20 f09f 8c90 202a 2a56 6572  n...- .... **Ver
+00001690: 7361 7469 6c65 204f 7074 696d 697a 6174  satile Optimizat
+000016a0: 696f 6e20 5375 6974 652a 2a3a 0a20 202d  ion Suite**:.  -
+000016b0: 2043 6174 6572 2074 6f20 616c 6c20 796f   Cater to all yo
+000016c0: 7572 206e 6565 6473 2077 6974 6820 626f  ur needs with bo
+000016d0: 7468 202a 2a53 696e 676c 652d 6f62 6a65  th **Single-obje
+000016e0: 6374 6976 652a 2a20 616e 6420 2a2a 4d75  ctive** and **Mu
+000016f0: 6c74 692d 6f62 6a65 6374 6976 652a 2a20  lti-objective** 
+00001700: 6f70 7469 6d69 7a61 7469 6f6e 2063 6170  optimization cap
+00001710: 6162 696c 6974 6965 732e 0a20 202d 2044  abilities..  - D
+00001720: 6976 6520 696e 746f 2061 2063 6f6d 7072  ive into a compr
+00001730: 6568 656e 7369 7665 206c 6962 7261 7279  ehensive library
+00001740: 206f 6620 2a2a 4265 6e63 686d 6172 6b20   of **Benchmark 
+00001750: 5072 6f62 6c65 6d73 2a2a 2c20 656e 7375  Problems**, ensu
+00001760: 7269 6e67 2072 6f62 7573 7420 7465 7374  ring robust test
+00001770: 696e 6720 616e 6420 6576 616c 7561 7469  ing and evaluati
+00001780: 6f6e 2e0a 2020 2d20 4578 706c 6f72 6520  on..  - Explore 
+00001790: 7468 6520 6672 6f6e 7469 6572 206f 6620  the frontier of 
+000017a0: 4149 2077 6974 6820 6578 7465 6e73 6976  AI with extensiv
+000017b0: 6520 746f 6f6c 7320 666f 7220 2a2a 4e65  e tools for **Ne
+000017c0: 7572 6f65 766f 6c75 7469 6f6e 2a2a 2074  uroevolution** t
+000017d0: 6173 6b73 2e0a 0a2d 20f0 9f9b a0ef b88f  asks...- .......
+000017e0: 202a 2a44 6573 6967 6e65 6420 666f 7220   **Designed for 
+000017f0: 5369 6d70 6c69 6369 7479 2a2a 3a0a 2020  Simplicity**:.  
+00001800: 2d20 456d 6272 6163 6520 7468 6520 656c  - Embrace the el
+00001810: 6567 616e 6365 206f 6620 2a2a 4675 6e63  egance of **Func
+00001820: 7469 6f6e 616c 2050 726f 6772 616d 6d69  tional Programmi
+00001830: 6e67 2a2a 2c20 7369 6d70 6c69 6679 696e  ng**, simplifyin
+00001840: 6720 636f 6d70 6c65 7820 616c 676f 7269  g complex algori
+00001850: 7468 6d69 6320 636f 6d70 6f73 6974 696f  thmic compositio
+00001860: 6e73 2e0a 2020 2d20 4265 6e65 6669 7420  ns..  - Benefit 
+00001870: 6672 6f6d 202a 2a48 6965 7261 7263 6869  from **Hierarchi
+00001880: 6361 6c20 5374 6174 6520 4d61 6e61 6765  cal State Manage
+00001890: 6d65 6e74 2a2a 2c20 656e 7375 7269 6e67  ment**, ensuring
+000018a0: 206d 6f64 756c 6172 2061 6e64 2063 6c65   modular and cle
+000018b0: 616e 2070 726f 6772 616d 6d69 6e67 2e0a  an programming..
+000018c0: 2020 2d20 4a75 6d70 7374 6172 7420 796f    - Jumpstart yo
+000018d0: 7572 206a 6f75 726e 6579 2077 6974 6820  ur journey with 
+000018e0: 6f75 7220 5b44 6574 6169 6c65 6420 5475  our [Detailed Tu
+000018f0: 746f 7269 616c 5d28 6874 7470 733a 2f2f  torial](https://
+00001900: 6576 6f78 2e72 6561 6474 6865 646f 6373  evox.readthedocs
+00001910: 2e69 6f2f 656e 2f6c 6174 6573 742f 6775  .io/en/latest/gu
+00001920: 6964 652f 6261 7369 6373 2f69 6e64 6578  ide/basics/index
+00001930: 2e68 746d 6c29 2e0a 0a2d 2d2d 0a0a 2323  .html)...---..##
+00001940: 2043 6f6d 7072 6568 656e 7369 7665 2045   Comprehensive E
+00001950: 766f 6c75 7469 6f6e 6172 7920 416c 676f  volutionary Algo
+00001960: 7269 7468 6d73 0a0a 2323 2320 5369 6e67  rithms..### Sing
+00001970: 6c65 2d4f 626a 6563 7469 7665 204f 7074  le-Objective Opt
+00001980: 696d 697a 6174 696f 6e0a 0a7c 2043 6174  imization..| Cat
+00001990: 6567 6f72 7920 2020 2020 2020 2020 2020  egory           
+000019a0: 2020 2020 2020 2020 207c 2041 6c67 6f72           | Algor
+000019b0: 6974 686d 204e 616d 6573 2020 2020 2020  ithm Names      
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 207c 0a7c 202d 2d2d 2d2d         |.| -----
+000019e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019f0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a20: 2d2d 2d20 7c0a 7c20 4469 6666 6572 656e  --- |.| Differen
+00001a30: 7469 616c 2045 766f 6c75 7469 6f6e 2020  tial Evolution  
+00001a40: 2020 2020 7c20 436f 4445 2c20 4a61 4445      | CoDE, JaDE
+00001a50: 2c20 5361 4445 2c20 5348 4144 452c 2049  , SaDE, SHADE, I
+00001a60: 4d4f 4445 2c20 2e2e 2e20 2020 2020 2020  MODE, ...       
+00001a70: 207c 0a7c 2045 766f 6c75 7469 6f6e 2053   |.| Evolution S
+00001a80: 7472 6174 6567 7920 2020 2020 2020 207c  trategy        |
+00001a90: 2043 4d41 2d45 532c 2050 4750 452c 204f   CMA-ES, PGPE, O
+00001aa0: 7065 6e45 532c 2043 522d 464d 2d4e 4553  penES, CR-FM-NES
+00001ab0: 2c20 784e 4553 2c20 2e2e 2e20 7c0a 7c20  , xNES, ... |.| 
+00001ac0: 5061 7274 6963 6c65 2053 7761 726d 204f  Particle Swarm O
+00001ad0: 7074 696d 697a 6174 696f 6e20 7c20 4649  ptimization | FI
+00001ae0: 5053 2c20 4353 4f2c 2043 5053 4f2c 2043  PS, CSO, CPSO, C
+00001af0: 4c50 534f 2c20 534c 2d50 534f 2c20 2e2e  LPSO, SL-PSO, ..
+00001b00: 2e20 2020 2020 2020 207c 0a0a 2323 2320  .        |..### 
+00001b10: 4d75 6c74 692d 4f62 6a65 6374 6976 6520  Multi-Objective 
+00001b20: 4f70 7469 6d69 7a61 7469 6f6e 0a0a 7c20  Optimization..| 
+00001b30: 4361 7465 676f 7279 2020 2020 2020 2020  Category        
+00001b40: 2020 207c 2041 6c67 6f72 6974 686d 204e     | Algorithm N
+00001b50: 616d 6573 2020 2020 2020 2020 2020 2020  ames            
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2020 2020 207c 0a7c 202d 2d2d 2d2d 2d2d       |.| -------
+00001b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
+00001bc0: 2044 6f6d 696e 616e 6365 2d62 6173 6564   Dominance-based
+00001bd0: 2020 2020 7c20 4e53 4741 2d49 492c 204e      | NSGA-II, N
+00001be0: 5347 412d 4949 492c 2053 5045 4132 2c20  SGA-III, SPEA2, 
+00001bf0: 4269 4745 2c20 4b6e 4541 2c20 2e2e 2e20  BiGE, KnEA, ... 
+00001c00: 2020 2020 207c 0a7c 2044 6563 6f6d 706f       |.| Decompo
+00001c10: 7369 7469 6f6e 2d62 6173 6564 7c20 4d4f  sition-based| MO
+00001c20: 4541 2f44 2c20 5256 4541 2c20 742d 4445  EA/D, RVEA, t-DE
+00001c30: 412c 204d 4f45 4144 2d4d 324d 2c20 4541  A, MOEAD-M2M, EA
+00001c40: 472d 4d4f 4541 442c 202e 2e2e 207c 0a7c  G-MOEAD, ... |.|
+00001c50: 2049 6e64 6963 6174 6f72 2d62 6173 6564   Indicator-based
+00001c60: 2020 2020 7c20 4942 4541 2c20 4879 7045      | IBEA, HypE
+00001c70: 2c20 5352 412c 204d 614f 4541 2d49 4744  , SRA, MaOEA-IGD
+00001c80: 2c20 4152 2d4d 4f45 412c 202e 2e2e 2020  , AR-MOEA, ...  
+00001c90: 2020 2020 207c 0a0a 466f 7220 6120 636f       |..For a co
+00001ca0: 6d70 7265 6865 6e73 6976 6520 6c69 7374  mprehensive list
+00001cb0: 2061 6e64 2066 7572 7468 6572 2064 6574   and further det
+00001cc0: 6169 6c73 206f 6620 616c 6c20 616c 676f  ails of all algo
+00001cd0: 7269 7468 6d73 2c20 706c 6561 7365 2063  rithms, please c
+00001ce0: 6865 636b 2074 6865 205b 4150 4920 446f  heck the [API Do
+00001cf0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001d00: 7073 3a2f 2f65 766f 782e 7265 6164 7468  ps://evox.readth
+00001d10: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001d20: 7374 2f61 7069 2f61 6c67 6f72 6974 686d  st/api/algorithm
+00001d30: 732f 696e 6465 782e 6874 6d6c 292e 0a0a  s/index.html)...
+00001d40: 2323 2044 6976 6572 7365 2042 656e 6368  ## Diverse Bench
+00001d50: 6d61 726b 2050 726f 626c 656d 730a 0a7c  mark Problems..|
+00001d60: 2043 6174 6567 6f72 7920 2020 2020 207c   Category      |
+00001d70: 2050 726f 626c 656d 204e 616d 6573 2020   Problem Names  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 207c 0a7c 202d 2d2d           |.| ---
+00001da0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00001db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dd0: 2d2d 2d2d 207c 0a7c 204e 756d 6572 6963  ---- |.| Numeric
+00001de0: 616c 2020 2020 207c 2044 544c 5a2c 204c  al     | DTLZ, L
+00001df0: 534d 4f50 2c20 4d61 462c 205a 4454 2c20  SMOP, MaF, ZDT, 
+00001e00: 4345 4327 3232 2c20 202e 2e2e 2020 2020  CEC'22,  ...    
+00001e10: 7c0a 7c20 4e65 7572 6f65 766f 6c75 7469  |.| Neuroevoluti
+00001e20: 6f6e 7c20 4272 6178 2c20 4779 6d2c 2054  on| Brax, Gym, T
+00001e30: 6f72 6368 5669 7369 6f6e 2044 6174 6173  orchVision Datas
+00001e40: 6574 2c20 2e2e 2e20 2020 207c 0a0a 466f  et, ...    |..Fo
+00001e50: 7220 6120 636f 6d70 7265 6865 6e73 6976  r a comprehensiv
+00001e60: 6520 6c69 7374 2061 6e64 2066 7572 7468  e list and furth
+00001e70: 6572 2064 6574 6169 6c73 206f 6620 616c  er details of al
+00001e80: 6c20 6265 6e63 686d 6172 6b20 7072 6f62  l benchmark prob
+00001e90: 6c65 6d73 2c20 706c 6561 7365 2063 6865  lems, please che
+00001ea0: 636b 2074 6865 205b 4150 4920 446f 6375  ck the [API Docu
+00001eb0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00001ec0: 3a2f 2f65 766f 782e 7265 6164 7468 6564  ://evox.readthed
+00001ed0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001ee0: 2f61 7069 2f70 726f 626c 656d 732f 696e  /api/problems/in
+00001ef0: 6465 782e 6874 6d6c 292e 0a0a 0a23 2320  dex.html)....## 
+00001f00: 5365 7474 696e 6720 5570 2045 766f 580a  Setting Up EvoX.
+00001f10: 0a49 6e73 7461 6c6c 2060 6576 6f78 6020  .Install `evox` 
+00001f20: 6566 666f 7274 6c65 7373 6c79 2076 6961  effortlessly via
+00001f30: 2060 7069 7060 3a0a 6060 6062 6173 680a   `pip`:.```bash.
+00001f40: 7069 7020 696e 7374 616c 6c20 6576 6f78  pip install evox
+00001f50: 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a 3a20  .```..**Note**: 
+00001f60: 546f 2069 6e73 7461 6c6c 2045 766f 5820  To install EvoX 
+00001f70: 7769 7468 204a 4158 2061 6e64 2068 6172  with JAX and har
+00001f80: 6477 6172 6520 6163 6365 6c65 7261 7469  dware accelerati
+00001f90: 6f6e 2063 6170 6162 696c 6974 6965 732c  on capabilities,
+00001fa0: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00001fb0: 206f 7572 2063 6f6d 7072 6568 656e 7369   our comprehensi
+00001fc0: 7665 205b 496e 7374 616c 6c61 7469 6f6e  ve [Installation
+00001fd0: 2047 7569 6465 5d28 6874 7470 733a 2f2f   Guide](https://
+00001fe0: 6576 6f78 2e72 6561 6474 6865 646f 6373  evox.readthedocs
+00001ff0: 2e69 6f2f 656e 2f6c 6174 6573 742f 6775  .io/en/latest/gu
+00002000: 6964 652f 696e 7374 616c 6c2e 6874 6d6c  ide/install.html
+00002010: 292e 0a0a 0a23 2320 5175 6963 6b20 5374  )....## Quick St
+00002020: 6172 740a 0a4b 6963 6b73 7461 7274 2079  art..Kickstart y
+00002030: 6f75 7220 6a6f 7572 6e65 7920 7769 7468  our journey with
+00002040: 2045 766f 5820 696e 206a 7573 7420 6120   EvoX in just a 
+00002050: 6665 7720 7369 6d70 6c65 2073 7465 7073  few simple steps
+00002060: 3a0a 312e 202a 2a49 6d70 6f72 7420 6e65  :.1. **Import ne
+00002070: 6365 7373 6172 7920 6d6f 6475 6c65 732a  cessary modules*
+00002080: 2a3a 0a60 6060 7079 7468 6f6e 0a69 6d70  *:.```python.imp
+00002090: 6f72 7420 6576 6f78 0a66 726f 6d20 6576  ort evox.from ev
+000020a0: 6f78 2069 6d70 6f72 7420 616c 676f 7269  ox import algori
+000020b0: 7468 6d73 2c20 7072 6f62 6c65 6d73 2c20  thms, problems, 
+000020c0: 776f 726b 666c 6f77 730a 6060 600a 322e  workflows.```.2.
+000020d0: 202a 2a43 6f6e 6669 6775 7265 2061 6e20   **Configure an 
+000020e0: 616c 676f 7269 7468 6d20 616e 6420 6465  algorithm and de
+000020f0: 6669 6e65 2061 2070 726f 626c 656d 2a2a  fine a problem**
+00002100: 3a0a 6060 6070 7974 686f 6e0a 7073 6f20  :.```python.pso 
+00002110: 3d20 616c 676f 7269 7468 6d73 2e50 534f  = algorithms.PSO
+00002120: 280a 2020 2020 6c62 3d6a 6e70 2e66 756c  (.    lb=jnp.ful
+00002130: 6c28 7368 6170 653d 2832 2c29 2c20 6669  l(shape=(2,), fi
+00002140: 6c6c 5f76 616c 7565 3d2d 3332 292c 0a20  ll_value=-32),. 
+00002150: 2020 2075 623d 6a6e 702e 6675 6c6c 2873     ub=jnp.full(s
+00002160: 6861 7065 3d28 322c 292c 2066 696c 6c5f  hape=(2,), fill_
+00002170: 7661 6c75 653d 3332 292c 0a20 2020 2070  value=32),.    p
+00002180: 6f70 5f73 697a 653d 3130 302c 0a29 0a61  op_size=100,.).a
+00002190: 636b 6c65 7920 3d20 7072 6f62 6c65 6d73  ckley = problems
+000021a0: 2e6e 756d 6572 6963 616c 2e41 636b 6c65  .numerical.Ackle
+000021b0: 7928 290a 6060 600a 332e 202a 2a43 6f6d  y().```.3. **Com
+000021c0: 706f 7365 2061 6e64 2069 6e69 7469 616c  pose and initial
+000021d0: 697a 6520 7468 6520 776f 726b 666c 6f77  ize the workflow
+000021e0: 2a2a 3a0a 6060 6070 7974 686f 6e0a 776f  **:.```python.wo
+000021f0: 726b 666c 6f77 203d 2077 6f72 6b66 6c6f  rkflow = workflo
+00002200: 7773 2e53 7464 576f 726b 666c 6f77 2870  ws.StdWorkflow(p
+00002210: 736f 2c20 6163 6b6c 6579 290a 6b65 7920  so, ackley).key 
+00002220: 3d20 6a61 782e 7261 6e64 6f6d 2e50 524e  = jax.random.PRN
+00002230: 474b 6579 2834 3229 0a73 7461 7465 203d  GKey(42).state =
+00002240: 2077 6f72 6b66 6c6f 772e 696e 6974 286b   workflow.init(k
+00002250: 6579 290a 6060 600a 342e 202a 2a52 756e  ey).```.4. **Run
+00002260: 2074 6865 2077 6f72 6b66 6c6f 772a 2a3a   the workflow**:
+00002270: 0a60 6060 7079 7468 6f6e 0a23 2045 7865  .```python.# Exe
+00002280: 6375 7465 2074 6865 2077 6f72 6b66 6c6f  cute the workflo
+00002290: 7720 666f 7220 3130 3020 6974 6572 6174  w for 100 iterat
+000022a0: 696f 6e73 0a66 6f72 2069 2069 6e20 7261  ions.for i in ra
+000022b0: 6e67 6528 3130 3029 3a0a 2020 2020 7374  nge(100):.    st
+000022c0: 6174 6520 3d20 776f 726b 666c 6f77 2e73  ate = workflow.s
+000022d0: 7465 7028 7374 6174 6529 0a60 6060 0a0a  tep(state).```..
+000022e0: 2323 2055 7365 2d63 6173 6573 2061 6e64  ## Use-cases and
+000022f0: 2041 7070 6c69 6361 7469 6f6e 730a 0a54   Applications..T
+00002300: 7279 206f 7574 2072 6561 6479 2d74 6f2d  ry out ready-to-
+00002310: 706c 6179 2065 7861 6d70 6c65 7320 696e  play examples in
+00002320: 2079 6f75 7220 6272 6f77 7365 7220 7769   your browser wi
+00002330: 7468 2043 6f6c 6162 3a0a 0a7c 2045 7861  th Colab:..| Exa
+00002340: 6d70 6c65 207c 204c 696e 6b20 7c0a 7c20  mple | Link |.| 
+00002350: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 207c  ------- | ---- |
+00002360: 0a7c 2042 6173 6963 2055 7361 6765 207c  .| Basic Usage |
+00002370: 205b 215b 4f70 656e 2069 6e20 436f 6c61   [![Open in Cola
+00002380: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
+00002390: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000023a0: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+000023b0: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
+000023c0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+000023d0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+000023e0: 6769 7468 7562 2f45 4d49 2d47 726f 7570  github/EMI-Group
+000023f0: 2f65 766f 782f 626c 6f62 2f6d 6169 6e2f  /evox/blob/main/
+00002400: 646f 6373 2f73 6f75 7263 652f 6775 6964  docs/source/guid
+00002410: 652f 6261 7369 6373 2f31 2d73 7461 7274  e/basics/1-start
+00002420: 2e69 7079 6e62 2920 7c0a 7c20 4e75 6d65  .ipynb) |.| Nume
+00002430: 7269 6361 6c20 4f70 7469 6d69 7a61 7469  rical Optimizati
+00002440: 6f6e 207c 205b 215b 4f70 656e 2069 6e20  on | [![Open in 
+00002450: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00002460: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00002470: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00002480: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
+00002490: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+000024a0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+000024b0: 636f 6d2f 6769 7468 7562 2f45 4d49 2d47  com/github/EMI-G
+000024c0: 726f 7570 2f65 766f 782f 626c 6f62 2f6d  roup/evox/blob/m
+000024d0: 6169 6e2f 646f 6373 2f73 6f75 7263 652f  ain/docs/source/
+000024e0: 6578 616d 706c 652f 7073 6f5f 6163 6b6c  example/pso_ackl
+000024f0: 6579 2e69 7079 6e62 2920 7c0a 7c20 4e65  ey.ipynb) |.| Ne
+00002500: 7572 6f65 766f 6c75 7469 6f6e 2077 6974  uroevolution wit
+00002510: 6820 4779 6d20 7c20 5b21 5b4f 7065 6e20  h Gym | [![Open 
+00002520: 696e 2043 6f6c 6162 5d28 6874 7470 733a  in Colab](https:
+00002530: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00002540: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
+00002550: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
+00002560: 7667 295d 2868 7474 7073 3a2f 2f63 6f6c  vg)](https://col
+00002570: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00002580: 6c65 2e63 6f6d 2f67 6974 6875 622f 454d  le.com/github/EM
+00002590: 492d 4772 6f75 702f 6576 6f78 2f62 6c6f  I-Group/evox/blo
+000025a0: 622f 6d61 696e 2f64 6f63 732f 736f 7572  b/main/docs/sour
+000025b0: 6365 2f65 7861 6d70 6c65 2f67 796d 5f63  ce/example/gym_c
+000025c0: 6c61 7373 6963 5f63 6f6e 7472 6f6c 2e69  lassic_control.i
+000025d0: 7079 6e62 2920 7c0a 7c20 4e65 7572 6f65  pynb) |.| Neuroe
+000025e0: 766f 6c75 7469 6f6e 2077 6974 6820 4272  volution with Br
+000025f0: 6178 207c 205b 215b 4f70 656e 2069 6e20  ax | [![Open in 
+00002600: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00002610: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00002620: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00002630: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
+00002640: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00002650: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00002660: 636f 6d2f 6769 7468 7562 2f45 4d49 2d47  com/github/EMI-G
+00002670: 726f 7570 2f65 766f 782f 626c 6f62 2f6d  roup/evox/blob/m
+00002680: 6169 6e2f 646f 6373 2f73 6f75 7263 652f  ain/docs/source/
+00002690: 6775 6964 652f 6261 7369 6373 2f32 2d70  guide/basics/2-p
+000026a0: 726f 626c 656d 732e 6970 796e 6229 207c  roblems.ipynb) |
+000026b0: 0a7c 2043 7573 746f 6d20 416c 676f 7269  .| Custom Algori
+000026c0: 7468 6d2f 5072 6f62 6c65 6d20 7c20 5b21  thm/Problem | [!
+000026d0: 5b4f 7065 6e20 696e 2043 6f6c 6162 5d28  [Open in Colab](
+000026e0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+000026f0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00002700: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
+00002710: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00002720: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+00002730: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
+00002740: 6875 622f 454d 492d 4772 6f75 702f 6576  hub/EMI-Group/ev
+00002750: 6f78 2f62 6c6f 622f 6d61 696e 2f64 6f63  ox/blob/main/doc
+00002760: 732f 736f 7572 6365 2f65 7861 6d70 6c65  s/source/example
+00002770: 2f63 7573 746f 6d5f 616c 676f 7269 7468  /custom_algorith
+00002780: 6d5f 616e 645f 7072 6f62 6c65 6d2e 6970  m_and_problem.ip
+00002790: 796e 6229 207c 0a0a 466f 7220 6d6f 7265  ynb) |..For more
+000027a0: 2075 7365 2d63 6173 6573 2061 6e64 2061   use-cases and a
+000027b0: 7070 6c69 6361 7469 6f6e 732c 2070 6c65  pplications, ple
+000027c0: 6165 2063 6865 636b 206f 7574 205b 4578  ae check out [Ex
+000027d0: 616d 706c 6520 4469 7265 6374 6f72 795d  ample Directory]
+000027e0: 2868 7474 7073 3a2f 2f65 766f 782e 7265  (https://evox.re
+000027f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00002800: 6c61 7465 7374 2f65 7861 6d70 6c65 2f69  latest/example/i
+00002810: 6e64 6578 2e68 746d 6c29 2e0a 0a23 2320  ndex.html)...## 
+00002820: 436f 6d6d 756e 6974 7920 2620 5375 7070  Community & Supp
+00002830: 6f72 740a 0a2d 2045 6e67 6167 6520 696e  ort..- Engage in
+00002840: 2064 6973 6375 7373 696f 6e73 2061 6e64   discussions and
+00002850: 2073 6861 7265 2079 6f75 7220 6578 7065   share your expe
+00002860: 7269 656e 6365 7320 6f6e 205b 4769 7448  riences on [GitH
+00002870: 7562 2044 6973 6375 7373 696f 6e20 426f  ub Discussion Bo
+00002880: 6172 645d 2868 7474 7073 3a2f 2f67 6974  ard](https://git
+00002890: 6875 622e 636f 6d2f 454d 492d 4772 6f75  hub.com/EMI-Grou
+000028a0: 702f 6576 6f78 2f64 6973 6375 7373 696f  p/evox/discussio
+000028b0: 6e73 292e 0a2d 204a 6f69 6e20 6f75 7220  ns)..- Join our 
+000028c0: 5151 2067 726f 7570 2028 4944 3a20 3239  QQ group (ID: 29
+000028d0: 3739 3639 3731 3729 2e0a 2d20 4865 6c70  7969717)..- Help
+000028e0: 2077 6974 6820 7468 6520 7472 616e 736c   with the transl
+000028f0: 6174 696f 6e20 6f66 2074 6865 2064 6f63  ation of the doc
+00002900: 756d 656e 7461 7469 6f6e 206f 6e20 5b57  umentation on [W
+00002910: 6562 6c61 7465 5d28 6874 7470 733a 2f2f  eblate](https://
+00002920: 686f 7374 6564 2e77 6562 6c61 7465 2e6f  hosted.weblate.o
+00002930: 7267 2f70 726f 6a65 6374 732f 6576 6f78  rg/projects/evox
+00002940: 2f65 766f 782f 292e 0a57 6520 6375 7272  /evox/)..We curr
+00002950: 656e 746c 7920 7375 7070 6f72 7420 7472  ently support tr
+00002960: 616e 736c 6174 696f 6e73 2069 6e20 7477  anslations in tw
+00002970: 6f20 6c61 6e67 7561 6765 732c 205b 456e  o languages, [En
+00002980: 676c 6973 685d 2868 7474 7073 3a2f 2f65  glish](https://e
+00002990: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
+000029a0: 696f 2f65 6e2f 6c61 7465 7374 2f29 202f  io/en/latest/) /
+000029b0: 205b e4b8 ade6 9687 5d28 6874 7470 733a   [......](https:
+000029c0: 2f2f 6576 6f78 2e72 6561 6474 6865 646f  //evox.readthedo
+000029d0: 6373 2e69 6f2f 7a68 2f6c 6174 6573 742f  cs.io/zh/latest/
+000029e0: 292e 0a2d 204f 6666 6963 6961 6c20 5765  )..- Official We
+000029f0: 6273 6974 653a 2068 7474 7073 3a2f 2f65  bsite: https://e
+00002a00: 766f 782e 6772 6f75 702f 0a0a 2323 2053  vox.group/..## S
+00002a10: 6973 7465 7220 5072 6f6a 6563 7473 0a0a  ister Projects..
+00002a20: 2d20 4576 6f58 4265 6e63 683a 2041 2062  - EvoXBench: A b
+00002a30: 656e 6368 6d61 726b 2070 6c61 7466 6f72  enchmark platfor
+00002a40: 6d20 666f 7220 4e65 7572 616c 2041 7263  m for Neural Arc
+00002a50: 6869 7465 6375 7472 6520 5365 6172 6368  hitecutre Search
+00002a60: 2028 4e41 5329 2077 6974 686f 7574 2074   (NAS) without t
+00002a70: 6865 2072 6571 7569 7265 6d65 6e74 206f  he requirement o
+00002a80: 6620 4750 5573 2f50 7954 6f72 6368 2f54  f GPUs/PyTorch/T
+00002a90: 656e 736f 7266 6c6f 772c 2073 7570 706f  ensorflow, suppo
+00002aa0: 7274 696e 6720 7661 7269 6f75 7320 7072  rting various pr
+00002ab0: 6f67 7261 6d6d 696e 6720 6c61 6e67 7561  ogramming langua
+00002ac0: 6765 7320 7375 6368 2061 7320 4a61 7661  ges such as Java
+00002ad0: 2c20 4d61 746c 6162 2c20 5079 7468 6f6e  , Matlab, Python
+00002ae0: 2c20 6563 742e 2043 6865 636b 206f 7574  , ect. Check out
+00002af0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+00002b00: 6769 7468 7562 2e63 6f6d 2f45 4d49 2d47  github.com/EMI-G
+00002b10: 726f 7570 2f65 766f 7862 656e 6368 292e  roup/evoxbench).
+00002b20: 0a0a 2323 2043 6974 696e 6720 4576 6f58  ..## Citing EvoX
+00002b30: 0a0a 4966 2079 6f75 2075 7365 2045 766f  ..If you use Evo
+00002b40: 5820 696e 2079 6f75 7220 7265 7365 6172  X in your resear
+00002b50: 6368 2061 6e64 2077 616e 7420 746f 2063  ch and want to c
+00002b60: 6974 6520 6974 2069 6e20 796f 7572 2077  ite it in your w
+00002b70: 6f72 6b2c 2070 6c65 6173 6520 7573 653a  ork, please use:
+00002b80: 0a60 6060 0a40 6172 7469 636c 657b 6576  .```.@article{ev
+00002b90: 6f78 2c0a 2020 7469 746c 6520 3d20 7b7b  ox,.  title = {{
+00002ba0: 4576 6f58 7d3a 207b 417d 207b 4469 7374  EvoX}: {A} {Dist
+00002bb0: 7269 6275 7465 647d 207b 4750 557d 2d61  ributed} {GPU}-a
+00002bc0: 6363 656c 6572 6174 6564 207b 4672 616d  ccelerated {Fram
+00002bd0: 6577 6f72 6b7d 2066 6f72 207b 5363 616c  ework} for {Scal
+00002be0: 6162 6c65 7d20 7b45 766f 6c75 7469 6f6e  able} {Evolution
+00002bf0: 6172 797d 207b 436f 6d70 7574 6174 696f  ary} {Computatio
+00002c00: 6e7d 7d2c 0a20 2061 7574 686f 7220 3d20  n}},.  author = 
+00002c10: 7b48 7561 6e67 2c20 4265 6963 6865 6e20  {Huang, Beichen 
+00002c20: 616e 6420 4368 656e 672c 2052 616e 2061  and Cheng, Ran a
+00002c30: 6e64 204c 692c 205a 6875 6f7a 6861 6f20  nd Li, Zhuozhao 
+00002c40: 616e 6420 4a69 6e2c 2059 616f 6368 7520  and Jin, Yaochu 
+00002c50: 616e 6420 5461 6e2c 204b 6179 2043 6865  and Tan, Kay Che
+00002c60: 6e7d 2c0a 2020 6a6f 7572 6e61 6c20 3d20  n},.  journal = 
+00002c70: 7b49 4545 4520 5472 616e 7361 6374 696f  {IEEE Transactio
+00002c80: 6e73 206f 6e20 4576 6f6c 7574 696f 6e61  ns on Evolutiona
+00002c90: 7279 2043 6f6d 7075 7461 7469 6f6e 7d2c  ry Computation},
+00002ca0: 0a20 2079 6561 7220 3d20 3230 3234 2c0a  .  year = 2024,.
+00002cb0: 2020 646f 6920 3d20 7b31 302e 3131 3039    doi = {10.1109
+00002cc0: 2f54 4556 432e 3230 3234 2e33 3338 3835  /TEVC.2024.33885
+00002cd0: 3530 7d0a 7d0a 6060 600a 0a23 2320 5374  50}.}.```..## St
+00002ce0: 6172 2048 6973 746f 7279 0a0a 5b21 5b53  ar History..[![S
+00002cf0: 7461 7220 4869 7374 6f72 7920 4368 6172  tar History Char
+00002d00: 745d 2868 7474 7073 3a2f 2f61 7069 2e73  t](https://api.s
+00002d10: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
+00002d20: 7376 673f 7265 706f 733d 454d 492d 4772  svg?repos=EMI-Gr
+00002d30: 6f75 702f 6576 6f78 2674 7970 653d 4461  oup/evox&type=Da
+00002d40: 7465 295d 2868 7474 7073 3a2f 2f73 7461  te)](https://sta
+00002d50: 722d 6869 7374 6f72 792e 636f 6d2f 2345  r-history.com/#E
+00002d60: 4d49 2d47 726f 7570 2f65 766f 7826 4461  MI-Group/evox&Da
+00002d70: 7465 290a 0a0a 0a                        te)....
```

### Comparing `evox-0.8.0/README.md` & `evox-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/pyproject.toml` & `evox-0.8.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 mypkg = ["*.txt", "*.json"]
 
 [project]
 name = "evox"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name = "Bill Huang", email = "bill.huang2001@gmail.com" },
   { name = "Christina Lee", email = "1315552992@qq.com" },
   { name = "Zhenyu Liang", email = "zhenyuliang97@gmail.com" },
 ]
 description = "evox"
 readme = "README.md"
@@ -39,41 +39,46 @@
 ]
 
 [project.optional-dependencies]
 test = [
   "chex >= 0.1.0",
   "flax >= 0.5.0",
   "pytest >= 6.0.0",
+  "tensorflow >= 2.12.0",
 ]
 
 vis = [
   "plotly >= 5.0.0",
   "pandas >= 2.0.0",
 ]
 
 gymnasium = ["gymnasium >= 0.29.0"]
 
 envpool = ["envpool >= 0.8.0"]
 
 neuroevolution = [
-  "torch >= 1.0.0",
-  "torchvision >= 0.1.0",
+  "tensorflow-datasets >= 4.0.0",
+  "grain >= 0.1.0",
+  "brax >= 0.1.0",
 ]
 
 distributed = ["ray >= 2.0.0"]
 
 full = [
   "gymnasium >= 0.29.0",
   "ray >= 2.0.0",
-  "torch >= 1.0.0",
-  "torchvision >= 0.1.0",
   "envpool >= 0.8.0",
   "gpjax >= 0.8.0",
   "plotly >= 5.0.0",
   "pandas >= 2.0.0",
+  "tensorflow-datasets >= 4.0.0",
+  "grain >= 0.1.0",
+  "brax >= 0.1.0",
+  "plotly >= 5.0.0",
+  "pandas >= 2.0.0",
 ]
 
 gp = ["gpjax >= 0.8.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/EMI-Group/evox"
 "Bug Tracker" = "https://github.com/EMI-Group/evox/issues"
```

### Comparing `evox-0.8.0/src/evox/algorithms/containers/clustered_algorithm.py` & `evox-0.8.1/src/evox/algorithms/containers/clustered_algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/containers/coevolution.py` & `evox-0.8.1/src/evox/algorithms/containers/coevolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/containers/tree_algorithm.py` & `evox-0.8.1/src/evox/algorithms/containers/tree_algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/bce_ibea.py` & `evox-0.8.1/src/evox/algorithms/mo/bce_ibea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/bige.py` & `evox-0.8.1/src/evox/algorithms/mo/bige.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/eagmoead.py` & `evox-0.8.1/src/evox/algorithms/mo/eagmoead.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/gde3.py` & `evox-0.8.1/src/evox/algorithms/mo/gde3.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/hype.py` & `evox-0.8.1/src/evox/algorithms/mo/hype.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/ibea.py` & `evox-0.8.1/src/evox/algorithms/mo/ibea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/im_moea.py` & `evox-0.8.1/src/evox/algorithms/mo/im_moea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/knea.py` & `evox-0.8.1/src/evox/algorithms/mo/knea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/lmocso.py` & `evox-0.8.1/src/evox/algorithms/mo/lmocso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/moead.py` & `evox-0.8.1/src/evox/algorithms/mo/moead.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/moeaddra.py` & `evox-0.8.1/src/evox/algorithms/mo/moeaddra.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/moeadm2m.py` & `evox-0.8.1/src/evox/algorithms/mo/moeadm2m.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/nsga2.py` & `evox-0.8.1/src/evox/algorithms/mo/nsga2.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/nsga3.py` & `evox-0.8.1/src/evox/algorithms/mo/nsga3.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/rvea.py` & `evox-0.8.1/src/evox/algorithms/mo/rvea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/rveaa.py` & `evox-0.8.1/src/evox/algorithms/mo/rveaa.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/spea2.py` & `evox-0.8.1/src/evox/algorithms/mo/spea2.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/sra.py` & `evox-0.8.1/src/evox/algorithms/mo/sra.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/mo/tdea.py` & `evox-0.8.1/src/evox/algorithms/mo/tdea.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/code.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/code.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/de.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/de.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/jade.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/jade.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/ode.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/ode.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/sade.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/sade.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/de_variants/shade.py` & `evox-0.8.1/src/evox/algorithms/so/de_variants/shade.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/__init__.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/amalgam.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/amalgam.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/ars.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/ars.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/asebo.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/asebo.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/cma_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/cma_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/cr_fm_nes.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/cr_fm_nes.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/des.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/des.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/esmc.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/esmc.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/guided_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/guided_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/les.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/les.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/ma_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/ma_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/nes.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/nes.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/noise_reuse_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/noise_reuse_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/open_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/open_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/persistent_es.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/persistent_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/pgpe.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/pgpe.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/rmes.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/rmes.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/es_variants/snes.py` & `evox-0.8.1/src/evox/algorithms/so/es_variants/snes.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/clpso.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/clpso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/cso.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/cso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/dms_pso_el.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/dms_pso_el.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/fips.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/fips.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/fs_pso.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/fs_pso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/pso.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/pso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/sl_pso_gs.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/sl_pso_gs.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/sl_pso_us.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/sl_pso_us.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/swmmpso.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/swmmpso.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/topology_utils.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/topology_utils.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/algorithms/so/pso_variants/utils.py` & `evox-0.8.1/src/evox/algorithms/so/pso_variants/utils.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/core/algorithm.py` & `evox-0.8.1/src/evox/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/core/module.py` & `evox-0.8.1/src/evox/core/module.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/core/monitor.py` & `evox-0.8.1/src/evox/core/monitor.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/core/problem.py` & `evox-0.8.1/src/evox/core/problem.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/core/state.py` & `evox-0.8.1/src/evox/core/state.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/metrics/gd.py` & `evox-0.8.1/src/evox/metrics/gd.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/metrics/hypervolume.py` & `evox-0.8.1/src/evox/metrics/hypervolume.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/metrics/igd.py` & `evox-0.8.1/src/evox/metrics/igd.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/monitors/eval_monitor.py` & `evox-0.8.1/src/evox/monitors/eval_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,20 +113,20 @@
                 individual_index = jnp.argmin(cand_fit)
                 # use slice to keepdim,
                 # because topk_solutions should have dim of (1, dim)
                 self.topk_solutions = cand_sol[individual_index : individual_index + 1]
         else:
             # since topk > 1, we have to sort the fitness
             if self.topk_fitness is None:
-                self.topk_fitness = fitness
+                self.topk_fitness = cand_fit
             else:
-                self.topk_fitness = jnp.concatenate([self.topk_fitness, fitness])
+                self.topk_fitness = jnp.concatenate([self.topk_fitness, cand_fit])
 
             if self.topk_solutions is None:
-                self.topk_solutions = cand_fit
+                self.topk_solutions = cand_sol
             else:
                 self.topk_solutions = jnp.concatenate(
                     [self.topk_solutions, cand_sol], axis=0
                 )
             rank = jnp.argsort(self.topk_fitness)
             topk_rank = rank[: self.topk]
             self.topk_solutions = self.topk_solutions[topk_rank]
```

### Comparing `evox-0.8.0/src/evox/monitors/evoxvis_monitor.py` & `evox-0.8.1/src/evox/monitors/evoxvis_monitor.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/monitors/pop_monitor.py` & `evox-0.8.1/src/evox/monitors/pop_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any
 import warnings
 
 import jax
 import jax.numpy as jnp
+from jax.experimental import io_callback
+from jax.sharding import SingleDeviceSharding
 
 from evox import Monitor
 from evox.vis_tools import plot
 
 
 class PopMonitor(Monitor):
     """Population monitor,
@@ -33,42 +35,47 @@
         Default to False.
     """
 
     def __init__(
         self,
         population_name="population",
         fitness_name="fitness",
-        to_host=False,
         fitness_only=False,
     ):
         super().__init__()
         self.population_name = population_name
         self.fitness_name = fitness_name
-        self.to_host = to_host
-        if to_host:
-            self.host = jax.devices("cpu")[0]
         self.population_history = []
         self.fitness_history = []
         self.fitness_only = fitness_only
 
     def hooks(self):
         return ["post_step"]
 
     def post_step(self, state):
+        monitor_device = SingleDeviceSharding(jax.devices()[0])
         if not self.fitness_only:
             population = getattr(
                 state.get_child_state("algorithm"), self.population_name
             )
-            if self.to_host:
-                population = jax.device_put(population, self.host)
-            self.population_history.append(population)
+        else:
+            population = None
 
         fitness = getattr(state.get_child_state("algorithm"), self.fitness_name)
-        if self.to_host:
-            fitness = jax.device_put(fitness, self.host)
+        io_callback(
+            self._record,
+            None,
+            population,
+            fitness,
+            sharding=monitor_device,
+        )
+
+    def _record(self, population, fitness):
+        if population is not None:
+            self.population_history.append(population)
         self.fitness_history.append(fitness)
 
     def plot(self, problem_pf=None, **kwargs):
         if not self.fitness_history:
             warnings.warn("No fitness history recorded, return None")
             return
 
@@ -82,12 +89,18 @@
         elif n_objs == 2:
             return plot.plot_obj_space_2d(self.fitness_history, problem_pf, **kwargs)
         elif n_objs == 3:
             return plot.plot_obj_space_3d(self.fitness_history, problem_pf, **kwargs)
         else:
             warnings.warn("Not supported yet.")
 
+    def get_latest_fitness(self):
+        return self.fitness_history[-1]
+
+    def get_latest_population(self):
+        return self.population_history[-1]
+
     def get_population_history(self):
         return self.population_history
 
     def get_fitness_history(self):
         return self.fitness_history
```

### Comparing `evox-0.8.0/src/evox/monitors/std_mo_monitor.py` & `evox-0.8.1/src/evox/monitors/std_mo_monitor.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/monitors/std_so_monitor.py` & `evox-0.8.1/src/evox/monitors/std_so_monitor.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/crossover/differential_evolution.py` & `evox-0.8.1/src/evox/operators/crossover/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/crossover/one_point.py` & `evox-0.8.1/src/evox/operators/crossover/one_point.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/crossover/sbx.py` & `evox-0.8.1/src/evox/operators/crossover/sbx.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/crossover/simulated_binary.py` & `evox-0.8.1/src/evox/operators/crossover/simulated_binary.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/crossover/uniform.py` & `evox-0.8.1/src/evox/operators/crossover/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/gaussian_process/__init__.py` & `evox-0.8.1/src/evox/operators/gaussian_process/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/gaussian_process/classification.py` & `evox-0.8.1/src/evox/operators/gaussian_process/classification.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/gaussian_process/regression.py` & `evox-0.8.1/src/evox/operators/gaussian_process/regression.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/mutation/bitflip.py` & `evox-0.8.1/src/evox/operators/mutation/bitflip.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/mutation/pm_mutation.py` & `evox-0.8.1/src/evox/operators/mutation/pm_mutation.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/sampling/grid.py` & `evox-0.8.1/src/evox/operators/sampling/grid.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/sampling/latin_hypercude.py` & `evox-0.8.1/src/evox/operators/sampling/latin_hypercude.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/sampling/uniform.py` & `evox-0.8.1/src/evox/operators/sampling/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/find_pbest.py` & `evox-0.8.1/src/evox/operators/selection/find_pbest.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/non_dominate.py` & `evox-0.8.1/src/evox/operators/selection/non_dominate.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/roulette_wheel.py` & `evox-0.8.1/src/evox/operators/selection/roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/rvea_selection.py` & `evox-0.8.1/src/evox/operators/selection/rvea_selection.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/topk_fit.py` & `evox-0.8.1/src/evox/operators/selection/topk_fit.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/tournament.py` & `evox-0.8.1/src/evox/operators/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/operators/selection/uniform_random.py` & `evox-0.8.1/src/evox/operators/selection/uniform_random.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/evoxbench/evoxbench.py` & `evox-0.8.1/src/evox/problems/evoxbench/evoxbench.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/__init__.py` & `evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/brax.py` & `evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/brax.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/env_pool.py` & `evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/env_pool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,18 @@
 from typing import Callable, Optional
 
 import envpool
 import jax
 import jax.numpy as jnp
 import numpy as np
 from jax import jit, random, vmap, lax
-from jax.tree_util import tree_map
 from jax.experimental import io_callback
 
 from evox import Problem, State, jit_class
-
-
-def _x32_func_call(func):
-    def inner_func(*args, **kwargs):
-        return _to_x32_if_needed(func(*args, **kwargs))
-
-    return inner_func
-
-
-def _to_x32_if_needed(values):
-    if jax.config.jax_enable_x64:
-        # we have 64-bit enabled, so nothing to do
-        return values
-
-    def to_x32(value):
-        if value.dtype == np.float64:
-            return value.astype(np.float32)
-        elif value.dtype == np.int64:
-            return value.astype(np.int32)
-        else:
-            return value
-    return tree_map(to_x32, values)
+from evox.utils.io import to_x32_if_needed, x32_func_call
 
 
 @jit_class
 class EnvPool(Problem):
     def __init__(
         self,
         policy: Callable,
@@ -56,34 +34,34 @@
     def setup(self, key):
         return State(key=key)
 
     def evaluate(self, state, pop):
         key, subkey = random.split(state.key)
         seed = random.randint(subkey, (1,), 0, jnp.iinfo(jnp.int32).max)
         io_callback(self.env.seed, None, seed)
-        obs, info = _to_x32_if_needed(self.env.reset(None))
-        obs, info = io_callback(_x32_func_call(self.env.reset), (obs, info), None)
+        obs, info = to_x32_if_needed(self.env.reset(None))
+        obs, info = io_callback(x32_func_call(self.env.reset), (obs, info), None)
         total_reward = 0
         i = 0
 
         def cond_func(loop_state):
             i, done, _total_reward, _obs = loop_state
             if self.cap_episode_length:
                 return (i < self.cap_episode_length) & ~jnp.all(done)
             else:
                 return ~jnp.all(done)
 
         def step(loop_state):
             i, done, total_reward, obs = loop_state
             action = self.batch_policy(pop, obs)
-            obs, reward, terminated, truncated, info = _to_x32_if_needed(
+            obs, reward, terminated, truncated, info = to_x32_if_needed(
                 self.env.step(np.zeros(action.shape))
             )
             obs, reward, terminated, truncated, info = io_callback(
-                _x32_func_call(lambda action: self.env.step(np.copy(action))),
+                x32_func_call(lambda action: self.env.step(np.copy(action))),
                 (obs, reward, terminated, truncated, info),
                 action,
             )
             total_reward += ~done * reward
             done = done | (terminated | truncated)
 
             return i + 1, done, total_reward, obs
```

### Comparing `evox-0.8.0/src/evox/problems/neuroevolution/reinforcement_learning/gym.py` & `evox-0.8.1/src/evox/problems/neuroevolution/reinforcement_learning/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/__init__.py` & `evox-0.8.1/src/evox/problems/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/ackley.py` & `evox-0.8.1/src/evox/problems/numerical/ackley.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D2.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D2.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_10_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_10_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D2.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D2.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_11_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_11_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D2.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D2.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_12_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_12_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_1_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_1_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_1_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_1_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_2_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_2_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_2_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_2_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_3_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_3_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_3_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_3_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_4_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_4_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_4_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_4_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_5_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_5_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_5_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_5_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_6_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_6_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_6_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_6_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_7_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_7_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_7_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_7_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_8_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_8_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_8_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_8_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D2.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D2.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/M_9_D20.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/M_9_D20.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/Rand_Seeds.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/Rand_Seeds.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_1.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_1.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_10.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_10.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_11.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_11.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_12.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_12.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_2.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_2.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_3.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_3.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_4.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_4.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_5.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_5.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_6.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_6.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_7.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_7.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_8.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_8.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_input_data/shift_data_9.txt` & `evox-0.8.1/src/evox/problems/numerical/cec2022_input_data/shift_data_9.txt`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/cec2022_so.py` & `evox-0.8.1/src/evox/problems/numerical/cec2022_so.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/dtlz.py` & `evox-0.8.1/src/evox/problems/numerical/dtlz.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/lsmop.py` & `evox-0.8.1/src/evox/problems/numerical/lsmop.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/maf.py` & `evox-0.8.1/src/evox/problems/numerical/maf.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/problems/numerical/zdt.py` & `evox-0.8.1/src/evox/problems/numerical/zdt.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/utils/common.py` & `evox-0.8.1/src/evox/utils/common.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/vis_tools/plot.py` & `evox-0.8.1/src/evox/vis_tools/plot.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/workflows/distributed.py` & `evox-0.8.1/src/evox/workflows/distributed.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/workflows/non_jit_workflow.py` & `evox-0.8.1/src/evox/workflows/non_jit_workflow.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox/workflows/std_workflow.py` & `evox-0.8.1/src/evox/workflows/std_workflow.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/src/evox.egg-info/PKG-INFO` & `evox-0.8.1/src/evox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6576 6f78  : 2.1.Name: evox
-00000020: 0a56 6572 7369 6f6e 3a20 302e 382e 300a  .Version: 0.8.0.
+00000020: 0a56 6572 7369 6f6e 3a20 302e 382e 310a  .Version: 0.8.1.
 00000030: 5375 6d6d 6172 793a 2065 766f 780a 4175  Summary: evox.Au
 00000040: 7468 6f72 2d65 6d61 696c 3a20 4269 6c6c  thor-email: Bill
 00000050: 2048 7561 6e67 203c 6269 6c6c 2e68 7561   Huang <bill.hua
 00000060: 6e67 3230 3031 4067 6d61 696c 2e63 6f6d  ng2001@gmail.com
 00000070: 3e2c 2043 6872 6973 7469 6e61 204c 6565  >, Christina Lee
 00000080: 203c 3133 3135 3535 3239 3932 4071 712e   <1315552992@qq.
 00000090: 636f 6d3e 2c20 5a68 656e 7975 204c 6961  com>, Zhenyu Lia
@@ -161,552 +161,568 @@
 00000a00: 4469 7374 3a20 6368 6578 3e3d 302e 312e  Dist: chex>=0.1.
 00000a10: 303b 2065 7874 7261 203d 3d20 2274 6573  0; extra == "tes
 00000a20: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
 00000a30: 3a20 666c 6178 3e3d 302e 352e 303b 2065  : flax>=0.5.0; e
 00000a40: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
 00000a50: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
 00000a60: 7465 7374 3e3d 362e 302e 303b 2065 7874  test>=6.0.0; ext
-00000a70: 7261 203d 3d20 2274 6573 7422 0a50 726f  ra == "test".Pro
-00000a80: 7669 6465 732d 4578 7472 613a 2076 6973  vides-Extra: vis
-00000a90: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000aa0: 706c 6f74 6c79 3e3d 352e 302e 303b 2065  plotly>=5.0.0; e
-00000ab0: 7874 7261 203d 3d20 2276 6973 220a 5265  xtra == "vis".Re
-00000ac0: 7175 6972 6573 2d44 6973 743a 2070 616e  quires-Dist: pan
-00000ad0: 6461 733e 3d32 2e30 2e30 3b20 6578 7472  das>=2.0.0; extr
-00000ae0: 6120 3d3d 2022 7669 7322 0a50 726f 7669  a == "vis".Provi
-00000af0: 6465 732d 4578 7472 613a 2067 796d 6e61  des-Extra: gymna
-00000b00: 7369 756d 0a52 6571 7569 7265 732d 4469  sium.Requires-Di
-00000b10: 7374 3a20 6779 6d6e 6173 6975 6d3e 3d30  st: gymnasium>=0
-00000b20: 2e32 392e 303b 2065 7874 7261 203d 3d20  .29.0; extra == 
-00000b30: 2267 796d 6e61 7369 756d 220a 5072 6f76  "gymnasium".Prov
-00000b40: 6964 6573 2d45 7874 7261 3a20 656e 7670  ides-Extra: envp
-00000b50: 6f6f 6c0a 5265 7175 6972 6573 2d44 6973  ool.Requires-Dis
-00000b60: 743a 2065 6e76 706f 6f6c 3e3d 302e 382e  t: envpool>=0.8.
-00000b70: 303b 2065 7874 7261 203d 3d20 2265 6e76  0; extra == "env
-00000b80: 706f 6f6c 220a 5072 6f76 6964 6573 2d45  pool".Provides-E
-00000b90: 7874 7261 3a20 6e65 7572 6f65 766f 6c75  xtra: neuroevolu
-00000ba0: 7469 6f6e 0a52 6571 7569 7265 732d 4469  tion.Requires-Di
-00000bb0: 7374 3a20 746f 7263 683e 3d31 2e30 2e30  st: torch>=1.0.0
-00000bc0: 3b20 6578 7472 6120 3d3d 2022 6e65 7572  ; extra == "neur
-00000bd0: 6f65 766f 6c75 7469 6f6e 220a 5265 7175  oevolution".Requ
-00000be0: 6972 6573 2d44 6973 743a 2074 6f72 6368  ires-Dist: torch
-00000bf0: 7669 7369 6f6e 3e3d 302e 312e 303b 2065  vision>=0.1.0; e
-00000c00: 7874 7261 203d 3d20 226e 6575 726f 6576  xtra == "neuroev
-00000c10: 6f6c 7574 696f 6e22 0a50 726f 7669 6465  olution".Provide
-00000c20: 732d 4578 7472 613a 2064 6973 7472 6962  s-Extra: distrib
-00000c30: 7574 6564 0a52 6571 7569 7265 732d 4469  uted.Requires-Di
-00000c40: 7374 3a20 7261 793e 3d32 2e30 2e30 3b20  st: ray>=2.0.0; 
-00000c50: 6578 7472 6120 3d3d 2022 6469 7374 7269  extra == "distri
-00000c60: 6275 7465 6422 0a50 726f 7669 6465 732d  buted".Provides-
-00000c70: 4578 7472 613a 2066 756c 6c0a 5265 7175  Extra: full.Requ
-00000c80: 6972 6573 2d44 6973 743a 2067 796d 6e61  ires-Dist: gymna
-00000c90: 7369 756d 3e3d 302e 3239 2e30 3b20 6578  sium>=0.29.0; ex
-00000ca0: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000cb0: 7175 6972 6573 2d44 6973 743a 2072 6179  quires-Dist: ray
-00000cc0: 3e3d 322e 302e 303b 2065 7874 7261 203d  >=2.0.0; extra =
-00000cd0: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
-00000ce0: 732d 4469 7374 3a20 746f 7263 683e 3d31  s-Dist: torch>=1
-00000cf0: 2e30 2e30 3b20 6578 7472 6120 3d3d 2022  .0.0; extra == "
-00000d00: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
-00000d10: 6973 743a 2074 6f72 6368 7669 7369 6f6e  ist: torchvision
-00000d20: 3e3d 302e 312e 303b 2065 7874 7261 203d  >=0.1.0; extra =
-00000d30: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
-00000d40: 732d 4469 7374 3a20 656e 7670 6f6f 6c3e  s-Dist: envpool>
-00000d50: 3d30 2e38 2e30 3b20 6578 7472 6120 3d3d  =0.8.0; extra ==
-00000d60: 2022 6675 6c6c 220a 5265 7175 6972 6573   "full".Requires
-00000d70: 2d44 6973 743a 2067 706a 6178 3e3d 302e  -Dist: gpjax>=0.
-00000d80: 382e 303b 2065 7874 7261 203d 3d20 2266  8.0; extra == "f
-00000d90: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
-00000da0: 7374 3a20 706c 6f74 6c79 3e3d 352e 302e  st: plotly>=5.0.
-00000db0: 303b 2065 7874 7261 203d 3d20 2266 756c  0; extra == "ful
-00000dc0: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000dd0: 3a20 7061 6e64 6173 3e3d 322e 302e 303b  : pandas>=2.0.0;
-00000de0: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-00000df0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000e00: 2067 700a 5265 7175 6972 6573 2d44 6973   gp.Requires-Dis
-00000e10: 743a 2067 706a 6178 3e3d 302e 382e 303b  t: gpjax>=0.8.0;
-00000e20: 2065 7874 7261 203d 3d20 2267 7022 0a0a   extra == "gp"..
-00000e30: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000e40: 7222 3e0a 2020 3c70 6963 7475 7265 3e0a  r">.  <picture>.
-00000e50: 2020 2020 3c73 6f75 7263 6520 6d65 6469      <source medi
-00000e60: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
-00000e70: 722d 7363 6865 6d65 3a20 6461 726b 2922  r-scheme: dark)"
-00000e80: 2073 7263 7365 743d 2264 6f63 732f 736f   srcset="docs/so
-00000e90: 7572 6365 2f5f 7374 6174 6963 2f65 766f  urce/_static/evo
-00000ea0: 785f 6c6f 676f 5f64 6172 6b2e 706e 6722  x_logo_dark.png"
-00000eb0: 3e0a 2020 2020 3c73 6f75 7263 6520 6d65  >.    <source me
-00000ec0: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
-00000ed0: 6c6f 722d 7363 6865 6d65 3a20 6c69 6768  lor-scheme: ligh
-00000ee0: 7429 2220 7372 6373 6574 3d22 646f 6373  t)" srcset="docs
-00000ef0: 2f73 6f75 7263 652f 5f73 7461 7469 632f  /source/_static/
-00000f00: 6576 6f78 5f6c 6f67 6f5f 6c69 6768 742e  evox_logo_light.
-00000f10: 706e 6722 3e0a 2020 2020 3c69 6d67 2061  png">.    <img a
-00000f20: 6c74 3d22 4576 6f58 204c 6f67 6f22 2068  lt="EvoX Logo" h
-00000f30: 6569 6768 743d 2231 3238 2220 7769 6474  eight="128" widt
-00000f40: 683d 2235 3030 7078 2220 7372 633d 2264  h="500px" src="d
-00000f50: 6f63 732f 736f 7572 6365 2f5f 7374 6174  ocs/source/_stat
-00000f60: 6963 2f65 766f 785f 6c6f 676f 5f6c 6967  ic/evox_logo_lig
-00000f70: 6874 2e70 6e67 223e 0a20 203c 2f70 6963  ht.png">.  </pic
-00000f80: 7475 7265 3e0a 3c2f 6831 3e0a 0a3c 7020  ture>.</h1>..<p 
-00000f90: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000fa0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000fb0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-00000fc0: 2f32 3330 312e 3132 3435 3722 3e0a 2020  /2301.12457">.  
-00000fd0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000fe0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000ff0: 696f 2f62 6164 6765 2f70 6170 6572 2d61  io/badge/paper-a
-00001000: 7278 6976 2d72 6564 3f73 7479 6c65 3d66  rxiv-red?style=f
-00001010: 6f72 2d74 6865 2d62 6164 6765 2220 616c  or-the-badge" al
-00001020: 743d 2245 766f 5820 5061 7065 7220 6f6e  t="EvoX Paper on
-00001030: 2061 7258 6976 223e 0a20 203c 2f61 3e0a   arXiv">.  </a>.
-00001040: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00001050: 733a 2f2f 6576 6f78 2e72 6561 6474 6865  s://evox.readthe
-00001060: 646f 6373 2e69 6f2f 223e 0a20 2020 203c  docs.io/">.    <
-00001070: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001080: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001090: 6261 6467 652f 646f 6373 2d72 6561 6474  badge/docs-readt
-000010a0: 6865 646f 6373 2d62 6c75 653f 7374 796c  hedocs-blue?styl
-000010b0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000010c0: 2061 6c74 3d22 4576 6f58 2044 6f63 756d   alt="EvoX Docum
-000010d0: 656e 7461 7469 6f6e 223e 0a20 203c 2f61  entation">.  </a
-000010e0: 3e0a 3c2f 703e 0a0a 3c70 2061 6c69 676e  >.</p>..<p align
-000010f0: 3d22 6365 6e74 6572 223e 0a20 203c 623e  ="center">.  <b>
-00001100: f09f 8c9f 4469 7374 7269 6275 7465 6420  ....Distributed 
-00001110: 4750 552d 6163 6365 6c65 7261 7465 6420  GPU-accelerated 
-00001120: 4672 616d 6577 6f72 6b20 666f 7220 5363  Framework for Sc
-00001130: 616c 6162 6c65 2045 766f 6c75 7469 6f6e  alable Evolution
-00001140: 6172 7920 436f 6d70 7574 6174 696f 6ef0  ary Computation.
-00001150: 9f8c 9f3c 2f62 3e0a 3c2f 703e 0a0a 2d2d  ...</b>.</p>..--
-00001160: 2d0a 0a23 230a 4275 696c 6469 6e67 2075  -..##.Building u
-00001170: 706f 6e20 5b4a 4158 5d28 6874 7470 733a  pon [JAX](https:
-00001180: 2f2f 6769 7468 7562 2e63 6f6d 2f67 6f6f  //github.com/goo
-00001190: 676c 652f 6a61 7829 2061 6e64 205b 5261  gle/jax) and [Ra
-000011a0: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000011b0: 622e 636f 6d2f 7261 792d 7072 6f6a 6563  b.com/ray-projec
-000011c0: 742f 7261 7929 2c20 4576 6f58 206f 6666  t/ray), EvoX off
-000011d0: 6572 7320 6120 636f 6d70 7265 6865 6e73  ers a comprehens
-000011e0: 6976 6520 7375 6974 6520 6f66 202a 2a35  ive suite of **5
-000011f0: 302b 2045 766f 6c75 7469 6f6e 6172 7920  0+ Evolutionary 
-00001200: 416c 676f 7269 7468 6d73 2028 4541 7329  Algorithms (EAs)
-00001210: 2a2a 2061 6e64 2061 2077 6964 6520 7261  ** and a wide ra
-00001220: 6e67 6520 6f66 202a 2a31 3030 2b20 4265  nge of **100+ Be
-00001230: 6e63 686d 6172 6b20 5072 6f62 6c65 6d73  nchmark Problems
-00001240: 2a2a 2c20 616c 6c20 6265 6e65 6669 7469  **, all benefiti
-00001250: 6e67 2066 726f 6d20 6469 7374 7269 6275  ng from distribu
-00001260: 7465 6420 4750 552d 6163 6365 6c65 7261  ted GPU-accelera
-00001270: 7469 6f6e 2e20 4974 2066 6163 696c 6974  tion. It facilit
-00001280: 6174 6573 2065 6666 6963 6965 6e74 2065  ates efficient e
-00001290: 7870 6c6f 7261 7469 6f6e 206f 6620 636f  xploration of co
-000012a0: 6d70 6c65 7820 6f70 7469 6d69 7a61 7469  mplex optimizati
-000012b0: 6f6e 206c 616e 6473 6361 7065 732c 2065  on landscapes, e
-000012c0: 6666 6563 7469 7665 2074 6163 6b6c 696e  ffective tacklin
-000012d0: 6720 6f66 2062 6c61 636b 2d62 6f78 206f  g of black-box o
-000012e0: 7074 696d 697a 6174 696f 6e20 6368 616c  ptimization chal
-000012f0: 6c65 6e67 6573 2c20 616e 6420 6465 6570  lenges, and deep
-00001300: 2064 6976 6573 2069 6e74 6f20 6e65 7572   dives into neur
-00001310: 6f65 766f 6c75 7469 6f6e 2077 6974 6820  oevolution with 
-00001320: 5b42 7261 785d 2868 7474 7073 3a2f 2f67  [Brax](https://g
-00001330: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
-00001340: 2f62 7261 7829 2e20 5769 7468 2061 2066  /brax). With a f
-00001350: 6f75 6e64 6174 696f 6e20 696e 2066 756e  oundation in fun
-00001360: 6374 696f 6e61 6c20 7072 6f67 7261 6d6d  ctional programm
-00001370: 696e 6720 616e 6420 6869 6572 6172 6368  ing and hierarch
-00001380: 6963 616c 2073 7461 7465 206d 616e 6167  ical state manag
-00001390: 656d 656e 742c 2045 766f 5820 6f66 6665  ement, EvoX offe
-000013a0: 7273 2061 2075 7365 722d 6672 6965 6e64  rs a user-friend
-000013b0: 6c79 2061 6e64 206d 6f64 756c 6172 2065  ly and modular e
-000013c0: 7870 6572 6965 6e63 652e 2046 6f72 206d  xperience. For m
-000013d0: 6f72 6520 6465 7461 696c 732c 2070 6c65  ore details, ple
-000013e0: 6173 6520 7265 6665 7220 746f 206f 7572  ase refer to our
-000013f0: 205b 5061 7065 725d 2868 7474 7073 3a2f   [Paper](https:/
-00001400: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00001410: 3330 312e 3132 3435 3729 2061 6e64 205b  301.12457) and [
-00001420: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00001430: 7474 7073 3a2f 2f65 766f 782e 7265 6164  ttps://evox.read
-00001440: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00001450: 7465 7374 2f29 202f 205b e696 87e6 a1a3  test/) / [......
-00001460: 5d28 6874 7470 733a 2f2f 6576 6f78 2e72  ](https://evox.r
-00001470: 6561 6474 6865 646f 6373 2e69 6f2f 7a68  eadthedocs.io/zh
-00001480: 2f6c 6174 6573 742f 292e 0a0a 2d2d 2d0a  /latest/)...---.
-00001490: 0a23 2320 4b65 7920 4665 6174 7572 6573  .## Key Features
-000014a0: 0a0a 2d20 f09f 9a80 202a 2a46 6173 7420  ..- .... **Fast 
-000014b0: 5065 7266 6f72 6d61 6e63 652a 2a3a 0a20  Performance**:. 
-000014c0: 202d 2045 7870 6572 6965 6e63 6520 2a2a   - Experience **
-000014d0: 4750 552d 4163 6365 6c65 7261 7465 642a  GPU-Accelerated*
-000014e0: 2a20 6f70 7469 6d69 7a61 7469 6f6e 2c20  * optimization, 
-000014f0: 6163 6869 6576 696e 6720 7370 6565 6473  achieving speeds
-00001500: 206f 7665 7220 3130 3078 2066 6173 7465   over 100x faste
-00001510: 7220 7468 616e 2074 7261 6469 7469 6f6e  r than tradition
-00001520: 616c 206d 6574 686f 6473 2e0a 2020 2d20  al methods..  - 
-00001530: 4c65 7665 7261 6765 2074 6865 2070 6f77  Leverage the pow
-00001540: 6572 206f 6620 2a2a 4469 7374 7269 6275  er of **Distribu
-00001550: 7465 6420 576f 726b 666c 6f77 732a 2a20  ted Workflows** 
-00001560: 666f 7220 6576 656e 206d 6f72 6520 7261  for even more ra
-00001570: 7069 6420 6f70 7469 6d69 7a61 7469 6f6e  pid optimization
-00001580: 2e0a 0a2d 20f0 9f8c 9020 2a2a 5665 7273  ...- .... **Vers
-00001590: 6174 696c 6520 4f70 7469 6d69 7a61 7469  atile Optimizati
-000015a0: 6f6e 2053 7569 7465 2a2a 3a0a 2020 2d20  on Suite**:.  - 
-000015b0: 4361 7465 7220 746f 2061 6c6c 2079 6f75  Cater to all you
-000015c0: 7220 6e65 6564 7320 7769 7468 2062 6f74  r needs with bot
-000015d0: 6820 2a2a 5369 6e67 6c65 2d6f 626a 6563  h **Single-objec
-000015e0: 7469 7665 2a2a 2061 6e64 202a 2a4d 756c  tive** and **Mul
-000015f0: 7469 2d6f 626a 6563 7469 7665 2a2a 206f  ti-objective** o
-00001600: 7074 696d 697a 6174 696f 6e20 6361 7061  ptimization capa
-00001610: 6269 6c69 7469 6573 2e0a 2020 2d20 4469  bilities..  - Di
-00001620: 7665 2069 6e74 6f20 6120 636f 6d70 7265  ve into a compre
-00001630: 6865 6e73 6976 6520 6c69 6272 6172 7920  hensive library 
-00001640: 6f66 202a 2a42 656e 6368 6d61 726b 2050  of **Benchmark P
-00001650: 726f 626c 656d 732a 2a2c 2065 6e73 7572  roblems**, ensur
-00001660: 696e 6720 726f 6275 7374 2074 6573 7469  ing robust testi
-00001670: 6e67 2061 6e64 2065 7661 6c75 6174 696f  ng and evaluatio
-00001680: 6e2e 0a20 202d 2045 7870 6c6f 7265 2074  n..  - Explore t
-00001690: 6865 2066 726f 6e74 6965 7220 6f66 2041  he frontier of A
-000016a0: 4920 7769 7468 2065 7874 656e 7369 7665  I with extensive
-000016b0: 2074 6f6f 6c73 2066 6f72 202a 2a4e 6575   tools for **Neu
-000016c0: 726f 6576 6f6c 7574 696f 6e2a 2a20 7461  roevolution** ta
-000016d0: 736b 732e 0a0a 2d20 f09f 9ba0 efb8 8f20  sks...- ....... 
-000016e0: 2a2a 4465 7369 676e 6564 2066 6f72 2053  **Designed for S
-000016f0: 696d 706c 6963 6974 792a 2a3a 0a20 202d  implicity**:.  -
-00001700: 2045 6d62 7261 6365 2074 6865 2065 6c65   Embrace the ele
-00001710: 6761 6e63 6520 6f66 202a 2a46 756e 6374  gance of **Funct
-00001720: 696f 6e61 6c20 5072 6f67 7261 6d6d 696e  ional Programmin
-00001730: 672a 2a2c 2073 696d 706c 6966 7969 6e67  g**, simplifying
-00001740: 2063 6f6d 706c 6578 2061 6c67 6f72 6974   complex algorit
-00001750: 686d 6963 2063 6f6d 706f 7369 7469 6f6e  hmic composition
-00001760: 732e 0a20 202d 2042 656e 6566 6974 2066  s..  - Benefit f
-00001770: 726f 6d20 2a2a 4869 6572 6172 6368 6963  rom **Hierarchic
-00001780: 616c 2053 7461 7465 204d 616e 6167 656d  al State Managem
-00001790: 656e 742a 2a2c 2065 6e73 7572 696e 6720  ent**, ensuring 
-000017a0: 6d6f 6475 6c61 7220 616e 6420 636c 6561  modular and clea
-000017b0: 6e20 7072 6f67 7261 6d6d 696e 672e 0a20  n programming.. 
-000017c0: 202d 204a 756d 7073 7461 7274 2079 6f75   - Jumpstart you
-000017d0: 7220 6a6f 7572 6e65 7920 7769 7468 206f  r journey with o
-000017e0: 7572 205b 4465 7461 696c 6564 2054 7574  ur [Detailed Tut
-000017f0: 6f72 6961 6c5d 2868 7474 7073 3a2f 2f65  orial](https://e
-00001800: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
-00001810: 696f 2f65 6e2f 6c61 7465 7374 2f67 7569  io/en/latest/gui
-00001820: 6465 2f62 6173 6963 732f 696e 6465 782e  de/basics/index.
-00001830: 6874 6d6c 292e 0a0a 2d2d 2d0a 0a23 2320  html)...---..## 
-00001840: 436f 6d70 7265 6865 6e73 6976 6520 4576  Comprehensive Ev
-00001850: 6f6c 7574 696f 6e61 7279 2041 6c67 6f72  olutionary Algor
-00001860: 6974 686d 730a 0a23 2323 2053 696e 676c  ithms..### Singl
-00001870: 652d 4f62 6a65 6374 6976 6520 4f70 7469  e-Objective Opti
-00001880: 6d69 7a61 7469 6f6e 0a0a 7c20 4361 7465  mization..| Cate
-00001890: 676f 7279 2020 2020 2020 2020 2020 2020  gory            
-000018a0: 2020 2020 2020 2020 7c20 416c 676f 7269          | Algori
-000018b0: 7468 6d20 4e61 6d65 7320 2020 2020 2020  thm Names       
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d        |.| ------
-000018e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000018f0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-00001900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001920: 2d2d 207c 0a7c 2044 6966 6665 7265 6e74  -- |.| Different
-00001930: 6961 6c20 4576 6f6c 7574 696f 6e20 2020  ial Evolution   
-00001940: 2020 207c 2043 6f44 452c 204a 6144 452c     | CoDE, JaDE,
-00001950: 2053 6144 452c 2053 4841 4445 2c20 494d   SaDE, SHADE, IM
-00001960: 4f44 452c 202e 2e2e 2020 2020 2020 2020  ODE, ...        
-00001970: 7c0a 7c20 4576 6f6c 7574 696f 6e20 5374  |.| Evolution St
-00001980: 7261 7465 6779 2020 2020 2020 2020 7c20  rategy        | 
-00001990: 434d 412d 4553 2c20 5047 5045 2c20 4f70  CMA-ES, PGPE, Op
-000019a0: 656e 4553 2c20 4352 2d46 4d2d 4e45 532c  enES, CR-FM-NES,
-000019b0: 2078 4e45 532c 202e 2e2e 207c 0a7c 2050   xNES, ... |.| P
-000019c0: 6172 7469 636c 6520 5377 6172 6d20 4f70  article Swarm Op
-000019d0: 7469 6d69 7a61 7469 6f6e 207c 2046 4950  timization | FIP
-000019e0: 532c 2043 534f 2c20 4350 534f 2c20 434c  S, CSO, CPSO, CL
-000019f0: 5053 4f2c 2053 4c2d 5053 4f2c 202e 2e2e  PSO, SL-PSO, ...
-00001a00: 2020 2020 2020 2020 7c0a 0a23 2323 204d          |..### M
-00001a10: 756c 7469 2d4f 626a 6563 7469 7665 204f  ulti-Objective O
-00001a20: 7074 696d 697a 6174 696f 6e0a 0a7c 2043  ptimization..| C
-00001a30: 6174 6567 6f72 7920 2020 2020 2020 2020  ategory         
-00001a40: 2020 7c20 416c 676f 7269 7468 6d20 4e61    | Algorithm Na
-00001a50: 6d65 7320 2020 2020 2020 2020 2020 2020  mes             
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d      |.| --------
-00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
-00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a 7c20  ----------- |.| 
-00001ac0: 446f 6d69 6e61 6e63 652d 6261 7365 6420  Dominance-based 
-00001ad0: 2020 207c 204e 5347 412d 4949 2c20 4e53     | NSGA-II, NS
-00001ae0: 4741 2d49 4949 2c20 5350 4541 322c 2042  GA-III, SPEA2, B
-00001af0: 6947 452c 204b 6e45 412c 202e 2e2e 2020  iGE, KnEA, ...  
-00001b00: 2020 2020 7c0a 7c20 4465 636f 6d70 6f73      |.| Decompos
-00001b10: 6974 696f 6e2d 6261 7365 647c 204d 4f45  ition-based| MOE
-00001b20: 412f 442c 2052 5645 412c 2074 2d44 4541  A/D, RVEA, t-DEA
-00001b30: 2c20 4d4f 4541 442d 4d32 4d2c 2045 4147  , MOEAD-M2M, EAG
-00001b40: 2d4d 4f45 4144 2c20 2e2e 2e20 7c0a 7c20  -MOEAD, ... |.| 
-00001b50: 496e 6469 6361 746f 722d 6261 7365 6420  Indicator-based 
-00001b60: 2020 207c 2049 4245 412c 2048 7970 452c     | IBEA, HypE,
-00001b70: 2053 5241 2c20 4d61 4f45 412d 4947 442c   SRA, MaOEA-IGD,
-00001b80: 2041 522d 4d4f 4541 2c20 2e2e 2e20 2020   AR-MOEA, ...   
-00001b90: 2020 2020 7c0a 0a46 6f72 2061 2063 6f6d      |..For a com
-00001ba0: 7072 6568 656e 7369 7665 206c 6973 7420  prehensive list 
-00001bb0: 616e 6420 6675 7274 6865 7220 6465 7461  and further deta
-00001bc0: 696c 7320 6f66 2061 6c6c 2061 6c67 6f72  ils of all algor
-00001bd0: 6974 686d 732c 2070 6c65 6173 6520 6368  ithms, please ch
-00001be0: 6563 6b20 7468 6520 5b41 5049 2044 6f63  eck the [API Doc
-00001bf0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001c00: 733a 2f2f 6576 6f78 2e72 6561 6474 6865  s://evox.readthe
-00001c10: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00001c20: 742f 6170 692f 616c 676f 7269 7468 6d73  t/api/algorithms
-00001c30: 2f69 6e64 6578 2e68 746d 6c29 2e0a 0a23  /index.html)...#
-00001c40: 2320 4469 7665 7273 6520 4265 6e63 686d  # Diverse Benchm
-00001c50: 6172 6b20 5072 6f62 6c65 6d73 0a0a 7c20  ark Problems..| 
-00001c60: 4361 7465 676f 7279 2020 2020 2020 7c20  Category      | 
-00001c70: 5072 6f62 6c65 6d20 4e61 6d65 7320 2020  Problem Names   
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2020 2020 7c0a 7c20 2d2d 2d2d          |.| ----
-00001ca0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00001cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cd0: 2d2d 2d20 7c0a 7c20 4e75 6d65 7269 6361  --- |.| Numerica
-00001ce0: 6c20 2020 2020 7c20 4454 4c5a 2c20 4c53  l     | DTLZ, LS
-00001cf0: 4d4f 502c 204d 6146 2c20 5a44 542c 2043  MOP, MaF, ZDT, C
-00001d00: 4543 2732 322c 2020 2e2e 2e20 2020 207c  EC'22,  ...    |
-00001d10: 0a7c 204e 6575 726f 6576 6f6c 7574 696f  .| Neuroevolutio
-00001d20: 6e7c 2042 7261 782c 2047 796d 2c20 546f  n| Brax, Gym, To
-00001d30: 7263 6856 6973 696f 6e20 4461 7461 7365  rchVision Datase
-00001d40: 742c 202e 2e2e 2020 2020 7c0a 0a46 6f72  t, ...    |..For
-00001d50: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
-00001d60: 206c 6973 7420 616e 6420 6675 7274 6865   list and furthe
-00001d70: 7220 6465 7461 696c 7320 6f66 2061 6c6c  r details of all
-00001d80: 2062 656e 6368 6d61 726b 2070 726f 626c   benchmark probl
-00001d90: 656d 732c 2070 6c65 6173 6520 6368 6563  ems, please chec
-00001da0: 6b20 7468 6520 5b41 5049 2044 6f63 756d  k the [API Docum
-00001db0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00001dc0: 2f2f 6576 6f78 2e72 6561 6474 6865 646f  //evox.readthedo
-00001dd0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001de0: 6170 692f 7072 6f62 6c65 6d73 2f69 6e64  api/problems/ind
-00001df0: 6578 2e68 746d 6c29 2e0a 0a0a 2323 2053  ex.html)....## S
-00001e00: 6574 7469 6e67 2055 7020 4576 6f58 0a0a  etting Up EvoX..
-00001e10: 496e 7374 616c 6c20 6065 766f 7860 2065  Install `evox` e
-00001e20: 6666 6f72 746c 6573 736c 7920 7669 6120  ffortlessly via 
-00001e30: 6070 6970 603a 0a60 6060 6261 7368 0a70  `pip`:.```bash.p
-00001e40: 6970 2069 6e73 7461 6c6c 2065 766f 780a  ip install evox.
-00001e50: 6060 600a 0a2a 2a4e 6f74 652a 2a3a 2054  ```..**Note**: T
-00001e60: 6f20 696e 7374 616c 6c20 4576 6f58 2077  o install EvoX w
-00001e70: 6974 6820 4a41 5820 616e 6420 6861 7264  ith JAX and hard
-00001e80: 7761 7265 2061 6363 656c 6572 6174 696f  ware acceleratio
-00001e90: 6e20 6361 7061 6269 6c69 7469 6573 2c20  n capabilities, 
-00001ea0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-00001eb0: 6f75 7220 636f 6d70 7265 6865 6e73 6976  our comprehensiv
-00001ec0: 6520 5b49 6e73 7461 6c6c 6174 696f 6e20  e [Installation 
-00001ed0: 4775 6964 655d 2868 7474 7073 3a2f 2f65  Guide](https://e
-00001ee0: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
-00001ef0: 696f 2f65 6e2f 6c61 7465 7374 2f67 7569  io/en/latest/gui
-00001f00: 6465 2f69 6e73 7461 6c6c 2e68 746d 6c29  de/install.html)
-00001f10: 2e0a 0a0a 2323 2051 7569 636b 2053 7461  ....## Quick Sta
-00001f20: 7274 0a0a 4b69 636b 7374 6172 7420 796f  rt..Kickstart yo
-00001f30: 7572 206a 6f75 726e 6579 2077 6974 6820  ur journey with 
-00001f40: 4576 6f58 2069 6e20 6a75 7374 2061 2066  EvoX in just a f
-00001f50: 6577 2073 696d 706c 6520 7374 6570 733a  ew simple steps:
-00001f60: 0a31 2e20 2a2a 496d 706f 7274 206e 6563  .1. **Import nec
-00001f70: 6573 7361 7279 206d 6f64 756c 6573 2a2a  essary modules**
-00001f80: 3a0a 6060 6070 7974 686f 6e0a 696d 706f  :.```python.impo
-00001f90: 7274 2065 766f 780a 6672 6f6d 2065 766f  rt evox.from evo
-00001fa0: 7820 696d 706f 7274 2061 6c67 6f72 6974  x import algorit
-00001fb0: 686d 732c 2070 726f 626c 656d 732c 2077  hms, problems, w
-00001fc0: 6f72 6b66 6c6f 7773 0a60 6060 0a32 2e20  orkflows.```.2. 
-00001fd0: 2a2a 436f 6e66 6967 7572 6520 616e 2061  **Configure an a
-00001fe0: 6c67 6f72 6974 686d 2061 6e64 2064 6566  lgorithm and def
-00001ff0: 696e 6520 6120 7072 6f62 6c65 6d2a 2a3a  ine a problem**:
-00002000: 0a60 6060 7079 7468 6f6e 0a70 736f 203d  .```python.pso =
-00002010: 2061 6c67 6f72 6974 686d 732e 5053 4f28   algorithms.PSO(
-00002020: 0a20 2020 206c 623d 6a6e 702e 6675 6c6c  .    lb=jnp.full
-00002030: 2873 6861 7065 3d28 322c 292c 2066 696c  (shape=(2,), fil
-00002040: 6c5f 7661 6c75 653d 2d33 3229 2c0a 2020  l_value=-32),.  
-00002050: 2020 7562 3d6a 6e70 2e66 756c 6c28 7368    ub=jnp.full(sh
-00002060: 6170 653d 2832 2c29 2c20 6669 6c6c 5f76  ape=(2,), fill_v
-00002070: 616c 7565 3d33 3229 2c0a 2020 2020 706f  alue=32),.    po
-00002080: 705f 7369 7a65 3d31 3030 2c0a 290a 6163  p_size=100,.).ac
-00002090: 6b6c 6579 203d 2070 726f 626c 656d 732e  kley = problems.
-000020a0: 6e75 6d65 7269 6361 6c2e 4163 6b6c 6579  numerical.Ackley
-000020b0: 2829 0a60 6060 0a33 2e20 2a2a 436f 6d70  ().```.3. **Comp
-000020c0: 6f73 6520 616e 6420 696e 6974 6961 6c69  ose and initiali
-000020d0: 7a65 2074 6865 2077 6f72 6b66 6c6f 772a  ze the workflow*
-000020e0: 2a3a 0a60 6060 7079 7468 6f6e 0a77 6f72  *:.```python.wor
-000020f0: 6b66 6c6f 7720 3d20 776f 726b 666c 6f77  kflow = workflow
-00002100: 732e 5374 6457 6f72 6b66 6c6f 7728 7073  s.StdWorkflow(ps
-00002110: 6f2c 2061 636b 6c65 7929 0a6b 6579 203d  o, ackley).key =
-00002120: 206a 6178 2e72 616e 646f 6d2e 5052 4e47   jax.random.PRNG
-00002130: 4b65 7928 3432 290a 7374 6174 6520 3d20  Key(42).state = 
-00002140: 776f 726b 666c 6f77 2e69 6e69 7428 6b65  workflow.init(ke
-00002150: 7929 0a60 6060 0a34 2e20 2a2a 5275 6e20  y).```.4. **Run 
-00002160: 7468 6520 776f 726b 666c 6f77 2a2a 3a0a  the workflow**:.
-00002170: 6060 6070 7974 686f 6e0a 2320 4578 6563  ```python.# Exec
-00002180: 7574 6520 7468 6520 776f 726b 666c 6f77  ute the workflow
-00002190: 2066 6f72 2031 3030 2069 7465 7261 7469   for 100 iterati
-000021a0: 6f6e 730a 666f 7220 6920 696e 2072 616e  ons.for i in ran
-000021b0: 6765 2831 3030 293a 0a20 2020 2073 7461  ge(100):.    sta
-000021c0: 7465 203d 2077 6f72 6b66 6c6f 772e 7374  te = workflow.st
-000021d0: 6570 2873 7461 7465 290a 6060 600a 0a23  ep(state).```..#
-000021e0: 2320 5573 652d 6361 7365 7320 616e 6420  # Use-cases and 
-000021f0: 4170 706c 6963 6174 696f 6e73 0a0a 5472  Applications..Tr
-00002200: 7920 6f75 7420 7265 6164 792d 746f 2d70  y out ready-to-p
-00002210: 6c61 7920 6578 616d 706c 6573 2069 6e20  lay examples in 
-00002220: 796f 7572 2062 726f 7773 6572 2077 6974  your browser wit
-00002230: 6820 436f 6c61 623a 0a0a 7c20 4578 616d  h Colab:..| Exam
-00002240: 706c 6520 7c20 4c69 6e6b 207c 0a7c 202d  ple | Link |.| -
-00002250: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d20 7c0a  ------ | ---- |.
-00002260: 7c20 4261 7369 6320 5573 6167 6520 7c20  | Basic Usage | 
-00002270: 5b21 5b4f 7065 6e20 696e 2043 6f6c 6162  [![Open in Colab
-00002280: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00002290: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-000022a0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
-000022b0: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
-000022c0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-000022d0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
-000022e0: 6974 6875 622f 454d 492d 4772 6f75 702f  ithub/EMI-Group/
-000022f0: 6576 6f78 2f62 6c6f 622f 6d61 696e 2f64  evox/blob/main/d
-00002300: 6f63 732f 736f 7572 6365 2f67 7569 6465  ocs/source/guide
-00002310: 2f62 6173 6963 732f 312d 7374 6172 742e  /basics/1-start.
-00002320: 6970 796e 6229 207c 0a7c 204e 756d 6572  ipynb) |.| Numer
-00002330: 6963 616c 204f 7074 696d 697a 6174 696f  ical Optimizatio
-00002340: 6e20 7c20 5b21 5b4f 7065 6e20 696e 2043  n | [![Open in C
-00002350: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
-00002360: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002370: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00002380: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
-00002390: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-000023a0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-000023b0: 6f6d 2f67 6974 6875 622f 454d 492d 4772  om/github/EMI-Gr
-000023c0: 6f75 702f 6576 6f78 2f62 6c6f 622f 6d61  oup/evox/blob/ma
-000023d0: 696e 2f64 6f63 732f 736f 7572 6365 2f65  in/docs/source/e
-000023e0: 7861 6d70 6c65 2f70 736f 5f61 636b 6c65  xample/pso_ackle
-000023f0: 792e 6970 796e 6229 207c 0a7c 204e 6575  y.ipynb) |.| Neu
-00002400: 726f 6576 6f6c 7574 696f 6e20 7769 7468  roevolution with
-00002410: 2047 796d 207c 205b 215b 4f70 656e 2069   Gym | [![Open i
-00002420: 6e20 436f 6c61 625d 2868 7474 7073 3a2f  n Colab](https:/
-00002430: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00002440: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
-00002450: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
-00002460: 6729 5d28 6874 7470 733a 2f2f 636f 6c61  g)](https://cola
-00002470: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00002480: 652e 636f 6d2f 6769 7468 7562 2f45 4d49  e.com/github/EMI
-00002490: 2d47 726f 7570 2f65 766f 782f 626c 6f62  -Group/evox/blob
-000024a0: 2f6d 6169 6e2f 646f 6373 2f73 6f75 7263  /main/docs/sourc
-000024b0: 652f 6578 616d 706c 652f 6779 6d5f 636c  e/example/gym_cl
-000024c0: 6173 7369 635f 636f 6e74 726f 6c2e 6970  assic_control.ip
-000024d0: 796e 6229 207c 0a7c 204e 6575 726f 6576  ynb) |.| Neuroev
-000024e0: 6f6c 7574 696f 6e20 7769 7468 2042 7261  olution with Bra
-000024f0: 7820 7c20 5b21 5b4f 7065 6e20 696e 2043  x | [![Open in C
-00002500: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
-00002510: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002520: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00002530: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
-00002540: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00002550: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00002560: 6f6d 2f67 6974 6875 622f 454d 492d 4772  om/github/EMI-Gr
-00002570: 6f75 702f 6576 6f78 2f62 6c6f 622f 6d61  oup/evox/blob/ma
-00002580: 696e 2f64 6f63 732f 736f 7572 6365 2f67  in/docs/source/g
-00002590: 7569 6465 2f62 6173 6963 732f 322d 7072  uide/basics/2-pr
-000025a0: 6f62 6c65 6d73 2e69 7079 6e62 2920 7c0a  oblems.ipynb) |.
-000025b0: 7c20 4375 7374 6f6d 2041 6c67 6f72 6974  | Custom Algorit
-000025c0: 686d 2f50 726f 626c 656d 207c 205b 215b  hm/Problem | [![
-000025d0: 4f70 656e 2069 6e20 436f 6c61 625d 2868  Open in Colab](h
-000025e0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-000025f0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00002600: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00002610: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00002620: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00002630: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00002640: 7562 2f45 4d49 2d47 726f 7570 2f65 766f  ub/EMI-Group/evo
-00002650: 782f 626c 6f62 2f6d 6169 6e2f 646f 6373  x/blob/main/docs
-00002660: 2f73 6f75 7263 652f 6578 616d 706c 652f  /source/example/
-00002670: 6375 7374 6f6d 5f61 6c67 6f72 6974 686d  custom_algorithm
-00002680: 5f61 6e64 5f70 726f 626c 656d 2e69 7079  _and_problem.ipy
-00002690: 6e62 2920 7c0a 0a46 6f72 206d 6f72 6520  nb) |..For more 
-000026a0: 7573 652d 6361 7365 7320 616e 6420 6170  use-cases and ap
-000026b0: 706c 6963 6174 696f 6e73 2c20 706c 6561  plications, plea
-000026c0: 6520 6368 6563 6b20 6f75 7420 5b45 7861  e check out [Exa
-000026d0: 6d70 6c65 2044 6972 6563 746f 7279 5d28  mple Directory](
-000026e0: 6874 7470 733a 2f2f 6576 6f78 2e72 6561  https://evox.rea
-000026f0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00002700: 6174 6573 742f 6578 616d 706c 652f 696e  atest/example/in
-00002710: 6465 782e 6874 6d6c 292e 0a0a 2323 2043  dex.html)...## C
-00002720: 6f6d 6d75 6e69 7479 2026 2053 7570 706f  ommunity & Suppo
-00002730: 7274 0a0a 2d20 456e 6761 6765 2069 6e20  rt..- Engage in 
-00002740: 6469 7363 7573 7369 6f6e 7320 616e 6420  discussions and 
-00002750: 7368 6172 6520 796f 7572 2065 7870 6572  share your exper
-00002760: 6965 6e63 6573 206f 6e20 5b47 6974 4875  iences on [GitHu
-00002770: 6220 4469 7363 7573 7369 6f6e 2042 6f61  b Discussion Boa
-00002780: 7264 5d28 6874 7470 733a 2f2f 6769 7468  rd](https://gith
-00002790: 7562 2e63 6f6d 2f45 4d49 2d47 726f 7570  ub.com/EMI-Group
-000027a0: 2f65 766f 782f 6469 7363 7573 7369 6f6e  /evox/discussion
-000027b0: 7329 2e0a 2d20 4a6f 696e 206f 7572 2051  s)..- Join our Q
-000027c0: 5120 6772 6f75 7020 2849 443a 2032 3937  Q group (ID: 297
-000027d0: 3936 3937 3137 292e 0a2d 2048 656c 7020  969717)..- Help 
-000027e0: 7769 7468 2074 6865 2074 7261 6e73 6c61  with the transla
-000027f0: 7469 6f6e 206f 6620 7468 6520 646f 6375  tion of the docu
-00002800: 6d65 6e74 6174 696f 6e20 6f6e 205b 5765  mentation on [We
-00002810: 626c 6174 655d 2868 7474 7073 3a2f 2f68  blate](https://h
-00002820: 6f73 7465 642e 7765 626c 6174 652e 6f72  osted.weblate.or
-00002830: 672f 7072 6f6a 6563 7473 2f65 766f 782f  g/projects/evox/
-00002840: 6576 6f78 2f29 2e0a 5765 2063 7572 7265  evox/)..We curre
-00002850: 6e74 6c79 2073 7570 706f 7274 2074 7261  ntly support tra
-00002860: 6e73 6c61 7469 6f6e 7320 696e 2074 776f  nslations in two
-00002870: 206c 616e 6775 6167 6573 2c20 5b45 6e67   languages, [Eng
-00002880: 6c69 7368 5d28 6874 7470 733a 2f2f 6576  lish](https://ev
-00002890: 6f78 2e72 6561 6474 6865 646f 6373 2e69  ox.readthedocs.i
-000028a0: 6f2f 656e 2f6c 6174 6573 742f 2920 2f20  o/en/latest/) / 
-000028b0: 5be4 b8ad e696 875d 2868 7474 7073 3a2f  [......](https:/
-000028c0: 2f65 766f 782e 7265 6164 7468 6564 6f63  /evox.readthedoc
-000028d0: 732e 696f 2f7a 682f 6c61 7465 7374 2f29  s.io/zh/latest/)
-000028e0: 2e0a 2d20 4f66 6669 6369 616c 2057 6562  ..- Official Web
-000028f0: 7369 7465 3a20 6874 7470 733a 2f2f 6576  site: https://ev
-00002900: 6f78 2e67 726f 7570 2f0a 0a23 2320 5369  ox.group/..## Si
-00002910: 7374 6572 2050 726f 6a65 6374 730a 0a2d  ster Projects..-
-00002920: 2045 766f 5842 656e 6368 3a20 4120 6265   EvoXBench: A be
-00002930: 6e63 686d 6172 6b20 706c 6174 666f 726d  nchmark platform
-00002940: 2066 6f72 204e 6575 7261 6c20 4172 6368   for Neural Arch
-00002950: 6974 6563 7574 7265 2053 6561 7263 6820  itecutre Search 
-00002960: 284e 4153 2920 7769 7468 6f75 7420 7468  (NAS) without th
-00002970: 6520 7265 7175 6972 656d 656e 7420 6f66  e requirement of
-00002980: 2047 5055 732f 5079 546f 7263 682f 5465   GPUs/PyTorch/Te
-00002990: 6e73 6f72 666c 6f77 2c20 7375 7070 6f72  nsorflow, suppor
-000029a0: 7469 6e67 2076 6172 696f 7573 2070 726f  ting various pro
-000029b0: 6772 616d 6d69 6e67 206c 616e 6775 6167  gramming languag
-000029c0: 6573 2073 7563 6820 6173 204a 6176 612c  es such as Java,
-000029d0: 204d 6174 6c61 622c 2050 7974 686f 6e2c   Matlab, Python,
-000029e0: 2065 6374 2e20 4368 6563 6b20 6f75 7420   ect. Check out 
-000029f0: 5b68 6572 655d 2868 7474 7073 3a2f 2f67  [here](https://g
-00002a00: 6974 6875 622e 636f 6d2f 454d 492d 4772  ithub.com/EMI-Gr
-00002a10: 6f75 702f 6576 6f78 6265 6e63 6829 2e0a  oup/evoxbench)..
-00002a20: 0a23 2320 4369 7469 6e67 2045 766f 580a  .## Citing EvoX.
-00002a30: 0a49 6620 796f 7520 7573 6520 4576 6f58  .If you use EvoX
-00002a40: 2069 6e20 796f 7572 2072 6573 6561 7263   in your researc
-00002a50: 6820 616e 6420 7761 6e74 2074 6f20 6369  h and want to ci
-00002a60: 7465 2069 7420 696e 2079 6f75 7220 776f  te it in your wo
-00002a70: 726b 2c20 706c 6561 7365 2075 7365 3a0a  rk, please use:.
-00002a80: 6060 600a 4061 7274 6963 6c65 7b65 766f  ```.@article{evo
-00002a90: 782c 0a20 2074 6974 6c65 203d 207b 7b45  x,.  title = {{E
-00002aa0: 766f 587d 3a20 7b41 7d20 7b44 6973 7472  voX}: {A} {Distr
-00002ab0: 6962 7574 6564 7d20 7b47 5055 7d2d 6163  ibuted} {GPU}-ac
-00002ac0: 6365 6c65 7261 7465 6420 7b46 7261 6d65  celerated {Frame
-00002ad0: 776f 726b 7d20 666f 7220 7b53 6361 6c61  work} for {Scala
-00002ae0: 626c 657d 207b 4576 6f6c 7574 696f 6e61  ble} {Evolutiona
-00002af0: 7279 7d20 7b43 6f6d 7075 7461 7469 6f6e  ry} {Computation
-00002b00: 7d7d 2c0a 2020 6175 7468 6f72 203d 207b  }},.  author = {
-00002b10: 4875 616e 672c 2042 6569 6368 656e 2061  Huang, Beichen a
-00002b20: 6e64 2043 6865 6e67 2c20 5261 6e20 616e  nd Cheng, Ran an
-00002b30: 6420 4c69 2c20 5a68 756f 7a68 616f 2061  d Li, Zhuozhao a
-00002b40: 6e64 204a 696e 2c20 5961 6f63 6875 2061  nd Jin, Yaochu a
-00002b50: 6e64 2054 616e 2c20 4b61 7920 4368 656e  nd Tan, Kay Chen
-00002b60: 7d2c 0a20 206a 6f75 726e 616c 203d 207b  },.  journal = {
-00002b70: 4945 4545 2054 7261 6e73 6163 7469 6f6e  IEEE Transaction
-00002b80: 7320 6f6e 2045 766f 6c75 7469 6f6e 6172  s on Evolutionar
-00002b90: 7920 436f 6d70 7574 6174 696f 6e7d 2c0a  y Computation},.
-00002ba0: 2020 7965 6172 203d 2032 3032 342c 0a20    year = 2024,. 
-00002bb0: 2064 6f69 203d 207b 3130 2e31 3130 392f   doi = {10.1109/
-00002bc0: 5445 5643 2e32 3032 342e 3333 3838 3535  TEVC.2024.338855
-00002bd0: 307d 0a7d 0a60 6060 0a0a 2323 2053 7461  0}.}.```..## Sta
-00002be0: 7220 4869 7374 6f72 790a 0a5b 215b 5374  r History..[![St
-00002bf0: 6172 2048 6973 746f 7279 2043 6861 7274  ar History Chart
-00002c00: 5d28 6874 7470 733a 2f2f 6170 692e 7374  ](https://api.st
-00002c10: 6172 2d68 6973 746f 7279 2e63 6f6d 2f73  ar-history.com/s
-00002c20: 7667 3f72 6570 6f73 3d45 4d49 2d47 726f  vg?repos=EMI-Gro
-00002c30: 7570 2f65 766f 7826 7479 7065 3d44 6174  up/evox&type=Dat
-00002c40: 6529 5d28 6874 7470 733a 2f2f 7374 6172  e)](https://star
-00002c50: 2d68 6973 746f 7279 2e63 6f6d 2f23 454d  -history.com/#EM
-00002c60: 492d 4772 6f75 702f 6576 6f78 2644 6174  I-Group/evox&Dat
-00002c70: 6529 0a0a 0a0a                           e)....
+00000a70: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
+00000a80: 7569 7265 732d 4469 7374 3a20 7465 6e73  uires-Dist: tens
+00000a90: 6f72 666c 6f77 3e3d 322e 3132 2e30 3b20  orflow>=2.12.0; 
+00000aa0: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
+00000ab0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000ac0: 7669 730a 5265 7175 6972 6573 2d44 6973  vis.Requires-Dis
+00000ad0: 743a 2070 6c6f 746c 793e 3d35 2e30 2e30  t: plotly>=5.0.0
+00000ae0: 3b20 6578 7472 6120 3d3d 2022 7669 7322  ; extra == "vis"
+00000af0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000b00: 7061 6e64 6173 3e3d 322e 302e 303b 2065  pandas>=2.0.0; e
+00000b10: 7874 7261 203d 3d20 2276 6973 220a 5072  xtra == "vis".Pr
+00000b20: 6f76 6964 6573 2d45 7874 7261 3a20 6779  ovides-Extra: gy
+00000b30: 6d6e 6173 6975 6d0a 5265 7175 6972 6573  mnasium.Requires
+00000b40: 2d44 6973 743a 2067 796d 6e61 7369 756d  -Dist: gymnasium
+00000b50: 3e3d 302e 3239 2e30 3b20 6578 7472 6120  >=0.29.0; extra 
+00000b60: 3d3d 2022 6779 6d6e 6173 6975 6d22 0a50  == "gymnasium".P
+00000b70: 726f 7669 6465 732d 4578 7472 613a 2065  rovides-Extra: e
+00000b80: 6e76 706f 6f6c 0a52 6571 7569 7265 732d  nvpool.Requires-
+00000b90: 4469 7374 3a20 656e 7670 6f6f 6c3e 3d30  Dist: envpool>=0
+00000ba0: 2e38 2e30 3b20 6578 7472 6120 3d3d 2022  .8.0; extra == "
+00000bb0: 656e 7670 6f6f 6c22 0a50 726f 7669 6465  envpool".Provide
+00000bc0: 732d 4578 7472 613a 206e 6575 726f 6576  s-Extra: neuroev
+00000bd0: 6f6c 7574 696f 6e0a 5265 7175 6972 6573  olution.Requires
+00000be0: 2d44 6973 743a 2074 656e 736f 7266 6c6f  -Dist: tensorflo
+00000bf0: 772d 6461 7461 7365 7473 3e3d 342e 302e  w-datasets>=4.0.
+00000c00: 303b 2065 7874 7261 203d 3d20 226e 6575  0; extra == "neu
+00000c10: 726f 6576 6f6c 7574 696f 6e22 0a52 6571  roevolution".Req
+00000c20: 7569 7265 732d 4469 7374 3a20 6772 6169  uires-Dist: grai
+00000c30: 6e3e 3d30 2e31 2e30 3b20 6578 7472 6120  n>=0.1.0; extra 
+00000c40: 3d3d 2022 6e65 7572 6f65 766f 6c75 7469  == "neuroevoluti
+00000c50: 6f6e 220a 5265 7175 6972 6573 2d44 6973  on".Requires-Dis
+00000c60: 743a 2062 7261 783e 3d30 2e31 2e30 3b20  t: brax>=0.1.0; 
+00000c70: 6578 7472 6120 3d3d 2022 6e65 7572 6f65  extra == "neuroe
+00000c80: 766f 6c75 7469 6f6e 220a 5072 6f76 6964  volution".Provid
+00000c90: 6573 2d45 7874 7261 3a20 6469 7374 7269  es-Extra: distri
+00000ca0: 6275 7465 640a 5265 7175 6972 6573 2d44  buted.Requires-D
+00000cb0: 6973 743a 2072 6179 3e3d 322e 302e 303b  ist: ray>=2.0.0;
+00000cc0: 2065 7874 7261 203d 3d20 2264 6973 7472   extra == "distr
+00000cd0: 6962 7574 6564 220a 5072 6f76 6964 6573  ibuted".Provides
+00000ce0: 2d45 7874 7261 3a20 6675 6c6c 0a52 6571  -Extra: full.Req
+00000cf0: 7569 7265 732d 4469 7374 3a20 6779 6d6e  uires-Dist: gymn
+00000d00: 6173 6975 6d3e 3d30 2e32 392e 303b 2065  asium>=0.29.0; e
+00000d10: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
+00000d20: 6571 7569 7265 732d 4469 7374 3a20 7261  equires-Dist: ra
+00000d30: 793e 3d32 2e30 2e30 3b20 6578 7472 6120  y>=2.0.0; extra 
+00000d40: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000d50: 6573 2d44 6973 743a 2065 6e76 706f 6f6c  es-Dist: envpool
+00000d60: 3e3d 302e 382e 303b 2065 7874 7261 203d  >=0.8.0; extra =
+00000d70: 3d20 2266 756c 6c22 0a52 6571 7569 7265  = "full".Require
+00000d80: 732d 4469 7374 3a20 6770 6a61 783e 3d30  s-Dist: gpjax>=0
+00000d90: 2e38 2e30 3b20 6578 7472 6120 3d3d 2022  .8.0; extra == "
+00000da0: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+00000db0: 6973 743a 2070 6c6f 746c 793e 3d35 2e30  ist: plotly>=5.0
+00000dc0: 2e30 3b20 6578 7472 6120 3d3d 2022 6675  .0; extra == "fu
+00000dd0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000de0: 743a 2070 616e 6461 733e 3d32 2e30 2e30  t: pandas>=2.0.0
+00000df0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+00000e00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000e10: 2074 656e 736f 7266 6c6f 772d 6461 7461   tensorflow-data
+00000e20: 7365 7473 3e3d 342e 302e 303b 2065 7874  sets>=4.0.0; ext
+00000e30: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+00000e40: 7569 7265 732d 4469 7374 3a20 6772 6169  uires-Dist: grai
+00000e50: 6e3e 3d30 2e31 2e30 3b20 6578 7472 6120  n>=0.1.0; extra 
+00000e60: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000e70: 6573 2d44 6973 743a 2062 7261 783e 3d30  es-Dist: brax>=0
+00000e80: 2e31 2e30 3b20 6578 7472 6120 3d3d 2022  .1.0; extra == "
+00000e90: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+00000ea0: 6973 743a 2070 6c6f 746c 793e 3d35 2e30  ist: plotly>=5.0
+00000eb0: 2e30 3b20 6578 7472 6120 3d3d 2022 6675  .0; extra == "fu
+00000ec0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000ed0: 743a 2070 616e 6461 733e 3d32 2e30 2e30  t: pandas>=2.0.0
+00000ee0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+00000ef0: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
+00000f00: 3a20 6770 0a52 6571 7569 7265 732d 4469  : gp.Requires-Di
+00000f10: 7374 3a20 6770 6a61 783e 3d30 2e38 2e30  st: gpjax>=0.8.0
+00000f20: 3b20 6578 7472 6120 3d3d 2022 6770 220a  ; extra == "gp".
+00000f30: 0a3c 6831 2061 6c69 676e 3d22 6365 6e74  .<h1 align="cent
+00000f40: 6572 223e 0a20 203c 7069 6374 7572 653e  er">.  <picture>
+00000f50: 0a20 2020 203c 736f 7572 6365 206d 6564  .    <source med
+00000f60: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
+00000f70: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
+00000f80: 2220 7372 6373 6574 3d22 646f 6373 2f73  " srcset="docs/s
+00000f90: 6f75 7263 652f 5f73 7461 7469 632f 6576  ource/_static/ev
+00000fa0: 6f78 5f6c 6f67 6f5f 6461 726b 2e70 6e67  ox_logo_dark.png
+00000fb0: 223e 0a20 2020 203c 736f 7572 6365 206d  ">.    <source m
+00000fc0: 6564 6961 3d22 2870 7265 6665 7273 2d63  edia="(prefers-c
+00000fd0: 6f6c 6f72 2d73 6368 656d 653a 206c 6967  olor-scheme: lig
+00000fe0: 6874 2922 2073 7263 7365 743d 2264 6f63  ht)" srcset="doc
+00000ff0: 732f 736f 7572 6365 2f5f 7374 6174 6963  s/source/_static
+00001000: 2f65 766f 785f 6c6f 676f 5f6c 6967 6874  /evox_logo_light
+00001010: 2e70 6e67 223e 0a20 2020 203c 696d 6720  .png">.    <img 
+00001020: 616c 743d 2245 766f 5820 4c6f 676f 2220  alt="EvoX Logo" 
+00001030: 6865 6967 6874 3d22 3132 3822 2077 6964  height="128" wid
+00001040: 7468 3d22 3530 3070 7822 2073 7263 3d22  th="500px" src="
+00001050: 646f 6373 2f73 6f75 7263 652f 5f73 7461  docs/source/_sta
+00001060: 7469 632f 6576 6f78 5f6c 6f67 6f5f 6c69  tic/evox_logo_li
+00001070: 6768 742e 706e 6722 3e0a 2020 3c2f 7069  ght.png">.  </pi
+00001080: 6374 7572 653e 0a3c 2f68 313e 0a0a 3c70  cture>.</h1>..<p
+00001090: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000010a0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000010b0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000010c0: 732f 3233 3031 2e31 3234 3537 223e 0a20  s/2301.12457">. 
+000010d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000010e0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000010f0: 2e69 6f2f 6261 6467 652f 7061 7065 722d  .io/badge/paper-
+00001100: 6172 7869 762d 7265 643f 7374 796c 653d  arxiv-red?style=
+00001110: 666f 722d 7468 652d 6261 6467 6522 2061  for-the-badge" a
+00001120: 6c74 3d22 4576 6f58 2050 6170 6572 206f  lt="EvoX Paper o
+00001130: 6e20 6172 5869 7622 3e0a 2020 3c2f 613e  n arXiv">.  </a>
+00001140: 0a0a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+00001150: 7073 3a2f 2f65 766f 782e 7265 6164 7468  ps://evox.readth
+00001160: 6564 6f63 732e 696f 2f22 3e0a 2020 2020  edocs.io/">.    
+00001170: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001180: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001190: 2f62 6164 6765 2f64 6f63 732d 7265 6164  /badge/docs-read
+000011a0: 7468 6564 6f63 732d 626c 7565 3f73 7479  thedocs-blue?sty
+000011b0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+000011c0: 2220 616c 743d 2245 766f 5820 446f 6375  " alt="EvoX Docu
+000011d0: 6d65 6e74 6174 696f 6e22 3e0a 2020 3c2f  mentation">.  </
+000011e0: 613e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  a>.</p>..<p alig
+000011f0: 6e3d 2263 656e 7465 7222 3e0a 2020 3c62  n="center">.  <b
+00001200: 3ef0 9f8c 9f44 6973 7472 6962 7574 6564  >....Distributed
+00001210: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
+00001220: 2046 7261 6d65 776f 726b 2066 6f72 2053   Framework for S
+00001230: 6361 6c61 626c 6520 4576 6f6c 7574 696f  calable Evolutio
+00001240: 6e61 7279 2043 6f6d 7075 7461 7469 6f6e  nary Computation
+00001250: f09f 8c9f 3c2f 623e 0a3c 2f70 3e0a 0a2d  ....</b>.</p>..-
+00001260: 2d2d 0a0a 2323 0a42 7569 6c64 696e 6720  --..##.Building 
+00001270: 7570 6f6e 205b 4a41 585d 2868 7474 7073  upon [JAX](https
+00001280: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
+00001290: 6f67 6c65 2f6a 6178 2920 616e 6420 5b52  ogle/jax) and [R
+000012a0: 6179 5d28 6874 7470 733a 2f2f 6769 7468  ay](https://gith
+000012b0: 7562 2e63 6f6d 2f72 6179 2d70 726f 6a65  ub.com/ray-proje
+000012c0: 6374 2f72 6179 292c 2045 766f 5820 6f66  ct/ray), EvoX of
+000012d0: 6665 7273 2061 2063 6f6d 7072 6568 656e  fers a comprehen
+000012e0: 7369 7665 2073 7569 7465 206f 6620 2a2a  sive suite of **
+000012f0: 3530 2b20 4576 6f6c 7574 696f 6e61 7279  50+ Evolutionary
+00001300: 2041 6c67 6f72 6974 686d 7320 2845 4173   Algorithms (EAs
+00001310: 292a 2a20 616e 6420 6120 7769 6465 2072  )** and a wide r
+00001320: 616e 6765 206f 6620 2a2a 3130 302b 2042  ange of **100+ B
+00001330: 656e 6368 6d61 726b 2050 726f 626c 656d  enchmark Problem
+00001340: 732a 2a2c 2061 6c6c 2062 656e 6566 6974  s**, all benefit
+00001350: 696e 6720 6672 6f6d 2064 6973 7472 6962  ing from distrib
+00001360: 7574 6564 2047 5055 2d61 6363 656c 6572  uted GPU-acceler
+00001370: 6174 696f 6e2e 2049 7420 6661 6369 6c69  ation. It facili
+00001380: 7461 7465 7320 6566 6669 6369 656e 7420  tates efficient 
+00001390: 6578 706c 6f72 6174 696f 6e20 6f66 2063  exploration of c
+000013a0: 6f6d 706c 6578 206f 7074 696d 697a 6174  omplex optimizat
+000013b0: 696f 6e20 6c61 6e64 7363 6170 6573 2c20  ion landscapes, 
+000013c0: 6566 6665 6374 6976 6520 7461 636b 6c69  effective tackli
+000013d0: 6e67 206f 6620 626c 6163 6b2d 626f 7820  ng of black-box 
+000013e0: 6f70 7469 6d69 7a61 7469 6f6e 2063 6861  optimization cha
+000013f0: 6c6c 656e 6765 732c 2061 6e64 2064 6565  llenges, and dee
+00001400: 7020 6469 7665 7320 696e 746f 206e 6575  p dives into neu
+00001410: 726f 6576 6f6c 7574 696f 6e20 7769 7468  roevolution with
+00001420: 205b 4272 6178 5d28 6874 7470 733a 2f2f   [Brax](https://
+00001430: 6769 7468 7562 2e63 6f6d 2f67 6f6f 676c  github.com/googl
+00001440: 652f 6272 6178 292e 2057 6974 6820 6120  e/brax). With a 
+00001450: 666f 756e 6461 7469 6f6e 2069 6e20 6675  foundation in fu
+00001460: 6e63 7469 6f6e 616c 2070 726f 6772 616d  nctional program
+00001470: 6d69 6e67 2061 6e64 2068 6965 7261 7263  ming and hierarc
+00001480: 6869 6361 6c20 7374 6174 6520 6d61 6e61  hical state mana
+00001490: 6765 6d65 6e74 2c20 4576 6f58 206f 6666  gement, EvoX off
+000014a0: 6572 7320 6120 7573 6572 2d66 7269 656e  ers a user-frien
+000014b0: 646c 7920 616e 6420 6d6f 6475 6c61 7220  dly and modular 
+000014c0: 6578 7065 7269 656e 6365 2e20 466f 7220  experience. For 
+000014d0: 6d6f 7265 2064 6574 6169 6c73 2c20 706c  more details, pl
+000014e0: 6561 7365 2072 6566 6572 2074 6f20 6f75  ease refer to ou
+000014f0: 7220 5b50 6170 6572 5d28 6874 7470 733a  r [Paper](https:
+00001500: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00001510: 3233 3031 2e31 3234 3537 2920 616e 6420  2301.12457) and 
+00001520: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
+00001530: 6874 7470 733a 2f2f 6576 6f78 2e72 6561  https://evox.rea
+00001540: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001550: 6174 6573 742f 2920 2f20 5be6 9687 e6a1  atest/) / [.....
+00001560: a35d 2868 7474 7073 3a2f 2f65 766f 782e  .](https://evox.
+00001570: 7265 6164 7468 6564 6f63 732e 696f 2f7a  readthedocs.io/z
+00001580: 682f 6c61 7465 7374 2f29 2e0a 0a2d 2d2d  h/latest/)...---
+00001590: 0a0a 2323 204b 6579 2046 6561 7475 7265  ..## Key Feature
+000015a0: 730a 0a2d 20f0 9f9a 8020 2a2a 4661 7374  s..- .... **Fast
+000015b0: 2050 6572 666f 726d 616e 6365 2a2a 3a0a   Performance**:.
+000015c0: 2020 2d20 4578 7065 7269 656e 6365 202a    - Experience *
+000015d0: 2a47 5055 2d41 6363 656c 6572 6174 6564  *GPU-Accelerated
+000015e0: 2a2a 206f 7074 696d 697a 6174 696f 6e2c  ** optimization,
+000015f0: 2061 6368 6965 7669 6e67 2073 7065 6564   achieving speed
+00001600: 7320 6f76 6572 2031 3030 7820 6661 7374  s over 100x fast
+00001610: 6572 2074 6861 6e20 7472 6164 6974 696f  er than traditio
+00001620: 6e61 6c20 6d65 7468 6f64 732e 0a20 202d  nal methods..  -
+00001630: 204c 6576 6572 6167 6520 7468 6520 706f   Leverage the po
+00001640: 7765 7220 6f66 202a 2a44 6973 7472 6962  wer of **Distrib
+00001650: 7574 6564 2057 6f72 6b66 6c6f 7773 2a2a  uted Workflows**
+00001660: 2066 6f72 2065 7665 6e20 6d6f 7265 2072   for even more r
+00001670: 6170 6964 206f 7074 696d 697a 6174 696f  apid optimizatio
+00001680: 6e2e 0a0a 2d20 f09f 8c90 202a 2a56 6572  n...- .... **Ver
+00001690: 7361 7469 6c65 204f 7074 696d 697a 6174  satile Optimizat
+000016a0: 696f 6e20 5375 6974 652a 2a3a 0a20 202d  ion Suite**:.  -
+000016b0: 2043 6174 6572 2074 6f20 616c 6c20 796f   Cater to all yo
+000016c0: 7572 206e 6565 6473 2077 6974 6820 626f  ur needs with bo
+000016d0: 7468 202a 2a53 696e 676c 652d 6f62 6a65  th **Single-obje
+000016e0: 6374 6976 652a 2a20 616e 6420 2a2a 4d75  ctive** and **Mu
+000016f0: 6c74 692d 6f62 6a65 6374 6976 652a 2a20  lti-objective** 
+00001700: 6f70 7469 6d69 7a61 7469 6f6e 2063 6170  optimization cap
+00001710: 6162 696c 6974 6965 732e 0a20 202d 2044  abilities..  - D
+00001720: 6976 6520 696e 746f 2061 2063 6f6d 7072  ive into a compr
+00001730: 6568 656e 7369 7665 206c 6962 7261 7279  ehensive library
+00001740: 206f 6620 2a2a 4265 6e63 686d 6172 6b20   of **Benchmark 
+00001750: 5072 6f62 6c65 6d73 2a2a 2c20 656e 7375  Problems**, ensu
+00001760: 7269 6e67 2072 6f62 7573 7420 7465 7374  ring robust test
+00001770: 696e 6720 616e 6420 6576 616c 7561 7469  ing and evaluati
+00001780: 6f6e 2e0a 2020 2d20 4578 706c 6f72 6520  on..  - Explore 
+00001790: 7468 6520 6672 6f6e 7469 6572 206f 6620  the frontier of 
+000017a0: 4149 2077 6974 6820 6578 7465 6e73 6976  AI with extensiv
+000017b0: 6520 746f 6f6c 7320 666f 7220 2a2a 4e65  e tools for **Ne
+000017c0: 7572 6f65 766f 6c75 7469 6f6e 2a2a 2074  uroevolution** t
+000017d0: 6173 6b73 2e0a 0a2d 20f0 9f9b a0ef b88f  asks...- .......
+000017e0: 202a 2a44 6573 6967 6e65 6420 666f 7220   **Designed for 
+000017f0: 5369 6d70 6c69 6369 7479 2a2a 3a0a 2020  Simplicity**:.  
+00001800: 2d20 456d 6272 6163 6520 7468 6520 656c  - Embrace the el
+00001810: 6567 616e 6365 206f 6620 2a2a 4675 6e63  egance of **Func
+00001820: 7469 6f6e 616c 2050 726f 6772 616d 6d69  tional Programmi
+00001830: 6e67 2a2a 2c20 7369 6d70 6c69 6679 696e  ng**, simplifyin
+00001840: 6720 636f 6d70 6c65 7820 616c 676f 7269  g complex algori
+00001850: 7468 6d69 6320 636f 6d70 6f73 6974 696f  thmic compositio
+00001860: 6e73 2e0a 2020 2d20 4265 6e65 6669 7420  ns..  - Benefit 
+00001870: 6672 6f6d 202a 2a48 6965 7261 7263 6869  from **Hierarchi
+00001880: 6361 6c20 5374 6174 6520 4d61 6e61 6765  cal State Manage
+00001890: 6d65 6e74 2a2a 2c20 656e 7375 7269 6e67  ment**, ensuring
+000018a0: 206d 6f64 756c 6172 2061 6e64 2063 6c65   modular and cle
+000018b0: 616e 2070 726f 6772 616d 6d69 6e67 2e0a  an programming..
+000018c0: 2020 2d20 4a75 6d70 7374 6172 7420 796f    - Jumpstart yo
+000018d0: 7572 206a 6f75 726e 6579 2077 6974 6820  ur journey with 
+000018e0: 6f75 7220 5b44 6574 6169 6c65 6420 5475  our [Detailed Tu
+000018f0: 746f 7269 616c 5d28 6874 7470 733a 2f2f  torial](https://
+00001900: 6576 6f78 2e72 6561 6474 6865 646f 6373  evox.readthedocs
+00001910: 2e69 6f2f 656e 2f6c 6174 6573 742f 6775  .io/en/latest/gu
+00001920: 6964 652f 6261 7369 6373 2f69 6e64 6578  ide/basics/index
+00001930: 2e68 746d 6c29 2e0a 0a2d 2d2d 0a0a 2323  .html)...---..##
+00001940: 2043 6f6d 7072 6568 656e 7369 7665 2045   Comprehensive E
+00001950: 766f 6c75 7469 6f6e 6172 7920 416c 676f  volutionary Algo
+00001960: 7269 7468 6d73 0a0a 2323 2320 5369 6e67  rithms..### Sing
+00001970: 6c65 2d4f 626a 6563 7469 7665 204f 7074  le-Objective Opt
+00001980: 696d 697a 6174 696f 6e0a 0a7c 2043 6174  imization..| Cat
+00001990: 6567 6f72 7920 2020 2020 2020 2020 2020  egory           
+000019a0: 2020 2020 2020 2020 207c 2041 6c67 6f72           | Algor
+000019b0: 6974 686d 204e 616d 6573 2020 2020 2020  ithm Names      
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 207c 0a7c 202d 2d2d 2d2d         |.| -----
+000019e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019f0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a20: 2d2d 2d20 7c0a 7c20 4469 6666 6572 656e  --- |.| Differen
+00001a30: 7469 616c 2045 766f 6c75 7469 6f6e 2020  tial Evolution  
+00001a40: 2020 2020 7c20 436f 4445 2c20 4a61 4445      | CoDE, JaDE
+00001a50: 2c20 5361 4445 2c20 5348 4144 452c 2049  , SaDE, SHADE, I
+00001a60: 4d4f 4445 2c20 2e2e 2e20 2020 2020 2020  MODE, ...       
+00001a70: 207c 0a7c 2045 766f 6c75 7469 6f6e 2053   |.| Evolution S
+00001a80: 7472 6174 6567 7920 2020 2020 2020 207c  trategy        |
+00001a90: 2043 4d41 2d45 532c 2050 4750 452c 204f   CMA-ES, PGPE, O
+00001aa0: 7065 6e45 532c 2043 522d 464d 2d4e 4553  penES, CR-FM-NES
+00001ab0: 2c20 784e 4553 2c20 2e2e 2e20 7c0a 7c20  , xNES, ... |.| 
+00001ac0: 5061 7274 6963 6c65 2053 7761 726d 204f  Particle Swarm O
+00001ad0: 7074 696d 697a 6174 696f 6e20 7c20 4649  ptimization | FI
+00001ae0: 5053 2c20 4353 4f2c 2043 5053 4f2c 2043  PS, CSO, CPSO, C
+00001af0: 4c50 534f 2c20 534c 2d50 534f 2c20 2e2e  LPSO, SL-PSO, ..
+00001b00: 2e20 2020 2020 2020 207c 0a0a 2323 2320  .        |..### 
+00001b10: 4d75 6c74 692d 4f62 6a65 6374 6976 6520  Multi-Objective 
+00001b20: 4f70 7469 6d69 7a61 7469 6f6e 0a0a 7c20  Optimization..| 
+00001b30: 4361 7465 676f 7279 2020 2020 2020 2020  Category        
+00001b40: 2020 207c 2041 6c67 6f72 6974 686d 204e     | Algorithm N
+00001b50: 616d 6573 2020 2020 2020 2020 2020 2020  ames            
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2020 2020 207c 0a7c 202d 2d2d 2d2d 2d2d       |.| -------
+00001b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c  ------------ |.|
+00001bc0: 2044 6f6d 696e 616e 6365 2d62 6173 6564   Dominance-based
+00001bd0: 2020 2020 7c20 4e53 4741 2d49 492c 204e      | NSGA-II, N
+00001be0: 5347 412d 4949 492c 2053 5045 4132 2c20  SGA-III, SPEA2, 
+00001bf0: 4269 4745 2c20 4b6e 4541 2c20 2e2e 2e20  BiGE, KnEA, ... 
+00001c00: 2020 2020 207c 0a7c 2044 6563 6f6d 706f       |.| Decompo
+00001c10: 7369 7469 6f6e 2d62 6173 6564 7c20 4d4f  sition-based| MO
+00001c20: 4541 2f44 2c20 5256 4541 2c20 742d 4445  EA/D, RVEA, t-DE
+00001c30: 412c 204d 4f45 4144 2d4d 324d 2c20 4541  A, MOEAD-M2M, EA
+00001c40: 472d 4d4f 4541 442c 202e 2e2e 207c 0a7c  G-MOEAD, ... |.|
+00001c50: 2049 6e64 6963 6174 6f72 2d62 6173 6564   Indicator-based
+00001c60: 2020 2020 7c20 4942 4541 2c20 4879 7045      | IBEA, HypE
+00001c70: 2c20 5352 412c 204d 614f 4541 2d49 4744  , SRA, MaOEA-IGD
+00001c80: 2c20 4152 2d4d 4f45 412c 202e 2e2e 2020  , AR-MOEA, ...  
+00001c90: 2020 2020 207c 0a0a 466f 7220 6120 636f       |..For a co
+00001ca0: 6d70 7265 6865 6e73 6976 6520 6c69 7374  mprehensive list
+00001cb0: 2061 6e64 2066 7572 7468 6572 2064 6574   and further det
+00001cc0: 6169 6c73 206f 6620 616c 6c20 616c 676f  ails of all algo
+00001cd0: 7269 7468 6d73 2c20 706c 6561 7365 2063  rithms, please c
+00001ce0: 6865 636b 2074 6865 205b 4150 4920 446f  heck the [API Do
+00001cf0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001d00: 7073 3a2f 2f65 766f 782e 7265 6164 7468  ps://evox.readth
+00001d10: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001d20: 7374 2f61 7069 2f61 6c67 6f72 6974 686d  st/api/algorithm
+00001d30: 732f 696e 6465 782e 6874 6d6c 292e 0a0a  s/index.html)...
+00001d40: 2323 2044 6976 6572 7365 2042 656e 6368  ## Diverse Bench
+00001d50: 6d61 726b 2050 726f 626c 656d 730a 0a7c  mark Problems..|
+00001d60: 2043 6174 6567 6f72 7920 2020 2020 207c   Category      |
+00001d70: 2050 726f 626c 656d 204e 616d 6573 2020   Problem Names  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 207c 0a7c 202d 2d2d           |.| ---
+00001da0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00001db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dd0: 2d2d 2d2d 207c 0a7c 204e 756d 6572 6963  ---- |.| Numeric
+00001de0: 616c 2020 2020 207c 2044 544c 5a2c 204c  al     | DTLZ, L
+00001df0: 534d 4f50 2c20 4d61 462c 205a 4454 2c20  SMOP, MaF, ZDT, 
+00001e00: 4345 4327 3232 2c20 202e 2e2e 2020 2020  CEC'22,  ...    
+00001e10: 7c0a 7c20 4e65 7572 6f65 766f 6c75 7469  |.| Neuroevoluti
+00001e20: 6f6e 7c20 4272 6178 2c20 4779 6d2c 2054  on| Brax, Gym, T
+00001e30: 6f72 6368 5669 7369 6f6e 2044 6174 6173  orchVision Datas
+00001e40: 6574 2c20 2e2e 2e20 2020 207c 0a0a 466f  et, ...    |..Fo
+00001e50: 7220 6120 636f 6d70 7265 6865 6e73 6976  r a comprehensiv
+00001e60: 6520 6c69 7374 2061 6e64 2066 7572 7468  e list and furth
+00001e70: 6572 2064 6574 6169 6c73 206f 6620 616c  er details of al
+00001e80: 6c20 6265 6e63 686d 6172 6b20 7072 6f62  l benchmark prob
+00001e90: 6c65 6d73 2c20 706c 6561 7365 2063 6865  lems, please che
+00001ea0: 636b 2074 6865 205b 4150 4920 446f 6375  ck the [API Docu
+00001eb0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00001ec0: 3a2f 2f65 766f 782e 7265 6164 7468 6564  ://evox.readthed
+00001ed0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001ee0: 2f61 7069 2f70 726f 626c 656d 732f 696e  /api/problems/in
+00001ef0: 6465 782e 6874 6d6c 292e 0a0a 0a23 2320  dex.html)....## 
+00001f00: 5365 7474 696e 6720 5570 2045 766f 580a  Setting Up EvoX.
+00001f10: 0a49 6e73 7461 6c6c 2060 6576 6f78 6020  .Install `evox` 
+00001f20: 6566 666f 7274 6c65 7373 6c79 2076 6961  effortlessly via
+00001f30: 2060 7069 7060 3a0a 6060 6062 6173 680a   `pip`:.```bash.
+00001f40: 7069 7020 696e 7374 616c 6c20 6576 6f78  pip install evox
+00001f50: 0a60 6060 0a0a 2a2a 4e6f 7465 2a2a 3a20  .```..**Note**: 
+00001f60: 546f 2069 6e73 7461 6c6c 2045 766f 5820  To install EvoX 
+00001f70: 7769 7468 204a 4158 2061 6e64 2068 6172  with JAX and har
+00001f80: 6477 6172 6520 6163 6365 6c65 7261 7469  dware accelerati
+00001f90: 6f6e 2063 6170 6162 696c 6974 6965 732c  on capabilities,
+00001fa0: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00001fb0: 206f 7572 2063 6f6d 7072 6568 656e 7369   our comprehensi
+00001fc0: 7665 205b 496e 7374 616c 6c61 7469 6f6e  ve [Installation
+00001fd0: 2047 7569 6465 5d28 6874 7470 733a 2f2f   Guide](https://
+00001fe0: 6576 6f78 2e72 6561 6474 6865 646f 6373  evox.readthedocs
+00001ff0: 2e69 6f2f 656e 2f6c 6174 6573 742f 6775  .io/en/latest/gu
+00002000: 6964 652f 696e 7374 616c 6c2e 6874 6d6c  ide/install.html
+00002010: 292e 0a0a 0a23 2320 5175 6963 6b20 5374  )....## Quick St
+00002020: 6172 740a 0a4b 6963 6b73 7461 7274 2079  art..Kickstart y
+00002030: 6f75 7220 6a6f 7572 6e65 7920 7769 7468  our journey with
+00002040: 2045 766f 5820 696e 206a 7573 7420 6120   EvoX in just a 
+00002050: 6665 7720 7369 6d70 6c65 2073 7465 7073  few simple steps
+00002060: 3a0a 312e 202a 2a49 6d70 6f72 7420 6e65  :.1. **Import ne
+00002070: 6365 7373 6172 7920 6d6f 6475 6c65 732a  cessary modules*
+00002080: 2a3a 0a60 6060 7079 7468 6f6e 0a69 6d70  *:.```python.imp
+00002090: 6f72 7420 6576 6f78 0a66 726f 6d20 6576  ort evox.from ev
+000020a0: 6f78 2069 6d70 6f72 7420 616c 676f 7269  ox import algori
+000020b0: 7468 6d73 2c20 7072 6f62 6c65 6d73 2c20  thms, problems, 
+000020c0: 776f 726b 666c 6f77 730a 6060 600a 322e  workflows.```.2.
+000020d0: 202a 2a43 6f6e 6669 6775 7265 2061 6e20   **Configure an 
+000020e0: 616c 676f 7269 7468 6d20 616e 6420 6465  algorithm and de
+000020f0: 6669 6e65 2061 2070 726f 626c 656d 2a2a  fine a problem**
+00002100: 3a0a 6060 6070 7974 686f 6e0a 7073 6f20  :.```python.pso 
+00002110: 3d20 616c 676f 7269 7468 6d73 2e50 534f  = algorithms.PSO
+00002120: 280a 2020 2020 6c62 3d6a 6e70 2e66 756c  (.    lb=jnp.ful
+00002130: 6c28 7368 6170 653d 2832 2c29 2c20 6669  l(shape=(2,), fi
+00002140: 6c6c 5f76 616c 7565 3d2d 3332 292c 0a20  ll_value=-32),. 
+00002150: 2020 2075 623d 6a6e 702e 6675 6c6c 2873     ub=jnp.full(s
+00002160: 6861 7065 3d28 322c 292c 2066 696c 6c5f  hape=(2,), fill_
+00002170: 7661 6c75 653d 3332 292c 0a20 2020 2070  value=32),.    p
+00002180: 6f70 5f73 697a 653d 3130 302c 0a29 0a61  op_size=100,.).a
+00002190: 636b 6c65 7920 3d20 7072 6f62 6c65 6d73  ckley = problems
+000021a0: 2e6e 756d 6572 6963 616c 2e41 636b 6c65  .numerical.Ackle
+000021b0: 7928 290a 6060 600a 332e 202a 2a43 6f6d  y().```.3. **Com
+000021c0: 706f 7365 2061 6e64 2069 6e69 7469 616c  pose and initial
+000021d0: 697a 6520 7468 6520 776f 726b 666c 6f77  ize the workflow
+000021e0: 2a2a 3a0a 6060 6070 7974 686f 6e0a 776f  **:.```python.wo
+000021f0: 726b 666c 6f77 203d 2077 6f72 6b66 6c6f  rkflow = workflo
+00002200: 7773 2e53 7464 576f 726b 666c 6f77 2870  ws.StdWorkflow(p
+00002210: 736f 2c20 6163 6b6c 6579 290a 6b65 7920  so, ackley).key 
+00002220: 3d20 6a61 782e 7261 6e64 6f6d 2e50 524e  = jax.random.PRN
+00002230: 474b 6579 2834 3229 0a73 7461 7465 203d  GKey(42).state =
+00002240: 2077 6f72 6b66 6c6f 772e 696e 6974 286b   workflow.init(k
+00002250: 6579 290a 6060 600a 342e 202a 2a52 756e  ey).```.4. **Run
+00002260: 2074 6865 2077 6f72 6b66 6c6f 772a 2a3a   the workflow**:
+00002270: 0a60 6060 7079 7468 6f6e 0a23 2045 7865  .```python.# Exe
+00002280: 6375 7465 2074 6865 2077 6f72 6b66 6c6f  cute the workflo
+00002290: 7720 666f 7220 3130 3020 6974 6572 6174  w for 100 iterat
+000022a0: 696f 6e73 0a66 6f72 2069 2069 6e20 7261  ions.for i in ra
+000022b0: 6e67 6528 3130 3029 3a0a 2020 2020 7374  nge(100):.    st
+000022c0: 6174 6520 3d20 776f 726b 666c 6f77 2e73  ate = workflow.s
+000022d0: 7465 7028 7374 6174 6529 0a60 6060 0a0a  tep(state).```..
+000022e0: 2323 2055 7365 2d63 6173 6573 2061 6e64  ## Use-cases and
+000022f0: 2041 7070 6c69 6361 7469 6f6e 730a 0a54   Applications..T
+00002300: 7279 206f 7574 2072 6561 6479 2d74 6f2d  ry out ready-to-
+00002310: 706c 6179 2065 7861 6d70 6c65 7320 696e  play examples in
+00002320: 2079 6f75 7220 6272 6f77 7365 7220 7769   your browser wi
+00002330: 7468 2043 6f6c 6162 3a0a 0a7c 2045 7861  th Colab:..| Exa
+00002340: 6d70 6c65 207c 204c 696e 6b20 7c0a 7c20  mple | Link |.| 
+00002350: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 207c  ------- | ---- |
+00002360: 0a7c 2042 6173 6963 2055 7361 6765 207c  .| Basic Usage |
+00002370: 205b 215b 4f70 656e 2069 6e20 436f 6c61   [![Open in Cola
+00002380: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
+00002390: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000023a0: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+000023b0: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
+000023c0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+000023d0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+000023e0: 6769 7468 7562 2f45 4d49 2d47 726f 7570  github/EMI-Group
+000023f0: 2f65 766f 782f 626c 6f62 2f6d 6169 6e2f  /evox/blob/main/
+00002400: 646f 6373 2f73 6f75 7263 652f 6775 6964  docs/source/guid
+00002410: 652f 6261 7369 6373 2f31 2d73 7461 7274  e/basics/1-start
+00002420: 2e69 7079 6e62 2920 7c0a 7c20 4e75 6d65  .ipynb) |.| Nume
+00002430: 7269 6361 6c20 4f70 7469 6d69 7a61 7469  rical Optimizati
+00002440: 6f6e 207c 205b 215b 4f70 656e 2069 6e20  on | [![Open in 
+00002450: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00002460: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00002470: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00002480: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
+00002490: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+000024a0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+000024b0: 636f 6d2f 6769 7468 7562 2f45 4d49 2d47  com/github/EMI-G
+000024c0: 726f 7570 2f65 766f 782f 626c 6f62 2f6d  roup/evox/blob/m
+000024d0: 6169 6e2f 646f 6373 2f73 6f75 7263 652f  ain/docs/source/
+000024e0: 6578 616d 706c 652f 7073 6f5f 6163 6b6c  example/pso_ackl
+000024f0: 6579 2e69 7079 6e62 2920 7c0a 7c20 4e65  ey.ipynb) |.| Ne
+00002500: 7572 6f65 766f 6c75 7469 6f6e 2077 6974  uroevolution wit
+00002510: 6820 4779 6d20 7c20 5b21 5b4f 7065 6e20  h Gym | [![Open 
+00002520: 696e 2043 6f6c 6162 5d28 6874 7470 733a  in Colab](https:
+00002530: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00002540: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
+00002550: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
+00002560: 7667 295d 2868 7474 7073 3a2f 2f63 6f6c  vg)](https://col
+00002570: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00002580: 6c65 2e63 6f6d 2f67 6974 6875 622f 454d  le.com/github/EM
+00002590: 492d 4772 6f75 702f 6576 6f78 2f62 6c6f  I-Group/evox/blo
+000025a0: 622f 6d61 696e 2f64 6f63 732f 736f 7572  b/main/docs/sour
+000025b0: 6365 2f65 7861 6d70 6c65 2f67 796d 5f63  ce/example/gym_c
+000025c0: 6c61 7373 6963 5f63 6f6e 7472 6f6c 2e69  lassic_control.i
+000025d0: 7079 6e62 2920 7c0a 7c20 4e65 7572 6f65  pynb) |.| Neuroe
+000025e0: 766f 6c75 7469 6f6e 2077 6974 6820 4272  volution with Br
+000025f0: 6178 207c 205b 215b 4f70 656e 2069 6e20  ax | [![Open in 
+00002600: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00002610: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00002620: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00002630: 636f 6c61 622d 6261 6467 652e 7376 6729  colab-badge.svg)
+00002640: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00002650: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00002660: 636f 6d2f 6769 7468 7562 2f45 4d49 2d47  com/github/EMI-G
+00002670: 726f 7570 2f65 766f 782f 626c 6f62 2f6d  roup/evox/blob/m
+00002680: 6169 6e2f 646f 6373 2f73 6f75 7263 652f  ain/docs/source/
+00002690: 6775 6964 652f 6261 7369 6373 2f32 2d70  guide/basics/2-p
+000026a0: 726f 626c 656d 732e 6970 796e 6229 207c  roblems.ipynb) |
+000026b0: 0a7c 2043 7573 746f 6d20 416c 676f 7269  .| Custom Algori
+000026c0: 7468 6d2f 5072 6f62 6c65 6d20 7c20 5b21  thm/Problem | [!
+000026d0: 5b4f 7065 6e20 696e 2043 6f6c 6162 5d28  [Open in Colab](
+000026e0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+000026f0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00002700: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
+00002710: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00002720: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+00002730: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
+00002740: 6875 622f 454d 492d 4772 6f75 702f 6576  hub/EMI-Group/ev
+00002750: 6f78 2f62 6c6f 622f 6d61 696e 2f64 6f63  ox/blob/main/doc
+00002760: 732f 736f 7572 6365 2f65 7861 6d70 6c65  s/source/example
+00002770: 2f63 7573 746f 6d5f 616c 676f 7269 7468  /custom_algorith
+00002780: 6d5f 616e 645f 7072 6f62 6c65 6d2e 6970  m_and_problem.ip
+00002790: 796e 6229 207c 0a0a 466f 7220 6d6f 7265  ynb) |..For more
+000027a0: 2075 7365 2d63 6173 6573 2061 6e64 2061   use-cases and a
+000027b0: 7070 6c69 6361 7469 6f6e 732c 2070 6c65  pplications, ple
+000027c0: 6165 2063 6865 636b 206f 7574 205b 4578  ae check out [Ex
+000027d0: 616d 706c 6520 4469 7265 6374 6f72 795d  ample Directory]
+000027e0: 2868 7474 7073 3a2f 2f65 766f 782e 7265  (https://evox.re
+000027f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00002800: 6c61 7465 7374 2f65 7861 6d70 6c65 2f69  latest/example/i
+00002810: 6e64 6578 2e68 746d 6c29 2e0a 0a23 2320  ndex.html)...## 
+00002820: 436f 6d6d 756e 6974 7920 2620 5375 7070  Community & Supp
+00002830: 6f72 740a 0a2d 2045 6e67 6167 6520 696e  ort..- Engage in
+00002840: 2064 6973 6375 7373 696f 6e73 2061 6e64   discussions and
+00002850: 2073 6861 7265 2079 6f75 7220 6578 7065   share your expe
+00002860: 7269 656e 6365 7320 6f6e 205b 4769 7448  riences on [GitH
+00002870: 7562 2044 6973 6375 7373 696f 6e20 426f  ub Discussion Bo
+00002880: 6172 645d 2868 7474 7073 3a2f 2f67 6974  ard](https://git
+00002890: 6875 622e 636f 6d2f 454d 492d 4772 6f75  hub.com/EMI-Grou
+000028a0: 702f 6576 6f78 2f64 6973 6375 7373 696f  p/evox/discussio
+000028b0: 6e73 292e 0a2d 204a 6f69 6e20 6f75 7220  ns)..- Join our 
+000028c0: 5151 2067 726f 7570 2028 4944 3a20 3239  QQ group (ID: 29
+000028d0: 3739 3639 3731 3729 2e0a 2d20 4865 6c70  7969717)..- Help
+000028e0: 2077 6974 6820 7468 6520 7472 616e 736c   with the transl
+000028f0: 6174 696f 6e20 6f66 2074 6865 2064 6f63  ation of the doc
+00002900: 756d 656e 7461 7469 6f6e 206f 6e20 5b57  umentation on [W
+00002910: 6562 6c61 7465 5d28 6874 7470 733a 2f2f  eblate](https://
+00002920: 686f 7374 6564 2e77 6562 6c61 7465 2e6f  hosted.weblate.o
+00002930: 7267 2f70 726f 6a65 6374 732f 6576 6f78  rg/projects/evox
+00002940: 2f65 766f 782f 292e 0a57 6520 6375 7272  /evox/)..We curr
+00002950: 656e 746c 7920 7375 7070 6f72 7420 7472  ently support tr
+00002960: 616e 736c 6174 696f 6e73 2069 6e20 7477  anslations in tw
+00002970: 6f20 6c61 6e67 7561 6765 732c 205b 456e  o languages, [En
+00002980: 676c 6973 685d 2868 7474 7073 3a2f 2f65  glish](https://e
+00002990: 766f 782e 7265 6164 7468 6564 6f63 732e  vox.readthedocs.
+000029a0: 696f 2f65 6e2f 6c61 7465 7374 2f29 202f  io/en/latest/) /
+000029b0: 205b e4b8 ade6 9687 5d28 6874 7470 733a   [......](https:
+000029c0: 2f2f 6576 6f78 2e72 6561 6474 6865 646f  //evox.readthedo
+000029d0: 6373 2e69 6f2f 7a68 2f6c 6174 6573 742f  cs.io/zh/latest/
+000029e0: 292e 0a2d 204f 6666 6963 6961 6c20 5765  )..- Official We
+000029f0: 6273 6974 653a 2068 7474 7073 3a2f 2f65  bsite: https://e
+00002a00: 766f 782e 6772 6f75 702f 0a0a 2323 2053  vox.group/..## S
+00002a10: 6973 7465 7220 5072 6f6a 6563 7473 0a0a  ister Projects..
+00002a20: 2d20 4576 6f58 4265 6e63 683a 2041 2062  - EvoXBench: A b
+00002a30: 656e 6368 6d61 726b 2070 6c61 7466 6f72  enchmark platfor
+00002a40: 6d20 666f 7220 4e65 7572 616c 2041 7263  m for Neural Arc
+00002a50: 6869 7465 6375 7472 6520 5365 6172 6368  hitecutre Search
+00002a60: 2028 4e41 5329 2077 6974 686f 7574 2074   (NAS) without t
+00002a70: 6865 2072 6571 7569 7265 6d65 6e74 206f  he requirement o
+00002a80: 6620 4750 5573 2f50 7954 6f72 6368 2f54  f GPUs/PyTorch/T
+00002a90: 656e 736f 7266 6c6f 772c 2073 7570 706f  ensorflow, suppo
+00002aa0: 7274 696e 6720 7661 7269 6f75 7320 7072  rting various pr
+00002ab0: 6f67 7261 6d6d 696e 6720 6c61 6e67 7561  ogramming langua
+00002ac0: 6765 7320 7375 6368 2061 7320 4a61 7661  ges such as Java
+00002ad0: 2c20 4d61 746c 6162 2c20 5079 7468 6f6e  , Matlab, Python
+00002ae0: 2c20 6563 742e 2043 6865 636b 206f 7574  , ect. Check out
+00002af0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+00002b00: 6769 7468 7562 2e63 6f6d 2f45 4d49 2d47  github.com/EMI-G
+00002b10: 726f 7570 2f65 766f 7862 656e 6368 292e  roup/evoxbench).
+00002b20: 0a0a 2323 2043 6974 696e 6720 4576 6f58  ..## Citing EvoX
+00002b30: 0a0a 4966 2079 6f75 2075 7365 2045 766f  ..If you use Evo
+00002b40: 5820 696e 2079 6f75 7220 7265 7365 6172  X in your resear
+00002b50: 6368 2061 6e64 2077 616e 7420 746f 2063  ch and want to c
+00002b60: 6974 6520 6974 2069 6e20 796f 7572 2077  ite it in your w
+00002b70: 6f72 6b2c 2070 6c65 6173 6520 7573 653a  ork, please use:
+00002b80: 0a60 6060 0a40 6172 7469 636c 657b 6576  .```.@article{ev
+00002b90: 6f78 2c0a 2020 7469 746c 6520 3d20 7b7b  ox,.  title = {{
+00002ba0: 4576 6f58 7d3a 207b 417d 207b 4469 7374  EvoX}: {A} {Dist
+00002bb0: 7269 6275 7465 647d 207b 4750 557d 2d61  ributed} {GPU}-a
+00002bc0: 6363 656c 6572 6174 6564 207b 4672 616d  ccelerated {Fram
+00002bd0: 6577 6f72 6b7d 2066 6f72 207b 5363 616c  ework} for {Scal
+00002be0: 6162 6c65 7d20 7b45 766f 6c75 7469 6f6e  able} {Evolution
+00002bf0: 6172 797d 207b 436f 6d70 7574 6174 696f  ary} {Computatio
+00002c00: 6e7d 7d2c 0a20 2061 7574 686f 7220 3d20  n}},.  author = 
+00002c10: 7b48 7561 6e67 2c20 4265 6963 6865 6e20  {Huang, Beichen 
+00002c20: 616e 6420 4368 656e 672c 2052 616e 2061  and Cheng, Ran a
+00002c30: 6e64 204c 692c 205a 6875 6f7a 6861 6f20  nd Li, Zhuozhao 
+00002c40: 616e 6420 4a69 6e2c 2059 616f 6368 7520  and Jin, Yaochu 
+00002c50: 616e 6420 5461 6e2c 204b 6179 2043 6865  and Tan, Kay Che
+00002c60: 6e7d 2c0a 2020 6a6f 7572 6e61 6c20 3d20  n},.  journal = 
+00002c70: 7b49 4545 4520 5472 616e 7361 6374 696f  {IEEE Transactio
+00002c80: 6e73 206f 6e20 4576 6f6c 7574 696f 6e61  ns on Evolutiona
+00002c90: 7279 2043 6f6d 7075 7461 7469 6f6e 7d2c  ry Computation},
+00002ca0: 0a20 2079 6561 7220 3d20 3230 3234 2c0a  .  year = 2024,.
+00002cb0: 2020 646f 6920 3d20 7b31 302e 3131 3039    doi = {10.1109
+00002cc0: 2f54 4556 432e 3230 3234 2e33 3338 3835  /TEVC.2024.33885
+00002cd0: 3530 7d0a 7d0a 6060 600a 0a23 2320 5374  50}.}.```..## St
+00002ce0: 6172 2048 6973 746f 7279 0a0a 5b21 5b53  ar History..[![S
+00002cf0: 7461 7220 4869 7374 6f72 7920 4368 6172  tar History Char
+00002d00: 745d 2868 7474 7073 3a2f 2f61 7069 2e73  t](https://api.s
+00002d10: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
+00002d20: 7376 673f 7265 706f 733d 454d 492d 4772  svg?repos=EMI-Gr
+00002d30: 6f75 702f 6576 6f78 2674 7970 653d 4461  oup/evox&type=Da
+00002d40: 7465 295d 2868 7474 7073 3a2f 2f73 7461  te)](https://sta
+00002d50: 722d 6869 7374 6f72 792e 636f 6d2f 2345  r-history.com/#E
+00002d60: 4d49 2d47 726f 7570 2f65 766f 7826 4461  MI-Group/evox&Da
+00002d70: 7465 290a 0a0a 0a                        te)....
```

### Comparing `evox-0.8.0/src/evox.egg-info/SOURCES.txt` & `evox-0.8.1/src/evox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 src/evox/problems/evoxbench/evoxbench.py
 src/evox/problems/neuroevolution/__init__.py
 src/evox/problems/neuroevolution/reinforcement_learning/__init__.py
 src/evox/problems/neuroevolution/reinforcement_learning/brax.py
 src/evox/problems/neuroevolution/reinforcement_learning/env_pool.py
 src/evox/problems/neuroevolution/reinforcement_learning/gym.py
 src/evox/problems/neuroevolution/supervised_learning/__init__.py
-src/evox/problems/neuroevolution/supervised_learning/torchvision_dataset.py
+src/evox/problems/neuroevolution/supervised_learning/tfds.py
 src/evox/problems/numerical/__init__.py
 src/evox/problems/numerical/ackley.py
 src/evox/problems/numerical/cec2022_so.py
 src/evox/problems/numerical/dtlz.py
 src/evox/problems/numerical/griewank.py
 src/evox/problems/numerical/lsmop.py
 src/evox/problems/numerical/maf.py
@@ -189,14 +189,15 @@
 src/evox/problems/numerical/cec2022_input_data/shuffle_data_6_D20.txt
 src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D10.txt
 src/evox/problems/numerical/cec2022_input_data/shuffle_data_7_D20.txt
 src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D10.txt
 src/evox/problems/numerical/cec2022_input_data/shuffle_data_8_D20.txt
 src/evox/utils/__init__.py
 src/evox/utils/common.py
+src/evox/utils/io.py
 src/evox/vis_tools/plot.py
 src/evox/workflows/__init__.py
 src/evox/workflows/distributed.py
 src/evox/workflows/non_jit_workflow.py
 src/evox/workflows/std_workflow.py
 tests/test_classic_problems.py
 tests/test_containers.py
```

### Comparing `evox-0.8.0/tests/test_classic_problems.py` & `evox-0.8.1/tests/test_classic_problems.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_containers.py` & `evox-0.8.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_crowding_distance.py` & `evox-0.8.1/tests/test_crowding_distance.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_envpool.py` & `evox-0.8.1/tests/test_envpool.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_evoxbench.py` & `evox-0.8.1/tests/test_evoxbench.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_gaussian_process.py` & `evox-0.8.1/tests/test_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_gym.py` & `evox-0.8.1/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_lsmop.py` & `evox-0.8.1/tests/test_lsmop.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_maf.py` & `evox-0.8.1/tests/test_maf.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_metrics.py` & `evox-0.8.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_multi_objective_algorithms.py` & `evox-0.8.1/tests/test_multi_objective_algorithms.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_non_dominated_sort.py` & `evox-0.8.1/tests/test_non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_single_objective_algorithms.py` & `evox-0.8.1/tests/test_single_objective_algorithms.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_state.py` & `evox-0.8.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_utils.py` & `evox-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evox-0.8.0/tests/test_workflows.py` & `evox-0.8.1/tests/test_workflows.py`

 * *Files identical despite different names*

