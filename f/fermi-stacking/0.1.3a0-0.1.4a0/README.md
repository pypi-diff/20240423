# Comparing `tmp/fermi_stacking-0.1.3a0.tar.gz` & `tmp/fermi_stacking-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fermi_stacking-0.1.3a0.tar", last modified: Fri Mar  1 14:26:46 2024, max compression
+gzip compressed data, was "fermi_stacking-0.1.4a0.tar", last modified: Tue Apr 23 13:50:36 2024, max compression
```

## Comparing `fermi_stacking-0.1.3a0.tar` & `fermi_stacking-0.1.4a0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.151507 fermi_stacking-0.1.3a0/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    11357 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/LICENSE
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-03-01 14:26:46.150507 fermi_stacking-0.1.3a0/PKG-INFO
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2323 2024-02-29 15:18:01.000000 fermi_stacking-0.1.3a0/README.md
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.043506 fermi_stacking-0.1.3a0/fermi_stacking/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      188 2024-02-22 20:54:20.000000 fermi_stacking-0.1.3a0/fermi_stacking/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.056506 fermi_stacking-0.1.3a0/fermi_stacking/analyze_results/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    34092 2024-02-29 17:31:31.000000 fermi_stacking-0.1.3a0/fermi_stacking/analyze_results/AnalyzeResults.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       36 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/fermi_stacking/analyze_results/__init__.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     1395 2024-02-28 21:29:53.000000 fermi_stacking-0.1.3a0/fermi_stacking/client.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      476 2024-02-28 21:13:42.000000 fermi_stacking-0.1.3a0/fermi_stacking/make_new_run.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.073506 fermi_stacking-0.1.3a0/fermi_stacking/pop_studies/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    29992 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/fermi_stacking/pop_studies/PopStudies.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       26 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/fermi_stacking/pop_studies/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.097506 fermi_stacking-0.1.3a0/fermi_stacking/preprocessing/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    24664 2024-02-29 14:45:18.000000 fermi_stacking-0.1.3a0/fermi_stacking/preprocessing/Preprocess.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       42 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/fermi_stacking/preprocessing/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.100506 fermi_stacking-0.1.3a0/fermi_stacking/science_tools/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)     3890 2024-02-28 21:30:25.000000 fermi_stacking-0.1.3a0/fermi_stacking/science_tools/BinnedAnalysis.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       47 2024-02-23 19:10:27.000000 fermi_stacking-0.1.3a0/fermi_stacking/science_tools/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.105507 fermi_stacking-0.1.3a0/fermi_stacking/stacking/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    21749 2024-02-28 18:00:27.000000 fermi_stacking-0.1.3a0/fermi_stacking/stacking/Stack.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       29 2024-02-08 20:27:23.000000 fermi_stacking-0.1.3a0/fermi_stacking/stacking/__init__.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    72337 2024-02-14 15:56:02.000000 fermi_stacking-0.1.3a0/fermi_stacking/stacking/add_stacking_module_LLAGN.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2333 2024-02-28 20:58:50.000000 fermi_stacking-0.1.3a0/fermi_stacking/submit_fermi_stacking_jobs.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-03-01 14:26:46.148507 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/PKG-INFO
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      850 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/SOURCES.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)        1 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/dependency_links.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       71 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/entry_points.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       14 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/requires.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       15 2024-03-01 14:26:45.000000 fermi_stacking-0.1.3a0/fermi_stacking.egg-info/top_level.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       38 2024-03-01 14:26:46.151507 fermi_stacking-0.1.3a0/setup.cfg
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      501 2024-02-29 18:29:37.000000 fermi_stacking-0.1.3a0/setup.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.953118 fermi_stacking-0.1.4a0/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    11357 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/LICENSE
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-04-23 13:50:36.952118 fermi_stacking-0.1.4a0/PKG-INFO
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2323 2024-02-29 15:18:01.000000 fermi_stacking-0.1.4a0/README.md
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.878117 fermi_stacking-0.1.4a0/fermi_stacking/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      188 2024-02-22 20:54:20.000000 fermi_stacking-0.1.4a0/fermi_stacking/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.907118 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    34113 2024-04-23 13:36:07.000000 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/AnalyzeResults.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       36 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/__init__.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     1395 2024-02-28 21:29:53.000000 fermi_stacking-0.1.4a0/fermi_stacking/client.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      476 2024-02-28 21:13:42.000000 fermi_stacking-0.1.4a0/fermi_stacking/make_new_run.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.929118 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    29992 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/PopStudies.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       26 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.933118 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    24664 2024-02-29 14:45:18.000000 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/Preprocess.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       42 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.947118 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)     3890 2024-02-28 21:30:25.000000 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/BinnedAnalysis.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       47 2024-02-23 19:10:27.000000 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.950118 fermi_stacking-0.1.4a0/fermi_stacking/stacking/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    21750 2024-04-23 13:28:52.000000 fermi_stacking-0.1.4a0/fermi_stacking/stacking/Stack.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       29 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/stacking/__init__.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2333 2024-02-28 20:58:50.000000 fermi_stacking-0.1.4a0/fermi_stacking/submit_fermi_stacking_jobs.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.951118 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/PKG-INFO
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      797 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/SOURCES.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)        1 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/dependency_links.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       71 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/entry_points.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       14 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/requires.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       15 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/top_level.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       38 2024-04-23 13:50:36.954118 fermi_stacking-0.1.4a0/setup.cfg
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      501 2024-04-23 13:46:07.000000 fermi_stacking-0.1.4a0/setup.py
```

### Comparing `fermi_stacking-0.1.3a0/LICENSE` & `fermi_stacking-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/README.md` & `fermi_stacking-0.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/analyze_results/AnalyzeResults.py` & `fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/AnalyzeResults.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,16 @@
         # Below I define 3 different methods to plot the array, just with different styles.
         # Use method 1 as the default.
         
 	# Method 1
         def plot_method_1():
             
             img = ax.pcolormesh(flux_list,index_list,summed_array,cmap="inferno",vmin=0,vmax=max_value)
