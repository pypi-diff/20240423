# Comparing `tmp/BubbleDet-1.0.0.tar.gz` & `tmp/bubbledet-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BubbleDet-1.0.0.tar", last modified: Wed Aug 30 22:44:16 2023, max compression
+gzip compressed data, was "bubbledet-1.0.7.tar", last modified: Tue Apr 23 09:49:26 2024, max compression
```

## Comparing `BubbleDet-1.0.0.tar` & `bubbledet-1.0.7.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.678898 BubbleDet-1.0.0/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      112 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/.gitignore
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      223 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/.readthedocs.yaml
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      650 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/CHANGELOG.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1106 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/LICENSE
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2634 2023-08-30 22:44:16.678898 BubbleDet-1.0.0/PKG-INFO
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2058 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/README.rst
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.666897 BubbleDet-1.0.0/docs/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      586 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/Makefile
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      787 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/make.bat
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.670897 BubbleDet-1.0.0/docs/source/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      177 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/bubbledet.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)       33 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/changelog.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      293 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/collected_examples.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     6230 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/conf.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      276 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/contact.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      574 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/development.rst
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.670897 BubbleDet-1.0.0/docs/source/examples/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      168 2023-08-10 20:47:06.000000 BubbleDet-1.0.0/docs/source/examples/analogue.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      165 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/examples/first_example.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      152 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/source/examples/kink.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      173 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/source/examples/symmetry_breaking.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      169 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/source/examples/thermal.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      162 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/source/examples/thinwall.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      167 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/docs/source/examples/unbounded.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2250 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/first_example.rst
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.670897 BubbleDet-1.0.0/docs/source/images/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     4649 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/images/bubbledet.svg
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    17010 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/images/bubbles.jpg
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    14418 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/images/components.svg
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    15406 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/images/favicon.ico
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    24793 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/docs/source/images/potential.svg
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      733 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/index.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1045 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/installation.rst
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1580 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/docs/source/intro.rst
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.674898 BubbleDet-1.0.0/examples/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)        0 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/examples/__init__.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1809 2023-08-29 17:41:39.000000 BubbleDet-1.0.0/examples/analogue.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     4401 2023-08-30 08:25:51.000000 BubbleDet-1.0.0/examples/derivative_expansion.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     3099 2023-08-30 13:51:43.000000 BubbleDet-1.0.0/examples/extrapolations.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1532 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/examples/first_example.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2870 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/examples/kink.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     3207 2023-08-30 13:51:43.000000 BubbleDet-1.0.0/examples/symmetry_breaking.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     3777 2023-08-29 20:46:11.000000 BubbleDet-1.0.0/examples/thermal.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     5318 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/examples/thinwall.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2032 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/examples/unbounded.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     5065 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/examples/wkb.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1052 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/pyproject.toml
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)       38 2023-08-30 22:44:16.678898 BubbleDet-1.0.0/setup.cfg
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)       69 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/setup.py
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.666897 BubbleDet-1.0.0/src/
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.674898 BubbleDet-1.0.0/src/BubbleDet/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)       93 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/src/BubbleDet/__init__.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     8751 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/src/BubbleDet/configs.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2838 2023-08-30 13:51:43.000000 BubbleDet-1.0.0/src/BubbleDet/derivative_expansion.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    41614 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/src/BubbleDet/determinant.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    17449 2023-08-30 13:51:43.000000 BubbleDet-1.0.0/src/BubbleDet/extrapolation.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     5207 2023-08-29 13:02:23.000000 BubbleDet-1.0.0/src/BubbleDet/gelfand_yaglom.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2066 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/src/BubbleDet/group_volumes.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2055 2023-08-29 10:47:10.000000 BubbleDet-1.0.0/src/BubbleDet/helpers.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     5935 2023-08-29 15:09:13.000000 BubbleDet-1.0.0/src/BubbleDet/laplacian.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     3330 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/src/BubbleDet/negative_eigenvalue.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)    11354 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/src/BubbleDet/phi_infinity.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2517 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/src/BubbleDet/renormalisation.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     9577 2023-08-30 22:44:00.000000 BubbleDet-1.0.0/src/BubbleDet/wkb.py
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.674898 BubbleDet-1.0.0/src/BubbleDet.egg-info/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2634 2023-08-30 22:44:16.000000 BubbleDet-1.0.0/src/BubbleDet.egg-info/PKG-INFO
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     2053 2023-08-30 22:44:16.000000 BubbleDet-1.0.0/src/BubbleDet.egg-info/SOURCES.txt
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)        1 2023-08-30 22:44:16.000000 BubbleDet-1.0.0/src/BubbleDet.egg-info/dependency_links.txt
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      182 2023-08-30 22:44:16.000000 BubbleDet-1.0.0/src/BubbleDet.egg-info/requires.txt
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)       10 2023-08-30 22:44:16.000000 BubbleDet-1.0.0/src/BubbleDet.egg-info/top_level.txt
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.678898 BubbleDet-1.0.0/tests/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)        0 2022-06-30 20:29:32.000000 BubbleDet-1.0.0/tests/__init__.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     3588 2023-08-28 11:34:15.000000 BubbleDet-1.0.0/tests/conftest.py
-drwxrwxr-x   0 ppzolg    (1000) ppzolg    (1000)        0 2023-08-30 22:44:16.678898 BubbleDet-1.0.0/tests/data/
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1764 2022-10-17 10:45:04.000000 BubbleDet-1.0.0/tests/data/baacke_lavrelashvili_table1
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      118 2022-10-17 10:45:04.000000 BubbleDet-1.0.0/tests/data/dunne_min_fig5
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      325 2022-10-17 10:45:04.000000 BubbleDet-1.0.0/tests/data/dunne_min_fig6_alpha0.01
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      324 2022-10-17 10:45:04.000000 BubbleDet-1.0.0/tests/data/dunne_min_fig6_alpha0.7
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      322 2022-10-17 10:45:04.000000 BubbleDet-1.0.0/tests/data/dunne_min_fig6_alpha0.9
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1812 2023-07-06 15:13:20.000000 BubbleDet-1.0.0/tests/data/ekstedt_fits.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)      560 2023-08-29 13:02:24.000000 BubbleDet-1.0.0/tests/data/scaleless_results.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1963 2023-08-29 15:09:13.000000 BubbleDet-1.0.0/tests/test_derivative_expansion.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     5316 2023-08-29 17:04:06.000000 BubbleDet-1.0.0/tests/test_determinant.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1578 2023-08-30 08:42:39.000000 BubbleDet-1.0.0/tests/test_extrapolation.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1260 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/tests/test_gelfand_yaglom.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1747 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/tests/test_negative_eigenvalue.py
--rw-rw-r--   0 ppzolg    (1000) ppzolg    (1000)     1132 2023-08-21 12:13:58.000000 BubbleDet-1.0.0/tests/test_phi_infinity.py
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.851586 bubbledet-1.0.7/
+-rw-r--r--   0 ogould     (502) staff       (20)      112 2024-01-20 09:00:15.000000 bubbledet-1.0.7/.gitignore
+-rw-r--r--   0 ogould     (502) staff       (20)      223 2024-01-20 09:00:15.000000 bubbledet-1.0.7/.readthedocs.yaml
+-rw-r--r--   0 ogould     (502) staff       (20)      650 2024-01-20 09:00:15.000000 bubbledet-1.0.7/CHANGELOG.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     1106 2024-01-20 09:00:15.000000 bubbledet-1.0.7/LICENSE
+-rw-r--r--   0 ogould     (502) staff       (20)     3265 2024-04-23 09:49:26.850278 bubbledet-1.0.7/PKG-INFO
+-rw-r--r--   0 ogould     (502) staff       (20)     2202 2024-01-20 09:00:15.000000 bubbledet-1.0.7/README.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      479 2024-01-20 09:00:15.000000 bubbledet-1.0.7/bitbucket-pipelines.yml
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.750133 bubbledet-1.0.7/docs/
+-rw-r--r--   0 ogould     (502) staff       (20)      586 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/Makefile
+-rw-r--r--   0 ogould     (502) staff       (20)      787 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/make.bat
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.770268 bubbledet-1.0.7/docs/source/
+-rw-r--r--   0 ogould     (502) staff       (20)      177 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/bubbledet.rst
+-rw-r--r--   0 ogould     (502) staff       (20)       33 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/changelog.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      293 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/collected_examples.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     6390 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/conf.py
+-rw-r--r--   0 ogould     (502) staff       (20)      276 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/contact.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      574 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/development.rst
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.779614 bubbledet-1.0.7/docs/source/examples/
+-rw-r--r--   0 ogould     (502) staff       (20)      168 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/analogue.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      165 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/first_example.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      152 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/kink.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      173 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/symmetry_breaking.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      169 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/thermal.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      162 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/thinwall.rst
+-rw-r--r--   0 ogould     (502) staff       (20)      167 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/examples/unbounded.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     2512 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/faq.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     2250 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/first_example.rst
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.787237 bubbledet-1.0.7/docs/source/images/
+-rw-r--r--   0 ogould     (502) staff       (20)     4649 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/images/bubbledet.svg
+-rw-r--r--   0 ogould     (502) staff       (20)    17010 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/images/bubbles.jpg
+-rw-r--r--   0 ogould     (502) staff       (20)    14418 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/images/components.svg
+-rw-r--r--   0 ogould     (502) staff       (20)    15406 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/images/favicon.ico
+-rw-r--r--   0 ogould     (502) staff       (20)    24793 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/images/potential.svg
+-rw-r--r--   0 ogould     (502) staff       (20)      807 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/index.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     1045 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/installation.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     1682 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/intro.rst
+-rw-r--r--   0 ogould     (502) staff       (20)     2193 2024-01-20 09:00:15.000000 bubbledet-1.0.7/docs/source/refs.bib
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.805471 bubbledet-1.0.7/examples/
+-rw-r--r--   0 ogould     (502) staff       (20)        0 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/__init__.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1809 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/analogue.py
+-rw-r--r--   0 ogould     (502) staff       (20)     4401 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/derivative_expansion.py
+-rw-r--r--   0 ogould     (502) staff       (20)     3099 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/extrapolations.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1532 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/first_example.py
+-rw-r--r--   0 ogould     (502) staff       (20)     2870 2024-04-23 08:34:41.000000 bubbledet-1.0.7/examples/kink.py
+-rw-r--r--   0 ogould     (502) staff       (20)     3207 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/symmetry_breaking.py
+-rw-r--r--   0 ogould     (502) staff       (20)     4040 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/thermal.py
+-rw-r--r--   0 ogould     (502) staff       (20)     5318 2024-04-23 08:34:24.000000 bubbledet-1.0.7/examples/thinwall.py
+-rw-r--r--   0 ogould     (502) staff       (20)     2032 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/unbounded.py
+-rw-r--r--   0 ogould     (502) staff       (20)     5065 2024-01-20 09:00:15.000000 bubbledet-1.0.7/examples/wkb.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1080 2024-01-20 09:00:15.000000 bubbledet-1.0.7/pyproject.toml
+-rw-r--r--   0 ogould     (502) staff       (20)       38 2024-04-23 09:49:26.851662 bubbledet-1.0.7/setup.cfg
+-rw-r--r--   0 ogould     (502) staff       (20)       69 2024-01-20 09:00:15.000000 bubbledet-1.0.7/setup.py
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.732117 bubbledet-1.0.7/src/
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.827668 bubbledet-1.0.7/src/BubbleDet/
+-rw-r--r--   0 ogould     (502) staff       (20)       93 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/__init__.py
+-rw-r--r--   0 ogould     (502) staff       (20)     8903 2024-04-23 09:48:53.000000 bubbledet-1.0.7/src/BubbleDet/configs.py
+-rw-r--r--   0 ogould     (502) staff       (20)     3110 2024-04-23 09:48:53.000000 bubbledet-1.0.7/src/BubbleDet/derivative_expansion.py
+-rw-r--r--   0 ogould     (502) staff       (20)    41614 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/determinant.py
+-rw-r--r--   0 ogould     (502) staff       (20)    17449 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/extrapolation.py
+-rw-r--r--   0 ogould     (502) staff       (20)     5207 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/gelfand_yaglom.py
+-rw-r--r--   0 ogould     (502) staff       (20)     2066 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/group_volumes.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1559 2024-04-23 09:48:53.000000 bubbledet-1.0.7/src/BubbleDet/helpers.py
+-rw-r--r--   0 ogould     (502) staff       (20)     5935 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/laplacian.py
+-rw-r--r--   0 ogould     (502) staff       (20)     3330 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/negative_eigenvalue.py
+-rw-r--r--   0 ogould     (502) staff       (20)    11354 2024-01-20 09:00:15.000000 bubbledet-1.0.7/src/BubbleDet/phi_infinity.py
+-rw-r--r--   0 ogould     (502) staff       (20)     2615 2024-04-23 09:48:53.000000 bubbledet-1.0.7/src/BubbleDet/renormalisation.py
+-rw-r--r--   0 ogould     (502) staff       (20)     9652 2024-04-23 09:48:53.000000 bubbledet-1.0.7/src/BubbleDet/wkb.py
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.848606 bubbledet-1.0.7/src/BubbleDet.egg-info/
+-rw-r--r--   0 ogould     (502) staff       (20)     3265 2024-04-23 09:49:26.000000 bubbledet-1.0.7/src/BubbleDet.egg-info/PKG-INFO
+-rw-r--r--   0 ogould     (502) staff       (20)     2118 2024-04-23 09:49:26.000000 bubbledet-1.0.7/src/BubbleDet.egg-info/SOURCES.txt
+-rw-r--r--   0 ogould     (502) staff       (20)        1 2024-04-23 09:49:26.000000 bubbledet-1.0.7/src/BubbleDet.egg-info/dependency_links.txt
+-rw-r--r--   0 ogould     (502) staff       (20)      203 2024-04-23 09:49:26.000000 bubbledet-1.0.7/src/BubbleDet.egg-info/requires.txt
+-rw-r--r--   0 ogould     (502) staff       (20)       10 2024-04-23 09:49:26.000000 bubbledet-1.0.7/src/BubbleDet.egg-info/top_level.txt
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.840460 bubbledet-1.0.7/tests/
+-rw-r--r--   0 ogould     (502) staff       (20)        0 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/__init__.py
+-rw-r--r--   0 ogould     (502) staff       (20)     3588 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/conftest.py
+drwxr-xr-x   0 ogould     (502) staff       (20)        0 2024-04-23 09:49:26.845558 bubbledet-1.0.7/tests/data/
+-rw-r--r--   0 ogould     (502) staff       (20)     1764 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/baacke_lavrelashvili_table1
+-rw-r--r--   0 ogould     (502) staff       (20)      118 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/dunne_min_fig5
+-rw-r--r--   0 ogould     (502) staff       (20)      325 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/dunne_min_fig6_alpha0.01
+-rw-r--r--   0 ogould     (502) staff       (20)      324 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/dunne_min_fig6_alpha0.7
+-rw-r--r--   0 ogould     (502) staff       (20)      322 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/dunne_min_fig6_alpha0.9
+-rw-r--r--   0 ogould     (502) staff       (20)     1812 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/ekstedt_fits.py
+-rw-r--r--   0 ogould     (502) staff       (20)      560 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/data/scaleless_results.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1899 2024-04-23 09:48:53.000000 bubbledet-1.0.7/tests/test_derivative_expansion.py
+-rw-r--r--   0 ogould     (502) staff       (20)     5100 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/test_determinant.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1578 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/test_extrapolation.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1260 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/test_gelfand_yaglom.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1747 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/test_negative_eigenvalue.py
+-rw-r--r--   0 ogould     (502) staff       (20)     1132 2024-01-20 09:00:15.000000 bubbledet-1.0.7/tests/test_phi_infinity.py
```

### Comparing `BubbleDet-1.0.0/CHANGELOG.rst` & `bubbledet-1.0.7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/LICENSE` & `bubbledet-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/PKG-INFO` & `bubbledet-1.0.7/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1
-Name: BubbleDet
-Version: 1.0.0
-Summary: A package for computing functional determinants
-Author-email: Andreas Ekstedt <andreas.ekstedt@desy.de>, Oliver Gould <oliver.gould@nottingham.ac.uk>, Joonas Hirvonen <joonas.o.hirvonen@helsinki.fi>
-License: MIT
-Project-URL: Homepage, https://bubbledet.readthedocs.io/
-Project-URL: Repository, https://bitbucket.org/og113/bubbledet/
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 ===========================================
 BubbleDet
 ===========================================
 
 Computes the one-loop functional determinant entering the bubble nucleation
 rate, or vacuum decay rate.
 
 |
 
 Documentation
 ===========================================
