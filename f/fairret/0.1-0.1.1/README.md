# Comparing `tmp/fairret-0.1.tar.gz` & `tmp/fairret-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairret-0.1.tar", last modified: Tue Feb 13 16:14:26 2024, max compression
+gzip compressed data, was "fairret-0.1.1.tar", last modified: Tue Apr 23 16:02:20 2024, max compression
```

## Comparing `fairret-0.1.tar` & `fairret-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 16:14:26.590060 fairret-0.1/
--rw-rw-rw-   0        0        0     1141 2024-01-23 13:54:55.000000 fairret-0.1/LICENSE
--rw-rw-rw-   0        0        0     5171 2024-02-13 16:14:26.590060 fairret-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3399 2024-02-08 18:00:23.000000 fairret-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-13 16:14:26.570059 fairret-0.1/fairret/
--rw-rw-rw-   0        0        0        0 2024-02-08 17:53:11.000000 fairret-0.1/fairret/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 16:14:26.580065 fairret-0.1/fairret/loss/
--rw-rw-rw-   0        0        0      275 2024-02-08 17:53:11.000000 fairret-0.1/fairret/loss/__init__.py
--rw-rw-rw-   0        0        0      151 2024-02-08 17:25:56.000000 fairret-0.1/fairret/loss/base.py
--rw-rw-rw-   0        0        0     9374 2024-02-08 17:30:23.000000 fairret-0.1/fairret/loss/projection.py
--rw-rw-rw-   0        0        0     1271 2024-02-08 17:30:23.000000 fairret-0.1/fairret/loss/violation.py
--rw-rw-rw-   0        0        0     2003 2024-02-12 09:00:29.000000 fairret-0.1/fairret/metric.py
--rw-rw-rw-   0        0        0     5928 2024-02-09 16:16:04.000000 fairret-0.1/fairret/statistic.py
--rw-rw-rw-   0        0        0      582 2024-01-25 18:56:36.000000 fairret-0.1/fairret/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-13 16:14:26.580065 fairret-0.1/fairret.egg-info/
--rw-rw-rw-   0        0        0     5171 2024-02-13 16:14:26.000000 fairret-0.1/fairret.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-02-13 16:14:26.000000 fairret-0.1/fairret.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 16:14:26.000000 fairret-0.1/fairret.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-02-13 16:14:26.000000 fairret-0.1/fairret.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-13 16:14:26.000000 fairret-0.1/fairret.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2024-02-13 16:02:23.000000 fairret-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-13 16:14:26.590060 fairret-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-13 16:14:26.580065 fairret-0.1/test/
--rw-rw-rw-   0        0        0     1822 2024-02-09 15:24:43.000000 fairret-0.1/test/test_loss.py
--rw-rw-rw-   0        0        0     1221 2024-02-09 16:26:29.000000 fairret-0.1/test/test_metric.py
--rw-rw-rw-   0        0        0     1270 2024-02-09 15:24:43.000000 fairret-0.1/test/test_statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.189058 fairret-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 16:02:14.000000 fairret-0.1.1/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 16:02:14.000000 fairret-0.1.1/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-23 16:02:14.000000 fairret-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 16:02:14.000000 fairret-0.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-23 16:02:14.000000 fairret-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-23 16:02:20.201058 fairret-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-23 16:02:14.000000 fairret-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/_static/Overview_fairret.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/generated/fairret.loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/statistic.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    88620 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/complex_sensitive_features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/custom_statistic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/simple_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/stacked_statistic.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22496 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/linear_fractional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/fairret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 16:02:14.000000 fairret-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:02:20.201058 fairret-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_statistic.py
```

### Comparing `fairret-0.1/LICENSE` & `fairret-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `fairret-0.1/PKG-INFO` & `fairret-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,113 @@
-Metadata-Version: 2.1
-Name: fairret
-Version: 0.1
-Summary: A fairness library in PyTorch.
-Author-email: Maarten Buyl <maarten.buyl@ugent.be>
-License: MIT License
-        
-        Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Keywords: fairness,machine-learning,ai,artificial-intelligence,pytorch,deep-learning,python,bias,fairness-ai,fairness-ml
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: cvxpy
-Requires-Dist: torchmetrics
-
-# fairret - a fairness library in PyTorch
-The goal of `fairret` is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
-1. *flexible* in how fairness is defined and pursued.
-2. *easy* to integrate into existing PyTorch pipelines.
-3. *clear* in what its tools can and cannot do.
-
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
-
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
-# Quickstart
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
-
-```python
-import torch.nn.functional as F
-from fairret.statistic import PositiveRate
-from fairret.loss import NormLoss
-
-statistic = PositiveRate()
-norm_fairret = NormLoss(statistic)
-
-def train(model, optimizer, train_loader):
-     for feat, sens, target in train_loader:
-            optimizer.zero_grad()
-            
-            logit = model(feat)
-            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
-            fairret_loss = norm_fairret(logit, feat, sens, target)
-            loss = bce_loss + fairret_loss
-            loss.backward()
-            
-            optimizer.step()
-```
-
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
-
-A notebook wil a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
-
-# Warning: AI fairness != fairness
-There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
-
-More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
-
-# Future plans
-The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
-
-Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
-
-# Citation
-This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
-
-```bibtex
-@inproceedings{buyl2024fairret,
-    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
-    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
-    booktitle={International Conference on Learning Representations},
-    year={2024}
-}
-```
+Metadata-Version: 2.1
+Name: fairret
+Version: 0.1.1
+Summary: A fairness library in PyTorch.
+Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
+License: MIT License
+        
+        Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Keywords: fairness,machine-learning,ai,artificial-intelligence,pytorch,deep-learning,python,bias,fairness-ai,fairness-ml
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: numpy
+
+# fairret - a fairness library in PyTorch
+
+[![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
+![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
+[![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+
+## Description
+
+The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+1. *flexible* in how fairness is defined and pursued.
+2. *easy* to integrate into existing PyTorch pipelines.
+3. *clear* in what its tools can and cannot do.
+
+The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
+These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+
+**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+### Dependencies
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+
+## Quickstart
+
+It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+
+```python
+import torch.nn.functional as F
+from fairret.statistic import PositiveRate
+from fairret.loss import NormLoss
+
+statistic = PositiveRate()
+norm_fairret = NormLoss(statistic)
+
+def train(model, optimizer, train_loader):
+     for feat, sens, target in train_loader:
+            optimizer.zero_grad()
+            
+            logit = model(feat)
+            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
+            fairret_loss = norm_fairret(logit, sens)
+            loss = bce_loss + fairret_loss
+            loss.backward()
+            
+            optimizer.step()
+```
+
+No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+
+A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
+
+## Warning: AI fairness != fairness
+There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
+
+More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
+
+## Future plans
+The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
+
+Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
+
+## Citation
+This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
+
+```bibtex
+@inproceedings{buyl2024fairret,
+    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
+    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
+    booktitle={International Conference on Learning Representations},
+    year={2024}
+}
+```
```

