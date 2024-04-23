# Comparing `tmp/samap-1.0.7.tar.gz` & `tmp/samap-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samap-1.0.7.tar", last modified: Wed Oct  5 15:27:27 2022, max compression
+gzip compressed data, was "samap-1.0.8.tar", last modified: Fri Dec 16 16:07:01 2022, max compression
```

## Comparing `samap-1.0.7.tar` & `samap-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-10-05 15:27:27.874576 samap-1.0.7/
--rwxr-xr-x   0 atarashansky   (503) staff       (20)     1069 2022-07-20 15:58:45.000000 samap-1.0.7/LICENSE
--rw-r--r--   0 atarashansky   (503) staff       (20)      488 2022-10-05 15:27:27.874404 samap-1.0.7/PKG-INFO
--rwxr-xr-x   0 atarashansky   (503) staff       (20)     2455 2022-10-05 15:26:29.000000 samap-1.0.7/README.md
-drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-10-05 15:27:27.873201 samap-1.0.7/samap/
--rwxr-xr-x   0 atarashansky   (503) staff       (20)      187 2022-07-20 15:58:46.000000 samap-1.0.7/samap/__init__.py
--rw-r--r--   0 atarashansky   (503) staff       (20)    65953 2022-10-05 15:01:37.000000 samap-1.0.7/samap/analysis.py
--rwxr-xr-x   0 atarashansky   (503) staff       (20)    64494 2022-10-05 14:44:53.000000 samap-1.0.7/samap/mapping.py
--rwxr-xr-x   0 atarashansky   (503) staff       (20)     3436 2022-10-05 14:42:27.000000 samap-1.0.7/samap/utils.py
-drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-10-05 15:27:27.874202 samap-1.0.7/samap.egg-info/
--rw-r--r--   0 atarashansky   (503) staff       (20)      488 2022-10-05 15:27:27.000000 samap-1.0.7/samap.egg-info/PKG-INFO
--rw-r--r--   0 atarashansky   (503) staff       (20)      266 2022-10-05 15:27:27.000000 samap-1.0.7/samap.egg-info/SOURCES.txt
--rw-r--r--   0 atarashansky   (503) staff       (20)        1 2022-10-05 15:27:27.000000 samap-1.0.7/samap.egg-info/dependency_links.txt
--rw-r--r--   0 atarashansky   (503) staff       (20)        1 2022-10-05 14:45:58.000000 samap-1.0.7/samap.egg-info/not-zip-safe
--rw-r--r--   0 atarashansky   (503) staff       (20)       86 2022-10-05 15:27:27.000000 samap-1.0.7/samap.egg-info/requires.txt
--rw-r--r--   0 atarashansky   (503) staff       (20)        6 2022-10-05 15:27:27.000000 samap-1.0.7/samap.egg-info/top_level.txt
--rw-r--r--   0 atarashansky   (503) staff       (20)       38 2022-10-05 15:27:27.874632 samap-1.0.7/setup.cfg
--rwxr-xr-x   0 atarashansky   (503) staff       (20)      837 2022-10-05 15:26:24.000000 samap-1.0.7/setup.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-12-16 16:07:01.213228 samap-1.0.8/
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)     1069 2022-07-20 15:58:45.000000 samap-1.0.8/LICENSE
+-rw-r--r--   0 atarashansky   (503) staff       (20)      488 2022-12-16 16:07:01.213033 samap-1.0.8/PKG-INFO
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)     2455 2022-12-16 16:06:39.000000 samap-1.0.8/README.md
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-12-16 16:07:01.211513 samap-1.0.8/samap/
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)      187 2022-12-16 16:06:49.000000 samap-1.0.8/samap/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    65953 2022-10-05 15:01:37.000000 samap-1.0.8/samap/analysis.py
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)    64586 2022-12-16 16:05:32.000000 samap-1.0.8/samap/mapping.py
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)     3436 2022-10-05 14:42:27.000000 samap-1.0.8/samap/utils.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2022-12-16 16:07:01.212802 samap-1.0.8/samap.egg-info/
+-rw-r--r--   0 atarashansky   (503) staff       (20)      488 2022-12-16 16:07:01.000000 samap-1.0.8/samap.egg-info/PKG-INFO
+-rw-r--r--   0 atarashansky   (503) staff       (20)      266 2022-12-16 16:07:01.000000 samap-1.0.8/samap.egg-info/SOURCES.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        1 2022-12-16 16:07:01.000000 samap-1.0.8/samap.egg-info/dependency_links.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        1 2022-10-05 14:45:58.000000 samap-1.0.8/samap.egg-info/not-zip-safe
+-rw-r--r--   0 atarashansky   (503) staff       (20)       86 2022-12-16 16:07:01.000000 samap-1.0.8/samap.egg-info/requires.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        6 2022-12-16 16:07:01.000000 samap-1.0.8/samap.egg-info/top_level.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)       38 2022-12-16 16:07:01.213290 samap-1.0.8/setup.cfg
+-rwxr-xr-x   0 atarashansky   (503) staff       (20)      837 2022-12-16 16:06:31.000000 samap-1.0.8/setup.py
```

### Comparing `samap-1.0.7/LICENSE` & `samap-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `samap-1.0.7/README.md` & `samap-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SAMap -- version 1.0.7
+# SAMap -- version 1.0.8
 
 # Citation
 Please cite the following paper if using SAMap: https://elifesciences.org/articles/66747
 
 Tarashansky, Alexander J., et al. "Mapping single-cell atlases throughout Metazoa unravels cell type evolution." Elife 10 (2021): e66747.
 
 ## Installation
```