-For complete documentation, see the
-`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_.
+For complete package documentation, see the
+`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_. For more information
+about the mathematics behind BubbleDet, see the accompanying paper on
+`arXiv <https://arxiv.org/abs/2308.15652>`_.
 
 |
 
 
 Requirements
 ===========================================
```

### Comparing `BubbleDet-1.0.0/README.rst` & `bubbledet-1.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,49 @@
+Metadata-Version: 2.1
+Name: BubbleDet
+Version: 1.0.7
+Summary: A package for computing functional determinants
+Author-email: Andreas Ekstedt <andreas.ekstedt@desy.de>, Oliver Gould <oliver.gould@nottingham.ac.uk>, Joonas Hirvonen <joonas.o.hirvonen@helsinki.fi>
+License: MIT
+Project-URL: Homepage, https://bubbledet.readthedocs.io/
+Project-URL: Repository, https://bitbucket.org/og113/bubbledet/
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: cosmoTransitions>=2.0.6
+Requires-Dist: findiff>=0.9.2
+Requires-Dist: numpy>=1.21.5
+Requires-Dist: packaging>=21.3
+Requires-Dist: scipy>=1.8.0
+Provides-Extra: tests
+Requires-Dist: pytest>=7.2.2; extra == "tests"
+Requires-Dist: matplotlib>=3.5.1; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: graphviz; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-automodapi; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+
 ===========================================
 BubbleDet
 ===========================================
 
 Computes the one-loop functional determinant entering the bubble nucleation
 rate, or vacuum decay rate.
 
 |
 
 Documentation
 ===========================================
