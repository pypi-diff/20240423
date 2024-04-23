# Comparing `tmp/hideandseek-0.2.1.tar.gz` & `tmp/hideandseek-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hideandseek-0.2.1.tar", last modified: Mon Apr 22 19:51:15 2024, max compression
+gzip compressed data, was "hideandseek-0.2.2.tar", last modified: Tue Apr 23 18:06:14 2024, max compression
```

## Comparing `hideandseek-0.2.1.tar` & `hideandseek-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.136883 hideandseek-0.2.1/
--rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2757 2024-04-22 19:51:15.135888 hideandseek-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.083213 hideandseek-0.2.1/hideandseek/
--rw-rw-rw-   0        0        0      330 2024-04-22 19:37:08.000000 hideandseek-0.2.1/hideandseek/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.1/hideandseek/dataset.py
--rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.1/hideandseek/evaluation.py
--rw-rw-rw-   0        0        0     9959 2024-04-22 19:50:56.000000 hideandseek-0.2.1/hideandseek/fv.py
--rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.1/hideandseek/loss.py
--rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.1/hideandseek/model.py
--rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.1/hideandseek/plot.py
--rw-rw-rw-   0        0        0    24904 2024-04-22 19:50:06.000000 hideandseek-0.2.1/hideandseek/trainer.py
--rw-rw-rw-   0        0        0     4757 2024-04-22 19:32:15.000000 hideandseek-0.2.1/hideandseek/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.133881 hideandseek-0.2.1/hideandseek.egg-info/
--rw-rw-rw-   0        0        0     2757 2024-04-22 19:51:13.000000 hideandseek-0.2.1/hideandseek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 19:51:13.000000 hideandseek-0.2.1/hideandseek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 19:51:15.137882 hideandseek-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:06:14.177507 hideandseek-0.2.2/
+-rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2757 2024-04-23 18:06:14.175501 hideandseek-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:06:14.118977 hideandseek-0.2.2/hideandseek/
+-rw-rw-rw-   0        0        0      330 2024-04-23 18:05:49.000000 hideandseek-0.2.2/hideandseek/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.2/hideandseek/dataset.py
+-rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.2/hideandseek/evaluation.py
+-rw-rw-rw-   0        0        0    10060 2024-04-23 18:05:45.000000 hideandseek-0.2.2/hideandseek/fv.py
+-rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.2/hideandseek/loss.py
+-rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.2/hideandseek/model.py
+-rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.2/hideandseek/plot.py
+-rw-rw-rw-   0        0        0    24906 2024-04-22 20:07:36.000000 hideandseek-0.2.2/hideandseek/trainer.py
+-rw-rw-rw-   0        0        0     4757 2024-04-22 19:32:15.000000 hideandseek-0.2.2/hideandseek/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:06:14.173632 hideandseek-0.2.2/hideandseek.egg-info/
+-rw-rw-rw-   0        0        0     2757 2024-04-23 18:06:13.000000 hideandseek-0.2.2/hideandseek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-23 18:06:13.000000 hideandseek-0.2.2/hideandseek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:06:13.000000 hideandseek-0.2.2/hideandseek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-23 18:06:13.000000 hideandseek-0.2.2/hideandseek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 18:06:13.000000 hideandseek-0.2.2/hideandseek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:06:14.178501 hideandseek-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.2/setup.py
```

### Comparing `hideandseek-0.2.1/LICENSE` & `hideandseek-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/PKG-INFO` & `hideandseek-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.1
+Version: 0.2.2
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.1/README.md` & `hideandseek-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/dataset.py` & `hideandseek-0.2.2/hideandseek/dataset.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/evaluation.py` & `hideandseek-0.2.2/hideandseek/evaluation.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/fv.py` & `hideandseek-0.2.2/hideandseek/fv.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,42 +60,48 @@
     # Gradient descent not ascent, so negate the objective if maximize=True
     if maximize: threshold = -threshold if threshold is not None else None
 
     # Thresholded flag for batch data when objective threshold is given
     if threshold is not None:
         thresholded = torch.zeros(len(data), dtype=torch.bool, device=data.device)
         data_optimized = torch.empty_like(data)
+    
+    # Default is doing nothing
+    preprocess = lambda x: x if preprocess is None else preprocess
+    regularization = lambda x: x if regularization is None else regularization
 
-    optimizer = optim.Adam([data], lr=lr) # Defaults to Adam
+    # Defaults to Adam optimizer
+    optimizer = optim.Adam([data], lr=lr) 
 
     l_history = []
     for i in range(1,updates+1):
-        data_p = preprocess(data) if preprocess is not None else data
-        data_r = regularization(data_p) if regularization is not None else data_p
+        data_p = preprocess(data)
+        data_r = regularization(data_p)
         loss = objective(data_r)
 
         if maximize:
             loss = -loss
 
         l_history.append(data_p.detach().clone())
         if threshold is not None:
             thresholded_ = (loss.detach() < threshold)
             store_idx = thresholded_ & ~thresholded
             data_optimized[store_idx] = data[store_idx].detach().clone()
             thresholded[store_idx] = True
             
-            print(-loss, thresholded)
             if thresholded.all(): break
 
-        # if threshold is not None: print(loss, thresholded)
         loss = loss.mean()
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
-        if verbose: print(f'[{i}/{updates}][Loss: {loss.item()}]')
+        
+        if verbose:
+            loss = -loss.item() if maximize else loss.item()
+            print(f'[{i}/{updates}][Loss: {loss}]')
 
     if threshold is not None:
         data_optimized[~thresholded] = data[~thresholded].detach().clone()
         data = data_optimized
     
     with torch.no_grad():
         features = preprocess(data)
```

### Comparing `hideandseek-0.2.1/hideandseek/loss.py` & `hideandseek-0.2.2/hideandseek/loss.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/model.py` & `hideandseek-0.2.2/hideandseek/model.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/plot.py` & `hideandseek-0.2.2/hideandseek/plot.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek/trainer.py` & `hideandseek-0.2.2/hideandseek/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,18 +454,18 @@
         Save the following:
         state_dict() -> path/state_dict.p
         network.state_dict() -> path/network.pt
         '''
         path = self.network_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
-        state_dict_path = os.path.join(path, 'node.p')
-        self.print(f'[save] Saving node info to: {state_dict_path}')
-        state_dict = self.state_dict()
+        self.print(f'[save] Saving Model info to: {state_dict_path}')
         self.print(f'[save] state_dict: {list(state_dict.keys())}')
+        state_dict_path = os.path.join(path, 'model.p')
+        state_dict = self.state_dict()
         tools.save_pickle(state_dict, state_dict_path)
 
         network_path = os.path.join(path, 'network.pt')
         if best:
             if self.earlystopper is None:
                 self.print(f'[save][best: {best}] earlystopper not defined. Saving current network -> [{network_path}]')
                 torch.save(self.network.state_dict(), network_path)
```

### Comparing `hideandseek-0.2.1/hideandseek/utils.py` & `hideandseek-0.2.2/hideandseek/utils.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.1/hideandseek.egg-info/PKG-INFO` & `hideandseek-0.2.2/hideandseek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.1
+Version: 0.2.2
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.1/setup.py` & `hideandseek-0.2.2/setup.py`

 * *Files identical despite different names*

