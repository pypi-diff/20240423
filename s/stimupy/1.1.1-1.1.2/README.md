# Comparing `tmp/stimupy-1.1.1.tar.gz` & `tmp/stimupy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimupy-1.1.1.tar", last modified: Fri Feb  9 19:04:34 2024, max compression
+gzip compressed data, was "stimupy-1.1.2.tar", last modified: Tue Apr 23 12:46:08 2024, max compression
```

## Comparing `stimupy-1.1.1.tar` & `stimupy-1.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.825109 stimupy-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    15220 2024-02-09 19:04:27.000000 stimupy-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      174 2024-02-09 19:04:27.000000 stimupy-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25679 2024-02-09 19:04:34.825109 stimupy-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6834 2024-02-09 19:04:27.000000 stimupy-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)     2535 2024-02-09 19:04:28.000000 stimupy-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-09 19:04:34.825109 stimupy-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.809109 stimupy-1.1.1/stimupy/
--rw-r--r--   0 root         (0) root         (0)      199 2024-02-09 19:04:28.000000 stimupy-1.1.1/stimupy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.813109 stimupy-1.1.1/stimupy/components/
--rw-r--r--   0 root         (0) root         (0)    10093 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9201 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/angulars.py
--rw-r--r--   0 root         (0) root         (0)     7958 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/edges.py
--rw-r--r--   0 root         (0) root         (0)     4604 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/frames.py
--rw-r--r--   0 root         (0) root         (0)     3617 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/gaussians.py
--rw-r--r--   0 root         (0) root         (0)    12563 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/lines.py
--rw-r--r--   0 root         (0) root         (0)    10403 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/radials.py
--rw-r--r--   0 root         (0) root         (0)    22166 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/shapes.py
--rw-r--r--   0 root         (0) root         (0)     4125 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/texts.py
--rw-r--r--   0 root         (0) root         (0)    28409 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/components/waves.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/logos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.813109 stimupy-1.1.1/stimupy/noises/
--rw-r--r--   0 root         (0) root         (0)     5750 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/noises/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/noises/binaries.py
--rw-r--r--   0 root         (0) root         (0)     3634 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/noises/narrowbands.py
--rw-r--r--   0 root         (0) root         (0)     5633 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/noises/naturals.py
--rw-r--r--   0 root         (0) root         (0)     2604 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/noises/whites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.817109 stimupy-1.1.1/stimupy/papers/
--rw-r--r--   0 root         (0) root         (0)    52618 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/RHS2007.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65164 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/bindmann2004.py
--rw-r--r--   0 root         (0) root         (0)    42984 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/domijan2015.py
--rw-r--r--   0 root         (0) root         (0)     3353 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/example.py
--rw-r--r--   0 root         (0) root         (0)    63991 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/modelfest.py
--rw-r--r--   0 root         (0) root         (0)    16281 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/modelfest_data.csv
--rw-r--r--   0 root         (0) root         (0)    56134 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/modelfest_natural_scene.tif
--rw-r--r--   0 root         (0) root         (0)    56498 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/modelfest_noise.tif
--rw-r--r--   0 root         (0) root         (0)     2673 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/murray2020.mat
--rw-r--r--   0 root         (0) root         (0)    22926 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/murray2020.py
--rw-r--r--   0 root         (0) root         (0)    19273 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/white1981.py
--rw-r--r--   0 root         (0) root         (0)    16725 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/papers/white1985.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.821109 stimupy-1.1.1/stimupy/stimuli/
--rw-r--r--   0 root         (0) root         (0)     5453 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26107 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/benarys.py
--rw-r--r--   0 root         (0) root         (0)    12710 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/bullseyes.py
--rw-r--r--   0 root         (0) root         (0)    16477 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/checkerboards.py
--rw-r--r--   0 root         (0) root         (0)     3320 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/cornsweets.py
--rw-r--r--   0 root         (0) root         (0)    11204 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/cubes.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/delboeufs.py
--rw-r--r--   0 root         (0) root         (0)     6307 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/dungeons.py
--rw-r--r--   0 root         (0) root         (0)      113 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/edges.py
--rw-r--r--   0 root         (0) root         (0)     3805 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/gabors.py
--rw-r--r--   0 root         (0) root         (0)    21153 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/gratings.py
--rw-r--r--   0 root         (0) root         (0)     3094 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/hermanns.py
--rw-r--r--   0 root         (0) root         (0)    11038 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/mondrians.py
--rw-r--r--   0 root         (0) root         (0)     6895 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/mueller_lyers.py
--rw-r--r--   0 root         (0) root         (0)     7163 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/pinwheels.py
--rw-r--r--   0 root         (0) root         (0)     6807 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/plaids.py
--rw-r--r--   0 root         (0) root         (0)     6293 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/ponzos.py
--rw-r--r--   0 root         (0) root         (0)     6922 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/rings.py
--rw-r--r--   0 root         (0) root         (0)    20433 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/sbcs.py
--rw-r--r--   0 root         (0) root         (0)    24124 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/todorovics.py
--rw-r--r--   0 root         (0) root         (0)    55912 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/waves.py
--rw-r--r--   0 root         (0) root         (0)     7046 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/wedding_cakes.py
--rw-r--r--   0 root         (0) root         (0)    32129 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/stimuli/whites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.825109 stimupy-1.1.1/stimupy/utils/
--rw-r--r--   0 root         (0) root         (0)      225 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/color_conversions.py
--rw-r--r--   0 root         (0) root         (0)     7355 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/contrast_conversions.py
--rw-r--r--   0 root         (0) root         (0)     6028 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/export.py
--rw-r--r--   0 root         (0) root         (0)     3452 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/filters.py
--rw-r--r--   0 root         (0) root         (0)     3446 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/masks.py
--rw-r--r--   0 root         (0) root         (0)    13201 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/pad.py
--rw-r--r--   0 root         (0) root         (0)     8148 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/plotting.py
--rw-r--r--   0 root         (0) root         (0)    25203 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/resolution.py
--rw-r--r--   0 root         (0) root         (0)    16149 2024-02-09 19:04:27.000000 stimupy-1.1.1/stimupy/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.825109 stimupy-1.1.1/stimupy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25679 2024-02-09 19:04:34.000000 stimupy-1.1.1/stimupy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2143 2024-02-09 19:04:34.000000 stimupy-1.1.1/stimupy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-09 19:04:34.000000 stimupy-1.1.1/stimupy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      170 2024-02-09 19:04:34.000000 stimupy-1.1.1/stimupy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-09 19:04:34.000000 stimupy-1.1.1/stimupy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 19:04:34.825109 stimupy-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)      187 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_overviews.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_pad.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_resolve_resolutions.py
--rw-r--r--   0 root         (0) root         (0)     2233 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_valid_resolution.py
--rw-r--r--   0 root         (0) root         (0)     4339 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_validate_resolution_components.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-02-09 19:04:27.000000 stimupy-1.1.1/tests/test_waves.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.498897 stimupy-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)    15220 2024-04-23 12:46:03.000000 stimupy-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-23 12:46:03.000000 stimupy-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25679 2024-04-23 12:46:08.498897 stimupy-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6834 2024-04-23 12:46:03.000000 stimupy-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-04-23 12:46:05.000000 stimupy-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 12:46:08.498897 stimupy-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.478897 stimupy-1.1.2/stimupy/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-23 12:46:05.000000 stimupy-1.1.2/stimupy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.482897 stimupy-1.1.2/stimupy/components/
+-rw-r--r--   0 root         (0) root         (0)    10093 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9201 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/angulars.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/edges.py
+-rw-r--r--   0 root         (0) root         (0)     4604 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/frames.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/gaussians.py
+-rw-r--r--   0 root         (0) root         (0)    12563 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/lines.py
+-rw-r--r--   0 root         (0) root         (0)    10403 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/radials.py
+-rw-r--r--   0 root         (0) root         (0)    22166 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/shapes.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/texts.py
+-rw-r--r--   0 root         (0) root         (0)    28411 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/components/waves.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/logos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.482897 stimupy-1.1.2/stimupy/noises/
+-rw-r--r--   0 root         (0) root         (0)     5750 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/noises/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/noises/binaries.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/noises/narrowbands.py
+-rw-r--r--   0 root         (0) root         (0)     5633 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/noises/naturals.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/noises/whites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.486897 stimupy-1.1.2/stimupy/papers/
+-rw-r--r--   0 root         (0) root         (0)    52618 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/RHS2007.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65164 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/bindmann2004.py
+-rw-r--r--   0 root         (0) root         (0)    42984 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/domijan2015.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/example.py
+-rw-r--r--   0 root         (0) root         (0)    63991 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/modelfest.py
+-rw-r--r--   0 root         (0) root         (0)    16281 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/modelfest_data.csv
+-rw-r--r--   0 root         (0) root         (0)    56134 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/modelfest_natural_scene.tif
+-rw-r--r--   0 root         (0) root         (0)    56498 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/modelfest_noise.tif
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/murray2020.mat
+-rw-r--r--   0 root         (0) root         (0)    22926 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/murray2020.py
+-rw-r--r--   0 root         (0) root         (0)    19273 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/white1981.py
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/papers/white1985.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.490897 stimupy-1.1.2/stimupy/stimuli/
+-rw-r--r--   0 root         (0) root         (0)     5453 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26107 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/benarys.py
+-rw-r--r--   0 root         (0) root         (0)    12710 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/bullseyes.py
+-rw-r--r--   0 root         (0) root         (0)    16477 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/checkerboards.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/cornsweets.py
+-rw-r--r--   0 root         (0) root         (0)    11204 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/cubes.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/delboeufs.py
+-rw-r--r--   0 root         (0) root         (0)     6307 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/dungeons.py
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/edges.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/gabors.py
+-rw-r--r--   0 root         (0) root         (0)    21155 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/gratings.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/hermanns.py
+-rw-r--r--   0 root         (0) root         (0)    11038 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/mondrians.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/mueller_lyers.py
+-rw-r--r--   0 root         (0) root         (0)     7163 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/pinwheels.py
+-rw-r--r--   0 root         (0) root         (0)     6807 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/plaids.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/ponzos.py
+-rw-r--r--   0 root         (0) root         (0)     6922 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/rings.py
+-rw-r--r--   0 root         (0) root         (0)    20433 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/sbcs.py
+-rw-r--r--   0 root         (0) root         (0)    24124 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/todorovics.py
+-rw-r--r--   0 root         (0) root         (0)    55912 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/waves.py
+-rw-r--r--   0 root         (0) root         (0)     7046 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/wedding_cakes.py
+-rw-r--r--   0 root         (0) root         (0)    32129 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/stimuli/whites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.494897 stimupy-1.1.2/stimupy/utils/
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/color_conversions.py
+-rw-r--r--   0 root         (0) root         (0)     7355 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/contrast_conversions.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/export.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/filters.py
+-rw-r--r--   0 root         (0) root         (0)     3446 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/masks.py
+-rw-r--r--   0 root         (0) root         (0)    13201 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/pad.py
+-rw-r--r--   0 root         (0) root         (0)     8148 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/plotting.py
+-rw-r--r--   0 root         (0) root         (0)    25203 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/resolution.py
+-rw-r--r--   0 root         (0) root         (0)    16149 2024-04-23 12:46:03.000000 stimupy-1.1.2/stimupy/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.494897 stimupy-1.1.2/stimupy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25679 2024-04-23 12:46:08.000000 stimupy-1.1.2/stimupy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-04-23 12:46:08.000000 stimupy-1.1.2/stimupy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:46:08.000000 stimupy-1.1.2/stimupy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-23 12:46:08.000000 stimupy-1.1.2/stimupy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 12:46:08.000000 stimupy-1.1.2/stimupy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:46:08.494897 stimupy-1.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_overviews.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_pad.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_resolve_resolutions.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_valid_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     4339 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_validate_resolution_components.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-23 12:46:03.000000 stimupy-1.1.2/tests/test_waves.py
```

### Comparing `stimupy-1.1.1/LICENSE` & `stimupy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/PKG-INFO` & `stimupy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimupy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Stimuli for vision science, as image arrays
 Author: Matko Matic, Guillermo Aguilar, Marianne Maertens
 Author-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 Maintainer-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

