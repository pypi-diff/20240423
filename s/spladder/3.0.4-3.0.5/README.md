# Comparing `tmp/spladder-3.0.4.tar.gz` & `tmp/spladder-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spladder-3.0.4.tar", last modified: Tue Feb  7 14:31:46 2023, max compression
+gzip compressed data, was "spladder-3.0.5.tar", last modified: Tue Apr 23 14:12:15 2024, max compression
```

## Comparing `spladder-3.0.4.tar` & `spladder-3.0.5.tar`

### file list

```diff
@@ -1,679 +1,679 @@
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.960944 spladder-3.0.4/
--rw-r--r--   0 akahles    (501) staff       (20)      203 2021-03-18 11:06:19.000000 spladder-3.0.4/MANIFEST.in
--rw-r--r--   0 akahles    (501) staff       (20)     3490 2023-02-07 14:31:45.961167 spladder-3.0.4/PKG-INFO
--rw-r--r--   0 akahles    (501) staff       (20)     2355 2021-03-18 11:06:19.000000 spladder-3.0.4/README.md
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.195160 spladder-3.0.4/docs/
--rw-r--r--   0 akahles    (501) staff       (20)      609 2021-03-18 11:06:19.000000 spladder-3.0.4/docs/Makefile
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.200125 spladder-3.0.4/docs/source/
--rw-r--r--   0 akahles    (501) staff       (20)     4831 2022-07-13 10:41:27.000000 spladder-3.0.4/docs/source/conf.py
--rw-r--r--   0 akahles    (501) staff       (20)    18383 2022-01-19 20:41:37.000000 spladder-3.0.4/docs/source/file_formats.rst
--rw-r--r--   0 akahles    (501) staff       (20)     4493 2021-03-18 11:06:19.000000 spladder-3.0.4/docs/source/general.rst
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.200841 spladder-3.0.4/docs/source/img/
--rw-r--r--   0 akahles    (501) staff       (20)    65001 2022-01-19 20:41:37.000000 spladder-3.0.4/docs/source/img/splice_events.png
--rw-r--r--   0 akahles    (501) staff       (20)     1121 2021-03-18 11:06:19.000000 spladder-3.0.4/docs/source/index.rst
--rw-r--r--   0 akahles    (501) staff       (20)     1128 2021-03-18 11:06:19.000000 spladder-3.0.4/docs/source/installation.rst
--rw-r--r--   0 akahles    (501) staff       (20)     6722 2021-03-18 11:06:19.000000 spladder-3.0.4/docs/source/spladder_cohort.rst
--rw-r--r--   0 akahles    (501) staff       (20)    38746 2022-01-19 20:41:37.000000 spladder-3.0.4/docs/source/spladder_modes.rst
--rw-r--r--   0 akahles    (501) staff       (20)      118 2022-01-19 20:41:37.000000 spladder-3.0.4/requirements.txt
--rw-r--r--   0 akahles    (501) staff       (20)      467 2023-02-07 14:31:45.962124 spladder-3.0.4/setup.cfg
--rw-r--r--   0 akahles    (501) staff       (20)     1383 2023-02-07 14:24:59.000000 spladder-3.0.4/setup.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.211644 spladder-3.0.4/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)      157 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/__init__.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.217808 spladder-3.0.4/spladder/alt_splice/
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/alt_splice/__init__.py
--rw-r--r--   0 akahles    (501) staff       (20)    11648 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/alt_splice/analyze.py
--rw-r--r--   0 akahles    (501) staff       (20)    17935 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/alt_splice/collect.py
--rw-r--r--   0 akahles    (501) staff       (20)    25692 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/alt_splice/detect.py
--rw-r--r--   0 akahles    (501) staff       (20)     6590 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/alt_splice/events.py
--rw-r--r--   0 akahles    (501) staff       (20)    24972 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/alt_splice/quantify.py
--rw-r--r--   0 akahles    (501) staff       (20)    31412 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/alt_splice/verify.py
--rw-r--r--   0 akahles    (501) staff       (20)    31846 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/alt_splice/write.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.221010 spladder-3.0.4/spladder/classes/
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/classes/__init__.py
--rw-r--r--   0 akahles    (501) staff       (20)      241 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/classes/counts.py
--rw-r--r--   0 akahles    (501) staff       (20)     1830 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/classes/datatrack.py
--rw-r--r--   0 akahles    (501) staff       (20)     3250 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/classes/event.py
--rw-r--r--   0 akahles    (501) staff       (20)     9723 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/classes/gene.py
--rw-r--r--   0 akahles    (501) staff       (20)      193 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/classes/region.py
--rw-r--r--   0 akahles    (501) staff       (20)     2288 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/classes/segmentgraph.py
--rw-r--r--   0 akahles    (501) staff       (20)    12025 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/classes/splicegraph.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.222024 spladder-3.0.4/spladder/core/
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/core/__init__.py
--rw-r--r--   0 akahles    (501) staff       (20)     9015 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/core/gen_graphs.py
--rw-r--r--   0 akahles    (501) staff       (20)      742 2022-01-19 20:41:37.000000 spladder-3.0.4/spladder/core/spladdercore.py
--rw-r--r--   0 akahles    (501) staff       (20)    15883 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/count.py
--rw-r--r--   0 akahles    (501) staff       (20)    93618 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/editgraph.py
--rw-r--r--   0 akahles    (501) staff       (20)     1377 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/hdf5.py
--rw-r--r--   0 akahles    (501) staff       (20)     9517 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/helpers.py
--rw-r--r--   0 akahles    (501) staff       (20)     7484 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/helpers_viz.py
--rw-r--r--   0 akahles    (501) staff       (20)    18694 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/init.py
--rw-r--r--   0 akahles    (501) staff       (20)    11477 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/merge.py
--rw-r--r--   0 akahles    (501) staff       (20)    29413 2023-02-07 14:24:59.000000 spladder-3.0.4/spladder/reads.py
--rw-r--r--   0 akahles    (501) staff       (20)    11430 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/settings.py
--rw-r--r--   0 akahles    (501) staff       (20)    23203 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/spladder.py
--rw-r--r--   0 akahles    (501) staff       (20)     7066 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/spladder_build.py
--rw-r--r--   0 akahles    (501) staff       (20)     6163 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/spladder_prep.py
--rw-r--r--   0 akahles    (501) staff       (20)    33391 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/spladder_test.py
--rw-r--r--   0 akahles    (501) staff       (20)    18637 2022-07-13 10:41:27.000000 spladder-3.0.4/spladder/spladder_viz.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.222570 spladder-3.0.4/spladder/testing/
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/testing/__init__.py
--rw-r--r--   0 akahles    (501) staff       (20)     1866 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/testing/likelihood.py
--rw-r--r--   0 akahles    (501) staff       (20)     4051 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/utils.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.225895 spladder-3.0.4/spladder/viz/
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/__init__.py
--rw-r--r--   0 akahles    (501) staff       (20)     2544 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/axes.py
--rw-r--r--   0 akahles    (501) staff       (20)    16516 2022-01-19 20:41:38.000000 spladder-3.0.4/spladder/viz/coverage.py
--rw-r--r--   0 akahles    (501) staff       (20)     6746 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/diagnose.py
--rw-r--r--   0 akahles    (501) staff       (20)     2466 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/genelets.py
--rw-r--r--   0 akahles    (501) staff       (20)     3691 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/graph.py
--rw-r--r--   0 akahles    (501) staff       (20)     1049 2021-03-18 11:06:19.000000 spladder-3.0.4/spladder/viz/highlight.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.213721 spladder-3.0.4/spladder.egg-info/
--rw-r--r--   0 akahles    (501) staff       (20)     3490 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/PKG-INFO
--rw-r--r--   0 akahles    (501) staff       (20)    44017 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/SOURCES.txt
--rw-r--r--   0 akahles    (501) staff       (20)        1 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/dependency_links.txt
--rw-r--r--   0 akahles    (501) staff       (20)       53 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/entry_points.txt
--rw-r--r--   0 akahles    (501) staff       (20)        1 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/not-zip-safe
--rw-r--r--   0 akahles    (501) staff       (20)      118 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/requires.txt
--rw-r--r--   0 akahles    (501) staff       (20)       15 2023-02-07 14:31:44.000000 spladder-3.0.4/spladder.egg-info/top_level.txt
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.226824 spladder-3.0.4/tests/
--rw-r--r--   0 akahles    (501) staff       (20)       58 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/__init__.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.227339 spladder-3.0.4/tests/templates/
--rw-r--r--   0 akahles    (501) staff       (20)     9689 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/templates/annotation_pos.gtf
--rw-r--r--   0 akahles    (501) staff       (20)    13120 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/test_end_to_end.py
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.186692 spladder-3.0.4/tests/testcase_basic/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.244938 spladder-3.0.4/tests/testcase_basic/data/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.265159 spladder-3.0.4/tests/testcase_basic/data/align/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.265606 spladder-3.0.4/tests/testcase_basic/data/align/neg_1/
--rw-r--r--   0 akahles    (501) staff       (20)    33923 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_1/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33923 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_1.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_1.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    13888 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_1.conf_3.filt.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)    13888 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_1.hdf5
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.266178 spladder-3.0.4/tests/testcase_basic/data/align/neg_2/
--rw-r--r--   0 akahles    (501) staff       (20)    33997 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_2/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33997 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_2.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_2.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.266538 spladder-3.0.4/tests/testcase_basic/data/align/neg_3/
--rw-r--r--   0 akahles    (501) staff       (20)    34063 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_3/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    34063 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_3.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_3.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.266863 spladder-3.0.4/tests/testcase_basic/data/align/neg_4/
--rw-r--r--   0 akahles    (501) staff       (20)    33932 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_4/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33932 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_4.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_4.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.267233 spladder-3.0.4/tests/testcase_basic/data/align/neg_5/
--rw-r--r--   0 akahles    (501) staff       (20)    33978 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_5/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33978 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_5.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/neg_5.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.267794 spladder-3.0.4/tests/testcase_basic/data/align/pos_1/
--rw-r--r--   0 akahles    (501) staff       (20)    33867 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_1/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33867 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_1.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_1.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    13888 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_1.conf_3.filt.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)    13888 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_1.hdf5
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.268177 spladder-3.0.4/tests/testcase_basic/data/align/pos_2/
--rw-r--r--   0 akahles    (501) staff       (20)    33821 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_2/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33821 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_2.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_2.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.268560 spladder-3.0.4/tests/testcase_basic/data/align/pos_3/
--rw-r--r--   0 akahles    (501) staff       (20)    33798 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_3/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33798 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_3.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_3.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.268958 spladder-3.0.4/tests/testcase_basic/data/align/pos_4/
--rw-r--r--   0 akahles    (501) staff       (20)    33679 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_4/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33679 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_4.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_4.bam.bai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.269318 spladder-3.0.4/tests/testcase_basic/data/align/pos_5/
--rw-r--r--   0 akahles    (501) staff       (20)    33736 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_5/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    33736 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_5.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/align/pos_5.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)     9734 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/annotation_neg.gtf
--rw-r--r--   0 akahles    (501) staff       (20)     2232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/data/annotation_neg.gtf.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     9689 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/annotation_pos.gtf
--rw-r--r--   0 akahles    (501) staff       (20)     2232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/data/annotation_pos.gtf.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      997 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/expr_ts.txt
--rw-r--r--   0 akahles    (501) staff       (20)      156 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/genome_neg.fa
--rw-r--r--   0 akahles    (501) staff       (20)      156 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/genome_pos.fa
--rw-r--r--   0 akahles    (501) staff       (20)   354449 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/testcase_basic_1.fq
--rw-r--r--   0 akahles    (501) staff       (20)   354449 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/testcase_basic_2.fq
--rw-r--r--   0 akahles    (501) staff       (20)   354449 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/testcase_basic_3.fq
--rw-r--r--   0 akahles    (501) staff       (20)   354449 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/testcase_basic_4.fq
--rw-r--r--   0 akahles    (501) staff       (20)   354449 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/data/testcase_basic_5.fq
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.290840 spladder-3.0.4/tests/testcase_basic/results_merged_neg/
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)       70 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)       70 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      218 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      261 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      163 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      353 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      251 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      343 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      198 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      198 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      296 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      380 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      220 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      370 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      516 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.297845 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3417 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_1.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_2.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_4.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_5.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.336328 spladder-3.0.4/tests/testcase_basic/results_merged_pos/
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)       62 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)       62 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      214 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      256 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      157 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      355 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      246 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      345 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      196 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      196 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      294 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      378 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      218 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      532 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      368 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      522 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.344968 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3417 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_1.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_2.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_4.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_5.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.366490 spladder-3.0.4/tests/testcase_basic/results_single_neg/
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      188 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      229 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      228 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      323 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.375981 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     2991 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.418111 spladder-3.0.4/tests/testcase_basic/results_single_pos/
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      185 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      227 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      227 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      322 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.424796 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     2991 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.426241 spladder-3.0.4/tests/testcase_events/
--rw-r--r--   0 akahles    (501) staff       (20)       16 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/.gitignore
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.624564 spladder-3.0.4/tests/testcase_events/data/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.715151 spladder-3.0.4/tests/testcase_events/data/align/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.715967 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1/
--rw-r--r--   0 akahles    (501) staff       (20)   104409 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   104409 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    19406 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.717098 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10/
--rw-r--r--   0 akahles    (501) staff       (20)    87640 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    87640 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    16115 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.717764 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11/
--rw-r--r--   0 akahles    (501) staff       (20)   136749 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   136749 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    29045 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.cram
--rw-r--r--   0 akahles    (501) staff       (20)       63 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.718356 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12/
--rw-r--r--   0 akahles    (501) staff       (20)   134059 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   134059 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    26983 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.719098 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13/
--rw-r--r--   0 akahles    (501) staff       (20)    38654 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    38654 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)     6343 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.cram
--rw-r--r--   0 akahles    (501) staff       (20)       45 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.719678 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14/
--rw-r--r--   0 akahles    (501) staff       (20)   130524 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   130524 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    25683 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.720418 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15/
--rw-r--r--   0 akahles    (501) staff       (20)    37976 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    37976 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)     6284 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.cram
--rw-r--r--   0 akahles    (501) staff       (20)       44 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.720950 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16/
--rw-r--r--   0 akahles    (501) staff       (20)    99434 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    99434 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    18513 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.721450 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17/
--rw-r--r--   0 akahles    (501) staff       (20)    57994 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    57994 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)     9914 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.cram
--rw-r--r--   0 akahles    (501) staff       (20)       45 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.722062 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18/
--rw-r--r--   0 akahles    (501) staff       (20)   167608 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   167608 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    38365 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.cram
--rw-r--r--   0 akahles    (501) staff       (20)       61 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.722875 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19/
--rw-r--r--   0 akahles    (501) staff       (20)   126962 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   126962 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    25052 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.723495 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2/
--rw-r--r--   0 akahles    (501) staff       (20)   152989 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   152989 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    33725 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.cram
--rw-r--r--   0 akahles    (501) staff       (20)       62 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.725250 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20/
--rw-r--r--   0 akahles    (501) staff       (20)    64726 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    64726 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    11132 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.726215 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3/
--rw-r--r--   0 akahles    (501) staff       (20)   186567 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   186567 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    44739 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.cram
--rw-r--r--   0 akahles    (501) staff       (20)       64 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.726924 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4/
--rw-r--r--   0 akahles    (501) staff       (20)   157108 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   157108 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    34778 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.cram
--rw-r--r--   0 akahles    (501) staff       (20)       63 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.727382 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5/
--rw-r--r--   0 akahles    (501) staff       (20)   187828 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   187828 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    44989 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.cram
--rw-r--r--   0 akahles    (501) staff       (20)       63 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.728404 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6/
--rw-r--r--   0 akahles    (501) staff       (20)   161242 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   161242 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    36501 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.cram
--rw-r--r--   0 akahles    (501) staff       (20)       62 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.729333 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7/
--rw-r--r--   0 akahles    (501) staff       (20)   101824 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   101824 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    18818 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.cram
--rw-r--r--   0 akahles    (501) staff       (20)       46 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.729820 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8/
--rw-r--r--   0 akahles    (501) staff       (20)   157121 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)   157121 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    35296 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.cram
--rw-r--r--   0 akahles    (501) staff       (20)       62 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.cram.crai
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.730273 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9/
--rw-r--r--   0 akahles    (501) staff       (20)    61333 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9/Aligned.sortedByCoord.out.bam
--rw-r--r--   0 akahles    (501) staff       (20)    61333 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.bam
--rw-r--r--   0 akahles    (501) staff       (20)       96 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.bam.bai
--rw-r--r--   0 akahles    (501) staff       (20)    10483 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.cram
--rw-r--r--   0 akahles    (501) staff       (20)       45 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.cram.crai
--rw-r--r--   0 akahles    (501) staff       (20)    10128 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/genome.fa
--rw-r--r--   0 akahles    (501) staff       (20)       16 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/genome.fa.fai
--rw-r--r--   0 akahles    (501) staff       (20)    17651 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events.gtf
--rw-r--r--   0 akahles    (501) staff       (20)   881921 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample1.fq
--rw-r--r--   0 akahles    (501) staff       (20)   708663 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample10.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1347762 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample11.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1282725 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample12.fq
--rw-r--r--   0 akahles    (501) staff       (20)   222750 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample13.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1228463 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample14.fq
--rw-r--r--   0 akahles    (501) staff       (20)   216112 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample15.fq
--rw-r--r--   0 akahles    (501) staff       (20)   836951 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample16.fq
--rw-r--r--   0 akahles    (501) staff       (20)   399396 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample17.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1801167 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample18.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1180269 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample19.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1582743 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample2.fq
--rw-r--r--   0 akahles    (501) staff       (20)   461865 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample20.fq
--rw-r--r--   0 akahles    (501) staff       (20)  2139805 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample3.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1627618 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample4.fq
--rw-r--r--   0 akahles    (501) staff       (20)  2142568 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample5.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1712710 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample6.fq
--rw-r--r--   0 akahles    (501) staff       (20)   856293 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample7.fq
--rw-r--r--   0 akahles    (501) staff       (20)  1657408 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample8.fq
--rw-r--r--   0 akahles    (501) staff       (20)   424277 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample9.fq
--rw-r--r--   0 akahles    (501) staff       (20)     9964 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/data/testcase_events_spladder.gtf
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.810626 spladder-3.0.4/tests/testcase_events/results_merged/
--rw-r--r--   0 akahles    (501) staff       (20)      391 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      235 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1669 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      524 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      689 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      307 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1334 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    26976 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1617 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      791 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1705 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      545 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      388 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      705 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      966 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      371 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1863 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    29539 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3881 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     2113 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1106 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     2243 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      782 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      466 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     3566 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      807 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      174 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1071 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      414 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     2311 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    30490 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     5942 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     3018 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1332 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     3085 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      472 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      237 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1747 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      532 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      679 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      353 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1159 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    29024 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3481 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1811 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      920 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1686 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      348 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      400 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      226 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1050 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    26976 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      659 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      390 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1040 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.txt.gz
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.856143 spladder-3.0.4/tests/testcase_events/results_merged/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)    37736 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      528 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      656 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    23016 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)    25153 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    16577 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    17256 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18100 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18097 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18229 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    17868 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.862871 spladder-3.0.4/tests/testcase_events/results_merged/testing/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.878114 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/
--rw-r--r--   0 akahles    (501) staff       (20)    18890 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    17086 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18811 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_adjusted_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18193 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_fitted_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18456 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_raw_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13740 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/ma_plot_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    14081 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13478 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13651 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    12509 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)     1595 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.gene_unique.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     1595 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     7756 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_extended_C3_exon_skip.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     6776 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged/testing/test_setup_C3_exon_skip.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.922917 spladder-3.0.4/tests/testcase_events/results_merged_cram/
--rw-r--r--   0 akahles    (501) staff       (20)      391 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      235 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1669 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      524 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      689 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      307 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1334 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    26976 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1617 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      791 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1705 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      545 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      388 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      705 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      966 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      371 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1863 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    29539 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3881 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     2113 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1106 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     2243 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      782 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      466 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     3566 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      807 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      174 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1071 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      414 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     2311 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    30490 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     5942 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     3018 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     1332 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     3085 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      472 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)      237 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)     1747 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      532 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      679 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      353 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1159 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    29024 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)     3481 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)     1811 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      920 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1686 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.bed
--rw-r--r--   0 akahles    (501) staff       (20)        0 2021-03-18 11:06:19.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.bed
--rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      348 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.icgc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      400 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)      226 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.tcga.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1050 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)    26976 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.counts.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.gff3
--rw-r--r--   0 akahles    (501) staff       (20)      659 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)      390 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.struc.txt.gz
--rw-r--r--   0 akahles    (501) staff       (20)     1040 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.txt.gz
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.948985 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/
--rw-r--r--   0 akahles    (501) staff       (20)    37736 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
--rw-r--r--   0 akahles    (501) staff       (20)      528 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
--rw-r--r--   0 akahles    (501) staff       (20)      656 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
--rw-r--r--   0 akahles    (501) staff       (20)    23016 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
--rw-r--r--   0 akahles    (501) staff       (20)    25153 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    16577 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    17256 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18100 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18097 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18229 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle
--rw-r--r--   0 akahles    (501) staff       (20)    17868 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.952201 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/
-drwxr-xr-x   0 akahles    (501) staff       (20)        0 2023-02-07 14:31:45.960378 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/
--rw-r--r--   0 akahles    (501) staff       (20)    18890 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    17086 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18810 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_adjusted_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18193 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_fitted_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    18453 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_raw_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13740 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/ma_plot_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    14080 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13479 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    13652 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.log10.pdf
--rw-r--r--   0 akahles    (501) staff       (20)    12510 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.pdf
--rw-r--r--   0 akahles    (501) staff       (20)     1595 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.gene_unique.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     1595 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     7744 2022-07-13 10:41:27.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_extended_C3_exon_skip.tsv
--rw-r--r--   0 akahles    (501) staff       (20)     6776 2022-01-19 20:41:38.000000 spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_setup_C3_exon_skip.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.764455 spladder-3.0.5/
+-rw-r--r--   0 akahles    (501) staff       (20)      203 2019-08-21 12:47:50.000000 spladder-3.0.5/MANIFEST.in
+-rw-r--r--   0 akahles    (501) staff       (20)     3490 2024-04-23 14:12:15.764655 spladder-3.0.5/PKG-INFO
+-rw-r--r--   0 akahles    (501) staff       (20)     2355 2019-08-21 12:47:50.000000 spladder-3.0.5/README.md
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.139330 spladder-3.0.5/docs/
+-rw-r--r--   0 akahles    (501) staff       (20)      609 2019-08-21 12:47:50.000000 spladder-3.0.5/docs/Makefile
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.145121 spladder-3.0.5/docs/source/
+-rw-r--r--   0 akahles    (501) staff       (20)     4831 2022-01-28 11:58:24.000000 spladder-3.0.5/docs/source/conf.py
+-rw-r--r--   0 akahles    (501) staff       (20)    18383 2022-01-07 18:44:19.000000 spladder-3.0.5/docs/source/file_formats.rst
+-rw-r--r--   0 akahles    (501) staff       (20)     4493 2019-09-16 12:28:52.000000 spladder-3.0.5/docs/source/general.rst
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.146559 spladder-3.0.5/docs/source/img/
+-rw-r--r--   0 akahles    (501) staff       (20)    65001 2022-01-07 18:44:19.000000 spladder-3.0.5/docs/source/img/splice_events.png
+-rw-r--r--   0 akahles    (501) staff       (20)     1121 2019-08-21 12:47:50.000000 spladder-3.0.5/docs/source/index.rst
+-rw-r--r--   0 akahles    (501) staff       (20)     1128 2019-08-21 12:47:50.000000 spladder-3.0.5/docs/source/installation.rst
+-rw-r--r--   0 akahles    (501) staff       (20)     9166 2024-04-23 14:03:12.000000 spladder-3.0.5/docs/source/spladder_cohort.rst
+-rw-r--r--   0 akahles    (501) staff       (20)    38746 2022-01-07 18:44:19.000000 spladder-3.0.5/docs/source/spladder_modes.rst
+-rw-r--r--   0 akahles    (501) staff       (20)      118 2024-04-23 14:03:12.000000 spladder-3.0.5/requirements.txt
+-rw-r--r--   0 akahles    (501) staff       (20)      467 2024-04-23 14:12:15.765579 spladder-3.0.5/setup.cfg
+-rw-r--r--   0 akahles    (501) staff       (20)     1383 2024-04-23 14:03:12.000000 spladder-3.0.5/setup.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.163674 spladder-3.0.5/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)      157 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/__init__.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.177322 spladder-3.0.5/spladder/alt_splice/
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/alt_splice/__init__.py
+-rw-r--r--   0 akahles    (501) staff       (20)    11648 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/alt_splice/analyze.py
+-rw-r--r--   0 akahles    (501) staff       (20)    17935 2022-01-28 11:58:24.000000 spladder-3.0.5/spladder/alt_splice/collect.py
+-rw-r--r--   0 akahles    (501) staff       (20)    25692 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/alt_splice/detect.py
+-rw-r--r--   0 akahles    (501) staff       (20)     6590 2022-01-28 11:58:24.000000 spladder-3.0.5/spladder/alt_splice/events.py
+-rw-r--r--   0 akahles    (501) staff       (20)    24972 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/alt_splice/quantify.py
+-rw-r--r--   0 akahles    (501) staff       (20)    31396 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/alt_splice/verify.py
+-rw-r--r--   0 akahles    (501) staff       (20)    31924 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/alt_splice/write.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.183879 spladder-3.0.5/spladder/classes/
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/classes/__init__.py
+-rw-r--r--   0 akahles    (501) staff       (20)      241 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/classes/counts.py
+-rw-r--r--   0 akahles    (501) staff       (20)     1830 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/classes/datatrack.py
+-rw-r--r--   0 akahles    (501) staff       (20)     3250 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/classes/event.py
+-rw-r--r--   0 akahles    (501) staff       (20)     9723 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/classes/gene.py
+-rw-r--r--   0 akahles    (501) staff       (20)      193 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/classes/region.py
+-rw-r--r--   0 akahles    (501) staff       (20)     2288 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/classes/segmentgraph.py
+-rw-r--r--   0 akahles    (501) staff       (20)    12025 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/classes/splicegraph.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.186260 spladder-3.0.5/spladder/core/
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/core/__init__.py
+-rw-r--r--   0 akahles    (501) staff       (20)     9015 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/core/gen_graphs.py
+-rw-r--r--   0 akahles    (501) staff       (20)      742 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/core/spladdercore.py
+-rw-r--r--   0 akahles    (501) staff       (20)    15883 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/count.py
+-rw-r--r--   0 akahles    (501) staff       (20)    93618 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/editgraph.py
+-rw-r--r--   0 akahles    (501) staff       (20)     1377 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/hdf5.py
+-rw-r--r--   0 akahles    (501) staff       (20)     9517 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/helpers.py
+-rw-r--r--   0 akahles    (501) staff       (20)     7484 2022-01-28 11:58:24.000000 spladder-3.0.5/spladder/helpers_viz.py
+-rw-r--r--   0 akahles    (501) staff       (20)    18694 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/init.py
+-rw-r--r--   0 akahles    (501) staff       (20)    11477 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/merge.py
+-rw-r--r--   0 akahles    (501) staff       (20)    29413 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/reads.py
+-rw-r--r--   0 akahles    (501) staff       (20)    11430 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/settings.py
+-rw-r--r--   0 akahles    (501) staff       (20)    23213 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/spladder.py
+-rw-r--r--   0 akahles    (501) staff       (20)     7066 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/spladder_build.py
+-rw-r--r--   0 akahles    (501) staff       (20)     6163 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/spladder_prep.py
+-rw-r--r--   0 akahles    (501) staff       (20)    33391 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/spladder_test.py
+-rw-r--r--   0 akahles    (501) staff       (20)    18652 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/spladder_viz.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.187363 spladder-3.0.5/spladder/testing/
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/testing/__init__.py
+-rw-r--r--   0 akahles    (501) staff       (20)     1866 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/testing/likelihood.py
+-rw-r--r--   0 akahles    (501) staff       (20)     4051 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/utils.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.192957 spladder-3.0.5/spladder/viz/
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/viz/__init__.py
+-rw-r--r--   0 akahles    (501) staff       (20)     2544 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/viz/axes.py
+-rw-r--r--   0 akahles    (501) staff       (20)    16528 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/viz/coverage.py
+-rw-r--r--   0 akahles    (501) staff       (20)     6746 2022-01-07 18:44:19.000000 spladder-3.0.5/spladder/viz/diagnose.py
+-rw-r--r--   0 akahles    (501) staff       (20)     2472 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/viz/genelets.py
+-rw-r--r--   0 akahles    (501) staff       (20)     3697 2024-04-23 14:03:12.000000 spladder-3.0.5/spladder/viz/graph.py
+-rw-r--r--   0 akahles    (501) staff       (20)     1049 2019-08-21 12:47:50.000000 spladder-3.0.5/spladder/viz/highlight.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.169843 spladder-3.0.5/spladder.egg-info/
+-rw-r--r--   0 akahles    (501) staff       (20)     3490 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/PKG-INFO
+-rw-r--r--   0 akahles    (501) staff       (20)    44017 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/SOURCES.txt
+-rw-r--r--   0 akahles    (501) staff       (20)        1 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/dependency_links.txt
+-rw-r--r--   0 akahles    (501) staff       (20)       53 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/entry_points.txt
+-rw-r--r--   0 akahles    (501) staff       (20)        1 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/not-zip-safe
+-rw-r--r--   0 akahles    (501) staff       (20)      118 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/requires.txt
+-rw-r--r--   0 akahles    (501) staff       (20)       15 2024-04-23 14:12:14.000000 spladder-3.0.5/spladder.egg-info/top_level.txt
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.194600 spladder-3.0.5/tests/
+-rw-r--r--   0 akahles    (501) staff       (20)       58 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/__init__.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.195533 spladder-3.0.5/tests/templates/
+-rw-r--r--   0 akahles    (501) staff       (20)     9689 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/templates/annotation_pos.gtf
+-rw-r--r--   0 akahles    (501) staff       (20)    13120 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/test_end_to_end.py
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.128974 spladder-3.0.5/tests/testcase_basic/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.219548 spladder-3.0.5/tests/testcase_basic/data/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.239968 spladder-3.0.5/tests/testcase_basic/data/align/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.240422 spladder-3.0.5/tests/testcase_basic/data/align/neg_1/
+-rw-r--r--   0 akahles    (501) staff       (20)    33923 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_1/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33923 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_1.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_1.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    13888 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_1.conf_3.filt.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)    13888 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_1.hdf5
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.240827 spladder-3.0.5/tests/testcase_basic/data/align/neg_2/
+-rw-r--r--   0 akahles    (501) staff       (20)    33997 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_2/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33997 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_2.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_2.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.241210 spladder-3.0.5/tests/testcase_basic/data/align/neg_3/
+-rw-r--r--   0 akahles    (501) staff       (20)    34063 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_3/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    34063 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_3.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_3.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.241594 spladder-3.0.5/tests/testcase_basic/data/align/neg_4/
+-rw-r--r--   0 akahles    (501) staff       (20)    33932 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_4/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33932 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_4.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_4.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.242094 spladder-3.0.5/tests/testcase_basic/data/align/neg_5/
+-rw-r--r--   0 akahles    (501) staff       (20)    33978 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_5/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33978 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_5.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/neg_5.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.242458 spladder-3.0.5/tests/testcase_basic/data/align/pos_1/
+-rw-r--r--   0 akahles    (501) staff       (20)    33867 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_1/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33867 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_1.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_1.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    13888 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_1.conf_3.filt.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)    13888 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_1.hdf5
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.242819 spladder-3.0.5/tests/testcase_basic/data/align/pos_2/
+-rw-r--r--   0 akahles    (501) staff       (20)    33821 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_2/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33821 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_2.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_2.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.243181 spladder-3.0.5/tests/testcase_basic/data/align/pos_3/
+-rw-r--r--   0 akahles    (501) staff       (20)    33798 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_3/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33798 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_3.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_3.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.243569 spladder-3.0.5/tests/testcase_basic/data/align/pos_4/
+-rw-r--r--   0 akahles    (501) staff       (20)    33679 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_4/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33679 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_4.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_4.bam.bai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.243960 spladder-3.0.5/tests/testcase_basic/data/align/pos_5/
+-rw-r--r--   0 akahles    (501) staff       (20)    33736 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_5/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    33736 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_5.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/align/pos_5.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)     9734 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/annotation_neg.gtf
+-rw-r--r--   0 akahles    (501) staff       (20)     2232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/data/annotation_neg.gtf.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     9689 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/annotation_pos.gtf
+-rw-r--r--   0 akahles    (501) staff       (20)     2232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/data/annotation_pos.gtf.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      997 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/expr_ts.txt
+-rw-r--r--   0 akahles    (501) staff       (20)      156 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/genome_neg.fa
+-rw-r--r--   0 akahles    (501) staff       (20)      156 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/genome_pos.fa
+-rw-r--r--   0 akahles    (501) staff       (20)   354449 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/testcase_basic_1.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   354449 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/testcase_basic_2.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   354449 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/testcase_basic_3.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   354449 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/testcase_basic_4.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   354449 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/data/testcase_basic_5.fq
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.263628 spladder-3.0.5/tests/testcase_basic/results_merged_neg/
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)       70 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)       70 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      218 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      261 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      163 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      353 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      251 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      343 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      198 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      198 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      296 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      380 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      220 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      370 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      516 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.271164 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3417 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_1.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_2.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_4.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_5.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.294882 spladder-3.0.5/tests/testcase_basic/results_merged_pos/
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)       62 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)       62 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      214 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      256 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      157 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      355 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      246 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      345 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      196 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      196 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      294 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      378 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      218 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      532 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      368 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      522 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.302178 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3417 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_1.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_2.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_4.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     2657 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_5.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.320034 spladder-3.0.5/tests/testcase_basic/results_single_neg/
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      573 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      188 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      229 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1735 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      228 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      323 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.324858 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     2991 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.341714 spladder-3.0.5/tests/testcase_basic/results_single_pos/
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      554 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      185 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      227 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      629 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1728 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      227 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      322 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    24928 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     1104 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.346503 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)     6232 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      168 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      224 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    20968 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     2991 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.347262 spladder-3.0.5/tests/testcase_events/
+-rw-r--r--   0 akahles    (501) staff       (20)       16 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/.gitignore
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.555211 spladder-3.0.5/tests/testcase_events/data/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.638738 spladder-3.0.5/tests/testcase_events/data/align/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.639132 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1/
+-rw-r--r--   0 akahles    (501) staff       (20)   104409 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   104409 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    19406 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.639550 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10/
+-rw-r--r--   0 akahles    (501) staff       (20)    87640 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    87640 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    16115 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.639919 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11/
+-rw-r--r--   0 akahles    (501) staff       (20)   136749 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   136749 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    29045 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       63 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.640365 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12/
+-rw-r--r--   0 akahles    (501) staff       (20)   134059 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   134059 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    26983 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.640807 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13/
+-rw-r--r--   0 akahles    (501) staff       (20)    38654 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    38654 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)     6343 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       45 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.641126 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14/
+-rw-r--r--   0 akahles    (501) staff       (20)   130524 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   130524 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    25683 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.641541 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15/
+-rw-r--r--   0 akahles    (501) staff       (20)    37976 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    37976 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)     6284 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       44 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.641911 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16/
+-rw-r--r--   0 akahles    (501) staff       (20)    99434 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    99434 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    18513 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.642294 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17/
+-rw-r--r--   0 akahles    (501) staff       (20)    57994 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    57994 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)     9914 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       45 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.642626 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18/
+-rw-r--r--   0 akahles    (501) staff       (20)   167608 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   167608 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    38365 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       61 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.643083 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19/
+-rw-r--r--   0 akahles    (501) staff       (20)   126962 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   126962 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    25052 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.643489 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2/
+-rw-r--r--   0 akahles    (501) staff       (20)   152989 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   152989 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    33725 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       62 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.643940 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20/
+-rw-r--r--   0 akahles    (501) staff       (20)    64726 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    64726 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    11132 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.644267 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3/
+-rw-r--r--   0 akahles    (501) staff       (20)   186567 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   186567 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    44739 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       64 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.644741 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4/
+-rw-r--r--   0 akahles    (501) staff       (20)   157108 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   157108 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    34778 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       63 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.645188 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5/
+-rw-r--r--   0 akahles    (501) staff       (20)   187828 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   187828 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    44989 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       63 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.645667 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6/
+-rw-r--r--   0 akahles    (501) staff       (20)   161242 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   161242 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    36501 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       62 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.646097 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7/
+-rw-r--r--   0 akahles    (501) staff       (20)   101824 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   101824 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    18818 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       46 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.646477 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8/
+-rw-r--r--   0 akahles    (501) staff       (20)   157121 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)   157121 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    35296 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       62 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.cram.crai
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.646917 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9/
+-rw-r--r--   0 akahles    (501) staff       (20)    61333 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9/Aligned.sortedByCoord.out.bam
+-rw-r--r--   0 akahles    (501) staff       (20)    61333 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.bam
+-rw-r--r--   0 akahles    (501) staff       (20)       96 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.bam.bai
+-rw-r--r--   0 akahles    (501) staff       (20)    10483 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.cram
+-rw-r--r--   0 akahles    (501) staff       (20)       45 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.cram.crai
+-rw-r--r--   0 akahles    (501) staff       (20)    10128 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/genome.fa
+-rw-r--r--   0 akahles    (501) staff       (20)       16 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/data/genome.fa.fai
+-rw-r--r--   0 akahles    (501) staff       (20)    17651 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events.gtf
+-rw-r--r--   0 akahles    (501) staff       (20)   881921 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample1.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   708663 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample10.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1347762 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample11.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1282725 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample12.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   222750 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample13.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1228463 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample14.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   216112 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample15.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   836951 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample16.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   399396 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample17.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1801167 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample18.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1180269 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample19.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1582743 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample2.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   461865 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample20.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  2139805 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample3.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1627618 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample4.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  2142568 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample5.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1712710 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample6.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   856293 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample7.fq
+-rw-r--r--   0 akahles    (501) staff       (20)  1657408 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample8.fq
+-rw-r--r--   0 akahles    (501) staff       (20)   424277 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample9.fq
+-rw-r--r--   0 akahles    (501) staff       (20)     9964 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/data/testcase_events_spladder.gtf
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.681270 spladder-3.0.5/tests/testcase_events/results_merged/
+-rw-r--r--   0 akahles    (501) staff       (20)      391 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      235 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1669 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      524 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      689 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      307 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1334 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    26976 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     2775 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1617 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      791 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1705 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      545 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      388 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      705 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      966 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      371 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1863 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    29539 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3881 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     2113 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1106 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     2243 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      782 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      466 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     3566 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      807 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      174 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1071 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      414 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     2311 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    30490 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     5942 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     3018 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1332 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     3085 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      472 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      237 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1747 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      532 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      679 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      353 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1159 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    29024 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3481 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1811 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      920 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1686 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2019-08-21 12:47:50.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      348 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      400 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      226 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1050 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    26976 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      659 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      390 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1040 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.txt.gz
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.695549 spladder-3.0.5/tests/testcase_events/results_merged/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)    37736 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      528 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      656 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    23016 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)    25153 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    16577 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    17256 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18100 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18097 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18229 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    17868 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.697695 spladder-3.0.5/tests/testcase_events/results_merged/testing/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.704769 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/
+-rw-r--r--   0 akahles    (501) staff       (20)    18890 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    17086 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18811 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_adjusted_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18193 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_fitted_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18456 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_raw_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13740 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/ma_plot_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    14081 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13478 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13651 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    12509 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)     1595 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.gene_unique.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     1595 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     7756 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_extended_C3_exon_skip.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     6776 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged/testing/test_setup_C3_exon_skip.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.737274 spladder-3.0.5/tests/testcase_events/results_merged_cram/
+-rw-r--r--   0 akahles    (501) staff       (20)      391 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      235 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1669 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      524 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      689 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      307 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1334 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    26976 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     2775 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1617 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      791 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1705 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      545 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      388 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     2775 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      705 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      166 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      966 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      371 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1863 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    29539 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3881 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     2113 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1106 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     2243 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      782 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      466 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     3566 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      807 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      174 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1071 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      414 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     2311 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    30490 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     5942 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     3018 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     1332 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     3085 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      472 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      237 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)     1747 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      532 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      150 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      679 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      353 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1159 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    29024 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)     3481 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)     1811 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      920 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1686 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)     5360 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      126 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.bed
+-rw-r--r--   0 akahles    (501) staff       (20)        0 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.bed
+-rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      348 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.icgc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      134 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      400 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)      226 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.tcga.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1050 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)    26976 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.counts.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      704 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.gff3
+-rw-r--r--   0 akahles    (501) staff       (20)      659 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)      390 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.struc.txt.gz
+-rw-r--r--   0 akahles    (501) staff       (20)     1040 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.txt.gz
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.752980 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/
+-rw-r--r--   0 akahles    (501) staff       (20)    37736 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)      526 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx
+-rw-r--r--   0 akahles    (501) staff       (20)      528 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges
+-rw-r--r--   0 akahles    (501) staff       (20)      656 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs
+-rw-r--r--   0 akahles    (501) staff       (20)    23016 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5
+-rw-r--r--   0 akahles    (501) staff       (20)    25153 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    16577 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    17256 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18100 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18097 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18184 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18229 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    18313 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle
+-rw-r--r--   0 akahles    (501) staff       (20)    17868 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.756738 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/
+drwxr-xr-x   0 akahles    (501) staff       (20)        0 2024-04-23 14:12:15.763853 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/
+-rw-r--r--   0 akahles    (501) staff       (20)    18890 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    17086 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18810 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_adjusted_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18193 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_fitted_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    18453 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_raw_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13740 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/ma_plot_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    14080 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13479 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    13652 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.log10.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)    12510 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.pdf
+-rw-r--r--   0 akahles    (501) staff       (20)     1595 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.gene_unique.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     1595 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     7744 2024-04-23 14:03:12.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_extended_C3_exon_skip.tsv
+-rw-r--r--   0 akahles    (501) staff       (20)     6776 2022-01-07 18:44:19.000000 spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_setup_C3_exon_skip.pickle
```

### Comparing `spladder-3.0.4/PKG-INFO` & `spladder-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spladder
-Version: 3.0.4
+Version: 3.0.5
 Summary: Tool for the detection and quantification of alternative splicing events from RNA-Seq data.
 Home-page: https://github.com/ratschlab/spladder
 Author: Andre Kahles
 Author-email: andre.kahles@inf.ethz.ch
 License: BSD license
 Description: What is SplAdder?
         -----------------
