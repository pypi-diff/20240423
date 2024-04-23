# Comparing `tmp/PyIBIS-AMI-5.1.3.tar.gz` & `tmp/pyibis_ami-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIBIS-AMI-5.1.3.tar", last modified: Thu Apr 11 14:09:37 2024, max compression
+gzip compressed data, was "pyibis_ami-5.1.4.tar", last modified: Tue Apr 23 18:46:02 2024, max compression
```

## Comparing `PyIBIS-AMI-5.1.3.tar` & `pyibis_ami-5.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/
--rw-rw-rw-   0        0        0     1301 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/LICENSE
--rw-rw-rw-   0        0        0      229 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3971 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2720 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.078482 PyIBIS-AMI-5.1.3/docs/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.088521 PyIBIS-AMI-5.1.3/docs/source/
--rw-rw-rw-   0        0        0      323 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/ami.rst
--rw-rw-rw-   0        0        0    10396 2024-04-11 14:06:38.000000 PyIBIS-AMI-5.1.3/docs/source/conf.py
--rw-rw-rw-   0        0        0      256 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/ibis.rst
--rw-rw-rw-   0        0        0      581 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/index.rst
--rw-rw-rw-   0        0        0     1371 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/install.rst
--rw-rw-rw-   0        0        0      158 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/modules.rst
--rw-rw-rw-   0        0        0      152 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/tools.rst
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.108653 PyIBIS-AMI-5.1.3/examples/
--rw-rw-rw-   0        0        0      990 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/all_taps.run
--rw-rw-rw-   0        0        0      398 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/bandwidth.run
--rw-rw-rw-   0        0        0      729 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/dummy.em
--rw-rw-rw-   0        0        0      362 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/examples.md
--rw-rw-rw-   0        0        0     3717 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/freq_resp.em
--rw-rw-rw-   0        0        0     1949 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/impulse.em
--rw-rw-rw-   0        0        0    27454 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/impulse_response_8ma.txt
--rw-rw-rw-   0        0        0      557 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/mode.run
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.108653 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/
--rw-rw-rw-   0        0        0     1693 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/all_taps.run
--rw-rw-rw-   0        0        0     4012 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/test_results.xml
--rw-rw-rw-   0        0        0     2000 2024-04-11 14:05:06.000000 PyIBIS-AMI-5.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.078482 PyIBIS-AMI-5.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/
--rw-rw-rw-   0        0        0     3971 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1198 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.118700 PyIBIS-AMI-5.1.3/src/pyibisami/
--rw-rw-rw-   0        0        0      624 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/__init__.py
--rw-rw-rw-   0        0        0      324 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.128736 PyIBIS-AMI-5.1.3/src/pyibisami/ami/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/__init__.py
--rw-rw-rw-   0        0        0     9835 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/config.py
--rw-rw-rw-   0        0        0      519 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ami.em
--rw-rw-rw-   0        0        0     5930 2024-02-12 22:17:02.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ibs.em
--rw-rw-rw-   0        0        0    15750 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/model.py
--rw-rw-rw-   0        0        0    12833 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/parameter.py
--rw-rw-rw-   0        0        0    19786 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/__init__.py
--rw-rw-rw-   0        0        0    11873 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/file.py
--rw-rw-rw-   0        0        0    16188 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/model.py
--rw-rw-rw-   0        0        0    13712 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/src/pyibisami/tools/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/__init__.py
--rw-rw-rw-   0        0        0     9166 2024-02-14 15:27:28.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/run_tests.py
--rw-rw-rw-   0        0        0     1704 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/test_results.xsl
-drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/tests/
--rw-rw-rw-   0        0        0     4621 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/tests/test_run_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.843487 pyibis_ami-5.1.4/
+-rw-rw-rw-   0        0        0     1301 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3971 2024-04-23 18:46:02.842487 pyibis_ami-5.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2720 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.771438 pyibis_ami-5.1.4/docs/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.787623 pyibis_ami-5.1.4/docs/source/
+-rw-rw-rw-   0        0        0      323 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/ami.rst
+-rw-rw-rw-   0        0        0    10396 2024-04-11 14:06:38.000000 pyibis_ami-5.1.4/docs/source/conf.py
+-rw-rw-rw-   0        0        0      256 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/ibis.rst
+-rw-rw-rw-   0        0        0      581 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1371 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/install.rst
+-rw-rw-rw-   0        0        0      158 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      152 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/docs/source/tools.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.799166 pyibis_ami-5.1.4/examples/
+-rw-rw-rw-   0        0        0      990 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/all_taps.run
+-rw-rw-rw-   0        0        0      398 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/bandwidth.run
+-rw-rw-rw-   0        0        0      729 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/dummy.em
+-rw-rw-rw-   0        0        0      362 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/examples.md
+-rw-rw-rw-   0        0        0     3717 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/freq_resp.em
+-rw-rw-rw-   0        0        0     1949 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/impulse.em
+-rw-rw-rw-   0        0        0    27454 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/impulse_response_8ma.txt
+-rw-rw-rw-   0        0        0      557 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/mode.run
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.802166 pyibis_ami-5.1.4/examples/stratix4_ami_tx_runs/
+-rw-rw-rw-   0        0        0     1693 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/stratix4_ami_tx_runs/all_taps.run
+-rw-rw-rw-   0        0        0     4012 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/examples/stratix4_ami_tx_runs/test_results.xml
+-rw-rw-rw-   0        0        0     2000 2024-04-23 18:44:41.000000 pyibis_ami-5.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:46:02.844486 pyibis_ami-5.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.773430 pyibis_ami-5.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.839486 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/
+-rw-rw-rw-   0        0        0     3971 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1198 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-23 18:46:02.000000 pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.812951 pyibis_ami-5.1.4/src/pyibisami/
+-rw-rw-rw-   0        0        0      624 2024-02-16 17:03:29.000000 pyibis_ami-5.1.4/src/pyibisami/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-02-16 17:03:29.000000 pyibis_ami-5.1.4/src/pyibisami/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.822952 pyibis_ami-5.1.4/src/pyibisami/ami/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/src/pyibisami/ami/__init__.py
+-rw-rw-rw-   0        0        0     9837 2024-04-23 18:10:04.000000 pyibis_ami-5.1.4/src/pyibisami/ami/config.py
+-rw-rw-rw-   0        0        0      519 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/src/pyibisami/ami/generic.ami.em
+-rw-rw-rw-   0        0        0     5930 2024-02-12 22:17:02.000000 pyibis_ami-5.1.4/src/pyibisami/ami/generic.ibs.em
+-rw-rw-rw-   0        0        0    15750 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/src/pyibisami/ami/model.py
+-rw-rw-rw-   0        0        0    12833 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/src/pyibisami/ami/parameter.py
+-rw-rw-rw-   0        0        0    19786 2024-02-16 17:03:29.000000 pyibis_ami-5.1.4/src/pyibisami/ami/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.829487 pyibis_ami-5.1.4/src/pyibisami/ibis/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 pyibis_ami-5.1.4/src/pyibisami/ibis/__init__.py
+-rw-rw-rw-   0        0        0    11873 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/src/pyibisami/ibis/file.py
+-rw-rw-rw-   0        0        0    16188 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/src/pyibisami/ibis/model.py
+-rw-rw-rw-   0        0        0    13712 2024-04-11 14:01:12.000000 pyibis_ami-5.1.4/src/pyibisami/ibis/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.834486 pyibis_ami-5.1.4/src/pyibisami/tools/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:09.000000 pyibis_ami-5.1.4/src/pyibisami/tools/__init__.py
+-rw-rw-rw-   0        0        0     9166 2024-02-14 15:27:28.000000 pyibis_ami-5.1.4/src/pyibisami/tools/run_tests.py
+-rw-rw-rw-   0        0        0     1704 2023-11-15 18:18:09.000000 pyibis_ami-5.1.4/src/pyibisami/tools/test_results.xsl
+drwxrwxrwx   0        0        0        0 2024-04-23 18:46:02.836488 pyibis_ami-5.1.4/tests/
+-rw-rw-rw-   0        0        0     4621 2023-11-15 18:18:09.000000 pyibis_ami-5.1.4/tests/test_run_tests.py
```

### Comparing `PyIBIS-AMI-5.1.3/LICENSE` & `pyibis_ami-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/PKG-INFO` & `pyibis_ami-5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIBIS-AMI
-Version: 5.1.3
+Version: 5.1.4
 Summary: Facilitates working directly with IBIS-AMI DLLs from the Python command prompt.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
 Project-URL: documentation, https://github.com/capn-freako/PyAMI/wiki
 Keywords: ibis-ami
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyIBIS-AMI-5.1.3/README.md` & `pyibis_ami-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/docs/source/conf.py` & `pyibis_ami-5.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/docs/source/index.rst` & `pyibis_ami-5.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/docs/source/install.rst` & `pyibis_ami-5.1.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/all_taps.run` & `pyibis_ami-5.1.4/examples/all_taps.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/dummy.em` & `pyibis_ami-5.1.4/examples/dummy.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/freq_resp.em` & `pyibis_ami-5.1.4/examples/freq_resp.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/impulse.em` & `pyibis_ami-5.1.4/examples/impulse.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/impulse_response_8ma.txt` & `pyibis_ami-5.1.4/examples/impulse_response_8ma.txt`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/mode.run` & `pyibis_ami-5.1.4/examples/mode.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/all_taps.run` & `pyibis_ami-5.1.4/examples/stratix4_ami_tx_runs/all_taps.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/test_results.xml` & `pyibis_ami-5.1.4/examples/stratix4_ami_tx_runs/test_results.xml`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/pyproject.toml` & `pyibis_ami-5.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 4249 532d 414d 4922 0d0a 6465 7363 7269  BIS-AMI"..descri
 00000080: 7074 696f 6e20 3d20 2246 6163 696c 6974  ption = "Facilit
 00000090: 6174 6573 2077 6f72 6b69 6e67 2064 6972  ates working dir
 000000a0: 6563 746c 7920 7769 7468 2049 4249 532d  ectly with IBIS-
 000000b0: 414d 4920 444c 4c73 2066 726f 6d20 7468  AMI DLLs from th
 000000c0: 6520 5079 7468 6f6e 2063 6f6d 6d61 6e64  e Python command
 000000d0: 2070 726f 6d70 742e 220d 0a76 6572 7369   prompt."..versi
