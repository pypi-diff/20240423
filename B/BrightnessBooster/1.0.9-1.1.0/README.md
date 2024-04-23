# Comparing `tmp/BrightnessBooster-1.0.9.tar.gz` & `tmp/BrightnessBooster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrightnessBooster-1.0.9.tar", last modified: Tue Apr  9 19:23:45 2024, max compression
+gzip compressed data, was "BrightnessBooster-1.1.0.tar", last modified: Tue Apr 23 13:18:18 2024, max compression
```

## Comparing `BrightnessBooster-1.0.9.tar` & `BrightnessBooster-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.095174 BrightnessBooster-1.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.065478 BrightnessBooster-1.0.9/BrightnessBooster/
--rw-rw-rw-   0        0        0      304 2024-04-09 18:12:38.000000 BrightnessBooster-1.0.9/BrightnessBooster/__init__.py
--rw-rw-rw-   0        0        0     9132 2024-04-09 19:23:06.000000 BrightnessBooster-1.0.9/BrightnessBooster/brightnessbooster.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.093245 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/
--rw-rw-rw-   0        0        0     3072 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3072 2024-04-09 19:23:45.095174 BrightnessBooster-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2024-04-09 19:03:55.000000 BrightnessBooster-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 19:23:45.097175 BrightnessBooster-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      566 2024-04-09 19:23:28.000000 BrightnessBooster-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:18:18.587684 BrightnessBooster-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-23 13:18:18.552641 BrightnessBooster-1.1.0/BrightnessBooster/
+-rw-rw-rw-   0        0        0      304 2024-04-09 18:12:38.000000 BrightnessBooster-1.1.0/BrightnessBooster/__init__.py
+-rw-rw-rw-   0        0        0    11955 2024-04-23 13:11:40.000000 BrightnessBooster-1.1.0/BrightnessBooster/brightnessbooster.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:18:18.584686 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/
+-rw-rw-rw-   0        0        0     3072 2024-04-23 13:18:18.000000 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-23 13:18:18.000000 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:18:18.000000 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 13:18:18.000000 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-23 13:18:18.000000 BrightnessBooster-1.1.0/BrightnessBooster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3072 2024-04-23 13:18:18.588685 BrightnessBooster-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2024-04-19 15:19:39.000000 BrightnessBooster-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:18:18.593697 BrightnessBooster-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      566 2024-04-23 13:16:41.000000 BrightnessBooster-1.1.0/setup.py
```

### Comparing `BrightnessBooster-1.0.9/BrightnessBooster/brightnessbooster.py` & `BrightnessBooster-1.1.0/BrightnessBooster/brightnessbooster.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from scipy import special
 import numpy as np
 from scipy.optimize import lsq_linear
+import torch
+import piq
+import scipy.optimize
+import cv2
 
 
 def calculate_brightness_and_contrast(image):
     blue = image[:,:,0]
     blue = np.concatenate(blue)
     green = image[:,:,1]
     green = np.concatenate(green)
@@ -58,15 +62,14 @@
         a = ((u*u) - (u*u*u) - (u * s)) / s
         b = ((u*u*u) - (2 * (u*u)) + u + (u - 1) * s) / s
 
         return [a, b]
         
 
 def beta_parameters_of_image(image):
-    
     blue = image[:,:,0]
     blue = np.concatenate(blue)
     green = image[:,:,1]
     green = np.concatenate(green)
     red = image[:,:,2]
     red = np.concatenate(red)
 
@@ -82,23 +85,20 @@
     norm_sorted_red_values = red_sorted_values / 255
     norm_sorted_green_values = green_sorted_values / 255
     norm_sorted_blue_values = blue_sorted_values / 255
 
 
     red_mean = np.mean(norm_sorted_red_values)
     red_variance = np.var(norm_sorted_red_values)
-    red_variance = red_variance * red_variance
 
     green_mean = np.mean(norm_sorted_green_values)
     green_variance = np.var(norm_sorted_green_values)
-    green_variance = green_variance * green_variance
 
     blue_mean = np.mean(norm_sorted_blue_values)
     blue_variance = np.var(norm_sorted_blue_values)
-    blue_variance = blue_variance * blue_variance
 
     red_a, red_b = calculate_beta_parameters(red_mean, red_variance)
     green_a, green_b = calculate_beta_parameters(green_mean, green_variance)
     blue_a, blue_b = calculate_beta_parameters(blue_mean, blue_variance)
 
     return red_a, red_b, green_a, green_b, blue_a, blue_b
 
@@ -258,12 +258,116 @@
 
     max = np.max(data)
     norm_sorted_values = sorted_values / max
 
 
     mean = np.mean(norm_sorted_values)
     variance = np.var(norm_sorted_values)
