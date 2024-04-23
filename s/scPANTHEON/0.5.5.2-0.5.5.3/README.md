# Comparing `tmp/scPANTHEON-0.5.5.2.tar.gz` & `tmp/scPANTHEON-0.5.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.5.5.2.tar", last modified: Wed Apr 17 10:33:48 2024, max compression
+gzip compressed data, was "scPANTHEON-0.5.5.3.tar", last modified: Tue Apr 23 11:10:24 2024, max compression
```

## Comparing `scPANTHEON-0.5.5.2.tar` & `scPANTHEON-0.5.5.3.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.138350 scPANTHEON-0.5.5.2/
--rw-rw-rw-   0        0        0      132 2024-03-24 08:59:16.000000 scPANTHEON-0.5.5.2/.gitattributes
--rw-rw-rw-   0        0        0       66 2024-04-02 11:16:17.000000 scPANTHEON-0.5.5.2/.gitignore
--rw-rw-rw-   0        0        0   837120 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/10k-genomics.png
--rw-rw-rw-   0        0        0      240 2024-04-17 10:33:48.137343 scPANTHEON-0.5.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.2/README.md
--rw-rw-rw-   0        0        0        0 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.471223 scPANTHEON-0.5.5.2/__pycache__/
--rw-rw-rw-   0        0        0      143 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      689 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     3789 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/qt.cpython-39.pyc
--rw-rw-rw-   0        0        0      363 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0    35541 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/source.cpython-36.pyc
--rw-rw-rw-   0        0        0    35243 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/source.cpython-38.pyc
--rw-rw-rw-   0        0        0    35200 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0    37871 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/sourceqt.cpython-39.pyc
--rw-rw-rw-   0        0        0      631 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.2/__pycache__/transform.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.473228 scPANTHEON-0.5.5.2/data/
--rw-rw-rw-   0        0        0  3207172 2022-11-04 12:04:08.000000 scPANTHEON-0.5.5.2/data/ADT.csv
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.486087 scPANTHEON-0.5.5.2/document/
--rw-rw-rw-   0        0        0      658 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/Makefile
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.510350 scPANTHEON-0.5.5.2/document/build/
--rw-rw-rw-   0        0        0      234 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.buildinfo
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.523368 scPANTHEON-0.5.5.2/document/build/.doctrees/
--rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Download.doctree
--rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Introduction.doctree
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.531884 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/
--rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.533886 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Navigation/contents.doctree
--rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree
--rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/index.doctree
--rw-rw-rw-   0        0        0    19829 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/environment.pickle
--rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/.doctrees/index.doctree
--rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Download.html
--rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Introduction.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.542924 scPANTHEON-0.5.5.2/document/build/Tutorials/
--rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Tutorials/Clustering with sacnpy.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.544923 scPANTHEON-0.5.5.2/document/build/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    12677 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Tutorials/Navigation/contents.html
--rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Tutorials/Preprocessing with scanpy.html
--rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/Tutorials/index.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.579079 scPANTHEON-0.5.5.2/document/build/_images/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/_images/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/_images/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/_images/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/_images/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.2/document/build/_images/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_images/7hlg1.png
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.588102 scPANTHEON-0.5.5.2/document/build/_sources/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Download.rst.txt
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Introduction.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.593623 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/
--rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/Clustering with sacnpy.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.596127 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/Navigation/contents.rst.txt
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/Preprocessing with scanpy.rst.txt
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/index.rst.txt
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.630366 scPANTHEON-0.5.5.2/document/build/_static/
--rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    11885 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/alabaster.css
--rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.635366 scPANTHEON-0.5.5.2/document/build/_static/css/
--rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.685113 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/css/theme.css
--rw-rw-rw-   0        0        0       43 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/custom.css
--rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/file.png
--rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/jquery-3.6.0.js
--rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.694602 scPANTHEON-0.5.5.2/document/build/_static/js/
--rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/plus.png
--rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/pygments.css
--rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/searchtools.js
--rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/_static/underscore.js
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.704630 scPANTHEON-0.5.5.2/document/build/doctrees/
--rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Download.doctree
--rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Introduction.doctree
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.710660 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/
--rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.712658 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Navigation/contents.doctree
--rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree
--rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/index.doctree
--rw-rw-rw-   0        0        0    19803 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/environment.pickle
--rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/doctrees/index.doctree
--rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/genindex.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.731251 scPANTHEON-0.5.5.2/document/build/html/
--rw-rw-rw-   0        0        0      234 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/.buildinfo
--rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Download.html
--rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Introduction.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.740100 scPANTHEON-0.5.5.2/document/build/html/Tutorials/
--rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Tutorials/Clustering with sacnpy.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.742102 scPANTHEON-0.5.5.2/document/build/html/Tutorials/Navigation/
--rw-rw-rw-   0        0        0    12248 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Tutorials/Navigation/contents.html
--rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Tutorials/Preprocessing with scanpy.html
--rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/Tutorials/index.html
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.772039 scPANTHEON-0.5.5.2/document/build/html/_images/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_images/7hlg1.png
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.780066 scPANTHEON-0.5.5.2/document/build/html/_sources/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Download.rst.txt
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Introduction.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.788012 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/
--rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/Clustering with sacnpy.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.789013 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/Preprocessing with scanpy.rst.txt
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/index.rst.txt
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.829232 scPANTHEON-0.5.5.2/document/build/html/_static/
--rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.835230 scPANTHEON-0.5.5.2/document/build/html/_static/css/
--rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.902052 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/css/theme.css
--rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/file.png
--rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/jquery-3.6.0.js
--rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.912280 scPANTHEON-0.5.5.2/document/build/html/_static/js/
--rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/plus.png
--rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/pygments.css
--rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/_static/underscore.js
--rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/genindex.html
--rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/index.html
--rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/objects.inv
--rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/search.html
--rw-rw-rw-   0        0        0     3080 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/html/searchindex.js
--rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/index.html
--rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/objects.inv
--rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/search.html
--rw-rw-rw-   0        0        0     3339 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/build/searchindex.js
--rwxrwxrwx   0        0        0      804 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/make.bat
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.924341 scPANTHEON-0.5.5.2/document/source/
--rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Download.rst
--rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Introduction.rst
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.932880 scPANTHEON-0.5.5.2/document/source/Tutorials/
--rw-rw-rw-   0        0        0       46 2024-03-23 11:22:01.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Clustering with sacnpy.rst
--rw-rw-rw-   0        0        0       46 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Clustering with scanpy.rst
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.934879 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/
--rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/contents.rst
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.968906 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/
--rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/1overview0.png
--rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/2mouse1.png
--rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map.png
--rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map1.png
--rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map2.png
--rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map3.png
--rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/4plot1.png
--rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/5group1.png
--rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/6cluster1.png
--rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/6cluster2.png
--rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/7hlg1.png
--rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/Preprocessing with scanpy.rst
--rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/Tutorials/index.rst
--rw-rw-rw-   0        0        0      951 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/conf.py
--rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/document/source/index.rst
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.407003 scPANTHEON-0.5.5.2/extension/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.971905 scPANTHEON-0.5.5.2/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.979937 scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     3990 2024-04-02 11:01:10.000000 scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     2348 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     1691 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2363 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1741 2024-03-24 09:06:41.000000 scPANTHEON-0.5.5.2/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.981937 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.990470 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     7058 2024-04-02 11:01:17.000000 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     3901 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     2896 2024-03-24 09:05:36.000000 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3911 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3354 2024-03-24 09:06:53.000000 scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:47.991477 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.000991 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0    11487 2024-04-02 11:01:13.000000 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     6104 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     4423 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5975 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5670 2024-03-24 09:06:59.000000 scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.002994 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.011309 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     9696 2024-04-02 11:01:11.000000 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     5101 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     3786 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5037 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4839 2024-03-24 09:07:32.000000 scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.014304 scPANTHEON-0.5.5.2/extension/Plot_Histogram/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.023319 scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/
--rw-rw-rw-   0        0        0      172 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8022 2024-04-02 10:04:39.000000 scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     4379 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     4412 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5244 2024-04-02 10:04:06.000000 scPANTHEON-0.5.5.2/extension/Plot_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.025323 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.035138 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0    16100 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     7921 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     5877 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     7827 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     8155 2024-03-24 09:07:39.000000 scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.037146 scPANTHEON-0.5.5.2/extension/R_UMAP/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.041153 scPANTHEON-0.5.5.2/extension/R_UMAP/__pycache__/
--rw-rw-rw-   0        0        0    18998 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/R_UMAP/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0    10979 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/R_UMAP/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0    12580 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/R_UMAP/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.044152 scPANTHEON-0.5.5.2/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.053244 scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0    20982 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0    10490 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-37.pyc
--rw-rw-rw-   0        0        0     7544 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0    10206 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    11454 2024-03-24 09:07:45.000000 scPANTHEON-0.5.5.2/extension/TOMAS/module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.068035 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      240 2024-04-17 10:33:45.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12245 2024-04-17 10:33:47.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:33:45.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-17 10:33:45.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      112 2024-04-17 10:33:45.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 10:33:45.000000 scPANTHEON-0.5.5.2/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.076039 scPANTHEON-0.5.5.2/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.2/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.097927 scPANTHEON-0.5.5.2/scpantheon/__pycache__/
--rw-rw-rw-   0        0        0   106928 2024-02-18 02:45:28.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/aaa.cpython-311.pyc
--rw-rw-rw-   0        0        0     1405 2023-03-11 01:52:14.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/anndata.cpython-39.pyc
--rw-rw-rw-   0        0        0     2701 2023-07-06 11:39:42.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     4877 2023-09-07 14:04:21.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/data_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     4144 2023-04-20 04:56:49.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/qt.cpython-39.pyc
--rw-rw-rw-   0        0        0   105962 2024-04-14 09:03:38.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-311.pyc
--rw-rw-rw-   0        0        0    35550 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-38.pyc
--rw-rw-rw-   0        0        0    50207 2023-08-04 11:20:46.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0      643 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.2/scpantheon/__pycache__/transform.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.101928 scPANTHEON-0.5.5.2/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.2/scpantheon/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.111192 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/
--rw-rw-rw-   0        0        0      179 2024-02-24 08:42:01.000000 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      161 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5557 2024-03-24 08:26:36.000000 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     2705 2023-07-10 06:20:31.000000 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0    49472 2023-07-12 11:46:18.000000 scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/source.cpython-39.pyc
--rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.2/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.118876 scPANTHEON-0.5.5.2/scpantheon/front_end/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.133072 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/
--rw-rw-rw-   0        0        0      185 2023-11-20 22:01:18.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      167 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    20629 2024-04-08 14:46:54.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     4722 2023-07-13 13:25:20.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0     7822 2024-03-24 05:59:04.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     7846 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     7576 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc
--rw-rw-rw-   0        0        0     3473 2023-07-10 13:34:08.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc
--rw-rw-rw-   0        0        0    13251 2024-04-17 10:32:16.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/extensions_qt.py
--rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/load_qt.py
--rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.2/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1326 2024-04-17 10:31:18.000000 scPANTHEON-0.5.5.2/scpantheon/main.py
--rw-rw-rw-   0        0        0    66961 2024-04-17 10:32:10.000000 scPANTHEON-0.5.5.2/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2024-04-17 10:33:48.138350 scPANTHEON-0.5.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1147 2024-04-17 10:30:42.000000 scPANTHEON-0.5.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:33:48.135230 scPANTHEON-0.5.5.2/tests/
--rw-rw-rw-   0        0        0     6815 2024-04-14 07:24:22.000000 scPANTHEON-0.5.5.2/tests/test_data.py
--rw-rw-rw-   0        0        0   104067 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.2/zhijiang.png
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.646738 scPANTHEON-0.5.5.3/
+-rw-rw-rw-   0        0        0      132 2024-03-24 08:59:16.000000 scPANTHEON-0.5.5.3/.gitattributes
+-rw-rw-rw-   0        0        0       67 2024-04-23 07:01:38.000000 scPANTHEON-0.5.5.3/.gitignore
+-rw-rw-rw-   0        0        0   837120 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/10k-genomics.png
+-rw-rw-rw-   0        0        0      240 2024-04-23 11:10:24.645664 scPANTHEON-0.5.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.3/README.md
+-rw-rw-rw-   0        0        0        0 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.893169 scPANTHEON-0.5.5.3/__pycache__/
+-rw-rw-rw-   0        0        0      143 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      689 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3789 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      363 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0    35541 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/source.cpython-36.pyc
+-rw-rw-rw-   0        0        0    35243 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/source.cpython-38.pyc
+-rw-rw-rw-   0        0        0    35200 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0    37871 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/sourceqt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      631 2024-03-24 09:05:35.000000 scPANTHEON-0.5.5.3/__pycache__/transform.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.896413 scPANTHEON-0.5.5.3/data/
+-rw-rw-rw-   0        0        0  3207172 2022-11-04 12:04:08.000000 scPANTHEON-0.5.5.3/data/ADT.csv
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.910901 scPANTHEON-0.5.5.3/document/
+-rw-rw-rw-   0        0        0      658 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.932738 scPANTHEON-0.5.5.3/document/build/
+-rw-rw-rw-   0        0        0      234 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.buildinfo
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.943258 scPANTHEON-0.5.5.3/document/build/.doctrees/
+-rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Download.doctree
+-rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Introduction.doctree
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.952496 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/
+-rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.955060 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Navigation/contents.doctree
+-rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree
+-rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/index.doctree
+-rw-rw-rw-   0        0        0    19829 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/.doctrees/index.doctree
+-rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Download.html
+-rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Introduction.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.963313 scPANTHEON-0.5.5.3/document/build/Tutorials/
+-rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Tutorials/Clustering with sacnpy.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.967602 scPANTHEON-0.5.5.3/document/build/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    12677 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Tutorials/Navigation/contents.html
+-rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Tutorials/Preprocessing with scanpy.html
+-rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/Tutorials/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.014887 scPANTHEON-0.5.5.3/document/build/_images/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/_images/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/_images/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/_images/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/_images/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:41.000000 scPANTHEON-0.5.5.3/document/build/_images/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_images/7hlg1.png
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.020716 scPANTHEON-0.5.5.3/document/build/_sources/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Download.rst.txt
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Introduction.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.028509 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/
+-rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/Clustering with sacnpy.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.031142 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/Navigation/contents.rst.txt
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/Preprocessing with scanpy.rst.txt
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/index.rst.txt
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.071089 scPANTHEON-0.5.5.3/document/build/_static/
+-rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    11885 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.075789 scPANTHEON-0.5.5.3/document/build/_static/css/
+-rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.123625 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/css/theme.css
+-rw-rw-rw-   0        0        0       43 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/custom.css
+-rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/doctools.js
+-rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/file.png
+-rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.133721 scPANTHEON-0.5.5.3/document/build/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/pygments.css
+-rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/searchtools.js
+-rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/_static/underscore.js
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.143292 scPANTHEON-0.5.5.3/document/build/doctrees/
+-rw-rw-rw-   0        0        0     2390 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Download.doctree
+-rw-rw-rw-   0        0        0     3738 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Introduction.doctree
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.151001 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/
+-rw-rw-rw-   0        0        0     2470 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.152979 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    19370 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Navigation/contents.doctree
+-rw-rw-rw-   0        0        0     2485 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree
+-rw-rw-rw-   0        0        0     2844 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/index.doctree
+-rw-rw-rw-   0        0        0    19803 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     4036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/genindex.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.170010 scPANTHEON-0.5.5.3/document/build/html/
+-rw-rw-rw-   0        0        0      234 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/.buildinfo
+-rw-rw-rw-   0        0        0     4380 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Download.html
+-rw-rw-rw-   0        0        0     4782 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Introduction.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.176761 scPANTHEON-0.5.5.3/document/build/html/Tutorials/
+-rw-rw-rw-   0        0        0     4758 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Tutorials/Clustering with sacnpy.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.179291 scPANTHEON-0.5.5.3/document/build/html/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0    12248 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Tutorials/Navigation/contents.html
+-rw-rw-rw-   0        0        0     5036 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Tutorials/Preprocessing with scanpy.html
+-rw-rw-rw-   0        0        0     6225 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/Tutorials/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.209875 scPANTHEON-0.5.5.3/document/build/html/_images/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_images/7hlg1.png
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.217227 scPANTHEON-0.5.5.3/document/build/html/_sources/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Download.rst.txt
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Introduction.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.223394 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/
+-rw-rw-rw-   0        0        0       46 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/Clustering with sacnpy.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.227012 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/Preprocessing with scanpy.rst.txt
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/index.rst.txt
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.261772 scPANTHEON-0.5.5.3/document/build/html/_static/
+-rw-rw-rw-   0        0        0     4552 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    15519 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.267212 scPANTHEON-0.5.5.3/document/build/html/_static/css/
+-rw-rw-rw-   0        0        0     3275 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.331274 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   129677 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/css/theme.css
+-rw-rw-rw-   0        0        0     8435 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      433 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/file.png
+-rw-rw-rw-   0        0        0   299461 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.346481 scPANTHEON-0.5.5.3/document/build/html/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4373 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2737 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    17650 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    70462 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19535 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0     3491 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/genindex.html
+-rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/index.html
+-rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/objects.inv
+-rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/search.html
+-rw-rw-rw-   0        0        0     3080 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/html/searchindex.js
+-rw-rw-rw-   0        0        0     6035 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/index.html
+-rw-rw-rw-   0        0        0      382 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/objects.inv
+-rw-rw-rw-   0        0        0     3905 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/search.html
+-rw-rw-rw-   0        0        0     3339 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/build/searchindex.js
+-rwxrwxrwx   0        0        0      804 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/make.bat
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.358047 scPANTHEON-0.5.5.3/document/source/
+-rw-rw-rw-   0        0        0       18 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Download.rst
+-rw-rw-rw-   0        0        0      357 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Introduction.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.371774 scPANTHEON-0.5.5.3/document/source/Tutorials/
+-rw-rw-rw-   0        0        0       46 2024-03-23 11:22:01.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Clustering with sacnpy.rst
+-rw-rw-rw-   0        0        0       46 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Clustering with scanpy.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.373950 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/
+-rw-rw-rw-   0        0        0     3685 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/contents.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.411384 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/
+-rw-rw-rw-   0        0        0   315646 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/1overview0.png
+-rw-rw-rw-   0        0        0    97838 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/2mouse1.png
+-rw-rw-rw-   0        0        0     7710 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map.png
+-rw-rw-rw-   0        0        0     2637 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map1.png
+-rw-rw-rw-   0        0        0     1135 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map2.png
+-rw-rw-rw-   0        0        0    74529 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map3.png
+-rw-rw-rw-   0        0        0    93253 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/4plot1.png
+-rw-rw-rw-   0        0        0     8705 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/5group1.png
+-rw-rw-rw-   0        0        0    16937 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/6cluster1.png
+-rw-rw-rw-   0        0        0     9660 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/6cluster2.png
+-rw-rw-rw-   0        0        0   108876 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/7hlg1.png
+-rw-rw-rw-   0        0        0       52 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/Preprocessing with scanpy.rst
+-rw-rw-rw-   0        0        0      136 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/Tutorials/index.rst
+-rw-rw-rw-   0        0        0      951 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/conf.py
+-rw-rw-rw-   0        0        0      503 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/document/source/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:23.838568 scPANTHEON-0.5.5.3/extension/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.413904 scPANTHEON-0.5.5.3/extension/Change_Color/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.424203 scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/
+-rw-rw-rw-   0        0        0     3990 2024-04-02 11:01:10.000000 scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2348 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1691 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2363 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1741 2024-03-24 09:06:41.000000 scPANTHEON-0.5.5.3/extension/Change_Color/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.427465 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.438989 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0     7058 2024-04-02 11:01:17.000000 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3901 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2896 2024-03-24 09:05:36.000000 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3911 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3354 2024-03-24 09:06:53.000000 scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.441042 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.455117 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/
+-rw-rw-rw-   0        0        0    11487 2024-04-02 11:01:13.000000 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6104 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4423 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5975 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5670 2024-03-24 09:06:59.000000 scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.458337 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.474290 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/
+-rw-rw-rw-   0        0        0     9696 2024-04-02 11:01:11.000000 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5101 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3786 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5037 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4839 2024-03-24 09:07:32.000000 scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.478752 scPANTHEON-0.5.5.3/extension/Plot_Histogram/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.493617 scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/
+-rw-rw-rw-   0        0        0      172 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8022 2024-04-02 10:04:39.000000 scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4379 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4412 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5244 2024-04-02 10:04:06.000000 scPANTHEON-0.5.5.3/extension/Plot_Histogram/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.496895 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.510171 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/
+-rw-rw-rw-   0        0        0    16100 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7921 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5877 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7827 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8155 2024-03-24 09:07:39.000000 scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.512739 scPANTHEON-0.5.5.3/extension/R_UMAP/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.517191 scPANTHEON-0.5.5.3/extension/R_UMAP/__pycache__/
+-rw-rw-rw-   0        0        0    18998 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/R_UMAP/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10979 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/R_UMAP/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12580 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/R_UMAP/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.520235 scPANTHEON-0.5.5.3/extension/TOMAS/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.530969 scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/
+-rw-rw-rw-   0        0        0    20982 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10490 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7544 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-38.pyc
+-rw-rw-rw-   0        0        0    10206 2024-03-24 09:04:54.000000 scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11454 2024-03-24 09:07:45.000000 scPANTHEON-0.5.5.3/extension/TOMAS/module.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.548651 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      240 2024-04-23 11:10:21.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12245 2024-04-23 11:10:23.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:10:21.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-23 11:10:21.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2024-04-23 11:10:21.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 11:10:21.000000 scPANTHEON-0.5.5.3/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.556507 scPANTHEON-0.5.5.3/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.3/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.585397 scPANTHEON-0.5.5.3/scpantheon/__pycache__/
+-rw-rw-rw-   0        0        0   106928 2024-02-18 02:45:28.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/aaa.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1405 2023-03-11 01:52:14.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/anndata.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2701 2023-07-06 11:39:42.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4877 2023-09-07 14:04:21.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/data_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4144 2023-04-20 04:56:49.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0   105962 2024-04-14 09:03:38.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-311.pyc
+-rw-rw-rw-   0        0        0    35550 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-38.pyc
+-rw-rw-rw-   0        0        0    50207 2023-08-04 11:20:46.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0      643 2023-02-09 07:28:42.000000 scPANTHEON-0.5.5.3/scpantheon/__pycache__/transform.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.591331 scPANTHEON-0.5.5.3/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.3/scpantheon/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.603915 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/
+-rw-rw-rw-   0        0        0      179 2024-02-24 08:42:01.000000 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      161 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5557 2024-03-24 08:26:36.000000 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2705 2023-07-10 06:20:31.000000 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0    49472 2023-07-12 11:46:18.000000 scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/source.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2978 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.3/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.616860 scPANTHEON-0.5.5.3/scpantheon/front_end/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.639934 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/
+-rw-rw-rw-   0        0        0      185 2023-11-20 22:01:18.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      167 2023-07-14 08:17:56.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    20629 2024-04-08 14:46:54.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4722 2023-07-13 13:25:20.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7822 2024-03-24 05:59:04.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7846 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7576 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3473 2023-07-10 13:34:08.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13252 2024-04-23 11:09:20.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     4227 2024-03-24 05:48:52.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/extensions_qt.py
+-rw-rw-rw-   0        0        0     4567 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/load_qt.py
+-rw-rw-rw-   0        0        0     4899 2024-03-23 11:36:17.000000 scPANTHEON-0.5.5.3/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1104 2024-04-23 08:14:22.000000 scPANTHEON-0.5.5.3/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66962 2024-04-23 11:09:13.000000 scPANTHEON-0.5.5.3/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:10:24.646738 scPANTHEON-0.5.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1147 2024-04-23 06:56:20.000000 scPANTHEON-0.5.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:10:24.642907 scPANTHEON-0.5.5.3/tests/
+-rw-rw-rw-   0        0        0     6815 2024-04-14 07:24:22.000000 scPANTHEON-0.5.5.3/tests/test_data.py
+-rw-rw-rw-   0        0        0   104067 2024-01-02 19:33:04.000000 scPANTHEON-0.5.5.3/zhijiang.png
```

### Comparing `scPANTHEON-0.5.5.2/10k-genomics.png` & `scPANTHEON-0.5.5.3/10k-genomics.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/main.cpython-39.pyc` & `scPANTHEON-0.5.5.3/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/__pycache__/qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/source.cpython-36.pyc` & `scPANTHEON-0.5.5.3/__pycache__/source.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/source.cpython-38.pyc` & `scPANTHEON-0.5.5.3/__pycache__/source.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.3/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/sourceqt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/__pycache__/sourceqt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/__pycache__/transform.cpython-39.pyc` & `scPANTHEON-0.5.5.3/__pycache__/transform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/data/ADT.csv` & `scPANTHEON-0.5.5.3/data/ADT.csv`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/Makefile` & `scPANTHEON-0.5.5.3/document/Makefile`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Download.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Download.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Introduction.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Introduction.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Clustering with sacnpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Navigation/contents.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Navigation/contents.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/Preprocessing with scanpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/Tutorials/index.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/Tutorials/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/environment.pickle` & `scPANTHEON-0.5.5.3/document/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/.doctrees/index.doctree` & `scPANTHEON-0.5.5.3/document/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Download.html` & `scPANTHEON-0.5.5.3/document/build/Download.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Introduction.html` & `scPANTHEON-0.5.5.3/document/build/Introduction.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Tutorials/Clustering with sacnpy.html` & `scPANTHEON-0.5.5.3/document/build/Tutorials/Clustering with sacnpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Tutorials/Navigation/contents.html` & `scPANTHEON-0.5.5.3/document/build/Tutorials/Navigation/contents.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Tutorials/Preprocessing with scanpy.html` & `scPANTHEON-0.5.5.3/document/build/Tutorials/Preprocessing with scanpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/Tutorials/index.html` & `scPANTHEON-0.5.5.3/document/build/Tutorials/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/1overview0.png` & `scPANTHEON-0.5.5.3/document/build/_images/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/2mouse1.png` & `scPANTHEON-0.5.5.3/document/build/_images/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/3map.png` & `scPANTHEON-0.5.5.3/document/build/_images/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/3map1.png` & `scPANTHEON-0.5.5.3/document/build/_images/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/3map2.png` & `scPANTHEON-0.5.5.3/document/build/_images/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/3map3.png` & `scPANTHEON-0.5.5.3/document/build/_images/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/4plot1.png` & `scPANTHEON-0.5.5.3/document/build/_images/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/5group1.png` & `scPANTHEON-0.5.5.3/document/build/_images/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/6cluster1.png` & `scPANTHEON-0.5.5.3/document/build/_images/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/6cluster2.png` & `scPANTHEON-0.5.5.3/document/build/_images/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_images/7hlg1.png` & `scPANTHEON-0.5.5.3/document/build/_images/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_sources/Tutorials/Navigation/contents.rst.txt` & `scPANTHEON-0.5.5.3/document/build/_sources/Tutorials/Navigation/contents.rst.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/_sphinx_javascript_frameworks_compat.js` & `scPANTHEON-0.5.5.3/document/build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/alabaster.css` & `scPANTHEON-0.5.5.3/document/build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/basic.css` & `scPANTHEON-0.5.5.3/document/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/badge_only.css` & `scPANTHEON-0.5.5.3/document/build/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Bold.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Regular.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.eot` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.svg` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.ttf` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/fontawesome-webfont.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold-italic.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold-italic.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-bold.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal-italic.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal-italic.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal.woff` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/fonts/lato-normal.woff2` & `scPANTHEON-0.5.5.3/document/build/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/css/theme.css` & `scPANTHEON-0.5.5.3/document/build/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/doctools.js` & `scPANTHEON-0.5.5.3/document/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/jquery-3.6.0.js` & `scPANTHEON-0.5.5.3/document/build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/jquery.js` & `scPANTHEON-0.5.5.3/document/build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/js/badge_only.js` & `scPANTHEON-0.5.5.3/document/build/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/js/html5shiv-printshiv.min.js` & `scPANTHEON-0.5.5.3/document/build/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/js/html5shiv.min.js` & `scPANTHEON-0.5.5.3/document/build/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/js/theme.js` & `scPANTHEON-0.5.5.3/document/build/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/language_data.js` & `scPANTHEON-0.5.5.3/document/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/pygments.css` & `scPANTHEON-0.5.5.3/document/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/searchtools.js` & `scPANTHEON-0.5.5.3/document/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/underscore-1.13.1.js` & `scPANTHEON-0.5.5.3/document/build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/_static/underscore.js` & `scPANTHEON-0.5.5.3/document/build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Download.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Download.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Introduction.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Introduction.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Clustering with sacnpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Navigation/contents.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Navigation/contents.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/Preprocessing with scanpy.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/Tutorials/index.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/Tutorials/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/environment.pickle` & `scPANTHEON-0.5.5.3/document/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/doctrees/index.doctree` & `scPANTHEON-0.5.5.3/document/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/genindex.html` & `scPANTHEON-0.5.5.3/document/build/genindex.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Download.html` & `scPANTHEON-0.5.5.3/document/build/html/Download.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Introduction.html` & `scPANTHEON-0.5.5.3/document/build/html/Introduction.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Tutorials/Clustering with sacnpy.html` & `scPANTHEON-0.5.5.3/document/build/html/Tutorials/Clustering with sacnpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Tutorials/Navigation/contents.html` & `scPANTHEON-0.5.5.3/document/build/html/Tutorials/Navigation/contents.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Tutorials/Preprocessing with scanpy.html` & `scPANTHEON-0.5.5.3/document/build/html/Tutorials/Preprocessing with scanpy.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/Tutorials/index.html` & `scPANTHEON-0.5.5.3/document/build/html/Tutorials/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/1overview0.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/2mouse1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/3map.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/3map1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/3map2.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/3map3.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/4plot1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/5group1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/6cluster1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/6cluster2.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_images/7hlg1.png` & `scPANTHEON-0.5.5.3/document/build/html/_images/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt` & `scPANTHEON-0.5.5.3/document/build/html/_sources/Tutorials/Navigation/contents.rst.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/basic.css` & `scPANTHEON-0.5.5.3/document/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/badge_only.css` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.eot` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.svg` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold-italic.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold-italic.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-bold.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal-italic.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal-italic.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal.woff` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/fonts/lato-normal.woff2` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/css/theme.css` & `scPANTHEON-0.5.5.3/document/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/doctools.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/jquery-3.6.0.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/jquery.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/js/badge_only.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/js/html5shiv-printshiv.min.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/js/html5shiv.min.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/js/theme.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/language_data.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/pygments.css` & `scPANTHEON-0.5.5.3/document/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/searchtools.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/underscore-1.13.1.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/_static/underscore.js` & `scPANTHEON-0.5.5.3/document/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/genindex.html` & `scPANTHEON-0.5.5.3/document/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/index.html` & `scPANTHEON-0.5.5.3/document/build/html/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/search.html` & `scPANTHEON-0.5.5.3/document/build/html/search.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/html/searchindex.js` & `scPANTHEON-0.5.5.3/document/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/index.html` & `scPANTHEON-0.5.5.3/document/build/index.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/search.html` & `scPANTHEON-0.5.5.3/document/build/search.html`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/build/searchindex.js` & `scPANTHEON-0.5.5.3/document/build/searchindex.js`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/make.bat` & `scPANTHEON-0.5.5.3/document/make.bat`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/contents.rst` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/contents.rst`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/1overview0.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/1overview0.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/2mouse1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/2mouse1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map2.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/3map3.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/3map3.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/4plot1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/4plot1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/5group1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/5group1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/6cluster1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/6cluster1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/6cluster2.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/6cluster2.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/Tutorials/Navigation/image/7hlg1.png` & `scPANTHEON-0.5.5.3/document/source/Tutorials/Navigation/image/7hlg1.png`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/document/source/conf.py` & `scPANTHEON-0.5.5.3/document/source/conf.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Change_Color/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Change_Color/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Change_Color/module.py` & `scPANTHEON-0.5.5.3/extension/Change_Color/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Clustering_with_Scanpy/module.py` & `scPANTHEON-0.5.5.3/extension/Clustering_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Differential_Expression_Analysis/module.py` & `scPANTHEON-0.5.5.3/extension/Differential_Expression_Analysis/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Find_Marker_Gene/module.py` & `scPANTHEON-0.5.5.3/extension/Find_Marker_Gene/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Plot_Histogram/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Plot_Histogram/module.py` & `scPANTHEON-0.5.5.3/extension/Plot_Histogram/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/Preprocessing_with_Scanpy/module.py` & `scPANTHEON-0.5.5.3/extension/Preprocessing_with_Scanpy/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/R_UMAP/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/R_UMAP/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/R_UMAP/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/R_UMAP/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/R_UMAP/module.py` & `scPANTHEON-0.5.5.3/extension/R_UMAP/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-311.pyc` & `scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-37.pyc` & `scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-38.pyc` & `scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/TOMAS/__pycache__/module.cpython-39.pyc` & `scPANTHEON-0.5.5.3/extension/TOMAS/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/extension/TOMAS/module.py` & `scPANTHEON-0.5.5.3/extension/TOMAS/module.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scPANTHEON.egg-info/SOURCES.txt` & `scPANTHEON-0.5.5.3/scPANTHEON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/aaa.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/aaa.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/anndata.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/anndata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/bokeh_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/data_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/data_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-38.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/__pycache__/transform.cpython-38.pyc` & `scPANTHEON-0.5.5.3/scpantheon/__pycache__/transform.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/bokeh_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/bokeh_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/app/__pycache__/source.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/app/__pycache__/source.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.5.5.3/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/data_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/data_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/extensions_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/load_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/save_qt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc` & `scPANTHEON-0.5.5.3/scpantheon/front_end/__pycache__/save_qt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.5.5.3/scpantheon/front_end/data_qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
 
 # create center directory to store all kinds of data
 try: 
     version = pkg_resources.get_distribution("scpantheon").version
 except:
-    subprocess.check_call(['pip', 'install', "scpantheon"])
+    subprocess.check_call(['pip3', 'install', "scpantheon"])
     version = pkg_resources.get_distribution("scpantheon").version
 
 import requests, zipfile, tarfile, shutil, subprocess
     
 from appdirs import AppDirs
 import pkg_resources
 global dir
```

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/extensions_qt.py` & `scPANTHEON-0.5.5.3/scpantheon/front_end/extensions_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/load_qt.py` & `scPANTHEON-0.5.5.3/scpantheon/front_end/load_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.5.5.3/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/scpantheon/source.py` & `scPANTHEON-0.5.5.3/scpantheon/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 try:
     from scpantheon.front_end import extensions_qt 
     from scpantheon.front_end.extensions_qt import get_extensions_path
     from scpantheon.front_end import save_qt, load_qt
     from scpantheon.front_end.data_qt import dir, extract_online_packages, auto_pip_install, read_path
     from scpantheon.front_end.save_qt import get_save_path
 except:
-    subprocess.check_call(['pip', 'install', "scpantheon"])
+    subprocess.check_call(['pip3', 'install', "scpantheon"])
     from scpantheon.front_end import extensions_qt 
     from scpantheon.front_end.extensions_qt import get_extensions_path
     from scpantheon.front_end import save_qt, load_qt
     from scpantheon.front_end.data_qt import dir, extract_online_packages, auto_pip_install, read_path
     from scpantheon.front_end.save_qt import get_save_path
```

### Comparing `scPANTHEON-0.5.5.2/setup.py` & `scPANTHEON-0.5.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.5.5.2',#版本
+    version='0.5.5.3',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                        'appdirs','requests','leidenalg', 'setuptools_scm'], # 依赖包,如果没有,可以不要 rpy2
```

### Comparing `scPANTHEON-0.5.5.2/tests/test_data.py` & `scPANTHEON-0.5.5.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.5.5.2/zhijiang.png` & `scPANTHEON-0.5.5.3/zhijiang.png`

 * *Files identical despite different names*