-For complete documentation, see the
-`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_.
+For complete package documentation, see the
+`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_. For more information
+about the mathematics behind BubbleDet, see the accompanying paper on
+`arXiv <https://arxiv.org/abs/2308.15652>`_.
 
 |
 
 
 Requirements
 ===========================================
```

### Comparing `BubbleDet-1.0.0/docs/Makefile` & `bubbledet-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/make.bat` & `bubbledet-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/conf.py` & `bubbledet-1.0.7/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,25 +45,30 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
 #    'sphinx.ext.autodoc',
 #    'sphinx.ext.autosummary',
     'sphinx_automodapi.automodapi',
     'sphinx_automodapi.smart_resolver',
+    'sphinxcontrib.bibtex',
+    "sphinx.ext.intersphinx", # links to other pages within docs
     'sphinx.ext.napoleon', # for numpy style docs
     'sphinx.ext.doctest', # test code snippets in docs
     'sphinx.ext.coverage', # collect doc coverage stats
     'sphinx.ext.mathjax', # support for mathjax
     'sphinx.ext.ifconfig', # if statements for including content
     'sphinx.ext.viewcode', # add links to highlighted source code
 ]
 #numpydoc_show_class_members = False # automodapi
 #autosummary_generate = True
 automodapi_inheritance_diagram = False
 
