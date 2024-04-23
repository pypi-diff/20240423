# Comparing `tmp/ScholarCodeCollective-0.1.1.tar.gz` & `tmp/ScholarCodeCollective-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.1.tar", last modified: Mon Apr 22 17:18:56 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.2.tar", last modified: Tue Apr 23 11:59:43 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.1.tar` & `ScholarCodeCollective-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.057505 ScholarCodeCollective-0.1.1/
--rw-rw-rw-   0        0        0     3782 2024-04-22 17:18:56.056491 ScholarCodeCollective-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.022217 ScholarCodeCollective-0.1.1/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.041345 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.045621 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     5448 2024-04-22 16:57:34.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.049092 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.052046 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.038045 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3782 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 17:18:56.057673 ScholarCodeCollective-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-04-22 17:18:36.000000 ScholarCodeCollective-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.054371 ScholarCodeCollective-0.1.1/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.333406 ScholarCodeCollective-0.1.2/
+-rw-rw-rw-   0        0        0     3782 2024-04-23 11:59:43.332530 ScholarCodeCollective-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.296111 ScholarCodeCollective-0.1.2/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.315152 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.321231 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.322765 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.328699 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.311939 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     3782 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:59:43.333406 ScholarCodeCollective-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-04-23 11:59:34.000000 ScholarCodeCollective-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.330211 ScholarCodeCollective-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.2/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.1/PKG-INFO` & `ScholarCodeCollective-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.1/README.md` & `ScholarCodeCollective-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,138 +1,140 @@
 import pandas as pd
 import numpy as np
 from collections import Counter
 from scipy.special import loggamma
-
-def MDL_regionalization(adjlist,dists,pops):
-    
-    """
-    inputs: 
-        adjlist: list of lists, representing adjacency list of integer node indices
-        dists: 2D numpy array with normalize probability mass function for each unit (in same order as node indices)
-        pops: populations of units (in same order as node indices)
-        
-    outputs:
-        inverse compression ratio of data
-        cluster labels for all units (in same order as node indices)
-        distributions 'dists' input to algorithm (just for reference)
+class MDL_regionalization:
+    def __init__(self,name):
+        self.name = name
+    def MDL_regionalization(adjlist,dists,pops):
+        
+        """
+        inputs: 
+            adjlist: list of lists, representing adjacency list of integer node indices
+            dists: 2D numpy array with normalize probability mass function for each unit (in same order as node indices)
+            pops: populations of units (in same order as node indices)
+            
+        outputs:
+            inverse compression ratio of data
+            cluster labels for all units (in same order as node indices)
+            distributions 'dists' input to algorithm (just for reference)
+            
+        """
         
-    """
-    
-    def str2int(l):
-        d = dict([(y,x+1) for x,y in enumerate(sorted(set(l)))])
-        return [d[x] for x in l]
-    
-    def logNcK(n,K):
-        return loggamma(n+1) - loggamma(n-K+1) - loggamma(K+1)
-    
-    def logMult(ns):
-        N = sum(ns)
-        return loggamma(N+1) - sum(loggamma(i+1) for i in ns)
-    
-    def log_num_bin_sizes(n,K):
-        if n >= K:
-            return logNcK(n-1,K-1)
-        else:
-            return 0.
-        
-    def log_omega(row_sums,col_sums):
-        n = sum(row_sums)
-        R = len(row_sums)
-        S = len(col_sums)
-        w = n/(n+0.5*R*S)
-        x = (1-w)/R + w*row_sums/n
-        y = (1-w)/S + w*col_sums/n
-        mu = (R+1)/(R*sum(y**2)) - 1/R
-        nu = (S+1)/(S*sum(x**2)) - 1/S
-        return (R-1)*(S-1)*np.log(n+0.5*R*S) + 0.5*(R+nu-2)*sum(np.log(y))\
-                    + 0.5*(S+mu-2)*sum(np.log(x)) + 0.5*loggamma(mu*R) + 0.5*loggamma(nu*S)\
-                    - 0.5*S*loggamma(nu) - 0.5*S*loggamma(R) - 0.5*R*loggamma(mu) - 0.5*R*loggamma(S) 
-        
-    def cluster_DL(cluster):
-        mix = dists[list(cluster),:].sum(axis=0)
-        mix /= sum(mix)
-        local_pops = [pops[ii] for ii in cluster]
-        n_clust,m_clust = sum(local_pops),len(cluster)
-        dl_model = log_num_bin_sizes(n_clust,R) + log_num_bin_sizes(n_clust,m_clust) 
-        row_sums = np.array(mix*n_clust)
-        col_sums = np.array(local_pops)
-        dl_loss = log_omega(row_sums,col_sums)
-        return dl_model + dl_loss 
-    
-    def global_DL(clusters):
-        dl = log_num_bin_sizes(n,len(clusters)) + log_num_bin_sizes(m,len(clusters)) 
-        return dl + sum([cluster_DL(cluster) for cluster in clusters])
-    
-    def random_key():
-        return str(np.random.randint(0,100000000000))
-    
-    def cluster_merge(key1,key2,update = False):
+        def str2int(l):
+            d = dict([(y,x+1) for x,y in enumerate(sorted(set(l)))])
+            return [d[x] for x in l]
+        
+        def logNcK(n,K):
+            return loggamma(n+1) - loggamma(n-K+1) - loggamma(K+1)
+        
+        def logMult(ns):
+            N = sum(ns)
+            return loggamma(N+1) - sum(loggamma(i+1) for i in ns)
+        
+        def log_num_bin_sizes(n,K):
+            if n >= K:
+                return logNcK(n-1,K-1)
+            else:
+                return 0.
+            
+        def log_omega(row_sums,col_sums):
+            n = sum(row_sums)
+            R = len(row_sums)
+            S = len(col_sums)
+            w = n/(n+0.5*R*S)
+            x = (1-w)/R + w*row_sums/n
+            y = (1-w)/S + w*col_sums/n
+            mu = (R+1)/(R*sum(y**2)) - 1/R
+            nu = (S+1)/(S*sum(x**2)) - 1/S
+            return (R-1)*(S-1)*np.log(n+0.5*R*S) + 0.5*(R+nu-2)*sum(np.log(y))\
+                        + 0.5*(S+mu-2)*sum(np.log(x)) + 0.5*loggamma(mu*R) + 0.5*loggamma(nu*S)\
+                        - 0.5*S*loggamma(nu) - 0.5*S*loggamma(R) - 0.5*R*loggamma(mu) - 0.5*R*loggamma(S) 
+            
+        def cluster_DL(cluster):
+            mix = dists[list(cluster),:].sum(axis=0)
+            mix /= sum(mix)
+            local_pops = [pops[ii] for ii in cluster]
+            n_clust,m_clust = sum(local_pops),len(cluster)
+            dl_model = log_num_bin_sizes(n_clust,R) + log_num_bin_sizes(n_clust,m_clust) 
+            row_sums = np.array(mix*n_clust)
+            col_sums = np.array(local_pops)
+            dl_loss = log_omega(row_sums,col_sums)
+            return dl_model + dl_loss 
+        
+        def global_DL(clusters):
+            dl = log_num_bin_sizes(n,len(clusters)) + log_num_bin_sizes(m,len(clusters)) 
+            return dl + sum([cluster_DL(cluster) for cluster in clusters])
         
