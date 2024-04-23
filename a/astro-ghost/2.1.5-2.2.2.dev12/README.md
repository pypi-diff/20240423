# Comparing `tmp/astro_ghost-2.1.5.tar.gz` & `tmp/astro_ghost-2.2.2.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.1.5.tar", last modified: Mon Apr 22 20:29:17 2024, max compression
+gzip compressed data, was "astro_ghost-2.2.2.dev12.tar", last modified: Tue Apr 23 00:57:21 2024, max compression
```

## Comparing `astro_ghost-2.1.5.tar` & `astro_ghost-2.2.2.dev12.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.629201 astro_ghost-2.1.5/
--rw-r--r--   0 alexgagliano   (501) staff       (20)       54 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.dockerignore
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.598475 astro_ghost-2.1.5/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.600456 astro_ghost-2.1.5/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      378 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      535 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      785 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 20:29:17.629130 astro_ghost-2.1.5/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.624405 astro_ghost-2.1.5/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    22169 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4678 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    44662 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2024-04-22 20:29:03.000000 astro_ghost-2.1.5/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39735 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)  4279296 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/gwgc_good.csv
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    19117 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9808 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7867 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.628380 astro_ghost-2.1.5/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1375 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      375 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.625905 astro_ghost-2.1.5/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.627233 astro_ghost-2.1.5/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      960 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.627553 astro_ghost-2.1.5/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2024-04-22 20:29:17.629589 astro_ghost-2.1.5/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1857 2024-04-22 20:28:58.000000 astro_ghost-2.1.5/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.628166 astro_ghost-2.1.5/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/Dockerfile
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4576 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1393 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tox.ini
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.105929 astro_ghost-2.2.2.dev12/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.dockerignore
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.056993 astro_ghost-2.2.2.dev12/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.063537 astro_ghost-2.2.2.dev12/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)      378 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.github/workflows/docs.yml
+-rw-r--r--   0 runner     (501) staff       (20)      910 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.github/workflows/release_to_pypi.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      535 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.github/workflows/tests.yml
+-rw-r--r--   0 runner     (501) staff       (20)      799 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      170 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/.readthedocs.yml
+-rw-r--r--   0 runner     (501) staff       (20)      341 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     4223 2024-04-23 00:57:21.106234 astro_ghost-2.2.2.dev12/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3662 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.096781 astro_ghost-2.2.2.dev12/astro_ghost/
+-rw-r--r--   0 runner     (501) staff       (20)    22169 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/DLR.py
+-rw-r--r--   0 runner     (501) staff       (20)     4678 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 runner     (501) staff       (20)    44662 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 runner     (501) staff       (20)     1296 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 runner     (501) staff       (20) 13643353 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 runner     (501) staff       (20)     1475 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 runner     (501) staff       (20)      112 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       28 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     1957 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/conftest.py
+-rw-r--r--   0 runner     (501) staff       (20)    39735 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 runner     (501) staff       (20)    32887 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/gradientAscent.py
+-rw-r--r--   0 runner     (501) staff       (20)  4279296 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/gwgc_good.csv
+-rw-r--r--   0 runner     (501) staff       (20)     2838 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/hostMatching.py
+-rw-r--r--   0 runner     (501) staff       (20)    18587 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/photoz_helper.py
+-rw-r--r--   0 runner     (501) staff       (20)     9808 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 runner     (501) staff       (20)     7867 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/starSeparation.py
+-rw-r--r--   0 runner     (501) staff       (20)     4610 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/stellarLocus.py
+-rw-r--r--   0 runner     (501) staff       (20)      302 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.099514 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4223 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1414 2024-04-23 00:57:21.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       18 2024-04-23 00:57:20.000000 astro_ghost-2.2.2.dev12/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.100987 astro_ghost-2.2.2.dev12/docs/
+-rw-r--r--   0 runner     (501) staff       (20)      634 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)     2545 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)     2641 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/make.bat
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.103640 astro_ghost-2.2.2.dev12/docs/source/
+-rw-r--r--   0 runner     (501) staff       (20)     1402 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/associationmodules.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2479 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/basicusage.rst
+-rw-r--r--   0 runner     (501) staff       (20)      819 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/catalogmodules.rst
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/detailedtutorials.rst
+-rw-r--r--   0 runner     (501) staff       (20)      960 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/installation.rst
+-rw-r--r--   0 runner     (501) staff       (20)      844 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 runner     (501) staff       (20)      320 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/supplementalmodules.rst
+-rw-r--r--   0 runner     (501) staff       (20)      268 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/docs/source/wrappermodules.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.104300 astro_ghost-2.2.2.dev12/licenses/
+-rw-r--r--   0 runner     (501) staff       (20)    37573 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/licenses/LICENSE.rst
+-rw-r--r--   0 runner     (501) staff       (20)      372 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/licenses/README.rst
+-rw-r--r--   0 runner     (501) staff       (20)      285 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1799 2024-04-23 00:57:21.107320 astro_ghost-2.2.2.dev12/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)       37 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 00:57:21.105644 astro_ghost-2.2.2.dev12/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      302 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tests/Dockerfile
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      648 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tests/debug.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tests/pytest.ini
+-rw-r--r--   0 runner     (501) staff       (20)     4576 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tests/test_tutorial.py
+-rw-r--r--   0 runner     (501) staff       (20)     1412 2024-04-23 00:57:08.000000 astro_ghost-2.2.2.dev12/tox.ini
```

### Comparing `astro_ghost-2.1.5/.github/workflows/tests.yml` & `astro_ghost-2.2.2.dev12/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/.gitignore` & `astro_ghost-2.2.2.dev12/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # Ignore .c files by default to avoid including generated code. If you want to
 # add a non-generated .c extension, use `git add -f filename.c`.
 *.c
 
 # Other generated files
 */version.py
