# Comparing `tmp/boxsers-1.4.5.tar.gz` & `tmp/boxsers-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxsers-1.4.5.tar", last modified: Thu Feb 22 20:29:28 2024, max compression
+gzip compressed data, was "boxsers-1.5.0.tar", last modified: Tue Apr 23 16:35:05 2024, max compression
```

## Comparing `boxsers-1.4.5.tar` & `boxsers-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 20:29:28.654356 boxsers-1.4.5/
--rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0     8731 2024-02-22 20:29:28.653353 boxsers-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    11442 2023-11-28 21:03:07.000000 boxsers-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 20:29:28.577099 boxsers-1.4.5/boxsers/
--rw-rw-rw-   0        0        0      775 2023-10-06 21:02:47.000000 boxsers-1.4.5/boxsers/__init__.py
--rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.4.5/boxsers/_boxsers_utils.py
--rw-rw-rw-   0        0        0    27673 2023-11-08 14:07:28.000000 boxsers-1.4.5/boxsers/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2024-02-22 20:29:28.652345 boxsers-1.4.5/boxsers/machine_learning/
--rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.4.5/boxsers/machine_learning/__init__.py
--rw-rw-rw-   0        0        0    12773 2023-11-14 19:19:54.000000 boxsers-1.4.5/boxsers/machine_learning/classification.py
--rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.4.5/boxsers/machine_learning/clustering.py
--rw-rw-rw-   0        0        0      180 2023-10-19 19:42:30.000000 boxsers-1.4.5/boxsers/machine_learning/deep_interpretability.py
--rw-rw-rw-   0        0        0    24227 2024-01-23 20:00:10.000000 boxsers-1.4.5/boxsers/machine_learning/dimension_reduction.py
--rw-rw-rw-   0        0        0    33875 2024-02-22 19:34:21.000000 boxsers-1.4.5/boxsers/machine_learning/neural_networks.py
--rw-rw-rw-   0        0        0     7950 2023-09-29 17:15:02.000000 boxsers-1.4.5/boxsers/machine_learning/validation_metrics.py
--rw-rw-rw-   0        0        0    11213 2023-11-23 20:29:48.000000 boxsers-1.4.5/boxsers/misc_tools.py
--rw-rw-rw-   0        0        0    13661 2024-02-22 20:21:30.000000 boxsers-1.4.5/boxsers/preprocessing.py
--rw-rw-rw-   0        0        0    18846 2024-01-24 17:00:34.000000 boxsers-1.4.5/boxsers/visual_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-22 20:29:28.600853 boxsers-1.4.5/boxsers.egg-info/
--rw-rw-rw-   0        0        0     8731 2024-02-22 20:29:28.000000 boxsers-1.4.5/boxsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2024-02-22 20:29:28.000000 boxsers-1.4.5/boxsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 20:29:28.000000 boxsers-1.4.5/boxsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-02-22 20:29:28.000000 boxsers-1.4.5/boxsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-22 20:29:28.000000 boxsers-1.4.5/boxsers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 20:29:28.654356 boxsers-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1096 2024-02-22 20:26:55.000000 boxsers-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.392550 boxsers-1.5.0/
+-rw-rw-rw-   0        0        0     1093 2021-08-13 16:59:11.000000 boxsers-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     8731 2024-04-23 16:35:05.391325 boxsers-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11442 2023-11-28 21:03:07.000000 boxsers-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.307386 boxsers-1.5.0/boxsers/
+-rw-rw-rw-   0        0        0      775 2023-10-06 21:02:47.000000 boxsers-1.5.0/boxsers/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-07-15 15:44:15.000000 boxsers-1.5.0/boxsers/_boxsers_utils.py
+-rw-rw-rw-   0        0        0    27673 2024-04-08 16:37:26.000000 boxsers-1.5.0/boxsers/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.390411 boxsers-1.5.0/boxsers/machine_learning/
+-rw-rw-rw-   0        0        0      380 2022-07-20 13:18:32.000000 boxsers-1.5.0/boxsers/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0    12773 2023-11-14 19:19:54.000000 boxsers-1.5.0/boxsers/machine_learning/classification.py
+-rw-rw-rw-   0        0        0     7295 2022-07-13 19:35:31.000000 boxsers-1.5.0/boxsers/machine_learning/clustering.py
+-rw-rw-rw-   0        0        0      180 2023-10-19 19:42:30.000000 boxsers-1.5.0/boxsers/machine_learning/deep_interpretability.py
+-rw-rw-rw-   0        0        0    24227 2024-01-23 20:00:10.000000 boxsers-1.5.0/boxsers/machine_learning/dimension_reduction.py
+-rw-rw-rw-   0        0        0    33878 2024-03-06 17:32:40.000000 boxsers-1.5.0/boxsers/machine_learning/neural_networks.py
+-rw-rw-rw-   0        0        0     9399 2024-02-23 17:02:55.000000 boxsers-1.5.0/boxsers/machine_learning/validation_metrics.py
+-rw-rw-rw-   0        0        0    11346 2024-03-06 18:00:45.000000 boxsers-1.5.0/boxsers/misc_tools.py
+-rw-rw-rw-   0        0        0    17859 2024-04-23 16:28:45.000000 boxsers-1.5.0/boxsers/preprocessing.py
+-rw-rw-rw-   0        0        0    18846 2024-01-24 17:00:34.000000 boxsers-1.5.0/boxsers/visual_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:35:05.336614 boxsers-1.5.0/boxsers.egg-info/
+-rw-rw-rw-   0        0        0     8731 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 16:35:05.000000 boxsers-1.5.0/boxsers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 16:35:05.392550 boxsers-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2024-04-23 16:33:15.000000 boxsers-1.5.0/setup.py
```

### Comparing `boxsers-1.4.5/LICENSE.txt` & `boxsers-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/PKG-INFO` & `boxsers-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.4.5
+Version: 1.5.0
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.4.5/README.md` & `boxsers-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/__init__.py` & `boxsers-1.5.0/boxsers/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/_boxsers_utils.py` & `boxsers-1.5.0/boxsers/_boxsers_utils.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/data_augmentation.py` & `boxsers-1.5.0/boxsers/data_augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,20 +522,20 @@
         slope_range : float or integer, list or tuple
             Values delimiting the range of possible values for random slope. These values can be
             specified as follows:
                 - slope_range = (a, b) or [a, b] --> a is the left limit value and b is the right limit value.
                 - slope_range = a --> -a is the left limit value and +a is the right limit value.
 
         xinter_range : float or integer, list or tuple
