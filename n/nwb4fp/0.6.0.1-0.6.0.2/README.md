# Comparing `tmp/nwb4fp-0.6.0.1.tar.gz` & `tmp/nwb4fp-0.6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.0.1.tar", last modified: Tue Apr 23 17:47:50 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.0.2.tar", last modified: Tue Apr 23 18:18:51 2024, max compression
```

## Comparing `nwb4fp-0.6.0.1.tar` & `nwb4fp-0.6.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:50.502206 nwb4fp-0.6.0.1/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.1/LICENSE
--rw-rw-rw-   0        0        0     5780 2024-04-23 17:47:50.495209 nwb4fp-0.6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:47:50.517240 nwb4fp-0.6.0.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-23 17:47:43.000000 nwb4fp-0.6.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.784208 nwb4fp-0.6.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.894215 nwb4fp-0.6.0.1/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.1/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:50.017212 nwb4fp-0.6.0.1/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.1/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.1/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:50.166204 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-04-09 09:11:18.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    12782 2024-04-23 17:47:12.000000 nwb4fp-0.6.0.1/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.801205 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.1/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.813210 nwb4fp-0.6.0.1/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.813210 nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:49.994207 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5780 2024-04-23 17:47:49.000000 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-23 17:47:49.000000 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:47:49.000000 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2910 2024-04-23 17:47:49.000000 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:47:49.000000 nwb4fp-0.6.0.1/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:51.247067 nwb4fp-0.6.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5780 2024-04-23 18:18:51.240064 nwb4fp-0.6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:18:51.263063 nwb4fp-0.6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-23 18:18:44.000000 nwb4fp-0.6.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.605072 nwb4fp-0.6.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.624066 nwb4fp-0.6.0.2/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.2/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.615066 nwb4fp-0.6.0.2/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.2/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.2/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.619072 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    12782 2024-04-23 17:47:12.000000 nwb4fp-0.6.0.2/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.624066 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.2/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.629072 nwb4fp-0.6.0.2/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.632064 nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:50.610072 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5780 2024-04-23 18:18:50.000000 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-23 18:18:50.000000 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:18:50.000000 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2910 2024-04-23 18:18:50.000000 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 18:18:50.000000 nwb4fp-0.6.0.2/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.0.1/LICENSE` & `nwb4fp-0.6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/PKG-INFO` & `nwb4fp-0.6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.1/README.md` & `nwb4fp-0.6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/setup.py` & `nwb4fp-0.6.0.2/setup.py`

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
-    version='0.6.0.1',
+    version='0.6.0.2',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.0.2/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 def main():
     path = r"S:/Sachuriga/Ephys_Recording/CR_CA1/65410/65410_2023-11-25_13-57-58_A_phy_k_manual"
     add_wf_cor(path)
 
 def add_wf_cor(path):
 
     path_cluster_group = Path(fr"{path}/cluster_group.tsv")
-    path_cluster_metrix = Path(fr"{path}/waveformsfm/template_metrics/metrics.csv")
-    path_ulocation = Path(fr"{path}/waveformsfm/unit_locations/unit_locations.npy")
+    path_cluster_metrix = Path(fr"{path}/waveformsfm/extensions/quality_metrics/metrics.csv")
+    path_ulocation = Path(fr"{path}/waveformsfm/extensions/unit_locations/unit_locations.npy")
     df0 = pd.read_csv(path_cluster_group, index_col=0, sep='\t')
     df1 = pd.read_csv(path_cluster_metrix)
     df2 = pd.DataFrame(np.load(path_ulocation),columns=['x', 'y','z'])
     df3 = pd.merge(df0, df1,left_index=True,right_index=True)
     df4 = pd.merge(df3, df2,left_index=True,right_index=True)
 
     # List all files in the current directory
```

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.0.2/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.0.2/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.0.2/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.0.2/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.0.2/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.0.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.0.2/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.0.2/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.1/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.0.2/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

