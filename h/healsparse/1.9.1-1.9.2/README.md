# Comparing `tmp/healsparse-1.9.1.tar.gz` & `tmp/healsparse-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healsparse-1.9.1.tar", last modified: Fri Mar 15 16:45:39 2024, max compression
+gzip compressed data, was "healsparse-1.9.2.tar", last modified: Tue Apr 23 15:48:49 2024, max compression
```

## Comparing `healsparse-1.9.1.tar` & `healsparse-1.9.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.116268 healsparse-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 16:45:23.000000 healsparse-1.9.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-15 16:45:23.000000 healsparse-1.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.096267 healsparse-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.100267 healsparse-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-15 16:45:23.000000 healsparse-1.9.1/.github/workflows/python-package-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-15 16:45:23.000000 healsparse-1.9.1/.github/workflows/python-package-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-15 16:45:23.000000 healsparse-1.9.1/.github/workflows/python-package-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-15 16:45:23.000000 healsparse-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-15 16:45:23.000000 healsparse-1.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-15 16:45:23.000000 healsparse-1.9.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-15 16:45:23.000000 healsparse-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-15 16:45:23.000000 healsparse-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-15 16:45:39.116268 healsparse-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-15 16:45:23.000000 healsparse-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-15 16:45:23.000000 healsparse-1.9.1/api_changes_to_1.0.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.104267 healsparse-1.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/basic_interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/concatenation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14662 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/filespec.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/operations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/randoms.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-15 16:45:23.000000 healsparse-1.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.108267 healsparse-1.9.1/healsparse/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/cat_healsparse_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)   104520 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/healSparseMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/healSparseRandoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_coverage_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_coverage_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    29117 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_map_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_map_healpix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/io_map_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    28625 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/packedBoolArray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/parquet_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-03-15 16:45:23.000000 healsparse-1.9.1/healsparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.112267 healsparse-1.9.1/healsparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-15 16:45:39.000000 healsparse-1.9.1/healsparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-15 16:45:39.000000 healsparse-1.9.1/healsparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:45:39.000000 healsparse-1.9.1/healsparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-15 16:45:39.000000 healsparse-1.9.1/healsparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 16:45:39.000000 healsparse-1.9.1/healsparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:45:38.000000 healsparse-1.9.1/healsparse.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-15 16:45:23.000000 healsparse-1.9.1/long_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-15 16:45:23.000000 healsparse-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-15 16:45:23.000000 healsparse-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-15 16:45:39.116268 healsparse-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.112267 healsparse-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_applymask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_astype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_boolean_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_buildmaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_cat_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_coverage_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_coverage_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    29282 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_degrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_emptypixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_fracdet_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_from_healpix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_generate_healpix.py
--rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_getset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_healpix_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_io_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_moc.py
--rw-r--r--   0 runner    (1001) docker     (127)    48106 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    53737 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_packedboolarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_pixel_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_randoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_recarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_single_covpix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_single_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_singlevalues.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_update_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_validarea.py
--rw-r--r--   0 runner    (1001) docker     (127)    35376 2024-03-15 16:45:23.000000 healsparse-1.9.1/tests/test_widemasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.112267 healsparse-1.9.1/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)    24213 2024-03-15 16:45:23.000000 healsparse-1.9.1/tutorial/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:45:39.112267 healsparse-1.9.1/ups/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-15 16:45:23.000000 healsparse-1.9.1/ups/healsparse.table
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:49.007284 healsparse-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 15:48:38.000000 healsparse-1.9.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 15:48:38.000000 healsparse-1.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:48.987284 healsparse-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:48.991284 healsparse-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-23 15:48:38.000000 healsparse-1.9.2/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-23 15:48:38.000000 healsparse-1.9.2/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-23 15:48:38.000000 healsparse-1.9.2/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 15:48:38.000000 healsparse-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 15:48:38.000000 healsparse-1.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 15:48:38.000000 healsparse-1.9.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-23 15:48:38.000000 healsparse-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 15:48:38.000000 healsparse-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-23 15:48:49.007284 healsparse-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-23 15:48:38.000000 healsparse-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 15:48:38.000000 healsparse-1.9.2/api_changes_to_1.0.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:48.995284 healsparse-1.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/basic_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/concatenation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14662 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/filespec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/operations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/randoms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 15:48:38.000000 healsparse-1.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:48.995284 healsparse-1.9.2/healsparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/cat_healsparse_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104520 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/healSparseMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/healSparseRandoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_coverage_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_coverage_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29164 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_map_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_map_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/io_map_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28625 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/packedBoolArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/parquet_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-23 15:48:38.000000 healsparse-1.9.2/healsparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:49.007284 healsparse-1.9.2/healsparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:48:48.000000 healsparse-1.9.2/healsparse.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-23 15:48:38.000000 healsparse-1.9.2/long_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 15:48:38.000000 healsparse-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 15:48:38.000000 healsparse-1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-23 15:48:49.007284 healsparse-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:49.007284 healsparse-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_applymask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_astype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_boolean_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_buildmaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_cat_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_coverage_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_coverage_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29282 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_degrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_emptypixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_fracdet_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_from_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_generate_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_getset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_healpix_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_io_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_moc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48106 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53737 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_packedboolarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_pixel_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_randoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_recarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_single_covpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_single_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_singlevalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_update_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_validarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35376 2024-04-23 15:48:38.000000 healsparse-1.9.2/tests/test_widemasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:49.007284 healsparse-1.9.2/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)    24213 2024-04-23 15:48:38.000000 healsparse-1.9.2/tutorial/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:48:49.007284 healsparse-1.9.2/ups/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 15:48:38.000000 healsparse-1.9.2/ups/healsparse.table
```

### Comparing `healsparse-1.9.1/.github/workflows/python-package-pr.yml` & `healsparse-1.9.2/.github/workflows/python-package-pr.yml`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install .[parquet,healpy,test]
+        pip install .[parquet,test,test_with_healpy]
     - name: Lint with flake8
       run: |
         flake8
     - name: Test with pytest
       run: |
         pip install mocpy
         pytest
```

