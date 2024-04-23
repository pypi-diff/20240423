# Comparing `tmp/pypoolparty-0.0.8.tar.gz` & `tmp/pypoolparty-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypoolparty-0.0.8.tar", last modified: Wed Jan 31 15:43:55 2024, max compression
+gzip compressed data, was "pypoolparty-0.2.1.tar", last modified: Tue Apr 23 11:52:17 2024, max compression
```

## Comparing `pypoolparty-0.0.8.tar` & `pypoolparty-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.588175 pypoolparty-0.0.8/pypoolparty/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/job_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/making_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/proto_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/pypoolparty/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/organizing_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.588175 pypoolparty-0.0.8/pypoolparty/slurm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/dummy_queue_state.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1314 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/dummy_sbatch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/dummy_scancel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2493 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/dummy_squeue.py
--rw-r--r--   0 runner    (1001) docker     (127)   100767 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/squeue_format_all.stdout
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/organizing_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.588175 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/resources/dummy_qdel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3366 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/resources/dummy_qstat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1454 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/resources/dummy_qsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pypoolparty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/pypoolparty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-01-31 15:43:55.000000 pypoolparty-0.0.8/pypoolparty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-01-31 15:43:55.000000 pypoolparty-0.0.8/pypoolparty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 15:43:55.000000 pypoolparty-0.0.8/pypoolparty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-31 15:43:55.000000 pypoolparty-0.0.8/pypoolparty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-31 15:43:55.000000 pypoolparty-0.0.8/pypoolparty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 15:43:55.592175 pypoolparty-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-31 15:43:46.000000 pypoolparty-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.454551 pypoolparty-0.2.1/pypoolparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/job_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/making_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/proto_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.454551 pypoolparty-0.2.1/pypoolparty/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.454551 pypoolparty-0.2.1/pypoolparty/slurm/array/
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/making_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/reducing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/array/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/organizing_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.450551 pypoolparty-0.2.1/pypoolparty/slurm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/dummy_queue_state.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2986 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/dummy_sbatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/dummy_scancel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4080 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/dummy_squeue.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100767 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/squeue_format_all.stdout
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/organizing_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.450551 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      708 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/dummy_qdel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3844 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/dummy_qstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1432 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/dummy_qsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pypoolparty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/pypoolparty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-23 11:52:17.000000 pypoolparty-0.2.1/pypoolparty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-23 11:52:17.000000 pypoolparty-0.2.1/pypoolparty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:52:17.000000 pypoolparty-0.2.1/pypoolparty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:52:17.000000 pypoolparty-0.2.1/pypoolparty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 11:52:17.000000 pypoolparty-0.2.1/pypoolparty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:52:17.458551 pypoolparty-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-23 11:52:13.000000 pypoolparty-0.2.1/setup.py
```

### Comparing `pypoolparty-0.0.8/LICENSE` & `pypoolparty-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/PKG-INFO` & `pypoolparty-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypoolparty
-Version: 0.0.8
+Version: 0.2.1
 Summary: A job pool for distributed compute clusters inspired by python's multoprocessing.Pool.
 Home-page: https://github.com/cherenkov-plenoscope/pypoolparty
 Author: Sebastian Achim Mueller
 Author-email: sebastian-achim.mueller@mpi-hd.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,24 +17,26 @@
 
 #################
 Python Pool Party
 #################
 |TestStatus| |PyPiStatus| |BlackStyle| |BlackPackStyle| |MITLicenseBadge|
 
 A python package for job pools (as in ``multiprocessing.Pool()``) which makes
-use of distributed compute clusters.
+use of workload managers on distributed compute clusters.
 
 The ``pypoolparty`` provides a ``Pool()`` with a ``map()`` function which aims
-to be a drop-in-replacement for ``builtins``' ``map()``, and ``multiprocessing.Pool()``'s ``map()``. The idea is to allow the user to always fall back to these builtin pools and map-functions in case a distributed compute cluster is not available.
+to be a drop-in-replacement for ``multiprocessing.Pool()``'s ``map()``.
+This way you can always fall back to the builtin pools and map-functions
+in case a distributed compute cluster is not available.
 
 This package respects the concept of 'fair share' what is commonly found
 in scientific environments, but is not common in commercial environments.
 Here, fair share means that compute resources are only requested when they
 are needed. Compute resources are not requested to just idle and wait for
-the user to submit jobs.
+jobs to be submitted.
 
 A consequence of this fair sharing is, that this package expects your jobs
 to randomly die in conflicts for resources with jobs submitted by other users,
 such as conflicts for limited disk space on temporary drives. If your jobs run
 into error states, they will be resubmitted until a predefined limit is
 reached.
 
@@ -48,43 +50,110 @@
 
 
 Basic Usage
 ===========
 
 .. code:: python
 
-    import pypoolparty as ppp
+    import pypoolparty
 
-    pool = ppp.slurm.Pool()
+    pool = pypoolparty.slurm.array.Pool()
     results = pool.map(sum, [[1, 2], [2, 3], [4, 5], ])
 
 
