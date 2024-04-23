# Comparing `tmp/titanq-0.9.1.tar.gz` & `tmp/titanq-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.9.1.tar", last modified: Wed Apr 17 16:04:04 2024, max compression
+gzip compressed data, was "titanq-0.9.2.tar", last modified: Tue Apr 23 20:49:34 2024, max compression
```

## Comparing `titanq-0.9.1.tar` & `titanq-0.9.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-11 20:26:44.000000 titanq-0.9.1/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-17 16:04:04.644055 titanq-0.9.1/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-11 20:26:44.000000 titanq-0.9.1/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-17 14:24:22.000000 titanq-0.9.1/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-11 20:26:44.000000 titanq-0.9.1/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-17 16:04:04.644055 titanq-0.9.1/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.640055 titanq-0.9.1/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.640055 titanq-0.9.1/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/manifest.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    29245 2024-04-17 14:41:47.000000 titanq-0.9.1/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3424 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/variable.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-16 15:57:02.000000 titanq-0.9.1/titanq/_model/variable_list.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-22 18:15:34.000000 titanq-0.9.2/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-23 20:49:34.415471 titanq-0.9.2/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5012 2024-04-22 18:15:34.000000 titanq-0.9.2/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1211 2024-04-23 20:35:00.000000 titanq-0.9.2/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-22 18:15:34.000000 titanq-0.9.2/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-23 20:49:34.415471 titanq-0.9.2/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    29177 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2058 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5236 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3499 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/variable.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/variable_list.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6643 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.9.1/LICENSE.txt` & `titanq-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/PKG-INFO` & `titanq-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.1
+Version: 0.9.2
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
-Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
+Project-URL: Documentation, https://sdk.titanq.infinityq.io
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Programming Language :: Python :: 3
@@ -93,15 +93,15 @@
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
 
-Additional parameters are avialble to tune the problem:
+Additional parameters are available to tune the problem:
 - beta
 - coupling_mult
 - num_chains
 - num_engines
 
 For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
```

### Comparing `titanq-0.9.1/README.md` & `titanq-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
 
-Additional parameters are avialble to tune the problem:
+Additional parameters are available to tune the problem:
 - beta
 - coupling_mult
 - num_chains
 - num_engines
 
 For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
```

### Comparing `titanq-0.9.1/pyproject.toml` & `titanq-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.9.1"
+version = "0.9.2"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 Homepage = "https://www.infinityq.tech"
-Documentation = "https://docs.titanq.infinityq.io/quickstart/category/python-sdk"
+Documentation = "https://sdk.titanq.infinityq.io"
 Examples = "https://github.com/infinityq-tech/titanq-examples"
 
 #Repository = "https://example.com"
 #Issues = "https://example.com"
 #Changelog = "https://example.com"
 
 [tool.setuptools.dynamic]
```

### Comparing `titanq-0.9.1/tests/test_client.py` & `titanq-0.9.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/tests/test_model.py` & `titanq-0.9.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/tests/test_numpy_util.py` & `titanq-0.9.2/tests/test_numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/tests/test_optimize_response.py` & `titanq-0.9.2/tests/test_optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/tests/test_variable.py` & `titanq-0.9.2/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/__init__.py` & `titanq-0.9.2/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_client/client.py` & `titanq-0.9.2/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_client/model.py` & `titanq-0.9.2/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_model/constraints.py` & `titanq-0.9.2/titanq/_model/constraints.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_model/errors.py` & `titanq-0.9.2/titanq/_model/errors.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_model/manifest.py` & `titanq-0.9.2/titanq/_model/manifest.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_model/model.py` & `titanq-0.9.2/titanq/_model/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,99 +26,111 @@
     reshape_to_2d,
     validate_cardinalities
 )
 from .variable_list import VariableVectorList
 
 log = logging.getLogger("TitanQ")
 