-        if key1 == key2:
-            return 0,False
+        def random_key():
+            return str(np.random.randint(0,100000000000))
         
-        merged = clusters[key1].union(clusters[key2])
-        K_before = len(clusters)
-        if not(tuple(sorted((key1,key2))) in merge_DL_dict):
-            merge_DL_dict[tuple(sorted((key1,key2)))] = cluster_DL(merged) - cluster_DL(clusters[key1]) - cluster_DL(clusters[key2]) 
-        delta_dl = merge_DL_dict[tuple(sorted((key1,key2)))] - log_num_bin_sizes(n,K_before) - log_num_bin_sizes(m,K_before) \
-                                                          + log_num_bin_sizes(n,K_before-1) + log_num_bin_sizes(m,K_before-1) 
-        
-        if (delta_dl < 0) and (update == True):
-            clusters.pop(key1,None)
-            clusters.pop(key2,None)
-            past_neigs = adjset[key1] + adjset[key2]
-            past_neigs.pop(key1,None)
-            past_neigs.pop(key2,None)
-            adjset.pop(key1,None)
-            adjset.pop(key2,None)
-            new_key = random_key()
-            clusters[new_key] = merged
-            for i in merged:
-                labels[i] = new_key
-            adjset[new_key] = past_neigs
-            for neig_key in past_neigs.keys():
-                adjset[neig_key][new_key] = adjset[new_key][neig_key]
-                adjset[neig_key].pop(key1,None)
-                adjset[neig_key].pop(key2,None)
-            cluster_pops[new_key] = cluster_pops[key1] + cluster_pops[key2]
-            cluster_pops.pop(key1,None)
-            cluster_pops.pop(key2,None)
+        def cluster_merge(key1,key2,update = False):
             
