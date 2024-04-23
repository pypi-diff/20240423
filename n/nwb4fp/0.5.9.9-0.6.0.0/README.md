# Comparing `tmp/nwb4fp-0.5.9.9.tar.gz` & `tmp/nwb4fp-0.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.9.9.tar", last modified: Tue Apr 23 16:43:17 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.0.0.tar", last modified: Tue Apr 23 17:25:44 2024, max compression
```

## Comparing `nwb4fp-0.5.9.9.tar` & `nwb4fp-0.6.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.718506 nwb4fp-0.5.9.9/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.9.9/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-04-23 16:43:17.710504 nwb4fp-0.5.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.9.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 16:43:17.735501 nwb4fp-0.5.9.9/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-23 16:43:13.000000 nwb4fp-0.5.9.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.217496 nwb4fp-0.5.9.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.243499 nwb4fp-0.5.9.9/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.9.9/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.226505 nwb4fp-0.5.9.9/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.9.9/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.9.9/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.232505 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-04-09 09:11:18.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    12768 2024-04-23 16:32:19.000000 nwb4fp-0.5.9.9/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.640499 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.9/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.253494 nwb4fp-0.5.9.9/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.253494 nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:43:17.392509 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-04-23 16:43:16.000000 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-23 16:43:17.000000 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:43:16.000000 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-04-23 16:43:16.000000 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 16:43:16.000000 nwb4fp-0.5.9.9/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.814302 nwb4fp-0.6.0.0/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5780 2024-04-23 17:25:44.807298 nwb4fp-0.6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 17:25:44.830298 nwb4fp-0.6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-23 17:25:41.000000 nwb4fp-0.6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.155307 nwb4fp-0.6.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.277306 nwb4fp-0.6.0.0/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.0/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.358312 nwb4fp-0.6.0.0/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.0/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.0/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.544379 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-04-09 09:11:18.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    12768 2024-04-23 16:32:19.000000 nwb4fp-0.6.0.0/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.707306 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.0/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.187300 nwb4fp-0.6.0.0/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.721317 nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:25:44.335302 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5780 2024-04-23 17:25:43.000000 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-23 17:25:44.000000 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:25:43.000000 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2910 2024-04-23 17:25:43.000000 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 17:25:43.000000 nwb4fp-0.6.0.0/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.5.9.9/LICENSE` & `nwb4fp-0.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/PKG-INFO` & `nwb4fp-0.6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.9.9
+Version: 0.6.0.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -71,14 +71,15 @@
 Requires-Dist: jupyterlab_pygments==0.3.0
 Requires-Dist: jupyterlab_server==2.25.3
 Requires-Dist: keyring==24.3.0
 Requires-Dist: llvmlite==0.42.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: matplotlib-inline==0.1.6
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mistune==3.0.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: msgpack==1.0.8
 Requires-Dist: multidict==6.0.5
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nbclient==0.9.0
```

### Comparing `nwb4fp-0.5.9.9/README.md` & `nwb4fp-0.6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/setup.py` & `nwb4fp-0.6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.5.9.9',
+    version='0.6.0.0',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.0.0/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.0.0/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.0.0/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.0.0/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.0.0/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.0.0/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.0.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.0.0/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.9.9
+Version: 0.6.0.0
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -71,14 +71,15 @@
 Requires-Dist: jupyterlab_pygments==0.3.0
 Requires-Dist: jupyterlab_server==2.25.3
 Requires-Dist: keyring==24.3.0
 Requires-Dist: llvmlite==0.42.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: matplotlib-inline==0.1.6
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mistune==3.0.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: msgpack==1.0.8
 Requires-Dist: multidict==6.0.5
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nbclient==0.9.0
```

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.0.0/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.9/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.0.0/src/nwb4fp.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 jupyterlab_pygments==0.3.0
 jupyterlab_server==2.25.3
 keyring==24.3.0
 llvmlite==0.42.0
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 matplotlib-inline==0.1.6
+matplotlib==3.8.4
 mdurl==0.1.2
 mistune==3.0.2
 more-itertools==10.2.0
 msgpack==1.0.8
 multidict==6.0.5
 natsort==8.4.0
 nbclient==0.9.0
```