-_TITANQ_BASE_URL = "https://titanq.infinityq.io"
-
 
 class Model:
     """
-    Root object to define a problem to be optimize
+    Root object to define a problem to be optimized
     """
 
     def __init__(
         self,
         *,
         api_key: str,
         storage_client: StorageClient = None,
-        base_server_url: str = _TITANQ_BASE_URL
+        base_server_url: str = "https://titanq.infinityq.io"
         ) -> None:
         """
-        Initiate the model with a storage client depending on the provided arguments.
-
-        If the storage_client is missing, the storage will be managed by TitanQ.
-
-        NOTE: the storage manged by TitanQ supports weight matrices with a size up to 10k
-
-        :param api_key: TitanQ api key to access the service.
-        :param storage_client: Storage to choose in order to store some items
-        :param base_server_url: TitanQ server url
-
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model, S3Storage
+        Initiate the model with a storage client. If the storage_client is missing, the storage will be managed by TitanQ.
 
-        # s3 storage on AWS
-        model = Model(
-            api_key="{insert API key here}",
-            storage_client=S3Storage(
+        Notes
+        -----
+        The storage manged by TitanQ supports weight matrices with a size up to 10k only.
+
+        Parameters
+        ----------
+        api_key
+            TitanQ API key to access the service.
+        storage_client
+            Storage to choose in order to store some items.
+        base_server_url
+            TitanQ API server url, default set to ``https://titanq.infinityq.io``.
+
+        Examples
+        --------
+        With an S3 storage client
+            >>> from titanq import Model, S3Storage
+            >>> api_key = "{insert API key here}",
+            >>> storage_client = S3Storage(
                 access_key="{insert aws bucket access key here}",
                 secret_key="{insert aws bucket secret key here}",
                 bucket_name="{insert bucket name here}"
             )
-        )
+            >>> model = Model(api_key, storage_client)
 
-        # managed Storage (Up to 10k variables only)
-        model = Model(api_key="{insert API key here}")
+        Managed storage client
+            >>> from titanq import Model, S3Storage
+            >>> api_key = "{insert API key here}",
+            >>> model = Model(api_key)
         """
         self._variables = VariableVectorList()
         self._objective: Objective = None
         self._constraints = Constraints()
         self._titanq_client = Client(api_key, base_server_url)
         self._manifest: Manifest = Manifest()
 
         # the user chose a managed storage or left it as default
         if storage_client is None:
             storage_client = ManagedStorage(self._titanq_client)
 
         self._storage_client = storage_client
 
 
-    def add_variable_vector(self, name='', size=1, vtype=Vtype.BINARY, variable_bounds: Union[List[Tuple[int, int]], List[Tuple[float, float]]]=[]):
+    def add_variable_vector(
+        self,
+        name: str = '',
+        size: int = 1,
+        vtype: Vtype = Vtype.BINARY,
+        variable_bounds: Union[List[Tuple[int, int]], List[Tuple[float, float]]]=[]
+    ):
         """
-        Add a vector of variable to the model. Multiple variable vectors can be set but with different names.
+        Add a vector of variable to the model. Multiple variables vector can be added but with different names.
 
+        Notes
+        -----
         If Vtype is set to ``Vtype.INTEGER`` or ``Vtype.CONTINUOUS``, variable_bounds need to be set.
 
-        :param name: The name given to this variable vector.
-        :param size: The size of the vector.
-        :param vtype: Type of the variables inside the vector.
-        :param variable_bounds: Lower and upper bounds for the variable vector.
-
-        :raises MaximumVariableLimitError: If a variable is already defined.
-        :raises ValueError: If the size of the vector is < 1.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model, Vtype
-
-        # set up model
-        ...
-
-        model.add_variable_vector('x', 3, Vtype.BINARY)
-        model.add_variable_vector('y', 3, Vtype.INTEGER, [[0, 5], [1, 6]])
-        model.add_variable_vector('z', 3, Vtype.CONTINUOUS, [[2.3, 4.6], [3.1, 5.3], [1.1, 4]])
+        Parameters
+        ----------
+        name
+            The name given to this variable vector.
+        size
+            The size of the vector.
+        vtype
+            Type of the variables inside the vector.
+        variable_bounds
+            Lower and upper bounds for the variable vector. A list of tuples (can be either integers or continuous)
+
+        Raises
+        ------
+        MaximumVariableLimitError
+            If the total size of variables exceed the limit.
+        ValueError
+            If the size of the vector is < 1
+
+        Examples
+        --------
+        >>> from titanq import Model, Vtype
+        >>> model.add_variable_vector('x', 3, Vtype.BINARY)
+        >>> model.add_variable_vector('y', 3, Vtype.INTEGER, [[0, 5], [1, 6]])
+        >>> model.add_variable_vector('z', 3, Vtype.CONTINUOUS, [[2.3, 4.6], [3.1, 5.3], [1.1, 4]])
         """
         # validation
         if not self._constraints.is_empty():
             raise ConstraintAlreadySetError("Cannot add additional variable once constraints have been defined")
 
         if self._objective is not None:
             raise ObjectiveAlreadySetError("Cannot add additional variable once objective have been defined")
@@ -145,54 +157,51 @@
 
         self._variables.add(variables)
         self._constraints.augment_size(size)
 
         log.debug(f"add variable name='{name}', type={str(vtype)}, size={size}.")
 
 
