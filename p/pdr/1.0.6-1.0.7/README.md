# Comparing `tmp/pdr-1.0.6.tar.gz` & `tmp/pdr-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-1.0.6.tar", last modified: Thu Mar 28 18:25:54 2024, max compression
+gzip compressed data, was "pdr-1.0.7.tar", last modified: Tue Apr 23 19:09:26 2024, max compression
```

## Comparing `pdr-1.0.6.tar` & `pdr-1.0.7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.440340 pdr-1.0.6/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2276 2023-12-08 19:57:58.000000 pdr-1.0.6/LICENSE.md
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3925 2024-03-28 18:25:54.440340 pdr-1.0.6/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2836 2024-03-28 17:39:04.000000 pdr-1.0.6/README.md
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.432340 pdr-1.0.6/pdr/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      617 2024-03-28 18:21:53.000000 pdr-1.0.6/pdr/__init__.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.432340 pdr-1.0.6/pdr/_patches/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       54 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/_patches/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      505 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/_patches/patches.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/_patches/six_new.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2024-03-28 17:21:19.000000 pdr-1.0.6/pdr/_patches/six_old.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4034 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5300 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11717 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8212 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      119 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/errors.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.436340 pdr-1.0.6/pdr/formats/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1550 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3990 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/cassini.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    25027 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/checkers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1123 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/clementine.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      380 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/dawn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/diviner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      493 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/epoxi.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3167 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/galileo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2803 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/ihw.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      895 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/juno.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2170 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/lro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.6/pdr/formats/lroc.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      276 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/mariner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      349 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/mer.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2577 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/mex.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2283 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/mgn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      917 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/mgs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1768 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/mro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/msl_apxs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/msl_ccam.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      555 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/msl_cmn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      268 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/msl_places.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3695 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/nh.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      489 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/odyssey.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3182 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/phoenix.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      532 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/pvo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      232 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/rosetta.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      246 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/saturn_rpx.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1035 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/formats/themis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1866 2023-12-08 19:59:12.000000 pdr-1.0.6/pdr/formats/ulysses.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1487 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/vega.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1742 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/viking.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3236 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/formats/voyager.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7133 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/func.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.436340 pdr-1.0.6/pdr/loaders/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.6/pdr/loaders/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2209 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6018 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/datawrap.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4148 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/dispatch.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8041 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/loaders/handlers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5683 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    24065 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/loaders/queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7944 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/loaders/table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2517 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/text.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1596 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/loaders/utility.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4238 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/np_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.436340 pdr-1.0.6/pdr/parselabel/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.6/pdr/parselabel/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    13139 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/parselabel/pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1441 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/parselabel/pds4.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      742 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/parselabel/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11105 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/pd_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    32076 2024-03-28 17:39:08.000000 pdr-1.0.6/pdr/pdr.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.6/pdr/pdrtypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/pvl_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.440340 pdr-1.0.6/pdr/tests/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5158 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/objects.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1921 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2478 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      752 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_data.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1526 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      509 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_fits_load.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3218 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_func.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      396 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2786 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_loader_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      474 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_metadata.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2112 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_np_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      601 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_parselabel_pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1731 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      548 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1039 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4818 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/test_vax.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1544 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/tests/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7088 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4477 2023-12-08 19:57:58.000000 pdr-1.0.6/pdr/vax.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-03-28 18:25:54.440340 pdr-1.0.6/pdr.egg-info/
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3925 2024-03-28 18:25:54.000000 pdr-1.0.6/pdr.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1980 2024-03-28 18:25:54.000000 pdr-1.0.6/pdr.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2024-03-28 18:25:54.000000 pdr-1.0.6/pdr.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      200 2024-03-28 18:25:54.000000 pdr-1.0.6/pdr.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2024-03-28 18:25:54.000000 pdr-1.0.6/pdr.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2024-03-28 18:25:54.440340 pdr-1.0.6/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1111 2024-03-28 18:21:53.000000 pdr-1.0.6/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2276 2023-12-08 19:57:58.000000 pdr-1.0.7/LICENSE.md
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-04-23 19:09:26.443641 pdr-1.0.7/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2863 2024-04-23 19:03:14.000000 pdr-1.0.7/README.md
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.415640 pdr-1.0.7/pdr/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1948 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/__init__.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.419640 pdr-1.0.7/pdr/_patches/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       54 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      505 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/patches.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/six_new.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2024-03-28 17:21:19.000000 pdr-1.0.7/pdr/_patches/six_old.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4063 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8351 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12781 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8608 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      261 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/errors.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/formats/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1576 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5148 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/cassini.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    30523 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/checkers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1283 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/clementine.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      453 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/dawn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1100 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/diviner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      542 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/epoxi.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3894 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/galileo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2792 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/ihw.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1227 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/juno.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2411 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/lro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      182 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/lroc.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      324 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mariner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      397 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mer.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4987 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mex.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2566 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mgn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      963 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mgs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1651 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      276 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_apxs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      273 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_ccam.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1463 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_cmn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      323 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_places.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4910 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/nh.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      557 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/odyssey.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3458 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/phoenix.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      633 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/pvo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      281 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/rosetta.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      410 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/saturn_rpx.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1373 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/themis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2152 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/ulysses.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1640 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/vega.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1877 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/viking.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3575 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/voyager.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7162 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/func.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/loaders/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.7/pdr/loaders/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3779 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6101 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/datawrap.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4629 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/dispatch.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11010 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/handlers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7880 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    31425 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8990 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4693 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/text.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1902 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/utility.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4843 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/np_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/parselabel/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.7/pdr/parselabel/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    15718 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2861 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/pds4.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      939 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    13514 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pd_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    36037 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pdr.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3682 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pdrtypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/pvl_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/pdr/tests/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5158 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/objects.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1991 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2478 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      752 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_data.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1526 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      509 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_fits_load.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3218 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_func.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      396 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2785 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_loader_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      474 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_metadata.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2112 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_np_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      601 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_parselabel_pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1731 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      548 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1038 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4818 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_vax.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1544 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7686 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4481 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/vax.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/pdr.egg-info/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1980 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      200 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2024-04-23 19:09:26.443641 pdr-1.0.7/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1111 2024-04-23 19:03:14.000000 pdr-1.0.7/setup.py
```

### Comparing `pdr-1.0.6/LICENSE.md` & `pdr-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/PKG-INFO` & `pdr-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.6
+Version: 1.0.7
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -35,24 +35,30 @@
 
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
-(under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](docs/supported_datasets.md) 
+(under PDS3 or PDS4) should be covered eventually. 
+[Currently-supported datasets are listed here.](docs/supported_datasets.md) 
 
-If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
+If the software fails while attempting to read from datasets that we have 
+listed as supported, please submit an issue with a link to the file and 
+information about the error (if applicable). There might also be datasets that 
+work but are not listed. We would like to hear about those too. If a dataset 
+is not yet supported that you would like us to consider prioritizing, 
+[please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
 ### Attribution
 If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
 
 ### Installation
-_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
-You can do this like so: 
+_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) 
+installation into a `conda` environment. You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
 conda install -c conda-forge pdr
 ```
 The minimum supported version of Python is _3.9_.
@@ -60,24 +66,28 @@
 Using the conda install will install all dependencies in the environment.yml 
 file (both required and optional) for pdr. If you'd prefer to forego the 
 optional dependencies, please use minimal_environment.yml in your 
 installation. This is not supported through a direct conda install as 
 described above and will reqiore additional steps. Optional dependencies 
 and the added functionality they support are listed below:
 
-  - `pvl`: allows `Data.load("LABEL", as_pvl=True)` which will load PDS3 labels as `pvl` objects rather than plain text
+  - `pvl`: allows `Data.load("LABEL", as_pvl=True)`, which will load PDS3 
+     labels as `pvl` objects rather than plain text
   - `astropy`: adds support for FITS files
-  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter notebooks you create)
+  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter 
+     notebooks you create)
   - `pillow`: adds support for TIFF files and browse image rendering
-  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
+  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse 
+    function
 
 ### Usage
 
 You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main)
 
-Additional information on usage including examples, output data types, notes and caveats, test, etc. 
-can now be accessed in our documentation on readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
+Additional information on usage including examples, output data types, notes 
+and caveats, tests, etc. can now be accessed in our documentation on 
+readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
 
 ---
 This work is supported by NASA grant No. 80NSSC21K0885.
```

### Comparing `pdr-1.0.6/README.md` & `pdr-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
-(under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](docs/supported_datasets.md) 
+(under PDS3 or PDS4) should be covered eventually. 
+[Currently-supported datasets are listed here.](docs/supported_datasets.md) 
 
-If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
+If the software fails while attempting to read from datasets that we have 
+listed as supported, please submit an issue with a link to the file and 
+information about the error (if applicable). There might also be datasets that 
+work but are not listed. We would like to hear about those too. If a dataset 
+is not yet supported that you would like us to consider prioritizing, 
+[please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
 ### Attribution
 If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
 
 ### Installation
-_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
-You can do this like so: 
+_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) 
+installation into a `conda` environment. You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
 conda install -c conda-forge pdr
 ```
 The minimum supported version of Python is _3.9_.
@@ -25,24 +31,28 @@
 Using the conda install will install all dependencies in the environment.yml 
 file (both required and optional) for pdr. If you'd prefer to forego the 
 optional dependencies, please use minimal_environment.yml in your 
 installation. This is not supported through a direct conda install as 
 described above and will reqiore additional steps. Optional dependencies 
 and the added functionality they support are listed below:
 
-  - `pvl`: allows `Data.load("LABEL", as_pvl=True)` which will load PDS3 labels as `pvl` objects rather than plain text
+  - `pvl`: allows `Data.load("LABEL", as_pvl=True)`, which will load PDS3 
+     labels as `pvl` objects rather than plain text
   - `astropy`: adds support for FITS files
-  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter notebooks you create)
+  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter 
+     notebooks you create)
   - `pillow`: adds support for TIFF files and browse image rendering
-  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
+  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse 
+    function
 
 ### Usage
 
 You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main)
 
-Additional information on usage including examples, output data types, notes and caveats, test, etc. 
-can now be accessed in our documentation on readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
+Additional information on usage including examples, output data types, notes 
+and caveats, tests, etc. can now be accessed in our documentation on 
+readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
 
 ---
 This work is supported by NASA grant No. 80NSSC21K0885.
```

### Comparing `pdr-1.0.6/pdr/_patches/six_new.py` & `pdr-1.0.7/pdr/_patches/six_new.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/_patches/six_old.py` & `pdr-1.0.7/pdr/_patches/six_old.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/_scaling.py` & `pdr-1.0.7/pdr/_scaling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from numbers import Number
 from typing import Optional
 
 import numpy as np
 
 from pdr.datatypes import PDS3_CONSTANT_NAMES, IMPLICIT_PDS3_CONSTANTS
 from pdr.np_utils import casting_to_float
 from pdr.pdrtypes import PDRLike
 
 
-def find_special_constants(meta, obj, object_name):
+def find_special_constants(
+    meta: PDRLike, obj: np.ndarray, object_name: str
+) -> dict[str, Number]:
     """
-    attempts to find special constants in the associated object
-    by referencing the label and "standard" implicit special constant
-    values, then populates self.special_constants as appropriate.
+    attempts to find special constants in an ndarray associated with a PDS3
+    object by referencing the label and "standard" special constant values.
     """
-    #TODO: doesn't do anything for PDS4 products at present. Also, we
-    # need an attribute for distinguishing PDS3 from PDS4 products.
-
+    # NOTE: doesn't do anything for PDS4 products at present, although this
+    #  may not be important; usually pds4_tools handles it.
     block = meta.metablock_(object_name)
     # check for explicitly-defined special constants
     specials = {
         name: block[name]
         for name in PDS3_CONSTANT_NAMES
         if (name in block.keys()) and not (block[name] == "N/A")
     }
```

### Comparing `pdr-1.0.6/pdr/browsify.py` & `pdr-1.0.7/pdr/browsify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """functions for producing browse versions of products"""
+from numbers import Number
 from pathlib import Path
 import pickle
-from typing import Any, Sequence, Union, Optional
+from typing import Any, Optional, Sequence, Union
 import warnings
 
 from dustgoggles.func import naturals
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 
-def find_masked_bounds(image, cheat_low, cheat_high):
+def find_masked_bounds(
+    image: np.ma.MaskedArray, cheat_low: int, cheat_high: int
+) -> tuple[Optional[Number], Optional[Number]]:
     """
     relatively memory-efficient way to perform bound calculations for
     normalize_range on a masked array.
     """
     valid = image[~image.mask].data
     if valid.size == 0:
         return None, None
@@ -35,27 +38,31 @@
     else:
         minimum = valid.min()
         maximum = valid.max()
     return minimum, maximum
 
 
 # noinspection PyArgumentList
-def find_unmasked_bounds(image, cheat_low, cheat_high):
+def find_unmasked_bounds(
+    image: np.ndarray, cheat_low: int, cheat_high: int
+) -> tuple[Number, Number]:
     """straightforward way to find unmasked array bounds for normalize_range"""
     if cheat_low != 0:
         minimum = np.percentile(image, cheat_low).astype(image.dtype)
     else:
         minimum = image.min()
     if cheat_high != 0:
         maximum = np.percentile(image, 100 - cheat_high).astype(image.dtype)
     else:
         maximum = image.max()
     return minimum, maximum
 
 
+# NOTE: the following two functions are sort-of-vendored from
+# marslab.imgops.imgutils.
 def normalize_range(
     image: np.ndarray,
     bounds: Sequence[int] = (0, 1),
     clip: Union[float, tuple[float, float]] = 0,
     inplace: bool = False,
 ) -> np.ndarray:
     """
@@ -114,15 +121,15 @@
         np.uint8
     )
 
 
 def colorfill_maskedarray(
     masked_array: np.ma.MaskedArray,
     color: Union[int, tuple[int, int, int]] = (0, 255, 255),
-):
+) -> np.ndarray:
     """
     masked_array: 2-D masked array or a 3-D masked array with last axis of
     length 3. for likely uses, this should probably be 8-bit unsigned integer.
     color: optionally-specified RGB color (default cyan)
     return a 2-D or 3-D array with masked values filled with color.
     """
     if isinstance(color, int):
@@ -132,15 +139,15 @@
     if masked_array.shape[-1] != 3:
         raise ValueError("3-D arrays must have last axis of length = 3")
     return np.dstack(
         [masked_array[:, :, ix].filled(color[ix]) for ix in range(3)]
     )
 
 
-def browsify(obj: Any, outbase: Union[str, Path], **dump_kwargs):
+def browsify(obj: Any, outbase: Union[str, Path], **dump_kwargs) -> None:
     """
     attempts to dump a browse version of a data object, writing it into a file
     type that can be opened with desktop software: .jpg for most arrays, .csv
     for tables, .txt for most other things. if it can't find a reasonable
     translation, it dumps as .pkl (pickled binary blob).
     """
     outbase = str(outbase)
@@ -175,17 +182,22 @@
     else:
         # this should usually work. it may need another backup binary blob
         # pickler for really weird binary objects.
         with open(outbase + ".txt", "w") as stream:
             stream.write(str(obj))
 
 
+# TODO: this needs to be like 'browsify_structured_array' to handle some
+#  nested dtypes that aren't recarrays.
 def _browsify_recarray(obj: np.recarray, outbase: str, **_):
-    """some tabular data with column groups ends up as numpy recarray, which is
-    challenging to turn into a useful .csv file in some cases"""
+    """
+    Some tabular data with column groups ends up as numpy recarray, which is
+    challenging to turn into a useful .csv file in some cases. This _tries_ to
+    save it as a CSV file, and if it fails, punts and pickles it.
+    """
     try:
         obj = pd.DataFrame.from_records(obj)
         # noinspection PyTypeChecker
         obj.to_csv(outbase + ".csv")
     except ValueError:
         pickle.dump(obj, open(outbase + "_nested_recarray.pkl", "wb"))
 
@@ -197,43 +209,55 @@
     image_clip: Union[float, tuple[float, float]] = (1, 1),
     mask_color: Optional[tuple[int, int, int]] = (0, 255, 255),
     band_ix: Optional[int] = None,
     save: bool = True,
     override_rgba: bool = False,
     image_format: str = "jpg",
     **_,
-):
+) -> list[Optional[Image]]:
     """
-    attempt to save array as one or more images
+    Attempt to render (and optionally save) an ndarray as one or more
+    images.
     """
     if len(obj.shape) == 3:
         obj = _format_multiband_image(obj, band_ix, override_rgba)
     if not isinstance(obj, tuple):
-        return _render_and_save(
+        return _render_array(
             obj, outbase, purge, image_clip, mask_color, save, image_format
         )
     results = []
     for ix, band in enumerate(obj):
-        result = _render_and_save(
+        result = _render_array(
             band,
             f"{outbase}_{ix}",
             purge,
             image_clip,
             mask_color,
             save,
             image_format,
         )
         results.append(result)
     return results
 
 
-def _render_and_save(
-    obj, outbase, purge, image_clip, mask_color, save, image_format
-):
-    """"""
+def _render_array(
+    obj: np.ndarray,
+    outbase: str,
+    purge: bool,
+    image_clip: Union[float, tuple[float, float]],
+    mask_color: Union[int, tuple[int, int, int]],
+    save: bool,
+    image_format: str
+) -> Optional[Image]:
+    """
+    Handler function for array-rendering pipeline, used by `browsify()` on
+    most ndarrays and by `show()` always. Render an ndarray as a PIL Image,
+    optionally clipping and masking it. If `save` is True, save it to disk;
+    if False, return it.
+    """
     # upcast integer data types < 32-bit to prevent unhelpful wraparound
     if (obj.dtype.char in np.typecodes["AllInteger"]) and (obj.itemsize <= 2):
         obj = obj.astype(np.int32)
     # convert to unsigned eight-bit integer to make it easy to write
     obj = eightbit(obj, image_clip, purge)
     # unless color_fill is set to None, fill masked elements -- probably
     # special constants -- with RGB value defined by mask_color
@@ -307,19 +331,22 @@
             f"band_ix={band_ix} does not exist, dumping band {middle_ix}"
         )
         return obj[middle_ix]
 
 
 def save_sparklines(
     df: pd.DataFrame,
-    outbase,
+    outbase: str,
     sparkline_column_key=lambda c: "spectrum" in c.lower(),
     orientation="rows",
 ):
-    """"""
+    """
+    Experimental function to render a DataFrame that represents time-series
+    samples as sparklines. Mostly doesn't work.
+    """
     from matplotlib import pyplot as plt
 
     sparkframe = (
         df[[c for c in df.columns if sparkline_column_key(c)]]
         .copy()
         .reset_index(drop=True)
     )
```

### Comparing `pdr-1.0.6/pdr/datatypes.py` & `pdr-1.0.7/pdr/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 """
 definitions of sample types / data types / dtypes / ctypes, file formats
 and extensions, associated special constants, and so on.
 """
-import re
+from __future__ import annotations
 from itertools import product
+import re
 from types import MappingProxyType
+from typing import TYPE_CHECKING
 
 from pdr.utils import read_hex
 
+if TYPE_CHECKING:
+    from pdr.pdrtypes import ByteOrder
+
 
-def integer_bytes(
-    endian: str, signed: bool, sample_bytes: int, for_numpy: bool = False
+def integer_code(
+    byteorder: ByteOrder,
+    signed: bool,
+    sample_bytes: int,
+    for_numpy: bool = False
 ) -> str:
     """
-    translation for inconsistent integer types
+    Translation from integer width, signedness, and byteorder to struct or
+    numpy dtype string.
     """
     # TODO: add struct letter for longlong
     if sample_bytes == 4:
         letter = "l"
     elif sample_bytes == 2:
         letter = "h"
     else:
         letter = "b"
     if signed is False:
         letter = letter.upper()
     if for_numpy is True and sample_bytes in (4, 8):
         letter = f"i{sample_bytes}" if signed is True else f"u{sample_bytes}"
 
-    return f"{endian}{letter}"
+    return f"{byteorder}{letter}"
 
 
-def determine_byte_order(sample_type):
-    """"""
+def determine_byte_order(sample_type: str) -> ByteOrder:
+    """defines generic byte order for PDS3 physical data types"""
     if any(sample_type.startswith(s) for s in ("PC", "LSB", "VAX")):
-        endian = "<"
-    else:
-        endian = ">"
-    return endian
+        return "<"
+    return ">"
 
 
 def sample_types(
     sample_type: str, sample_bytes: int, for_numpy: bool = False
 ) -> str:
     """
-    Defines a translation from PDS data types to Python struct or numpy dtype
-    format strings, using both the type and bytes specified (because the
-    mapping to type alone is not consistent across PDS3).
+    Defines a translation from PDS3 physical data types to Python struct or
+    numpy dtype format strings, using both the type and byte width specified
+    (because the mapping to type alone is not consistent across PDS3).
     """
     sample_type = sample_type.replace(" ", "_")
     if (("INTEGER" in sample_type) or (sample_type == "BOOLEAN")) and (
         "ASCII" not in sample_type
     ):
         endian = determine_byte_order(sample_type)
         signed = "UNSIGNED" not in sample_type
-        return integer_bytes(endian, signed, sample_bytes, for_numpy)
+        return integer_code(endian, signed, sample_bytes, for_numpy)
     void = "V" if for_numpy is True else "s"
     if sample_bytes == 8:
         _float = "d"
     elif sample_bytes == 4:
         _float = "f"
     elif "ASCII" in sample_type:
         _float = ""
@@ -101,59 +108,42 @@
         "VAX_REAL": f"<{_float}",
         "IBM_REAL": f">u{sample_bytes}",
         "EBCDIC": f"V{sample_bytes}",
         "EBCDIC_CHARACTER": f"V{sample_bytes}",
     }[sample_type]
 
 
-# "basic" PDS3 special constants
 PDS3_CONSTANT_NAMES = (
     "INVALID_CONSTANT",
     "MISSING_CONSTANT",
     "INFINITY_CONSTANT",
     "NOT_APPLICABLE_CONSTANT",
     "NULL_CONSTANT",
     "UNKNOWN_CONSTANT",
 )
-# some (all?) of these are derived from ISIS properties; these are names they
-# take on when they are made explicit in a PDS3 label
+"""basic" PDS3 special constant parameter names"""
+
 PDS3_ISIS_CONSTANT_NAMES = tuple(
     [
         f"{category}{direction}{entity}{prop}"
         for category, direction, entity, prop in product(
             ("CORE_", "BAND_SUFFIX_", "SAMPLE_SUFFIX_", "LINE_SUFFIX_", ""),
             ("HIGH_", "LOW_", ""),
             ("INST_", "REPR_", ""),
             ("NULL", "SATURATION", "SAT"),
         )
     ]
 )
+"""
+some (all?) of these special constants are derived from ISIS properties; these 
+are names they take on when they are made explicit in a PDS3 label
+"""
+
 # noinspection PyTypeChecker
 PDS3_CONSTANT_NAMES = tuple(PDS3_ISIS_CONSTANT_NAMES + PDS3_CONSTANT_NAMES)
-# this dictionary contains common "implicit" (not specified in the label)
-# special constants. the keys of the dictionary are bits per array element.
-# some of these constants are derived from ISIS, others are suggested in the
-# PDS3 Standards.
-# note that the Standards allow other special constants to exist, undefined in
-# the label, determined only by the operating environment of the data provider,
-# so there can be no guarantee that other special constants do not exist in
-# any particular product.
-# the "implicit" use of ISIS constants may in fact be illegal, but appears
-# common. also note that some ISIS values collide with Standards-specified
-# N/A / UNK / NULL values -- again, we have no way to automatically
-# distinguish them, and interpret them as the Standards values when found.
-# References:
-# PDS3 Standards Reference v3.8, p.172
-# (https://pds.nasa.gov/datastandards/pds3/standards/sr/StdRef_20090227_v3.8.pdf)
-# GDAL PDS3 driver
-# TODO: -32768 is noted in this driver as NULL but defined in the Standards as
-#   an N/A value -- should clarify
-# (https://github.com/OSGeo/gdal/blob/master/frmts/pds/pdsdataset.cpp)
-# ISIS special pixel values
-# (https://isis.astrogeology.usgs.gov/Object/Developer/_special_pixel_8h_source.html)
 
 
 # TODO: make all the dicts nested in this into MappingProxyTypes
 IMPLICIT_PDS3_CONSTANTS = MappingProxyType(
     {
         # we define the uint8 constants but do not by default use them: they
         # are simply too problematic in too many cases.
@@ -211,7 +201,35 @@
         #  I'm not sure when we explicitly read doubles out
         #  of PDS3 objects anyway?
         "float64": {
             "NULL": -3.4028226550889044521e38,
         },
     }
 )
+"""
+This constant defines common "implicit" (not specified in the label) PDS3
+special constants. Its keys are bits per array element.
+Some of these constants are derived from ISIS (although sometimes used in 
+products that were not generated by ISIS!); others are suggested in the PDS3 
+Standards.
+
+Note that the Standards specifically permit other special constants to exist, 
+undefined in the label, and determined only by the operating environment of 
+the data provider, so there can be no guarantee that other special constants 
+do not exist in any particular product.
+
+The "implicit" use of ISIS constants may in fact be illegal, but appears
+common. also note that some ISIS values collide with Standards-specified N/A / 
+UNK / NULL values -- again, we have no way to automatically distinguish them, 
+and interpret them as the Standards values when we find them unless a label
+specifically states otherwise.
+
+References:
+PDS3 Standards Reference v3.8, p.172
+(https://pds.nasa.gov/datastandards/pds3/standards/sr/StdRef_20090227_v3.8.pdf)
+GDAL PDS3 driver
+TODO: -32768 is noted in this driver as NULL but defined in the Standards as
+  an N/A value -- should clarify
+(https://github.com/OSGeo/gdal/blob/master/frmts/pds/pdsdataset.cpp)
+ISIS special pixel values
+(https://isis.astrogeology.usgs.gov/Object/Developer/_special_pixel_8h_source.html)
+"""
```

### Comparing `pdr-1.0.6/pdr/formats/__init__.py` & `pdr-1.0.7/pdr/formats/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-"""This module contains special case formats for nonconforming or malformatted data
-types organized by mission and/or instrument. The `checkers` module consists of functions
-that are called by `pdr.func.specialize` to determine if a given file meets the stated criteria.
-If a file meets the criteria in the checker, a file from the respective special case formats
-module is returned. If not, the base pdr workflow is continued."""
+"""
+This module implements a wide variety of special-case behaviors for
+nonconforming or malformatted data products. It implements these behaviors as
+functions in distinct submodules organized by 'dataset' (mission, instrument,
+etc.); the `checkers` submodule contains dispatch functions that preempt
+generic behaviors and redirect them to functions from one of the dataset
+submodules. See the documentation for `checkers` for details on this behavior.
+"""
 
 from .checkers import *
 import pdr.formats.cassini as cassini
 import pdr.formats.clementine as clementine
 import pdr.formats.dawn as dawn
 import pdr.formats.diviner as diviner
 import pdr.formats.epoxi as epoxi
