# Comparing `tmp/pairtools-1.0.3.tar.gz` & `tmp/pairtools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pairtools-1.0.3.tar", last modified: Mon Nov 20 19:32:47 2023, max compression
+gzip compressed data, was "pairtools-1.1.0.tar", last modified: Tue Apr 23 19:21:29 2024, max compression
```

## Comparing `pairtools-1.0.3.tar` & `pairtools-1.1.0.tar`

### file list

```diff
@@ -1,126 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.297023 pairtools-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2023-11-20 19:32:31.000000 pairtools-1.0.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-20 19:32:31.000000 pairtools-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-20 19:32:31.000000 pairtools-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2023-11-20 19:32:47.297023 pairtools-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-11-20 19:32:31.000000 pairtools-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.281023 pairtools-1.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.285023 pairtools-1.0.3/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    54070 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/hic-processing-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (127)    23804 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/hic-processing-pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (127)   304356 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read-vs-alignment-vs-pairs.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16927 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_MU.png
--rw-r--r--   0 runner    (1001) docker     (127)    43535 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_MU_MM_NM.png
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_NU.png
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_NU_NN.png
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_UR.png
--rw-r--r--   0 runner    (1001) docker     (127)    33143 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_UR_MorN.png
--rw-r--r--   0 runner    (1001) docker     (127)    44943 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_UR_criteria.png
--rw-r--r--   0 runner    (1001) docker     (127)    33056 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_WW.png
--rw-r--r--   0 runner    (1001) docker     (127)    28811 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/read_pair_gaps_vs_null_alignment.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    20222 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/report-orientation.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    30397 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/report-positions.svg
--rw-r--r--   0 runner    (1001) docker     (127)    21164 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/rescue_modes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24638 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/rescue_modes_readthrough.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33232 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/_static/terminology.png
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/cli_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.285023 pairtools-1.0.3/doc/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.289023 pairtools-1.0.3/doc/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (127)   561452 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/benchmark/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/benchmark/benchmarking_1mln.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/example_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/example_singlecell_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (127)    73813 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/pairtools_phase_walkthrough.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   278013 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/pairtools_restrict_walkthrough.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   157369 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/pairtools_walkthrough.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    81628 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/examples/scalings_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/sorting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2023-11-20 19:32:31.000000 pairtools-1.0.3/doc/technotes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.289023 pairtools-1.0.3/pairtools/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.289023 pairtools-1.0.3/pairtools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/dedup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/filterbycov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/flip.py
--rw-r--r--   0 runner    (1001) docker     (127)    18402 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/markasdup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/parse2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/restrict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/cli/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.293022 pairtools-1.0.3/pairtools/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18534 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/dedup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/dedup_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/filterbycov.py
--rw-r--r--   0 runner    (1001) docker     (127)    24272 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/headerops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/pairsam_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    56326 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/parse_pysam.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/regions.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/restrict.py
--rw-r--r--   0 runner    (1001) docker     (127)    14031 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/select.py
--rw-r--r--   0 runner    (1001) docker     (127)    39346 2023-11-20 19:32:31.000000 pairtools-1.0.3/pairtools/lib/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.289023 pairtools-1.0.3/pairtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-20 19:32:47.000000 pairtools-1.0.3/pairtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-20 19:32:31.000000 pairtools-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-20 19:32:31.000000 pairtools-1.0.3/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 19:32:47.297023 pairtools-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2023-11-20 19:32:31.000000 pairtools-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.293022 pairtools-1.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 19:32:47.297023 pairtools-1.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.2.pairsam
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.4dedup.pairsam
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.4filterbycov.pairs
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.4flip.pairs
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.4stats.pairs
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.chrom.sizes
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.pairsam
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.parse-all.sam
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.parse2.sam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.rsites.bed
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.sam
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/data/mock.test-restr.pairs
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_dedup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_filterbycov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_headerops.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_markasdup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_parse2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_restrict.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2023-11-20 19:32:31.000000 pairtools-1.0.3/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.018078 pairtools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-23 19:21:21.000000 pairtools-1.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 19:21:21.000000 pairtools-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-23 19:21:21.000000 pairtools-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-23 19:21:29.018078 pairtools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-23 19:21:21.000000 pairtools-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:28.998077 pairtools-1.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.002078 pairtools-1.1.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    54070 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/hic-processing-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23804 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/hic-processing-pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   304356 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read-vs-alignment-vs-pairs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16927 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_MU.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43535 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_MU_MM_NM.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_NU.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_NU_NN.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_UR.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33143 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_UR_MorN.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44943 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_UR_criteria.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33056 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_WW.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28811 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/read_pair_gaps_vs_null_alignment.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20222 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/report-orientation.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30397 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/report-positions.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    21164 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/rescue_modes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24638 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/rescue_modes_readthrough.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33232 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/_static/terminology.png
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/cli_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/designnotes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.002078 pairtools-1.1.0/doc/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.006078 pairtools-1.1.0/doc/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)   561452 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/benchmark/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/benchmark/benchmarking_1mln.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   169526 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/duplicate_distance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/example_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/example_singlecell_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   106274 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/pairtools_phase_walkthrough.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   278001 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/pairtools_restrict_walkthrough.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   157369 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/pairtools_walkthrough.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   129783 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/examples/scalings_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/protocols_pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/sorting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-23 19:21:21.000000 pairtools-1.1.0/doc/stats.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.006078 pairtools-1.1.0/pairtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.010078 pairtools-1.1.0/pairtools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18850 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/filterbycov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18402 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/markasdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/parse2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/restrict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/cli/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.014078 pairtools-1.1.0/pairtools/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22841 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/dedup_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/filterbycov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23828 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/headerops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/pairsam_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/pairsio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56320 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/parse_pysam.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/regions.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/restrict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15590 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45489 2024-04-23 19:21:21.000000 pairtools-1.1.0/pairtools/lib/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.018078 pairtools-1.1.0/pairtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 19:21:28.000000 pairtools-1.1.0/pairtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 19:21:21.000000 pairtools-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 19:21:21.000000 pairtools-1.1.0/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:21:29.018078 pairtools-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-23 19:21:21.000000 pairtools-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.014078 pairtools-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:29.018078 pairtools-1.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.2.pairsam
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.4dedup.pairsam
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.4dedup_diffcolnames.pairsam
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.4filterbycov.pairs
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.4flip.pairs
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.4stats.pairs
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.chrom.sizes
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.pairsam
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.parse-all.sam
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.parse2.sam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.rsites.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock.test-restr.pairs
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/data/mock_empty.4dedup.pairsam
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_dedup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_filterbycov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_headerops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_markasdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_parse2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_restrict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-23 19:21:21.000000 pairtools-1.1.0/tests/test_stats.py
```

### Comparing `pairtools-1.0.3/LICENSE` & `pairtools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/PKG-INFO` & `pairtools-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pairtools
-Version: 1.0.3
+Version: 1.1.0
 Summary: CLI tools to process mapped Hi-C data
 Home-page: https://github.com/open2c/pairtools
 Author: Open2C
 Author-email: open.chromosome.collective@gmail.com
 License: MIT
 Keywords: genomics,bioinformatics,Hi-C,contact
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cython
+Requires-Dist: numpy>=1.10
+Requires-Dist: click>=6.6
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: pandas>=1.3.4
+Requires-Dist: pysam>=0.15.0
+Requires-Dist: pyyaml
+Requires-Dist: bioframe>=0.3.3
 
 # pairtools
 
 [![Documentation Status](https://readthedocs.org/projects/pairtools/badge/?version=latest)](http://pairtools.readthedocs.org/en/latest/)
 [![Build Status](https://travis-ci.org/mirnylab/pairtools.svg?branch=master)](https://travis-ci.org/mirnylab/pairtools)
 [![Join the chat on Slack](https://img.shields.io/badge/chat-slack-%233F0F3F?logo=slack)](https://bit.ly/2UaOpAe)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1490831.svg)](https://doi.org/10.5281/zenodo.1490831)
```

### Comparing `pairtools-1.0.3/README.md` & `pairtools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/Makefile` & `pairtools-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/hic-processing-pipeline.png` & `pairtools-1.1.0/doc/_static/hic-processing-pipeline.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/hic-processing-pipeline.svg` & `pairtools-1.1.0/doc/_static/hic-processing-pipeline.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read-vs-alignment-vs-pairs.svg` & `pairtools-1.1.0/doc/_static/read-vs-alignment-vs-pairs.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_MU.png` & `pairtools-1.1.0/doc/_static/read_pair_MU.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_MU_MM_NM.png` & `pairtools-1.1.0/doc/_static/read_pair_MU_MM_NM.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_NU.png` & `pairtools-1.1.0/doc/_static/read_pair_NU.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_NU_NN.png` & `pairtools-1.1.0/doc/_static/read_pair_NU_NN.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_UR.png` & `pairtools-1.1.0/doc/_static/read_pair_UR.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_UR_MorN.png` & `pairtools-1.1.0/doc/_static/read_pair_UR_MorN.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_UR_criteria.png` & `pairtools-1.1.0/doc/_static/read_pair_UR_criteria.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_WW.png` & `pairtools-1.1.0/doc/_static/read_pair_WW.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/read_pair_gaps_vs_null_alignment.png` & `pairtools-1.1.0/doc/_static/read_pair_gaps_vs_null_alignment.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/report-orientation.svg` & `pairtools-1.1.0/doc/_static/report-orientation.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/report-positions.svg` & `pairtools-1.1.0/doc/_static/report-positions.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/rescue_modes.svg` & `pairtools-1.1.0/doc/_static/rescue_modes.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/rescue_modes_readthrough.svg` & `pairtools-1.1.0/doc/_static/rescue_modes_readthrough.svg`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/_static/terminology.png` & `pairtools-1.1.0/doc/_static/terminology.png`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/conf.py` & `pairtools-1.1.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-# sys.path.insert(0, os.path.abspath('.'))
+sys.path.insert(0, os.path.abspath('..'))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -34,15 +34,14 @@
     "sphinx.ext.coverage",
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinx.ext.mathjax",
     "sphinx_click.ext",
-    "recommonmark",
     "nbsphinx",
     "sphinx_rtd_theme",
 ]
 # extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
@@ -96,15 +95,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
```

### Comparing `pairtools-1.0.3/doc/examples/benchmark/Snakefile` & `pairtools-1.1.0/doc/examples/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/examples/benchmark/benchmark.ipynb` & `pairtools-1.1.0/doc/examples/benchmark/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/examples/benchmark/benchmarking_1mln.csv` & `pairtools-1.1.0/doc/examples/benchmark/benchmarking_1mln.csv`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/examples/example_pipeline.sh` & `pairtools-1.1.0/doc/examples/example_pipeline.sh`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/examples/example_singlecell_pipeline.sh` & `pairtools-1.1.0/doc/examples/example_singlecell_pipeline.sh`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/examples/pairtools_restrict_walkthrough.ipynb` & `pairtools-1.1.0/doc/examples/pairtools_restrict_walkthrough.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998421717171717%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '# Pairtools restrict walkthrough\\n')], delete: [0]}}, "*

 * *            "18: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAA5IAAAJyCAYAAAC2Qv8kAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAB+DElEQVR4nOzdeZyP9f7/8efLzJjBWIYhFMYSkqJSlpQ9a9QpJSmUflrOOVKnlUIUvu2b6nSKog4pR7ajVJbSKOqkUiRZqiNLI9liZrx/f3yWM5/PfGbmc82Ox/12+9yY9/V+X9f7el/b5/V5X9f7MuecAAAAAACIVpmSrgAAAAAA […]*

```diff
@@ -38,15 +38,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "66194c2b-8c1b-4e21-80ef-1d2bf069199c",
             "metadata": {},
             "source": [
-                "# Pairtools: restriction walkthrough\n",
+                "# Pairtools restrict walkthrough\n",
                 "\n",
                 "The common approach to analyse Hi-C data is based to analyse the contacts of the restriction fragments. It is used in *hiclib*, Juicer, HiC-Pro. \n",
                 "\n",
                 "Throughout this notebook, we will work with one of [Rao et al. 2014 datasets for IMR90 cells](https://data.4dnucleome.org/experiment-set-replicates/4DNES1ZEJNRU/) [1]. \n",
                 "\n",
                 "\n",
                 "[1] Rao, S. S., Huntley, M. H., Durand, N. C., Stamenova, E. K., Bochkov, I. D., Robinson, J. T., Sanborn, A. L., Machol, I., Omer, A. D., Lander, E. S., & Aiden, E. L. (2014). A 3D map of the human genome at kilobase resolution reveals principles of chromatin looping. Cell, 159(7), 1665\u20131680. https://doi.org/10.1016/j.cell.2014.11.021"
@@ -225,15 +225,15 @@
             "cell_type": "code",
             "execution_count": 8,
             "id": "1a7ef073-082b-4aa6-972f-85ada84be4d4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5IAAAJyCAYAAAC2Qv8kAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAB+DElEQVR4nOzdeZyP9f7/8efLzJjBWIYhFMYSkqJSlpQ9a9QpJSmUflrOOVKnlUIUvu2b6nSKog4pR7ajVJbSKOqkUiRZqiNLI9liZrx/f3yWM5/PfGbmc82Ox/12+9yY9/V+X9f7el/b5/V5X9f7MuecAAAAAACIVpmSrgAAAAAA4NhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAAT2JLugIniuTkZJeSklLS1QAAAABwnPrss892O+eqF8eyCCSLSUpKitasWVPS1QAAAABwnDKzrcW1LG5tBQAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnjNqKY87Ro0d15MgRHT16tKSrAgAAABSpMmXKqGzZsipTpnT1AZau2gB5SE9P186dO5Wenl7SVQEAAACKXGn9/kuPJI4ZR48e1a+//qqTTjpJZlbS1QEAAACKRWJionbs2KEaNWqUmp7J0lELIApHjhxRhQoVCCIBAABwQjEzVahQoVT1ShJI4phx9OhRxcTElHQ1AAAAgGIXExOjzMzMkq5GEIEkAAAAAMATAkkAAAAAgCcEkgAAAAAATxi1FceF1z/ZVqLLH9i6br7KTZs2TUOHDg3+Xb58eVWvXl1nnXWWrrrqKl1++eUhI3Nt2bJF9evX19SpUzVkyJColrFs2TItW7ZM999/f6kZ5Su/UlNTdeutt+rrr7/WwYMH9Z///EctW7Ys6Wpl88QTT6hu3br605/+FJI+duxYjRs3Tunp6YqNLbrTb04DUmVtr8C+tHTpUnXs2LHI6lJQgbotW7asROsRqEOnTp3ybLNp06bp6NGjuu666wpt2XPnztUPP/yg2267LWKdlixZoq5duxba8k4UObVraXE8nb8LQ6RjMKfzLUqX/Hx/KQlDhgzRsmXLtGXLlpKuyjGBsxJQCsyePVupqalatGiRxo8fr/j4eF111VW66KKLdOjQoWC+WrVqKTU1Vb1794563suWLdO4ceN09OjRoqh6sbr++uuVkZGh+fPnKzU1VY0bNy7pKkX0xBNPaM6cOSVahyFDhig1NTXkU1rb63gzbdo0vfzyy4U6z7lz5+qxxx4r1Hmi9Lfr8XT+Lgxnn322UlNTdfbZZwfTSsP5FjhR0SMJlAItW7ZUo0aNgn9fc8016t+/v/r3768777xTTz/9tCQpPj5ebdq0KalqlqijR49qw4YNGjVqlDp37pxr3sOHDys+Pr6YalY6nXzyyUW2r9C+KCmZmZlyzhVpj/6xKnCnw7H4iqxozymVKlUqVdfAjh07KiUlRdOmTSvpqhzXuOaUXvRIAqXUZZddpn79+unFF1/UwYMHJfluDTGzkIvW6tWr1a1bN1WrVk3ly5dXgwYNdPPNN0v6362UkhQXFyczC/mSMWbMGJ199tmqXLmykpOT1blzZ61atSqkHsuWLZOZad68efrzn/+s5ORkVa9eXYMGDdJvv/0WkjcjI0OTJ09Ws2bNlJCQoOrVq6tHjx5av359MM/u3bt100036eSTT1Z8fLyaNm2qv//977m2xbRp0xQTE6OjR49q/PjxMjOlpKRI8vW8nXLKKUpNTVW7du1Urlw53XnnnZKkDRs26NJLL1WVKlVUrlw5tWnTRosXLw6Z99ixY2VmWr9+vbp3764KFSqobt26mjp1qiRp+vTpatq0qRITE9WpUydt2rQp17qmpKRo69ateu2114LtHX4bz+bNm9W7d28lJiaqXr16euCBB7L1OOSnnYpCbu0bTR137dql4cOHq3Hjxipfvrzq1KmjgQMH6ueff862rJkzZ6pp06aKj4/X6aefrn/9619R1/PgwYO66667VL9+fZUtW1b169fXgw8+GNKuXvblXbt2aeDAgapUqZKqVKmia6+9NlueSDp27Kjly5dr5cqVwe2f9TbYTz/9VF27dlViYqIqVKigLl266NNPP811nkOGDNErr7yin3/+OTjPwP6fdf2jOT4nTpwYbOPatWvr9ttv1x9//JHnepmZRo8eraeeekr169dXxYoV1aFDB61bty5b3jlz5qhNmzYqX768qlSpov79+2vbttDHD2bOnKnOnTurevXqSkxM1FlnnaVXXnkl4nJHjRqlSZMmBbftV199JUlavny5unTpoooVK6pChQrq3r27vv7665Dy77zzjtq1a6fKlSsrMTFRTZo00QMPPBB1u2YV2H/Cb7OeNm2azCzkVriUlBQNGjRIL774oho1aqSEhASdffbZWrp0aUjZ/J6/A9eCKVOm6M4771Tt2rUVHx8f3OaFvQ1Gjx6tRx99VPXq1VOFChXUu3dv7dy5Uzt37tQVV1yhypUrq06dOpo8eXKO7RfejnPmzNENN9yg6tWr66STTpIkfffdd7r00ktVo0YNJSQkqG7duurfv78yMjIiboO8zrdr165V3759lZSUpHLlyun888/Xhx9+mGcdi1rHjh3Vvn17LV68WC1btlS5cuV01lln6ZNPPlFGRobuvfde1apVS1WrVtWQIUN04MCBkPJert1vvfWWhgwZoqSkJFWqVElXX321fv3115C8gePswQcf1CmnnKJy5crpwgsv1BdffJGt7tHsWwcPHtTNN9+satWqKTExUX379tVPP/0UVdsErslff/21unfvrsTERF1xxRXB+eZ1nv/jjz80cuRINW/eXImJiapZs6YuvvjikO8hAe+//77OPvtsJSQkqGHDhnrhhRey5cnIyNB9992nhg0bKiEhQcnJyWrfvr0++uijqNbneMdPekAp1qtXL82dO1dr1qzRhRdemG36/v371b17d5133nmaNm2aKlasqC1btujjjz+WJA0bNkw//fSTXnrpJX300UfZ3sP5888/a+TIkTrllFN04MABzZgxQxdeeKHWrFmjM888MyTviBEj1KdPH73++uvasGGD7rzzTsXExIR88RgwYIDmzp2rW2+9VV27dtUff/yhFStWaPv27WratKl+//13nX/++Tp06JDGjh2r+vXr65133tFNN92kw4cP6y9/+UvEdujdu7c++ugjtW/fXtdff72GDRsW8uvk3r17NWDAAP3tb3/TQw89pHLlyum///2v2rdvr4oVK+qZZ55R5cqV9eyzz6p3795asGCBevbsGbKM/v3764YbbtDf/vY3TZkyRdddd502btyoZcuWadKkSUpPT9eIESM0cOBAffLJJzlus3/961/q1auXWrRoobFjx0qSqlevHpLn0ksv1dChQzVy5EjNnz9fY8aMUZ06dYLPy+a3nbJ67rnn9PDDDysmJkZt2rTRuHHjdMEFFwSnp6SkyDmX53xyat9o65iWlqaEhARNnDhR1atX13//+189+uijOv/887V+/XolJCRIkt577z0NHDhQvXv31qOPPqpdu3ZpxIgRSk9PV5MmTXKtX0ZGhrp3765vvvlG9913n8444wytWrVK48ePV1pamh599NGQ/NHsy3/605+0du1aPfTQQzr11FM1a9asqNp9ypQpGjRokDIzM4NfSipVqiRJ+vLLL9WhQwc1a9YsGHxMmjRJHTp00KpVq9SiRYuI87zvvvu0a9curV69WvPmzZOkbL/OR7NOgwYN0vz583XXXXepXbt2+vbbb3Xfffdpy5Yteuutt/JctxkzZqhJkyZ68skndeTIEd1xxx3q16+f1q9fH+whfP7553XTTTdp6NChuv/++7Vv3z6NHTtWHTp00JdffqmKFStKkn744Qddfvnluvvuu1WmTBmtWLFCw4YN06FDh3TjjTeGLHfatGlq0KCBHnnkEVWoUEG1a9fWwoUL1a9fP/Xu3VszZsyQJE2ePFkXXHCBvvzyS9WpU0c//PCD+vbtq8svv1z333+/ypYtq40bN+qHH36Iul0LYvny5frss8/04IMPKj4+XpMnT1bPnj21du1aNWnSpMDnb0l68MEHde655+rvf/+7MjMzlZCQUCTbYPr06WrevLmmTJmiHTt26NZbb9W1116rffv2qWfPnvp//+//afbs2br77rt1xhlnqFevXnm2z1/+8hf17NlT06dPD/6Y0adPH1WpUkXPPfeckpOT9fPPP2vRokU53tqb2/n2888/1wUXXKCzzjpLL774osqXL6/nn39eXbt21ccff6xzzjknug1ZRL7//nvdcccdGjVqlBITE3XnnXeqb9++6tu3rzIyMjRt2jR9++23uuOOO1SjRg393//9X7Csl2t34Hr8z3/+Uxs3btS9996r//73v9l+1Hj11VdVt25dPfPMMzp8+LDuv/9+denSRRs3blTVqlUlRX98Dx8+XLNmzdKYMWN07rnnasmSJRo4cKCn9unXr5+uv/563XXXXSpTpkzU5/nDhw9r3759Gj16tGrVqqW0tDRNmTJFbdq00fr161WzZk1J0rfffqtevXqpVatWmjlzpg4fPqyxY8dq//79Icfa5MmT9fjjj+vBBx9Uy5Yt9fvvv2vNmjVKS0vztD7HLeccn2L4nHPOOQ4Fc+DAAXfgwIGI015btbVEP/k1depUJ8lt3Lgx4vTFixc7SW7mzJnOOec2b97sJLmpU6c655xbvXq1k+TWrl2b4zLGjBnjJLn09PRc65KRkeHS09Nd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3jzYa3Do0KHgiV7yjX4WExMTcrL+4IMPtG3bNtWvX99zfS+66CJNmjRJ//jHP3IclKRHjx56+umnVbdu3WBPSFHp0KGDnnjiCW3ZsiV4gcnMzNSsWbN01llnhbRFYYuPjw95/6dXhd1Ov//+uxYuXKjWrVsXeF4B0dbx4MGDIbcHSwqOiBsQExOjc889V2+++abGjh0b/IL3ySefaMuWLXkGkj169NBbb72lxMTE4O1hBdG2bVtlZmbqrbfeCrkda+bMmVGVj4+P1759+7Kld+jQQQsXLtS+ffuC+9++ffs0f/78kJFdc5pnQfepyZMna+/everSpUu+55Obdu3aqWLFivr+++81ePDgHPMFRqEO/xL89ttvR7WcJk2aKCUlRevWrdPdd98dVZn4+Hh17txZ+/fvV79+/bR582YlJyd7atfAfvj1118HbwmWpEWLFkXMv2rVKv3444+qU6eOJN+2XrhwYcT3AHs9f+ekuLZBUTMztWzZUo899pheeuklff311zkGkpG2YYUKFXTBBRdo7dq1Ovvssz0HjaWZ12v3G2+8oeuuuy749+zZs3X06FG1bds2JN+iRYt04MCB4K2eW7Zs0apVq4LHWLT7VuvWrVWmTBm98cYbIcdntOfPnER7nj948GC21wNNnz492KMb0LZt22zr/OOPP2rlypU5/rBWs2ZNDRs2TIsWLco2QvSJikASKAW++OIL7d69W0eOHNG2bdu0YMECzZ49W926ddPEiRNzLLdgwQL9/e9/1yWXXKL69evrwIEDeuqpp1SxYsXgRaJZs2aSpEcffVQ9e/ZUTEyMWrVqpR49euiJJ57QkCFDNHToUH333XcaP358tl8po9WpUydddtlluu222/Tjjz+qc+fOSk9P14oVK9S7d2917NhRI0eO1KxZs3TBBRdo5MiRatKkiQ4cOKD169frww8/LNQvMSNHjtS0adPUrVs3jRs3TpUqVdKUKVP03XffaeHChYW2nEiaNWumDz/8UAsWLFDNmjWVnJzsqVesIO30yCOPaMOGDerUqZNq166trVu36pFHHtEvv/yi1157rRDWzlsdAwHMQw89pPPOO08ffPCB3nzzzWzzGzdunC666CJdcsklGj58uHbt2qUxY8YER9jLzdVXX62pU6eqS5cuuv3229WiRQsdOXJEmzZt0rx58zR37tyofowJ6Nat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9FN17dpViYmJqlChgrp06aJPP/0013kOGTJEr7zyin7++efgPAP7f9b1j+b4nDhxYrCNa9eurdtvv11//PFHnutlZho9erSeeuop1a9fXxUrVlSHDh20bt26bHnnzJmjNm3aqHz58qpSpYr69++vbdu2heSZOXOmOnfurOrVqysxMVFnnXWWXnnllYjLHTVqlCZNmhTctl999ZUkafny5erSpYsqVqyoChUqqHv37vr6669Dyr/zzjtq166dKleurMTERDVp0kQPPPBA1O0a7ocfflDv3r1Vvnx5Va9eXSNGjNDhw4ez5UtPT9fo0aOVkpKismXLKiUlRaNHj1Z6enowT/PmzTVs2LDg33v37lVMTIxOOeWUkHmdf/75uuKKK0LaJJptkd91Dxwnc+bM0Q033KDq1avrpJNOCs73xRdfVIsWLZSQkKDk5GRdf/31SktLC1n2M888o7Zt26pq1aqqUqWK2rRpo4ULF4bkCVzPnn/+ed1zzz2qWbOmKlasqEGDBungwYP6/vvv1b17dyUmJqpRo0YR949wgdtTV6xYof79+6tKlSpq3bq1pNyvlVnLBm5tDVwrH3zwwWAbZQ3qotn/SkJKSooGDRqk6dOnq0mTJipXrpwuuOACbdy4UQcOHNDw4cNVrVo1nXTSSbr99ttDHrX4448/NHLkSDVv3lyJiYmqWbOmLr744pBruBTazpdccokSExNVrVo13XLLLSF3UQW28ZQpU3TbbbepRo0aKl++vPr06RPxVvBo9q38npul0nc9279/v/7yl7+obt26io+P10knnaSuXbtma+/SjJ/0gFKsV69emjt3rtasWaMLL7ww2/T9+/ere/fuOu+88zRt2jRVrFhRW7Zs0ccffyxJGjZsmH766Se99NJL+uijjxQTExNS/ueff9bIkSN1yimn6MCBA5oxY4YuvPBCrVmzRmeeeWZI3hEjRqhPnz56/fXXtWHDBt15552KiYkJubgPGDBAc+fO1a233qquXbvqjz/+0IoVK7R9+3Y1bdpUv//+u84//3wdOnRIY8eOVf369fXOO+/opptu0uHDh/WXv/wlYjv07t1bH330kdq3b6/rr79ew4YNC/kFce/evRowYID+9re/6aGHHlK5cuX03//+V+3bt1fFihX1zDPPqHLlynr22WfVu3dvLViwQD179gxZRv/+/XXDDTfob3/7m6ZMmaLrrrtOGzdu1LJlyzRp0iSlp6drxIgRGjhwoD755JMct9m//vUv9erVSy1atAh+6Qj/lfvSSy/V0KFDNXLkSM2fP19jxoxRnTp1NHToUEnKdztl9dxzz+nhhx9WTEyM2rRpo3HjxumCCy4ITk9JSZFzLs/55NS+0dYxLS1NCQkJmjhxoqpXr67//ve/evTRR3X++edr/fr1SkhIkCS99957GjhwoHr37q1HH31Uu3bt0ogRI5Senq4mTZrkWr+MjAx1795d33zzje677z6dccYZWrVqlcaPH6+0tDQ9+uijIfmj2Zf/9Kc/ae3atXrooYd06qmnatasWVG1+5QpUzRo0CBlZmbqhRdekCRVqlRJkvTll1+qQ4cOatasWfCL2KRJk9ShQwetWrVKLVq0iDjP++67T7t27dLq1as1b948Scr2C3o06zRo0CDNnz9fd911l9q1a6dvv/1W9913n7Zs2aK33norz3WbMWOGmjRpoieffFJHjhzRHXfcoX79+mn9+vXBHsLnn39eN910k4YOHar7779f+/bt09ixY9WhQwd9+eWXqlixoiRfQHb55Zfr7rvvVpkyZbRixQoNGzZMhw4d0o033hiy3GnTpqlBgwZ65JFHVKFCBdWuXVsLFy5Uv3791Lt3b82YMUOSNHnyZF1wwQX68ssvVadOHf3www/q27evLr/8ct1///0qW7asNm7cqB9++CHqds3qyJEj6tatmw4dOqRnn31WNWrU0AsvvBDxNvbBgwfrjTfe0L333qv27dsrNTVVEyZM0A8//KDXX39dktS5c2ctWLAgWGbZsmWKj4/Xzz//rO+++06NGzfWgQMHtHr1ag0aNMjTtiiMdf/LX/6inj17avr06cEfG+6++249+uij+utf/6qHH35YP//8s0aPHq2vv/5aH3/8cfAas2XLFg0bNkwpKSnBxxH69OmjRYsWZTv3Tpw4UR07dtQrr7yib775RnfeeafKlCmj//znP8Fz8nPPPaehQ4eqVatWOv3003PcRgFXX321rrrqKr355pvKyMjI81oZSWpqqtq2bashQ4Zo+PDhkhQM8qPZ/0rSihUrtGnTJk2ePFlHjhzRrbfeqssuu0wNGjRQo0aNNHPmTK1YsUITJkxQw4YNgwH14cOHtW/fPo0ePVq1atVSWlqapkyZojZt2mj9+vWqWbNmyHIGDRqkK664QjfffLM+/fRTPfDAAzpw4EC2cRwmTpyoli1baurUqdq5c6fuvfdeXXTRRVq3bp3i4uIkRb9v5ffcHFCarmcjR47UvHnzguvy66+/auXKlVEHxqWCc45PMXzOOa2ec6tfjvxBVA4cOOAOHDgQeWJObVtcn3yaOnWqk+Q2btwYcfrixYudJDdz5kznnHObN292ktzUqVN9q716tZPk1q5dm+MyxowZ4yS59PT0XOuSkZHh0tPTXePGjd1f//rXYPrSpUudJHfttdeG5L/llltcfHy8O3r0qHPOuffff99Jck8++WSOy3jggQdcfHy8++6770LShw0b5qpVq5ZrHdPT050kN2bMmJD0wYMHO0lu7ty5Iem33367i4mJCWnbjIwM17hxY3fWWWcF0wLt88orrwTT0tLSXExMjKtatarbu3dvMP3JJ590ktyWLVtyrKdzztWrV89dffXV2dIDy3r55dB9pnnz5q5bt27BvwvSTs45N2jQIDdz5ky3YsUKN336dHfmmWe62NhYt3Tp0lzLRZJT++a3jhkZGW7btm1OkpszZ04wvV27du60005zmZmZwbRVq1Y5Sa5Dhw651vHVV191ktzy5ctD0idMmODi4uLcjh07nHPR78vvvvuuk+T++c9/huTr0aOHk5RnO3bo0MGdf/752dIvu+wyV7lyZbdnz55g2t69e11SUpK79NJLc53n4MGD3cknn5wtPdp1WrFiRbb93DnnZsyY4SS5//znP7kuX5Jr1KiRO3LkSDBt9uzZTpJbuXKlc865ffv2uUqVKrmhQ4eGlN28ebOLi4tzjz/+eMR5Z2ZmuvT0dDds2DB35plnZlturVq13MGDB0PSGzZs6Dp37hyStnfvXletWjU3YsSIkPplPYbD5dSukfz97393klxqampI3Zs1a+Ykuc2bNzvnnPvqq68inqvGjx8fcr6eM2dOyPlkxIgR7uKLL3aNGjVyzz//vHPOuX//+99Okvv2229D2iSvbVGQdQ/sU5dccklI+ubNm12ZMmXcuHHjQtI/+ugjJ8n961//iricwPbt1q2b69u3b8j8JLlOnTqF5L/00kudJDd9+vRgWuCcPHbs2BzXx7n/XVNvvfXWkPRorpWBsoHt6JyvrUeNGpUtbzT7nxdHjx516enpIZ969eq5++67LyQtIyMjz3nVq1fPJSUlud9++y2YFrh2XX/99SF5zzrrLNexY8cc55WRkeEOHDjgEhMT3WOPPRZMD7TV8OHDQ/JPmDDBlSlTxm3YsME5979tHH5uD+wz//jHP4L5otm3CnpuLm3Xs9NPP92NHDky1zqHy/W7sJ+kNa6Y4htubQVKMd/5QCG3o2Z16qmnqkqVKho+fLhmzJihH3/80dP833vvPXXq1EnVqlVTbGys4uLi9N1332nDhg3Z8oYP8HPGGWfo8OHD2rFjhyTp3XfflZnphhtuyHF5ixcvVuvWrVW/fn1lZGQEP927d9evv/6qb775xlP9A2JjY9WnT5+QtBUrVqhNmzYhz57GxMToqquu0hdffKHff/89JH/WX8mTkpJUo0YNtWnTJtibJElNmzaVJM/tHC68LZs3bx5y619B22n69Om68sordcEFF2jQoEH66KOPVLt2bY0ePTpf9Y3Uvl7q+Nxzz6lFixZKTExUbGys6tatK0nB/SwzM1OrV6/W5ZdfrjJl/ndZat26dZ63GgbqUq9ePbVr1y6kLhdddJHS09Oz3a6d176cmpqqmJgYXXbZZSH5BgwYkGddcrNixQr16dNHVapUCaZVqlRJffv21fLlyws077zWafHixSpbtqwuu+yybG0UqFteunXrFuw9CCxDUnDfTU1N1e+//66rr746ZBmnnHKKmjZtGrKMjRs36qqrrtLJJ5+suLg4xcXF6R//+EfEc0+PHj1Urly5kLKbNm3Ktpzy5curbdu2weW0bNlScXFxGjBggN58803t3LkzqrbMSWpqqurUqRPy7HGZMmVCbjuV/teW4b2Igb8D27pDhw4qU6ZMcDCXDz74QJ07d1bnzp1D0mrVqhU89wTktS0KY90vvfTSkL+XLFmio0ePZmv31q1bq1KlSiHb97PPPlOfPn100kknBa8tS5Ysibh9w3soA+vavXv3YFrgnBztuTe87gW9VmYV7f7nxfLly4PHQeCzdetWjR8/PiStS5cuUc2vbdu2qly5cvDvSG0aSA9vizfeeEOtW7dWlSpVFBsbqwoVKmj//v0Rt134vj9gwAAdPXo02+364ef2888/P3iLqRT9vlUY5+bSdD0799xzNW3aND300ENas2aNMjMzo16P0oJAEijFAif4rKPIZVW5cmUtXbpUtWvX1s0336y6deuqefPmUd2m9vnnn6tXr15KTEzUSy+9pFWrVmn16tVq0aJFxGemqlatGvJ34DaoQN5ff/1VVatWDfnCF27nzp1asWJFtgtm//79g/PIjxo1amS7bTctLS1iu9WsWVPOOe3ZsyckPSkpKeTvsmXLRkyTFNUzZbmJ1JZZ51nY7VSxYkX17t1bq1evzld9I7VvtHV8+umndfPNN6tr166aM2eOPv3002BgF1jn3bt3Kz09PeQ5rIBIaeF27typrVu3ZqvLeeedF1KXgLz25e3btyspKSnki3q0dclNbvtk+P7oVV7rtHPnTh05ckSJiYkhbVSjRg1J0e1T0SxDkrp27ZptW3z11VfBZezfv1/dunXT2rVrNWnSJH344YdavXq1rrvuuojPG4a3WWA5119/fbblLFiwILicRo0a6Z133tHRo0d1zTXXqGbNmmrdunW+g/bt27dHtY8GnukKr3fgtsDA9KpVq6pFixZaunSpdu/era+//lqdOnVSp06dgq8xWLp0qTp16pRtmXlti8JY95zavVGjRtna/ffffw+2+48//qguXbooLS1NTz/9tD7++GOtXr1aPXr0iHjuzOk8Gyk92nNveN0Lcq0MF+3+58U555yj1atXh3xq1aqlG264ISQtcLt8XvLbpvPnz9eVV16p0047Ta+//ro++eQTrV69WtWrV4/Y9uH7fuDv8GcGczpuAvmi3bcK49xcmq5nTz/9tIYPH66XX35Z5557rmrUqKGRI0cGx8U4FvCMJFCKLVy4UAkJCTrnnHNyzNOyZUu99dZbysjI0Jo1azRx4kRdccUVWrt2rZo3b55jubfeekuxsbGaM2dOyEl5z549IT0m0UpOTlZaWpoOHTqUYzBZrVo11ahRQ08++WTE6Xk9C5eTSD22VatW1S+//JIt/ZdffpGZZfsiVpoURTs553Ls2c5LpHLR1nHmzJnq0qVLyHOKmzdvDsmbnJysuLi4YO9ZVjt27FC9evVyrV+1atVUv359vfHGGxGnR9OrmVWtWrW0Z88epaenhxwbkernRW77ZFHvj9WqVVNCQoI+/PDDiNNr165dKMuQfM80RnqOLfB8ZGpqqrZu3aoPP/xQ7du3D07P6f2q4ftfYDkTJ05U165ds+UPfGmWFAzMDh8+rJUrV+r+++9X7969tWXLFiUnJ3tav1q1akUcXCh8vwhsy19++UUNGzYMpge2faD+gfrNmjVLS5cuVbVq1XTmmWeqVq1a2rlzp1auXKn//Oc/wefzvCrouufU7u+++262gCTr9MWLF2vv3r164403QgYOKs4vx5HOWfm9Vobzsv9Fq2LFimrVqlW2+dSuXTtbelGaOXOmGjVqFPKMY3p6erYBbwJ27NgRcqwHjoWTTz45W75IZVu2bCkp+n2rMM7Npel6lpiYqIkTJ2rixInaunWr3nzzTd19990qW7asJk+eHPU6lSQCSaCUmjNnjubNm6cRI0aofPnyeeaPjY1VmzZtNH78eM2bN0/ffvutmjdvHvyl+tChQ8EvcpLvoh4TExNyUv3ggw+0bds21a9f33N9L7roIk2aNEn/+Mc/cnzwvUePHnr66adVt27dYE9IUenQoYOeeOIJbdmyJRhIZGZmatasWTrrrLNC2qKwxcfHh4xc51Vht9Pvv/+uhQsXBkcvLAzR1vHgwYMhtwdLCo6IGxATE6Nzzz1Xb775psaOHRu8HeiTTz7Rli1b8gwke/ToobfeekuJiYnZbgHMj7Zt2yozM1NvvfVWyC1TM2fOjKp8fHy89u3bly29Q4cOWrhwofbt2xfc//bt26f58+fn+ZLqwtinJk+erL1790Z9e5xX7dq1U8WKFfX9999r8ODBOeYLBBThP2C9/fbbUS2nSZMmSklJ0bp163T33XdHVSY+Pl6dO3fW/v371a9fP23evFnJycme2rVt27aaOnWqVq1aFby99ejRo9l+wOjQoYMk3/4yatSoYPprr70mSSEDp3Xq1EmPPfaYXnjhBXXs2FFmpho1auj000/XmDFjlJmZmefrjopj3SXf7bRlypTRtm3b1K1btxzzRdq+3333nVauXJltRNqSkNO1MpKyZctma6P87H/HioMHD2Z7tc706dNzvOXyjTfeCNk/Z86cqTJlygTvBgkIP7evXLlSP/30k9q2bSsp+n2roOfmnJSG61m9evV0++2367XXXisVo/9Gi0ASKAW++OIL7d69W0eOHNG2bdu0YMECzZ49W926ddPEiRNzLLdgwQL9/e9/1yWXXKL69evrwIEDeuqpp1SxYsXgCbpZs2aSpEcffVQ9e/ZUTEyMWrVqpR49euiJJ57QkCFDNHToUH333XcaP358tl8So9WpUydddtlluu222/Tjjz+qc+fOSk9P14oVK9S7d2917NhRI0eO1KxZs3TBBRdo5MiRatKkiQ4cOKD169frww8/jPqLZDRGjhypadOmqVu3bho3bpwqVaqkKVOm6Lvvvss2DH1ha9asmT788EMtWLBANWvWVHJysqdesYK00yOPPKINGzaoU6dOql27trZu3apHHnlEv/zyS/CLbGGIto6BAOahhx7Seeedpw8++EBvvvlmtvmNGzdOF110kS655BINHz5cu3bt0pgxY7KNEhjJ1VdfralTp6pLly66/fbb1aJFCx05ckSbNm3SvHnzNHfu3Kh+jAno1q2b2rdvr+HDh2v37t3BkQGjvbg3a9ZMU6ZM0axZs9SwYUNVrFhRTZo00X333acFCxaoS5cuuuuuu2Rmmjx5sg4ePKj7778/z3mmpaXpueeeU6tWrZSQkBB8Li4aHTt21FVXXaXLL79ct912m8477zyVKVNGW7Zs0aJFizR58mQ1btw46vlFUqlSJT388MO65ZZbtGvXLvXs2VOVK1fWzz//rOXLl6tjx44aOHCg2rVrp0qVKumWW27RuHHjdODAAU2YMEHJycnau3dvnssxMz377LPq16+fjhw5oiuuuELJycnasWOHPv74Y9WtW1e33Xabnn/+ea1YsUK9evVSnTp1tHv3bk2cOFG1a9cOBg5e2nXw4MGaNGmS/vSnP+mhhx5SjRo19Pzzz2d73vr000/XVVddpbFjxyojI0Pt2rVTamqqxo8fr6uuuipkROwLL7xQMTExev/99/Xss88G0zt16qRnnnlGdevWVYMGDTxvi8Jed0lq2LCh7rrrLv35z3/Whg0b1KFDByUkJOjHH3/UkiVLNGzYMHXq1Eldu3ZVbGysrr32Wt1+++3avn27xowZo7p162Z7zVFxieZaGUmzZs20cOFC9ejRQ0lJSapdu7Zq164d1f4n+Xrnhw4dqqVLl+b5Y1Fp0KNHD82dO1cjR45Unz599Nlnn+mpp57K8S6lRYsW6Y477tBFF12kTz/9VOPGjdO1116b7Vyyb9++kHP7Pffco1NPPVXXXnutpOj3rYKem3NSUteztm3bqm/fvjrjjDOUmJio5cuXa+3atbn+EFfqFNeoPif6h1FbCy6akaqONYGRzwKfhIQEV7duXXfJJZe4N954IzjiYkD4qK3r1693V1xxhUtJSXHx8fEuOTnZ9ezZ061atSpYJiMjw918882uevXqzsyc77D3eeqpp1xKSopLSEhwrVq1ckuWLHEdOnQIGVUsMILfkiVLItY96wh36enpbsKECe7UU091cXFxwfqsX78+mCctLc3deuutLiUlxcXFxbnq1au79u3b5ziiY9Z5K4dRW3MadXH9+vWuX79+rlKlSi4+Pt61bt3a/fvf/w7Jk9OotpFGXs2pLcJ9++23rn379q5cuXJOkhs8eHCuyxo8eLCrV69eSFp+22nevHmuXbt2rlq1ai42NtZVrVrVXXzxxe6TTz7JtVxOcmvfaOp48OBBd+ONN7rk5GSXmJjoevfu7X744YeI2/L11193jRs3dmXLlnXNmjVzc+bMybY/5uTQoUNuzJgxrkmTJq5s2bIuKSnJtWrVyo0ZMybY3l725Z07d7oBAwa4xMREV7lyZXfNNde4uXPnRjUy4Pbt213Pnj1dYmJitlH6Vq1a5bp06eIqVKjgypcv7zp37hzVttm/f78bMGCAq1KlipMU3F+8rFNmZqZ74okn3Jlnnuni4+NdpUqV3JlnnunuuOOOkBEeI1GE0SvDz0cBCxcudB07dnQVK1Z0CQkJrmHDhm7o0KFu3bp1wTzvv/++a9mypUtISHANGjRwTz75ZPD4yGu5AR9//LHr3bu3q1KliouPj3f16tVzV155pfv444+D0/v27etOOeUUV7ZsWVezZk13+eWXh5yPcmrXnGzatMn17NnTlStXziUnJ7u//vWv7vnnn8/W1keOHHGjRo1ydevWdbGxsa5u3bpu1KhRISOtBpx33nnZRmYNjOgaOHfk1Sbh26Ig657Xee7VV191rVu3duXLl3cVKlRwTZs2dbfccov78ccfg3lmzZrlmjRp4uLj412zZs3cP//5z2znuUCdX3zxxZD5ezknh8tpJPRorpWRjpmPPvrInX322S4+Pj7bOSuv/c8555555hknyX3zzTe51juSevXqZTtHRlsu2mtX+Pk9MzPTjRo1ytWqVcuVK1fOXXjhhe7zzz939erVC9kXA221fPly17dvX1ehQgWXlJTkbr755pARlgPb+Nlnn3UjR450ycnJrly5cq5Xr17uhx9+yFb3aPatgpybS9v17M4773QtW7Z0lSpVcuXLl3fNmzfPdeR750rfqK3mWx6KWqtmKW7Nq2NymDi0eCtzjArcLuOlZwEAAKAkDBw4UL/99psWLVpU0lUpVIGe1o0bN4aMjB5uy5Ytql+/vl588UUNGzas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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5IAAAJyCAYAAAC2Qv8kAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAB+DElEQVR4nOzdeZyP9f7/8efLzJjBWIYhFMYSkqJSlpQ9a9QpJSmUflrOOVKnlUIUvu2b6nSKog4pR7ajVJbSKOqkUiRZqiNLI9liZrx/f3yWM5/PfGbmc82Ox/12+9yY9/V+X9f7el/b5/V5X9f7MuecAAAAAACIVpmSrgAAAAAA4NhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAAT2JLugIniuTkZJeSklLS1QAAAABwnPrss892O+eqF8eyCCSLSUpKitasWVPS1QAAAABwnDKzrcW1LG5tBQAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnjNqKY87Ro0d15MgRHT16tKSrAgAAABSpMmXKqGzZsipTpnT1AZau2gB5SE9P186dO5Wenl7SVQEAAACKXGn9/kuPJI4ZR48e1a+//qqTTjpJZlbS1QEAAACKRWJionbs2KEaNWqUmp7J0lELIApHjhxRhQoVCCIBAABwQjEzVahQoVT1ShJI4phx9OhRxcTElHQ1AAAAgGIXExOjzMzMkq5GEIEkAAAAAMATAkkAAAAAgCcEkgAAAAAATxi1FceF1z/ZVqLLH9i6br7KTZs2TUOHDg3+Xb58eVWvXl1nnXWWrrrqKl1++eUhI3Nt2bJF9evX19SpUzVkyJColrFs2TItW7ZM999/f6kZ5Su/UlNTdeutt+rrr7/WwYMH9Z///EctW7Ys6Wpl88QTT6hu3br605/+FJI+duxYjRs3Tunp6YqNLbrTb04DUmVtr8C+tHTpUnXs2LHI6lJQgbotW7asROsRqEOnTp3ybLNp06bp6NGjuu666wpt2XPnztUPP/yg2267LWKdlixZoq5duxba8k4UObVraXE8nb8LQ6RjMKfzLUqX/Hx/KQlDhgzRsmXLtGXLlpKuyjGBsxJQCsyePVupqalatGiRxo8fr/j4eF111VW66KKLdOjQoWC+WrVqKTU1Vb1794563suWLdO4ceN09OjRoqh6sbr++uuVkZGh+fPnKzU1VY0bNy7pKkX0xBNPaM6cOSVahyFDhig1NTXkU1rb63gzbdo0vfzyy4U6z7lz5+qxxx4r1Hmi9Lfr8XT+Lgxnn322UlNTdfbZZwfTSsP5FjhR0SMJlAItW7ZUo0aNgn9fc8016t+/v/r3768777xTTz/9tCQpPj5ebdq0KalqlqijR49qw4YNGjVqlDp37pxr3sOHDys+Pr6YalY6nXzyyUW2r9C+KCmZmZlyzhVpj/6xKnCnw7H4iqxozymVKlUqVdfAjh07KiUlRdOmTSvpqhzXuOaUXvRIAqXUZZddpn79+unFF1/UwYMHJfluDTGzkIvW6tWr1a1bN1WrVk3ly5dXgwYNdPPNN0v6362UkhQXFyczC/mSMWbMGJ199tmqXLmykpOT1blzZ61atSqkHsuWLZOZad68efrzn/+s5ORkVa9eXYMGDdJvv/0WkjcjI0OTJ09Ws2bNlJCQoOrVq6tHjx5av359MM/u3bt100036eSTT1Z8fLyaNm2qv//977m2xbRp0xQTE6OjR49q/PjxMjOlpKRI8vW8nXLKKUpNTVW7du1Urlw53XnnnZKkDRs26NJLL1WVKlVUrlw5tWnTRosXLw6Z99ixY2VmWr9+vbp3764KFSqobt26mjp1qiRp+vTpatq0qRITE9WpUydt2rQp17qmpKRo69ateu2114LtHX4bz+bNm9W7d28lJiaqXr16euCBB7L1OOSnnYpCbu0bTR137dql4cOHq3Hjxipfvrzq1KmjgQMH6ueff862rJkzZ6pp06aKj4/X6aefrn/9619R1/PgwYO66667VL9+fZUtW1b169fXgw8+GNKuXvblXbt2aeDAgapUqZKqVKmia6+9NlueSDp27Kjly5dr5cqVwe2f9TbYTz/9VF27dlViYqIqVKigLl266NNPP811nkOGDNErr7yin3/+OTjPwP6fdf2jOT4nTpwYbOPatWvr9ttv1x9//JHnepmZRo8eraeeekr169dXxYoV1aFDB61bty5b3jlz5qhNmzYqX768qlSpov79+2vbttDHD2bOnKnOnTurevXqSkxM1FlnnaVXXnkl4nJHjRqlSZMmBbftV199JUlavny5unTpoooVK6pChQrq3r27vv7665Dy77zzjtq1a6fKlSsrMTFRTZo00QMPPBB1u2YV2H/Cb7OeNm2azCzkVriUlBQNGjRIL774oho1aqSEhASdffbZWrp0aUjZ/J6/A9eCKVOm6M4771Tt2rUVHx8f3OaFvQ1Gjx6tRx99VPXq1VOFChXUu3dv7dy5Uzt37tQVV1yhypUrq06dOpo8eXKO7RfejnPmzNENN9yg6tWr66STTpIkfffdd7r00ktVo0YNJSQkqG7duurfv78yMjIiboO8zrdr165V3759lZSUpHLlyun888/Xhx9+mGcdi1rHjh3Vvn17LV68WC1btlS5cuV01lln6ZNPPlFGRobuvfde1apVS1WrVtWQIUN04MCBkPJert1vvfWWhgwZoqSkJFWqVElXX321fv3115C8gePswQcf1CmnnKJy5crpwgsv1BdffJGt7tHsWwcPHtTNN9+satWqKTExUX379tVPP/0UVdsErslff/21unfvrsTERF1xxRXB+eZ1nv/jjz80cuRINW/eXImJiapZs6YuvvjikO8hAe+//77OPvtsJSQkqGHDhnrhhRey5cnIyNB9992nhg0bKiEhQcnJyWrfvr0++uijqNbneMdPekAp1qtXL82dO1dr1qzRhRdemG36/v371b17d5133nmaNm2aKlasqC1btujjjz+WJA0bNkw//fSTXnrpJX300UfZ3sP5888/a+TIkTrllFN04MABzZgxQxdeeKHWrFmjM888MyTviBEj1KdPH73++uvasGGD7rzzTsXExIR88RgwYIDmzp2rW2+9VV27dtUff/yhFStWaPv27WratKl+//13nX/++Tp06JDGjh2r+vXr65133tFNN92kw4cP6y9/+UvEdujdu7c++ugjtW/fXtdff72GDRsW8uvk3r17NWDAAP3tb3/TQw89pHLlyum///2v2rdvr4oVK+qZZ55R5cqV9eyzz6p3795asGCBevbsGbKM/v3764YbbtDf/vY3TZkyRdddd502btyoZcuWadKkSUpPT9eIESM0cOBAffLJJzlus3/961/q1auXWrRoobFjx0qSqlevHpLn0ksv1dChQzVy5EjNnz9fY8aMUZ06dYLPy+a3nbJ67rnn9PDDDysmJkZt2rTRuHHjdMEFFwSnp6SkyDmX53xyat9o65iWlqaEhARNnDhR1atX13//+189+uijOv/887V+/XolJCRIkt577z0NHDhQvXv31qOPPqpdu3ZpxIgRSk9PV5MmTXKtX0ZGhrp3765vvvlG9913n8444wytWrVK48ePV1pamh599NGQ/NHsy3/605+0du1aPfTQQzr11FM1a9asqNp9ypQpGjRokDIzM4NfSipVqiRJ+vLLL9WhQwc1a9YsGHxMmjRJHTp00KpVq9SiRYuI87zvvvu0a9curV69WvPmzZOkbL/OR7NOgwYN0vz583XXXXepXbt2+vbbb3Xfffdpy5Yteuutt/JctxkzZqhJkyZ68skndeTIEd1xxx3q16+f1q9fH+whfP7553XTTTdp6NChuv/++7Vv3z6NHTtWHTp00JdffqmKFStKkn744Qddfvnluvvuu1WmTBmtWLFCw4YN06FDh3TjjTeGLHfatGlq0KCBHnnkEVWoUEG1a9fWwoUL1a9fP/Xu3VszZsyQJE2ePFkXXHCBvvzyS9WpU0c//PCD+vbtq8svv1z333+/ypYtq40bN+qHH36Iul0LYvny5frss8/04IMPKj4+XpMnT1bPnj21du1aNWnSpMDnb0l68MEHde655+rvf/+7MjMzlZCQUCTbYPr06WrevLmmTJmiHTt26NZbb9W1116rffv2qWfPnvp//+//afbs2br77rt1xhlnqFevXnm2z1/+8hf17NlT06dPD/6Y0adPH1WpUkXPPfeckpOT9fPPP2vRokU53tqb2/n2888/1wUXXKCzzjpLL774osqXL6/nn39eXbt21ccff6xzzjknug1ZRL7//nvdcccdGjVqlBITE3XnnXeqb9++6tu3rzIyMjRt2jR9++23uuOOO1SjRg393//9X7Csl2t34Hr8z3/+Uxs3btS9996r//73v9l+1Hj11VdVt25dPfPMMzp8+LDuv/9+denSRRs3blTVqlUlRX98Dx8+XLNmzdKYMWN07rnnasmSJRo4cKCn9unXr5+uv/563XXXXSpTpkzU5/nDhw9r3759Gj16tGrVqqW0tDRNmTJFbdq00fr161WzZk1J0rfffqtevXqpVatWmjlzpg4fPqyxY8dq//79Icfa5MmT9fjjj+vBBx9Uy5Yt9fvvv2vNmjVKS0vztD7HLeccn2L4nHPOOQ4Fc+DAAXfgwIGI015btbVEP/k1depUJ8lt3Lgx4vTFixc7SW7mzJnOOec2b97sJLmpU6c655xbvXq1k+TWrl2b4zLGjBnjJLn09PRc65KRkeHS09Nd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3jzYa3Do0KHgiV7yjX4WExMTcrL+4IMPtG3bNtWvX99zfS+66CJNmjRJ//jHP3IclKRHjx56+umnVbdu3WBPSFHp0KGDnnjiCW3ZsiV4gcnMzNSsWbN01llnhbRFYYuPjw95/6dXhd1Ov//+uxYuXKjWrVsXeF4B0dbx4MGDIbcHSwqOiBsQExOjc889V2+++abGjh0b/IL3ySefaMuWLXkGkj169NBbb72lxMTE4O1hBdG2bVtlZmbqrbfeCrkda+bMmVGVj4+P1759+7Kld+jQQQsXLtS+ffuC+9++ffs0f/78kJFdc5pnQfepyZMna+/everSpUu+55Obdu3aqWLFivr+++81ePDgHPMFRqEO/xL89ttvR7WcJk2aKCUlRevWrdPdd98dVZn4+Hh17txZ+/fvV79+/bR582YlJyd7atfAfvj1118HbwmWpEWLFkXMv2rVKv3444+qU6eOJN+2XrhwYcT3AHs9f+ekuLZBUTMztWzZUo899pheeuklff311zkGkpG2YYUKFXTBBRdo7dq1Ovvssz0HjaWZ12v3G2+8oeuuuy749+zZs3X06FG1bds2JN+iRYt04MCB4K2eW7Zs0apVq4LHWLT7VuvWrVWmTBm98cYbIcdntOfPnER7nj948GC21wNNnz492KMb0LZt22zr/OOPP2rlypU5/rBWs2ZNDRs2TIsWLco2QvSJikASKAW++OIL7d69W0eOHNG2bdu0YMECzZ49W926ddPEiRNzLLdgwQL9/e9/1yWXXKL69evrwIEDeuqpp1SxYsXgRaJZs2aSpEcffVQ9e/ZUTEyMWrVqpR49euiJJ57QkCFDNHToUH333XcaP358tl8po9WpUydddtlluu222/Tjjz+qc+fOSk9P14oVK9S7d2917NhRI0eO1KxZs3TBBRdo5MiRatKkiQ4cOKD169frww8/LNQvMSNHjtS0adPUrVs3jRs3TpUqVdKUKVP03XffaeHChYW2nEiaNWumDz/8UAsWLFDNmjWVnJzsqVesIO30yCOPaMOGDerUqZNq166trVu36pFHHtEvv/yi1157rRDWzlsdAwHMQw89pPPOO08ffPCB3nzzzWzzGzdunC666CJdcsklGj58uHbt2qUxY8YER9jLzdVXX62pU6eqS5cuuv3229WiRQsdOXJEmzZt0rx58zR37tyofowJ6Nat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9FN17dpViYmJqlChgrp06aJPP/0013kOGTJEr7zyin7++efgPAP7f9b1j+b4nDhxYrCNa9eurdtvv11//PFHnutlZho9erSeeuop1a9fXxUrVlSHDh20bt26bHnnzJmjNm3aqHz58qpSpYr69++vbdu2heSZOXOmOnfurOrVqysxMVFnnXWWXnnllYjLHTVqlCZNmhTctl999ZUkafny5erSpYsqVqyoChUqqHv37vr6669Dyr/zzjtq166dKleurMTERDVp0kQPPPBA1O0a7ocfflDv3r1Vvnx5Va9eXSNGjNDhw4ez5UtPT9fo0aOVkpKismXLKiUlRaNHj1Z6enowT/PmzTVs2LDg33v37lVMTIxOOeWUkHmdf/75uuKKK0LaJJptkd91Dxwnc+bM0Q033KDq1avrpJNOCs73xRdfVIsWLZSQkKDk5GRdf/31SktLC1n2M888o7Zt26pq1aqqUqWK2rRpo4ULF4bkCVzPnn/+ed1zzz2qWbOmKlasqEGDBungwYP6/vvv1b17dyUmJqpRo0YR949wgdtTV6xYof79+6tKlSpq3bq1pNyvlVnLBm5tDVwrH3zwwWAbZQ3qotn/SkJKSooGDRqk6dOnq0mTJipXrpwuuOACbdy4UQcOHNDw4cNVrVo1nXTSSbr99ttDHrX4448/NHLkSDVv3lyJiYmqWbOmLr744pBruBTazpdccokSExNVrVo13XLLLSF3UQW28ZQpU3TbbbepRo0aKl++vPr06RPxVvBo9q38npul0nc9279/v/7yl7+obt26io+P10knnaSuXbtma+/SjJ/0gFKsV69emjt3rtasWaMLL7ww2/T9+/ere/fuOu+88zRt2jRVrFhRW7Zs0ccffyxJGjZsmH766Se99NJL+uijjxQTExNS/ueff9bIkSN1yimn6MCBA5oxY4YuvPBCrVmzRmeeeWZI3hEjRqhPnz56/fXXtWHDBt15552KiYkJubgPGDBAc+fO1a233qquXbvqjz/+0IoVK7R9+3Y1bdpUv//+u84//3wdOnRIY8eOVf369fXOO+/opptu0uHDh/WXv/wlYjv07t1bH330kdq3b6/rr79ew4YNC/kFce/evRowYID+9re/6aGHHlK5cuX03//+V+3bt1fFihX1zDPPqHLlynr22WfVu3dvLViwQD179gxZRv/+/XXDDTfob3/7m6ZMmaLrrrtOGzdu1LJlyzRp0iSlp6drxIgRGjhwoD755JMct9m//vUv9erVSy1atAh+6Qj/lfvSSy/V0KFDNXLkSM2fP19jxoxRnTp1NHToUEnKdztl9dxzz+nhhx9WTEyM2rRpo3HjxumCCy4ITk9JSZFzLs/55NS+0dYxLS1NCQkJmjhxoqpXr67//ve/evTRR3X++edr/fr1SkhIkCS99957GjhwoHr37q1HH31Uu3bt0ogRI5Senq4mTZrkWr+MjAx1795d33zzje677z6dccYZWrVqlcaPH6+0tDQ9+uijIfmj2Zf/9Kc/ae3atXrooYd06qmnatasWVG1+5QpUzRo0CBlZmbqhRdekCRVqlRJkvTll1+qQ4cOatasWfCL2KRJk9ShQwetWrVKLVq0iDjP++67T7t27dLq1as1b948Scr2C3o06zRo0CDNnz9fd911l9q1a6dvv/1W9913n7Zs2aK33norz3WbMWOGmjRpoieffFJHjhzRHXfcoX79+mn9+vXBHsLnn39eN910k4YOHar7779f+/bt09ixY9WhQwd9+eWXqlixoiRfQHb55Zfr7rvvVpkyZbRixQoNGzZMhw4d0o033hiy3GnTpqlBgwZ65JFHVKFCBdWuXVsLFy5Uv3791Lt3b82YMUOSNHnyZF1wwQX68ssvVadOHf3www/q27evLr/8ct1///0qW7asNm7cqB9++CHqds3qyJEj6tatmw4dOqRnn31WNWrU0AsvvBDxNvbBgwfrjTfe0L333qv27dsrNTVVEyZM0A8//KDXX39dktS5c2ctWLAgWGbZsmWKj4/Xzz//rO+++06NGzfWgQMHtHr1ag0aNMjTtiiMdf/LX/6inj17avr06cEfG+6++249+uij+utf/6qHH35YP//8s0aPHq2vv/5aH3/8cfAas2XLFg0bNkwpKSnBxxH69OmjRYsWZTv3Tpw4UR07dtQrr7yib775RnfeeafKlCmj//znP8Fz8nPPPaehQ4eqVatWOv3003PcRgFXX321rrrqKr355pvKyMjI81oZSWpqqtq2bashQ4Zo+PDhkhQM8qPZ/0rSihUrtGnTJk2ePFlHjhzRrbfeqssuu0wNGjRQo0aNNHPmTK1YsUITJkxQw4YNgwH14cOHtW/fPo0ePVq1atVSWlqapkyZojZt2mj9+vWqWbNmyHIGDRqkK664QjfffLM+/fRTPfDAAzpw4EC2cRwmTpyoli1baurUqdq5c6fuvfdeXXTRRVq3bp3i4uIkRb9v5ffcHFCarmcjR47UvHnzguvy66+/auXKlVEHxqWCc45PMXzOOa2ec6tfjvxBVA4cOOAOHDgQeWJObVtcn3yaOnWqk+Q2btwYcfrixYudJDdz5kznnHObN292ktzUqVN9q716tZPk1q5dm+MyxowZ4yS59PT0XOuSkZHh0tPTXePGjd1f//rXYPrSpUudJHfttdeG5L/llltcfHy8O3r0qHPOuffff99Jck8++WSOy3jggQdcfHy8++6770LShw0b5qpVq5ZrHdPT050kN2bMmJD0wYMHO0lu7ty5Iem33367i4mJCWnbjIwM17hxY3fWWWcF0wLt88orrwTT0tLSXExMjKtatarbu3dvMP3JJ590ktyWLVtyrKdzztWrV89dffXV2dIDy3r55dB9pnnz5q5bt27BvwvSTs45N2jQIDdz5ky3YsUKN336dHfmmWe62NhYt3Tp0lzLRZJT++a3jhkZGW7btm1OkpszZ04wvV27du60005zmZmZwbRVq1Y5Sa5Dhw651vHVV191ktzy5ctD0idMmODi4uLcjh07nHPR78vvvvuuk+T++c9/huTr0aOHk5RnO3bo0MGdf/752dIvu+wyV7lyZbdnz55g2t69e11SUpK79NJLc53n4MGD3cknn5wtPdp1WrFiRbb93DnnZsyY4SS5//znP7kuX5Jr1KiRO3LkSDBt9uzZTpJbuXKlc865ffv2uUqVKrmhQ4eGlN28ebOLi4tzjz/+eMR5Z2ZmuvT0dDds2DB35plnZlturVq13MGDB0PSGzZs6Dp37hyStnfvXletWjU3YsSIkPplPYbD5dSukfz97393klxqampI3Zs1a+Ykuc2bNzvnnPvqq68inqvGjx8fcr6eM2dOyPlkxIgR7uKLL3aNGjVyzz//vHPOuX//+99Okvv2229D2iSvbVGQdQ/sU5dccklI+ubNm12ZMmXcuHHjQtI/+ugjJ8n961//iricwPbt1q2b69u3b8j8JLlOnTqF5L/00kudJDd9+vRgWuCcPHbs2BzXx7n/XVNvvfXWkPRorpWBsoHt6JyvrUeNGpUtbzT7nxdHjx516enpIZ969eq5++67LyQtIyMjz3nVq1fPJSUlud9++y2YFrh2XX/99SF5zzrrLNexY8cc55WRkeEOHDjgEhMT3WOPPRZMD7TV8OHDQ/JPmDDBlSlTxm3YsME5979tHH5uD+wz//jHP4L5otm3CnpuLm3Xs9NPP92NHDky1zqHy/W7sJ+kNa6Y4htubQVKMd/5QCG3o2Z16qmnqkqVKho+fLhmzJihH3/80dP833vvPXXq1EnVqlVTbGys4uLi9N1332nDhg3Z8oYP8HPGGWfo8OHD2rFjhyTp3XfflZnphhtuyHF5ixcvVuvWrVW/fn1lZGQEP927d9evv/6qb775xlP9A2JjY9WnT5+QtBUrVqhNmzYhz57GxMToqquu0hdffKHff/89JH/WX8mTkpJUo0YNtWnTJtibJElNmzaVJM/tHC68LZs3bx5y619B22n69Om68sordcEFF2jQoEH66KOPVLt2bY0ePTpf9Y3Uvl7q+Nxzz6lFixZKTExUbGys6tatK0nB/SwzM1OrV6/W5ZdfrjJl/ndZat26dZ63GgbqUq9ePbVr1y6kLhdddJHS09Oz3a6d176cmpqqmJgYXXbZZSH5BgwYkGddcrNixQr16dNHVapUCaZVqlRJffv21fLlyws077zWafHixSpbtqwuu+yybG0UqFteunXrFuw9CCxDUnDfTU1N1e+//66rr746ZBmnnHKKmjZtGrKMjRs36qqrrtLJJ5+suLg4xcXF6R//+EfEc0+PHj1Urly5kLKbNm3Ktpzy5curbdu2weW0bNlScXFxGjBggN58803t3LkzqrbMSWpqqurUqRPy7HGZMmVCbjuV/teW4b2Igb8D27pDhw4qU6ZMcDCXDz74QJ07d1bnzp1D0mrVqhU89wTktS0KY90vvfTSkL+XLFmio0ePZmv31q1bq1KlSiHb97PPPlOfPn100kknBa8tS5Ysibh9w3soA+vavXv3YFrgnBztuTe87gW9VmYV7f7nxfLly4PHQeCzdetWjR8/PiStS5cuUc2vbdu2qly5cvDvSG0aSA9vizfeeEOtW7dWlSpVFBsbqwoVKmj//v0Rt134vj9gwAAdPXo02+364ef2888/P3iLqRT9vlUY5+bSdD0799xzNW3aND300ENas2aNMjMzo16P0oJAEijFAif4rKPIZVW5cmUtXbpUtWvX1s0336y6deuqefPmUd2m9vnnn6tXr15KTEzUSy+9pFWrVmn16tVq0aJFxGemqlatGvJ34DaoQN5ff/1VVatWDfnCF27nzp1asWJFtgtm//79g/PIjxo1amS7bTctLS1iu9WsWVPOOe3ZsyckPSkpKeTvsmXLRkyTFNUzZbmJ1JZZ51nY7VSxYkX17t1bq1evzld9I7VvtHV8+umndfPNN6tr166aM2eOPv3002BgF1jn3bt3Kz09PeQ5rIBIaeF27typrVu3ZqvLeeedF1KXgLz25e3btyspKSnki3q0dclNbvtk+P7oVV7rtHPnTh05ckSJiYkhbVSjRg1J0e1T0SxDkrp27ZptW3z11VfBZezfv1/dunXT2rVrNWnSJH344YdavXq1rrvuuojPG4a3WWA5119/fbblLFiwILicRo0a6Z133tHRo0d1zTXXqGbNmmrdunW+g/bt27dHtY8GnukKr3fgtsDA9KpVq6pFixZaunSpdu/era+//lqdOnVSp06dgq8xWLp0qTp16pRtmXlti8JY95zavVGjRtna/ffffw+2+48//qguXbooLS1NTz/9tD7++GOtXr1aPXr0iHjuzOk8Gyk92nNveN0Lcq0MF+3+58U555yj1atXh3xq1aqlG264ISQtcLt8XvLbpvPnz9eVV16p0047Ta+//ro++eQTrV69WtWrV4/Y9uH7fuDv8GcGczpuAvmi3bcK49xcmq5nTz/9tIYPH66XX35Z5557rmrUqKGRI0cGx8U4FvCMJFCKLVy4UAkJCTrnnHNyzNOyZUu99dZbysjI0Jo1azRx4kRdccUVWrt2rZo3b55jubfeekuxsbGaM2dOyEl5z549IT0m0UpOTlZaWpoOHTqUYzBZrVo11ahRQ08++WTE6Xk9C5eTSD22VatW1S+//JIt/ZdffpGZZfsiVpoURTs553Ls2c5LpHLR1nHmzJnq0qVLyHOKmzdvDsmbnJysuLi4YO9ZVjt27FC9evVyrV+1atVUv359vfHGGxGnR9OrmVWtWrW0Z88epaenhxwbkernRW77ZFHvj9WqVVNCQoI+/PDDiNNr165dKMuQfM80RnqOLfB8ZGpqqrZu3aoPP/xQ7du3D07P6f2q4ftfYDkTJ05U165ds+UPfGmWFAzMDh8+rJUrV+r+++9X7969tWXLFiUnJ3tav1q1akUcXCh8vwhsy19++UUNGzYMpge2faD+gfrNmjVLS5cuVbVq1XTmmWeqVq1a2rlzp1auXKn//Oc/wefzvCrouufU7u+++262gCTr9MWLF2vv3r164403QgYOKs4vx5HOWfm9Vobzsv9Fq2LFimrVqlW2+dSuXTtbelGaOXOmGjVqFPKMY3p6erYBbwJ27NgRcqwHjoWTTz45W75IZVu2bCkp+n2rMM7Npel6lpiYqIkTJ2rixInaunWr3nzzTd19990qW7asJk+eHPU6lSQCSaCUmjNnjubNm6cRI0aofPnyeeaPjY1VmzZtNH78eM2bN0/ffvutmjdvHvyl+tChQ8EvcpLvoh4TExNyUv3ggw+0bds21a9f33N9L7roIk2aNEn/+Mc/cnzwvUePHnr66adVt27dYE9IUenQoYOeeOIJbdmyJRhIZGZmatasWTrrrLNC2qKwxcfHh4xc51Vht9Pvv/+uhQsXBkcvLAzR1vHgwYMhtwdLCo6IGxATE6Nzzz1Xb775psaOHRu8HeiTTz7Rli1b8gwke/ToobfeekuJiYnZbgHMj7Zt2yozM1NvvfVWyC1TM2fOjKp8fHy89u3bly29Q4cOWrhwofbt2xfc//bt26f58+fn+ZLqwtinJk+erL1790Z9e5xX7dq1U8WKFfX9999r8ODBOeYLBBThP2C9/fbbUS2nSZMmSklJ0bp163T33XdHVSY+Pl6dO3fW/v371a9fP23evFnJycme2rVt27aaOnWqVq1aFby99ejRo9l+wOjQoYMk3/4yatSoYPprr70mSSEDp3Xq1EmPPfaYXnjhBXXs2FFmpho1auj000/XmDFjlJmZmefrjopj3SXf7bRlypTRtm3b1K1btxzzRdq+3333nVauXJltRNqSkNO1MpKyZctma6P87H/HioMHD2Z7tc706dNzvOXyjTfeCNk/Z86cqTJlygTvBgkIP7evXLlSP/30k9q2bSsp+n2roOfmnJSG61m9evV0++2367XXXisVo/9Gi0ASKAW++OIL7d69W0eOHNG2bdu0YMECzZ49W926ddPEiRNzLLdgwQL9/e9/1yWXXKL69evrwIEDeuqpp1SxYsXgCbpZs2aSpEcffVQ9e/ZUTEyMWrVqpR49euiJJ57QkCFDNHToUH333XcaP358tl8So9WpUydddtlluu222/Tjjz+qc+fOSk9P14oVK9S7d2917NhRI0eO1KxZs3TBBRdo5MiRatKkiQ4cOKD169frww8/jPqLZDRGjhypadOmqVu3bho3bpwqVaqkKVOm6Lvvvss2DH1ha9asmT788EMtWLBANWvWVHJysqdesYK00yOPPKINGzaoU6dOql27trZu3apHHnlEv/zyS/CLbGGIto6BAOahhx7Seeedpw8++EBvvvlmtvmNGzdOF110kS655BINHz5cu3bt0pgxY7KNEhjJ1VdfralTp6pLly66/fbb1aJFCx05ckSbNm3SvHnzNHfu3Kh+jAno1q2b2rdvr+HDh2v37t3BkQGjvbg3a9ZMU6ZM0axZs9SwYUNVrFhRTZo00X333acFCxaoS5cuuuuuu2Rmmjx5sg4ePKj7778/z3mmpaXpueeeU6tWrZSQkBB8Li4aHTt21FVXXaXLL79ct912m8477zyVKVNGW7Zs0aJFizR58mQ1btw46vlFUqlSJT388MO65ZZbtGvXLvXs2VOVK1fWzz//rOXLl6tjx44aOHCg2rVrp0qVKumWW27RuHHjdODAAU2YMEHJycnau3dvnssxMz377LPq16+fjhw5oiuuuELJycnasWOHPv74Y9WtW1e33Xabnn/+ea1YsUK9evVSnTp1tHv3bk2cOFG1a9cOBg5e2nXw4MGaNGmS/vSnP+mhhx5SjRo19Pzzz2d73vr000/XVVddpbFjxyojI0Pt2rVTamqqxo8fr6uuuipkROwLL7xQMTExev/99/Xss88G0zt16qRnnnlGdevWVYMGDTxvi8Jed0lq2LCh7rrrLv35z3/Whg0b1KFDByUkJOjHH3/UkiVLNGzYMHXq1Eldu3ZVbGysrr32Wt1+++3avn27xowZo7p162Z7zVFxieZaGUmzZs20cOFC9ejRQ0lJSapdu7Zq164d1f4n+Xrnhw4dqqVLl+b5Y1Fp0KNHD82dO1cjR45Unz599Nlnn+mpp57K8S6lRYsW6Y477tBFF12kTz/9VOPGjdO1116b7Vyyb9++kHP7Pffco1NPPVXXXnutpOj3rYKem3NSUteztm3bqm/fvjrjjDOUmJio5cuXa+3atbn+EFfqFNeoPif6h1FbCy6akaqONYGRzwKfhIQEV7duXXfJJZe4N954IzjiYkD4qK3r1693V1xxhUtJSXHx8fEuOTnZ9ezZ061atSpYJiMjw918882uevXqzsyc77D3eeqpp1xKSopLSEhwrVq1ckuWLHEdOnQIGVUsMILfkiVLItY96wh36enpbsKECe7UU091cXFxwfqsX78+mCctLc3deuutLiUlxcXFxbnq1au79u3b5ziiY9Z5K4dRW3MadXH9+vWuX79+rlKlSi4+Pt61bt3a/fvf/w7Jk9OotpFGXs2pLcJ9++23rn379q5cuXJOkhs8eHCuyxo8eLCrV69eSFp+22nevHmuXbt2rlq1ai42NtZVrVrVXXzxxe6TTz7JtVxOcmvfaOp48OBBd+ONN7rk5GSXmJjoevfu7X744YeI2/L11193jRs3dmXLlnXNmjVzc+bMybY/5uTQoUNuzJgxrkmTJq5s2bIuKSnJtWrVyo0ZMybY3l725Z07d7oBAwa4xMREV7lyZXfNNde4uXPnRjUy4Pbt213Pnj1dYmJitlH6Vq1a5bp06eIqVKjgypcv7zp37hzVttm/f78bMGCAq1KlipMU3F+8rFNmZqZ74okn3Jlnnuni4+NdpUqV3JlnnunuuOOOkBEeI1GE0SvDz0cBCxcudB07dnQVK1Z0CQkJrmHDhm7o0KFu3bp1wTzvv/++a9mypUtISHANGjRwTz75ZPD4yGu5AR9//LHr3bu3q1KliouPj3f16tVzV155pfv444+D0/v27etOOeUUV7ZsWVezZk13+eWXh5yPcmrXnGzatMn17NnTlStXziUnJ7u//vWv7vnnn8/W1keOHHGjRo1ydevWdbGxsa5u3bpu1KhRISOtBpx33nnZRmYNjOgaOHfk1Sbh26Ig657Xee7VV191rVu3duXLl3cVKlRwTZs2dbfccov78ccfg3lmzZrlmjRp4uLj412zZs3cP//5z2znuUCdX3zxxZD5ezknh8tpJPRorpWRjpmPPvrInX322S4+Pj7bOSuv/c8555555hknyX3zzTe51juSevXqZTtHRlsu2mtX+Pk9MzPTjRo1ytWqVcuVK1fOXXjhhe7zzz939erVC9kXA221fPly17dvX1ehQgWXlJTkbr755pARlgPb+Nlnn3UjR450ycnJrly5cq5Xr17uhx9+yFb3aPatgpybS9v17M4773QtW7Z0lSpVcuXLl3fNmzfPdeR750rfqK3mWx6KWqtmKW7Nq2NymDi0eCtzjArcLuOlZwEAAKAkDBw4UL/99psWLVpU0lUpVIGe1o0bN4aMjB5uy5Ytql+/vl588UUNGzasGGt4/Irmu7CZfeacK5aHa7m1FQAAAChkK1asyHEQMOB4QCAJAAAAFLKffvqppKsAFKkSfY+kmdUxszfNbK+Z/W5mc8ysbpRlE8zsYTPbbmaHzCzVzC6MkK+Mmd1jZlvM7A8zW2tml0XIt8zMXITPrYWwqgAAAMAxb8iQIXLO5Xpbq+R79ZJzjttaj2Ml1iNpZuUlfSDpsKTB8g02MkHSUjM70zl3II9ZvCSpt6Q7JP0g6RZJ75hZW+fcF1nyjZf0N0mjJH0maYCk2WbWxzkXftP6l5LCX9i0xeOqAQAAAMBxrSRvbb1BUgNJTZxz30uSmX0paaN8wdxjORU0sxaSBkq6zjk31Z+2XNI6SQ9I6utPqyFfEDnJOfeIv/hSM2skaZKk8EByn3NuVeGsHgpbmTJlcnxhNQAAAHA8y8zMDHlHa0kryVtb+0paFQgiJck5t1nSSkn9oiibLmlWlrIZkmZK6m5m8f7k7pLKSpoRVn6GpDPMzPtb11FiYmNjdeTIkZKuBgAAAFDs0tPTFRtbeoa4KclA8nRJkd4guk5SsyjKbnbOHYxQtqykRlnyHZb0fYR8irCcs/zPa6ab2Zdmdn0e9ciVmX0W+BRkPvCJjY1VRkZGib3QGAAAACgJR48eVUZGRqkKJEuyJlUl7YmQniYpqQBlA9MD//7msr8sMzyfJK2Q9Jqk7yRVkXStpH+YWS3n3IQ86oNikpSUpF27dql8+fKKiYkp6eoAAAAARSozM1MHDx5U1apV885cjEo6pA0P8CTJoihnUZaNNp+cc/eHJb1tZv+SNMrMnnDO7Y+iXuHzPCfw/1bNUiLVAx7FxcWpRo0aOnz4MD2TAAAAOO4Fvv+aRRMmFZ+SDCT3KLRHMCBJkXsbs0qTFOk1IUlZpgf+TTIzC+uVDM+Xk39KukTSGZJS88iLYmJmSkhIKOlqAAAAACesknxGcp18zzCGaybpmyjK1ve/QiS87BH975nIdZLiJTWMkE9RLCcQ9tObCAAAAAB+JRlIzpPUxswaBBLMLEXS+f5peZWNk9Q/S9lYSVdKetc5d9ifvFi+wPLqsPKDJH3tHyU2NwMlHZL0VR75AAAAAOCEUZK3tr4o6c/yPYs4Wr5ev/GSfpT0QiCTmdWTtEnSA865ByTJOfeFmc2S9ISZxUnaLOkmSfWVJWh0zu00s8cl3WNm+yR9Ll+w2VlZXjFiZhdIulvSHElbJFWWNFi+14zc7Zw7UBQNAAAAAADHohILJJ1zB8yss6THJU2X7zbS9yXdGjawjUmKUfbe06GSHpQ0Qb5RVtdK6uGc+zws3yhJ+yWNkFRT0gZJVzjn5mfJs90//wckJcv3jsovJQ10zv2zYGsKAAAAAMcXy/5mDBSFVs1S3JpXx+QwcWjxVgYAAADAccfMPnPOtSqOZZXkM5IAAAAAgGMQgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhSooGkmdUxszfNbK+Z/W5mc8ysbpRlE8zsYTPbbmaHzCzVzC6MkK+Mmd1jZlvM7A8zW2tml+Ux73ZmdtTMnJnF5nf9AAAAAOB4VGKBpJmVl/SBpKaSBku6RtKpkpaaWYUoZvGSpBsk3S+pj6Ttkt4xs5Zh+cZLGivpGUk9Ja2SNNvMeuVQrzhJL0ja4W2NAAAAAODEUJK9bTdIaiCpiXPue0kysy8lbZQ0XNJjORU0sxaSBkq6zjk31Z+2XNI6SQ9I6utPqyHpb5ImOece8RdfamaNJE2StCjC7O+QZJJelnRvAdcRAAAAAI47JXlra19JqwJBpCQ55zZLWimpXxRl0yXNylI2Q9JMSd3NLN6f3F1SWUkzwsrPkHSGmdXPmmhmDSWNknSzf/4AAAAAgDAlGUieLunrCOnrJDWLouxm59zBCGXLSmqUJd9hSd9HyKcIy3lO0pvOuRV5LB8AAAAATlgleWtrVUl7IqSnSUoqQNnA9MC/vznnXB75ZGaDJLWS75nNQmFmnwX+f85p9QprtgAAAABQokr69R/hAZ7kez4xLxZl2ajymVlVSY9Kutc5tzOK5QMAAADACaskA8k9ytIjmEWSIvc2ZpWWS9nA9MC/SWYWHmCG55sg3yitb5hZFTOrIinBP61ylKPIZuOcOyfwyU95AAAAACiNSjKQXCffM4zhmkn6Joqy9f2vEAkve0T/eyZynaR4SQ0j5FOW5TSTdIakX+ULYvdIuss/bbek1/KoDwAAAACcMEoykJwnqY2ZNQgkmFmKpPP90/IqGyepf5aysZKulPSuc+6wP3mxfIHl1WHlB0n62j9KrCTdKqlT2OcV/7SukkZ7WC8AAAAAOK6V5GA7L0r6s6S3zWy0fM8yjpf0o6QXApnMrJ6kTZIecM49IEnOuS/MbJakJ8wsTtJmSTdJqq8sQaNzbqeZPS7pHjPbJ+lz+YLNzsryihHn3BfhlTOzjv7/Lve/WgQAAAAAoBIMJJ1zB8yss6THJU2XbwCc9yXd6pzbnyWrSYpR9t7ToZIelO/5xiqS1krq4Zz7PCzfKEn7JY2QVFPSBklXOOfmF+oKAQAAAMAJwrK/GQNFoVWzFLfm1TE5TBxavJUBAAAAcNwxs8+cc62KY1kl/foPAAAAAMAxhkASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHgSW9IVQCFYMzX36a2GFk89AAAAAJwQ6JEEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOBJbElXAMVgzdTcp7caWjz1AAAAAHBcoEcSAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ4QSAIAAAAAPCGQBAAAAAB4wnskjwV5vQcSAAAAAIoRPZIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADyJLekKoBRYMzX36a2GFk89AAAAABwT6JEEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOCJ50DSzKoWRUUAAAAAAMeG2HyU2W5mb0t6WdI7zjlXyHVCabNmau7TWw0tnnoAAAAAKBXyc2vrDEndJS2UtM3MJphZo8KtFgAAAACgtPIcSDrnrpdUU9JQSd9LukfSBjNbbmaDzax8tPMyszpm9qaZ7TWz381sjpnVjbJsgpk9bGbbzeyQmaWa2YUR8pUxs3vMbIuZ/WFma83ssgj5pprZt/567Pfn+4uZxUS7PgAAAABwIsjXYDvOuUPOuVedc50kNZQ0QVJd+W533W5mL5pZ29zm4Q84P5DUVNJgSddIOlXSUjOrEEU1XpJ0g6T7JfWRtF3SO2bWMizfeEljJT0jqaekVZJmm1mvsHzlJD0tqb+kP0l6T9KTkh6Loi4AAAAAcMKwwnrE0cwqSnpO0kB/kpO0XtIk59z0CPlHyBekNXHOfe9Pqy9po6Q7nXM5BnBm1kLSF5Kuc85N9afFSlonaYNzrq8/rYakH/11GJOl/PuSqjvnzsxjnf4pqY9zrmLeLZC7Vs1S3JpXx+QwMY9nDPN6RrGk8YwkAAAAUOLM7DPnXKviWFaBX/9hZh3MbKqk/8oXRH4h6S+SbpGUIWmamU2MULSvpFWBIFKSnHObJa2U1C+PxfaVlC5pVpayGZJmSupuZvH+5O6Sysr3XGdWMySd4Q9cc/Orfx0AAAAAAH75CiTNrJ6Z3W9mm+S7PfUSSdMlneucO9s596xz7nnnXAtJ0+S7BTXc6ZK+jpC+TlKzPKpwuqTNzrmDEcqWldQoS77D8j3LGZ5P4csxn1gzq+J/jnKwuLUVAAAAAEJ4fv2H/7bQDvIFoR9JGidptnPuUA5F3pNvYJ5wVSXtiZCeJikpj2rkVjYwPfDvbxFeURKeL6C3pPn+/zv5bokdn0ddcmRmnwX+f85p9fI7GwAAAAAoVfLzHsnm8vXS/cM5910U+d+T1CmHaZEe0LQo5mlRlo02X8CHks6VVFlSF0l/MzPnnBsVRZ0AAAAA4ISQn0CytnMuM9rMzrldkpZHmLRH2XsEJV9vZKTexqzS5BslNlLZwPTAv0nmjwZzyReo615Ja/x/vm9mRyTdZ2ZTnHM/51GnbJxz5wT+36pZSuGMagQAAAAAJSw/z0geMbOrcppoZleaWTSB5jr5nmEM10zSN1GUrR/hnZXNJB3R/56JXCcpXr5XlITnUxTLWSNfG+U1KA8AAAAAnDDyE0iacr/9NJpbUyVpnqQ2ZtYgWNAsRdL5/ml5lY2T752PgbKxkq6U9K5z7rA/ebF8geXVYeUHSfraP0psbjrId2vsD3nkAwAAAIATRn5ubZUiP3cY0ETS3ijm8aKkP0t628xG++c5Xr73Pr4QyGRm9SRtkvSAc+4BSXLOfWFmsyQ9YWZxkjZLukm+nsNg0Oic22lmj0u6x8z2SfpcvmCzs7K8YsTMess3INB8SdskVZTUU9L/k/SCc+6/UawPAAAAAJwQogokzWywfK/CCBhtZpFe6ZEk6Qzl3aMo59wBM+ss6XH5Xh1ikt6XdKtzbn/WxUuKUfbe06GSHpQ0QVIVSWsl9XDOfR6Wb5Sk/ZJGSKopaYOkK5xz87Pk2eSf/wRJNST9JmmjpGsl/TOvdQEAAACAE0m0PZJV9L/nBJ2k6pLCn0908gVsUyWNjmamzrltki7LI88WRbhd1v+6kdv8n9zKZ8oXIE7IJc96SX/Ku8YAAAAAgKgCSefck5KelCQzOypfr+HrRVkxAAAAAEDp5PkZSedcfgboAQAAAAAcJwgKAQAAAACe5NkjaWabJR2V1NQ5l25m0bwKwznnwt/dCAAAAAA4DkRza+tW+QbSCbzyY5tyf/0HAAAAAOA4lmcg6ZzrmNvfAAAAAIATC89IAgAAAAA88RxImlmKmXUMSzvLzGab2QdmNrSwKgcAAAAAKH08v/5D0iOSkiV1lCQzqyppiaRKkg5J6mBme5xzcwupjijt1kzNfXorflsAAAAAjif5ubX1XEnvZfn7SkmVJZ0tX4C5StKtBa4ZAAAAAKBUyk8gWUPSz1n+7i7pQ+fc1865dEn/lNSsMCoHAAAAACh98hNI7pNURZLMrIykCyUtzzL9iKTEAtcMAAAAAFAq5SeQXCvpGjOrJul6+W5rXZxlen1JOwqhbgAAAACAUig/g+2Mly9w3On/e6lz7pMs0/tI+rSgFQMAAAAAlE6eA0nn3AozO1vSRZJ+kzQzMM0/gut7kuYWUv0AAAAAAKVMfnok5ZxbL2l9hPQ0SSMLWikAAAAAQOmVn2ckAQAAAAAnsHwFkmZ2tZl9bGY7zSwzwiejsCsKAAAAACgdPN/aamb3yjfgzm5JqZLSCrtSAAAAAIDSKz/PSN4kaaWki5xzfxRyfQAAAAAApVx+bm1NlvQ6QSQAAAAAnJjyE0h+Lemkwq4IAAAAAODYkJ9A8j5JN5pZg8KuDAAAAACg9MvPM5KdJf0k6WszWyRpq6TMsDzOOXdXQSsHAAAAACh98hNI/i3L//+UQx4niUASAAAAAI5D+Qkk6xd6LQAAAAAAxwzPgaRzbmtRVAQAAAAAcGzIT4+kJMnMEiW1lVRD0nvOuR2FVisAAAAAQKmVn1FbZWa3SvqvpMWSXpV0uj+9upntN7NhhVZDAAAAAECp4rlH0swGSXpM0juSFkp6KjDNObfLzN6RdJmkfxRWJY97a6aWdA0AAAAAIGr56ZG8TdL7zrmekv4ZYfpn8vdQAgAAAACOP/l5RvI0SbfnMn2HfM9NAj559bi2Glo89QAAAABQKPLTI3lIUkIu01Mk/ZafygAAAAAASr/8BJKrJPWPNME/kusQSSsKUCcAAAAAQCmWn0DyQUnnmNk8SV38aaeZ2TWSPpVUXdLEQqofAAAAAKCU8fyMpHNupZldIenvkvr4k5+SZJLSJF3hnPtP4VURAAAAAFCa5GewHTnn5prZYkndJDWVr2dzo6R3nHMHCrF+AAAAAIBSJj/vkSwvqb2kxpIqSton6TtJHznnDhZu9QAAAAAApY2nQNLM7pF0l3wBpPmTnf/ffWY22TnH85EAAAAAcByLOpA0s6ck/VnSXkmvSPpSvt7IipJaSLpE0gQzq+mcG1H4VQUAAAAAlAZRBZJmdo58QeQS+QbT2Rshz62SZkn6s5m96pz7rDArCgAAAAAoHaJ9/cdQSXsk9Y8UREqSP/0Kf74hhVI7AAAAAECpE20g2VbSW86533PL5J/+lqR2Ba0YAAAAAKB0ijaQrCdpbZR5v5SUkq/aAAAAAABKvWgDycqSfosy7175BuABAAAAAByHog0kY/S/13zkxfnzAwAAAACOQ17eI9nNzKpEke+8fNYFJ6o1U3Of3mpo8dQDAAAAQFS8BJKD/Z9oRNt7CQAAAAA4xkQbSHYq0loAAAAAAI4ZUQWSzrnlRV0RAAAAAMCxIdrBdgAAAAAAkEQgCQAAAADwiEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPon2PJFBy1kzNfXqrocVTDwAAAACS6JEEAAAAAHhEIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJwSSAAAAAABPCCQBAAAAAJ7ElnQFgAJbMzX36a2GFk89AAAAgBMEPZIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCexJV2BE8WBw5n6ZHNaxGmt61ct5toAAAAAQP7RIwkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATxi1Fce/NVNzn95qaPHUAwAAADhOlGiPpJnVMbM3zWyvmf1uZnPMrG6UZRPM7GEz225mh8ws1cwujJCvjJndY2ZbzOwPM1trZpeF5allZhPNbI2/LrvM7P1I8wMAAACAE12JBZJmVl7SB5KaShos6RpJp0paamYVopjFS5JukHS/pD6Stkt6x8xahuUbL2mspGck9ZS0StJsM+uVJc85kq6U9LakyyUNkfSHpGVm1sf72gEAAADA8askb229QVIDSU2cc99Lkpl9KWmjpOGSHsupoJm1kDRQ0nXOuan+tOWS1kl6QFJff1oNSX+TNMk594i/+FIzayRpkqRF/rSPJDV2zmVkWcY7/vndKWlBYawwAAAAABwPSvLW1r6SVgWCSElyzm2WtFJSvyjKpkualaVshqSZkrqbWbw/ubukspJmhJWfIekMM6vvL/tb1iAyy/y+kHSyt9UCAAAAgONbSQaSp0v6OkL6OknNoii72Tl3MELZspIaZcl3WNL3EfIpt+WYWVlJbSV9m0ddcmRmnwU++Z0HAAAAAJQ2JXlra1VJeyKkp0lKKkDZwPTAv78551we+SIZK+kUSVfnURcAAAAAOKGU9Os/wgM8SbIoylmUZaPNFzrRbKCkuyWNd859GEV9InLOnRP4/2kN60SqBwAAAAAcc0ry1tY9itwjmKTIvY1ZpeVSNjA98G+SmYUHjuH5gszsYknTJL3knBuTRz0AAAAA4IRTkoHkOvmeYQzXTNI3UZSt73+FSHjZI/rfM5HrJMVLahghn8KXY2ZdJM2W9C/5Ro4FAAAAAIQpyUBynqQ2ZtYgkGBmKZLO90/Lq2ycpP5ZysbK9y7Id51zh/3Ji+ULLMOfcxwk6Wv/KLGB8m3le4/k+5IGOeeO5mOdAAAAAOC4V5LPSL4o6c+S3jaz0fI9yzhe0o+SXghkMrN6kjZJesA594AkOee+MLNZkp4wszhJmyXdJKm+sgSNzrmdZva4pHvMbJ+kz+ULNjsryytGzKyppIWSdkt6WNI5We+Gdc6tKvS1BwAAAIBjVIkFks65A2bWWdLjkqbLNwDO+5Judc7tz5LVJMUoe+/pUEkPSpogqYqktZJ6OOc+D8s3StJ+SSMk1ZS0QdIVzrn5WfK0ke+5ySRJSyNUN5oBgAAAAADghGDZ34yBonBawzpu2qRbI05rXT+3t5CgyLUaWtI1AAAAAArMzD5zzrUqjmWV5DOSAAAAAIBjEIEkAAAAAMATAkkAAAAAgCclOWorUDqsmZr7dJ6hBAAAAELQIwkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcMtnMM+GRzWq7TW9evWkw1AQAAAAB6JAEAAAAAHhFIAgAAAAA8IZAEAAAAAHjCM5KlQF7PQAIAAABAaUKPJAAAAADAE3okTwCM+goAAACgMNEjCQAAAADwhB7J4wDPWAIAAAAoTvRIAgAAAAA8IZAEAAAAAHjCra1AXtZMzX16q6HFUw8AAACglKBHEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgkAQAAAACeEEgCAAAAADwhkAQAAAAAeMJ7JKFPNqflOr11/arFVBMAAAAAxwJ6JAEAAAAAnhBIAgAAAAA84dZW5IlbXwEAAABkRY8kAAAAAMATeiRR5OjRBAAAAI4v9EgCAAAAADwhkAQAAAAAeMKtrSiwvG5dBQAAAHB8IZAECmrN1NyntxpaPPUAAAAAigm3tgIAAAAAPCGQBAAAAAB4QiAJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHgSW9IVAD7ZnJbr9Nb1qxZTTQAAAABEgx5JAAAAAIAnBJIAAAAAAE8IJAEAAAAAnvCMJEq9vJ6hzAvPWAIAAACFix5JAAAAAIAnBJIAAAAAAE8IJAEAAAAAnvCMJI57vKcSAAAAKFz0SAIAAAAAPKFHEihqa6bmPr3V0OKpBwAAAFBI6JEEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATBtvBCY/XgwAAAADe0CMJAAAAAPCEHkkgD/RYAgAAAKHokQQAAAAAeEIgCQAAAADwhEASAAAAAOAJgSQAAAAAwBMCSQAAAACAJ4zaChQQo7oCAADgREOPJAAAAADAEwJJAAAAAIAnBJIAAAAAAE94RhIoYnk+Q9mqmCoCAAAAFBJ6JAEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8ITBdoAS9snsR3Od3rr/7cVUEwAAACA69EgCAAAAADwhkAQAAAAAeEIgCQAAAADwhEASAAAAAOAJg+0Apdzrn2zLdfrA1nWLqSYAAACADz2SAAAAAABPCCQBAAAAAJ6UaCBpZnXM7E0z22tmv5vZHDOL6j49M0sws4fNbLuZHTKzVDO7MEK+MmZ2j5ltMbM/zGytmV0WId9gM3vLzLaamTOzaYWwigAAAABw3CmxQNLMykv6QFJTSYMlXSPpVElLzaxCFLN4SdINku6X1EfSdknvmFnLsHzjJY2V9IyknpJWSZptZr3C8g2S1FDSEkm/e18jAAAAADgxlORgOzdIaiCpiXPue0kysy8lbZQ0XNJjORU0sxaSBkq6zjk31Z+2XNI6SQ9I6utPqyHpb5ImOece8RdfamaNJE2StCjLbLs75476y/UorJUEAAAAgONNSQaSfSWtCgSRkuSc22xmKyX1Uy6BpL9suqRZWcpmmNlMSXebWbxz7rCk7pLKSpoRVn6GpJfNrL5zbrO//NHCWCmguDGqKwAAAIpbST4jebqkryOkr5PULIqym51zByOULSupUZZ8hyV9HyGfolgOAAAAACBMSfZIVpW0J0J6mqSkApQNTA/8+5tzzuWRr0iY2WeB/zdtcEpRLgoAAAAAik1JBpKSFB7gSZJFUc6iLBttPuC4xa2vAAAAKGwleWvrHkXuEUxS5N7GrNJyKRuYHvg3yczCA8fwfEXCOXdO4FOUywEAAACA4lSSgeQ6+Z5hDNdM0jdRlK3vf4VIeNkj+t8zkeskxcv3Wo/wfIpiOQAAAACAMCUZSM6T1MbMGgQSzCxF0vn+aXmVjZPUP0vZWElXSnrXP2KrJC2WL7C8Oqz8IElfB0ZsBQAAAABErySfkXxR0p8lvW1mo+V7lnG8pB8lvRDIZGb1JG2S9IBz7gFJcs59YWazJD1hZnGSNku6SVJ9ZQkanXM7zexxSfeY2T5Jn8sXbHaW7xUjyrKcZvpfT2U5SfXM7HL/38udc7sKc+UBAAAA4FhVYoGkc+6AmXWW9Lik6fINgPO+pFudc/uzZDVJMcreezpU0oOSJkiqImmtpB7Ouc/D8o2StF/SCEk1JW2QdIVzbn5Yviskjcnyd0f/R5I6SVrmZf2AYwWD8QAAAMAry/5mDBSF0xrWcdMm3VrS1cAxaFPd/nlnKkIEkgAAAMcGM/vMOdeqOJZVks9IAgAAAACOQQSSAAAAAABPSnKwHQDHAJ6hBAAAQDgCSaCUa7htdq7TS/oZSgAAAJx4uLUVAAAAAOAJgSQAAAAAwBMCSQAAAACAJzwjCaBAGIwHAADgxEOPJAAAAADAEwJJAAAAAIAnBJIAAAAAAE94RhJAkeIZSgAAgOMPPZIAAAAAAE8IJAEAAAAAnhBIAgAAAAA8IZAEAAAAAHjCYDsAShSD8QAAABx76JEEAAAAAHhCIAkAAAAA8IRAEgAAAADgCc9IAijVeIYSAACg9KFHEgAAAADgCYEkAAAAAMATbm0FcEzj1lcAAIDiR48kAAAAAMATeiSBY1zDbbNznb6pbv9iqgkAAABOFASSAI5r3PoKAABQ+Li1FQAAAADgCYEkAAAAAMATAkkAAAAAgCc8IwnghMYzlAAAAN7RIwkAAAAA8IRAEgAAAADgCbe2AkAuuPUVAAAgO3okAQAAAACeEEgCAAAAADzh1lYAKABufQUAACcieiQBAAAAAJ7QIwkARYgeSwAAcDyiRxIAAAAA4AmBJAAAAADAE25tBYASxK2vAADgWESPJAAAAADAEwJJAAAAAIAn3NoKHOcabpud6/RNdfsXU02QH9z6CgAASiN6JAEAAAAAntAjCQDHMHosAQBASaBHEgAAAADgCT2SAHAco8cSAAAUBXokAQAAAACe0CMJACcweiwBAEB+0CMJAAAAAPCEHkkAQI7osQQAAJHQIwkAAAAA8IQeSQBAvuXWY0lvJQAAxy96JAEAAAAAntAjCQAoEjxfCQDA8YseSQAAAACAJ/RIAgBKBD2WAAAcuwgkgRNcw22zc52+qW7/YqoJEIpAEwCA0otbWwEAAAAAntAjCQA4JtFjCQBAySGQBAAclwg0AQAoOgSSAIATEoEmAAD5xzOSAAAAAABP6JEEACACeiwBAMgZgSQAAPlAoAkAOJERSAIAUAQINAEAxzMCSQAASgCBJgDgWMZgOwAAAAAAT+iRBJCrhttm5zp9U93+xVQT4MRCjyUAoDQjkAQA4BhEoAkAKEkEkgAAHIcINAEARYlAEgCAExCBJgCgIAgkAQBANgSaAIDcEEgCAADPCDQB4MRGIAkAAApdXoFmXghEAaB0I5AEUCC8HgRAUaDHEwBKNwJJAABwzCHQBICSRSAJAACOOwSaAFC0CCQBAMAJp6DPcBYUgSyAY12Zkq4AAAAAAODYQo8kAABAMWNUWwDHOgJJAEWKUV0BoPAV9a25BKoA8kIgCQAAgBD0mALIC4EkAAAAChU9psDxj0ASAAAAxxQCVaDklWggaWZ1JD0uqZskk/SepFudc3meHcwsQdJ4SYMkVZH0haS7nHMrwvKVkXSXpOGSakraIOkB59xbEeZ5g6TbJdWXtEXS48655/O3dgCiwTOUAIDSpigDVYJUHC9KLJA0s/KSPpB0WNJgSU7SBElLzexM59yBPGbxkqTeku6Q9IOkWyS9Y2ZtnXNfZMk3XtLfJI2S9JmkAZJmm1kf59yiLPW5QdILkibKF9B2kTTFzMw591xB1xcAAAAo6XeY5oVAF9Ey51zJLNhshKTHJDVxzn3vT6svaaOkO51zj+VStoV8PZDXOeem+tNiJa2TtME519efVkPSj5ImOefGZCn/vqTqzrkzs5T9r6R/O+cGZ8n3sqS+kmo559ILsr6nNazjpk26tSCzABABPZYAACDgRA+Ezewz51yr4lhWSd7a2lfSqkAQKUnOuc1mtlJSP/mCzNzKpkualaVshpnNlHS3mcU75w5L6i6prKQZYeVnSHrZzOo75zZLaiupeoR80yUNldRe0tJ8rGNQmaNHVOHQzx5KmKf5e/s5wNu8vfE4bw/ZXWmqdxHO33muSuloF+8/SXmody5Zm33/Qq4FttbuWbh18XpsWtHNu0i3TxHW29Ox7Kke3nk7r3g9v3nZPkW47Yv0nFKE214q4v2wqOoheTs2i27eXutdpN8lPNeldBybOPYc6z2+edW/NAXKJRlIni7p7Qjp6yTl1cVwuqTNzrmDEcqWldTI///T5bt19vsI+SSpmaTN/nyS9HUu+QoUSJY7vFvNf3ipILMAkA8tNz5d0lUAAJwgjhbpjwjR8zpv7/m9KLq6FOWP2EXVhgf/nXu9+0VM/d+8Dy72UquiVZKBZFVJeyKkp0lKKkDZwPTAv7+57PfvRsqnCPMMz+eJmX0W+P85tcrkZxYAAAA4RpTxFNqUzONlOMaVot2mpF//EakpognnLcqyXvLlVJ/C0PSz7UczbNzva4to/ojeaf5/vy3RWiCA7VG6sD1KD7ZF6cL2KF3YHqUH26J0OU1Si+JaWEkGknsUuacvSZF7G7NKkxTpBuGkLNMD/yb5R151eeSTvz7bs+SrGjbdE+fcOdL/eiaL68FX5IxtUbqwPUoXtkfpwbYoXdgepQvbo/RgW5QuWe+GLA4leb9l4BnGcM0kfRNF2fr+V4iElz2i/z0TuU5SvKSGEfIpy3ICz0KG1yc8HwAAAACc8EoykJwnqY2ZNQgkmFmKpPP90/IqG6csg/L4X+FxpaR3/SO2StJi+QLLq8PKD5L0tX/EVklKlbQ7h3xpklZGt0oAAAAAcPwryfdIVpC0VtIhSaPlez5xvKSKks50zu3356snaZOkB5xzD2QpP1O+13vcId/IqzdJ6iOpnXPu8yz5Jkm6VdK9kj6XL9gcLqmfc25+lnw3Spoi6SFJ70nq7K/XX5xzzxZ+CwAAAADAsanEnpF0zh0ws86SHpfvfY0m6X1JtwaCSD+TFKPsvadDJT0oaYKkKvIFpT2yBpF+oyTtlzRCUk1JGyRdkTWI9NfneTNzkm6XLzjdJunPzrkpBVxVAAAAADiulFiPJAAAAADg2MTLDQEAAAAAnhBIAgAAAAA8IZAEAAAAAHhCIAkAAAAA8IRAEgAAAADgCYEkAAAAAMATAkkAAAAAgCcEkgAAAAAATwgki4iZ1TGzN81sr5n9bmZzzKxuSdfreGJml5vZW2a21cwOmdkGM5toZhWz5EkxM5fDp0rY/BLM7GEz2+6fX6qZXVjsK3aMMrOOObTzb2H5kszsH2a228wOmNl7ZnZGhPmxPQrAzJblsu8v9ufh+CgCZnaKmT3tb6OD/vZMiZCvUI8FMytjZveY2RYz+8PM1prZZUW0mseEaLaFmXUxsxlmtsnfvpvM7DkzqxFhfjkdLy3D8rEtIohyexT6eYntEVmU22NaLttjfVhejo98sii+0/rzlarrBoFkETCz8pI+kNRU0mBJ10g6VdJSM6tQknU7zvxNUqakeyX1kPScpJskLTGz8H17oqS2YZ99YXleknSDpPsl9ZG0XdI74SdA5OmvCm3nroEJZmaS5sm3vf4i6TJJcfIdG6eEzYftUTA3K/s+f5t/2rywvBwfhauRpCsk7ZH0YaQMRXQsjJc0VtIzknpKWiVptpn1KvAaHbvy3BaSbpRUTdIE+bbHREl9Ja0ys8QI+acp+/HyXVgetkVk0WyPgMI8L7E9Iotme4xX9u1wlX9a+LVE4vjIrzy/05bK64Zzjk8hfySN8O8MjbKk1ZeUIem2kq7f8fKRVD1C2rWSnKTO/r9T/H8Py2NeLfz5hmZJi5W0QdK8kl7XY+EjqaO/DbvmkqefP0+nLGmVJaVJeortUeTb6CVJhyVV9f/N8VE07Vwmy/+H+dsuJSxPoR4Lkmr4t+24sOW8L+nLkm6TUr4tIl1LLvTnvS4s3UmakMcy2RYF2x6Fel5iexRse+RQ7j5/3tPD0jk+8r8tovlOW+quG/RIFo2+klY5574PJDjnNktaKd9OgELgnNsVIXm1/9+TPc6ur6R0SbOyzD9D0kxJ3c0sPl+VRLi+kv7rnFsaSHDO7ZU0X6HHBtujkJlZOUn9Jc13zqV5LM728MA5dzSKbIV9LHSXVFbSjLDlzJB0hpnV97oex4NotkUhX0sktkWOojw2osWxUUAF2B7XSvrMObcuH2XZHhFEeR4qddcNAsmicbqkryOkr5PUrJjrcqLp4P/327D0iWaWYb5nVudFuJ/8dEmbnXMHw9LXyXeQNSqCuh6vXjOzTDP71cxet9Bng3M7NupmuY2M7VH4/iSpoqRXIkzj+Ch+hX0snC7fL8vfR8gnce3xKqdriSTdZGaH/c+UfWBmF4RNZ1sUjsI6L7E9CpGZnS9f20a6lkgcH4Up/DxU6q4bBJJFo6p895uHS5OUVMx1OWGY2cmSHpD0nnNujT/5sKQXJA2X1Em+e9DPkPSxmZ2WpXhu2ywwHbnbK+lR+W6P6SzfffddJaXa/watyKudk6LMx/bw7lpJOyX9O0sax0fJKexjoaqk35z/vqRc8iEP/sEtnpDvy9vcsMkz5Hv+uKuk/yffs5UfmFnHLHnYFgVT2Ocltkfhula+3q5/RpjG8VFIcvhOW+quG7F5ZUC+hW8USbJir8UJwv8rzNvyPYc6NJDunNsu30AKAR+ab8TKdZJGSRoUmIXYZgXinPuPpP9kSVpuZiskfSrfADyjFX07sz0KkZnVlu/C/qT/9hZJHB8lrLCPBbZRITCzWPm+IJ8s6fysx4skOeeuyfLnh2b2tnw9BBMktQ/MRmyLfCuC8xLbo5D4b4m8QtIC59zu8OkcH4Ujp++0KoXXDXoki8YeRY7ikxT5FwIUgJklyDeKVQNJ3Z1zP+WW3zn3o6SPJJ2bJTlNOW+zwHR45Jz7XL7R2gJtnVc774kyH9vDm0Hyne9zuhUpiOOj2BT2sZAmKck/ql9u+ZAD/8iIr8j3o8slzrkv8yrjnNsnaaGyHy9si0JUwPMS26Pw9JNURVFcSySOj/zI4zttqbtuEEgWjXXy3Xccrpmkb4q5Lsc1M4uT9Jak8yT1cs59FW1Rhf4Ks05Sff+rW7JqJumIst8/juhlbevcjo1tzrn9WfKxPQrPtZLWOufWRpmf46PoFfaxsE5SvKSGEfJJXHui8bykKyUNcM6976FcpOOFbVH48nteYnsUnsGSdkta5KEMx0eUovhOW+quGwSSRWOepDZm1iCQYL4XvJ6vyO/cQT74fz1+TVIXSf2cc6uiLFdXvm3xSZbkefK9i6d/lnyx8n2peNc5d7iw6n0iMbNWkhrrf209T9LJZtYhS55Kki5W6LHB9igk/m1wuqL8BZnjo9gU9rGwWL4vCFeHLWeQpK/9I4cjB2YWeL57qHNurodylST1VujxwrYoZAU8L7E9CoGZnSTpIkmvO+fSoyzD8RGlKL/TlrrrBs9IFo0XJf1Z0ttmNlq+X2LGS/pRvgfIUTiele8geVDSATNrk2XaT865n/xfDspISpW0S1ITSfdIOirpoUBm59wXZjZL0hP+X4Q2y/ci2PrKfoAhAjN7Tb52+1zSb5LOkq+tf5b0tD/bPPm2xQwzu0O+2zDuke8Xy/8LzIvtUaiule85i9fDJ3B8FB0zu9z/33P8//Y0s12SdjnnlquQjwXn3E4ze1zSPWa2T77j8Er5Br46oV87lde2MLO7JN0m6WVJG8OuJbucc5v88/mbfMfIUkn/lVRPvoFgaoptEbUotkehnpfYHrmL4lwVcLV8cUPEHyU5Pgosz++0Ko3XjWheNsknXy8WrStf9/TvkvbJN/JbSknX63j6SNoiX5Ae6TPWn+c6+d7Ds0e+L9O/yPeFukmE+ZWT9Jg/zx/y/YLWsaTX81j5+E9mX8o3emu6fD+c/F1SrbB8VeX7wpYm6aB8L75twfYokm0SJ98Xsfk5TOf4KLq2z+nctCxLnkI9FiTFyDeo1Vb5Rr78UtLlJd0WJf3Ja1tIWpZLnmlZ5nOxfO+D3u0/x/0q3xe789gWhbo9Cv28xPbI//bIkm+tpK9ymQ/HR8G2w5ZctsXYLPlK1XXD/DMBAAAAACAqPCMJAAAAAPCEQBIAAAAA4AmBJAAAAADAEwJJAAAAAIAnBJIAAAAAAE8IJAEAAAAAnhBIAgBKHTNzZjYty98p/rSxJVer7MwszswmmdlWM8s0sy0lXafiEr6N8lF+i5mtKcQqAQCKEYEkAOC4ZWZVzGysmXUsokXcKOkuSe9IGirp1iJaTp7MrJaZPWRm75jZbn+g90hJ1acwmdklpe1HBAA40cWWdAUAAIjCVknlJGV4LFdF0hj//5cVYn0CLpL0m6ThzjlXBPP3oomke+Rrq8/kq1tRKicps4iXEXCJpMGSxhbT8gAAeSCQBACUev4g7Y+SrockmVmMpBjn3BFJJ0naG00QaWblnXMHi7Bqn0mq7pzbbWYpkjYX9gKyrrtzrlRsDwBAyeDWVgBAiTGzemb2LzPbZ2Z7zOyfZnZShHzZnpE0sxgzu9PM1pnZATP7zcy+MrOH/NM76n/B1Bh/eWdmyzzUb4i/zCVmdr//GcjDktqZmZN0rqR6WeY91l9ui5mtMbOWZvaeme2TtMg/ramZPW9m6/313mdmy8ysSw51uMq/jn+Y2SYzu9XMhvqX1zGQzzm3zzm3O9p1K8i6+6dne0bSzBLN7Gkz2+lft2Vm1sr/75YclnOqmS3Msg+8YmaVskxfJl9vZGCZLnzdAQDFjx5JAECJMLMkSR/K16v3rKRNknpL+neUs7hPvttWX5X0lHzXtFMldfRP/1bSSEmPS/qXpDn+9B35qO4Dkpy/noclHZJ0jT+9on85kvRlljInSVoiabakNyQd9ad3lNRG0lvy3YZaXdIwSe+aWWfn3PLADMzsakkzJK2TNFpSWUkjJKXlYx3yK3zdt0fKZGYm3zpdJGmmfNv2dEnvSvo1h3lXl7RU0jxJd0g6X9K18t3CfL0/z4Py/fB9gXxtHvBtflcIAFBwBJIAgJJyl6Q6kq5wzs2WJDObIl/gdVYU5ftJ+rdzbnCkic65HWY2V75A8kvn3IwC1DVBUgvn3KEsaZ+Y2a2SyuQw71MkDXPOvRSW/qpz7vmsCWb2gqRvJN0tabk/LVbSI5K2SWrrnNvnT/+HpO8KsC5eRVr3SHrJF0Q+4ZwLBNYysy8lPS9f0ByurqTBzrlX/X8/b2ZVJF1rZiOcc/udc0v8AfUFBdyGAIBCxK2tAICS0k++IOnNQIL/WcNoRxr9TVIzMzut8KuWzctRBFLh9kt6JTwx63OSZlbezKr5//xU0nlZsraSVNO/7H1Zyu+U9JrHuhREtOt+sf/fJ8LLS9qbQ5k9kqaHpS2V74fulCjrBwAoAQSSAICSUl/ShggD1UR7y+JoSRUkfWNmG8zsOTPr7b/FsrBtykeZbc65bKPMmlklM3vKzLZLOiBpt6Rd8t3Wm5Qla4r/340R5l2cPZLRrnuKpCPy/TgQ5JxLV84D/2yNsP0Dt+1WC88MACg9CCQBAMck59xKSQ0kXSlfL9ZFkhZIWuK/LbQwee2NzK3MPyXdIt8tvAMkdZfUTdIHkrIGwYH/l/RrRaJdd5P3uub2+pCi+EEAAFBICCQBACVls6QmEXoQo75V1T9S6RvOuRudcw0l/Z+kLpJ6BrIUTlULh//5v16Spjvn/uqcm+Wce9c5957+f3v3DmJXFcVh/PtHEkHwERCjNmKTQtLFQhEFQbCxUXwnvhJNIQoBQSFoJQEVFBQbLSxE0MIqRAlKgoooEkUtgk18gTASsdERxNey2Gfi9WbI3MfcORfm+8Fw5m7O2ezDbe5i7bV2O5dx0FIWb+syUy031rdvgTNpdY8nJdlIyz5PY66+R0mSgaQkqT8HaEHHzUsDXVD5yCgPJzl/meHPu+vStsjF7rp5mXv78DctKPpf8Jzkalon10GfAj8Cu5KcPXDvBcCOGa9zEge7696h8V3AuVPOvQgnO/1KkuaAXVslSX15BrgTeC3Jlfx3/MdFIz7/VZKPaE1qFoBLgAdpNXZvA1TVz0m+Bm5PcpxWi3iiqo6s6puMqKp+TXIY2JlkEfiCloHdTTviY9vAvX8leYzWsOfj7szGjcAe4DiwnaFMXZLHu3/P665XDIwdqKrB40lW21vAYWBvkguBD2jHf9zRrXea3xyfAA8BLyY5BPwJHOkaD0mSemAgKUnqRRfkXUPr8rmHFhwcAu6jZeJW8ixwAy0Ddk73zEFg/1CAcRfwHPA0bfvo+7R6xL7soK39FuBe4EvgJto6tw3eWFWvJvkH2Ec7T/EH4HlaZnM7p9YvPjn0+aruj+7ZmQWSVVVJbgSeAm6ldeU9SqtdfQk4a4rpX6e97220utINwLWAgaQk9SSnNkuTJEnzLMkLwMPAxVW10Pd6TifJGbRM8NGqur7v9UiSVoc1kpIkzakkm5JsGBrbQsteHpu3IDLJcMMggPtpNarvrvFyJEkz5NZWSdK609XwreSnqjrd8RRr4TLgzSRvAN/TmhM9QNvKe88kE8743fcn2UrbPvwbrYHQTuAb4OUJ5pMkzSkDSUnSejRKJu9S4LsZr2MlC8BntAzkFuCP7vPdVfXOFHOuZNJ3fw+4HHiU1vDnBPAK8ERV/TLBfJKkOWWNpCRp3Uly3Qi3fVhVv898MWtsPb+7JGn1GEhKkiRJksZisx1JkiRJ0lgMJCVJkiRJYzGQlCRJkiSNxUBSkiRJkjQWA0lJkiRJ0lj+BaT7FkkeZJ/cAAAAAElFTkSuQmCC",
                         "text/plain": [
                             "<Figure size 921.6x633.6 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -257,15 +257,15 @@
             "cell_type": "code",
             "execution_count": 9,
             "id": "8fb2a16b-a921-4451-9250-4c0e381ac516",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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ySe5jnP48OF64YUX9NNPPwXHGdj+s85/NPvnlClTgsu4Vq1auu222/Tbb7/lOV9mpnHjxunxxx9XvXr1VL58eXXo0EHr1q3LVnfevHlq3bq1ypYtq0qVKmnAgAHati309oM5c+aoc+fOqlatmpKTk3XuuefqhRdeiDjdsWPHaurUqcF1+5///EeStHz5cnXp0kXly5dXuXLl1KNHD3311Vchw7/99ttq27atKlasqOTkZDVu3Fj3339/1Ms1q8D2E36Z9cyZM2VmIZfCpaamasiQIXruuefUsGFDJSUl6bzzztPSpUtDhs3v8TvwWTB9+nTdcccdqlWrlhITE4PrvLDXwbhx4/Twww+rbt26KleunPr06aOdO3dq586duvLKK1WxYkXVrl1b06ZNy3H5hS/HefPm6frrr1e1atV02mmnSZI2btyoyy67TNWrV1dSUpLq1KmjAQMGKCMjI+I6yOt4u3btWvXr10+VK1dWmTJl1K5dO33wwQd5trGodezYUe3bt9fixYvVokULlSlTRueee64+/vhjZWRk6J577lHNmjVVpUoVDR8+XIcOHQoZ3stn9+uvv67hw4ercuXKqlChgq6++mr98ssvIXUD+9kDDzygM844Q2XKlNHFF1+sL774Ilvbo9m2Dh8+rJtuuklVq1ZVcnKy+vXrpx9//DGqZRP4TP7qq6/Uo0cPJScn68orrwyON6/j/G+//aYxY8aoWbNmSk5OVo0aNXTJJZeEfA8JeO+993TeeecpKSlJDRo00N/+9rdsdTIyMnTvvfeqQYMGSkpKUkpKitq3b68PP/wwqvk5mcTy57uzJL0RoXydpAFFNVEzqyKpmaQZ+Rz+08D/zz+fq2NR/Hr37q358+drzZo1uvjii7O9f/DgQfXo0UMXXnihZs6cqfLly2vLli366KOPJEkjR47Ujz/+qOeff14ffvhhtudw/vTTTxozZozOOOMMHTp0SLNnz9bFF1+sNWvW6JxzzgmpO3r0aPXt21cvv/yyNmzYoDvuuENxcXEhXzwGDhyo+fPn65ZbblHXrl3122+/acWKFdq+fbuaNGmi/fv3q127djpy5IgmTJigevXq6e2339aNN96oo0eP6o9//GPE5dCnTx99+OGHat++va677jqNHDky5NfJffv2aeDAgfrzn/+sBx98UGXKlNF///tftW/fXuXLl9eTTz6pihUr6qmnnlKfPn20cOFC9erVK2QaAwYM0PXXX68///nPmj59uq699lpt2rRJy5Yt09SpU5Wenq7Ro0dr8ODB+vjjj3NcZ//617/Uu3dvNW/eXBMmTJAkVatWLaTOZZddphEjRmjMmDF68803NX78eNWuXTt4v2x+l1NWTz/9tP7yl78oLi5OrVu31sSJE3XRRRcF309NTVXYb285irR8o23jnj17lJSUpClTpqhatWr673//q4cffljt2rXT+vXrlZSUJEl69913NXjwYPXp00cPP/ywdu3apdGjRys9PV2NGzfOtX0ZGRnq0aOHvv76a9177706++yztWrVKk2aNEl79uzRww8/HFI/mm3597//vdauXasHH3xQZ555pubOnRvVcp8+fbqGDBmizMzM4JeSChUqSJK+/PJLdejQQU2bNg2Gj6lTp6pDhw5atWqVmjdvHnGc9957r3bt2qXVq1drwYIFkpTt1/lo5mnIkCF68803deedd6pt27b65ptvdO+992rLli16/fXX85y32bNnq3Hjxnrsscd07Ngx3X777erfv7/Wr18fPEP4zDPP6MYbb9SIESN033336cCBA5owYYI6dOigL7/8UuXLl5ckff/997riiit01113qVSpUlqxYoVGjhypI0eO6IYbbgiZ7syZM1W/fn099NBDKleunGrVqqVFixapf//+6tOnj2bPni1JmjZtmi666CJ9+eWXql27tr7//nv169dPV1xxhe677z6VLl1amzZt0vfffx/1ci2I5cuX69NPP9UDDzygxMRETZs2Tb169dLatWvVuHHjAh+/JemBBx7QBRdcoGeffVaZmZlKSkoqknUwa9YsNWvWTNOnT9eOHTt0yy23aOjQoTpw4IB69eql//f//p9effVV3XXXXTr77LPVu3fvPJfPH//4R/Xq1UuzZs0K/pjRt29fVapUSU8//bRSUlL0008/6a233srx0t7cjrefffaZLrroIp177rl67rnnVLZsWT3zzDPq2rWrPvroo5h/r/v22291++23a+zYsUpOTtYdd9yhfv36qV+/fsrIyNDMmTP1zTff6Pbbb1f16tX1f//3f8FhvXx2Bz6P//nPf2rTpk2655579N///jfbjxovvvii6tSpoyeffFJHjx7Vfffdpy5dumjTpk2qUqWKpOj371GjRmnu3LkaP368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aOTIkXrrrbey9RB9KohlkHxO0h8kvWFm4+S7X3KSpB8kBfvaNbO6kr6TdL9z7v4s5R0kVZNUw1/U0swOSpJz7jV/nYsl/VPSl5JmmlnWBw0ddc59XkTzBhTYF198od27d+vYsWPatm2bFi5cqFdffVXdunXTlClTchxu4cKFevbZZ3XppZeqXr16OnTokB5//HGVL18++CHRtGlTSdLDDz+sXr16KS4uTi1btlTPnj316KOPavjw4RoxYoQ2btyoSZMmZfuVMlqdOnXS5ZdfrltvvVU//PCDOnfurPT0dK1YsUJ9+vRRx44dNWbMGM2dO1cXXXSRxowZo8aNG+vQoUNav369Pvjgg0L9EjNmzBjNnDlT3bp108SJE1WhQgVNnz5dGzdu1KJFiwptOpE0bdpUH3zwgRYuXKgaNWooJSXF01mxgiynhx56SBs2bFCnTp1Uq1Ytbd26VQ899JB+/vlnvfTSS4Uwd97aGAgwDz74oC688EK9//77eu2117KNb+LEierevbsuvfRSjRo1Srt27dL48eODPezl5uqrr9aMGTPUpUsX3XbbbWrevLmOHTum7777TgsWLND8+fOj+jEmoFu3bmrfvr1GjRql3bt3B3ttjfaLQ9OmTTV9+nTNnTtXDRo0UPny5dW4cWPde++9Wrhwobp06aI777xTZqZp06bp8OHDuu+++/Ic5549e/T000+rZcuWSkpKCt6jGI2OHTtq0KBBuuKKK3TrrbfqwgsvVKlSpbRlyxa99dZbmjZtmho1ahT1+CKpUKGC/vKXv+jmm2/Wrl271KtXL1WsWFE//fSTli9fro4dO2rw4MFq27atKlSooJtvvlkTJ07UoUOHNHnyZKWkpGjfvn15TsfM9NRTT6l///46duyYrrzySqWkpGjHjh366KOPVKdOHd1666165plntGLFCvXu3Vu1a9fW7t27NWXKFNWqVSt4ts/Lcq1Zs6Y6dOigKVOmKCUlRdWrV9fs2bNzfCTQaaedpu7du2vChAnBXlsPHTqke++9V1LBjt+xXgdF4csvv9To0aN11VVXqWHDhsrMzNTMmTMVHx+f67ODczrePvLII7r44ovVo0cPXXfddapZs6Z2796tzz77TJmZmZo6daok32MyOnXqpBkzZmR7VFNJ5PWze926dRoxYoQGDhyojRs3auzYserQoUO2H5TKlCmj7t276/bbb9fRo0c1fvx4VahQQWPGjJEU/bbVuHFjDR48WPfdd5+OHz8e7LU1px9cohXtcb5nz56aP3++xowZo759++rTTz/V448/nu1s7bhx4/Tqq68G5/nYsWMaP358tktb+/fvr+bNm+u8885T5cqV9fnnn2vx4sUaNWpUgebnhFQUPfhE+5JUR9LrkvZLOiBpvqTUsDqp8oXMCWHly/zl2V5Z6kzIqY6kLQVtf1S9tq7+R+gLhSqanqpONIHe/gKvpKQkV6dOHXfppZe6V155JaQ3Puey99q6fv16d+WVV7rU1FSXmJjoUlJSXK9evdyqVauCw2RkZLibbrrJVatWzZlZYL9xzjn3+OOPu9TUVJeUlORatmzplixZ4jp06BDSS2ag57clS5ZEbHvWngrT09Pd5MmT3ZlnnukSEhKC7Vm/fn2wzp49e9wtt9ziUlNTXUJCgqtWrZpr3759jr0JZh23cui1NadeF9evX+/69+/vKlSo4BITE12rVq3cv//975A6OfWKGKknwJyWRbhvvvnGtW/f3pUpU8ZJcsOGDct1WsOGDQvpJc65/C+nBQsWuLZt27qqVau6+Ph4V6VKFXfJJZe4jz/+ONfhcpLb8o2mjYcPH3Y33HCDS0lJccnJya5Pnz7u+++/j7guX375ZdeoUSNXunRp17RpUzdv3rxs22NOjhw54saPH+8aN27sSpcu7SpXruxatmzpxo8fH1zeXrblnTt3uoEDB7rk5GRXsWJFd80117j58+dH1Wvr9u3bXa9evVxycnK2XmdXrVrlunTp4sqVK+fKli3rOnfuHNW6OXjwoBs4cKCrVKmSkxTcXrzMU2Zmpnv00UfdOeec4xITE12FChXcOeec426//Xb366+/5jp9SW7s2LEhZeHHo4BFixa5jh07uvLly7ukpCTXoEEDN2LECLdu3bpgnffee8+1aNHCJSUlufr167vHHnssuH/kNd2Ajz76yPXp08dVqlTJJSYmurp167qrrrrKffTRR8H3+/Xr58444wxXunRpV6NGDXfFFVeEHI9yWq45+eGHH1zfvn1dxYoV3Wmnnebuvvtu99xzz0XstfXqq692zz33nKtfv74rXbq0a9GihXvvvfeCdQpy/A4s++eeey5iO4t6HeTU43hOPRZnldM2u2PHDjd06FB35plnujJlyrjKlSu7iy++2C1evDjbsFn3wZyOt8459/XXX7urrrrKVatWzZUuXdqdfvrp7pJLLnGLFi0K1lm4cKGTlO2zIRodOnQImZ6X4cKXU07rNNLnhpfP7tdff90NGzbMVaxY0SUnJ7tBgwa5Xbt2hUxDkrvnnnvcAw884E4//XSXmJjo2rdvH7E352i2rUOHDrkbbrjBVa5c2ZUrV85dcskl7sMPP/TUa2uknr+jOc5nZma6sWPHupo1a7oyZcq4iy++2H322Weubt262dbVkiVLXIsWLVzp0qVdvXr13DPPPJPt8/ihhx5yrVq1clWqVHFJSUmuUaNGbvz48SE9WBenWPbaai5Lj0/wpmXLlm7NmjW5V1oTermWWo4ougadggKX4ng5swAAQHFLTU1V+/btg8+4RMl1zz33aMGCBfrPf/6T7/vIS6LAmdYlS5ZEvJc4KzPT2LFjNXny5GJqHfIrmu/CZvapc67Qb9w9eS4QBwAAAApo+fLluueee06qEAkUhVjeIwkAAACUKCtXrox1E4ATAkESAACgiG3ZsiXWTcAprmPHjor2ljZufUM0uLQVAAAAAOAJQRIAAAAA4AlBEgAAAADgCUESAAAAAOAJQRIAAAAA4AlBEgAAAADgCUESAAAAAOAJQRInrzUzYvvKp5kzZ8rMgq9y5copNTVVl112mV555RUdP348pP6WLVtkZpo5c2bU01i2bJkmTJiQbVwnorS0NLVq1UrlypWTmemLL76IdZMievTRRzVv3rxs5RMmTJCZKSMjo0inn3WbyvrKurwC29KyZcuKtC0F1bFjR3Xs2DHWzZDk25eiWWYzZ87UP/7xj0Kd9vz58/XII4/k2KZ33323UKd3qshpuXoROI6faM+OLIx5P5lEWo8TJkzQ+++/H7tGISrRHptjrSR9nuUHQRIooV599VWlpaXprbfe0qRJk5SYmKhBgwape/fuOnLkSLBezZo1lZaWpj59+kQ97mXLlmnixIknRZC87rrrlJGRoTfffFNpaWlq1KhRrJsUUU5BsjgNHz5caWlpIa+SurxONsUZJFEwp/JyPZXnPZI+ffooLS1NNWvWDJZNnDiRIAn4xce6AQAia9GihRo2bBj8+5prrtGAAQM0YMAA3XHHHXriiSckSYmJiWrdunWsmhlTx48f14YNGzR27Fh17tw517pHjx5VYmJiMbWsZDr99NOLbFth+SJWMjMz5ZxTfDxfaYrTibzPR9v2atWqqVq1asXQouikpqZq+PDhmjBhQqybclI7kbft4sYZSeAEcvnll6t///567rnndPjwYUmRL21dvXq1unXrpqpVq6ps2bKqX7++brrpJkm+y3ImTpwoSUpISAhe4hgwfvx4nXfeeapYsaJSUlLUuXNnrVq1KqQdgUtGFixYoD/84Q9KSUlRtWrVNGTIEP36668hdTMyMjRt2jQ1bdpUSUlJqlatmnr27Kn169cH6+zevVs33nijTj/9dCUmJqpJkyZ69tlnc10WM2fOVFxcnI4fP65JkybJzJSamirJd+btjDPOUFpamtq2basyZcrojjvukCRt2LBBl112mSpVqqQyZcqodevWWrx4cci4A5ebrl+/Xj169FC5cuVUp04dzZjhu2R51qxZatKkiZKTk9WpUyd99913ubY1NTVVW7du1UsvvRRc3sOHDw+ps3nzZvXp00fJycmqW7eu7r///mxnjPOznIpCbss3mjbu2rVLo0aNUqNGjVS2bFnVrl1bgwcP1k8//ZRtWnPmzFGTJk2UmJios846S//617+ibufhw4d15513ql69eipdurTq1aunBx54IGS5etmWd+3apcGDB6tChQqqVKmShg4dmq1OJB07dtTy5cu1cuXK4PrPeinTJ598oq5duyo5OVnlypVTly5d9Mknn+Q6zuHDh+uFF17QTz/9FBxnYPvPOv/R7J9TpkwJLuNatWrptttu02+//ZbnfJmZxo0bp8cff1z16tVT+fLl1aFDB61bty5b3Xnz5ql169YqW7asKlWqpAEDBmjbtm0hdebMmaPOnTurWrVqSk5O1rnnnqsXXngh4nTHjh2rqVOnBtftf/7zH0nS8uXL1aVLF5UvX17lypVTjx499NVXX4UM//bbb6tt27aqWLGikpOT1bhxY91///1RL9dw33//vfr06aOyZcuqWrVqGj16tI4ePZqtXnp6usaNG6fU1FSVLl1aqampGjdunNLT04N1mjVrppEjRwb/3rdvn+Li4nTGGWeEjKtdu3a68sorQ5ZJNOsiv/Me2E/mzZun66+/XtWqVdNpp50WHO9zzz2n5s2bKykpSSkpKbruuuu0Z8+ekGk/+eSTatOmjapUqaJKlSqpdevWWrRoUUidwOfZM888o7vvvls1atRQ+fLlNWTIEB0+fFjffvutevTooeTkZDVs2DDi9hEucHnqihUrNGDAAFWqVEmtWrWSlPtnZdZhA5e2Bj4rH3jggeAyyhrqotn+YiE1NVVDhgzRrFmz1LhxY5UpU0YXXXSRNm3apEOHDmnUqFGqWrWqTjvtNN12220ht1r89ttvGjNmjJo1a6bk5GTVqFFDl1xySchnuBS6nC+99FIlJyeratWquvnmm0Ouogqs4+nTp+vWW29V9erVVbZsWfXt2zfipeDRbFv5PTZLJe/z7ODBg/rjH/+oOnXqKDExUaeddpq6du2abXmXFPx8B5xgevfurfnz52vNmjW6+OKLs71/8OBB9ejRQxdeeKFmzpyp8uXLa8uWLfroo48kSSNHjtSPP/6o559/Xh9++KHi4uJChv/pp580ZswYnXHGGTp06JBmz56tiy++WGvWrNE555wTUnf06NHq27evXn75ZW3YsEF33HGH4uLiQj7cBw4cqPnz5+uWW25R165d9dtvv2nFihXavn27mjRpov3796tdu3Y6cuSIJkyYoHr16untt9/WjTfeqKNHj+qPf/xjxOXQp08fffjhh2rfvr2uu+46jRw5MuQXxH379mngwIH685//rAcffFBlypTRf//7X7Vv317ly5fXk08+qYoVK+qpp55Snz59tHDhQvXq1StkGgMGDND111+vP//5z5o+fbquvfZabdq0ScuWLdPUqVOVnp6u0aNHa/Dgwfr4449zXGf/+te/1Lt3bzVv3jz4pSP8V+7LLrtMI0aM0JgxY/Tmm29q/Pjxql27tkaMGCFJ+V5OWT399NP6y1/+ori4OLVu3VoTJ07URRddFHw/NTVVzrk8x5PT8o22jXv27FFSUpKmTJmiatWq6b///a8efvhhtWvXTuvXr1dSUpIk6d1339XgwYPVp08fPfzww9q1a5dGjx6t9PR0NW7cONf2ZWRkqEePHvr6669177336uyzz9aqVas0adIk7dmzRw8//HBI/Wi25d///vdau3atHnzwQZ155pmaO3duVMt9+vTpGjJkiDIzM/W3v/1NklShQgVJ0pdffqkOHTqoadOmwS9iU6dOVYcOHbRq1So1b9484jjvvfde7dq1S6tXr9aCBQskKdsv6NHM05AhQ/Tmm2/qzjvvVNu2bfXNN9/o3nvv1ZYtW/T666/nOW+zZ89W48aN9dhjj+nYsWO6/fbb1b9/f61fvz54hvCZZ57RjTfeqBEjRui+++7TgQMHNGHCBHXo0EFffvmlypcvL8kXyK644grdddddKlWqlFasWKGRI0fqyJEjuuGGG0KmO3PmTNWvX18PPfSQypUrp1q1amnRokXq37+/+vTpo9mzZ0uSpk2bposuukhffvmlateure+//179+vXTFVdcofvuu0+lS5fWpk2b9P3330e9XLM6duyYunXrpiNHjuipp55S9erV9be//S3iZezDhg3TK6+8onvuuUft27dXWlqaJk+erO+//14vv/yyJKlz585auHBhcJhly5YpMTFRP/30kzZu3KhGjRrp0KFDWr16tYYMGeJpXRTGvP/xj39Ur169NGvWrOCPDXfddZcefvhh/elPf9Jf/vIX/fTTTxo3bpy++uorffTRR8HPmC1btmjkyJFKTU0N3o7Qt29fvfXWW9mOvVOmTFHHjh31wgsv6Ouvv9Ydd9yhUqVK6fPPPw8ek59++mmNGDFCLVu21FlnnZXjOgq4+uqrNWjQIL322mvKyMjI87MykrS0NLVp00bDhw/XqFGjJCkY8qPZ/mJpxYoV+u677zRt2jQdO3ZMt9xyiy6//HLVr19fDRs21Jw5c7RixQpNnjxZDRo0CAbqo0eP6sCBAxo3bpxq1qypPXv2aPr06WrdurXWr1+vGjVqhExnyJAhuvLKK3XTTTfpk08+0f33369Dhw5l68dhypQpatGihWbMmKGdO3fqnnvuUffu3bVu3TolJCRIin7byu+xOaAkfZ6NGTNGCxYsCM7LL7/8opUrV0YdjIudc45XPl/nn3++y9Pqf4S+UKgOHTrkDh06FPnN8GVf3K98mjFjhpPkNm3aFPH9xYsXO0luzpw5zjnnNm/e7CS5GTNm+GZ79Wonya1duzbHaYwfP95Jcunp6bm2JSMjw6Wnp7tGjRq5P/3pT8HypUuXOklu6NChIfVvvvlml5iY6I4fP+6cc+69995zktxjjz2W4zTuv/9+l5iY6DZu3BhSPnLkSFe1atVc25ienu4kufHjx4eUDxs2zEly8+fPDym/7bbbXFxcXMiyzcjIcI0aNXLnnntusCywfF544YVg2Z49e1xcXJyrUqWK27dvX7D8sccec5Lcli1bcmync87VrVvXXX311dnKA9P6xz9Ct5lmzZq5bt26Bf8uyHJyzrkhQ4a4OXPmuBUrVrhZs2a5c845x8XHx7ulS5fmOlwkOS3f/LYxIyPDbdu2zUly8+bNC5a3bdvW/e53v3OZmZnBslWrVjlJrkOHDrm28cUXX3SS3PLly0PKJ0+e7BISEtyOHTucc9Fvy++8846T5P75z3+G1OvZs6eTlOdy7NChg2vXrl228ssvv9xVrFjR7d27N1i2b98+V7lyZXfZZZflOs5hw4a5008/PVt5tPO0YsWKbNu5c87Nnj3bSXKff/55rtOX5Bo2bOiOHTsWLHv11VedJLdy5UrnnHMHDhxwFSpUcCNGjAgZdvPmzS4hIcH99a9/jTjuzMxMl56e7kaOHOnOOeecbNOtWbOmO3z4cEh5gwYNXOfOnUPK9u3b56pWrepGjx4d0r6s+3C4nJZrJM8++6yT5NLS0kLa3rRpUyfJbd682Tnn3H/+85+Ix6pJkyaFHK/nzZsXcjwZPXq0u+SSS1zDhg3dM88845xz7t///reT5L755puQZZLXuijIvAe2qUsvvTSkfPPmza5UqVJu4sSJIeUffvihk+T+9a9/RZxOYP1269bN9evXL2R8klynTp1C6l922WVOkps1a1awLHBMnjBhQo7z49z/PlNvueWWkPJoPisDwwbWo3O+ZT127NhsdaPZ/rw4fvy4S09PD3nVrVvX3XvvvSFlGRkZeY6rbt26rnLlyu7XX38NlgU+u6677rqQuueee67r2LFjjuPKyMhwhw4dcsnJye6RRx4JlgeW1ahRo0LqT5482ZUqVcpt2LDBOfe/dRx+bA9sM3//+9+D9aLZtgp6bC5pn2dnnXWWGzNmTK5tDpfrd2E/SWtcEWQhLm0FTjDOf8Yo6+WoWZ155pmqVKmSRo0apdmzZ+uHH37wNP53331XnTp1UtWqVRUfH6+EhARt3LhRGzZsyFY3vIOfs88+W0ePHtWOHTskSe+8847MTNdff32O01u8eLFatWqlevXqKSMjI/jq0aOHfvnlF3399dee2h8QHx+vvn37hpStWLFCrVu3Drn3NC4uToMGDdIXX3yh/fv3h9TP+it55cqVVb16dbVu3Tp4NkmSmjRpIkmel3O48GXZrFmzkEv/CrqcZs2apauuukoXXXSRhgwZog8//FC1atXSuHHj8tXeSMvXSxuffvppNW/eXMnJyYqPj1edOnUkKbidZWZmavXq1briiitUqtT/PqpatWqV56WGgbbUrVtXbdu2DWlL9+7dlZ6enu1y7by25bS0NMXFxenyyy8PqTdw4MA825KbFStWqG/fvqpUqVKwrEKFCurXr5+WL19eoHHnNU+LFy9W6dKldfnll2dbRoG25aVbt27BsweBaUgKbrtpaWnav3+/rr766pBpnHHGGWrSpEnINDZt2qRBgwbp9NNPV0JCghISEvT3v/894rGnZ8+eKlOmTMiw3333XbbplC1bVm3atAlOp0WLFkpISNDAgQP12muvaefOnVEty5ykpaWpdu3aIfcelypVKuSyU+l/yzL8LGLg78C67tChg0qVKhXszOX9999X586d1blz55CymjVrBo89AXmti8KY98suuyzk7yVLluj48ePZlnurVq1UoUKFkPX76aefqm/fvjrttNOCny1LliyJuH7Dz1AG5rVHjx7BssAxOdpjb3jbC/pZmVW0258Xy5cvD+4HgdfWrVs1adKkkLIuXbpENb42bdqoYsWKwb8jLdNAefiyeOWVV9SqVStVqlRJ8fHxKleunA4ePBhx3YVv+wMHDtTx48ezXa4ffmxv165d8BJTKfptqzCOzSXp8+yCCy7QzJkz9eCDD2rNmjXKzMyMej5igSAJnGACB/isvchlVbFiRS1dulS1atXSTTfdpDp16qhZs2ZRXab22WefqXfv3kpOTtbzzz+vVatWafXq1WrevHnEe6aqVKkS8nfgMqhA3V9++UVVqlQJ+cIXbufOnVqxYkW2D8wBAwYEx5Ef1atXz3bZ7p49eyIutxo1asg5p71794aUV65cOeTv0qVLRyyTFNU9ZbmJtCyzjrOwl1P58uXVp08frV69Ol/tjbR8o23jE088oZtuukldu3bVvHnz9MknnwSDXWCed+/erfT09JD7sAIilYXbuXOntm7dmq0tF154YUhbAvLalrdv367KlSuHfFGPti25yW2bDN8evcprnnbu3Kljx44pOTk5ZBlVr15dUnTbVDTTkKSuXbtmWxf/+c9/gtM4ePCgunXrprVr12rq1Kn64IMPtHr1al177bUR7zcMX2aB6Vx33XXZprNw4cLgdBo2bKi3335bx48f1zXXXKMaNWqoVatW+Q7t27dvj2obDdzTFd7uwGWBgferVKmi5s2ba+nSpdq9e7e++uorderUSZ06dQo+xmDp0qXq1KlTtmnmtS4KY95zWu4NGzbMttz3798fXO4//PCDunTpoj179uiJJ57QRx99pNWrV6tnz54Rj505HWcjlUd77A1ve0E+K8NFu/15cf7552v16tUhr5o1a+r6668PKQtcLp+X/C7TN998U1dddZV+97vf6eWXX9bHH3+s1atXq1q1ahGXffi2H/g7/J7BnPabQL1ot63CODaXpM+zJ554QqNGjdI//vEPXXDBBapevbrGjBkT7BejpOEeSeAEs2jRIiUlJen888/PsU6LFi30+uuvKyMjQ2vWrNGUKVN05ZVXau3atWrWrFmOw73++uuKj4/XvHnzQg7Ke/fuDTljEq2UlBTt2bNHR44cyTFMVq1aVdWrV9djjz0W8f287oXLSaQztlWqVNHPP/+crfznn3+WmWX7IlaSFMVycs7leGY7L5GGi7aNc+bMUZcuXULuU9y8eXNI3ZSUFCUkJATPnmW1Y8cO1a1bN9f2Va1aVfXq1dMrr7wS8f1ozmpmVbNmTe3du1fp6ekh+0ak9nmR2zZZ1Ntj1apVlZSUpA8++CDi+7Vq1SqUaUi+exoj3ccWuD8yLS1NW7du1QcffKD27dsH38/p+arh219gOlOmTFHXrl2z1Q98aZYUDGZHjx7VypUrdd9996lPnz7asmWLUlJSPM1fzZo1I3YuFL5dBNblzz//rAYNGgTLA+s+0P5A++bOnaulS5eqatWqOuecc1SzZk3t3LlTK1eu1Oeffx68P8+rgs57Tsv9nXfeyRZIsr6/ePFi7du3T6+88kpIx0HF+eU40jErv5+V4bxsf9EqX768WrZsmW08tWrVylZelObMmaOGDRuG3OOYnp6ercObgB07doTs64F94fTTT89WL9KwLVq0kBT9tlUYx+aS9HmWnJysKVOmaMqUKdq6datee+013XXXXSpdurSmTZsW9TwVF4IkcAKZN2+eFixYoNGjR6ts2bJ51o+Pj1fr1q01adIkLViwQN98842aNWsW/KX6yJEjwS9yku9DPS4uLuSg+v7772vbtm2qV6+e5/Z2795dU6dO1d///vccb3zv2bOnnnjiCdWpUyd4JqSodOjQQY8++qi2bNkSDBKZmZmaO3euzj333JBlUdgSExNDeq7zqrCX0/79+7Vo0aJg74WFIdo2Hj58OOTyYEnBHnED4uLidMEFF+i1117ThAkTgpcDffzxx9qyZUueQbJnz556/fXXlZycnO0SwPxo06aNMjMz9frrr4dcMjVnzpyohk9MTNSBAweylXfo0EGLFi3SgQMHgtvfgQMH9Oabb+b5kOrC2KamTZumffv2RX15nFdt27ZV+fLl9e2332rYsGE51gsEivAfsN54442optO4cWOlpqZq3bp1uuuuu6IaJjExUZ07d9bBgwfVv39/bd68WSkpKZ6Wa5s2bTRjxgytWrUqeHnr8ePHs/2A0aFDB0m+7WXs2LHB8pdeekmSQjpO69Spkx555BH97W9/U8eOHWVmql69us466yyNHz9emZmZeT7uqDjmXfJdTluqVClt27ZN3bp1y7FepPW7ceNGrVy5MluPtLGQ02dlJKVLl862jPKz/Z0oDh8+nO3ROrNmzcrxkstXXnklZPucM2eOSpUqFbwaJCD82L5y5Ur9+OOPatOmjaTot62CHptzUhI+z+rWravbbrtNL730Uono/TcSgiRQQn3xxRfavXu3jh07pm3btmnhwoV69dVX1a1bN02ZMiXH4RYuXKhnn31Wl156qerVq6dDhw7p8ccfV/ny5YMH6KZNm0qSHn74YfXq1UtxcXFq2bKlevbsqUcffVTDhw/XiBEjtHHjRk2aNCnbL4nR6tSpky6//HLdeuut+uGHH9S5c2elp6drxYoV6tOnjzp27KgxY8Zo7ty5uuiiizRmzBg1btxYhw4d0vr16/XBBx9E/UUyGmPGjNHMmTPVrVs3TZw4URUqVND06dO1cePGbN3QF7amTZvqgw8+0MKFC1WjRg2lpKR4OitWkOX00EMPacOGDerUqZNq1aqlrVu36qGHHtLPP/8c/CJbGKJtYyDAPPjgg7rwwgv1/vvv67XXXss2vokTJ6p79+669NJLNWrUKO3atUvjx4/P1ktgJFdffbVmzJihLl266LbbblPz5s117Ngxfffdd1qwYIHmz58f1Y8xAd26dVP79u01atQo7d69O9gzYLQf7k2bNtX06dM1d+5cNWjQQOXLl1fjxo117733auHCherSpYvuvPNOmZmmTZumw4cP67777stznHv27NHTTz+tli1bKikpKXhfXDQ6duyoQYMG6YorrtCtt96qCy+8UKVKldKWLVv01ltvadq0aWrUqFHU44ukQoUK+stf/qKbb75Zu3btUq9evVSxYkX99NNPWr58uTp27KjBgwerbdu2qlChgm6++WZNnDhRhw4d0uTJk5WSkqJ9+/blOR0z01NPPaX+/fvr2LFjuvLKK5WSkqIdO3boo48+Up06dXTrrbfqmWee0YoVK9S7d2/Vrl1bu3fv1pQpU1SrVq1gcPCyXIcNG6apU6fq97//vR588EFVr15dzzzzTLb7rc866ywNGjRIEyZMUEZGhtq2bau0tDRNmjRJgwYNCukR++KLL1ZcXJzee+89PfXUU8HyTp066cknn1SdOnVUv359z+uisOddkho0aKA777xTf/jDH7RhwwZ16NBBSUlJ+uGHH7RkyRKNHDlSnTp1UteuXRUfH6+hQ4fqtttu0/bt2zV+/HjVqVMn22OOiks0n5WRNG3aVIsWLVLPnj1VuXJl1apVS7Vq1Ypq+5N8Z+dHjBihpUuX5vljUUnQs2dPzZ8/X2PGjFHfvn316aef6vHHH8/xKqW33npLt99+u7p3765PPvlEEydO1NChQ7MdSw4cOBBybL/77rt15plnaujQoZKi37YKemzOSaw+z9q0aaN+/frp7LPPVnJyspYvX661a9fm+kNcTBVFDz6nyoteW2Mvmp6qTjSBns8Cr6SkJFenTh136aWXuldeeSXY42JAeK+t69evd1deeaVLTU11iYmJLiUlxfXq1cutWrUqOExGRoa76aabXLVq1ZyZOd+hwOfxxx93qampLikpybVs2dItWbLEdejQIaRXsUAPfkuWLInY9qw93KWnp7vJkye7M8880yUkJATbs379+mCdPXv2uFtuucWlpqa6hIQEV61aNde+ffsce3TMOm7l0GtrTr0url+/3vXv399VqFDBJSYmulatWrl///vfIXVy6tU2Us+rOS2LcN98841r3769K1OmjJPkhg0bluu0hg0b5urWrRtSlt/ltGDBAte2bVtXtWpVFx8f76pUqeIuueQS9/HHH+c6XE5yW77RtPHw4cPuhhtucCkpKS45Odn16dPHff/99xHX5csvv+waNWrkSpcu7Zo2bermzZuXbXvMyZEjR9z48eNd48aNXenSpV3lypVdy5Yt3fjx44PL28u2vHPnTjdw4ECXnJzsKlas6K655ho3f/78qHoG3L59u+vVq5dLTk7O1kvfqlWrXJcuXVy5cuVc2bJlXefOnaNaNwcPHnQDBw50lSpVcpKC24uXecrMzHSPPvqoO+ecc1xiYqKrUKGCO+ecc9ztt98e0sNj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\n",
+                        "image/png": "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ySe5jnP48OF64YUX9NNPPwXHGdj+s85/NPvnlClTgsu4Vq1auu222/Tbb7/lOV9mpnHjxunxxx9XvXr1VL58eXXo0EHr1q3LVnfevHlq3bq1ypYtq0qVKmnAgAHati309oM5c+aoc+fOqlatmpKTk3XuuefqhRdeiDjdsWPHaurUqcF1+5///EeStHz5cnXp0kXly5dXuXLl1KNHD3311Vchw7/99ttq27atKlasqOTkZDVu3Fj3339/1Ms1q8D2E36Z9cyZM2VmIZfCpaamasiQIXruuefUsGFDJSUl6bzzztPSpUtDhs3v8TvwWTB9+nTdcccdqlWrlhITE4PrvLDXwbhx4/Twww+rbt26KleunPr06aOdO3dq586duvLKK1WxYkXVrl1b06ZNy3H5hS/HefPm6frrr1e1atV02mmnSZI2btyoyy67TNWrV1dSUpLq1KmjAQMGKCMjI+I6yOt4u3btWvXr10+VK1dWmTJl1K5dO33wwQd5trGodezYUe3bt9fixYvVokULlSlTRueee64+/vhjZWRk6J577lHNmjVVpUoVDR8+XIcOHQoZ3stn9+uvv67hw4ercuXKqlChgq6++mr98ssvIXUD+9kDDzygM844Q2XKlNHFF1+sL774Ilvbo9m2Dh8+rJtuuklVq1ZVcnKy+vXrpx9//DGqZRP4TP7qq6/Uo0cPJScn68orrwyON6/j/G+//aYxY8aoWbNmSk5OVo0aNXTJJZeEfA8JeO+993TeeecpKSlJDRo00N/+9rdsdTIyMnTvvfeqQYMGSkpKUkpKitq3b68PP/wwqvk5mcTy57uzJL0RoXydpAFFNVEzqyKpmaQZ+Rz+08D/zz+fq2NR/Hr37q358+drzZo1uvjii7O9f/DgQfXo0UMXXnihZs6cqfLly2vLli366KOPJEkjR47Ujz/+qOeff14ffvhhtudw/vTTTxozZozOOOMMHTp0SLNnz9bFF1+sNWvW6JxzzgmpO3r0aPXt21cvv/yyNmzYoDvuuENxcXEhXzwGDhyo+fPn65ZbblHXrl3122+/acWKFdq+fbuaNGmi/fv3q127djpy5IgmTJigevXq6e2339aNN96oo0eP6o9//GPE5dCnTx99+OGHat++va677jqNHDky5NfJffv2aeDAgfrzn/+sBx98UGXKlNF///tftW/fXuXLl9eTTz6pihUr6qmnnlKfPn20cOFC9erVK2QaAwYM0PXXX68///nPmj59uq699lpt2rRJy5Yt09SpU5Wenq7Ro0dr8ODB+vjjj3NcZ//617/Uu3dvNW/eXBMmTJAkVatWLaTOZZddphEjRmjMmDF68803NX78eNWuXTt4v2x+l1NWTz/9tP7yl78oLi5OrVu31sSJE3XRRRcF309NTVXYb285irR8o23jnj17lJSUpClTpqhatWr673//q4cffljt2rXT+vXrlZSUJEl69913NXjwYPXp00cPP/ywdu3apdGjRys9PV2NGzfOtX0ZGRnq0aOHvv76a9177706++yztWrVKk2aNEl79uzRww8/HFI/mm3597//vdauXasHH3xQZ555pubOnRvVcp8+fbqGDBmizMzM4JeSChUqSJK+/PJLdejQQU2bNg2Gj6lTp6pDhw5atWqVmjdvHnGc9957r3bt2qXVq1drwYIFkpTt1/lo5mnIkCF68803deedd6pt27b65ptvdO+992rLli16/fXX85y32bNnq3Hjxnrsscd07Ngx3X777erfv7/Wr18fPEP4zDPP6MYbb9SIESN033336cCBA5owYYI6dOigL7/8UuXLl5ckff/997riiit01113qVSpUlqxYoVGjhypI0eO6IYbbgiZ7syZM1W/fn099NBDKleunGrVqqVFixapf//+6tOnj2bPni1JmjZtmi666CJ9+eWXql27tr7//nv169dPV1xxhe677z6VLl1amzZt0vfffx/1ci2I5cuX69NPP9UDDzygxMRETZs2Tb169dLatWvVuHHjAh+/JemBBx7QBRdcoGeffVaZmZlKSkoqknUwa9YsNWvWTNOnT9eOHTt0yy23aOjQoTpw4IB69eql//f//p9effVV3XXXXTr77LPVu3fvPJfPH//4R/Xq1UuzZs0K/pjRt29fVapUSU8//bRSUlL0008/6a233srx0t7cjrefffaZLrroIp177rl67rnnVLZsWT3zzDPq2rWrPvroo5h/r/v22291++23a+zYsUpOTtYdd9yhfv36qV+/fsrIyNDMmTP1zTff6Pbbb1f16tX1f//3f8FhvXx2Bz6P//nPf2rTpk2655579N///jfbjxovvvii6tSpoyeffFJHjx7Vfffdpy5dumjTpk2qUqWKpOj371GjRmnu3LkaP368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aOTIkXrrrbey9RB9KohlkHxO0h8kvWFm4+S7X3KSpB8kBfvaNbO6kr6TdL9z7v4s5R0kVZNUw1/U0swOSpJz7jV/nYsl/VPSl5JmmlnWBw0ddc59XkTzBhTYF198od27d+vYsWPatm2bFi5cqFdffVXdunXTlClTchxu4cKFevbZZ3XppZeqXr16OnTokB5//HGVL18++CHRtGlTSdLDDz+sXr16KS4uTi1btlTPnj316KOPavjw4RoxYoQ2btyoSZMmZfuVMlqdOnXS5ZdfrltvvVU//PCDOnfurPT0dK1YsUJ9+vRRx44dNWbMGM2dO1cXXXSRxowZo8aNG+vQoUNav369Pvjgg0L9EjNmzBjNnDlT3bp108SJE1WhQgVNnz5dGzdu1KJFiwptOpE0bdpUH3zwgRYuXKgaNWooJSXF01mxgiynhx56SBs2bFCnTp1Uq1Ytbd26VQ899JB+/vlnvfTSS4Uwd97aGAgwDz74oC688EK9//77eu2117KNb+LEierevbsuvfRSjRo1Srt27dL48eODPezl5uqrr9aMGTPUpUsX3XbbbWrevLmOHTum7777TgsWLND8+fOj+jEmoFu3bmrfvr1GjRql3bt3B3ttjfaLQ9OmTTV9+nTNnTtXDRo0UPny5dW4cWPde++9Wrhwobp06aI777xTZqZp06bp8OHDuu+++/Ic5549e/T000+rZcuWSkpKCt6jGI2OHTtq0KBBuuKKK3TrrbfqwgsvVKlSpbRlyxa99dZbmjZtmho1ahT1+CKpUKGC/vKXv+jmm2/Wrl271KtXL1WsWFE//fSTli9fro4dO2rw4MFq27atKlSooJtvvlkTJ07UoUOHNHnyZKWkpGjfvn15TsfM9NRTT6l///46duyYrrzySqWkpGjHjh366KOPVKdOHd1666165plntGLFCvXu3Vu1a9fW7t27NWXKFNWqVSt4ts/Lcq1Zs6Y6dOigKVOmKCUlRdWrV9fs2bNzfCTQaaedpu7du2vChAnBXlsPHTqke++9V1LBjt+xXgdF4csvv9To0aN11VVXqWHDhsrMzNTMmTMVHx+f67ODczrePvLII7r44ovVo0cPXXfddapZs6Z2796tzz77TJmZmZo6daok32MyOnXqpBkzZmR7VFNJ5PWze926dRoxYoQGDhyojRs3auzYserQoUO2H5TKlCmj7t276/bbb9fRo0c1fvx4VahQQWPGjJEU/bbVuHFjDR48WPfdd5+OHz8e7LU1px9cohXtcb5nz56aP3++xowZo759++rTTz/V448/nu1s7bhx4/Tqq68G5/nYsWMaP358tktb+/fvr+bNm+u8885T5cqV9fnnn2vx4sUaNWpUgebnhFQUPfhE+5JUR9LrkvZLOiBpvqTUsDqp8oXMCWHly/zl2V5Z6kzIqY6kLQVtf1S9tq7+R+gLhSqanqpONIHe/gKvpKQkV6dOHXfppZe6V155JaQ3Puey99q6fv16d+WVV7rU1FSXmJjoUlJSXK9evdyqVauCw2RkZLibbrrJVatWzZlZYL9xzjn3+OOPu9TUVJeUlORatmzplixZ4jp06BDSS2ag57clS5ZEbHvWngrT09Pd5MmT3ZlnnukSEhKC7Vm/fn2wzp49e9wtt9ziUlNTXUJCgqtWrZpr3759jr0JZh23cui1NadeF9evX+/69+/vKlSo4BITE12rVq3cv//975A6OfWKGKknwJyWRbhvvvnGtW/f3pUpU8ZJcsOGDct1WsOGDQvpJc65/C+nBQsWuLZt27qqVau6+Ph4V6VKFXfJJZe4jz/+ONfhcpLb8o2mjYcPH3Y33HCDS0lJccnJya5Pnz7u+++/j7guX375ZdeoUSNXunRp17RpUzdv3rxs22NOjhw54saPH+8aN27sSpcu7SpXruxatmzpxo8fH1zeXrblnTt3uoEDB7rk5GRXsWJFd80117j58+dH1Wvr9u3bXa9evVxycnK2XmdXrVrlunTp4sqVK+fKli3rOnfuHNW6OXjwoBs4cKCrVKmSkxTcXrzMU2Zmpnv00UfdOeec4xITE12FChXcOeec426//Xb366+/5jp9SW7s2LEhZeHHo4BFixa5jh07uvLly7ukpCTXoEEDN2LECLdu3bpgnffee8+1aNHCJSUlufr167vHHnssuH/kNd2Ajz76yPXp08dVqlTJJSYmurp167qrrrrKffTRR8H3+/Xr58444wxXunRpV6NGDXfFFVeEHI9yWq45+eGHH1zfvn1dxYoV3Wmnnebuvvtu99xzz0XstfXqq692zz33nKtfv74rXbq0a9GihXvvvfeCdQpy/A4s++eeey5iO4t6HeTU43hOPRZnldM2u2PHDjd06FB35plnujJlyrjKlSu7iy++2C1evDjbsFn3wZyOt8459/XXX7urrrrKVatWzZUuXdqdfvrp7pJLLnGLFi0K1lm4cKGTlO2zIRodOnQImZ6X4cKXU07rNNLnhpfP7tdff90NGzbMVaxY0SUnJ7tBgwa5Xbt2hUxDkrvnnnvcAw884E4//XSXmJjo2rdvH7E352i2rUOHDrkbbrjBVa5c2ZUrV85dcskl7sMPP/TUa2uknr+jOc5nZma6sWPHupo1a7oyZcq4iy++2H322Weubt262dbVkiVLXIsWLVzp0qVdvXr13DPPPJPt8/ihhx5yrVq1clWqVHFJSUmuUaNGbvz48SE9WBenWPbaai5Lj0/wpmXLlm7NmjW5V1oTermWWo4ougadggKX4ng5swAAQHFLTU1V+/btg8+4RMl1zz33aMGCBfrPf/6T7/vIS6LAmdYlS5ZEvJc4KzPT2LFjNXny5GJqHfIrmu/CZvapc67Qb9w9eS4QBwAAAApo+fLluueee06qEAkUhVjeIwkAAACUKCtXrox1E4ATAkESAACgiG3ZsiXWTcAprmPHjor2ljZufUM0uLQVAAAAAOAJQRIAAAAA4AlBEgAAAADgCUESAAAAAOAJQRIAAAAA4AlBEgAAAADgCUESAAAAAOAJQRInrzUzYvvKp5kzZ8rMgq9y5copNTVVl112mV555RUdP348pP6WLVtkZpo5c2bU01i2bJkmTJiQbVwnorS0NLVq1UrlypWTmemLL76IdZMievTRRzVv3rxs5RMmTJCZKSMjo0inn3WbyvrKurwC29KyZcuKtC0F1bFjR3Xs2DHWzZDk25eiWWYzZ87UP/7xj0Kd9vz58/XII4/k2KZ33323UKd3qshpuXoROI6faM+OLIx5P5lEWo8TJkzQ+++/H7tGISrRHptjrSR9nuUHQRIooV599VWlpaXprbfe0qRJk5SYmKhBgwape/fuOnLkSLBezZo1lZaWpj59+kQ97mXLlmnixIknRZC87rrrlJGRoTfffFNpaWlq1KhRrJsUUU5BsjgNHz5caWlpIa+SurxONsUZJFEwp/JyPZXnPZI+ffooLS1NNWvWDJZNnDiRIAn4xce6AQAia9GihRo2bBj8+5prrtGAAQM0YMAA3XHHHXriiSckSYmJiWrdunWsmhlTx48f14YNGzR27Fh17tw517pHjx5VYmJiMbWsZDr99NOLbFth+SJWMjMz5ZxTfDxfaYrTibzPR9v2atWqqVq1asXQouikpqZq+PDhmjBhQqybclI7kbft4sYZSeAEcvnll6t///567rnndPjwYUmRL21dvXq1unXrpqpVq6ps2bKqX7++brrpJkm+y3ImTpwoSUpISAhe4hgwfvx4nXfeeapYsaJSUlLUuXNnrVq1KqQdgUtGFixYoD/84Q9KSUlRtWrVNGTIEP36668hdTMyMjRt2jQ1bdpUSUlJqlatmnr27Kn169cH6+zevVs33nijTj/9dCUmJqpJkyZ69tlnc10WM2fOVFxcnI4fP65JkybJzJSamirJd+btjDPOUFpamtq2basyZcrojjvukCRt2LBBl112mSpVqqQyZcqodevWWrx4cci4A5ebrl+/Xj169FC5cuVUp04dzZjhu2R51qxZatKkiZKTk9WpUyd99913ubY1NTVVW7du1UsvvRRc3sOHDw+ps3nzZvXp00fJycmqW7eu7r///mxnjPOznIpCbss3mjbu2rVLo0aNUqNGjVS2bFnVrl1bgwcP1k8//ZRtWnPmzFGTJk2UmJios846S//617+ibufhw4d15513ql69eipdurTq1aunBx54IGS5etmWd+3apcGDB6tChQqqVKmShg4dmq1OJB07dtTy5cu1cuXK4PrPeinTJ598oq5duyo5OVnlypVTly5d9Mknn+Q6zuHDh+uFF17QTz/9FBxnYPvPOv/R7J9TpkwJLuNatWrptttu02+//ZbnfJmZxo0bp8cff1z16tVT+fLl1aFDB61bty5b3Xnz5ql169YqW7asKlWqpAEDBmjbtm0hdebMmaPOnTurWrVqSk5O1rnnnqsXXngh4nTHjh2rqVOnBtftf/7zH0nS8uXL1aVLF5UvX17lypVTjx499NVXX4UM//bbb6tt27aqWLGikpOT1bhxY91///1RL9dw33//vfr06aOyZcuqWrVqGj16tI4ePZqtXnp6usaNG6fU1FSVLl1aqampGjdunNLT04N1mjVrppEjRwb/3rdvn+Li4nTGGWeEjKtdu3a68sorQ5ZJNOsiv/Me2E/mzZun66+/XtWqVdNpp50WHO9zzz2n5s2bKykpSSkpKbruuuu0Z8+ekGk/+eSTatOmjapUqaJKlSqpdevWWrRoUUidwOfZM888o7vvvls1atRQ+fLlNWTIEB0+fFjffvutevTooeTkZDVs2DDi9hEucHnqihUrNGDAAFWqVEmtWrWSlPtnZdZhA5e2Bj4rH3jggeAyyhrqotn+YiE1NVVDhgzRrFmz1LhxY5UpU0YXXXSRNm3apEOHDmnUqFGqWrWqTjvtNN12220ht1r89ttvGjNmjJo1a6bk5GTVqFFDl1xySchnuBS6nC+99FIlJyeratWquvnmm0Ouogqs4+nTp+vWW29V9erVVbZsWfXt2zfipeDRbFv5PTZLJe/z7ODBg/rjH/+oOnXqKDExUaeddpq6du2abXmXFPx8B5xgevfurfnz52vNmjW6+OKLs71/8OBB9ejRQxdeeKFmzpyp8uXLa8uWLfroo48kSSNHjtSPP/6o559/Xh9++KHi4uJChv/pp580ZswYnXHGGTp06JBmz56tiy++WGvWrNE555wTUnf06NHq27evXn75ZW3YsEF33HGH4uLiQj7cBw4cqPnz5+uWW25R165d9dtvv2nFihXavn27mjRpov3796tdu3Y6cuSIJkyYoHr16untt9/WjTfeqKNHj+qPf/xjxOXQp08fffjhh2rfvr2uu+46jRw5MuQXxH379mngwIH685//rAcffFBlypTRf//7X7Vv317ly5fXk08+qYoVK+qpp55Snz59tHDhQvXq1StkGgMGDND111+vP//5z5o+fbquvfZabdq0ScuWLdPUqVOVnp6u0aNHa/Dgwfr4449zXGf/+te/1Lt3bzVv3jz4pSP8V+7LLrtMI0aM0JgxY/Tmm29q/Pjxql27tkaMGCFJ+V5OWT399NP6y1/+ori4OLVu3VoTJ07URRddFHw/NTVVzrk8x5PT8o22jXv27FFSUpKmTJmiatWq6b///a8efvhhtWvXTuvXr1dSUpIk6d1339XgwYPVp08fPfzww9q1a5dGjx6t9PR0NW7cONf2ZWRkqEePHvr6669177336uyzz9aqVas0adIk7dmzRw8//HBI/Wi25d///vdau3atHnzwQZ155pmaO3duVMt9+vTpGjJkiDIzM/W3v/1NklShQgVJ0pdffqkOHTqoadOmwS9iU6dOVYcOHbRq1So1b9484jjvvfde7dq1S6tXr9aCBQskKdsv6NHM05AhQ/Tmm2/qzjvvVNu2bfXNN9/o3nvv1ZYtW/T666/nOW+zZ89W48aN9dhjj+nYsWO6/fbb1b9/f61fvz54hvCZZ57RjTfeqBEjRui+++7TgQMHNGHCBHXo0EFffvmlypcvL8kXyK644grdddddKlWqlFasWKGRI0fqyJEjuuGGG0KmO3PmTNWvX18PPfSQypUrp1q1amnRokXq37+/+vTpo9mzZ0uSpk2bposuukhffvmlateure+//179+vXTFVdcofvuu0+lS5fWpk2b9P3330e9XLM6duyYunXrpiNHjuipp55S9erV9be//S3iZezDhg3TK6+8onvuuUft27dXWlqaJk+erO+//14vv/yyJKlz585auHBhcJhly5YpMTFRP/30kzZu3KhGjRrp0KFDWr16tYYMGeJpXRTGvP/xj39Ur169NGvWrOCPDXfddZcefvhh/elPf9Jf/vIX/fTTTxo3bpy++uorffTRR8HPmC1btmjkyJFKTU0N3o7Qt29fvfXWW9mOvVOmTFHHjh31wgsv6Ouvv9Ydd9yhUqVK6fPPPw8ek59++mmNGDFCLVu21FlnnZXjOgq4+uqrNWjQIL322mvKyMjI87MykrS0NLVp00bDhw/XqFGjJCkY8qPZ/mJpxYoV+u677zRt2jQdO3ZMt9xyiy6//HLVr19fDRs21Jw5c7RixQpNnjxZDRo0CAbqo0eP6sCBAxo3bpxq1qypPXv2aPr06WrdurXWr1+vGjVqhExnyJAhuvLKK3XTTTfpk08+0f33369Dhw5l68dhypQpatGihWbMmKGdO3fqnnvuUffu3bVu3TolJCRIin7byu+xOaAkfZ6NGTNGCxYsCM7LL7/8opUrV0YdjIudc45XPl/nn3++y9Pqf4S+UKgOHTrkDh06FPnN8GVf3K98mjFjhpPkNm3aFPH9xYsXO0luzpw5zjnnNm/e7CS5GTNm+GZ79Wonya1duzbHaYwfP95Jcunp6bm2JSMjw6Wnp7tGjRq5P/3pT8HypUuXOklu6NChIfVvvvlml5iY6I4fP+6cc+69995zktxjjz2W4zTuv/9+l5iY6DZu3BhSPnLkSFe1atVc25ienu4kufHjx4eUDxs2zEly8+fPDym/7bbbXFxcXMiyzcjIcI0aNXLnnntusCywfF544YVg2Z49e1xcXJyrUqWK27dvX7D8sccec5Lcli1bcmync87VrVvXXX311dnKA9P6xz9Ct5lmzZq5bt26Bf8uyHJyzrkhQ4a4OXPmuBUrVrhZs2a5c845x8XHx7ulS5fmOlwkOS3f/LYxIyPDbdu2zUly8+bNC5a3bdvW/e53v3OZmZnBslWrVjlJrkOHDrm28cUXX3SS3PLly0PKJ0+e7BISEtyOHTucc9Fvy++8846T5P75z3+G1OvZs6eTlOdy7NChg2vXrl228ssvv9xVrFjR7d27N1i2b98+V7lyZXfZZZflOs5hw4a5008/PVt5tPO0YsWKbNu5c87Nnj3bSXKff/55rtOX5Bo2bOiOHTsWLHv11VedJLdy5UrnnHMHDhxwFSpUcCNGjAgZdvPmzS4hIcH99a9/jTjuzMxMl56e7kaOHOnOOeecbNOtWbOmO3z4cEh5gwYNXOfOnUPK9u3b56pWrepGjx4d0r6s+3C4nJZrJM8++6yT5NLS0kLa3rRpUyfJbd682Tnn3H/+85+Ix6pJkyaFHK/nzZsXcjwZPXq0u+SSS1zDhg3dM88845xz7t///reT5L755puQZZLXuijIvAe2qUsvvTSkfPPmza5UqVJu4sSJIeUffvihk+T+9a9/RZxOYP1269bN9evXL2R8klynTp1C6l922WVOkps1a1awLHBMnjBhQo7z49z/PlNvueWWkPJoPisDwwbWo3O+ZT127NhsdaPZ/rw4fvy4S09PD3nVrVvX3XvvvSFlGRkZeY6rbt26rnLlyu7XX38NlgU+u6677rqQuueee67r2LFjjuPKyMhwhw4dcsnJye6RRx4JlgeW1ahRo0LqT5482ZUqVcpt2LDBOfe/dRx+bA9sM3//+9+D9aLZtgp6bC5pn2dnnXWWGzNmTK5tDpfrd2E/SWtcEWQhLm0FTjDOf8Yo6+WoWZ155pmqVKmSRo0apdmzZ+uHH37wNP53331XnTp1UtWqVRUfH6+EhARt3LhRGzZsyFY3vIOfs88+W0ePHtWOHTskSe+8847MTNdff32O01u8eLFatWqlevXqKSMjI/jq0aOHfvnlF3399dee2h8QHx+vvn37hpStWLFCrVu3Drn3NC4uToMGDdIXX3yh/fv3h9TP+it55cqVVb16dbVu3Tp4NkmSmjRpIkmel3O48GXZrFmzkEv/CrqcZs2apauuukoXXXSRhgwZog8//FC1atXSuHHj8tXeSMvXSxuffvppNW/eXMnJyYqPj1edOnUkKbidZWZmavXq1briiitUqtT/PqpatWqV56WGgbbUrVtXbdu2DWlL9+7dlZ6enu1y7by25bS0NMXFxenyyy8PqTdw4MA825KbFStWqG/fvqpUqVKwrEKFCurXr5+WL19eoHHnNU+LFy9W6dKldfnll2dbRoG25aVbt27BsweBaUgKbrtpaWnav3+/rr766pBpnHHGGWrSpEnINDZt2qRBgwbp9NNPV0JCghISEvT3v/894rGnZ8+eKlOmTMiw3333XbbplC1bVm3atAlOp0WLFkpISNDAgQP12muvaefOnVEty5ykpaWpdu3aIfcelypVKuSyU+l/yzL8LGLg78C67tChg0qVKhXszOX9999X586d1blz55CymjVrBo89AXmti8KY98suuyzk7yVLluj48ePZlnurVq1UoUKFkPX76aefqm/fvjrttNOCny1LliyJuH7Dz1AG5rVHjx7BssAxOdpjb3jbC/pZmVW0258Xy5cvD+4HgdfWrVs1adKkkLIuXbpENb42bdqoYsWKwb8jLdNAefiyeOWVV9SqVStVqlRJ8fHxKleunA4ePBhx3YVv+wMHDtTx48ezXa4ffmxv165d8BJTKfptqzCOzSXp8+yCCy7QzJkz9eCDD2rNmjXKzMyMej5igSAJnGACB/isvchlVbFiRS1dulS1atXSTTfdpDp16qhZs2ZRXab22WefqXfv3kpOTtbzzz+vVatWafXq1WrevHnEe6aqVKkS8nfgMqhA3V9++UVVqlQJ+cIXbufOnVqxYkW2D8wBAwYEx5Ef1atXz3bZ7p49eyIutxo1asg5p71794aUV65cOeTv0qVLRyyTFNU9ZbmJtCyzjrOwl1P58uXVp08frV69Ol/tjbR8o23jE088oZtuukldu3bVvHnz9MknnwSDXWCed+/erfT09JD7sAIilYXbuXOntm7dmq0tF154YUhbAvLalrdv367KlSuHfFGPti25yW2bDN8evcprnnbu3Kljx44pOTk5ZBlVr15dUnTbVDTTkKSuXbtmWxf/+c9/gtM4ePCgunXrprVr12rq1Kn64IMPtHr1al177bUR7zcMX2aB6Vx33XXZprNw4cLgdBo2bKi3335bx48f1zXXXKMaNWqoVatW+Q7t27dvj2obDdzTFd7uwGWBgferVKmi5s2ba+nSpdq9e7e++uorderUSZ06dQo+xmDp0qXq1KlTtmnmtS4KY95zWu4NGzbMttz3798fXO4//PCDunTpoj179uiJJ57QRx99pNWrV6tnz54Rj505HWcjlUd77A1ve0E+K8NFu/15cf7552v16tUhr5o1a+r6668PKQtcLp+X/C7TN998U1dddZV+97vf6eWXX9bHH3+s1atXq1q1ahGXffi2H/g7/J7BnPabQL1ot63CODaXpM+zJ554QqNGjdI//vEPXXDBBapevbrGjBkT7BejpOEeSeAEs2jRIiUlJen888/PsU6LFi30+uuvKyMjQ2vWrNGUKVN05ZVXau3atWrWrFmOw73++uuKj4/XvHnzQg7Ke/fuDTljEq2UlBTt2bNHR44cyTFMVq1aVdWrV9djjz0W8f287oXLSaQztlWqVNHPP/+crfznn3+WmWX7IlaSFMVycs7leGY7L5GGi7aNc+bMUZcuXULuU9y8eXNI3ZSUFCUkJATPnmW1Y8cO1a1bN9f2Va1aVfXq1dMrr7wS8f1ozmpmVbNmTe3du1fp6ekh+0ak9nmR2zZZ1Ntj1apVlZSUpA8++CDi+7Vq1SqUaUi+exoj3ccWuD8yLS1NW7du1QcffKD27dsH38/p+arh219gOlOmTFHXrl2z1Q98aZYUDGZHjx7VypUrdd9996lPnz7asmWLUlJSPM1fzZo1I3YuFL5dBNblzz//rAYNGgTLA+s+0P5A++bOnaulS5eqatWqOuecc1SzZk3t3LlTK1eu1Oeffx68P8+rgs57Tsv9nXfeyRZIsr6/ePFi7du3T6+88kpIx0HF+eU40jErv5+V4bxsf9EqX768WrZsmW08tWrVylZelObMmaOGDRuG3OOYnp6ercObgB07doTs64F94fTTT89WL9KwLVq0kBT9tlUYx+aS9HmWnJysKVOmaMqUKdq6datee+013XXXXSpdurSmTZsW9TwVF4IkcAKZN2+eFixYoNGjR6ts2bJ51o+Pj1fr1q01adIkLViwQN98842aNWsW/KX6yJEjwS9yku9DPS4uLuSg+v7772vbtm2qV6+e5/Z2795dU6dO1d///vccb3zv2bOnnnjiCdWpUyd4JqSodOjQQY8++qi2bNkSDBKZmZmaO3euzj333JBlUdgSExNDeq7zqrCX0/79+7Vo0aJg74WFIdo2Hj58OOTyYEnBHnED4uLidMEFF+i1117ThAkTgpcDffzxx9qyZUueQbJnz556/fXXlZycnO0SwPxo06aNMjMz9frrr4dcMjVnzpyohk9MTNSBAweylXfo0EGLFi3SgQMHgtvfgQMH9Oabb+b5kOrC2KamTZumffv2RX15nFdt27ZV+fLl9e2332rYsGE51gsEivAfsN54442optO4cWOlpqZq3bp1uuuuu6IaJjExUZ07d9bBgwfVv39/bd68WSkpKZ6Wa5s2bTRjxgytWrUqeHnr8ePHs/2A0aFDB0m+7WXs2LHB8pdeekmSQjpO69Spkx555BH97W9/U8eOHWVmql69us466yyNHz9emZmZeT7uqDjmXfJdTluqVClt27ZN3bp1y7FepPW7ceNGrVy5MluPtLGQ02dlJKVLl862jPKz/Z0oDh8+nO3ROrNmzcrxkstXXnklZPucM2eOSpUqFbwaJCD82L5y5Ur9+OOPatOmjaTot62CHptzUhI+z+rWravbbrtNL730Uono/TcSgiRQQn3xxRfavXu3jh07pm3btmnhwoV69dVX1a1bN02ZMiXH4RYuXKhnn31Wl156qerVq6dDhw7p8ccfV/ny5YMH6KZNm0qSHn74YfXq1UtxcXFq2bKlevbsqUcffVTDhw/XiBEjtHHjRk2aNCnbL4nR6tSpky6//HLdeuut+uGHH9S5c2elp6drxYoV6tOnjzp27KgxY8Zo7ty5uuiiizRmzBg1btxYhw4d0vr16/XBBx9E/UUyGmPGjNHMmTPVrVs3TZw4URUqVND06dO1cePGbN3QF7amTZvqgw8+0MKFC1WjRg2lpKR4OitWkOX00EMPacOGDerUqZNq1aqlrVu36qGHHtLPP/8c/CJbGKJtYyDAPPjgg7rwwgv1/vvv67XXXss2vokTJ6p79+669NJLNWrUKO3atUvjx4/P1ktgJFdffbVmzJihLl266LbbblPz5s117Ngxfffdd1qwYIHmz58f1Y8xAd26dVP79u01atQo7d69O9gzYLQf7k2bNtX06dM1d+5cNWjQQOXLl1fjxo117733auHCherSpYvuvPNOmZmmTZumw4cP67777stznHv27NHTTz+tli1bKikpKXhfXDQ6duyoQYMG6YorrtCtt96qCy+8UKVKldKWLVv01ltvadq0aWrUqFHU44ukQoUK+stf/qKbb75Zu3btUq9evVSxYkX99NNPWr58uTp27KjBgwerbdu2qlChgm6++WZNnDhRhw4d0uTJk5WSkqJ9+/blOR0z01NPPaX+/fvr2LFjuvLKK5WSkqIdO3boo48+Up06dXTrrbfqmWee0YoVK9S7d2/Vrl1bu3fv1pQpU1SrVq1gcPCyXIcNG6apU6fq97//vR588EFVr15dzzzzTLb7rc866ywNGjRIEyZMUEZGhtq2bau0tDRNmjRJgwYNCukR++KLL1ZcXJzee+89PfXUU8HyTp066cknn1SdOnVUv359z+uisOddkho0aKA777xTf/jDH7RhwwZ16NBBSUlJ+uGHH7RkyRKNHDlSnTp1UteuXRUfH6+hQ4fqtttu0/bt2zV+/HjVqVMn22OOiks0n5WRNG3aVIsWLVLPnj1VuXJl1apVS7Vq1Ypq+5N8Z+dHjBihpUuX5vljUUnQs2dPzZ8/X2PGjFHfvn316aef6vHHH8/xKqW33npLt99+u7p3765PPvlEEydO1NChQ7MdSw4cOBBybL/77rt15plnaujQoZKi37YKemzOSaw+z9q0aaN+/frp7LPPVnJyspYvX661a9fm+kNcTBVFDz6nyoteW2Mvmp6qTjSBns8Cr6SkJFenTh136aWXuldeeSXY42JAeK+t69evd1deeaVLTU11iYmJLiUlxfXq1cutWrUqOExGRoa76aabXLVq1ZyZOd+hwOfxxx93qampLikpybVs2dItWbLEdejQIaRXsUAPfkuWLInY9qw93KWnp7vJkye7M8880yUkJATbs379+mCdPXv2uFtuucWlpqa6hIQEV61aNde+ffsce3TMOm7l0GtrTr0url+/3vXv399VqFDBJSYmulatWrl///vfIXVy6tU2Us+rOS2LcN98841r3769K1OmjJPkhg0bluu0hg0b5urWrRtSlt/ltGDBAte2bVtXtWpVFx8f76pUqeIuueQS9/HHH+c6XE5yW77RtPHw4cPuhhtucCkpKS45Odn16dPHff/99xHX5csvv+waNWrkSpcu7Zo2bermzZuXbXvMyZEjR9z48eNd48aNXenSpV3lypVdy5Yt3fjx44PL28u2vHPnTjdw4ECXnJzsKlas6K655ho3f/78qHoG3L59u+vVq5dLTk7O1kvfqlWrXJcuXVy5cuVc2bJlXefOnaNaNwcPHnQDBw50lSpVcpKC24uXecrMzHSPPvqoO+ecc1xiYqKrUKGCO+ecc9ztt98e0sNj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",
                         "text/plain": [
                             "<Figure size 921.6x633.6 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -369,15 +369,15 @@
             "cell_type": "code",
             "execution_count": 13,
             "id": "bf07b649-d184-4ded-827b-d8ff3f9f4284",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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T7kvvfRSxB133JE0ZsyYyhEjRlS19hpdc801vc4777yim266aY/D4VClpaWGc845p9+QIUMqFyxYsDcwMNCVkZFh+f7775veX7G236eeemr/hlPD66anv/fee0GXX355n4kTJ5a88sorewGefvrp6ClTpvTfuHHj1j59+nT6FGhPT/F9EKgATgZKgDzgDq3110qpy4F5wAWea55oj+/2FAAwpnf4UY1uOl1OlmYsBeD24bdTvr17p8IbTWa8/QOoqiinqrycGpt7hNHXYGfvsgicVUYM/v5E/+1+AqdPP6KvMX37U5qXS/audMITerD562UADJky9bBygyfG88v/9pPxcx5lhTYCw36bspyxyf37LbxHMjk7Mzm4fUsTAepvI6gAfUaNISQ2nuKsg2z++n8MO/0sAKptNg5s/RVlMHDbhfdxV0AgP2UWsea1t/DPqUQbInACLsdBqq0OVr34GeecU40K7QlxaWDusg/IhBBCiDZxuVzUjYo1Pm63//b3sVIKk6njf976+fk5v/rqq91GozufTkpKStUZZ5zRf8GCBWFz5swpAHjsscdy6so7nU6mTZtWnpOTY/7Xv/4V0ZYA9cYbb8y7//778+qev/rqqyF2u1299tpr+0JDQ+umMnX4j59zzz23aNq0aSUJCQn2jIwMy3PPPRd99tln91uyZMmus88+u831Op1OHn/88djx48eXffjhh5l1xyMiIhw33nhjr5auXbt2rV9AQIBz8eLF9QNNF1xwQf2UsbS0tCp/f3+X0+k8Yir00KFDq1999dX66xwOB6ecckpF3759h3z44YdBV155ZUnD8rfddlvOHXfcUQhw3nnnla9duzbggw8+CL3jjjsKY2NjHb17964GGDlypHXQoEEtrsOdMmVK5fPPP++wWCy6qSnSQ4cOrXz//ff31T1fv36999KlS0PnzJmTXTfV/IILLigzGo08+eSTsT/88EPOSSedZKsrn5iYWP3xxx9nAsyYMaNs7dq1AUuWLAl78cUX995yyy1FAOPHj6+MiYkZ9u6774aMGDEiu6X2AkybNq345ZdfPlj3fM2aNb5lZWXGp5566mDDe99+++3NTlmu62tTU8PvvvvuhJEjR5avWLGiflbrWWedVda7d+/BjzzySHTD17izeDpAHQs8r7XerZSq27/DAKC1fkspdTLwBDC1uQrEsWPtbneAOu4os/f+mPMjudZc4vzjSI1MZc32NZ3RvHbxCw6hqqKcypJiqmuTGpkrqnFWGfEZnkrck09ijotr8tqYvsnsWLuarF07CIqMpjQ3h4DwCHoMTT2snH+IF31GRLLzx1w2rzzIuJl968/t/cX9+63vqOHk7FzGwe1HZtktrJ3iGxbvnrFhMBgZd9HlLH32Mb555zX6jDgJ/9AwMjb+iMvpJHHQkPo1piOSQhl2/228v243OUtW4rdPgyMHZS/jYE4Y8z6dz/mmNfQM7AnX/Q98Q4+4vxBCiN+XY3nksjWff/55wPTp0/s1Pv7cc8/FPPfcc/VTYUeOHFnx448/poM7sNH6t8E2g8FAXeDZnOnTpxc3LHP66adXRkVF2detW+cHFABs3rzZ669//WvsDz/8EFBYWGh2udwxpcViadN6xFmzZpU0fD5y5EiryWTS559/fq+rr7668PTTTy+Pi4vr8PrAJUuWHDZqd8kll5QMHDhw4N///vfYs88+O7256xrLyMiw5Obmmv/yl78canj86quvLr755ptb7OtJJ51UWVZWZjz33HN7zpo1q+i0006rCA8PbzVBUZ3HH388YvHixREHDhzwqhupBNixY8cRn5rPnDmztOHz5ORk25YtW7pkKti5555b0vD5ihUrAgCuvfbaw4K/6667rvDJJ5+MXb58eUDDIPG00047rK39+vWr+uqrrzjvvPPqg/eIiAhnaGio/eDBg23KiDxz5szihs8HDhxYHRAQ4Lzpppt63HjjjXmnn356eUdHOTdv3ux14MABr7lz52Y3/CAoICDAlZqaWrlu3bpmR2WPhqfXoHrz2xTeuk80Gs4N/QkY060tEh3idGnWZbjXSY7rc3SZdT/d8ykA5/Q+B4PyzFvULzgYgMrSEiprEySZbS5MIb4kLFzYbHAK7gAVIGf3Tn5d/gUAg085HYPhyF+KQ6e4Rz+3rc2mpsr9u6imUpO3rxyT2cDgycMxms0U7M/EVnH4h55FtSOoYXG/ZT/vN3ocvYaPpMZmZcXilwHY9aM7OVOfUWMPu95kNHDZuH7c8Y/H0SExaKWIObQEgIDMy3g9M5EbXaW89O7Z7MjbfNgveSGEEKI7jRs3rnL16tXbGz4iIiLss2bNKmh4bNGiRZl114wdOzbZYrGk1T3uuuuuVrd8iYqKOuIP+fDwcHt2drYFoLS01DB16tR+27Zt8/373/9+8Msvv9yxevXq7RdeeGFBTU1Nm6aPNZ5eOmjQoOqPP/54l8vlUjfffHPPhISEoUOGDOn/2Wefdcof/yEhIa5TTjmldPPmzX7tue7AgQNmgOjo6MOCZbPZXD8dtznTpk2rWLx4cUZWVpbliiuu6B0dHT107Nix/X744YdWM1w+/PDDkX/5y18SJ0yYUPbWW2/tWbVq1fYVK1bsAKiqqjriD8PIyMjD2mexWHRNTU2X/AEZFxd32GtXVFRkgiNf07rMv0VFRYf98RcSEnLYz63uQ42IiIjGP2PdVF+bEh8ff9i9w8LCnF9++WV6VFSU/e677+7Rt2/fIX379h342muvBbelvoays7NNAHPmzElq+G/JYrGkrVy5MqhuynZn8/QI6iEgHkBrXamUKgZSgf/Unu8NHHepnY9H27LKKLXZiQ/xISG06Q+tSqtLWXVgFWcknYG3qelpo5X2SpbvXw7A9F7Tu6q5rfINqt1qpqSY8vQtAHg7nMQ8cB9G/5Z/X0T06IWxNjNucfYhlDIwaPJpTZaN7BFITJ8gsneX8tXibVRV2MnZ6w4EEwaE4uPvQ0yfZA5u38KBLZvoN3o8ANXWSiqKCjGZLQRGRtbXp5RiynW3cGDbLexe/z3bv1lJ5qafAQ7b9qahIF8zw0eP5OcvP6VgYBRehTlUe0czYt/pJHz/CWtTSvhL3iWUJEVwUcqFXJZyGUFeQU3WJYQQQnSFkJAQ14QJE6wNj5nNZh0TE2NvfLzOokWLMktLS+sDhLZsgZKbm2tufKygoMA8cOBAK8DXX3/tn5WVZfnyyy/TzzjjjPo1nc8++2yb1zYZDIYjPvGdPn16+fTp08ttNpv66quv/P/xj3/EXnjhhX337NmzOSYm5qizrWrd9I4BLakLsnJycg6LF+x2OyUlJa3uKXrNNdcUX3PNNcWlpaWGzz//POD++++Pnz59et/s7OxfWxrJ/uijj0LHjBlTvmjRovppqzt27Gjz/qpdSSl12GsXGhrqAHcwP3DgwPrpw3XBfVhYWJdnym3qdR07dqxt2bJle+x2O2vWrPF75JFHoq+77rreAwcO3Dpy5MhW17XWiYiIcALcc889h6ZOnXpEVs+6ddmdzdMjqN8BUxo8Xwr8SSl1v1Lq78AfgW890jLRLmv31E3vbX709PWtr3Pf2vt4cN2DzZZZvm85NoeN1MhUEgI9ty9yXSbfiqJC8pZ+AkBwhAX/M85v9VqT2Uxkz94AuJxOeqWNJCC0+Z9L3Shq5q8F5GS4Z35E9QxkxFlJACQNc+e0yNi4vv6aokPu/7NDYuOOGJkNDI/g5EuvAuDLl57FUVNNTJ/kFtsQ13+gu75QC9Pud69d3Z94KuWBA+hbeDKX/nQtl3z1B7a9v5YzPprK/J/nU1JV0urPQgghhPCUoUOHVk+YMMFa90hKSmo1QP30009DGq51/d///ueXm5trHj16dCVAZWWlAdzBcV2Z/Px841dffRXcGW328fHR55xzTvncuXNzbDabYefOnUcdmBUVFRm+/vrroCFDhrRr25levXrVREdH13z00UeHrfN57bXXQpxOZ5uj3aCgINcll1xSevXVV+fn5+ebc3NzTQAWi8XV1CihzWYzmEymwwKfl19+ucPT8+qCqNYSO3XEqaeeWg7wxhtvHJbNc/HixaEAU6ZMqWjquu5iNpuZMmVK5SOPPJLlcrnYvHlzsyPYZrNZN5xODTB06NCq2NjYmm3btvk0/LdU92g4fbkzddoIqlLKiXtE9D6t9RttvOxF4DyllLfWugr4MzAc+Eft+R3AnM5qo+g63+1xT70f26f59aeZZZkAfLLnE6YmTeXk+JOPKPPJHncweE7vczq/ke1QF6AWrl5FpdUO3t5ETmv7UuiYvv3r90JtnBypsZ5DIxhxVhL2aifxySHsydnMlNNH1J/vnTaKb999nYyN63G5nBgMRgoP1mbwjU9sss5hp53F9m9Xkb1zB+BOoNSS+BR3gJq1cweRPfwYMC6GbWuz2TTk1sPKpWadS3DxP1lU8wrvbn2DV898k+Sw/lSWuj809AvqcMJBIYQQwuMqKyuNp512Wp8bb7wxPy8vz/Tggw/G9ejRo/qWW24pBDjllFMq/P39nbfffnvifffdl1VRUWF44oknYkJCQhwVFRWtjio25Yknnoj45ptv/M8888zSHj161OTn55ueeuqpmIiICHtaWpoN3NuU9O/ff3DDZDxN+dvf/ha1c+dO70mTJpXHx8fb9+7da5k/f35UQUGB+dVXX93b3HVNMRqN3H333dlz587tMXPmzKRLLrmkaOfOnV7PPvtsjL+/f4tTfGfPnh2bl5dnnjRpUllCQoJ93759loULF0b279/fVrf/ZnJyctWbb74ZsWjRopDk5OTqoKAg59ChQ6tPOeWU0pdeein6L3/5S/To0aMrly9fHrh06dIOb+cwZMgQG8Czzz4bce211xZaLBY9atQom7e391GP/o0YMaLq7LPPLnr66adjHQ6HGj9+fOXatWv9nn322Zizzz67qKsCuJa8++67QYsWLYo455xzinv37l1TUVFheOGFFyL9/PxcEydObDZg7t27d9Xy5cuD/vOf/5SFhYU5EhMT7UlJSfZnnnlm/2WXXdZ72rRp6sILLyyKiIhwZGdnm7/77jv/xMTEmgceeCC3s/vQmVN8DwB+wGtKqdla6+GtXaC1/hH4scHzHKXUEGAw4AR2aK3bvKBadI+KagcurQn0ds+CqXG4WL/Xvf50TAsJknIq65Pe8Y/v/8GSc5fgb/ltumxWRRY/5vyIxWDh9KTTu6j1LXNVVVHx9dfULPsfACVbt1Btdv++CRg4qc311K1DDQiLIGlYy/8UDAbFSef8lgwvs+jwDyXD4hPrt67J3rWTuOSUBhl845usUxkMnH7jH3nzz3fgcjro20qA6hccUp8B+O175jD+khs4mO5dHzTH8iM/rfOh0ieK07YMYtT+n3n4XPjrV3/gtTM/54MHN+Byamb+OY2Q6HYtcRFCCCGOGbNnz87evXu3180335xUVVVlOOmkk8pffvnl/XWjcLGxsY633357z5///OeEq6++undERETNTTfdlFdUVGSaN29eh/YtHT58uHXZsmWB//znP+OLiopMQUFBjhEjRlS8/fbbGf7+/hqgvLzcABAdHd3iKHD//v2rli5dGrJs2bLg8vJyo7+/v2v48OEVr7zySubkyZObnArdkjlz5hRUVFQYXnrppahPP/00tG/fvrY33ngj49prr+3Z0nWjR4+ufOGFFyLvvffehNLSUlNoaKhjwoQJpU888UR9cP33v/89e/fu3V6zZ89OslqthroEV48//nhWSUmJ8ZVXXomaP3++YdSoUeVffvnlzpSUlMHtbT/AmDFjbHPnzs168803I95///0Il8vFjh07NicnJ9d0pL7GPvzww8y77rqr+t133w1/7rnnYiIjI+233HJLzpNPPtlqBt6uMGDAgCofHx/Xk08+GVtQUGD29fV1DhkypPKTTz7Z2bt372bfP88999y+OXPmJM6aNatPTU2Nqvsw5OKLLy4NCwtLf/jhh2Nu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3vdshv+0mC1XXszA19/D6H/EUiIhhBCiW6xcuTLopptuip86dWrZunXrfJ955pnY888/v7Bu/elZZ51Vunjx4siZM2f2vPbaawt27Njh/fTTT8c0NXW3rS655JIe/v7+zrFjx1ZGR0fbt2/f7v3RRx+FjR8/vj6xzfPPPx92xx13JLW2lvacc87pmZSUVJ2WlmYNCQlxbtiwwff555+PjoyMrLn77rvzmruuKUOHDq2ePn160ZNPPhnrcrmoy+K7cuXKoNaunTJlSu/Bgwfb0tLSrKGhoY4NGzb4fvPNN4GXXnppfVbb3r17Vy1fvjzoP//5T1lYWJgjMTHRnpSUZB86dGjlSy+9FBUTE2OPiIhwvPrqq2G5ubkdXguUkpJie/fdd8Mff/zxiNGjR1f6+PjohutCj8att95a+Morr0RdcsklfRpm8f3uu+8Cn3zyyX0dyXB7tGbPnh2bl5dnnjRpUllCQoJ93759loULF0b279/f1tz07EGDBlUZjUb96quvhoeHhzu8vb314MGDqwYOHFh9880359xzzz2J6enp3pMmTSr38fFx7du3z7J8+fLAG264oWD69Omtru1uzNN/lc9s8H3/2kdjbVow3UjjpEsLar+uxp3MCa11pVLqFNz7kr6JOznSCmC21rrFjFgnohyrO9B02YMJ8//tQ8Aze57JUz89xY85P7KnZA+9g3sffl0XBai2XzfjqqjAkpSEOc49omvu0YPq7dupKbTiEx8CfhFU7XCPpoZdfz0l77+P9aefKHhxAdaffgKXi9CrrsJnsKw/7SoGgyI8PoCcDPea/0mX9ie6V/O/t/qMHE1ITBzF2YdIO306+76wUxKaxrY+B0jZupyfLj6b4W//B3NwuxJtCyGEEJ1i8eLFe5966qmoyy67rLfZbNazZs0qeOmll+qzoc6YMaPsoYceOrBgwYKoZcuWhfTp08e2cOHCvY888khsR+85duzYijfffDP8o48+CquoqDBGRETYL7jggqInn3zyUF2ZyspKAxy5RraxgQMH2j766KPQV199NdJmsxnCw8MdU6dOLXnssceyWlv72ZQ333xz3x/+8AfnSy+9FP3888+r0aNHl7/22msZZ5xxRlN/09cbP358xZIlS0Jee+21yKqqKkN0dHTNzTffnPvoo4/WZ4J97rnn9s2ZMydx1qxZfWpqatScOXOy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oYTQQwi9NynSFFBRsVw76EVAUa+iqIgFQQUUC5/YCyqKiigiTVApgiIIhB5KKOm9zcz+/pgEA4SQQWAo632e85A558zea88EmDW7GZRLFzMXQghRA3a7nap6bux2O2VlZcceK6UwmZz5eHs8Ly8v2+LFi3dWfFhv1KhRcZ8+fRrOmjUraOzYsekAzz///OGK+202G/379887fPiw+e233w6pSYJ61113HX388cePTZV75513AsrKytS7776bEhgYWJGw5Z1pGwYPHpzZv3//7Fq1apXt3r3bMn369PABAwY0mD9//o4BAwbUuNykpKRib29vu81mO2m48sSJEyPMZrN9xYoV24ODg20AgwYNyq1Tp07ziRMnRv7444+7rFYrzz33XFSbNm3yFixYcCzpatKkSXHfvn3jZ86cGTxhwoQTpwwCjqGoc+fOLYWTh0rPnTs3peJnq9XKsGHDcuLi4pq+8cYbwW3btt1f+d6EhISCyvdXpV69emVFRUWF5T+XnFhfdna2acGCBVs6dOhwLOns27dv3dO1v+LegoICw6uvvppSMXS4Vq1aZe3atWu8ePFi/507d26u+H3dvHmzx7vvvhtqtVpP+zucl5dn/P3337fExMQcGxK2du1a706dOuVW/t264YYbcqprd1RUVBlA9+7dC8zmf/oZ33rrrcANGzZ4L1y4MLki7sGDB+cBvPTSS5FPPvnk4aioqHM2HM2Zv8FzgbFKqU9xzEGF8qG+Sqk7gCHAI07W7w0scPI54jwK9QzlurDZTF+STEgP57aYqWCJjaVwzRpK9+yB0HzY+RO4+UGPJ0ApGDQT0pLhyCb4+l4Y/tEpy7KmOkZ8m9ztkHgT/PEBfPEfsJWBwQSBdc8oRnHxq58USmlxQ5Z9uI3fvtpFabGVTcsPOq61bMP21T9gK9vNwdB4GiUrbO/8wiPufXjquvl4WLxOU7oQQlz8LuSey9NZuHChz8CBA0/aLWL69OkR06dPPzYUtnXr1vlr165NBkfyovU/s9IMBgOnm8s4cODArMr39O7duyAsLKxs9erVXkA6wKZNm9weffTRyDVr1vhkZGSY7XZHTmmxWGo0L3H48OHZlR+3bt260GQy6auvvrrurbfemtG7d++8f/Phf/78+cdNj7v++uuzmzRp0mTixImRAwYMSD7Tcitbu3atT48ePXIqkjOAwMBA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uabuX3/9te1M2nEirfVZWxshODjYCnDo0KGTlrJNT083N2vWrAD+ScD2799vbtKkybH3af/+/WaAoKCgGg83rjBv3rzA9u3b582ePftYL/G2bdssp7rfYDD866mGJ75nNW3/uVTVexkVFWX94IMP9gH7Nm7c6DZ79uzgadOmRYaEhFgffvjh0w4brszf39/WunXrvP/973+Hq7peu3btf5X4O/2VvdY6W2s9V2v9gtb6ea31Z/8mOVVKxSmlXlNKrVNK7VRK7T7h2HWmZYtLg/bwwFSepEoPqriQWdxNdL+xIZFx/sedv6JffZQRtKElBqWwGuxoezaUOealbltd5b/vQgghLjCffvppQOXH77//foDBYKBTp04FAIWFhQaDwXBc4vPNN9/4HDp06JRJkjNCQkJsd955Z9bAgQMzd+zY4XE2yvz55589U1JS3Fu1auV04mQ2m3XlYbQACQkJxUFBQdbPP//8uNdq8eLFXqmpqZbOnTvnA/Tq1SsPHK9h5fvmzJkTCNCzZ898Z+MpKioymEym4xLGN95447zOo6lp+10pISGh5NVXXz3o6+trq9hCpyoWi8VeVc9z165dc7Zu3erZsmXLoi5duhSeePzbrZGcXv1LKdUNuAIIBaZprbcppbyB5sDfWusaT4pVSiUCPwNmHHNa6wJ/AwFAJI7e2dMtvCQuA56tW5H77QLc4+JcHYoQTrN4mPCLgew9Ckz1oWwHfmmLabp3E7+1m8SO9al0uyEei8c//yTv/jONtH15tB5QB4NBVvwVQogLwbJly/zuvvvu6L59++auXr3a86WXXoq8+uqrMyrmn1555ZU5c+bMCR02bFid2267LX3btm3u06ZNi6hq6G5NXX/99bW9vb1tHTp0KAgPDy/bunWr+7x584I6dep0bI5ixf6up5tLO2jQoDqxsbElSUlJhQEBAbb169d7zpgxIzw0NLT0oYceqnaxoKrUq1ev+KeffvL76quvcoOCgqwxMTFlsbGxZY888sjB8ePH1x48eHCdm266KWP//v2WyZMnR9WuXbvkvvvuSwdo1apV8YABAzKnTZsWabVaVadOnQp++eUXr1deeSViwIABmWcy/7RHjx45r7/+evgjjzwS3q5du4KffvrJd8GCBQGnf+bZYzKZqEn7z6eMjAxj165dG1x77bUZjRs3Ljabzfqrr77yz83N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tT7t+/Dhhx/633rrrfUSExPzp02blhIaGmrdtGmTR0pKyimXj1+zZo1Hv379GtarV6/otdde26uU0lOnTo3o169fw2XLlm1t3759UU5OjmHQoEENmjdvXjBr1qw9vr6+9t27d1t+++23Y0nYzp07zR06dGgUFBRknTx58v6wsDDrp59+GnjrrbfWMxqNO2+88cacquq/99570w4ePGj+7LPPghctWrSt8hDf3NxcQ9euXeNzcnKMjz322MGYmJjSDz/8MOjee++tU1hYaHjwwQdPu2PJ+PHjY7p3754ze/bsPUVFRQaAQYMGxfn4+NheeumllJCQEOv+/fst33//vZ/NZlNms/mkHtbPPvts51VXXRXXsGHDoieffDIVIDw83AqwatUqzyuuuCK+cePGhdOnT0/x9PS0v/nmmyGDBg1qsGTJkm2dO3cuPF2MF7vqEtQyoPIvXzfg/85m5Vrr2LNZnhBCXC68/AMYNPZ+Zo+tS3H2T9ite9lUJ4COW49gHzeZHbsPE3evzEkVQlwa7HY7VS14Y7fbqeilAseUCJPJmRlsx/Py8rItXrx4Z0VS06hRo+I+ffo0nDVrVtDYsWPTAZ5//vnDFffbbDb69++fd/jwYfPbb78dUpME9a677jr6+OOPH+uMeeeddwLKysrUu+++mxIYGGgvP513pm0YPHhwZv/+/bNr1apVtnv3bsv06dPDBwwY0GD+/Pk7BgwYUONy7XY7Dz/8cK2GDRsWrl69OrniNbnqqquqLWPixIkRZrPZvmLFiu3BwcE2gEGDBuXWqVOn+cSJEyN//PHHXRs3bnTPzc01Tp069UDbtm2PzcscPXp0RsXPjz76aKTWmpUrV24LDw+3AQwdOjS3Q4cO5kmTJkWdKkGtV69eWVRUVBlA9+7dC8xm87Frr776alBKSorbt99+u73itbj22mtzO3ToYH722WejxowZk36635+EhISCuXPnplQ8PnTokCklJcXtww8/PC5pvueeezJPVUbHjh2LLBaLDgwMtJ449Hf8+PHRERERpb/88st2d3d3Xd7unAYNGjR56qmnIn766add1QZ4CajuHdgJ3KSU2gBUvNhBSqmYap5TMa9TCCHEOWayGKmXWJ/taw2U5s4mx+LFylYWOv9einXm22wpyKPxQ0+5OkwhxAXiQu65PJ2FCxf6DBw4sMGJ56dPnx4x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Bg4cmDVq1Khdq1ev9nr55ZcjCgsLDfPmzdtbcU9qaqr53nvvPRITE1OWn59v+Oijj4L69u0bv2rVqq1t27atdkjvnj173MePHx8zfvz41Pr165eGhIRYX3/99cCnnnqq1pgxY1K7du2aX1hYaNi4caNHRkaGM5/jj3P77bfXHTp0qMnHx8fWuXPnnJdeeulgXFxcacX10aNHZ4wePfq0w1/vuuuu6NmzZ4dde+216RMmTEg1GAz89ttvXnv27LEAVfYITp06NXj8+PG1+/fvn/X0008fPHjwoPmZZ56J6tq1a/zGjRu3+Pn52RctWuQ9atSoOrfeeuvR5557br/dbldbtmxxz87OPtbmTz/91G/EiBH1u3btmv3mm2/uAZg2bVp4z549G27YsOHv+vXrl1VV/+uvv55y00031bHZbGrWrFkpAP7+/jaANWvWePTr169hvXr1il577bW9Sik9derUiH79+jVctmzZ1vbt2592SPaQIUPq33jjjekPPfTQYYPBwJYtWyzXX399/b59+2Y99thjqRaLRScnJ7vt3r3brarnx8TElL333nu7brnllnr33nvv4auvvjoboFGjRiUAU6ZMCXn44Ydjhg0blvHoo48eys3NNTz33HOR3bp1i9+8efPfAQEBzuZjFxxnfrHXAzcqpV7UWh/35iilPIAbyu9xRjDwbTXXvwY6O1mmEEIIJ0U2aMiGhV+Tun0r7Yddz7Z2FnYvXUqJzmJT7do0X7mS3IUL8evf39WhCiEuQ3a7HZvNVuX5srJ/8hClFCbTPx9vrVYrWuvj7geOew6A0WjEYDj9wMLu3bvnvPXWWwcAhgwZkluewET99ddfh5o3b14CMHfu3JTK9Q8bNiwnLi6u6RtvvBHctm3b/dWVn52dbVqwYMGWDh06HPus/dprr4U0aNCgcOrUqYcqzl133XU5VZdQvYCAAOudd955pFu3bnl+fn629evXe77yyisRHTt29Pnjjz+2REVFWWta1ubNm93efvvtsNtvv/3I//3f/x2oOD98+PBTxma1Wnnuueei2rRpk7dgwYLdFeebNGlS3Ldv3/iZM2cGT5gw4egvv/zi5ePjY5szZ86x12vIkCG5lct66KGHarVu3TpvyZIluyrOXXnllbn16tVr9uyzz4ZXfm5lSUlJxd7e3nabzcaJw2onTpwYYTab7StWrNge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\n",
+                        "image/png": "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T7kvvfRSxB133JE0ZsyYyhEjRlS19hpdc801vc4777yim266aY/D4VClpaWGc845p9+QIUMqFyxYsDcwMNCVkZFh+f7775veX7G236eeemr/hlPD66anv/fee0GXX355n4kTJ5a88sorewGefvrp6ClTpvTfuHHj1j59+nT6FGhPT/F9EKgATgZKgDzgDq3110qpy4F5wAWea55oj+/2FAAwpnf4UY1uOl1OlmYsBeD24bdTvr17p8IbTWa8/QOoqiinqrycGpt7hNHXYGfvsgicVUYM/v5E/+1+AqdPP6KvMX37U5qXS/audMITerD562UADJky9bBygyfG88v/9pPxcx5lhTYCw36bspyxyf37LbxHMjk7Mzm4fUsTAepvI6gAfUaNISQ2nuKsg2z++n8MO/0sAKptNg5s/RVlMHDbhfdxV0AgP2UWsea1t/DPqUQbInACLsdBqq0OVr34GeecU40K7QlxaWDusg/IhBBCiDZxuVzUjYo1Pm63//b3sVIKk6njf976+fk5v/rqq91GozufTkpKStUZZ5zRf8GCBWFz5swpAHjsscdy6so7nU6mTZtWnpOTY/7Xv/4V0ZYA9cYbb8y7//778+qev/rqqyF2u1299tpr+0JDQ+umMnX4j59zzz23aNq0aSUJCQn2jIwMy3PPPRd99tln91uyZMmus88+u831Op1OHn/88djx48eXffjhh5l1xyMiIhw33nhjr5auXbt2rV9AQIBz8eLF9QNNF1xwQf2UsbS0tCp/f3+X0+k8Yir00KFDq1999dX66xwOB6ecckpF3759h3z44YdBV155ZUnD8rfddlvOHXfcUQhw3nnnla9duzbggw8+CL3jjjsKY2NjHb17964GGDlypHXQoEEtrsOdMmVK5fPPP++wWCy6qSnSQ4cOrXz//ff31T1fv36999KlS0PnzJmTXTfV/IILLigzGo08+eSTsT/88EPOSSedZKsrn5iYWP3xxx9nAsyYMaNs7dq1AUuWLAl78cUX995yyy1FAOPHj6+MiYkZ9u6774aMGDEiu6X2AkybNq345ZdfPlj3fM2aNb5lZWXGp5566mDDe99+++3NTlmu62tTU8PvvvvuhJEjR5avWLGiflbrWWedVda7d+/BjzzySHTD17izeDpAHQs8r7XerZSq27/DAKC1fkspdTLwBDC1uQrEsWPtbneAOu4os/f+mPMjudZc4vzjSI1MZc32NZ3RvHbxCw6hqqKcypJiqmuTGpkrqnFWGfEZnkrck09ijotr8tqYvsnsWLuarF07CIqMpjQ3h4DwCHoMTT2snH+IF31GRLLzx1w2rzzIuJl968/t/cX9+63vqOHk7FzGwe1HZtktrJ3iGxbvnrFhMBgZd9HlLH32Mb555zX6jDgJ/9AwMjb+iMvpJHHQkPo1piOSQhl2/228v243OUtW4rdPgyMHZS/jYE4Y8z6dz/mmNfQM7AnX/Q98Q4+4vxBCiN+XY3nksjWff/55wPTp0/s1Pv7cc8/FPPfcc/VTYUeOHFnx448/poM7sNH6t8E2g8FAXeDZnOnTpxc3LHP66adXRkVF2detW+cHFABs3rzZ669//WvsDz/8EFBYWGh2udwxpcViadN6xFmzZpU0fD5y5EiryWTS559/fq+rr7668PTTTy+Pi4vr8PrAJUuWHDZqd8kll5QMHDhw4N///vfYs88+O7256xrLyMiw5Obmmv/yl78canj86quvLr755ptb7OtJJ51UWVZWZjz33HN7zpo1q+i0006rCA8PbzVBUZ3HH388YvHixREHDhzwqhupBNixY8cRn5rPnDmztOHz5ORk25YtW7pkKti5555b0vD5ihUrAgCuvfbaw4K/6667rvDJJ5+MXb58eUDDIPG00047rK39+vWr+uqrrzjvvPPqg/eIiAhnaGio/eDBg23KiDxz5szihs8HDhxYHRAQ4Lzpppt63HjjjXmnn356eUdHOTdv3ux14MABr7lz52Y3/CAoICDAlZqaWrlu3bpmR2WPhqfXoHrz2xTeuk80Gs4N/QkY060tEh3idGnWZbjXSY7rc3SZdT/d8ykA5/Q+B4PyzFvULzgYgMrSEiprEySZbS5MIb4kLFzYbHAK7gAVIGf3Tn5d/gUAg085HYPhyF+KQ6e4Rz+3rc2mpsr9u6imUpO3rxyT2cDgycMxms0U7M/EVnH4h55FtSOoYXG/ZT/vN3ocvYaPpMZmZcXilwHY9aM7OVOfUWMPu95kNHDZuH7c8Y/H0SExaKWIObQEgIDMy3g9M5EbXaW89O7Z7MjbfNgveSGEEKI7jRs3rnL16tXbGz4iIiLss2bNKmh4bNGiRZl114wdOzbZYrGk1T3uuuuuVrd8iYqKOuIP+fDwcHt2drYFoLS01DB16tR+27Zt8/373/9+8Msvv9yxevXq7RdeeGFBTU1Nm6aPNZ5eOmjQoOqPP/54l8vlUjfffHPPhISEoUOGDOn/2Wefdcof/yEhIa5TTjmldPPmzX7tue7AgQNmgOjo6MOCZbPZXD8dtznTpk2rWLx4cUZWVpbliiuu6B0dHT107Nix/X744YdWM1w+/PDDkX/5y18SJ0yYUPbWW2/tWbVq1fYVK1bsAKiqqjriD8PIyMjD2mexWHRNTU2X/AEZFxd32GtXVFRkgiNf07rMv0VFRYf98RcSEnLYz63uQ42IiIjGP2PdVF+bEh8ff9i9w8LCnF9++WV6VFSU/e677+7Rt2/fIX379h342muvBbelvoays7NNAHPmzElq+G/JYrGkrVy5MqhuynZn8/QI6iEgHkBrXamUKgZSgf/Unu8NHHepnY9H27LKKLXZiQ/xISG06Q+tSqtLWXVgFWcknYG3qelpo5X2SpbvXw7A9F7Tu6q5rfINqt1qpqSY8vQtAHg7nMQ8cB9G/5Z/X0T06IWxNjNucfYhlDIwaPJpTZaN7BFITJ8gsneX8tXibVRV2MnZ6w4EEwaE4uPvQ0yfZA5u38KBLZvoN3o8ANXWSiqKCjGZLQRGRtbXp5RiynW3cGDbLexe/z3bv1lJ5qafAQ7b9qahIF8zw0eP5OcvP6VgYBRehTlUe0czYt/pJHz/CWtTSvhL3iWUJEVwUcqFXJZyGUFeQU3WJYQQQnSFkJAQ14QJE6wNj5nNZh0TE2NvfLzOokWLMktLS+sDhLZsgZKbm2tufKygoMA8cOBAK8DXX3/tn5WVZfnyyy/TzzjjjPo1nc8++2yb1zYZDIYjPvGdPn16+fTp08ttNpv66quv/P/xj3/EXnjhhX337NmzOSYm5qizrWrd9I4BLakLsnJycg6LF+x2OyUlJa3uKXrNNdcUX3PNNcWlpaWGzz//POD++++Pnz59et/s7OxfWxrJ/uijj0LHjBlTvmjRovppqzt27Gjz/qpdSSl12GsXGhrqAHcwP3DgwPrpw3XBfVhYWJdnym3qdR07dqxt2bJle+x2O2vWrPF75JFHoq+77rreAwcO3Dpy5MhW17XWiYiIcALcc889h6ZOnXpEVs+6ddmdzdMjqN8BUxo8Xwr8SSl1v1Lq78AfgW890jLRLmv31E3vbX709PWtr3Pf2vt4cN2DzZZZvm85NoeN1MhUEgI9ty9yXSbfiqJC8pZ+AkBwhAX/M85v9VqT2Uxkz94AuJxOeqWNJCC0+Z9L3Shq5q8F5GS4Z35E9QxkxFlJACQNc+e0yNi4vv6aokPu/7NDYuOOGJkNDI/g5EuvAuDLl57FUVNNTJ/kFtsQ13+gu75QC9Pud69d3Z94KuWBA+hbeDKX/nQtl3z1B7a9v5YzPprK/J/nU1JV0urPQgghhPCUoUOHVk+YMMFa90hKSmo1QP30009DGq51/d///ueXm5trHj16dCVAZWWlAdzBcV2Z/Px841dffRXcGW328fHR55xzTvncuXNzbDabYefOnUcdmBUVFRm+/vrroCFDhrRr25levXrVREdH13z00UeHrfN57bXXQpxOZ5uj3aCgINcll1xSevXVV+fn5+ebc3NzTQAWi8XV1CihzWYzmEymwwKfl19+ucPT8+qCqNYSO3XEqaeeWg7wxhtvHJbNc/HixaEAU6ZMqWjquu5iNpuZMmVK5SOPPJLlcrnYvHlzsyPYZrNZN5xODTB06NCq2NjYmm3btvk0/LdU92g4fbkzddoIqlLKiXtE9D6t9RttvOxF4DyllLfWugr4MzAc+Eft+R3AnM5qo+g63+1xT70f26f59aeZZZkAfLLnE6YmTeXk+JOPKPPJHncweE7vczq/ke1QF6AWrl5FpdUO3t5ETmv7UuiYvv3r90JtnBypsZ5DIxhxVhL2aifxySHsydnMlNNH1J/vnTaKb999nYyN63G5nBgMRgoP1mbwjU9sss5hp53F9m9Xkb1zB+BOoNSS+BR3gJq1cweRPfwYMC6GbWuz2TTk1sPKpWadS3DxP1lU8wrvbn2DV898k+Sw/lSWuj809AvqcMJBIYQQwuMqKyuNp512Wp8bb7wxPy8vz/Tggw/G9ejRo/qWW24pBDjllFMq/P39nbfffnvifffdl1VRUWF44oknYkJCQhwVFRWtjio25Yknnoj45ptv/M8888zSHj161OTn55ueeuqpmIiICHtaWpoN3NuU9O/ff3DDZDxN+dvf/ha1c+dO70mTJpXHx8fb9+7da5k/f35UQUGB+dVXX93b3HVNMRqN3H333dlz587tMXPmzKRLLrmkaOfOnV7PPvtsjL+/f4tTfGfPnh2bl5dnnjRpUllCQoJ93759loULF0b279/fVrf/ZnJyctWbb74ZsWjRopDk5OTqoKAg59ChQ6tPOeWU0pdeein6L3/5S/To0aMrly9fHrh06dIOb+cwZMgQG8Czzz4bce211xZaLBY9atQom7e391GP/o0YMaLq7LPPLnr66adjHQ6HGj9+fOXatWv9nn322Zizzz67qKsCuJa8++67QYsWLYo455xzinv37l1TUVFheOGFFyL9/PxcEydObDZg7t27d9Xy5cuD/vOf/5SFhYU5EhMT7UlJSfZnnnlm/2WXXdZ72rRp6sILLyyKiIhwZGdnm7/77jv/xMTEmgceeCC3s/vQmVN8DwB+wGtKqdla6+GtXaC1/hH4scHzHKXUEGAw4AR2aK3bvKBadI+KagcurQn0ds+CqXG4WL/Xvf50TAsJknIq65Pe8Y/v/8GSc5fgb/ltumxWRRY/5vyIxWDh9KTTu6j1LXNVVVHx9dfULPsfACVbt1Btdv++CRg4qc311K1DDQiLIGlYy/8UDAbFSef8lgwvs+jwDyXD4hPrt67J3rWTuOSUBhl845usUxkMnH7jH3nzz3fgcjro20qA6hccUp8B+O175jD+khs4mO5dHzTH8iM/rfOh0ieK07YMYtT+n3n4XPjrV3/gtTM/54MHN+Byamb+OY2Q6HYtcRFCCCGOGbNnz87evXu3180335xUVVVlOOmkk8pffvnl/XWjcLGxsY633357z5///OeEq6++undERETNTTfdlFdUVGSaN29eh/YtHT58uHXZsmWB//znP+OLiopMQUFBjhEjRlS8/fbbGf7+/hqgvLzcABAdHd3iKHD//v2rli5dGrJs2bLg8vJyo7+/v2v48OEVr7zySubkyZObnArdkjlz5hRUVFQYXnrppahPP/00tG/fvrY33ngj49prr+3Z0nWjR4+ufOGFFyLvvffehNLSUlNoaKhjwoQJpU888UR9cP33v/89e/fu3V6zZ89OslqthroEV48//nhWSUmJ8ZVXXomaP3++YdSoUeVffvnlzpSUlMHtbT/AmDFjbHPnzs168803I95///0Il8vFjh07NicnJ9d0pL7GPvzww8y77rqr+t133w1/7rnnYiIjI+233HJLzpNPPtlqBt6uMGDAgCofHx/Xk08+GVtQUGD29fV1DhkypPKTTz7Z2bt372bfP88999y+OXPmJM6aNatPTU2Nqvsw5OKLLy4NCwtLf/jhh2Nu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3vdshv+0mC1XXszA19/D6H/EUiIhhBCiW6xcuTLopptuip86dWrZunXrfJ955pnY888/v7Bu/elZZ51Vunjx4siZM2f2vPbaawt27Njh/fTTT8c0NXW3rS655JIe/v7+zrFjx1ZGR0fbt2/f7v3RRx+FjR8/vj6xzfPPPx92xx13JLW2lvacc87pmZSUVJ2WlmYNCQlxbtiwwff555+PjoyMrLn77rvzmruuKUOHDq2ePn160ZNPPhnrcrmoy+K7cuXKoNaunTJlSu/Bgwfb0tLSrKGhoY4NGzb4fvPNN4GXXnppfVbb3r17Vy1fvjzoP//5T1lYWJgjMTHRnpSUZB86dGjlSy+9FBUTE2OPiIhwvPrqq2G5ubkdXguUkpJie/fdd8Mff/zxiNGjR1f6+PjohutCj8att95a+Morr0RdcsklfRpm8f3uu+8Cn3zyyX0dyXB7tGbPnh2bl5dnnjRpUllCQoJ93759loULF0b279/f1tz07EGDBlUZjUb96quvhoeHhzu8vb314MGDqwYOHFh9880359xzzz2J6enp3pMmTSr38fFx7du3z7J8+fLAG264oWD69Omtru1uzNN/lc9s8H3/2kdjbVow3UjjpEsLar+uxp3MCa11pVLqFNz7kr6JOznSCmC21rrFjFgnohyrO9B02YMJ8//tQ8Aze57JUz89xY85P7KnZA+9g3sffl0XBai2XzfjqqjAkpSEOc49omvu0YPq7dupKbTiEx8CfhFU7XCPpoZdfz0l77+P9aefKHhxAdaffgKXi9CrrsJnsKw/7SoGgyI8PoCcDPea/0mX9ie6V/O/t/qMHE1ITBzF2YdIO306+76wUxKaxrY+B0jZupyfLj6b4W//B3NwuxJtCyGEEJ1i8eLFe5966qmoyy67rLfZbNazZs0qeOmll+qzoc6YMaPsoYceOrBgwYKoZcuWhfTp08e2cOHCvY888khsR+85duzYijfffDP8o48+CquoqDBGRETYL7jggqInn3zyUF2ZyspKAxy5RraxgQMH2j766KPQV199NdJmsxnCw8MdU6dOLXnssceyWlv72ZQ333xz3x/+8AfnSy+9FP3888+r0aNHl7/22msZZ5xxRlN/09cbP358xZIlS0Jee+21yKqqKkN0dHTNzTffnPvoo4/WZ4J97rnn9s2ZMydx1qxZfWpqatScOXOy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oYTQQwi9NynSFFBRsVw76EVAUa+iqIgFQQUUC5/YCyqKiigiTVApgiIIhB5KKOm9zcz+/pgEA4SQQWAo632e85A558zea88EmDW7GZRLFzMXQghRA3a7nap6bux2O2VlZcceK6UwmZz5eHs8Ly8v2+LFi3dWfFhv1KhRcZ8+fRrOmjUraOzYsekAzz///OGK+202G/379887fPiw+e233w6pSYJ61113HX388cePTZV75513AsrKytS7776bEhgYWJGw5Z1pGwYPHpzZv3//7Fq1apXt3r3bMn369PABAwY0mD9//o4BAwbUuNykpKRib29vu81mO2m48sSJEyPMZrN9xYoV24ODg20AgwYNyq1Tp07ziRMnRv7444+7rFYrzz33XFSbNm3yFixYcCzpatKkSXHfvn3jZ86cGTxhwoQTpwwCjqGoc+fOLYWTh0rPnTs3peJnq9XKsGHDcuLi4pq+8cYbwW3btt1f+d6EhISCyvdXpV69emVFRUWF5T+XnFhfdna2acGCBVs6dOhwLOns27dv3dO1v+LegoICw6uvvppSMXS4Vq1aZe3atWu8ePFi/507d26u+H3dvHmzx7vvvhtqtVpP+zucl5dn/P3337fExMQcGxK2du1a706dOuVW/t264YYbcqprd1RUVBlA9+7dC8zmf/oZ33rrrcANGzZ4L1y4MLki7sGDB+cBvPTSS5FPPvnk4aioqHM2HM2Zv8FzgbFKqU9xzEGF8qG+Sqk7gCHAI07W7w0scPI54jwK9QzlurDZTF+STEgP57aYqWCJjaVwzRpK9+yB0HzY+RO4+UGPJ0ApGDQT0pLhyCb4+l4Y/tEpy7KmOkZ8m9ztkHgT/PEBfPEfsJWBwQSBdc8oRnHxq58USmlxQ5Z9uI3fvtpFabGVTcsPOq61bMP21T9gK9vNwdB4GiUrbO/8wiPufXjquvl4WLxOU7oQQlz8LuSey9NZuHChz8CBA0/aLWL69OkR06dPPzYUtnXr1vlr165NBkfyovU/s9IMBgOnm8s4cODArMr39O7duyAsLKxs9erVXkA6wKZNm9weffTRyDVr1vhkZGSY7XZHTmmxWGo0L3H48OHZlR+3bt260GQy6auvvrrurbfemtG7d++8f/Phf/78+cdNj7v++uuzmzRp0mTixImRAwYMSD7Tcitbu3atT48ePXIqkjOAwMBA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uabuX3/9te1M2nEirfVZWxshODjYCnDo0KGTlrJNT083N2vWrAD+ScD2799vbtKkybH3af/+/WaAoKCgGg83rjBv3rzA9u3b582ePftYL/G2bdssp7rfYDD866mGJ75nNW3/uVTVexkVFWX94IMP9gH7Nm7c6DZ79uzgadOmRYaEhFgffvjh0w4brszf39/WunXrvP/973+Hq7peu3btf5X4O/2VvdY6W2s9V2v9gtb6ea31Z/8mOVVKxSmlXlNKrVNK7VRK7T7h2HWmZYtLg/bwwFSepEoPqriQWdxNdL+xIZFx/sedv6JffZQRtKElBqWwGuxoezaUOealbltd5b/vQgghLjCffvppQOXH77//foDBYKBTp04FAIWFhQaDwXBc4vPNN9/4HDp06JRJkjNCQkJsd955Z9bAgQMzd+zY4XE2yvz55589U1JS3Fu1auV04mQ2m3XlYbQACQkJxUFBQdbPP//8uNdq8eLFXqmpqZbOnTvnA/Tq1SsPHK9h5fvmzJkTCNCzZ898Z+MpKioymEym4xLGN95447zOo6lp+10pISGh5NVXXz3o6+trq9hCpyoWi8VeVc9z165dc7Zu3erZsmXLoi5duhSeePzbrZGcXv1LKdUNuAIIBaZprbcppbyB5sDfWusaT4pVSiUCPwNmHHNa6wJ/AwFAJI7e2dMtvCQuA56tW5H77QLc4+JcHYoQTrN4mPCLgew9Ckz1oWwHfmmLabp3E7+1m8SO9al0uyEei8c//yTv/jONtH15tB5QB4NBVvwVQogLwbJly/zuvvvu6L59++auXr3a86WXXoq8+uqrMyrmn1555ZU5c+bMCR02bFid2267LX3btm3u06ZNi6hq6G5NXX/99bW9vb1tHTp0KAgPDy/bunWr+7x584I6dep0bI5ixf6up5tLO2jQoDqxsbElSUlJhQEBAbb169d7zpgxIzw0NLT0oYceqnaxoKrUq1ev+KeffvL76quvcoOCgqwxMTFlsbGxZY888sjB8ePH1x48eHCdm266KWP//v2WyZMnR9WuXbvkvvvuSwdo1apV8YABAzKnTZsWabVaVadOnQp++eUXr1deeSViwIABmWcy/7RHjx45r7/+evgjjzwS3q5du4KffvrJd8GCBQGnf+bZYzKZqEn7z6eMjAxj165dG1x77bUZjRs3Ljabzfqrr77yz83N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tT7t+/Dhhx/633rrrfUSExPzp02blhIaGmrdtGmTR0pKyimXj1+zZo1Hv379GtarV6/otdde26uU0lOnTo3o169fw2XLlm1t3759UU5OjmHQoEENmjdvXjBr1qw9vr6+9t27d1t+++23Y0nYzp07zR06dGgUFBRknTx58v6wsDDrp59+GnjrrbfWMxqNO2+88cacquq/99570w4ePGj+7LPPghctWrSt8hDf3NxcQ9euXeNzcnKMjz322MGYmJjSDz/8MOjee++tU1hYaHjwwQdPu2PJ+PHjY7p3754ze/bsPUVFRQaAQYMGxfn4+NheeumllJCQEOv+/fst33//vZ/NZlNms/mkHtbPPvts51VXXRXXsGHDoieffDIVIDw83AqwatUqzyuuuCK+cePGhdOnT0/x9PS0v/nmmyGDBg1qsGTJkm2dO3cuPF2MF7vqEtQyoPIvXzfg/85m5Vrr2LNZnhBCXC68/AMYNPZ+Zo+tS3H2T9ite9lUJ4COW49gHzeZHbsPE3evzEkVQlwa7HY7VS14Y7fbqeilAseUCJPJmRlsx/Py8rItXrx4Z0VS06hRo+I+ffo0nDVrVtDYsWPTAZ5//vnDFffbbDb69++fd/jwYfPbb78dUpME9a677jr6+OOPH+uMeeeddwLKysrUu+++mxIYGGgvP513pm0YPHhwZv/+/bNr1apVtnv3bsv06dPDBwwY0GD+/Pk7BgwYUONy7XY7Dz/8cK2GDRsWrl69OrniNbnqqquqLWPixIkRZrPZvmLFiu3BwcE2gEGDBuXWqVOn+cSJEyN//PHHXRs3bnTPzc01Tp069UDbtm2PzcscPXp0RsXPjz76aKTWmpUrV24LDw+3AQwdOjS3Q4cO5kmTJkWdKkGtV69eWVRUVBlA9+7dC8xm87Frr776alBKSorbt99+u73itbj22mtzO3ToYH722WejxowZk36635+EhISCuXPnplQ8PnTokCklJcXtww8/PC5pvueeezJPVUbHjh2LLBaLDgwMtJ449Hf8+PHRERERpb/88st2d3d3Xd7unAYNGjR56qmnIn766add1QZ4CajuHdgJ3KSU2gBUvNhBSqmYap5TMa9TCCHEOWayGKmXWJ/taw2U5s4mx+LFylYWOv9einXm22wpyKPxQ0+5OkwhxAXiQu65PJ2FCxf6DBw4sMGJ56dPnx4x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Bg4cmDVq1Khdq1ev9nr55ZcjCgsLDfPmzdtbcU9qaqr53nvvPRITE1OWn59v+Oijj4L69u0bv2rVqq1t27atdkjvnj173MePHx8zfvz41Pr165eGhIRYX3/99cCnnnqq1pgxY1K7du2aX1hYaNi4caNHRkaGM5/jj3P77bfXHTp0qMnHx8fWuXPnnJdeeulgXFxcacX10aNHZ4wePfq0w1/vuuuu6NmzZ4dde+216RMmTEg1GAz89ttvXnv27LEAVfYITp06NXj8+PG1+/fvn/X0008fPHjwoPmZZ56J6tq1a/zGjRu3+Pn52RctWuQ9atSoOrfeeuvR5557br/dbldbtmxxz87OPtbmTz/91G/EiBH1u3btmv3mm2/uAZg2bVp4z549G27YsOHv+vXrl1VV/+uvv55y00031bHZbGrWrFkpAP7+/jaANWvWePTr169hvXr1il577bW9Sik9derUiH79+jVctmzZ1vbt2592SPaQIUPq33jjjekPPfTQYYPBwJYtWyzXX399/b59+2Y99thjqRaLRScnJ7vt3r3brarnx8TElL333nu7brnllnr33nvv4auvvjoboFGjRiUAU6ZMCXn44Ydjhg0blvHoo48eys3NNTz33HOR3bp1i9+8efPfAQEBzuZjFxxnfrHXAzcqpV7UWh/35iilPIAbyu9xRjDwbTXXvwY6O1mmEEIIJ0U2aMiGhV+Tun0r7Yddz7Z2FnYvXUqJzmJT7do0X7mS3IUL8evf39WhCiEuQ3a7HZvNVuX5srJ/8hClFCbTPx9vrVYrWuvj7geOew6A0WjEYDj9wMLu3bvnvPXWWwcAhgwZkluewET99ddfh5o3b14CMHfu3JTK9Q8bNiwnLi6u6RtvvBHctm3b/dWVn52dbVqwYMGWDh06HPus/dprr4U0aNCgcOrUqYcqzl133XU5VZdQvYCAAOudd955pFu3bnl+fn629evXe77yyisRHTt29Pnjjz+2REVFWWta1ubNm93efvvtsNtvv/3I//3f/x2oOD98+PBTxma1Wnnuueei2rRpk7dgwYLdFeebNGlS3Ldv3/iZM2cGT5gw4egvv/zi5ePjY5szZ86x12vIkCG5lct66KGHarVu3TpvyZIluyrOXXnllbn16tVr9uyzz4ZXfm5lSUlJxd7e3nabzcaJw2onTpwYYTab7StWrNge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",
                         "text/plain": [
                             "<Figure size 921.6x633.6 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -487,15 +487,15 @@
             "cell_type": "code",
             "execution_count": 16,
             "id": "c2e77360-e8ee-43c6-8322-b9990aef19bc",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA3oAAAJyCAYAAACSd7KhAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAADLmklEQVR4nOzdd3xUVfrH8c+Z9E4CIRB6DSXSRURFFEEsICrYe8FVV39iX8u6ru7ae1lFbNgLir0gCoqKFOm9hd5CCeltzu+PmYkB0gYmuSnf9+t1X8nce+feZ65hN0/OOc9jrLWIiIiIiIhI/eFyOgAREREREREJLCV6IiIiIiIi9YwSPRERERERkXpGiZ6IiIiIiEg9o0RPRERERESknlGiJyIiIiIiUs8EOx2AHJr4+HjboUMHp8Oo1XJycoiMjHQ6jFqvOp5TVlYW1lqMMURHRwf02k7Qz1Ll9Iwqp2dUOT2jyukZVW7u3Lnp1tpEp+MQcZoSvTrGGDMWGJuUlMScOXOcDqdWmzZtGoMHD3Y6jFqvOp7TE088QVZWFtHR0dxyyy0BvbYT9LNUOT2jyukZVU7PqHJ6RpUzxqx3OgaR2kBTN+sYa+14a22/uLg4p0MREREREZFaSomeiIiIiIhIPaNET0REREREpJ5RoiciIiIiIlLPKNETERERERGpZ1R1U0QC7sQTT6SwsJCQkBCnQxERERFpkJTo1TGl2yuI1Fa9e/d2OgQRERGRBk1TN+sYtVcQEREREZHKKNETERERERGpZzR1U0QCLisrC2stxhiio6OdDkdERESkwVGiJyIB9/LLL5OVlUV0dDS33HKL0+GIiIiINDiauikiIiIiIlLPKNETERERERGpZ5ToiYiIiIiI1DNK9EREREREROoZJXp1jDFmrDFmTkZGhtOhiIiIiIhILaVEr45Rw3QREREREamMEj0REREREZF6RomeiIiIiIhIPaNET0REREREpJ4JdjoAEal/Ro8eTXFxMUFBQU6HIiIiItIgKdETkYBr06aN0yGIiIiINGiauilSwyb8spYxL/3Gt4u3Yq11OhwRERERqYc0oidSg4rdlmenrmJfXhGz0/ZwZNt47jq1K71bxzsdmoiIiIjUIxrRE6lBS7fsY19eEY0iQ2gcFcrstD2c+eJv3PDePLbvy3M6vIBZv349a9euZf369U6HIiIiItIgKdETqUG/rUkH4ORuzfjptsFcN7gDocEuvliwhds+XuhwdIHz8ccf89Zbb/Hxxx87HYqIiIhIg6RET6QG/b52FwADOzYmNjyE24d34bubBgEwe91uit1asyciIiIih0+JnkgNKSx2M2vdbgCObt+4ZH+7JlG0aBRBbmEx69KznApPREREROoRJXp1jDFmrDFmTkZGhtOhiJ8WbtpLTkExHRKjaBobvt+xbsmxACzZss+J0ERERESknlGiV8dYa8dba/vFxcU5HYr46fc13mmbHZocdKy7Ej0RERERCSAleiI15Ddvond0h8YHHeue7Encl2zRSK2IiIiIHD4leiI1IK+wmDnr9wAwoP3BiV5qC8+I3uLN+9REXUREREQOmxI9kRowb8NeCorcdGkWQ0JU6EHHm8WGkxAVSkZuIZv35joQoYiIiIjUJ0r0RGrA797+eWWtzwMwxmidnoiIiIgEjBI9kRpQ0fo8H1XeFBEREZFACXY6AJH6LqegiPkb9+Iy0L9dQrnn+QqyLK0HBVmuueYarLUYY5wORURERKRBUqInUs1mp+2hyG3p2TKOuIiQcs+rT1M3o6OjnQ5BREREpEHT1E2RaubrnzeggmmbAO0aRxEZGsTWjDx2ZeXXRGgiIiIiUk8p0ROpZpUVYvFxuQzdmtefUT0RERERcY4SPZFqtC+vkEWbMwh2Gfq1ia/0/PoyfXPevHnMmjWLefPmOR2KiIiISIOkNXoi1Wj2ut24LfRp3YiosMr/ufkKsiyp4wVZfvzxR7KysoiOjqZ3795OhyMiIiLS4GhET6QaLd+WCUCPlo2qdL6vxcLSOj6iJyIiIiLOUqInUo3W7swGoH1iVJXO75wUQ0iQYd2ubLLzi6ozNBERERGpx5ToBYAx5i5jzApjjNsYM6qM41ONMQuMMfONMb8YY3rVfJTihHXpWUDVE73QYBedmsZgLSzbqlE9ERERETk0SvQCYypwKvBzOcfPstb2tNb2Ap4E3qihuMRha9M9I3odEqveV85XkGXx5rq9Tk9EREREnFPvEj1jTEtjzHPGmN+NMTnGGGuMaVvOua2MMR8bYzKMMfuMMZ8YY1r7e09r7R/W2jUVHC/9G3usv9eXuml3dgF7cwqJCg2iaUxYld+X2sJXkEUjeiIiIiJyaOpdogd0BM4B9gC/lHeSMSYS+BHoAlwKXAx0An4yxlRtnp0fjDHvGGM2AQ8AFwX6+lL7+KZttkuMwhhT5ffVlxYLIiIiIuKc+the4WdrbRKAMeYqYFg5510NtAdSrLWrvecvBFYB1+CZYokx5k+gvFG+3tbajVUJylp7YamYHgFOq9KnkTprja8QS5OqT9sE6No8FmNg1Y5MCorchAbXx7/HiIiIiEh1qne/QVpr3VU8dSQw05fked+7DvgVOKPUvj7W2iblbFVK8g7wKjDUGNP4EN4rdYi/FTd9osKCadc4isJiy8rtmdURmoiIiIjUc/Uu0fNDd2BxGfuXAN0CdRNjTLwxpnmpXWcDO4Ddh3Ctub4tUPFJ9Vm70zt1s4n/M4G7eqdvrthWNxO9sLCwkk1EREREal59nLpZVQl41vEdaDcQ78+FjDH3AH8DEoFUY8zzQD9r7TbvtT4wxoQDbjxJ3unWWns4wRcWFjJt2rTDuUS9l5aW5ugzWrwhB4A965czbe8qv95rMwsA+G3+Uhpnrq7k7MNTHc8pNTW15Pv68HPq9M9SXaBnVDk9o8rpGVVOz0hEqqohJ3oAZSVbVa+a4buItQ8CD5ZzbC1wpL/XLOdafX3fp6Sk2MGDBwfisvXWtGnTcOoZFbst6VO+BSxjhh9PVJh//9TWBq/j63VLiWyczODBqZW/4TA4+ZzqCj2jyukZVU7PqHJ6RpXTMxKRqmrIUzf34BnVO1A8ZY/0iVTZpj05FBS7SYoN8zvJA2gWFw7Atn15gQ5NRERERBqAhpzoLcGzTu9A3YClNRxLlRljxhpj5mRkqJl2beZrlO5vxU2fpFhPorddiZ6IiIiIHIKGnOh9DgwwxrT37fA2Vj/Ge6xWstaOt9b2i4uLczoUqcChVtz08Y3o1dVEb+rUqXz99ddMnTrV6VBEREREGqR6uUbPGDPa+61vTdspxpidwE5r7XTvvleAvwOfeYupWDzNzDcCL9dkvFL/+Cputk88tBG9pjGeapU7M/MpKnYTHFS3/iYzf/58srKyiI6OZsiQIU6HIyIiItLg1MtED/jogNcver9OBwYDWGuzjTEnAk8Bb+EpwjIVuMlam1VDcUo9ta5k6uahjeiFBLloEh1KelYB6VkFJSN8IiIiIiJVUS8TPWttlSpnWms34OlrV2cYY8YCY5OSkpwORSpwuFM3wbNOLz2rgG378pToiYiIiIhf6tZ8MNEavTogO7+IbfvyCAkytIyPPOTrNPMWZNmWUTfX6YmIiIiIc5ToiQSYb9pmm8ZRBLn8bstYIsk7ircjU4meiIiIiPhHiZ5IgK09zPV5PhrRExEREZFDpUSvjlEfvdrvcCtu+iTFeipvqmm6iIiIiPhLiV4dozV6tV8gCrGAmqaLiIiIyKFToicSYIfbWsHnr6bp+Ycdk4iIiIg0LPWyvYKIU6y1AZu66Vujt70OrtFr3rw5OTk5REYeetVRERERETl0SvREAmhHZj7ZBcU0igwhISr0sK4VFxFCWLCLzPwisvOLiAqrO/9cL7jgAqdDEBEREWnQNHWzjlExltrNtz6v3WFO2wQwxpSs01NBFhERERHxhxK9OkbFWGq3teneaZtNDm/apk9dnr4pIiIiIs5RoicSQIGquOnja5q+XU3TRURERMQPdWfRj0gdEKiKmz7NfL30MupW5c2PPvqI3NxcIiIiGDNmjNPhiIiIiDQ4SvREAihQFTd96movvQ0bNpCVlUV0dGCeg4iIiIj4R1M3RQKksNjNxj25GANtGgemrUBJMRat0RMRERERPyjRq2NUdbP22rg7h2K3JTkugvCQoIBc09c0XVU3RURERMQfSvTqGFXdrL3SdnnW57VtErgm4b6qmzuU6ImIiIiIH5ToiQTIuvQcANo2DkwhFoCm3mIsOzLzcbttwK4rIiIiIvWbEj2RAElLD1yzdJ+w4CASokIpclvSs+tW5U0RERERcY4SPZEAKZm6GcARPYCmMZ5Rve11rMWCiIiIiDhHiZ5IgPh66LUN4Ige/FWQpa61WBARERER59RoHz1jzNpDeJu11nYIeDAiAZRfVMyWvbm4DLROCFwxFvirIIsqb4qIiIhIVdV0w/QNgCpKHAZjzFhgbFJSktOhSCkbd+fgttAqIYLQ4MAOlNfFpundu3cnPz+fsLAwp0MRERERaZBqNNGz1g6uyfvVR9ba8cD4lJQUJcy1SHVU3PQp6aVXh5qmDx8+3OkQRERERBo0rdETCYD1uwJfcdMnydtiQVM3RURERKSqlOiJBEBJIZZqGNFLKmmarqqbIiIiIlI1jid6xpjjjDFfGWN2GmOKjDHFB2xFTscoUpm0ahzRUzEWEREREfFXTRdj2Y8x5kTgO2A3MBM4DfgRiASOApYAcx0LUKSK0nxr9Koh0UuICiU0yEVGbiF5hcWEhwQF/B6B9vLLL5OVlUV0dDTXXHON0+GIiIiINDhOj+jdi6cSZ1fgcu++/1prBwKDgdbARGdCE6mavMJitmTkEuQytIyPCPj1jTE09a3TqyMFWbKysko2EREREal5Tid6fYEJ1trdgNu7zwVgrf0FeA14wKHYRKpkw+4crIVW8RGEBFXPP6kkTd8UERERET84nei5gJ3e73O9X+NLHV8K9KzRiET8VFKIpRqmbfo0q4O99ERERETEOU4nehuBNgDW2lxgGzCw1PFeQHbNh1V7GWPGGmPmZGRkOB2KeKVVY8VNn7rYNF1EREREnON0ojcdTwEWn4+BvxtjXjXGvA5cg6dYi3hZa8dba/vFxcU5HYp4VWfFTZ9mcb41emqxICIiIiKVc7TqJvAUMNgYE26tzQPuBjrgKcxiganArQ7GJ1Kpmpi6qRE9EREREfGHo4metXYFsKLU60zgNGNMHFBsrVXJPqn1fK0V2mnqpoiIiIjUEo5O3TTG/NMYk3rgfmtthrU2yxjT3RjzTydiE6mK3IJitu3LIyTIkNwovNruo6bpIiIiIuIPp9fo/QvoUcHxVOC+mglFxH++9Xmt4iMJrqbWCkBJH70dmflYa6vtPiIiIiJSPzi9Rq8ykUCR00GIlCetBtbnAUSGBhMZGkROQTGZ+UXEhodU6/0O13HHHUdhYSEhIbU7ThEREZH6qsYTPWNMa6BtqV1djDGDyjg1Hk/VzbU1EZfIoVi3q/pbK/g0iQ5jw+4cdmUV1PpEr3///k6HICIiItKgOTGidzme6ZjWu93t3Q5kADdwVc2FJuIf34heuyaR1X6vJtGhbNidQ3pWfrW2chARERGRus+JRG8ykIYnkXsNGA/8fsA5FsgC5lhrN9RkcCL+8FXcrO6pm+AZ0QNIz1QvPRERERGpWI0netbaBcACAGNMG2CStXZxTcchEghpNTl1M8ab6GXV/kQvP99TNMYYQ1hYmNPhiIiIiDQ4TvfRu7/0a2OMy7NbZQWl9svOL2JHZj6hQS6SG0VU+/18I3o7swqq/V6H6/nnnycrK4vo6GhuueUWp8MRERERaXCcbq+AMaaxMeYZY0waUAgUGWPSjDFPG2OaOByeSLl8o3mtG0cS5DLVfr8m0aFA3RjRExERERFnOd0wPRn4E7gByAM+9255wI3AHGNMc+cirH2MMWONMXMyMjKcDqXBK1mfVwPTNkFr9ERERESk6pwe0XsQSAJGW2u7WGvP9G5dgLOBZt5zxMtaO95a2y8uLs7pUBo834heTVTchL8SvV3ZtX/qpoiIiIg4y+lE7xTgBWvtJwcesNZ+CrwInFrjUYlUwYptmQB0SIyukftp6qaIiIiIVJXTiV48sLqC46u854jUOku37gOge3LNjK6WVN3U1E0RERERqYTTid56YFgFx4cC6qMntU5uQTFrd2YR5DJ0SqqZEb2YsGBCg11kFxSTW1BcI/cUERERkbrJ6UTvHeAMY8wrxpgOvp3GmPbGmP8BZwBvORadSDlWbM/EbaFjYjThIUE1ck9jDE2iNH1TRERERCrnaB894CGgD3AlcIUxxldlIhQwwGfec0RqlSVbPFVPuyfH1uh9m8SEsSUjj51Z+bRKqJkiMCIiIiJS9zjdML0QGGWMOQUYAbTzHloHfG6t/dax4EQqsHSLZ31et5pO9NRiQURERESqwOkRPQCstd8A3zgdh0hV+QqxdGte04meZ+pmbW+xMGrUKIqKiggOrhX/EyMiIiLS4DjdMH2tMWZkBcdPN8asrcmYRCpT7LYs3+pprdC1xhO9ujGi16FDB1JSUujQoUPlJ4uIiIhIwDldjKUtUFHJwiigTc2EIlI1abuyyS0sJjkunHhvcZSaUpLoqRiLiIiIiFTA6USvMq2ALKeDECltiUPr8wAalzRNr91TN0VERETEWTW+gMYYcwaetgk+Y40xJ5VxajxwEjCzRgITqaK/CrHUTKP00hK9I3o7a/mI3pYtW3C73bhcLpKTk50OR0RERKTBcaJSQi/gMu/3Fhjk3Q6UhSfJu75GohKpIqcKsYCnvQLU/qmb7733HllZWURHR3PLLbc4HY6IiIhIg1PjUzettfdba13WWheeXnkX+V4fsMVaa4daa1fWdIwiFfGN6NV0Dz2oO8VYRERERMRZTq/RawdMdjiGw2aMucsYs8IY4zbGjKrgvMuNMbaic6R225GZR3pWPjFhwbSMj6jx+zeKCCHIZdiXV0RBkbvG7y8iIiIidYOjiZ61dr21NsfJGAJkKnAq8HN5Jxhj2gBXozWHdZpvNK9rcizGmBq/v8tlaBzl66WnUT0RERERKZvTI3oBZ4xpaYx5zhjzuzEmxzuC1racc1sZYz42xmQYY/YZYz4xxrT2957W2j+stWsqiMkFvArcAOi38zpsiYPTNn3+mr6pypsiIiIiUrZ6l+gBHYFzgD3AL+WdZIyJBH4EugCXAhcDnYCfjDFRAY7pZuBXa+3cAF9XapiThVh8/mqxoL8ZiIiIiEjZnKi6Wd1+ttYmARhjrgKGlXPe1UB7IMVau9p7/kJgFXAN8KR3359AeaN8va21GysKxhjTHRgNHOfn55BaaJmDPfR86kqLBRERERFxTr1L9Ky1Va1QMRKY6UvyvO9dZ4z5FU+fvye9+/ocZkiDgDbAKu+armbAeGNMc2vt/w7z2lKDsvOLWLcrm5AgQ6emMY7FUVdaLIiIiIiIcxydummMSXDw9t2BxWXsXwJ0C9RNrLX/s9Y2t9a2tda2xVOMZeyhJHnGmLm+LVDxSdUt35aJtdCxaQyhwc7902nim7qpNXoiIiIiUg6nR/S2GmM+A14DvrPW2hq8dwKedXwH2g3E+3MhY8w9wN+ARCDVGPM80M9au+2woyxHYWEh06ZNq67L1wtpaWkBfUY/bigEIMHkOPrsd272xLF07QamTdtx2NcL9HMCKCgoKPlaH35Oq+MZ1Td6RpXTM6qcnlHl9IxEpKqcTvTexrN+7WxgizHmTeCN0tMpq1lZiaXfNfOttQ8CD1bx3MH+Xr/Ue/v6vk9JSbGDBx/ypRqEadOmEchn9N0nC4GNDOnTmcHHtgvYdf3lWrmTVxbNIiiqEYMHDzjs6wX6OQH07NkTay3GGOLj/fq7Sa1UHc+ovtEzqpyeUeX0jCqnZyQiVeV0H70r8axZuxxYDfwDWGGMmW6MudRbGbO67MEzqnegeMoe6ZMGbmktKMQCpapu1uKpm/Hx8SQkJNSLJE9ERESkLnK8vYK1NtdaO9FaewLQAc/IWGs80zm3GmNeMcYcXQ23XoJnnd6BugFLq+F+AWGMGWuMmZORkeF0KA1KUbGb5dsyAejqYGsF+KvqpoqxiIiIiEh5HE/0SrPWpllr7wN6AO8BMcCVwAxjzBJjzMUBvN3nwABjTHvfDm9j9WO8x2ola+14a22/uLg4p0NpUBZuziC/yE2bxpHERYQ4GktCVCjGwO6cAoqKq1pkVkREREQaEqfX6O3HGHM8cBmedXtRwHzgVaAYuBZ4wxjTzVr7j0quM9r7rW9N2ynGmJ3ATmvtdO++V4C/A595i6lY4AFgI/ByoD6T1A/TVuwEYFCnRIcjgeAgF/GRoezOLmB3TgFNY8KdDukgixcvprCwkJCQEFJTU50OR0RERKTBcTzRM8a0AS71bm2BfcBbwKvW2tJtBF4yxryKp9F5hYke8NEBr1/0fp0ODAaw1mYbY04EnvLezwBTgZustVmH+nmkfpq+wlPdcnCK84keeFos7M4uID2zdiZ63333HVlZWURHRyvRExEREXGAo4meMWYqcDyeKaQzgPuBj6y1ueW85Qc8hVsqZK2tUuVMa+0GPBU/6wxjzFhgbFJSktOhNBi7svJZuDmD0CAXR3do7HQ4ADSJDmPl9ix2ZWudnoiIiIgczOk1et2BJ4Eu1tpB3qIs5SV54En0TqiZ0GonrdGreT+v2om1cFT7BCJDHR8EBzyJHqggi4iIiIiUzenfWltaa4uqerK1diee6ZciNca3Pu/4zrVj2ibUjRYLIiIiIuIcRxM9X5JnjDF4Cqf4ulCvA+Zaa8tqaC5SY4rdlp9XehK9wSlNHY7mLxrRExEREZGKOD11E2PMWUAa8Afwvnf7A0grVT1TvNRHr2Yt3LSXPTmFtIyPoENilNPhlPD10tupRE9EREREyuBooudN5D4CgvA0Sr/Yu/0Hz2jjB0r29qc1ejXLN21zcEoinoHn2qFJjHfqZpamboqIiIjIwZxeo/dPYDkw0Fq73xCVMeYJYCZwH/CxA7GJMN03bbNz7Zm2CaWmbmZqRE9EREREDub01M1OePrlHTQP0bvvVaBjjUclAuzOLmDBpr2EBrkY2LF2tFXw0Ro9EREREamI04neJqCibs+h3nNEatwv3rYK/dvVnrYKPglRnqmbu7MLcLtrX80il8tVsomIiIhIzXP6t9fngFuNMW9aazeXPmCMaQVcCzziSGS1lBqm15zS6/Nqm/CQIGLCg8nMKyIjt5B4b+JXW4wbN87pEEREREQatBpN9Iwx1x2wqwjYBawwxnwErPDu7wKMBlYC7pqLsPaz1o4HxqekpNS+YZx6xL1fW4Xal+iBp/JmZl4R6Vn5tS7RExERERFn1fSI3vMVHLu0jH298Iz6vVgt0YiUY9HmDHZlF3jbKkQ7HU6ZmkSHsTY9m51Z+XRKinE6HBERERGpRWo60Tuhhu8nckimLN0O1L62CqWpxYKIiIiIlKdGEz1r7fSavJ/IoVi6ZR/jf1kLwKmpzR2Opny1ucXCzz//TH5+PmFhYQwaNMjpcEREREQaHKeLsYjUKtn5Rfz9vT8pKHJzfv9WDOzYxOmQytWiUQQAabuyHY7kYLNnzyYrK4vo6GgleiIiIiIOUO3zOsYYM9YYMycj46DWgxIA//xsCWt3ZtM5KZp/nt7d6XAq1D05DoDFm/WzICIiIiL7U6JXx1hrx1tr+8XFxTkdSr3zyZ+bmPTnJsJDXLxwQR8iQoOcDqlC3ZNjAVi2NZPiWthLT0RERESco0RPBFizM4t7Ji8G4P6R3etEFcv4qFBaNIogt7CYdelZTocjIiIiIrWIEj1p8PKLivn7u/PIKShmZM9kzunXyumQqqybd1RvyZZ9DkciIiIiIrWJEj1p8N6ftZFlW/fRpnEk/zkztda2UyhLqtbpiYiIiEgZlOhJg1ZQ5Obl6WsA+McpXYgJD3E4Iv9014ieiIiIiJShRtsrGGPWHsLbrLW2Q8CDEQEmz9vMlow8OjWNZli3Zk6H47fUFp4RvSVb9mGtrVOjkSIiIiJSfWp6RG8DsP6ArRhoCyQAe4EM7/dtvcc21HCMtZraKwROsdvyP+9o3nUndMDlqntJUlJsGI2jQsnILWTTnlynwxERERGRWqJGEz1r7WBr7Qm+DbgNaAzcACRaa/tYa3sDicD/4Un4bq3JGGs7tVcInK8WbWVdejatEyIZ0SPZ6XAOiTGG7qVG9WqLxMREmjZtSmJiotOhiIiIiDRINTp1swyPA+9Za18ovdNaWwg8Z4zp6j3nBCeCk/rL7ba8+NNqAP52fAeCg+ructXuybH8vHInS7ZkMDy1dkw/veSSS5wOQURERKRBc/q32yOBRRUcX+Q9RySgpi7fwfJtmTSLDefsvi2cDuew+Cpv1qYRPRERERFxltOJXiZwfAXHBwPqBC0BZa3lee9o3tWD2hMWHORwRIcntYWn8qZaLIiIiIiIj9OJ3nvAOcaYZ40xbX07jTFtjTHPAaO954gEzK+rd7Fg414SokI5v3/daY5enlbxkcSEBbMjM58dmXlOhyMiIiIitYDTa/TuAjoCfweuN8YUABYIAwzwDfAP58KT+mbFtkwe+HIpAFce247IUKf/CRw+l8vQLTmWP9btZsmWfTRNCXc6JCZPnkxubi4RERGMGjXK6XBEREREGhxHf8u11uYCI4wxw4Ez8LRUMMBa4HNr7bcOhif1yL68Qp6esoo3f0+j2G1Jjgvn4qPbOB1WwHRPjuOPdbtZumUfJ6Q0dToc1qxZQ1ZWFtHR0U6HIiIiItIg1YrhDG9Cp6ROAq7Ybfls/mb++/Vy0rPycRm45Og23Dy0M7HhIU6HFzBapyciIiIipdWKRM8YEw0cDTQFfrDWbnc4pFrLGDMWGJuUlOR0KLXanuwCvl5bwD1//FTSSLxvm3juH9md1Bb1rwdhd1XeFBEREZFSHE/0jDE3Af8Gory7hgLbjTGJwDrgJmvtBIfCq3WsteOB8SkpKdbpWGqjDbtyePbHVXy+YAsFRW6gkJbxEdx0UmfO6t0Cl8s4HWK16JAYRViwiw27c8jILSQuov6MVoqIiIiI/xxN9IwxFwFPAt8BXwHP+o5Za3caY74DzgaU6Eml3G7Lpa/PYl16NgA9mgTxf6f1ZnBKU4LqaYLnExzkokvzWBZs3MvSLfs4ukNjp0MSEREREQc53V7hZmCqtfYUym6jMBfoXrMhSV01b+Me1qVn0yw2nGm3DubmfuEM6ZpU75M8n9Rkzzq9JVu0Tk9ERESkoXM60esKfFrB8e141u2JVOqLBVsBGNGzOW2bRFVydv2jdXoiIiIi4uN0opcLVNT0qy2wt0YikTqt2G35apEv0Ut2OBpnqPKmiIiIiPg4nejNBMaUdcBbifMy4OeaDEjqpj/W7WJnZj5tGkdyRD2sqlkVnZNiCHYZ1uzMYsHGvU6HIyIiIiIOcjrR+w/Q1xjzOTDEu6+rMeZiYBaQCDzkVHBSd5RM2+yRjDENY03egcJDghjTryVuC5e9PovVO7IciyUlJYXu3buTkpLiWAwiIiIiDZmjVTettb8aY84BxgOneXc/CxhgN3COtXaeU/FJ3VBY7OabxQ172qbPv89IZWtGHtNW7OSSV//g42sHktwoosbjOP3002v8niIiIiLyF6dH9LDWTgZaA6OAO4C7gNFAG2vt585FJnXFjNXp7M0ppHNSNCnNYpwOx1EhQS7+d2Ff+raJZ0tGHhe/+ge7swucDktEREREapjjiR6AtTbPWvuFtfYxa+0j1tpPrLXZTscldcMXC7YAnmmbAhGhQbx26ZGkJMWwZmc2l78+i6z8IqfDEhEREZEa5GiiZ4z50RjzrjEmoZzjJxljfqzpuKTuyCss5vsl2wE4vYFP2ywtLjKEiVf2p2V8BAs2ZXD0Q1O5Z/IiFm7ai7XW6fBEREREpJo5ukYPGOz9eqQxZoS1dvkBx5OA42s2JKlLpq3YSVZ+EaktYmnXAHvnlZaRn8F3ad+RX5zP0DZDaRbbjLevPIqbPpjP/I17eXvmBt6euYGUpBhO79Gc1o0jaRYbzo4cN3mFxYSHBAUslldffZXs7GyioqK48sorA3ZdEREREakapxM9gCeBc4DfjTHnWWu/czqg2swYMxYYm5SU5HQotcIXCxv2tM0idxG/bfmNyasnM23jNKL2FRCdC483fpT+LQYwssNI3h07hPXphbwzexlfLV3O6uxlPDOzEHdBE9wFTcCGcvvP3zK8ezMeGd2DuIiQw45r7969ZGVlUVhYePgfUkRERET8VhsSvT+Bx4EvgC+NMTdba59zOKZay1o7HhifkpLS4OffZecXMXWZZ9rmaT2aOxxNzbLW8sXaL3h67tOk5+zgiHWWm/609F1tcVnICYOVyb8yt+VvfNw6lLXNDHtDC6E5RB54saI4ivOb8sOGIxn5/D5euqgvXZvHOvGxRERERCRAakOih7V2mzHmOGAi8LQxphvwd4fDklrujd/SyCt007dNPC3jD0pf6q19Bft44PcH+HXpNwxabDltfhBNdnlHzkJCCE5sQuSWrfRaZ+m1zgJ5AOxs5GJni0j2tW3CnlZxzG+0j0WuLRQFZxAUnEFE1Cq27kjnzBdzeeTsnpzRq4VzH1JEREREDkutSPTAU3kTOMcY8yCeFgudgMmOBiW11uu/ruOx71YAcOWx7RyOpubM2TiT91+7lR5zdnPJGkuwG8BNcPPmxJ97Lo1Gn01wkyYUbt9B7rw/yZ03j31z51C8ag2Je/NJ3JsFSzyN1E8BXI0asa9pAvu6NOb7nLnkhH1LZsFa3nz2WNZ0b0VihIuczFxysnPJy8nF3bQZbY7tz4COTeiQGN1gm9OLiIiI1Ha1JtHzsdbeY4xZBkwAjnU6Hql9Xpuxjn9/uRSAB87ozqlH1P9pm8XuYr695zISv5nDlbnenUEuoo4/lvhzzyX6+OMxQX8VUwlJakrI8OHEDh9OEmCLiihISyNv2TLyli0nb9lS8pcuo3jvXqL37iV65VouK3n3cs/2W9mx7Ho3lk+ap7K4fW9iBxzFKT1bMqRr04AWcxERERGRw+N0ojcd2H7gTmvtO8aYdXhG9BrXdFBSe+2X5I1K5eIBbRyOqPq5rZt3HruCIz+ZA0Bm68a0Pe9yEkaMJDgxsUrXMMHBhHXsSFjHjsSNGAF41vkVbd3KnA8/omNIMMW797AjfT0L1/9BSF4RUUXhhITGExwWRVhELJHh0ZgVS2m8aycj1v3GiHW/kfXri8xu05ir2qaScPRwLh4wkH5tmpTc1wKZeYXEhB9+gRcRERERqTpHEz1r7QkVHPsNaFqD4UgtVzrJe3BUKhc1gCSv2F3Mo1/fydB3ZwGQddtl9L/yjoBc2xhDSHIy+b16kjh4MADNgPA9K7l2yrXsyN0B7Cg5PwRD0XFu2u4Iov8KN0etsLTcZTlhRTonrJhG1vRpzO4YxP9aJ5MUcxzhLtiZmc8R//qe4zo14f6R3WmfGB2Q2EVERESkYo42TBepqjd+bZhJ3r0z7qHFy18RlQ+FA3rS74rbq/emuXvpvGsj7zUexP+5Ejkzp4C+uXkkFhVRiCXIQEh8ITn9LVuuasyOq5qwsV8+uxu7ic6DExYXc9vXG2mUlw1AbEE2Vy/5ks2zFzD86V944vsV5BUWV+9nEBEREZGaHdEzxryGZzbXWGttsfd1Zay1Vh2XG7C3Z67nX180rCSvyF3EXTPuYu/XX3HkKouNDKfrw08HpvjJtsWw4msoyIKCHFI2roUdr8H2pbBrFeAZSr/Kd35Mc2jVn5yWfQlO7k1o0+4QmfDX9TbNgZ/+S/686WzbFMGKPVFYb5jBxcWMXDWNs1ZNY0byEby152Q+nb+Jf53enZO6NTv8zyIiIiIiZarpqZuX4Un0rgWKva8rYwEleg3U+7M2cM/kxQDcP7J7vU3ysj57C1fjFkQccwJu6+auGXfxy5Kvefp7T7vE5rffSUizAxKjld/B1H9DfFtI7gXJvSG5z/5JWGnWwtzX4Zs7oLigZHdzgG3eF0Fh0LwntOgLLftBq/4Q1wqMObj/nk/LfnDxJ4QNnkWb6Y/Qet0vpAXNZ5YrhsjiIqb1gWMXWI7dsoiBWxbxW1cXj5oIHp91Ck8Mv4HuzTRDW0RERCTQajTRs9a6KnotUtpHczbyj08XAXDPaV25dGBbZwOqJllvPMDGh98FILR5ArMHtuD35KVcNc1FbE4xkf370+icMfu/aeMs+PASKMqD7Yth+Zd/HWvaHY66BnqcCyHhnn2FufDVrTD/bc/rHudCYhcIiWT5uo10Se0NCe0hKRWCQw/tg7TqDxdNwriLGZuxkVM2zeQfSyfwYodg3htoGfW7m5PmW45d5mbgsmwWtpvEE8u/wt3nXB4/7XqaRGn9noiIiEigOF11U+Qgbrdl4u9p3P/lUqyFO0/pwlXHtXc6rOqxYSbpr74JhGCC3BRs3U3PSbv5n4EgW4wJD6f5A//GuEr9TSR9Nbx7rifJ63UhtDsetszzbFsXwI4l8MWNntG+/ldD55Phi//zHAuOgBHPQM9zSy63LW8aXY4YHLjP5AqC+La0im/LG91H8+vmX3Hn7qFxp19plPIZ5o88MtdF0msd9FqXy+4f3uC1byYSNaAvV130BGFRVaskKiIiIiLlU6IntcrqHVn845OFzE7bA8Ctwzrzt+M7OBxVNdmznpynLyJ3ZwiuiBB+urc/v837nSEL3By5ygKGxBv+TmibUtNVs3bA22dB7m7oNAxGPAtBwX8lbkUFsHQy/PYcbFsI0x7ybOCZ4nnu29DsiBr7iMGuYI5vdbznRedRMOQ/sHQyxfO/ZO8vi9iyMJuEjCBG/O6G32fz3ceDCOuVxOBL7yKs+1BQQ3YRERGRQ1LTxVh+PIS3WWvtkIAHI7VKQZGbl6ev4bkfV1NQ7KZJdBj3j+zOaT3qaTP0vH3w3nmkzysGQthwWj9eyPyDoE7BXNK5OZ2X/EFBZjARux6CL5dA9zM9a+feGQN713vW441+3ZPklRYcCj3OgSPGQNoM+P0FWPkNdDoZznoZIuJr5OMVF/9VWTOoVCN3X3xBPc6h8SWQUJhH5veT+PP1CcQv30anjcDG7Sz/5v/I7eCi8xX/R/zIqwNThEZERESkAanpEb32eIqriJTYkZnHpa/NZtnWfQCc268Vd53albjIetpk210Mk64ib8VKsrc2xYaH8s8WszC4eOCYBzmp/emw4D2Cf34Mdq+FOa96tqAwKM73jMxd8CGEVbCmzRhod5xny9sHYTE1Ojr29NNPk5WVRXR0NLfcckv5YYaEE3vahQw+7UI2bd7Oe4/eTqclc0jZ5CZ0hZvtdzzF8sdfJOScURxxyY2Ex5VTaEZERERE9lPTxVja1uT9aoox5i7gUqATcJa1dvIBx9OAfCDXu+t5a+2EmoyxtsrMK+Ty1z1JXpvGkTx05hEM7NjE6bCq148PwqrvSF/hqTY5vV84WZE53ND774zoMMJzTq8LoOf5numXSz6FxZ94RvIiEuDCSRDtR6XK8Nhq+BCB17JFErc+/QafzNvAjZ/9j1PSvuGoJQUk7MyHFz5g+fgPWHNSL854bCLBwfX0jwAiIiIiAaI1eoExFfgAeLWCc8611s6vmXDqhoIiN9e+/SdLtuyjbeNIPr52IE2iw5wOq3plboffnyd/XzCZ60NwBxve65VNx0aduDz18v3PNcYzXbN5TxhyH2xfApGNIbaeTmcFjDGc3acNx3e+n4/nXs3P88bTYc1HRKwIpeMGQ7dv5jN+y0k0u+N1RvRsS0iQCveKiIiIlKXe/ZZkjGlpjHnOGPO7MSbHGGONMW3LObeVMeZjY0yGMWafMeYTY0xrf+9prf3DWrvmsINvQNxuy20fL2DG6nSaRIcy8Yqj6n+SB/DHS1BcwK6tXcFapqUa9sQY7jv6PkJcFYxSGQPNUut1kldak+gw/nZ8B/5x0yOMuPVjhpzkInPYPgqD4IQFO9j08DkMfOQznp26isy8QqfDFREREal1HE/0jDGdjDEvGGNmG2NWG2PWHrD5m0B1BM4B9gC/VHDfSOBHoAueaZcX45l6+ZMxJurQPk2FJhpjFhljJhpjWlTD9euUh79dzmfztxAVGsQbl/endeNy23HXH/mZMPtVCrNdZCzai9vAp0fB6M6j6dW0l9PR1VoRbfoQ+fcZ9D/mBMIG76UwCIYuzOaKRfcwb/qLjHhmOvM37nU6TBEREZFaxdFEzxjTG/gTuBIIxVOsJdv7fVvADWzw87I/W2uTrLWnAh9VcN7V3vuNstZOttZ+BowE2gDXlIrxT2NMejlbqyrGdLy1tgfQG1gNfOznZ6pX3vwtjfE/ryXYZXjp4r6ktohzOqSaMfdNbG4GO9d1gKJifu9iKExuzE19bnI6stovMgHOfZuU+38h4bLeFAXB4Hlu+q75lpODb+KB1x7mxZ9W43ar1pOIiIgIOD+i9wCQBaQCvhYK/2etbQlcAsQB/+fPBa217iqeOhKYaa1dXeq964BfgTNK7etjrW1SzraxijGt934tAp4CjjLGNMhqEht35/Dfr5cB8NiYHhzXqYE0xy4qoOjHF9gwvTEZi7MpNvDpQBe3H3k7cWENJNENhCYdaXnbuzR7/L8UB8GQuXDSW8WMnvk5WRPP4Na7z+C7+d86HaWIiIiI45xO9AYCL3uTLV+C5gKw1r4NfAI8Wk337g4sLmP/EqBboG5ijIkyxjQqtetCYLG11u+FRcaYub4tUPHVtH9/uZT8IjcjeyZzZu+WTodTY7Lfe4y1HxeTsz2M7KhgHjrHRYueAzm13alOh1YnJZ5yJi2fe56ixEZE50GvdZYRv7u5+tNVJFw2jldeu9fpEEVEREQc5XTVzXDANyqW7/0aU+r4HOC8arp3Ap51fAfaDfjVVdoYcw/wNyARSDXGPA/0s9ZuA5KAScaYIMDg+bxjDidwgMLCQqZNm3a4l6lRC3YWMWVpPuFBcEL8nmqPPy0tzfln5HZjPv+QxG+nYwhicRvDsyMthbEx3GKGMn36dGfjo3qeU0FBQcnXavtv4AqCBx7CtWcP4SsXYRZ+TfGG3cTtDKL/kx/z0Lp1HD3kqoDcqlb8LNVyekaV0zOqnJ5R5fSMRKSqnE70NgMtAay12caYPXjWsX3qPd4BqM6SemUt6PG7q7S19kHgwXKOrcXzmQ6btbav7/uUlBQ7ePDgQFy2RuQVFnPf0z8DcMvJXTlzUPtqv+e0adNw+hktnvAkQd9Oxw18fKxh/qmd+FvXczi9/em1ZspmdTynuXPnUlBQQGhoaA39NzgT+CeFa3/n11suJ2mZYcTHc5lelMd1//0Ic5jN4mvDz1Jtp2dUOT2jyukZVU7PSESqyulE7zc8a/Pu977+ErjFGFOIZwrnDcCUarr3HjyjegeKp+yRPjkMr/y8lvW7cujUNJrLjmnrdDg1wl1QQN6rbxMFfD+siBFnnMO9Jz542ElHXXDaaadRVFREcHDN/k9MSPujGfTWL0z92zBazsnjxE+X8OreE7jomR8ID3X6f+5EREREak7A1ugZY4qNMRuMMZf48bYXgBnGmHDv6zuAtXgSv/uA9cC4QMV4gCV41ukdqBuwtJruediMMWONMXMyMjKcDqXKNu7O4fmfPDVv/n1GaoNpcr373YlE7cklrSmMaFlI72PuaBBJHkCXLl1ITU2lS5cuNX5vV3QiQyfOIe0kTxeTY37azrdjerLqq5drPBYRERERpwTyN+6NQATwhjHmz6q8wVo7y1p7l7U2z/t6G9AD6AUcARzhrYRZHT4HBhhjSuYQehurH+M9VitZa8dba/vFxdWOaX+VsdbuV4Dl6A6NnQ6p+hXk4P7pCbY/9zgAMwa46XjMzRAe63BgDYgriFOe/4F15/WjyAUpK9wU3PI000b2YM93E52OTkRERKTaBSzRs9a2tdYmAj2Btw7jOtZau9Bau8RaW3wo1zDGjDbGjAZ8a9pO8e47vtRprwBpwGfGmDOMMSOBz/AkrPrTfwCs2p7JRa/+wZSl24kKDeLu07o6HVL1W/wJPNuLvRMex5VtSGsKycPPhGNudDqyBunUf71F0YQnmXVEBMVBkLSykG3/9xCzTutNwbrlTocnIiIiUm0CvmjFWrsIWOTPe7wVKVviWTN30Nw2a22VRghLObBR+over9OBwd5rZhtjTsTT1+4t732nAjdZa7P8vJ+Usi+vkGd+WMWbv6VR5LbERYTwyNlHkBQbXvmb67KMTfDJWNyFhexa0RJw8/GxLu7ofYXTkdW4nTt34na7cblcJCY62yux98BT6HrkMP4x4QXazXiVYxcVELMmj4Wjz6TtE4/QZPBIR+MTERERqQ5VTvSMMX8H3rHWBqxQiTEmCngEuBxPq4XyBPlzXWttlRZCWWs3AGf7c22nGWPGAmOTkpKcDqVMy7ft46IJf5CeVYAxcOFRrbl1WArxUaFOh1b9fnse3IXszR5AUdYG0prCzr7t6NSok9OR1biJEyeSlZVFdHQ0t9xyi9PhEB4SxJN/u4HnOw/nlmkvc8PMr+m6EbZefweTT5tK0wvvYEiXpkSFqWCLiIiI1A/+/FbzLPCYMeYz4DVgirW2rPYE/ngJTwPxacCvwN7DvF69Z60dD4xPSUk53GdfLV6fkUZ6VgE9WzXiP6NSSW1RN9YSHrbsdJj7Bu5i2DUrE4CPjnVxUrthDaYAS21njOGGIZ3plnw777boy+5p/+GY+W6O+fx7pq5aypnH3MlH1w0iLjLE6VBFREREDps/id7xwGV4mn2PATYbY94A3vD2ijsUZwBvWWsvPcT3Sy2zbNs+AO46pUvDSfIAZv4PinLZu68vRelb2dAsmNmdLbe3HeZ0ZHKAIV2TGNL1ArIuGsZHdw+j35RchizbRGLOHVwb9TivX30cYcF+TSIQERERqXWqXIzFWvuLtfZKoBlwBZ42CHcDq4wx04wxFxtjIvy8fwGeXnpSDxS7LSu2eUazujRrOBUmbeYu9n30GhumJ7B9yjYAPjjGTavY1qTEpzgcnZQnOroJlz8xk62XtiAzAnqsz2bk1//HP96bweFPVhARERFxlt9VN621OdbaN621g4FOwH+AtsAbwFZjzMvGmCOreLmvgeP8jaEhq8199NJ2ZZNf5KZFo4gGMf2tOCuLHU88waohQ9k8LZzsreEQFMyaIZ2Z3ckwtM1QTdus7YJDGXbbd4T+bQB5IdBzVQG9vriWVz9+z+nIRERERA7L4bZX2IZnZG8jnqqVYcDFwExjzFRjTOtK3n8T0M0Y87Axpq3Rb8WVqs199JZv9Y3mxTgcSc3Ycsed7HplAsX7cgmNLaTpVWfTYfpPPHH8PjCGYZq2WTe4guh1zetE/vMqCoPgyIWWoi//zYy3boLiIqejExERETkkh5ToGWOON8a8jifRexWIA8YBLYDmwO14eti9XtF1rLW7gbeB24A1QJExpviATb9plSEmcw3cn+DZxp8ARQVOh8Ry7/q8Ls3rf6KX+cMPZE2diis8lDYnptP+yhY0vuUBFhWmkZ6bTovoFnRL6OZ0mOKHlDG3EPvQPRQbOP4Pw28zvmXWS2dQmJ/jdGgiIiIifvOnvUIb4FLv1hbIAt4HJlhrZx1w+hPeBO3hSq75T+A+YA8wD1Xd9IMFXz/5LX/CjiWQ3NvRiJZtbRjr84qzstj2wIMAJPYpJLJpAQy6DYxhyvopAJq2WUe1HXkhm/Itmff+hxHTDd8Vryb/8ZPY0PUup0MTERER8Ys/VTfX4pmeORPPurz3rbUV/al7DZ4Rv4pci6e1wqnW2nw/YmnwMmM6wr1L4NOxsHgSbF3oeKLnG9HrWs9H9HY+8yxF27cT3iGZuJZzWJTUmZ/z0pj+xTks270M8CR6Uje1HHMRW3Lz2fPfxzl5hovFO3eRknM3j5p4rj/1KPXaExERkTrBn6mbzwCp1tqB1trXKknysNZ+aa1tV8k1o4EPleRV3X7FWIKCoVkPz4FtixyNa19eIZv25BIa7KJt4yhHY6lOuYsWsefttyEoiN3DYxnaJpkLIvN4aeHLLNu9jPCgcM7qdBZHNDnC6VDlMCRfciWxT/2XvFBD6goXub/kMeLXq7j8mU/ZuFtTOUVERKT2q/Kfpq21N1fD/WcCnavhuvXWQQ3Tm/sSvYXOBQWs9LZV6JwUTXDQ4db4qZ1sURFb/3kfWEvcJRcyLuYDdppgmofFM6jtMAa1HET/Zv0JDw53OlTHXXLJJbjdblyuuvuz0OqUMylqlsCma68jaQfk/GR59Og7GfdiDvdfMYruybWvIJKIiIiIT5V/CzPGjDDGPF/B8eeNMaf5ef+bgHOMMaP9fJ/4lIzoLQa327EwljWA/nm7J75F/rJlhCQn8/2QeDabYjoWFPD1yW9xz4B7GNRykJI8r8TERJKSkkhMTHQ6lMPSrvfxNH7nVZa1dhGZbciYHsKtu/7FfS+/w2+r050OT0RERKRc/vy5/Ragot/io73n+ON1oAj4wBiz0xgz1xgz64DtDz+v2bBENYGYZCjMhj3rHAtj2VZvxc162lqhaM8edj73HACRd47jpRWegrK3ZuQQHNfKydCkmnXrMIBdN/6dX7sHEVpoCPopnITQ57jvs1t4e858p8MTERERKZM/iV4qMLeC43O95/ijqffrBjxVPBOAxAO2pmW/VUo0864H27rAsRCWb/UVYqmfI3oZkz/D5uYSdcwxTIj5k+yiHI7NyeWYyFZQh6cnStV0iu7K4Jc/YWvf1kTnwRWTwGXm8sjii7n522edDk9ERETkIP78hhoFVDY30K/hHGttW2ttu8o2f67ZIDV3tiCL221Zsa3+Nku31rL3ww8ByB0xiEmrJhGE4bbde6Bxe4ejq52WL1/O4sWLWb58udOhBEzHJp0Z/PoXRB4zkLgc+M87RSRmWKZsf4V//TTB6fBERERE9uNPorcGGFzB8cHA+qpezBgTYYx5zRgzxo8YGrz9qm76+Eb0HCrIsmlPLtkFxSTGhNE4OsyRGKpTzuzZFKxbR3BiIk+G/YLbuhkT04n2hUXQuKPT4dVKX331FZMmTeKrr75yOpSAcoWG0ur554no25eobMOTbxeStMcyaf0zPPXru06HJyIiIlLCn0TvA2CUMeZWY0zJ+4wxLmPMzcAoPA3Uq8RamwucS8Xr/uQA1trx1tp+cXGlKv453GJh2bb6PW1z7wee0byMYUfy246ZxITEcJ3bO3KZ0MHByMQJrogIWr38EuGpqYRlunh6QhFnzHTz1vL/8vrsj50OT0RERATwL9F7FE87hEeBTcaYKcaYKcBG4HFgFvCwn/efj9orHL5GbSAsFrK2Q+b2Gr/98q2eaZtd6+G0zaI9e8j8/nswhmdbLgXgmp7XEL9ng+eExkr0GqKg6GhavzqB2NNPJ6jIcOE0Nw+9Ucw33/+LT+d+5HR4IiIiIlVP9LxNzU8A7gZ2Asd4t53AXcBga22en/e/B7jKGDPYz/dJaS4XJHnr4DgwqrfcO6LXpXn9S/QyPp2MLSxk6xHNmefaRJvYNlyQcj7sWu05QVM3G6yguDhaPP4YrSZMIDg5idY74f63itn4+H28+eNjTocnIiIiDZxf5QKttQXW2oestT2ttZHerZe19mFvIuiva4EdwFRjzFJjzBfGmA8P2D44hOs2PCUFWWq+8ubyetpDr3QRlrc6bSPUFcqjgx4lJD8T8jIgNAai6nafODl80cceQ4evvyX2sosodsHQeZbwR1/nng8vo6C4wOnwREREpIEKdvj+pRuld/FuB7I1FEvdVlKQpWZH9HIKikjblU2wy9AhMbpG713dcmbNpiAtjd0xhj87Gu456k66Ne4GG7ytHRu3B2OcDVJqBVd4OC3uvJvIk04m7epL6ZHmJvb5P7h678k8dME7JEcnOx2iiIiINDB+JXrGGAMMBToCjYEDf8u11toHqno9a60akAWKQwVZVm7PwlromBRNaHD9+s+Z/r6niuLUHnBqxxGM7uT9u8TuNZ6vmrYpB4jv14/gSV+y8oIzabsjn6smbOPGzNO4/YKX6N/8KKfDExERkQakyomeMaYLMBnoxMEJno8Fqpzoif+MMWOBsUlJSfsfSOwCrhDYtQbysyCsZkbXlnkbpde3/nmFu3aR+f33GANrjmvH/wbci/GN3u3yJnqquClliGnfjm5f/siiMafTZOse7ngrj6dzruKmKydwZLKSPREREakZ/gzBPA+0Bm4D+gLtytgOqXu0MSbUGDPYGHO5MeYy7/ehh3Kt+q7M9goAwaHQtAtgYfuSGotnuS/Rq0etFazbzcyHbiGo2LKwYxD3jXqOyJDIv05QIRapRESTBHp9+QO7O7YlOg9uf7+IV5+7ijlbZjkdmoiIiDQQ/iR6A4EnrbVPWmvnWWvXl7X5G4Ax5jw8LRqmAq8Cr3m/32iMOdff6zVoJdM3a65x+rKSQix1Z0RvZ85O1mWsK/NYUXo6Ky6/iCZfetbhNb38Sto3OuDvFyVTNzWiJ+ULjYpkwKdfsOvIPoQWww2fFvHRw5fzS9rvTocmIiIiDYA/a/SygM2BvLkxZjjwjve69wBLvYe64anI+Y4xZq+19rtA3rfeatYDeKfGEj1rbcmIXl1qln7l91eyYd8Gnhj8BENaDynZn/3772y+7XZsejr7ImDu1QO57qxx+7/ZWti11vN9wiENYDcIN910k9Mh1ApBIcEcM/FtFt45jtDPvuOy7918lnkVu8a9wKgeg50OT0REROoxf0b0PgZOCfD97wZWAEd42zZ85t0eAo4AVuLp0SdV4au8ubVmEr2tGXnsyysiPjKEpjFhNXLPw7U1ayvrMtZRbIu5bfpt/LblN6y17Hz2OTZccSXF6eksaQ1P39iaS69+9uALZG6DwmyISIDIhJr/AHVEUFBQydbQGWPo+cjTRFx3MW5jOeN3N9seuI63ZnzudGgiIiJSj/mT6P0bSDLGvGKMOcIYE2OMiTxw8/P+vYDXrLUZBx7w7nsd6OPnNRuuZt6m6TuWQXFhtd+upFF6s9i/CpXUcvN2zAMgPCicQnch//fj/7Hg89dJf/FFrIGPjjX894Iw7h7xBFEhUQdfQNM25RC1vfEukv51C4XBluMXWVredgefvvGI02GJiIhIPeVPorcF6AdcCcwH9gKZB2z7DiGGiv7kX7/q9Ve38DiIbwvF+bBuerXf7ueV6UDdmrb5544/AbjqiKs4s+OZ5BXnMfvdZwD4alAEHx0XxHV9/05qk9SyL+ArxKKKm3IImpx7NW2ff4Q9jaHZHujy8BtMv/JsivbscTo0ERERqWf8WaM3kcA3L/8TuNoYM95au99vOsaYODxJ5dwA37N+63I6/P48vH8RnDMROg8L+C2stTz+/Qre+C0NgBO7NA34ParL/B3zAeiT1IerjriK3Pwseq34BoCpnfLp3+woLu9+efkX2KUeelXx22+/UVBQQGhoKAMHDnQ6nFoldvAZ9J3UjS/uPINOsy1Nf13KkqEn0O7Bh4kdPtzp8ERERKSeqHKiZ629rBru/yDwDbDMGDMeWIYnmeyGJ8lrClxXDfetv066H/IyYN5b8P75MOp/0OOcgF3e7bb88/PFvD1zA0Euw2Oje3BspyYBu351yirIYtXeVQSbYFKbpBLkCuKe0DPZkvcNmxpDVotG/OfY/xDkqmCQebe3EEtjFWKpyO+//05WVhbR0dFK9MoQ1qwTpz71IxOfPZn43wvpkZbP5pvGkX/jWppce22dmQotIiIitZc/I3oBZ62d4m2h8AyeqpuWv5qxbwHOtdb+4FR8tVG5DdN9goJh5HMQ2Rh+fRo+uRpydsGAaw/73oXFbm75cAGfL9hCaLCLFy7ow9Bu5cRRCy3cuRC3dZPaJJWI4AgAcn6YCoAZPJBXht5Ks6hmFV9EPfQkQCLjm3HejT/xVtRwJq7L4qKplvRnnyNvfRotH3gQE6pWoiIiUrm5c+eG4ul1XXd6XcnhygQ29O3bt6Cik/xK9IwxjYCbgKF4Rtsusdb+boxpDFwDfGytXenPNa21k4wxk/mrCTvAOmCutbbYn2s1BNba8cD4lJSU8qfRGgND74eoJvD9PfDtnZC9E06813PsEOQWFHPdO3P5acVOokKDeOXSfgzsUDdG8nx86/N6Ne0FgC0uJtOb6B174S2EN+5a8QXcxbDb239PrRUkABrFJzD68u/58LVzee6sjVzzhYXPvmDtxg20/d/LBMXFOR2iiIjUYvPnz09KSEh4LT4+vnlwcHDdKIEuh62oqCh/z549W+fPn39Fr169tpd3XpUTPWNMc+BXoA2wCWgJRABYa3cZYy4HEoFx5V6kHN6EbpZ3k0AZeANENoHProdfnoDsdDj9KahoamIZ9uUVctUbc5iVtpv4yBDevKI/PVo2qp6Yq5FvfV7vpr0ByJ0/n+L0dEJatiSsayVJHkDGJk+hm+gkCNMfzSQwmjduxJU3fsUrE+/l6fMmc80nEP/nAlaeNYKO73xISLNKRplFRKRBmjt3bmhCQsJrbdq0aeZyudxArtMxSc2JjY1ttn79+tfmzp17Znkje/5Utfwv0Bg4Bs/o24FDQ5OBkw4lUABve4ZWxpjWB26Hek0Bep0P570DweHw55vw0aVQmFflt6dn5XP++JnMSttNs9hwPvrb0XUyyStyF7Ew3dNf0Deil/n99wDEDB1atTVRu1WIRapHdFgw465+iFMHPMqL5wexPhHYvJOlF55JcVa20+GJiEjt1Do+Pr65y+UKdLFEqQNcLpdt1KhRc6BVuef4cb1TgeestTMpu/rmuopuVBZjTJAx5m5jzBY8c03TvNc5cJPDkXIKXDwZwuJg2RfwzmjIq7wTxua9uZzz0u8s2bKPto0j+ehvR9Oxad0cyVqxZwW5Rbm0jmlNk4gmWGvZN2UKADHDhlbtIr6Km5q2KdXk3CEjuPPcr3hrdCxb4iF0815+Of94CvKU7ImIyEFiNF2zYQsJCQkHyu1z5s8avTg8iVhF1wrx43oAj+FZ87cI+AjY7ef7paraHA2Xfw1vnw1pv8Cbp8OFkyA6sczT1+zM4uIJf7AlI48uzWKYeGV/msaE13DQgTNvu6dRum80L2/xEoq2bCW4aVMievaETXOgMBdikz1bSMTBF9mlZulS/VJbteF/10zn/pwxnPPhapJWZfPelUcz5LlPaJmg0WQREREpUeForj+J3nqgewXHjwNW+XE9gAuBL621I/18nxyKZqlw5XcwcRRsXQCvDfOM9MW32e+0xZszuOS1WezOLqBvm3heu+xI4iL8zeFrj+KsbObt8CR6vvV5JdM2TzoJs3kuvHrArOOIeIhvB70u8GyhUZq6KTUmNjycf9/8KU9nXseIz36h/9xCXvrnGRx//X0M7Rq4dikiIiJSf/kzdfMD4CpjzFGl9lkAY8xVwFnAO37ePxr40s/3yOGIbwtXfg/NjvD0hHt1GGxfWnL4j7W7OG/8THZnF3B850TeurJ/nUzybEEBYXPmsP6ii1nZrx/9n/6RRlmWPk37YK39K9EbNgxWfO15U2xLaNQaXCGQuwe2/Alf3wpPdoMf7ocdyzznJWhET6pfVFgwN/7zBaaeeBoA5//g5oOJ9/P1rKedDUxERETqBH8SvYeAhcAvwHd4krxHjDFrgJeBGcDTft5/NqDfmmtadFO47CtocyxkbYPXh8OGmfy4fDuXvDaLrPwiTuvRnFcu6UdkqKOtFv2Wvmk1qx99gFUnDqHRhFfJmTMHgB7L83jqFTcJPy8mf+UqCtavJyg+nsh+fWHtT543j3gGbloE9+yAW1fB6Neh5ZGQtxdmPAkZGwEDCe3Kvb94NGrUiPj4eBo1auR0KHVaTHgIVz72ENOPHIYLuOVTN9n3vsyMZy7Gut1OhyciItLgGWP63nzzzclOx1GWKv8Wb63NNcYMxrOm7jwgDzgCz3TNu4EnrbWFft7/NuBLY8wX1toZfr5XDkd4HFw0CSZdCcu/pOjNM3g37wbyi3tzfv/WPDgqlSDXofXcc0rB9m2sOvtMGmUUAVCYnEzLq65kVvMc9jz6JL3WWbbefgfB3mbz0UNOxBTsgy3zISgU2gz0XMjl8iTDqWd5to2z4PcXYNnn0OqostfvyX6uvPJKp0OoN2LDQzjvpceYeG0Yg+Z9Sep6C/+bw6JP+9D25nuJOf1MjMufv9mJiIhIoPzwww/L27ZtW2Hjcqf49duBtbbQWvuYtbavtTbKWhthre1hrX3YWnsoH/A2YAcw3Rgz1xgzyRjz4QHbB4dwXamKkHAY8yarWpxJcHEeLwU/wX39CvnvmXUvyXPn5rL86ktplFHE6uZw/0Wh/HTLCBIuuIDZ4Vv577kuVv1tGK7oaIq2e/pKxg4bBmunARZaD4DQyLIv3qo/nPMm3L4WLv60xj6TiE+jqFCunvAQb/zfS3zRP5G9kRCyLZ/Nt9/D9n/43bpURESkzmjRosURtXXEDGDIkCHZHTp0qHCwKzc315FfrJ3+M/BoPAVeDNAbONO778BNqoG1luenr2PomtF8WHQ8wcbN5SFTqtZTrhaxbjdb/nEXISs3sL0RfDy2C0tauXk9/Q1+3vQz83bOA2Noef6ltP/ic2KGDyd6yBCiBgz4a9pm+xMqv1FEvEbzxDERoUE8ecVxBF/0CuMu6MWEYS4KgmDPZ9+z+6G/g1UbJRERkYqsWLEi1BjT9+GHH0686qqrWiYkJPSMiIjofcIJJ3RcsWJFaOlzx48fHz9gwIDO8fHxPSMjI3t37dq123PPPdf4wGseOHXz5ptvTjbG9J09e3b4scce2ykyMrL36aef3h5g0qRJsb179+4SExPTKzIysnfbtm1Tb7311ubV9XmrPHXTGHNJVc6z1k6s6jWttU4nmg2WtZb/fr2MV35ZhzGGiCG3wfTpsPgTOPkhCC+3JUetk/7882R++y05YfDsedFMPPst/rfgf0xcOpGbfrqJIncRIa4QujfpTkhQGC2ffsrzRmthjTfR63Cicx9ApIpcLsPNw1Jo3/Qx7v3lLnLC5nLjF262TvyBYDOa2HFvQli002GKiIjUak8//XTzbt265bz44otp27dvD37wwQdbnHzyyZ1XrFixJCwszAKsXbs2bNSoUXs6d+68zeVy2WnTpsWMGzeuTW5uruv222/fWdk9zjrrrI4XXnhh+u23377N5XKxdOnS0PPPP7/j8OHD99x9991bQkND7YoVK8LWrl1bbb0Q/am08QaeAiwHDvcc+GfkKid64j9jzFhgbJJ3ndmhKCp2c9eni/hwziZCggxPnduL03skQ9oxsP5XWPIJ9L0sYDFXp4wvviT9xf/hNvDUGS6OGjia6NBobu13K2kb0/g582cAujXuRljQAf+Odq3xFFiJbAzNejgQff315ZdfkpeXR3h4OKeffrrT4dQ7o3q1pHXCU4z9/FE+PfoLzvwd1ry3hOZFg2h29duQ1M3pEEVExCFt7/yqr9MxAKQ9fNpcf9/jdrspLi4uc39h4V+zI40xBAcfesHAqKio4ilTpqwOCgoCoGvXrnknn3xylxdffLHxuHHj0gEefvjhbb7zi4uLOe200zK3bdsW8uqrryZWJdEbO3bsjnvvvXeH7/Xrr78eX1hYaN544431CQkJvopqmYf8IarAnxG1E4ATvV9920nA34AFwCxgaKADlP1Za8dba/vFxcUd0vvzi4r5+7vz+HDOJsJDXLxyST9PkgfQxzto++dbAYq2euX8+Sdb774bgLeGBrOoYzAXdr0Q8PwPwOj40YzpPAaAY1sce/AFSqZtDvYUYJGAWbFiBUuWLGHFihVOh1Jv9WndmKlXPMiiE+5kVsdgwvMNy7/KZdaE4bBtkdPhiYiI+O3rr7+OCQ0N7Vt627JlS+gzzzzTvPS+gQMHpvjeU1RURGFhYclWVqJ4oBEjRuzxJXkAw4YNy05KSiqcOXNmlG/fokWLwkaMGNGuadOmPXz3/eCDD5qkpaWFV+WznHfeeXtLvz7yyCNzgoOD7Zlnntn+9ddfj9+8eXO1l7b3p+rm9HIO/WiMeROYCRwJ/BiIwCTwsvOLuOatucxYnU5MeDCvX3Yk/dom/HVC15Hw9W2weY6nt56DowK5OfvYuHw2HXudgKuMJCx3yRI2jr0GW1DAxpO681Wf5ZzU6kRaxrQsOccYw70D7uX8LufTNq7twTdZ4/1Rrcr6PJFaKC4yhHcvvpjXWnQm7b5raJtewJLpUfwWeS7XXv4dYY1aOR2iiIjUsEMZSastjjnmmOzp06cvK71v9OjRHYcMGZJx7bXXloyixcXFlWRzAwcOTJk9e3bJuoVx48ZtffLJJ7dUdJ+kpKSDiqc0adKkcOvWraEAGRkZruHDh3cODw9333fffZs6d+6cHxYWZp9//vnEjz76qElVPkvr1q33u0dqamr+J598surRRx9tdu2117YrKCgwqamp2Q899NCm0047Lasq1/RXQDJJa22BMeZt4AbgkUBcUwJrb04Bl70+m/kb99IkOoyJV/SnW/IB6/BCI+GIMTDnVZj3Fgx/yJlggSlXnk6neTv55shkjnlqIo2atCg5lr96NRuvvAp3VhZRJw/lwaP+hELDxd0uPug6xhg6xXc6+AbFhbDuF8/3HZToSd1ljOHKIQNY3uR99l5+Ht03FJD0nuX2fady7bVv06VpT6dDFBERqZL4+Hj3oEGDckrvCwkJsc2bNy88cL/PK6+8kpaRkVEyPHdgglWW7du3hxy4Lz09PaR79+45AD/++GP0li1bQr/99tsVJ598ckkS9vTTT1e5YqHL5TqoStqIESMyR4wYkZmbm2umTJkSff/99yePGTOm05o1axY1b968qKrXrnIMAb5etVWNkUO3Y18e5748k/kb99KiUQQf/e3og5M8nz7eZGnBe1CUX3NBljJz1qd0mOf5o0372VtYcvrJLJj6IQAFGzey4YorKd67l6hBxzFr7NHsKcwgtXEqvZv2rvpNNs+Fgkxo0hniWlZ+vkgt16VnV7p9NJltLZrTZB+Mfa+IT+48n5fmvECRO+D/3yEiIlIr9OzZM3/QoEE5vq1t27aVJnpffPFFfOkpnt9//33U9u3bQwYMGJANkJ2d7QJPkuk7Z+fOnUFTpkxpFIiYIyIi7MiRIzNvvvnmbbm5ua6VK1eGVv4u/wVkRM8Y0xtPI3UtyKllNuzK4aJX/2DD7hw6No3m7SuPollcBVOLm/eCZkd41vgs/8rTMLwGua2bJeMfZyCwrWcL3Lt2k7wpF/ff7+PbM76g45xtFO3YQeSRR9LimWd467vzALi428X+tYXQtE2ph2I7tOP4b75lxi3jaDJlKmf+BivTnue2y3/nP+eNJzKknF6RIiIiDUh2dnbQ0KFDO44dO3bnjh07gh944IEWbdq0yb/uuut2AZx44olZ0dHRxTfeeGPre+65Z0tWVpbr0UcfbR4fH1+UlZUVVNn1y/Loo48m/vLLL9GnnHJKRps2bQp27twZ/PjjjzdPTEws7Nu3b25gP6GHP+0V1pZzKB6IBYqB6/y4XgTwAvCNtfajqr5PPNbvc5N633eVnpdfVExhsaVnyzhev7w/CVGV/MHAGOh9CXxzG/w5scYTva8XT6LX7N0A9LnncSI6dmbKPZfT/quFtJk8h0JgbXIQj5+4kpxPBpNTlENSZBJD2/pZB6ikrYISPalfXKGhDHruBVa++iiFL06g85YgWj02l6eWj+Rv93xA44iDWgCJiIg0KDfddNPW1atXh1177bVt8/LyXEcddVTmSy+9tMHXWiE5ObnonXfeWXPHHXe0uuyyyzokJiYWXHPNNTt2794d/NRTTx3SDMY+ffrkfPfdd7H//ve/W+7evTs4Li6uqF+/flnvvPPO2ujo6GpphuvPiN4GDm6lYIF5wCpgvLW2vGTwINbaXGPMucCvfsQgXhbIyq/adKzBKYk8f0EfosOq+J+7xxj4/h5YOw32rIf4Noccpz/yi/P5880nGZMPOd3bEndELwBOe+IDZg+eQMGDT7M7spj/joEsVzYUgcEwtsdYQlwHTbUuX+5ez9RNVzC0LaMap0g90PnK28lIKmb7c+OJWB/OWZM2M2XpUI597h1atuzqdHgiIiJVsnnz5oCXkg4NDbUTJkzYNGHChE3lnTNy5MjMkSNHLj1w/4GFXqy1cw88XlYxmJNOOin7pJNOWnM4cfvLn6qbg6vh/vOBztVw3XqvdYyLP/81rNLzjDFVT/B8IuKh20hY9BHMfwdOuOsQo/TPe0veZeBvewHocNWN+x07csRVFJ16GTmF2QwuVYUz2BVMRHCEfzdK+wVsMbQaCGExhxu2SK0Vd9qdhDVNZstL/yRjTgQ9l+WyadTZ5Pz7Pjqfeq7T4YmIiEg1crp52D3AVcaYwQ7HUee4DMSEh1S6+Z3k+fh66s17B9yV9yM5XBn5Gfz6+Yu02A3FifHEDT14KmZwUDCx4XHEhMaUbH4neVBq2uaJhxm1SC1nDOH9L6XVY9NxjWrMxhaWuCxL8c3/Yu7T9zodnYiIiFQjf9botT6UG1hrN1Rw+FpgBzDVGLMCWAMcuBjRWmv1p+ea1uZYiG8Le9I8iVGnk6r1dhMWTeD437MBaHbRpZjgauwh6SvEovV51aZDhw7k5uYSEXEIibgEXEjjtvT41898+/o/mfXLR/SfGUTkSx/z/dZ1nPTQxDJ7VYqIiNQ3KSkpBQdOtazP/PltOo2D1+hVRUWVaUaX+r6LdztQtSxOlEq4XND7YvjxAfjzzWpN9Hbl7mLqr2/zxBqLDQ2h0TnnVNu92L0W9qyD8EaQ7Ec7BvHLqFGjnA5BDmBcQZxy5X/4vMWxzI+4iSOmuWj12Vw+2TmU4S9+SnR4OS1XREREpE7yJ9H7NzAS6AFMAZYBBugKnAQsAD735+bWWv0ZuTbrdQH89B9Y8Q1k7YToxGq5zYrdKzhxtqdnX6MRIwiOj6+W+wCweqrna4cTwHVI1XFF6rSRw09hblIiW1wXkDQ9iO6/beHLC06g/8vv0T5RS6ZFRETqC38SvdVAa6C3tXa/6jfGmJ7AVGC1tfadAMYnTopNhk7DYOW3sPB9GHiD/9fIy4BJV0PnYXDkVWWesmXHGk5Y6Bm4TbjoosOJuHIlid6Q6r2PSC3Wt3c/Nt3+NVuCz8D9UzE9l+aw4KKzcY9/i45tejkdnoiIiASAPyNqdwDPHZjkAVhrF+DpifePQAUmtUTviz1f/3wL7CHMop3zOqz6Dr7/pyfpK8u304gsgIyuLQjvWo1l34sKYN3Pnu9ViEUauJZtOtLtvqmEnxxBdqSly/oiNp5/AYtnT3E6NBEREQkAf0b0OgJ7Kji+C+hQ0QWMMT/iWXN3srW2yPu6MtZaq+EXp3Q+GaKaQvoK2DgLWh9V9fe6i2H2q57vC7NhwQdw1Nj9TrFuNy2+XQBA3pnV/J9540xPHE27QVyL6r1XAzdx4kSys7OJiorikksucTocKUd0QjNS/j2NZQkXsPOrNTRLh6yrb+SXq0Zw3PWPgDFOhygiIiKHyJ8RvY3AecaYgzpTe/dd4D2nIu2BdnjW9pV+XdHW3o8YHWGMucsYs8IY4zbGjCrjeKgx5mljzCpjzBJjzNcOhHlogkKg1/me7+dN9O+9K7+FjA0QFOZ5PXvCQaOC2b/+RqPt2aTHQPzQkwMQcAVKpm1qNK+67dy5kx07drBz506nQ5FKuCLi6P6Pr2j20AOsbGeIzoNGL37BnL/1I3vbKqfDExERkUPkT6L3NDAA+M0Yc6kxZoB3uwz4HTjSe065rLVtrbXtrbWFpV63q2w7pE9Ws6YCpwI/l3P8v0AokGKt7Q5cWVOBBURv74jM4k8hP7Pq75s13vP1xLshprlnVHDd/o9o99tvAfB9HxctG7UJRLTl8yV6Hau3VYRIXdT5uDEM/vAXfu0XSbAboqbnkHbVqeycVXf+LiUiIiJ/qXKiZ619Ebgd6Aa8Bvzq3V7z7vuH9xxHGWNaGmOeM8b8bozJMcZYY0zbcs5tZYz52BiTYYzZZ4z55FD6BVpr/7DWrinnHpHAWOBOa63be/5Wf+9Rxk1xZ2eXuRVnVbRlVbxlZh68hSVRnDSA4uwc7KJJVYtv5wpYOw1CIqHPpdD3cs/+2a+UnFKQlkb29J8pCIJf+0WQEJ5w2I+lXJnbYPsiCI6A1kdX331E6rC4mMac+9o0Ph/ZnMIgcK0OZtu141j/wl1OhyYiIlIrGWP63nzzzclOx1EWv7pSW2sfN8ZMAE4G2uKZgrkWmGKtrWj9Xk3qCJwDzAV+AYaVdZI3AfsRyAcuxbN28EHgJ2NMD2ttdgDj2QPcaYwZChQCj1hrPzuci4Zs2MiKvv0CEZ8fmhO98BlafXlZ5afO8iZ0Pc6FiEbQ91L4+VFY/jVkbIa4Fux+910AZnQ3xDVthanO9UC+JuntjoOQ8Oq7j0gdFxMaw/UPfs5jR4yj32sz6LjVRc5zn7Jixiw6vvQxQXGNnA5RRESk1vjhhx+Wt23btsDpOMriV6IHYK3dC3wQqACMMZ2Am4D+QDwHjzJaa22FRV4O8LO1Nsl77asoJ9EDrsaz/i/FWrvae/5CYBVwDfCkd9+feNpKlKW3tbaydYkh3vevsdbeZYzpAvxijFlc3ihglbgMJjKy3MMVpkwVJVTlHrO4s7LJWp1H0YaVBLeuoN9W3j5Y8J7n+/5Xe77GNIOuI2DJpzD3DYr730TGpE8A+Kafi3bRLSuK+PCprYJIlUWHRvOvi8bzds93ePfFhxnzSzEh8zazfOhxdHr7PUI7pzodooiINGArVqwI7dKlyxFffPHFytNPP92PdUWBN2TIkEoHh3Jzc01ERMQhlK8/PH4nesaYwcBQoCnwhLV2uTEmGk8j9SXW2nJq6Jd5rd541rWFACvwJF5L8CR8yXhGCytLpPbjmx5ZBSOBmb4kz/vedcaYX4Ez8CZ61to+/ty/DOvxjBa+5b3ecmPMfKA34FeiZ4yZ6/u+c+fOdPlzbkWnB9yGU/uRvTab7M/fIO7v/y3/xAXvQUEWtD0Okrr/tf/Iq0sSvYxNLXFnZ7Ova0vWJ23juJhqTPTcxX+N6HVUoidSFcYYLu5xEYsf6M2/J17FpZ/vpf32IlacO4YOzz1B5LGnOh2iiIiIX3wJ4kMPPbRh9erVYZ988knj3Nxc14ABAzJfeumlDSkpKSUjc+PHj49/7bXXElesWBGRn5/vatOmTf511123/YYbbthV+prGmL7jxo3b+uSTT24BuPnmm5Ofeuqp5rNmzVoybty4Vn/++Wf00UcfvW/q1KlrJk2aFPvggw8mr169Ory4uNg0bdq0cPTo0bsef/zxw1/WVYYqJ3reypof4kmQDJ7k5T1gOVAEfAE8gafwSFU9AGQBxwF7gR3A/1lrfzTGXAQ8BZzlx/X80R0oa/rkEmBMoG5irU03xnwHDAc+N8Y0B1KBg/oR+qOwsJBp06YFIMKqa96hFaxdTvqUH5iXWs5AqXXTf9bTRAKLowaSXjpGa+kX1YaorPVsm/wCBpjRKw7YRu623IB/nrS0NKZNm0bMvlX0zd1NbnhT/li0CczmgN6nrvM9p0AqKCgo+VrTP6fVoTqeUV1yee9/8mr0y5zzyUqOWG9Zdd3NuC/8moyjRpec09CfUVXoGVVOz6hyekYih+/pp59u3q1bt5wXX3wxbfv27cEPPvhgi5NPPrnzihUrloSFhVmAtWvXho0aNWpP586dt7lcLjtt2rSYcePGtcnNzXXdfvvtlZYVP+usszpeeOGF6bfffvs2l8vF0qVLQ88///yOw4cP33P33XdvCQ0NtStWrAhbu3ZtWHV9Tn9G9O7Fk+TdDXyHZw0cANbaPGPMJGAE/iV6A4FnrbWrjTG+Shwu7zXfNsYcBzyKJ0kKtATK7gu4G8+IYpUZY+4B/gYkAqnGmOeBftbabd5TrgVeNcb8B3ADt1prV/gbsLW2r+/7lJQUO3jwYH8vcVjyo4tZO+XvFK/fx/HHHosJLuPHZ/VUmL4FYluQetbtEHTAOdH/R9aEf2B2ZRLctDGr+4TDbhjcvhODux0HrqCAxTtt2jQGDx4M02cBENH9NAafcELArl9flDynAJo7dy4FBQWEhoYG/NpOqI5nVNcMP2E4/2n3DDnPj+eolVD41g+0tHvoeNubEBSsZ1QFekaV0zOqnJ6RVOpfcX0rP6kG/CsjYFPPiouLcbv/mrRXVFRkfPsLCwtL9rtcLoKCKv9dMioqqnjKlCmrfed27do17+STT+7y4osvNh43blw6wMMPP+z7PZ7i4mJOO+20zG3btoW8+uqriVVJ9MaOHbvj3nvv3eF7/frrr8cXFhaaN954Y31CQoLvw1TrtFN/2itcCLxurX0Y2FDG8eX43/MunL+mZuZ7v8aUOj4HqM4SiWXNlfW7Ioi19kFrbUtrbZi1ton3+22ljqdZa4dYa4+w1va01r5zWFE7JLTPCYREQ3GeIe/nyWWf5CvC0u+Kg5M8gB7nsmdNHADxzdaxadscAFp89n/w8eXVEDVqqyASAMYY7hl2E00eGs/PRwQTUmTIe/NPpt8+GArznA5PRETqOLfbTWFh4X6bz2233ZYcGhra17elpqamAowaNapz6f233XZblapfjhgxYk/phHDYsGHZSUlJhTNnzozy7Vu0aFHYiBEj2jVt2rSH7/offPBBk7S0tCpV9TvvvPP2ln595JFH5gQHB9szzzyz/euvvx6/efNmv5fQ+cufG7QEZlZwPAuI8/P+m73XxVqbbYzZg2ft2qfe4x3wVKmsDnvwjOodKJ6yR/oaPONyEZXakr0zN5H97adEnDh6/xN2r/M0SQ8K9bRUKEPh7kyyNoeAyxJ7ZDM2h3im+LUoKoK0GYEPOncvbJoNrmBoNyjw15cyHXnkkeTn5xMWVm2zEcQhp3c/llUvTuHrm0cxbHYGTb/axdsZR5E45l6nQxMREQjoSFpN+vrrr2NGjBixX7U/a+1cgBtvvHHnqFGj9vr2b9q0KeTCCy/s+Oijj64/6qijcnz7W7duXaW8ISkp6aDzmjRpUrh169ZQgIyMDNfw4cM7h4eHu++7775NnTt3zg8LC7PPP/984kcffdSkKvc4MJbU1NT8Tz75ZNWjjz7a7Nprr21XUFBgUlNTsx966KFNp512WlZVrukvfxK9XXgKpJTnCDyJmz9+A4YA93tffwncYowpxDPaeAMwxc9rVtUSPOv0DtQNWFpN9zxsxpixwNikpCRH7h89eAh7Z75J1twlHPRTPudVwELq2RCdWOb79076BKwlZvhw9lx3J4Ufn0RCeAKRwemQswtydkNkAPvprfsZbDG0PgbCYwN3XanQoEFKquuzTonNuPrVX5hw8/kM+WEJfWcUMGPfP/mtXRgDO49wOjwREamDjjnmmOzp06cvK+tY27ZtC9u2bVuSOK1YsSIUoGvXrvmDBg3KKes9Fdm+fXvIgfvS09NDunfvngPw448/Rm/ZsiX022+/XXHyySeXJGFPP/10lWf+uVyug2YOjhgxInPEiBGZubm5ZsqUKdH3339/8pgxYzqtWbNmUfPmzYv8/RyVxuDHud8CVxljGh14wBjTHbgC+MrP+78AzDDG+IZA78BTafN+4D48FSvH+XnNqvocGGCMKZlu6m2sfoz3WK1krR1vre0XF+fv4GlgRJ5+CRhL7pY8irev/+tAQQ78+Zbne19LhQPY4mL2TvI0XI8fM4ZNWZsAaBnTEhp7O2jsXhvYgHd4c/ZW/QN7XZEGLjI0hBue+4gFF59LYRAcu9Cybtwd/OfbWylyB/z/q0REpJ6Lj493Dxo0KKf0Vl33+uKLL+KLi4tLXn///fdR27dvDxkwYEA2QHZ2tgsgJCSkJFnbuXNn0JQpUxoF4v4RERF25MiRmTfffPO23Nxc18qVK0MDcd0D+ZPo3QeEAQuAf+JZ33a+MeZVYDaeqpn/8efm1tpZ1tq7rLV53tfb8LRp6IVnhPAIa+06f64JYIwZbYwZDfgWo57i3Xd8qdNeAdKAz4wxZxhjRuKpwrkReNnfezYUQU2SiWwZAdaQ/cXEvw4s+gjy9kKLftCi7DXA2b/+StHWrYS0bEnkgAFszvIMALeIbgGNO3pOSl9V9WC2LYaXjoM1P5V/zj7vIHNcNffpE2mAjDFccPe/2HP3v8kPhz5rLL0e/op737qQQnd1zboXERE5PNnZ2UFDhw7t+P7778c9++yzjS+88MIO3vYJuwBOPPHErOjo6OIbb7yx9fvvvx83YcKE+GOOOSYlPj7+kP+S+eijjyaOGDGi3Ysvvpjw1VdfRb/xxhuNHnrooeTExMTCvn375gbu0/2lyometzH40cBi4Ho8RUuuBC7D0wvvWGvt9sMNyHostNYusdYWV/6OMn3k3f7mff2i97VviijW2mzgRGAlnh537wDrgBOttdUyTzYQjDFjjTFzMjKq3K4w4KKOPAKArOnTPDus/asIS/+x5b5v70cfA9Bo9GiMy8WmTO+IXnRLaNzJc9Ku1eW9/WAznoJtC2Hhh+Wfk+FN9GKV6IlUl+MvGMPa624lP8bQfhuc+dRCHn1gCIVFKtIiIiK1z0033bS1ffv2eddee23bO+64o3X37t1zvv3225W+1grJyclF77zzzpri4mJz2WWXdbj//vtbXHLJJemjR4/efaj37NOnT05OTo7r3//+d8szzzyz82233da6VatW+VOmTFkRHR1dLc3U/ar2Yq1dC5xmjIkDOuNJFNdYa9MPJwhjzFA8TcrbeXetAz6z1h7S+jxrbZXmz1prNwBnH8o9nGKtHQ+MT0lJqZYfiKqIPmU0Oz+ZTfbSLVi3G7NxJmxfBFGJ0H1Ume8pSk8n86efICiIuDPPBPgr0YtpCUHev/5XNdHLz4Tl3pnCGRvLP883ohdbpSJMEiBPPfUUWVlZREdHM25cdc2+ltokoXMHWn7yA8uvPJPGG/Yx6r2dvLXuSM59bDJRiR2cDk9EROqRlJSUAl+hlkMRGhpqJ0yYsGnChAmbyjtn5MiRmSNHjjyoboevMbrPgXE8+eSTWw48B+Ckk07KPumkk9YcasyHokojesaYCGNMsTHmXgBrbYa1dra19o/DSfK8152MZ/3fdXgKswzxfv+tMeYLY0zEoV5fqkfYMacTFGEpyob8P76HWeM9B/peBsFlV1nc++mnUFRE9PHHE5LUFKBk6qZnRM87dXNXFX/+l30BRd5R7r1ldfvw2uf9d6apmzXK7XaXbNJwNGmVzNFf/8a6IX0AOHpmEb9ceBqbp7/vcGQiIiINT5USPWttLp5G4oc1cleGh/A0Yf8f0MFaG26tDcfTVuEl4DTvOVKLGJeL6K7NAMj+dAIs/RxMEPQtuw+etZa9H3unbY75qyWDb0SvRUyLv4qx7FoNVUkOFn7w1/f7NoP74Fm+QUU5kL8PgiMgIr4qH01EDlNQcBCnvvAOm2+/hn0R0GaDYeu4f7Ho4bGead4iIiJSI/wpxvIVMDzA9z8f+MBa+/fSRVesteustdfjWVd3foDvKQEQ5S2fn/XHn572BV1HQFyLMs/N+WMWhes3EJyURPRxxwGQX5zPjtwdBJtgkiKTIKKRZ+pnUS5kHjTavb99W2HtdE+/vvA4cBdB5taDTgvL9/5dIjYZTJWr4YpIAAy74ibMq8+zvJWLqBxD8Bu/8MfooynetcPp0EREpIHyTfm8+eabAz14VSv5W3WzrTHmDWNMf2NMY2NM5IGbn/ePAqZXcPwnwN9r1mu1oRgLQNTIyz1tFnaG4i40lRRh+QiARmefhQn2LAv1TdtsFtWMYJd3qWjJ9M1K1ukt/hiw0GnYX0Vc9h68Tq8k0SsnARWR6tW/zxAGTPqRz4bEkx8MsUsyWDBsMBlff+p0aCIiIvWeP8VY1uFpqXAEcHE551g/rzkHTyuF8vTyniNetaEYC0BwcjsimoWSu7WQtT+0wMx/yFOHtQwFaevBGBqd/Vfdm82Z3vV5MaXWzjXuABt+97RYaD+4/Jv7pm32OBeWfAKb53gLshy932nheb4RPa3PE3FK89gkbnvuF/750vUcOWk6KZstW26+i91rl9Hu73c5HZ6IiEi95U9SNhFPIhdINwFTjDErgRd9/fS8DdT/DpwFDAvwPSVAYk88htx3plGY4YaMiouoxAw9iZAWf42s+Zqlt4guNdpW0mKhgmttXwrbFnmmbHYa5knyAPauP+hUjeiJ1A5BriD+c91LvNjpPZZ9+CCjfnGT9/xbfJeeydB//heXS1OrRUREAq3cRM8Y0xrY6S3EgrX2smq4/3ggC3gMeNAY4yuf2AoIBzYA483+66ustfaoaohF/BR/9wtEn7MY66qkMKrLRWjr1vvtKntErwpTNxd5e+Z1GwUh4RDXyvO6oqmbaq0gUitcN/R8prVI5fPg8xn5UzGt35/M41vTOfEfj9CvbYLT4YmIiNQrFY3orcMzRfNdAGPMj8B/rLVTA3j/pnhGCX0Jnq82f+nV+okBvJ8EkHG5CE3pcUjv9Y3otYwuK9FbVfab3G5Y6FnvR8/zPF8beRPIMnrpheXv8nyjqZsitcbgbkfQ75EpTLxzGCf8WMSI6TN4Le96vjz7Hu4b0Q2jwkkiIiIBUVExlkIgtNTrwUBSIG9urW1rrW3n7xbIGOqa2lKM5XCV9NArPaKX0A6My9MXryj/4Ddt+A32bYK41tBqgGdfVUb0NHVTpFaJjm3ONY/9yPwTQwC44o/55H5yJ6/8XM4feURERMRvFSV6q4GLjTE9jDFtvPsaG2NaV7TVQMwNmrV2vLW2X1xcnNOhHDJrbUkPvf1G9ILDPCN01g170g5+Y0kRljHg8v7oNvImehkb9+/RZW2pYiyaulnTTj75ZEaOHMnJJ5/sdChSSwVFJXLeIz+wfrBnYsllM1djnz2PSXPmOhyZiIhI/VBRovcInlG8ecBaPFMsn8YzpbOiTaRC+wr2kVWYRVRIFHFhBySs5a3TK8yDJZ95vj/inL/2h8V4mqEX5UH2zr/252UQ5M6DkCgIbxTwzyAVS01NpXfv3qSmpjoditRiJqYpwx/9nuzh4RQEw6AluYTedjFvf/uc06GJiIgcti+//DLGGNP3yy+/jHHi/uWu0bPWvmWMWQCcBDQDbgG+AZbVUGxST5UezTtoPU7jTrD6B0+LhdJWfgv5GdC8JzTtsv+xuFaQu8czfTO6qWffvs3eYy3ULF2kNottTr/H/2Db23ey4YWv6bgV9t79Io8u+5brr/+AqNBopyMUERE5JAMHDsz+4Ycflvfu3TvXiftX2DDdWrvQWvuktfZ2PF3S3rXW3lbRVjNhS11WZmsFn8YdPF8PHNFb6K222ePcg9/jK8hSusVChjfRi9X6PJFaLziUZpc9SbeJE9mVHESjbDjllbU8fffxpGdtdTo6ERFxUIsWLY64+eab/VqH8+yzzzY2xvStrpiqKiEhwT1kyJDshIQEd0Xn5ebmVsuoRIWJXmnWWpe19t3qCEKqrj4UYykZ0YspoxpmydTNUr30cnbDqu89hVpSzz74PWVV3tynRM9Je/bsYffu3ezZs8fpUKQOie7an/Yf/sbirq0JdsNZX+Tw+s3DWLt9odOhiYhIA+BLEL/55pvok046qUNkZGTvRo0a9br44otbZ2Vl7ZeMjRs3Lrlbt25dY2JiesXHx/ccMGBA56lTp0aVPqesqZv9+/dP6du3b8q7774b17Vr126hoaF9Hn300USABx54oGn79u27h4eH94mNje2VmpradeLEiY0O9fP40zBdagFr7XhgfEpKSqCb19cYX8XNMkf0mviappeaurnkU3AXQocTIabZwe8pq/Jm6ambUuNee+01srKyiI6O5pZbbnE6HKlDkpvE0vX5D/nhrps58Y/fOP3nIr656TwG/Otx+qac6nR4IiLSAFxxxRXtRowYsee6665bM3PmzKinnnqqeU5OjmvSpElpvnO2bNkScv31129v3bp1YVZWluudd95pPHz48JQZM2YsO+qooyqcqrlu3brw2267rfVtt922pWPHjgWJiYlF//vf/xLuv//+VjfddNOW448/PisnJ8e1YMGCiF27dh1yvqZET2pchSN6MckQHOEprJK7FyIalZq2eV7ZFyxdedNHUzdF6qzUFnG0Hf8yHz3wMP0+fYcT51nm3HoL629dzVnH3+h0eCIitdoRbx7h+JRFgEWXLvK7jLLb7aa4uLjM/YWFhSWvjTEEB/+VxhQVFWFLVV93uz0zJUu/ByAoKAiXq/IJjSeccELG+PHjNwGcddZZ+4wx9vHHH2+xcOHCrT169MgH+OCDD0rWDBUVFTF69OiMTp06pb700ktNjjrqqIP7fpWyd+/e4C+//HLpwIEDSxLCF154IbFz5845jz/+eMmahXPPPfewpvBVeepmdTHGBBljrjbGfGmMWeLdvvTuUyJaD8WFxdEkosn+rRV8XK6/1untXgO718HGmRASCV1OK+eCvhG9DX/t27fJe0yJnkhdFB0WzOUP3sPeux8gLwz6rQLzwP/4/JN7nQ5NRESqyddffx0TGhrat/S2ZcuW0GeeeaZ56X0DBw5MKf2+gQMHppQ+Pm7cuLYAB17r66+/rlL1y/POO2+/tSeXXHLJHrfbzYwZM0qmZk6ePDnmqKOO6tyoUaNeISEhfUNDQ/uuX78+bPXq1eGVXT85ObmgdJIHcOSRR2YvX7488tJLL201efLkmMzMzMPO0xxNpIwxCcB3QB+gAPBl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2v3CtDT7s83sFsZr2xYz9M1xZOU4NSuVIzHBdndIEYljKvREREREYkCraq2om1SXjTs3MnfrAg5o/yMJyVt5tVdTEqtXh8REVrYsx7LkJGrveI0mNSpy47Ftgo4tIgFJCjqAiMSf2rVrU7FiRSpVqhR0FBGRuGFmdKrUic82fca7C97lp+1TAVi8/p/sfPxoWiZl0GX1W/yw5iPW1viJh45uR8Vy+lVPpKzSd7+IFLtzzz036AgiInGpU8VQoTd28VgA6iS3Y+HWVjz1yw4ePaMjH05YRcVqHzK3QiKVNrwHXBxsYBEJjG7dFBEREYkR9ZPr06xqsz9f33bo1ZRLTOSzeau4dvT3/Lomh322NQXglXkvB5RSRKKBCr0YownTRUREyi4z45jmxwBweMPD6dH8YPoe2Ah3+PiHlSQYDDzidhLd+a9vZtXy6QEnFpGgqNCLMZowXUREpGw7v/35XH/g9Qw9bCgAFx/Rgl0Da154RAv+sf8h/CO5FllmvDH1/gCTikiQ9IyeiBS7MWPGsH37dipUqECfPn2CjiMiElcqJFXg3Hb/exa6ac1K3HLcvsxfuYWr/9EagHM7XMLYmfcwK30xnpODJehv+yJljQo9ESl2CxcuJD09ncqVKwcdRUSkTLjg8BZ/eb1/uzN4OSeTju3PUpEnUkap0BMRERGJN2YcsP85QacQkQDpTzwiIiIiIiJxRoWeiIiIiIhInFGhJyIiIiIiEmdU6ImIiIiIiMQZFXoiIiIiIiJxRoWeiIiIiIhInFGhJyIiIiIiEmc0j56IFLu0tDR27NhB+fLlg44iIiIiUiap0IsxZnYRcFHdunWDjiKyWyeccELQEURERETKNN26GWPcfYS7H5iamhp0FBERERERiVIq9EREREREROKMCj0REREREZE4o2f0RKTYPf/882zdupVKlSoxaNCgoOOIiIiIlDkq9ESk2G3cuJH09HQyMzODjiIiIiJSJunWTRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4owKPRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4oy5e9AZJEJmNhPYH/i+BA5fC/ijBPYpqM3utuW3Pu+63b3eN/x6fiG59kS89BFEVz8VtX2k/bQn66K1j4q6T3F8LamPirZeP5MKX68+Kny9+qjw9ZH0UTl3Ty4kl0j8c3ctMbYAM4GZJXTsGSWxT0Ftdrctv/V51+3utfqoaK+jqZ+K2j7SftqTddHaR6X5taQ+2rOvL/1MUh+pj+K3j7RoibVFt25KXiNKaJ+C2uxuW37r864r7HVJUB8VTaTnKWr7SPtpT9ZFax8VdZ/i+FpSHxVtfTR8v6mPCqc+Kpz6SCTO6NbNGBS+dRN37xx0lmilPioa9VPh1EeFUx8VTn1UOPVR4dRHhVMfifyPCj0REREREZE4o1s3RURERERE4owKPRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4owKPRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4owKPRERERERkTijQk9ERERERCTOqNCLU2Z2i5n9bGY5ZtYn6DzRxszKm9kYM5tvZrPNbKyZtQg6V7Qxs3Fm9n24jyabWcegM0UrMzvPzFzfb/kzs8Xhn0mzw8sFQWeKNmZWzsweM7MFZjbPzD4JOlM0MbMGub5+Zof7KcvMagSdLZqY2XFmNtPMZpnZHDM7N+hM0cbMjjGzGWb2g5l9Y2Ydgs4kUhKSgg4gJWYcMAp4PuggUWy4u48FMLMhwHNAz2AjRZ1T3H0TgJmdDLwEdAwyUDQys6bAhcA3QWeJcme4++ygQ0Sxe4FyQJq755hZ/aADRRN3X0Gunz9mdhPQ1d3XBxYqyphZAjCSUL/8GP7Z9IuZvevu6QHHiwpmVh14HTjM3eebWdfw6/bBJhMpfrqiFyXMrJGZPWFmU81sW/jKQLPdtG1sZm+b2SYz22xm75pZk9xt3H2auy8slfClpDj7yN137Crywr4BYv6KXgl8HW3K9bJqSWYvLcXdR+FfrJ4HLgd2lvw7KB3F3U/xqDj7yMwqAhcBN7l7DoC7ryyVN1KCSvjr6Hzi4I+ZxdxHFv646ypnNWAdkFFib6AUFHMftQTWuft8AHefAjQxswNK/p2IlC4VetGjFXA6sAGYvLtG4V8GxgNtgAHAOcA+wJdmVqkUcgapJPvocuD9Yk0bjGLvIzN73cyWAf8C+pdQ7tJU3H10DfC1u88sscTBKInvt1csdCvZK2bWsGRil6ri7KNW4ePcZGbfmtkUMzupJMOXkhL5uW1mRwBVgI9LIHNpK7Y+cvds4DRgjJktCR/vXHeP6UKP4v06WgDUMLNu4X16E/paalZS4UUC4+5aomABEnJ9fgHgQLN82l0JZAOtcq1rDmQB1+TTfgLQJ+j3F+V9dDMwFagY9HuM1j7KdbyPg36P0dRHQDtCV4OTw6/1/babryWgafhjEnAHMDXo9xhNfQR0Du8/KPy6DbAWaBn0+4yWPsrT/mXg/qDfX7T1Ufj7awJwRPj1QcAKoFbQ7zNa+ii87ohwP80EHgfmAScG/T61aCnuRVf0ooSHb9Upgt7AN+7+a659FwFfA/Hw19/dKok+MrPrgFOBY919W3FlDUoJfx09DxxtZjX3LmWwirmPjgCaAgvMbDFwCDDCzAYXX+JgFPfXkrsvCX/MAh4FDjaz5OJLXPqKuY+WEPrl9dXw9p+A2UCn4sobhBL6uV2V0M/tmL9tE4q9jzoCDdx9Unj7t8By9HWU9+fRJHfv7u6dgRuABsD8YowsEhVU6MWedsDcfNbPA9qWcpZoVaQ+MrNrgH7A0e6+sXSiRY1C+8jMqttfB4M4FVgDlJWBDwrtI3cf7u713b2ZuzcjdHXvIncfXnoxA1eUr6VKZlYt17azgbnunlny8aJCUb6W/gDGAscAhL/32gNzSilj0CL5v60fMNPdF5R4quhSlD76HWhgZru+91oRuu3x51JJGLyi/v+f+/+224HxuYtDkXihUTdjTw1C96jntR6ovuuFmd0GXALUBtqb2TDgQHdfVSopg1VoH5lZI+Bh4DdC9+4DZLn7gaUVMmBF+TqqDowys/JADqEi7wR399KJGLgifa9JkfqpLvCOmSUSGizid0LPEZUVRf1aGgw8b2b3EPqeu87dy8ov6JF8vw0CnijxRNGn0D5y99VmdiGhn905hP6gf5m7Ly29mIEq6tfR3WZ2OKHfg6cS+poSiTsq9GJTfr9o218auA8FhpZOnKhUYB+5+zLy9FkZVFgf/Ubo+Y6yrNDvtb80du9eclGiWlG+lmL61rFiUJSf24uBo0olTXQq0vebu3cphSzRqihfR28Ab5ROnKhUlD66sJSyiARKt27Gng38b9jk3KqT/1+xyiL1UeHUR4VTHxWN+qlw6qPCqY8Kpz4qnPpIJBcVerFnHqF70PNqC/xYylmilfqocOqjwqmPikb9VDj1UeHUR4VTHxVOfSSSiwq92PMBcIiZ/Tm5d3jS0G7hbaI+Kgr1UeHUR0Wjfiqc+qhw6qPCqY8Kpz4SycXKzrgK0c/M+oY/PYrQQCqXEppHaa27Twy3qQR8D2wHbiN0L/q/CE32ub+7p5d27tKkPiqc+qhw6qOiUT8VTn1UOPVR4dRHhVMfiUROhV4UMbPd/WNMzD3Ig5k1ITQP1dGEHjAeB1wVfpA/rqmPCqc+Kpz6qGjUT4VTHxVOfVQ49VHh1EcikVOhJyIiIiIiEmf0jJ6IiIiIiEicUaEnIiIiIiISZ1ToiYiIiIiIxBkVeiIiIiIiInFGhZ6IiIiIiEicUaEnIiIiIiISZ1ToiYiIiIiIxBkVeiIiUcTM3MxeyvW6WXjdXcGlig1mdle4r9oHnUVERCRoKvREROKQmVULFz7dg84iIiIipS8p6AAiIlKgJUAFICvC/aoBd4Y/n1CMeURERCQGqNATEYli7u7AjqBziIiISGzRrZsiIgEws6Zm9p6ZbTGzDWb2hpnVzafd357RM7NEM7vBzOaZ2VYz22hmc8zs3vD27sCicPM7w/u7mU0Ib69iZveY2QwzW29mO8L7X5rP+Xc993aAmQ01s+Xh9tPNrFs+7RPM7HIz+87MtoWzTTOz8/O0q2lmj5nZEjPLMLNlZvaEmaXuea/+qaKZDTOz1eEM482sQ57zdw+/ryFmdoWZ/ZqrH04rhgwiIiKB0hU9EZFSZmbVgclAXeBJYCFwPPBpEQ9xO6HbMl8B/kPoZ/k+QPfw9vnA1cCjwHvAu+H1q8MfGwLnAW8DLwLJwCnAk2ZWw92H5nPOp4GdwL+BysB1wIdm1szdN4fflwGjgL6Ebhe9E9gOdAB6Ay/kev9TgVrACOA3oB1wCXCImXVz94wi9kV+RhC6Cnpv+ByXAxPNrLO7L8zT9oJwm6fD+wwCRpmZu/vbe5FBREQkUCr0RERK341AY+B0dx8NYGZPAaOBTkXY/yTgU3cfkN9Gd19tZmMIFXo/uPtreZr8BjRx9z+f+zOzx4EvgOvN7AF3z8yzzybgn+6eE27/E6FC8SxCRRLAmYSKvOHAZeHbTncd33IdayhQDzjA3X/N1eYbYCTQn3BRuIdygCPdfWf4uB8C08Ln7ZenbWugjbsvDbd9DpgHPGpm77l79l7kEBERCYxu3RQRKX0nAUsJFUrAn8/iPVTE/TcCbc1s3z05ubtn7CryzKycmdUAahIq9KoCbfLZbdiuIi/sy/DHVrnW9QOygVtyF3nhc3r4fAacAYwHNppZrV1L+JhZwNF78r7yZN2Z69zTCV1BPcHM8v6/9/auIi/cdiPwPNAI6LyXOURERAKjQk9EpPQ1B37OWwwRuuWyKG4DKgE/mtnPZjbczI7Pc9VstyzkqvBVuR3AOmAtoVsdAarns9vi3C/cfX3405q5Vu8DLAkXS7tTO7zPSeFz5l5WErrTpE5R3kcBfspn3c+EbjmtXcS2EPp3EhERiUm6dVNEJMa4+9dm1gI4FugJ9CL0fNs4Mzsm9y2Zu3EdoWftPgbuJ/TsXiZwHKFn+/L7I+DubmEsUnGZy65jf0Lo1tL8bIjwmCIiIpKHCj0RkdK3CEiz8IgfudYX+VZMd98CvBVeMLMHgBsIFX8fAnmvFuZ2VjjDiXmeo+tZ5HeQv1+A48ws1d037abNWkLP+1V09y/28ny70waYkmddGpAePn/etnmlhT8uymebiIhITNCtmyIipe8DoAmhgUuAP59du7YoO4efZ8trVvjjrlsp08Mf87sNM5tQIfjn/wFmVhM4P5+2kXiT0B8Q/zZq567bSsODm4wCuptZr3zaJYVH5dwbQ8wsJdcxuwCHAx/nec4QoK+ZNcnVNpXQyJvLgZl7mUNERCQwuqInIlL6/k3oqtprZnYo/5teoX4R959vZlOA6YSea2sKXAqsJ3RLJO6+zswWAmea2a+ErmStcffxhKZcGAp8FB6dsw5wEaHi5m9z+UXgTeA0QoVWW0LTRWwD9iM0yubJ4XY3A0cAn5jZq8AMQv8ftQJOJXRl8jUAMxtIaAqI/3P3u4qYI4HQdApv8L/pFTYTmpYir1+AKWY2nND0EYOABsCZGnFTRERimQo9EZFSFi7CjgAeI1RgZQKfEZrbblURDvEwcAJwFaFRMlcBHwH3uPuaXO3OAR4BHgAqABMJjXb5AFAOGAD0IHSL4gOErgK+uBfvy8OTjV8Zfi9DCQ328jOhKRd2tVtvZocQmmbiVEJF71ZgCfAyoTn4dqkS/rg8gigXAecCt4b3/wa4xt0X5NP2OUKF4ZWERtr8lVCRNyqC84mIiEQd+/ugbyIiItHBzN4B9gfa5jO3394ctzuh6Rwud/dhxXVcERGRaKEreiIiEpXCc971AC4sziJPRESkLFChJyIiUSk8cEqNoHOIiIjEIo26KSIiIiIiEmf0jJ6IiIiIiEic0RU9ERERERGROKNCT0REREREJM6o0BMREREREYkzKvRERERERETijAo9ERERERGROKNCT0REREREJM78P6xy8rfhFnAYAAAAAElFTkSuQmCC\n",
+                        "image/png": "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RM9Je/bsYffu3ezZs8fpUKQOie7an/Yf/sbirq0JdsNZX+Tw+s3DWLt9odOhiYhIA+BLEL/55pvok046qUNkZGTvRo0a9br44otbZ2Vl7ZeMjRs3Lrlbt25dY2JiesXHx/ccMGBA56lTp0aVPqesqZv9+/dP6du3b8q7774b17Vr126hoaF9Hn300USABx54oGn79u27h4eH94mNje2VmpradeLEiY0O9fP40zBdagFr7XhgfEpKSqCb19cYX8XNMkf0mviappeaurnkU3AXQocTIabZwe8pq/Jm6ambUuNee+01srKyiI6O5pZbbnE6HKlDkpvE0vX5D/nhrps58Y/fOP3nIr656TwG/Otx+qac6nR4IiLSAFxxxRXtRowYsee6665bM3PmzKinnnqqeU5OjmvSpElpvnO2bNkScv31129v3bp1YVZWluudd95pPHz48JQZM2YsO+qooyqcqrlu3brw2267rfVtt922pWPHjgWJiYlF//vf/xLuv//+VjfddNOW448/PisnJ8e1YMGCiF27dh1yvqZET2pchSN6MckQHOEprJK7FyIalZq2eV7ZFyxdedNHUzdF6qzUFnG0Hf8yHz3wMP0+fYcT51nm3HoL629dzVnH3+h0eCIitdoRbx7h+JRFgEWXLvK7jLLb7aa4uLjM/YWFhSWvjTEEB/+VxhQVFWFLVV93uz0zJUu/ByAoKAiXq/IJjSeccELG+PHjNwGcddZZ+4wx9vHHH2+xcOHCrT169MgH+OCDD0rWDBUVFTF69OiMTp06pb700ktNjjrqqIP7fpWyd+/e4C+//HLpwIEDSxLCF154IbFz5845jz/+eMmahXPPPfewpvBVeepmdTHGBBljrjbGfGmMWeLdvvTuUyJaD8WFxdEkosn+rRV8XK6/1untXgO718HGmRASCV1OK+eCvhG9DX/t27fJe0yJnkhdFB0WzOUP3sPeux8gLwz6rQLzwP/4/JN7nQ5NRESqyddffx0TGhrat/S2ZcuW0GeeeaZ56X0DBw5MKf2+gQMHppQ+Pm7cuLYAB17r66+/rlL1y/POO2+/tSeXXHLJHrfbzYwZM0qmZk6ePDnmqKOO6tyoUaNeISEhfUNDQ/uuX78+bPXq1eGVXT85ObmgdJIHcOSRR2YvX7488tJLL201efLkmMzMzMPO0xxNpIwxCcB3QB+gAPBl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2v3CtDT7s83sFsZr2xYz9M1xZOU4NSuVIzHBdndIEYljKvREREREYkCraq2om1SXjTs3MnfrAg5o/yMJyVt5tVdTEqtXh8REVrYsx7LkJGrveI0mNSpy47Ftgo4tIgFJCjqAiMSf2rVrU7FiRSpVqhR0FBGRuGFmdKrUic82fca7C97lp+1TAVi8/p/sfPxoWiZl0GX1W/yw5iPW1viJh45uR8Vy+lVPpKzSd7+IFLtzzz036AgiInGpU8VQoTd28VgA6iS3Y+HWVjz1yw4ePaMjH05YRcVqHzK3QiKVNrwHXBxsYBEJjG7dFBEREYkR9ZPr06xqsz9f33bo1ZRLTOSzeau4dvT3/Lomh322NQXglXkvB5RSRKKBCr0YownTRUREyi4z45jmxwBweMPD6dH8YPoe2Ah3+PiHlSQYDDzidhLd+a9vZtXy6QEnFpGgqNCLMZowXUREpGw7v/35XH/g9Qw9bCgAFx/Rgl0Da154RAv+sf8h/CO5FllmvDH1/gCTikiQ9IyeiBS7MWPGsH37dipUqECfPn2CjiMiElcqJFXg3Hb/exa6ac1K3HLcvsxfuYWr/9EagHM7XMLYmfcwK30xnpODJehv+yJljQo9ESl2CxcuJD09ncqVKwcdRUSkTLjg8BZ/eb1/uzN4OSeTju3PUpEnUkap0BMRERGJN2YcsP85QacQkQDpTzwiIiIiIiJxRoWeiIiIiIhInFGhJyIiIiIiEmdU6ImIiIiIiMQZFXoiIiIiIiJxRoWeiIiIiIhInFGhJyIiIiIiEmc0j56IFLu0tDR27NhB+fLlg44iIiIiUiap0IsxZnYRcFHdunWDjiKyWyeccELQEURERETKNN26GWPcfYS7H5iamhp0FBERERERiVIq9EREREREROKMCj0REREREZE4o2f0RKTYPf/882zdupVKlSoxaNCgoOOIiIiIlDkq9ESk2G3cuJH09HQyMzODjiIiIiJSJunWTRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4owKPRERERERkTijQk9ERERERCTOqNATERERERGJMyr0RERERERE4oy5e9AZJEJmNhPYH/i+BA5fC/ijBPYpqM3utuW3Pu+63b3eN/x6fiG59kS89BFEVz8VtX2k/bQn66K1j4q6T3F8LamPirZeP5MKX68+Kny9+qjw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",
                         "text/plain": [
                             "<Figure size 921.6x633.6 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
```

### Comparing `pairtools-1.0.3/doc/examples/pairtools_walkthrough.ipynb` & `pairtools-1.1.0/doc/examples/pairtools_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/formats.rst` & `pairtools-1.1.0/doc/formats.rst`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/index.rst` & `pairtools-1.1.0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
    quickstart
    installation
    parsing
    sorting
    formats
    stats
-   technotes
+   protocols_pipelines
+   designnotes
    cli_tools
 
 .. toctree::
   :maxdepth: 3
   :caption: Tutorials
   :titlesonly:
```

### Comparing `pairtools-1.0.3/doc/installation.rst` & `pairtools-1.1.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/parsing.rst` & `pairtools-1.1.0/doc/parsing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -280,11 +280,25 @@
 
 - "E1_R1" is a pair obtained by combining left alignment of some pair in R1 read and right alignment of the next pair in R1 sequence of the same read.
 - "E2_R1" is a pair obtained by combining left alignment of some pair in R1 read and right alignment of the pair separated by 2 alignments in R1 sequence of the same read.
 - "E2_R1&2" as above, both source pairs were sequenced on both R1 and R2.
 - "E4_R1-2" is a pair obtained by combining left alignment of some pair in R1 read and right alignment of some pair in R1 sequence, separated by at least 4 alignments in between.
 Note that "-" in the pair type means that pair is separated by unsequenced gap, which may contain other pairs.
 
+Aligner settings
+-----------------
+
+We recommended using local DNA sequence aligners, such as `BWA-MEM <http://bio-bwa.sourceforge.net/>`_ and `Bowtie2 <http://bowtie-bio.sourceforge.net/bowtie2/index.shtml>`_ (in the local alignment mode), 
+as opposed to global aligners (e.g. Bowtie2 in the end-to-end mode). 
+Local aligners assume that DNA molecules may contain fragments aligning to different locations in the genome and thus are better suited for mapping chimeric Hi-C molecules.
+
+Aligning Hi-C reads may further require adjusting aligner settings.
+Some aligners assume DNA libraries contain only contiguous fragments, leading to 'mate rescue' where one read's alignment is modified or even forced based on its pair's alignment. 
+This behavior is incompatible with Hi-C, which produces chimeric molecules with unrelated alignments on each side. 
+To avoid erroneous results, disable mate rescue/pairing and align reads pairs independently. 
+In `bwa mem`, use the '-SP' flags to achieve this.
+
+
 .. [1] Following the lead of `C-walks <https://www.nature.com/articles/nature20158>`_
 
 .. [2] This procedure was first introduced in `HiC-Pro <https://github.com/nservant/HiC-Pro>`_ 
    and the in `Juicer <https://github.com/theaidenlab/juicer>`_ .
```

### Comparing `pairtools-1.0.3/doc/quickstart.rst` & `pairtools-1.1.0/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/sorting.rst` & `pairtools-1.1.0/doc/sorting.rst`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/doc/technotes.rst` & `pairtools-1.1.0/doc/designnotes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Technical notes
-===============
+Design notes
+=============
 
 Designing scientific software and formats requires making a multitude of 
 tantalizing technical decisions and compromises. Often, the reasons behind a 
 certain decision are non-trivial and convoluted, involving many factors.
 Here, we collect the notes and observations made during the desing stage of 
 `pairtools` and provide a justification for most non-trivial decisions.
 We hope that this document will elucidate the design of `pairtools` and
```

### Comparing `pairtools-1.0.3/pairtools/cli/__init__.py` & `pairtools-1.1.0/pairtools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/dedup.py` & `pairtools-1.1.0/pairtools/cli/dedup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import ast
 import pathlib
 
 from .._logging import get_logger
 
 logger = get_logger()
 
-from ..lib import fileio, pairsam_format, headerops
-from . import cli, common_io_options
-
 import click
 
+from ..lib import fileio, headerops, pairsam_format
 from ..lib.dedup import streaming_dedup, streaming_dedup_cython
 from ..lib.stats import PairCounter
+from . import cli, common_io_options
 
 UTIL_NAME = "pairtools_dedup"
 
 
 @cli.command()
 @click.argument("pairs_path", type=str, required=False)
 
@@ -101,15 +100,15 @@
     " (e.g. pairs A and B are duplicates, and B and C are duplicates, then A and C are "
     " not necessary duplicates of each other), while with scipy and sklearn it's "
     " transitive (i.e. A and C are necessarily duplicates)."
     " Cython is the original version used in pairtools since its beginning."
     " It is available for backwards compatibility and to allow specification of the"
     " column order."
     " Now the default scipy backend is generally the fastest, and with chunksize below"
-    " 1 mln has the lowest memory requirements. [dedup option]"
+    " 1 mln has the lowest memory requirements. [dedup option]",
     # " 'cython' is deprecated and provided for backwards compatibility",
 )
 
 ### Scipy and sklearn-specific options:
 @click.option(
     "--chunksize",
     type=int,
@@ -136,18 +135,19 @@
     default=1,
     help="Number of cores to use. Only applies with sklearn backend."
     "Still needs testing whether it is ever useful. [dedup option]",
 )
 
 ### Output options:
 @click.option(
-    "--mark-dups",
+    "--mark-dups/--no-mark-dups",
+    default=True,
     is_flag=True,
-    help='If specified, duplicate pairs are marked as DD in "pair_type" and '
-    "as a duplicate in the sam entries. [output format option]",
+    help='Specify if duplicate pairs should be marked as DD in "pair_type" and '
+    "as a duplicate in the sam entries. True by default. [output format option]",
 )
 @click.option(
     "--keep-parent-id",
     is_flag=True,
     help="If specified, duplicate pairs are marked with the readID of the retained"
     " deduped read in the 'parent_readID' field. [output format option]",
 )
@@ -175,53 +175,53 @@
     "--send-header-to",
     type=click.Choice(["dups", "dedup", "both", "none"]),
     default="both",
     help="Which of the outputs should receive header and comment lines. [input format option]",
 )
 @click.option(
     "--c1",
-    type=int,
-    default=pairsam_format.COL_C1,
-    help=f"Chrom 1 column; default {pairsam_format.COL_C1}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[1],
+    help=f"Chrom 1 column; default {pairsam_format.COLUMNS_PAIRS[1]}"
+    "[input format option]",
 )
 @click.option(
     "--c2",
-    type=int,
-    default=pairsam_format.COL_C2,
-    help=f"Chrom 2 column; default {pairsam_format.COL_C2}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[3],
+    help=f"Chrom 2 column; default {pairsam_format.COLUMNS_PAIRS[3]}"
+    "[input format option]",
 )
 @click.option(
     "--p1",
-    type=int,
-    default=pairsam_format.COL_P1,
-    help=f"Position 1 column; default {pairsam_format.COL_P1}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[2],
+    help=f"Position 1 column; default {pairsam_format.COLUMNS_PAIRS[2]}"
+    "[input format option]",
 )
 @click.option(
     "--p2",
-    type=int,
-    default=pairsam_format.COL_P2,
-    help=f"Position 2 column; default {pairsam_format.COL_P2}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[4],
+    help=f"Position 2 column; default {pairsam_format.COLUMNS_PAIRS[4]}"
+    "[input format option]",
 )
 @click.option(
     "--s1",
-    type=int,
-    default=pairsam_format.COL_S1,
-    help=f"Strand 1 column; default {pairsam_format.COL_S1}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[5],
+    help=f"Strand 1 column; default {pairsam_format.COLUMNS_PAIRS[5]}"
+    "[input format option]",
 )
 @click.option(
     "--s2",
-    type=int,
-    default=pairsam_format.COL_S2,
-    help=f"Strand 2 column; default {pairsam_format.COL_S2}"
-    " Only works with '--backend cython'. [input format option]",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[6],
+    help=f"Strand 2 column; default {pairsam_format.COLUMNS_PAIRS[6]}"
+    "[input format option]",
 )
 @click.option(
     "--unmapped-chrom",
     type=str,
     default=pairsam_format.UNMAPPED_CHROM,
     help="Placeholder for a chromosome on an unmapped side; default {}".format(
         pairsam_format.UNMAPPED_CHROM
@@ -482,44 +482,52 @@
 
     header, body_stream = headerops.get_header(instream)
     if not any([l.startswith("#sorted") for l in header]):
         logger.warning(
             "Pairs file appears not to be sorted, dedup might produce wrong results."
         )
     header = headerops.append_new_pg(header, ID=UTIL_NAME, PN=UTIL_NAME)
+    dups_header = header.copy()
+    if keep_parent_id and len(dups_header) > 0:
+        dups_header = headerops.append_columns(dups_header, ["parent_readID"])
+    if outstream == outstream_dups:
+        header = dups_header
     if send_header_to_dedup:
         outstream.writelines((l + "\n" for l in header))
     if send_header_to_dup and outstream_dups and (outstream_dups != outstream):
-        dups_header = header
-        if keep_parent_id and len(dups_header) > 0:
-            dups_header = headerops.append_columns(dups_header, ["parent_readID"])
         outstream_dups.writelines((l + "\n" for l in dups_header))
     if (
         outstream_unmapped
         and (outstream_unmapped != outstream)
         and (outstream_unmapped != outstream_dups)
     ):
         outstream_unmapped.writelines((l + "\n" for l in header))
 
     column_names = headerops.extract_column_names(header)
     extra_cols1 = []
     extra_cols2 = []
     if extra_col_pair is not None:
         for col1, col2 in extra_col_pair:
-            extra_cols1.append(column_names[col1] if col1.isdigit() else col1)
-            extra_cols2.append(column_names[col2] if col2.isdigit() else col2)
+            extra_cols1.append(column_names[col1] if col1.isnumeric() else col1)
+            extra_cols2.append(column_names[col2] if col2.isnumeric() else col2)
 
     if backend == "cython":
         # warnings.warn(
         #     "'cython' backend is deprecated and provided only"
         #     " for backwards compatibility",
         #     DeprecationWarning,
         # )
         extra_cols1 = [column_names.index(col) for col in extra_cols1]
         extra_cols2 = [column_names.index(col) for col in extra_cols2]
+        c1 = column_names.index(c1)
+        c2 = column_names.index(c2)
+        p1 = column_names.index(p1)
+        p2 = column_names.index(p2)
+        s1 = column_names.index(s1)
+        s2 = column_names.index(s2)
         streaming_dedup_cython(
             method,
             max_mismatch,
             sep,
             c1,
             c2,
             p1,
@@ -551,26 +559,32 @@
             unmapped_chrom=unmapped_chrom,
             outstream=outstream,
             outstream_dups=outstream_dups,
             outstream_unmapped=outstream_unmapped,
             out_stat=out_stat,
             backend=backend,
             n_proc=n_proc,
+            c1=c1,
+            c2=c2,
+            p1=p1,
+            p2=p2,
+            s1=s1,
+            s2=s2,
         )
     else:
         raise ValueError("Unknown backend")
 
     # save statistics to a file if it was requested:
     if out_stat:
         out_stat.save(
             out_stats_stream,
             yaml=kwargs.get("yaml", False),  # format as yaml
-            filter=first_filter_name
-            if not kwargs.get("yaml", False)
-            else None,  # output only the first filter if non-YAML output
+            filter=(
+                first_filter_name if not kwargs.get("yaml", False) else None
+            ),  # output only the first filter if non-YAML output
         )
 
     if bytile_dups:
         out_stat.save_bytile_dups(out_bytile_stats_stream)
 
     if instream != sys.stdin:
         instream.close()
```

### Comparing `pairtools-1.0.3/pairtools/cli/filterbycov.py` & `pairtools-1.1.0/pairtools/cli/filterbycov.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/flip.py` & `pairtools-1.1.0/pairtools/cli/flip.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/header.py` & `pairtools-1.1.0/pairtools/cli/header.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/markasdup.py` & `pairtools-1.1.0/pairtools/cli/markasdup.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/merge.py` & `pairtools-1.1.0/pairtools/cli/merge.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/parse.py` & `pairtools-1.1.0/pairtools/cli/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     ' longer than the specified value are treated as "null" alignments.'
     " These null alignments convert otherwise linear alignments into walks,"
     " and affect how they get reported as a Hi-C pair (see --walks-policy).",
 )
 @click.option(
     "--walks-policy",
     type=click.Choice(["mask", "5any", "5unique", "3any", "3unique", "all"]),
-    default="mask",
+    default="5unique",
     help="the policy for reporting unrescuable walks (reads containing more"
     " than one alignment on one or both sides, that can not be explained by a"
     " single ligation between two mappable DNA fragments)."
     ' "mask" - mask walks (chrom="!", pos=0, strand="-"); '
     ' "5any" - report the 5\'-most alignment on each side;'
     ' "5unique" - report the 5\'-most unique alignment on each side, if present;'
     ' "3any" - report the 3\'-most alignment on each side;'
```

### Comparing `pairtools-1.0.3/pairtools/cli/parse2.py` & `pairtools-1.1.0/pairtools/cli/parse2.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/phase.py` & `pairtools-1.1.0/pairtools/cli/phase.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/restrict.py` & `pairtools-1.1.0/pairtools/cli/restrict.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/sample.py` & `pairtools-1.1.0/pairtools/cli/sample.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/scaling.py` & `pairtools-1.1.0/pairtools/cli/scaling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import io
 import sys
 import click
 import pandas as pd
 
-from ..lib import fileio, pairsam_format, headerops
+from ..lib import fileio
 from . import cli, common_io_options
 
 from ..lib.scaling import compute_scaling
 
 
 UTIL_NAME = "pairtools_scaling"
 
@@ -35,42 +35,42 @@
     show_default=True,
     required=False,
     help="Number of pairs in each chunk. Reduce for lower memory footprint.",
 )
 @click.option(
     "--dist-range",
     type=click.Tuple([int, int]),
-    default=(10, 1_000_000_000),
+    default=(1, 1_000_000_000),
     show_default=True,
     required=False,
     help="Distance range. ",
 )
 @click.option(
-    "--n-dist-bins",
+    "--n-dist-bins-decade",
     type=int,
-    default=128,
+    default=8,
     show_default=True,
     required=False,
-    help="Number of distance bins to split the distance range. ",
+    help="Number of bins to split the distance range in log10-space, specified per a factor of 10 difference.",
 )
 @common_io_options
-def scaling(input_path, output, view, chunksize, dist_range, n_dist_bins, **kwargs):
+def scaling(input_path, output, view, chunksize, dist_range, n_dist_bins_decade, **kwargs):
     """Calculate pairs scalings.
 
     INPUT_PATH : by default, a .pairs/.pairsam file to calculate statistics.
     If not provided, the input is read from stdin.
 
     The files with paths ending with .gz/.lz4 are decompressed by bgzip/lz4c.
 
     Output is .tsv file with scaling stats (both cis scalings and trans levels).
     """
-    scaling_py(input_path, output, view, chunksize, dist_range, n_dist_bins, **kwargs)
+    scaling_py(input_path, output, view, chunksize, dist_range, n_dist_bins_decade, **kwargs)
 
 
-def scaling_py(input_path, output, view, chunksize, dist_range, n_dist_bins, **kwargs):
+def scaling_py(input_path, output, view, chunksize, dist_range, n_dist_bins_decade, **kwargs):
 
     if len(input_path) == 0:
         raise ValueError(f"No input paths: {input_path}")
 
     instream = fileio.auto_open(
         input_path[0],
         mode="r",
@@ -89,21 +89,21 @@
 
     # Pass the header to the instream so that it can parse the header automatically
     cis_scalings, trans_levels = compute_scaling(
         instream,
         regions=view,
         chromsizes=None,
         dist_range=dist_range,
-        n_dist_bins=n_dist_bins,
+        n_dist_bins_decade=n_dist_bins_decade,
         chunksize=chunksize,
     )
     summary_stats = pd.concat([cis_scalings, trans_levels])
 
     # save statistics to the file
-    summary_stats.to_csv(outstream, sep="\t")
+    summary_stats.to_csv(outstream, sep="\t", index=False)
 
     if instream != sys.stdin:
         instream.close()
     if outstream != sys.stdout:
         outstream.close()
```

### Comparing `pairtools-1.0.3/pairtools/cli/select.py` & `pairtools-1.1.0/pairtools/cli/select.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/sort.py` & `pairtools-1.1.0/pairtools/cli/sort.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,14 +21,58 @@
     type=str,
     default="",
     help="output pairs file."
     " If the path ends with .gz or .lz4, the output is compressed by bgzip "
     "or lz4, correspondingly. By default, the output is printed into stdout.",
 )
 @click.option(
+    "--c1",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[1],
+    help=f"Chrom 1 column; default {pairsam_format.COLUMNS_PAIRS[1]}"
+    "[input format option]",
+)
+@click.option(
+    "--c2",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[3],
+    help=f"Chrom 2 column; default {pairsam_format.COLUMNS_PAIRS[3]}"
+    "[input format option]",
+)
+@click.option(
+    "--p1",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[2],
+    help=f"Position 1 column; default {pairsam_format.COLUMNS_PAIRS[2]}"
+    "[input format option]",
+)
+@click.option(
+    "--p2",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[4],
+    help=f"Position 2 column; default {pairsam_format.COLUMNS_PAIRS[4]}"
+    "[input format option]",
+)
+@click.option(
+    "--pt",
+    type=str,
+    default=pairsam_format.COLUMNS_PAIRS[7],
+    help=f"Pair type column; default {pairsam_format.COLUMNS_PAIRS[7]}"
+    "[input format option]",
+)
+@click.option(
+    "--extra-col",
+    nargs=1,
+    type=str,
+    multiple=True,
+    help="Extra column (name or numerical index) that is also used for sorting."
+    "The option can be provided multiple times."
+    'Example: --extra-col "phase1" --extra-col "phase2". [output format option]',
+)
+@click.option(
     "--nproc",
     type=int,
     default=8,
     show_default=True,
     help="Number of processes to split the sorting work between.",
 )
 @click.option(
@@ -52,29 +96,71 @@
     help="A binary to compress temporary sorted chunks. "
     "Must decompress input when the flag -d is provided. "
     "Suggested alternatives: gzip, lzop, lz4c, snzip. "
     'If "auto", then use lz4c if available, and gzip '
     "otherwise.",
 )
 @common_io_options
-def sort(pairs_path, output, nproc, tmpdir, memory, compress_program, **kwargs):
+def sort(
+    pairs_path,
+    output,
+    c1,
+    c2,
+    p1,
+    p2,
+    pt,
+    extra_col,
+    nproc,
+    tmpdir,
+    memory,
+    compress_program,
+    **kwargs,
+):
     """Sort a .pairs/.pairsam file.
 
     Sort pairs in the lexicographic order along chrom1 and chrom2, in the
     numeric order along pos1 and pos2 and in the lexicographic order along
     pair_type.
 
     PAIRS_PATH : input .pairs/.pairsam file. If the path ends with .gz or .lz4, the
     input is decompressed by bgzip or lz4c, correspondingly. By default, the
     input is read as text from stdin.
     """
-    sort_py(pairs_path, output, nproc, tmpdir, memory, compress_program, **kwargs)
+    sort_py(
+        pairs_path,
+        output,
+        c1,
+        c2,
+        p1,
+        p2,
+        pt,
+        extra_col,
+        nproc,
+        tmpdir,
+        memory,
+        compress_program,
+        **kwargs,
+    )
 
 
-def sort_py(pairs_path, output, nproc, tmpdir, memory, compress_program, **kwargs):
+def sort_py(
+    pairs_path,
+    output,
+    c1,
+    c2,
+    p1,
+    p2,
+    pt,
+    extra_col,
+    nproc,
+    tmpdir,
+    memory,
+    compress_program,
+    **kwargs,
+):
 
     instream = fileio.auto_open(
         pairs_path,
         mode="r",
         nproc=kwargs.get("nproc_in"),
         command=kwargs.get("cmd_in", None),
     )
@@ -100,43 +186,37 @@
             warnings.warn(
                 "lz4c is not found. Using gzip for compression of sorted chunks, "
                 "which results in a minor decrease in performance. Please install "
                 "lz4c for faster sorting."
             )
             compress_program = "gzip"
 
-    command = r"""
+    column_names = headerops.extract_column_names(header)
+    columns = [c1, c2, p1, p2, pt] + list(extra_col)
+    # Now generating the "-k <i>,<i><mode>" expressions for all columns.
+    # If column name is in the default pairsam format and has an integer dtype there, do numerical sorting
+    cols = []
+    for col in columns:
+        colindex = int(col) if col.isnumeric() else column_names.index(col) + 1
+        cols.append(
+            f"-k {colindex},{colindex}{'n' if issubclass(pairsam_format.DTYPES_PAIRSAM.get(column_names[colindex-1], str), int) else ''}"
+        )
+    cols = " ".join(cols)
+    command = rf"""
         /bin/bash -c 'export LC_COLLATE=C; export LANG=C; sort 
-        -k {0},{0} -k {1},{1} -k {2},{2}n -k {3},{3}n -k {4},{4} 
+        {cols}
         --stable
-        --field-separator=$'\''{5}'\'' 
-        {6}
-        {7}
-        -S {8}
-        {9}
+        --field-separator=$'\''{pairsam_format.PAIRSAM_SEP_ESCAPE}'\''
+        --parallel={nproc}
+        {f'--temporary-directory={tmpdir}' if tmpdir else ''}
+        -S {memory}
+        {f'--compress-program={compress_program}' if compress_program else ''}'
         """.replace(
         "\n", " "
-    ).format(
-        pairsam_format.COL_C1 + 1,
-        pairsam_format.COL_C2 + 1,
-        pairsam_format.COL_P1 + 1,
-        pairsam_format.COL_P2 + 1,
-        pairsam_format.COL_PTYPE + 1,
-        pairsam_format.PAIRSAM_SEP_ESCAPE,
-        " --parallel={} ".format(nproc) if nproc > 0 else " ",
-        " --temporary-directory={} ".format(tmpdir) if tmpdir else " ",
-        memory,
-        (
-            " --compress-program={} ".format(compress_program)
-            if compress_program
-            else " "
-        ),
     )
-    command += "'"
-
     with subprocess.Popen(
         command, stdin=subprocess.PIPE, bufsize=-1, shell=True, stdout=outstream
     ) as process:
         stdin_wrapper = io.TextIOWrapper(process.stdin, "utf-8")
         for line in body_stream:
             stdin_wrapper.write(line)
         stdin_wrapper.flush()
```

### Comparing `pairtools-1.0.3/pairtools/cli/split.py` & `pairtools-1.1.0/pairtools/cli/split.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/cli/stats.py` & `pairtools-1.1.0/pairtools/cli/stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,22 @@
     is_flag=True,
     help="If specified, merge multiple input stats files instead of calculating"
     " statistics of a .pairs/.pairsam file. Merging is performed via summation of"
     " all overlapping statistics. Non-overlapping statistics are appended to"
     " the end of the file. Supported for tsv stats with single filter.",
 )
 @click.option(
+    "--n-dist-bins-decade",
+    type=int,
+    default=PairCounter.N_DIST_BINS_DECADE_DEFAULT,
+    show_default=True,
+    required=False,
+    help="Number of bins to split the distance range in log10-space, specified per a factor of 10 difference.",
+)
+@click.option(
     "--with-chromsizes/--no-chromsizes",
     is_flag=True,
     default=True,
     help="If enabled, will store sizes of chromosomes from the header of the pairs file"
     " in the stats file.",
 )
 @click.option(
@@ -103,15 +111,15 @@
     multiple=True,
     help="Cast a given column to a given type. By default, only pos and mapq "
     "are cast to int, other columns are kept as str. Provide as "
     "-t <column_name> <type>, e.g. -t read_len1 int. Multiple entries are allowed.",
 )
 @common_io_options
 def stats(
-    input_path, output, merge, bytile_dups, output_bytile_stats, filter, **kwargs
+    input_path, output, merge, n_dist_bins_decade, bytile_dups, output_bytile_stats, filter, **kwargs
 ):
     """Calculate pairs statistics.
 
     INPUT_PATH : by default, a .pairs/.pairsam file to calculate statistics.
     If not provided, the input is read from stdin.
     If --merge is specified, then INPUT_PATH is interpreted as an arbitrary number
     of stats files to merge.
@@ -119,26 +127,27 @@
     The files with paths ending with .gz/.lz4 are decompressed by bgzip/lz4c.
     """
 
     stats_py(
         input_path,
         output,
         merge,
+        n_dist_bins_decade,
         bytile_dups,
         output_bytile_stats,
         filter,
         **kwargs,
     )
 
 
 def stats_py(
-    input_path, output, merge, bytile_dups, output_bytile_stats, filter, **kwargs
+    input_path, output, merge, n_dist_bins_decade, bytile_dups, output_bytile_stats, filter, **kwargs
 ):
     if merge:
-        do_merge(output, input_path, **kwargs)
+        do_merge(output, input_path, n_dist_bins_decade=n_dist_bins_decade, **kwargs)
         return
 
     if len(input_path) == 0:
         raise ValueError(f"No input paths: {input_path}")
 
     instream = fileio.auto_open(
         input_path[0],
@@ -177,14 +186,15 @@
             )
 
         filter = dict([f.split(":", 1) for f in filter])
     else:
         filter = None
 
     stats = PairCounter(
+        n_dist_bins_decade=n_dist_bins_decade,
         bytile_dups=bytile_dups,
         filters=filter,
         startup_code=kwargs.get("startup_code", ""),  # for evaluation of filters
         type_cast=kwargs.get("type_cast", ()),  # for evaluation of filters
         engine=kwargs.get("engine", "pandas"),
     )
```

### Comparing `pairtools-1.0.3/pairtools/lib/dedup.py` & `pairtools-1.1.0/pairtools/lib/dedup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
 import pandas as pd
 
 import scipy.spatial
 from scipy.sparse import coo_matrix
 from scipy.sparse.csgraph import connected_components
+from csv import QUOTE_NONE
 
 from . import dedup_cython, pairsam_format
-from .stats import PairCounter
 
 from .._logging import get_logger
 
 logger = get_logger()
 import time
 
 # Ignore pandas future warnings:
 import warnings
-warnings.simplefilter(action='ignore', category=FutureWarning)
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
 
 # Setting for cython deduplication:
 # you don't need to load more than 10k lines at a time b/c you get out of the
 # CPU cache, so this parameter is not adjustable
 MAX_LEN = 10000
 
 
@@ -36,70 +37,98 @@
     outstream,
     outstream_dups,
     outstream_unmapped,
     keep_parent_id,
     out_stat,
     backend,
     n_proc,
+    c1="chrom1",
+    c2="chrom2",
+    p1="pos1",
+    p2="pos2",
+    s1="strand1",
+    s2="strand2",
 ):
-
     deduped_chunks = _dedup_stream(
         in_stream=in_stream,
         colnames=colnames,
         method=method,
         chunksize=chunksize,
         carryover=carryover,
         mark_dups=mark_dups,
         max_mismatch=max_mismatch,
         extra_col_pairs=extra_col_pairs,
         keep_parent_id=keep_parent_id,
         backend=backend,
         n_proc=n_proc,
+        c1=c1,
+        c2=c2,
+        p1=p1,
+        p2=p2,
+        s1=s1,
+        s2=s2,
+        unmapped_chrom=unmapped_chrom,
     )
 
     t0 = time.time()
     N = 0
 
     for df_chunk in deduped_chunks:
         N += df_chunk.shape[0]
 
         # Write the stats if requested:
         if out_stat is not None:
             out_stat.add_pairs_from_dataframe(df_chunk, unmapped_chrom=unmapped_chrom)
 
         # Define masks of unmapped and duplicated reads:
         mask_mapped = np.logical_and(
-            (df_chunk["chrom1"] != unmapped_chrom),
-            (df_chunk["chrom2"] != unmapped_chrom),
+            (df_chunk[c1] != unmapped_chrom),
+            (df_chunk[c2] != unmapped_chrom),
         )
         mask_duplicates = df_chunk["duplicate"]
 
         # Clean up dataframe:
         df_chunk = df_chunk.drop(columns=["duplicate"])
 
-        # Stream the dups:
-        if outstream_dups:
-            df_chunk.loc[mask_mapped & mask_duplicates, :].to_csv(
-                outstream_dups, index=False, header=False, sep="\t"
-            )
-
-        # Drop readID if it was created (not needed for nodup and unmapped pairs):
-        if keep_parent_id:
-            df_chunk = df_chunk.drop(columns=["parent_readID"])
+        # Save the pairs:
 
         # Stream unmapped:
         if outstream_unmapped:
             df_chunk.loc[~mask_mapped, :].to_csv(
-                outstream_unmapped, index=False, header=False, sep="\t"
+                outstream_unmapped,
+                index=False,
+                header=False,
+                sep="\t",
+                quoting=QUOTE_NONE,
             )
 
-        # Stream unique pairs:
-        df_chunk.loc[mask_mapped & (~mask_duplicates), :].to_csv(
-            outstream, index=False, header=False, sep="\t"
-        )
+        # If outstream_dups is the same as outstream, we save the mapped pairs to the same file
+        if outstream_dups == outstream:
+            df_chunk.loc[mask_mapped, :].to_csv(
+                outstream, index=False, header=False, sep="\t", quoting=QUOTE_NONE
+            )
+        else:
+            # Save the dups:
+            if outstream_dups:
+                df_chunk.loc[mask_duplicates, :].to_csv(
+                    outstream_dups,
+                    index=False,
+                    header=False,
+                    sep="\t",
+                    quoting=QUOTE_NONE,
+                )
+            # Drop readID if it was created (not needed for nodup and unmapped pairs):
+            if keep_parent_id:
+                df_chunk = df_chunk.drop(columns=["parent_readID"])
+
+            # Save unique:
+            if outstream:
+                df_chunk.loc[mask_mapped & (~mask_duplicates), :].to_csv(
+                    outstream, index=False, header=False, sep="\t", quoting=QUOTE_NONE
+                )
 
     t1 = time.time()
     t = t1 - t0
     logger.debug(f"total time: {t}")
     if N > 0:
         logger.debug(f"time per mln pairs: {t/N*1e6}")
     else:
@@ -114,61 +143,240 @@
     carryover,
     mark_dups,
     max_mismatch,
     extra_col_pairs,
     keep_parent_id,
     backend,
     n_proc,
+    c1,
+    c2,
+    p1,
+    p2,
+    s1,
+    s2,
+    unmapped_chrom,
 ):
     # Stream the input dataframe:
     dfs = pd.read_table(
-        in_stream, comment=None, names=colnames, chunksize=chunksize
+        in_stream,
+        comment=None,
+        names=colnames,
+        chunksize=chunksize,
+        dtype=pairsam_format.DTYPES_PAIRSAM,
+        sep="\t",
     )
 
     # Set up the carryover dataframe:
     df_prev_nodups = pd.DataFrame([])
     prev_i = 0
 
     # Iterate over chunks:
     for df in dfs:
+        df["carryover"] = False
+        input_chunk = pd.concat(
+            [df_prev_nodups, df], axis=0, ignore_index=True
+        ).reset_index(drop=True)
         df_marked = _dedup_chunk(
-            pd.concat([df_prev_nodups, df], axis=0, ignore_index=True).reset_index(
-                drop=True
-            ),
+            input_chunk,
             r=max_mismatch,
             method=method,
             keep_parent_id=keep_parent_id,
             extra_col_pairs=extra_col_pairs,
             backend=backend,
             n_proc=n_proc,
+            c1=c1,
+            c2=c2,
+            p1=p1,
+            p2=p2,
+            s1=s1,
+            s2=s2,
+            unmapped_chrom=unmapped_chrom,
         )
-        df_marked = df_marked.loc[prev_i:, :].reset_index(drop=True)
+
+        df_marked = (
+            df_marked[~df_marked["carryover"]]
+            .drop(columns=["carryover"])
+            .reset_index(drop=True)
+        )
+
         mask_duplicated = df_marked["duplicate"]
         if mark_dups:
             df_marked.loc[mask_duplicated, "pair_type"] = "DD"
 
+        yield df_marked
+
         # Filter out duplicates and store specific columns:
         df_nodups = df_marked.loc[~mask_duplicated, colnames]
 
         # Re-define carryover pairs:
         df_prev_nodups = df_nodups.tail(carryover).reset_index(drop=True)
+        df_prev_nodups["carryover"] = True
         prev_i = len(df_prev_nodups)
 
-        yield df_marked
+
+def _make_adj_mat(arr, size, r, method, n_proc=None, backend=None):
+    if method not in ("max", "sum"):
+        raise ValueError('Unknown method, only "sum" or "max" allowed')
+
+    if method == "sum":
+        p = 1
+    else:
+        p = np.inf
+
+    if backend == "sklearn":
+        from sklearn import neighbors
+
+        a_mat = neighbors.radius_neighbors_graph(
+            arr,
+            radius=r,
+            p=p,
+            n_jobs=n_proc,
+        )
+        return a_mat
+
+    elif backend == "scipy":
+        import scipy.spatial
+        from scipy.sparse import coo_matrix
+
+        z = scipy.spatial.KDTree(
+            arr,
+        )
+        a = z.query_pairs(r=r, p=p, output_type="ndarray")
+        a0 = a[:, 0]
+        a1 = a[:, 1]
+        a_mat = coo_matrix((np.ones_like(a0), (a0, a1)), shape=(size, size))
+        return a_mat
+
+    else:
+        raise ValueError('Unknown backend, only "scipy" or "sklearn" allowed')
+
+
+def _cluster_pairs(
+    df_mapped,
+    cols,
+    p1,
+    p2,
+    r,
+    method,
+    n_proc,
+    backend,
+):
+    groups = (
+        df_mapped[cols]
+        .drop_duplicates()
+        .reset_index(drop=True)
+        .reset_index()
+        .rename(columns={"index": "group"})
+    )
+
+    df_mapped = df_mapped.merge(groups, how="left", on=list(cols))
+
+    components = []
+    maxcluster_id = 0
+
+    for name, group in df_mapped.groupby("group"):
+        a_mat = _make_adj_mat(
+            group[[p1, p2]],
+            size=group.shape[0],
+            r=r,
+            method=method,
+            n_proc=n_proc,
+            backend=backend,
+        )
+        comp = connected_components(a_mat, directed=False)[1] + maxcluster_id + 1
+        components.append(
+            pd.Series(
+                name="cluster_id",
+                index=group.index,
+                data=comp,
+            )
+        )
+        maxcluster_id = components[-1].max()
+
+    df_mapped["cluster_id"] = pd.concat(components)
+    df_mapped.drop(columns=["group"], inplace=True)
+
+    return df_mapped
+
+
+def _cluster_pairs_nonmatching_col_pairs(
+    df_mapped,
+    col_pairs,
+    p1,
+    p2,
+    r,
+    method,
+    n_proc,
+    backend,
+):
+    groups_left = (
+        df_mapped[col_pairs[:, 0]]
+        .drop_duplicates()
+        .reset_index(drop=True)
+        .reset_index()
+        .rename(columns={"index": "group"})
+    )
+
+    df_mapped = df_mapped.merge(groups_left, how="left", on=list(col_pairs[:, 0]))
+
+    groups_right = (
+        df_mapped[col_pairs[:, 1]]
+        .drop_duplicates()
+        .reset_index(drop=True)
+        .reset_index()
+        .rename(columns={"index": "group"})
+    )
+
+    df_mapped = df_mapped.merge(
+        groups_right, on=list(col_pairs[:, 1]), suffixes=["_left", "_right"]
+    )
+
+    components = []
+    maxcluster_id = 0
+
+    for name, group in df_mapped.groupby("group_left"):
+        group = group[group["group_right"] == name]
+        a_mat = _make_adj_mat(
+            group[[p1, p2]],
+            size=group.shape[0],
+            r=r,
+            method=method,
+            n_proc=n_proc,
+            backend=backend,
+        )
+        components.append(
+            pd.Series(
+                name="cluster_id",
+                index=group.index,
+                data=connected_components(a_mat, directed=False)[1] + maxcluster_id,
+            )
+        )
+        maxcluster_id = components[-1].max()
+
+    df_mapped["cluster_id"] = pd.concat(components)
+    df_mapped.drop(columns=["group_left", "group_right"], inplace=True)
+
+    return df_mapped
 
 
 def _dedup_chunk(
     df,
     r,
     method,
     keep_parent_id,
     extra_col_pairs,
     backend,
-    unmapped_chrom="!",
-    n_proc=1,
+    n_proc,
+    c1,
+    c2,
+    p1,
+    p2,
+    s1,
+    s2,
+    unmapped_chrom,
 ):
     """Mark duplicates in a dataframe of pairs
 
     Parameters
     ----------
     df : pd.DataFrame
         Dataframe with pairs, has to contain columns 'chrom1', 'pos1', 'chrom2', 'pos2'
@@ -197,96 +405,84 @@
     Returns
     -------
     pd.DataFrame
         Dataframe with marked duplicates (extra boolean field 'duplicate'), and
         optionally recorded 'parent_readID'
 
     """
-    if method not in ("max", "sum"):
-        raise ValueError('Unknown method, only "sum" or "max" allowed')
-    if backend == "sklearn":
-        from sklearn import neighbors
-
-    if method == "sum":
-        p = 1
-    else:
-        p = np.inf
 
     # Store the index of the dataframe:
     index_colname = df.index.name
     if index_colname is None:
         index_colname = "index"
     df = df.reset_index()  # Remove the index temporarily
 
     # Set up columns to store the dedup info:
-    df.loc[:, "clusterid"] = np.nan
-    df.loc[:, "duplicate"] = False
+    df["cluster_id"] = -1
+    df["duplicate"] = False
 
     # Split mapped and unmapped reads:
-    mask_unmapped = (df["chrom1"] == unmapped_chrom) | (df["chrom2"] == unmapped_chrom)
+    mask_unmapped = (df[c1] == unmapped_chrom) | (df[c2] == unmapped_chrom)
     df_unmapped = df.loc[mask_unmapped, :].copy()
     df_mapped = df.loc[~mask_unmapped, :].copy()
     N_mapped = df_mapped.shape[0]
 
     # If there are some mapped reads, dedup them:
     if N_mapped > 0:
-        if backend == "sklearn":
-            a = neighbors.radius_neighbors_graph(
-                df_mapped[["pos1", "pos2"]],
-                radius=r,
-                p=p,
-                n_jobs=n_proc,
-            )
-            a0, a1 = a.nonzero()
-        elif backend == "scipy":
-            z = scipy.spatial.cKDTree(df_mapped[["pos1", "pos2"]])
-            a = z.query_pairs(r=r, p=p, output_type="ndarray")
-            a0 = a[:, 0]
-            a1 = a[:, 1]
-        need_to_match = np.array(
+        col_pairs = np.array(
             [
-                ("chrom1", "chrom1"),
-                ("chrom2", "chrom2"),
-                ("strand1", "strand1"),
-                ("strand2", "strand2"),
+                (c1, c1),
+                (c2, c2),
+                (s1, s1),
+                (s2, s2),
             ]
             + extra_col_pairs
         )
-        nonpos_matches = np.all(
-            [
-                df_mapped.iloc[a0, df_mapped.columns.get_loc(lc)].values
-                == df_mapped.iloc[a1, df_mapped.columns.get_loc(rc)].values
-                for (lc, rc) in need_to_match
-            ],
-            axis=0,
-        )
-        a0 = a0[nonpos_matches]
-        a1 = a1[nonpos_matches]
-        a_mat = coo_matrix((np.ones_like(a0), (a0, a1)), shape=(N_mapped, N_mapped))
 
-        # Set up inferred clusterIDs:
-        df_mapped.loc[:, "clusterid"] = connected_components(a_mat, directed=False)[1]
+        if (col_pairs[:, 0] == col_pairs[:, 1]).all():
+            df_mapped = _cluster_pairs(
+                df_mapped,
+                col_pairs[:, 0],
+                p1,
+                p2,
+                r,
+                method,
+                n_proc,
+                backend,
+            )
+
+        else:
+            df_mapped = _cluster_pairs_nonmatching_col_pairs(
+                df_mapped,
+                col_pairs,
+                p1,
+                p2,
+                r,
+                method,
+                n_proc,
+                backend,
+            )
 
-    mask_dups = df_mapped["clusterid"].duplicated()
+    mask_dups = df_mapped["cluster_id"].duplicated()
     df_mapped.loc[mask_dups, "duplicate"] = True
 
     # Mark parent IDs if requested:
     if keep_parent_id:
-        df_mapped.loc[:, "parent_readID"] = df_mapped["clusterid"].map(
-            df_mapped[~mask_dups].set_index("clusterid")["readID"]
+        df_mapped.loc[:, "parent_readID"] = df_mapped["cluster_id"].map(
+            df_mapped[~mask_dups].set_index("cluster_id")["readID"]
         )
-        df_unmapped.loc[:, "parent_readID"] = ""
+        df_unmapped["parent_readID"] = ""
 
-    # Reconstruct original dataframe with removed duplicated reads:
+    # Reconstruct original dataframe with removed duplicated reads
+    # (here, we rely on the sorting order that puts unmapped reads first):
     df = pd.concat([df_unmapped, df_mapped]).reset_index(drop=True)
     df = df.set_index(index_colname)  # Set up the original index
     df = df.drop(
-        ["clusterid"], axis=1
+        ["cluster_id"], axis=1
     )  # Remove the information that we don't need anymore:
-
     return df
 
 
 ### Cython deduplication ####
 def streaming_dedup_cython(
     method,
     max_mismatch,
@@ -372,15 +568,15 @@
     t0 = time.time()
     N = 0
 
     instream = iter(instream)
     read_idx = 0  # read index to mark the parent readID
     while True:
         rawline = next(instream, None)
-        stripline = rawline.strip('\n') if rawline else None
+        stripline = rawline.strip("\n") if rawline else None
 
         # take care of empty lines not at the end of the file separately
         if rawline and (not stripline):
             logger.warning("Empty line detected not at the end of the file")
             continue
 
         if stripline:
@@ -388,15 +584,14 @@
             if len(cols) <= maxind:
                 raise ValueError(
                     "Error parsing line {}: ".format(stripline)
                     + " expected {} columns, got {}".format(maxind, len(cols))
                 )
 
             if (cols[c1ind] == unmapped_chrom) or (cols[c2ind] == unmapped_chrom):
-
                 if outstream_unmapped:
                     outstream_unmapped.write(stripline)
                     # don't forget terminal newline
                     outstream_unmapped.write("\n")
 
                 # add a pair to PairCounter if stats output is requested:
                 if out_stat:
@@ -404,14 +599,15 @@
                         cols[c1ind],
                         int(cols[p1ind]),
                         cols[s1ind],
                         cols[c2ind],
                         int(cols[p2ind]),
                         cols[s2ind],
                         cols[ptind],
+                        unmapped_chrom=unmapped_chrom,
                     )
             else:
                 line_buffer.append(stripline)
                 cols_buffer.append(cols)
 
                 c1.append(fetchadd(cols[c1ind], chromDict))
                 c2.append(fetchadd(cols[c2ind], chromDict))
@@ -473,26 +669,28 @@
                             cols_buffer[i][c1ind],
                             int(cols_buffer[i][p1ind]),
                             cols_buffer[i][s1ind],
                             cols_buffer[i][c2ind],
                             int(cols_buffer[i][p2ind]),
                             cols_buffer[i][s2ind],
                             cols_buffer[i][ptind],
+                            unmapped_chrom=unmapped_chrom,
                         )
                 # duplicated pair:
                 else:
                     if out_stat:
                         out_stat.add_pair(
                             cols_buffer[i][c1ind],
                             int(cols_buffer[i][p1ind]),
                             cols_buffer[i][s1ind],
                             cols_buffer[i][c2ind],
                             int(cols_buffer[i][p2ind]),
                             cols_buffer[i][s2ind],
                             "DD",
+                            unmapped_chrom=unmapped_chrom,
                         )
                     if outstream_dups:
                         if mark_dups:  # DD-marked pair:
                             output = sep.join(mark_split_pair_as_dup(cols_buffer[i]))
                         else:  # pair as is:
                             output = line_buffer[i]
 
@@ -554,15 +752,14 @@
     # should as well.
     original_has_newline = cols[-1].endswith("\n")
 
     cols[pairsam_format.COL_PTYPE] = "DD"
 
     if (len(cols) > pairsam_format.COL_SAM1) and (len(cols) > pairsam_format.COL_SAM2):
         for i in (pairsam_format.COL_SAM1, pairsam_format.COL_SAM2):
-
             # split each sam column into sam entries, tag and assemble back
             cols[i] = pairsam_format.INTER_SAM_SEP.join(
                 [
                     mark_sam_as_dup(sam)
                     for sam in cols[i].split(pairsam_format.INTER_SAM_SEP)
                 ]
             )
```

### Comparing `pairtools-1.0.3/pairtools/lib/dedup_cython.pyx` & `pairtools-1.1.0/pairtools/lib/dedup_cython.pyx`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/fileio.py` & `pairtools-1.1.0/pairtools/lib/fileio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import shutil
 import pipes
 import subprocess
 import sys
 
-
 class ParseError(Exception):
     pass
 
 
 def auto_open(path, mode, nproc=1, command=None):
     """Guess the file format from the extension and use the corresponding binary
     to open it for reading or writing. If the extension is not known, open the
@@ -231,7 +230,36 @@
         self.write = self._stream.write
         self.writelines = self._stream.writelines
 
     def close(self, timeout=None):
         self._stream.close()
         retcode = self._proc.wait(timeout=timeout)
         return retcode
+
+
+def get_stream_handlers(instream):
+    """
+    Get the readline and peek functions for the provided input stream.
+
+    Parameters:
+        instream (file-like object): The input stream to get the handlers for.
+
+    Returns:
+        tuple: A tuple containing the following elements:
+            - readline_f (function): The readline function for the input stream.
+            - peek_f (function): The peek function for the input stream.
+
+    Raises:
+        ValueError: If the peek function cannot be found for the provided stream.
+    """
+    readline_f, peek_f = None, None
+    if hasattr(instream, "buffer"):
+        peek_f = instream.buffer.peek
+        readline_f = instream.buffer.readline
+    elif hasattr(instream, "peek"):
+        peek_f = instream.peek
+        readline_f = instream.readline
+    else:
+        raise ValueError("Cannot find the peek() function of the provided stream!")
+    return readline_f, peek_f
+
+
```

### Comparing `pairtools-1.0.3/pairtools/lib/filterbycov.py` & `pairtools-1.1.0/pairtools/lib/filterbycov.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/headerops.py` & `pairtools-1.1.0/pairtools/lib/headerops.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,26 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from .. import __version__
 from . import pairsam_format
-from .fileio import ParseError
+from .fileio import ParseError, get_stream_handlers
 
 from .._logging import get_logger
 
 logger = get_logger()
 
 PAIRS_FORMAT_VERSION = "1.0.0"
 SEP_COLS = " "
 SEP_CHROMS = " "
 COMMENT_CHAR = "#"
 
 
-def get_stream_handlers(instream):
-    # get peekable buffer for the instream
-    readline_f, peek_f = None, None
-    if hasattr(instream, "buffer"):
-        peek_f = instream.buffer.peek
-        readline_f = instream.buffer.readline
-    elif hasattr(instream, "peek"):
-        peek_f = instream.peek
-        readline_f = instream.readline
-    else:
-        raise ValueError("Cannot find the peek() function of the provided stream!")
-    return readline_f, peek_f
-
 
 def get_header(instream, comment_char=COMMENT_CHAR, ignore_warning=False):
     """Returns a header from the stream and an the reaminder of the stream
     with the actual data.
     Parameters
     ----------
     instream : a file object
```

### Comparing `pairtools-1.0.3/pairtools/lib/parse.py` & `pairtools-1.1.0/pairtools/lib/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,43 @@
         Additionally, these functions also output all alignments for each side.
 
 """
 from . import pairsam_format
 from .parse_pysam import get_mismatches_c
 
 
+def group_alignments_by_side(sams):
+    return [sam for sam in sams if sam.is_read1], [sam for sam in sams if sam.is_read2]
+
+
+def read_alignment_block(instream, sort=True, group_by_side=True, return_readID=True):
+    sams = []
+
+    prev_readID = None
+    while True:
+        sam_entry = next(instream, None)
+        readID = sam_entry.query_name if sam_entry else None
+
+        # Read is fully populated, then parse and write:
+        if not (sam_entry) or ((readID != prev_readID) and prev_readID):
+            if sort:
+                sams = sorted(sams, key=lambda a: (a.is_read2, a.query_alignment_start))
+            out = sams if not group_by_side else group_alignments_by_side(sams)
+            out = out if not return_readID else (prev_readID, out)
+            yield out
+            
+            sams.clear()
+            
+        if sam_entry is None:
+            break
+        else:
+            sams.append(sam_entry)
+            prev_readID = readID
+
+
 def streaming_classify(
     instream, outstream, chromosomes, out_alignments_stream, out_stat, **kwargs
 ):
     """
     Parse input sam file into individual reads, pairs, walks,
     then write to the outstream(s).
 
@@ -89,126 +118,102 @@
     store_seq = "seq" in add_columns
 
     ### Compile readID transformation:
     readID_transform = kwargs.get("readid_transform", None)
     if readID_transform is not None:
         readID_transform = compile(readID_transform, "<string>", "eval")
 
-    ### Prepare for iterative parsing of the input stream
-    # Each read is represented by readID, sams1 (left alignments) and sams2 (right alignments)
-    readID = ""  # Read id of the current read
-    sams1 = []  # Placeholder for the left alignments
-    sams2 = []  # Placeholder for the right alignments
-    # Each read is comprised of multiple alignments, or sam entries:
-    sam_entry = ""  # Placeholder for each aligned segment
-    # Keep the id of the previous sam entry to detect when the read is completely populated:
-    prev_readID = ""  # Placeholder for the read id
-
     ### Iterate over input pysam:
     instream = iter(instream)
-    while sam_entry is not None:
-        sam_entry = next(instream, None)
-
-        readID = sam_entry.query_name if sam_entry else None
-        if readID_transform is not None and readID is not None:
+    for (readID, (sams1, sams2)) in read_alignment_block(instream, sort=True, group_by_side=True, return_readID=True):
+        if readID_transform is not None:
             readID = eval(readID_transform)
 
-        # Read is fully populated, then parse and write:
-        if not (sam_entry) or ((readID != prev_readID) and prev_readID):
+        ### Parse
+        if not parse2:  # regular parser:
+            pairstream, all_algns1, all_algns2 = parse_read(
+                sams1,
+                sams2,
+                min_mapq=kwargs["min_mapq"],
+                max_molecule_size=kwargs["max_molecule_size"],
+                max_inter_align_gap=kwargs["max_inter_align_gap"],
+                walks_policy=kwargs["walks_policy"],
+                sam_tags=sam_tags,
+                store_seq=store_seq,
+                report_mismatches=True if "mismatches" in add_columns else False,
+            )
+        else:  # parse2 parser:
+            pairstream, all_algns1, all_algns2 = parse2_read(
+                sams1,
+                sams2,
+                min_mapq=kwargs["min_mapq"],
+                max_inter_align_gap=kwargs["max_inter_align_gap"],
+                max_insert_size=kwargs.get("max_insert_size", 500),
+                single_end=kwargs["single_end"],
+                report_position=kwargs["report_position"],
+                report_orientation=kwargs["report_orientation"],
+                sam_tags=sam_tags,
+                dedup_max_mismatch=kwargs["dedup_max_mismatch"],
+                store_seq=store_seq,
+                expand=kwargs["expand"],
+                max_expansion_depth=kwargs["max_expansion_depth"],
+                report_mismatches=True if "mismatches" in add_columns else False,
+            )
 
-            ### Parse
-            if not parse2:  # regular parser:
-                pairstream, all_algns1, all_algns2 = parse_read(
-                    sams1,
-                    sams2,
-                    min_mapq=kwargs["min_mapq"],
-                    max_molecule_size=kwargs["max_molecule_size"],
-                    max_inter_align_gap=kwargs["max_inter_align_gap"],
-                    walks_policy=kwargs["walks_policy"],
-                    sam_tags=sam_tags,
-                    store_seq=store_seq,
-                    report_mismatches=True if "mismatches" in add_columns else False,
-                )
-            else:  # parse2 parser:
-                pairstream, all_algns1, all_algns2 = parse2_read(
-                    sams1,
-                    sams2,
-                    min_mapq=kwargs["min_mapq"],
-                    max_inter_align_gap=kwargs["max_inter_align_gap"],
-                    max_insert_size=kwargs.get("max_insert_size", 500),
-                    single_end=kwargs["single_end"],
-                    report_position=kwargs["report_position"],
-                    report_orientation=kwargs["report_orientation"],
-                    sam_tags=sam_tags,
-                    dedup_max_mismatch=kwargs["dedup_max_mismatch"],
-                    store_seq=store_seq,
-                    expand=kwargs["expand"],
-                    max_expansion_depth=kwargs["max_expansion_depth"],
-                    report_mismatches=True if "mismatches" in add_columns else False,
-                )
+        ### Write:
+        read_has_alignments = False
+        for (algn1, algn2, pair_index) in pairstream:
+            read_has_alignments = True
+
+            # Alignment end defaults to 5' if report_alignment_end is unspecified:
+            if kwargs.get("report_alignment_end", "5") == "5":
+                algn1["pos"] = algn1["pos5"]
+                algn2["pos"] = algn2["pos5"]
+            else:
+                algn1["pos"] = algn1["pos3"]
+                algn2["pos"] = algn2["pos3"]
 
-            ### Write:
-            read_has_alignments = False
-            for (algn1, algn2, pair_index) in pairstream:
-                read_has_alignments = True
-
-                # Alignment end defaults to 5' if report_alignment_end is unspecified:
-                if kwargs.get("report_alignment_end", "5") == "5":
-                    algn1["pos"] = algn1["pos5"]
-                    algn2["pos"] = algn2["pos5"]
-                else:
-                    algn1["pos"] = algn1["pos3"]
-                    algn2["pos"] = algn2["pos3"]
-
-                if kwargs["flip"]:
-                    flip_pair = not check_pair_order(algn1, algn2, chrom_enum)
-                    if flip_pair:
-                        algn1, algn2 = algn2, algn1
-                        sams1, sams2 = sams2, sams1
-
-                write_pairsam(
-                    algn1,
-                    algn2,
-                    readID=prev_readID,
-                    pair_index=pair_index,
-                    sams1=sams1,
-                    sams2=sams2,
-                    out_file=outstream,
-                    drop_readid=kwargs["drop_readid"],
-                    drop_seq=kwargs["drop_seq"],
-                    drop_sam=kwargs["drop_sam"],
-                    add_pair_index=kwargs["add_pair_index"],
-                    add_columns=add_columns,
-                )
+            if kwargs["flip"]:
+                flip_pair = not check_pair_order(algn1, algn2, chrom_enum)
+                if flip_pair:
+                    algn1, algn2 = algn2, algn1
+                    sams1, sams2 = sams2, sams1
+
+            write_pairsam(
+                algn1,
+                algn2,
+                readID=readID,
+                pair_index=pair_index,
+                sams1=sams1,
+                sams2=sams2,
+                out_file=outstream,
+                drop_readid=kwargs["drop_readid"],
+                drop_seq=kwargs["drop_seq"],
+                drop_sam=kwargs["drop_sam"],
+                add_pair_index=kwargs["add_pair_index"],
+                add_columns=add_columns,
+            )
 
-                # add a pair to PairCounter for stats output:
-                if out_stat:
-                    out_stat.add_pair(
-                        algn1["chrom"],
-                        int(algn1["pos"]),
-                        algn1["strand"],
-                        algn2["chrom"],
-                        int(algn2["pos"]),
-                        algn2["strand"],
-                        algn1["type"] + algn2["type"],
-                    )
-
-            # write all alignments:
-            if out_alignments_stream and read_has_alignments:
-                write_all_algnments(
-                    prev_readID, all_algns1, all_algns2, out_alignments_stream
+            # add a pair to PairCounter for stats output:
+            if out_stat:
+                out_stat.add_pair(
+                    algn1["chrom"],
+                    int(algn1["pos"]),
+                    algn1["strand"],
+                    algn2["chrom"],
+                    int(algn2["pos"]),
+                    algn2["strand"],
+                    algn1["type"] + algn2["type"],
                 )
 
-            # Empty read after writing:
-            sams1.clear()
-            sams2.clear()
-
-        if sam_entry is not None:
-            push_pysam(sam_entry, sams1, sams2)
-            prev_readID = readID
+        # write all alignments:
+        if out_alignments_stream and read_has_alignments:
+            write_all_algnments(
+                readID, all_algns1, all_algns2, out_alignments_stream
+            )
 
 
 ############################
 ### Alignment utilities: ###
 ############################
 
 
@@ -405,14 +410,74 @@
     :return:
     """
     hic_algn = dict(hic_algn)  # overwrite the variable with the copy of dictionary
     hic_algn["pos5"], hic_algn["pos3"] = hic_algn["pos3"], hic_algn["pos5"]
     return hic_algn
 
 
+
+def _convert_gaps_into_alignments(sorted_algns, max_inter_align_gap):
+    """
+    Inplace conversion of gaps longer than max_inter_align_gap into alignments
+    """
+    if (len(sorted_algns) == 1) and (not sorted_algns[0]["is_mapped"]):
+        return
+
+    last_5_pos = 0
+    for i in range(len(sorted_algns)):
+        algn = sorted_algns[i]
+        if algn["dist_to_5"] - last_5_pos > max_inter_align_gap:
+            new_algn = empty_alignment()
+            new_algn["dist_to_5"] = last_5_pos
+            new_algn["algn_read_span"] = algn["dist_to_5"] - last_5_pos
+            new_algn["read_len"] = algn["read_len"]
+            new_algn["dist_to_3"] = new_algn["read_len"] - algn["dist_to_5"]
+
+            last_5_pos = algn["dist_to_5"] + algn["algn_read_span"]
+
+            sorted_algns.insert(i, new_algn)
+            i += 2
+        else:
+            last_5_pos = max(last_5_pos, algn["dist_to_5"] + algn["algn_read_span"])
+            i += 1
+
+
+def normalize_alignment_list(algns, side, sort_by="dist_to_5", max_inter_align_gap=None):
+    """
+    Normalize the alignment list: insert empty alignments in gaps between alignments, 
+    sort by distance to the 5' end, add read side, alignment index.
+
+    Args:
+        algns (list): The list of alignments.
+        side (str): The side of the alignment.
+        sort_by (str, optional): The key to sort the alignments by. Defaults to "dist_to_5".
+        max_inter_align_gap (int, optional): The maximum allowed gap between alignments. Defaults to None.
+
+    Returns:
+        list: The normalized alignment list.
+
+    """
+    if len(algns) == 0:
+        algns = [empty_alignment()]
+
+    if sort_by:
+        algns = sorted(algns, key=lambda algn: algn[sort_by])
+
+    if max_inter_align_gap is not None:
+        _convert_gaps_into_alignments(algns, max_inter_align_gap)
+
+    for i, algn in enumerate(algns):
+        algn["read_side"] = side
+        algn["algn_idx"] = i
+        algn["same_side_algn_count"] = len(algns)
+
+    return algns
+            
+
+
 ####################
 ### Parsing utilities:
 ####################
 
 
 def parse_read(
     sams1,
@@ -466,26 +531,17 @@
     algns2 = [
         parse_pysam_entry(
             sam, min_mapq, sam_tags, store_seq, report_mismatches=report_mismatches
         )
         for sam in sams2
     ]
 
-    if len(algns1) > 0:
-        algns1 = sorted(algns1, key=lambda algn: algn["dist_to_5"])
-    else:
-        algns1 = [empty_alignment()]  # Empty alignment dummy
-    if len(algns2) > 0:
-        algns2 = sorted(algns2, key=lambda algn: algn["dist_to_5"])
-    else:
-        algns2 = [empty_alignment()]  # Empty alignment dummy
+    algns1 = normalize_alignment_list(algns1, 1, sort_by="dist_to_5", max_inter_align_gap=max_inter_align_gap)
+    algns2 = normalize_alignment_list(algns2, 2, sort_by="dist_to_5", max_inter_align_gap=max_inter_align_gap)
 
-    if max_inter_align_gap is not None:
-        _convert_gaps_into_alignments(algns1, max_inter_align_gap)
-        _convert_gaps_into_alignments(algns2, max_inter_align_gap)
 
     # By default, assume each molecule is a single pair with single unconfirmed pair:
     hic_algn1 = algns1[0]
     hic_algn2 = algns2[0]
     pair_index = (1, "R1-2")
 
     # Define the type of alignment on each side:
@@ -555,22 +611,22 @@
 
                     hic_algn2 = algns2[-1]
                     for algn in algns2[::-1]:
                         if algn["is_mapped"] and algn["is_unique"]:
                             hic_algn2 = algn
                             break
 
-                # lower-case reported walks on the chimeric side
+                # DEPRECATED: lower-case reported walks on the chimeric side
                 if walks_policy != "mask":
                     if is_chimeric_1:
                         hic_algn1 = dict(hic_algn1)
-                        hic_algn1["type"] = hic_algn1["type"].lower()
+                        # hic_algn1["type"] = hic_algn1["type"].lower()
                     if is_chimeric_2:
                         hic_algn2 = dict(hic_algn2)
-                        hic_algn2["type"] = hic_algn2["type"].lower()
+                        # hic_algn2["type"] = hic_algn2["type"].lower()
 
         else:
             raise ValueError(f"Walks policy {walks_policy} is not supported.")
 
     return iter([(hic_algn1, hic_algn2, pair_index)]), algns1, algns2
 
 
@@ -610,18 +666,16 @@
         # Generate a sorted, gap-filled list of all alignments
         algns1 = [
             parse_pysam_entry(
                 sam, min_mapq, sam_tags, store_seq, report_mismatches=report_mismatches
             )
             for sam in sams2  # note sams2, that's how these reads are typically parsed
         ]
-        algns1 = sorted(algns1, key=lambda algn: algn["dist_to_5"])
-        if max_inter_align_gap is not None:
-            _convert_gaps_into_alignments(algns1, max_inter_align_gap)
-
+        
+        algns1 = normalize_alignment_list(algns1, 1, sort_by="dist_to_5", max_inter_align_gap=max_inter_align_gap)
         algns2 = [empty_alignment()]  # Empty alignment dummy
 
         if len(algns1) > 1:
             # Look for ligation pair, and report linear alignments after deduplication of complex walks:
             # (Note that coordinate system for single-end reads does not change the behavior)
             output = parse_complex_walk(
                 algns1,
@@ -669,28 +723,16 @@
         algns2 = [
             parse_pysam_entry(
                 sam, min_mapq, sam_tags, store_seq, report_mismatches=report_mismatches
             )
             for sam in sams2
         ]
 
-        # Sort alignments by the distance to the 5'-end:
-        if len(algns1) > 0:
-            algns1 = sorted(algns1, key=lambda algn: algn["dist_to_5"])
-        else:
-            algns1 = [empty_alignment()]  # Empty alignment dummy
-        if len(algns2) > 0:
-            algns2 = sorted(algns2, key=lambda algn: algn["dist_to_5"])
-        else:
-            algns2 = [empty_alignment()]  # Empty alignment dummy
-
-        # Convert alignment gaps to alignments:
-        if max_inter_align_gap is not None:
-            _convert_gaps_into_alignments(algns1, max_inter_align_gap)
-            _convert_gaps_into_alignments(algns2, max_inter_align_gap)
+        algns1 = normalize_alignment_list(algns1, 1, sort_by="dist_to_5", max_inter_align_gap=max_inter_align_gap)
+        algns2 = normalize_alignment_list(algns2, 2, sort_by="dist_to_5", max_inter_align_gap=max_inter_align_gap)
 
         is_chimeric_1 = len(algns1) > 1
         is_chimeric_2 = len(algns2) > 1
 
         if is_chimeric_1 or is_chimeric_2:
             # If at least one side is chimera, we must look for ligation pair, and
             # report linear alignments after deduplication of complex walks:
@@ -820,40 +862,14 @@
             algns1[0]["type"] = "R"
             algns2[1]["type"] = "X"
             return 2
     else:
         return None
 
 
-def _convert_gaps_into_alignments(sorted_algns, max_inter_align_gap):
-    """
-    Inplace conversion of gaps longer than max_inter_align_gap into alignments
-    """
-    if (len(sorted_algns) == 1) and (not sorted_algns[0]["is_mapped"]):
-        return
-
-    last_5_pos = 0
-    for i in range(len(sorted_algns)):
-        algn = sorted_algns[i]
-        if algn["dist_to_5"] - last_5_pos > max_inter_align_gap:
-            new_algn = empty_alignment()
-            new_algn["dist_to_5"] = last_5_pos
-            new_algn["algn_read_span"] = algn["dist_to_5"] - last_5_pos
-            new_algn["read_len"] = algn["read_len"]
-            new_algn["dist_to_3"] = new_algn["read_len"] - algn["dist_to_5"]
-
-            last_5_pos = algn["dist_to_5"] + algn["algn_read_span"]
-
-            sorted_algns.insert(i, new_algn)
-            i += 2
-        else:
-            last_5_pos = max(last_5_pos, algn["dist_to_5"] + algn["algn_read_span"])
-            i += 1
-
-
 def parse_complex_walk(
     algns1,
     algns2,
     max_insert_size,
     report_position,
     report_orientation,
     dedup_max_mismatch=3,
```

### Comparing `pairtools-1.0.3/pairtools/lib/parse_pysam.pyx` & `pairtools-1.1.0/pairtools/lib/parse_pysam.pyx`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/phase.py` & `pairtools-1.1.0/pairtools/lib/phase.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/regions.pyx` & `pairtools-1.1.0/pairtools/lib/regions.pyx`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/restrict.py` & `pairtools-1.1.0/pairtools/lib/restrict.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/scaling.py` & `pairtools-1.1.0/pairtools/lib/scaling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 
 from .regions import assign_regs_c
+from . import pairsio
 import bioframe
 
 
 def geomprog(factor, start=1):
     yield start
     while True:
         start *= factor
@@ -203,15 +204,16 @@
             "n_pairs": 1,
         },
         copy=False,
     )
 
     if not keep_unassigned:
         pairs_reduced_df = (pairs_reduced_df
-            .query('(start1 >= 0) and (end1 > 0) and (start2 >= 0) and (end2 > 0)')
+            .query('(start1 >= 0) and (start2 >= 0)') 
+            # do not test for end1 and end2, as they can be -1 if regions and not specified
             .reset_index(drop=True))
 
     pairs_reduced_df["min_dist"] = np.where(
         pairs_reduced_df["dist_bin_idx"] > 0,
         dist_bins[pairs_reduced_df["dist_bin_idx"] - 1],
         0,
     )
@@ -221,18 +223,22 @@
         dist_bins[pairs_reduced_df["dist_bin_idx"]],
         np.iinfo(np.int64).max,
     )
 
     # importantly, in the future, we may want to extend the function to plot scalings
     # for pairs from different regions!
 
-    pairs_for_scaling_mask = (
+    cis_region_pairs = (
         (pairs_reduced_df.chrom1 == pairs_reduced_df.chrom2)
         & (pairs_reduced_df.start1 == pairs_reduced_df.start2)
         & (pairs_reduced_df.end1 == pairs_reduced_df.end2)
+    )
+
+    pairs_for_scaling_mask = (
+        cis_region_pairs
         & (pairs_reduced_df.min_dist > 0)
         & (pairs_reduced_df.max_dist < np.iinfo(np.int64).max)
     )
 
     pairs_for_scaling_df = pairs_reduced_df.loc[pairs_for_scaling_mask]
 
     pairs_for_scaling_counts = pairs_for_scaling_df.groupby(
@@ -258,15 +264,15 @@
     pairs_for_scaling_counts["n_pairs"] = pairs_for_scaling_counts["n_pairs"].astype(
         np.int64
     )
 
     if ignore_trans:
         pairs_no_scaling_counts = None
     else:
-        pairs_no_scaling_df = pairs_reduced_df.loc[~pairs_for_scaling_mask]
+        pairs_no_scaling_df = pairs_reduced_df.loc[~cis_region_pairs]
 
         pairs_no_scaling_counts = pairs_no_scaling_df.groupby(
             by=[
                 "chrom1",
                 "start1",
                 "end1",
                 "chrom2",
@@ -324,79 +330,69 @@
     )
 
 
 def compute_scaling(
     pairs,
     regions=None,
     chromsizes=None,
-    dist_range=(int(1e1), int(1e9)),
-    n_dist_bins=8 * 8,
+    dist_range=(int(1e0), int(1e9)),
+    n_dist_bins_decade=8,
     chunksize=int(1e7),
     ignore_trans=False,
     keep_unassigned=False,
     filter_f=None,
-    nproc_in=1,
-    cmd_in=None,
+    nproc_in=4,
 ):
     """
-    Main function for computing scaling.
+    Compute the contact-frequency-vs-distance (aka "scaling") curve from a table of contacts.
 
     Parameters
     ----------
-    pairs: pd.DataFrame, stream of fiel paht with pairs.
-    regions: bioframe viewframe, anything that can serve as input to bioframe.from_any, or None
-    chromsizes: additional dataframe with chromosome sizes, if different from regions
-    dist_range: (int, int) tuple with distance ranges that will be split into windows
-    n_dist_bins: number of logarithmic bins
-    chunksize: size of chunks for calculations
-    ignore_trans: bool, ignore trans or not
-    keep_unassigned: bool, keep pairs that are not assigned to any region
-    filter_f: filter function that can be applied to each chunk
-    nproc_in
-    cmd_in
+    pairs : pd.DataFrame or str or file-like object
+        A table with pairs of genomic coordinates representing contacts. 
+        It can be a pandas DataFrame, a path to a pairs file, or a file-like object.
+    regions : bioframe viewframe or None, optional
+        Genomic regions of interest. It can be anything that can serve as input to bioframe.from_any,
+        or None if not applicable.
+    chromsizes : pd.DataFrame or None, optional
+        Additional dataframe with chromosome sizes, if different from regions.
+    dist_range : tuple of int, optional
+        The range of distances to calculate the scaling curve. Default is (10, 1000000000).
+    n_dist_bins : int, optional
+        The number of distance bins per order of magnitude in a log10-space. Default is 8.
+    chunksize : int, optional
+        Size of chunks for calculations. Default is 10000000.
+    ignore_trans : bool, optional
+        Ignore trans interactions or not. Default is False.
+    keep_unassigned : bool, optional
+        Keep pairs that are not assigned to any region or not. Default is False.
+    filter_f : function or None, optional
+        A function that to filter contacts. Default is None.
+    nproc_in : int, optional
+        Number of processes to use for reading pairs file. Default is 1.
 
     Returns
     -------
-
+    sc : pd.DataFrame
+        Scaling information for each distance bin.
+    trans_counts : pd.DataFrame or None
+        Trans interaction counts for each distance bin. None if ignore_trans is True.
     """
 
-    dist_bins = geomspace(dist_range[0], dist_range[1], n_dist_bins)
+    dist_bins = geomspace(
+        dist_range[0], 
+        dist_range[1],
+        int(np.round(np.log10(dist_range[1]/dist_range[0])*n_dist_bins_decade))
+    )
 
     if isinstance(pairs, pd.DataFrame):
         pairs_df = pairs
 
     elif isinstance(pairs, str) or hasattr(pairs, "buffer") or hasattr(pairs, "peek"):
-        from . import fileio, headerops
-
-        pairs_stream = (
-            fileio.auto_open(
-                pairs,
-                mode="r",
-                nproc=nproc_in,
-                command=cmd_in,
-            )
-            if isinstance(pairs, str)
-            else pairs
-        )
-
-        header, pairs_body = headerops.get_header(pairs_stream)
-
-        cols = headerops.extract_column_names(header)
-
-        if chromsizes is None:
-            chromsizes = headerops.extract_chromsizes(header)
-
-        pairs_df = pd.read_csv(
-            pairs_body,
-            header=None,
-            names=cols,
-            chunksize=chunksize,
-            sep="\t",
-            dtype={"chrom1": str, "chrom2": str},
-        )
+        pairs_df, _, _ = pairsio.read_pairs(pairs, nproc=nproc_in, chunksize=chunksize)
     else:
         raise ValueError(
             "pairs must be either a path to a pairs file or a pd.DataFrame"
         )
 
     sc, trans_counts = None, None
     for pairs_chunk in [pairs_df] if isinstance(pairs_df, pd.DataFrame) else pairs_df:
@@ -408,47 +404,81 @@
             regions=regions,
             chromsizes=chromsizes,
             ignore_trans=ignore_trans,
             keep_unassigned=keep_unassigned
         )
 
         sc = sc_chunk if sc is None else sc.add(sc_chunk, fill_value=0)
+
         trans_counts = (
             trans_counts_chunk
             if trans_counts is None
             else trans_counts.add(trans_counts_chunk, fill_value=0)
         )
 
+
     #         if not (isinstance(regions, pd.DataFrame) and
     #                  (set(regions.columns) == set(['chrom', 'start','end']))):
     #             raise ValueError('regions must be provided as a dict or chrom-indexed Series of chromsizes or as a bedframe.')
 
     sc.reset_index(inplace=True)
     sc["n_bp2"] = contact_areas_same_reg(
         sc["min_dist"], sc["max_dist"], sc["end1"] - sc["start1"]
     )
 
     if not ignore_trans:
         trans_counts.reset_index(inplace=True)
-        trans_counts["n_bp2"] = (trans_counts["end1"] - trans_counts["start1"]) * (
+        trans_counts["n_bp2"] = (
+            (trans_counts["end1"] - trans_counts["start1"]) * (
             trans_counts["end2"] - trans_counts["start2"]
-        )
+        ))
 
     return sc, trans_counts
 
 
-def norm_scaling_factor(bins, cfreqs, anchor=1.0, binwindow=(0, 3)):
-    i = np.searchsorted(bins, anchor)
-    return cfreqs[i + binwindow[0] : i + binwindow[1]].mean()
+def norm_scaling_factor(bins, cfreqs, norm_window):
+    """
+    Calculate the normalization factor for a contact-frequency-vs-distance curve,
+    by setting the average contact frequency in a specified range of distances to 1.0.
+
+    Args:
+        bins (array-like): The distance bins.
+        cfreqs (array-like): The contact frequencies.
+        norm_window (tuple of float): A tuple with the range of distances to use for normalization.
 
+    Returns:
+        float: The normalization scaling factor.
+    """
 
-def norm_scaling(bins, cfreqs, anchor=1.0, binwindow=(0, 3)):
-    return cfreqs / norm_scaling_factor(bins, cfreqs, anchor, binwindow)
+    lo, hi = np.searchsorted(bins, norm_window)
+    return cfreqs[lo:hi+1].mean()
 
 
+def norm_scaling(bins, cfreqs, norm_window, log_input=False):
+    """
+    Normalize a contact-frequency-vs-distance curve, by setting the average contact frequency 
+    in a given window to 1.0.
+
+    Args:
+        bins (array-like): The distance bins.
+        cfreqs (array-like): The contact frequencies.
+        norm_window (tuple of float): A tuple with the range of distances to use for normalization.
+        log_input (bool, optional): Whether the input contact frequencies were log-transformed. Defaults to False.
+
+    Returns:
+        float or array-like: The normalized contact frequencies.
+    """
+    
+    norm = norm_scaling_factor(bins, cfreqs, norm_window)
+    if log_input:
+        return cfreqs - norm
+    else:
+        return cfreqs / norm
+
+    
 def unity_norm_scaling(bins, cfreqs, norm_range=(1e4, 1e9)):
     bin_lens = np.diff(bins)
     bin_mids = np.sqrt(bins[1:] * bins[:-1])
 
     if norm_range is None:
         norm_cfreqs = cfreqs / np.sum(1.0 * (bin_lens * cfreqs)[np.isfinite(cfreqs)])
     else:
```

### Comparing `pairtools-1.0.3/pairtools/lib/select.py` & `pairtools-1.1.0/pairtools/lib/select.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/pairtools/lib/stats.py` & `pairtools-1.1.0/pairtools/lib/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,214 @@
 from .select import evaluate_df
 
 from .._logging import get_logger
 
 logger = get_logger()
 
 
+def parse_number(s):
+    if s.isdigit():
+        return int(s)
+    elif s.replace(".", "", 1).isdigit():
+        return float(s)
+    else:
+        return s   
+
+
+def flat_dict_to_nested(input_dict, sep='/'):
+    output_dict = {}
+
+    for key, value in input_dict.items():
+        if type(key) == tuple:
+            key_parts = key
+        elif type(key) == str:
+            key_parts = key.split(sep)
+        else:
+            raise ValueError(f"Key type can be either str or tuple. Found key {key} of type {type(key)}.")
+        
+        current_dict = output_dict
+        for key_part in key_parts[:-1]:
+            current_dict = current_dict.setdefault(key_part, {})
+        current_dict[key_parts[-1]] = value
+
+    return output_dict
+
+
+def nested_dict_to_flat(d, tuple_keys=False, sep='/'):
+    """Flatten a nested dictionary to a flat dictionary.
+
+    Parameters
+    ----------
+    d: dict
+        A nested dictionary to flatten.
+    tuple_keys: bool
+        If True, keys will be joined into tuples. Otherwise, they will be joined into strings.
+    sep: str
+        The separator to use between the parent key and the key if tuple_keys==False.
+    Returns
+    -------
+    dict
+        A flat dictionary.
+    """
+    
+    if tuple_keys:
+        join_keys = lambda k1,k2: (k1,) + k2
+    else:
+        join_keys = lambda k1,k2: (k1+sep+k2) if k2 else k1
+
+    out = {}
+
+    for k1, v1 in d.items():
+        if isinstance(v1, dict):
+            out.update({
+                join_keys(k1,k2): v2
+                for k2, v2 in nested_dict_to_flat(v1, tuple_keys, sep).items()
+            })
+        else:
+            if tuple_keys:
+                out[(k1,)] = v1
+            else:
+                out[k1] = v1
+    
+    return out
+
+def is_nested_dict(d):
+    """Check if a dictionary is nested.
+
+    Parameters
+    ----------
+    d: dict
+        A dictionary to check.
+    Returns
+    -------
+    bool
+        True if the dictionary is nested, False otherwise.
+    """
+
+    if not isinstance(d, dict):
+        return False
+
+    for v in d.values():
+        if isinstance(v, dict):
+            return True
+
+    return False
+
+def is_tuple_keyed_dict(d):
+    """Check if a dictionary is tuple-keyed.
+
+    Parameters
+    ----------
+    d: dict
+        A dictionary to check.
+    Returns
+    -------
+    bool
+        True if the dictionary is tuple-keyed, False otherwise.
+    """
+
+    if not isinstance(d, dict):
+        return False
+
+    for k,v in d.items():
+        if not isinstance(k, tuple):
+            return False
+        if isinstance(v, dict):
+            return False
+
+    return True
+
+def is_str_keyed_dict(d):
+    """Check if a dictionary is string-keyed.
+
+    Parameters
+    ----------
+    d: dict
+        A dictionary to check.
+    Returns
+    -------
+    bool
+        True if the dictionary is string-keyed, False otherwise.
+    """
+
+    if not isinstance(d, dict):
+        return False
+
+    for k,v in d.keys():
+        if not isinstance(k, str):
+            return False
+        if isinstance(v, dict):
+            return False
+
+    return True
+
+
+def swap_levels_nested_dict(nested_dict, level1, level2, sep='/'):
+    """Swap the order of two levels in a nested dictionary.
+
+    Parameters
+    ----------
+    nested_dict: dict
+        A nested dictionary.
+    level1: int
+        The index of the first level to swap.
+    level2: int
+        The index of the second level to swap.
+    Returns
+    -------
+    dict
+        A nested dictionary with the levels swapped.
+    """
+
+    if is_tuple_keyed_dict(nested_dict):
+        out = {}
+        for k1, v1 in nested_dict.items():
+            k1_list = list(k1)
+            k1_list[level1], k1_list[level2] = k1_list[level2], k1_list[level1]
+            out[tuple(k1_list)] = v1        
+        return out
+    
+    elif is_nested_dict(nested_dict):
+        out = nested_dict_to_flat(nested_dict, tuple_keys=True)
+        out = swap_levels_nested_dict(out, level1, level2)
+        out = flat_dict_to_nested(out)
+        return out
+    
+    elif is_str_keyed_dict(nested_dict):
+        out = nested_dict_to_flat(nested_dict, sep=sep)
+        out = swap_levels_nested_dict(out, level1, level2)
+        out = {sep.join(k):v for k,v in out.items()}
+        return out
+    
+    else:
+        raise ValueError("Input dictionary must be either nested, string-keyed or tuple-keyed")
+
 class PairCounter(Mapping):
     """
     A Counter for Hi-C pairs that accumulates various statistics.
     PairCounter implements two interfaces to access multi-level statistics:
     1. as a nested dict, e.g. pairCounter['pair_types']['LL']
     2. as a flat dict, with the level keys separated by '/', e.g. pairCounter['pair_types/LL']
     Other features:
     -- PairCounters can be saved into/loaded from a file
     -- multiple PairCounters can be merged via addition.
     """
 
     _SEP = "\t"
     _KEY_SEP = "/"
+    DIST_FREQ_REL_DIFF_THRESHOLD = 0.05
+    N_DIST_BINS_DECADE_DEFAULT = 8
+    MIN_LOG10_DIST_DEFAULT = 0
+    MAX_LOG10_DIST_DEFAULT = 9    
 
     def __init__(
         self,
-        min_log10_dist=0,
-        max_log10_dist=9,
-        log10_dist_bin_step=0.25,
+        min_log10_dist=MIN_LOG10_DIST_DEFAULT,
+        max_log10_dist=MAX_LOG10_DIST_DEFAULT,
+        n_dist_bins_decade=N_DIST_BINS_DECADE_DEFAULT,
         bytile_dups=False,
         filters=None,
         **kwargs,
     ):
         # Define filters and parameters for filters evaluation:
         if filters is not None:
             self.filters = filters
@@ -47,23 +228,26 @@
         # Define default filter:
         if "no_filter" not in self.filters:
             self.filters["no_filter"] = ""
         self._stat = {key: {} for key in self.filters}
 
         # some variables used for initialization:
         # genomic distance bining for the ++/--/-+/+- distribution
-        self._dist_bins = np.r_[
-            0,
-            np.round(
-                10
-                ** np.arange(
-                    min_log10_dist, max_log10_dist + 0.001, log10_dist_bin_step
-                )
-            ).astype(np.int_),
-        ]
+        log10_dist_bin_step = 1.0 / n_dist_bins_decade
+        self._dist_bins = np.unique(
+                np.r_[
+                0,
+                np.round(
+                    10
+                    ** np.arange(
+                        min_log10_dist, max_log10_dist + 0.001, log10_dist_bin_step
+                    )
+                ).astype(np.int_),
+            ]
+        )
 
         # establish structure of an empty _stat:
         for key in self.filters:
             self._stat[key]["filter_expression"] = self.filters[key]
             self._stat[key]["total"] = 0
             self._stat[key]["total_unmapped"] = 0
             self._stat[key]["total_single_sided_mapped"] = 0
@@ -73,16 +257,17 @@
             self._stat[key]["total_nodups"] = 0
             ########################################
             # the rest of stats are based on nodups:
             ########################################
             self._stat[key]["cis"] = 0
             self._stat[key]["trans"] = 0
             self._stat[key]["pair_types"] = {}
+            
             # to be removed:
-            self._stat[key]["dedup"] = {}
+            # self._stat[key]["dedup"] = {}
 
             self._stat[key]["cis_1kb+"] = 0
             self._stat[key]["cis_2kb+"] = 0
             self._stat[key]["cis_4kb+"] = 0
             self._stat[key]["cis_10kb+"] = 0
             self._stat[key]["cis_20kb+"] = 0
             self._stat[key]["cis_40kb+"] = 0
@@ -118,14 +303,15 @@
             self._bytile_dups = pd.DataFrame(
                 index=pd.MultiIndex(
                     levels=[[], []], codes=[[], []], names=["tile", "parent_tile"]
                 )
             )
         self._summaries_calculated = False
 
+
     def __getitem__(self, key, filter="no_filter"):
         if isinstance(key, str):
             # let's strip any unintentional '/'
             # from either side of the key
             key = key.strip("/")
             if self._KEY_SEP in key:
                 # multi-key to access nested elements
@@ -172,240 +358,277 @@
             # SHOULD THAT BE CHANGED IN .stats AND HERE AS WELL?
             if len(k_fields) == 2:
                 # assert 'dirs' in ['++','--','+-','-+']
                 dirs = k_fields.pop()
                 # there is only genomic distance range of the bin that's left:
                 (bin_range,) = k_fields
                 # extract left border of the bin "1000000+" or "1500-6000":
-                dist_bin_left = (
+                dist_bin_left = int(
                     bin_range.strip("+")
                     if bin_range.endswith("+")
                     else bin_range.split("-")[0]
                 )
-                # get the index of that bin:
-                bin_idx = (
-                    np.searchsorted(self._dist_bins, int(dist_bin_left), "right") - 1
-                )
                 # store corresponding value:
-                return self._stat[filter]["dist_freq"][dirs][bin_idx]
+                return self._stat[filter]["dist_freq"][dirs][dist_bin_left]
             else:
                 raise ValueError(
                     "{} is not a valid key: {} section implies 2 identifiers".format(
                         key, k
                     )
                 )
         else:
             raise ValueError("{} is not a valid key".format(k))
 
+
     def __iter__(self):
         return iter(self._stat)
 
+
     def __len__(self):
         return len(self._stat)
 
+
+    def find_dist_freq_convergence_distance(self, rel_threshold):
+        """Finds the largest distance at which the frequency of pairs of reads 
+        with different strands deviates from their average by the specified 
+        relative threshold."""
+        
+        out = {}
+        all_strands = ["++", "--", "-+", "+-"]
+
+        for filter in self.filters:
+            out[filter] = {}
+            
+            dist_freqs_by_strands = {
+                strands: np.array(list(self._stat[filter]["dist_freq"][strands].values()))
+                for strands in all_strands}
+            
+            # Calculate the average frequency of pairs with different strands
+            avg_freq_all_strands = np.mean(np.vstack(list(dist_freqs_by_strands.values())), axis=0)
+
+            # Calculate the largest distance at which the frequency of pairs of at least one strand combination deviates from the average by the given threshold
+            rel_deviations = {strands: np.nan_to_num(
+                np.abs(dist_freqs_by_strands[strands] - avg_freq_all_strands) 
+                / avg_freq_all_strands)
+                  for strands in all_strands}
+            
+            idx_maxs = {strand:0 for strand in all_strands}
+            for strands in all_strands:
+                bin_exceeds = rel_deviations[strands] > rel_threshold
+                if np.any(bin_exceeds):
+                    idx_maxs[strands] = np.max(np.nonzero(bin_exceeds))
+
+            # Find the largest distance and the strand combination where frequency of pairs deviates from the average by the given threshold:
+            convergence_bin_idx = 0
+            convergence_strands = '??'
+            convergence_dist = '0'
+
+            for strands in all_strands:
+                if (idx_maxs[strands] > convergence_bin_idx):
+                    convergence_bin_idx = idx_maxs[strands]
+                    convergence_strands = strands
+
+                    if idx_maxs[strands] < len(self._dist_bins):
+                        convergence_dist = self._dist_bins[convergence_bin_idx+1]
+                    else:
+                        convergence_dist = np.iinfo(np.int64)
+                    
+            
+            out[filter]["convergence_dist"] = convergence_dist
+            out[filter]["strands_w_max_convergence_dist"] = convergence_strands
+            out[filter]['convergence_rel_diff_threshold'] = rel_threshold
+
+            out[filter]['n_cis_pairs_below_convergence_dist'] = {
+                strands:dist_freqs_by_strands[strands][:convergence_bin_idx+1].sum() for strands in all_strands
+                for strands in all_strands
+            }
+
+            out[filter]['n_cis_pairs_below_convergence_dist_all_strands'] = sum(
+                list(out[filter]['n_cis_pairs_below_convergence_dist'].values())) 
+
+            n_cis_pairs_above_convergence_dist = {
+                strands:dist_freqs_by_strands[strands][convergence_bin_idx+1:].sum() for strands in all_strands
+                for strands in all_strands
+            }
+            
+            out[filter]['n_cis_pairs_above_convergence_dist_all_strands'] = sum(
+                list(n_cis_pairs_above_convergence_dist.values())) 
+
+            norms = dict(
+                cis=self._stat[filter]['cis'],
+                total_mapped=self._stat[filter]['total_mapped']
+            )
+
+            if 'total_nodups' in self._stat[filter]:
+                norms['total_nodups'] = self._stat[filter]['total_nodups']
+
+            for key, norm_factor in norms.items():
+                out[filter][f'frac_{key}_in_cis_below_convergence_dist'] = {
+                    strands: n_cis_pairs / norm_factor 
+                    for strands, n_cis_pairs in out[filter]['n_cis_pairs_below_convergence_dist'].items()
+                }
+
+                out[filter][f'frac_{key}_in_cis_below_convergence_dist_all_strands'] = sum(
+                    list(out[filter][f'frac_{key}_in_cis_below_convergence_dist'].values()))
+
+                out[filter][f'frac_{key}_in_cis_above_convergence_dist_all_strands'] = (
+                    sum(list(n_cis_pairs_above_convergence_dist.values())) / norm_factor )
+
+        return out
+
+
     def calculate_summaries(self):
         """calculate summary statistics (fraction of cis pairs at different cutoffs,
         complexity estimate) based on accumulated counts. Results are saved into
         self._stat["filter_name"]['summary"]
         """
-        for key in self.filters.keys():
-            self._stat[key]["summary"]["frac_dups"] = (
-                (self._stat[key]["total_dups"] / self._stat[key]["total_mapped"])
-                if self._stat[key]["total_mapped"] > 0
-                else 0
-            )
+        convergence_stats = self.find_dist_freq_convergence_distance(
+            self.DIST_FREQ_REL_DIFF_THRESHOLD)
 
+        for filter_name in self.filters.keys():
             for cis_count in (
                 "cis",
                 "cis_1kb+",
                 "cis_2kb+",
                 "cis_4kb+",
                 "cis_10kb+",
                 "cis_20kb+",
                 "cis_40kb+",
             ):
-                self._stat[key]["summary"][f"frac_{cis_count}"] = (
-                    (self._stat[key][cis_count] / self._stat[key]["total_nodups"])
-                    if self._stat[key]["total_nodups"] > 0
+                self._stat[filter_name]["summary"][f"frac_{cis_count}"] = (
+                    (self._stat[filter_name][cis_count] / self._stat[filter_name]["total_nodups"])
+                    if self._stat[filter_name]["total_nodups"] > 0
                     else 0
                 )
 
-            self._stat[key]["summary"][
+            self._stat[filter_name]["summary"]["dist_freq_convergence"] = convergence_stats[filter_name]
+
+            self._stat[filter_name]["summary"]["frac_dups"] = (
+                (self._stat[filter_name]["total_dups"] / self._stat[filter_name]["total_mapped"])
+                if self._stat[filter_name]["total_mapped"] > 0
+                else 0
+            )
+
+            self._stat[filter_name]["summary"][
                 "complexity_naive"
             ] = estimate_library_complexity(
-                self._stat[key]["total_mapped"], self._stat[key]["total_dups"], 0
+                self._stat[filter_name]["total_mapped"], self._stat[filter_name]["total_dups"], 0
             )
-            if key == "no_filter" and self._save_bytile_dups:
+
+            if filter_name == "no_filter" and self._save_bytile_dups:
                 # Estimate library complexity with information by tile, if provided:
                 if self._bytile_dups.shape[0] > 0:
-                    self._stat[key]["dups_by_tile_median"] = int(
+                    self._stat[filter_name]["dups_by_tile_median"] = int(
                         round(
                             self._bytile_dups["dup_count"].median()
                             * self._bytile_dups.shape[0]
                         )
                     )
-                if "dups_by_tile_median" in self._stat[key].keys():
-                    self._stat[key]["summary"][
+                if "dups_by_tile_median" in self._stat[filter_name].keys():
+                    self._stat[filter_name]["summary"][
                         "complexity_dups_by_tile_median"
                     ] = estimate_library_complexity(
-                        self._stat[key]["total_mapped"],
-                        self._stat[key]["total_dups"],
-                        self._stat[key]["total_dups"]
-                        - self._stat[key]["dups_by_tile_median"],
+                        self._stat[filter_name]["total_mapped"],
+                        self._stat[filter_name]["total_dups"],
+                        self._stat[filter_name]["total_dups"]
+                        - self._stat[filter_name]["dups_by_tile_median"],
                     )
 
             self._summaries_calculated = True
 
+
     @classmethod
-    def from_file(cls, file_handle):
+    def from_file(cls, file_handle, n_dist_bins_decade=N_DIST_BINS_DECADE_DEFAULT):
         """create instance of PairCounter from file
         Parameters
         ----------
         file_handle: file handle
         Returns
         -------
         PairCounter
             new PairCounter filled with the contents of the input file
         """
         # fill in from file - file_handle:
         default_filter = "no_filter"
-        stat_from_file = cls()
+        stat_from_file = cls(n_dist_bins_decade=n_dist_bins_decade)
+        raw_stat = {}
         for l in file_handle:
-            fields = l.strip().split(cls._SEP)
-            if len(fields) == 0:
+            key_val_pair = l.strip().split(cls._SEP)
+            if len(key_val_pair) == 0:
                 # skip empty lines:
                 continue
-            if len(fields) != 2:
+            if len(key_val_pair) != 2:
                 # expect two _SEP separated values per line:
                 raise fileio.ParseError(
                     "{} is not a valid stats file".format(file_handle.name)
                 )
-            # extract key and value, then split the key:
-            putative_key, putative_val = fields[0], fields[1]
-            key_fields = putative_key.split(cls._KEY_SEP)
-            # we should impose a rigid structure of .stats or redo it:
-            if len(key_fields) == 1:
-                key = key_fields[0]
-                if key in stat_from_file._stat[default_filter]:
-                    stat_from_file._stat[default_filter][key] = int(fields[1])
-                else:
-                    raise fileio.ParseError(
-                        "{} is not a valid stats file: unknown field {} detected".format(
-                            file_handle.name, key
-                        )
-                    )
-            else:
-                # in this case key must be in ['pair_types','chrom_freq','dist_freq','dedup', 'summary']
-                # get the first 'key' and keep the remainders in 'key_fields'
-                key = key_fields.pop(0)
-                if key in ["pair_types", "dedup", "summary", "chromsizes"]:
-                    # assert there is only one element in key_fields left:
-                    # 'pair_types', 'dedup', 'summary' and 'chromsizes' treated the same
-                    if len(key_fields) == 1:
-                        try:
-                            stat_from_file._stat[default_filter][key][
-                                key_fields[0]
-                            ] = int(fields[1])
-                        except ValueError:
-                            stat_from_file._stat[default_filter][key][
-                                key_fields[0]
-                            ] = float(fields[1])
-                    else:
-                        raise fileio.ParseError(
-                            "{} is not a valid stats file: {} section implies 1 identifier".format(
-                                file_handle.name, key
-                            )
-                        )
+            raw_stat[key_val_pair[0]] = parse_number(key_val_pair[1])
+        
 
-                elif key == "chrom_freq":
-                    # assert remaining key_fields == [chr1, chr2]:
-                    if len(key_fields) == 2:
-                        stat_from_file._stat[default_filter][key][
-                            tuple(key_fields)
-                        ] = int(fields[1])
-                    else:
-                        raise fileio.ParseError(
-                            "{} is not a valid stats file: {} section implies 2 identifiers".format(
-                                file_handle.name, key
-                            )
-                        )
+        ## TODO: check if raw_stat does not contain any unknown keys 
 
-                elif key == "dist_freq":
-                    # assert that last element of key_fields is the 'directions'
-                    if len(key_fields) == 2:
-                        # assert 'dirs' in ['++','--','+-','-+']
-                        dirs = key_fields.pop()
-                        # there is only genomic distance range of the bin that's left:
-                        (bin_range,) = key_fields
-                        # extract left border of the bin "1000000+" or "1500-6000":
-                        dist_bin_left = (
-                            bin_range.strip("+")
-                            if bin_range.endswith("+")
-                            else bin_range.split("-")[0]
-                        )
-                        # get the index of that bin:
-                        bin_idx = (
-                            np.searchsorted(
-                                stat_from_file._dist_bins, int(dist_bin_left), "right"
-                            )
-                            - 1
-                        )
-                        # store corresponding value:
-                        stat_from_file._stat[default_filter][key][dirs][bin_idx] = int(
-                            fields[1]
-                        )
-                    else:
-                        raise fileio.ParseError(
-                            "{} is not a valid stats file: {} section implies 2 identifiers".format(
-                                file_handle.name, key
-                            )
-                        )
-                else:
-                    raise fileio.ParseError(
-                        "{} is not a valid stats file: unknown field {} detected".format(
-                            file_handle.name, key
-                        )
-                    )
-        # return PairCounter from a non-empty dict:
+        # Convert flat dict to nested dict
+        stat_from_file._stat[default_filter].update(flat_dict_to_nested(raw_stat, sep=cls._KEY_SEP))
+
+        stat_from_file._stat[default_filter]['chrom_freq'] = nested_dict_to_flat(
+            stat_from_file._stat[default_filter]['chrom_freq'], tuple_keys=True)   
+
+        bin_to_left_val = lambda bin: int(bin.rstrip('+') if ('+' in bin) else bin.split('-')[0])
+
+        stat_from_file._stat[default_filter]['dist_freq'] = {
+            bin_to_left_val(k): v
+            for k,v in stat_from_file._stat[default_filter]['dist_freq'].items()
+        }  
+
+        stat_from_file._stat[default_filter]['dist_freq'] = swap_levels_nested_dict(
+            stat_from_file._stat[default_filter]['dist_freq'], 0, 1
+        )
+
+            
         return stat_from_file
 
     @classmethod
-    def from_yaml(cls, file_handle):
+    def from_yaml(cls, file_handle, n_dist_bins_decade=N_DIST_BINS_DECADE_DEFAULT):
         """create instance of PairCounter from file
         Parameters
         ----------
         file_handle: file handle
         Returns
         -------
         PairCounter
             new PairCounter filled with the contents of the input file
         """
         # fill in from file - file_handle:
-        stat_from_file = cls()
-
         stat = yaml.safe_load(file_handle)
+        stat_from_file = cls(
+            n_dist_bins_decade=n_dist_bins_decade,
+            filters={key: val.get("filter_expression", "") for key, val in stat.items()}
+        )
+
         for key, filter in stat.items():
             chromdict = {}
             for chroms in stat[key]["chrom_freq"].keys():
                 chromdict[tuple(chroms.split(cls._KEY_SEP))] = stat[key]["chrom_freq"][
                     chroms
                 ]
             stat[key]["chrom_freq"] = chromdict
         stat_from_file._stat = stat
         return stat_from_file
 
+
     def add_pair(
         self,
         chrom1,
         pos1,
         strand1,
         chrom2,
         pos2,
         strand2,
         pair_type,
+        unmapped_chrom="!",
         filter="no_filter",
     ):
         """Gather statistics for a Hi-C pair and add to the PairCounter.
         Parameters
         ----------
         chrom1: str
             chromosome of the first read
@@ -417,59 +640,57 @@
             chromosome of the first read
         pos2: int
             position of the first read
         strand2: str
             strand of the first read
         pair_type: str
             type of the mapped pair of reads
+        unmapped_chrom: str
+            what string denotes chromosomes in unmapped pairs (default: "!")
+        filter: str
+            name of the filter toward which the pair should count (default: "no_filter")
         """
 
         self._stat[filter]["total"] += 1
         # collect pair type stats including DD:
         self._stat[filter]["pair_types"][pair_type] = (
             self._stat[filter]["pair_types"].get(pair_type, 0) + 1
         )
-        if chrom1 == "!" and chrom2 == "!":
+        if chrom1 == unmapped_chrom and chrom2 == unmapped_chrom:
             self._stat[filter]["total_unmapped"] += 1
-        elif chrom1 != "!" and chrom2 != "!":
+        elif chrom1 != unmapped_chrom and chrom2 != unmapped_chrom:
             self._stat[filter]["total_mapped"] += 1
             # only mapped ones can be duplicates:
             if pair_type == "DD":
                 self._stat[filter]["total_dups"] += 1
             else:
                 self._stat[filter]["total_nodups"] += 1
                 self._stat[filter]["chrom_freq"][(chrom1, chrom2)] = (
                     self._stat[filter]["chrom_freq"].get((chrom1, chrom2), 0) + 1
                 )
 
                 if chrom1 == chrom2:
                     self._stat[filter]["cis"] += 1
                     dist = np.abs(pos2 - pos1)
-                    bin = self._dist_bins[
+                    dist_bin = self._dist_bins[
                         np.searchsorted(self._dist_bins, dist, "right") - 1
                     ]
-                    self._stat[filter]["dist_freq"][strand1 + strand2][bin] += 1
-                    if dist >= 1000:
-                        self._stat[filter]["cis_1kb+"] += 1
-                    if dist >= 2000:
-                        self._stat[filter]["cis_2kb+"] += 1
-                    if dist >= 4000:
-                        self._stat[filter]["cis_4kb+"] += 1
-                    if dist >= 10000:
-                        self._stat[filter]["cis_10kb+"] += 1
-                    if dist >= 20000:
-                        self._stat[filter]["cis_20kb+"] += 1
-                    if dist >= 40000:
-                        self._stat[filter]["cis_40kb+"] += 1
+                    self._stat[filter]["dist_freq"][strand1 + strand2][dist_bin] += 1
+
+                    for dist_kb in [1, 2, 4, 10, 20, 40]:
+                        if dist >= dist_kb * 1000:
+                            self._stat[filter][f"cis_{dist_kb}kb+"] += 1
+                        
 
                 else:
                     self._stat[filter]["trans"] += 1
         else:
             self._stat[filter]["total_single_sided_mapped"] += 1
 
+
     def add_pairs_from_dataframe(self, df, unmapped_chrom="!"):
         """Gather statistics for Hi-C pairs in a dataframe and add to the PairCounter.
 
         Parameters
         ----------
         df: pd.DataFrame
             DataFrame with pairs. Needs to have columns:
@@ -541,25 +762,29 @@
                     self._stat[key]["chrom_freq"].get((chrom1, chrom2), 0) + chrom_count
                 )
 
             # Count cis-trans by pairs:
 
             self._stat[key]["cis"] += df_cis.shape[0]
             self._stat[key]["trans"] += df_nodups.shape[0] - df_cis.shape[0]
+
+            # Count cis distance frequencies:
             dist = np.abs(df_cis["pos2"].values - df_cis["pos1"].values)
 
             df_cis.loc[:, "bin_idx"] = (
                 np.searchsorted(self._dist_bins, dist, "right") - 1
             )
+
             for (strand1, strand2, bin_id), strand_bin_count in (
                 df_cis[["strand1", "strand2", "bin_idx"]].value_counts().items()
             ):
                 self._stat[key]["dist_freq"][strand1 + strand2][
                     self._dist_bins[bin_id].item()
                 ] += strand_bin_count
+
             self._stat[key]["cis_1kb+"] += int(np.sum(dist >= 1000))
             self._stat[key]["cis_2kb+"] += int(np.sum(dist >= 2000))
             self._stat[key]["cis_4kb+"] += int(np.sum(dist >= 4000))
             self._stat[key]["cis_10kb+"] += int(np.sum(dist >= 10000))
             self._stat[key]["cis_20kb+"] += int(np.sum(dist >= 20000))
             self._stat[key]["cis_40kb+"] += int(np.sum(dist >= 40000))
 
@@ -592,69 +817,73 @@
         # If 'chromsizes' are present, they must be identical
         #
         # initialize empty PairCounter for the result of summation:
         sum_stat = PairCounter()
         # use the empty PairCounter to iterate over:
         for k, v in sum_stat._stat[filter].items():
             if k != "chromsizes" and (
-                k not in self._stat[filter] or k not in other._stat[filter]
+                (k not in self._stat[filter]) or (k not in other._stat[filter])
             ):
                 # Skip any missing fields and warn
                 logger.warning(
                     f"{k} not found in at least one of the input stats, skipping"
                 )
                 continue
+
             # not nested fields are summed trivially:
             if isinstance(v, int):
                 sum_stat._stat[filter][k] = (
                     self._stat[filter][k] + other._stat[filter][k]
                 )
+            
             # sum nested dicts/arrays in a context dependet manner:
             else:
-                if k in ["pair_types", "dedup", "summary"]:
+                if k in ["pair_types", "dedup"]:
                     # handy function for summation of a pair of dicts:
                     # https://stackoverflow.com/questions/10461531/merge-and-sum-of-two-dictionaries
                     sum_dicts = lambda dict_x, dict_y: {
                         key: dict_x.get(key, 0) + dict_y.get(key, 0)
                         for key in set(dict_x) | set(dict_y)
                     }
                     # sum a pair of corresponding dicts:
                     sum_stat._stat[filter][k] = sum_dicts(
                         self._stat[filter][k], other._stat[filter][k]
                     )
+                
                 elif k == "chrom_freq":
                     # union list of keys (chr1,chr2) with potential duplicates:
                     union_keys_with_dups = list(self._stat[filter][k].keys()) + list(
                         other._stat[filter][k].keys()
                     )
                     # dict.fromkeys will take care of keys' order and duplicates in a consistent manner:
                     # https://stackoverflow.com/questions/1720421/how-to-concatenate-two-lists-in-python
                     # last comment to the 3rd Answer
                     sum_stat._stat[filter][k] = dict.fromkeys(union_keys_with_dups)
                     # perform a summation:
                     for union_key in sum_stat._stat[filter][k]:
                         sum_stat._stat[filter][k][union_key] = self._stat[filter][
                             k
                         ].get(union_key, 0) + other._stat[filter][k].get(union_key, 0)
+                
                 elif k == "dist_freq":
                     for dirs in sum_stat[k]:
-
                         from functools import reduce
 
                         def reducer(accumulator, element):
                             for key, value in element.items():
                                 accumulator[key] = accumulator.get(key, 0) + value
                             return accumulator
 
                         sum_stat[k][dirs] = reduce(
                             reducer,
                             [self._stat[filter][k][dirs], other._stat[filter][k][dirs]],
                             {},
                         )
                         # sum_stat[k][dirs] = self._stat[filter][k][dirs] + other._stat[filter][k][dirs]
+                
                 elif k == "chromsizes":
                     if k in self._stat[filter] and k in other._stat[filter]:
                         if self._stat[filter][k] == other._stat[filter][k]:
                             sum_stat._stat[filter][k] = self._stat[filter][k]
                         elif (
                             len(self._stat[filter][k]) == 0
                             or len(other._stat[filter][k]) == 0
@@ -672,14 +901,16 @@
                                 "Can't merge stats with different chromsizes"
                             )
                     else:
                         logger.warning(
                             "One or both stats don't have chromsizes recorded"
                         )
 
+        sum_stat.calculate_summaries()
+
         return sum_stat
 
     # we need this to be able to sum(list_of_PairCounters)
     def __radd__(self, other):
         if other == 0:
             return self
         else:
@@ -691,88 +922,85 @@
         # dict for flat store:
         flat_stat = {}
 
         # Storing statistics
         for k, v in self._stat[filter].items():
             if isinstance(v, int):
                 flat_stat[k] = v
-            # store nested dicts/arrays in a context dependet manner:
+            # store nested dicts/arrays in a context dependent manner:
             # nested categories are stored only if they are non-trivial
             else:
                 if (k == "dist_freq") and v:
                     for i in range(len(self._dist_bins)):
                         for dirs, freqs in v.items():
+                            dist = self._dist_bins[i]
+                            
                             # last bin is treated differently: "100000+" vs "1200-3000":
-                            if i != len(self._dist_bins) - 1:
-                                dist = self._dist_bins[i]
+                            if i < len(self._dist_bins) - 1:
                                 dist_next = self._dist_bins[i + 1]
                                 formatted_key = self._KEY_SEP.join(
                                     ["{}", "{}-{}", "{}"]
                                 ).format(k, dist, dist_next, dirs)
-                            else:
+                            elif i == len(self._dist_bins) - 1:
                                 formatted_key = self._KEY_SEP.join(
                                     ["{}", "{}+", "{}"]
                                 ).format(k, dist, dirs)
+                            else:
+                                raise ValueError("There is a mismatch between dist_freq bins in the instance")
+                            
                             # store key,value pair:
-                            flat_stat[formatted_key] = freqs[dist]
-                elif (k in ["pair_types", "dedup", "chromsizes"]) and v:
+                            try:                        
+                                flat_stat[formatted_key] = freqs[dist]
+                            except:
+                                # in some previous versions of stats, last bin was not reported, so we need to skip it now:
+                                if (dist not in freqs) and (i == len(self._dist_bins) - 1):
+                                    flat_stat[formatted_key] = 0 
+                                else:
+                                    raise ValueError(f"Error in {k} {dirs} {dist} {dist_next} {freqs}: source and destination bins do not match")
+                
+                elif (k in ["pair_types", "dedup", "chromsizes", 'summary']) and v:
                     # 'pair_types' and 'dedup' are simple dicts inside,
                     # treat them the exact same way:
-                    for k_item, freq in v.items():
-                        formatted_key = self._KEY_SEP.join(["{}", "{}"]).format(
-                            k, k_item
-                        )
-                        # store key,value pair:
-                        flat_stat[formatted_key] = freq
+                    flat_stat.update(
+                        {k+self._KEY_SEP+k2 : v2 for k2,v2 in nested_dict_to_flat(v, sep=self._KEY_SEP).items()})
+                
                 elif (k == "chrom_freq") and v:
                     for (chrom1, chrom2), freq in v.items():
                         formatted_key = self._KEY_SEP.join(["{}", "{}", "{}"]).format(
                             k, chrom1, chrom2
                         )
                         # store key,value pair:
                         flat_stat[formatted_key] = freq
-                elif (k == "summary") and v:
-                    for key, frac in v.items():
-                        formatted_key = self._KEY_SEP.join(["{}", "{}"]).format(k, key)
-                        # store key,value pair:
-                        flat_stat[formatted_key] = frac
 
         # return flattened dict
         return flat_stat
 
     def format_yaml(self, filter="no_filter"):
         """return a formatted dict (for the yaml output)
         Performed for all filters at once."""
 
         from copy import deepcopy
 
-        formatted_stat = {key: {} for key in self.filters.keys()}
+        formatted_stat = {filter_name: {} for filter_name in self.filters.keys()}
 
         # Storing statistics for each filter
-        for key in self.filters.keys():
-            for k, v in self._stat[key].items():
-                if isinstance(v, int):
-                    formatted_stat[key][k] = v
-                # store nested dicts/arrays in a context dependet manner:
-                # nested categories are stored only if they are non-trivial
-                else:
-                    if (k != "chrom_freq") and v:
-                        # simple dicts inside
-                        # treat them the exact same way:
-                        formatted_stat[key][k] = deepcopy(v)
-                    elif (k == "chrom_freq") and v:
-                        # need to convert tuples of chromosome names to str
-                        freqs = {}
-                        for (chrom1, chrom2), freq in sorted(v.items()):
-                            freqs[
-                                self._KEY_SEP.join(["{}", "{}"]).format(chrom1, chrom2)
-                            ] = freq
-                            # store key,value pair:
-                        formatted_stat[key][k] = deepcopy(freqs)
+        for filter_name in self.filters.keys():
+            for k, v in self._stat[filter_name].items():
+                if (k == "chrom_freq"):
+                    v = {self._KEY_SEP.join(k2):v2 for k2, v2 in v.items()}
+                if v:
+                    formatted_stat[filter_name][k] = deepcopy(v)
             # return formatted dict
+        formatted_stat = nested_dict_to_flat(formatted_stat, tuple_keys=True)
+        for k in formatted_stat:
+            v = formatted_stat[k]
+            if isinstance(v, np.generic):
+                formatted_stat[k] = v.item()
+        formatted_stat = flat_dict_to_nested(formatted_stat)
+
         return formatted_stat
 
     def save(self, outstream, yaml=False, filter="no_filter"):
         """save PairCounter to tab-delimited text file.
         Flattened version of PairCounter is stored in the file.
         Parameters
         ----------
@@ -799,14 +1027,15 @@
             data = self.format_yaml()
             yaml.dump(data, outstream, default_flow_style=False, sort_keys=False)
         else:  # will output a single filter
             data = self.flatten(filter=filter)
             for k, v in data.items():
                 outstream.write("{}{}{}\n".format(k, self._SEP, v))
 
+
     def save_bytile_dups(self, outstream):
         """save bytile duplication counts to a tab-delimited text file.
         Parameters
         ----------
         outstream: file handle
         """
         if self._save_bytile_dups:
@@ -830,17 +1059,17 @@
             stat_file,
             mode="r",
             nproc=kwargs.get("nproc_in"),
             command=kwargs.get("cmd_in", None),
         )
         # use a factory method to instanciate PairCounter
         if kwargs.get("yaml", False):
-            stat = PairCounter.from_yaml(f)
+            stat = PairCounter.from_yaml(f, n_dist_bins_decade=kwargs.get('n_dist_bins_decade', PairCounter.N_DIST_BINS_DECADE_DEFAULT))
         else:
-            stat = PairCounter.from_file(f)
+            stat = PairCounter.from_file(f, n_dist_bins_decade=kwargs.get('n_dist_bins_decade', PairCounter.N_DIST_BINS_DECADE_DEFAULT))
         stats.append(stat)
         f.close()
 
     # combine stats from several files (files_to_merge):
     out_stat = sum(stats)
 
     # Save merged stats.
```

### Comparing `pairtools-1.0.3/pairtools.egg-info/PKG-INFO` & `pairtools-1.1.0/pairtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pairtools
-Version: 1.0.3
+Version: 1.1.0
 Summary: CLI tools to process mapped Hi-C data
 Home-page: https://github.com/open2c/pairtools
 Author: Open2C
 Author-email: open.chromosome.collective@gmail.com
 License: MIT
 Keywords: genomics,bioinformatics,Hi-C,contact
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cython
+Requires-Dist: numpy>=1.10
+Requires-Dist: click>=6.6
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: pandas>=1.3.4
+Requires-Dist: pysam>=0.15.0
+Requires-Dist: pyyaml
+Requires-Dist: bioframe>=0.3.3
 
 # pairtools
 
 [![Documentation Status](https://readthedocs.org/projects/pairtools/badge/?version=latest)](http://pairtools.readthedocs.org/en/latest/)
 [![Build Status](https://travis-ci.org/mirnylab/pairtools.svg?branch=master)](https://travis-ci.org/mirnylab/pairtools)
 [![Join the chat on Slack](https://img.shields.io/badge/chat-slack-%233F0F3F?logo=slack)](https://bit.ly/2UaOpAe)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1490831.svg)](https://doi.org/10.5281/zenodo.1490831)
```

### Comparing `pairtools-1.0.3/pairtools.egg-info/SOURCES.txt` & `pairtools-1.1.0/pairtools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 requirements_doc.txt
 setup.py
-/home/runner/work/pairtools/pairtools/pairtools/lib/dedup_cython.c
-/home/runner/work/pairtools/pairtools/pairtools/lib/parse_pysam.c
-/home/runner/work/pairtools/pairtools/pairtools/lib/regions.cpp
 doc/Makefile
 doc/cli_tools.rst
 doc/conf.py
+doc/designnotes.rst
 doc/formats.rst
 doc/index.rst
 doc/installation.rst
 doc/parsing.rst
+doc/protocols_pipelines.rst
 doc/quickstart.rst
 doc/sorting.rst
 doc/stats.rst
-doc/technotes.rst
 doc/_static/hic-processing-pipeline.png
 doc/_static/hic-processing-pipeline.svg
 doc/_static/read-vs-alignment-vs-pairs.svg
 doc/_static/read_pair_MU.png
 doc/_static/read_pair_MU_MM_NM.png
 doc/_static/read_pair_NU.png
 doc/_static/read_pair_NU_NN.png
@@ -32,14 +30,15 @@
 doc/_static/read_pair_WW.png
 doc/_static/read_pair_gaps_vs_null_alignment.png
 doc/_static/report-orientation.svg
 doc/_static/report-positions.svg
 doc/_static/rescue_modes.svg
 doc/_static/rescue_modes_readthrough.svg
 doc/_static/terminology.png
+doc/examples/duplicate_distance.ipynb
 doc/examples/example_pipeline.sh
 doc/examples/example_singlecell_pipeline.sh
 doc/examples/pairtools_phase_walkthrough.ipynb
 doc/examples/pairtools_restrict_walkthrough.ipynb
 doc/examples/pairtools_walkthrough.ipynb
 doc/examples/scalings_example.ipynb
 doc/examples/benchmark/Snakefile
@@ -75,14 +74,15 @@
 pairtools/lib/__init__.py
 pairtools/lib/dedup.py
 pairtools/lib/dedup_cython.pyx
 pairtools/lib/fileio.py
 pairtools/lib/filterbycov.py
 pairtools/lib/headerops.py
 pairtools/lib/pairsam_format.py
+pairtools/lib/pairsio.py
 pairtools/lib/parse.py
 pairtools/lib/parse_pysam.pyx
 pairtools/lib/phase.py
 pairtools/lib/regions.pyx
 pairtools/lib/restrict.py
 pairtools/lib/scaling.py
 pairtools/lib/select.py
@@ -100,17 +100,19 @@
 tests/test_scaling.py
 tests/test_select.py
 tests/test_sort.py
 tests/test_split.py
 tests/test_stats.py
 tests/data/mock.2.pairsam
 tests/data/mock.4dedup.pairsam
+tests/data/mock.4dedup_diffcolnames.pairsam
 tests/data/mock.4filterbycov.pairs
 tests/data/mock.4flip.pairs
 tests/data/mock.4stats.pairs
 tests/data/mock.chrom.sizes
 tests/data/mock.pairsam
 tests/data/mock.parse-all.sam
 tests/data/mock.parse2.sam
 tests/data/mock.rsites.bed
 tests/data/mock.sam
-tests/data/mock.test-restr.pairs
+tests/data/mock.test-restr.pairs
+tests/data/mock_empty.4dedup.pairsam
```

### Comparing `pairtools-1.0.3/setup.py` & `pairtools-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.2.pairsam` & `pairtools-1.1.0/tests/data/mock.2.pairsam`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.4dedup.pairsam` & `pairtools-1.1.0/tests/data/mock.4dedup.pairsam`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.4filterbycov.pairs` & `pairtools-1.1.0/tests/data/mock.4filterbycov.pairs`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.4flip.pairs` & `pairtools-1.1.0/tests/data/mock.4flip.pairs`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.4stats.pairs` & `pairtools-1.1.0/tests/data/mock.4stats.pairs`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.pairsam` & `pairtools-1.1.0/tests/data/mock.pairsam`

 * *Files 10% similar despite different names*

```diff
@@ -94,8 +94,27 @@
 000005d0: 2d09 5757 0972 6561 6469 6430 3819 3132  -.WW.readid08.12
 000005e0: 3919 6368 7231 1931 1936 3019 3130 314d  9.chr1.1.60.101M
 000005f0: 1963 6872 3119 3319 3019 4347 1946 4619  .chr1.3.0.CG.FF.
 00000600: 5853 3a69 3a30 1959 743a 5a3a 5757 0972  XS:i:0.Yt:Z:WW.r
 00000610: 6561 6469 6430 3819 3635 1963 6872 3119  eadid08.65.chr1.
 00000620: 3319 3630 1931 3031 4d19 6368 7231 1931  3.60.101M.chr1.1
 00000630: 1930 1941 5419 4949 1958 533a 693a 3019  .0.AT.II.XS:i:0.
-00000640: 5974 3a5a 3a57 570a                      Yt:Z:WW.
+00000640: 5974 3a5a 3a57 570a 7265 6164 6964 3039  Yt:Z:WW.readid09
+00000650: 0963 6872 3109 3132 3009 6368 7231 0931  .chr1.120.chr1.1
+00000660: 3231 092b 092b 0955 5509 7265 6164 6964  21.+.+.UU.readid
+00000670: 3039 1931 3239 1963 6872 3119 3132 3019  09.129.chr1.120.
+00000680: 3630 1931 3031 4d19 6368 7231 1931 3231  60.101M.chr1.121
+00000690: 1930 1943 4719 4646 1958 533a 693a 3019  .0.CG.FF.XS:i:0.
+000006a0: 5974 3a5a 3a55 5509 7265 6164 6964 3039  Yt:Z:UU.readid09
+000006b0: 1936 3519 6368 7231 1931 3231 1936 3019  .65.chr1.121.60.
+000006c0: 3130 314d 1963 6872 3119 3132 3019 3019  101M.chr1.120.0.
+000006d0: 4154 1949 4919 5853 3a69 3a30 1959 743a  AT.II.XS:i:0.Yt:
+000006e0: 5a3a 5555 0a72 6561 6469 6431 3009 6368  Z:UU.readid10.ch
+000006f0: 7231 0931 3309 6368 7231 0931 3409 2b09  r1.13.chr1.14.+.
+00000700: 2b09 5555 0972 6561 6469 6431 3019 3132  +.UU.readid10.12
+00000710: 3919 6368 7231 1931 3319 3630 1931 3031  9.chr1.13.60.101
+00000720: 4d19 6368 7231 1931 3419 3019 4347 1946  M.chr1.14.0.CG.F
+00000730: 4619 5853 3a69 3a30 1959 743a 5a3a 5555  F.XS:i:0.Yt:Z:UU
+00000740: 0972 6561 6469 6431 3019 3635 1963 6872  .readid10.65.chr
+00000750: 3119 3134 1936 3019 3130 314d 1963 6872  1.14.60.101M.chr
+00000760: 3119 3133 1930 1941 5419 4949 1958 533a  1.13.0.AT.II.XS:
+00000770: 693a 3019 5974 3a5a 3a55 550a            i:0.Yt:Z:UU.
```

### Comparing `pairtools-1.0.3/tests/data/mock.parse-all.sam` & `pairtools-1.1.0/tests/data/mock.parse-all.sam`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.parse2.sam` & `pairtools-1.1.0/tests/data/mock.parse2.sam`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.sam` & `pairtools-1.1.0/tests/data/mock.sam`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/data/mock.test-restr.pairs` & `pairtools-1.1.0/tests/data/mock.test-restr.pairs`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_filterbycov.py` & `pairtools-1.1.0/tests/test_filterbycov.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_flip.py` & `pairtools-1.1.0/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_header.py` & `pairtools-1.1.0/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_headerops.py` & `pairtools-1.1.0/tests/test_headerops.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_markasdup.py` & `pairtools-1.1.0/tests/test_markasdup.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_merge.py` & `pairtools-1.1.0/tests/test_merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,19 +86,19 @@
     # check the sorting order of the output:
     prev_pair = None
     for l in output_body:
         cur_pair = l.split("\t")[1:8]
         if prev_pair is not None:
             assert cur_pair[0] >= prev_pair[0]
             if cur_pair[0] == prev_pair[0]:
-                assert cur_pair[1] >= prev_pair[1]
-                if cur_pair[1] == prev_pair[1]:
-                    assert cur_pair[2] >= prev_pair[2]
-                    if cur_pair[2] == prev_pair[2]:
-                        assert cur_pair[3] >= prev_pair[3]
+                assert cur_pair[2] >= prev_pair[2]
+                if cur_pair[2] == prev_pair[2]:
+                    assert int(cur_pair[1]) >= int(prev_pair[1])
+                    if int(cur_pair[1]) == int(prev_pair[1]):
+                        assert int(cur_pair[3]) >= int(prev_pair[3])
 
         prev_pair = cur_pair
 
     # Check that the header is preserved:
     try:
         result = subprocess.check_output(
             [
```

### Comparing `pairtools-1.0.3/tests/test_parse.py` & `pairtools-1.1.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_parse2.py` & `pairtools-1.1.0/tests/test_parse2.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_restrict.py` & `pairtools-1.1.0/tests/test_restrict.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_scaling.py` & `pairtools-1.1.0/tests/test_scaling.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,8 +18,10 @@
     except subprocess.CalledProcessError as e:
         print(e.output)
         print(sys.exc_info())
         raise e
 
     output = pd.read_csv(io.StringIO(result), sep="\t", header=0)
 
-    assert output["n_pairs"].sum() == 5
+    assert (
+        output["n_pairs"].sum() == 9
+    )  # double unmapped pairs are currently ignored by lib.scaling
```

### Comparing `pairtools-1.0.3/tests/test_select.py` & `pairtools-1.1.0/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `pairtools-1.0.3/tests/test_sort.py` & `pairtools-1.1.0/tests/test_sort.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,12 +52,12 @@
     for l in output_body:
         cur_pair = l.split("\t")[1:8]
         if prev_pair is not None:
             assert cur_pair[0] >= prev_pair[0]
             if cur_pair[0] == prev_pair[0]:
                 assert cur_pair[2] >= prev_pair[2]
                 if cur_pair[2] == prev_pair[2]:
-                    assert cur_pair[1] >= prev_pair[1]
-                    if cur_pair[1] == prev_pair[1]:
-                        assert cur_pair[3] >= prev_pair[3]
+                    assert int(cur_pair[1]) >= int(prev_pair[1])
+                    if int(cur_pair[1]) == int(prev_pair[1]):
+                        assert int(cur_pair[3]) >= int(prev_pair[3])
 
         prev_pair = cur_pair
```

### Comparing `pairtools-1.0.3/tests/test_split.py` & `pairtools-1.1.0/tests/test_split.py`

 * *Files identical despite different names*