-
     def set_objective_matrices(self, weights: np.ndarray, bias: np.ndarray, target=Target.MINIMIZE):
         """
         Set the objective matrices for the model.
 
-        :param weights: The quadratic objective matrix, **this matrix needs to be symmetrical**
-        :type weights: a NumPy 2-D dense ndarray (must be float32)
-
-        :param bias: The linear constraint vector
-        :type bias:  a NumPy 1-D ndarray
-
-        :param target: The target of this objective matrix.
-        :type target: Target Enum
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises ObjectiveAlreadySetError: If an objective has already been setted in this model.
-        :raises ValueError: If the weights shape or the bias shape does not fit the variable in the model.
-        :raises ValueError: If the weights or bias data type is not f32.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model, Target
-
-        edges = {0:[4,5,6,7], 1:[4,5,6,7], 2:[4,5,6,7], 3:[4,5,6,7], 4:[0,1,2,3], 5:[0,1,2,3], 6:[0,1,2,3], 7:[0,1,2,3]}
-        size = len(edges)
-
-        # construct the weight matrix from the edges list
-        weights = np.zeros((size, size), dtype=np.float32)
-        for root, connections in edges.items():
-            for c in connections:
-                weights[root][c] = 1
-
-        # construct the bias vector (Uniform weighting across all nodes)
-        bias = np.asarray([0]*size, dtype=np.float32)
-
-        model.set_objective_matrices(weights, bias, Target.MINIMIZE)
+        Parameters
+        ----------
+        weights
+            The quadratic objective matrix, **this matrix needs to be symmetrical**.
+            A NumPy 2-D dense ndarray (must be float32).
+        bias
+            The linear constraint vector. A NumPy 1-D ndarray.
+        target
+            The target of this objective matrix.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        ObjectiveAlreadySetError
+            If an objective has already been set in this model.
+        ValueError
+            If the weights shape or the bias shape does not fit the variables in the model.
+            If the weights or bias data type is not float32.
+
+        Examples
+        --------
+        >>> from titanq import Model, Target
+        >>> edges = {0:[4,5,6,7], 1:[4,5,6,7], 2:[4,5,6,7], 3:[4,5,6,7], 4:[0,1,2,3], 5:[0,1,2,3], 6:[0,1,2,3], 7:[0,1,2,3]}
+        >>> size = len(edges)
+        >>> weights = np.zeros((size, size), dtype=np.float32)
+        >>> for root, connections in edges.items():
+        >>>     for c in connections:
+        >>>         weights[root][c] = 1
+        >>> # construct the bias vector (Uniform weighting across all nodes)
+        >>> bias = np.asarray([0]*size, dtype=np.float32)
+        >>> model.set_objective_matrices(weights, bias, Target.MINIMIZE)
         """
-
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set objective before adding a variable to the model.")
 
         if self._objective is not None:
             raise ObjectiveAlreadySetError("An objective has already have been set for this model.")
 
         log.debug(f"set objective matrix and bias vector.")
@@ -200,33 +209,35 @@
         self._objective = Objective(self._variables.total_variable_size(), weights, bias, target)
 
 
     def add_set_partitioning_constraints_matrix(self, constraint_mask: np.ndarray):
         """
         Adds set partitioning constraints in matrix format to the model.
 
-        :param constraint_mask: The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
-        :type constraint_mask: A NumPy 2-D dense ndarray (must be binary)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask data type is not binary.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
-        model.add_set_partitioning_constraints_matrix(constraint_mask)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 2-D dense ndarray (must be binary).
+            The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraints exceed the limit.
+        ConstraintSizeError
+            If the constraint_mask shape does not fit the expected shape of this model.
+        ValueError
+            If the constraint_mask data type is not binary.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
+        >>> model.add_set_partitioning_constraints_matrix(constraint_mask)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_set_partitioning_constraints_matrix() function with a vector, " \
@@ -241,69 +252,73 @@
         )
         self._manifest.activate_set_partitioning_constraint()
 
     def add_set_partitioning_constraint(self, constraint_mask: np.ndarray):
         """
         Adds set partitioning constraint vector to the model.
 
