# Comparing `tmp/neuroHarmonize-2.3.1.tar.gz` & `tmp/neuroharmonize-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroHarmonize-2.3.1.tar", last modified: Tue Mar 19 12:20:45 2024, max compression
+gzip compressed data, was "neuroharmonize-2.4.1.tar", last modified: Tue Apr 23 17:22:40 2024, max compression
```

## Comparing `neuroHarmonize-2.3.1.tar` & `neuroharmonize-2.4.1.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-03-19 12:20:45.663040 neuroHarmonize-2.3.1/
--rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroHarmonize-2.3.1/LICENSE
--rw-r--r--   0 pomponior   (501) staff       (20)       19 2024-02-01 14:00:43.000000 neuroHarmonize-2.3.1/MANIFEST.in
--rw-r--r--   0 pomponior   (501) staff       (20)    10396 2024-03-19 12:20:45.662953 neuroHarmonize-2.3.1/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)     9838 2024-03-19 12:20:02.000000 neuroHarmonize-2.3.1/README.rst
--rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroHarmonize-2.3.1/pyproject.toml
--rw-r--r--   0 pomponior   (501) staff       (20)      684 2024-03-19 12:20:45.663293 neuroHarmonize-2.3.1/setup.cfg
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-03-19 12:20:45.660659 neuroHarmonize-2.3.1/src/
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-03-19 12:20:45.662013 neuroHarmonize-2.3.1/src/neuroHarmonize/
--rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-03-19 12:20:37.000000 neuroHarmonize-2.3.1/src/neuroHarmonize/__init__.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)     8881 2024-03-19 12:20:37.000000 neuroHarmonize-2.3.1/src/neuroHarmonize/harmonizationApply.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)    17493 2024-03-19 12:20:37.000000 neuroHarmonize-2.3.1/src/neuroHarmonize/harmonizationLearn.py
--rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-03-19 12:20:37.000000 neuroHarmonize-2.3.1/src/neuroHarmonize/harmonizationNIFTI.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)     9601 2024-03-19 12:20:37.000000 neuroHarmonize-2.3.1/src/neuroHarmonize/neuroCombat.py
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-03-19 12:20:45.662735 neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/
--rw-r--r--   0 pomponior   (501) staff       (20)    10396 2024-03-19 12:20:45.000000 neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)      411 2024-03-19 12:20:45.000000 neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/SOURCES.txt
--rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-03-19 12:20:45.000000 neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/dependency_links.txt
--rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-03-19 12:20:45.000000 neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/top_level.txt
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.947218 neuroharmonize-2.4.1/
+-rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.1/LICENSE
+-rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.1/MANIFEST.in
+-rw-r--r--   0 pomponior   (501) staff       (20)    10843 2024-04-23 17:22:40.947105 neuroharmonize-2.4.1/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)    10285 2024-04-23 17:20:20.000000 neuroharmonize-2.4.1/README.md
+-rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.1/pyproject.toml
+-rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-04-23 17:22:40.947461 neuroharmonize-2.4.1/setup.cfg
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.945467 neuroharmonize-2.4.1/src/
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.946925 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/
+-rw-r--r--   0 pomponior   (501) staff       (20)    10843 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)      222 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/top_level.txt
```

### Comparing `neuroHarmonize-2.3.1/LICENSE` & `neuroharmonize-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroHarmonize-2.3.1/PKG-INFO` & `neuroharmonize-2.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,256 +1,279 @@
-Metadata-Version: 2.1
-Name: neuroHarmonize
-Version: 2.3.1
-Summary: Harmonization tools for multi-center neuroimaging studies.
-Home-page: https://github.com/rpomponio/neuroHarmonize
-Author: Raymond Pomponio
-Author-email: raymond.pomponio@outlook.com
-Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-==============
-neuroHarmonize
-==============
+# neuroHarmonize
 
 Harmonization tools for multi-site neuroimaging analysis. Part of the work
-reported in our paper with data from the ISTAGING consoritum [1]_.
+reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Nick Cullen [2]_,
-``neuroCombat``.
+This package extends the functionality of the package developed by Jean-Philippe
+Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
+`neuroCombat` is now a formal dependency for `neuroHarmonize`.
 
-Cullen's package, ``neuroCombat``, allows the user to perform a
-harmonization procedure using the ComBat [3]_ algorithm for correcting
+The reference implementation, `neuroCombat`, allows the user to perform a
+harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
-This package, ``neuroHarmonize``, provides similar functionality, with additional
-features:
+This package, `neuroHarmonize`, provides similar functionality, with
+additional features:
 
-1. Support for working with NIFTI images. Implemented with the ``nibabel`` package.
+1. Support for working with NIFTI images, with the `nibabel` package.
 2. Separate train/test datasets.
 3. Specify covariates with generic nonlinear effects. Implemented using
-   Generalized Additive Models (GAMs) from the ``statsmodels`` package.
+   Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest version: `2.3.1` (March 2024)
+Latest development version: `2.4.1` (April 2024)
 
 Requirements:
 
