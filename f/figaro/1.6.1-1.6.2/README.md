# Comparing `tmp/figaro-1.6.1.tar.gz` & `tmp/figaro-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.1.tar", last modified: Mon Apr 15 09:15:34 2024, max compression
+gzip compressed data, was "figaro-1.6.2.tar", last modified: Tue Apr 23 15:21:21 2024, max compression
```

## Comparing `figaro-1.6.1.tar` & `figaro-1.6.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464909 figaro-1.6.1/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.1/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.1/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-15 09:15:34.464695 figaro-1.6.1/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.1/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.451147 figaro-1.6.1/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.456055 figaro-1.6.1/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.458485 figaro-1.6.1/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.1/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.1/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.462635 figaro-1.6.1/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.1/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-09 08:31:38.000000 figaro-1.6.1/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.1/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464209 figaro-1.6.1/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    13588 2024-04-15 07:19:49.000000 figaro-1.6.1/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    18793 2024-04-15 07:19:52.000000 figaro-1.6.1/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10486 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9321 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2341 2024-04-10 10:07:12.000000 figaro-1.6.1/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.1/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    33823 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6282 2024-02-24 19:48:07.000000 figaro-1.6.1/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    54015 2024-04-15 09:14:03.000000 figaro-1.6.1/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.1/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40056 2024-04-10 10:07:14.000000 figaro-1.6.1/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.1/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.1/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16147 2024-04-14 14:47:57.000000 figaro-1.6.1/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-15 09:15:34.464424 figaro-1.6.1/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1746 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-15 09:15:34.000000 figaro-1.6.1/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-15 09:15:16.000000 figaro-1.6.1/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-15 09:15:34.464954 figaro-1.6.1/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.994186 figaro-1.6.2/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.2/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.2/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-23 15:21:21.992163 figaro-1.6.2/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.2/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.967786 figaro-1.6.2/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.974557 figaro-1.6.2/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.2/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.2/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.977400 figaro-1.6.2/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.2/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.2/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.986164 figaro-1.6.2/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.2/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.2/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.2/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.989450 figaro-1.6.2/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.2/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    19845 2024-04-18 08:10:10.000000 figaro-1.6.2/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    23315 2024-04-18 07:54:46.000000 figaro-1.6.2/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10386 2024-04-18 07:25:21.000000 figaro-1.6.2/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9221 2024-04-18 07:25:04.000000 figaro-1.6.2/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2818 2024-04-18 07:51:37.000000 figaro-1.6.2/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.2/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.2/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-04-17 14:55:45.000000 figaro-1.6.2/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.2/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.2/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    34199 2024-04-22 14:26:21.000000 figaro-1.6.2/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.2/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    55429 2024-04-22 14:27:23.000000 figaro-1.6.2/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.2/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40427 2024-04-22 10:30:10.000000 figaro-1.6.2/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.2/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    12098 2024-04-23 13:33:43.000000 figaro-1.6.2/figaro/rate.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.2/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-04-17 08:40:42.000000 figaro-1.6.2/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:21:21.991529 figaro-1.6.2/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1761 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-23 15:21:21.000000 figaro-1.6.2/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-16 11:57:09.000000 figaro-1.6.2/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-23 15:21:21.996211 figaro-1.6.2/setup.cfg
```

### Comparing `figaro-1.6.1/LICENSE` & `figaro-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/PKG-INFO` & `figaro-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.1
+Version: 1.6.2
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.1/README.md` & `figaro-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/docs/source/index.rst` & `figaro-1.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/_likelihood.py` & `figaro-1.6.2/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/_numba_functions.py` & `figaro-1.6.2/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.2/figaro/_pipelines/par_probability_density.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 import numpy as np
 
 import optparse
+import dill
 import importlib
-import warnings
 
 from pathlib import Path
 from tqdm import tqdm
 
-from figaro.mixture import DPGMM, HDPGMM
-from figaro.transform import transform_to_probit
+from figaro.mixture import DPGMM
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_data, load_single_event, load_selection_function, save_density, load_density, supported_pars
+from figaro.load import load_single_event, save_density, load_density, supported_extensions, supported_pars
+
+import ray
+from ray.util import ActorPool
+
+@ray.remote
+class worker:
+    def __init__(self, bounds,
+                       sigma = None,
+                       samples = None,
+                       probit = True,
+                       scale = None,
+                       ):
+        self.dim     = bounds.shape[-1]
+        self.mixture = DPGMM(bounds, prior_pars = get_priors(bounds, samples = samples, std = sigma, scale = scale, probit = probit, hierarchical = False), probit = probit)
+        self.samples = np.copy(samples)
+        self.samples.setflags(write = True)
+
+    def draw_sample(self):
+        return self.mixture.density_from_samples(self.samples, make_comp = False)
 
 def main():
 
-    parser = optparse.OptionParser(prog = 'figaro-hierarchical', description = 'Hierarchical probability density reconstruction')
+    parser = optparse.OptionParser(prog = 'figaro-par-density', description = 'Parallelised probability density reconstruction')
     # Input/output
-    parser.add_option("-i", "--input", type = "string", dest = "input", help = "Folder with single-event samples files", default = None)
+    parser.add_option("-i", "--input", type = "string", dest = "input", help = "File with samples", default = None)
     parser.add_option("-b", "--bounds", type = "string", dest = "bounds", help = "Density bounds. Must be a string formatted as '[[xmin, xmax], [ymin, ymax],...]'. For 1D distributions use '[xmin, xmax]'. Quotation marks are required and scientific notation is accepted", default = None)
-    parser.add_option("-o", "--output", type = "string", dest = "output", help = "Output folder. Default: same directory as samples folder", default = None)
+    parser.add_option("-o", "--output", type = "string", dest = "output", help = "Output folder. Default: same directory as samples", default = None)
     parser.add_option("--ext", dest = "ext", type = "choice", choices = ['pkl', 'json'], help = "Format of mixture output file", default = 'json')
     parser.add_option("--inj_density", type = "string", dest = "inj_density_file", help = "Python module with injected density - please name the method 'density'", default = None)
     parser.add_option("--selfunc", type = "string", dest = "selfunc_file", help = "Python module with selection function - please name the method 'selection_function'", default = None)
     parser.add_option("--parameter", type = "string", dest = "par", help = "GW parameter(s) to be read from file", default = None)
     parser.add_option("--waveform", type = "choice", dest = "wf", help = "Waveform to load from samples file. To be used in combination with --parameter.", choices = ['combined', 'seob', 'imr'], default = 'combined')
     # Plot
-    parser.add_option("--name", type = "string", dest = "hier_name", help = "Name to be given to hierarchical inference files. Default: same name as samples folder parent directory", default = None)
     parser.add_option("-p", "--postprocess", dest = "postprocess", action = 'store_true', help = "Postprocessing", default = False)
-    parser.add_option("-s", "--save_se", dest = "save_single_event", action = 'store_true', help = "Save single event plots", default = False)
     parser.add_option("--symbol", type = "string", dest = "symbol", help = "LaTeX-style quantity symbol, for plotting purposes", default = None)
     parser.add_option("--unit", type = "string", dest = "unit", help = "LaTeX-style quantity unit, for plotting purposes", default = None)
-    parser.add_option("--hier_samples", type = "string", dest = "hier_samples", help = "Samples from hierarchical distribution (true single-event values, for simulations only)", default = None)
     # Settings
-    parser.add_option("--draws", type = "int", dest = "draws", help = "Number of draws for hierarchical distribution", default = 100)
-    parser.add_option("--se_draws", type = "int", dest = "se_draws", help = "Number of draws for single-event distribution. Default: same as hierarchical distribution", default = None)
+    parser.add_option("--draws", type = "int", dest = "draws", help = "Number of draws", default = 100)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
-    parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
-    parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
-    parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
-    parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
+    parser.add_option("--cosmology", type = "choice", dest = "cosmology", help = "Set of cosmological parameters. Default values from Planck (2021)", choices = ['Planck18', 'Planck15'], default = 'Planck18')
+    parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
-    parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
-    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
+    parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
+    parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
+    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
     
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
@@ -62,145 +75,106 @@
         options.output = Path(options.output).resolve()
         if not options.output.exists():
             options.output.mkdir(parents=True)
     else:
         options.output = options.input.parent
     if options.config is not None:
         options.config = Path(options.config).resolve()
-    output_plots = Path(options.output, 'plots')
-    if not output_plots.exists():
-        output_plots.mkdir()
-    output_draws = Path(options.output, 'draws')
-    if not output_draws.exists():
-        output_draws.mkdir()
-    # Read hierarchical name
-    if options.hier_name is None:
-        options.hier_name = options.output.parts[-1]
-    if options.selfunc_file is None:
-        hier_name = 'observed_'+options.hier_name
-    else:
-        hier_name = 'intrinsic_'+options.hier_name
-
-    if options.config is None:
-        save_options(options, options.output, name = options.hier_name)
     