-        :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
-        :type constraint_mask: A NumPy 1-D dense ndarray (must be binary)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask data type is not binary.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([1, 1, 1, 0, 1])
-        model.add_set_partitioning_constraint(constraint_mask)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 1-D dense ndarray (must be binary).
+            The constraint_mask vector of shape (N,) where N is the number of variables.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ConstraintSizeError
+            If the constraint_mask shape does not fit the expected shape of this model.
+        ValueError
+            If the constraint_mask data type is not binary.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([1, 1, 1, 0, 1])
+        >>> model.add_set_partitioning_constraint(constraint_mask)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use this add_set_partitioning_constraint() function with a matrix, " \
                 "please use add_set_partitioning_constraints_matrix() instead")
 
         self.add_set_partitioning_constraints_matrix(reshape_to_2d(constraint_mask))
 
 
     def add_cardinality_constraints_matrix(self, constraint_mask: np.ndarray, cardinalities: np.ndarray):
         """
         Adds cardinality constraints in matrix format to the model.
 
-        :param constraint_mask: The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
-        :type constraint_mask: a NumPy 2-D dense ndarray (must be binary)
-
-        :param cardinalities: The constraint_rhs vector of shape (M,) where M is the number of constraints
-        :type cardinalities:  a NumPy 1-D ndarray (must be non-zero unsigned integer)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask is not binary or cardinalities data type is not unsigned integer.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
-        cardinalities = np.array([3, 2])
-        model.add_cardinality_constraints_matrix(constraint_mask, cardinalities)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 2-D dense ndarray (must be binary).
+            The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
+        cardinalities
+            A NumPy 1-D ndarray (must be non-zero unsigned integer).
+            The constraint_rhs vector of shape (M,) where M is the number of constraints.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ConstraintSizeError
+            If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
+        ValueError
+            If the constraint_mask is not binary or cardinalities data type are not unsigned integers.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
+        >>> cardinalities = np.array([3, 2])
+        >>> model.add_cardinality_constraints_matrix(constraint_mask, cardinalities)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_cardinality_constraints_matrix() function with a vector, " \
@@ -333,75 +348,79 @@
             constraint_bounds=np.repeat(cardinalities, 2).reshape(-1, 2)
         )
         self._manifest.activate_cardinality_constraint()
 
 
     def add_cardinality_constraint(self, constraint_mask: np.ndarray, cardinality: int):
         """
-        Adds cardinality constraints vector to the model.
-
-        :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
-        :type constraint_mask: a NumPy 1-D dense ndarray (must be binary)
+        Adds cardinality constraint vector to the model.
 
-        :param cardinality: The constraint_rhs vector of shape (M,) where M is the number of constraints
-        :type cardinality:  a non-zero unsigned integer
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask is not binary or constraint_rhs data type is not unsigned integer.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([1, 1, 1, 0, 1])
-        cardinality = 3
-        model.add_cardinality_constraint(constraint_mask, cardinality)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 1-D dense ndarray (must be binary).
+            The constraint_mask vector of shape (N,) where N is the number of variables.
+        cardinality
+            The constraint_rhs cardinality.
+            This value has to be a non-zero unsigned integer.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            If the number of constraints exceed the limit.
+        ConstraintSizeError
+            If the constraint_mask shape or the constraint_rhs shape does not fit
+            the expected shape of this model.
+        ValueError
+            If the constraint_mask is not in binary or the cardinality is not an unsigned integer.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([1, 1, 1, 0, 1])
+        >>> cardinality = 3
+        >>> model.add_cardinality_constraint(constraint_mask, cardinality)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_cardinality_constraint() function with a matrix, " \
                 "please use add_cardinality_constraints_matrix() instead")
 
         self.add_cardinality_constraints_matrix(reshape_to_2d(constraint_mask), np.full((1,), cardinality))
 
 
     def add_equality_constraints_matrix(self, constraint_mask: np.ndarray, limit: np.ndarray) -> None:
         """
         Adds an equality constraint matrix to the model.
 
-        :param constraint_mask: The constraint_mask vector of shape (M, N) where M the number of constraints and N is the number of variables.
-        :type constraint_mask: A NumPy 2-D dense ndarray (float32)
-        :param limit: The limit vector of shape (M,) where M is the number of constraints
-        :type limit: A NumPy 1-D array (float32)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exceed the limit.
-        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32)
-        limit = np.array([2, 10], dtype=np.float32)
-
-        model.add_equality_constraints_matrix(constraint_mask, limit)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 2-D dense ndarray (float32).
+            The constraint_mask vector of shape (M, N) where M the number of constraints and N is the number of variables.
+        limit
+            A NumPy 1-D array (float32).
+            The limit vector of shape (M,) where M is the number of constraints.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ValueError
+            If the constraint_mask shape does not fit the expected shape of this model.
+            If the constraint_mask or limit contains irregular format ('NaN' or 'inf').
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32)
+        >>> limit = np.array([2, 10], dtype=np.float32)
+        >>> model.add_equality_constraints_matrix(constraint_mask, limit)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.dtype != np.float32 or limit.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {limit.dtype}")
 
@@ -428,74 +447,75 @@
         )
         self._manifest.activate_equality_constraint()
 
     def add_equality_constraint(self, constraint_mask: np.ndarray, limit: np.float32) -> None:
         """
         Adds an equality constraint vector to the model.
 