-* ``git >= 2.17.2``
-* ``python >= 3.6.8``
-
-To make installation easier, neuroCombat is not a formal dependency for this
-package, but the source code is included to call neuroCombat functions.
+* `git >= 2.17.2`
+* `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
     >>> pip install neuroHarmonize
 
 **Option 2: Install from GitHub (Development Version)**
 
     >>> pip install git+https://github.com/rpomponio/neuroHarmonize
 
 Quick Start
 -----------
 
-*Please note:* the ComBat [3]_ algorithm corrects for site effects but
+*Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
-effects as well you can use the argument ``return_s_data``.
+effects as well you can use the argument `return_s_data`.
 
-You must provide a **data matrix** which is a ``numpy.array`` containing the
-features to be harmonized. For example, an ``array`` of brain volumes:
+You must provide a **data matrix** which is a `numpy.array` containing the
+features to be harmonized. For example, an `array` of brain volumes:
 
-::
+```
 
   array([[3138.0, 3164.2,  ..., 206.4],
          [1708.4, 2351.2,  ..., 364.0],
          ...,
          [1119.6, 1071.6,  ..., 326.6]])
+```
 
 The dimensionality of this matrix must be: **N_samples x N_features**
 
-You must also provide a **covariate matrix** which is a ``pandas.DataFrame``
+You must also provide a **covariate matrix** which is a `pandas.DataFrame`
 containing all covariates to control for during harmonization. All covariates
 must be encoded numerically (you must handle categorical covariates in a
-pre-processing step, see ``pandas.get_dummies``). The ``DataFrame`` must
+pre-processing step, see `pandas.get_dummies`). The `DataFrame` must
 also contain a single column called "SITE" with labels that identify sites
 (the labels in "SITE" need not be numeric).
 
-::
+```
 
        SITE   AGE  SEX_M
   0  SITE_A  76.5      1
   1  SITE_B  80.1      1
   2  SITE_A  82.9      0
   ...   ...   ...    ...
   9  SITE_B  82.1      0
+```
 
 The dimensionality of this dataframe must be: **N_samples x N_Covariates**
 
 The order of samples must be identical in the **covariate_matrix** and the
 **data_matrix**.
 
-After preparing both inputs, you can call ``harmonizationLearn`` to harmonize
+After preparing both inputs, you can call `harmonizationLearn` to harmonize
 the provided dataset.
 
 Example usage:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization and store the adjusted data
-    >>> my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```
 
-The dimensionality of the matrix ``my_data_adj`` will be identical to
-``my_data``: **N_samples x N_features**
+The dimensionality of the matrix `my_data_adj` will be identical to
+`my_data`: **N_samples x N_features**
 
 Working with NIFTI Images
 -------------------------
 
-To work with NIFTI images, you compute a mask using a ``pandas.DataFrame`` which
+To work with NIFTI images, you compute a mask using a `pandas.DataFrame` which
 contains file paths for all of the images in the **training set**.
 
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
-    >>> nifti_list = pd.read_csv('brain_images_paths.csv')
-    >>> nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```python
+import pandas as pd
+import numpy as np
+from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
+nifti_list = pd.read_csv('brain_images_paths.csv')
+nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```
 
-After the mask is created, you can flatten the images to a 2D ``numpy.array``
+After the mask is created, you can flatten the images to a 2D `numpy.array`
 very similar to what is done with the tabular data example above.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
-    >>> nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
+nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```
 
 The next step is identical to working with tabular data. You simply pass the 2D
-array to ``neuroHarmonize.harmonizationLearn``.
+array to `neuroHarmonize.harmonizationLearn`.
 
-    >>> import neuroHarmonize as nh
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
-    >>> nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```python
+import neuroHarmonize as nh
+covars = pd.read_csv('subject_info.csv')
+my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
+nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```
 
 Lastly, you can apply the model sequentially to images in a larger dataset with
-``applyModelNIFTIs``. When performing NIFTI harmonization, loading the entire set
+`applyModelNIFTIs`. When performing NIFTI harmonization, loading the entire set
 of images may exceed memory capacity. This function will reduce the burden on
 memory by applying the model to images one-by-one and saving the results as NIFTIs.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
-    >>> # load pre-trained model
-    >>> my_model = nh.loadHarmonizationModel('MY_MODEL')
-    >>> applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
+# load pre-trained model
+my_model = nh.loadHarmonizationModel('MY_MODEL')
+applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```
 
 Applying Pre-Trained Models to New Data
 ---------------------------------------
 
 This feature allows you to train a harmonization model on a subset of data, then
 apply the model to the entire set. For example, in longitudinal analyses, one may
 wish to train a harmonization model on baseline cases and apply the model to
 follow-up cases, to avoid double-counting subjects.
 
-If you have previously trained a harmonization model with ``harmonizationLearn``,
-you may apply the model parameters to new data with ``harmonizationApply``.
+If you have previously trained a harmonization model with `harmonizationLearn`,
+you may apply the model parameters to new data with `harmonizationApply`.
 
 First load the model:
 
-    >>> from neuroHarmonize import harmonizationApply, loadHarmonizationModel
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load a pre-trained model
-    >>> my_model = loadHarmonizationModel('../models/my_model')
+```python
+from neuroHarmonize import harmonizationApply, loadHarmonizationModel
+import pandas as pd
+import numpy as np
+# load a pre-trained model
+my_model = loadHarmonizationModel('../models/my_model')
+```
 
 Next, prepare the holdout data on which you will apply the model. This data