-            plt.contour(flux_list,index_list,summed_array,levels = (third,second,first),colors='limegreen',linestyles=["-.",'--',"-"], alpha=1,linewidths=2)
+            plt.contour(flux_list,index_list,summed_array,levels = (third,second,first),
+                    colors='limegreen',linestyles=["-.",'--',"-"], alpha=1,linewidths=2)
             plt.plot(best_flux,best_index,marker="+",ms=12,color="black")
             ax.set_xscale('log')
             plt.xticks(fontsize=16)
             plt.yticks(fontsize=16)
             
             return img
```

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/client.py` & `fermi_stacking-0.1.4a0/fermi_stacking/client.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/pop_studies/PopStudies.py` & `fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/PopStudies.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/preprocessing/Preprocess.py` & `fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/Preprocess.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/science_tools/BinnedAnalysis.py` & `fermi_stacking-0.1.4a0/fermi_stacking/science_tools/BinnedAnalysis.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/stacking/Stack.py` & `fermi_stacking-0.1.4a0/fermi_stacking/stacking/Stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
                 stacking_dir = os.path.join(self.home,"Stacked_Sources",srcname)
 	
                 if os.path.exists(stacking_dir) == False or os.path.exists(likelihood_dir) == False:
                     print() 
                     print('Does not exist: ' + srcname)
                     print()
 
-                if srcname not in exclusion_list and os.path.exists(lielihood_dir) == True and os.path.exists(stacking_dir) == True:
+                if srcname not in exclusion_list and os.path.exists(likelihood_dir) == True and os.path.exists(stacking_dir) == True:
 				
                     os.chdir(stacking_dir)
 	            
                     print_list.append(srcname)
 		
                     array_list = []
```

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking/submit_fermi_stacking_jobs.py` & `fermi_stacking-0.1.4a0/fermi_stacking/submit_fermi_stacking_jobs.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.3a0/fermi_stacking.egg-info/SOURCES.txt` & `fermi_stacking-0.1.4a0/fermi_stacking.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 fermi_stacking/pop_studies/PopStudies.py
 fermi_stacking/pop_studies/__init__.py
 fermi_stacking/preprocessing/Preprocess.py
 fermi_stacking/preprocessing/__init__.py
 fermi_stacking/science_tools/BinnedAnalysis.py
 fermi_stacking/science_tools/__init__.py
 fermi_stacking/stacking/Stack.py
-fermi_stacking/stacking/__init__.py
-fermi_stacking/stacking/add_stacking_module_LLAGN.py
+fermi_stacking/stacking/__init__.py
```