-        :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
-        :type constraint_mask: a NumPy 1-D dense ndarray (float32)
-        :param limit: Limit value to the constraint mask
-        :type limit: np.float32
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
-        limit = -3.45
-
-        model.add_equality_constraint(constraint_mask, limit)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 1-D dense ndarray (float32).
+            The constraint_mask vector of shape (N,) where N is the number of variables.
+        limit
+            Limit value to the constraint mask.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ValueError
+            If the constraint_mask shape does not fit the expected shape of this model.
+            If the constraint_mask or limit contains irregular format ('NaN' or 'inf').
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
+        >>> limit = -3.45
+        >>> model.add_equality_constraint(constraint_mask, limit)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_equality_constraint() function with a matrix, " \
                 "please use add_equality_constraint_matrix() instead")
 
         self.add_equality_constraints_matrix(reshape_to_2d(constraint_mask), np.full((1,), limit, dtype=np.float32))
 
 
     def add_inequality_constraints_matrix(self, constraint_mask: np.ndarray, constraint_bounds: np.ndarray):
         """
         Adds inequality constraint matrix to the model.
 
-        :param constraint_mask: The constraint_mask vector of shape (M, N) where N is the number of variables.
-        :type constraint_mask: A NumPy 2-D dense ndarray (float32)
-        :param constraints_bounds: Vector of shape (M, 2) where M is the number of constraints
-        :type constraint_bounds: A NumPy 2-D ndarray (float32)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: A lowerbound is equal or higher than its given upperbound
-        :raises ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([[-3.51, 0], [10, 0]], dtype=np.float32)
-        constraint_bounds = np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32)
-
-        model.add_inequality_constraints_matrix(constraint_mask, constraint_bounds)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 2-D dense ndarray (float32).
+            The constraint_mask vector of shape (M, N) where N is the number of variables.
+        constraint_bounds
+            A NumPy 2-D ndarray (float32).
+            Vector of shape (M, 2) where M is the number of constraints.
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ValueError
+            If the constraint_mask shape does not fit the expected shape of this model.
+            If the constraint_mask contains irregular format ('NaN' or 'inf').
+            If the lowerbound is equal or higher than its given upperbound.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([[-3.51, 0], [10, 0]], dtype=np.float32)
+        >>> constraint_bounds = np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32)
+        >>> model.add_inequality_constraints_matrix(constraint_mask, constraint_bounds)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.dtype != np.float32 or constraint_bounds.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {constraint_bounds.dtype}")
 
@@ -517,91 +537,108 @@
         self._manifest.activate_inequality_constraint()
 
 
     def add_inequality_constraint(self, constraint_mask: np.ndarray, constraint_bounds: np.ndarray):
         """
         Adds inequality constraint vector to the model. At least one bound must be set.
 
-        :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
-        :type constraint_mask: A NumPy 1-D dense ndarray (float32)
-        :param constraints_bounds: Vector of shape (2,)
-        :type constraint_bounds: A NumPy 1-D ndarray (float32)
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raises ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
-        :raises ValueError: Lowerbound is equal or higher than the upperbound
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model
-        ...
-
-        constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
-        constraint_bounds = np.array([1.0, np.nan], dtype=np.float32)
-
-        model.add_inequality_constraint(constraint_mask, constraint_bounds)
+        Parameters
+        ----------
+        constraint_mask
+            A NumPy 1-D dense ndarray (float32).
+            The constraint_mask vector of shape (N,) where N is the number of variables.
+        constraint_bounds
+            A NumPy 1-D ndarray (float32).
+            Vector of shape (2,)
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MaximumConstraintLimitError
+            The number of constraint exceed the limit.
+        ValueError
+            If the constraint_mask shape does not fit the expected shape of this model.
+            If the constraint_mask contains irregular format ('NaN' or 'inf').
+            If the lowerbound is equal or higher than the upperbound.
+
+        Examples
+        --------
+        >>> constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
+        >>> constraint_bounds = np.array([1.0, np.nan], dtype=np.float32)
+        >>> model.add_inequality_constraint(constraint_mask, constraint_bounds)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_inequality_constraint() function with a matrix, " \
                 "please use add_inequality_constraint_matrix() instead")
 
         self.add_inequality_constraints_matrix(reshape_to_2d(constraint_mask), reshape_to_2d(constraint_bounds))
 
 