```

### Comparing `pdr-1.0.6/pdr/formats/cassini.py` & `pdr-1.0.7/pdr/formats/mex.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,168 @@
-import warnings
-from pathlib import Path
+from pdr.loaders.queries import table_position
 
-import os
 
-import pdr.loaders.queries
-from pdr.loaders.utility import tbd
-from pdr.loaders._helpers import count_from_bottom_of_file
-from pdr.loaders.queries import table_position
+def marsis_get_position(identifiers, block, target, name, start_byte):
+    """
+    HITS
+    * mex_marsis
+        * TEC_EDR
+    """
+    table_props = table_position(identifiers, block, target, name, start_byte)
+    n_records = identifiers["FILE_RECORDS"]
+    record_bytes = 143
+    table_props["length"] = n_records * record_bytes
+    return table_props
 
 
-def spreadsheet_loader(filename, fmtdef_dt, data_set_id):
-    """"""
+def aspera_table_loader(filename, fmtdef_dt):
+    """
+    The ASPERA IMA EDRs are ascii csv tables containing 2 data types: SENSOR
+    and MODE. The VALUES column is repeated and has 96 items total. In the MODE
+    rows only the first VALUES item contains data, and should be followed by 95
+    'missing' items.
+    In reality these rows have 96 empty/missing items because of an extra
+    comma. This special case cuts off the extra column during the pd.read_csv()
+    call.
+
+    HITS
+    * mex_aspera
+        * ima
+    """
     import pandas as pd
-
-    if "UNCALIB" in data_set_id:
-        return pd.read_csv(filename)
+    
     fmtdef, dt = fmtdef_dt
-    names = fmtdef.NAME
-    header = None
-    if "FULL" in filename:
-        skiprows = 4
-        if data_set_id == "CO-S-MIMI-4-CHEMS-CALIB-V1.0":
-            header = 0
-            names = None
-            skiprows = range(1, 4)
-    elif data_set_id == "CO-SSA-RADAR-3-ABDR-SUMMARY-V1.0":
-        skiprows = 0
-    else:
-        skiprows = 7
-    table = pd.read_csv(
-        filename, header=header, skiprows=skiprows, names=names
-    )
+    table = pd.read_csv(filename, header=None,
+                        usecols=range(len(fmtdef.NAME.tolist())))
+    assert len(table.columns) == len(fmtdef.NAME.tolist())
+    table.columns = fmtdef.NAME.tolist()
     return table
 
 
-def get_structure(block, name, filename, data, identifiers):
-    """"""
-    # the data type that goes here double defines the 32 byte prefix/offset.
-    # By skipping the parse_table_structure we never add the prefix bytes so
-    # it works as is. (added HASI/HUY if block after this comment)
-    fmtdef = pdr.loaders.queries.read_table_structure(
+def aspera_ima_ddr_structure(block, name, filename, data, identifiers):
+    """
+    The ASPERA IMA DDR table opens correctly as written in its label, but
+    the BYTES values for columns 3 and 4 are wrong.
+
+    HITS
+    * mex_aspera
+        * ima_ddr
+    """
+    from pdr.loaders.queries import read_table_structure
+
+    fmtdef = read_table_structure(
         block, name, filename, data, identifiers
     )
-    if ("HASI" in filename) or ("HUY_DTWG_ENTRY_AERO" in filename):
-        if "HUY_DTWG_ENTRY_AERO" in filename:
-            fmtdef.at[
-                5, "NAME"
-            ] = "KNUDSEN FREESTR. HARD SPHERE NR. [=2.8351E-8/RHO]"
-            fmtdef.at[6, "NAME"] = "KNUDSEN NR. [=1.2533*SQRT(2)*Ma/Re]"
-            fmtdef.at[7, "NAME"] = "REYNOLD NR. [=RHO*VREL*D/Mu]"
-        dt = None
-    else:
-        from pdr.pd_utils import insert_sample_types_into_df, compute_offsets
-
-        fmtdef = compute_offsets(fmtdef)
-        fmtdef, dt = insert_sample_types_into_df(fmtdef, identifiers)
-    return fmtdef, dt
-
-
-def looks_like_ascii(data, pointer):
-    """"""
-    return (
-        ("SPREADSHEET" in pointer)
-        or ("ASCII" in pointer)
-        or (data.metablock(pointer).get("INTERCHANGE_FORMAT") == "ASCII")
-    )
-
+    fmtdef.at[2, "BYTES"] = 12
+    fmtdef.at[3, "BYTES"] = 12
+    return fmtdef, None
+
+
+def pfs_edr_special_block(data, name):
+    """
+    The PFS EDRs have a few errors in their labels prior to orbit 8945, after
+    which they are corrected.
+
+    HITS
+    * mex_marsis
+        * raw_lwc
+        * raw_swc
+        * cal_lwc
+        * cal_swc
+        * hk_early_mission
+    """
+    block = data.metablock_(name)
+    orbit_number = data.metaget_("ORBIT_NUMBER")
+    
+    if orbit_number == "N/A" or int(orbit_number) < 8945:
+        # Fixes the number of rows in the table by replacing ROWS with
+        # FILE_RECORDS.
+        block["ROWS"] = data.metaget_("FILE_RECORDS")
+        # Replaces the time columns' DATA_TYPEs with the correct type based on
+        # products created later in the mission.
+        for item in iter(block.items()):
+            if "COLUMN" in item:
+                if item[1]["NAME"] == "OBT OBSERVATION TIME":
+                    item[1]["DATA_TYPE"] = "PC_REAL"
+                if item[1]["NAME"] == "SCET OBSERVATION TIME":
+                    item[1]["DATA_TYPE"] = "PC_UNSIGNED_INTEGER"
+        return True, block
+    return False, block
+
+def spicam_rdr_hdu_name(data, identifiers, fn, name):
+    """
+    The SPICAM RDRs have multiple fits HDUs per product. The HDU indexing is
+    off by 1 because the first QUBE pointer shares the '0' HDU index with the
+    HEADER pointer.
+    
+    HITS
+    * mex_spicam
+        * ir_rdr
+        * uv_rdr
+    """
+    from pdr.loaders.queries import get_fits_id
+    
+    if name == "HEADER":
+        return 0
+    return get_fits_id(data, identifiers, fn, name, other_stubs=None)[0] - 1
 
-def get_position(identifiers, block, target, name, filename, start_byte):
-    if "IR_" in filename:
-        tbd(name, block)
+def mrs_ddr_atmo_position(identifiers, block, target, name, start_byte):
+    """
+    The MRS derived atmosphere profiles were opening with data cut off at the
+    ends of the tables. Recalculating the table length with ROW_BYTES = 278
+    instead of 276 fixes it.
+
+    HITS
+    * mex_mrs
+        * occ_atmo
+    """
     table_props = table_position(identifiers, block, target, name, start_byte)
-    n_records = identifiers["ROWS"]
-    if any(sub in filename for sub in ["ULVS_DDP", "DLIS_AZ_DDP", "DLV_DDP"]):
-        record_bytes = identifiers["ROW_BYTES"]
-    else:
-        record_bytes = identifiers["ROW_BYTES"] + 1
-    length = n_records * record_bytes
-    if name == "HEADER":
-        tab_size = length
-        if isinstance(filename, list):
-            filename = filename[0]
-        file = Path(filename)
-        file_size = os.path.getsize(file)
-        length = file_size - tab_size
-        start = 0
-        table_props["start"] = start
-    table_props["length"] = length
+    row_bytes = 278
+    table_props["length"] = row_bytes * block["ROWS"]
     return table_props
 
+def mrs_get_position(identifiers, block, target, name, start_byte):
+    """
+    MRS ICL level 1b DOPPLER_TABLEs and ODF level 2 RANGING_TABLEs undercount
+    ROW_BYTES by 1.
+
+    HITS
+    * mex_mrs
+        * lvl_1b_icl (partial)
+        * lvl_2_odf (partial)
+    """
+    table_props = table_position(identifiers, block, target, name, start_byte)
+    row_bytes = block["ROW_BYTES"] + 1
+    table_props["length"] = row_bytes * block["ROWS"]
+    return table_props
 
-def get_offset(filename, identifiers):
-    """"""
-    if any(sub in filename for sub in ["ULVS_DDP", "DLIS_AZ_DDP", "DLV_DDP"]):
-        row_bytes = identifiers["ROW_BYTES"]
-    else:
-        row_bytes = identifiers["ROW_BYTES"] + 1
-    rows = identifiers["ROWS"]
-    start_byte = count_from_bottom_of_file(
-        filename, rows, row_bytes=row_bytes
-    )
-    return True, start_byte
-
-
-def trivial_loader(pointer):
-    """"""
-    warnings.warn(
-        f"The Cassini ISS EDR/calibration {pointer} tables are not currently "
-        f"supported."
-    )
-    return True
-
-
-def cda_table_filename(data):
-    """"""
-    label = Path(data.labelname)
-    return True, Path(label.parent, f"{label.stem}.TAB")
+def mrs_l1b_odf_table_loader(filename, fmtdef_dt):
+    """
+    MRS level 1b ODF labels have variable and sometimes incorrect ROW_BYTES
+    values.
+
+    HITS
+    * mex_mrs
+        * lvl_1b_odf
+    """
+    import pandas as pd
 
+    fmtdef, dt = fmtdef_dt
+    table = pd.read_csv(filename, header=None, sep=r"\s+")
+    table.columns = [
+        f for f in fmtdef['NAME'] if not f.startswith('PLACEHOLDER')
+    ]
+    return table
 
-# TODO: find a way to point find_special_constants at this so we can write
-#  scaled versions of these images
-def xdr_redirect_to_image_block(data):
-    """"""
-    object_name = "IMAGE"
+def mrs_l1b_odf_rmp_redirect(data):
+    """
+    RMP tables are a subset of MRS level 1b ODFs that were not opening because
+    their pointer and object names do not match.
+    
+    HITS:
+    * mex_mrs
+        * lvl_1b_odf (partial)
+    """
+    object_name = "RAMP_TABLE"
     block = data.metablock_(object_name)
     return block
 
-
-def get_special_qube_band_storage():
-    """"""
-    band_storage_type = "BAND_SEQUENTIAL"
-    return True, band_storage_type
```

### Comparing `pdr-1.0.6/pdr/formats/checkers.py` & `pdr-1.0.7/pdr/formats/checkers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,114 @@
+"""
+This module contains functions that preempt generic metadata- or data-parsing
+behaviors. They are intended to manage idiosyncracies common to all products
+of a particular type (or even all products in a whole dataset), including but
+not limited to:
+
+* Malformatted labels
+* Incorrect metadata
+* Malformatted data
+* Technically correct but extremely unusual data formatting
+
+To put this another way, they facilitate single-dispatch polymorphism on the
+semantic level of data product type.
+
+Most functions in this file are intended to be applied by `func.specialize`
+as wrappers to other functions, typically a query function in `loaders.queries`
+or the `loader_function` attribute of a `loaders.queries.Loader` subclass.
+However, this is not strict; they may also wrap functions in other
+modules, and functions may call them inline rather than use them as wrappers.
+
+Every function in this module should be named `check_special_{something}`,
+where 'something' clearly designates the metadata-parsing or data-loading
+behavior it may sometimes preempt.
+
+Most functions in this module should return a tuple whose first element is a
+`bool` and whose second element is the "special" value. If the first element
+is `True`, it means that there is a relevant special case, so the caller
+should use the "special" value instead of engaging in its normal behavior; if
+it is `False`, there is no relevant special case and the caller should continue
+with its normal behavior. The second element of the tuple should always be
+`None` if the first element is `False`.
+
+If the function is intended to wrap a generic function, the second element of
+this tuple, when not None, must always share the return type of that generic
+function. Also, if it is intended for the `func.softquery()` workflow, it
+should follow that workflow's argument naming and type annotation conventions.
+
+Exceptions to these naming and signature conventions can be made for checkers
+designed specifically to be called inline of a specific handler function.
+"""
+
 from __future__ import annotations
+from pathlib import Path
 import re
-from typing import TYPE_CHECKING, Optional
+from typing import Any, Mapping, Optional, TYPE_CHECKING, Union
+
+from multidict import MultiDict
 
 from pdr import formats
 from pdr.loaders.utility import is_trivial
 
 if TYPE_CHECKING:
-    from pdr.pdrtypes import PDRLike
+    import pandas as pd
+    import numpy as np
+    from pdr.pdrtypes import DataIdentifiers, PDRLike, PhysicalTarget
 
 
 def check_special_offset(
-    name: str, data: PDRLike, identifiers: dict, fn
+    name: str, data: PDRLike, identifiers: DataIdentifiers, fn: str
 ) -> tuple[bool, Optional[int]]:
-    """"""
+    """
+    Preempt generic inference of an object's byte offset within a file. Wraps
+    `loaders.queries.data_start_byte()`.
+    """
     # these incorrectly specify object length rather than
     # object offset in the ^HISTOGRAM pointer target
     if identifiers["INSTRUMENT_ID"] == "CHEMIN":
         return formats.msl_cmn.get_offset(name)
-    if identifiers["DATA_SET_ID"] == "CLEM1-L-RSS-5-BSR-V1.0" and name in (
-        "HEADER_TABLE",
-        "DATA_TABLE",
+    if (
+        identifiers["DATA_SET_ID"] == "CLEM1-L-RSS-5-BSR-V1.0"
+        and re.match("(HEADER|DATA)_TABLE", name)
     ):
         # sequence wrapped as string for object names
         return formats.clementine.get_offset(data, name)
     if identifiers["INSTRUMENT_ID"] == "THEMIS" and name == "QUBE":
         return formats.themis.get_qube_offset(data)
+    disrsubs = re.compile(r"STRIP|VISIBL|IMAGE|IR_|TIME|SUN|SOLAR")
     if (
         identifiers["INSTRUMENT_NAME"] == "DESCENT IMAGER SPECTRAL RADIOMETER"
-        and (identifiers["PRODUCT_TYPE"] == "RDR")
-        or any(
-            sub in identifiers["FILE_NAME"]
-            for sub in [
-                "STRIP",
-                "VISIBL",
-                "IMAGE",
-                "IR_",
-                "TIME",
-                "SUN",
-                "SOLAR",
-            ]
-        )
+        and identifiers["PRODUCT_TYPE"] == "RDR"
+        or disrsubs.search(identifiers["FILE_NAME"])
     ):
         return formats.cassini.get_offset(fn, identifiers)
     if (
         identifiers["INSTRUMENT_ID"] == "CRAT"
         and identifiers["PRODUCT_TYPE"] == "EDR"
         and name == "TABLE_1"
     ):
         return formats.lro.get_crater_offset()
     if (
         identifiers["DATA_SET_ID"] == "PHX-M-MECA-4-NIRDR-V1.0"
-         and identifiers["PRODUCT_TYPE"] in ("MECA_WCL_CP",
-                                             "MECA_WCL_CV")
-         and "TABLE" in name
+        and identifiers["PRODUCT_TYPE"] in ("MECA_WCL_CP", "MECA_WCL_CV")
+        and "TABLE" in name
     ):
         return formats.phoenix.wcl_rdr_offset(data, name)
     return False, None
 
 
 def check_special_table_reader(
-    identifiers, name, fn, fmtdef_dt, block, start_byte
+    identifiers: DataIdentifiers,
+    name: str,
+    fn: str,
+    fmtdef_dt: tuple[pd.DataFrame, np.dtype],
+    block: MultiDict,
+    start_byte: int,
 ):
-    """"""
+    """Preempt loaders.datawrap.ReadTable's dispatch to `read_table()`."""
     if identifiers["DATA_SET_ID"] in (
         "CO-S-MIMI-4-CHEMS-CALIB-V1.0",
         "CO-S-MIMI-4-LEMMS-CALIB-V1.0",
         "CO-S-MIMI-4-INCA-CALIB-V1.0",
         "CO-E/J/S/SW-MIMI-2-LEMMS-UNCALIB-V1.0",
         "CO-SSA-RADAR-3-ABDR-SUMMARY-V1.0",
     ):
@@ -105,15 +148,15 @@
             "CAL_DATA.TAB" in identifiers["PRODUCT_ID"]
             or "G_DATA.TAB" in identifiers["PRODUCT_ID"]
             or "R_DATA.TAB" in identifiers["PRODUCT_ID"]
         )
     ):
         return True, formats.mgn.geom_table_loader(fn, fmtdef_dt)
     if (
-        str(identifiers["DATA_SET_ID"]).startswith("MGN-V-RSS-5-OCC-PROF")
+        identifiers["DATA_SET_ID"].startswith("MGN-V-RSS-5-OCC-PROF")
         and name == "TABLE"
     ):
         return True, formats.mgn.occultation_loader(
             identifiers, fmtdef_dt, block, fn
         )
     if (
         identifiers["INSTRUMENT_ID"] == "DLRE"
@@ -146,64 +189,81 @@
         )
     if (
         identifiers["DATA_SET_ID"] == "IHW-C-IRFCURV-3-EDR-HALLEY-V2.0"
         and name == "TABLE"
     ):
         return True, formats.ihw.curve_table_loader(fn, fmtdef_dt)
     if (
-        identifiers["DATA_SET_ID"] in (
+        identifiers["DATA_SET_ID"]
+        in (
             "IHW-C-PPFLX-3-RDR-HALLEY-V1.0",
             "IHW-C-PPOL-3-RDR-HALLEY-V1.0",
             "IHW-C-PPSTOKE-3-RDR-HALLEY-V1.0",
             "IHW-C-PPMAG-3-RDR-HALLEY-V1.0",
             "IHW-C-MSNRDR-3-RDR-HALLEY-ETA-AQUAR-V1.0",
             "IHW-C-MSNRDR-3-RDR-HALLEY-ORIONID-V1.0",
             "IHW-C-MSNVIS-3-RDR-HALLEY-ETA-AQUAR-V1.0",
             "IHW-C-MSNVIS-3-RDR-HALLEY-ORIONID-V1.0",
             "IHW-C-IRFTAB-3-RDR-HALLEY-V1.0",
             "IHW-C-IRPOL-3-RDR-HALLEY-V1.0",
             "IHW-C-IRPHOT-3-RDR-HALLEY-V1.0",
-        ) and name == "TABLE"
+        )
+        and name == "TABLE"
     ):
         return True, formats.ihw.add_newlines_table_loader(
             fmtdef_dt, block, fn, start_byte
         )
     if (
         identifiers["DATA_SET_ID"] == "VG1-J-LECP-4-SUMM-SECTOR-15MIN-V1.1"
         and name == "TABLE"
     ):
         return True, formats.voyager.lecp_table_loader(fn, fmtdef_dt)
-    if (
-        identifiers["DATA_SET_ID"] == "VL2-M-SEIS-5-RDR-V1.0"
-        and name in ("TABLE", "SPREADSHEET")
+    if identifiers["DATA_SET_ID"] == "VL2-M-SEIS-5-RDR-V1.0" and name in (
+        "TABLE",
+        "SPREADSHEET",
     ):
         return True, formats.viking.seis_table_loader(fn, fmtdef_dt)
     if (
         "MEX-M-ASPERA3-2-EDR-IMA" in identifiers["DATA_SET_ID"]
         and name == "SPREADSHEET"
     ):
         return True, formats.mex.aspera_table_loader(fn, fmtdef_dt)
     if (
-        identifiers["DATA_SET_ID"] in ("MER1-M-RSS-1-EDR-V1.0",
-                                       "MER2-M-RSS-1-EDR-V1.0",)
+        re.match(r"MER[12]-M-RSS-1-EDR-V1.0", identifiers["DATA_SET_ID"])
         and identifiers["PRODUCT_TYPE"] == "UHFD"
         and name == "SPREADSHEET"
     ):
         return True, formats.mer.rss_spreadsheet_loader(fn, fmtdef_dt)
     if (
         identifiers["DATA_SET_ID"] == "PHX-M-MECA-4-NIRDR-V1.0"
         and identifiers["INSTRUMENT_ID"] == "MECA_AFM"
         and "TABLE" in name
     ):
         return True, formats.phoenix.afm_table_loader(fn, fmtdef_dt, name)
+    if (
+        identifiers["INSTRUMENT_HOST_NAME"] == "MARS EXPRESS"
+        and identifiers["INSTRUMENT_ID"] == "MRS"
+        and all(x in identifiers["PRODUCT_ID"] for x in ["ODF","L1B"])
+        and "TABLE" in name
+    ):
+        return True, formats.mex.mrs_l1b_odf_table_loader(fn, fmtdef_dt)
     return False, None
 
 
-def check_special_structure(block, name, fn, identifiers, data):
-    """"""
+def check_special_structure(
+    name: str,
+    block: MultiDict,
+    fn: str,
+    data: PDRLike,
+    identifiers: DataIdentifiers
+) -> tuple[bool, Optional[tuple[pd.DataFrame, Optional[np.dtype]]]]:
+    """
+    Preempt generic ARRAY/TABLE/SPREADSHEET format definition parsing. Wraps
+    `parse_array_structure()` and `parse_table_structure()`.
+    """
     if (
         identifiers["DATA_SET_ID"] == "CLEM1-L-RSS-5-BSR-V1.0"
         and name == "DATA_TABLE"
     ):
         # sequence wrapped as string for object names
         return True, formats.clementine.get_structure(
             block, name, fn, data, identifiers
@@ -222,14 +282,15 @@
         identifiers.get("INSTRUMENT_HOST_NAME") == "MARS GLOBAL SURVEYOR"
         and identifiers.get("INSTRUMENT_NAME") == "RADIO SCIENCE SUBSYSTEM"
         and identifiers.get("PRODUCT_TYPE") == "ECS"
     ):
         return True, formats.mgs.get_ecs_structure(
             block, name, fn, data, identifiers
         )
+    # TODO: yikes
     if (
         identifiers["INSTRUMENT_HOST_NAME"] == "CASSINI ORBITER"
         and identifiers["INSTRUMENT_ID"] == "RPWS"
         and name == "TIME_SERIES"
     ) or (
         identifiers["INSTRUMENT_HOST_NAME"] == "HUYGENS PROBE"
         and (
@@ -240,17 +301,19 @@
             )
         )
     ):
         return True, formats.cassini.get_structure(
             block, name, fn, data, identifiers
         )
     if (
-        identifiers["DATA_SET_ID"] == "GP-J-NMS-3-ENTRY-V1.0"
-        or identifiers["DATA_SET_ID"] == "GP-J-ASI-3-ENTRY-V1.0"
-    ) and name == "TABLE":
+        re.match(
+            r"GP-J-(NMS|ASI)-3-ENTRY-V1.0", identifiers["DATA_SET_ID"]
+        )
+        and name == "TABLE"
+    ):
         return True, formats.galileo.probe_structure(
             block, name, fn, data, identifiers
         )
     if (
         identifiers["DATA_SET_ID"] == "GO-E-EPD-2-SAMP-PAD-V1.0"
         and identifiers["PRODUCT_ID"] == "E1PAD_7.TAB"
         and name == "TIME_SERIES"
@@ -264,39 +327,35 @@
         and name == "TABLE"
     ):
         return True, formats.vega.get_structure(
             block, name, fn, data, identifiers
         )
     if (
         "GIO-C-PIA-3-RDR-HALLEY-V1.0" == identifiers["DATA_SET_ID"]
-        or re.match(r"VEGA.-C-PUMA.*", str(identifiers["DATA_SET_ID"]))
+        or re.match(r"VEGA.-C-PUMA.*", identifiers["DATA_SET_ID"])
     ) and name == "ARRAY":
         return True, formats.vega.fix_array_structure(
             name, block, fn, data, identifiers
         )
     if (
-        (identifiers["DATA_SET_ID"] == "MRO-M-MCS-4-RDR-V1.0"
-        or identifiers["DATA_SET_ID"] == "MRO-M-MCS-2-EDR-V1.0")
+        re.match(r"MRO-M-MCS-(4-RDR|2-EDR)-V1.0", identifiers["DATA_SET_ID"])
         and name == "TABLE"
     ):
         return True, formats.mro.get_structure(
             block, name, fn, data, identifiers
         )
     if (
         identifiers["DATA_SET_ID"] == "VG2-SS-PLS-4-SUMM-1HR-AVG-V1.0"
         and name == "TABLE"
         and block["^STRUCTURE"] == "VGR_PLS_HR_2017.FMT"
     ):
         return True, formats.voyager.get_structure(
             block, name, fn, data, identifiers
         )
-    if (
-        "IHW-C-SPEC-" in identifiers["DATA_SET_ID"]
-        and name == "SPECTRUM"
-    ):
+    if "IHW-C-SPEC-" in identifiers["DATA_SET_ID"] and name == "SPECTRUM":
         return True, formats.ihw.get_structure(
             block, name, fn, data, identifiers
         )
     if (
         identifiers["DATA_SET_ID"] == "PHX-M-MECA-2-NIEDR-V1.0"
         and name == "TBL_TABLE"
         and block["CONTAINER"]["^STRUCTURE"] == "TBL_0_STATE_DATA.FMT"
@@ -318,44 +377,45 @@
     ):
         return True, formats.mex.aspera_ima_ddr_structure(
             block, name, fn, data, identifiers
         )
     return False, None
 
 
-def check_special_position(identifiers, block, target, name, fn, start_byte):
-    """"""
+def check_special_position(
+    identifiers: DataIdentifiers,
+    block: MultiDict,
+    target: PhysicalTarget,
+    name: str,
+    fn: str,
+    start_byte: int,
+) -> tuple[bool, Optional[int]]:
+    """
+    Preempt generic detection of a table's row or byte offset within a file.
+    Wraps `table_position()`. Used for table-specific cases that are partially
+    but not wholly handled by `data_start_byte()`, so should not be defined
+    in `check_special_offset()`.
+    """
     if (
         identifiers["INSTRUMENT_ID"] == "MARSIS"
         and " TEC " in identifiers["DATA_SET_NAME"]
     ):
         return True, formats.mex.marsis_get_position(
             identifiers, block, target, name, start_byte
         )