-    variance = variance * variance
 
     a, b = calculate_beta_parameters(mean, variance)
 
-    return [a, b]
+    return [a, b]
+
+
+def get_score(img):
+    img = torch.tensor(img).permute(2, 0, 1)[None, ...] / 255.
+
+    if torch.cuda.is_available():
+        # Move to GPU to make computaions faster
+        img =img.cuda()
+
+    brisque_index: torch.Tensor = piq.brisque(img, data_range=1., reduction='none')
+    return brisque_index.item()
+
+
+def objective_function(x, img_org):
+    red_a, red_b = x
+    green_a = red_a
+    green_b = red_b
+    blue_a = red_a
+    blue_b = red_b
+    distribution_parameter = (
+        red_a, red_b, green_a, green_b, blue_a, blue_b)
+
+    restored_image = modify_brightness_distribution(img_org, distribution_parameter)
+
+
+    score = get_score(restored_image)
+    print('score =', score)
+    if score < 0:
+      score = 100
+    return score
+
+
+def get_optimal_parameters(image):
+    small_image = cv2.resize(image, (256, 256))
+    a, b = beta_parameters_of_image(image)[:2]
+    print("a, b :", a, b)
+    initial_guess = [a, b]
+    bounds = ((0.1, 10), (0.1, 10)) 
+
+    result = scipy.optimize.minimize(lambda x: objective_function(x,
+         small_image),
+         initial_guess, method='nelder-mead', bounds=bounds)
+    print("result:", result.x)
+    return result.x
+
+
+def get_the_ratios_of_averages(image):
+    blue = image[:,:,0]
+    blue = np.concatenate(blue)
+    green = image[:,:,1]
+    green = np.concatenate(green)
+    red = image[:,:,2]
+    red = np.concatenate(red)
+
+    
+    red_sorted_values = np.sort(red)
+    green_sorted_values = np.sort(green)
+    blue_sorted_values = np.sort(blue)
+
+    norm_sorted_red_values = red_sorted_values / 255
+    norm_sorted_green_values = green_sorted_values / 255
+    norm_sorted_blue_values = blue_sorted_values / 255
+
+
+    red_mean = np.mean(norm_sorted_red_values)
+    # red_variance = np.var(norm_sorted_red_values)
+    #red_variance = red_variance ** 2
+
+    green_mean = np.mean(norm_sorted_green_values)
+    # green_variance = np.var(norm_sorted_green_values)
+    #green_variance = green_variance ** 2
+
+    blue_mean = np.mean(norm_sorted_blue_values)
+    # blue_variance = np.var(norm_sorted_blue_values)
+
+    ratios = ((red_mean / green_mean), (green_mean / blue_mean), red_mean / blue_mean)
+    return ratios
+
+
+def get_parameters_from_one_chanel(image, optimal_parameters):
+    r_a, r_b = optimal_parameters
+    r_mean, r_var = calculate_mean_and_variance_for_color(r_a, r_b)
+
+    rg_ratio, gb_ratio, rb_ratio = get_the_ratios_of_averages(image)
+    
+    g_mean = r_mean / rg_ratio
+    b_mean = r_mean / rb_ratio
+
+    g_a, g_b = calculate_beta_parameters(g_mean, r_var)
+    b_a, b_b = calculate_beta_parameters(b_mean, r_var)
+
+    return (r_a, r_b, g_a, g_b, b_a, b_b)
+
+
+def optimize_brightness(image):
+    small_image = cv2.resize(image, (256, 256))
+    optimal_parameters = get_optimal_parameters(image)
+    distribution_parameters = get_parameters_from_one_chanel(image, optimal_parameters)
+    new_image = modify_brightness_distribution(image, distribution_parameters)
+
+    return new_image
+
+
+
+
```

### Comparing `BrightnessBooster-1.0.9/BrightnessBooster.egg-info/PKG-INFO` & `BrightnessBooster-1.1.0/BrightnessBooster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrightnessBooster
-Version: 1.0.9
+Version: 1.1.0
 Summary: The code enhances an image's brightness and contrast
 Home-page: UNKNOWN
 Author: necros2604
 Author-email: bair1hasykov@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BrightnessBooster-1.0.9/PKG-INFO` & `BrightnessBooster-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrightnessBooster
-Version: 1.0.9
+Version: 1.1.0
 Summary: The code enhances an image's brightness and contrast
 Home-page: UNKNOWN
 Author: necros2604
 Author-email: bair1hasykov@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BrightnessBooster-1.0.9/README.md` & `BrightnessBooster-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `BrightnessBooster-1.0.9/setup.py` & `BrightnessBooster-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from setuptools import setup
 
-version = '1.0.9'
+version = '1.1.0'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BrightnessBooster',
     version=version,
```