-    def optimize(self, *, beta=[0.1], coupling_mult=0.5, timeout_in_secs=10.0, num_chains=8, num_engines=1, normalized=False):
+    def optimize(
+        self,
+        *,
+        beta: List[float] = [0.1],
+        coupling_mult: float = 0.5,
+        timeout_in_secs: float = 10.0,
+        num_chains: int = 8,
+        num_engines: int = 1,
+        normalized: bool = False
+    ) -> OptimizeResponse:
         """
         Optimize this model.
 
-        Note: All of the files used during the computation will be cleaned at the end.
-
-        :param beta: ``beta`` hyper parameter used by the solver.
-        :param coupling_mult: ``coupling_mult`` hyper parameter used by the solver.
-        :param timeout_in_secs: Maximum time (in seconds) the solver can take to resolve this problem.
-        :param num_chains: ``num_chains`` hyper parameter used by the solver.
-        :param num_engines: ``num_engines`` parameter used by the solver.
-
-        :param normalized: DEPRECATED ``normalized`` parameter used by the solver, this will be removed.
-        Note: ``normalized`` should only be used when the model is only using binary or bipolar variables and does not contain any constraints
-
-        For more information on how to tunes those parameters, visit the API doc at `https://docs.titanq.infinityq.io/`
-
-        :raises MissingVariableError: If no variable have been added to the model.
-        :raises MissingObjectiveError: If no variable have been added to the model.
-
-        Example
-        ~~~~~~~
-        ..  highlight:: python
-        ..  code-block:: python
-        from titanq import Model
-
-        # set up model, objective and variable
-        ...
-
-        # basic solve
-        response = model.optimize(timeout_in_secs=60)
-
-        # multiple engine
-        response = model.optimize(timeout_in_secs=60, num_engines=2)
-
-        # custom values
-        response = model.optimize(beta=[0.1], coupling_mult=0.75, num_chains=8)
-
-        # print values
-        print("-" * 15, "+", "-" * 26, sep="")
-        print("Ising energy   | Result vector")
-        print("-" * 15, "+", "-" * 26, sep="")
-        for ising_energy, result_vector in response.result_items():
-            print(f"{ising_energy: <14f} | {result_vector}")
+        Notes
+        -----
+        All of the files used during this computation will be cleaned at the end.
+        For more information on how to tunes those parameters, visit the API doc at `TitanQ API <https://docs.titanq.infinityq.io/>`_.
+
+        Parameters
+        ----------
+        beta
+            ``beta`` hyper parameter used by the solver.
+        coupling_mult
+            ``coupling_mult`` hyper parameter used by the solver.
+        timeout_in_secs
+            Maximum time (in seconds) the solver can take to solve this problem.
+        num_chains
+            ``num_chains`` hyper parameter used by the solver.
+        num_engines
+            ``num_engines`` parameter used by the solver.
+        normalized
+            **DEPRECATED since version 0.9.1**. ``normalized`` should only be used when the model is only using
+            binary or bipolar variables and does not contain any constraints.
+
+        Returns
+        -------
+        OptimizeResponse
+            Optimized response data object
+
+        Raises
+        ------
+        MissingVariableError
+            If no variable have been added to the model.
+        MissingObjectiveError
+            If no objective matrices have been added to the model.
+
+        Examples
+        --------
+        basic solve
+            >>> response = model.optimize(timeout_in_secs=60)
+        multiple engine
+            >>> response = model.optimize(timeout_in_secs=60, num_engines=2)
+        custom values
+            >>> response = model.optimize(beta=[0.1], coupling_mult=0.75, num_chains=8)
+        print values
+            >>> print("-" * 15, "+", "-" * 26, sep="")
+            >>> print("Ising energy   | Result vector")
+            >>> print("-" * 15, "+", "-" * 26, sep="")
+            >>> for ising_energy, result_vector in response.result_items():
+            >>>     print(f"{ising_energy: <14f} | {result_vector}")
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot optimize before adding a variable to the model.")
 
         if self._objective is None:
             raise MissingObjectiveError("Cannot optimize before adding an objective to the model.")
 
@@ -616,21 +653,31 @@
             num_chains: int,
             num_engines: int,
             normalized: bool
         ) -> Tuple[np.ndarray, Dict[str, Any]]:
         """
         issue a solve request and wait for it to complete.
 