+    huysubs = re.compile(r"DARK|STRIP|VIS_EX|SUN|VISIBL|TIME|SOLAR|IMAGE")
     if (
         identifiers["INSTRUMENT_HOST_NAME"] == "HUYGENS PROBE"
-        and any(
-            sub in identifiers["FILE_NAME"]
-            for sub in [
-                "DARK",
-                "STRIP",
-                "VIS_EX",
-                "SUN",
-                "VISIBL",
-                "TIME",
-                "SOLAR",
-                "IMAGE",
-            ]
-        )
+        and huysubs.search(identifiers["FILE_NAME"])
         or (
             identifiers["INSTRUMENT_NAME"]
             == "DESCENT IMAGER SPECTRAL RADIOMETER"
             and identifiers["PRODUCT_TYPE"] == "RDR"
         )
-        and (name in ("TABLE", "HEADER"))
+        and name in ("TABLE", "HEADER")
     ):
         return True, formats.cassini.get_position(
             identifiers, block, target, name, fn, start_byte
         )
     if (
         identifiers["DATA_SET_ID"] == "LRO-L-RSS-1-TRACKING-V1.0"
         and name == "WEAREC_TABLE"
@@ -366,23 +426,51 @@
     if (
         identifiers["DATA_SET_ID"] == "DIF-C-HRIV/MRI-5-HARTLEY2-SHAPE-V1.0"
         and identifiers["PRODUCT_ID"] == "HARTLEY2-CARTESIAN-PLATE-MODEL"
         and "TABLE" in name
     ):
         return True, formats.epoxi.cart_model_get_position(
             identifiers, block, target, name, start_byte
-            )
+        )
+    if (
+        "MEX-M-MRS-5-OCC" in identifiers["DATA_SET_ID"]
+        and name == "ATM_TABLE"
+    ):
+        return True, formats.mex.mrs_ddr_atmo_position(
+            identifiers, block, target, name, start_byte
+        )
+    if (
+        identifiers["INSTRUMENT_HOST_NAME"] == "MARS EXPRESS"
+        and identifiers["INSTRUMENT_ID"] == "MRS"
+        and all(x in identifiers["PRODUCT_ID"] for x in ["ICL","L1B"])
+        and name == "DOPPLER_TABLE"
+    ):
+        return True, formats.mex.mrs_get_position(
+            identifiers, block, target, name, start_byte
+        )
+    if (
+        identifiers["INSTRUMENT_HOST_NAME"] == "MARS EXPRESS"
+        and identifiers["INSTRUMENT_ID"] == "MRS"
+        and all(x in identifiers["PRODUCT_ID"] for x in ["ODF","L02"])
+        and name == "RANGING_TABLE"
+    ):
+        return True, formats.mex.mrs_get_position(
+            identifiers, block, target, name, start_byte
+        )
     return False, None
 
 
 def check_special_sample_type(
-    identifiers: dict,
+    identifiers: DataIdentifiers,
     base_samp_info: dict,
 ) -> tuple[bool, Optional[str]]:
-    """"""
+    """
+    Preempt generic mapping of PDS3 data types to numpy dtype strings. Wraps
+    `image_sample_type()`; called inline by `insert_sample_types_into_df()`.
+    """
     if (
         identifiers["DATA_SET_ID"] == "JNO-J-JIRAM-3-RDR-V1.0"
         and identifiers.get("PRODUCT_TYPE", "") == "RDR"
     ):
         return True, formats.juno.jiram_rdr_sample_type()
     if (
         identifiers["INSTRUMENT_ID"] == "LROC"
@@ -407,46 +495,59 @@
         identifiers["DATA_SET_ID"] == "ULY-J-EPAC-4-SUMM-PHA-24HR-V1.0"
         and identifiers["PRODUCT_ID"].endswith("BIN")
     ):
         return formats.ulysses.get_sample_type(base_samp_info)
     return False, None
 
 
-def check_special_bit_column_case(identifiers: dict):
-    """"""
+def check_special_bit_column_case(
+    identifiers: Mapping[str, Any]
+) -> tuple[bool, Optional[str]]:
+    """
+    Special case checker used by `bit_handling.set_bit_string_data_type()`
+    to preempt generic data type inference.
+    """
     instrument = identifiers["INSTRUMENT_NAME"]
     if instrument in (
         "ALPHA PARTICLE X-RAYSPECTROMETER",
         "JOVIAN AURORAL PLASMA DISTRIBUTIONS EXPERIMENT",
         "CHEMISTRY AND MINERALOGY INSTRUMENT",
         "MARS ADVANCED RADAR FOR SUBSURFACE ANDIONOSPHERE SOUNDING",
     ):
         return True, "MSB_BIT_STRING"
     return False, None
 
 
 def check_special_bit_start_case(
     identifiers, list_of_pvl_objects_for_bit_columns, start_bit_list
-):
-    """"""
+) -> tuple[bool, Optional[list[int]]]:
+    """
+    Special case checker used by get_bit_start_and_size() to fix
+    incorrectly-defined bit offsets.
+    """
     if identifiers["INSTRUMENT_NAME"] in "JOVIAN INFRARED AURORAL MAPPER":
         return formats.juno.bit_start_find_and_fix(
             list_of_pvl_objects_for_bit_columns, start_bit_list
         )
     return False, None
 
 