+# Options for sphinxcontrib.bibtex
+bibtex_bibfiles = ['refs.bib']
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
```

### Comparing `BubbleDet-1.0.0/docs/source/development.rst` & `bubbledet-1.0.7/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/first_example.rst` & `bubbledet-1.0.7/docs/source/first_example.rst`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/images/bubbledet.svg` & `bubbledet-1.0.7/docs/source/images/bubbledet.svg`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/images/bubbles.jpg` & `bubbledet-1.0.7/docs/source/images/bubbles.jpg`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/images/components.svg` & `bubbledet-1.0.7/docs/source/images/components.svg`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/images/favicon.ico` & `bubbledet-1.0.7/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/images/potential.svg` & `bubbledet-1.0.7/docs/source/images/potential.svg`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/installation.rst` & `bubbledet-1.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/docs/source/intro.rst` & `bubbledet-1.0.7/docs/source/intro.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 .. image:: images/potential.svg
     :width: 300
     :align: center
     :alt: Potential with metastable and stable minima
 
 then the decay rate,
-:math:`\Gamma`, is given by
+:math:`\Gamma`, is given by\ :footcite:p:`Callan:1977pt`
 
 .. math::
   \Gamma = \underbrace{\left( \frac{S[\phi_\text{b}]}{2\pi} \right)^{d/2}
   \left(\frac{\vert\det ' (- \Box + V''(\phi_\text{b}))\vert}{\det (- \Box + V''(\phi_\text{F}))}
   \right)^{-1/2}}_\text{prefactor}
   e^{-\left(S[\phi_\text{b}] - S[\phi_\text{F}]\right)} .
 
@@ -30,11 +30,19 @@
 and :math:`\phi_\text{F}` is the homogeneous metastable phase, or false vacuum.
 BubbleDet can compute the prefactor term highlighted above. BubbleDet is applicable for
 arbitrary potentials, and in any dimension up to seven. It can also compute
 multi-particle functional determinants, which arise for example in
 symmetry-breaking transitions.
 There are several packages which focus on the computation of the exponential
 factor in the nucleation rate, such as
-`CosmoTransitions <https://clwainwright.net/CosmoTransitions/>`_.
+CosmoTransitions\ :footcite:p:`Wainwright:2011kj`.
 
