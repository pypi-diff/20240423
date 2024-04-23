# Comparing `tmp/pylemur-0.2.0.tar.gz` & `tmp/pylemur-0.2.1.tar.gz`

## Comparing `pylemur-0.2.0.tar` & `pylemur-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.2.0/.codecov.yaml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pylemur-0.2.0/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.2.0/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pylemur-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pylemur-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/changelog.md
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/index.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/images/equation_schematic.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/notebooks/Tutorial.myst
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/check_implementation.qmd
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/devel_experiments.qmd
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/kang_analysis_in_R.qmd
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/lemur_model_experiments.qmd
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/scanpy_experiments.qmd
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pl/__init__.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pl/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pp/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pp/basic.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_design_matrix_utils.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_grassmann.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_grassmann_lm.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_lin_alg_wrappers.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/alignment.py
--rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/lemur.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_grasmann_lm.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_grassmann.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_lin_alg_utils.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pylemur-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.2.0/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylemur-0.2.0/README.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pylemur-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pylemur-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.2.1/.codecov.yaml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pylemur-0.2.1/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.2.1/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pylemur-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pylemur-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/changelog.md
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/index.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/images/equation_schematic.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     9771 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/notebooks/Tutorial.myst
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/check_implementation.qmd
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/devel_experiments.qmd
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/kang_analysis_in_R.qmd
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/lemur_model_experiments.qmd
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/scanpy_experiments.qmd
+-rw-r--r--   0        0        0   307919 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/test.ipynb
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pl/__init__.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pl/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pp/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pp/basic.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_design_matrix_utils.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_grassmann.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_grassmann_lm.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_lin_alg_wrappers.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/alignment.py
+-rw-r--r--   0        0        0    19198 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/lemur.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_grasmann_lm.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_grassmann.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_lin_alg_utils.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pylemur-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylemur-0.2.1/README.md
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 pylemur-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 pylemur-0.2.1/PKG-INFO
```

### Comparing `pylemur-0.2.0/.cruft.json` & `pylemur-0.2.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/.pre-commit-config.yaml` & `pylemur-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/CHANGELOG.md` & `pylemur-0.2.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 and this project adheres to [Semantic Versioning][].
 
 [keep a changelog]: https://keepachangelog.com/en/1.0.0/
 [semantic versioning]: https://semver.org/spec/v2.0.0.html
 
 ## [Unreleased]
 
+## [0.2.1]
+
+- Change example gene to one with clearer differential expression pattern
+- Remove error output in `align_harmony
+
 ## [0.2.0]
 
 Major rewrite of the API. Instead of adding coefficients as custom fields
 to the input `AnnData` object, the API now follows an object-oriented style
 similar to scikit-learn or `SCVI`. This change was motivated by the feedback 
 during the submission to the `scverse` ecosystem.
 ([Thanks]((https://github.com/scverse/ecosystem-packages/pull/156#issuecomment-2014676654)) Gregor).
```

### Comparing `pylemur-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `pylemur-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/.github/workflows/build.yaml` & `pylemur-0.2.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/.github/workflows/release.yaml` & `pylemur-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/.github/workflows/test.yaml` & `pylemur-0.2.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/Makefile` & `pylemur-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/conf.py` & `pylemur-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/references.bib` & `pylemur-0.2.1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/_static/images/equation_schematic.png` & `pylemur-0.2.1/docs/_static/images/equation_schematic.png`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/_templates/autosummary/class.rst` & `pylemur-0.2.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/extensions/typed_returns.py` & `pylemur-0.2.1/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/docs/notebooks/Tutorial.myst` & `pylemur-0.2.1/docs/notebooks/Tutorial.myst`

 * *Files 6% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 kernelspec:
   name: python3
 ---
 
 # pyLemur Walkthrough
 
 
-The goal of `pyLemur` is to simplify analysis of multi-condition single-cell data. If you have collected a single-cell RNA-seq dataset with more than one condition, lemur predicts for each cell and gene how much the expression would change if the cell had been in the other condition.
+The goal of `pyLemur` is to simplify the analysis of multi-condition single-cell data. If you have collected a single-cell RNA-seq dataset with more than one condition, LEMUR predicts for each cell and gene how much the expression would change if the cell had been in the other condition.
 