### Comparing `fairret-0.1/README.md` & `fairret-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,79 @@
-# fairret - a fairness library in PyTorch
-The goal of `fairret` is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
-1. *flexible* in how fairness is defined and pursued.
-2. *easy* to integrate into existing PyTorch pipelines.
-3. *clear* in what its tools can and cannot do.
-
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
-
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
-# Quickstart
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
-
-```python
-import torch.nn.functional as F
-from fairret.statistic import PositiveRate
-from fairret.loss import NormLoss
-
-statistic = PositiveRate()
-norm_fairret = NormLoss(statistic)
-
-def train(model, optimizer, train_loader):
-     for feat, sens, target in train_loader:
-            optimizer.zero_grad()
-            
-            logit = model(feat)
-            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
-            fairret_loss = norm_fairret(logit, feat, sens, target)
-            loss = bce_loss + fairret_loss
-            loss.backward()
-            
-            optimizer.step()
-```
-
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
-
-A notebook wil a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
-
-# Warning: AI fairness != fairness
-There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
-
-More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
-
-# Future plans
-The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
-
-Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
-
-# Citation
-This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
-
-```bibtex
-@inproceedings{buyl2024fairret,
-    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
-    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
-    booktitle={International Conference on Learning Representations},
-    year={2024}
-}
-```
+# fairret - a fairness library in PyTorch
+
+[![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
+![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
+[![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+
+## Description
+
+The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+1. *flexible* in how fairness is defined and pursued.
+2. *easy* to integrate into existing PyTorch pipelines.
+3. *clear* in what its tools can and cannot do.
+
+The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
+These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+
+**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+### Dependencies
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+
+## Quickstart
+
+It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+
+```python
+import torch.nn.functional as F
+from fairret.statistic import PositiveRate
+from fairret.loss import NormLoss
+
+statistic = PositiveRate()
+norm_fairret = NormLoss(statistic)
+
+def train(model, optimizer, train_loader):
+     for feat, sens, target in train_loader:
+            optimizer.zero_grad()
+            
+            logit = model(feat)
+            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
+            fairret_loss = norm_fairret(logit, sens)
+            loss = bce_loss + fairret_loss
+            loss.backward()
+            
+            optimizer.step()
+```
+
+No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+
+A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
+
+## Warning: AI fairness != fairness
+There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
+
+More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
+
+## Future plans
+The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
+
+Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
+
+## Citation
+This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
+
+```bibtex
+@inproceedings{buyl2024fairret,
+    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
+    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
+    booktitle={International Conference on Learning Representations},
+    year={2024}
+}
+```
```

### Comparing `fairret-0.1/fairret.egg-info/PKG-INFO` & `fairret-0.1.1/fairret.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,113 @@
-Metadata-Version: 2.1
-Name: fairret
-Version: 0.1
-Summary: A fairness library in PyTorch.
-Author-email: Maarten Buyl <maarten.buyl@ugent.be>
-License: MIT License
-        
-        Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Keywords: fairness,machine-learning,ai,artificial-intelligence,pytorch,deep-learning,python,bias,fairness-ai,fairness-ml
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: cvxpy
-Requires-Dist: torchmetrics
-
-# fairret - a fairness library in PyTorch
-The goal of `fairret` is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
-1. *flexible* in how fairness is defined and pursued.
-2. *easy* to integrate into existing PyTorch pipelines.
-3. *clear* in what its tools can and cannot do.
-
-The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
-These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
-
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
-# Quickstart
-It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
-
-```python
-import torch.nn.functional as F
-from fairret.statistic import PositiveRate
-from fairret.loss import NormLoss
-
-statistic = PositiveRate()
-norm_fairret = NormLoss(statistic)
-
-def train(model, optimizer, train_loader):
-     for feat, sens, target in train_loader:
-            optimizer.zero_grad()
-            
-            logit = model(feat)
-            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
-            fairret_loss = norm_fairret(logit, feat, sens, target)
-            loss = bce_loss + fairret_loss
-            loss.backward()
-            
-            optimizer.step()
-```
-
-No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
-
-A notebook wil a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
-
-# Warning: AI fairness != fairness
-There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
-
-More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
-
-# Future plans
-The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
-
-Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
-
-# Citation
-This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
-
-```bibtex
-@inproceedings{buyl2024fairret,
-    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
-    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
-    booktitle={International Conference on Learning Representations},
-    year={2024}
-}
-```
+Metadata-Version: 2.1
+Name: fairret
+Version: 0.1.1
+Summary: A fairness library in PyTorch.
+Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
+License: MIT License
+        
+        Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Keywords: fairness,machine-learning,ai,artificial-intelligence,pytorch,deep-learning,python,bias,fairness-ai,fairness-ml
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: numpy
+
+# fairret - a fairness library in PyTorch
+
+[![Licence](https://img.shields.io/github/license/aida-ugent/fairret)](https://github.com/aida-ugent/fairret/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/fairret)](https://pypi.org/project/fairret/)
+![Static Badge](https://img.shields.io/badge/PyTorch-ee4c2c)
+[![Static Badge](https://img.shields.io/badge/Original%20Paper-00a0ff)](https://openreview.net/pdf?id=NnyD0Rjx2B)
+
+## Description
+
+The goal of fairret is to serve as an open-source Python library for measuring and mitigating statistical fairness in PyTorch models. The library is designed to be 
+1. *flexible* in how fairness is defined and pursued.
+2. *easy* to integrate into existing PyTorch pipelines.
+3. *clear* in what its tools can and cannot do.
+
+The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
+These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
+
+**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
+
+## Installation
+The fairret library can be installed via PyPi:
+
+```
+pip install fairret
+```
+
+### Dependencies
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+
+## Quickstart
+
+It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
+
+```python
+import torch.nn.functional as F
+from fairret.statistic import PositiveRate
+from fairret.loss import NormLoss
+
+statistic = PositiveRate()
+norm_fairret = NormLoss(statistic)
+
+def train(model, optimizer, train_loader):
+     for feat, sens, target in train_loader:
+            optimizer.zero_grad()
+            
+            logit = model(feat)
+            bce_loss = F.binary_cross_entropy_with_logits(logit, target)
+            fairret_loss = norm_fairret(logit, sens)
+            loss = bce_loss + fairret_loss
+            loss.backward()
+            
+            optimizer.step()
+```
+
+No special data structure is required for the sensitive features. If the training batch contains N elements, then `sens` should be a tensor of floats with shape (N, d_s), with d_s the number of sensitive features. **Like any categorical feature, it is expected that categorical sensitive features are one-hot encoded.**
+
+A notebook with a full example pipeline is provided here: [simple_pipeline.ipynb](/examples/simple_pipeline.ipynb).
+
+## Warning: AI fairness != fairness
+There are many ways in which technical approaches to AI fairness, such as this library, are simplistic and limited in actually achieving fairness in real-world decision processes.
+
+More information on these limitations can be found [here](https://dl.acm.org/doi/full/10.1145/3624700) or [here](https://ojs.aaai.org/index.php/AAAI/article/view/26798).
+
+## Future plans
+The library maintains a core focus on only fairrets for now, yet we plan to add more fairness tools that align with the design principles in the future. These may involve breaking changes. At the same time, we'll keep reviewing the role of this library within the wider ecosystem of fairness toolkits. 
+
+Want to help? Please don't hesitate to open an issue, draft a pull request, or shoot an email to [maarten.buyl@ugent.be](mailto:maarten.buyl@ugent.be).
+
+## Citation
+This framework will be presented as a paper at ICLR 2024. If you found this library useful in your work, please consider citing it as follows:
+
+```bibtex
+@inproceedings{buyl2024fairret,
+    title={fairret: a Framework for Differentiable Fairness Regularization Terms},
+    author={Buyl, Maarten and Defrance, Marybeth and De Bie, Tijl},
+    booktitle={International Conference on Learning Representations},
+    year={2024}
+}
+```
```