```

### Comparing `spladder-3.0.4/README.md` & `spladder-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/Makefile` & `spladder-3.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/conf.py` & `spladder-3.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/file_formats.rst` & `spladder-3.0.5/docs/source/file_formats.rst`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/general.rst` & `spladder-3.0.5/docs/source/general.rst`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/img/splice_events.png` & `spladder-3.0.5/docs/source/img/splice_events.png`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/index.rst` & `spladder-3.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/installation.rst` & `spladder-3.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/docs/source/spladder_modes.rst` & `spladder-3.0.5/docs/source/spladder_modes.rst`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/setup.py` & `spladder-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords='spladder',
     name='spladder',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ratschlab/spladder',
-    version='3.0.4',
+    version='3.0.5',
     zip_safe=False,
 )
```

### Comparing `spladder-3.0.4/spladder/alt_splice/analyze.py` & `spladder-3.0.5/spladder/alt_splice/analyze.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/alt_splice/collect.py` & `spladder-3.0.5/spladder/alt_splice/collect.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/alt_splice/detect.py` & `spladder-3.0.5/spladder/alt_splice/detect.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/alt_splice/events.py` & `spladder-3.0.5/spladder/alt_splice/events.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/alt_splice/quantify.py` & `spladder-3.0.5/spladder/alt_splice/quantify.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/alt_splice/verify.py` & `spladder-3.0.5/spladder/alt_splice/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         info[2] >= options.intron_retention['min_retention_rel_cov'] * (info[1] + info[3]) / 2) or \
        (options.use_anno_support and exon_long in set([(_[0], _[1]) for _ in np.vstack(gene.exons)])):
         verified[0] = 1
 
     ### check intron confirmation as sum of valid intron scores
     ### intron score is the number of reads confirming this intron
     # intron conf
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon1[-1], seg_exon2[0]], segs.seg_edges.shape))[0]
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon1[-1], seg_exon2[0]], segs.seg_edges.shape))[0].item()
     info[4] = counts_edges[idx, 1]
 
     if (info[4] >= options.intron_retention['min_non_retention_count']) or \
        (options.use_anno_support and intron in gene.introns_anno):
         verified[1] = 1
 
     return (verified, info)