-        return min([delta_dl,0]),delta_dl < 0
-    
-    n = sum(pops) #notation in code: n's are populations, m's are numbers of units
-    m = len(adjlist)
-    R = dists.shape[1]
-    keys = [random_key() for i in range(m)]
-    clusters = {keys[i]:{i} for i in range(m)}
-    labels = np.copy(keys)
-    adjset = {labels[i]:Counter([labels[j] for j in adjlist[i]]) for i in range(m)}
-    initial_DL = global_DL(list(clusters.values()))
-    cluster_pops = {labels[i]:pops[i] for i in range(m)}
-    
-    ct = 0
-    DL = initial_DL
-    merge_DL_dict = {}
-    while (len(clusters.keys()) > 1):
- 
-        all_pairs = [(key1,key2) for key1 in adjset.keys() for key2 in adjset[key1] if (key2 > key1)]
-        neg_pairs,neg_deltas,neg_sizes = [],[],[]
-        for pair in all_pairs:
-            delta = cluster_merge(pair[0],pair[1],update = False)[0]
-            if delta < 0:
-                neg_pairs.append(pair)
-                neg_deltas.append(delta)
-                neg_sizes.append(cluster_pops[pair[0]] + cluster_pops[pair[1]])
+            if key1 == key2:
+                return 0,False
+            
+            merged = clusters[key1].union(clusters[key2])
+            K_before = len(clusters)
+            if not(tuple(sorted((key1,key2))) in merge_DL_dict):
+                merge_DL_dict[tuple(sorted((key1,key2)))] = cluster_DL(merged) - cluster_DL(clusters[key1]) - cluster_DL(clusters[key2]) 
+            delta_dl = merge_DL_dict[tuple(sorted((key1,key2)))] - log_num_bin_sizes(n,K_before) - log_num_bin_sizes(m,K_before) \
+                                                            + log_num_bin_sizes(n,K_before-1) + log_num_bin_sizes(m,K_before-1) 
+            
+            if (delta_dl < 0) and (update == True):
+                clusters.pop(key1,None)
+                clusters.pop(key2,None)
+                past_neigs = adjset[key1] + adjset[key2]
+                past_neigs.pop(key1,None)
+                past_neigs.pop(key2,None)
+                adjset.pop(key1,None)
+                adjset.pop(key2,None)
+                new_key = random_key()
+                clusters[new_key] = merged
+                for i in merged:
+                    labels[i] = new_key
+                adjset[new_key] = past_neigs
+                for neig_key in past_neigs.keys():
+                    adjset[neig_key][new_key] = adjset[new_key][neig_key]
+                    adjset[neig_key].pop(key1,None)
+                    adjset[neig_key].pop(key2,None)
+                cluster_pops[new_key] = cluster_pops[key1] + cluster_pops[key2]
+                cluster_pops.pop(key1,None)
+                cluster_pops.pop(key2,None)
+                
+            return min([delta_dl,0]),delta_dl < 0
+        
+        n = sum(pops) #notation in code: n's are populations, m's are numbers of units
+        m = len(adjlist)
+        R = dists.shape[1]
+        keys = [random_key() for i in range(m)]
+        clusters = {keys[i]:{i} for i in range(m)}
+        labels = np.copy(keys)
+        adjset = {labels[i]:Counter([labels[j] for j in adjlist[i]]) for i in range(m)}
+        initial_DL = global_DL(list(clusters.values()))
+        cluster_pops = {labels[i]:pops[i] for i in range(m)}
+        
+        ct = 0
+        DL = initial_DL
+        merge_DL_dict = {}
+        while (len(clusters.keys()) > 1):
+    
+            all_pairs = [(key1,key2) for key1 in adjset.keys() for key2 in adjset[key1] if (key2 > key1)]
+            neg_pairs,neg_deltas,neg_sizes = [],[],[]
+            for pair in all_pairs:
+                delta = cluster_merge(pair[0],pair[1],update = False)[0]
+                if delta < 0:
+                    neg_pairs.append(pair)
+                    neg_deltas.append(delta)
+                    neg_sizes.append(cluster_pops[pair[0]] + cluster_pops[pair[1]])
 
-        if len(neg_deltas) == 0:
-            return [global_DL(list(clusters.values()))/initial_DL,str2int(labels),dists]
-        else:
-            best_ind = np.argmin(neg_deltas)
-            key1,key2 = neg_pairs[best_ind]
-            delta_DL,accepted = cluster_merge(key1,key2,update = True)
-                   
-        DL += delta_DL
-        ct += 1
-               
-    return [global_DL(list(clusters.values()))/initial_DL,str2int(labels),dists] 
+            if len(neg_deltas) == 0:
+                return [global_DL(list(clusters.values()))/initial_DL,str2int(labels),dists]
+            else:
+                best_ind = np.argmin(neg_deltas)
+                key1,key2 = neg_pairs[best_ind]
+                delta_DL,accepted = cluster_merge(key1,key2,update = True)
+                    
+            DL += delta_DL
+            ct += 1
+                
+        return [global_DL(list(clusters.values()))/initial_DL,str2int(labels),dists]
```

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.1/setup.py` & `ScholarCodeCollective-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='ScholarCodeCollective',
-    version='0.1.1',
+    version='0.1.2',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name', 
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.1/tests/__init__.py` & `ScholarCodeCollective-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

