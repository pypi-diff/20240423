# Comparing `tmp/crawlnet-0.0.3.tar.gz` & `tmp/crawlnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.3.tar", last modified: Tue Apr 23 13:17:00 2024, max compression
+gzip compressed data, was "crawlnet-0.0.4.tar", last modified: Tue Apr 23 17:28:39 2024, max compression
```

## Comparing `crawlnet-0.0.3.tar` & `crawlnet-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.321701 crawlnet-0.0.3/
--rw-rw-rw-   0        0        0      794 2024-04-23 13:17:00.321701 crawlnet-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.259197 crawlnet-0.0.3/crawlnet/
--rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.3/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    21573 2024-04-23 13:16:42.000000 crawlnet-0.0.3/crawlnet/cl3.py
--rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.3/crawlnet/cl4.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.321701 crawlnet-0.0.3/crawlnet.egg-info/
--rw-rw-rw-   0        0        0      794 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 13:17:00.321701 crawlnet-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-04-23 13:16:22.000000 crawlnet-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:28:39.333965 crawlnet-0.0.4/
+-rw-rw-rw-   0        0        0      794 2024-04-23 17:28:39.333965 crawlnet-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 17:28:39.312222 crawlnet-0.0.4/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.4/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    23781 2024-04-23 17:25:04.000000 crawlnet-0.0.4/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.4/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:28:39.333965 crawlnet-0.0.4/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0      794 2024-04-23 17:28:39.000000 crawlnet-0.0.4/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-23 17:28:39.000000 crawlnet-0.0.4/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:28:39.000000 crawlnet-0.0.4/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-23 17:28:39.000000 crawlnet-0.0.4/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 17:28:39.000000 crawlnet-0.0.4/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 17:28:39.343069 crawlnet-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-23 14:05:59.000000 crawlnet-0.0.4/setup.py
```

### Comparing `crawlnet-0.0.3/PKG-INFO` & `crawlnet-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.3/crawlnet/cl3.py` & `crawlnet-0.0.4/crawlnet/cl3.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,16 @@
 # To run use commands
 pyro4-ns
 python server2.py
 python client2.py
 """
 
 mapreduce_character_count = """
+!pip install mrjob
+
 # character_count.py
 from mrjob.job import MRJob
 import sys
 
 class CharacterCount(MRJob):
     
     def mapper(self, _, line):
@@ -161,14 +163,18 @@
     WordCount.run()
 ##############################################################
 
 # x.txt    
 Dr D y Patil Institute Of Engineering Management And Research , Akurdi
 
 ##############################################################
+
+### To run
+python3 .\character_count.py x.txt
+python3 .\word_count.py x.txt
 """
 
 fuzzy_sets_u_n = """
 A = dict()
 B = dict()
 Y = dict()
 
@@ -576,15 +582,15 @@
 print("Accuracy:", accuracy)
 
 
 print("Classification Report:")
 print(classification_report(y_test, y_pred))
 """
 
-art_neural_style_transfer = """
+art_neural_style_transfer_1 = """
 !pip install tensorflow
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras.applications import vgg19
 from tensorflow.keras.preprocessing import image as keras_image
 from tensorflow.keras import backend as K
@@ -669,25 +675,94 @@
 
 # Display the final stylized image
 plt.imshow(final_image)
 plt.axis('off')
 plt.show()
 """
 
+art_neural_style_transfer_2 = """
+import os
+import tensorflow as tf
+# Load compressed models from tensorflow_hub
+os.environ['TFHUB_MODEL_LOAD_FORMAT'] = 'COMPRESSED'
+
+import IPython.display as display
+
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+mpl.rcParams['figure.figsize'] = (12, 12)
+mpl.rcParams['axes.grid'] = False
+
+import numpy as np
+import PIL.Image
+import time
+import functools
+
+def tensor_to_image(tensor):
+  tensor = tensor*255
+  tensor = np.array(tensor, dtype=np.uint8)
+  if np.ndim(tensor)>3:
+    assert tensor.shape[0] == 1
+    tensor = tensor[0]
+  return PIL.Image.fromarray(tensor)
+
+content_path = tf.keras.utils.get_file('YellowLabradorLooking_new.jpg', 'https://storage.googleapis.com/download.tensorflow.org/example_images/YellowLabradorLooking_new.jpg')
+style_path = tf.keras.utils.get_file('kandinsky5.jpg','https://storage.googleapis.com/download.tensorflow.org/example_images/Vassily_Kandinsky%2C_1913_-_Composition_7.jpg')
+
+def load_img(path_to_img):
+  max_dim = 512
+  img = tf.io.read_file(path_to_img)
+  img = tf.image.decode_image(img, channels=3)
+  img = tf.image.convert_image_dtype(img, tf.float32)
+
+  shape = tf.cast(tf.shape(img)[:-1], tf.float32)
+  long_dim = max(shape)
+  scale = max_dim / long_dim
+
+  new_shape = tf.cast(shape * scale, tf.int32)
+
+  img = tf.image.resize(img, new_shape)
+  img = img[tf.newaxis, :]
+  return img
+
+def imshow(image, title=None):
+  if len(image.shape) > 3:
+    image = tf.squeeze(image, axis=0)
+
+  plt.imshow(image)
+  if title:
+    plt.title(title)
+
+content_image = load_img(content_path)
+style_image = load_img(style_path)
+
+plt.subplot(1, 2, 1)
+imshow(content_image, 'Content Image')
+
+plt.subplot(1, 2, 2)
+imshow(style_image, 'Style Image')
+
+import tensorflow_hub as hub
+hub_model = hub.load('https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2')
+stylized_image = hub_model(tf.constant(content_image), tf.constant(style_image))[0]
+tensor_to_image(stylized_image)
+"""
+
 masterDict = {
     "rpc": rpc,
     "rmi": rmi,
     "mapreduce_character_count": mapreduce_character_count,
     "fuzzy_sets_u_n": fuzzy_sets_u_n,
     "optimize_gen_algo_spray_dry": optimize_gen_algo_spray_dry,
     "clonal_select_algo": clonal_select_algo,
     "Deap": Deap,
     "ant_colony": ant_colony,
     "arti_immune_pr_damage_class": arti_immune_pr_damage_class,
-    "art_neural_style_transfer": art_neural_style_transfer
+    "art_neural_style_transfer_1": art_neural_style_transfer_1,
+    "art_neural_style_transfer_2": art_neural_style_transfer_2
 }
 
 
 class Writer:
     def __init__(self, filename):
         self.filename = os.path.join(os.getcwd(), filename)
         self.masterDict = masterDict
```

### Comparing `crawlnet-0.0.3/crawlnet/cl4.py` & `crawlnet-0.0.4/crawlnet/cl4.py`

 * *Files identical despite different names*

### Comparing `crawlnet-0.0.3/crawlnet.egg-info/PKG-INFO` & `crawlnet-0.0.4/crawlnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.3/setup.py` & `crawlnet-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "CrawlNet"
 
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