@@ -241,27 +241,27 @@
     if (info[2] >= options.exon_skip['min_skip_rel_cov'] * (info[1] + info[3]) / 2) or \
        (options.use_anno_support and intron_pre in gene.introns_anno and intron_aft in gene.introns_anno): 
         verified[0] = 1
 
     ### check intron confirmation as sum of valid intron scores
     ### intron score is the number of reads confirming this intron
     # exon_pre_exon_conf
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon_pre[-1], seg_exon[0]], segs.seg_edges.shape))[0]
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon_pre[-1], seg_exon[0]], segs.seg_edges.shape))[0].item()
     info[4] = counts_edges[idx, 1]
     if (info[4] >= options.exon_skip['min_non_skip_count']) or \
        (options.use_anno_support and intron_pre in gene.introns_anno):
         verified[1] = 1
     # exon_exon_aft_conf
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon[-1], seg_exon_aft[0]], segs.seg_edges.shape))[0]
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon[-1], seg_exon_aft[0]], segs.seg_edges.shape))[0].item()
     info[5] = counts_edges[idx, 1]
     if (info[5] >= options.exon_skip['min_non_skip_count']) or \
        (options.use_anno_support and intron_aft in gene.introns_anno):
         verified[2] = 1
     # exon_pre_exon_aft_conf
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon_pre[-1], seg_exon_aft[0]], segs.seg_edges.shape))[0]
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([seg_exon_pre[-1], seg_exon_aft[0]], segs.seg_edges.shape))[0].item()
     info[6] = counts_edges[idx, 1]
     if (info[6] >= options.exon_skip['min_skip_count']) or \
        (options.use_anno_support and intron_skip in gene.introns_anno):
         verified[3] = 1
 
     return (verified, info)
 