### Comparing `healsparse-1.9.1/.github/workflows/python-package-publish.yml` & `healsparse-1.9.2/.github/workflows/python-package-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: "setup.cfg"
 
       - name: Build and install
         run: |
           python -m pip install --upgrade pip setuptools
-          python -m pip install .[parquet,healpy,test]
+          python -m pip install .[parquet,test,test_with_healpy]
       - name: Run tests
         run: |
           cd tests
           pytest
 
   pypi_build:
     runs-on: ubuntu-latest
```

### Comparing `healsparse-1.9.1/.github/workflows/python-package-push.yml` & `healsparse-1.9.2/.github/workflows/python-package-push.yml`

 * *Files 26% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install .[parquet,healpy,test]
+        python -m pip install .[parquet,test,test_with_healpy]
     - name: Lint with flake8
       run: |
         flake8
     - name: Test with pytest
       run: |
         pip install mocpy
         pytest
```

### Comparing `healsparse-1.9.1/CHANGES.md` & `healsparse-1.9.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/LICENSE` & `healsparse-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/PKG-INFO` & `healsparse-1.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.9.1
+Version: 1.9.2
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and the Dark Energy Science Collaboration
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
@@ -24,16 +24,16 @@
 Requires-Dist: hpgeom>=1.2.0
 Requires-Dist: astropy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Provides-Extra: parquet
 Requires-Dist: pyarrow>=5.0.0; extra == "parquet"
-Provides-Extra: healpy
-Requires-Dist: healpy; extra == "healpy"
+Provides-Extra: test-with-healpy
+Requires-Dist: healpy; extra == "test-with-healpy"
 Provides-Extra: fitsio
 Requires-Dist: fitsio; extra == "fitsio"
 
 # `healsparse`
 Python implementation of sparse HEALPix maps.
 
 `HealSparse` is a sparse implementation of