-Currently, there is ``ppp.slurm.Pool()`` and ``ppp.sun_grid_engine.Pool()``.
+For more details, see the ``Pool()'s`` docs, e.g. ``pypoolparty.slurm.array.Pool?``.
+Options to the ``Pool()s`` are defined in therir constructors e.g.
+
+
+.. code:: python
+
+    pool = pypoolparty.slurm.array.Pool(
+        num_simultaneously_running_tasks=200,
+        python_path="/path/to/python/interpreter/to/be/called/on/the/worker/nodes",
+        polling_interval=5.0,
+        work_dir="/path/to/the/pools/work_dir/where/the/map/and/reduce/happens",
+        keep_work_dir=True,  # e.g for debugging
+        verbose=True,  # Talk to me!
+        slurm_call_timeout=60.0,
+        max_num_resubmissions=3,
+    )
+
+
+Pools
+=====
+
+``pypoolparty.slurm.array.Pool()``
+----------------------------------
+Uses slurm's ``--array`` option.
+It will call ``sbatch --array``, ``squeue`` and ``scancel``.
+
+``pypoolparty.sun_grid_engine.Pool()``
+--------------------------------------
+It will call ``qsub``, ``qstat`` and ``qdel``.
+
+``pypoolparty.slurm.Pool()``
+----------------------------
+It will call ``sbatch``, ``squeue`` and ``scancel``.
+Uses the same inner workings as ``pypoolparty.sun_grid_engine.Pool()``.
+
+Testing
+=======
+The ``pypoolparty`` comes with ist own dummys for slurm and the sun grid engine.
+This allows to test the full chain without the actual workload managers to be installed.
+
+.. code:: bash
+
+    pytest -s pypoolparty
+
+
+Workload managers
+=================
+We tested:
+
+- SLURM, version 22.05.6
+- Sun Grid Engine (SGE), version 8.1.9
 
 
 Alternatives
 ============
 When you do not share resources with other users, when you do not need to respect fair share, and when you have some administrative power you might want to use one of these:
 
 - Dask_ has a ``job_queue`` which also supports other flavors such as PBS, SLURM.
 
 - pyABC.sge_ has a ``pool.map()`` very much like the one in this package.
 
 - ipyparallel_
 
 
-Queue Flavors
-=============
+Inner Workings
+==============
+The maaping and reducing takes place in a ``work_dir`` in the filesystem.
+The ``work_dir`` can be defined manually and must be reachable by all
+compute notes.
 
-- SLURM, version 22.05.6
-- Sun Grid Engine (SGE), version 8.1.9
+``slurm.array.Pool``
+--------------------
+- Makes a ``work_dir`` where it creates a zip-file named ``tasks.zip`` in which it dumps all ``tasks`` using ``pickle``.
 
+- Starts a logger which logs into a file named ``log.jsonl`` in the ``work_dir``.
+
+- Makea a script which will execute the tasks on the compute nodes and dumps the script named ``script.py`` into the ``work_dir``. The script contains the path to the ``work_dir`` and queries the environment variable ``SLURM_ARRAY_TASK_ID`` to determine which ``task`` it shall process. It will write its result, ``stdout`` and ``stderr``, and potentially a report of raised ``exceptions`` into the ``work_dir``.
+
+- Calls ``sbatch --array``
+
+- After the initial call of ``sbatch``, we wait for the jobs to return (to write their results) or to get stuck in some error state. With a polling interval of 5s (can be adjusted), the ``work_dir`` is searched for results and ``squeue`` is searched for jobs in error states. When results are found in the ``work_dir``, they are read and appended into the four zip-files named ``tasks.results.zip``, ``tasks.stdout.zip``, ``tasks.stderr.zip``, and ``tasks.exceptions.zip``. When the individual files writen by a job got appended to the zip-files, the individual files are removed to keep the number of files low.
+
+- If the poll of ``squeue`` indicates ``tasks`` with error like flags, these specific ``tasks`` will be removed from the queue by calling ``scancel`` and then added again by calling ``sbatch --array`` until a predefined limit of resubmissions is reached.
+
+- Finally, either all ``tasks`` returned results or got finally stuck in errors and exceptions. The results are read into memory from ``work_dir/tasks_results.zip`` and returned by the ``map()`` function. If there was non zero ``stderr`` or an exception, the ``work_dir`` will not be removed after the call of ``map()``, but will stay for potential debugging.
+
+
+``sun_grid_engine.Pool`` and ``slurm.Pool``
+-------------------------------------------
 
-Inner Workings
-==============
 - ``map()`` makes a ``work_dir`` because the mapping and reducing takes place in the filesystem. You can set ``work_dir`` manually to make sure both the worker nodes and the process node can reach it.
 
 - ``map()`` serializes your ``tasks`` using ``pickle`` into separate files in ``work_dir/{ichunk:09d}.pkl``.
 
 - ``map()`` reads all environment variables in its process.
 
 - ``map()`` creates the worker-node script in ``work_dir/worker_node_script.py``. It contains and exports the process' environment variables into the batch job's context. It reads the chunk of tasks in ``work_dir/{ichunk:09d}.pkl``, imports and runs your ``func(task)``, and finally writes the result back to ``work_dir/{ichunk:09d}.pkl.out``.