@@ -349,20 +349,18 @@
     if (info[2] >= options.alt_prime['min_diff_rel_cov'] * ((info[1] * np.sum(seg_lens[seg_const1])) + (info[3] * np.sum(seg_lens[seg_const2]))) / np.sum(seg_lens[np.r_[seg_const1, seg_const2]])) or \
        (options.use_anno_support and intron1 in gene.introns_anno and intron2 in gene.introns_anno):
         verified[0] = 1
 
     ### check intron confirmations as sum of valid intron scores
     ### intron score is the number of reads confirming this intron
     # intron1_conf 
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([segs_exon11[-1], segs_exon12[0]], segs.seg_edges.shape))[0]
-    assert(idx.shape[0] > 0)
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([segs_exon11[-1], segs_exon12[0]], segs.seg_edges.shape))[0].item()
     info[4] = counts_edges[idx, 1]
     # intron2_conf 
-    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([segs_exon21[-1], segs_exon22[0]], segs.seg_edges.shape))[0]
-    assert(idx.shape[0] > 0)
+    idx = np.where(counts_edges[:, 0] == np.ravel_multi_index([segs_exon21[-1], segs_exon22[0]], segs.seg_edges.shape))[0].item()
     info[5] = counts_edges[idx, 1]
 
     if (min(info[4], info[5]) >= options.alt_prime['min_intron_count']) or \
        (options.use_anno_support and intron1 in gene.introns_anno and intron2 in gene.introns_anno):
         verified[1] = 1
 
     return (verified, info)