-            Values delimiting the possible random values for the x-intersept. These values are specified the
+            Values delimiting the possible random values for the x-intercept. These values are specified the
             same way as "slope_range". If = 0, the x-intercept will be at the left end of the spectrum, and
             if =1 at the right end.
 
         yinter_range : float or integer, list or tuple
-            Values delimiting the possible random values for the y-intersept. Same effect as adding an offset
+            Values delimiting the possible random values for the y-intercept. Same effect as adding an offset
             with the function "aug_ioffset". These values are specified the same way as "slope_range".
 
         quantity : integer, default=1
             Quantity of new spectra generated for one spectrum. If less than or equal to zero, no new
             spectrum is generated.
 
         shuffle_enabled : boolean, default=True
```

### Comparing `boxsers-1.4.5/boxsers/machine_learning/classification.py` & `boxsers-1.5.0/boxsers/machine_learning/classification.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/machine_learning/clustering.py` & `boxsers-1.5.0/boxsers/machine_learning/clustering.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/machine_learning/dimension_reduction.py` & `boxsers-1.5.0/boxsers/machine_learning/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers/machine_learning/neural_networks.py` & `boxsers-1.5.0/boxsers/machine_learning/neural_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from tensorflow.keras.models import load_model
 from sklearn.metrics import precision_recall_fscore_support
 from skimage.transform import resize
 import time
 import matplotlib.pyplot as plt
 import numpy as np
 from boxsers._boxsers_utils import _lightdark_switch