-For further details of the physics and mathematics behind BubbleDet, see
-`BubbleDet: A Python package to compute functional determinants for bubble nucleation <https://arxiv.org/>`_.
+For further details of the physics and mathematics behind BubbleDet, see the
+acommpanying paper,
+BubbleDet: A Python package to compute functional determinants for bubble
+nucleation\ :footcite:p:`Ekstedt:2023sqc`.
+
+**********
+References
+**********
+
+.. footbibliography::
```

### Comparing `BubbleDet-1.0.0/examples/analogue.py` & `bubbledet-1.0.7/examples/analogue.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/derivative_expansion.py` & `bubbledet-1.0.7/examples/derivative_expansion.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/extrapolations.py` & `bubbledet-1.0.7/examples/extrapolations.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/first_example.py` & `bubbledet-1.0.7/examples/first_example.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/kink.py` & `bubbledet-1.0.7/examples/kink.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/symmetry_breaking.py` & `bubbledet-1.0.7/examples/symmetry_breaking.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/thermal.py` & `bubbledet-1.0.7/examples/thermal.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,49 +24,45 @@
 lam = 0.1
 mf = -0.2
 y = 0.3
 
 # dimensional reduction relations at leading order
 def params_3d(T):
     return {
-        "s3": (s + 1 / 24 * (g + 4 * y * mf) * T ** 2) / np.sqrt(T),
-        "m3sq": msq + 1 / 24 * (lam + 4 * y ** 2) * T ** 2,
+        "s3": (s + 1 / 24 * (g + 4 * y * mf) * T**2) / np.sqrt(T),
+        "m3sq": msq + 1 / 24 * (lam + 4 * y**2) * T**2,
         "g3": np.sqrt(T) * g,
-        "lam3": T * lam
+        "lam3": T * lam,
     }
 
 
 # potential and its derivatives
 def VT(x, T):
     p = params_3d(T)
     return (
         p["s3"] * x
-        + 1 / 2 * p["m3sq"] * x ** 2
-        + 1 / 6 * p["g3"] * x ** 3
-        + 1 / 24 * p["lam3"] * x ** 4
+        + 1 / 2 * p["m3sq"] * x**2
+        + 1 / 6 * p["g3"] * x**3
+        + 1 / 24 * p["lam3"] * x**4
     )
 
 
 def dVT(x, T):
     p = params_3d(T)
     return (
         p["s3"]
         + p["m3sq"] * x
-        + 1 / 2 * p["g3"] * x ** 2
-        + 1 / 6 * p["lam3"] * x ** 3
+        + 1 / 2 * p["g3"] * x**2
+        + 1 / 6 * p["lam3"] * x**3
     )
 
 
 def ddVT(x, T):
     p = params_3d(T)
-    return (
-        + p["m3sq"]
-        + p["g3"] * x
-        + 1 / 2 * p["lam3"] * x ** 2
-    )
+    return +p["m3sq"] + p["g3"] * x + 1 / 2 * p["lam3"] * x**2
 
 
 # minima
 def minima(T):
     p = params_3d(T)
     # soliving for cubic roots with np
     cubic = np.polynomial.polynomial.Polynomial(
@@ -82,15 +78,15 @@
     elif len(x0_real) == 3:
         # order solutions based on potential
         return x0_real[np.argsort(VT(x0_real, T))]
     else:
         raise ValueError("Neither 1 nor 3 real solutions")
 
 
-print("%-12s %-12s %-12s %-12s" % ("T", "S0", "-log(A/T^4)", "-log(rate)"))
+print(f"{'T':<12} {'S0':<12} {'-log(A/T^4)':<12} {'-log(rate/T^4)':<12}")
 
 # running over temperatures
 T_max = 8.4
 T_min = 7.9
 nT = 50 + 1
 
 for T in np.linspace(T_max, T_min, num=nT):
@@ -129,24 +125,28 @@
         W_Phi=ddV,
         spin=0,
         dof_internal=1,
         zero_modes="Higgs",
     )
 
     # creating bubble determinant instance
-    bub_det = BubbleDeterminant(
-        bub_config, higgs, thermal=True
-    )
+    bub_det = BubbleDeterminant(bub_config, higgs, thermal=True)
 
-    # full one-loop correction
+    # full one-loop correction, including the dynamical part of the rate
+    # S1=-log(A) where A is the one-loop prefactor
+    # as in equation (1) of arXiv:2308.15652
     S1, S1_err = bub_det.findDeterminant()
 
     # dynamical part assuming that damping is negligible
+    # separately computing this, just to show how it could be done
+    # note that A_dyn is already included in S1
     eig_neg, eig_neg_err = bub_det.findNegativeEigenvalue()
-    dynamical_prefactor = np.sqrt(abs(eig_neg)) / (2 * np.pi)
+    A_dyn = np.sqrt(abs(eig_neg)) / (2 * np.pi)
 
-    minusLogAOnT4 = S1 + 4 * np.log(T)
+    # -log(A/T^4), dividing out T^4 just to fix units
+    minus_log_A_T4 = S1 + 4 * np.log(T)
 
-    minusLogRate = S0 + minusLogAOnT4
+    # -log(rate/T^4)
+    minus_log_rate_T4 = S0 + S1 + 4 * np.log(T)
 
     # printing results
-    print("%-12g %-12g %-12g %-12g" % (T, S0, minusLogAOnT4, minusLogRate))
+    print(f"{T:<12g} {S0:<12g} {minus_log_A_T4:<12g} {minus_log_rate_T4:<12g}")
```

### Comparing `BubbleDet-1.0.0/examples/thinwall.py` & `bubbledet-1.0.7/examples/thinwall.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/unbounded.py` & `bubbledet-1.0.7/examples/unbounded.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/examples/wkb.py` & `bubbledet-1.0.7/examples/wkb.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/pyproject.toml` & `bubbledet-1.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,12 +33,13 @@
     "matplotlib>=3.5.1",
 ]
 docs = [
     "graphviz",
     "sphinx",
     "sphinx-rtd-theme",
     "sphinx-automodapi",
+    "sphinxcontrib-bibtex",
 ]
 
 [project.urls]
 Homepage = "https://bubbledet.readthedocs.io/"
 Repository = "https://bitbucket.org/og113/bubbledet/"
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet/configs.py` & `bubbledet-1.0.7/src/BubbleDet/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,14 +244,19 @@
         self.W_inf = self.W_Phi(self.phi_metaMin)
         self.Delta_W = self.W - self.W_inf
         self.Delta_W_interp = interpolate.interp1d(
             self.R, self.Delta_W, kind="cubic"
         )
         self.m_W_meta = np.sqrt(self.W_Phi(self.phi_metaMin))
         self.m_max = np.sqrt(max(max(self.W), self.m_Higgs_meta**2))