+*/_version.py
 */cython_version.py
 htmlcov
 .coverage
 MANIFEST
 .ipynb_checkpoints
 
 # Sphinx
```

### Comparing `astro_ghost-2.1.5/README.rst` & `astro_ghost-2.2.2.dev12/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-*****
+"At the last dim horizon, we search among ghostly errors of observations for
+landmarks that are scarcely more substantial. The search will continue. The
+urge is older than history. It is not satisfied and it will not be oppressed."
+--Edwin Hubble
+
 GHOST
-*****
 -----------
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
 
 .. image:: https://img.shields.io/pypi/dm/astro-ghost
@@ -15,19 +18,14 @@
    :target: https://github.com/uiucsn/astro_ghost/actions/workflows/tests.yml
    :alt: Unit Tests
 
 .. image:: https://img.shields.io/readthedocs/uiucsnastro-ghost
    :target: https://uiucsnastro-ghost.readthedocs.io/en/latest/
    :alt: Read the Docs
 
-"At the last dim horizon, we search among ghostly errors of observations for
-landmarks that are scarcely more substantial. The search will continue. The
-urge is older than history. It is not satisfied and it will not be oppressed."
---Edwin Hubble
-
 Welcome to GHOST, the database for supernovae and their host galaxies. This
 database contains ~16k sources in PS1, which were used to predict supernova
 classes in Gagliano et al. (2020). Installation instructions for the analysis
 tools are below.
 
 Installation
 ------------
```

### Comparing `astro_ghost-2.1.5/astro_ghost/DLR.py` & `astro_ghost-2.2.2.dev12/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.2.2.dev12/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.2.2.dev12/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.2.2.dev12/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.2.2.dev12/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.2.2.dev12/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/conftest.py` & `astro_ghost-2.2.2.dev12/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.2.2.dev12/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/gradientAscent.py` & `astro_ghost-2.2.2.dev12/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/gwgc_good.csv` & `astro_ghost-2.2.2.dev12/astro_ghost/gwgc_good.csv`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/hostMatching.py` & `astro_ghost-2.2.2.dev12/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/photoz_helper.py` & `astro_ghost-2.2.2.dev12/astro_ghost/photoz_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,17 @@
-# from astropy.table import Table
-#import pkg_resources
-# import sys
-# import re
+import pkg_resources
 import numpy as np
-# import pylab
-# import json
 import requests
-# from astropy.io import fits
 from astro_ghost.PS1QueryFunctions import *
 
-# try: # Python 3.x
-#     from urllib.parse import quote as urlencode
-#     from urllib.request import urlretrieve
-#     import http.client as httplib
-# except ImportError:  # Python 2.x
-#     from urllib import pathname2url as urlencode
-#     from urllib import urlretrieve
-#     import httplib
-
 import pandas as pd
 import tensorflow as tf
-# from tensorflow import keras
 
-# from concurrent.futures import ThreadPoolExecutor
-# import asyncio
 import codecs
 
-# import time
 from sfdmap2 import sfdmap
 import os
 import tarfile
 
 DEFAULT_MODEL_PATH = './MLP_lupton.hdf5'
 DEFAULT_DUST_PATH = '.'
```