### Comparing `samap-1.0.7/samap/analysis.py` & `samap-1.0.8/samap/analysis.py`

 * *Files identical despite different names*

### Comparing `samap-1.0.7/samap/mapping.py` & `samap-1.0.8/samap/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                     gns_dict[sid].size, sid
                 )
             )
 
         for sid in sams:
             if not sp.sparse.issparse(sams[sid].adata.X):
                 sams[sid].adata.X = sp.sparse.csr_matrix(sams[sid].adata.X)
-                
+
         smap = _Samap_Iter(sams, gnnm, gns_dict, keys=keys)
         self.sams = sams
         self.gnnm = gnnm
         self.gns_dict = gns_dict
         self.gns = gns
         self.ids = ids
         self.smap = smap
@@ -1101,18 +1101,18 @@
 
                 A = A[A.index.astype("str") != "nan"]
                 A = A[A.iloc[:, 0].astype("str") != "nan"]
                 B = B[B.index.astype("str") != "nan"]
                 B = B[B.iloc[:, 0].astype("str") != "nan"]
 
                 A.index = _prepend_blast_prefix(A.index,id1)
-                B.iloc[:, 0] = _prepend_blast_prefix(B.iloc[:, 0].values.flatten(),id1)
+                B[B.columns[0]] = _prepend_blast_prefix(B.iloc[:, 0].values.flatten(),id1)
 
                 B.index = _prepend_blast_prefix(B.index,id2)
-                A.iloc[:, 0] = _prepend_blast_prefix(A.iloc[:, 0].values.flatten(),id2)
+                A[A.columns[0]] = _prepend_blast_prefix(A.iloc[:, 0].values.flatten(),id2)
 
                 i1 = np.where(A.columns == "10")[0][0]
                 i3 = np.where(A.columns == "11")[0][0]
 
                 inA = q(A.index)
                 inB = q(B.index)
 
@@ -1121,16 +1121,16 @@
                 gn1 = np.unique(np.append(inB2, inA))
                 gn2 = np.unique(np.append(inA2, inB))
                 gn = np.append(gn1, gn2)
                 gnind = pd.DataFrame(data=np.arange(gn.size)[None, :], columns=gn)
 
                 A.index = pd.Index(gnind[A.index].values.flatten())
                 B.index = pd.Index(gnind[B.index].values.flatten())
-                A.iloc[:, 0] = gnind[A.iloc[:, 0].values.flatten()].values.flatten()
-                B.iloc[:, 0] = gnind[B.iloc[:, 0].values.flatten()].values.flatten()
+                A[A.columns[0]] = gnind[A.iloc[:, 0].values.flatten()].values.flatten()
+                B[B.columns[0]] = gnind[B.iloc[:, 0].values.flatten()].values.flatten()
 
                 Arows = np.vstack((A.index, A.iloc[:, 0], A.iloc[:, i3])).T
                 Arows = Arows[A.iloc[:, i1].values.flatten() <= eval_thr, :]
                 gnnm1 = sp.sparse.lil_matrix((gn.size,) * 2)
                 gnnm1[Arows[:, 0].astype("int32"), Arows[:, 1].astype("int32")] = Arows[
                     :, 2
                 ]  # -np.log10(Arows[:,2]+1e-200)
@@ -1310,14 +1310,18 @@
 
     a = []
     for i,sid in enumerate(sams.keys()):
         a.extend(["batch" + str(i + 1)] * sams[sid].adata.shape[0])
     sam.adata.obs["batch"] = pd.Categorical(np.array(a))
     sam.adata.obs.columns = sam.adata.obs.columns.astype("str")
     sam.adata.var.columns = sam.adata.var.columns.astype("str")
+
+    for i in sam.adata.obs:
+        sam.adata.obs[i] = sam.adata.obs[i].astype("str")
+        
     return sam
 
 def _map_features_un(A, B, sam1, sam2, thr=1e-6):
     i1 = np.where(A.columns == "10")[0][0]
     i3 = np.where(A.columns == "11")[0][0]
 
     inA = q(A.index)
```

### Comparing `samap-1.0.7/samap/utils.py` & `samap-1.0.8/samap/utils.py`

 * *Files identical despite different names*

### Comparing `samap-1.0.7/setup.py` & `samap-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="samap",
-    version="1.0.7",
+    version="1.0.8",
     description="The SAMap algorithm",
     long_description="The Self-Assembling Manifold Mapping algorithm for mapping single-cell datasets across species.",
     long_description_content_type="text/markdown",
     author="Alexander J. Tarashansky",
     url="https://github.com/atarashansky/SAMap",
     author_email="tarashan@stanford.edu",
     keywords="scrnaseq analysis manifold reconstruction cross-species mapping",
```