-        :param beta: beta hyper parameter used by the backend solver.
-        :param coupling_mult: coupling_mult hyper parameter used by the backend solver.
-        :param timeout_in_secs: Maximum time (in seconds) the backend solver can take to resolve this problem.
-        :param num_chains: num_chains hyper parameter used by the backend solver.
-        :param num_engines: num_engines parameter used by the backend solver.
-
-        :return: the result numpy array and the metric json object
+        Parameters
+        ----------
+        beta
+            beta hyper parameter used by the backend solver.
+        coupling_mult
+            coupling_mult hyper parameter used by the backend solver.
+        timeout_in_secs
+            Maximum time (in seconds) the backend solver can take to resolve this problem.
+        num_chains
+            num_chains hyper parameter used by the backend solver.
+        num_engines
+            num_engines parameter used by the backend solver.
+        normalized
+
+        Returns
+        -------
+        The result numpy array and the metric json object.
         """
         with self._storage_client.temp_files_manager(
             self._objective.bias(),
             self._objective.weights(),
             self._constraints.bounds() if self._constraints else None,
             self._constraints.weights() if self._constraints else None,
             # variables bounds is only sent if variable is set to binary
```

### Comparing `titanq-0.9.1/titanq/_model/numpy_util.py` & `titanq-0.9.2/titanq/_model/numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_model/objective.py` & `titanq-0.9.2/titanq/_model/objective.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import enum
 from typing import Tuple
 
 import numpy as np
 
 
 class Target(enum.Enum):
+    """
+    All target types currently supported by the solver
+    """
+
     MINIMIZE = 'minimize'
 
 
 def _verify_nd_array(array: np.ndarray, array_name: str, *, expected_shape: Tuple, expected_type: np.dtype):
     """
     Make sure the given array is the right shape and the right type.
```

### Comparing `titanq-0.9.1/titanq/_model/optimize_response.py` & `titanq-0.9.2/titanq/_model/optimize_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""
+``OptimizeResponse`` data object that is returned from the model when optimizing a problem.
+"""
+
 import logging
 from typing import Any, Dict, List, Tuple, Union
 import uuid
 import warnings
 
 import numpy as np
 
 from .variable_list import VariableVectorList
 
 log = logging.getLogger('TitanQ')
 
 class OptimizeResponse:
     """
-    Object containing Optimization response and all its metrics.
+    Object containing the optimization results and all of the metrics returned by the solver.
     """
     def __init__(self, variable_list: VariableVectorList, result_array: np.ndarray, metrics: Dict[str, Any]) -> None:
         self._result_by_variable: Dict[str, np.ndarray] = {}
         start_index = 0
 
         # extract all the result for each given variable
         # The result array is a 2d array where each line is a different result of the same problem
@@ -73,76 +77,103 @@
             return self._metrics[attr]
         except KeyError:
             raise AttributeError(attr)
 
 
     def result_vector(self) -> np.ndarray:
         """
-        :return: The result vector of this optimization.
+        The result vector
+
+        Returns
+        -------
+        The result vector of this optimization.
         """
         return self._all_results
 
 
     def result_items(self) -> List[Tuple[int, np.ndarray]]:
         """
         ex. [(-10000, [0, 1, 1, 0]), (-20000, [1, 0, 1, 0]), ...]
 
-        :return: list of tuples containing the solutions objective value and it's corresponding result vector
+        Returns
+        -------
+        List of tuples containing the solutions objective value and it's corresponding result vector
         """
 
         solutions_objective_value = self.ising_energy
         return [(solutions_objective_value[i], self._all_results[i]) for i in range(len(self._all_results))]
 
 
     def computation_metrics(self, key: str = None) -> Any:
         """
-        :return: All computation metrics if no key is given of the specific metrics with the associated key if one is provided.
+        The computation metrics the solver returnes
 
-        :raise KeyError: The given key does not exist
+        Returns
+        -------
+        All computation metrics if no key is given of the specific metrics with the associated key if one is provided.
+
+        Raises
+        ------
+        KeyError
+            The given key does not exist.
         """
         metrics = self._metrics['computation_metrics']
         if key:
             metrics = metrics[key]
         return metrics
 
 
     def computation_id(self) -> uuid.UUID:
         """
         The computation id is a Universal unique id that identify this computation inside the TitanQ platform.
 
         Provide this id on any support request to the InfinityQ.
 
-        :return: The computation id of this solve.
+        Returns
+        -------
+        The computation id of this solve.
         """
         return self._metrics['computation_id']
 
 
     def original_input_params(self, key: str = None) -> Any:
         """
-        :return: All original params if no key is given of the specific params with the associated key if one is provided.
+        The original input params sent to the solver
 
-        :raise KeyError: The given key does not exist
+        Returns
+        -------
+        All original params if no key is given. A specific param with the associated key if one is provided.
+
+        Raises
+        ------
+        KeyError
+            The given key does not exist
         """
         metrics = self._metrics['original_input_params']
         if key:
             metrics = metrics[key]
         return metrics
 
 
     def metrics(self, key: str = None) -> Union[str, Dict[str, Any]]:
         """
-        # Deprecated
-        use computation_metrics() or original_input_params instead
-
-        :return: All metrics if no key is given of the specific metrics with the associated key if one is provided.
+        .. deprecated:: 0.7.0
+            Use computation_metrics() or original_input_params() instead.
 