-from typing import Union, List
-from numpy.typing import ArrayLike
+from typing import Union
 
 
 class SpectroCNN:
     """ Convolutional Neural Network (CNN) for vibrational spectra classification.
 
     Parameters:
         shape_in : non-zero positive integer value
@@ -33,15 +32,15 @@
 
         shape_out : non-zero positive integer value
             Number of output classes.
 
         ks : Odd positive integer value, default=5
             Size of kernel filters.
 
-        dropout_rate : positive float integer between 0 and  1, default=0.4
+        dropout_rate : positive float between 0 and  1, default=0.4
             Dropout rate in dense layers.
 
         hidden_activation : string, default='relu'
             Hidden layer activation function.
 
         architecture : string, default='ConvModel'
 
@@ -164,15 +163,15 @@
             else:  # loss_function is not a string
                 self.loss_function = loss_function
                 self.hyperparameter_dict["Loss function"] = self.loss_function.__class__.__name__
 
         # model compilation
         self.model.compile(loss=self.loss_function, optimizer=self.optimizer, metrics=self.metrics)
 
-    def print_info(self, structure=True, hyperparameters=True):
+    def print_info(self, structure=True, hyperparameters=False):
         """ Prints CNN model information.
 
         Parameters:
             structure : boolean, default=True
                 If true, prints the structure of the CNN model with each of its layers.
 
             hyperparameters : boolean, default=True
@@ -199,29 +198,31 @@
             monit : {'acc', 'loss', 'val_acc', 'val_loss'}, default='val_loss'
                 Metric used to determine whether or not the model is improving. The metrics 'val_acc'
                 and 'val_loss' are not available if val_data=None in 'self.train_model' method.
         """
         es = EarlyStopping(monitor=monit, patience=epoch, verbose=1)
         self.callbacks.append(es)
 
-    def config_modelcheckpoint(self, save_path='best_model', monit='val_acc'):
+    def config_modelcheckpoint(self, save_path='best_model', monit='val_acc', verbose=2):
         """ Configures a checkpoint during CNN model training.
 
         Stores the model with the best performance and reinstores it at the end of training.
 
         Parameters:
-            save_path : string, default='best_model
+            save_path : string, default='best_model'
                 Path where the model is saved
 
             monit : {'acc', 'loss', 'val_acc', 'val_loss'}, default='val_loss'
                 Metric used to determine whether or not the model is improving. The metrics 'val_acc'
                 and 'val_loss' are not available if val_data=None in 'self.train_model' method.
+
+            verbose : int, default=2
         """
         self.modelcheckpoint_path = save_path
-        mc = ModelCheckpoint(monitor=monit, filepath=self.modelcheckpoint_path, verbose=2, save_best_only=True)
+        mc = ModelCheckpoint(monitor=monit, filepath=self.modelcheckpoint_path, verbose=verbose, save_best_only=True)
         self.callbacks.append(mc)
 
     def train_model(self, x_train, y_train, val_data=None, batch_size=92, n_epochs=25, reset_callbacks=True,
                     plot_history=True, verbose=1):
         """ Train the model on a given set of spectra.
 
         Parameters:
@@ -387,15 +388,15 @@
         # adjusts subplot params so that the subplot(s) fits in to the figure area
         fig.tight_layout()
         # save figure
         if save_path is not None:
             plt.savefig(save_path, dpi=300, bbox_inches='tight')
         plt.show()
 
-    def predict_classes(self, x_test, threshold: Union[float, list] = 0.5, return_integers=True, sums_classes=False):
+    def predict_classes(self, x_test, threshold=0.5, return_integers=True, sums_classes=False):
         """ Predicts classes for the input spectra.
 
         Notes:
             This function must be preceded by the 'train_model()' function in order to properly work.
 
         Parameters:
             x_test : array_like
@@ -616,16 +617,17 @@
         """
         warnings.warn('\'get_conf_matrix\' instance method is no longer supported, use instead'
                       ' the standalone \'cf_matrix\' method found in boxsers.validation_metrics module.',
                       DeprecationWarning)
 
 
 # Convolutional neural network architectures ----------------------------------------------------------
