# Comparing `tmp/scmallet-0.1.1.tar.gz` & `tmp/scmallet-0.1.2.tar.gz`

## Comparing `scmallet-0.1.1.tar` & `scmallet-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.1/.codecov.yaml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.1.1/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.1.1/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.1.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/__init__.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/binarize.py
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/eval_model.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/infer.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/input.py
--rw-r--r--   0        0        0    26625 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/mallet.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/topic_metrices.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.1.1/src/scmallet/utils.py
--rw-r--r--   0        0        0    18088 2020-02-02 00:00:00.000000 scmallet-0.1.1/tests/example.ipynb
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.1.1/tests/test_basic.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.1.1/LICENSE
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scmallet-0.1.1/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 scmallet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.2/.codecov.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.1.2/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.1.2/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.1.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/__init__.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/binarize.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/eval_model.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/infer.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/input.py
+-rw-r--r--   0        0        0    26625 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/mallet.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/topic_metrices.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.1.2/src/scmallet/utils.py
+-rw-r--r--   0        0        0    18088 2020-02-02 00:00:00.000000 scmallet-0.1.2/tests/example.ipynb
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.1.2/tests/test_basic.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scmallet-0.1.2/README.md
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 scmallet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 scmallet-0.1.2/PKG-INFO
```

### Comparing `scmallet-0.1.1/.cruft.json` & `scmallet-0.1.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/.pre-commit-config.yaml` & `scmallet-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `scmallet-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/.github/workflows/build.yaml` & `scmallet-0.1.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/.github/workflows/release.yaml` & `scmallet-0.1.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/.github/workflows/test.yaml` & `scmallet-0.1.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/binarize.py` & `scmallet-0.1.2/src/scmallet/binarize.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/eval_model.py` & `scmallet-0.1.2/src/scmallet/eval_model.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/infer.py` & `scmallet-0.1.2/src/scmallet/infer.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/input.py` & `scmallet-0.1.2/src/scmallet/input.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/mallet.py` & `scmallet-0.1.2/src/scmallet/mallet.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/topic_metrices.py` & `scmallet-0.1.2/src/scmallet/topic_metrices.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/src/scmallet/utils.py` & `scmallet-0.1.2/src/scmallet/utils.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/tests/example.ipynb` & `scmallet-0.1.2/tests/example.ipynb`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/LICENSE` & `scmallet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/README.md` & `scmallet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scmallet-0.1.1/pyproject.toml` & `scmallet-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 urls.Source = "https://github.com/lhqing/scmallet"
 urls.Home-page = "https://github.com/lhqing/scmallet"
 dependencies = [
     "anndata",
     "numpy",
     "pandas",
     "gensim",
+    "scipy<1.13",
     "pyranges",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "twine>=4.0.2",
```

### Comparing `scmallet-0.1.1/PKG-INFO` & `scmallet-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scmallet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper of MALLET for LDA analysis on single-cell data
 Project-URL: Source, https://github.com/lhqing/scmallet
 Project-URL: Home-page, https://github.com/lhqing/scmallet
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanqingliu@fas.harvard.edu>
 License: MIT License
         
@@ -30,14 +30,15 @@
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: anndata
 Requires-Dist: gensim
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyranges
+Requires-Dist: scipy<1.13
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
```