+        self.massless_meta = (
+            self.m_max == 0.0
+            or self.m_max == 0
+            or self.m_W_meta / self.m_max < 1e-15
+        )
 
         # setting renormalisation scale
         if renormalisation_scale is None:
             if bubble.m_Higgs_meta > 0:
                 self.renormalisation_scale = bubble.m_Higgs_meta
             else:
                 self.renormalisation_scale = 1
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet/derivative_expansion.py` & `bubbledet-1.0.7/src/BubbleDet/derivative_expansion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import numpy as np  # arrays and maths
 from scipy.special import gamma # special functions
-from .helpers import simpson # integrator
 from cosmoTransitions.helper_functions import deriv14  # derivatives for arrays
+try:
+    from scipy.integrate import simpson
+except ImportError:
+    # scipy.version < 1.6
+    from scipy.integrate import simps as simpson
 
 
 def findDerivativeExpansion(config, NLO=False):
     r"""Derivative expansion of determinant
 
     Full docs in BubbleDet.py.
     """
     if config.zero_modes.lower() != "none":
         raise ValueError("Derivative expansion requires absence of zero modes")
     d = config.dim
     R = config.R
     mu = config.renormalisation_scale
     angles = 2 * np.pi ** (d / 2) / gamma(d / 2)
     measure = angles * R ** (d - 1)
-    offset =  2e-16 / R[-1] ** 2 # to prevent 1/0
+    offset = 2e-16 / R[-1] ** 2  # to prevent 1/0
     W_offset = config.W + offset
     W_inf_offset = config.W_inf + offset
 
     # constructing integrand at LO
     if d % 2 == 0:  # even dimensions
         n = d // 2
         prefactor = -1 / 2 * (-1) ** n / gamma(n + 1) / (4 * np.pi) ** (d / 2)
@@ -34,24 +38,26 @@
                 np.log(mu**2 / W_inf_offset) + harmonic + eps_term
             )
         )
     else:  # odd dimensions
         prefactor = -1 / 2 * gamma(-d / 2) / (4 * np.pi) ** (d / 2)
         integrand = prefactor * (config.W ** (d / 2) - config.W_inf ** (d / 2))
     if config.spin == 1:
-        integrand *= (d - 1) # massive vector degrees of freedom
+        integrand *= (d - 1)  # massive vector degrees of freedom
     # integrating
     integrand *= measure
     S1 = simpson(integrand, x=R)
     S1_half = simpson(integrand[::2], x=R[::2])
     S1_err = abs(S1 - S1_half) / 7
 
     if NLO:
-        if d == 2:
-            raise ValueError("Derivative expansion diverges at NLO in d=2")
+        if d == 2 and config.massless_meta:
+            raise ValueError(
+                "Derivative expansion for scale shifters diverges at NLO in d=2"
+            )
         # constructing integrand at NLO
         integrand = deriv14(config.W, R) ** 2 * W_offset ** (d / 2 - 3)
         integrand *= 1 / (4 * np.pi) ** (d / 2)
         if d % 2 == 0 and d > 5:  # even dimensions
             n = d // 2
             harmonic = np.sum([1 / h for h in range(1, (n - 3) + 1)])
             eps_term = - 2 / (d - 1) if config.spin == 1 else 0
@@ -65,9 +71,13 @@
         integrand *= measure
         S1_NLO = simpson(integrand, x=R)
         S1_NLO_half = simpson(integrand[::2], x=R[::2])
         S1_NLO_err = abs(S1_NLO - S1_NLO_half) / 7
         S1 += S1_NLO
         S1_err += S1_NLO_err
 
+    # multiplying by internal dof
+    S1 *= config.dof_internal
+    S1_err *= config.dof_internal
+
     # returning result
     return S1, S1_err
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet/determinant.py` & `bubbledet-1.0.7/src/BubbleDet/determinant.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/extrapolation.py` & `bubbledet-1.0.7/src/BubbleDet/extrapolation.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/gelfand_yaglom.py` & `bubbledet-1.0.7/src/BubbleDet/gelfand_yaglom.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/group_volumes.py` & `bubbledet-1.0.7/src/BubbleDet/group_volumes.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/helpers.py` & `bubbledet-1.0.7/src/BubbleDet/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # helper functions for BubbleDet
 import findiff