```

### Comparing `healsparse-1.9.1/README.md` & `healsparse-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/api_changes_to_1.0.md` & `healsparse-1.9.2/api_changes_to_1.0.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/Makefile` & `healsparse-1.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/basic_interface.rst` & `healsparse-1.9.2/docs/basic_interface.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/concatenation.rst` & `healsparse-1.9.2/docs/concatenation.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/conf.py` & `healsparse-1.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/filespec.rst` & `healsparse-1.9.2/docs/filespec.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/geometry.rst` & `healsparse-1.9.2/docs/geometry.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/index.rst` & `healsparse-1.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/install.rst` & `healsparse-1.9.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/make.bat` & `healsparse-1.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/modules.rst` & `healsparse-1.9.2/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/operations.rst` & `healsparse-1.9.2/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/docs/randoms.rst` & `healsparse-1.9.2/docs/randoms.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/__init__.py` & `healsparse-1.9.2/healsparse/__init__.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/cat_healsparse_files.py` & `healsparse-1.9.2/healsparse/cat_healsparse_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/fits_shim.py` & `healsparse-1.9.2/healsparse/fits_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/geom.py` & `healsparse-1.9.2/healsparse/geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/healSparseCoverage.py` & `healsparse-1.9.2/healsparse/healSparseCoverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/healSparseMap.py` & `healsparse-1.9.2/healsparse/healSparseMap.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/healSparseRandoms.py` & `healsparse-1.9.2/healsparse/healSparseRandoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/io_coverage.py` & `healsparse-1.9.2/healsparse/io_coverage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import pathlib
 
 from .fits_shim import HealSparseFits
 from .io_coverage_fits import _read_coverage_fits
 from .io_coverage_parquet import _read_coverage_parquet
 from .parquet_shim import check_parquet_dataset
 
 