-def check_special_block(name, data, identifiers):
-    """"""
+def check_special_block(
+    name: str, data: PDRLike, identifiers: Mapping
+) -> tuple[bool, Optional[MultiDict]]:
+    """
+    `specialize()` target for `queries.get_block()`. Intended for cases in
+    which label pointers don't correspond to label block names.
+    """
     if name == "XDR_DOCUMENT":
         return True, formats.cassini.xdr_redirect_to_image_block(data)
     if name == "CHMN_HSK_HEADER_TABLE":
         return True, formats.msl_cmn.fix_mangled_name(data)
     if (
-        str(identifiers["DATA_SET_ID"]).startswith("JNO-E/J/SS")
+        identifiers["DATA_SET_ID"].startswith("JNO-E/J/SS")
         and "BSTFULL" in identifiers["DATA_SET_ID"]
         and "FREQ_OFFSET_TABLE" in data.keys()
         and name in ("FREQ_OFFSET_TABLE", "DATA_TABLE")
     ):
         return True, formats.juno.waves_burst_fix_table_names(data, name)
     if (
         identifiers["INSTRUMENT_ID"] == "LAMP"
@@ -482,18 +583,15 @@
         return True, formats.galileo.epd_special_block(data, name)
     if (
         identifiers["INSTRUMENT_NAME"] == "PLASMA WAVE RECEIVER"
         and "SUMM" in identifiers["DATA_SET_ID"]
         and (name == "TIME_SERIES" or name == "TABLE")
     ):
         return True, formats.galileo.pws_special_block(data, name)
-    if (
-        "ULY-J-EPAC-4-SUMM" in identifiers["DATA_SET_ID"]
-        and name == "TABLE"
-    ):
+    if "ULY-J-EPAC-4-SUMM" in identifiers["DATA_SET_ID"] and name == "TABLE":
         return True, formats.ulysses.get_special_block(data, name, identifiers)
     if (
         "VG2-N-MAG-4-RDR-HGCOORDS" in identifiers["DATA_SET_ID"]
         and identifiers["STANDARD_DATA_PRODUCT_ID"] == "ASCII DATA"
         and name == "TABLE"
     ):
         return True, formats.voyager.mag_special_block(data, name)
@@ -509,54 +607,64 @@
         return formats.voyager.pls_fine_special_block(data, name)
     if (
         identifiers["DATA_SET_ID"] == "VG2-U-PLS-5-SUMM-IONBR-48SEC-V1.0"
         and identifiers["PRODUCT_ID"] == "SUMRY.DAT"
         and name == "TIME_SERIES"
     ):
         return formats.voyager.pls_ionbr_special_block(data, name)
-    if (
-        identifiers["DATA_SET_ID"] == "M9-M-IRIS-3-RDR-V1.0"
-        and (name == "SPECTRAL_SERIES"  # the data product
-             or "SPECTRUM" in name  # the calibration data
-             )
+    if identifiers["DATA_SET_ID"] == "M9-M-IRIS-3-RDR-V1.0" and (
+        name == "SPECTRAL_SERIES"  # the data product
+        or "SPECTRUM" in name  # the calibration data
     ):
         return True, formats.mariner.get_special_block(data, name)
     if (
-        identifiers["DATA_SET_ID"] in (
-            "IHW-C-MSNRDR-3-RDR-HALLEY-ETA-AQUAR-V1.0",
-            "IHW-C-MSNRDR-3-RDR-HALLEY-ORIONID-V1.0",
-        ) and name == "TABLE"
+        re.match(
+            r"IHW-C-MSNRDR-3-RDR-HALLEY-(ETA-AQUAR|ORIONID)-V1.0",
+            identifiers["DATA_SET_ID"],
+        )
+        and name == "TABLE"
     ):
         return True, formats.ihw.get_special_block(data, name)
     if (
         "VG2-" in identifiers["DATA_SET_ID"]
         and "-PRA-3-RDR-LOWBAND-6SEC-V1.0" in identifiers["DATA_SET_ID"]
         and name == "TABLE"
     ):
         return formats.voyager.pra_special_block(data, name, identifiers)
     if (
-         identifiers["DATA_SET_ID"] == "PHX-M-MECA-2-NIEDR-V1.0"
-         and identifiers["PRODUCT_TYPE"] in ("MECA-EM10",
-                                             "MECA-EM11",
-                                             "MECA-EM12",)
-         and name == "WCHEM_TABLE"
+        identifiers["DATA_SET_ID"] == "PHX-M-MECA-2-NIEDR-V1.0"
+        and re.match(r"MECA-EM1[012]", identifiers["PRODUCT_TYPE"])
+        and name == "WCHEM_TABLE"
     ):
         return True, formats.phoenix.wcl_edr_special_block(data, name)
     if (
-         "MEX-M-PFS-2-EDR-" in identifiers["DATA_SET_ID"]
-         and ("RAW" in identifiers["PRODUCT_ID"]
-              or "HK" in identifiers["PRODUCT_ID"])
-         and name == "TABLE"
+        "MEX-M-PFS-2-EDR-" in identifiers["DATA_SET_ID"]
+        and (
+            "RAW" in identifiers["PRODUCT_ID"]
+            or "HK" in identifiers["PRODUCT_ID"]
+        )
+        and name == "TABLE"
     ):
         return formats.mex.pfs_edr_special_block(data, name)
+    if (
+        identifiers["INSTRUMENT_HOST_NAME"] == "MARS EXPRESS"
+        and identifiers["INSTRUMENT_ID"] == "MRS"
+        and all(x in identifiers["PRODUCT_ID"] for x in ["ODF","L1B","RMP"]) 
+        and "TABLE" in name
+    ):
+        return True, formats.mex.mrs_l1b_odf_rmp_redirect(data)
     return False, None
 
 
-def check_trivial_case(pointer, identifiers, fn) -> bool:
-    """"""
+def check_trivial_case(pointer: str, identifiers: DataIdentifiers, fn: str) -> bool:
+    """
+    Supplement generic definition of 'trivial' pointers. Intended primarily to
+    preempt attempts to load known-unsupported data objects associated with
+    otherwise-supported products. Called inline by `pointer_to_loader()`.
+    """
     if is_trivial(pointer):
         return True
     if (
         identifiers["INSTRUMENT_ID"] == "APXS"
         and "ERROR_CONTROL_TABLE" in pointer
     ):
         return formats.msl_apxs.table_loader(pointer)
@@ -568,20 +676,20 @@
         return formats.galileo.galileo_table_loader()
     if (
         identifiers["INSTRUMENT_NAME"]
         == "CHEMISTRY CAMERA REMOTE MICRO-IMAGER"
         and pointer == "IMAGE_REPLY_TABLE"
     ):
         return formats.msl_ccam.image_reply_table_loader()
-    if str(identifiers["DATA_SET_ID"]).startswith("ODY-M-THM-5") and (
+    if identifiers["DATA_SET_ID"].startswith("ODY-M-THM-5") and (
         pointer in ("HEADER", "HISTORY")
     ):
         return formats.themis.trivial_themis_geo_loader(pointer)
     if re.match(
-        r"CO-(CAL-ISS|[S/EVJ-]+ISSNA/ISSWA-2)", str(identifiers["DATA_SET_ID"])
+        r"CO-(CAL-ISS|[S/EVJ-]+ISSNA/ISSWA-2)", identifiers["DATA_SET_ID"]
     ):
         if pointer in ("TELEMETRY_TABLE", "LINE_PREFIX_TABLE"):
             return formats.cassini.trivial_loader(pointer)
     if (
         identifiers["SPACECRAFT_NAME"] == "MAGELLAN"
         and (fn.endswith(".img") or fn.endswith(".ibg"))
         and pointer == "TABLE"
@@ -592,104 +700,114 @@
         and "-CALIMAGES-V1.0" in identifiers["DATA_SET_ID"]
         and "QUB" in identifiers["PRODUCT_ID"]
         and pointer == "HEADER"
     ):
         return formats.galileo.ssi_cubes_header_loader()
     if identifiers["INSTRUMENT_ID"] == "CHEMIN" and (pointer == "HEADER"):
         return formats.msl_cmn.trivial_header_loader()
-    if (
-        "MSL-M-SAM-" in identifiers["DATA_SET_ID"]
-        and "FILE" in pointer
-    ):
+    if "MSL-M-SAM-" in identifiers["DATA_SET_ID"] and "FILE" in pointer:
         # reusing the msl_cmn special case for msl_sam 'FILE' pointers
         return formats.msl_cmn.trivial_header_loader()
     return False
 
 
-def special_image_constants(identifiers):
-    """"""
+def special_image_constants(identifiers: DataIdentifiers) -> dict[str, int]:
+    """
+    Defines 'secret' special constants for a dataset or product type. Called
+    inline by `Data.find_special_constants()`.
+    """
     consts = {}
     if identifiers["INSTRUMENT_ID"] == "CRISM":
         consts["NULL"] = 65535
     return consts
 
 
 def check_special_fn(
-    data, object_name, identifiers
+    data: PDRLike, object_name: str, identifiers: DataIdentifiers
 ) -> tuple[bool, Optional[str]]:
     """
-    special-case handling for labels with nonstandard filename specifications
+    Preempts generic filename specification. Called inline by
+    `Data._object_to_filename()`.
     """
     if (identifiers["DATA_SET_ID"] == "CLEM1-L-RSS-5-BSR-V1.0") and (
         object_name in ("HEADER_TABLE", "DATA_TABLE")
     ):
         # sequence wrapped as string for object names
         return formats.clementine.get_fn(data, object_name)
     if (
         identifiers["SPACECRAFT_NAME"] == "MAGELLAN"
         and (data.filename.endswith(".img") or data.filename.endswith("ibg"))
         and object_name == "TABLE"
     ):
         return formats.mgn.get_fn(data)
     # filenames are frequently misspecified
-    if str(identifiers["DATA_SET_ID"]).startswith("CO-D-CDA") and (
+    if identifiers["DATA_SET_ID"].startswith("CO-D-CDA") and (
         object_name == "TABLE"
     ):
         return formats.cassini.cda_table_filename(data)
     # THEMIS labels don't always mention when a file is stored gzipped
     if identifiers["INSTRUMENT_ID"] == "THEMIS":
         return formats.themis.check_gzip_fn(data, object_name)
     if (
-        identifiers["DATA_SET_ID"] in ["NH-P-PEPSSI-4-PLASMA-V1.0",
-                                       "NH-X-SWAP-5-DERIVED-SOLARWIND-V1.0",
-                                       "NH-P/PSA-LORRI/ALICE/REX-5-ATMOS-V1.0"]
+        identifiers["DATA_SET_ID"]
+        in (
+            "NH-P-PEPSSI-4-PLASMA-V1.0",
+            "NH-X-SWAP-5-DERIVED-SOLARWIND-V1.0",
+            "NH-P/PSA-LORRI/ALICE/REX-5-ATMOS-V1.0",
+        )
         and object_name == "SPREADSHEET"
     ):
         return formats.nh.get_fn(data)
     return False, None
 
 
-def check_special_qube_band_storage(identifiers):
-    """"""
-    if (
-        identifiers["INSTRUMENT_HOST_NAME"]
-        == "CASSINI_ORBITER"
-        # and object_name == "QUBE" #should be repetitive because it's only called
-        # inside a QUBE reading function.
-    ):
+def check_special_qube_band_storage(identifiers: DataIdentifiers):
+    """
+    Defines band storage types for QUBE procuts whose labels do not correctly
+    specify them. Wraps `get_qube_band_storage_type()`.
+    """
+    if identifiers["INSTRUMENT_HOST_NAME"] == "CASSINI_ORBITER":
         return formats.cassini.get_special_qube_band_storage()
     return False, None
 
 
-def check_special_hdu_name(data, identifiers, fn, name):
-    """"""
+def check_special_hdu_name(
+    data: PDRLike, identifiers: DataIdentifiers, fn: Union[str, Path], name: str
+) -> tuple[bool, Optional[int]]:
+    """
+    Preempts generic PDS3 data object -> FITS HDU index mapping. Wraps
+    `get_fits_id()`.
+    """
     if (
-        identifiers['INSTRUMENT_HOST_NAME'] == 'DAWN'
-        and 'FC2' in identifiers['DATA_SET_ID']
+        identifiers["INSTRUMENT_HOST_NAME"] == "DAWN"
+        and "FC2" in identifiers["DATA_SET_ID"]
     ):
         return True, formats.dawn.dawn_hdu_name(name)
-    if identifiers['DATA_SET_ID'].startswith('MSGR-H-MDIS-6-CAL'):
+    if identifiers["DATA_SET_ID"].startswith("MSGR-H-MDIS-6-CAL"):
         return True, formats.galileo.mdis_hdu_name(name)
     if (
         identifiers["INSTRUMENT_NAME"] == "STUDENT DUST COUNTER"
-        and '-SDC-' in identifiers["DATA_SET_ID"]
-        and identifiers['PRODUCT_TYPE'] == 'EDR'
+        and "-SDC-" in identifiers["DATA_SET_ID"]
+        and identifiers["PRODUCT_TYPE"] == "EDR"
     ):
         return True, formats.nh.sdc_edr_hdu_name(name)
-    if re.match(r"NH-\w-REX-[23]", identifiers['DATA_SET_ID']):
+    if re.match(r"NH-\w-REX-[23]", identifiers["DATA_SET_ID"]):
         return True, formats.nh.rex_hdu_name(name)
-    if identifiers['INSTRUMENT_ID'] == 'PEPSSI':
-        if re.search(
-            r"(JUPITER|LAUNCH|CRUISE)", identifiers['DATA_SET_ID']
-        ):
+    if identifiers["INSTRUMENT_ID"] == "PEPSSI":
+        if re.search(r"(JUPITER|LAUNCH|CRUISE)", identifiers["DATA_SET_ID"]):
             return False, None  # these seem ok
-        elif identifiers['PRODUCT_TYPE'] == 'EDR':
+        elif identifiers["PRODUCT_TYPE"] == "EDR":
             return True, formats.nh.pepssi_edr_hdu_name(name)
-        elif "PLUTO" in identifiers['DATA_SET_ID']:
+        elif "PLUTO" in identifiers["DATA_SET_ID"]:
             return True, formats.nh.pepssi_pluto_rdr_hdu_name(name)
         else:
             return True, formats.nh.pepssi_rdr_hdu_name(name)
     if re.match(r"NH.*SWAP", identifiers["DATA_SET_ID"]):
         return True, formats.nh.swap_hdu_stubs(data, identifiers, fn, name)
-    if identifiers['DATA_SET_ID'].startswith('HST-S-WFPC2-3-RPX'):
+    if identifiers["DATA_SET_ID"].startswith("HST-S-WFPC2-3-RPX"):
         return True, formats.saturn_rpx.hst_hdu_name(name)
+    if (
+        "MEX-M-SPI-2-IRRDR-CLEANED" in identifiers['DATA_SET_ID']
+        or "MEX-M-SPI-2-UVRDR-CLEANED" in identifiers['DATA_SET_ID']
+    ):
+        return True, formats.mex.spicam_rdr_hdu_name(data, identifiers, fn, name)
     return False, None
```

### Comparing `pdr-1.0.6/pdr/formats/clementine.py` & `pdr-1.0.7/pdr/formats/clementine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 import re
 
-import numpy as np
-
 import pdr.loaders.queries
 
 
 def get_offset(data, pointer):
-    """"""
+    """
+    HITS
+    * clem_GEO
+        * bsr_rdr_data
+    """
     start_row = int(re.split(r",|[(|)]", data.metadata[f"^{pointer}"])[2])
     return True, (start_row - 1) * data.metadata["RECORD_BYTES"]
 
 
 def get_fn(data, object_name):
-    """"""
+    """
+    HITS
+    * clem_GEO
+        * bsr_rdr_data
+    """
     target = re.split(r",|[(|)]", data.metadata[f"^{object_name}"])[1]
     return True, target
 
 
 def get_structure(block, name, filename, data, identifiers):
-    """"""
+    """
+    HITS:
+    * clem_GEO
+        * bsr_rdr_data
+    """
     fmtdef = pdr.loaders.queries.read_table_structure(
         block, name, filename, data, identifiers
     )
+    import numpy as np
     import pandas as pd
 
     fmtdef = pd.concat([fmtdef, fmtdef], ignore_index=True)
     fmtdef["NAME"] = fmtdef["NAME"].str.split("_", expand=True)[0]
     fmtdef["NAME"] = fmtdef["NAME"].str.cat(map(str, fmtdef.index), sep="_")
     fmtdef.ITEM_OFFSET = 8
     fmtdef.ITEM_BYTES = 8
```

### Comparing `pdr-1.0.6/pdr/formats/diviner.py` & `pdr-1.0.7/pdr/formats/diviner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # because these can contain the value "NaN", combined with the fact that they
 # are space-padded, pd.read_csv sometimes casts some columns to object,
 # turning some of their values into strings and some into float, throwing
 # warnings and making it obnoxious to work with them (users will randomly not
 # be able to, e.g., add two columns together without a data cleaning step).
 def diviner_l4_table_loader(fmtdef_dt, filename):
-    """because these can contain the value "NaN", combined with the fact that they
+    """
+    because these can contain the value "NaN", combined with the fact that they
     are space-padded, pd.read_csv sometimes casts some columns to object,
     turning some of their values into strings and some into float, throwing
     warnings and making it obnoxious to work with them (users will randomly not
-    be able to, e.g., add two columns together without a data cleaning step)."""
+    be able to, e.g., add two columns together without a data cleaning step).
+
+    HITS
+    * diviner
+        * l4
+    """
     import numpy as np
     import pandas as pd
 
     table = pd.DataFrame(
         np.loadtxt(filename, delimiter=",", skiprows=1),
         columns=[c for c in fmtdef_dt[0]["NAME"] if "PLACEHOLDER" not in c],
     )
```

### Comparing `pdr-1.0.6/pdr/formats/galileo.py` & `pdr-1.0.7/pdr/formats/phoenix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,114 @@
-import warnings
+from pdr.loaders.queries import read_table_structure
 
-import pdr.loaders.queries
 
+def elec_em6_structure(block, name, filename, data, identifiers):
+    """
+    ELEC EDR em6/TBL tables: All the START_BYTEs in TBL_0_STATE_DATA.FMT
+    are off by 36 bytes.
 
-def mdis_hdu_name(name):
-    """the MDIS cal labels do not include file size information."""
-    if name in ("IMAGE", "HEADER"):
-        return 0
-    raise NotImplementedError("Unknown MDIS extension name")
-
-
-def galileo_table_loader():
-    """"""
-    warnings.warn("Galileo EDR binary tables are not yet supported.")
-    return True
-
-
-def ssi_cubes_header_loader():
-    """ The Ida and Gaspra cubes have HEADER pointers but no defined HEADER
-    objects"""
-    return True
-
-
-def nims_edr_sample_type(base_samp_info):
-    """ Each time byte order is specified for these products it is LSB, so this
-    assumes BIT_STRING refers to LSB_BIT_STRING. N/A samples are read as CHARACTER"""
-    from pdr.datatypes import sample_types
-
-    sample_type = base_samp_info["SAMPLE_TYPE"]
-    sample_bytes = base_samp_info["BYTES_PER_PIXEL"]
-    if "BIT_STRING" == sample_type:
-        sample_type = "LSB_BIT_STRING"
-        return True, sample_types(
-            sample_type, int(sample_bytes), for_numpy=True
-        )
-    if "N/A" in sample_type:
-        sample_type = "CHARACTER"
-        return True, sample_types(
-            sample_type, int(sample_bytes), for_numpy=True
-        )
-    return False, None
-
-
-def probe_structure(block, name, filename, data, identifiers):
-    """Several NMS products have an incorrect BYTES value in one column.
-    One ASI product has incorrect BYTES values in multiple columns """
-    fmtdef = pdr.loaders.queries.read_table_structure(
+    HITS
+    * phoenix
+        * elec_edr (partial)
+    """
+    from pdr.pd_utils import insert_sample_types_into_df, compute_offsets
+
+    fmtdef = read_table_structure(
         block, name, filename, data, identifiers
     )
-    # Several NMS products have an incorrect BYTES value in one column
-    if fmtdef.at[1, "NAME"] == "COUNTS":
-        fmtdef.at[1, "BYTES"] = 8
-    # One ASI product has incorrect BYTES values in multiple columns
-    elif identifiers["PRODUCT_ID"] == "HK01AD.TAB":
-        fmtdef.at[1, "BYTES"] = 4
-        fmtdef.at[3, "BYTES"] = 2
-        fmtdef.at[5, "BYTES"] = 2
+    for line in range(0, len(fmtdef)):
+        if fmtdef.at[line, "BLOCK_NAME"] == "TBL0 DATA":
+            fmtdef.at[line, "START_BYTE"] -= 36
+    fmtdef = compute_offsets(fmtdef)
+    return insert_sample_types_into_df(fmtdef, identifiers)
+
+
+def afm_rdr_structure(block, name, filename, data, identifiers):
+    """
+    AFM RDR header tables: Several columns' NAME fields start with lowercase
+    letters, which is_an_assignment_line() in /parselabel/pds3.py evaluates as
+    NOT an assignment statement.
+
+    HITS
+    * phoenix
+        * afm_rdr
+    """
+    fmtdef = read_table_structure(block, name, filename, data, identifiers)
+    fmtdef.insert(1, 'NAME', fmtdef.pop('NAME'))
+    for line in range(0, len(fmtdef)):
+        col_number_text = fmtdef.at[line, "COLUMN_NUMBER"]
+        if (
+            isinstance(col_number_text, str)
+            and "NAME" in col_number_text
+        ):
+            fmtdef.at[
+                line, "COLUMN_NUMBER"
+            ] = col_number_text.split("NAME = ")[0]
+            fmtdef.at[line, "NAME"] = col_number_text.split("NAME = ")[1]
     return fmtdef, None
 
 
-def epd_special_block(data, name):
-    """All 'E1' EPD SUMM products incorrectly say ROW_BYTES = 90; changing them
-    to the RECORD_BYTES values."""
-    block = data.metablock_(name)
-    block["ROW_BYTES"] = data.metaget_("RECORD_BYTES")
-    return block
-
-
-def epd_structure(block, name, filename, data, identifiers):
-    """E1PAD_7.TAB has an extra/unaccounted for byte at the start of each row"""
-    fmtdef = pdr.loaders.queries.read_table_structure(
-        block, name, filename, data, identifiers
+def afm_table_loader(filename, fmtdef_dt, name):
+    """
+    AFM RDR tables: Several labels miscount bytes somewhere in the tables
+
+    HITS
+    * phoenix
+        * afm_rdr
+    """
+    import pandas as pd
+    
+    if "HEADER_TABLE" in name:
+        num_rows_skipped = 0
+        num_rows = 4
+    elif name == "AFM_F_ERROR_TABLE":
+        num_rows_skipped = 4
+        num_rows = 512
+    elif name == "AFM_F_HEIGHT_TABLE":
+        num_rows_skipped = 516
+        num_rows = 512
+    elif name == "AFM_B_ERROR_TABLE":
+        num_rows_skipped = 1028
+        num_rows = 512
+    elif name == "AFM_B_HEIGHT_TABLE":
+        num_rows_skipped = 1540
+        num_rows = 512
+    table = pd.read_csv(
+        filename,
+        header=None,
+        sep=",",
+        skiprows=num_rows_skipped, nrows=num_rows
     )
-    for row in range(0, 9):
-        fmtdef.at[row, "START_BYTE"] += 1
-    return fmtdef, None
+    names = [c for c in fmtdef_dt[0]['NAME'] if "PLACEHOLDER" not in c]
+    assert len(table.columns) == len(names), "mismatched column count"
+    table.columns = names
+    return table
 
 
-def pws_special_block(data, name):
-    """The PWS SUMM products sometimes undercount ROW_BYTES by 2"""
+def wcl_edr_special_block(data, name):
+    """
+    WCL EDR ema/emb/emc tables: the START_BYTE for columns 13 and 14 are
+    off by 1 and 2 bytes respectively. (The em8/em9/emf tables are fine.)
+
+    HITS
+    * phoenix
+        * wcl_edr (partial)
+    """
     block = data.metablock_(name)
-    product_id = data.metaget_("PRODUCT_ID")
-    if "B.TAB" in product_id:
-        block["ROW_BYTES"] = 366
-    if "E.TAB" in product_id:
-        block["ROW_BYTES"] = 516
+    
+    for item in iter(block.items()):
+        if "COLUMN" in item:
+            if item[1]["COLUMN_NUMBER"] == 13:
+                item[1]["START_BYTE"] -= 1
+            if item[1]["COLUMN_NUMBER"] == 14:
+                item[1]["START_BYTE"] -= 2
     return block
 
 
-def pws_table_loader(filename, fmtdef_dt):
-    """"""
-    import pandas as pd
+def wcl_rdr_offset(data, name):
+    """WCL RDR CP/CV tables: in the labels, each pointer's start byte is
+    missing '<BYTES>' even though the units are bytes rather than file_records.
+    This doesn't fix the header table though, they still need attention."""
+    target = data.metaget_("^"+name)
+    start_byte = target[-1] - 1
+    return True, start_byte
 
-    fmtdef, dt = fmtdef_dt
-    table = pd.read_csv(filename, header=1, sep=";")
-    assert len(table.columns) == len(fmtdef.NAME.tolist())
-    table.columns = fmtdef.NAME.tolist()
-    return table
```

### Comparing `pdr-1.0.6/pdr/formats/lro.py` & `pdr-1.0.7/pdr/formats/lro.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,22 +15,34 @@
     defined by a single image object (CAL_HISTOGRAM_DATA_IMAGE)."""
     object_name = "CAL_HISTOGRAM_DATA_IMAGE"
     block = data.metablock_(object_name)
     return block
 
 
 def get_crater_offset():
-    """lro crater edr products have a header table with 64 bytes per row, the second
-    table start byte is given in rows (also the wrong row) but had a different number
-    of row bytes"""
+    """
+    lro crater edr products have a header table with 64 bytes per row, the
+    second table start byte is given in rows (also the wrong row) but had a
+    different number of row bytes
+
+    HITS
+    * lro_crater
+        * edr_sec
+        * edr_hk
+    """
     return True, 64
 
 
 def crater_bit_col_sample_type(base_samp_info):
-    """"""
+    """
+    HITS
+    * lro_crater
+        * edr_sec
+        * edr_hk
+    """
     from pdr.datatypes import sample_types
 
     sample_type = base_samp_info["SAMPLE_TYPE"]
     sample_bytes = base_samp_info["BYTES_PER_PIXEL"]
     if "BIT_STRING" == sample_type:
         sample_type = "MSB_BIT_STRING"
         return True, sample_types(
@@ -41,22 +53,34 @@
         return True, sample_types(
             sample_type, int(sample_bytes), for_numpy=True
         )
     return False, None
 
 
 def rss_get_position(identifiers, block, target, name, start_byte):
-    """The RSS WEA products' WEAREC_TABLE undercounts ROW_BYTES by 1"""
+    """
+    The RSS WEA products' WEAREC_TABLE undercounts ROW_BYTES by 1
+
+    HITS
+    * lro_rss
+        * wea
+    """
     table_props = table_position(identifiers, block, target, name, start_byte)
     n_records = block["ROWS"]
     record_bytes = block["ROW_BYTES"] + 1
     length = n_records * record_bytes
     table_props["length"] = length
     return True, table_props
 
 
 def mini_rf_image_loader(data, name):
-    """one of the mosaic labels has the wrong values for lines/line_samples"""
+    """
+    one of the mosaic labels has the wrong values for lines/line_samples
+
+    HITS
+    * lro_mini_rf
+        * mosaic
+    """
     block = data.metablock_(name)
     block["LINES"] = 5760
     block["LINE_SAMPLES"] = 11520
     return block
```

### Comparing `pdr-1.0.6/pdr/formats/mgn.py` & `pdr-1.0.7/pdr/formats/mgn.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 from pdr.utils import head_file
 
 
 def geom_table_loader(filename, fmtdef_dt):
     """
     The Magellan radar system geometry tables include null bytes between rows.
+
+    HITS
+    * gal_nims
+        * impact
+    * mgn_image
+        * midr_tables
     """
     import pandas as pd
     from pdr.utils import head_file
 
     fmtdef, dt = fmtdef_dt
     with head_file(filename) as buf:
         bytes_ = buf.read().replace(b"\x00", b"")
@@ -20,27 +26,44 @@
     assert len(table.columns) == len(names), 'column name mismatch'
     string_buffer.close()
     table.columns = names
     return table
 
 
 def orbit_table_in_img_loader():
-    """"""
+    """
+    HITS
+    * mgn_post_mission
+        * fmap
+        * fmap_browse
+    """
     return True
 
 
 def get_fn(data):
-    """"""
+    """
+    HITS
+    * mgn_post_mission
+        * fmap
+        * fmap_browse
+    """
     target = data.filename
     return True, target
 
 
 def occultation_loader(identifiers, fmtdef_dt, block, filename):
-    """Checks end of each row for newline character. If missing, removes extraneous
-    newline from middle of the row and adjusts for the extra byte. Adapted from _interpret_as_ascii()"""
+    """
+    Checks end of each row for newline character. If missing, removes
+    extraneous newline from middle of the row and adjusts for the extra byte.
+    Adapted from _interpret_as_ascii()
+
+    HITS
+    * mgn_occult
+        * ddr
+    """
     import pandas as pd
 
     fmtdef, dt = fmtdef_dt
     record_length = block["ROW_BYTES"]
 
     # Checks end of each row for newline character. If missing, removes extraneous
     # newline from middle of the row and adjusts for the extra byte.
```

### Comparing `pdr-1.0.6/pdr/formats/mgs.py` & `pdr-1.0.7/pdr/formats/mgs.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,19 @@
     from pdr.pd_utils import insert_sample_types_into_df
 
     fmtdef, dt = insert_sample_types_into_df(fmtdef, identifiers)
     return fmtdef, dt
 
 
 def get_ecs_structure(block, name, filename, data, identifiers):
-    """"""
+    """
+    HITS
+    * mgs_rss_raw
+        * ecs
+    """
     fmtdef = pdr.loaders.queries.read_table_structure(
         block, name, filename, data, identifiers
     )
     fmtdef.at[5, "START_BYTE"] = 80
     fmtdef[f"ROW_BYTES"] = block.get(f"ROW_BYTES")
     from pdr.pd_utils import insert_sample_types_into_df, compute_offsets
```

### Comparing `pdr-1.0.6/pdr/formats/mro.py` & `pdr-1.0.7/pdr/formats/mro.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-from pdr.loaders.queries import read_table_structure
 from io import StringIO
+
+from pdr.loaders.queries import read_table_structure
 from pdr.utils import head_file
-from pdr.pd_utils import compute_offsets
-import pandas as pd
 
 
 def get_structure(block, name, filename, data, identifiers):
-    """The first column in the MCS (EDR/RDR/DDR) format files are just named "1"
+    """
+    The first column in the MCS (EDR/RDR/DDR) format files are just named "1"
     which is being read as 'int'. This was causing problems in read_table
-    #during the table.drop call """
+    during the table.drop call
+
+    HITS
+    * mro
+        * mcs_edr
+        * mcs_rdr
+    """
     fmtdef = read_table_structure(
         block, name, filename, data, identifiers
     )
-    # The first column in the MCS (EDR/RDR/DDR) format files are just named "1"
-    # which is being read as 'int'. This was causing problems in read_table
-    # during the table.drop call 
     fmtdef["NAME"] = fmtdef["NAME"].values.astype(str)
     return fmtdef, None
 
 
 def mcs_ddr_table_loader(fmtdef_dt, block, filename, start_byte):
     """Reads each row of the table and removes extra newline characters. Adapted from _interpret_as_ascii()."""
     with head_file(filename) as f:
         f.read(start_byte)
         newlines_removed = bytearray()
         for row in range(0, block["ROWS"]):
             bytes_ = f.read(block["ROW_BYTES"])
             newlines_removed += bytes_.replace(b"\n", b"") + b"\n"
     string_buffer = StringIO(newlines_removed.decode())
+    import pandas as pd
+    from pdr.pd_utils import compute_offsets
 
     # Adapted from _interpret_as_ascii()
     fmtdef, dt = fmtdef_dt
     colspecs = []
     position_records = compute_offsets(fmtdef).to_dict("records")
     for record in position_records:
         col_length = record["BYTES"]
```

### Comparing `pdr-1.0.6/pdr/formats/ulysses.py` & `pdr-1.0.7/pdr/formats/ulysses.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 def gas_table_loader(filename, fmtdef_dt):
-    """GASDATA.FMT has the wrong START_BYTE for columns in the container.
+    """
+    GASDATA.FMT has the wrong START_BYTE for columns in the container.
     After manually changing the labels during testing, START_BYTE was still
     not incrementing correctly with each repetition of the container.
-    This fixes both issues with 1 special case."""
+    This fixes both issues with 1 special case.
+
+    HITS
+    * ulysses
+        * gas
+    """
     import pandas as pd
     fmtdef, dt = fmtdef_dt
     # Some tables use tabs as column deliminators, others use spaces.
-    table = pd.read_csv(filename, skiprows=17, delim_whitespace=True, header=None)
+    table = pd.read_csv(filename, skiprows=17, sep=r"\s+", header=None)
     assert len(table.columns) == len(fmtdef.NAME.tolist())
     table.columns = fmtdef.NAME.tolist()
     return table
 
 
 def get_sample_type(base_samp_info):
-    """The bit column's data_type is BIT_STRING, which throws errors. Guessing
+    """
+    The bit column's data_type is BIT_STRING, which throws errors. Guessing
     this should be MSB_BIT_STRING. The tables look correct when compared to
-    their ASCII versions."""
+    their ASCII versions.
+
+    HITS
+    * ulysses
+        * epac_pha_bin
+    """
     from pdr.datatypes import sample_types
     sample_type = base_samp_info["SAMPLE_TYPE"]
     sample_bytes = base_samp_info["BYTES_PER_PIXEL"]
 
     if "BIT_STRING" == sample_type:
         sample_type = "MSB_BIT_STRING"
         return True, sample_types(
             sample_type, int(sample_bytes), for_numpy=True
         )
     return False, None
 
 
 def get_special_block(data, name, identifiers):
-    """START_BYTE is wrong for repeated columns within the container.
-    ITEM_BYTES is also off by 1."""
+    """
+    START_BYTE is wrong for repeated columns within the container. ITEM_BYTES
+    is also off by 1.
+
+    HITS
+    * ulysses
+        * epac_all_chan
+        * epac_omni_ele
+        * epac_omni_pro
+        * epac_pha_asc
+        * epac_pha_bin
+        * epac_prtl
+        * epac_pstl
+    """
     block = data.metablock_(name)
     if "ULY-J-EPAC-4-SUMM-PSTL" in identifiers["DATA_SET_ID"]:
         block["CONTAINER"]["COLUMN"]["ITEM_BYTES"] = 13
         block["CONTAINER"]["COLUMN"]["START_BYTE"] = 1
     elif "ULY-J-EPAC-4-SUMM-ALL-CHAN" in identifiers["DATA_SET_ID"]:
         block.getall('CONTAINER')[0]['COLUMN']['START_BYTE'] = 1
         block.getall('CONTAINER')[1]['CONTAINER']['START_BYTE'] = 1
```

### Comparing `pdr-1.0.6/pdr/formats/vega.py` & `pdr-1.0.7/pdr/formats/vega.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 from pdr.datatypes import sample_types
 from pdr.loaders.queries import read_table_structure, check_array_for_subobject
-from pdr.pd_utils import compute_offsets
 
 
 def get_structure(block, name, filename, data, identifiers):
-    """The "encounter data" tables miscount the last column's START_BYTE by 1"""
+    """
+    "Encounter data" tables miscount the last column's START_BYTE by 1
+
+    HITS
+    * vega
+        * ducma
+    """
     fmtdef = read_table_structure(
         block, name, filename, data, identifiers
     )
 
     if "encounter data" in block['DESCRIPTION']:
         fmtdef.at[10, "START_BYTE"] = 62
     return fmtdef, None
 
 
 def fix_array_structure(name, block, fn, data, identifiers):
-    """"""
+    """
+    HITS
+
+    * giotto
+        * pia
+    * vega
+        * puma_mode
+    """
     if not block.get("INTERCHANGE_FORMAT") == "BINARY":
         return None, None
     has_sub = check_array_for_subobject(block)
     if not has_sub:
         dt = sample_types(block["DATA_TYPE"], block["BYTES"], True)
         return None, dt
     fmtdef = read_table_structure(block, name, fn, data, identifiers)
-    fmtdef.loc[fmtdef['NAME'] == 'PLACEHOLDER_SPECTRUM', "AXIS_ITEMS"] = \
-        (block.get("COLLECTION").get("BYTES") -
-            (fmtdef[fmtdef['NAME'] == 'PLACEHOLDER_SPECTRUM']["START_BYTE"].values[0] - 1)) / \
-        len(fmtdef.loc[fmtdef['BLOCK_NAME'].str.contains('SPECTRUM')].index)
+    specbytes = block.get("COLLECTION").get("BYTES")
+    specstart = fmtdef.loc[
+        fmtdef['NAME'] == 'PLACEHOLDER_SPECTRUM', "START_BYTE"
+    ].iloc[0]
+    fmtdef.loc[fmtdef['NAME'] == 'PLACEHOLDER_SPECTRUM', "AXIS_ITEMS"] = (
+        (specbytes - specstart + 1)
+        / len(fmtdef.loc[fmtdef['BLOCK_NAME'].str.contains('SPECTRUM')])
+    )
     # Sometimes arrays define start_byte, sometimes their elements do
     if "START_BYTE" in fmtdef.columns:
-        fmtdef['START_BYTE'].fillna(1, inplace=True)
+        fmtdef['START_BYTE'] = fmtdef['START_BYTE'].fillna(1)
+    from pdr.pd_utils import compute_offsets, insert_sample_types_into_df
 
-    from pdr.pd_utils import insert_sample_types_into_df
     return insert_sample_types_into_df(compute_offsets(fmtdef), identifiers)
```

### Comparing `pdr-1.0.6/pdr/formats/viking.py` & `pdr-1.0.7/pdr/formats/viking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 def seis_table_loader(filepath, fmtdef_dt):
     """
     The Viking 2 seismometer tables have mangled labels. The raw data tables
     are variable length CSVs, and labels for the summary tables count column
     bytes wrong. Half the labels define columns that do not match the data.
+
+    HITS
+    * viking
+        * seis_raw
+        * seis_summary
     """
     import pandas as pd
+
     col_names = [c for c in fmtdef_dt[0].NAME if "PLACEHOLDER" not in c]
     filename = filepath.split("/")[-1]
     # The summary tables have miscounted bytes in their labels. The columns are
-    # separated by whitespace, so can be read by read_csv() instead.
-    # Both labels define a SEISMIC_TIME_SOLS column that doesn't exist in the data.
+    # separated by whitespace, so can be read by read_csv() instead. Also, both
+    # labels define a SEISMIC_TIME_SOLS column that doesn't exist in the data.
     if "summary" in filename.lower():
-        table = pd.read_csv(filepath, header=None, delim_whitespace=True)
+        table = pd.read_csv(filepath, header=None, sep=r"\s+")
         col_names.remove("SEISMIC_TIME_SOLS")
         if "event_wind_summary" in filename.lower():
             # event_wind_summary.tab has a column not included in the label. It
             # is listed in: https://pds-geosciences.wustl.edu/viking/vl2-m-seis-5-rdr-v1/vl_9020/document/vpds_event_winds_format.txt
             col_names.insert(7, "ORIGINAL_LINES_COUNT")
     # The raw event tables are variable-length CSVs. Their labels include a
     # SEISMIC_SOL column that doesn't exist in the data.
     elif "event" in filename.lower():
         table = pd.read_csv(filepath, header=None, sep=",")
         col_names.remove("SEISMIC_SOL")
     # The raw high-rate tables are variable-length CSVs. Their labels list the
     # correct number of columns.
     elif "high" in filename.lower():
         table = pd.read_csv(filepath, header=None, sep=",")
+    else:
+        raise ValueError("Unknown Viking 2 SEIS table format.")
     assert len(table.columns) == len(col_names), "mismatched column count"
     table.columns = col_names
     return table
```

### Comparing `pdr-1.0.6/pdr/formats/voyager.py` & `pdr-1.0.7/pdr/formats/voyager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,125 @@
 def mag_special_block(data, name):
-    """ROW_BYTES are listed as 144 in the labels for Uranus and Neptune MAG RDRs.
+    """
+    ROW_BYTES are listed as 144 in the labels for Uranus and Neptune MAG RDRs.
     Their tables look the same, but the Neptune products open wrong. Setting
-    ROW_BYTES to 145 fixes it."""
+    ROW_BYTES to 145 fixes it.
+
+    HITS
+    * vg_mag
+        * rdr_nep
+    """
     block = data.metablock_(name)
     block["ROW_BYTES"] = 145 
     return block
 
 
 def get_structure(block, name, filename, data, identifiers):
-    """The VGR_PLS_HR_2017.FMT for PLS 1-hour averages undercounts the last
-    column by 1 byte."""
+    """
+    The VGR_PLS_HR_2017.FMT for PLS 1-hour averages undercounts the last column
+    by 1 byte.
+
+    HITS
+    * vg_pls
+        * sys_1hr_avg (partial)
+    """
     from pdr.loaders.queries import read_table_structure
     fmtdef = read_table_structure(
         block, name, filename, data, identifiers
     )
     fmtdef.at[8, "BYTES"] = 6
     return fmtdef, None
 
 
 def pls_avg_special_block(data, name):
-    """Because VGR_PLS_HR_2017.FMT undercounts by 1 byte, the products that
-    reference it also undercount their ROW_BYTES by."""
+    """
+    Because VGR_PLS_HR_2017.FMT undercounts by 1 byte, the products that
+    reference it also undercount their ROW_BYTES by 1.
+
+    HITS
+    * vg_pls
+        * sys_1hr_avg
+    """
     block = data.metablock_(name)
     if block["^STRUCTURE"] == "VGR_PLS_HR_2017.FMT":
         block["ROW_BYTES"] = 57 
         return True, block
     return False, None
 
 
 def pls_fine_special_block(data, name):
-    """Most of the PLS FINE RES labels undercount the ROW_BYES. The most recent
-    product (2007-241_2018-309) is formatted differently and opens correctly."""
+    """
+    Most of the PLS FINE RES labels undercount the ROW_BYTES. The most recent
+    product (2007-241_2018-309) is formatted differently and opens correctly.
+
+    HITS
+    * vg_pls
+        * sys_fine_res
+    """
     block = data.metablock_(name)
     if block["ROW_BYTES"] == 57:
         block["ROW_BYTES"] = 64 
         return True, block
     return False, None
 
 
 def pls_ionbr_special_block(data, name):
-    """SUMRY.LBL references the wrong format file"""
+    """
+    SUMRY.LBL references the wrong format file
+
+    HITS
+    * vg_pls
+        * ur_ionbr (partial)
+    """
     block = data.metablock_(name)
     block["^STRUCTURE"] = "SUMRY.FMT" 
     return True, block
 
+
 def pra_special_block(data, name, identifiers):
-    """PRA Lowband RDRs: The Jupiter labels use the wrong START_BYTE for columns 
-    in containers. The Saturn/Uranus/Neptune labels define columns with multiple 
-    ITEMS, but ITEM_BYTES is missing and the BYTES value is wrong."""
+    """
+    PRA Lowband RDRs: The Jupiter labels use the wrong START_BYTE for columns
+    in containers. The Saturn/Uranus/Neptune labels define columns with
+    multiple ITEMS, but ITEM_BYTES is missing and the BYTES value is wrong.
+
+    HITS
+    * vg_pra
+        * lowband_jup
+        * lowband_other
+    """
     block = data.metablock_(name)
-    if identifiers["DATA_SET_ID"] in ("VG2-S-PRA-3-RDR-LOWBAND-6SEC-V1.0",
-                                      "VG2-N-PRA-3-RDR-LOWBAND-6SEC-V1.0",
-                                      "VG2-U-PRA-3-RDR-LOWBAND-6SEC-V1.0"
-                                      ):
-      for item in iter(block.items()):
+    if identifiers["DATA_SET_ID"] in (
+        "VG2-S-PRA-3-RDR-LOWBAND-6SEC-V1.0",
+        "VG2-N-PRA-3-RDR-LOWBAND-6SEC-V1.0",
+        "VG2-U-PRA-3-RDR-LOWBAND-6SEC-V1.0"
+    ):
+        for item in iter(block.items()):
             if "COLUMN" in item and "SWEEP" in item[1]["NAME"]:
-                item[1].add("ITEM_BYTES", 4) # The original BYTES value
-                item[1]["BYTES"] = 284 # ITEM_BYTES * ITEMS
+                item[1].add("ITEM_BYTES", 4)  # The original BYTES value
+                item[1]["BYTES"] = 284  # ITEM_BYTES * ITEMS
     elif identifiers["DATA_SET_ID"] == "VG2-J-PRA-3-RDR-LOWBAND-6SEC-V1.0":
         for item in iter(block["CONTAINER"].items()):
             if "COLUMN" in item:
                 if item[1]["NAME"] == "STATUS_WORD":
                     item[1]["START_BYTE"] = 1
                 if item[1]["NAME"] == "DATA_CHANNELS":
                     item[1]["START_BYTE"] = 5
     return True, block
 
+
 def lecp_table_loader(filename, fmtdef_dt):
-    """VG1 LECP Jupiter SUMM Sector tables reference a format file with
-    incorrect START_BYTEs for columns within a CONTAINER. Columns are
-    consistently separated by whitespace."""
+    """
+    VG1 LECP Jupiter SUMM Sector tables reference a format file with incorrect
+    START_BYTEs for columns within a CONTAINER. Columns are consistently
+    separated by whitespace.
+
+    HITS
+    vg_lecp
+        * j_summ_sector_vg1
+    """
     import pandas as pd
 
     fmtdef, dt = fmtdef_dt
-    table = pd.read_csv(filename, header=None, delim_whitespace=True)
+    table = pd.read_csv(filename, header=None, sep=r"\s+")
     assert len(table.columns) == len(fmtdef.NAME.tolist())
     table.columns = fmtdef.NAME.tolist()
     return table
```

### Comparing `pdr-1.0.6/pdr/func.py` & `pdr-1.0.7/pdr/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from functools import wraps, reduce
-# noinspection PyProtectedMember
+# noinspection PyProtectedMember,PyUnresolvedReferences
 from inspect import signature, _empty, Signature, Parameter
 from itertools import combinations, chain
 from typing import Callable, Any, Mapping, Optional, Collection
 
 from cytoolz import keyfilter
 from cytoolz.curried import valfilter
 from dustgoggles.tracker import TrivialTracker
 
 
 def get_argnames(func: Callable) -> set[str]:
     """return names of all parameters of a function"""
     return set(signature(func).parameters.keys())
 
 
-def not_optional(param: Parameter):
+def not_optional(param: Parameter) -> bool:
     """
     is this Parameter flagged as not required according to the conventions of
     this module?
     """
     if "Optional" in str(param):
         return False
     if param.name in ("_", "__"):
@@ -128,15 +128,15 @@
             # we already removed it
             continue
     return Signature(paramsort(outparams))
 
 
 def specialize(
     func: Callable,
-    check: Callable[[Any], tuple[bool, Any]],
+    check: Callable[..., tuple[bool, Any]],
     error: Optional[Callable[[Exception], str]] = None,
     tracker: TrivialTracker = TrivialTracker(),
 ) -> Callable:
     """
     function decorator that permits dispatch of calls to func to an arbitrary
     set of special-case functions defined in check.
     replaces the pre-1.0 pdr special case checks.
```

### Comparing `pdr-1.0.6/pdr/loaders/datawrap.py` & `pdr-1.0.7/pdr/loaders/datawrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Union
+"""Classes to wrap and manage complex data-loading workflows."""
+from typing import Any
 
 from dustgoggles.dynamic import exc_report
 
 from pdr.formats import (
     check_special_sample_type,
     check_special_qube_band_storage,
     check_special_position,
@@ -31,19 +32,21 @@
 class Loader:
     """
     compact wrapper for loader functions, intended principally but not solely
     for library-internal use. provides a common interface, adds compactness,
     delays imports, etc.
     """
 
-    def __init__(self, loader_function: Union[LoaderFunction, str]):
+    def __init__(self, loader_function: LoaderFunction):
         self.loader_function = loader_function
         self.argnames = get_argnames(loader_function)
 
-    def __call__(self, pdrlike: PDRLike, name: str, **kwargs):
+    def __call__(
+        self, pdrlike: PDRLike, name: str, **kwargs
+    ) -> dict[str, Any]:
         kwargdict = {"data": pdrlike, "name": depointerize(name)} | kwargs
         kwargdict["tracker"].set_metadata(loader=self.__class__.__name__)
         record_exc = {"status": "query_ok"}
         try:
             info = softquery(self.loader_function, self.queries, kwargdict)
         except Exception as exc:
             record_exc = {"status": "query_failed"} | _format_exc_report(exc)
```

### Comparing `pdr-1.0.6/pdr/loaders/dispatch.py` & `pdr-1.0.7/pdr/loaders/dispatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
+"""Functions to select appropriate Loader subclasses for data objects."""
+
+from __future__ import annotations
+
 import re
-from typing import Optional, Callable
+from typing import Optional, TYPE_CHECKING
+
 from pdr.formats import check_trivial_case
 from pdr.loaders.utility import (
     looks_like_this_kind_of_file,
     FITS_EXTENSIONS,
-    TIFF_EXTENSIONS,
-    JP2_EXTENSIONS,
+    GIF_EXTENSIONS,
     IMAGE_EXTENSIONS,
+    JP2_EXTENSIONS,
     TABLE_EXTENSIONS,
-    TEXT_EXTENSIONS, GIF_EXTENSIONS,
+    TEXT_EXTENSIONS,
+    TIFF_EXTENSIONS,
 )
 from pdr.loaders.datawrap import (
-    ReadLabel,
+    Loader,
     ReadArray,
+    ReadCompressedImage,
     ReadFits,
-    ReadText,
-    ReadImage,
     ReadHeader,
-    ReadCompressedImage,
+    ReadImage,
+    ReadLabel,
     ReadTable,
+    ReadText,
     TBD,
     Trivial
 )
 
+if TYPE_CHECKING:
+    from pdr import Data
 
-def image_lib_dispatch(pointer: str, data: "Data") -> Optional[Callable]:
+
+def image_lib_dispatch(pointer: str, data: Data) -> Optional[Loader]:
     """
     check file extensions to see if we want to toss a file to an external
     library rather than using our internal raster handling. current cases are:
     pillow for tiff, gif, or jp2; astropy for fits
     """
     object_filename = data._target_path(pointer)
     if looks_like_this_kind_of_file(object_filename, FITS_EXTENSIONS):
@@ -36,24 +46,24 @@
     if looks_like_this_kind_of_file(
         object_filename, TIFF_EXTENSIONS + JP2_EXTENSIONS + GIF_EXTENSIONS
     ):
         return ReadCompressedImage()
     return None
 
 
-# noinspection PyTypeChecker
-def pointer_to_loader(pointer: str, data: "Data") -> Callable:
+def pointer_to_loader(pointer: str, data: Data) -> Loader:
     """
-    attempt to select an appropriate loading function based on a PDS3 pointer
-    name. checks for special cases and then falls back to generic loading
-    methods of pdr.Data.
+    Attempt to select an appropriate Loader subclass based on a PDS3 object
+    name (and sometimes the file extension).
+
+    The apparently-redundant sequence of conditionals is not in fact redundant;
+    it is based on our knowledge of the most frequently used but sometimes
+    redundant object names in the PDS3 corpus.
     """
-    if check_trivial_case(
-        pointer, data.identifiers, data.filename
-    ):
+    if check_trivial_case(pointer, data.identifiers, data.filename):
         return Trivial()
     if pointer == "LABEL":
         return ReadLabel()
     if image_lib_dispatch(pointer, data) is not None:
         return image_lib_dispatch(pointer, data)
     if (
         "TEXT" in pointer
@@ -91,22 +101,22 @@
         ("IMAGE" in pointer)
         or ("QUB" in pointer)
         or ("XDR_DOCUMENT" in pointer)
     ):
         return ReadImage()
     if "FILE_NAME" in pointer:
         return file_extension_to_loader(pointer)
-    # TODO: sloppy pt. 2
     return TBD()
 
 
-def file_extension_to_loader(fn: str) -> Callable:
+def file_extension_to_loader(fn: str) -> Loader:
     """
-    attempt to select the correct method of pdr.Data for objects only
-    specified by a PDS3 FILE_NAME pointer (or by filename otherwise).
+    Attempt to select the correct Loader subclass for an object based solely on
+    its file extension. Used primarily for objects only specified by a PDS3
+    FILE_NAME pointer or similar.
     """
     if looks_like_this_kind_of_file(fn, FITS_EXTENSIONS):
         return ReadFits()
     if looks_like_this_kind_of_file(fn, TIFF_EXTENSIONS):
         return ReadCompressedImage()
     if looks_like_this_kind_of_file(fn, IMAGE_EXTENSIONS):
         return ReadImage()
@@ -115,14 +125,17 @@
     if looks_like_this_kind_of_file(fn, TABLE_EXTENSIONS):
         return ReadTable()
     if looks_like_this_kind_of_file(fn, JP2_EXTENSIONS):
         return ReadCompressedImage()
     return TBD()
 
 
-# pointers we do not automatically load even when loading greedily --
-# generally these are reference files, usually throwaway ones, that are not
-# archived in the same place as the data products and add little, if any,
-# context to individual products
-
-objects_to_ignore = ["DATA_SET_MAP_PROJECT.*", ".*_DESC$", ".*DESCRIPTION$"]
-OBJECTS_IGNORED_BY_DEFAULT = re.compile("|".join(objects_to_ignore))
+OBJECTS_TO_IGNORE = ["DATA_SET_MAP_PROJECT.*", ".*_DESC$", ".*DESCRIPTION$"]
+"""
+PDS3 objects we do not automatically load, even when loading greedily.
+These are reference files, usually throwaway ones, that are usually not
+archived in the same place as the data products and add little, if any, context 
+to individual products (they are the same across an entire 'product type').
+This means that in almost all cases, attempting to greedily load them has no
+purpose but to throw irrelevant warnings at the user. 
+"""
+OBJECTS_IGNORED_BY_DEFAULT = re.compile("|".join(OBJECTS_TO_IGNORE))
```

### Comparing `pdr-1.0.6/pdr/loaders/handlers.py` & `pdr-1.0.7/pdr/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,254 @@
+"""generic i/o, parsing, and functional utilities."""
+import bz2
+from io import BytesIO
+from itertools import chain
+from numbers import Number
+from pathlib import Path
+import struct
+import textwrap
+from typing import (
+    Collection,
+    IO,
+    Mapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Union,
+)
 import warnings
-from typing import Optional
-import Levenshtein as lev
-from cytoolz import groupby
+from zipfile import ZipFile
+
+from dustgoggles.structures import listify
 from multidict import MultiDict
 
 
-def handle_fits_file(
-    fn, name="", hdu_id="", hdulist: Optional["HDUList"] = None
-):
-    """
-    This function attempts to read all FITS files, compressed or
-    uncompressed, with astropy.io.fits. Files with 'HEADER' pointer
-    return the header, all others return data.
-
-    we distinguish name and hdu_name as a slightly hacky way to facilitate
-    special cases in which we explicitly map a PDS pointer to a FITS HDU name
-    or index.
-    """
-
-    #TODO, maybe: dispatch to decompress() for weirdo compression
-    # formats, but possibly not right here? hopefully we shouldn't need
-    # to handle compressed FITS files too often anyway, and astropy can deal
-    # with gzip without special help (although inline igzip is faster)
-
-    from astropy.io import fits
-
-    if hdulist is None:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", module="astropy.io.fits.card")
-            hdulist = fits.open(fn)
-    # this means the id was generated by queries.get_fits_id and includes the
-    # number of distinct HDUs mentioned in the PDS label, so we can do a
-    # validity check.
-    if isinstance(hdu_id, tuple):
-        hdu_id, inferred_hdu_count = hdu_id
-        if len(hdulist) != inferred_hdu_count:
+SUPPORTED_COMPRESSION_EXTENSIONS = (".gz", ".bz2", ".zip")
+"""compression 'types' we support"""
+
+
+def read_hex(hex_string: str, fmt: str = ">I") -> Number:
+    """
+    return the decimal representation of a hexadecimal number in a given
+    number format (expressed as a struct-style format string, default is
+    unsigned 32-bit integer)
+    """
+    return struct.unpack(fmt, bytes.fromhex(hex_string))[0]
+
+
+def head_file(
+    fn_or_reader: Union[IO, Path, str],
+    nbytes: Union[int, None] = None,
+    offset: int = 0,
+    tail: bool = False,
+) -> BytesIO:
+    """"""
+    head_buffer = BytesIO()
+    if not hasattr(fn_or_reader, "read"):
+        fn_or_reader = open(fn_or_reader, "rb")
+    whence = 2 if tail is True else False
+    offset = offset * -1 if tail is True else offset
+    fn_or_reader.seek(offset, whence)
+    head_buffer.write(fn_or_reader.read(nbytes))
+    fn_or_reader.close()
+    head_buffer.seek(0)
+    return head_buffer
+
+
+def stem_path(path: Path):
+    """
+    convert a Path to lowercase and remove any compression extensions
+    from it to stem for loose matching
+    """
+    lowercase = path.stem.lower()
+    # noinspection PyTypeChecker
+    exts = tuple(map(str.lower, path.suffixes))
+    if len(exts) == 0:
+        return lowercase
+    # don't remove compression suffix if it's the only suffix
+    if (len(exts) == 1) or (exts[-1] in SUPPORTED_COMPRESSION_EXTENSIONS):
+        return f"{lowercase}{exts[0]}"
+    return f"{lowercase}{exts[-1]}"
+
+
+def check_cases(
+    filenames: Union[Collection[Union[Path, str]], Union[Path, str]],
+    skip: bool = False,
+) -> str:
+    """
+    check for oddly-cased versions of a specified filename in local path --
+    very common to have case mismatches between PDS3 labels and actual archive
+    contents. similarly, check common compression extensions.
+
+    the skip argument makes the function simply return filename.
+    """
+    filenames = listify(filenames)
+    for filename in filenames:
+        if skip is True:
+            return str(filename)
+        path = Path(filename)
+        if path.exists():
+            return str(filename)
+        if not path.parent.exists():
+            continue
+        matches = tuple(
+            filter(
+                lambda p: stem_path(p) == Path(filename).name.lower(),
+                path.parent.iterdir(),
+            )
+        )
+        if len(matches) == 0:
+            continue
+        if len(matches) > 1:
+            warning_list = ", ".join([path.name for path in matches])
             warnings.warn(
-                "The number of HDUs inferred from the PDS label differs "
-                "from the number of HDUs in the FITS file. Indexing may "
-                "be off."
+                f"Multiple off-case or possibly-compressed versions of "
+                f"{filename} found in search path: {warning_list}. Using "
+                f"{matches[0].name}."
             )
-    try:
-        hdr_val = handle_fits_header(hdulist, hdu_id)
-    # astropy.io.fits does not call any verification on read. on 'output'
-    # tasks -- which iterating over header cards (sometimes) counts as, and
-    # which we have to do in order to place the header content into our
-    # preferred data structure -- it does call verification, at the strictest
-    # settings. we do not want to prospectively fix every case because it is
-    # quite slow. so, when astropy.io.fits decides something is too invalid to
-    # show us, tell it to fix it first.
-    except fits.VerifyError:
-        try:
-            hdulist.verify('silentfix')
-            hdr_val = handle_fits_header(hdulist, hdu_id)
-        except (fits.VerifyError, ValueError):  # real messed up
-            hdr_val = handle_fits_header(hdulist, hdu_id, skip_bad_cards=True)
-    if (
-        "HEADER" not in name
-        # cases where HDUs are named things like "IMAGE HEADER"
-        or hdu_id in [h[1] for h in hdulist.info(False)]
-    ):
-        output = {f"{name}_HEADER": hdr_val}
+        return str(matches[0])
+    filelist = ";".join([str(f) for f in filenames])
+    raise FileNotFoundError(
+        f"No candidate paths for required file exist. Checked:{filelist}"
+    )
+
+
+def append_repeated_object(
+    obj: Union[Sequence, Mapping],
+    fields: MutableSequence,
+    repeat_count: int,
+) -> MutableSequence:
+    """
+    Polymorphic function to append `obj` `repeat_count` times to `fields`.
+    If `obj` is a non-string sequence, it instead concatenates and adds it.
+    For instance:
+    ```
+    >>> append_repeated_object([1, 2], [4], 3)
+    [4, 1, 2, 1, 2, 1, 2]
+    >>> append_repeated_object({"a": "b"}, ["a"], 3)
+    ["a", {"a": "b"}, {"a": "b"}, {"a": "b"}]
+    ```
+    NOTE: This function treats `repeat_count` values < 1 as 1.
+    WARNING: this function does not copy `obj` or any of its elements, even if
+    they are mutable. This is not a bug, but can cause unexpected behavior, so
+    take care (and in particular, always go depth-first if you are using this
+    function in a recursive operation).
+    """
+    if hasattr(obj, "__add__"):
+        if repeat_count > 1:
+            fields += chain.from_iterable([obj for _ in range(repeat_count)])
+        else:
+            fields += obj
     else:
-        return {name: hdr_val}
-    hdu = hdulist[pointer_to_fits_key(hdu_id, hdulist)]
-    # binary table HDUs with repeated column names break astropy
-    if isinstance(hdu, fits.BinTableHDU):
-        reindex_dupe_names(hdu)
-    body = hdu.data
-    if body is None:
-        import numpy as np
-
-        body = np.array([])
-    # i.e., it's a FITS table, binary or ascii
-    if isinstance(body, fits.fitsrec.FITS_rec):
-        import pandas as pd
-        from pdr.pd_utils import structured_array_to_df
-        try:
-            body = pd.DataFrame.from_records(body)
-        except ValueError:
-            import numpy as np
-
-            # nested arrays, generally -- we don't do this by default because
-            # it requires us to 'reassemble' the array twice, so is inefficient
-            body = structured_array_to_df(np.rec.fromarrays([body[k] for k in
-                                          body.dtype.names], dtype=body.dtype))
-    return output | {name: body}
-
-
-def reindex_dupe_names(hdu: "astropy.io.fits.BinTableHDU"):
-    """
-    rename duplicate column names in a fits binary table -- astropy will not
-    be able to construct the .data attribute otherwise
-    """
-    names = [c.name for c in hdu.columns]
-    repeats = {n for n in names if names.count(n) > 1}
-    for r in repeats:
-        indices = [ix for ix, n in enumerate(names) if n == r]
-        for i, ix in enumerate(indices):
-            hdu.columns[ix].name += f"_{i}"
-
-
-def handle_compressed_image(fn):
-    """"""
-    import numpy as np
-    from PIL import Image
-
-    # deactivate pillow's DecompressionBombError: many planetary images
-    # are legitimately very large
-    Image.MAX_IMAGE_PIXELS = None
-    im = Image.open(fn)
-    if im.mode == 'P':
-        # classic-style GIFs
-        im = im.convert('RGB', palette=im.palette)
-    # noinspection PyTypeChecker
-    image = np.ascontiguousarray(im).copy()
-    # pillow reads images as [x, y, channel] rather than [channel, x, y]
-    if len(image.shape) == 3:
-        return np.ascontiguousarray(np.rollaxis(image, 2))
-    return image
+        if repeat_count > 1:
+            fields += [obj for _ in range(repeat_count)]
+        else:
+            fields.append(obj)
+    return fields
 
 
-def handle_fits_header(hdulist, hdu_id="", skip_bad_cards=False):
+def import_best_gzip():
     """"""
-    if isinstance(hdu_id, int):
-        astro_hdr = hdulist[hdu_id].header
-    else:
-        astro_hdr = hdulist[pointer_to_fits_key(hdu_id, hdulist)].header
-    output_hdr = MultiDict()
-    from astropy.io import fits
-    for i in range(len(astro_hdr.cards)):
-        try:
-            key, val, com = astro_hdr.cards[i]
-            if len(key) > 0:
-                if isinstance(val, (str, float, int)):
-                    output_hdr.add(key, val)
-                else:
-                    output_hdr.add(key, str(val))
-                if len(com) > 0:
-                    comment_key = key + "_comment"
-                    output_hdr.add(comment_key, com)
-        except fits.VerifyError:
-            if skip_bad_cards is True:
-                continue
-            raise
-        except StopIteration:
-            break
-    return output_hdr
-
-
-def pointer_to_fits_key(pointer, hdulist):
-    """
-    In some datasets with FITS, the PDS3 object names and FITS object
-    names are not identical. This function attempts to use Levenshtein
-    "fuzzy matching" to identify the correlation between the two. It is not
-    guaranteed to be correct! And special case handling might be required in
-    the future.
-    """
-    if isinstance(pointer, int):  # permit explicit specification of HDU number
-        return pointer
-    # something astropy does sometimes
-    elif pointer.isnumeric():
-        return int(pointer)
-    hdu_names = [h[1].lower() for h in hdulist.info(False)]
     try:
-        return hdu_names.index(pointer.lower())
-    except ValueError:
-        pass
-    if pointer in ("IMAGE", "TABLE", None, ""):
-        return 0
-    levratio = [lev.ratio(name, pointer.lower()) for name in hdu_names]
-    return levratio.index(max(levratio))
+        from isal import igzip as gzip_lib
+    except ImportError:
+        import gzip as gzip_lib
+    return gzip_lib
 
 
-def add_bit_column_info(obj, definition, identifiers):
-    if "BIT_COLUMN" not in obj.keys():
-        return obj
-    from pdr.bit_handling import (
-        set_bit_string_data_type, get_bit_start_and_size
-    )
-    obj["DATA_TYPE"] = obj["DATA_TYPE"].replace(" ", "_")
-    if "BIT_STRING" not in obj["DATA_TYPE"]:
-        obj = set_bit_string_data_type(obj, identifiers)
-    return get_bit_start_and_size(obj, definition, identifiers)
-
-
-def unpack_fits_headers(
-    filename, hdulist=None
-) -> tuple[MultiDict, list[str], dict[str, int]]:
-    """"""
-    from astropy.io import fits
-
-    hdumap = {}
-    headerdict = MultiDict()
-    if hdulist is None:
-        hdulist = fits.open(filename)
-    namegroups = groupby(lambda hi: hi[1], hdulist.info(False))
-    for name, group in namegroups.items():
-        if len(group) == 1:
-            hdu_ix = group[0][0]
-            headerdict.add(name, handle_fits_header(hdulist, hdu_ix))
-            hdumap[name] = hdu_ix
-            continue
-        for ix, hdu in enumerate(group):
-            hdu_ix, hdu_name = hdu[0], f'{name}_{ix}'
-            headerdict.add(
-                hdu_name, handle_fits_header(hdulist, hdu_ix)
+def decompress(filename):
+    """"""
+    if filename.lower().endswith(".gz"):
+        f = import_best_gzip().open(filename, "rb")
+    elif filename.lower().endswith(".bz2"):
+        f = bz2.BZ2File(filename, "rb")
+    elif filename.lower().endswith(".zip"):
+        f = ZipFile(filename, "r").open(
+            ZipFile(filename, "r").infolist()[0].filename
+        )
+    else:
+        f = open(filename, "rb")
+    return f
+
+
+def with_extension(fn: Union[str, Path], new_suffix: str) -> str:
+    """"""
+    return str(Path(fn).with_suffix(new_suffix))
+
+
+def find_repository_root(absolute_path):
+    """"""
+    parts = Path(absolute_path).parts
+    data_indices = [
+        ix for ix, part in enumerate(parts) if part.lower() == "data"
+    ]
+    return Path(*parts[: data_indices[-1]])
+
+
+def prettify_multidict(multi, sep=" ", indent=0):
+    """"""
+    indentation, output, first_line = "", "{", True
+    for k, v in multi.items():
+        if sep == "\n":
+            indentation = " " * indent
+            if first_line is True:
+                output += "\n"
+        if isinstance(v, MultiDict):
+            output += (
+                f"{indentation}{k}: "
+                f"{prettify_multidict(v, indent = indent + 2)},{sep}"
             )
-            hdumap[hdu_name] = hdu_ix
-    params = []
-    for hdu_name in headerdict.keys():
-        # note that FITS headers can't be deeply nested
-        params.append(hdu_name)
-        for field in headerdict[hdu_name].keys():
-            params.append(field)
-    return headerdict, params, hdumap
+        elif (not isinstance(v, str)) or (len(v) <= 70):
+            output += f"{indentation}{k}: {v},{sep}"
+        else:
+            lines = textwrap.wrap(v, width=(70 - len(indentation)))
+            vstr = f"{lines[0]}\n" + "\n".join(
+                [(" " * (indent + 1)) + line for line in lines[1:]]
+            )
+            output += f"{indentation}{k}: {vstr},{sep}"
+        first_line = False
+        if sep != " ":
+            continue
+        if len(output) > 70:
+            return prettify_multidict(multi, sep="\n", indent=indent + 1)
+    if len(indentation) > 0:
+        indentation = indentation[:-1]
+    return output + indentation + "}"
+
+
+def associate_label_file(
+    data_filename: str,
+    label_filename: Optional[str] = None,
+    skip_check: bool = False,
+) -> Optional[str]:
+    """"""
+    from pdr.loaders.utility import LABEL_EXTENSIONS
+
+    if label_filename is not None:
+        return check_cases(Path(label_filename).absolute(), skip_check)
+    elif data_filename.lower().endswith(LABEL_EXTENSIONS):
+        return check_cases(data_filename)
+    for lext in LABEL_EXTENSIONS:
+        try:
+            return check_cases(with_extension(data_filename, lext))
+        except FileNotFoundError:
+            continue
+    return None
+
+
+def check_primary_fmt(data_filename: str):
+    """"""
+    from pdr.loaders.utility import FITS_EXTENSIONS
+
+    for ext in FITS_EXTENSIONS:
+        if data_filename.lower().endswith(ext):
+            return "FITS"
+
+
+def catch_return_default(debug: bool, return_default, exception: Exception):
+    """
+    if we are in debug mode, reraise an exception. otherwise, return
+    the default only.
+    """
+    if debug is True:
+        raise exception
+    return return_default
```

### Comparing `pdr-1.0.6/pdr/loaders/image.py` & `pdr-1.0.7/pdr/loaders/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-import warnings
+"""Functions for the nitty-gritty array-shaping parts of image loading."""
+
+from io import BufferedIOBase
 from itertools import product
+from typing import Optional
+import warnings
 
 import numpy as np
 
+from pdr import vax
 from pdr.loaders.queries import get_image_properties
-from pdr.np_utils import np_from_buffered_io
+from pdr.np_utils import make_c_contiguous, np_from_buffered_io
+from pdr.pdrtypes import ImageProps
 from pdr.utils import decompress
-from pdr import vax
 
 
-def read_image(name, gen_props, fn, start_byte):
-    """
-    Read an image object from this product and return it as a numpy array.
-    """
-    # TODO: Check for and apply BIT_MASK.
+def read_image(
+    name: str, gen_props: ImageProps, fn: str, start_byte: int
+) -> np.ndarray:
+    """Read an IMAGE object and return it as a numpy array."""
     props = get_image_properties(gen_props)
     f = decompress(fn)  # seamlessly deal with compression
     f.seek(start_byte)
     try:
         # Make sure that single-band images are 2-dim arrays.
         if props["nbands"] == 1:
             image, axplanes, pre, suf = process_single_band_image(f, props)
@@ -30,80 +34,119 @@
     if "PREFIX" in name:
         return pre
     elif "SUFFIX" in name:
         return suf
     return image
 
 
-def make_format_specifications(props):
-    """"""
+def make_format_specifications(props: ImageProps) -> tuple[str, np.dtype]:
+    """
+    Given an image properties dict, construct a struct format string and a
+    numpy dtype that could be used to interpret the described image using,
+    respectively, struct or numpy.
+    """
     endian, ctype = props["sample_type"][0], props["sample_type"][-1]
     struct_fmt = f"{endian}{props['pixels']}{ctype}"
     np_type = props["sample_type"][1:]
     dtype = np.dtype(f"{endian}{np_type}")
     return struct_fmt, dtype
 
 
-def extract_single_band_linefix(image, props):
-    """"""
+def extract_single_band_linefix(
+    image: np.ndarray, props: ImageProps
+) -> tuple[np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]:
+    """
+    If they exist, extract line prefixes and/or suffixes from a single-band
+    image (i.e., a 2D ndarray). Return the image shorn of pre/suffixes, the
+    prefixes (if any), and the suffixes (if any).
+    """
     if props["linepad"] == 0:
         return image, None, None
     prefix, suffix = None, None
     image = image.reshape(props["nrows"], props["ncols"] + props["linepad"])
     if props.get("line_suffix_pix", 0) > 0:
         suffix = image[:, -props["line_suffix_pix"] :]
         image = image[:, : -props["line_suffix_pix"]]
     if props.get("line_prefix_pix", 0) > 0:
         prefix = image[:, : props["line_prefix_pix"]]
         image = image[:, props["line_prefix_pix"] :]
     return image, prefix, suffix
 
 
-def convert_if_vax(image, props):
-    """"""
+def convert_if_vax(image: np.ndarray, props: dict) -> np.ndarray:
+    """If an array is in 32-bit VAX real format, convert it to 32-bit float."""
     if props.get('is_vax_real') is True:
         return vax.from_vax32(image)
     return image
 
 
-def process_single_band_image(f, props):
-    """"""
+def process_single_band_image(
+    f: BufferedIOBase, props: ImageProps
+) -> tuple[
+    np.ndarray,
+    dict[str, np.ndarray],
+    Optional[np.ndarray],
+    Optional[np.ndarray]
+]:
+    """
+    Load a single-band image from an open file stream,
+    perform any cleanup / segmentation operations implied by the `props` dict,
+    and return it, along with any side/bottom/topplanes or line pre/suffixes.
+    """
     _, numpy_dtype = make_format_specifications(props)
     # TODO: added this 'count' parameter to handle a case in which the image
     #  was not the last object in the file. We might want to add it to
     #  the multiband loaders too.
     image = np_from_buffered_io(f, dtype=numpy_dtype, count=props["pixels"])
     image, prefix, suffix = extract_single_band_linefix(image, props)
     image = convert_if_vax(image, props)
     image = image.reshape(
         (props["nrows"] + props["rowpad"], props["ncols"] + props["colpad"])
     )
     image, axplanes = extract_axplanes(image, props)
     return make_c_contiguous(image), axplanes, prefix, suffix
 
 
-def extract_bil_linefix(image, props):
-    """"""
+def extract_bil_linefix(
+    image: np.ndarray, props: ImageProps
+) -> tuple[np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]:
+    """
+    If they exist, extract line prefixes and/or suffixes from a raveled BIL
+    (LINE_INTERLEAVED) image. Return the image shorn of pre/suffixes, the
+    prefixes (if any), and the suffixes (if any).
+    """
     if props["linepad"] == 0:
         return image, None, None
     prefix, suffix = None, None
     image = image.reshape(props["nrows"], int(image.size / props["nrows"]))
     if props.get("line_suffix_pix") is not None:
         suffix = image[:, -props["line_suffix_pix"] :]
         image = image[:, : -props["line_suffix_pix"]]
     if props.get("line_prefix_pix") is not None:
         prefix = image[:, : props["line_prefix_pix"]]
         image = image[:, props["line_prefix_pix"] :]
     return image, prefix, suffix
 
 
-def process_multiband_image(f, props):
-    """"""
+def process_multiband_image(f: BufferedIOBase, props: ImageProps) -> tuple[
+    np.ndarray,
+    dict[str, np.ndarray],
+    Optional[np.ndarray],
+    Optional[np.ndarray]
+]:
+    """
+    Load the elements of a multiband image from an open file stream, reshape
+    the resulting array as appropriate for the image's band storage type,
+    perform any cleanup / segmentation operations implied by the `props` dict,
+    and return it, along with any side/bottom/topplanes or line pre/suffixes.
+    """
     bst = props["band_storage_type"]
-    if bst not in ("BAND_SEQUENTIAL", "LINE_INTERLEAVED", "SAMPLE_INTERLEAVED"):
+    if bst not in (
+        "BAND_SEQUENTIAL", "LINE_INTERLEAVED", "SAMPLE_INTERLEAVED"
+    ):
         warnings.warn(
             f"Unsupported BAND_STORAGE_TYPE={bst}. Guessing BAND_SEQUENTIAL."
         )
         bst = "BAND_SEQUENTIAL"
     _, numpy_dtype = make_format_specifications(props)
     image = np_from_buffered_io(f, numpy_dtype, count=props["pixels"])
     image = convert_if_vax(image, props)
@@ -115,25 +158,33 @@
     prefix, suffix = None, None
     if bst == "BAND_SEQUENTIAL":
         image = image.reshape(bands, lines, samples)
     elif bst == "SAMPLE_INTERLEAVED":
         image = image.reshape(lines, samples, bands)
         image = np.moveaxis(image, 2, 0)
     elif bst == "LINE_INTERLEAVED":
+        # NOTE: we haven't implemented linefix extraction for non-BIL images
+        # because we haven't yet found any non-BIL multiband images in the PDS
+        # with linefixes. queries.check_fix_validity() will throw a
+        # NotImplementedError should it ever encounter them, at which point
+        # we can implement support for them.
         image, prefix, suffix = extract_bil_linefix(image, props)
         image = image.reshape(lines, bands, samples)
         image = np.moveaxis(image, 0, 1)
     image, axplanes = extract_axplanes(image, props)
     return make_c_contiguous(image), axplanes, prefix, suffix
 
 
-def extract_axplanes(image, props):
-    """extract ISIS-style side/bottom/backplanes from an array"""
+def extract_axplanes(
+    image: np.ndarray, props: ImageProps
+) -> tuple[np.ndarray, dict[str, np.ndarray]]:
+    """extract ISIS-style side/bottom/top/backplanes from an array"""
     axplanes = {}
     for side, ax in product(("prefix", "suffix"), ("row", "col", "band")):
+        # noinspection PyTypedDict
         if (count := props.get(f"{side}_{ax}s")) is None:
             continue
         axn, axname = {
             "band": (0, "BAND"),
             "row": (1, "LINE"),
             "col": (2, "SAMPLE"),
         }[ax]
@@ -148,14 +199,7 @@
                 pslice.append(slice(None, count))
             else:
                 aslice.append(slice(None, -count))
                 pslice.append(slice(-count, None))
         axplanes[f"{side}_{ax}s"] = image[tuple(pslice)]
         image = image[tuple(aslice)]
     return image, axplanes
-
-
-def make_c_contiguous(image: np.ndarray) -> np.ndarray:
-    """"""
-    if image.flags["C_CONTIGUOUS"] is False:
-        return np.ascontiguousarray(image)
-    return image
```

### Comparing `pdr-1.0.6/pdr/loaders/table.py` & `pdr-1.0.7/pdr/loaders/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,41 @@
-import re
+"""
+Functions for the nitty-gritty byte-juggling parts of
+TABLE/SPREADSHEET/ARRAY/HISTOGRAM loading.
+"""
+from __future__ import annotations
+from io import StringIO
+from typing import Optional, TYPE_CHECKING
+
 import numpy as np
 import pandas as pd
-from io import StringIO
+from multidict import MultiDict
 from pandas.errors import ParserError
+import re
 
-from pdr.loaders._helpers import check_explicit_delimiter
-from pdr.loaders.queries import get_array_num_items
 from pdr import bit_handling
 from pdr.datatypes import sample_types
+from pdr.loaders._helpers import check_explicit_delimiter
+from pdr.loaders.queries import get_array_num_items
 from pdr.np_utils import np_from_buffered_io, enforce_order_and_object
-from pdr.pd_utils import booleanize_booleans, convert_ebcdic, convert_ibm_reals, compute_offsets
+from pdr.pd_utils import (
+    booleanize_booleans, compute_offsets, convert_ebcdic, convert_ibm_reals
+)
 from pdr.utils import decompress, head_file
 
+if TYPE_CHECKING:
+    from pdr.pdrtypes import DataIdentifiers
+
+
+PAD_CHARACTERS = ' \t",'
+"""
+Characters we want to strip from the beginning/end of every element of an 
+ASCII table.
+"""
+
 
 def read_array(fn, block, start_byte, fmtdef_dt):
     """
     Read an array object from this product and return it as a numpy array.
     """
     if block.get("INTERCHANGE_FORMAT") == "BINARY":
         _, dt = fmtdef_dt
@@ -54,31 +74,28 @@
     fn,
     fmtdef_dt,
     table_props,
     block,
     start_byte,
 ):
     """
-    Read a table. Parse the label format definition and then decide
-    whether to parse it as text or binary.
+    Read a table. Parse the label format definition and then decide whether to
+    treat the table as text or binary.
     """
     fmtdef, dt = fmtdef_dt
     if dt is None:  # we believe object is an ascii file
         table = _interpret_as_ascii(
             identifiers, fn, fmtdef, block, table_props
         )
         if len(table.columns) != len(fmtdef):
             table.columns = [
                 f for f in fmtdef['NAME'] if not f.startswith('PLACEHOLDER')
         ]
         else:
             table.columns = fmtdef['NAME']
-#        print("columns\n", table.columns)
-#        print("names\n", fmtdef['NAME'])
-#        print("last\n", table.iloc[-1, 0])
     else:
         table = _interpret_as_binary(fn, fmtdef, dt, block, start_byte)
     table = _drop_placeholders(table)
     # If there is an offset and/or scaling factor, apply them:
     if fmtdef.get("OFFSET") is not None or fmtdef.get("SCALING_FACTOR") is not None:
         for col in table.columns:
             record = fmtdef.loc[fmtdef['NAME'] == col].to_dict("records")[0]
@@ -109,93 +126,124 @@
     table.columns = fmtdef.NAME.tolist()
     table = convert_ebcdic(table, fmtdef)
     table = booleanize_booleans(table, fmtdef)
     table = bit_handling.expand_bit_strings(table, fmtdef)
     return table
 
 
-# TODO: this is still generally hacky and should be untangled
-# noinspection PyTypeChecker
-def _interpret_as_ascii(identifiers, fn, fmtdef, block, table_props):
-    """
-    read an ASCII table. first assume it's delimiter-separated; attempt to
-    parse it as a fixed-width table if that fails.
+def _read_as_delimited(
+    fn: str,
+    identifiers: DataIdentifiers,
+    sep: str,
+    string_buffer: StringIO,
+    fmtdef: pd.DataFrame
+) -> Optional[pd.DataFrame]:
+    """
+    Attempt to read an ASCII table as a delimiter-separated file. We always
+    try this first before moving to a fixed-width parser.
+    """
+    table = pd.read_csv(string_buffer, sep=sep, header=None)
+    # TODO: adding this 'PLACEHOLDER' check has allowed many tables to use
+    #  read_csv() instead of read_fwf(), which is generally preferable
+    #  because read_fwf() is very slow. This may also be able to invalidate
+    #  some special cases; should check.
+    n_place = len(fmtdef.loc[fmtdef.NAME.str.contains('PLACEHOLDER')])
+    if len(table.columns) + n_place != len(fmtdef.NAME.tolist()):
+        raise IndexError("Mismatched column length.")
+    for c, d in zip(table.columns, table.dtypes):
+        if d.name == "object":
+            table[c] = table[c].str.strip(PAD_CHARACTERS)
+    return table
+
+
+def _read_fwf_with_colspecs(
+    fmtdef: pd.DataFrame, string_buffer: StringIO
+) -> pd.DataFrame:
+    """
+    Attempt to read an ASCII table as a fixed-width file using column
+    boundaries specified by or inferred from its format definition.
+    """
+    colspecs = []
+    # TODO: this if clause is a 'general special' statement, intended to handle
+    #  instances in which special cases call read_table_structure() but do not
+    #  pass its results to parse_table_structure() due to some special required
+    #  handling. We probably want to change something upstream to avoid this.
+    if "SB_OFFSET" not in fmtdef.columns:
+        position_records = compute_offsets(fmtdef).to_dict("records")
+    else:
+        position_records = fmtdef.to_dict("records")
+    for record in position_records:
+        if np.isnan(record.get("ITEM_BYTES", np.nan)):
+            col_length = record["BYTES"]
+        else:
+            col_length = int(record["ITEM_BYTES"])
+        colspecs.append(
+            (record["SB_OFFSET"], record["SB_OFFSET"] + col_length)
+        )
+    # NOTE: the 'delimiter' argument to read_fwf() does _not_ specify
+    # an actual delimiter. It defines characters the read_fwf parser
+    # will treat as 'padding' and strip from each table element.
+    table = pd.read_fwf(
+        string_buffer,
+        header=None,
+        colspecs=colspecs,
+        delimiter=PAD_CHARACTERS
+    )
+    return table
+
+
+def _read_table_from_stringio(
+    fmtdef: pd.DataFrame,
+    fn: str,
+    identifiers: DataIdentifiers,
+    block: MultiDict,
+    string_buffer: StringIO
+) -> pd.DataFrame:
+    """
+    Attempt to parse a string buffer, presumably containing an ASCII table, as
+    a pandas DataFrame. First try to treat it as a delimiter-separated table;
+    fall back to fixed-width parsing if that doesn't work.
     """
     # TODO, maybe: add better delimiter detection & dispatch
-    sep = check_explicit_delimiter(block)
+    try:
+        sep = check_explicit_delimiter(block)
+        return _read_as_delimited(fn, identifiers, sep, string_buffer, fmtdef)
+    except (IndexError, UnicodeError, AttributeError, ParserError):
+        string_buffer.seek(0)
+    if "BYTES" in fmtdef.columns:
+        try:
+            return _read_fwf_with_colspecs(fmtdef, string_buffer)
+        except (pd.errors.EmptyDataError, pd.errors.ParserError):
+            string_buffer.seek(0)
+    # last-ditch fallback if we don't have column specifications or using the
+    # column specifications didn't work. This usually won't work!
+    # NOTE: see note in _read_fwf_with_colspecs() on 'delimiter' argument
+    return pd.read_fwf(string_buffer, header=None, delimiter=PAD_CHARACTERS)
+
+
+def _interpret_as_ascii(
+    identifiers: DataIdentifiers,
+    fn: str,
+    fmtdef: pd.DataFrame,
+    block: MultiDict,
+    table_props: dict
+):
+    """Load text from a file and parse it as an ASCII table."""
     with decompress(fn) as f:
         if table_props["as_rows"] is False:
-            bytes_buffer = head_file(
+            bytesbuf = head_file(
                 f, nbytes=table_props["length"], offset=table_props["start"]
             )
-            string_buffer = StringIO(bytes_buffer.read().decode())
-            bytes_buffer.close()
+            try:
+                stringbuf = StringIO(bytesbuf.read().decode())
+            finally:
+                bytesbuf.close()
         else:
             if table_props["start"] > 0:
                 [next(f) for _ in range(table_props["start"])]
             if table_props["length"] in (None, ""):
                 lines = f.readlines()
             else:
                 lines = [next(f) for _ in range(table_props["length"])]
-            string_buffer = StringIO("\r\n".join(map(bytes.decode, lines)))
-        string_buffer.seek(0)
-    try:
-        table = pd.read_csv(string_buffer, sep=sep, header=None)
-    # TODO: I'm not sure this except clause is a good idea.
-    except (UnicodeError, AttributeError, ParserError):
-        table = None
-    if table is None:
-        try:
-            table = pd.DataFrame(
-                # TODO: are we ever actually using this at this point? note
-                #  that it will never work for compressed files.
-                np.loadtxt(
-                    fn,
-                    delimiter=sep,
-                    # TODO, maybe: this currently fails -- perhaps
-                    #  correctly -- when there is no LABEL_RECORDS key.
-                    #  but perhaps it is better to set a default of 0
-                    #  and avoid use of read_fwf. Update: Now has the possibility of
-                    #  the key being "". Unsure how this will affect the behavior.
-                    skiprows=identifiers["LABEL_RECORDS"],
-                )
-                .copy()
-                .newbyteorder("=")
-            )
-        except (TypeError, KeyError, ValueError):
-            pass
-    if table is not None:
-        # TODO: adding this placeholder check allows many tables to use
-        #  read_csv() instead of read_fwf(). This may be able to invalidate
-        #  some special cases; should check.
-        n_place = len(
-            fmtdef.loc[fmtdef.NAME.str.contains('PLACEHOLDER')]
-        )
-        if len(table.columns) + n_place == len(fmtdef.NAME.tolist()):
-            string_buffer.close()
-            for c, d in zip(table.columns, table.dtypes):
-                if d.name == "object":
-                    table[c] = table[c].str.strip('" \t')
-            return table
-    string_buffer.seek(0)
-    if "BYTES" in fmtdef.columns:
-        try:
-            if "SB_OFFSET" not in fmtdef.columns:
-                colspecs, position_records = [], compute_offsets(fmtdef).to_dict("records")
-            else:
-                colspecs, position_records = [], fmtdef.to_dict("records")
-            for record in position_records:
-                if np.isnan(record.get("ITEM_BYTES", np.nan)):
-                    col_length = record["BYTES"]
-                else:
-                    col_length = int(record["ITEM_BYTES"])
-                colspecs.append(
-                    (record["SB_OFFSET"], record["SB_OFFSET"] + col_length)
-                )
-            table = pd.read_fwf(string_buffer, header=None, colspecs=colspecs, delimiter='\t'+' '+'"'+',')
-            string_buffer.close()
-            return table
-        except (pd.errors.EmptyDataError, pd.errors.ParserError):
-            string_buffer.seek(0)
-    table = pd.read_fwf(string_buffer, header=None, delimiter='\t'+' '+'"'+',')
-    string_buffer.close()
-    return table
+            stringbuf = StringIO("\r\n".join(map(bytes.decode, lines)))
+    stringbuf.seek(0)
+    return _read_table_from_stringio(fmtdef, fn, identifiers, block, stringbuf)
```

### Comparing `pdr-1.0.6/pdr/loaders/utility.py` & `pdr-1.0.7/pdr/loaders/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""Support objects for 'utility' Loader subclasses."""
+
 from functools import partial
 from operator import contains
 from pathlib import Path
+from typing import Collection
 import warnings
 
 from multidict import MultiDict
 
 
 LABEL_EXTENSIONS = (".xml", ".lbl")
 IMAGE_EXTENSIONS = (".img", ".rgb")
@@ -22,30 +25,35 @@
     for any pointers we don't want to load and instead simply want ignored.
     """
     pass
 
 
 def tbd(name: str, block: MultiDict, *_, **__):
     """
-    This is a placeholder function for pointers that are
-    not explicitly supported elsewhere. It throws a warning and
+    This is a placeholder function for objects that are not explicitly
+    supported elsewhere. It throws a warning and
     passes just the value of the pointer.
     """
     warnings.warn(f"The {name} pointer is not yet fully supported.")
     return block
 
 
-def looks_like_this_kind_of_file(filename: str, kind_extensions) -> bool:
-    """"""
+def looks_like_this_kind_of_file(
+    filename: str, kind_extensions: Collection[str]
+) -> bool:
+    """Does this file have any of these extensions?"""
     is_this_kind_of_extension = partial(contains, kind_extensions)
     return any(map(is_this_kind_of_extension, Path(filename.lower()).suffixes))
 
 
-def is_trivial(pointer) -> bool:
-    """"""
+def is_trivial(pointer: str) -> bool:
+    """
+    Returns True if this is the name of a data object we want to handle
+    trivally, in the sense that we never ever want to load it directly.
+    """
     # TIFF tags / headers should always be parsed by the TIFF parser itself
     if (
         ("TIFF" in pointer)
         and ("IMAGE" not in pointer)
         and ("DOCUMENT" not in pointer)
     ):
         return True
```

### Comparing `pdr-1.0.6/pdr/np_utils.py` & `pdr-1.0.7/pdr/np_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 """
-methods for working with numpy objects, primarily intended as components of
-pdr.Data's processing pipelines.
+Methods for working with numpy objects, primarily intended as components of
+pdr's image- and table-loading routines.
 """
 from bz2 import BZ2File
 from gzip import GzipFile
 from io import BufferedIOBase, BytesIO
 from numbers import Number
-from typing import Collection, Optional, Union
+from typing import Optional, Union
 from zipfile import ZipFile
 
 import numpy as np
 
 
 def enforce_order_and_object(array: np.ndarray, inplace=True) -> np.ndarray:
     """
-    determine which, if any, of an array's fields are in nonnative byteorder
-    and swap them.
-
-    furthermore:
-    pandas does not support numpy void ('V') types, which are sometimes
-    required to deal with unstructured padding containing null bytes, etc.,
-    and are probably the appropriate representation for binary blobs like
-    bit strings. cast them to object so it does not explode. doing this here
-    is inelegant but is somewhat efficient.
-    TODO: still not that efficient
-    TODO: benchmark
-    """
+    Make an ndarray compatible for use with pandas or other similarly-strict
+    interfaces. Determine which, if any, of the array's fields are in nonnative
+    byteorder and swap them; also convert any void dtypes to object.
+    """
+    # NOTE: doing the void conversion in this function is inelegant but
+    # somewhat efficient.
+    # TODO: or is it? benchmark.
     if inplace is False:
         array = array.copy()
     if len(array.dtype) < 2:
         if len(array.dtype) == 0:
             dtype = array.dtype
             void_return = array
         else:
             dtype = array.dtype[0]
             # if we don't slice the field out explicitly, numpy will transform
             # it into an array of tuples
             void_return = array[tuple(array.dtype.fields.keys())[0]]
+
         if "V" in str(dtype):
             return void_return.astype("O")
         if dtype.isnative:
             return array
         return array.byteswap().newbyteorder("=")
     swap_targets = []
     swapped_dtype = []
@@ -65,56 +61,73 @@
         [isinstance(operand, int) for operand in operands]
     )
 
 
 # TODO: shake this out with a bunch of different compression type examples,
 #  including specific compressions on band/line/single-plane/etc. images,
 #  compressed binary tables, etc.
+# TODO: I'm not sure if the above TODO is still relevant.
 def np_from_buffered_io(
     buffered_io: BufferedIOBase,
     dtype: Union[np.dtype, str],
     offset: Optional[int] = None,
     count: Optional[int] = None,
-):
+) -> np.ndarray:
     """
-    return a numpy array from a buffered IO object, first decompressing it in
-    memory if it's a compressed buffer, and just using np.fromfile if it's not
+    Read a 1D numpy array of the specified dtype, size, and offset from a
+    buffered IO object.
     """
     if offset is not None:
         buffered_io.seek(offset)
     if isinstance(buffered_io, (BZ2File, ZipFile, GzipFile, BytesIO)):
+        # we need to read the appropriate amount into a new buffer, especially
+        # if it's monolithically compressed
         n_bytes = None if count is None else count * dtype.itemsize
         stream = BytesIO(buffered_io.read(n_bytes))
         return np.frombuffer(stream.getbuffer(), dtype=dtype)
     count = -1 if count is None else count
+    # In this case, buffered_io is just an open file stream
     return np.fromfile(buffered_io, dtype=dtype, count=count)
 
 
 def make_c_contiguous(arr: np.ndarray) -> np.ndarray:
-    """"""
+    """
+    If an ndarray isn't C-contiguous, reorder it as C-contiguous. If it is,
+    don't mess with it.
+    """
     if arr.flags["C_CONTIGUOUS"] is False:
         return np.ascontiguousarray(arr)
     return arr
 
 
 # TODO: really all arguments but ibm/sreg are redundant for basic S/360 formats
-def ibm_to_np(ibm, sreg, ereg, mmask):
-    """"""
+def ibm_to_np(ibm: np.ndarray, sreg: int, ereg: int, mmask: int) -> np.ndarray:
+    """
+    Convert an array composed of IBM System 360-style floats (expressed as
+    4- or 8-byte unsigned integers, as appropriate for byte width) to numpy
+    float64.
+    """
     # dtype conversion: this field must be signed
     ibm_sign = (ibm >> sreg & 0x01).astype('int8')
-    # dtype_conversion: largest values possible will overfloat int64 or float32
+    # dtype conversion: largest values possible will overfloat int64 or float32
     ibm_exponent = (ibm >> ereg & 0x7f).astype('float64')
     ibm_mantissa = ibm & mmask
     mantissa = ibm_mantissa / (2 ** ereg)
     exponent = 16 ** (ibm_exponent - 64)
     sign = 1 - (2 * ibm_sign).astype('int8')
     return sign * mantissa * exponent
 
 
 def ibm32_to_np_f32(ibm):
-    """"""
+    """
+    Convert an array of IBM System 360-style 32-bit floats (expressed as 32-bit
+    unsigned integers) to numpy float64.
+    """
     return ibm_to_np(ibm, 31, 24, 0x00ffffff)
 
 
 def ibm64_to_np_f64(ibm):
-    """"""
+    """
+    Convert an array of IBM System 360-style 64-bit floats (expressed as 64-bit
+    unsigned integers) to numpy float64.
+    """
     return ibm_to_np(ibm, 63, 56, 0x00ffffffffffffff)
```

### Comparing `pdr-1.0.6/pdr/parselabel/pds3.py` & `pdr-1.0.7/pdr/parselabel/pds3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-"""simple parsing utilities for PDS3 labels."""
+"""Parsing utilities for PDS3 labels."""
 from ast import literal_eval
 import re
+from numbers import Number
 from operator import eq
 from pathlib import Path
-from typing import Iterable, Mapping, Optional, Type, Union, Collection, Any
+from typing import Iterable, Mapping, Optional, Type, Union, Collection, Any, \
+    Hashable, Callable
 import warnings
 
 from cytoolz import groupby, identity
 from dustgoggles.func import constant
 from dustgoggles.structures import dig_for_keys
 from more_itertools import split_before
 from multidict import MultiDict
@@ -18,23 +20,23 @@
 
 PVL_BLOCK_INITIALS = ("OBJECT", "GROUP", "BEGIN_OBJECT", "BEGIN_GROUP")
 PVL_BLOCK_TERMINAL = re.compile(r"END(_OBJECT|$)")
 PVL_QUANTITY_VALUE = re.compile(r"((\d|\.|-)+([eE]-?\d+)?)|NULL|UNK|N/A")
 PVL_QUANTITY_UNITS = re.compile(r"<(.*)>")
 
 
-def extract_pvl_block_terminal(line):
-    """"""
+def extract_pvl_block_terminal(line: str) -> Optional[str]:
+    """get the PVL block terminator, if any, from a string"""
     try:
         return re.match(PVL_BLOCK_TERMINAL, line).group()
     except AttributeError:
         return None
 
 
-def is_an_assignment_line(line):
+def is_an_assignment_line(line: str) -> bool:
     """
     pick lines that begin assignment statements.
 
     in PDS labels, it never (?) seems to be the case that people use
     delimiters to put multiple assignment statements on a line
 
     there is an issue with people who put '=' in text blocks --
@@ -46,15 +48,15 @@
         return False
     start = line[:8]
     if start != start.upper():
         return False
     return True
 
 
-def chunk_statements(trimmed_lines: Iterable[str]):
+def chunk_statements(trimmed_lines: Iterable[str]) -> list[tuple[str, str]]:
     """chunk trimmed lines from a pvl-text into assignment statements."""
     statements = []
     for statement in split_before(trimmed_lines, is_an_assignment_line):
         assignment = statement[0]
         if (terminal := extract_pvl_block_terminal(assignment)) is not None:
             statements.append((terminal, ""))
             continue
@@ -68,35 +70,41 @@
             continue
         value_head += " ".join(map(str.strip, statement[1:]))
         statements.append((parameter, value_head))
     return statements
 
 
 class BlockParser:
-    """"""
+    """
+    Utility class for stateful recursive parsing and aggregation of a series
+    of PVL statements.
+    """
     def __init__(self):
         """"""
         self.names, self.aggregations, self.parameters = [], [MultiDict()], []
 
     def _step_out(self):
-        """"""
+        """Exit a block."""
         self.add_statement(self.names.pop(), self.aggregations.pop())
 
     def _step_in(self, name):
-        """"""
+        """Enter a block."""
         self.names.append(name)
         self.aggregations.append(MultiDict())
 
     def add_statement(self, parameter, value):
-        """"""
+        """Add a statement."""
         self.aggregations[-1].add(parameter, value)
         self.parameters.append(parameter)
 
-    def parse_statements(self, statements):
-        """"""
+    def parse_statements(self, statements) -> tuple[MultiDict, list[str]]:
+        """
+        Parse a series of PVL statements into a (possibly nested) MultiDict
+        and a flattened list of all keys at all levels of that MultiDict.
+        """
         for parameter, value in statements:
             if parameter in PVL_BLOCK_INITIALS:
                 self._step_in(value)
             elif parameter.startswith("END"):
                 # not bothering with aggregation name verification
                 if len(self.names) > 0:
                     self._step_out()
@@ -111,58 +119,65 @@
                 "consider increasing max_size or passing a larger number as "
                 "the pvl_limit parameter when initializing the calling "
                 "pdr.Data object."
             )
         return self.aggregations[0], self.parameters
 
 
-def looks_pvl(filename):
-    """"""
+def looks_pvl(filename) -> bool:
+    """Is this probably a PVL file?"""
     return Path(filename).suffix.lower() in (".lbl", ".fmt")
 
 
-def parse_pvl(label, deduplicate_pointers=True):
-    """"""
+def parse_pvl(
+    label: str, deduplicate_pointers: bool = True
+) -> tuple[MultiDict, list[str]]:
+    """Parse a PVL-text into a MultiDict and a flattened list of keys."""
     uncommented_label = re.sub(r"/\*.*?(\r|\n|/\*)", "\n", label)
     trimmed_lines = filter(
         None, map(lambda line: line.strip(), uncommented_label.split("\n"))
     )
     statements = chunk_statements(trimmed_lines)
     mapping, params = BlockParser().parse_statements(statements)
     if deduplicate_pointers:
         pointers = get_pds3_pointers(mapping)
         mapping, params = index_duplicate_pointers(pointers, mapping, params)
     return mapping, params
 
 
-def read_pvl(filename, deduplicate_pointers=True, max_size=DEFAULT_PVL_LIMIT):
-    """"""
+def read_pvl(
+    filename: Union[str, Path],
+    deduplicate_pointers: bool = True,
+    max_size: int = DEFAULT_PVL_LIMIT
+) -> tuple[MultiDict, list[str]]:
+    """Read and parse a file containing a PVL-text."""
     with decompress(filename) as stream:
         errors = "replace" if looks_pvl(filename) else "strict"
         label = trim_label(stream, max_size).decode("utf-8", errors=errors)
     return parse_pvl(label, deduplicate_pointers)
 
 
-def parse_pvl_quantity_object(obj):
-    """"""
+def parse_pvl_quantity_object(obj: str) -> dict[str, Union[str, Number]]:
+    """
+    Parse a PVL quantity string into a dict like {'value': 2, 'units': 'km'}.
+    """
     return {
         "value": literalize_pvl(
             re.search(PVL_QUANTITY_VALUE, obj).group()
         ),
         "units": literalize_pvl(re.search(PVL_QUANTITY_UNITS, obj).group(1)),
     }
 
 
-def parse_pvl_quantity_statement(statement):
+def parse_pvl_quantity_statement(statement: str) -> Any:
     """
     parse pvl statements including quantities. returns quantities as mappings.
     this will also handle statements that do not consist entirely of
-    quantities, notably including tuples of the form
-    ("SOMETHING.DAT", 1000 <BYTES>) that are commonly used to specify offsets
-    within files for data objects
+    quantities, notably including tuples of the form '("A5.DAT", 1000 <BYTES>)'
+    that are commonly used to specify start byte offsets for data objects.
     """
     objects = statement.strip("()").split(",")
     output = []
     for obj in objects:
         # TODO, maybe: a bit redundant
         if ("<" in obj) and (">" in obj):
             try:
@@ -174,42 +189,46 @@
             output.append(literalize_pvl(obj))
     if len(output) == 1:
         return output[0]
     return tuple(output)
 
 
 def multidict_dig_and_edit(
-    input_multidict,
-    target,
-    input_object=None,
-    predicate=eq,
-    setter_function=None,
-    key_editor=False,
-    keep_values=True,
-):
-    """
-    This function searches through a multidict's items, recursively continuing
-    into any children that are themselves multidicts, looking for keys that
-    match "target".
+    input_multidict: MultiDict,
+    target: Any,
+    input_object: Any = None,
+    predicate: Callable[[Any, Any], bool] = eq,
+    setter_function: Callable = None,
+    key_editor: bool = False,
+    keep_values: bool = True,
+    mtypes: tuple[type, ...] = (MultiDict,)
+) -> MultiDict:
+    """
+    This function produces a modified copy of a MultiDict (or other mapping,
+    but may produce unintended results). It searches through
+    a MultiDict's items, recursively continuing into any children that are
+    an instance of mtypes, and checking for keys for which
+    `predicate(key, target)` (by default meaning `key == target`) is `True`.
+
     If "key_editor" is False, the function changes the values associated with
     those keys. if it is True, the function changes the key names themselves.
 
     If "setter_function" is not None, it replaces those keys/values with the
     output of "setter function", executed with "input_object" and the original
     key/value as arguments. If it is None, it will simply replace them with
     "input_object".
 
-    If "keep_values" is not True, the output_multidict will contain _only_
+    If "keep_values" is not True, the returned MultiDict will contain _only_
     edited values, causing this to also act as a filtering function.
     """
     output_multidict = MultiDict()
     if setter_function is None:
         setter_function = constant(input_object)
     for key, value in input_multidict.items():
-        if isinstance(value, MultiDict):
+        if isinstance(value, mtypes):
             edited_multidict = multidict_dig_and_edit(
                 value,
                 target,
                 input_object,
                 predicate,
                 setter_function,
                 key_editor,
@@ -230,35 +249,41 @@
             output_multidict.add(key, setter_function(input_object, value))
         else:
             output_multidict.add(setter_function(input_object, key), value)
     return output_multidict
 
 
 def parse_non_base_10(text: str) -> int:
-    """"""
+    """
+    Convert a PVL representation of a non-base-10 integer to a base-10 Python
+    integer.
+    """
     try:
         base, number = text[:-1].split("#")
         return int(number, int(base))
     except ValueError:
         raise SyntaxError("possible malformatted non-base-10 number")
 
 
 def parse_non_base_10_collection(
     class_: Union[Type[set], Type[tuple]], obj: str
 ) -> Union[tuple[int], set[int]]:
-    """"""
+    """
+    Convert a collection of PVL representations of non-base-10 integers to a
+    collection (of the same class) of base-10 Python integers.
+    """
     return class_(
         map(parse_non_base_10, obj.strip('{}()').replace(" ", '').split(','))
     )
 
 
 def parse_unusual_collection(
     obj: str
 ) -> Union[tuple[Union[int, str]], set[Union[int, str]]]:
-    """handle collections of non-base-10 numbers or unquoted strings"""
+    """Parse a PVL collection of non-base-10 numbers or unquoted strings."""
     class_ = set if obj.startswith('{') else tuple
     if re.match(r'.*\d{1,2}#', obj):
         try:
             return parse_non_base_10_collection(class_, obj)
         except (SyntaxError, ValueError):
             pass
     return class_([s.strip(' ') for s in obj.strip('{}()').split(',')])
@@ -293,30 +318,36 @@
             pass
         except IndexError:
             a = 1
     return obj
 
 
 def literalize_pvl_block(block: MultiDict) -> MultiDict:
-    """"""
+    """
+    Parse the values of an entire (possibly-nested) MultiDict whose values are
+    PVL strings into Python objects.
+    """
     literalized = multidict_dig_and_edit(
         block,
         None,
         predicate=lambda x, y: True,
         setter_function=lambda _, obj: literalize_pvl(obj),
     )
     return literalized
 
 
 def get_pds3_pointers(
     label: Optional[MultiDict] = None,
-) -> tuple:
+) -> tuple[str]:
     """
     attempt to get all PDS3 "pointers" -- PVL parameters starting with "^" --
-    from a MultiDict generated from a PDS3 label
+    from a MultiDict generated from a PDS3 label. These typically specify
+    physical data locations, and in most cases correspond to data object
+    definitions later in the label (common exceptions include "^STRUCTURE" and
+    "^DATA_SET_MAP_PROJECTION").
     """
     return dig_for_keys(
         label, lambda k, _: k.startswith("^"), mtypes=(dict, MultiDict)
     )
 
 
 def pointerize(string: str) -> str:
@@ -325,16 +356,27 @@
 
 
 def depointerize(string: str) -> str:
     """prevent a string from starting with ^"""
     return string[1:] if string.startswith("^") else string
 
 
-def index_duplicate_pointers(pointers, mapping, params):
-    """"""
+def index_duplicate_pointers(
+    pointers: Collection[str], mapping: MultiDict, params: list[str]
+) -> tuple[MultiDict, list[str]]:
+    """
+    Although technically illegal, some PDS3 objects have multiple data objects
+    with the same name. This produces counterintuitive results. This function
+    appends ascending integers to any duplicate members of a specified set of
+    "pointer" keys of a MultiDict, and also their "depointerized" versions,
+    in order to distinguish data objects. This _can_ potentially fail if
+    duplicate-named object pointers and their corresponding object definitions
+    are not given in the same order in a label, but we have not yet
+    encountered that case.
+    """
     if pointers is None:
         return mapping, params
     # noinspection PyTypeChecker
     pt_groups = groupby(identity, pointers)
     for pointer, group in pt_groups.items():
         if (len(group) > 1) and (
             pointer not in ("^STRUCTURE", "^DESCRIPTION", "^PDS_OBJECT")
@@ -368,12 +410,15 @@
                 params.append(indexed_pointer)
                 params.append(indexed_depointer)
                 params.remove(pointer)
                 params.remove(depointer)
     return mapping, params
 
 
-def set_key_index(pointer_range: list, key: str) -> str:
-    """"""
+def set_key_index(pointer_range: list[int], key: str) -> str:
+    """
+    utility setter function for `multidict_dig_and_edit()` as called by
+    `index_duplicate_pointers()`; appends a number from a list to a string
+    """
     indexed_key = f"{key}_{pointer_range[0]}"
     pointer_range.pop(0)
     return indexed_key
```

### Comparing `pdr-1.0.6/pdr/pd_utils.py` & `pdr-1.0.7/pdr/pd_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
-methods for working with pandas objects, primarily intended as components of
-pdr.Data's processing pipelines. some may require a Data object as an
-argument.
+Methods for working with pandas objects, primarily intended for use in
+TABLE/ARRAY/SPREADSHEET/HISTOGRAM-loading workflows.
 """
+from __future__ import annotations
+from itertools import chain
 import re
+from typing import Hashable, TYPE_CHECKING
 import warnings
-from typing import Hashable
 
+from more_itertools import divide
 import numpy as np
-import pandas.api.types
 import pandas as pd
-from more_itertools import chunked, divide
+import pandas.api.types
 from pandas.errors import SettingWithCopyWarning
 
 from pdr.datatypes import sample_types
 from pdr.formats import check_special_sample_type
-from pdr.np_utils import enforce_order_and_object, ibm32_to_np_f32, \
-    ibm64_to_np_f64
+from pdr.np_utils import (
+    enforce_order_and_object, ibm32_to_np_f32, ibm64_to_np_f64
+)
+
+if TYPE_CHECKING:
+    from pdr.pdrtypes import DataIdentifiers
 
 
 def numeric_columns(df: pd.DataFrame) -> list[Hashable]:
-    """"""
+    """Return names of all 'numeric' columns in a DataFrame."""
     return [
         col
         for col, dtype in df.dtypes.iteritems()
         if pandas.api.types.is_numeric_dtype(dtype)
     ]
 
 
@@ -36,83 +41,101 @@
 
     include START_BYTE in string for values marked as RESERVED.
     """
     namegroups = df.groupby(column)
     for name, field_group in namegroups:
         if len(field_group) == 1:
             continue
+        # TODO: check what this is hitting.
         if name == "RESERVED":
             name = f"RESERVED_{field_group['START_BYTE'].iloc[0]}"
         names = [f"{name}_{ix}" for ix in range(len(field_group))]
         df.loc[field_group.index, column] = names
     return df
 
 
-def _apply_item_offsets(fmtdef):
-    """"""
+def _apply_item_offsets(fmtdef: pd.DataFrame) -> pd.Series:
+    """
+    Select item offsets (for a column or container with multiple items). If
+    the specification didn't give item offsets, just assume they're equal to
+    the byte width (i.e. there's no variable padding between fields).
+    """
     item_offsets = fmtdef["ITEM_BYTES"].copy()
     if "ITEM_OFFSET" not in fmtdef.columns:
         return item_offsets
     offset = fmtdef.loc[fmtdef["ITEM_OFFSET"].notna()]
     if (offset["ITEM_OFFSET"] < offset["ITEM_BYTES"]).any():
         raise ValueError(
             "Don't know how to intepret a field narrower than its value."
         )
     item_offsets.loc[offset.index] = offset["ITEM_OFFSET"]
     return item_offsets
 
 
-def compute_offsets(fmtdef):
+def compute_offsets(fmtdef: pd.DataFrame) -> pd.DataFrame:
     """
-    given a DataFrame containing PDS3 binary table structure specifications,
-    including a START_BYTE column, add an SB_OFFSET column, unpacking objects
-    if necessary
+    PDS3 TABLE/SPREADSHEET/ARRAY specifications do not explicitly give the
+    correct byte offsets for CONTAINERs, COLLECTIONs, anything loaded in by
+    reference from a STRUCTURE, or repeated elements of a COLUMN. Byte offsets
+    in these cases always refer to their parent containers, which can repeat,
+    have children with their own repetitions, etc., etc. This function
+    'unpacks' a format definition as necessary and adds an SB_OFFSET column
+    giving the correct byte offsets (from record start) for each field of the
+    data table/array.
     """
     # START_BYTE is 1-indexed, but we're preparing these offsets for
     # numpy, which 0-indexes
     fmtdef["SB_OFFSET"] = fmtdef["START_BYTE"].astype(int) - 1
     if "ROW_PREFIX_BYTES" in fmtdef.columns:
         fmtdef["SB_OFFSET"] += fmtdef["ROW_PREFIX_BYTES"]
-    block_names = fmtdef.loc[fmtdef['NAME'] != "PLACEHOLDER_0", "BLOCK_NAME"].unique()
+    block_names = fmtdef.loc[
+        fmtdef['NAME'] != "PLACEHOLDER_0", "BLOCK_NAME"
+    ].unique()
     # calculate offsets for formats loaded in by reference
     for block_name in block_names[1:]:
         if block_name in ("PLACEHOLDER_None", f"PLACEHOLDER_{block_names[0]}"):
             continue
         fmt_block = fmtdef.loc[fmtdef["BLOCK_NAME"] == block_name]
         if "PLACEHOLDER" in block_name:
             prior = fmtdef[fmtdef["NAME"] == block_name].squeeze()
         else:
             prior = fmtdef.loc[fmt_block.index[0] - 1]
         fmtdef.loc[fmt_block.index, "SB_OFFSET"] += (
             prior["SB_OFFSET"] + prior["BYTES"]
         )
         count = fmt_block["BLOCK_REPETITIONS"].iloc[0]
-        if prior["BLOCK_REPETITIONS"]:
+        if (reps := prior["BLOCK_REPETITIONS"]) > 1:
             if "PLACEHOLDER" in block_name:
-                fmtdef.loc[fmt_block.index, "BLOCK_REPETITIONS"] *= prior["BLOCK_REPETITIONS"]
+                fmtdef.loc[fmt_block.index, "BLOCK_REPETITIONS"] *= reps
             else:
-                count = count * prior["BLOCK_REPETITIONS"]
+                count *= reps
         if count == 1:
             continue
         chunks = tuple(map(list, divide(count, fmt_block.index)))
         block_size = fmt_block['BLOCK_BYTES'].iloc[0]
         if block_size != int(block_size):
             raise NotImplementedError("irregular repeated container size.")
         block_size = int(block_size)
-        for repetition, indices in enumerate(chunks):
-            fmtdef.loc[indices, "SB_OFFSET"] += int(repetition * block_size)
+        offset_chain = chain(
+            *[[i for _ in c] for (i, c) in enumerate(chunks)]
+        )
+        fmtdef.loc[
+            fmt_block.index, "SB_OFFSET"
+        ] += np.array(list(offset_chain)) * block_size
     # correctly compute offsets within columns w/multiple items
-    # TODO: ITEM_BYTES will _always_ be in fmtdef because we filled it with NaN earlier
-    if "ITEM_BYTES" in fmtdef:
+    if "ITEM_BYTES" in fmtdef.columns:
         fmtdef["ITEM_SIZE"] = _apply_item_offsets(fmtdef)
         column_groups = fmtdef.loc[fmtdef["ITEM_SIZE"].notna()]
-        for _, group in column_groups.groupby("SB_OFFSET"):
-            fmtdef.loc[group.index, "SB_OFFSET"] = group["SB_OFFSET"] + int(
-                group["ITEM_SIZE"].iloc[0]
-            ) * np.arange(len(group))
+        group_offs = column_groups['SB_OFFSET'].value_counts().sort_index()
+        gix_list, position = [], 0
+        for off, gl in zip(group_offs.index, group_offs.values):
+            itemsize = int(column_groups['ITEM_SIZE'].iloc[position])
+            gix_list += [(i * itemsize) + off for i in range(gl)]
+            position += gl
+        fmtdef.loc[column_groups.index, 'SB_OFFSET'] = gix_list
     pad_length = 0
     end_byte = fmtdef["SB_OFFSET"].iloc[-1] + fmtdef["BYTES"].iloc[-1]
     if "ROW_BYTES" in fmtdef.columns:
         pad_length += fmtdef["ROW_BYTES"].iloc[0] - end_byte
     if "ROW_SUFFIX_BYTES" in fmtdef.columns:
         pad_length += fmtdef["ROW_SUFFIX_BYTES"].iloc[0]
     if pad_length > 0:
@@ -125,20 +148,21 @@
         }
         fmtdef = pd.concat(
             [fmtdef, pd.DataFrame([placeholder_rec])]
         ).reset_index(drop=True)
     return fmtdef
 
 
-def insert_sample_types_into_df(fmtdef, identifiers):
+def insert_sample_types_into_df(
+    fmtdef: pd.DataFrame, identifiers: DataIdentifiers
+) -> tuple[pd.DataFrame, np.dtype]:
     """
-    given a DataFrame containing PDS3 binary table structure specifications,
-    insert numpy-compatible data type strings into that DataFrame;
-    return that DataFrame along with a numpy dtype object generated from it.
-    used in the Data.read_table pipeline.
+    Insert numpy-compatible data type strings into a TABLE/ARRAY format
+    definition DataFrame. Also generate a numpy dtype object from that
+    DataFrame.
     """
     fmtdef["dt"] = None
     if "ITEM_BYTES" not in fmtdef.columns:
         fmtdef["ITEM_BYTES"] = np.nan
     data_types = tuple(
         fmtdef.groupby(["DATA_TYPE", "ITEM_BYTES", "BYTES"], dropna=False)
     )
@@ -157,71 +181,97 @@
                     dt, int(sample_bytes), for_numpy=True
                 )
         except KeyError:
             raise KeyError(
                 f"{data_type} is not a currently-supported data type."
             )
     if "BLOCK_NAME" in fmtdef.columns:
-        fmtdef = create_nested_array_dtypes(fmtdef)
-    dt = get_dtype(fmtdef)
+        fmtdef = construct_nested_array_format(fmtdef)
+    dt = fmtdef_to_dtype(fmtdef)
     return fmtdef, dt
 
 
-def get_dtype(fmtdef: pd.DataFrame):
-    """"""
+def fmtdef_to_dtype(fmtdef: pd.DataFrame) -> np.dtype:
+    """
+    Construct a structured (but ideally never nested, see
+    `construct_nested_array_format()` below) dtype from a format definition.
+    """
     dtype_spec = fmtdef[
-        [c for c in ("NAME", "dt", "SB_OFFSET") if c in fmtdef.columns]].to_dict("list")
+        [c for c in ("NAME", "dt", "SB_OFFSET") if c in fmtdef.columns]
+    ].to_dict("list")
     spec_keys = ("names", "formats", "offsets")[: len(dtype_spec)]
     return np.dtype({k: v for k, v in zip(spec_keys, dtype_spec.values())})
 
 
-def create_nested_array_dtypes(fmtdef: pd.DataFrame):
-    """"""
-    block_names_df = fmtdef.drop(fmtdef[fmtdef["NAME"] == "PLACEHOLDER_0"].index)
-    block_names = block_names_df["BLOCK_NAME"].unique()
-    for block_name in block_names[1:]:
+def construct_nested_array_format(fmtdef: pd.DataFrame) -> pd.DataFrame:
+    """
+    ARRAY objects can be deeply nested. This function computes the correct
+    byte offsets and dtypes (including array shape) for any nested subelements.
+    """
+    for block_name in fmtdef.loc[
+        fmtdef["NAME"] != "PLACEHOLDER_0", "BLOCK_NAME"
+    ].unique()[1:]:
         if block_name == "":
             continue
         fmt_block = fmtdef.loc[fmtdef["BLOCK_NAME"] == block_name]
         prior = fmtdef.loc[fmt_block.index[0] - 1]
-        if "AXIS_ITEMS" in prior.keys():
-            axis_items = prior["AXIS_ITEMS"]
-            if not np.isnan(axis_items):
-                with warnings.catch_warnings():
-                    warnings.filterwarnings("ignore", category=SettingWithCopyWarning)
-                    fmt_block["SB_OFFSET"] = fmt_block["SB_OFFSET"]-prior["SB_OFFSET"]
-                dt = get_dtype(fmt_block)
-                if isinstance(axis_items, float):
-                    axis_items = int(axis_items)
-                dt = (dt, axis_items)
-                fmtdef.at[fmt_block.index[0] - 1, "dt"] = dt
-                fmtdef = fmtdef[~fmtdef.NAME.isin(fmt_block.NAME)]
+        if "AXIS_ITEMS" not in prior.keys():
+            continue
+        if np.isnan(axis_items := prior["AXIS_ITEMS"]):
+            continue
+        with warnings.catch_warnings():
+            # TODO: We are intentionally setting with copy here. However, it
+            #  will start hard-failing in pandas 3.x and needs to be changed.
+            warnings.filterwarnings("ignore", category=SettingWithCopyWarning)
+            fmt_block[
+                "SB_OFFSET"
+            ] = fmt_block["SB_OFFSET"] - prior["SB_OFFSET"]
+        if isinstance(axis_items, float):
+            axis_items = int(axis_items)
+        dt = fmtdef_to_dtype(fmt_block)
+        fmtdef.at[fmt_block.index[0] - 1, "dt"] = (dt, axis_items)
+        fmtdef = fmtdef[~fmtdef.NAME.isin(fmt_block.NAME)]
     return fmtdef
 
 
 def booleanize_booleans(
     table: pd.DataFrame, fmtdef: pd.DataFrame
 ) -> pd.DataFrame:
-    """"""
+    """
+    We generally load boolean columns from binary tables as uint8 of value 0
+    or 1. This converts all such columns of a DataFrame to np.bool.
+    """
     boolean_columns = fmtdef.loc[fmtdef["DATA_TYPE"] == "BOOLEAN", "NAME"]
     table[boolean_columns] = table[boolean_columns].astype(bool)
     return table
 
 
 def convert_ebcdic(
     table: pd.DataFrame, fmtdef: pd.DataFrame
 ) -> pd.DataFrame:
-    ebcdic_columns = fmtdef.loc[fmtdef["DATA_TYPE"].str.contains("EBCDIC"), "NAME"]
+    """
+    Decode any columns of a DataFrame that contain bytestrings constructed from
+    IBM S/360-style EBCDIC-encoded text to Python strings.
+    """
+    ebcdic_columns = fmtdef.loc[
+        fmtdef["DATA_TYPE"].str.contains("EBCDIC"), "NAME"
+    ]
     for col in ebcdic_columns:
+        # TODO: why do we copy table[col] twice?
         series = pd.Series(table[col])
         table[col] = series.str.decode('cp500')
     return table
 
 
 def rectified_rec_df(array: np.ndarray) -> pd.DataFrame:
+    """
+    Attempt to 'flatten' a 1- or 2D ndarray, possibly with a structured dtype
+    but with no nested arrays, into a DataFrame, typecasting as necessary for
+    pandas compatibility.
+    """
     if len(array.shape) == 3:
         # it's possible to pack 2D arrays into individual records. this
         # obviously does not work for pandas. if we encounter > 2D elements,
         # we can generalize this.
         array = array.reshape(array.shape[0], array.shape[1] * array.shape[2])
     elif len(array.shape) > 3:
         raise NotImplementedError("dtypes with >2D elements are not supported")
@@ -230,14 +280,21 @@
         # it's slow and acts weird
         return pd.DataFrame(enforce_order_and_object(array))
     # but if it does, do
     return pd.DataFrame.from_records(enforce_order_and_object(array))
 
 
 def structured_array_to_df(array: np.ndarray) -> pd.DataFrame:
+    """
+    Attempt to convert an ndarray with a structured dtype to a DataFrame,
+    flattening any nested 1- or 2-D arrays into blocks of columns and
+    typecasting as necessary for pandas compatibility. This does not attempt
+    to flatten nested elements with dimensionality > 2, and will raise a
+    NotImplementedError if it encounters them.
+    """
     sub_dfs = []
     name_buffer = []
     for field in array.dtype.descr:
         if len(field) == 2:
             name_buffer.append(field[0])
         else:
             if len(name_buffer) > 0:
@@ -253,27 +310,28 @@
     if len(sub_dfs) == 1:
         return sub_dfs[0]
     return pd.concat(sub_dfs, axis=1)
 
 
 def convert_ibm_reals(df: pd.DataFrame, fmtdef: pd.DataFrame) -> pd.DataFrame:
     """
-    converts all IBM reals in a dataframe from packed 16- or 32-bit integer
-    form to floating-point
+    Converts all IBM reals in a dataframe from packed 32- or 64-bit integer
+    form to np.float32 or np.float64.
     """
     if not fmtdef['DATA_TYPE'].str.contains('IBM').any():
         return df
     reals = {}
     for _, field in fmtdef.iterrows():
         if not re.match(r'IBM.*REAL', field['DATA_TYPE']):
             continue
         func = ibm32_to_np_f32 if field['BYTES'] == 4 else ibm64_to_np_f64
         converted = func(df[field['NAME']].values)
         if field['BYTES'] == 4:
-            # IBM shorts are wider-range than IEEE shorts
+            # IBM shorts are wider-range than IEEE shorts; check if we can
+            # safely cast them back down to float32
             absolute = abs(converted)
             big = absolute.max() > np.finfo(np.float32).max
             nonzero = absolute[absolute > 0]
             if len(nonzero) > 0:
                 small = nonzero.min() < 1e-44
             else:
                 small = False
```

### Comparing `pdr-1.0.6/pdr/pdr.py` & `pdr-1.0.7/pdr/pdr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,58 @@
-import warnings
+from __future__ import annotations
 from functools import partial, cache
+from inspect import get_annotations
 from itertools import chain, product
+from numbers import Number
 from pathlib import Path
 from typing import (
+    Any,
+    Callable,
+    Collection,
+    Literal,
     Mapping,
     Optional,
-    Union,
     Sequence,
-    Collection,
-    Literal, Any, Callable,
+    TYPE_CHECKING,
+    Union,
 )
+import warnings
 
 import Levenshtein as lev
 from cytoolz import countby, identity
 from dustgoggles.dynamic import Dynamic
 from dustgoggles.func import gmap
 from dustgoggles.structures import dig_for_value, listify
 from dustgoggles.tracker import Tracker, TrivialTracker
 from multidict import MultiDict
 
 from pdr.errors import AlreadyLoadedError, DuplicateKeyWarning
-from pdr.formats import (
-    check_special_fn,
-    special_image_constants,
-)
+from pdr.formats import check_special_fn, special_image_constants
 from pdr.parselabel.pds3 import (
+    depointerize,
     get_pds3_pointers,
+    literalize_pvl,
     pointerize,
-    depointerize,
     read_pvl,
-    literalize_pvl,
 )
 from pdr.parselabel.pds4 import reformat_pds4_tools_label
 from pdr.parselabel.utils import DEFAULT_PVL_LIMIT
+from pdr.pdrtypes import DataIdentifiers
 from pdr.utils import (
     associate_label_file,
     catch_return_default,
     check_cases,
     check_primary_fmt,
     prettify_multidict,
 )
 
-
-ID_FIELDS = (
-    "INSTRUMENT_ID",
-    "INSTRUMENT_NAME",
-    "SPACECRAFT_NAME",
-    "PRODUCT_TYPE",
-    "DATA_SET_NAME",
-    "DATA_SET_ID",
-    "STANDARD_DATA_PRODUCT_ID",
-    "FILE_NAME",
-    "INSTRUMENT_HOST_NAME",
-    "PRODUCT_TYPE",
-    "PRODUCT_ID",
-    "RECORD_BYTES",
-    "RECORD_TYPE",
-    "ROW_BYTES",
-    "ROWS",
-    "FILE_RECORDS",
-    "LABEL_RECORDS",
-    "NOTE",
-)
-"""
-Standard 'identifier' fields for PDS3 products. Used to make special case 
-checks more compact.
-"""
+if TYPE_CHECKING:
+    import numpy as np
+    import pandas as pd
+    from PIL.Image import Image
 
 
 class Metadata(MultiDict):
     """
     MultiDict subclass intended primarily as a helper class for Data.
     includes various convenience methods for handling metadata syntaxes,
     common access and display interfaces, etc.
@@ -148,15 +131,15 @@
     def metaget_(
         self, text: str, default: Any = None, evaluate: bool = True
     ) -> Any:
         """quiet-by-default version of metaget"""
         return self.metaget(text, default, evaluate, False)
 
     def metaget_fuzzy(self, text: str, evaluate: bool = True) -> Any:
-        """"""
+        """Like `metaget()`, but fuzzy-matches key names."""
         levratio = {
             key: lev.ratio(key, text) for key in set(self.fieldcounts.keys())
         }
         if levratio == {}:
             return None
         peak = max(levratio.values())
         for k, v in levratio.items():
@@ -204,20 +187,23 @@
 
     def __repr__(self):
         """"""
         return f"Metadata({prettify_multidict(self)})"
 
 
 class DebugExceptionPreempted(Exception):
-    """"""
+    """
+    Stub Exception subclass for selectively ignoring Exceptions from load
+    failures when not in debug mode.
+    """
     pass
 
 
 class Data:
-    """"""
+    """Core `pdr` class."""
     def __init__(
         self,
         fn: Union[Path, str],
         *,
         debug: bool = False,
         label_fn: Optional[Union[Path, str]] = None,
         search_paths: Union[Collection[str], str] = (),
@@ -247,15 +233,15 @@
         self.file_mapping = {}
         # known special constants per data object
         self.specials = {}
         # dict to flag images loaded prescaled (currently only from FITS files)
         self._scaleflags = {}
         # where can we look for files containing data objects?
         # not yet fully implemented; only uses first (automatic) one.
-        self.search_paths = [self._init_search_paths()] + listify(search_paths)
+        self.search_paths = [self._init_search_path()] + listify(search_paths)
         self.standard = None
         # cache for pds4_tools.reader.general_objects.Structure objects.
         self._pds4_structures = None
         # cache for hdulist, for primary FITS files -- this is primarily
         # an optimization for compressed files
         self._hdulist = None
         # dict of [str, int] for cases in which we need to reindex duplicate
@@ -301,16 +287,21 @@
         # if self.pointers is None, we've probably got a weird edge case where
         # someone directly opened a PVL file that's not an individual product
         # label (e.g. a format file or a non-PDS PVL file) -- but there's no
         # reason to not allow them to use PDR as a PVL parser.
         if self.pointers is not None:
             self._find_objects()
         self.identifiers = {
-            field: self.metaget_(field, "") for field in ID_FIELDS
+            field: self.metaget_(field, "")
+            for field in get_annotations(DataIdentifiers)
         }
+        # it never does us any favors to have tuples or sets in here
+        for k, v in self.identifiers.items():
+            if isinstance(v, (tuple, set)):
+                self.identifiers[k] = str(v)
 
     def _init_pds4(self):
         """use pds4_tools to open pds4 files, but in our interface idiom."""
         # pds4_tools currently uses an outdated version of six.py that is
         # incompatible with Python 3.12. Replace it if necessary at runtime.
         from pdr._patches import patch_pds4_tools_six
 
@@ -323,70 +314,102 @@
         )
         for structure in structure_list.structures:
             self._pds4_structures[structure.id.replace(" ", "_")] = structure
             self.index.append(structure.id.replace(" ", "_"))
         self._pds4_structures["label"] = structure_list.label
         self.index.append("label")
 
-    def _init_search_paths(self):
-        """"""
+    def _init_search_path(self) -> str:
+        """
+        Set initial path this object will check for additional files (just the
+        directory that contains its "primary" file).
+        """
         for target in ("labelname", "filename"):
             if (target in dir(self)) and (target is not None):
                 return str(Path(self.getattr(target)).absolute().parent)
         raise FileNotFoundError
 
     def _find_objects(self):
-        """"""
+        """
+        Add all top-level data objects mentioned in the label to this object's
+        index, except for 'trivial' one (see `loaders.utility.is_trivial()`).
+        """
         from pdr.loaders.utility import is_trivial
 
         # TODO: make this not add objects again if called multiple times
         for pointer in self.pointers:
             object_name = depointerize(pointer)
             if is_trivial(object_name):
                 continue
             self.index.append(object_name)
 
     def _object_to_filename(self, object_name: str) -> Union[str, list[str]]:
-        """"""
+        """
+        Construct one or more on-disk search paths for the file that contains
+        a named data object. Does not actually check if files exist at those
+        paths (typically performed by calls to `utils.check_cases()).
+        """
         is_special, special_target = check_special_fn(
             self, object_name, self.identifiers
         )
         if is_special is True:
             return self.get_absolute_paths(special_target)
         is_comp, comp_paths = self._check_compressed_file_pointer(object_name)
         if is_comp is True:
             return comp_paths
         target = self.metaget_(pointerize(object_name))
         if isinstance(target, Sequence) and not (isinstance(target, str)):
             if isinstance(target[0], str):
                 target = target[0]
-        # TODO: should we move every check_cases call here?
         if isinstance(target, str):
             return self.get_absolute_paths(target)
         else:
             return self.filename
 
-    def _check_compressed_file_pointer(self, object_name):
-        """"""
+    def _check_compressed_file_pointer(
+        self, object_name: str
+    ) -> tuple[bool, Optional[tuple[Path, ...]]]:
+        """
+        When PDS3 labels describe data objects in compressed files, they often
+        give the names that the compressed files _would_ have, were someone to
+        decompress them, as the physical locations of those objects. This can
+        be confusing, because you cannot load an object from a merely
+        hypothetical file.
+
+        However, this is by no means a strict convention, so we can't just
+        assume that it's the case -- we have to check all the file names
+        mentioned for that object in the label, including those not given as
+        top-level pointers.
+        """
         compkeys = {"COMPRESSED_FILE", "UNCOMPRESSED_FILE"}
         if (
             len(compkeys.intersection(self.metadata.keys())) == 2
             and object_name in self.metablock_("UNCOMPRESSED_FILE").keys()
         ):
             blocks = filter(None, [self.metaget_(k) for k in compkeys])
             filenames = filter(None, [b.get("FILE_NAME") for b in blocks])
             return True, tuple(
                 chain.from_iterable(map(self.get_absolute_paths, filenames))
             )
         return False, None
 
-    def _target_path(self, object_name, cached=True, raise_missing=False):
-        """
-        find the path on the local filesystem to the file containing a named
-        data object. autopopulate the file_mapping
+    def _target_path(
+        self,
+        object_name: str,
+        cached: bool = True,
+        raise_missing: bool = False
+    ) -> Optional[Union[Path, list[Path], str]]:
+        """
+        Considering all known search paths and treating filenames as
+        case-insensitive, attempt to find a filesystem path to a
+        file or files in which a particular named data object might exist.
+        This autopopulates self.file_mapping[object_name] if it finds one or
+        more files, and by default treats this value as cached on subsequent
+        calls (which can improve performance significantly, especially on
+        networked filesystems).
         """
         if cached is True and (self.file_mapping.get(object_name) is not None):
             return self.file_mapping[object_name]
         try:
             if isinstance(object_name, set):
                 file_list = [self._target_path(obj) for obj in object_name]
                 self.file_mapping[object_name] = file_list
@@ -395,20 +418,26 @@
             self.file_mapping[object_name] = path
             return path
         except FileNotFoundError:
             if raise_missing is True:
                 raise
             return None
 
-    def unloaded(self):
-        """"""
+    def unloaded(self) -> tuple[str]:
+        """Return names of all identified but unloaded data objects."""
         return tuple(filter(lambda k: k not in dir(self), self.index))
 
     def load(self, name: str, reload: bool = False, **load_kwargs: Any):
-        """"""
+        """
+        Explicitly load an identified data object by name; alternatively
+        `name="all"` means "load every identified object". Does not return the
+        object; just assigns it to the `name` attribute of `self`. The
+        `Data.__getitem__()` interface lazy-loads by calling this function
+        with default arguments in response to `data['NOTYETLOADED']` etc.
+        """
         # prelude: don't try to load nonexistent keys; facilitate
         # load-everything behavior; don't reload by default
         if (name != "all") and (name not in self.index):
             raise KeyError(f"{name} not found in index: {self.index}.")
         if name == "all":
             return self.load_all()
         if (name in dir(self)) and (reload is False):
@@ -427,15 +456,17 @@
                 return self._file_not_found(name)
             self.file_mapping[name] = target
         try:
             obj = self.load_from_pointer(name, **load_kwargs)
             if obj is None:
                 return
             if not isinstance(obj, dict):
-                raise TypeError(f"loader returned non-dict object of type ({type(obj)}")
+                raise TypeError(
+                    f"loader returned non-dict object of type ({type(obj)}"
+                )
             self._add_loaded_objects(obj)
             return
         except DebugExceptionPreempted:
             pass
         except KeyboardInterrupt:
             raise
         except NotImplementedError as ex:
@@ -443,74 +474,78 @@
         except FileNotFoundError as _ex:
             warnings.warn(f"Unable to find files required by {name}.")
         except Exception as ex:
             warnings.warn(f"Unable to load {name}: {ex}")
         setattr(self, name, self.metaget_(name))
 
     def _add_loaded_objects(self, obj: Mapping[str, Any]):
-        """"""
+        """Helper for `load()`. Ingests objects returned by a `Loader`."""
         for k, v in obj.items():
             if v is not None:
                 setattr(self, k, v)
                 if k not in self.index:
                     self.index.append(k)
 
     def load_all(self):
-        """"""
+        """Handler (and alias) for `Data.load("all")`."""
         from pdr.loaders.dispatch import OBJECTS_IGNORED_BY_DEFAULT
 
         for name in self.keys():
             if OBJECTS_IGNORED_BY_DEFAULT.match(name):
                 continue
             try:
                 self.load(name)
             except AlreadyLoadedError:
                 continue
 
     def _file_not_found(self, object_name: str):
-        """"""
+        """Implements default file-not-found behavior."""
         warnings.warn(
             f"{object_name} file {self._object_to_filename(object_name)} "
             f"not found in path."
         )
         return_default = self.metaget_(object_name)
         maybe = catch_return_default(
             self.debug, return_default, FileNotFoundError()
         )
         setattr(self, object_name, maybe)
 
     def _load_primary_fits(
         self, object_name: str
-    ) -> Union["np.ndarray", "pd.DataFrame", None]:
-        """"""
+    ) -> Union[np.ndarray, pd.DataFrame, None]:
+        """Handle loading an HDU from a FITS file in "primary" FITS mode."""
         from pdr.loaders.handlers import handle_fits_file
 
         obj = handle_fits_file(
             self.filename,
             object_name,
             self._hdumap[object_name],
             self._hdulist
         )
         if obj.__class__.__name__ == "ndarray":
             self._scaleflags[object_name] = True
         return obj
 
     def _init_primary_format(self):
-        """"""
+        """
+        Initialization handler for "primary" format modes (cases in which
+        `Data` offers an interface to a file or files in a standard format).
+        Currently only supports FITS.
+        """
         if self.standard == "FITS":
             for k in self.metadata.keys():
                 self.index.append(k)
             return
         raise NotImplementedError
 
     def _load_pds4(self, object_name: str):
         """
-        load this object however pds4_tools wants to load this object, then
-        reformat to df or expose the array handle in accordance with our type
-        conventions.
+        Load this object however pds4_tools wants to load this object, then
+        reformat to DataFrame, expose the array handle in accordance with our
+        type conventions, et..
         """
         structure = self._pds4_structures[object_name]
         from pds4_tools.reader.label_objects import Label
 
         if isinstance(structure, Label):
             setattr(self, "label", structure)
         elif structure.is_array():
@@ -529,17 +564,21 @@
     def read_metadata(self, pvl_limit: int = DEFAULT_PVL_LIMIT) -> Metadata:
         """
         Attempt to ingest a product's metadata. if it is a PDS4 product,
         pds4_tools will already have ingested its detached XML label in
         Data._init_pds4(). In that case, simply preprocess it for
         Metadata.__init__.
         Otherwise, if it has a detached PDS3/PVL label, ingest it with
-        pdr.parselabel.pds3.read_pvl_label.
-        Finally, if we have found no detached label, look for an attached PVL
-        label (also using read_pvl_label).
+        pdr.parselabel.pds3.read_pvl.
+        Then, if we found no detached label, look for an attached PVL
+        label (also using read_pvl).
+        If we are in a "primary" mode, ignore all that and ingest the product's
+        metadata with the appropriate format-specific functions.
+        Then, construct a Metadata object from whatever we loaded and add all
+        the objects it implies to our index.
         """
         if self.standard == "FITS":
             from pdr.loaders.handlers import unpack_fits_headers
 
             mapping, params, self._hdumap = unpack_fits_headers(
                 self.filename, hdulist=self._hdulist
             )
@@ -554,29 +593,39 @@
         # we wait until after the read step to make these assignments in order
         # to facilitate debugging in cases where there is not in fact an
         # attached label or we couldn't read it
         self.labelname, self.file_mapping["LABEL"] = target, target
         self.index.append("LABEL")
         return metadata
 
-    def load_from_pointer(self, pointer: str, **load_kwargs: Any) -> Any:
-        """"""
+    def load_from_pointer(
+        self, pointer: str, **load_kwargs: Any
+    ) -> dict[
+        str, Union[pd.DataFrame, np.ndarray, str, MultiDict, "PVLModule"]
+    ]:
+        """
+        PDS3 data object-loading handler. Set up the appropriate `Loader` for
+        the object, set up load flow tracking, call the loader, and perform
+        basic cleanup.
+        """
         from pdr.loaders.dispatch import pointer_to_loader
 
         loader = pointer_to_loader(pointer, self)
         if self.debug is True:
             loader = Dynamic.from_function(loader, optional=True)
         self.loaders[pointer] = loader
         self.tracker.set_metadata(
             filename=self.file_mapping[pointer], obj=pointer
         )
         obj = self.loaders[pointer](
             self, pointer, tracker=self.tracker, **load_kwargs
         )
         # FITS arrays are scaled by default
+        # TODO: obj should never be an ndarray; it should always be a dict.
+        #  Fix this.
         if (
             (loader.__class__.__name__ == "ReadFits")
             and (obj.__class__.__name__ == "ndarray")
         ):
             self._scaleflags[pointer] = True
         if self.debug is True and len(loader.errors) > 0:
             warnings.warn(
@@ -585,16 +634,16 @@
             raise DebugExceptionPreempted
         return obj
 
     def get_scaled(
         self,
         object_name: str,
         inplace: bool = False,
-        float_dtype: Optional["np.dtype"] = None
-    ) -> "np.ndarray":
+        float_dtype: Optional[np.dtype] = None
+    ) -> np.ndarray:
         """
         fetches copy of data object corresponding to key, masks special
         constants, then applies any scale and offset specified in the label.
         only relevant to arrays.
 
         if `inplace` is True, does calculations in-place on original array,
         with attendant memory savings and destructiveness.
@@ -623,15 +672,15 @@
             )
         if self.specials[object_name] != {}:
             obj = mask_specials(obj, list(self.specials[object_name].values()))
         return scale_array(self, obj, object_name, inplace, float_dtype)
 
     def find_special_constants(
         self, object_name: str
-    ) -> dict[str, Union[float, int]]:
+    ) -> dict[str, Number]:
         """
         look up or infer special constants for one of our data objects.
         in general, only works well on ndarrays.
         """
         if len(consts := special_image_constants(self.identifiers)) > 0:
             return consts
         from pdr._scaling import find_special_constants
@@ -655,15 +704,15 @@
             this function's return values are memoized for performance.
             updating elements of self.metadata that have already been accessed
             with this function will not update future calls to this function.
         """
         return self.metadata.metaget(text, default, evaluate, warn)
 
     def metaget_(
-        self, text: str, default: bool = None, evaluate: bool = True
+        self, text: str, default: Any = None, evaluate: bool = True
     ) -> Any:
         """quiet-by-default version of metaget"""
         return self.metadata.metaget(text, default, evaluate, False)
 
     def metablock(
         self, text: str, evaluate: bool = True, warn: bool = True
     ) -> Optional[Mapping]:
@@ -682,30 +731,36 @@
     def metablock_(
         self, text: str, evaluate: bool = True
     ) -> Optional[Mapping]:
         """quiet-by-default version of metablock"""
         return self.metadata.metablock(text, evaluate, False)
 
     def get_absolute_paths(self, filename: Union[str, Path]) -> list[str]:
-        """"""
+        """
+        Construct `Path`s for a filename in all our search paths. (These are
+        places we can look for that file).
+        """
         return gmap(
             lambda sf: Path(*sf).absolute(),
             product(self.search_paths, listify(filename)),
             evaluator=list,
         )
 
     # TODO: reorganize this -- common dispatch funnel with dump_browse,
     #  split up the image-gen part of _browsify_array, something like that
     def show(
         self,
         object_name: str = None,
         scaled: bool = True,
         **browse_kwargs: Any
-    ) -> "PIL.Image.Image":
-        """"""
+    ) -> Image:
+        """
+        Produce an Image from a data object associated with this product. A
+        convenient way to quickly look at data.
+        """
         if object_name is None:
             raise ValueError(
                 f"please specify the name of an image object. "
                 f"keys include {self.index}"
             )
         if not self[object_name].__class__.__name__ == "ndarray":
             raise TypeError("Data.show only works on array data.")
@@ -742,15 +797,18 @@
         for obj in filter(lambda i: i in dir(self), self.index):
             outfile = str(Path(outpath, f"{prefix}_{obj}"))
             # no need to have all this mpl stuff in the namespace normally
             from pdr.browsify import browsify
 
             dump_it = partial(browsify, purge=purge, **browse_kwargs)
             fdt = browse_kwargs.get("float_dtype")
-            if self[obj].__class__.__name__ == "ndarray" and len(self[obj].shape) != 1:
+            if (
+                self[obj].__class__.__name__ == "ndarray"
+                and len(self[obj].shape) != 1
+            ):
                 if scaled == "both":
                     dump_it(
                         self.get_scaled(obj, float_dtype=fdt),
                         outfile + "_scaled",
                         purge=False,
                     )
                     dump_it(self[obj], outfile + "_unscaled")
@@ -796,15 +854,18 @@
         risking infinite loops inside lazy-load behaviors.
         """
         return super().__getattribute__(attr)
 
     # The following two functions make this object act sort of dict-like
     #  in useful ways for data exploration.
     def keys(self) -> list[str]:
-        """Returns the keys for observational data and metadata objects"""
+        """
+        Returns names of all data objects defined in the label (or inferred
+        while loading an object, like FITS headers).
+        """
         return self.index
 
     # make it possible to get data objects with slice notation, like a dict
     def __getitem__(self, item):
         """"""
         return self.__getattribute__(item)
 
@@ -828,15 +889,18 @@
         for key in self.keys():
             yield self[key]
 
 
 def _metaget_factory(
     metadata: Metadata, cached: bool = True
 ) -> Callable[[str, bool, bool], Any]:
-    """"""
+    """
+    Factory function for an internal component of `metaget()`. Reduces the risk
+    that the metadata access cache will create reference cycles.
+    """
     def metaget_interior(text, default, evaluate):
         """"""
         value = dig_for_value(metadata, text, mtypes=(dict, MultiDict))
         if value is not None:
             return metadata.formatter(value) if evaluate is True else value
         return default
 
@@ -844,15 +908,18 @@
         return cache(metaget_interior)
     return metaget_interior
 
 
 def _metablock_factory(
     metadata: Metadata, cached: bool = True
 ) -> Callable[[str, bool], Mapping]:
-    """"""
+    """
+    Factory function for an internal component of `metablock()`. Reduces the
+    risk that the metadata access cache will create reference cycles.
+    """
     def metablock_interior(text, evaluate):
         """"""
         value = dig_for_value(metadata, text, mtypes=(dict, MultiDict))
         if not isinstance(value, Mapping):
             value = metadata
         return metadata.formatter(value) if evaluate is True else value
```

### Comparing `pdr-1.0.6/pdr/pvl_utils.py` & `pdr-1.0.7/pdr/pvl_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/objects.py` & `pdr-1.0.7/pdr/tests/objects.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_bit_handling.py` & `pdr-1.0.7/pdr/tests/test_bit_handling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from inspect import get_annotations
 import random
 
 import pandas as pd
 
 from pdr.bit_handling import expand_bit_strings
 from pdr.loaders.queries import read_table_structure
-from pdr.parselabel.pds3 import parse_pvl, literalize_pvl_block
-from pdr.pdr import ID_FIELDS
+from pdr.parselabel.pds3 import literalize_pvl_block, parse_pvl
+from pdr.pdrtypes import DataIdentifiers
 
 BIT_STUB = """
 OBJECT                  = COLUMN
     NAME                = BITS1
     BYTES               = 2
     START_BYTE          = 1
     DATA_TYPE           = "MSB_BIT_STRING"
@@ -36,15 +37,15 @@
         BIT_DATA_TYPE   = "MSB_INTEGER"
         BITS            = 4
         START_BIT       = 13
     END_OBJECT          = BIT_COLUMN
 END_OBJECT              = COLUMN
 """
 
-NULL_IDENTIFIERS = {field: "" for field in ID_FIELDS}
+NULL_IDENTIFIERS = {field: "" for field in get_annotations(DataIdentifiers)}
 
 
 def test_bit_handling():
     block = literalize_pvl_block(parse_pvl(BIT_STUB)[0])
     fmtdef = read_table_structure(block, 'TABLE', None, None, NULL_IDENTIFIERS)
     bits = random.choices((0, 1), k=16)
     table = pd.DataFrame(
```

### Comparing `pdr-1.0.6/pdr/tests/test_browsify.py` & `pdr-1.0.7/pdr/tests/test_browsify.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_data.py` & `pdr-1.0.7/pdr/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_datatypes.py` & `pdr-1.0.7/pdr/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_func.py` & `pdr-1.0.7/pdr/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_loader_helpers.py` & `pdr-1.0.7/pdr/tests/test_loader_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         assert (
                 count_from_bottom_of_file(fn, rows, row_bytes) == rows * row_bytes
         )
     finally:
         Path(fn[0]).unlink(missing_ok=True)
 
 
-
 def test_check_delimiter_stream():
     byte_target = {"units": "BYTES", "value": 19200}
     rec_target = {"units": "RECORDS", "value": 1200}
     identifiers = {
         "SPACECRAFT_ID": "NOSTALGIA_FOR_INFINITY",
         'RECORD_BYTES': 100,
         "ETC": ...,
```

### Comparing `pdr-1.0.6/pdr/tests/test_np_utils.py` & `pdr-1.0.7/pdr/tests/test_np_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_parselabel_pds3.py` & `pdr-1.0.7/pdr/tests/test_parselabel_pds3.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_queries.py` & `pdr-1.0.7/pdr/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_scaling.py` & `pdr-1.0.7/pdr/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/test_table.py` & `pdr-1.0.7/pdr/tests/test_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     fpath, lpath = make_simple_dsv_table_product()
     data = pdr.read(fpath, debug=True)
     assert list(data.SPREADSHEET.columns) == ['X_0', 'Y', 'X_1']
     assert list(data.SPREADSHEET.dtypes) == [
         np.dtype('float64'), np.dtype('O'), np.dtype('int64')
     ]
     assert np.isclose(data.SPREADSHEET.loc[0, 'X_0'], 5.5)
-    assert data.SPREADSHEET.loc[5, 'Y'] == ' cat'
+    assert data.SPREADSHEET.loc[5, 'Y'] == 'cat'
     assert data.SPREADSHEET.loc[9, "X_1"] == -12
```

### Comparing `pdr-1.0.6/pdr/tests/test_vax.py` & `pdr-1.0.7/pdr/tests/test_vax.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/tests/utils.py` & `pdr-1.0.7/pdr/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/pdr/vax.py` & `pdr-1.0.7/pdr/vax.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 and copyright in addition to the terms of the BSD-3 Clause license, copyright
 Million Concepts, that apply to pdr as a whole, including our Contributions
 to this module.
 
 Million Concepts explicitly makes no claim to the SETI name or trademarks.
 
 ############################################################################
-# vax.py: Conversions between Vax single-precision floats IEEE floats
+# vax.py: Conversions between Vax single-precision floats and IEEE floats
 ############################################################################
 """
 
 import numpy as np
 
 
 def from_vax32(data):
```

### Comparing `pdr-1.0.6/pdr.egg-info/PKG-INFO` & `pdr-1.0.7/pdr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.6
+Version: 1.0.7
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -35,24 +35,30 @@
 
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
-(under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](docs/supported_datasets.md) 
+(under PDS3 or PDS4) should be covered eventually. 
+[Currently-supported datasets are listed here.](docs/supported_datasets.md) 
 
-If the software fails while attempting to read from datasets that we have listed as supported, please submit an issue with a link to the file and information about the error (if applicable). There might also be datasets that work but are not listed. We would like to hear about those too. If a dataset is not yet supported that you would like us to consider prioritizing, [please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
+If the software fails while attempting to read from datasets that we have 
+listed as supported, please submit an issue with a link to the file and 
+information about the error (if applicable). There might also be datasets that 
+work but are not listed. We would like to hear about those too. If a dataset 
+is not yet supported that you would like us to consider prioritizing, 
+[please fill out this request form](https://docs.google.com/forms/d/1JHyMDzC9LlXY4MOMcHqV5fbseSB096_PsLshAMqMWBw/viewform).
 
 ### Attribution
 If you use _pdr_ in your work, please cite us using our Zenodo DOI: [![DOI](https://zenodo.org/badge/266449940.svg)](https://zenodo.org/badge/latestdoi/266449940)
 
 ### Installation
-_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) installation into a `conda` environment.
-You can do this like so: 
+_pdr_ is now on `conda` and `pip`. We recommend (and only officially support) 
+installation into a `conda` environment. You can do this like so: 
 
 ```
 conda create --name pdrenv
 conda activate pdrenv
 conda install -c conda-forge pdr
 ```
 The minimum supported version of Python is _3.9_.
@@ -60,24 +66,28 @@
 Using the conda install will install all dependencies in the environment.yml 
 file (both required and optional) for pdr. If you'd prefer to forego the 
 optional dependencies, please use minimal_environment.yml in your 
 installation. This is not supported through a direct conda install as 
 described above and will reqiore additional steps. Optional dependencies 
 and the added functionality they support are listed below:
 
-  - `pvl`: allows `Data.load("LABEL", as_pvl=True)` which will load PDS3 labels as `pvl` objects rather than plain text
+  - `pvl`: allows `Data.load("LABEL", as_pvl=True)`, which will load PDS3 
+     labels as `pvl` objects rather than plain text
   - `astropy`: adds support for FITS files
-  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter notebooks you create)
+  - `jupyter`: allows usage of the Example Jupyter Notebook (and other jupyter 
+     notebooks you create)
   - `pillow`: adds support for TIFF files and browse image rendering
-  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse function
+  - `matplotlib`: allows usage of `save_sparklines`, an experimental browse 
+    function
 
 ### Usage
 
 You can check out our example Notebook on Binder for a 
 quick interactive demo of functionality: 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/millionconcepts/pdr/main)
 
-Additional information on usage including examples, output data types, notes and caveats, test, etc. 
-can now be accessed in our documentation on readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
+Additional information on usage including examples, output data types, notes 
+and caveats, tests, etc. can now be accessed in our documentation on 
+readthedocs at: https://pdr.readthedocs.io [![Documentation Status](https://readthedocs.org/projects/pdr/badge/?version=latest)](https://pdr.readthedocs.io/en/latest/?badge=latest)
 
 ---
 This work is supported by NASA grant No. 80NSSC21K0885.
```

### Comparing `pdr-1.0.6/pdr.egg-info/SOURCES.txt` & `pdr-1.0.7/pdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdr-1.0.6/setup.py` & `pdr-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdr",
-    version="1.0.6",
+    version="1.0.7",
     author="Chase Million",
     author_email="chase@millionconcepts.com",
     description="Planetary Data Reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MillionConcepts/pdr",
     packages=setuptools.find_packages(),
```

