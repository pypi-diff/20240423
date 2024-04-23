# Comparing `tmp/RsWaveform-0.2.0.tar.gz` & `tmp/rswaveform-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RsWaveform-0.2.0.tar", last modified: Tue Mar 12 07:42:29 2024, max compression
+gzip compressed data, was "rswaveform-0.3.0.tar", last modified: Tue Apr 23 12:28:52 2024, max compression
```

## Comparing `RsWaveform-0.2.0.tar` & `rswaveform-0.3.0.tar`

### file list

```diff
@@ -1,94 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.949536 RsWaveform-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.933536 RsWaveform-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.933536 RsWaveform-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-03-12 07:42:29.949536 RsWaveform-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.937536 RsWaveform-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-12 07:42:29.949536 RsWaveform-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.929536 RsWaveform-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.937536 RsWaveform-0.2.0/src/RsWaveform/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/LoadInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/ParentStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/SaveInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.937536 RsWaveform-0.2.0/src/RsWaveform/iqtar/
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqtar/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqtar/Save.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqtar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.937536 RsWaveform-0.2.0/src/RsWaveform/iqw/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqw/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqw/Save.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/iqw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.941536 RsWaveform-0.2.0/src/RsWaveform/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/meta/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/meta/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/meta/meta_iqtar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/meta/meta_wv.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.941536 RsWaveform-0.2.0/src/RsWaveform/utility/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/fake_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/integer_indexedproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/utility/meta_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.941536 RsWaveform-0.2.0/src/RsWaveform/wv/
--rw-r--r--   0 runner    (1001) docker     (127)    18632 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/wv/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11814 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/wv/Save.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/wv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.941536 RsWaveform-0.2.0/src/RsWaveform/wv/utility/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/wv/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/src/RsWaveform/wv/utility/array_to_bytes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.949536 RsWaveform-0.2.0/src/RsWaveform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-03-12 07:42:29.000000 RsWaveform-0.2.0/src/RsWaveform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-12 07:42:29.000000 RsWaveform-0.2.0/src/RsWaveform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 07:42:29.000000 RsWaveform-0.2.0/src/RsWaveform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-12 07:42:29.000000 RsWaveform-0.2.0/src/RsWaveform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 07:42:29.000000 RsWaveform-0.2.0/src/RsWaveform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.945536 RsWaveform-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:42:29.949536 RsWaveform-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy.iq.tar
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy.iqw
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy.wv
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy_2.wv
--rw-r--r--   0 runner    (1001) docker     (127)   808960 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy_huge.iq.tar
--rw-r--r--   0 runner    (1001) docker     (127)   800120 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy_huge.iqw
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy_multi_channel.iq.tar
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/dummy_mwv.wv
--rw-r--r--   0 runner    (1001) docker     (127)   400584 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/data/huge_dummy.wv
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_array_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_fake_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_integer_indexproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_iqtar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_iqw.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tests/test_wv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-12 07:42:05.000000 RsWaveform-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.952177 rswaveform-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.932177 rswaveform-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.936177 rswaveform-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 12:28:17.000000 rswaveform-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 12:28:17.000000 rswaveform-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-23 12:28:17.000000 rswaveform-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-23 12:28:52.952177 rswaveform-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-23 12:28:17.000000 rswaveform-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.936177 rswaveform-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 12:28:17.000000 rswaveform-0.3.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-23 12:28:17.000000 rswaveform-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 12:28:17.000000 rswaveform-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-23 12:28:52.952177 rswaveform-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.932177 rswaveform-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.936177 rswaveform-0.3.0/src/RsWaveform/
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.936177 rswaveform-0.3.0/src/RsWaveform/iqtar/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqtar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqtar/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqtar/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/iqw/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqw/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/iqw/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/load_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/meta/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/meta/meta_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/meta/meta_iqtar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/meta/meta_wv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/npz/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/npz/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/npz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/npz/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/npz/npz_inteface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/npz/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/parent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/save_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/fake_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/integer_indexedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/utility/meta_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/wv/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/wv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/wv/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/wv/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.940177 rswaveform-0.3.0/src/RsWaveform/wv/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/wv/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-23 12:28:17.000000 rswaveform-0.3.0/src/RsWaveform/wv/utility/array_to_bytes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.948177 rswaveform-0.3.0/src/RsWaveform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-23 12:28:52.000000 rswaveform-0.3.0/src/RsWaveform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-23 12:28:52.000000 rswaveform-0.3.0/src/RsWaveform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:28:52.000000 rswaveform-0.3.0/src/RsWaveform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 12:28:52.000000 rswaveform-0.3.0/src/RsWaveform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 12:28:52.000000 rswaveform-0.3.0/src/RsWaveform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.944177 rswaveform-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:28:52.948177 rswaveform-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy.iq.tar
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy.iqw
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy.wv
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy_2.wv
+-rw-r--r--   0 runner    (1001) docker     (127)   808960 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy_huge.iq.tar
+-rw-r--r--   0 runner    (1001) docker     (127)   800120 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy_huge.iqw
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy_multi_channel.iq.tar
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/dummy_mwv.wv
+-rw-r--r--   0 runner    (1001) docker     (127)   400584 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/data/huge_dummy.wv
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_array_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_fake_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_integer_indexproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_iqtar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_iqw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_npz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tests/test_wv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-23 12:28:17.000000 rswaveform-0.3.0/tox.ini
```

### Comparing `RsWaveform-0.2.0/.github/dependabot.yml` & `rswaveform-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/.github/workflows/linting.yml` & `rswaveform-0.3.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/.github/workflows/python-publish.yml` & `rswaveform-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/.github/workflows/tests.yml` & `rswaveform-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/.gitignore` & `rswaveform-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/.readthedocs.yaml` & `rswaveform-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/LICENSE` & `rswaveform-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/PKG-INFO` & `rswaveform-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsWaveform
-Version: 0.2.0
+Version: 0.3.0
 Summary: Load, manipulate and save R&S waveform files
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <Carsten.Sauerbrey@rohde-schwarz.com>, Daniela Rossetto <Daniela.Rossetto@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/RsWaveform
 Keywords: waveform,signal,load,save
 Platform: Unix
