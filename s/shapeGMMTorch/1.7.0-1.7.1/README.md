# Comparing `tmp/shapeGMMTorch-1.7.0.tar.gz` & `tmp/shapeGMMTorch-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapeGMMTorch-1.7.0.tar", last modified: Fri Jan 19 20:12:45 2024, max compression
+gzip compressed data, was "shapeGMMTorch-1.7.1.tar", last modified: Tue Apr 23 18:41:25 2024, max compression
```

## Comparing `shapeGMMTorch-1.7.0.tar` & `shapeGMMTorch-1.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mmccull    (503) staff       (20)        0 2024-01-19 20:12:45.399908 shapeGMMTorch-1.7.0/
--rw-r--r--   0 mmccull    (503) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.7.0/LICENSE
--rw-r--r--   0 mmccull    (503) staff       (20)     7804 2024-01-19 20:12:45.399562 shapeGMMTorch-1.7.0/PKG-INFO
--rw-r--r--   0 mmccull    (503) staff       (20)     7217 2023-09-12 15:32:23.000000 shapeGMMTorch-1.7.0/README.md
--rw-r--r--   0 mmccull    (503) staff       (20)       38 2024-01-19 20:12:45.399987 shapeGMMTorch-1.7.0/setup.cfg
--rw-r--r--   0 mmccull    (503) staff       (20)     1006 2023-12-13 15:19:11.000000 shapeGMMTorch-1.7.0/setup.py
-drwxr-xr-x   0 mmccull    (503) staff       (20)        0 2024-01-19 20:12:45.356930 shapeGMMTorch-1.7.0/src/
-drwxr-xr-x   0 mmccull    (503) staff       (20)        0 2024-01-19 20:12:45.396193 shapeGMMTorch-1.7.0/src/shapeGMMTorch/
--rw-r--r--   0 mmccull    (503) staff       (20)        0 2023-06-28 14:43:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/__init__.py
--rw-r--r--   0 mmccull    (503) staff       (20)     1683 2023-12-13 16:05:56.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/generate_points.py
--rw-r--r--   0 mmccull    (503) staff       (20)     3013 2023-10-17 00:12:40.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/plots.py
--rw-r--r--   0 mmccull    (503) staff       (20)    11361 2024-01-19 20:10:50.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/scripts.py
--rw-r--r--   0 mmccull    (503) staff       (20)     6771 2023-12-13 15:04:54.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/similarities.py
--rw-r--r--   0 mmccull    (503) staff       (20)    14547 2024-01-09 23:27:17.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_align.py
--rw-r--r--   0 mmccull    (503) staff       (20)     6666 2023-12-03 20:01:00.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
--rw-r--r--   0 mmccull    (503) staff       (20)    21568 2023-12-13 15:05:13.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_sgmm.py
--rw-r--r--   0 mmccull    (503) staff       (20)     5781 2023-07-10 14:27:01.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
-drwxr-xr-x   0 mmccull    (503) staff       (20)        0 2024-01-19 20:12:45.399090 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/
--rw-r--r--   0 mmccull    (503) staff       (20)     7804 2024-01-19 20:12:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/PKG-INFO
--rw-r--r--   0 mmccull    (503) staff       (20)      542 2024-01-19 20:12:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/SOURCES.txt
--rw-r--r--   0 mmccull    (503) staff       (20)        1 2024-01-19 20:12:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/dependency_links.txt
--rw-r--r--   0 mmccull    (503) staff       (20)       18 2024-01-19 20:12:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/requires.txt
--rw-r--r--   0 mmccull    (503) staff       (20)       14 2024-01-19 20:12:45.000000 shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/top_level.txt
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2024-04-23 18:41:25.639674 shapeGMMTorch-1.7.1/
+-rw-r--r--   0 mmccull    (502) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.7.1/LICENSE
+-rw-r--r--   0 mmccull    (502) staff       (20)     7804 2024-04-23 18:41:25.639320 shapeGMMTorch-1.7.1/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)     7217 2023-09-12 15:32:23.000000 shapeGMMTorch-1.7.1/README.md
+-rw-r--r--   0 mmccull    (502) staff       (20)       38 2024-04-23 18:41:25.639782 shapeGMMTorch-1.7.1/setup.cfg
+-rw-r--r--   0 mmccull    (502) staff       (20)     1006 2024-04-23 17:52:58.000000 shapeGMMTorch-1.7.1/setup.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2024-04-23 18:41:25.527183 shapeGMMTorch-1.7.1/src/
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2024-04-23 18:41:25.636929 shapeGMMTorch-1.7.1/src/shapeGMMTorch/
+-rw-r--r--   0 mmccull    (502) staff       (20)        0 2023-06-28 14:43:45.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/__init__.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     1683 2023-12-13 14:48:54.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/generate_points.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     3013 2023-10-17 00:12:34.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/plots.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    11840 2024-02-15 22:28:59.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/scripts.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     6772 2024-04-23 18:39:29.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/similarities.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    14547 2024-01-09 23:27:17.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_align.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     6666 2023-12-03 20:00:48.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    21764 2024-04-23 18:36:16.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_sgmm.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     5781 2023-07-10 14:27:01.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2024-04-23 18:41:25.638974 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/
+-rw-r--r--   0 mmccull    (502) staff       (20)     7804 2024-04-23 18:41:24.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)      542 2024-04-23 18:41:25.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/SOURCES.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)        1 2024-04-23 18:41:24.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/dependency_links.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       18 2024-04-23 18:41:24.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/requires.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       14 2024-04-23 18:41:24.000000 shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/top_level.txt
```

### Comparing `shapeGMMTorch-1.7.0/LICENSE` & `shapeGMMTorch-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/PKG-INFO` & `shapeGMMTorch-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.7.0
+Version: 1.7.1
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shapeGMMTorch-1.7.0/README.md` & `shapeGMMTorch-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/setup.py` & `shapeGMMTorch-1.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='shapeGMMTorch',
-    version='1.7.0',
+    version='1.7.1',
     author='Martin McCullagh',
     author_email='martin.mccullagh@okstate.edu',
     description='Gaussian Mixture Model clustering in size-and-shape space using PyTorch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mccullaghlab/shapeGMMTorch',
     project_urls = {
```

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/generate_points.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/generate_points.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/plots.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/plots.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/scripts.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import time
 import sys
 import torch
 import MDAnalysis as md
 from scipy import stats
 from . import torch_sgmm
+from . import torch_align
 from . import generate_points
 
 def cross_validate_cluster_scan(traj_data, n_train_frames, frame_weights = [], covar_type="kronecker", cluster_array = np.arange(2,9,1).astype(int), n_training_sets=10, n_attempts = 5, dtype=torch.float32, device=torch.device("cuda:0")):
     """
     perform cross validation weighted shape-GMM for range of cluster sizes. Return train and CV log likelihoods as a function of number of clusters for each training set.
     Inputs:
         traj_data                    (required)  : float64 array with dimensions (n_frames, n_atoms,3) of molecular configurations
@@ -120,15 +121,15 @@
         print("%8d %19.3f %15.3f" % (i+1, np.round(wsgmm.log_likelihood,3), np.round(elapsed_time,3)))
         objs.append(wsgmm)
         log_likes.append(wsgmm.log_likelihood)
     # return obj with max log likelihood per frame
     return objs[np.nanargmax(log_likes)]
 
 # write cluster trajectories
-def write_cluster_trajectories(sgmm, n_frames_per_cluster=100):
+def generate_cluster_trajectories(sgmm, n_frames_per_cluster=100):
     """
     Write generated trajectories for each cluster in shapeGMM object sgmm
     """
     # create MDAnalysis universe
     u = md.Universe.empty(sgmm.n_atoms, 1, atom_resindex=np.zeros(sgmm.n_atoms), trajectory=True)
     u.trajectory.n_frames = n_frames_per_cluster
     sel_all = u.select_atoms("all")
@@ -144,31 +145,36 @@
         # write dcd of generated trajectory
         with md.Writer(dcd_file_name, sel_all.n_atoms) as W:
             for ts in range(n_frames_per_cluster):
                 sel_all.positions = trj[ts]
                 W.write(sel_all)
         W.close()
 
-# write cluster trajectories
-def write_cluster_trajectories(traj_data, cluster_ids):
+# write aligned cluster trajectories
+def write_aligned_cluster_trajectories(traj_data, cluster_ids, covar_type='kronecker',dtype=torch.float64,device=torch.device("cpu")):
     """
     Write trajectories for each cluster from trajectory data and cluster ids
     """
     # get meta data from inputs
     n_frames = traj_data.shape[0]
     n_atoms = traj_data.shape[1]
     n_cluster_frames = np.unique(cluster_ids,return_counts=True)[1]
     n_clusters = n_cluster_frames.size
     # loop through clusters
     for cluster_id in range(n_clusters):
         # create MDAnalysis universe
         u = md.Universe.empty(n_atoms, 1, atom_resindex=np.zeros(n_atoms), trajectory=True)
         u.trajectory.n_frames = n_cluster_frames[cluster_id]
         sel_all = u.select_atoms("all")
-        trj = traj_data[cluster_ids==cluster_id]
+        # align cluster trajectory
+        trj_tensor = torch.tensor(traj_data[cluster_ids==cluster_id],dtype=dtype,device=device)
+        torch_align.torch_remove_center_of_geometry(trj_tensor,dtype=dtype,device=device)
+        aligned_traj_tensor = torch_align.torch_iterative_align_kronecker(trj_tensor,dtype=dtype,device=device)[0]
+        trj = aligned_traj_tensor.cpu().numpy()
+        # create file names
         pdb_file_name = "cluster" + str(cluster_id+1) + "_frame1.pdb"
         dcd_file_name = "cluster" + str(cluster_id+1) + "_" + str(n_cluster_frames[cluster_id]) + "frames.dcd"
         # write pdb of mean structure
         sel_all.positions = trj[0]
         sel_all.write(pdb_file_name)
         # write dcd of generated trajectory
         with md.Writer(dcd_file_name, sel_all.n_atoms) as W:
```

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/similarities.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/similarities.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,21 @@
     Compute the configurational entropy of shapeGMM object sgmmP using sampling
     with n_points
 
     sgmmP      : shapeGMM object
     n_points   : (integer) number of frames to generate to sample
 
     returns:
-    lnP        : (float) configurational entropy
+    -lnP       : (float) configurational entropy
     sterr(lnP) : (float) standard error of sampled configurational entropy
     """
     # sample the object and compute probabilities of each sampled point
     trj = sgmmP.generate(n_points)
     lnP = sgmmP.predict(trj)[2]
-    return lnP, stats.sem(sgmmP.predict_frame_log_likelihood)
+    return -lnP, stats.sem(sgmmP.predict_frame_log_likelihood)
 
 def _pinv(sigma):
     e, v = np.linalg.eigh(sigma)
     e[0] = 0.0
     e[1:] = 1/e[1:]
     return np.dot(v,np.dot(np.diag(e),v.T))
```

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_align.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_align.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_sgmm.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_sgmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,15 @@
         for k in range(self.n_clusters):
             indeces = np.argwhere(self.cluster_ids == k).flatten()
             # initialize weights as populations of clusters
             self.weights[k] = indeces.size/self.n_train_frames
             if self.covar_type == 'uniform':
                 centers_tensor[k], vars_tensor[k] = torch_align.torch_iterative_align_uniform_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,device=self.device,dtype=self.dtype)[1:]
             else:
-                if (self.verbose==True):
-                    centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,max_iter=self.kabsch_max_steps,device=self.device,dtype=self.dtype,verbose=True)[1:]
-                else:
-                    centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,max_iter=self.kabsch_max_steps, device=self.device,dtype=self.dtype)[1:]        
+                centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,max_iter=self.kabsch_max_steps, device=self.device,dtype=self.dtype)[1:]        
         if (self.verbose == True):
             print("Weights from initial clusters in fit:", self.weights)
     
         # pass remaining data to device
         ln_weights_tensor = torch.tensor(np.log(self.weights),dtype=torch.float64,device=self.device)
         
         # perform Expectation Maximization
@@ -159,15 +156,15 @@
         del centers_tensor
         torch.cuda.empty_cache()
         
         # sort object
         if self.sort == True:
             self._sort_object()
         # return aligned trajectory
-        return traj_data
+        #return traj_data
 
     # predict clustering of provided data based on prefit parameters from fit_weighted
     def predict(self,traj_data, frame_weights = []):
         """
         Predict size-and-shape GMM using traj_data as prediction set and already fit object parameters.
         traj_data (required)     - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
         frame_weights (optional) - (n_frames) float numpy array of frame weights
@@ -223,47 +220,56 @@
             # align each cluster to its average
             for k in range(self.n_clusters):
                 indeces = np.argwhere(clusters == k).flatten()
                 if self.covar_type == 'uniform':
                     traj_tensor[indeces] = torch_align.torch_align_uniform(traj_tensor[indeces], centers_tensor[k])
                 else:
                     traj_tensor[indeces] = torch_align.torch_align_kronecker(traj_tensor[indeces], centers_tensor[k], precisions_tensor[k], dtype=self.dtype, device=self.device)
-            # return traj_data to cpu
-            traj_data = traj_tensor.cpu().numpy()
             # delete data from gpu
             del traj_tensor
             del ln_weights_tensor
             del centers_tensor
             if self.covar_type == 'uniform': 
                 del vars_tensor 
             else: # assume weighted
                 del precisions_tensor 
                 del lpdets_tensor 
             torch.cuda.empty_cache()
             # return values
-            return clusters, traj_data, log_likelihood
+            return clusters
         else:
             print("shapeGMM must be fit before it can predict.")
 
     # generate a trajectory from shapeGMM object - no time correlation!
     def generate(self,n_frames):
         """
         Generate a trajectory from a fit shapeGMM object using multivariate Gaussian generator (from scipy)
         n_frames (required)     - int of number of frames to generater
 
         Returns:
         trajectory      - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions generated from shapeGMM object. 
         """
 
         if self._gmm_fit_flag == True:
+            # generate random cluster ids based on frame weights - not could adapt this to account for transition matrix
             cluster_ids = generate_points.cluster_ids_from_rand(np.random.rand(n_frames),self.weights)
             trj = np.empty((n_frames,self.n_atoms,3))
             for cluster_id in range(self.n_clusters):
+                if self.covar_type == "kronecker":
+                    precision = self.precisions[cluster_id]
+                else:
+                    precision = 1/self.vars[cluster_id] * np.identity(self.n_atoms)
+                    # now enforece that constant vector is in null space of precision
+                    wsum = -1/self.vars[cluster_id]/(self.n_atoms-1)
+                    for i in range(self.n_atoms):
+                        for j in range(self.n_atoms):
+                            if i != j:
+                                precision[i,j] = wsum
                 indeces = np.argwhere(cluster_ids == cluster_id).flatten()
-                trj[indeces] = generate_points.gen_mv(self.centers[cluster_id],self.precisions[cluster_id],indeces.size)
+                trj[indeces] = generate_points.gen_mv(self.centers[cluster_id],precision,indeces.size)
             return trj
         else:
             print("shapeGMM must be fit before it can generate.")
         
     # initialize clusters
     def _init_clusters(self, traj_tensor, cluster_ids=[]):
```

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch/torch_uniform_sgmm_lib.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/PKG-INFO` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.7.0
+Version: 1.7.1
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shapeGMMTorch-1.7.0/src/shapeGMMTorch.egg-info/SOURCES.txt` & `shapeGMMTorch-1.7.1/src/shapeGMMTorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