-def conv_model(shape_in, shape_out, nf_0=6, n_conv_layers=3, dense_layers_size=None,  ks=5, batchnorm=True, dropout_rate=0.3,
-               hidden_activation='relu', output_activation='softmax', reshaping_layer='flatten'):
+def conv_model(shape_in, shape_out, nf_0=6, n_conv_layers=3, dense_layers_size=None,  ks=5, batchnorm=True,
+               dropout_rate=0.3, hidden_activation='relu', output_activation='softmax',
+               reshaping_layer='flatten'):
     """
     Returns a CNN model with an architecture based on AlexNet.
 
         Fixed hyperparameters:
             - 3 conv layer, kernel filters number doubles from one convolutional layer to the next one.
             - 2 dense layer (1000, 500) neurons fixed
```

### Comparing `boxsers-1.4.5/boxsers/machine_learning/validation_metrics.py` & `boxsers-1.5.0/boxsers/machine_learning/validation_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 School : Université Laval (Qc, Canada)
 
 This module provides different tools to evaluate the quality of a model’s predictions.
 """
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
-from sklearn.metrics import classification_report, confusion_matrix
+from sklearn.metrics import classification_report, confusion_matrix, precision_recall_curve
 from boxsers._boxsers_utils import _lightdark_switch
 
 
 def cf_matrix(y_true, y_pred, normalize='true', class_names=None, title=None,
               xlabel='Predicted label', ylabel='True label', darktheme=False,
               color_map='Blues', fmt='.2f', fontsize=10, fig_width=5.5, fig_height=5.5,
               save_path=None):
@@ -183,9 +183,41 @@
     if save_path is not None:
         text_file = open(save_path, "w")
         text_file.write(report)
         text_file.close()
     return report
 
 
+def fbeta_threshold(y_true, y_pred, beta=1.0, pred_index=0):
+    """ Return a threshold value that maximizes the fbeta score.
+
+    Parameters:
+        y_true : array
+            True labels. Array shape = (n_spectra,) for integer labels
+            and (n_spectra, n_classes) for binary labels.
+
+        y_pred : array
+            Predicted labels. Array shape = (n_spectra, n_classes) for binary labels.
+        
+        beta : non-zero positive float value, default=1.0
+            Determines importance ratio between recall and precision in the calculation of
+            the Fbeta value. A beta = 1 results in the conventional F1 score, a beta > 1 focuses
+            more on the recall and a beta < 1 focuses more on the precision.
+
+        pred_index : int, default=0
+            Used to specify the class that needs to be analyzed.
+
+    Returns:
+        float : Threshold value that maximizes the f_beta score.
+    """
+    # Precision-recall curve computation
+    precision, recall, thresholds = precision_recall_curve(y_true[:, pred_index], y_pred[:, pred_index])
+    # f_beta score calculation
+    f_beta = ((1 + beta**2) * precision * recall)/(beta**2 * precision + recall)
+    # Determining the threshold value that maximizes the f_beta score
+    optimal_threshold_index = np.argmax(f_beta)
+    optimal_threshold = thresholds[optimal_threshold_index]
+    return optimal_threshold
+
+
 if __name__ == "__main__":
     help(__name__)
```

### Comparing `boxsers-1.4.5/boxsers/misc_tools.py` & `boxsers-1.5.0/boxsers/misc_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,17 @@
         batch_size = int(batch_size * sp.shape[0])
     else:
         batch_size = batch_size
 
     random_row = np.random.choice(sp.shape[0], size=batch_size, replace=False)
     sp_sample = sp[random_row, :]
     if lab is not None:
+        if lab.ndim == 1:
+            # lab is forced to be a two-dimensional array
+            lab = np.expand_dims(lab, axis=1)
         lab_sample = lab[random_row, :]
         return sp_sample, lab_sample
     return sp_sample
 
 
 def find_classes_index(lab_array, *labels):
     """
```

### Comparing `boxsers-1.4.5/boxsers/preprocessing.py` & `boxsers-1.5.0/boxsers/preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,30 +93,31 @@
     n_spectra, sp_length = sp.shape  # number of spectra, spectrum length
 
     # initialization and space allocation
     baseline = np.zeros(sp.shape)  # baseline signal array
     indexes = np.arange(sp_length)
 
     for i in range(n_spectra):
-        # find the convex hull vertices
+        # find the vertices of the spectrum's convex hull
         convex_v = ConvexHull(np.array(list(zip(indexes, sp[i])))).vertices
-        # rotate convex hull vertices until they start from the lowest one
+        # rolls the vertex indices of the convex hull until they start from the lowest element of the array
         convex_v = np.roll(convex_v, -convex_v.argmin())
-        # leave only the ascending part
-        convex_v = convex_v[:convex_v.argmax()]
+        # keeps only the ascending part of the vertexes determined above
+        convex_v = convex_v[:(convex_v.argmax()+1)]
 
-        # create baseline using linear interpolation between vertices
+        # baseline is generated by linear interpolation between the remaining vertices
         baseline[i] = np.interp(indexes, indexes[convex_v], sp[i, convex_v])
 
     if return_baseline:
+        # returns the baseline signal if requested
         return sp - baseline, baseline
     return sp - baseline
 
 
-def cosmic_filter(sp, ks=3):
+def _deprecated_cosmic_filter(sp, ks=3):
     """
     Apply a median filter to the spectrum(s) to remove cosmic rays.
 
     Parameters:
         sp : array
             Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
              for a single spectrum.
@@ -130,14 +131,69 @@
     """
     sp = np.array(sp, ndmin=2)  # sp is forced to be a two-dimensional array
     ks_1d = (1, ks)
     sp_med = medfilt(sp, ks_1d)  # from scipy
     return sp_med
 
 
+def cosmic_filter(sp, width=3, threshold=11.0):
+    """
+    Suppresses cosmic rays using a sliding window that compares each portion of each spectrum with the other spectra.
+
+    Notes:
+        - Does not work for an individual spectrum, since this function relies on other spectra
+           to determine the presence of a cosmic peak in a spectrum.
+        - The cosmic peak is replaced by the linear interpolation of the two closest values of the window.
+
+    Parameters:
+        sp : array
+            Input Spectrum(s). Array shape = (n_spectra, n_pixels). Does not work for an individual
+             spectrum.
+
+        width : positive odd integer, default = 7
+            Size(in pixel) of the moving window.
+
+        threshold : positive float, default = 11.0
+            Threshold used to detect cosmic peaks. This threshold is multiplied by the standard deviation
+             and compare to the median of the moving window
+
+    Returns:
+        (array) Filtered spectrum(s). Array shape = (n_spectra, n_pixels).
+    """
+    half_width = width // 2  # integer division
+    # To avoid modifying the original spectra
+    sp = sp.copy()
+    filtered_spectrum = sp.copy()
+
+    if sp.ndim == 1 or (sp.ndim == 2 and sp.shape[0] == 1):
+        raise ValueError('This function does not work for an individual spectrum, since it'
+                         ' relies on other spectra to determine the presence of a cosmic peak'
+                         ' in a spectrum.')
+
+    for i in range(half_width, sp.shape[1] - half_width):  # window slides over the spectral axis.
+        window = sp[:, i - half_width:i + half_width + 1]
+        median_value = np.median(window)  # median value of the window for the entire sp dataset
+        std_value = np.std(window)  # std value of the window for the entire sp dataset
+
+        abs_diff = np.abs(sp[:, i] - median_value)
+        # Returns a mask with True values where cosmic peaks are detected
+        cosmspike_mask = abs_diff > threshold * std_value
+
+        for n in range(sp.shape[0]):  # loop over the spectra
+            if cosmspike_mask[n]:  # a cosmic peak was detected
+                # Following max and min function are used for spectrum edge cases
+                left_index = max(i - half_width - 1, 0)
+                right_index = min(i + half_width + 1, sp.shape[1] - 1)
+                left_value = sp[n, left_index]
+                right_value = sp[n, right_index]
+                # Cosmic peak detected are removed by linear interpolation
+                filtered_spectrum[n, i] = np.interp(i, [left_index, right_index], [left_value, right_value])
+    return filtered_spectrum
+
+
 def spectral_normalization(sp, norm='l2', wn=None, band=None):
     """ Normalizes the spectrum(s) using one of the available norms in this function.
 
     Notes:
         The snv norm corresponds to 'Standard Normal Variate' method.
 
     Parameters:
@@ -180,15 +236,15 @@
     if norm == 'minmax':
         return (sp-sp_min)/(sp_max-sp_min)
     if norm == 'snv':
         return (sp-sp_mean)/sp_std
     if norm == 'band':
         # band conversion to index
         ind = (np.abs(wn-band)).argmin()
-        return sp/sp[:, ind]
+        return sp/sp[:, ind, np.newaxis]  # np.newaxis is used to obtain an array of size (n_spectres, 1)
     else:
         raise ValueError(norm, 'is not among the following valid choices:\'l2\', \'l1\', \'max\', \'minmax\', \'snv\'')
 
 
 def savgol_smoothing(sp, window_length=9, p=3, degree=0):
     """
     Smoothes the spectrum(s) using a Savitzky-Golay polynomial filter.
@@ -212,67 +268,98 @@
                 for a single spectrum.
     """
     #  Scipy's Savitzky-Golay filter is used
     sp_svg = savgol_filter(sp, window_length, polyorder=p, deriv=degree)  # from Scipy
     return sp_svg
 
 
-def spectral_cut(sp, wn, wn_start, wn_end, sub_mode='zero'):
+def spectral_cut(sp, wn, wn_start, wn_end, sub_mode='zero', keep_it=False, reduce_gap=False):
     """
-    Subtracts or sets to zero a delimited spectral region of the spectrum(s)
+    Subtracts or sets to zero a spectral region of the spectrum(s) bounded by [wn_start, wn_end]. Can also
+    be used to keep only the delimited part of the spectrum.
 
     Parameters:
         sp : array
             Input Spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
              for a single spectrum.
 
         wn : array
             X-axis(wavenumber, wavelenght, Raman shift, etc.) used for the spectra. Array shape = (n_pixels, ).
 
         wn_start : Int or float
             Starting point (same unit as wn) of the subtracted spectral region.
 
         wn_end : Int or float
-            Ending point (same unit as wn) of the subtracted spectral region.
+            Ending point (same unit as wn) of the subtracted spectral region. d
 
         sub_mode : {'zero', 'remove'}, default='zero'
             Determines how the subtracted part of the spectrum is handled.
                 - 'zero': The subtracted part of the spectrum is set to zero.
-                - 'remove': The subtracted part of the spectrum is removed and the remaining parts are joined together.
+                - 'remove': The subtracted part of the spectrum is removed.
+
+        keep_it : boolean, default=False
+            If True, keeps the specified region instead and subtracts the rest.
+
+        reduce_gap : boolean, default=False
+            If True, reduces the gap to zero between the left and right parts to minimize discontinuity.
 
     Returns:
         (array) Cutted spectrum(s). Array shape = (n_spectra, n_pixels) for multiple spectra and (n_pixels,)
                 for a single spectrum.
 
         (array) New x-axis( if sub_mode = 'removed') or the intial one(if sub_mode = 'zero').
                 Array shape = (n_pixels, ).
     """
+    sp = sp.copy()
     # sp is forced to be a two-dimensional array
     sp = np.array(sp, ndmin=2)
     # conversion to indexes
     i_start = (np.abs(wn - wn_start)).argmin()
     i_end = (np.abs(wn - wn_end)).argmin()
-    if sub_mode == 'zero':
-        # preserved part on the left side of the spectral cut
-        sp[:, i_start:i_end] = 0
-        return sp, wn
 
