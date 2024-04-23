# Comparing `tmp/fse_baro-0.0.7.tar.gz` & `tmp/fse_baro-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.0.7.tar", last modified: Sat Apr 20 17:13:38 2024, max compression
+gzip compressed data, was "fse_baro-0.0.8.tar", last modified: Tue Apr 23 13:36:35 2024, max compression
```

## Comparing `fse_baro-0.0.7.tar` & `fse_baro-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.898778 fse_baro-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.898778 fse_baro-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 17:13:28.000000 fse_baro-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-20 17:13:38.902778 fse_baro-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-20 17:13:28.000000 fse_baro-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-20 17:13:28.000000 fse_baro-0.0.7/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-20 17:13:28.000000 fse_baro-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:13:38.902778 fse_baro-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-20 17:13:28.000000 fse_baro-0.0.7/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-20 17:13:28.000000 fse_baro-0.0.7/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.808563 fse_baro-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.808563 fse_baro-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 13:36:30.000000 fse_baro-0.0.8/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-23 13:36:30.000000 fse_baro-0.0.8/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 13:36:30.000000 fse_baro-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 13:36:35.812563 fse_baro-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-23 13:36:30.000000 fse_baro-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 13:36:30.000000 fse_baro-0.0.8/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 13:36:30.000000 fse_baro-0.0.8/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 13:36:30.000000 fse_baro-0.0.8/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 13:36:30.000000 fse_baro-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:36:35.812563 fse_baro-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-23 13:36:30.000000 fse_baro-0.0.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-23 13:36:30.000000 fse_baro-0.0.8/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.0.7/.github/workflows/build-and-test.yml` & `fse_baro-0.0.8/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/.github/workflows/python-publish.yml` & `fse_baro-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/.gitignore` & `fse_baro-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/LICENSE` & `fse_baro-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/PKG-INFO` & `fse_baro-0.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.7
+Version: 0.0.8
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,35 +38,16 @@
 Requires-Dist: matplotlib
 
 # BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
 [![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
 
+BARO is an end-to-end approach to perform anomaly detection and root cause analysis for microservices's failures. This repository contains the artifact for reproducing the main experimental results in our paper accepted to ESEC/FSE 2024, and reusing purposes.
 
-In the progress of preparing the Artifact submission:
-- Deadline 30/4
-- https://2024.esec-fse.org/track/fse-2024-artifacts#submission-for-replicated-and-reproduced-badges
-- Can apply for all three badges: Available, Function, Reusable
-
-**Functional: The artifacts associated with the research are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation.	
-**
-
-**Reusable: Functional + the artifacts associated with the paper are of a quality that significantly exceeds minimal functionality. They are very carefully documented and well-structured to the extent that reuse and repurposing is facilitated. In particular, norms and standards of the research community for artifacts of this type are strictly adhered to.	
-**
-
-TODO:
-
-- [x] reproduce RobustScorer
-- [ ] reproduce BOCPD
-- [ ] make docs directly on readme, show available AD + RCA methods + tutorials
-- [ ] make the API
-- [ ] restructure + lint code
-- [ ] better readme
-- [ ] make a Helm chart
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/fse-baro)
 
 ```bash
 pip install fse-baro
@@ -75,14 +56,16 @@
 Or, build from source
 
 ```bash
 git clone https://github.com/phamquiluan/baro.git && cd baro
 pip install -e .
 ```
 
+More details are in [INSTALLATION.md](INSTALLATION.md).
+
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
 from baro import BARO
@@ -96,24 +79,31 @@
 
 ## Download Paper
 
 TBD
 
 ## Download Datasets
 
-TBD 
+Our datasets are publicly available in Zenodo repository with the following information:
+
+- Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11046533.svg)](https://doi.org/10.5281/zenodo.11046533)
+- Dataset URL: https://zenodo.org/records/11046533
 
-## Performance comparison
+## Reproducibility
 
-TBD 
+Check the Jupyter Notebook at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb) to reproduce the performance of BARO.
 
 ## Citation
 
 ```
 @inproceedings{pham2024baro,
   title={BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection},
   author={Luan Pham, Huong Ha, and Hongyu Zhang},
-  booktitle={Proceedings of the 32nd ACM Symposium on the Foundations of Software Engineering (FSE'24)},
+  booktitle={Proceedings of the ACM on Software Engineering, Vol 1},
   year={2024},
   organization={ACM}
 }
 ```
+
+## Contact
+
+[luan.pham\@rmit.edu.au](mailto:luan.pham@rmit.edu.au?subject=BARO)
```

### Comparing `fse_baro-0.0.7/baro/_bocpd.py` & `fse_baro-0.0.8/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/baro/anomaly_detection.py` & `fse_baro-0.0.8/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/baro/root_cause_analysis.py` & `fse_baro-0.0.8/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/baro/utility.py` & `fse_baro-0.0.8/baro/utility.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.0.8/fse_baro.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.7
+Version: 0.0.8
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,35 +38,16 @@
 Requires-Dist: matplotlib
 
 # BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
 [![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
 
+BARO is an end-to-end approach to perform anomaly detection and root cause analysis for microservices's failures. This repository contains the artifact for reproducing the main experimental results in our paper accepted to ESEC/FSE 2024, and reusing purposes.
 
-In the progress of preparing the Artifact submission:
-- Deadline 30/4
-- https://2024.esec-fse.org/track/fse-2024-artifacts#submission-for-replicated-and-reproduced-badges
-- Can apply for all three badges: Available, Function, Reusable
-
-**Functional: The artifacts associated with the research are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation.	
-**
-
-**Reusable: Functional + the artifacts associated with the paper are of a quality that significantly exceeds minimal functionality. They are very carefully documented and well-structured to the extent that reuse and repurposing is facilitated. In particular, norms and standards of the research community for artifacts of this type are strictly adhered to.	
-**
-
-TODO:
-
-- [x] reproduce RobustScorer
-- [ ] reproduce BOCPD
-- [ ] make docs directly on readme, show available AD + RCA methods + tutorials
-- [ ] make the API
-- [ ] restructure + lint code
-- [ ] better readme
-- [ ] make a Helm chart
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/fse-baro)
 
 ```bash
 pip install fse-baro
@@ -75,14 +56,16 @@
 Or, build from source
 
 ```bash
 git clone https://github.com/phamquiluan/baro.git && cd baro
 pip install -e .
 ```
 
+More details are in [INSTALLATION.md](INSTALLATION.md).
+
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
 from baro import BARO
@@ -96,24 +79,31 @@
 
 ## Download Paper
 
 TBD
 
 ## Download Datasets
 
-TBD 
+Our datasets are publicly available in Zenodo repository with the following information:
+
+- Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11046533.svg)](https://doi.org/10.5281/zenodo.11046533)
+- Dataset URL: https://zenodo.org/records/11046533
 
-## Performance comparison
+## Reproducibility
 
-TBD 
+Check the Jupyter Notebook at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb) to reproduce the performance of BARO.
 
 ## Citation
 
 ```
 @inproceedings{pham2024baro,
   title={BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection},
   author={Luan Pham, Huong Ha, and Hongyu Zhang},
-  booktitle={Proceedings of the 32nd ACM Symposium on the Foundations of Software Engineering (FSE'24)},
+  booktitle={Proceedings of the ACM on Software Engineering, Vol 1},
   year={2024},
   organization={ACM}
 }
 ```
+
+## Contact
+
+[luan.pham\@rmit.edu.au](mailto:luan.pham@rmit.edu.au?subject=BARO)
```

### Comparing `fse_baro-0.0.7/main.py` & `fse_baro-0.0.8/main.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/pyproject.toml` & `fse_baro-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/tests/test.py` & `fse_baro-0.0.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.7/tutorials/reproducibility.ipynb` & `fse_baro-0.0.8/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