### Comparing `stimupy-1.1.1/README.md` & `stimupy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/pyproject.toml` & `stimupy-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   { name = "Guillermo Aguilar" },
   { name = "Marianne Maertens" },
 ]
 maintainers = [
   { name = "Lynn Schmittwilken", email = "l.schmittwilken@tu-berlin.de" },
   { name = "Joris Vincent", email = "j.vincent@tu-berlin.de" },
 ]
-version = "1.1.1"
+version = "1.1.2"
 
 requires-python = ">=3.6"
 dependencies = ["numpy", "scipy", "matplotlib", "pandas", "Pillow"]
 
 [project.optional-dependencies]
 dev = ["pytest", "black", "pyupgrade", "flake8"]
 docs = [
@@ -83,9 +83,9 @@
 type = "github"
 
 [tool.semantic_release.publish]
 upload_to_vcs_release = true # upload sdist, wheel to release-tag
 
 
 [tool.codespell]
-skip = "./docs/_build/*"
+skip = "./docs/_build/*,CHANGELOG.md"
 exclude-file = ".codespell.ignore"
```

### Comparing `stimupy-1.1.1/stimupy/components/__init__.py` & `stimupy-1.1.2/stimupy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/angulars.py` & `stimupy-1.1.2/stimupy/components/angulars.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/edges.py` & `stimupy-1.1.2/stimupy/components/edges.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,16 @@
 
     if ramp_width > max(base["visual_size"]) / 2:
         raise ValueError("ramp_width is too large")
 
     dist = np.round(base["oblique"] / ramp_width, 6)
     d1 = copy.deepcopy(dist)
     d2 = copy.deepcopy(dist) * (-1)
+    d1 = d1 - np.abs(d1).min()
+    d2 = d2 - np.abs(d2).min()
     d1[d1 < 0] = -1
     d1[d1 > 1] = 1
     d2[d2 < 0] = -1
     d2[d2 > 1] = 1
 
     # Create ramp profiles individually for left and right side
     profile1 = (1.0 - d1) ** exponent * (
```

### Comparing `stimupy-1.1.1/stimupy/components/frames.py` & `stimupy-1.1.2/stimupy/components/frames.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/gaussians.py` & `stimupy-1.1.2/stimupy/components/gaussians.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/lines.py` & `stimupy-1.1.2/stimupy/components/lines.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/radials.py` & `stimupy-1.1.2/stimupy/components/radials.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/shapes.py` & `stimupy-1.1.2/stimupy/components/shapes.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/texts.py` & `stimupy-1.1.2/stimupy/components/texts.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/components/waves.py` & `stimupy-1.1.2/stimupy/components/waves.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             warnings.warn(
                 f"Adjusted frequency={old_frequency} -> {frequency} because of period={period}"
             )
 
     # Check that frequency does not exceed Nyquist limit:
     if frequency > (ppd / 2):
         raise ValueError(
-            f"Grating frequency ({frequency}) should not exceed Nyquist limit {ppd/2} (ppd/2)"
+            f"Grating frequency ({frequency}) should not exceed Nyquist limit {ppd / 2} (ppd/2)"
         )
 
     # Accumulate edges of phases (rounding to avoid accumulation of
     # floating point imprecisions)
     edges = [*itertools.accumulate(itertools.repeat(phase_width, int(np.ceil(n_phases))))]
     edges = np.round(np.array(edges), 8)
     edges = list(edges)
```

### Comparing `stimupy-1.1.1/stimupy/logos.py` & `stimupy-1.1.2/stimupy/logos.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/noises/__init__.py` & `stimupy-1.1.2/stimupy/noises/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/noises/binaries.py` & `stimupy-1.1.2/stimupy/noises/binaries.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/noises/narrowbands.py` & `stimupy-1.1.2/stimupy/noises/narrowbands.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/noises/naturals.py` & `stimupy-1.1.2/stimupy/noises/naturals.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/noises/whites.py` & `stimupy-1.1.2/stimupy/noises/whites.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/RHS2007.py` & `stimupy-1.1.2/stimupy/papers/RHS2007.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/bindmann2004.py` & `stimupy-1.1.2/stimupy/papers/bindmann2004.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/domijan2015.py` & `stimupy-1.1.2/stimupy/papers/domijan2015.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/example.py` & `stimupy-1.1.2/stimupy/papers/example.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/modelfest.py` & `stimupy-1.1.2/stimupy/papers/modelfest.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/modelfest_data.csv` & `stimupy-1.1.2/stimupy/papers/modelfest_data.csv`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/modelfest_natural_scene.tif` & `stimupy-1.1.2/stimupy/papers/modelfest_natural_scene.tif`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/modelfest_noise.tif` & `stimupy-1.1.2/stimupy/papers/modelfest_noise.tif`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/murray2020.mat` & `stimupy-1.1.2/stimupy/papers/murray2020.mat`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/murray2020.py` & `stimupy-1.1.2/stimupy/papers/murray2020.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/white1981.py` & `stimupy-1.1.2/stimupy/papers/white1981.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/papers/white1985.py` & `stimupy-1.1.2/stimupy/papers/white1985.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/__init__.py` & `stimupy-1.1.2/stimupy/stimuli/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/benarys.py` & `stimupy-1.1.2/stimupy/stimuli/benarys.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/bullseyes.py` & `stimupy-1.1.2/stimupy/stimuli/bullseyes.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/checkerboards.py` & `stimupy-1.1.2/stimupy/stimuli/checkerboards.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/cornsweets.py` & `stimupy-1.1.2/stimupy/stimuli/cornsweets.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/cubes.py` & `stimupy-1.1.2/stimupy/stimuli/cubes.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/delboeufs.py` & `stimupy-1.1.2/stimupy/stimuli/delboeufs.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/dungeons.py` & `stimupy-1.1.2/stimupy/stimuli/dungeons.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/gabors.py` & `stimupy-1.1.2/stimupy/stimuli/gabors.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/gratings.py` & `stimupy-1.1.2/stimupy/stimuli/gratings.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     target_amount = target_phasea / 360.0
     target_shift = target_amount * cycle_px
     target_shifti = int(np.round(target_shift))
     target_phasei = target_shifti / cycle_px * 360
 
     if target_shift != int(target_shift):
         s = np.sign(target_phase_shift)
-        warnings.warn(f"Rounding phase; {target_phase_shift} -> {s*target_phasei}")
+        warnings.warn(f"Rounding phase; {target_phase_shift} -> {s * target_phasei}")
 
     # Shift targets by specified phase
     cy, cx = stim["shape"]
     if target_phase_shift < 0:
         if distance_metric == "horizontal":
             stim_target["img"][:, 0 : cx - target_shifti] = stim_target["img"][:, target_shifti::]
             stim_target["grating_mask"][:, 0 : cx - target_shifti] = stim_target["grating_mask"][
```

### Comparing `stimupy-1.1.1/stimupy/stimuli/hermanns.py` & `stimupy-1.1.2/stimupy/stimuli/hermanns.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/mondrians.py` & `stimupy-1.1.2/stimupy/stimuli/mondrians.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/mueller_lyers.py` & `stimupy-1.1.2/stimupy/stimuli/mueller_lyers.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/pinwheels.py` & `stimupy-1.1.2/stimupy/stimuli/pinwheels.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/plaids.py` & `stimupy-1.1.2/stimupy/stimuli/plaids.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/ponzos.py` & `stimupy-1.1.2/stimupy/stimuli/ponzos.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/rings.py` & `stimupy-1.1.2/stimupy/stimuli/rings.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/sbcs.py` & `stimupy-1.1.2/stimupy/stimuli/sbcs.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/todorovics.py` & `stimupy-1.1.2/stimupy/stimuli/todorovics.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/waves.py` & `stimupy-1.1.2/stimupy/stimuli/waves.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/wedding_cakes.py` & `stimupy-1.1.2/stimupy/stimuli/wedding_cakes.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/stimuli/whites.py` & `stimupy-1.1.2/stimupy/stimuli/whites.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/color_conversions.py` & `stimupy-1.1.2/stimupy/utils/color_conversions.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/contrast_conversions.py` & `stimupy-1.1.2/stimupy/utils/contrast_conversions.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/export.py` & `stimupy-1.1.2/stimupy/utils/export.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/filters.py` & `stimupy-1.1.2/stimupy/utils/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         raise ValueError("bandpass() missing argument 'bandwidth' which is not 'None'")
 
     # Resolve resolution
     shape, visual_size, ppd = resolution.resolve(shape=shape, visual_size=visual_size, ppd=ppd)
 
     if center_frequency > (min(ppd) / 2):
         raise ValueError(
-            f"Center frequency ({center_frequency}) should not exceed Nyquist limit {min(ppd)/2} (ppd/2)"
+            f"Center frequency ({center_frequency}) should not exceed Nyquist limit {min(ppd) / 2} (ppd/2)"
         )
 
     # Create frequency axes
     fy = np.fft.fftshift(np.fft.fftfreq(shape[0], d=1.0 / ppd[0]))
     fx = np.fft.fftshift(np.fft.fftfreq(shape[1], d=1.0 / ppd[1]))
     Fx, Fy = np.meshgrid(fx, fy)
```

### Comparing `stimupy-1.1.1/stimupy/utils/masks.py` & `stimupy-1.1.2/stimupy/utils/masks.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/pad.py` & `stimupy-1.1.2/stimupy/utils/pad.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/plotting.py` & `stimupy-1.1.2/stimupy/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/resolution.py` & `stimupy-1.1.2/stimupy/utils/resolution.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy/utils/utils.py` & `stimupy-1.1.2/stimupy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/stimupy.egg-info/PKG-INFO` & `stimupy-1.1.2/stimupy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimupy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Stimuli for vision science, as image arrays
 Author: Matko Matic, Guillermo Aguilar, Marianne Maertens
 Author-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 Maintainer-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

### Comparing `stimupy-1.1.1/stimupy.egg-info/SOURCES.txt` & `stimupy-1.1.2/stimupy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/tests/test_pad.py` & `stimupy-1.1.2/tests/test_pad.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/tests/test_resolve_resolutions.py` & `stimupy-1.1.2/tests/test_resolve_resolutions.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/tests/test_valid_resolution.py` & `stimupy-1.1.2/tests/test_valid_resolution.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/tests/test_validate_resolution_components.py` & `stimupy-1.1.2/tests/test_validate_resolution_components.py`

 * *Files identical despite different names*

### Comparing `stimupy-1.1.1/tests/test_waves.py` & `stimupy-1.1.2/tests/test_waves.py`

 * *Files identical despite different names*