@@ -122,53 +191,37 @@
 - ``ichunk`` is the index of a chunk. It is used to create the chunks's filenames such as ``work_dir/{ichunk:09d}.pkl``.
 
 - `queue-job` is what we submit into the queue. Each queue-job processes the tasks in a single chunk in series.
 
 - ``jobname`` or ``job["name"]`` is assigned to a queue job by our ``map()``. It is composed of our ``map()``'s session-id, and ``ichunk``. E.g. ``"q"%Y-%m-%dT%H:%M:%S"#{ichunk:09d}"``
 
 
-Testing
-=======
+Testing for developers
+======================
+The tests have an option ``--debug_dir`` which allows to make the otherwise
+temporary output and working directories to remain after the tests have run.
 
 .. code:: bash
 
-    pytest -s .
+    pytest -s --debug_dir path/to/do/debugging pypoolparty
 
 
 dummy queue
 -----------
 To test our ``map()`` we provide a dummy ``qsub``, ``qstat``, and ``qdel``
-for the sun-grid-engine.
+for the sun-grid-engine, and a dummy ``sbatch``, ``squeue``, and ``scancel``
+for slurm.
 These are individual ``python`` scripts which all act on a common state file
-in ``tests/resources/dummy_queue_state.json`` in order to fake the
-sun-grid-engine's queue.
-
-- ``dummy_qsub.py`` only appends queue jobs to the list of pending jobs in the state-file.
-
-- ``dummy_qdel.py`` only removes queue jobs from the state-file.
-
-- ``dummy_qstat.py`` does move the queue jobs from the pending to the running list, and does trigger the actual processing of the jobs. Each time ``dummy_qstat.py`` is called it performs a single action on the state file. So it must be called multiple times to process all jobs. It can intentionally bring jobs into the error-state when this is set in the state-file.
-
-Before running the dummy queue, its state file must be initialized:
-
-.. code:: python
-
-    from pypoolparty import sun_grid_engine
-
-    sun_grid_engine.testing.init_queue_state(
-        path="tests/resources/dummy_queue_state.json"
-    )
+named ``queue_state.json`` in order to imitate the workload managers.
 
-When testing our ``map()`` you set its arguments ``qsub_path``, ``qdel_path``,
-and ``qstat_path`` to point to the dummy queue.
+- ``qsub``/``sbatch`` only append pening jobs to the list of jobs in ``queue_state.json``.
 
-See ``tests/test_full_chain_with_dummy_qsub.py``.
+- ``qdel``/``scancel`` only remove jobs from the list of jobs in ``queue_state.json``.
 
-Because of the global state file, only one instance of dummy_queue must run
-at a time.
+- ``qstat``/``squeue`` changes  the state of jobs from pending to running, and triggers the actual processing of the jobs. Each time ``qstat.py`` is called it performs a single action on ``queue_state.json``. So it must be called multiple times to process all jobs. It can intentionally bring jobs into error states when this is set accordingly in the ``queue_state.json``.
 
 
 .. |TestStatus| image:: https://github.com/cherenkov-plenoscope/pypoolparty/actions/workflows/test.yml/badge.svg?branch=main
     :target: https://github.com/cherenkov-plenoscope/pypoolparty/actions/workflows/test.yml
 
 .. |PyPiStatus| image:: https://img.shields.io/pypi/v/pypoolparty
     :target: https://pypi.org/project/pypoolparty
```

### Comparing `pypoolparty-0.0.8/pypoolparty/chunking.py` & `pypoolparty-0.2.1/pypoolparty/chunking.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/debugging.py` & `pypoolparty-0.2.1/pypoolparty/debugging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 from . import utils
 import glob
 import os
 
 
+class SerialPool:
+    def __init__(self, verbose=True):
+        self.verbose = verbose
+
+    def map(self, func, iterable):
+        results = []
+        for i, item in enumerate(iterable):
+            print("SerialPool compute {:d} of {:d}".format(i, len(iterable)))
+            result = func(item)
+            results.append(result)
+        return results
+
+
 def list_ids(work_dir, wildcard, num_digits_jobid=9):
     paths = glob.glob(os.path.join(work_dir, wildcard))
     basenames = [os.path.basename(path) for path in paths]
     list_ids = [int(basename[0:num_digits_jobid]) for basename in basenames]
     return list_ids