-        :raise KeyError: The given key does not exist
+        Returns
+        -------
+        All metrics if no key is given. A specific metric with the associated key if one is provided.
+
+        Raises
+        ------
+        KeyError
+            The given key does not exist
         """
         warnings.warn(
-            'Calling metrics() is deprecated. Use computation_metrics or original_input_params instead.',
+            'Calling metrics() is deprecated. Use computation_metrics() or original_input_params() instead.',
             DeprecationWarning,
             stacklevel=2
         )
         if key:
             return self._metrics[key]
         else:
             return self._metrics
```

### Comparing `titanq-0.9.1/titanq/_model/variable.py` & `titanq-0.9.2/titanq/_model/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import abc
 import enum
 from typing import List, Tuple
 import numpy as np
 from numpy._typing import NDArray
 
 class Vtype(str, enum.Enum):
+    """
+    All variables types currently supported by the solver
+    """
+
     BINARY = 'binary'
     BIPOLAR = 'bipolar'
     INTEGER = 'integer'
     CONTINUOUS = 'continuous'
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `titanq-0.9.1/titanq/_model/variable_list.py` & `titanq-0.9.2/titanq/_model/variable_list.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_storage/managed_storage.py` & `titanq-0.9.2/titanq/_storage/managed_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq/_storage/s3_storage.py` & `titanq-0.9.2/titanq/_storage/s3_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,22 +17,45 @@
 _CONSTRAINT_WEIGHTS_FILE = "constraints_weights.npy"
 _VARIABLE_BOUNDS_FILE = "variable_bounds.npy"
 _RESULT_FILE = "result.zip"
 
 
 
 class S3Storage(StorageClient):
-    def __init__(self, access_key, secret_key, bucket_name):
+    """Storage client using S3 bucket from AWS"""
+    def __init__(
+        self,
+        access_key: str,
+        secret_key: str,
+        bucket_name: str,
+    ) -> None:
         """
-        Initiate the s3 client for handling the temporary files.
-        If any aws argument is missing this will raise an exception.
+        Initiate the S3 bucket client for handling temporary files.
 
-        :param aws_access_key_id: aws access key id used to upload and download files from an aws bucket.
-        :param aws_secret_access_key: aws secret access key used to upload and download files from an aws bucket.
-        :param aws_bucket_name: name of the aws bucket use to store temporairly data use by the titanq optimizer backend.
+        Parameters
+        ----------
+        access_key
+            Used to upload and download files from an AWS S3 bucket.
+        secret_key
+            Used to upload and download files from an AWS S3 bucket.
+        bucket_name
+            Name of the AWS S3 bucket used to store temporarily data that the TitanQ optimizer will read.
+
+        Raises
+        ------
+        botocore.exceptions.ParamValidationError
+            If any AWS argument is missing this will raise an exception.
+
+        Examples
+        --------
+        >>> storage_client = S3Storage(
+        >>>     access_key="{insert aws bucket access key here}",
+        >>>     secret_key="{insert aws bucket secret key here}",
+        >>>     bucket_name="{insert bucket name here}"
+        >>> )
         """
         self._s3 = boto3.client('s3', aws_access_key_id=access_key, aws_secret_access_key=secret_key)
         self._access_key_id = access_key
         self._secret_access_key = secret_key
         self._bucket_name = bucket_name
 
         timestamp = datetime.datetime.now().isoformat()
@@ -44,15 +67,15 @@
     def _upload_arrays(
         self,
         bias: bytes,
         weights: bytes,
         constraint_bounds: Optional[bytes],
         constraint_weights: Optional[bytes],
         variable_bounds: Optional[bytes]
-        ) -> None:
+    ) -> None:
 
         upload_tuple = [
             (self._get_full_filename(_BIAS_FILE), bias),
             (self._get_full_filename(_WEIGHTS_FILE), weights)
         ]
 
         if constraint_bounds:
```

### Comparing `titanq-0.9.1/titanq/_storage/storage_client.py` & `titanq-0.9.2/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.1/titanq.egg-info/PKG-INFO` & `titanq-0.9.2/titanq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.1
+Version: 0.9.2
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
-Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
+Project-URL: Documentation, https://sdk.titanq.infinityq.io
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Programming Language :: Python :: 3
@@ -93,15 +93,15 @@
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
 
-Additional parameters are avialble to tune the problem:
+Additional parameters are available to tune the problem:
 - beta
 - coupling_mult
 - num_chains
 - num_engines
 
 For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
```

### Comparing `titanq-0.9.1/titanq.egg-info/SOURCES.txt` & `titanq-0.9.2/titanq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

