# Comparing `tmp/astro_ghost-2.1.4.tar.gz` & `tmp/astro_ghost-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.1.4.tar", last modified: Mon Apr 22 19:53:04 2024, max compression
+gzip compressed data, was "astro_ghost-2.1.5.tar", last modified: Mon Apr 22 20:29:17 2024, max compression
```

## Comparing `astro_ghost-2.1.4.tar` & `astro_ghost-2.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.289554 astro_ghost-2.1.4/
--rw-r--r--   0 alexgagliano   (501) staff       (20)       54 2024-04-22 19:34:11.000000 astro_ghost-2.1.4/.dockerignore
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.255287 astro_ghost-2.1.4/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.257573 astro_ghost-2.1.4/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      378 2023-08-14 00:02:43.000000 astro_ghost-2.1.4/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      535 2024-04-22 19:51:51.000000 astro_ghost-2.1.4/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      785 2024-04-22 19:34:11.000000 astro_ghost-2.1.4/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 19:53:04.289456 astro_ghost-2.1.4/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.1.4/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.284503 astro_ghost-2.1.4/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    22169 2024-04-22 19:51:56.000000 astro_ghost-2.1.4/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4678 2023-10-25 22:56:24.000000 astro_ghost-2.1.4/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    44662 2024-04-22 01:28:50.000000 astro_ghost-2.1.4/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.1.4/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.1.4/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.1.4/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.1.4/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2024-04-22 19:52:52.000000 astro_ghost-2.1.4/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.1.4/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39735 2024-03-28 23:23:31.000000 astro_ghost-2.1.4/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.1.4/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)  4279296 2023-10-25 21:44:38.000000 astro_ghost-2.1.4/astro_ghost/gwgc_good.csv
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.1.4/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    19117 2024-04-22 19:34:11.000000 astro_ghost-2.1.4/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9808 2023-07-03 22:17:51.000000 astro_ghost-2.1.4/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7867 2024-02-10 21:13:19.000000 astro_ghost-2.1.4/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.1.4/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.1.4/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.288482 astro_ghost-2.1.4/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1375 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      375 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2024-04-22 19:53:04.000000 astro_ghost-2.1.4/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.286079 astro_ghost-2.1.4/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.1.4/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.1.4/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.287182 astro_ghost-2.1.4/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.1.4/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.1.4/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.1.4/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.1.4/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      960 2024-04-22 19:34:11.000000 astro_ghost-2.1.4/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.1.4/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.1.4/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.1.4/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.287528 astro_ghost-2.1.4/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.1.4/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2024-04-22 19:53:04.289952 astro_ghost-2.1.4/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1857 2024-04-22 19:52:37.000000 astro_ghost-2.1.4/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 19:53:04.288155 astro_ghost-2.1.4/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2024-04-22 19:34:11.000000 astro_ghost-2.1.4/tests/Dockerfile
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.1.4/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.1.4/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.1.4/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4576 2024-02-10 23:04:40.000000 astro_ghost-2.1.4/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1393 2023-08-13 23:50:34.000000 astro_ghost-2.1.4/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.629201 astro_ghost-2.1.5/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       54 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.dockerignore
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.598475 astro_ghost-2.1.5/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.600456 astro_ghost-2.1.5/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      378 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      535 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      785 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 20:29:17.629130 astro_ghost-2.1.5/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.624405 astro_ghost-2.1.5/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    22169 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4678 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    44662 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2024-04-22 20:29:03.000000 astro_ghost-2.1.5/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    39735 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)  4279296 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/gwgc_good.csv
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    19117 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9808 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7867 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.628380 astro_ghost-2.1.5/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     5262 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1375 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      375 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2024-04-22 20:29:17.000000 astro_ghost-2.1.5/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.625905 astro_ghost-2.1.5/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.627233 astro_ghost-2.1.5/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      960 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.627553 astro_ghost-2.1.5/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2024-04-22 20:29:17.629589 astro_ghost-2.1.5/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1857 2024-04-22 20:28:58.000000 astro_ghost-2.1.5/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:29:17.628166 astro_ghost-2.1.5/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/Dockerfile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4576 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1393 2024-04-22 20:26:22.000000 astro_ghost-2.1.5/tox.ini
```

### Comparing `astro_ghost-2.1.4/.github/workflows/tests.yml` & `astro_ghost-2.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/.gitignore` & `astro_ghost-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/PKG-INFO` & `astro_ghost-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.1.4
+Version: 2.1.5
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.1.4/README.rst` & `astro_ghost-2.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/DLR.py` & `astro_ghost-2.1.5/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.1.5/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.1.5/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.1.5/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.1.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.1.5/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/conftest.py` & `astro_ghost-2.1.5/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.1.5/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/gradientAscent.py` & `astro_ghost-2.1.5/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/gwgc_good.csv` & `astro_ghost-2.1.5/astro_ghost/gwgc_good.csv`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/hostMatching.py` & `astro_ghost-2.1.5/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/photoz_helper.py` & `astro_ghost-2.1.5/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/sourceCleaning.py` & `astro_ghost-2.1.5/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/starSeparation.py` & `astro_ghost-2.1.5/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost/stellarLocus.py` & `astro_ghost-2.1.5/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.1.5/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.1.4
+Version: 2.1.5
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.1.4/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.1.5/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/Makefile` & `astro_ghost-2.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/conf.py` & `astro_ghost-2.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/index.rst` & `astro_ghost-2.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/make.bat` & `astro_ghost-2.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/source/associationmodules.rst` & `astro_ghost-2.1.5/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/source/basicusage.rst` & `astro_ghost-2.1.5/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/source/catalogmodules.rst` & `astro_ghost-2.1.5/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/source/installation.rst` & `astro_ghost-2.1.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/docs/source/preprocessingmodules.rst` & `astro_ghost-2.1.5/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/licenses/LICENSE.rst` & `astro_ghost-2.1.5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/setup.cfg` & `astro_ghost-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/setup.py` & `astro_ghost-2.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.1.4"
+version = "2.1.5"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.1.4/tests/debug.py` & `astro_ghost-2.1.5/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/tests/test_tutorial.py` & `astro_ghost-2.1.5/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.1.4/tox.ini` & `astro_ghost-2.1.5/tox.ini`

 * *Files identical despite different names*