@@ -62,14 +62,22 @@
 
 ```sh
 $ pip install RsWaveform
 ```
 
 You need at least Python 3.8.
 
+## Setup environment
+
+To set up your environment, just run
+
+```py 
+pip install -r requirements-dev.txt
+```
+
 ## Usage
 
 ```py
 import RsWaveform
 ```
 
 ### Load waveform files
```

### Comparing `RsWaveform-0.2.0/README.md` & `rswaveform-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 
 ```sh
 $ pip install RsWaveform
 ```
 
 You need at least Python 3.8.
 
+## Setup environment
+
+To set up your environment, just run
+
+```py 
+pip install -r requirements-dev.txt
+```
+
 ## Usage
 
 ```py
 import RsWaveform
 ```
 
 ### Load waveform files
```

### Comparing `RsWaveform-0.2.0/docs/conf.py` & `rswaveform-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/pyproject.toml` & `rswaveform-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/LoadInterface.py` & `rswaveform-0.3.0/src/RsWaveform/load_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Load R&S waveform files."""
 
 from __future__ import annotations
 
 import abc
 import typing
 
-from .ParentStorage import ParentStorage
+from .parent_storage import ParentStorage
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
 
 
 class LoadInterface(abc.ABC):
     """Load R&S waveform implementation."""
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/ParentStorage.py` & `rswaveform-0.3.0/src/RsWaveform/parent_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 """Storage wrapper class for list of Storages."""
 
 import abc
 import typing
 from datetime import datetime
 
-from .Storage import Storage
+from .storage import Storage
 
 
 class ParentStorage(abc.ABC):
-    """ParentStorage class implementation."""
+    """ParentStorage class implementation.
 