-from importlib import metadata
-from packaging import version
-from scipy.integrate import simps  # integrator
 
 
 def derivative(f, x, dx=1.0, n=1, order=4, scheme="center"):
     r"""Computes numerical derivatives of a callable function.
 
     To replace scipy.misc.derivative which is to be deprecated.
 
@@ -49,20 +46,7 @@
     for i in range(n_coeffs):
         coeff = coeffs["coefficients"][i]
         offset = coeffs["offsets"][i]
         c_i = coeff / dx ** n
         x_i = x + offset * dx
         res += c_i * f(x_i)
     return res
-
-
-def simpson(integrand, x=None):
-    """Simple wrapper for SciPy's simpson integrator
-
-    Wrapper to deal with deprecation of 'even=' optional argument in later
-    versions of scipy
-    """
-    vSciPy = metadata.version("scipy")
-    if version.parse(vSciPy) >= version.parse("1.11.0"):
-        return simps(integrand, x=x)
-    else:
-        return simps(integrand, x=x, even="first")
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet/laplacian.py` & `bubbledet-1.0.7/src/BubbleDet/laplacian.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/negative_eigenvalue.py` & `bubbledet-1.0.7/src/BubbleDet/negative_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/phi_infinity.py` & `bubbledet-1.0.7/src/BubbleDet/phi_infinity.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/src/BubbleDet/renormalisation.py` & `bubbledet-1.0.7/src/BubbleDet/renormalisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import numpy as np  # arrays and maths
-from scipy import special # integrator, special functions
-from .helpers import simpson  # integrator
+from scipy import special  # integrator, special functions
 from cosmoTransitions.helper_functions import deriv14  # derivatives for arrays
+try:
+    from scipy.integrate import simpson
+except ImportError:
+    # scipy.version < 1.6
+    from scipy.integrate import simps as simpson
 
 
 def findRenormalisationTerm(config):
     r"""Renormalisation scale dependent part of determinant
 
     Full docs in BubbleDet.py.
     """
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet/wkb.py` & `bubbledet-1.0.7/src/BubbleDet/wkb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np  # arrays and maths
-from scipy import special # for special functions etc
-from scipy.special import zeta
-from .helpers import simpson  # integrator
+from scipy import special  # for special functions etc
 from cosmoTransitions.helper_functions import deriv14  # derivatives for arrays
+try:
+    from scipy.integrate import simpson
+except ImportError:
+    # scipy.version < 1.6
+    from scipy.integrate import simps as simpson
 
 
 def findWKB(config, l_max, Delta_W_inf, a_inf, separate_orders=False):
     r"""Terms in the WKB approximation of determinant
 
     Full docs in BubbleDet.py.
     """
@@ -134,15 +137,15 @@
         l1Sum=-1/2*l1Int*(3)
         l3Sum=-1/2*l3Int*(3/2)
     elif dim==5:
         l1Sum=-1/2*l1Int*(8/3)
         l3Sum=-1/2*l3Int*(416/675 + np.pi**2/24)
     elif dim==6:
         l1Sum=-1/2*l1Int*(5/2)
-        l3Sum=-1/2*l3Int*(829/2592 + zeta(3)/12)
+        l3Sum=-1/2*l3Int*(829/2592 + special.zeta(3)/12)
         l5Sum=0
     elif dim==7:
         l1Sum=-1/2*l1Int*(12/5)
         l3Sum=-1/2*l3Int*(0.1810015354923426)
         l5Sum=-1/2*l5Int*(0.07698283370702798)
     elif dim==9:
         l1Sum=-1/2*l1Int*(16/7)
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet.egg-info/PKG-INFO` & `bubbledet-1.0.7/src/BubbleDet.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 Metadata-Version: 2.1
 Name: BubbleDet
-Version: 1.0.0
+Version: 1.0.7
 Summary: A package for computing functional determinants
 Author-email: Andreas Ekstedt <andreas.ekstedt@desy.de>, Oliver Gould <oliver.gould@nottingham.ac.uk>, Joonas Hirvonen <joonas.o.hirvonen@helsinki.fi>
 License: MIT
 Project-URL: Homepage, https://bubbledet.readthedocs.io/
 Project-URL: Repository, https://bitbucket.org/og113/bubbledet/
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: cosmoTransitions>=2.0.6
+Requires-Dist: findiff>=0.9.2
+Requires-Dist: numpy>=1.21.5
+Requires-Dist: packaging>=21.3
+Requires-Dist: scipy>=1.8.0
 Provides-Extra: tests
+Requires-Dist: pytest>=7.2.2; extra == "tests"
+Requires-Dist: matplotlib>=3.5.1; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: graphviz; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-automodapi; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
 
 ===========================================
 BubbleDet
 ===========================================
 
 Computes the one-loop functional determinant entering the bubble nucleation
 rate, or vacuum decay rate.
 
 |
 
 Documentation
 ===========================================
-For complete documentation, see the
-`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_.
+For complete package documentation, see the
+`BubbleDet homepage <https://bubbledet.readthedocs.io/>`_. For more information
+about the mathematics behind BubbleDet, see the accompanying paper on
+`arXiv <https://arxiv.org/abs/2308.15652>`_.
 
 |
 
 
 Requirements
 ===========================================
```

### Comparing `BubbleDet-1.0.0/src/BubbleDet.egg-info/SOURCES.txt` & `bubbledet-1.0.7/src/BubbleDet.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 .gitignore
 .readthedocs.yaml
 CHANGELOG.rst
 LICENSE
 README.rst
+bitbucket-pipelines.yml
 pyproject.toml
 setup.py
 docs/Makefile
 docs/make.bat
 docs/source/bubbledet.rst
 docs/source/changelog.rst
 docs/source/collected_examples.rst
 docs/source/conf.py
 docs/source/contact.rst
 docs/source/development.rst
+docs/source/faq.rst
 docs/source/first_example.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/intro.rst
+docs/source/refs.bib
 docs/source/examples/analogue.rst
 docs/source/examples/first_example.rst
 docs/source/examples/kink.rst
 docs/source/examples/symmetry_breaking.rst
 docs/source/examples/thermal.rst
 docs/source/examples/thinwall.rst
 docs/source/examples/unbounded.rst
```

### Comparing `BubbleDet-1.0.0/tests/conftest.py` & `bubbledet-1.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/data/baacke_lavrelashvili_table1` & `bubbledet-1.0.7/tests/data/baacke_lavrelashvili_table1`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/data/ekstedt_fits.py` & `bubbledet-1.0.7/tests/data/ekstedt_fits.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/data/scaleless_results.py` & `bubbledet-1.0.7/tests/data/scaleless_results.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/test_derivative_expansion.py` & `bubbledet-1.0.7/tests/test_derivative_expansion.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,59 +4,55 @@
 from .conftest import profile_object
 
 
 @pytest.mark.parametrize(
     "dim, alpha, g",
     [
         (2, 0.5, 1.5),
-        (3, 0.5, 1.5),
         (4, 0.5, 1.5),
-        (5, 0.5, 1.5),
         (6, 0.5, 1.5),
-        (7, 0.5, 1.5),
     ],
 )
 def test_findDerivativeExpansion_V4(cosmo_transitions_V4, dim, alpha, g):
     """
     Tests that the derivative expansion agrees with the full result when
     the fluctuating particle is much heavier than the Higgs.
     """
     ct_prof = profile_object(cosmo_transitions_V4, dim, alpha)
     bubble = BubbleConfig.fromCosmoTransitions(cosmo_transitions_V4, ct_prof)
     gauge = ParticleConfig(
         W_Phi=lambda phi: g**2 * phi**2,
         spin=1,
+        dof_internal=3,
         zero_modes="None",
     )
     bd = BubbleDeterminant(bubble, gauge, gauge_groups=["U1", "None"])
     S1, err = bd.findDeterminant()
-    S1_DE, S1_DE_err = bd.findDerivativeExpansion(gauge)
+    S1_DE, S1_DE_err = bd.findDerivativeExpansion(gauge, NLO=(dim>2))
     assert S1_DE == pytest.approx(S1, rel=0.1)
 
 
 @pytest.mark.parametrize(
     "dim, alpha, g",
     [
-        (2, 0.5, 1.5),
         (3, 0.5, 1.5),
-        (4, 0.5, 1.5),
         (5, 0.5, 1.5),
-        (6, 0.5, 1.5),
         (7, 0.5, 1.5),
     ],
 )
 def test_findDerivativeExpansion_V6(cosmo_transitions_V6, dim, alpha, g):
     """
     Tests that the derivative expansion agrees with the full result when
     the fluctuating particle is much heavier than the Higgs.
     """
     ct_prof = profile_object(cosmo_transitions_V6, dim, alpha)
     bubble = BubbleConfig.fromCosmoTransitions(cosmo_transitions_V6, ct_prof)
     gauge = ParticleConfig(
         W_Phi=lambda phi: g**2 * phi**2,
         spin=1,
+        dof_internal=3,
         zero_modes="None",
     )
     bd = BubbleDeterminant(bubble, gauge, gauge_groups=["U1", "None"])
     S1, err = bd.findDeterminant()
-    S1_DE, S1_DE_err = bd.findDerivativeExpansion(gauge)
+    S1_DE, S1_DE_err = bd.findDerivativeExpansion(gauge, NLO=(dim>2))
     assert S1_DE == pytest.approx(S1, rel=0.1)
```

### Comparing `BubbleDet-1.0.0/tests/test_determinant.py` & `bubbledet-1.0.7/tests/test_determinant.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 dir_path = os.path.dirname(real_path)
 
 
 @pytest.mark.parametrize(
     "dim, alpha",
     [
         (3, 0.3),
-        (3, 0.5),
-        (3, 0.7),
-        (3, 0.9),
+        (3, 0.6),
         (3, 0.95),
     ],
 )
 def test_findDeterminant_Higgs_V4_3d(cosmo_transitions_V4, dim, alpha):
     """
     Tests that the one-loop determinant agrees with Table 1 in
     Eur.Phys.J.C 82 (2022) 2, 173, arXiv:2104.11804 [hep-ph].