-must look exactly like the training data for ``harmonizationLearn``, including
+must look exactly like the training data for `harmonizationLearn`, including
 the same number and order of covariates. If the holdout data contains a
 different number of sites, an error will be thrown.
 
 After preparing the holdout data simply apply the model:
 
-    >>> df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
-    >>> my_holdout_data = np.array(df_holdout)
-    >>> covars = pd.read_csv('subject_info_holdout.csv')
-    >>> my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```python
+df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
+my_holdout_data = np.array(df_holdout)
+covars = pd.read_csv('subject_info_holdout.csv')
+my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```
 
 Specifying Nonlinear Covariate Effects
 --------------------------------------
 
 You may specify nonlinear covariate effects with the optional argument:
-``smooth_terms``. For example, you may want to specify age as a nonlinear
+`smooth_terms`. For example, you may want to specify age as a nonlinear
 term in the harmonization model, if age exhibits nonlinear relationships with
-brain volumes. This can be done easily with ``harmonizationLearn``:
+brain volumes. This can be done easily with `harmonizationLearn`:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization with NONLINEAR effects of age
-    >>> my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization with NONLINEAR effects of age
+my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```
 
 When applying nonlinear models to holdout data, you may get an error: "some data
 points fall outside the outermost knots, and I'm not sure how to handle them".
 This is documented: https://github.com/statsmodels/statsmodels/issues/2361.
-The current workaround is to use the optional argument: ``smooth_term_bounds``,
+The current workaround is to use the optional argument: `smooth_term_bounds`,
 which controls the boundary knots for nonlinear estimation. You should specify
 boundaries that contain the limits of the entire dataset, including holdout data.
 
 Empirical Bayes
 ---------------
 
 Note the default behavior is to run the empirical Bayes (EB) step of ComBat, which
 is useful for harmonizing multiple features that are similar such as genes or
 brain regional volumes.
 
-To run without EB, simply pass the optional argument ``eb=False`` to
-``harmonizationLearn``. This is convenient when harmonizing a small number of
+To run without EB, simply pass the optional argument `eb=False` to
+`harmonizationLearn`. This is convenient when harmonizing a small number of
 features, e.g. fewer than 10.
 
-When ``eb=True``, ComBat uses Empirical Bayes to fit a prior distribution for
+When `eb=True`, ComBat uses Empirical Bayes to fit a prior distribution for
 the site effects for each site. You may wish to visualize fit of the prior
 distribution, along with the observed distribution of site effects. The following
 code example plots both distributions for the location effect of site 1.
 
-    >>> import matplotlib.pyplot as plt
-    >>> import seaborn as sns
-    >>> from neuroHarmonize import loadHarmonizationModel
-    >>> model = loadHarmonizationModel('../models/my_model')
-    >>> site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
-    >>> sns.kdeplot(site_01, color='blue', label='Site-1-prior')
-    >>> sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
-    >>> plt.show()
+```python
+import matplotlib.pyplot as plt
+import seaborn as sns
+from neuroHarmonize import loadHarmonizationModel
+model = loadHarmonizationModel('../models/my_model')
+site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
+sns.kdeplot(site_01, color='blue', label='Site-1-prior')
+sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
+plt.show()
+```
+
+![Fig 1](figure_1.png)
+
+Reference Sites
+---------------
+
+Recently other implementations have been including the ability to specify a
+reference site or scanner, such that all data will be harmonized to that site.
+
+**This feature was added in version 2.4.x.** It can be used as in the following
+example:
+
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars, ref_batch='SITE_A')
+```
 