@@ -26,14 +27,17 @@
     -------
     cov_map : `HealSparseCoverage`
         HealSparseCoverage map from file.
     """
     is_fits = False
     is_parquet_file = False
 
+    if isinstance(filename_or_fits, pathlib.PurePath):
+        filename_or_fits = os.fspath(filename_or_fits)
+
     if isinstance(filename_or_fits, str):
         try:
             fits = HealSparseFits(filename_or_fits)
             is_fits = True
             fits.close()
         except OSError:
             is_fits = False
```

### Comparing `healsparse-1.9.1/healsparse/io_coverage_fits.py` & `healsparse-1.9.2/healsparse/io_coverage_fits.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/io_coverage_parquet.py` & `healsparse-1.9.2/healsparse/io_coverage_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/io_map.py` & `healsparse-1.9.2/healsparse/io_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/io_map_fits.py` & `healsparse-1.9.2/healsparse/io_map_fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,36 +86,39 @@
             )
             if hdr['ORDERING'] == 'RING':
                 _pix = hpg.ring_to_nest(hdr['NSIDE'], data['PIXEL'])
             else:
                 _pix = data['PIXEL']
             healsparse_map[_pix] = data[signal_column]
         elif hdr['INDXSCHM'].rstrip() == 'IMPLICIT':
-            try:
-                import healpy as hp
-            except ImportError:
-                raise RuntimeError("Cannot read full sky HEALPix maps without healpy.")
-            # This is an implicit (full) healpix map
-            # Figure out the datatype
             with HealSparseFits(filename) as fits:
-                row = fits.read_ext_data(1, row_range=[0, 1])
-                dtype = row[0][0][0].dtype.type
+                data = fits.read_ext_data(1)
+                if "T" in data.dtype.names:
+                    field_name = "T"
+                elif "TEMPERATURE" in data.dtype.names:
+                    field_name = "TEMPERATURE"
+                else:
+                    raise RuntimeError("Healpix file does not comply with standards.")
+
+            # Ravel the data into one contiguous array.
+            data = data[field_name].ravel()
+
+            if hdr["ORDERING"] == "RING":
+                data = hpg.reorder(data, ring_to_nest=True)
 
-            # Read in the map using healpy
-            healpix_map = hp.read_map(filename, nest=True, dtype=dtype)
             # Convert to healsparse format
-            healsparse_map = healsparse_class(healpix_map=healpix_map,
+            healsparse_map = healsparse_class(healpix_map=data,
                                               nside_coverage=nside_coverage,
                                               nest=True)
         else:
             raise ValueError(f"Illegal value for INDXSCHM: {hdr['INDXSCHM']}")
 
         if degrade_nside is not None:
             # Degrade this map.  Note that this could not be done on read
-            # because healpy maps do not have that functionality.
+            # because healpix maps do not have that functionality.
             healsparse_map = healsparse_map.degrade(degrade_nside, reduction=reduction)
 
         if header:
             return (healsparse_map, hdr)
         else:
             return healsparse_map
     elif 'PIXTYPE' in hdr and hdr['PIXTYPE'].rstrip() == 'HEALSPARSE':
```

### Comparing `healsparse-1.9.1/healsparse/io_map_healpix.py` & `healsparse-1.9.2/healsparse/io_map_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/io_map_parquet.py` & `healsparse-1.9.2/healsparse/io_map_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/operations.py` & `healsparse-1.9.2/healsparse/operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/packedBoolArray.py` & `healsparse-1.9.2/healsparse/packedBoolArray.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/parquet_shim.py` & `healsparse-1.9.2/healsparse/parquet_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse/utils.py` & `healsparse-1.9.2/healsparse/utils.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/healsparse.egg-info/PKG-INFO` & `healsparse-1.9.2/healsparse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.9.1
+Version: 1.9.2
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and the Dark Energy Science Collaboration
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
@@ -24,16 +24,16 @@
 Requires-Dist: hpgeom>=1.2.0
 Requires-Dist: astropy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Provides-Extra: parquet
 Requires-Dist: pyarrow>=5.0.0; extra == "parquet"
-Provides-Extra: healpy
-Requires-Dist: healpy; extra == "healpy"
+Provides-Extra: test-with-healpy
+Requires-Dist: healpy; extra == "test-with-healpy"
 Provides-Extra: fitsio
 Requires-Dist: fitsio; extra == "fitsio"
 
 # `healsparse`
 Python implementation of sparse HEALPix maps.
 
 `HealSparse` is a sparse implementation of
```

### Comparing `healsparse-1.9.1/healsparse.egg-info/SOURCES.txt` & `healsparse-1.9.2/healsparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/long_description.md` & `healsparse-1.9.2/long_description.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/setup.cfg` & `healsparse-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [options.extras_require]
 test = 
 	pytest
 	flake8
 parquet = 
 	pyarrow>=5.0.0
-healpy = 
+test_with_healpy = 
 	healpy
 fitsio = 
 	fitsio
 
 [options.packages.find]
 exclude = 
 	tests
```

### Comparing `healsparse-1.9.1/tests/test_applymask.py` & `healsparse-1.9.2/tests/test_applymask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_astype.py` & `healsparse-1.9.2/tests/test_astype.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_boolean_operations.py` & `healsparse-1.9.2/tests/test_boolean_operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_buildmaps.py` & `healsparse-1.9.2/tests/test_buildmaps.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_cat_files.py` & `healsparse-1.9.2/tests/test_cat_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_coverage_map.py` & `healsparse-1.9.2/tests/test_coverage_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_coverage_mask.py` & `healsparse-1.9.2/tests/test_coverage_mask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_degrade.py` & `healsparse-1.9.2/tests/test_degrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_emptypixels.py` & `healsparse-1.9.2/tests/test_emptypixels.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_fits_shim.py` & `healsparse-1.9.2/tests/test_fits_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_fracdet_map.py` & `healsparse-1.9.2/tests/test_fracdet_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_from_healpix.py` & `healsparse-1.9.2/tests/test_from_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_generate_healpix.py` & `healsparse-1.9.2/tests/test_generate_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_geom.py` & `healsparse-1.9.2/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_getset.py` & `healsparse-1.9.2/tests/test_getset.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_healSparseCoverage.py` & `healsparse-1.9.2/tests/test_healSparseCoverage.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy.testing as testing
 import numpy as np
 import hpgeom as hpg
 import tempfile
 import shutil
 import os
 import pytest
+import pathlib
 
 import healsparse
 
 try:
     import healpy as hp
     has_healpy = True
 except ImportError:
@@ -36,23 +37,24 @@
 
         # Generate a coverage mask from the 0: 20000
         cov_mask_test = np.zeros(hpg.nside_to_npixel(nside_coverage), dtype=np.bool_)
         ra, dec = hpg.pixel_to_angle(nside_map, np.arange(20000))
         ipnest = np.unique(hpg.angle_to_pixel(nside_coverage, ra, dec))
         cov_mask_test[ipnest] = True
 
-        cov_map = healsparse.HealSparseCoverage.read(fname)
+        for readfile in (fname, pathlib.Path(fname)):
+            cov_map = healsparse.HealSparseCoverage.read(readfile)
 
-        # Ensure that the coverage mask is what we think it should be
-        testing.assert_array_equal(cov_map.coverage_mask, cov_mask_test)
+            # Ensure that the coverage mask is what we think it should be
+            testing.assert_array_equal(cov_map.coverage_mask, cov_mask_test)
 
-        # Ensure that we can address the cov_map by index
-        testing.assert_array_equal(cov_map[:], cov_map._cov_index_map)
-        testing.assert_array_equal(cov_map[0: 100], cov_map._cov_index_map[0: 100])
-        testing.assert_array_equal([cov_map[0]], [cov_map._cov_index_map[0]])
+            # Ensure that we can address the cov_map by index
+            testing.assert_array_equal(cov_map[:], cov_map._cov_index_map)
+            testing.assert_array_equal(cov_map[0: 100], cov_map._cov_index_map[0: 100])
+            testing.assert_array_equal([cov_map[0]], [cov_map._cov_index_map[0]])
 
         if not has_healpy:
             return
 
         # Make a healpy file and make sure we can't read it
         test_map = np.zeros(hpg.nside_to_npixel(nside_coverage))
         fname = os.path.join(self.test_dir, 'healpy_map_test.fits')
@@ -80,41 +82,44 @@
 
         # Generate a coverage mask from the 0: 20000
         cov_mask_test = np.zeros(hpg.nside_to_npixel(nside_coverage), dtype=np.bool_)
         ra, dec = hpg.pixel_to_angle(nside_map, np.arange(20000))
         ipnest = np.unique(hpg.angle_to_pixel(nside_coverage, ra, dec))
         cov_mask_test[ipnest] = True
 
-        cov_map = healsparse.HealSparseCoverage.read(fname)
+        for readfile in (fname, pathlib.Path(fname)):
+            cov_map = healsparse.HealSparseCoverage.read(fname)
 
-        # Ensure that the coverage mask is what we think it should be
-        testing.assert_array_equal(cov_map.coverage_mask, cov_mask_test)
+            # Ensure that the coverage mask is what we think it should be
+            testing.assert_array_equal(cov_map.coverage_mask, cov_mask_test)
 
-        # Ensure that we can address the cov_map by index
-        testing.assert_array_equal(cov_map[:], cov_map._cov_index_map)
-        testing.assert_array_equal(cov_map[0: 100], cov_map._cov_index_map[0: 100])
-        testing.assert_array_equal([cov_map[0]], [cov_map._cov_index_map[0]])
+            # Ensure that we can address the cov_map by index
+            testing.assert_array_equal(cov_map[:], cov_map._cov_index_map)
+            testing.assert_array_equal(cov_map[0: 100], cov_map._cov_index_map[0: 100])
+            testing.assert_array_equal([cov_map[0]], [cov_map._cov_index_map[0]])
 
     def test_read_non_fits(self):
         """Test reading coverage from a file that isn't fits or parquet."""
         self.test_dir = tempfile.mkdtemp(dir='./', prefix='TestHealSparse-')
 
         fname = os.path.join(self.test_dir, 'NOT_A_FITS_FILE')
         with open(fname, 'w') as f:
             f.write('some text.')
 
         self.assertRaises(NotImplementedError, healsparse.HealSparseCoverage.read, fname)