```

### Comparing `pypoolparty-0.0.8/pypoolparty/job_counter.py` & `pypoolparty-0.2.1/pypoolparty/job_counter.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/making_script.py` & `pypoolparty-0.2.1/pypoolparty/making_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,24 +71,21 @@
     ----------
     environ : dict
         The envirionment variables to be set when the script is executed on the
         worker node.
     """
     env = io.StringIO()
     for key in environ:
+        value = environ[key]
         keydec = key.encode("unicode_escape").decode()
-        valdec = environ[key].encode("unicode_escape").decode()
 
         if '"' in keydec:
-            keytmpl = "os.environ['{key:s}']"
+            start = "os.environ['{key:s}']".format(key=keydec)
         else:
-            keytmpl = 'os.environ["{key:s}"]'
-        if '"' in valdec:
-            valtmpl = " = '{value:s}'\n"
-        else:
-            valtmpl = ' = "{value:s}"\n'
-        tmpl = keytmpl + valtmpl
+            start = 'os.environ["{key:s}"]'.format(key=keydec)
 
-        line = tmpl.format(key=keydec, value=valdec)
+        iiivalue = [int(b) for b in bytes(value, "utf8")]
+        stop = "bytes(" + str(iiivalue) + ").decode()" + "\n"
+        line = start + " = " + stop
         env.write(line)
     env.seek(0)
     return env.read()
```

### Comparing `pypoolparty-0.0.8/pypoolparty/pooling.py` & `pypoolparty-0.2.1/pypoolparty/pooling.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/proto_pool.py` & `pypoolparty-0.2.1/pypoolparty/proto_pool.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/slurm/__init__.py` & `pypoolparty-0.2.1/pypoolparty/slurm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from . import array
 from . import testing
-from . import call
+from . import calling
 from . import organizing_jobs
 from .. import proto_pool
 from .. import utils
 
 
 @utils.add_doc(
     proto_pool.Pool.__init__.__doc__
@@ -64,15 +65,15 @@
     stderr_path,
     logger,
     # slurm specific
     # --------------
     sbatch_path="sbatch",
     clusters=None,
 ):
-    return call.sbatch(
+    return calling.sbatch(
         script_path=script_path,
         script_arguments=script_arguments,
         stdout_path=stdout_path,
         stderr_path=stderr_path,
         jobname=jobname,
         logger=logger,
         clusters=clusters,
@@ -83,15 +84,15 @@
 def status(
     jobnames,
     logger,
     # slurm specific
     # --------------
     squeue_path,
 ):
-    all_jobs = call.squeue(
+    all_jobs = calling.squeue(
         squeue_path=squeue_path,
         logger=logger,
     )
     our_jobs = organizing_jobs.filter_jobs_by_jobnames(
         jobs=all_jobs,
         jobnames=jobnames,
     )
@@ -120,15 +121,15 @@
 def delete(
     job,
     logger,
     # slurm specific
     # --------------
     scancel_path,
 ):
-    return call.scancel(
+    return calling.scancel(
         jobname=job["name"],
         scancel_path=scancel_path,
         logger=logger,
     )
 
 
 def _make_job(slurm_job):
@@ -143,26 +144,40 @@
 
     example
     -------
         '''
         slurmstepd: error: *** JOB 123456 STEPD TERMINATED ON node12 AT
         1846-03-28T02:04:23 DUE TO JOB NOT ENDING WITH SIGNALS ***
         '''
+        and
+        '''
+        slurmstepd: error: slurm_get_node_energy: Socket timed out on send/recv operation
+        slurmstepd: error: _get_joules_task: can't get info from slurmd
+        '''
     """
     ends_with_newline = False
     if len(stderr) > 0:
         ends_with_newline = stderr[-1] == "\n"
 
+    slurm_foos = [
+        "DUE TO JOB NOT ENDING WITH SIGNALS",
+        "slurm_get_node_energy: Socket timed out on send/recv operation",
+        "_get_joules_task: can't get info from slurmd",
+    ]
+
     lines = str.splitlines(stderr)
     out = []
     for line in lines:
-        if (
-            "slurmstepd: error:" in line
-            and "DUE TO JOB NOT ENDING WITH SIGNALS" in line
-        ):
-            continue
-        out.append(line)
+        line_contains_slurm_foo = False
+
+        if "slurmstepd: error:" in line:
+            for slurm_foo in slurm_foos:
+                if slurm_foo in line:
+                    line_contains_slurm_foo = True
+
+        if not line_contains_slurm_foo:
+            out.append(line)
 
     out = str.join("\n", out)
     if ends_with_newline:
         out += "\n"
     return out
```

### Comparing `pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/dummy_scancel.py` & `pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/dummy_qdel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 #!/usr/bin/env python3
 import sys
 import json
 import datetime
-import pypoolparty
+from pypoolparty import sun_grid_engine
 
-qpaths = pypoolparty.slurm.testing.dummy_paths()
+queue_state_path = None  #  <- REQUIRED
 
-# dummy scancel
-# =============
-assert len(sys.argv) == 3
-assert sys.argv[1] == "--name"
-jobname = sys.argv[2]
+# dummy qdel
+# ==========
+assert len(sys.argv) == 2
+JB_job_number = sys.argv[1]
 
-with open(qpaths["queue_state"], "rt") as f:
+with open(queue_state_path, "rt") as f:
     old_state = json.loads(f.read())
 
 found = False
 state = {
-    "pending": [],
-    "running": [],
+    "jobs": [],
     "evil_jobs": old_state["evil_jobs"],
 }
-for job in old_state["running"]:
-    if job["NAME"] == jobname:
+for job in old_state["jobs"]:
+    if job["JB_job_number"] == JB_job_number:
         found = True
     else:
-        state["running"].append(job)
+        state["jobs"].append(job)
 
-for job in old_state["pending"]:
-    if job["NAME"] == jobname:
-        found = True
-    else:
-        state["pending"].append(job)
-
-with open(qpaths["queue_state"], "wt") as f:
+with open(queue_state_path, "wt") as f:
     f.write(json.dumps(state, indent=4))
 
 if found == True:
     sys.exit(0)
 else:
-    print("Can not find ", jobname)
+    print("Can not find ", JB_job_number)
     sys.exit(1)
```

### Comparing `pypoolparty-0.0.8/pypoolparty/slurm/tests/resources/squeue_format_all.stdout` & `pypoolparty-0.2.1/pypoolparty/slurm/tests/resources/squeue_format_all.stdout`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/sun_grid_engine/__init__.py` & `pypoolparty-0.2.1/pypoolparty/sun_grid_engine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import testing
-from . import call
+from . import calling
 from . import organizing_jobs
 from .. import proto_pool
 from .. import utils
 
 
 @utils.add_doc(
     proto_pool.Pool.__init__.__doc__
@@ -70,15 +70,15 @@
     logger,
     # sge specific
     # ------------
     qsub_path,
     queue_name,
     script_exe_path,
 ):
-    return call.qsub(
+    return calling.qsub(
         qsub_path=qsub_path,
         queue_name=queue_name,
         script_exe_path=script_exe_path,
         script_path=script_path,
         arguments=script_arguments,
         JB_name=jobname,
         stdout_path=stdout_path,
@@ -91,15 +91,15 @@
     jobnames,
     logger,
     # sge specific
     # ------------
     qstat_path,
     error_state_indicator,
 ):
-    all_jobs_running, all_jobs_pending = call.qstat(
+    all_jobs_running, all_jobs_pending = calling.qstat(
         qstat_path=qstat_path,
         logger=logger,
     )
     running, pending, error = organizing_jobs.get_jobs_running_pending_error(
         JB_names_set=jobnames,
         all_jobs_running=all_jobs_running,
         all_jobs_pending=all_jobs_pending,
@@ -122,15 +122,15 @@
 def delete(
     job,
     logger,
     # sge specific
     # ------------
     qdel_path,
 ):
-    return call.qdel(
+    return calling.qdel(
         JB_job_number=job["JB_job_number"],
         qdel_path=qdel_path,
         logger=logger,
     )
 
 
 def _make_job(sge_job):
```

### Comparing `pypoolparty-0.0.8/pypoolparty/sun_grid_engine/call.py` & `pypoolparty-0.2.1/pypoolparty/sun_grid_engine/calling.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/sun_grid_engine/organizing_jobs.py` & `pypoolparty-0.2.1/pypoolparty/sun_grid_engine/organizing_jobs.py`

 * *Files identical despite different names*

### Comparing `pypoolparty-0.0.8/pypoolparty/sun_grid_engine/tests/resources/dummy_qstat.py` & `pypoolparty-0.2.1/pypoolparty/sun_grid_engine/tests/resources/dummy_qstat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import sys
 import json
 import datetime
 import subprocess
 import pypoolparty
 