+    if options.config is None:
+        save_options(options, options.output)
+
     # Read bounds
     if options.bounds is not None:
         options.bounds = np.array(np.atleast_2d(eval(options.bounds)), dtype = np.float64)
     elif options.bounds is None and not options.postprocess:
         raise Exception("Please provide bounds for the inference (use -b '[[xmin,xmax],[ymin,ymax],...]')")
-    # Read cosmology
-    options.h, options.om, options.ol = (float(x) for x in options.cosmology.split(','))
+
     # Read parameter(s)
     if options.par is not None:
         options.par = options.par.split(',')
         if not np.all([par in supported_pars for par in options.par]):
             raise Exception("Please provide parameters from this list: "+', '.join(supported_pars[:-2]))
-    # Read number of single-event draws
-    if options.se_draws is None:
-        options.se_draws = options.draws
-    if options.se_sigma_prior is not None:
-        options.se_sigma_prior = np.array([float(s) for s in options.se_sigma_prior.split(',')])
-    if options.sigma_prior is not None:
-        options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
-
     # If provided, load injected density
     inj_density = None
     if options.inj_density_file is not None:
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
-    # If provided, load selecton function
-    selfunc     = None
-    inj_pdf     = None
-    n_total_inj = None
+    #If provided, load selecton function
+    selfunc = None
     if options.selfunc_file is not None:
-        selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
-        if not callable(selfunc) and not options.probit:
-            # Keeping only the samples within bounds
-            selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
-            inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
-    # If provided, load true values
-    hier_samples = None
-    if options.hier_samples is not None:
-        options.hier_samples = Path(options.hier_samples).resolve()
-        hier_samples, true_name = load_single_event(options.hier_samples, par = options.par, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
-        if np.shape(hier_samples)[-1] == 1:
-            hier_samples = hier_samples.flatten()
-            
-    # Load samples
-    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
-    try:
-        dim = np.shape(events[0][0])[-1]
-    except IndexError:
-        dim = 1
+        selfunc, _, _, _ = load_selection_function(options.selfunc_file, par = options.par)
+        if not callable(selfunc):
+            raise Exception("Only .py files with callable approximants are allowed for DPGMM reconstruction")
+        
+    if options.sigma_prior is not None:
+        options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
+    if options.input.is_file():
+        files = [options.input]
+        output_draws = options.output
+        subfolder = False
+    else:
+        files = sum([list(options.input.glob('*.'+ext)) for ext in supported_extensions], [])
+        output_draws = Path(options.output, 'draws')
+        if not output_draws.exists():
+            output_draws.mkdir()
+        subfolder = True
     if options.exclude_points:
         print("Ignoring points outside bounds.")
-        for i, ev in enumerate(events):
-            events[i] = ev[np.where((np.prod(options.bounds[:,0] < ev, axis = 1) & np.prod(ev < options.bounds[:,1], axis = 1)))]
-    else:
-        # Check if all samples are within bounds
-        all_samples = np.atleast_2d(np.concatenate(events))
-        if options.probit:
-            if not np.all([(all_samples[:,i] > options.bounds[i,0]).all() and (all_samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
-                raise ValueError("One or more samples are outside the given bounds.")
-
-    # Plot labels
-    if dim > 1:
-        if options.symbol is not None:
-            symbols = options.symbol.split(',')
-        else:
-            symbols = options.symbol
-        if options.unit is not None:
-            units = options.unit.split(',')
-        else:
-            units = options.unit
     
-    # Reconstruction
     if not options.postprocess:
-        if options.run_events:
-            mix = DPGMM(options.bounds, probit = options.probit)
-            posteriors = []
-            # Run each single-event analysis
-            for i in tqdm(range(len(events)), desc = 'Events'):
-                ev   = events[i]
-                name = names[i]
-                prior_pars = get_priors(mix.bounds, samples = ev, probit = options.probit, std = options.se_sigma_prior, scale = options.fraction, hierarchical = False)
-                mix.initialise(prior_pars = prior_pars)
-                # Draw samples
-                draws = [mix.density_from_samples(ev, make_comp = False) for _ in range(options.se_draws)]
-                posteriors.append(draws)
-                # Make plots
-                if options.save_single_event:
-                    plt_bounds = np.atleast_2d([ev.min(axis = 0), ev.max(axis = 0)]).T
-                    if dim == 1:
-                        plot_median_cr(draws, samples = ev, bounds = plt_bounds[0], out_folder = output_plots, name = name, label = options.symbol, unit = options.unit, subfolder = True)
-                    else:
-                        plot_multidim(draws, samples = ev, bounds = plt_bounds, out_folder = output_plots, name = name, labels = symbols, units = units, subfolder = True)
-                # Save single-event draws
-                save_density(draws, folder = output_draws, name = 'draws_'+name, ext = options.ext)
-            # Save all single-event draws together
-            posteriors = np.array(posteriors)
-            save_density(posteriors, folder = output_draws, name = 'posteriors_single_event', ext = options.ext)
+        ray.init(num_cpus = options.n_parallel)
+    
+    for i, file in enumerate(files):
+        # Load samples
+        samples, name = load_single_event(file, par = options.par, n_samples = options.n_samples_dsp, cosmology = options.cosmology, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+        try:
+            dim = np.shape(samples)[-1]
+        except IndexError:
+            dim = 1
+        if options.exclude_points:
+            samples = samples[np.where((np.prod(options.bounds[:,0] < samples, axis = 1) & np.prod(samples < options.bounds[:,1], axis = 1)))]
         else:
-            # Load pre-computed posteriors
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", category=UserWarning)
-                posteriors = load_density(Path(output_draws, 'posteriors_single_event.'+options.ext), make_comp = False)
-        # Run hierarchical analysis
-        prior_pars = get_priors(options.bounds, samples = events, std = options.sigma_prior, scale = options.fraction, probit = options.probit, hierarchical = True)
-        mix        = HDPGMM(options.bounds, prior_pars = prior_pars, MC_draws = options.mc_draws, probit = options.probit, selection_function = selfunc, injection_pdf = inj_pdf, total_injections = n_total_inj)
-        draws      = np.array([mix.density_from_samples(posteriors, make_comp = False) for _ in tqdm(range(options.draws), desc = 'Hierarchical')])
-        # Save draws
-        save_density(draws, folder = output_draws, name = 'draws_'+hier_name, ext = options.ext)
-    else:
-        draws = load_density(Path(output_draws, 'draws_'+hier_name+'.'+options.ext))
-    # Plot
-    if dim == 1:
-        plot_median_cr(draws, injected = inj_density, samples = hier_samples, out_folder = output_plots, name = options.hier_name, label = options.symbol, unit = options.unit, hierarchical = True)
-    else:
-        plot_multidim(draws, samples = hier_samples, out_folder = output_plots, name = hier_name, labels = symbols, units = units, hierarchical = True)
+            # Check if all samples are within bounds
+            if options.probit:
+                if not np.all([(samples[:,i] > options.bounds[i,0]).all() and (samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
+                    raise ValueError("One or more samples are outside the given bounds.")
+
+        # Reconstruction
+        if not options.postprocess:
+            # Actual analysis
+            desc = name + ' ({0}/{1})'.format(i+1, len(files))
+            pool = ActorPool([worker.remote(bounds  = options.bounds,
+                                            sigma   = options.sigma_prior,
+                                            scale   = options.fraction,
+                                            samples = samples,
+                                            probit  = options.probit,
+                                            )
+                              for _ in range(options.n_parallel)])
+            draws = []
+            for s in tqdm(pool.map_unordered(lambda a, v: a.draw_sample.remote(), [_ for _ in range(options.draws)]), total = options.draws, desc = desc):
+                draws.append(s)
+            draws = np.array(draws)
+            # Save reconstruction
+            save_density(draws, folder = output_draws, name = 'draws_'+name, ext = options.ext)
+        else:
+            draws = load_density(Path(output_draws, 'draws_'+name+'.'+options.ext))
+
+        # Plot
+        if dim == 1:
+            plot_median_cr(draws, injected = inj_density, selfunc = selfunc, samples = samples, out_folder = options.output, name = name, label = options.symbol, unit = options.unit, subfolder = subfolder)
+        else:
+            if options.symbol is not None:
+                symbols = options.symbol.split(',')
+            else:
+                symbols = options.symbol
+            if options.unit is not None:
+                units = options.unit.split(',')
+            else:
+                units = options.unit
+            plot_multidim(draws, samples = samples, out_folder = options.output, name = name, labels = symbols, units = units, subfolder = subfolder)
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `figaro-1.6.1/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.2/figaro/_pipelines/hierarchical_inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,113 +8,21 @@
 from tqdm import tqdm
 
 from figaro.mixture import DPGMM, HDPGMM
 from figaro.transform import transform_to_probit
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
 from figaro.load import load_data, load_single_event, load_selection_function, save_density, load_density, supported_pars
+from figaro.rate import sample_rate, normalise_alpha_factor, plot_integrated_rate, plot_differential_rate
+from figaro.cosmology import _decorator_dVdz, dVdz_approx_planck18, dVdz_approx_planck15
+from figaro.marginal import marginalise
 
-import ray
-from ray.util import ActorPool
-
-@ray.remote
-class worker:
-    def __init__(self, bounds,
-                       out_folder_plots,
-                       out_folder_draws,
-                       ext         = 'json',
-                       se_sigma    = None,
-                       hier_sigma  = None,
-                       scale       = None,
-                       events      = None,
-                       label       = None,
-                       unit        = None,
-                       save_se     = True,
-                       MC_draws    = None,
-                       probit      = True,
-                       selfunc     = None,
-                       inj_pdf     = None,
-                       n_total_inj = None,
-                       ):
-        self.dim                  = bounds.shape[0]
-        self.bounds               = bounds
-        self.mixture              = DPGMM(self.bounds, probit = probit)
-        self.hierarchical_mixture = HDPGMM(self.bounds,
-                                           MC_draws           = MC_draws,
-                                           probit             = probit,
-                                           selection_function = selfunc,
-                                           injection_pdf      = inj_pdf,
-                                           total_injections   = n_total_inj,
-                                           prior_pars         = get_priors(self.bounds,
-                                                                           samples      = events,
-                                                                           std          = hier_sigma,
-                                                                           scale        = scale,
-                                                                           probit       = probit,
-                                                                           hierarchical = True,
-                                                                           ),
-                                           )
-        self.out_folder_plots = out_folder_plots
-        self.out_folder_draws = out_folder_draws
-        self.se_sigma         = se_sigma
-        self.scale            = scale
-        self.save_se          = save_se
-        self.label            = label
-        self.unit             = unit
-        self.probit           = probit
-        self.ext              = ext
-
-    def run_event(self, pars):
-        # Unpack data
-        samples, name, n_draws = pars
-        # Copying (issues with shuffling)
-        ev = np.copy(samples)
-        ev.setflags(write = True)
-        # Actual inference
-        prior_pars = get_priors(self.bounds, samples = ev, probit = self.probit, std = self.se_sigma, scale = self.scale, hierarchical = False)
-        self.mixture.initialise(prior_pars = prior_pars)
-        draws      = [self.mixture.density_from_samples(ev, make_comp = False) for _ in range(n_draws)]
-        # Plots
-        plt_bounds = np.atleast_2d([ev.min(axis = 0), ev.max(axis = 0)]).T
-        if self.save_se:
-            if self.dim == 1:
-                plot_median_cr(draws,
-                               samples    = ev,
-                               bounds     = plt_bounds[0],
-                               out_folder = self.out_folder_plots,
-                               name       = name,
-                               label      = self.label,
-                               unit       = self.unit,
-                               subfolder  = True,
-                               )
-            else:
-                plot_multidim(draws,
-                              samples    = ev,
-                              bounds     = plt_bounds,
-                              out_folder = self.out_folder_plots,
-                              name       = name,
-                              labels     = self.label,
-                              units      = self.unit,
-                              subfolder  = True,
-                              )
-        # Saving
-        save_density(draws, folder = self.out_folder_draws, name = 'draws_'+name, ext = self.ext)
-        return draws
-
-    def draw_hierarchical(self):
-        return self.hierarchical_mixture.density_from_samples(self.posteriors, make_comp = False)
-    
-    def load_posteriors(self, posteriors):
-        self.posteriors = np.copy(posteriors)
-        self.posteriors.setflags(write = True)
-        for i in range(len(self.posteriors)):
-            self.posteriors[i].setflags(write = True)
-            
 def main():
 
-    parser = optparse.OptionParser(prog = 'figaro-par-hierarchical', description = 'Parallelised hierarchical probability density reconstruction')
+    parser = optparse.OptionParser(prog = 'figaro-hierarchical', description = 'Hierarchical probability density reconstruction')
     # Input/output
     parser.add_option("-i", "--input", type = "string", dest = "input", help = "Folder with single-event samples files", default = None)
     parser.add_option("-b", "--bounds", type = "string", dest = "bounds", help = "Density bounds. Must be a string formatted as '[[xmin, xmax], [ymin, ymax],...]'. For 1D distributions use '[xmin, xmax]'. Quotation marks are required and scientific notation is accepted", default = None)
     parser.add_option("-o", "--output", type = "string", dest = "output", help = "Output folder. Default: same directory as samples folder", default = None)
     parser.add_option("--ext", dest = "ext", type = "choice", choices = ['pkl', 'json'], help = "Format of mixture output file", default = 'json')
     parser.add_option("--inj_density", type = "string", dest = "inj_density_file", help = "Python module with injected density - please name the method 'density'", default = None)
     parser.add_option("--selfunc", type = "string", dest = "selfunc_file", help = "Python module with selection function - please name the method 'selection_function'", default = None)
@@ -128,25 +36,26 @@
     parser.add_option("--unit", type = "string", dest = "unit", help = "LaTeX-style quantity unit, for plotting purposes", default = None)
     parser.add_option("--hier_samples", type = "string", dest = "hier_samples", help = "Samples from hierarchical distribution (true single-event values, for simulations only)", default = None)
     # Settings
     parser.add_option("--draws", type = "int", dest = "draws", help = "Number of draws for hierarchical distribution", default = 100)
     parser.add_option("--se_draws", type = "int", dest = "se_draws", help = "Number of draws for single-event distribution. Default: same as hierarchical distribution", default = None)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
-    parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
+    parser.add_option("--cosmology", type = "choice", dest = "cosmology", help = "Set of cosmological parameters. Default values from Planck (2021)", choices = ['Planck18', 'Planck15'], default = 'Planck18')
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
-    parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
     parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
-
+    parser.add_option("--rate", dest = "rate", action = 'store_true', help = "Compute rate", default = False)
+    parser.add_option("--include_dvdz", dest = "include_dvdz", action = 'store_true', help = "Include dV/dz*(1+z)^{-1} term in selection effects.", default = False)
+    
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
     # Paths
     if options.input is not None:
         options.input = Path(options.input).resolve()
@@ -164,73 +73,107 @@
         options.config = Path(options.config).resolve()
     output_plots = Path(options.output, 'plots')
     if not output_plots.exists():
         output_plots.mkdir()
     output_draws = Path(options.output, 'draws')
     if not output_draws.exists():
         output_draws.mkdir()
+    if options.rate:
+        output_rate = Path(options.output, 'rate')
+        if not output_rate.exists():
+            output_rate.mkdir()
     # Read hierarchical name
     if options.hier_name is None:
         options.hier_name = options.output.parts[-1]
     if options.selfunc_file is None:
         hier_name = 'observed_'+options.hier_name
     else:
         hier_name = 'intrinsic_'+options.hier_name
 
     if options.config is None:
         save_options(options, options.output, name = options.hier_name)
-
+    
     # Read bounds
     if options.bounds is not None:
         options.bounds = np.array(np.atleast_2d(eval(options.bounds)), dtype = np.float64)
     elif options.bounds is None and not options.postprocess:
         raise Exception("Please provide bounds for the inference (use -b '[[xmin,xmax],[ymin,ymax],...]')")
-
-    # Read cosmology
-    options.h, options.om, options.ol = (float(x) for x in options.cosmology.split(','))
     # Read parameter(s)
     if options.par is not None:
         options.par = options.par.split(',')
         if not np.all([par in supported_pars for par in options.par]):
             raise Exception("Please provide parameters from this list: "+', '.join(supported_pars[:-2]))
     # Read number of single-event draws
     if options.se_draws is None:
         options.se_draws = options.draws
     if options.se_sigma_prior is not None:
         options.se_sigma_prior = np.array([float(s) for s in options.se_sigma_prior.split(',')])
     if options.sigma_prior is not None:
         options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
+    # Cosmology
+    if options.cosmology == 'Planck18':
+        approx_dVdz = dVdz_approx_planck18
+    else:
+        approx_dVdz = dVdz_approx_planck15
 
     # If provided, load injected density
     inj_density = None
     if options.inj_density_file is not None:
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
-        spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
-        inj_module = importlib.util.module_from_spec(spec)
+        spec          = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
+        inj_module    = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
-        inj_density = inj_module.density
+        inj_density   = inj_module.density
     # If provided, load selecton function
     selfunc     = None
     inj_pdf     = None
     n_total_inj = None
+    duration    = 1.
     if options.selfunc_file is not None:
-        selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
-        if not callable(selfunc):
+        selfunc, inj_pdf, n_total_inj, duration = load_selection_function(options.selfunc_file,
+                                                                          par           = options.par,
+                                                                          far_threshold = options.far_threshold,
+                                                                          )
+        if not callable(selfunc) and not options.probit:
             # Keeping only the samples within bounds
             selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
             inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
+    if options.include_dvdz and not callable(selfunc):
+        raise Exception("The inclusion of dV/dz*(1+z)^{-1} is available only with a selection function approximant.")
+    if options.include_dvdz:
+        if options.par is None:
+            print("Redshift is assumed to be the last parameter")
+            z_index = -1
+        elif 'z' in options.par:
+            z_index = np.where(np.array(options.par)=='z')[0][0]
+        else:
+            raise Exception("Redshift must be included in the rate analysis")
+        dec_selfunc = _decorator_dVdz(selfunc, approx_dVdz, z_index, options.bounds[z_index][1])
+    else:
+        dec_selfunc = selfunc
+    
     # If provided, load true values
     hier_samples = None
     if options.hier_samples is not None:
         options.hier_samples = Path(options.hier_samples).resolve()
-        hier_samples, true_name = load_single_event(options.hier_samples, par = options.par, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
+        hier_samples, true_name = load_single_event(options.hier_samples,
+                                                    par       = options.par,
+                                                    cosmology = options.cosmology,
+                                                    waveform  = options.wf,
+                                                    )
         if np.shape(hier_samples)[-1] == 1:
             hier_samples = hier_samples.flatten()
+            
     # Load samples
-    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
+    events, names = load_data(options.input,
+                              par       = options.par,
+                              n_samples = options.n_samples_dsp,
+                              cosmology = options.cosmology,
+                              waveform  = options.wf,
+                              )
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
@@ -248,60 +191,87 @@
             symbols = options.symbol.split(',')
         else:
             symbols = options.symbol
         if options.unit is not None:
             units = options.unit.split(',')
         else:
             units = options.unit
-    else:
-        symbols = options.symbol
-        units   = options.unit
     
     # Reconstruction
     if not options.postprocess:
-        ray.init(num_cpus = options.n_parallel)
-        pool = ActorPool([worker.remote(bounds           = options.bounds,
-                                        out_folder_plots = output_plots,
-                                        out_folder_draws = output_draws,
-                                        ext              = options.ext,
-                                        se_sigma         = options.se_sigma_prior,
-                                        hier_sigma       = options.sigma_prior,
-                                        scale            = options.fraction,
-                                        events           = events,
-                                        label            = symbols,
-                                        unit             = units,
-                                        save_se          = options.save_single_event,
-                                        MC_draws         = options.mc_draws,
-                                        probit           = options.probit,
-                                        selfunc          = selfunc,
-                                        inj_pdf          = inj_pdf,
-                                        n_total_inj      = n_total_inj,
-                                        )
-                          for _ in range(options.n_parallel)])
-        
         if options.run_events:
-            # Run each single-event analysis
+            mix = DPGMM(options.bounds, probit = options.probit)
             posteriors = []
-            for s in tqdm(pool.map_unordered(lambda a, v: a.run_event.remote(v), [[ev, name, options.se_draws] for ev, name in zip(events, names)]), total = len(events), desc = 'Events'):
-                posteriors.append(s)
+            # Run each single-event analysis
+            for i in tqdm(range(len(events)), desc = 'Events'):
+                ev   = events[i]
+                name = names[i]
+                prior_pars = get_priors(mix.bounds,
+                                        samples      = ev,
+                                        probit       = options.probit,
+                                        std          = options.se_sigma_prior,
+                                        scale        = options.fraction,
+                                        hierarchical = False,
+                                        )
+                mix.initialise(prior_pars = prior_pars)
+                # Draw samples
+                draws = [mix.density_from_samples(ev, make_comp = False) for _ in range(options.se_draws)]
+                posteriors.append(draws)
+                # Make plots
+                if options.save_single_event:
+                    plt_bounds = np.atleast_2d([ev.min(axis = 0), ev.max(axis = 0)]).T
+                    if dim == 1:
+                        plot_median_cr(draws,
+                                       samples    = ev,
+                                       bounds     = plt_bounds[0],
+                                       out_folder = output_plots,
+                                       name       = name,
+                                       label      = options.symbol,
+                                       unit       = options.unit,
+                                       subfolder  = True,
+                                       )
+                    else:
+                        plot_multidim(draws,
+                                      samples    = ev,
+                                      bounds     = plt_bounds,
+                                      out_folder = output_plots,
+                                      name       = name,
+                                      labels     = symbols,
+                                      units      = units,
+                                      subfolder  = True,
+                                      )
+                # Save single-event draws
+                save_density(draws, folder = output_draws, name = 'draws_'+name, ext = options.ext)
             # Save all single-event draws together
             posteriors = np.array(posteriors)
             save_density(posteriors, folder = output_draws, name = 'posteriors_single_event', ext = options.ext)
         else:
+            # Load pre-computed posteriors
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=UserWarning)
                 posteriors = load_density(Path(output_draws, 'posteriors_single_event.'+options.ext), make_comp = False)
-        # Load posteriors
-        for s in pool.map(lambda a, v: a.load_posteriors.remote(v), [posteriors for _ in range(options.n_parallel)]):
-            pass
         # Run hierarchical analysis
-        draws = []
-        for s in tqdm(pool.map_unordered(lambda a, v: a.draw_hierarchical.remote(), [_ for _ in range(options.draws)]), total = options.draws, desc = 'Sampling'):
-            draws.append(s)
-        draws = np.array(draws)
+        prior_pars = get_priors(options.bounds,
+                                samples      = events,
+                                std          = options.sigma_prior,
+                                scale        = options.fraction,
+                                probit       = options.probit,
+                                hierarchical = True,
+                                )
+        mix = HDPGMM(options.bounds,
+                     prior_pars         = prior_pars,
+                     MC_draws           = options.mc_draws,
+                     probit             = options.probit,
+                     selection_function = dec_selfunc,
+                     injection_pdf      = inj_pdf,
+                     total_injections   = n_total_inj,
+                     )
+        draws = np.array([mix.density_from_samples(posteriors, make_comp = False) for _ in tqdm(range(options.draws), desc = 'Hierarchical')])
+        if options.include_dvdz:
+            normalise_alpha_factor(draws, dvdz = approx_dVdz, z_index = z_index, options.bounds[z_index][1])
         # Save draws
         save_density(draws, folder = output_draws, name = 'draws_'+hier_name, ext = options.ext)
     else:
         draws = load_density(Path(output_draws, 'draws_'+hier_name+'.'+options.ext))
     # Plot
     if dim == 1:
         plot_median_cr(draws,
@@ -319,9 +289,61 @@
                       out_folder   = output_plots,
                       name         = hier_name,
                       labels       = symbols,
                       units        = units,
                       hierarchical = True,
                       )
 
+    if options.rate:
+        R_samples = sample_rate(draws,
+                                n_obs   = len(events),
+                                selfunc = selfunc,
+                                T       = duration,
+                                size    = 1e4,
+                                dvdz    = approx_dVdz,
+                                z_index = z_index,
+                                )
+        plot_integrated_rate(R_samples,
+                             out_folder = output_rate,
+                             name       = options.hier_name,
+                             )
+        np.savetxt(Path(output_rate, 'samples_integrated_rate_{}.txt'.format(options.hier_name)), R_samples)
+        # Best estimate for rate
+        rates = sample_rate(draws,
+                            n_obs   = len(events),
+                            selfunc = selfunc,
+                            T       = duration,
+                            size    = 1e4,
+                            dvdz    = approx_dVdz,
+                            z_index = z_index,
+                            each    = True,
+                            )
+        if options.par is not None:
+            names = options.par
+        else:
+            names = np.arange(dim)
+        # Marginal rates
+        if dim == 1:
+            plot_differential_rate(draws,
+                                   rate         = rates,
+                                   out_folder   = output_rate,
+                                   name         = options.hier_name,
+                                   label        = options.symbol,
+                                   unit         = options.unit,
+                                   hierarchical = True,
+                                   )
+        else:
+            for i in range(dim):
+                dims = list(np.arange(dim))
+                dims.remove(i)
+                dd   = marginalise(draws, dims)
+                plot_differential_rate(dd,
+                                       rate         = rates,
+                                       out_folder   = output_rate,
+                                       name         = names[i],
+                                       label        = symbols[i],
+                                       unit         = units[i],
+                                       hierarchical = True,
+                                       )
+
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `figaro-1.6.1/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.2/figaro/_pipelines/probability_density.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,42 +2,24 @@
 
 import optparse
 import dill
 import importlib
 
 from pathlib import Path
 from tqdm import tqdm
+from warnings import warn
 
 from figaro.mixture import DPGMM
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_single_event, save_density, load_density, supported_extensions, supported_pars
-
-import ray
-from ray.util import ActorPool
-
-@ray.remote
-class worker:
-    def __init__(self, bounds,
-                       sigma = None,
-                       samples = None,
-                       probit = True,
-                       scale = None,
-                       ):
-        self.dim     = bounds.shape[-1]
-        self.mixture = DPGMM(bounds, prior_pars = get_priors(bounds, samples = samples, std = sigma, scale = scale, probit = probit, hierarchical = False), probit = probit)
-        self.samples = np.copy(samples)
-        self.samples.setflags(write = True)
-
-    def draw_sample(self):
-        return self.mixture.density_from_samples(self.samples, make_comp = False)
+from figaro.load import load_single_event, load_selection_function, save_density, load_density, supported_extensions, supported_pars
 
 def main():
 
-    parser = optparse.OptionParser(prog = 'figaro-par-density', description = 'Parallelised probability density reconstruction')
+    parser = optparse.OptionParser(prog = 'figaro-density', description = 'Probability density reconstruction')
     # Input/output
     parser.add_option("-i", "--input", type = "string", dest = "input", help = "File with samples", default = None)
     parser.add_option("-b", "--bounds", type = "string", dest = "bounds", help = "Density bounds. Must be a string formatted as '[[xmin, xmax], [ymin, ymax],...]'. For 1D distributions use '[xmin, xmax]'. Quotation marks are required and scientific notation is accepted", default = None)
     parser.add_option("-o", "--output", type = "string", dest = "output", help = "Output folder. Default: same directory as samples", default = None)
     parser.add_option("--ext", dest = "ext", type = "choice", choices = ['pkl', 'json'], help = "Format of mixture output file", default = 'json')
     parser.add_option("--inj_density", type = "string", dest = "inj_density_file", help = "Python module with injected density - please name the method 'density'", default = None)
     parser.add_option("--selfunc", type = "string", dest = "selfunc_file", help = "Python module with selection function - please name the method 'selection_function'", default = None)
@@ -47,18 +29,17 @@
     parser.add_option("-p", "--postprocess", dest = "postprocess", action = 'store_true', help = "Postprocessing", default = False)
     parser.add_option("--symbol", type = "string", dest = "symbol", help = "LaTeX-style quantity symbol, for plotting purposes", default = None)
     parser.add_option("--unit", type = "string", dest = "unit", help = "LaTeX-style quantity unit, for plotting purposes", default = None)
     # Settings
     parser.add_option("--draws", type = "int", dest = "draws", help = "Number of draws", default = 100)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
-    parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
+    parser.add_option("--cosmology", type = "choice", dest = "cosmology", help = "Set of cosmological parameters. Default values from Planck (2021)", choices = ['Planck18', 'Planck15'], default = 'Planck18')
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
-    parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
     
     (options, args) = parser.parse_args()
 
@@ -75,26 +56,22 @@
         options.output = Path(options.output).resolve()
         if not options.output.exists():
             options.output.mkdir(parents=True)
     else:
         options.output = options.input.parent
     if options.config is not None:
         options.config = Path(options.config).resolve()
-    
     if options.config is None:
         save_options(options, options.output)
 
     # Read bounds
     if options.bounds is not None:
         options.bounds = np.array(np.atleast_2d(eval(options.bounds)), dtype = np.float64)
     elif options.bounds is None and not options.postprocess:
         raise Exception("Please provide bounds for the inference (use -b '[[xmin,xmax],[ymin,ymax],...]')")
-
-    # Read cosmology
-    options.h, options.om, options.ol = (float(x) for x in options.cosmology.split(','))
     # Read parameter(s)
     if options.par is not None:
         options.par = options.par.split(',')
         if not np.all([par in supported_pars for par in options.par]):
             raise Exception("Please provide parameters from this list: "+', '.join(supported_pars[:-2]))
     # If provided, load injected density
     inj_density = None
@@ -103,18 +80,18 @@
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
     #If provided, load selecton function
     selfunc = None
     if options.selfunc_file is not None:
-        selfunc, _ = load_selection_function(options.selfunc_file, par = options.par)
+        selfunc, _, _, _ = load_selection_function(options.selfunc_file, par = options.par)
         if not callable(selfunc):
             raise Exception("Only .py files with callable approximants are allowed for DPGMM reconstruction")
-        
+    
     if options.sigma_prior is not None:
         options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
     if options.input.is_file():
         files = [options.input]
         output_draws = options.output
         subfolder = False
     else:
@@ -122,20 +99,17 @@
         output_draws = Path(options.output, 'draws')
         if not output_draws.exists():
             output_draws.mkdir()
         subfolder = True
     if options.exclude_points:
         print("Ignoring points outside bounds.")
     
-    if not options.postprocess:
-        ray.init(num_cpus = options.n_parallel)
-    
     for i, file in enumerate(files):
         # Load samples
-        samples, name = load_single_event(file, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+        samples, name = load_single_event(file, par = options.par, n_samples = options.n_samples_dsp, cosmology = options.cosmology, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
         try:
             dim = np.shape(samples)[-1]
         except IndexError:
             dim = 1
         if options.exclude_points:
             samples = samples[np.where((np.prod(options.bounds[:,0] < samples, axis = 1) & np.prod(samples < options.bounds[:,1], axis = 1)))]
         else:
@@ -143,26 +117,18 @@
             if options.probit:
                 if not np.all([(samples[:,i] > options.bounds[i,0]).all() and (samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
                     raise ValueError("One or more samples are outside the given bounds.")
 
         # Reconstruction
         if not options.postprocess:
             # Actual analysis
-            desc = name + ' ({0}/{1})'.format(i+1, len(files))
-            pool = ActorPool([worker.remote(bounds  = options.bounds,
-                                            sigma   = options.sigma_prior,
-                                            scale   = options.fraction,
-                                            samples = samples,
-                                            probit  = options.probit,
-                                            )
-                              for _ in range(options.n_parallel)])
-            draws = []
-            for s in tqdm(pool.map_unordered(lambda a, v: a.draw_sample.remote(), [_ for _ in range(options.draws)]), total = options.draws, desc = desc):
-                draws.append(s)
-            draws = np.array(draws)
+            prior_pars = get_priors(options.bounds, samples = samples, std = options.sigma_prior, scale = options.fraction, probit = options.probit, hierarchical = False)
+            mix        = DPGMM(options.bounds, prior_pars = prior_pars, probit = options.probit)
+            desc       = name + ' ({0}/{1})'.format(i+1, len(files))
+            draws      = np.array([mix.density_from_samples(samples, make_comp = False) for _ in tqdm(range(options.draws), desc = desc)])
             # Save reconstruction
             save_density(draws, folder = output_draws, name = 'draws_'+name, ext = options.ext)
         else:
             draws = load_density(Path(output_draws, 'draws_'+name+'.'+options.ext))
 
         # Plot
         if dim == 1:
```

### Comparing `figaro-1.6.1/figaro/credible_regions.py` & `figaro-1.6.2/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/cumulative.py` & `figaro-1.6.2/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/decorators.py` & `figaro-1.6.2/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/diagnostic.py` & `figaro-1.6.2/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/exceptions.py` & `figaro-1.6.2/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/load.py` & `figaro-1.6.2/figaro/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 import json
 import dill
 import copy
 import importlib
 from figaro.exceptions import FIGAROException
 from figaro.mixture import mixture
-from figaro.cosmology import CosmologicalParameters
+from figaro.cosmology import Planck18, Planck15
 from pathlib import Path
 from tqdm import tqdm
 
 supported_extensions = ['h5', 'hdf5', 'txt', 'dat', 'csv']
 supported_waveforms  = ['combined', 'imr', 'seob']
 injected_pars        = ['m1', 'm2', 'z', 's1x', 's1y', 's1z', 's2x', 's2y', 's2z', 'ra', 'dec']
 loadable_inj_pars    = injected_pars + ['q', 'chi_eff', 'chi_p', 's1', 's2']
@@ -73,30 +73,28 @@
 
 def available_gw_pars():
     """
     Print a list of available GW parameters
     """
     print(supported_pars)
 
-def load_single_event(event, seed = False, par = None, n_samples = -1, h = 0.674, om = 0.315, ol = 0.685, volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None):
+def load_single_event(event, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None):
     '''
     Loads the data from .txt/.dat files (for simulations) or .h5/.hdf5 files (posteriors from GWTC) for a single event.
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of the available parameters.
     
     Arguments:
-        str or Path file: file with samples
-        bool seed:        fixes the seed to a default value (1) for reproducibility
-        list-of-str par:  list with parameter(s) to extract from GW posteriors (m1, m2, mc, z, chi_effective)
-        int n_samples:    number of samples for (random) downsampling. Default -1: all samples
-        double h:         Hubble constant H0/100 [km/(s*Mpc)]
-        double om:        matter density parameter
-        double ol:        cosmological constant density parameter
-        bool volume:      if True, loads RA, dec and Luminosity distance (for skymaps)
-        str waveform:     waveform family to be used ('combined', 'seob', 'imr')
+        str or Path file:     file with samples
+        bool seed:            fixes the seed to a default value (1) for reproducibility
+        list-of-str par:      list with parameter(s) to extract from GW posteriors (m1, m2, mc, z, chi_effective)
+        int n_samples:        number of samples for (random) downsampling. Default -1: all samples
+        str cosmology:        set of cosmological parameters (Planck18 or Planck15)
+        bool volume:          if True, loads RA, dec and Luminosity distance (for skymaps)
+        str waveform:         waveform family to be used ('combined', 'seob', 'imr')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
         
     Returns:
         np.ndarray: samples
         np.ndarray: name
     '''
@@ -125,37 +123,35 @@
             raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
         # Check that all the parametes are loadable
         if not np.all([p in GW_par.keys() for p in par]):
             wrong_pars = [p for p in par if not p in GW_par.keys()]
             raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
         # If everything is ok, load the samples
         else:
-            out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = (h, om, ol), rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
+            out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
     
     if out is None:
         return out, name
     
     if len(np.shape(out)) == 1:
         out = np.atleast_2d(out).T
     return out, name
 
-def load_data(path, seed = False, par = None, n_samples = -1, h = 0.674, om = 0.315, ol = 0.685, volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None, verbose = True):
+def load_data(path, seed = False, par = None, n_samples = -1, cosmology = 'Planck18', volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None, verbose = True):
     '''
     Loads the data from .txt files (for simulations) or .h5/.hdf5/.dat files (posteriors from GWTC-x).
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of available parameters.
     
     Arguments:
         str or Path path:     folder with data files
         bool seed:            fixes the seed to a default value (1) for reproducibility
         list-of-str par:      list with parameter(s) to extract from GW posteriors
         int n_samples:        number of samples for (random) downsampling. Default -1: all samples
-        double h:             Hubble constant H0/100 [km/(s*Mpc)]
-        double om:            matter density parameter
-        double ol:            cosmological constant density parameter
+        str cosmology:        set of cosmological parameters (Planck18 or Planck15)
         str waveform:         waveform family to be used ('combined', 'seob', 'imr')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
         bool verbose:         show progress bar
 
     Returns:
         np.ndarray: samples
@@ -203,15 +199,15 @@
                 raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
             # Check that all the parametes are loadable
             if not np.all([p in GW_par.keys() for p in par]):
                 wrong_pars = [p for p in par if not p in GW_par.keys()]
                 raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
             # If everything is ok, load the samples
             else:
-                out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = (h, om, ol), rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
+                out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
                 if out is not None:
                     if out.shape[-1] == len(par):
                         events.append(out)
                     elif 'snr' in par:
                         removed_snr = True
                         names.remove(name)
                 else:
@@ -243,16 +239,20 @@
         str waveform:         waveform family to be used ('combined', 'imr', 'seob')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
     
     Returns:
         np.ndarray: samples
     '''
-    h, om, ol = cosmology
-    omega = CosmologicalParameters(h, om, ol, -1, 0, 0)
+    if cosmology == 'Planck18':
+        omega = Planck18
+    elif cosmology == 'Planck15':
+        omega = Planck15
+    else:
+        raise FIGAROException("Cosmology not supported")
     if not waveform in supported_waveforms:
         raise FIGAROException("Unknown waveform: please use 'combined' (default), 'imr' or 'seob'")
     
     if far_threshold is not None and snr_threshold is not None:
         warnings.warn("Both FAR and SNR threshold provided. FAR will be used.")
         snr_threshold = None
     
@@ -617,62 +617,72 @@
         str or Path file: selection function file
         list-of-str par:  list with parameter(s) to extract from GW posteriors
         double threshold: FAR threshold to filter LVK injections
     
     Returns:
         np.ndarray or callable: detected samples or callable with approximant
         np.ndarray or NoneType: injection pdf (for samples) or None (for approximant)
+        int or NoneType:        total number of injections
+        double duration:        duration of the observation
     """
     file = Path(file)
     ext  = file.parts[-1].split('.')[1]
     if not ext in supported_extensions + ['py']:
         raise FIGAROException("Selection function file not supported")
     if ext == 'py':
         selfunc_file_name = file.parts[-1].split('.')[0]
         spec              = importlib.util.spec_from_file_location(selfunc_file_name, file)
         selfunc_module    = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(selfunc_module)
         selfunc           = selfunc_module.selection_function
         inj_pdf           = None
         n_total_inj       = None
+        try:
+            duration      = selfunc_module.duration
+        except:
+            duration      = 1.
     else:
         if not ext in ['h5','hdf5']:
             samples     = np.loadtxt(file)
             det_idx     = samples[:,-1]
             selfunc     = samples[:,:-2][det_idx == 1]
             inj_pdf     = samples[:,-2][det_idx == 1]
             n_total_inj = len(samples)
+            duration    = 1.
         else:
-            selfunc, inj_pdf, n_total_inj = _unpack_injections(file, par, far_threshold)
-    return selfunc, inj_pdf, n_total_inj
+            selfunc, inj_pdf, n_total_inj, duration = _unpack_injections(file, par, far_threshold)
+    return selfunc, inj_pdf, n_total_inj, duration
 
 def _unpack_injections(file, par, far_threshold = 1.):
     """
     Reads data from .h5/.hdf5 injection file (https://zenodo.org/records/7890437).
     A sample is considered detected if at least one of the searches calls a detection.
     
     Arguments:
         str event:            file to read
         str par:              parameter to extract
         double far_threshold: FAR threshold for injection filtering
     
     Returns:
-        np.ndarray: samples
-        np.ndarray: injection pdf
+        np.ndarray:      samples
+        np.ndarray:      injection pdf
+        int or NoneType: total number of injections
+        double duration: duration of the observation
     """
     # Check that a list of parameters is passed
     if par is None:
         raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
     # Check that all the parametes are loadable
     if not np.all([p in loadable_inj_pars for p in par]):
         wrong_pars = [p for p in par if not p in loadable_inj_pars]
         raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars))
     with h5py.File(file, 'r') as f:
         data = f['injections']
         n_total_inj = int(data.attrs['total_generated'])
+        duration    = data.attrs['analysis_time_s']/(60.*60.*24.*365) # Years
         # Detected injections
         far_cwb    = np.array(data['far_cwb'])
         far_gstlal = np.array(data['far_gstlal'])
         far_mbta   = np.array(data['far_mbta'])
         try:
             far_pycbc = np.array(data['far_pycbc_bbh'])
         except:
@@ -736,8 +746,8 @@
         if 'z' in par:
             inj_pdf *= np.array(data['redshift_sampling_pdf'])[idx]
         # Sky position
         if 'ra' in par:
             inj_pdf *= np.array(data['right_ascension_sampling_pdf'])[idx]
         if 'dec' in par:
             inj_pdf *= np.array(data['declination_sampling_pdf'])[idx]
-    return samples.T, inj_pdf, n_total_inj
+    return samples.T, inj_pdf, n_total_inj, duration
```

### Comparing `figaro-1.6.1/figaro/marginal.py` & `figaro-1.6.2/figaro/marginal.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     means  = np.delete(mix.means, ax, axis = -1)
     covs   = np.delete(np.delete(mix.covs, ax, axis = -1), ax, axis = -2)
     bounds = np.delete(mix.bounds, ax, axis = 0)
     if mix.components is None:
         make_comp = False
     else:
         make_comp = True
-    return mixture(means, covs, mix.w, bounds, dim, mix.n_cl, mix.n_pts, mix.alpha, probit = mix.probit, make_comp = make_comp)
+    return mixture(means, covs, mix.w, bounds, dim, mix.n_cl, mix.n_pts, mix.alpha, probit = mix.probit, make_comp = make_comp, alpha_factor = mix.alpha_factor)
 
 def marginalise(draws, axis = -1):
     """
     Marginalise out one or more dimensions from a FIGARO draw.
     
     Arguments:
         figaro.mixture.mixture draws: mixture(s)
@@ -130,15 +130,15 @@
         idx_filt = [i in idx[m:] for i in range(len(ww))]
         if norm:
             log_weights -= logsumexp(log_weights[idx_filt])
     if mix.components is None:
         make_comp = False
     else:
         make_comp = True
-    return mixture(means[idx_filt], covs[idx_filt], np.exp(log_weights[idx_filt]), bounds, dim, len(log_weights[idx_filt]), mix.n_pts, mix.alpha, probit = mix.probit, log_w = log_weights[idx_filt], make_comp = make_comp)
+    return mixture(means[idx_filt], covs[idx_filt], np.exp(log_weights[idx_filt]), bounds, dim, len(log_weights[idx_filt]), mix.n_pts, mix.alpha, probit = mix.probit, log_w = log_weights[idx_filt], make_comp = make_comp, alpha_factor = mix.alpha_factor)
 
 def condition(draws, vals, dims, norm = True, filter = True, tol = 1e-4):
     """
     Probability density conditioned on specific values of a subset of parameters.
     
     Arguments:
         figaro.mixture.mixture draws: mixture(s)
```

### Comparing `figaro-1.6.1/figaro/mixture.py` & `figaro-1.6.2/figaro/mixture.py`

 * *Files 7% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         
         idx        = np.random.choice(len(mu_MC), p = np.exp(logL_D - log_norm_D))
         self.mu    = np.copy(mu_MC[idx])
         self.sigma = np.copy(sigma_MC[idx])
         if dim == 1:
             self.mu = np.atleast_2d(self.mu).T
             self.sigma = np.atleast_2d(self.sigma).T
-        self.N_true = np.exp(np.log(self.N) - log_alpha_factor[idx])
+        self.log_N_true = np.log(self.N) - log_alpha_factor[idx]
             
 class density:
     """
     Class to initialise a common set of methods for mixture models. Not to be used.
     """
     def __init__(self):
         pass
@@ -677,48 +677,50 @@
 
 class mixture(density):
     """
     Class to store a single draw from DPGMM/(H)DPGMM.
     Methods inherited from density class
     
     Arguments:
-        iterable means:    component means
-        iterable covs:     component covariances
-        np.ndarray w:      component weights
-        np.ndarray bounds: bounds of probit transformation
-        int dim:           number of dimensions
-        int n_cl:          number of clusters in the mixture
-        int n_pts:         number of points used to infer the mixture
-        double alpha:      concentration parameter
-        bool probit:       whether to use the probit transformation or not
-        np.ndarray log_w:  component log weights
-        bool make_comp:    make component objects
+        iterable means:      component means
+        iterable covs:       component covariances
+        np.ndarray w:        component weights
+        np.ndarray bounds:   bounds of probit transformation
+        int dim:             number of dimensions
+        int n_cl:            number of clusters in the mixture
+        int n_pts:           number of points used to infer the mixture
+        double alpha:        concentration parameter
+        bool probit:         whether to use the probit transformation or not
+        np.ndarray log_w:    component log weights
+        bool make_comp:      make component objects
+        double alpha_factor: evaluated \int pdet(theta)p(theta|lambda) conditioned on the mixture parameters
     
     Returns:
         mixture: instance of mixture class
     """
-    def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, alpha = 1., probit = True, log_w = None, make_comp = True):
+    def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, alpha = 1., probit = True, log_w = None, make_comp = True, alpha_factor = 1.):
         self.means = means
         self.covs  = covs
         if make_comp:
             self.components = [mn(mean, cov, allow_singular = True) for mean, cov in zip(self.means, self.covs)]
         else:
             self.components = None
         if log_w is None:
             self.w      = w
             self.log_w  = np.log(w)
         else:
             self.log_w  = log_w
-            self.w      = np.exp(log_w)
-        self.bounds = bounds
-        self.dim    = int(dim)
-        self.n_cl   = int(n_cl)
-        self.n_pts  = int(n_pts)
-        self.probit = probit
-        self.alpha  = alpha
+            self.w        = np.exp(log_w)
+        self.bounds       = bounds
+        self.dim          = int(dim)
+        self.n_cl         = int(n_cl)
+        self.n_pts        = int(n_pts)
+        self.probit       = probit
+        self.alpha        = alpha
+        self.alpha_factor = alpha_factor
     
     def marginalise(self, axis = -1):
         """
         Marginalise out one or more dimensions from the mixture.
         
         Arguments:
             int or list of int axis: axis to marginalise on. Default: last
@@ -1178,17 +1180,18 @@
         self.selfunc = selection_function
         if not callable(self.selfunc) and self.selfunc is not None:
             try:
                 self.log_inj_pdf = np.log(injection_pdf)
                 self.total_inj   = int(total_injections)
             except TypeError:
                 raise FIGAROException("Please provide injection pdf")
+            self.selfunc_probit   = self.selfunc
             self.log_jacobian_inj = np.zeros(len(self.selfunc))
             if self.probit:
-                self.selfunc = transform_to_probit(self.selfunc, self.bounds)
+                self.selfunc_probit   = transform_to_probit(self.selfunc, self.bounds)
                 self.log_jacobian_inj = -probit_logJ(self.selfunc, self.bounds, self.probit)
         # MC samples
         self._draw_MC_samples()
         
     def initialise(self):
         """
         Initialise the mixture to initial conditions
@@ -1214,23 +1217,23 @@
             self.sigma_MC = np.array([r*outer_jit(s,s) for r, s in zip(rhos, np.sqrt(self.sigma_MC))])
         if self.selfunc is not None:
             # Approximant
             if callable(self.selfunc):
                 n_samples = self.MC_draws
                 with np.errstate(divide = 'ignore', invalid = 'ignore'):
                     if self.probit:
-                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(transform_from_probit(mn(m,s).rvs(self.MC_draws), self.bounds)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
+                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(transform_from_probit(mn(m,s, allow_singular = True).rvs(self.MC_draws), self.bounds)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
                     else:
-                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(mn(m,s).rvs(self.MC_draws)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
+                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(mn(m,s, allow_singular = True).rvs(self.MC_draws)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
             # Injections
             else:
                 n_samples = self.total_inj
-                self.log_alpha_factor = np.array([logsumexp_jit(mn(m,s).logpdf(self.selfunc) + self.log_jacobian_inj - self.log_inj_pdf) - np.log(self.total_inj) for m, s in zip(self.mu_MC, self.sigma_MC)])
+                self.log_alpha_factor = np.array([logsumexp_jit(mn(m,s, allow_singular = True).logpdf(self.selfunc_probit) + self.log_jacobian_inj - self.log_inj_pdf) - np.log(self.total_inj) for m, s in zip(self.mu_MC, self.sigma_MC)])
             # Numerical stability: mu+sigma ignored if p_det too small (not enough predicted points to have a reliable value for alpha)
-            self.log_alpha_factor[self.log_alpha_factor < np.log(5e-3)] = np.inf
+            self.log_alpha_factor[self.log_alpha_factor < np.log(5e-4)] = np.inf
             # Check for NaNs
             self.log_alpha_factor = np.nan_to_num(self.log_alpha_factor, nan = np.inf, posinf = np.inf, neginf = np.inf)
         else:
             self.log_alpha_factor = np.zeros(self.MC_draws)
         
     def add_new_point(self, ev):
         """
@@ -1352,15 +1355,15 @@
         ss.mu    = np.copy(self.mu_MC[idx])
         ss.sigma = np.copy(self.sigma_MC[idx])
         if self.dim == 1:
             ss.mu = np.atleast_2d(ss.mu).T
             ss.sigma = np.atleast_2d(ss.sigma).T
         
         ss.N += 1
-        ss.N_true = np.exp(np.log(ss.N) - self.log_alpha_factor[idx])
+        ss.log_N_true = np.log(ss.N) - self.log_alpha_factor[idx]
         return ss
 
     def _remove_datapoint_from_component(self, ss, logL_D):
         """
         Update component parameters after assigning a sample to a component
         
         Arguments:
@@ -1377,32 +1380,58 @@
         ss.mu    = np.copy(self.mu_MC[idx])
         ss.sigma = np.copy(self.sigma_MC[idx])
         if self.dim == 1:
             ss.mu = np.atleast_2d(ss.mu).T
             ss.sigma = np.atleast_2d(ss.sigma).T
         
         ss.N -= 1
-        ss.N_true = np.exp(np.log(ss.N) - self.log_alpha_factor[idx])
+        ss.log_N_true = np.log(ss.N) - self.log_alpha_factor[idx]
         return ss
 
     def build_mixture(self, make_comp = True):
         """
         Instances a mixture class representing the inferred distribution
         
         Arguments:
             bool make_comp:   whether to instantiate the scipy.stats.multivariate_normal components or not
         
         Returns:
             mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
-        idx = np.where(np.array(self.N_list) > 0)[0]
-        w   = dirichlet(np.array([comp.N_true for comp in np.array(self.mixture)[idx]])+self.alpha/self.n_cl).rvs()[0]
-        return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp)
+        idx   = np.where(np.array(self.N_list) > 0)[0]
+        N_pts = np.array([comp.log_N_true for comp in np.array(self.mixture)[idx]])
+        if self.selfunc is not None:
+            log_w, w           = self.log_w, self.w
+            self.log_w         = N_pts - logsumexp_jit(N_pts)
+            self.w             = np.exp(self.log_w)
+            alpha_factor       = self.compute_alpha_factor()
+            N_pts              = self.w*self.n_pts/alpha_factor
+            self.log_w, self.w = log_w, w
+        else:
+            alpha_factor = 1.
+            N_pts = np.exp(N_pts)
+        w = dirichlet(N_pts+self.alpha/self.n_cl).rvs()[0]
+        return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp, alpha_factor = alpha_factor)
+    
+    def compute_alpha_factor(self):
+        """
+        Compute the integral \int pdet(theta)p(theta|lambda) dtheta conditioned on the specific DPGMM parameters
+        
+        Returns:
+            double: value of the integral
+        """
+        # Approximant
+        if callable(self.selfunc):
+            alpha_factor = np.mean(self.selfunc(self.rvs(self.MC_draws)))
+        # Injections
+        else:
+            alpha_factor = np.exp(logsumexp_jit(self.logpdf(self.selfunc) - self.log_inj_pdf) - np.log(self.total_inj))
+        return alpha_factor
 
     def density_from_samples(self, events, make_comp = True):
         """
         Reconstruct the probability density from a set of samples.
         
         Arguments:
             iterable samples: set of single-event draws from DPGMM
```

### Comparing `figaro-1.6.1/figaro/montecarlo.py` & `figaro-1.6.2/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/plot.py` & `figaro-1.6.2/figaro/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         bool save:                       whether to save the plots or not
         bool show:                       whether to show the plots during the run or not
         bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
         float true_value:                true value to infer
         str true_value_label:            label to assign to the true value marker
         str injected_label:              label to assign to the injected distribution
         str median_label:                label to assign to the reconstruction
-        matplotlib.figure.Figure fig:    figure to use for plotting. Must have (dim,dim) axes.
+        matplotlib.figure.Figure fig:    figure to use for plotting.
         list-of-str colors:              list of colors for median, 68% and 90% credible regions
         
     
     Returns:
         matplotlib.figure.Figure: figure with the plot
     """
     if median_label is None:
@@ -164,17 +164,15 @@
         if bounds is None:
             x_min_l, x_max_l = ax.get_xlim()
             x_min = np.max((x_min, x_min_l))
             x_max = np.min((x_max, x_max_l))
     xlim = (x_min, x_max)
     x    = np.linspace(x_min, x_max, n_pts)
     dx   = x[1]-x[0]
-    
     probs = np.array([d.pdf(x) for d in draws])
-    
     percentiles = [50, 5, 16, 84, 95]
     p = {}
     for perc in percentiles:
         p[perc] = np.percentile(probs, perc, axis = 0)
     norm = p[50].sum()*dx
     for perc in percentiles:
         p[perc] = p[perc]/norm
@@ -548,15 +546,15 @@
                     Path(out_folder, 'density').mkdir()
                 except FileExistsError:
                     pass
             fig.savefig(Path(out_folder, 'density', '{0}.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
     return fig
     
-def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False, colors = ['steelblue','darkturquoise','mediumturquoise']):
+def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False, colors = ['steelblue','darkturquoise','mediumturquoise'], fig = None):
     """
     Plot a 1D distribution along with samples from the true distribution (if available).
     Differently from plot_median_cr, this method requires the distribution to be already evaluated.
     For FIGARO mixture instances, please use plot_median_cr.
 
     Arguments:
         iterable x:                      values at which realisations are evaluated
@@ -573,27 +571,31 @@
         float true_value:                true value to infer
         str true_value_label:            label to assign to the true value marker
         str injected_label:              label to assign to the injected distribution
         str median_label:                label to assign to the median distribution
         bool logx:                       x log scale
         bool logy:                       y log scale
         list-of-str colors:              list of colors for median, 68% and 90% credible regions
+        matplotlib.figure.Figure fig:    figure to use for plotting.
     """
     
     if not np.shape(x)[0] == np.shape(draws)[-1]:
         raise ValueError("x and each draw must have the same length")
     
     percentiles = [50, 5, 16, 84, 95]
     p = {}
     for perc in percentiles:
         p[perc] = np.percentile(draws, perc, axis = 0)
     
     color_med, color_68, color_90 = colors
     
-    fig, ax = plt.subplots()
+    if fig is None:
+        fig, ax = plt.subplots()
+    else:
+        ax = fig.axes[0]
     
     # Samples (if available)
     if samples is not None:
         ax.hist(samples, bins = int(np.sqrt(len(samples))), histtype = 'step', density = True, label = '$\mathrm{Samples}$')
         xlim = ax.get_xlim()
         ylim = ax.get_ylim()
     
@@ -661,15 +663,15 @@
         np.savetxt(Path(txt_folder, 'prob_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
     if show:
         ax.autoscale(True)
         if samples is not None:
             ax.set_xlim(xlim)
         plt.show()
     plt.close()
-    
+    return fig
 
 def plot_n_clusters_alpha(n_cl, alpha, out_folder = '.', name = 'event', show = False, save = True):
     """
     Plot the number of clusters and the concentration parameter as functions of the number of samples.
     
     Arguments:
         np.ndarray n_cl:        number of active clusters
@@ -727,66 +729,72 @@
     ax.set_ylabel('$\mathrm{FIGARO}$')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, '{0}_ppplot.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
 
-def pp_plot_levels(CR_levels, median_CR = None, out_folder = '.', name = 'MDC', show = False, save = True):
+def pp_plot_levels(CR_levels, median_CR = None, out_folder = '.', name = 'MDC', show = False, save = True, fig = None, color = 'steelblue'):
     """
     Make pp-plot.
     
     Arguments:
-        iterable CR:            2D array with credible levels for each event
-        iterable median_CR:     credible levels of medians
-        str or Path out_folder: output folder
-        str name:               name to be given to outputs
-        bool save:              whether to save the plot or not
-        bool show:              whether to show the plot during the run or not
+        iterable CR:                  2D array with credible levels for each event
+        iterable median_CR:           credible levels of medians
+        str or Path out_folder:       output folder
+        str name:                     name to be given to outputs
+        bool save:                    whether to save the plot or not
+        bool show:                    whether to show the plot during the run or not
+        matplotlib.figure.Figure fig: figure to use for plotting.
+        str color:                    color for the main line
     """
     CR_levels = np.atleast_1d(CR_levels)
     if len(CR_levels.shape) > 1:
         CR_levels = CR_levels.T
     n_evs     = CR_levels.shape[-1]
     L         = np.linspace(0,1,n_evs+2)
     
-    fig = plt.figure()
-    ax  = fig.add_subplot(111, projection = 'pp_plot')
+    if fig is None:
+        fig = plt.figure()
+        ax  = fig.add_subplot(111, projection = 'pp_plot')
+    else:
+        ax = fig.axes[0]
     ax.add_confidence_band(n_evs, zorder = n_evs)
     ax.add_diagonal(zorder = n_evs+1)
     if len(CR_levels.shape) > 1:
         sorted = []
         for cr in CR_levels:
             if median_CR is not None:
                 lw = 0.3
                 c  = 'lightsteelblue'
             else:
                 lw = 0.6
-                c  = 'steelblue'
+                c  = color
             x = np.append(0, np.append(cr, 1))
             ax.plot(np.sort(x), L, lw = lw, alpha = 0.5, color = c)
         if median_CR is not None:
             x = np.append(0, np.append(median_CR, 1))
-            ax.plot(np.sort(x), L, lw = 0.8, color = 'steelblue', label = '$\mathrm{Median}$', zorder = n_evs+2)
+            ax.plot(np.sort(x), L, lw = 0.8, color = color, label = '$\mathrm{Median}$', zorder = n_evs+2)
         # Add label for draws
         handles, labels = ax.get_legend_handles_labels()
         line = Line2D([0], [0], label='$\mathrm{Draws}$', lw = lw, color = c)
         handles.extend([line])
         ax.legend(handles=handles, loc = 0, frameon = False)
     else:
         x = np.append(0, np.append(CR_levels, 1))
-        ax.plot(np.sort(x), L, lw = 0.8, color = 'steelblue', zorder = n_evs+2)
+        ax.plot(np.sort(x), L, lw = 0.8, color = color, zorder = n_evs+2)
     # Maquillage
     ax.set_xlabel('$P$')
     ax.set_ylabel('$\mathrm{Fraction\ of\ events\ within\ }CR_P$')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, '{0}_ppplot.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
+    return fig
 
 def joyplot(draws, x_values, y_values, credible_regions = False, fill = True, solid = False, overlap = 1., xlabel = None, ylabel = None, xunit = None, yunit = None, colormap = 'coolwarm', out_folder = '.', name = 'joyplot', subfolder = False, show = False, save = True, joy = False):
     """
     Make a joyplot (also known as ridgeline plot) of a set of distributions.
     Heavily inspired by leotac's JoyPy (https://github.com/leotac/joypy).
     
     Arguments:
```

### Comparing `figaro-1.6.1/figaro/plot_settings.py` & `figaro-1.6.2/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/transform.py` & `figaro-1.6.2/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.1/figaro/utils.py` & `figaro-1.6.2/figaro/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import numpy as np
 import warnings
-import dill
 import configparser
 import optparse
 
 from pathlib import Path
-from tqdm import tqdm
-from typing import cast
 from collections import Counter
 from scipy.stats import multivariate_normal as mn
 
 from figaro._numba_functions import *
 from figaro.transform import transform_to_probit, transform_from_probit
-from figaro.exceptions import FIGAROException
 
 def recursive_grid(bounds, n_pts, get_1d = False):
     """
     Recursively generates the n-dimensional grid points (extremes are excluded).
     
     Arguments:
         list-of-lists bounds: extremes for each dimension (excluded)
@@ -225,15 +221,15 @@
 
 def rvs_median(draws, size = 1):
     """
     Generates samples from median distribution of a set of draws.
     
     Arguments:
         iterable draws: container for mixture instances
-        int size:    number of samples
+        int size:       number of samples
     
     Returns:
         np.ndarray: samples
     """
     idx = np.random.choice(np.arange(len(draws)), size = int(size))
     ctr = Counter(idx)
     samples = np.empty(shape = (1, draws[0].dim))
```

### Comparing `figaro-1.6.1/figaro.egg-info/PKG-INFO` & `figaro-1.6.2/figaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.1
+Version: 1.6.2
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.1/figaro.egg-info/SOURCES.txt` & `figaro-1.6.2/figaro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 figaro/exceptions.py
 figaro/load.py
 figaro/marginal.py
 figaro/mixture.py
 figaro/montecarlo.py
 figaro/plot.py
 figaro/plot_settings.py
+figaro/rate.py
 figaro/transform.py
 figaro/utils.py
 figaro.egg-info/PKG-INFO
 figaro.egg-info/SOURCES.txt
 figaro.egg-info/dependency_links.txt
 figaro.egg-info/entry_points.txt
 figaro.egg-info/requires.txt
```

### Comparing `figaro-1.6.1/pyproject.toml` & `figaro-1.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.1'
+version = '1.6.2'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