-`pyLemur` is a Python implementation of the LEMUR model; there is also an `R` package called [lemur](https://bioconductor.org/packages/lemur/) which provides additional functionality: identifying neighborhoods of cells that show consistent differential expression values and a pseudo-bulk test to validate the findings.
+`pyLemur` is a Python implementation of the LEMUR model; there is also an `R` package called [lemur](https://bioconductor.org/packages/lemur/), which provides additional functionality: identifying neighborhoods of cells that show consistent differential expression values and a pseudo-bulk test to validate the findings.
 
-`pyLemur` implements a novel framework to disentangle the effects of known covariates, latent cell states, and their interactions. At the core, is a combination of matrix factorization and regression analysis implemented as geodesic regression on Grassmann manifolds. We call this latent embedding multivariate regression. For more details see our [preprint](https://www.biorxiv.org/content/10.1101/2023.03.06.531268) {cite:p}`Ahlmann-Eltze2024`.
+`pyLemur` implements a novel framework to disentangle the effects of known covariates, latent cell states, and their interactions. At the core is a combination of matrix factorization and regression analysis implemented as geodesic regression on Grassmann manifolds. We call this latent embedding multivariate regression (LEMUR). For more details, see our [preprint](https://www.biorxiv.org/content/10.1101/2023.03.06.531268) {cite:p}`Ahlmann-Eltze2024`.
 
-<img src="../_static/images/equation_schematic.png" alt="Schematic of the matrix decomposition atthe core of LEMUR" />
+<img src="../_static/images/equation_schematic.png" alt="Schematic of the matrix decomposition at the core of LEMUR" />
 
 
 ## Data
 
-For demonstration, I will use the a dataset of interferon-$\beta$ stimuted blood cells from {cite:t}`kang2018`.
+For demonstration, I will use a dataset of interferon-$\beta$ stimulated blood cells from {cite:t}`kang2018`.
 
 ```{code-cell} ipython3
 ---
 output_stderr: remove
 ---
 # Standard imports
 import numpy as np
 import scanpy as sc
-# pertpy is need to download the kang data
+# pertpy is needed to download the Kang data
 import pertpy 
 
 # This will download the data to ./data/kang_2018.h5ad
 adata = pertpy.data.kang_2018()
 # Store counts separately in the layers
 adata.layers["counts"] = adata.X.copy()
 ```
 
-The data consist of $24\,673$ cells and $15\,706$ genes. The cells were measured in two conditions (`label="ctrl"` and `label="stim"`). The authors have annotated the cell type for each cell. This will be useful to analyze LEMUR's results, but the cell type labels are not actually used to the LEMUR model.
+The data consists of $24\,673$ cells and $15\,706$ genes. The cells were measured in two conditions (`label="ctrl"` and `label="stim"`). The authors have annotated the cell type for each cell, which will be useful to analyze LEMUR's results; however, note that the cell type labels are not used (and not needed) to fit the LEMUR model.
 
 ```{code-cell} ipython3
 :tags: ["remove-cell"]
 import pandas as pd
 pd.options.display.width = 200
 pd.options.display.max_colwidth = 20
 ```
@@ -51,28 +51,27 @@
 print(adata)
 print(adata.obs)
 ```
 
 ## Preprocessing
 
 LEMUR expects that the input has been variance-stabilized. Here, I will use the log-transformation as a simple, yet effective approach.
-In addition, I will select the $1\,000$ most variable genes, to make the results easier to manage.
+In addition, I will only work on the $1\,000$ most variable genes to make the results easier to manage.
 ```{code-cell} ipython3
 # This follows the standard recommendation from scanpy 
 sc.pp.normalize_total(adata, target_sum = 1e4, inplace=True)
 sc.pp.log1p(adata)
 adata.layers["logcounts"] = adata.X.copy()
 sc.pp.highly_variable_genes(adata, n_top_genes=1000, flavor="cell_ranger")
 adata = adata[:, adata.var.highly_variable]
 adata
 ```
 
-If we make a dimensional-embedding of the data using UMAP, we see that the cell types split-up by treatment status.
+If we make a 2D plot of the data using UMAP, we see that the cell types separate by treatment status.
 ```{code-cell} ipython3
-#| label: fig-raw-umap
 sc.tl.pca(adata)
 sc.pp.neighbors(adata)
 sc.tl.umap(adata)
 sc.pl.umap(adata, color=["label", "cell_type"])
 ```
 
 
@@ -84,46 +83,52 @@
 import pylemur
 model = pylemur.tl.LEMUR(adata, design = "~ label", n_embedding=15)
 model.fit()
 model.align_with_harmony()
 print(model)
 ```
 
-To assess the success of the LEMUR model fit, we plot a UMAP representation of the embedding calculated by LEMUR. Here, the two conditions are mixed and the different cell types and cell states drive the visible variation.
+To assess if the model was fit successfully, we plot a UMAP representation of the 15-dimensional embedding calculated by LEMUR. We want to see that the two conditions are well mixed in the embedding space because that means that LEMUR was able to disentangle the treatment effect from the cell type effect and that the residual variation is driven by the cell states.
 ```{code-cell} ipython3
-# Recalculate the UMAP embedding on calculated by LEMUR
+# Recalculate the UMAP on the embedding calculated by LEMUR
 adata.obsm["embedding"] = model.embedding
 sc.pp.neighbors(adata, use_rep="embedding")
 sc.tl.umap(adata)
 sc.pl.umap(adata, color=["label", "cell_type"])
 ```
 
-The LEMUR model is fully parametric, which means that we can predict for each cell what it's expression would have been in any condition (i.e., for a cell observed in the control condition, we can predict its expression under treatment), as a function of its low-dimensional embedding.
+The LEMUR model is fully parametric, which means that we can predict for each cell what its expression would have been in any condition (i.e., for a cell observed in the control condition, we can predict its expression under treatment) as a function of its low-dimensional embedding.
 
 ```{code-cell} ipython3
+# The model.cond(**kwargs) call specifies the condition for the prediction
 ctrl_pred = model.predict(new_condition=model.cond(label="ctrl"))
 stim_pred = model.predict(new_condition=model.cond(label="stim"))
 ```
 
-We can now check the predicted differential expression against the underlying observed expression patterns for individual genes.
+We can now check the predicted differential expression against the underlying observed expression patterns for individual genes. Here, I chose _TSC22D3_ as an example. The blue cells in the first plot are in neighborhoods with higher expression in the control condition than in the stimulated condition. The two other plots show the underlying gene expression for the control and stimulated cells and confirm LEMUR's inference.
 ```{code-cell} ipython3
 import matplotlib.pyplot as plt
 adata.layers["diff"] = stim_pred - ctrl_pred
-sel_gene = "TNFRSF18"
+# Also try CXCL10, IL8, and FBXO40
+sel_gene = "TSC22D3"
 
-_,axs = plt.subplots(nrows = 1, ncols = 3)
+fsize = plt.rcParams['figure.figsize']
+fig = plt.figure(figsize=(fsize[0] * 3, fsize[1])) 
+axs = [fig.add_subplot(1, 3, i+1) for i in range(3)]
+for ax in axs:
+    ax.set_aspect('equal')
 sc.pl.umap(adata, layer="diff", color=[sel_gene], cmap = plt.get_cmap("seismic"), vcenter=0,
-    vmin = -0.5, vmax =0.5, title="Pred diff (ctrl - stim)", ax=axs[0], show=False)
+    vmin=-4, vmax=4, title="Pred diff (stim - ctrl)", ax=axs[0], show=False)
 sc.pl.umap(adata[adata.obs["label"]=="ctrl"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
     title="Ctrl expr", ax=axs[1], show=False)
 sc.pl.umap(adata[adata.obs["label"]=="stim"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
     title="Stim expr", ax=axs[2])
 ```
 
-To assess the overall accuracy of LEMUR's predictions, I compare the average prediction per cell type across conditions. Genes on the diagonal don't change expression much between conditions, whereas all genes off-diagonal show differential expression within a cell type:
+To assess the overall accuracy of LEMUR's predictions, I will compare the average observed and predicted expression per cell type between conditions. The next plot simply shows the observed expression values. Genes on the diagonal don't change expression much between conditions within a cell type, whereas all off-diagonal genes are differentially expressed:
 ```{code-cell} ipython3
 def rowMeans_per_group(X, group):
     uniq = np.unique(group)
     res = np.zeros((len(uniq), X.shape[1]))
     for i, e in enumerate(uniq):
         res[i,:] = X[group == e,:].sum(axis=0) / sum(group == e)
     return res
@@ -136,55 +141,66 @@
 plt.scatter(ctrl_expr_per_cell_type, stim_expr_per_cell_type, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "Inf-b stim. increases gene expression for many genes")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
-Too check how well LEMUR learned the underlying expression relations, I predict the expression of cells from the control condition under stimulation, against the observed expression in the stimulated condition.
+To demonstrate that LEMUR learned the underlying expression relations, I predict what the expression of cells from the control condition would have been had they been stimulated and compare the results against the observed expression in the stimulated condition. The closer the points are to the diagonal, the better the predictions.
 ```{code-cell} ipython3
 stim_pred_per_cell_type = rowMeans_per_group(stim_pred[adata.obs["label"]=="ctrl"], adata_ctrl.obs["cell_type"])
 
 plt.scatter(stim_expr_per_cell_type, stim_pred_per_cell_type, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "LEMUR's expression predictions are accurate")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
-Lastly, I diretly, compare the predicted differential expression against the observed differential expression per cell type.
+Lastly, I directly compare the average predicted differential expression against the average observed differential expression per cell type. Again, the closer the points are to the diagonal, the better the predictions.
 
 ```{code-cell} ipython3
 pred_diff = rowMeans_per_group(adata.layers["diff"], adata.obs["cell_type"])
 
 plt.scatter(obs_diff, pred_diff, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "LEMUR's DE predictions are accurate")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
-Another advantage of LEMUR's parametricity is that you could also train the model on a subset of the data and then apply it to the full data. I train the same LEMUR model on 5% of the original data, `transform` the full data, and compare the first three dimensions of the embedding against the embedding from the model trained on the full model.
+Another advantage of LEMUR's parametricity is that you could train the model on a subset of the data and then apply it to the full data. 
+
+I will demonstrate this by training the same LEMUR model on 5% of the original data, then `transform` the full data, and finally compare the first three dimensions of the embedding against the embedding from the model trained on the full model.
+
 ```{code-cell} ipython3
 adata_subset = adata[np.random.choice(np.arange(adata.shape[0]), size = round(adata.shape[0] * 0.05)),]
 model_small = pylemur.tl.LEMUR(adata_subset, design = "~ label", n_embedding=15)
 model_small.fit().align_with_harmony()
 emb_proj = model_small.transform(adata)
 plt.scatter(emb_proj[:,0:3], model.embedding[:,0:3], s = 0.1)
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 plt.axline((0, 0), (-1, 1), linewidth=1, color='black')
 ```
 
+We see that the small model still captures most of the relevant variation.
+```{code-cell} ipython3
+adata.obsm["embedding_from_small_fit"] = emb_proj
+sc.pp.neighbors(adata, use_rep="embedding_from_small_fit")
+sc.tl.umap(adata)
+sc.pl.umap(adata, color=["label", "cell_type"])
+```
+
 ### Session Info
 
 ```{code-cell} ipython3
 import session_info
 session_info.show()
 ```
 
 
-### Referenes
+### References
 
 ```{bibliography}
 :style: plain
 :filter: docname in docnames
 ```
```

### Comparing `pylemur-0.2.0/notebooks/check_implementation.qmd` & `pylemur-0.2.1/notebooks/check_implementation.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/notebooks/devel_experiments.qmd` & `pylemur-0.2.1/notebooks/devel_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/notebooks/kang_analysis_in_R.qmd` & `pylemur-0.2.1/notebooks/kang_analysis_in_R.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/notebooks/lemur_model_experiments.qmd` & `pylemur-0.2.1/notebooks/lemur_model_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/notebooks/scanpy_experiments.qmd` & `pylemur-0.2.1/notebooks/scanpy_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/pl/basic.py` & `pylemur-0.2.1/src/pylemur/pl/basic.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/pp/basic.py` & `pylemur-0.2.1/src/pylemur/pp/basic.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/tl/_design_matrix_utils.py` & `pylemur-0.2.1/src/pylemur/tl/_design_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/tl/_grassmann.py` & `pylemur-0.2.1/src/pylemur/tl/_grassmann.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/tl/_grassmann_lm.py` & `pylemur-0.2.1/src/pylemur/tl/_grassmann_lm.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/tl/_lin_alg_wrappers.py` & `pylemur-0.2.1/src/pylemur/tl/_lin_alg_wrappers.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/src/pylemur/tl/alignment.py` & `pylemur-0.2.1/src/pylemur/tl/alignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,17 @@
         # NA's are converted to zero so that they don't propagate.
         diff[np.isnan(diff)] = 0
         new_pos[sel, :] = new_pos[sel, :] + (diff @ grouping_matrix[:, sel]).T
 
     intercept_emb = np.hstack([np.ones((embedding.shape[0], 1)), embedding])
     interact_design_matrix = np.repeat(design_matrix, n_emb + 1, axis=1) * np.hstack([intercept_emb] * K)
     alignment_coefs = ridge_regression(new_pos - embedding, interact_design_matrix, ridge_penalty)
-    if verbose:
-        print(f"Alignment error: {np.linalg.norm((new_pos - embedding) - interact_design_matrix @ alignment_coefs)}")
+    ## The alignment error is weird, as it doesn't necessarily go down. Better not to show it
+    # if verbose:
+    #     print(f"Alignment error: {np.linalg.norm((new_pos - embedding) - interact_design_matrix @ alignment_coefs)}")
     alignment_coefs = alignment_coefs.reshape((K, n_emb + 1, n_emb)).transpose((2, 1, 0))
     if calculate_new_embedding:
         new_embedding = _apply_linear_transformation(embedding, alignment_coefs, design_matrix)
         return alignment_coefs, new_embedding
     else:
         return alignment_coefs
```

### Comparing `pylemur-0.2.0/src/pylemur/tl/lemur.py` & `pylemur-0.2.1/src/pylemur/tl/lemur.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         """
         embedding = self.embedding.copy()
         design_matrix = self.design_matrix
         # Init harmony
         harm_obj = _init_harmony(embedding, design_matrix, verbose=verbose)
         for idx in range(max_iter):
             if verbose:
-                print(f"Iteration {idx}")
+                print(f"Alignment iteration {idx}")
             # Update harmony
             harm_obj.cluster()
             # alignment <- align_impl(training_fit$embedding, harm_obj$R, act_design_matrix, ridge_penalty = ridge_penalty)
             al_coef, new_emb = _align_impl(
                 embedding,
                 harm_obj.R,
                 design_matrix,
```

### Comparing `pylemur-0.2.0/tests/test_grasmann_lm.py` & `pylemur-0.2.1/tests/test_grasmann_lm.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/tests/test_grassmann.py` & `pylemur-0.2.1/tests/test_grassmann.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/tests/test_lin_alg_utils.py` & `pylemur-0.2.1/tests/test_lin_alg_utils.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/.gitignore` & `pylemur-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/LICENSE` & `pylemur-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/README.md` & `pylemur-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.0/pyproject.toml` & `pylemur-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "pyLemur"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Constantin Ahlmann-Eltze"},
 ]
@@ -44,14 +44,18 @@
     "sphinxext-opengraph",
     "sphinx-design",
     # For notebooks
     "ipykernel",
     "ipython",
     "sphinx-copybutton",
     "pandas",
+    "scanpy",
+    "pertpy",
+    "matplotlib",
+    "session-info",
 ]
 test = [
     "pytest",
     "coverage",
 ]
 
 [tool.coverage.run]
```

### Comparing `pylemur-0.2.0/PKG-INFO` & `pylemur-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyLemur
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data.
 Project-URL: Documentation, https://pyLemur.readthedocs.io/
 Project-URL: Source, https://github.com/const-ae/pyLemur
 Project-URL: Home-page, https://github.com/const-ae/pyLemur
 Author: Constantin Ahlmann-Eltze
 Maintainer-email: Constantin Ahlmann-Eltze <artjom31415@googlemail.com>
 License: MIT License
@@ -40,16 +40,20 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc'
 Requires-Dist: ipykernel; extra == 'doc'
 Requires-Dist: ipython; extra == 'doc'
+Requires-Dist: matplotlib; extra == 'doc'
 Requires-Dist: myst-nb; extra == 'doc'
 Requires-Dist: pandas; extra == 'doc'
+Requires-Dist: pertpy; extra == 'doc'
+Requires-Dist: scanpy; extra == 'doc'
+Requires-Dist: session-info; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc'
 Requires-Dist: sphinx-copybutton; extra == 'doc'
 Requires-Dist: sphinx-design; extra == 'doc'
 Requires-Dist: sphinx>=4; extra == 'doc'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
 Requires-Dist: sphinxext-opengraph; extra == 'doc'
```