-qpaths = pypoolparty.sun_grid_engine.testing.dummy_paths()
+queue_state_path = None  #  <- REQUIRED
 
 
 def job_to_xml(job):
     jld = ""
     jld += '<job_list state="{:s}">\n'.format(job["@state"])
     jld += "    <JB_job_number>{:s}</JB_job_number>\n".format(
         job["JB_job_number"]
@@ -28,21 +28,23 @@
 
 
 def state_to_xml(state):
     out_xml = "<?xml version='1.0'?>\n"
     out_xml += "<job_info>\n"
 
     out_xml += "    <queue_info>\n"
-    for job in state["running"]:
-        out_xml += indent_text(job_to_xml(job), indent=8)
+    for job in state["jobs"]:
+        if job["@state"] == "running":
+            out_xml += indent_text(job_to_xml(job), indent=8)
     out_xml += "    </queue_info>\n"
 
     out_xml += "    <job_info>\n"
-    for job in state["pending"]:
-        out_xml += indent_text(job_to_xml(job), indent=8)
+    for job in state["jobs"]:
+        if job["@state"] != "running":
+            out_xml += indent_text(job_to_xml(job), indent=8)
     out_xml += "    </job_info>\n"
 
     out_xml += "</job_info>\n"
     return out_xml
 
 
 def indent_text(text, indent=4):
@@ -57,48 +59,63 @@
 # ===========
 # Every time this is called, it runs one job.
 MAX_NUM_RUNNING = 10
 
 assert len(sys.argv) == 2
 assert sys.argv[1] == "-xml"
 
-with open(qpaths["queue_state"], "rt") as f:
+with open(queue_state_path, "rt") as f:
     state = json.loads(f.read())
 
 evil_ichunks_num_fails = {}
 evil_ichunks_max_num_fails = {}
 for evil in state["evil_jobs"]:
     evil_ichunks_num_fails[evil["ichunk"]] = evil["num_fails"]
     evil_ichunks_max_num_fails[evil["ichunk"]] = evil["max_num_fails"]
 
 
-if len(state["running"]) >= MAX_NUM_RUNNING:
-    run_job = state["running"].pop(0)
+def count_jobs(jobs, state):
+    count = 0
+    for job in jobs:
+        if job["@state"] == state:
+            count += 1
+    return count
+
+
+def find_first_job(jobs, state):
+    for i in range(len(jobs)):
+        if jobs[i]["@state"] == state:
+            break
+    return i
+
+
+if count_jobs(state["jobs"], "running") >= MAX_NUM_RUNNING:
+    run_job = state["jobs"].pop(find_first_job(state["jobs"], "running"))
     pypoolparty.testing.dummy_run_job(run_job)
-elif len(state["pending"]) > 0:
-    job = state["pending"].pop(0)
+elif count_jobs(state["jobs"], "pending") > 0:
+    job = state["jobs"].pop(find_first_job(state["jobs"], "pending"))
     ichunk = pypoolparty.pooling.make_ichunk_from_jobname(
         jobname=job["JB_name"]
     )
     if ichunk in evil_ichunks_num_fails:
         if evil_ichunks_num_fails[ichunk] < evil_ichunks_max_num_fails[ichunk]:
-            job["@state"] = "?"
+            job["@state"] = "pending"
             job["state"] = "Eqw"
-            state["pending"].append(job)
+            state["jobs"].append(job)
             evil_ichunks_num_fails[ichunk] += 1
         else:
             job["@state"] = "running"
             job["state"] = "r"
-            state["running"].append(job)
+            state["jobs"].append(job)
     else:
         job["@state"] = "running"
         job["state"] = "r"
-        state["running"].append(job)
-elif len(state["running"]) > 0:
-    run_job = state["running"].pop(0)
+        state["jobs"].append(job)
+elif count_jobs(state["jobs"], "running") > 0:
+    run_job = state["jobs"].pop(find_first_job(state["jobs"], "running"))
     pypoolparty.testing.dummy_run_job(run_job)
 
 
 evil_jobs = []
 for ichunk in evil_ichunks_num_fails:
     evil_jobs.append(
         {
@@ -106,14 +123,14 @@
             "num_fails": evil_ichunks_num_fails[ichunk],
             "max_num_fails": evil_ichunks_max_num_fails[ichunk],
         }
     )
 state["evil_jobs"] = evil_jobs
 
 
-with open(qpaths["queue_state"], "wt") as f:
+with open(queue_state_path, "wt") as f:
     f.write(json.dumps(state, indent=4))
 
 out_xml = state_to_xml(state)
 print(out_xml)
 
 sys.exit(0)
```

### Comparing `pypoolparty-0.0.8/pypoolparty.egg-info/PKG-INFO` & `pypoolparty-0.2.1/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1
-Name: pypoolparty
-Version: 0.0.8
-Summary: A job pool for distributed compute clusters inspired by python's multoprocessing.Pool.
-Home-page: https://github.com/cherenkov-plenoscope/pypoolparty
-Author: Sebastian Achim Mueller
-Author-email: sebastian-achim.mueller@mpi-hd.mpg.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: qstat>=0.0.5
-Requires-Dist: json_line_logger
-Requires-Dist: rename_after_writing
-
 #################
 Python Pool Party
 #################
 |TestStatus| |PyPiStatus| |BlackStyle| |BlackPackStyle| |MITLicenseBadge|
 
 A python package for job pools (as in ``multiprocessing.Pool()``) which makes
-use of distributed compute clusters.
+use of workload managers on distributed compute clusters.
 
 The ``pypoolparty`` provides a ``Pool()`` with a ``map()`` function which aims
-to be a drop-in-replacement for ``builtins``' ``map()``, and ``multiprocessing.Pool()``'s ``map()``. The idea is to allow the user to always fall back to these builtin pools and map-functions in case a distributed compute cluster is not available.
+to be a drop-in-replacement for ``multiprocessing.Pool()``'s ``map()``.
+This way you can always fall back to the builtin pools and map-functions
+in case a distributed compute cluster is not available.
 
 This package respects the concept of 'fair share' what is commonly found
 in scientific environments, but is not common in commercial environments.
 Here, fair share means that compute resources are only requested when they
 are needed. Compute resources are not requested to just idle and wait for
-the user to submit jobs.
+jobs to be submitted.
 
 A consequence of this fair sharing is, that this package expects your jobs
 to randomly die in conflicts for resources with jobs submitted by other users,
 such as conflicts for limited disk space on temporary drives. If your jobs run
 into error states, they will be resubmitted until a predefined limit is
 reached.
 
@@ -48,43 +33,110 @@
 
 
 Basic Usage
 ===========
 
 .. code:: python
 
-    import pypoolparty as ppp
+    import pypoolparty
 
-    pool = ppp.slurm.Pool()
+    pool = pypoolparty.slurm.array.Pool()
     results = pool.map(sum, [[1, 2], [2, 3], [4, 5], ])
 
 
-Currently, there is ``ppp.slurm.Pool()`` and ``ppp.sun_grid_engine.Pool()``.
+For more details, see the ``Pool()'s`` docs, e.g. ``pypoolparty.slurm.array.Pool?``.
+Options to the ``Pool()s`` are defined in therir constructors e.g.
+
+
+.. code:: python
+
+    pool = pypoolparty.slurm.array.Pool(
+        num_simultaneously_running_tasks=200,
+        python_path="/path/to/python/interpreter/to/be/called/on/the/worker/nodes",
+        polling_interval=5.0,
+        work_dir="/path/to/the/pools/work_dir/where/the/map/and/reduce/happens",
+        keep_work_dir=True,  # e.g for debugging
+        verbose=True,  # Talk to me!
+        slurm_call_timeout=60.0,
+        max_num_resubmissions=3,
+    )
+
+
+Pools
+=====
+
+``pypoolparty.slurm.array.Pool()``
+----------------------------------
+Uses slurm's ``--array`` option.
+It will call ``sbatch --array``, ``squeue`` and ``scancel``.
+
+``pypoolparty.sun_grid_engine.Pool()``
+--------------------------------------
+It will call ``qsub``, ``qstat`` and ``qdel``.
+
+``pypoolparty.slurm.Pool()``
+----------------------------
+It will call ``sbatch``, ``squeue`` and ``scancel``.
+Uses the same inner workings as ``pypoolparty.sun_grid_engine.Pool()``.
+
+Testing
+=======
+The ``pypoolparty`` comes with ist own dummys for slurm and the sun grid engine.
+This allows to test the full chain without the actual workload managers to be installed.
+
+.. code:: bash
+
+    pytest -s pypoolparty
+
+
+Workload managers
+=================
+We tested:
+
+- SLURM, version 22.05.6
+- Sun Grid Engine (SGE), version 8.1.9
 
 
 Alternatives
 ============
 When you do not share resources with other users, when you do not need to respect fair share, and when you have some administrative power you might want to use one of these:
 
 - Dask_ has a ``job_queue`` which also supports other flavors such as PBS, SLURM.
 
 - pyABC.sge_ has a ``pool.map()`` very much like the one in this package.
 
 - ipyparallel_
 
 
-Queue Flavors
-=============
+Inner Workings
+==============
+The maaping and reducing takes place in a ``work_dir`` in the filesystem.
+The ``work_dir`` can be defined manually and must be reachable by all
+compute notes.
+
+``slurm.array.Pool``
+--------------------
+- Makes a ``work_dir`` where it creates a zip-file named ``tasks.zip`` in which it dumps all ``tasks`` using ``pickle``.
+
+- Starts a logger which logs into a file named ``log.jsonl`` in the ``work_dir``.
 
-- SLURM, version 22.05.6
-- Sun Grid Engine (SGE), version 8.1.9
+- Makea a script which will execute the tasks on the compute nodes and dumps the script named ``script.py`` into the ``work_dir``. The script contains the path to the ``work_dir`` and queries the environment variable ``SLURM_ARRAY_TASK_ID`` to determine which ``task`` it shall process. It will write its result, ``stdout`` and ``stderr``, and potentially a report of raised ``exceptions`` into the ``work_dir``.
 
+- Calls ``sbatch --array``
+
+- After the initial call of ``sbatch``, we wait for the jobs to return (to write their results) or to get stuck in some error state. With a polling interval of 5s (can be adjusted), the ``work_dir`` is searched for results and ``squeue`` is searched for jobs in error states. When results are found in the ``work_dir``, they are read and appended into the four zip-files named ``tasks.results.zip``, ``tasks.stdout.zip``, ``tasks.stderr.zip``, and ``tasks.exceptions.zip``. When the individual files writen by a job got appended to the zip-files, the individual files are removed to keep the number of files low.
+
+- If the poll of ``squeue`` indicates ``tasks`` with error like flags, these specific ``tasks`` will be removed from the queue by calling ``scancel`` and then added again by calling ``sbatch --array`` until a predefined limit of resubmissions is reached.
+
+- Finally, either all ``tasks`` returned results or got finally stuck in errors and exceptions. The results are read into memory from ``work_dir/tasks_results.zip`` and returned by the ``map()`` function. If there was non zero ``stderr`` or an exception, the ``work_dir`` will not be removed after the call of ``map()``, but will stay for potential debugging.
+
+
+``sun_grid_engine.Pool`` and ``slurm.Pool``
+-------------------------------------------
 
-Inner Workings
-==============
 - ``map()`` makes a ``work_dir`` because the mapping and reducing takes place in the filesystem. You can set ``work_dir`` manually to make sure both the worker nodes and the process node can reach it.
 
 - ``map()`` serializes your ``tasks`` using ``pickle`` into separate files in ``work_dir/{ichunk:09d}.pkl``.
 
 - ``map()`` reads all environment variables in its process.
 
 - ``map()`` creates the worker-node script in ``work_dir/worker_node_script.py``. It contains and exports the process' environment variables into the batch job's context. It reads the chunk of tasks in ``work_dir/{ichunk:09d}.pkl``, imports and runs your ``func(task)``, and finally writes the result back to ``work_dir/{ichunk:09d}.pkl.out``.
@@ -122,53 +174,37 @@
 - ``ichunk`` is the index of a chunk. It is used to create the chunks's filenames such as ``work_dir/{ichunk:09d}.pkl``.
 
 - `queue-job` is what we submit into the queue. Each queue-job processes the tasks in a single chunk in series.
 
 - ``jobname`` or ``job["name"]`` is assigned to a queue job by our ``map()``. It is composed of our ``map()``'s session-id, and ``ichunk``. E.g. ``"q"%Y-%m-%dT%H:%M:%S"#{ichunk:09d}"``
 
 
-Testing
-=======
+Testing for developers
+======================
+The tests have an option ``--debug_dir`` which allows to make the otherwise
+temporary output and working directories to remain after the tests have run.
 
 .. code:: bash
 
-    pytest -s .
+    pytest -s --debug_dir path/to/do/debugging pypoolparty
 
 
 dummy queue
 -----------
 To test our ``map()`` we provide a dummy ``qsub``, ``qstat``, and ``qdel``
-for the sun-grid-engine.
+for the sun-grid-engine, and a dummy ``sbatch``, ``squeue``, and ``scancel``
+for slurm.
 These are individual ``python`` scripts which all act on a common state file
-in ``tests/resources/dummy_queue_state.json`` in order to fake the
-sun-grid-engine's queue.
-
-- ``dummy_qsub.py`` only appends queue jobs to the list of pending jobs in the state-file.
-
-- ``dummy_qdel.py`` only removes queue jobs from the state-file.
-
-- ``dummy_qstat.py`` does move the queue jobs from the pending to the running list, and does trigger the actual processing of the jobs. Each time ``dummy_qstat.py`` is called it performs a single action on the state file. So it must be called multiple times to process all jobs. It can intentionally bring jobs into the error-state when this is set in the state-file.
-
-Before running the dummy queue, its state file must be initialized:
-
-.. code:: python
-
-    from pypoolparty import sun_grid_engine
-
-    sun_grid_engine.testing.init_queue_state(
-        path="tests/resources/dummy_queue_state.json"
-    )
+named ``queue_state.json`` in order to imitate the workload managers.
 
-When testing our ``map()`` you set its arguments ``qsub_path``, ``qdel_path``,
-and ``qstat_path`` to point to the dummy queue.
+- ``qsub``/``sbatch`` only append pening jobs to the list of jobs in ``queue_state.json``.
 
-See ``tests/test_full_chain_with_dummy_qsub.py``.
+- ``qdel``/``scancel`` only remove jobs from the list of jobs in ``queue_state.json``.
 
-Because of the global state file, only one instance of dummy_queue must run
-at a time.
+- ``qstat``/``squeue`` changes  the state of jobs from pending to running, and triggers the actual processing of the jobs. Each time ``qstat.py`` is called it performs a single action on ``queue_state.json``. So it must be called multiple times to process all jobs. It can intentionally bring jobs into error states when this is set accordingly in the ``queue_state.json``.
 
 
 .. |TestStatus| image:: https://github.com/cherenkov-plenoscope/pypoolparty/actions/workflows/test.yml/badge.svg?branch=main
     :target: https://github.com/cherenkov-plenoscope/pypoolparty/actions/workflows/test.yml
 
 .. |PyPiStatus| image:: https://img.shields.io/pypi/v/pypoolparty
     :target: https://pypi.org/project/pypoolparty
```

### Comparing `pypoolparty-0.0.8/pypoolparty.egg-info/SOURCES.txt` & `pypoolparty-0.2.1/pypoolparty.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,28 @@
 pypoolparty/version.py
 pypoolparty.egg-info/PKG-INFO
 pypoolparty.egg-info/SOURCES.txt
 pypoolparty.egg-info/dependency_links.txt
 pypoolparty.egg-info/requires.txt
 pypoolparty.egg-info/top_level.txt
 pypoolparty/slurm/__init__.py
-pypoolparty/slurm/call.py
+pypoolparty/slurm/calling.py
 pypoolparty/slurm/organizing_jobs.py
 pypoolparty/slurm/testing.py
+pypoolparty/slurm/array/__init__.py
+pypoolparty/slurm/array/making_script.py
+pypoolparty/slurm/array/mapping.py
+pypoolparty/slurm/array/polling.py
+pypoolparty/slurm/array/reducing.py
+pypoolparty/slurm/array/utils.py
 pypoolparty/slurm/tests/resources/dummy_queue_state.json
 pypoolparty/slurm/tests/resources/dummy_sbatch.py
 pypoolparty/slurm/tests/resources/dummy_scancel.py
 pypoolparty/slurm/tests/resources/dummy_squeue.py
 pypoolparty/slurm/tests/resources/squeue_format_all.stdout
 pypoolparty/sun_grid_engine/__init__.py
-pypoolparty/sun_grid_engine/call.py
+pypoolparty/sun_grid_engine/calling.py
 pypoolparty/sun_grid_engine/organizing_jobs.py
 pypoolparty/sun_grid_engine/testing.py
 pypoolparty/sun_grid_engine/tests/resources/dummy_qdel.py
 pypoolparty/sun_grid_engine/tests/resources/dummy_qstat.py
 pypoolparty/sun_grid_engine/tests/resources/dummy_qsub.py
```

### Comparing `pypoolparty-0.0.8/setup.py` & `pypoolparty-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     url="https://github.com/cherenkov-plenoscope/pypoolparty",
     author="Sebastian Achim Mueller",
     author_email="sebastian-achim.mueller@mpi-hd.mpg.de",
     packages=[
         "pypoolparty",
         "pypoolparty.sun_grid_engine",
         "pypoolparty.slurm",
+        "pypoolparty.slurm.array",
     ],
     package_data={
         "pypoolparty": [
             os.path.join("slurm", "tests", "resources", "*"),
             os.path.join("sun_grid_engine", "tests", "resources", "*"),
         ]
     },
```