```

### Comparing `spladder-3.0.4/spladder/alt_splice/write.py` & `spladder-3.0.5/spladder/alt_splice/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         fd.write('%s\t%c\t%s.%i\t%i\t%s' % (events[i].chr, events[i].strand, events[i].event_type, events[i].id, events[i].annotated, events[i].gene_name[0]))
         if anno_fn is not None:
             a_idx = anno_names.index(events[i].gene_name[0])
             fd.write('\t%i\t%i' % (anno[a_idx].start, anno[a_idx].stop))
         
         ### new count chunk needed?
         if i >= chunk_idx_event[1]:
-            chunk_idx_event += cs1
+            chunk_idx_event += cs1 * (1 + (i - chunk_idx_event[1]) // cs1)
             event_counts_chunk = IN['event_counts'][:, :, chunk_idx_event[0]:chunk_idx_event[1]]
         ### new psi chunk needed?
         if i >= chunk_idx_psi[1]:
-            chunk_idx_psi += cs2
+            chunk_idx_psi += cs2 * (1 + (i - chunk_idx_psi[1]) // cs2)
             psi_chunk = IN['psi'][:, chunk_idx_psi[0]:chunk_idx_psi[1]]
 
         ev = events[i]
         counts = event_counts_chunk[:, :, i - chunk_idx_event[0]]
         psi = psi_chunk[:, i - chunk_idx_psi[0]]
         if ev.event_type == 'exon_skip':
             fd.write('\t%i\t%i\t%i\t%i\t%i\t%i' % (ev.exons2[0, 0] + 1, ev.exons2[0, 1], ev.exons2[1, 0] + 1, ev.exons2[1, 1], ev.exons2[2, 0] + 1, ev.exons2[2, 1]))
```

### Comparing `spladder-3.0.4/spladder/classes/datatrack.py` & `spladder-3.0.5/spladder/classes/datatrack.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/classes/event.py` & `spladder-3.0.5/spladder/classes/event.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/classes/gene.py` & `spladder-3.0.5/spladder/classes/gene.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/classes/segmentgraph.py` & `spladder-3.0.5/spladder/classes/segmentgraph.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/classes/splicegraph.py` & `spladder-3.0.5/spladder/classes/splicegraph.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/core/gen_graphs.py` & `spladder-3.0.5/spladder/core/gen_graphs.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/core/spladdercore.py` & `spladder-3.0.5/spladder/core/spladdercore.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/count.py` & `spladder-3.0.5/spladder/count.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/editgraph.py` & `spladder-3.0.5/spladder/editgraph.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/hdf5.py` & `spladder-3.0.5/spladder/hdf5.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/helpers.py` & `spladder-3.0.5/spladder/helpers.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/helpers_viz.py` & `spladder-3.0.5/spladder/helpers_viz.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/init.py` & `spladder-3.0.5/spladder/init.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/merge.py` & `spladder-3.0.5/spladder/merge.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/reads.py` & `spladder-3.0.5/spladder/reads.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/settings.py` & `spladder-3.0.5/spladder/settings.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/spladder.py` & `spladder-3.0.5/spladder/spladder.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     splice.add_argument('--ase-edge-limit', dest='detect_edge_limit', metavar='INT', type=int, help='max number of edges in the graph to still extract events for a gene [500]', default=500)
     splice.add_argument('--curate-alt-prime', dest='curate_alt_prime', action='store_true', help='curate alt prime events [on]', default=True)
     splice.add_argument('--no-curate-alt-prime', dest='curate_alt_prime', action='store_false', default=None)
     splice.add_argument('--quantify-graph', dest='quantify_graph', action='store_true', help='quantify graph [on]', default=True)
     splice.add_argument('--no-quantify-graph', dest='quantify_graph', action='store_false', default=None)
     splice.add_argument('--use-anno-support', dest='use_anno_support', action='store_true', help='use annotation for validating event introns [off]', default=False)
     splice.add_argument('--no-use-anno-support', dest='use_anno_support', action='store_false', default=None)
-    splice.add_argument('--psi-min-reads', dest='psi_min_reads', metavar='INT', help='minimum number of spliced reads covering either isoform to compute PSI [10]', default=10)
+    splice.add_argument('--psi-min-reads', dest='psi_min_reads', metavar='INT', type=int, help='minimum number of spliced reads covering either isoform to compute PSI [10]', default=10)
     splice.add_argument('--qmode', dest='qmode', metavar='STRING', help='quantification mode: single, collect, all [all]', default='all')
     parser_build.set_defaults(func=spladder)
 
     ### RUN MODE "TEST"
     parser_test = subparsers.add_parser('test', help='run mode to differentially test events')
     required_test = parser_test.add_argument_group('MANDATORY')
     required_test.add_argument('-o', '--outdir', dest='outdir', metavar='DIR', help='spladder output directory', default='-')
```

### Comparing `spladder-3.0.4/spladder/spladder_build.py` & `spladder-3.0.5/spladder/spladder_build.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/spladder_prep.py` & `spladder-3.0.5/spladder/spladder_prep.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/spladder_test.py` & `spladder-3.0.5/spladder/spladder_test.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/spladder_viz.py` & `spladder-3.0.5/spladder/spladder_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 import sys
 import os
 import re
 import matplotlib
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
-plt.style.use('seaborn')
+plt.style.use('seaborn-v0_8-whitegrid')
 import matplotlib.gridspec as gridspec
 import matplotlib.patches as patches
 import numpy as np
 import pickle
 import copy
 from collections import namedtuple
```

### Comparing `spladder-3.0.4/spladder/testing/likelihood.py` & `spladder-3.0.5/spladder/testing/likelihood.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/utils.py` & `spladder-3.0.5/spladder/utils.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/viz/axes.py` & `spladder-3.0.5/spladder/viz/axes.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/viz/coverage.py` & `spladder-3.0.5/spladder/viz/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             add_intron_patch2(ax, gene.segmentgraph.segments[1, s], gene.segmentgraph.segments[0, t], np.mean(counts), color=cmap_edg(norm(c)))
 
     if xlim is not None:
         ax.set_xlim(xlim)
 
     ### draw grid
     if grid:
-        ax.grid(b=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
+        ax.grid(visible=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
         ax.xaxis.grid(False)
 
     ax.set_ylim([0, int(seg_counts.max() * 1.1)])
 
 def cov_from_bam(chrm, start, stop, files, subsample=0, verbose=False,
                  bins=None, log=False, ax=None, ymax=0, outfile=None,
                  frm='pdf', xlim=None, title=None, xoff=None, yoff=None,
@@ -316,15 +316,15 @@
     if strand == '+':
         ax.arrow(0.05, 0.9, 0.2, 0, head_width=0.05, head_length=0.02, fc='#cccccc', ec='#cccccc', transform=ax.transAxes)
     elif strand == '-':
         ax.arrow(0.25, 0.9, -0.2, 0, head_width=0.05, head_length=0.02, fc='#cccccc', ec='#cccccc', transform=ax.transAxes)
 
     ### draw grid
     if grid:
-        ax.grid(b=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
+        ax.grid(visible=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
         ax.xaxis.grid(False)
 
     if marker_pos is not None:
         ax.plot(0, marker_pos, 'or')
 
     if log:
         ax.set_ylabel('coverage (log10)')
```

### Comparing `spladder-3.0.4/spladder/viz/diagnose.py` & `spladder-3.0.5/spladder/viz/diagnose.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder/viz/genelets.py` & `spladder-3.0.5/spladder/viz/genelets.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     if ax is None:
         fig = plt.figure(figsize = (10, 4))
         ax = fig.add_subplot(111)
     
     ### draw grid
     if grid:
-        ax.grid(b=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
+        ax.grid(visible=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
         ax.yaxis.grid(False)
 
     min_ex = None
     max_ex = None
     for i, exons in enumerate(exon_set):
         if len(exons.shape) == 1:
             exons = exons[np.newaxis, :]
```

### Comparing `spladder-3.0.4/spladder/viz/graph.py` & `spladder-3.0.5/spladder/viz/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                edge_color='#999999', label=None):
     """Takes a graph given as vertices and edges and visualizes its structure"""
 
     start = vertices.ravel().min()
     stop = vertices.ravel().max()
 
     ### draw grid
-    ax.grid(b=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
+    ax.grid(visible=True, which='major', linestyle='--', linewidth=0.2, color='#222222')
     ax.yaxis.grid(False)
 
     ### nodes
     patchlist = []
     exon_num = np.zeros((stop - start,))
     exon_loc = np.zeros((1, stop - start))
     exon_level = np.zeros((vertices.shape[1], )) #vertices.shape[1]))
```

### Comparing `spladder-3.0.4/spladder/viz/highlight.py` & `spladder-3.0.5/spladder/viz/highlight.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/spladder.egg-info/PKG-INFO` & `spladder-3.0.5/spladder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spladder
-Version: 3.0.4
+Version: 3.0.5
 Summary: Tool for the detection and quantification of alternative splicing events from RNA-Seq data.
 Home-page: https://github.com/ratschlab/spladder
 Author: Andre Kahles
 Author-email: andre.kahles@inf.ethz.ch
 License: BSD license
 Description: What is SplAdder?
         -----------------
```

### Comparing `spladder-3.0.4/spladder.egg-info/SOURCES.txt` & `spladder-3.0.5/spladder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/templates/annotation_pos.gtf` & `spladder-3.0.5/tests/templates/annotation_pos.gtf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/test_end_to_end.py` & `spladder-3.0.5/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_1/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_1/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_1.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_1.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_1.conf_3.filt.hdf5` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_1.conf_3.filt.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_1.hdf5` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_1.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_2/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_2/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_2.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_2.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_3/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_3/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_3.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_3.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_4/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_4/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_4.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_4.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_5/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_5/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/neg_5.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/neg_5.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_1/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_1/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_1.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_1.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_1.conf_3.filt.hdf5` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_1.conf_3.filt.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_1.hdf5` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_1.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_2/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_2/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_2.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_2.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_3/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_3/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_3.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_3.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_4/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_4/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_4.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_4.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_5/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_5/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/align/pos_5.bam` & `spladder-3.0.5/tests/testcase_basic/data/align/pos_5.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/annotation_neg.gtf` & `spladder-3.0.5/tests/testcase_basic/data/annotation_neg.gtf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/annotation_neg.gtf.pickle` & `spladder-3.0.5/tests/testcase_basic/data/annotation_neg.gtf.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/annotation_pos.gtf` & `spladder-3.0.5/tests/testcase_basic/data/annotation_pos.gtf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/annotation_pos.gtf.pickle` & `spladder-3.0.5/tests/testcase_basic/data/annotation_pos.gtf.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/expr_ts.txt` & `spladder-3.0.5/tests/testcase_basic/data/expr_ts.txt`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/testcase_basic_1.fq` & `spladder-3.0.5/tests/testcase_basic/data/testcase_basic_1.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/testcase_basic_2.fq` & `spladder-3.0.5/tests/testcase_basic/data/testcase_basic_2.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/testcase_basic_3.fq` & `spladder-3.0.5/tests/testcase_basic/data/testcase_basic_3.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/testcase_basic_4.fq` & `spladder-3.0.5/tests/testcase_basic/data/testcase_basic_4.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/data/testcase_basic_5.fq` & `spladder-3.0.5/tests/testcase_basic/data/testcase_basic_5.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.txt.gz` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_intron_retention_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/merge_graphs_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.merge_graphs.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_1.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_2.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_2.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_4.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_4.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_5.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_neg/spladder/genes_graph_conf3.neg_5.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.gff3` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.txt.gz` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_intron_retention_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/merge_graphs_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.merge_graphs.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_1.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_2.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_2.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_4.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_4.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_5.pickle` & `spladder-3.0.5/tests/testcase_basic/results_merged_pos/spladder/genes_graph_conf3.pos_5.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/neg_1_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_neg/spladder/genes_graph_conf3.neg_1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/pos_1_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.pickle` & `spladder-3.0.5/tests/testcase_basic/results_single_pos/spladder/genes_graph_conf3.pos_1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample1.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample1.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample10.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample10.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample11.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample11.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample12.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample12.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample13.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample13.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample14.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample14.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample15.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample15.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample16.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample16.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample17.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample17.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample18.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample18.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample19.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample19.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample2.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample2.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample20.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample20.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample3.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample3.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample4.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample4.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample5.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample5.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample6.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample6.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample7.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample7.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample8.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample8.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9/Aligned.sortedByCoord.out.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9/Aligned.sortedByCoord.out.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.bam` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.bam`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/align/testcase_events_1_sample9.cram` & `spladder-3.0.5/tests/testcase_events/data/align/testcase_events_1_sample9.cram`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/genome.fa` & `spladder-3.0.5/tests/testcase_events/data/genome.fa`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events.gtf` & `spladder-3.0.5/tests/testcase_events/data/testcase_events.gtf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample1.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample1.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample10.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample10.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample11.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample11.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample12.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample12.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample13.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample13.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample14.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample14.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample15.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample15.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample16.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample16.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample17.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample17.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample18.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample18.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample19.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample19.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample2.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample2.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample20.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample20.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample3.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample3.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample4.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample4.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample5.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample5.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample6.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample6.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample7.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample7.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample8.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample8.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_1_sample9.fq` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_1_sample9.fq`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/data/testcase_events_spladder.gtf` & `spladder-3.0.5/tests/testcase_events/data/testcase_events_spladder.gtf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_3prime_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.bed` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.bed`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_alt_5prime_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.bed` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.bed`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_exon_skip_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_intron_retention_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged/merge_graphs_mutex_exons_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.merge_graphs.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/count_distribution.exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_adjusted_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_adjusted_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_fitted_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_fitted_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/dispersion_raw_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/dispersion_raw_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/ma_plot_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/ma_plot_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.adj.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/plots/qq_plot_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.gene_unique.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.gene_unique.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_C3_exon_skip.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/test_results_extended_C3_exon_skip.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/test_results_extended_C3_exon_skip.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged/testing/test_setup_C3_exon_skip.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged/testing/test_setup_C3_exon_skip.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_3prime_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.bed` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.bed`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_alt_5prime_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.bed` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.bed`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_exon_skip_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.icgc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.struc.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.struc.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_intron_retention_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mult_exon_skip_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.confirmed.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.counts.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.counts.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.gff3` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.gff3`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.txt.gz` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/merge_graphs_mutex_exons_C3.txt.gz`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_edge_idx`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_edges`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.count.hdf5.quick_ids_segs`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.gene_exp.hdf5`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.merge_graphs.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample1.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample10.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample11.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample12.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample13.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample14.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample15.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample16.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample17.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample18.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample19.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample2.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample20.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample3.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample4.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample5.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample6.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample7.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample8.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/spladder/genes_graph_conf3.testcase_events_1_sample9.pickle`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/count_distribution.exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_adjusted_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_adjusted_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_fitted_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_fitted_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/dispersion_raw_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/dispersion_raw_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/ma_plot_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/ma_plot_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.adj.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.log10.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.log10.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.pdf` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/plots/qq_plot_exon_skip.pdf`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.gene_unique.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.gene_unique.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_C3_exon_skip.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_results_extended_C3_exon_skip.tsv` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_results_extended_C3_exon_skip.tsv`

 * *Files identical despite different names*

### Comparing `spladder-3.0.4/tests/testcase_events/results_merged_cram/testing/test_setup_C3_exon_skip.pickle` & `spladder-3.0.5/tests/testcase_events/results_merged_cram/testing/test_setup_C3_exon_skip.pickle`

 * *Files identical despite different names*