-    def __init__(self, number_of_storages: int = 1):
+    Args:
+        number_of_storages (int, optional): Initialize number of storages.
+            Defaults to 1.
+        no_defaults (bool, optional): Storage meta data should have no defaults at
+            initialization. Defaults to False.
+
+    Raises:
+        ValueError: If number of storages is smaller than 1.
+    """
+
+    def __init__(self, number_of_storages: int = 1, no_defaults: bool = False):
         """Initialize ParentStorage class."""
         if number_of_storages <= 0:
             raise ValueError("Only positive number of storages allowed!")
-        self._storages = [Storage() for _ in range(number_of_storages)]
+        self._storages = [
+            Storage(no_defaults=no_defaults) for _ in range(number_of_storages)
+        ]
         self._filename: str = ""
         self._timestamp: datetime = datetime.now()
 
     @property
     def timestamp(self) -> datetime:
         """Get timestamp."""
         return self._timestamp
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/Storage.py` & `rswaveform-0.3.0/src/RsWaveform/storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,24 +31,32 @@
     """Encode datetime for msgpack."""
     if isinstance(obj, datetime):
         obj = {"__datetime__": True, "as_str": obj.strftime("%Y%m%dT%H:%M:%S.%f")}
     return obj
 
 
 class Storage(abc.ABC):
-    """Storage class implementation."""
+    """Storage class implementation.
 
-    def __init__(self, serialized: typing.Optional[bytes] = None) -> None:
+    Args:
+        serialized (typing.Optional[bytes], optional): Serialized data.
+            Defaults to None.
+        no_defaults (bool, optional): Storage meta data should have no defaults at
+            initialization. Defaults to False.
+    """
+
+    def __init__(
+        self, serialized: typing.Optional[bytes] = None, no_defaults: bool = False
+    ) -> None:
         """Initialize Storage class."""
         if serialized:
             self.deserialize(serialized)
         else:
             self.data: np.ndarray = np.zeros((1024,), dtype=np.complex128)
-            # self.meta: dict = {}
-            self.meta: Meta = Meta()
+            self.meta: Meta = Meta(no_defaults=no_defaults)
 
     @property
     def samples(self) -> int:
         """Number of waveform samples."""
         return len(self.data)
 
     def serialize(self) -> bytes:
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/__init__.py` & `rswaveform-0.3.0/src/RsWaveform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import io
 import typing
 from importlib.metadata import PackageNotFoundError, version
 
 import numpy as np
 
 from . import iqtar, iqw, wv
-from .LoadInterface import LoadInterface
+from .load_interface import LoadInterface
 from .meta import Meta
-from .ParentStorage import ParentStorage
-from .SaveInterface import SaveInterface
+from .parent_storage import ParentStorage
+from .save_interface import SaveInterface
 from .utility.dsp import (
     calculate_par,
     calculate_peak,
     calculate_rms,
     convert_to_db,
     normalize,
 )
@@ -188,15 +188,15 @@
         self.saver.save(file, self._parent_storage, scale)
 
 
 __all__ = [
     "RsWaveform",
     "Iqw",
     "IqTar",
-    "LoadInterface",
-    "SaveInterface",
+    "load_interface",
+    "save_interface",
     "calculate_par",
     "calculate_peak",
     "calculate_rms",
     "normalize",
     "convert_to_db",
 ]
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/__main__.py` & `rswaveform-0.3.0/src/RsWaveform/__main__.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/iqtar/Load.py` & `rswaveform-0.3.0/src/RsWaveform/iqtar/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from io import BytesIO
 
 import numpy as np
 
 from RsWaveform.meta import Meta
 
 from ..iqw import Load as LoadIqw
-from ..LoadInterface import LoadInterface
-from ..ParentStorage import ParentStorage
-from ..Storage import Storage
+from ..load_interface import LoadInterface
+from ..parent_storage import ParentStorage
+from ..storage import Storage
 from ..utility.file_handling import read_file_handle, read_file_handle_tar
 from ..utility.meta_utils import map_meta_information_name
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/iqtar/Save.py` & `rswaveform-0.3.0/src/RsWaveform/iqtar/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Save implementation for iqtar."""
 
 import os
 import re
 import typing
 from pathlib import Path
 
-from ..iqw.Save import Save as SaveIqw
+from ..iqw.save import Save as SaveIqw
 from ..meta.defaults import META_IQTAR_DEFAULTS as META_DEFAULTS