-.. image:: figure_1.png
+Please submit any issues to [GitHub](https://github.com/rpomponio/neuroHarmonize/issues)
+if you run into trouble with this feature, as I am still testing its utility.
 
 Citations
 ---------
 
-.. [1] Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
+[^1]: Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
    "Harmonization of large MRI datasets for the analysis of brain imaging
    patterns throughout the lifespan." Neuroimage 208.
    https://doi.org/10.1016/j.neuroimage.2019.116450.
-.. [2] Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
+[^2]: Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
    P. A. Cook, P. Adams, C. Cooper, M. Fava, P. J. McGrath, M. McInnis,
    M. L. Phillips, M. H. Trivedi, M. M. Weissman and R. T. Shinohara (2017).
    "Harmonization of cortical thickness measurements across scanners and sites."
    Neuroimage 167: 104-120. https://doi.org/10.1016/j.neuroimage.2017.11.024.
-.. [3] W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray
-   expression data using empirical Bayes methods. Biostatistics, 8(1):118-127,
-   2007. https://doi.org/10.1093/biostatistics/kxj037.
+[^3]: W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray expression data using empirical Bayes methods. Biostatistics, 8(1):118-127, 2007. https://doi.org/10.1093/biostatistics/kxj037.
```

### Comparing `neuroHarmonize-2.3.1/README.rst` & `neuroharmonize-2.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,241 +1,294 @@
-==============
-neuroHarmonize
-==============
+Metadata-Version: 2.1
+Name: neuroHarmonize
+Version: 2.4.1
+Summary: Harmonization tools for multi-center neuroimaging studies.
+Home-page: https://github.com/rpomponio/neuroHarmonize
+Author: Raymond Pomponio
+Author-email: raymond.pomponio@outlook.com
+Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# neuroHarmonize
 
 Harmonization tools for multi-site neuroimaging analysis. Part of the work
-reported in our paper with data from the ISTAGING consoritum [1]_.
+reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Nick Cullen [2]_,
-``neuroCombat``.
+This package extends the functionality of the package developed by Jean-Philippe
+Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
+`neuroCombat` is now a formal dependency for `neuroHarmonize`.
 
-Cullen's package, ``neuroCombat``, allows the user to perform a
-harmonization procedure using the ComBat [3]_ algorithm for correcting
+The reference implementation, `neuroCombat`, allows the user to perform a
+harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
-This package, ``neuroHarmonize``, provides similar functionality, with additional
-features:
+This package, `neuroHarmonize`, provides similar functionality, with
+additional features:
 
-1. Support for working with NIFTI images. Implemented with the ``nibabel`` package.
+1. Support for working with NIFTI images, with the `nibabel` package.
 2. Separate train/test datasets.
 3. Specify covariates with generic nonlinear effects. Implemented using
-   Generalized Additive Models (GAMs) from the ``statsmodels`` package.
+   Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest version: `2.3.1` (March 2024)
+Latest development version: `2.4.1` (April 2024)
 
 Requirements:
 
-* ``git >= 2.17.2``
-* ``python >= 3.6.8``
-
-To make installation easier, neuroCombat is not a formal dependency for this
-package, but the source code is included to call neuroCombat functions.
+* `git >= 2.17.2`
+* `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
     >>> pip install neuroHarmonize
 
 **Option 2: Install from GitHub (Development Version)**
 
     >>> pip install git+https://github.com/rpomponio/neuroHarmonize
 
 Quick Start
 -----------
 
-*Please note:* the ComBat [3]_ algorithm corrects for site effects but
+*Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
-effects as well you can use the argument ``return_s_data``.
+effects as well you can use the argument `return_s_data`.
 
-You must provide a **data matrix** which is a ``numpy.array`` containing the
-features to be harmonized. For example, an ``array`` of brain volumes:
+You must provide a **data matrix** which is a `numpy.array` containing the
+features to be harmonized. For example, an `array` of brain volumes:
 
-::
+```
 
   array([[3138.0, 3164.2,  ..., 206.4],
          [1708.4, 2351.2,  ..., 364.0],
          ...,
          [1119.6, 1071.6,  ..., 326.6]])
+```
 
 The dimensionality of this matrix must be: **N_samples x N_features**
 
-You must also provide a **covariate matrix** which is a ``pandas.DataFrame``
+You must also provide a **covariate matrix** which is a `pandas.DataFrame`
 containing all covariates to control for during harmonization. All covariates
 must be encoded numerically (you must handle categorical covariates in a
-pre-processing step, see ``pandas.get_dummies``). The ``DataFrame`` must
+pre-processing step, see `pandas.get_dummies`). The `DataFrame` must
 also contain a single column called "SITE" with labels that identify sites
 (the labels in "SITE" need not be numeric).
 
-::
+```
 
        SITE   AGE  SEX_M
   0  SITE_A  76.5      1
   1  SITE_B  80.1      1
   2  SITE_A  82.9      0
   ...   ...   ...    ...
   9  SITE_B  82.1      0
+```
 
 The dimensionality of this dataframe must be: **N_samples x N_Covariates**
 
 The order of samples must be identical in the **covariate_matrix** and the
 **data_matrix**.
 
-After preparing both inputs, you can call ``harmonizationLearn`` to harmonize
+After preparing both inputs, you can call `harmonizationLearn` to harmonize
 the provided dataset.
 
 Example usage:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization and store the adjusted data
-    >>> my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```
 
-The dimensionality of the matrix ``my_data_adj`` will be identical to
-``my_data``: **N_samples x N_features**
+The dimensionality of the matrix `my_data_adj` will be identical to
+`my_data`: **N_samples x N_features**
 
 Working with NIFTI Images
 -------------------------
 
-To work with NIFTI images, you compute a mask using a ``pandas.DataFrame`` which
+To work with NIFTI images, you compute a mask using a `pandas.DataFrame` which
 contains file paths for all of the images in the **training set**.
 
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
-    >>> nifti_list = pd.read_csv('brain_images_paths.csv')
-    >>> nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```python
+import pandas as pd
+import numpy as np
+from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
+nifti_list = pd.read_csv('brain_images_paths.csv')
+nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```
 
-After the mask is created, you can flatten the images to a 2D ``numpy.array``
+After the mask is created, you can flatten the images to a 2D `numpy.array`
 very similar to what is done with the tabular data example above.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
-    >>> nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
+nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```
 
 The next step is identical to working with tabular data. You simply pass the 2D
-array to ``neuroHarmonize.harmonizationLearn``.
+array to `neuroHarmonize.harmonizationLearn`.
 
-    >>> import neuroHarmonize as nh
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
-    >>> nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```python
+import neuroHarmonize as nh
+covars = pd.read_csv('subject_info.csv')
+my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
+nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```
 
 Lastly, you can apply the model sequentially to images in a larger dataset with
-``applyModelNIFTIs``. When performing NIFTI harmonization, loading the entire set
+`applyModelNIFTIs`. When performing NIFTI harmonization, loading the entire set
 of images may exceed memory capacity. This function will reduce the burden on
 memory by applying the model to images one-by-one and saving the results as NIFTIs.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
-    >>> # load pre-trained model
-    >>> my_model = nh.loadHarmonizationModel('MY_MODEL')
-    >>> applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
+# load pre-trained model
+my_model = nh.loadHarmonizationModel('MY_MODEL')
+applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```
 
 Applying Pre-Trained Models to New Data
 ---------------------------------------
 
 This feature allows you to train a harmonization model on a subset of data, then
 apply the model to the entire set. For example, in longitudinal analyses, one may
 wish to train a harmonization model on baseline cases and apply the model to
 follow-up cases, to avoid double-counting subjects.
 
-If you have previously trained a harmonization model with ``harmonizationLearn``,
-you may apply the model parameters to new data with ``harmonizationApply``.
+If you have previously trained a harmonization model with `harmonizationLearn`,
+you may apply the model parameters to new data with `harmonizationApply`.
 
 First load the model:
 
-    >>> from neuroHarmonize import harmonizationApply, loadHarmonizationModel
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load a pre-trained model
-    >>> my_model = loadHarmonizationModel('../models/my_model')
+```python
+from neuroHarmonize import harmonizationApply, loadHarmonizationModel
+import pandas as pd
+import numpy as np
+# load a pre-trained model
+my_model = loadHarmonizationModel('../models/my_model')
+```
 
 Next, prepare the holdout data on which you will apply the model. This data
-must look exactly like the training data for ``harmonizationLearn``, including
+must look exactly like the training data for `harmonizationLearn`, including
 the same number and order of covariates. If the holdout data contains a
 different number of sites, an error will be thrown.
 
 After preparing the holdout data simply apply the model:
 
-    >>> df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
-    >>> my_holdout_data = np.array(df_holdout)
-    >>> covars = pd.read_csv('subject_info_holdout.csv')
-    >>> my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```python
+df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
+my_holdout_data = np.array(df_holdout)
+covars = pd.read_csv('subject_info_holdout.csv')
+my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```
 
 Specifying Nonlinear Covariate Effects
 --------------------------------------
 
 You may specify nonlinear covariate effects with the optional argument:
-``smooth_terms``. For example, you may want to specify age as a nonlinear
+`smooth_terms`. For example, you may want to specify age as a nonlinear
 term in the harmonization model, if age exhibits nonlinear relationships with
-brain volumes. This can be done easily with ``harmonizationLearn``:
+brain volumes. This can be done easily with `harmonizationLearn`:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization with NONLINEAR effects of age
-    >>> my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization with NONLINEAR effects of age
+my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```
 
 When applying nonlinear models to holdout data, you may get an error: "some data
 points fall outside the outermost knots, and I'm not sure how to handle them".
 This is documented: https://github.com/statsmodels/statsmodels/issues/2361.
-The current workaround is to use the optional argument: ``smooth_term_bounds``,
+The current workaround is to use the optional argument: `smooth_term_bounds`,
 which controls the boundary knots for nonlinear estimation. You should specify
 boundaries that contain the limits of the entire dataset, including holdout data.
 
 Empirical Bayes
 ---------------
 
 Note the default behavior is to run the empirical Bayes (EB) step of ComBat, which
 is useful for harmonizing multiple features that are similar such as genes or
 brain regional volumes.
 
-To run without EB, simply pass the optional argument ``eb=False`` to
-``harmonizationLearn``. This is convenient when harmonizing a small number of
+To run without EB, simply pass the optional argument `eb=False` to
+`harmonizationLearn`. This is convenient when harmonizing a small number of
 features, e.g. fewer than 10.
 
-When ``eb=True``, ComBat uses Empirical Bayes to fit a prior distribution for
+When `eb=True`, ComBat uses Empirical Bayes to fit a prior distribution for
 the site effects for each site. You may wish to visualize fit of the prior
 distribution, along with the observed distribution of site effects. The following
 code example plots both distributions for the location effect of site 1.
 
-    >>> import matplotlib.pyplot as plt
-    >>> import seaborn as sns
-    >>> from neuroHarmonize import loadHarmonizationModel
-    >>> model = loadHarmonizationModel('../models/my_model')
-    >>> site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
-    >>> sns.kdeplot(site_01, color='blue', label='Site-1-prior')
-    >>> sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
-    >>> plt.show()
+```python
+import matplotlib.pyplot as plt
+import seaborn as sns
+from neuroHarmonize import loadHarmonizationModel
+model = loadHarmonizationModel('../models/my_model')
+site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
+sns.kdeplot(site_01, color='blue', label='Site-1-prior')
+sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
+plt.show()
+```
+
+![Fig 1](figure_1.png)
+
+Reference Sites
+---------------
+
+Recently other implementations have been including the ability to specify a
+reference site or scanner, such that all data will be harmonized to that site.
+
+**This feature was added in version 2.4.x.** It can be used as in the following
+example:
+
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars, ref_batch='SITE_A')
+```
 
-.. image:: figure_1.png
+Please submit any issues to [GitHub](https://github.com/rpomponio/neuroHarmonize/issues)
+if you run into trouble with this feature, as I am still testing its utility.
 
 Citations
 ---------
 
-.. [1] Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
+[^1]: Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
    "Harmonization of large MRI datasets for the analysis of brain imaging
    patterns throughout the lifespan." Neuroimage 208.
    https://doi.org/10.1016/j.neuroimage.2019.116450.
-.. [2] Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
+[^2]: Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
    P. A. Cook, P. Adams, C. Cooper, M. Fava, P. J. McGrath, M. McInnis,
    M. L. Phillips, M. H. Trivedi, M. M. Weissman and R. T. Shinohara (2017).
    "Harmonization of cortical thickness measurements across scanners and sites."
    Neuroimage 167: 104-120. https://doi.org/10.1016/j.neuroimage.2017.11.024.
-.. [3] W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray
-   expression data using empirical Bayes methods. Biostatistics, 8(1):118-127,
-   2007. https://doi.org/10.1093/biostatistics/kxj037.
+[^3]: W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray expression data using empirical Bayes methods. Biostatistics, 8(1):118-127, 2007. https://doi.org/10.1093/biostatistics/kxj037.
```

### Comparing `neuroHarmonize-2.3.1/setup.cfg` & `neuroharmonize-2.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = neuroHarmonize
-version = 2.3.1
+version = 2.4.1
 author = Raymond Pomponio
 author_email = raymond.pomponio@outlook.com
 description = Harmonization tools for multi-center neuroimaging studies.
-long_description = file: README.rst
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rpomponio/neuroHarmonize
 project_urls = 
 	Bug Tracker = https://github.com/rpomponio/neuroHarmonize/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `neuroHarmonize-2.3.1/src/neuroHarmonize.egg-info/PKG-INFO` & `neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,256 +1,294 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.3.1
+Version: 2.4.1
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-==============
-neuroHarmonize
-==============
+# neuroHarmonize
 
 Harmonization tools for multi-site neuroimaging analysis. Part of the work
-reported in our paper with data from the ISTAGING consoritum [1]_.
+reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Nick Cullen [2]_,
-``neuroCombat``.
+This package extends the functionality of the package developed by Jean-Philippe
+Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
+`neuroCombat` is now a formal dependency for `neuroHarmonize`.
 
-Cullen's package, ``neuroCombat``, allows the user to perform a
-harmonization procedure using the ComBat [3]_ algorithm for correcting
+The reference implementation, `neuroCombat`, allows the user to perform a
+harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
-This package, ``neuroHarmonize``, provides similar functionality, with additional
-features:
+This package, `neuroHarmonize`, provides similar functionality, with
+additional features:
 
-1. Support for working with NIFTI images. Implemented with the ``nibabel`` package.
+1. Support for working with NIFTI images, with the `nibabel` package.
 2. Separate train/test datasets.
 3. Specify covariates with generic nonlinear effects. Implemented using
-   Generalized Additive Models (GAMs) from the ``statsmodels`` package.
+   Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest version: `2.3.1` (March 2024)
+Latest development version: `2.4.1` (April 2024)
 
 Requirements:
 
-* ``git >= 2.17.2``
-* ``python >= 3.6.8``
-
-To make installation easier, neuroCombat is not a formal dependency for this
-package, but the source code is included to call neuroCombat functions.
+* `git >= 2.17.2`
+* `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
     >>> pip install neuroHarmonize
 
 **Option 2: Install from GitHub (Development Version)**
 
     >>> pip install git+https://github.com/rpomponio/neuroHarmonize
 
 Quick Start
 -----------
 
-*Please note:* the ComBat [3]_ algorithm corrects for site effects but
+*Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
-effects as well you can use the argument ``return_s_data``.
+effects as well you can use the argument `return_s_data`.
 
-You must provide a **data matrix** which is a ``numpy.array`` containing the
-features to be harmonized. For example, an ``array`` of brain volumes:
+You must provide a **data matrix** which is a `numpy.array` containing the
+features to be harmonized. For example, an `array` of brain volumes:
 
-::
+```
 
   array([[3138.0, 3164.2,  ..., 206.4],
          [1708.4, 2351.2,  ..., 364.0],
          ...,
          [1119.6, 1071.6,  ..., 326.6]])
+```
 
 The dimensionality of this matrix must be: **N_samples x N_features**
 
-You must also provide a **covariate matrix** which is a ``pandas.DataFrame``
+You must also provide a **covariate matrix** which is a `pandas.DataFrame`
 containing all covariates to control for during harmonization. All covariates
 must be encoded numerically (you must handle categorical covariates in a
-pre-processing step, see ``pandas.get_dummies``). The ``DataFrame`` must
+pre-processing step, see `pandas.get_dummies`). The `DataFrame` must
 also contain a single column called "SITE" with labels that identify sites
 (the labels in "SITE" need not be numeric).
 
-::
+```
 
        SITE   AGE  SEX_M
   0  SITE_A  76.5      1
   1  SITE_B  80.1      1
   2  SITE_A  82.9      0
   ...   ...   ...    ...
   9  SITE_B  82.1      0
+```
 
 The dimensionality of this dataframe must be: **N_samples x N_Covariates**
 
 The order of samples must be identical in the **covariate_matrix** and the
 **data_matrix**.
 
-After preparing both inputs, you can call ``harmonizationLearn`` to harmonize
+After preparing both inputs, you can call `harmonizationLearn` to harmonize
 the provided dataset.
 
 Example usage:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization and store the adjusted data
-    >>> my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars)
+```
 
-The dimensionality of the matrix ``my_data_adj`` will be identical to
-``my_data``: **N_samples x N_features**
+The dimensionality of the matrix `my_data_adj` will be identical to
+`my_data`: **N_samples x N_features**
 
 Working with NIFTI Images
 -------------------------
 
-To work with NIFTI images, you compute a mask using a ``pandas.DataFrame`` which
+To work with NIFTI images, you compute a mask using a `pandas.DataFrame` which
 contains file paths for all of the images in the **training set**.
 
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
-    >>> nifti_list = pd.read_csv('brain_images_paths.csv')
-    >>> nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```python
+import pandas as pd
+import numpy as np
+from neuroHarmonize.harmonizationNIFTI import createMaskNIFTI
+nifti_list = pd.read_csv('brain_images_paths.csv')
+nifti_avg, nifti_mask, affine, hdr0 = createMaskNIFTI(nifti_list, threshold=0)
+```
 
-After the mask is created, you can flatten the images to a 2D ``numpy.array``
+After the mask is created, you can flatten the images to a 2D `numpy.array`
 very similar to what is done with the tabular data example above.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
-    >>> nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import flattenNIFTIs
+nifti_array = flattenNIFTIs(nifti_list, 'thresholded_mask.nii.gz')
+```
 
 The next step is identical to working with tabular data. You simply pass the 2D
-array to ``neuroHarmonize.harmonizationLearn``.
+array to `neuroHarmonize.harmonizationLearn`.
 
-    >>> import neuroHarmonize as nh
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
-    >>> nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```python
+import neuroHarmonize as nh
+covars = pd.read_csv('subject_info.csv')
+my_model, nifti_array_adj = nh.harmonizationLearn(nifti_array, covars)
+nh.saveHarmonizationModel(my_model, 'MY_MODEL')
+```
 
 Lastly, you can apply the model sequentially to images in a larger dataset with
-``applyModelNIFTIs``. When performing NIFTI harmonization, loading the entire set
+`applyModelNIFTIs`. When performing NIFTI harmonization, loading the entire set
 of images may exceed memory capacity. This function will reduce the burden on
 memory by applying the model to images one-by-one and saving the results as NIFTIs.
 
-    >>> from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
-    >>> # load pre-trained model
-    >>> my_model = nh.loadHarmonizationModel('MY_MODEL')
-    >>> applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```python
+from neuroHarmonize.harmonizationNIFTI import applyModelNIFTIs
+# load pre-trained model
+my_model = nh.loadHarmonizationModel('MY_MODEL')
+applyModelNIFTIs(covars, my_model, nifti_list, 'thresholded_mask.nii.gz')
+```
 
 Applying Pre-Trained Models to New Data
 ---------------------------------------
 
 This feature allows you to train a harmonization model on a subset of data, then
 apply the model to the entire set. For example, in longitudinal analyses, one may
 wish to train a harmonization model on baseline cases and apply the model to
 follow-up cases, to avoid double-counting subjects.
 
-If you have previously trained a harmonization model with ``harmonizationLearn``,
-you may apply the model parameters to new data with ``harmonizationApply``.
+If you have previously trained a harmonization model with `harmonizationLearn`,
+you may apply the model parameters to new data with `harmonizationApply`.
 
 First load the model:
 
-    >>> from neuroHarmonize import harmonizationApply, loadHarmonizationModel
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load a pre-trained model
-    >>> my_model = loadHarmonizationModel('../models/my_model')
+```python
+from neuroHarmonize import harmonizationApply, loadHarmonizationModel
+import pandas as pd
+import numpy as np
+# load a pre-trained model
+my_model = loadHarmonizationModel('../models/my_model')
+```
 
 Next, prepare the holdout data on which you will apply the model. This data
-must look exactly like the training data for ``harmonizationLearn``, including
+must look exactly like the training data for `harmonizationLearn`, including
 the same number and order of covariates. If the holdout data contains a
 different number of sites, an error will be thrown.
 
 After preparing the holdout data simply apply the model:
 
-    >>> df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
-    >>> my_holdout_data = np.array(df_holdout)
-    >>> covars = pd.read_csv('subject_info_holdout.csv')
-    >>> my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```python
+df_holdout = pd.read_csv('../data/brain_volumes_holdout.csv')
+my_holdout_data = np.array(df_holdout)
+covars = pd.read_csv('subject_info_holdout.csv')
+my_holdout_data_adj = harmonizationApply(my_holdout_data, covars, my_model)
+```
 
 Specifying Nonlinear Covariate Effects
 --------------------------------------
 
 You may specify nonlinear covariate effects with the optional argument:
-``smooth_terms``. For example, you may want to specify age as a nonlinear
+`smooth_terms`. For example, you may want to specify age as a nonlinear
 term in the harmonization model, if age exhibits nonlinear relationships with
-brain volumes. This can be done easily with ``harmonizationLearn``:
+brain volumes. This can be done easily with `harmonizationLearn`:
 
-    >>> from neuroHarmonize import harmonizationLearn
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> # load your data and all numeric covariates
-    >>> my_data = pd.read_csv('brain_volumes.csv')
-    >>> my_data = np.array(my_data)
-    >>> covars = pd.read_csv('subject_info.csv')
-    >>> # run harmonization with NONLINEAR effects of age
-    >>> my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization with NONLINEAR effects of age
+my_model, my_data_adj = harmonizationLearn(data, covars, smooth_terms=['AGE'])
+```
 
 When applying nonlinear models to holdout data, you may get an error: "some data
 points fall outside the outermost knots, and I'm not sure how to handle them".
 This is documented: https://github.com/statsmodels/statsmodels/issues/2361.
-The current workaround is to use the optional argument: ``smooth_term_bounds``,
+The current workaround is to use the optional argument: `smooth_term_bounds`,
 which controls the boundary knots for nonlinear estimation. You should specify
 boundaries that contain the limits of the entire dataset, including holdout data.
 
 Empirical Bayes
 ---------------
 
 Note the default behavior is to run the empirical Bayes (EB) step of ComBat, which
 is useful for harmonizing multiple features that are similar such as genes or
 brain regional volumes.
 
-To run without EB, simply pass the optional argument ``eb=False`` to
-``harmonizationLearn``. This is convenient when harmonizing a small number of
+To run without EB, simply pass the optional argument `eb=False` to
+`harmonizationLearn`. This is convenient when harmonizing a small number of
 features, e.g. fewer than 10.
 
-When ``eb=True``, ComBat uses Empirical Bayes to fit a prior distribution for
+When `eb=True`, ComBat uses Empirical Bayes to fit a prior distribution for
 the site effects for each site. You may wish to visualize fit of the prior
 distribution, along with the observed distribution of site effects. The following
 code example plots both distributions for the location effect of site 1.
 
-    >>> import matplotlib.pyplot as plt
-    >>> import seaborn as sns
-    >>> from neuroHarmonize import loadHarmonizationModel
-    >>> model = loadHarmonizationModel('../models/my_model')
-    >>> site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
-    >>> sns.kdeplot(site_01, color='blue', label='Site-1-prior')
-    >>> sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
-    >>> plt.show()
+```python
+import matplotlib.pyplot as plt
+import seaborn as sns
+from neuroHarmonize import loadHarmonizationModel
+model = loadHarmonizationModel('../models/my_model')
+site_01 = stats.norm.rvs(size=10000, loc=model['gamma_bar'][0], scale=np.sqrt(model['t2'][0]))
+sns.kdeplot(site_01, color='blue', label='Site-1-prior')
+sns.kdeplot(model['gamma_hat'][0, :], color='blue', label='Site-1-observed', linestyle='--')
+plt.show()
+```
+
+![Fig 1](figure_1.png)
+
+Reference Sites
+---------------
+
+Recently other implementations have been including the ability to specify a
+reference site or scanner, such that all data will be harmonized to that site.
+
+**This feature was added in version 2.4.x.** It can be used as in the following
+example:
+
+```python
+from neuroHarmonize import harmonizationLearn
+import pandas as pd
+import numpy as np
+# load your data and all numeric covariates
+my_data = pd.read_csv('brain_volumes.csv')
+my_data = np.array(my_data)
+covars = pd.read_csv('subject_info.csv')
+# run harmonization and store the adjusted data
+my_model, my_data_adj = harmonizationLearn(my_data, covars, ref_batch='SITE_A')
+```
 
-.. image:: figure_1.png
+Please submit any issues to [GitHub](https://github.com/rpomponio/neuroHarmonize/issues)
+if you run into trouble with this feature, as I am still testing its utility.
 
 Citations
 ---------
 
-.. [1] Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
+[^1]: Pomponio, R., Shou, H., Davatzikos, C., et al., (2019).
    "Harmonization of large MRI datasets for the analysis of brain imaging
    patterns throughout the lifespan." Neuroimage 208.
    https://doi.org/10.1016/j.neuroimage.2019.116450.
-.. [2] Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
+[^2]: Fortin, J. P., N. Cullen, Y. I. Sheline, W. D. Taylor, I. Aselcioglu,
    P. A. Cook, P. Adams, C. Cooper, M. Fava, P. J. McGrath, M. McInnis,
    M. L. Phillips, M. H. Trivedi, M. M. Weissman and R. T. Shinohara (2017).
    "Harmonization of cortical thickness measurements across scanners and sites."
    Neuroimage 167: 104-120. https://doi.org/10.1016/j.neuroimage.2017.11.024.
-.. [3] W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray
-   expression data using empirical Bayes methods. Biostatistics, 8(1):118-127,
-   2007. https://doi.org/10.1093/biostatistics/kxj037.
+[^3]: W. Evan Johnson and Cheng Li, Adjusting batch effects in microarray expression data using empirical Bayes methods. Biostatistics, 8(1):118-127, 2007. https://doi.org/10.1093/biostatistics/kxj037.
```