+        self.assertRaises(NotImplementedError, healsparse.HealSparseCoverage.read, pathlib.Path(fname))
 
     def test_read_missing_file(self):
         """Test reading coverage from a file that isn't there."""
         self.test_dir = tempfile.mkdtemp(dir='./', prefix='TestHealSparse-')
 
         fname = os.path.join(self.test_dir, 'NOT_A_FILE')
 
         self.assertRaises(IOError, healsparse.HealSparseCoverage.read, fname)
+        self.assertRaises(IOError, healsparse.HealSparseCoverage.read, pathlib.Path(fname))
 
     def setUp(self):
         self.test_dir = None
 
     def tearDown(self):
         if self.test_dir is not None:
             if os.path.exists(self.test_dir):
```

### Comparing `healsparse-1.9.1/tests/test_healpix_io.py` & `healsparse-1.9.2/tests/test_healpix_io.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_interpolation.py` & `healsparse-1.9.2/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_io.py` & `healsparse-1.9.2/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy.testing as testing
 import numpy as np
 import hpgeom as hpg
 from numpy import random
 import tempfile
 import shutil
 import os
+import pathlib
 
 import healsparse
 
 
 class HealsparseFitsIoTestCase(unittest.TestCase):
     def test_fits_writeread(self):
         """
@@ -35,54 +36,56 @@
         test_values = full_map[ipnest]
 
         # Test that we can do a basic set
         sparse_map = healsparse.HealSparseMap(healpix_map=full_map, nside_coverage=nside_coverage, nest=True)
 
         sparse_map[30000: 30005] = np.zeros(5, dtype=np.float64)
 
-        # Write it to healsparse format
-        sparse_map.write(os.path.join(self.test_dir, 'healsparse_map.hs'))
-
-        # Read in healsparse format (full map)
-        sparse_map = healsparse.HealSparseMap.read(os.path.join(self.test_dir, 'healsparse_map.hs'))
-
-        # Check that we can do a basic lookup
-        testing.assert_almost_equal(sparse_map.get_values_pix(ipnest), test_values)
-
-        # Check that we can do a basic set
-        sparse_map[30000: 30005] = np.zeros(5, dtype=np.float64)
-
-        # Try to read in healsparse format, non-unique pixels
-        self.assertRaises(RuntimeError, healsparse.HealSparseMap.read,
-                          os.path.join(self.test_dir, 'healsparse_map.hs'), pixels=[0, 0])
-
-        # Read in healsparse format (two pixels)
-        sparse_map_small = healsparse.HealSparseMap.read(os.path.join(self.test_dir,
-                                                                      'healsparse_map.hs'),
-                                                         pixels=[0, 1])
-
-        # Test the coverage map only has two pixels
-        cov_mask = sparse_map_small.coverage_mask
-        self.assertEqual(cov_mask.sum(), 2)
-
-        # Test lookup of values in those two pixels
-        ipnestCov = np.right_shift(ipnest, sparse_map_small._cov_map.bit_shift)
-        outside_small, = np.where(ipnestCov > 1)
-        test_values2 = test_values.copy()
-        test_values2[outside_small] = hpg.UNSEEN
-
-        testing.assert_almost_equal(sparse_map_small.get_values_pix(ipnest), test_values2)
-
-        # Read in healsparse format (all pixels)
-        sparse_map_full = healsparse.HealSparseMap.read(
-            os.path.join(self.test_dir,
-                         'healsparse_map.hs'),
-            pixels=np.arange(hpg.nside_to_npixel(nside_coverage))
-        )
-        testing.assert_almost_equal(sparse_map_full.get_values_pix(ipnest), test_values)
+        for mode in ("str", "path"):
+            if mode == "str":
+                readfile = os.path.join(self.test_dir, "healsparse_map.hsp")
+            else:
+                readfile = self.test_dir / pathlib.Path("healsparse_map2.hsp")
+
+            # Write it to healsparse format
+            sparse_map.write(readfile)
+
+            # Read in healsparse format (full map)
+            sparse_map = healsparse.HealSparseMap.read(readfile)
+
+            # Check that we can do a basic lookup
+            testing.assert_almost_equal(sparse_map.get_values_pix(ipnest), test_values)
+
+            # Check that we can do a basic set
+            sparse_map[30000: 30005] = np.zeros(5, dtype=np.float64)
+
+            # Try to read in healsparse format, non-unique pixels
+            self.assertRaises(RuntimeError, healsparse.HealSparseMap.read, readfile, pixels=[0, 0])
+
+            # Read in healsparse format (two pixels)
+            sparse_map_small = healsparse.HealSparseMap.read(readfile, pixels=[0, 1])
+
+            # Test the coverage map only has two pixels
+            cov_mask = sparse_map_small.coverage_mask
+            self.assertEqual(cov_mask.sum(), 2)
+
+            # Test lookup of values in those two pixels
+            ipnestCov = np.right_shift(ipnest, sparse_map_small._cov_map.bit_shift)
+            outside_small, = np.where(ipnestCov > 1)
+            test_values2 = test_values.copy()
+            test_values2[outside_small] = hpg.UNSEEN
+
+            testing.assert_almost_equal(sparse_map_small.get_values_pix(ipnest), test_values2)
+
+            # Read in healsparse format (all pixels)
+            sparse_map_full = healsparse.HealSparseMap.read(
+                readfile,
+                pixels=np.arange(hpg.nside_to_npixel(nside_coverage)),
+            )
+            testing.assert_almost_equal(sparse_map_full.get_values_pix(ipnest), test_values)
 
     def test_fits_read_outoforder(self):
         """
         Test reading fits maps that have been written with out-of-order pixels
         """
         random.seed(seed=12345)
```

### Comparing `healsparse-1.9.1/tests/test_io_parquet.py` & `healsparse-1.9.2/tests/test_io_parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import hpgeom as hpg
 from numpy import random
 import tempfile
 import shutil
 import os
 import pytest
+import pathlib
 
 import healsparse
 
 
 if not healsparse.parquet_shim.use_pyarrow:
     pytest.skip("Skipping pyarrow/parquet tests", allow_module_level=True)
 
@@ -41,49 +42,53 @@
 
         sparse_map = healsparse.HealSparseMap.make_empty(nside_coverage,
                                                          nside_map,
                                                          full_map.dtype)
         u, = np.where(full_map > hpg.UNSEEN)
         sparse_map[u] = full_map[u]
 
-        fname = os.path.join(self.test_dir, 'healsparse_map.hsparquet')
-
-        # Write it in healsparse parquet format
-        sparse_map.write(fname, format='parquet')
-
-        # Read in healsparse format (full map)
-        sparse_map = healsparse.HealSparseMap.read(fname)
-        # Check that we can do a basic lookup
-        testing.assert_almost_equal(sparse_map.get_values_pix(ipnest), test_values)
-
-        # Try to read in healsparse format, non-unique pixels
-        self.assertRaises(RuntimeError, healsparse.HealSparseMap.read,
-                          fname, pixels=[0, 0])
-
-        # Read in healsparse (two pixels)
-        sparse_map_small = healsparse.HealSparseMap.read(fname, pixels=[0, 1])
-
-        # Test the coverage map only has two pixels
-        cov_mask = sparse_map_small.coverage_mask
-        self.assertEqual(cov_mask.sum(), 2)
-
-        # Test lookup of values in those two pixels
-        ipnestCov = np.right_shift(ipnest, sparse_map_small._cov_map.bit_shift)
-        outside_small, = np.where(ipnestCov > 1)
-        test_values2 = test_values.copy()
-        test_values2[outside_small] = hpg.UNSEEN
-
-        testing.assert_almost_equal(sparse_map_small.get_values_pix(ipnest), test_values2)
-
-        # Read in healsparse format (all pixels)
-        sparse_map_full = healsparse.HealSparseMap.read(
-            fname,
-            pixels=np.arange(hpg.nside_to_npixel(nside_coverage))
-        )
-        testing.assert_almost_equal(sparse_map_full.get_values_pix(ipnest), test_values)
+        for mode in ("str", "path"):
+            if mode == "str":
+                readfile = os.path.join(self.test_dir, "healsparse_map.hsparquet")
+            else:
+                readfile = self.test_dir / pathlib.Path("healsparse_map2.hsparquet")
+
+                # Write it in healsparse parquet format
+                sparse_map.write(readfile, format="parquet")
+
+                # Read in healsparse format (full map)
+                sparse_map = healsparse.HealSparseMap.read(readfile)
+                # Check that we can do a basic lookup
+                testing.assert_almost_equal(sparse_map.get_values_pix(ipnest), test_values)
+
+                # Try to read in healsparse format, non-unique pixels
+                self.assertRaises(RuntimeError, healsparse.HealSparseMap.read,
+                                  readfile, pixels=[0, 0])
+
+                # Read in healsparse (two pixels)
+                sparse_map_small = healsparse.HealSparseMap.read(readfile, pixels=[0, 1])
+
+                # Test the coverage map only has two pixels
+                cov_mask = sparse_map_small.coverage_mask
+                self.assertEqual(cov_mask.sum(), 2)
+
+                # Test lookup of values in those two pixels
+                ipnestCov = np.right_shift(ipnest, sparse_map_small._cov_map.bit_shift)
+                outside_small, = np.where(ipnestCov > 1)
+                test_values2 = test_values.copy()
+                test_values2[outside_small] = hpg.UNSEEN
+
+                testing.assert_almost_equal(sparse_map_small.get_values_pix(ipnest), test_values2)
+
+                # Read in healsparse format (all pixels)
+                sparse_map_full = healsparse.HealSparseMap.read(
+                    readfile,
+                    pixels=np.arange(hpg.nside_to_npixel(nside_coverage)),
+                )
+                testing.assert_almost_equal(sparse_map_full.get_values_pix(ipnest), test_values)
 
     def test_parquet_read_outoforder(self):
         """
         Test reading parquet maps that have been written with out-of-order pixels
         """
         random.seed(seed=12345)
```

### Comparing `healsparse-1.9.1/tests/test_lookup.py` & `healsparse-1.9.2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_metadata.py` & `healsparse-1.9.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_moc.py` & `healsparse-1.9.2/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_operations.py` & `healsparse-1.9.2/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_packedboolarray.py` & `healsparse-1.9.2/tests/test_packedboolarray.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_pixel_ranges.py` & `healsparse-1.9.2/tests/test_pixel_ranges.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_randoms.py` & `healsparse-1.9.2/tests/test_randoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_recarray.py` & `healsparse-1.9.2/tests/test_recarray.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_single_covpix.py` & `healsparse-1.9.2/tests/test_single_covpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_single_datatypes.py` & `healsparse-1.9.2/tests/test_single_datatypes.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_singlevalues.py` & `healsparse-1.9.2/tests/test_singlevalues.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_update_values.py` & `healsparse-1.9.2/tests/test_update_values.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_upgrade.py` & `healsparse-1.9.2/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_validarea.py` & `healsparse-1.9.2/tests/test_validarea.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tests/test_widemasks.py` & `healsparse-1.9.2/tests/test_widemasks.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.9.1/tutorial/quickstart.ipynb` & `healsparse-1.9.2/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