-000000e0: 6f6e 203d 2022 352e 312e 3322 0d0a 6175  on = "5.1.3"..au
+000000e0: 6f6e 203d 2022 352e 312e 3422 0d0a 6175  on = "5.1.4"..au
 000000f0: 7468 6f72 7320 3d20 5b20 7b6e 616d 6520  thors = [ {name 
 00000100: 3d20 2244 6176 6964 2042 616e 6173 222c  = "David Banas",
 00000110: 2020 2020 2065 6d61 696c 203d 2022 6361       email = "ca
 00000120: 706e 2e66 7265 616b 6f40 676d 6169 6c2e  pn.freako@gmail.
 00000130: 636f 6d22 7d0d 0a20 2020 2020 2020 2020  com"}..         
 00000140: 202c 207b 6e61 6d65 203d 2022 4461 7669   , {name = "Davi
 00000150: 6420 5061 7474 6572 736f 6e22 7d0d 0a20  d Patterson"}..
```

### Comparing `PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/PKG-INFO` & `pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIBIS-AMI
-Version: 5.1.3
+Version: 5.1.4
 Summary: Facilitates working directly with IBIS-AMI DLLs from the Python command prompt.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
 Project-URL: documentation, https://github.com/capn-freako/PyAMI/wiki
 Keywords: ibis-ami
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/SOURCES.txt` & `pyibis_ami-5.1.4/src/PyIBIS_AMI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/__init__.py` & `pyibis_ami-5.1.4/src/pyibisami/__init__.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/config.py` & `pyibis_ami-5.1.4/src/pyibisami/ami/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 from pathlib import Path
 
 import click
 import em
 
 param_types = {
     "INT": {"c_type": "int", "ami_type": "Integer", "getter": "get_param_int"},
-    "FLOAT": {"c_type": "float", "ami_type": "Float", "getter": "get_param_float"},
-    "TAP": {"c_type": "float", "ami_type": "Tap", "getter": "get_param_float"},
+    "FLOAT": {"c_type": "double", "ami_type": "Float", "getter": "get_param_float"},
+    "TAP": {"c_type": "double", "ami_type": "Tap", "getter": "get_param_float"},
     "BOOL": {"c_type": "bool", "ami_type": "Boolean", "getter": "get_param_bool"},
     "STRING": {"c_type": "char *", "ami_type": "String", "getter": "get_param_str"},
 }
 
 
 def print_param(indent, name, param):
     """Print AMI parameter specification. Handle nested parameters, via
```

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ami.em` & `pyibis_ami-5.1.4/src/pyibisami/ami/generic.ami.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ibs.em` & `pyibis_ami-5.1.4/src/pyibisami/ami/generic.ibs.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/model.py` & `pyibis_ami-5.1.4/src/pyibisami/ami/model.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/parameter.py` & `pyibis_ami-5.1.4/src/pyibisami/ami/parameter.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ami/parser.py` & `pyibis_ami-5.1.4/src/pyibisami/ami/parser.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/file.py` & `pyibis_ami-5.1.4/src/pyibisami/ibis/file.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/model.py` & `pyibis_ami-5.1.4/src/pyibisami/ibis/model.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/parser.py` & `pyibis_ami-5.1.4/src/pyibisami/ibis/parser.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/tools/run_tests.py` & `pyibis_ami-5.1.4/src/pyibisami/tools/run_tests.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/src/pyibisami/tools/test_results.xsl` & `pyibis_ami-5.1.4/src/pyibisami/tools/test_results.xsl`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.3/tests/test_run_tests.py` & `pyibis_ami-5.1.4/tests/test_run_tests.py`

 * *Files identical despite different names*