-    elif sub_mode == 'remove':
-        # preserved part on the left side of the spectral cut
-        sp_l = sp[:, 0:i_start]
-        wn_l = wn[0:i_start]
-        # preserved part on the right side of the spectral cut
-        sp_r = sp[:, i_end:]
-        wn_r = wn[i_end:]
-        # remaining parts are joined together
-        sp_cut = np.concatenate([sp_l, sp_r], axis=1)
-        wn_cut = np.concatenate([wn_l, wn_r])
-        return sp_cut, wn_cut
+    intensity_left = sp[:, i_start]
+    intensity_right = sp[:, i_end]
 
-    raise ValueError('invalid sub_mode among \'zero\' and \'remove\'')
+    # intensity gap determination
+    intensity_gap = intensity_left - intensity_right
+    intensity_gap = np.expand_dims(intensity_gap, axis=1)
+
+    if sub_mode not in ['zero', 'remove']:
+        raise ValueError('Invalid sub_mode, must be \'zero\' or \'remove\'')
+
+    if keep_it:
+        if sub_mode == 'zero':
+            sp[:, :i_start] = 0  # sets the left side part of the spectral cut to zero
+            sp[:, i_end + 1:] = 0  # sets the right side part of the spectral cut to zero
+
+        elif sub_mode == 'remove':
+            sp = sp[:, i_start:i_end + 1]
+            wn = wn[i_start:i_end + 1]
+        return sp, wn
+    else:
+        if sub_mode == 'zero':
+            # preserved part on the left side of the spectral cut
+            sp[:, i_start:i_end+1] = 0
+            return sp, wn
+
+        elif sub_mode == 'remove':
+            # preserves the left side part of the spectral cut
+            sp_l = sp[:, 0:i_start]
+            wn_l = wn[0:i_start]
+            # preserves the right side part of the spectral cut
+            sp_r = sp[:, i_end+1:]
+            wn_r = wn[i_end+1:]
+            if reduce_gap:
+                # Reduces the gap to zero between the left and right parts
+                sp_r = sp_r + intensity_gap
+
+            # remaining parts are joined together
+            sp_cut = np.concatenate([sp_l, sp_r], axis=1)
+            wn_cut = np.concatenate([wn_l, wn_r])
+            return sp_cut, wn_cut
 
 
 def spline_interpolation(sp, wn, new_wn, degree=1, same_w=False):
     """
     Performs a one-dimensional interpolation spline on the spectra to reproduce them with a new x-axis.
 
     Parameters:
```

### Comparing `boxsers-1.4.5/boxsers/visual_tools.py` & `boxsers-1.5.0/boxsers/visual_tools.py`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/boxsers.egg-info/PKG-INFO` & `boxsers-1.5.0/boxsers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsers
-Version: 1.4.5
+Version: 1.5.0
 Summary: Python package that provides a full range of functionality to process and analyze vibrational spectra (Raman, SERS, FTIR, etc.).
 Home-page: https://github.com/ALebrun-108/BoxSERS
 Author: Alexis Lebrun
 Author-email: alexis.lebrun.1@ulaval.ca
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boxsers-1.4.5/boxsers.egg-info/SOURCES.txt` & `boxsers-1.5.0/boxsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxsers-1.4.5/setup.py` & `boxsers-1.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     author='Alexis Lebrun',
     author_email='alexis.lebrun.1@ulaval.ca',
     # dependencies
     install_requires=['numpy', 'pandas', 'matplotlib', 'seaborn', 'scipy', 'scikit-learn', 'tensorflow',
                       'tables', 'scikit-image'],
     python_requires='>=3.6',
     # *strongly* suggested for sharing
-    version='1.4.5',
+    version='1.5.0',
     # The license can be anything you like
     license='MIT',
     description='Python package that provides a full range of functionality to process and analyze vibrational'
                 ' spectra (Raman, SERS, FTIR, etc.).',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README_pypi.md').read(),
     long_description_content_type="text/markdown",
```