-from ..ParentStorage import ParentStorage
-from ..SaveInterface import SaveInterface
-from ..Storage import Storage
+from ..parent_storage import ParentStorage
+from ..save_interface import SaveInterface
+from ..storage import Storage
 from ..utility.file_handling import write_file_handle, write_file_handle_tar
 
 
 class Save(SaveInterface):
     """Save class for iqtar."""
 
     def save(
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/iqw/Load.py` & `rswaveform-0.3.0/src/RsWaveform/iqw/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from __future__ import annotations
 
 import typing
 
 import numpy as np
 
-from ..LoadInterface import LoadInterface
-from ..ParentStorage import ParentStorage
+from ..load_interface import LoadInterface
+from ..parent_storage import ParentStorage
 from ..utility.fake_jit import jit
 from ..utility.file_handling import read_file_handle
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
 
 
 class Load(LoadInterface):
     """Load class for iqw."""
 
     def load(self, file: typing.Union[str, typing.IO, Path]) -> ParentStorage:
         """Load iwq data from file."""
-        parent_storage = ParentStorage()
+        parent_storage = ParentStorage(no_defaults=True)
         with read_file_handle(file) as fp:
             content = fp.read()
         iq_data = self._extract_iq(content)
         parent_storage.storages[0].data = iq_data
         if isinstance(file, str):
             parent_storage.filename = file
         return parent_storage
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/iqw/Save.py` & `rswaveform-0.3.0/src/RsWaveform/iqw/save.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from __future__ import annotations
 
 import math
 import typing
 
 import numpy as np
 
-from ..ParentStorage import ParentStorage
-from ..SaveInterface import SaveInterface
-from ..Storage import Storage
+from ..parent_storage import ParentStorage
+from ..save_interface import SaveInterface
+from ..storage import Storage
 from ..utility.fake_jit import jit
 from ..utility.file_handling import write_file_handle
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/meta/meta_base.py` & `rswaveform-0.3.0/src/RsWaveform/meta/meta_base.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/meta/meta_iqtar.py` & `rswaveform-0.3.0/src/RsWaveform/meta/meta_iqtar.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/meta/meta_wv.py` & `rswaveform-0.3.0/src/RsWaveform/meta/meta_wv.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,22 +78,40 @@
 
     @control_length.setter
     def control_length(self, value: typing.Optional[int]) -> None:
         self._items["control_length"] = value
 
     @property
     def rms(self) -> typing.Optional[float]:
-        """Read the RMS value."""
+        """The RMS value of the signal."""
         return self._items.get("rms")
 
     @rms.setter
     def rms(self, value: float) -> None:
         self._items["rms"] = value
 
     @property
     def peak(self) -> typing.Optional[float]:
-        """Read the signal peak value."""
+        """The signal peak value of the signal."""
         return self._items.get("peak")
 
     @peak.setter
     def peak(self, value: float) -> None:
         self._items["peak"] = value
+
+    @property
+    def samples(self) -> typing.Optional[int]:
+        """The sample count of the waveform."""
+        return self._items.get("samples")
+
+    @samples.setter
+    def samples(self, value: int) -> None:
+        self._items["samples"] = value
+
+    @property
+    def reflevel(self) -> typing.Optional[float]:
+        """The reference value of the signal."""
+        return self._items.get("reflevel")
+
+    @reflevel.setter
+    def reflevel(self, value: float) -> None:
+        self._items["reflevel"] = value
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/utility/dsp.py` & `rswaveform-0.3.0/src/RsWaveform/utility/dsp.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/utility/file_handling.py` & `rswaveform-0.3.0/src/RsWaveform/utility/file_handling.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/utility/integer_indexedproperty.py` & `rswaveform-0.3.0/src/RsWaveform/utility/integer_indexedproperty.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform/wv/Load.py` & `rswaveform-0.3.0/src/RsWaveform/wv/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import logging
 import re
 import typing
 from datetime import datetime
 
 import numpy as np
 
-from ..LoadInterface import LoadInterface
+from ..load_interface import LoadInterface
 from ..meta import Meta
-from ..ParentStorage import ParentStorage
-from ..Storage import Storage
+from ..parent_storage import ParentStorage
+from ..storage import Storage
 from ..utility.fake_jit import jit
 from ..utility.file_handling import read_file_handle
 from .utility.array_to_bytes import unpack_bytes_to_bool_array
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
 
@@ -88,44 +88,44 @@
                     break
                 else:
                     return part, separator + buffer
 
     def load_in_chunks(
         self,
         file: typing.Union[str, typing.IO, Path],
-        nr_samples: int,
-        samples_offset: int,
+        samples: int,
+        offset: int,
     ) -> ParentStorage:
         """Load chunk waveform data from file."""
         separators = ["{WWAVEFORM", "{WAVEFORM"]
         with read_file_handle(file) as fp:
             header_content, content = self._read_chunks(fp, separators)
-            content += fp.read((nr_samples + 4) * 4 + 100)
+            content += fp.read((samples + 4) * 4 + 100)
             # +4 due to opt words and 100 just an offset to make sure we get everything
 
         tags = self._split_data_via_tags_meta(header_content)
         tags.update(self._split_data_via_tags_waveform(content, True))
         tags.update(
-            self._split_data_via_tags_control_list_width4(content, nr_samples, True)
+            self._split_data_via_tags_control_list_width4(content, samples, True)
         )
 
         mwv_segment_count = int(tags.pop("mwv segment count", 1))
         if mwv_segment_count > 1:  # multi segment waveform
             raise ValueError("feature only supported for non multi segment wv")
         parent_storage = ParentStorage()
         if isinstance(file, str):
             parent_storage.filename = file
         storages = [Storage() for _ in range(mwv_segment_count)]
-        iq_data = self._extract_iq_chunks(tags, nr_samples, samples_offset)
+        iq_data = self._extract_iq_chunks(tags, samples, offset)
         index = 0
         storages[index].data = iq_data
         meta = self._extract_meta(tags, index)
         meta = self._handle_mwv_meta_data(meta, index)
         storages[index].meta = Meta(**meta)
-        if nr_samples != len(iq_data):
+        if samples != len(iq_data):
             raise ValueError(
                 "Sanity problem. Sample setting and actual sample count does not match."
             )
         parent_storage.storages = storages
         return parent_storage
 
     def load_meta(self, file: typing.Union[str, typing.IO, Path]) -> ParentStorage:
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/wv/Save.py` & `rswaveform-0.3.0/src/RsWaveform/wv/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import math
 import typing
 
 import numpy as np
 
 from ..meta.defaults import META_WV_DEFAULTS as META_DEFAULTS
-from ..ParentStorage import ParentStorage
-from ..SaveInterface import SaveInterface
-from ..Storage import Storage
+from ..parent_storage import ParentStorage
+from ..save_interface import SaveInterface
+from ..storage import Storage
 from ..utility.dsp import calculate_peak, calculate_rms
 from ..utility.fake_jit import jit
 from ..utility.file_handling import write_file_handle
 from .utility.array_to_bytes import pack_bool_array_to_bytes
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform/wv/utility/array_to_bytes.py` & `rswaveform-0.3.0/src/RsWaveform/wv/utility/array_to_bytes.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/src/RsWaveform.egg-info/PKG-INFO` & `rswaveform-0.3.0/src/RsWaveform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsWaveform
-Version: 0.2.0
+Version: 0.3.0
 Summary: Load, manipulate and save R&S waveform files
 Author-email: "Rohde & Schwarz GmbH & Co. KG" <info@rohde-schwarz.com>
 Maintainer-email: Carsten Sauerbrey <Carsten.Sauerbrey@rohde-schwarz.com>, Daniela Rossetto <Daniela.Rossetto@rohde-schwarz.com>
 License: MIT
 Project-URL: project, https://github.com/Rohde-Schwarz/RsWaveform
 Keywords: waveform,signal,load,save
 Platform: Unix
@@ -62,14 +62,22 @@
 
 ```sh
 $ pip install RsWaveform
 ```
 
 You need at least Python 3.8.
 
+## Setup environment
+
+To set up your environment, just run
+
+```py 
+pip install -r requirements-dev.txt
+```
+
 ## Usage
 
 ```py
 import RsWaveform
 ```
 
 ### Load waveform files
```

### Comparing `RsWaveform-0.2.0/src/RsWaveform.egg-info/SOURCES.txt` & `rswaveform-0.3.0/src/RsWaveform.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,64 +15,71 @@
 docs/api.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/installation.md
 docs/usage.md
-src/RsWaveform/LoadInterface.py
-src/RsWaveform/ParentStorage.py
-src/RsWaveform/SaveInterface.py
-src/RsWaveform/Storage.py
 src/RsWaveform/__init__.py
 src/RsWaveform/__main__.py
+src/RsWaveform/load_interface.py
+src/RsWaveform/parent_storage.py
 src/RsWaveform/py.typed
+src/RsWaveform/save_interface.py
+src/RsWaveform/storage.py
 src/RsWaveform.egg-info/PKG-INFO
 src/RsWaveform.egg-info/SOURCES.txt
 src/RsWaveform.egg-info/dependency_links.txt
 src/RsWaveform.egg-info/requires.txt
 src/RsWaveform.egg-info/top_level.txt
-src/RsWaveform/iqtar/Load.py
-src/RsWaveform/iqtar/Save.py
 src/RsWaveform/iqtar/__init__.py
-src/RsWaveform/iqw/Load.py
-src/RsWaveform/iqw/Save.py
+src/RsWaveform/iqtar/load.py
+src/RsWaveform/iqtar/save.py
 src/RsWaveform/iqw/__init__.py
+src/RsWaveform/iqw/load.py
+src/RsWaveform/iqw/save.py
 src/RsWaveform/meta/__init__.py
 src/RsWaveform/meta/defaults.py
 src/RsWaveform/meta/meta_base.py
 src/RsWaveform/meta/meta_iqtar.py
 src/RsWaveform/meta/meta_wv.py
+src/RsWaveform/npz/README.md
+src/RsWaveform/npz/__init__.py
+src/RsWaveform/npz/load.py
+src/RsWaveform/npz/npz_inteface.py
+src/RsWaveform/npz/save.py
 src/RsWaveform/utility/__init__.py
 src/RsWaveform/utility/dsp.py
 src/RsWaveform/utility/fake_jit.py
 src/RsWaveform/utility/file_handling.py
 src/RsWaveform/utility/integer_indexedproperty.py
 src/RsWaveform/utility/meta_utils.py
-src/RsWaveform/wv/Load.py
-src/RsWaveform/wv/Save.py
 src/RsWaveform/wv/__init__.py
+src/RsWaveform/wv/load.py
+src/RsWaveform/wv/save.py
 src/RsWaveform/wv/utility/__init__.py
 src/RsWaveform/wv/utility/array_to_bytes.py
 tests/__init__.py
 tests/conftest.py
 tests/test_Storage.py
 tests/test_array_to_bytes.py
 tests/test_dsp.py
 tests/test_fake_jit.py
 tests/test_file_handling.py
 tests/test_integer_indexproperty.py
 tests/test_iqtar.py
 tests/test_iqw.py
 tests/test_main.py
 tests/test_meta.py
+tests/test_npz.py
 tests/test_version.py
 tests/test_wv.py
 tests/data/dummy.iq.tar
 tests/data/dummy.iqw
+tests/data/dummy.npz
 tests/data/dummy.wv
 tests/data/dummy_2.wv
 tests/data/dummy_huge.iq.tar
 tests/data/dummy_huge.iqw
 tests/data/dummy_multi_channel.iq.tar
 tests/data/dummy_mwv.wv
 tests/data/huge_dummy.wv
```

### Comparing `RsWaveform-0.2.0/tests/conftest.py` & `rswaveform-0.3.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,7 +45,13 @@
     return os.path.join(os.path.realpath(dirname), "data", "dummy_huge.iq.tar")
 
 
 @pytest.fixture
 def reference_iqtar_file_name_multi_channel() -> str:
     dirname = os.path.dirname(__file__)
     return os.path.join(os.path.realpath(dirname), "data", "dummy_multi_channel.iq.tar")
+
+
+@pytest.fixture
+def reference_npz_file_name() -> str:
+    dirname = os.path.dirname(__file__)
+    return os.path.join(os.path.realpath(dirname), "data", "dummy.npz")
```

### Comparing `RsWaveform-0.2.0/tests/data/dummy.iq.tar` & `rswaveform-0.3.0/tests/data/dummy.iq.tar`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/data/dummy_huge.iq.tar` & `rswaveform-0.3.0/tests/data/dummy_huge.iq.tar`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/data/dummy_multi_channel.iq.tar` & `rswaveform-0.3.0/tests/data/dummy_multi_channel.iq.tar`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/data/dummy_mwv.wv` & `rswaveform-0.3.0/tests/data/dummy_mwv.wv`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/data/huge_dummy.wv` & `rswaveform-0.3.0/tests/data/huge_dummy.wv`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_Storage.py` & `rswaveform-0.3.0/tests/test_Storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from datetime import datetime
 
 import numpy as np
 import pytest
 
 from RsWaveform.meta import Meta
-from RsWaveform.ParentStorage import ParentStorage
-from RsWaveform.Storage import Storage, encode_datetime, msgpack_import
+from RsWaveform.parent_storage import ParentStorage
+from RsWaveform.storage import Storage, encode_datetime, msgpack_import
 
 
 @pytest.fixture
 def reference_now() -> datetime:
     return datetime.now()
```

### Comparing `RsWaveform-0.2.0/tests/test_array_to_bytes.py` & `rswaveform-0.3.0/tests/test_array_to_bytes.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_dsp.py` & `rswaveform-0.3.0/tests/test_dsp.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_file_handling.py` & `rswaveform-0.3.0/tests/test_file_handling.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_integer_indexproperty.py` & `rswaveform-0.3.0/tests/test_integer_indexproperty.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_iqtar.py` & `rswaveform-0.3.0/tests/test_iqtar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from datetime import datetime
 
 import numpy as np
 import pytest
 
 from RsWaveform import IqTar
-from RsWaveform.iqtar.Load import Load
-from RsWaveform.iqtar.Save import Save
+from RsWaveform.iqtar.load import Load
+from RsWaveform.iqtar.save import Save
 from RsWaveform.meta import Meta
-from RsWaveform.ParentStorage import ParentStorage
-from RsWaveform.Storage import Storage
+from RsWaveform.parent_storage import ParentStorage
+from RsWaveform.storage import Storage
 
 
 @pytest.fixture
 def reference() -> np.ndarray:
     return np.array([0.2, 0.6]) + 1j * np.array([0.4, 0.8])
```

### Comparing `RsWaveform-0.2.0/tests/test_iqw.py` & `rswaveform-0.3.0/tests/test_iqw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import io
 
 import numpy as np
 import pytest
 
 from RsWaveform import Iqw
-from RsWaveform.iqw.Load import Load
-from RsWaveform.iqw.Save import Save
+from RsWaveform.iqw.load import Load
+from RsWaveform.iqw.save import Save
 from RsWaveform.meta import Meta
-from RsWaveform.ParentStorage import ParentStorage
+from RsWaveform.parent_storage import ParentStorage
 
 
 @pytest.fixture
 def reference() -> np.ndarray:
     return np.array([0.2, 0.6]) + 1j * np.array([0.4, 0.8])
```

### Comparing `RsWaveform-0.2.0/tests/test_meta.py` & `rswaveform-0.3.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `RsWaveform-0.2.0/tests/test_wv.py` & `rswaveform-0.3.0/tests/test_wv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 
 from RsWaveform import RsWaveform, normalize
 from RsWaveform.meta import Meta
-from RsWaveform.ParentStorage import ParentStorage
-from RsWaveform.Storage import Storage
-from RsWaveform.wv.Load import Load
-from RsWaveform.wv.Save import Save
+from RsWaveform.parent_storage import ParentStorage
+from RsWaveform.storage import Storage
+from RsWaveform.wv.load import Load
+from RsWaveform.wv.save import Save
 
 
 @pytest.fixture
 def reference() -> np.ndarray:
     return np.array([0.2, 0.6]) + 1j * np.array([0.4, 0.8])
```

### Comparing `RsWaveform-0.2.0/tox.ini` & `rswaveform-0.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 commands = pydocstyle {posargs:src/}
 
 [testenv:flake]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     flake8
-    flake8-colors
 commands =
     flake8 --select F {posargs:src/ tests/}
 
 [testenv:pylint]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
```