@@ -48,17 +46,15 @@
 
 
 @pytest.mark.filterwarnings("ignore:ddphi=0 at r=0")
 @pytest.mark.parametrize(
     "dim, alpha",
     [
         (3, 0.3),
-        (3, 0.5),
-        (3, 0.7),
-        (3, 0.9),
+        (3, 0.6),
         (3, 0.95), # warning arises here, due to inaccurate bounce
     ],
 )
 def test_findDeterminant_Higgs_V6_3d(cosmo_transitions_V6, dim, alpha):
     """
     Tests that the one-loop determinant agrees with Table 2 in
     Eur.Phys.J.C 82 (2022) 2, 173, arXiv:2104.11804 [hep-ph].
@@ -71,17 +67,15 @@
     assert S1 == pytest.approx(SH1_V6_fit(alpha), rel=0.05)
 
 
 @pytest.mark.parametrize(
     "dim, alpha",
     [
         (3, 0.3),
-        (3, 0.5),
-        (3, 0.7),
-        (3, 0.9),
+        (3, 0.6),
         (3, 0.95),
     ],
 )
 def test_findDeterminant_Goldstone_V4_3d(cosmo_transitions_V4, dim, alpha):
     """
     Tests that the one-loop determinant agrees with Table 1 in
     Eur.Phys.J.C 82 (2022) 2, 173, arXiv:2104.11804 [hep-ph].
@@ -97,17 +91,15 @@
     assert S1 == pytest.approx(SG1_V4_fit(alpha), rel=0.01)
 
 
 @pytest.mark.parametrize(
     "dim, alpha",
     [
         (3, 0.3),
-        (3, 0.5),
-        (3, 0.7),
-        (3, 0.9),
+        (3, 0.6),
         (3, 0.95),
     ],
 )
 def test_findDeterminant_Goldstone_V6_3d(cosmo_transitions_V6, dim, alpha):
     """
     Tests that the one-loop determinant agrees with Table 2 in
     Eur.Phys.J.C 82 (2022) 2, 173, arXiv:2104.11804 [hep-ph].
@@ -123,19 +115,15 @@
     assert S1 == pytest.approx(SG1_V6_fit(alpha), rel=0.01)
 
 
 @pytest.mark.parametrize(
     "dim, alpha",
     [
         (4, 0.05),
-        (4, 0.1),
-        (4, 0.3),
         (4, 0.5),
-        (4, 0.7),
-        (4, 0.9),
         (4, 0.95),
     ],
 )
 def test_findDeterminant_Higgs_V4_4d(cosmo_transitions_V4, dim, alpha):
     """
     Tests that the one-loop determinant agrees with Table 1 in
     Phys.Rev.D 69 (2004) 025009, arXiv:hep-th/0307202.
```

### Comparing `BubbleDet-1.0.0/tests/test_extrapolation.py` & `bubbledet-1.0.7/tests/test_extrapolation.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/test_gelfand_yaglom.py` & `bubbledet-1.0.7/tests/test_gelfand_yaglom.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/test_negative_eigenvalue.py` & `bubbledet-1.0.7/tests/test_negative_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `BubbleDet-1.0.0/tests/test_phi_infinity.py` & `bubbledet-1.0.7/tests/test_phi_infinity.py`

 * *Files identical despite different names*