### Comparing `astro_ghost-2.1.5/astro_ghost/sourceCleaning.py` & `astro_ghost-2.2.2.dev12/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/starSeparation.py` & `astro_ghost-2.2.2.dev12/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost/stellarLocus.py` & `astro_ghost-2.2.2.dev12/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.2.2.dev12/astro_ghost.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/docs.yml
+.github/workflows/release_to_pypi.yaml
 .github/workflows/tests.yml
 astro_ghost/DLR.py
 astro_ghost/NEDQueryFunctions.py
 astro_ghost/PS1QueryFunctions.py
 astro_ghost/SimbadQueryFunctions.py
 astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
 astro_ghost/TNSQueryFunctions.py
```

### Comparing `astro_ghost-2.1.5/docs/Makefile` & `astro_ghost-2.2.2.dev12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/conf.py` & `astro_ghost-2.2.2.dev12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/index.rst` & `astro_ghost-2.2.2.dev12/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/make.bat` & `astro_ghost-2.2.2.dev12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/source/associationmodules.rst` & `astro_ghost-2.2.2.dev12/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/source/basicusage.rst` & `astro_ghost-2.2.2.dev12/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/source/catalogmodules.rst` & `astro_ghost-2.2.2.dev12/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/source/installation.rst` & `astro_ghost-2.2.2.dev12/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/docs/source/preprocessingmodules.rst` & `astro_ghost-2.2.2.dev12/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/licenses/LICENSE.rst` & `astro_ghost-2.2.2.dev12/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/setup.cfg` & `astro_ghost-2.2.2.dev12/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,47 @@
 author = Alexander Gagliano
 author_email = gaglian2@illinois.edu
 license = GNU GPL v3+
 license_file = licenses/LICENSE.rst
 url = http://astro-ghost.readthedocs.io
 description = Database of supernovae and the photometric and spectroscopic properties of their host galaxies
 long_description = file: README.rst
+classifiers = 
+	Programming Language :: Python :: 3
+	License :: OSI Approved :: MIT License
+	Operating System :: OS Independent
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.7
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	pytest
 	pandas
-	sklearn
+	scikit-learn<1.3.0
 	numpy
+	mastcasjobs
 	seaborn
 	matplotlib
 	joypy
 	photutils
 	scipy
 	datetime
 	requests
 	imblearn
 	rfpimp
 	Pillow
+	opencv-python
 	pyvo
 	astroquery
 	tensorflow
-	sfdmap
+	sfdmap2
+	importlib_resources
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
@@ -45,23 +52,27 @@
 	sphinx
 	sphinx-automodapi
 	sphinx-astropy
 	sphinx-rtd-theme
 	sphinx_toolbox
 	sphinx_copybutton
 
-[options.package_data]
-astro_ghost = data/*
-
 [tool:pytest]
 testpaths = "astro_ghost" "docs" "tests"
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
 
+[options.package_data]
+astro_ghost = 
+	data/*
+	Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+	tonry_ps1_locus.txt
+	gwgc_good.csv
+
 [coverage:run]
 omit = 
 	astro_ghost/__init*
 	astro_ghost/conftest.py
 	astro_ghost/*setup_package*
 	astro_ghost/extern/*
 	astro_ghost/version*
```

### Comparing `astro_ghost-2.1.5/tests/debug.py` & `astro_ghost-2.2.2.dev12/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/tests/test_tutorial.py` & `astro_ghost-2.2.2.dev12/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.5/tox.ini` & `astro_ghost-2.2.2.dev12/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     run tests
 
 deps =
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     docs
+    setuptools_scm
     alldeps: all
 
 commands =
     pip freeze
     pytest --cov=astro_ghost {toxinidir}/tests
     #pytest --pyargs astro_ghost {toxinidir}/docs --cov astro_ghost --cov-config={toxinidir}/setup.cfg {posargs}
```

