# Comparing `tmp/ocrd_froc-0.5.2.tar.gz` & `tmp/ocrd_froc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrd_froc-0.5.2.tar", last modified: Thu Feb  1 13:59:19 2024, max compression
+gzip compressed data, was "ocrd_froc-0.6.1.tar", last modified: Tue Apr 23 12:23:08 2024, max compression
```

## Comparing `ocrd_froc-0.5.2.tar` & `ocrd_froc-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-02-01 13:59:19.563856 ocrd_froc-0.5.2/
--rw-r--r--   0 kba       (1000) kba       (1000)     2765 2024-02-01 13:59:19.563856 ocrd_froc-0.5.2/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)     2340 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/README.md
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-02-01 13:59:19.559856 ocrd_froc-0.5.2/ocrd_froc/
--rw-rw-r--   0 kba       (1000) kba       (1000)     3346 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/charmap.json
--rw-rw-r--   0 kba       (1000) kba       (1000)     2848 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/classmap.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-02-01 13:59:19.559856 ocrd_froc-0.5.2/ocrd_froc/cli/
--rw-rw-r--   0 kba       (1000) kba       (1000)        0 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/cli/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      362 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/cli/ocrd_cli.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3332 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/converter.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      266 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/font_map.json
--rw-rw-r--   0 kba       (1000) kba       (1000)     6512 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/froc.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    29407 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/ocrd_froc/network.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2468 2024-02-01 13:59:12.000000 ocrd_froc-0.5.2/ocrd_froc/ocrd-tool.json
--rw-rw-r--   0 kba       (1000) kba       (1000)     6717 2024-02-01 13:58:17.000000 ocrd_froc-0.5.2/ocrd_froc/processor.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-02-01 13:59:19.559856 ocrd_froc-0.5.2/ocrd_froc.egg-info/
--rw-r--r--   0 kba       (1000) kba       (1000)     2765 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)      449 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       67 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/entry_points.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       65 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       10 2024-02-01 13:59:19.000000 ocrd_froc-0.5.2/ocrd_froc.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2024-02-01 13:59:19.563856 ocrd_froc-0.5.2/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      927 2024-01-31 18:38:26.000000 ocrd_froc-0.5.2/setup.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/
+-rw-r--r--   0 kba       (1000) kba       (1000)     2745 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2320 2024-04-23 12:13:24.000000 ocrd_froc-0.6.1/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/ocrd_froc/
+-rw-rw-r--   0 kba       (1000) kba       (1000)        0 2024-04-22 12:56:29.000000 ocrd_froc-0.6.1/ocrd_froc/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3346 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/charmap.json
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2848 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/classmap.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/ocrd_froc/cli/
+-rw-rw-r--   0 kba       (1000) kba       (1000)        0 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/cli/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      362 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/cli/ocrd_cli.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3332 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/converter.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      266 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/ocrd_froc/font_map.json
+-rw-rw-r--   0 kba       (1000) kba       (1000)     6517 2024-04-23 12:13:24.000000 ocrd_froc-0.6.1/ocrd_froc/froc.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    29412 2024-04-23 12:13:24.000000 ocrd_froc-0.6.1/ocrd_froc/network.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2940 2024-04-23 12:15:01.000000 ocrd_froc-0.6.1/ocrd_froc/ocrd-tool.json
+-rw-rw-r--   0 kba       (1000) kba       (1000)     6990 2024-04-23 12:13:24.000000 ocrd_froc-0.6.1/ocrd_froc/processor.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/ocrd_froc.egg-info/
+-rw-r--r--   0 kba       (1000) kba       (1000)     2745 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)      471 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       67 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/entry_points.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       65 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       10 2024-04-23 12:23:08.000000 ocrd_froc-0.6.1/ocrd_froc.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2024-04-23 12:23:08.718102 ocrd_froc-0.6.1/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      927 2024-04-11 12:06:35.000000 ocrd_froc-0.6.1/setup.py
```

### Comparing `ocrd_froc-0.5.2/PKG-INFO` & `ocrd_froc-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ocrd_froc
-Version: 0.5.2
+Version: 0.6.1
 Summary: font recognition and OCR
 Home-page: https://github.com/MegaloPat/ocrd_froc
 Author: Guillaume Carriere, Matthias Seuret, Konstantin Baierer
 Author-email: 
 License: Apache License 2.0
 Description-Content-Type: text/markdown
-Requires-Dist: ocrd>=2.22.3
+Requires-Dist: ocrd>=2.64.1
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: torch>=1.4.0
 Requires-Dist: torchvision>=0.5.0
 
 # ocrd_froc
 
@@ -84,17 +84,17 @@
    "replace_textstyle" [bool - true]
     Whether to replace existing textStyle
    "network" [string]
     The file name of the neural network to use, including sufficient path
     information. Defaults to the model bundled with ocrd_froc.
    "fast_cocr" [boolean - true]
     Whether to use optimization steps on the COCR strategy
-   "adaptive_treshold" [number - 95]
-    Treshold of certitude needed to use SelOCR when using the adaptive
+   "adaptive_threshold" [number - 95]
+    Threshold of certitude needed to use SelOCR when using the adaptive
     strategy
    "font_class_priors" [array - []]
     List of font classes which are known to be present on the data when
-    using the adaptive/SelOCR strategies. When this option is specified,
-    every font classes not included will be ignored. If 'other' is
-    included in the list, font classification will not be outputted and
-    a generic model will be used for transcriptions.
+    using the adaptive/SelOCR strategies. If this option is specified,
+    any font classes not included are ignored. If 'other' is
+    included in the list, no font classification is output and
+    a generic model is used for transcriptions.
 ```
```

### Comparing `ocrd_froc-0.5.2/README.md` & `ocrd_froc-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -69,17 +69,17 @@
    "replace_textstyle" [bool - true]
     Whether to replace existing textStyle
    "network" [string]
     The file name of the neural network to use, including sufficient path
     information. Defaults to the model bundled with ocrd_froc.
    "fast_cocr" [boolean - true]
     Whether to use optimization steps on the COCR strategy
-   "adaptive_treshold" [number - 95]
-    Treshold of certitude needed to use SelOCR when using the adaptive
+   "adaptive_threshold" [number - 95]
+    Threshold of certitude needed to use SelOCR when using the adaptive
     strategy
    "font_class_priors" [array - []]
     List of font classes which are known to be present on the data when
-    using the adaptive/SelOCR strategies. When this option is specified,
-    every font classes not included will be ignored. If 'other' is
-    included in the list, font classification will not be outputted and
-    a generic model will be used for transcriptions.
+    using the adaptive/SelOCR strategies. If this option is specified,
+    any font classes not included are ignored. If 'other' is
+    included in the list, no font classification is output and
+    a generic model is used for transcriptions.
 ```
```

### Comparing `ocrd_froc-0.5.2/ocrd_froc/charmap.json` & `ocrd_froc-0.6.1/ocrd_froc/charmap.json`

 * *Files identical despite different names*

### Comparing `ocrd_froc-0.5.2/ocrd_froc/classmap.py` & `ocrd_froc-0.6.1/ocrd_froc/classmap.py`

 * *Files identical despite different names*

### Comparing `ocrd_froc-0.5.2/ocrd_froc/converter.py` & `ocrd_froc-0.6.1/ocrd_froc/converter.py`

 * *Files identical despite different names*

### Comparing `ocrd_froc-0.5.2/ocrd_froc/froc.py` & `ocrd_froc-0.6.1/ocrd_froc/froc.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def save(self, output):
         """ Stores the instance to a file
 
             Parameters
             ----------
                 output: string or file
-                    File or path to the file to which the instane has to
+                    File or path to the file to which the instance has to
                     be stored.
         """
 
         if isinstance(output, str):
             with open(output, 'wb') as f:
                 self.save(f)
                 return
@@ -104,27 +104,27 @@
         # machines which do not have CUDA available.
         self.selocr.to("cpu")
         self.cocr.to("cpu")
         pickle.dump(self, output)
         self.selocr.to(self.dev)
         self.cocr.to(self.dev)
 
-    def run(self, pil_image, method='adaptive', fast_cocr=True, adaptive_treshold=95, classification_result=None):
+    def run(self, pil_image, method='adaptive', fast_cocr=True, adaptive_threshold=95, classification_result=None):
 
         if method in ('SelOCR', 'adaptive') and not classification_result:
             raise ValueError(f"Froc.run(): if method is SelOCR or adaptive, classification_result is required")
 
         tns = self.preprocess_image(pil_image)
 
         if method == 'SelOCR':
             out = self.run_selocr(tns, classification_result)
         elif method == 'COCR':
             out = self.run_cocr(tns, fast_cocr)
         else:
-            out = self.run_adaptive(tns, classification_result, fast_cocr, adaptive_treshold)
+            out = self.run_adaptive(tns, classification_result, fast_cocr, adaptive_threshold)
 
         # constrain to image width, expand to batch format (batch size 1)
         base_width = [tns.shape[2]]
 
         out = torch.softmax(out, 2)
         scores, res = torch.max(out[:, :, :], 2)
 
@@ -196,12 +196,12 @@
 
             out = self.cocr(tns, fast_cocr)
             out = out.transpose(0,1)
 
             return out
 
 
-    def run_adaptive(self, tns, classification_result, fast_cocr, adaptive_treshold):
-        if max(classification_result.values()) > adaptive_treshold / 100:
+    def run_adaptive(self, tns, classification_result, fast_cocr, adaptive_threshold):
+        if max(classification_result.values()) > adaptive_threshold / 100:
             return self.run_selocr(tns, classification_result)
         else:
             return self.run_cocr(tns, fast_cocr)
```

### Comparing `ocrd_froc-0.5.2/ocrd_froc/network.py` & `ocrd_froc-0.6.1/ocrd_froc/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         :return: long tensor containing the converted widths
         """
         return torch.Tensor([min(self.__length_map[x], max_width) for x in w]).long()
 
     def __init_length_map(self):
         """
         Initializes the map conversion system for convert_width(). Note
-        that it tries to cache the resuts in dat/length_map.json.
+        that it tries to cache the results in dat/length_map.json.
         """
         max_length = 2000
         try:
             with open(join('dat', 'length_map.json'), 'rt', encoding='utf-8') as f:
                 self.__length_map = json.load(f)
                 return
         except:
@@ -268,15 +268,15 @@
             json.dump(self.__length_map, f)
 
     def forward(self, x):
         """
         Processes an input batch.
 
         :param x: input batch
-        :return: the network's output, ready to be convered to a string
+        :return: the network's output, ready to be converted to a string
         """
         x = self.backbone(x)
         x = self.act(x)
         x = torch.mean(x, axis=2)
         x = x.permute(2, 0, 1)
         x = self.embed(x)
         x, _ = self.rnn(x)
@@ -396,15 +396,15 @@
 
     def forward(self, x, model_idx=None):
         """
         Processes an input batch - batch which must contain only one
         single text line (because of the branching).
 
         :param x: input batch
-        :return: the network's output, ready to be convered to a string
+        :return: the network's output, ready to be converted to a string
         """
         if x.shape[0] != 1:
             raise ValueError('SelOCR cannot work on batches containing multiple inputs, sorry')
         if model_idx == None:
             scores = self.classifier(x).sum(axis=1)#.view(-1,13).mean(axis=1)
             n = torch.argmax(scores[0,:]).item()
             model_idx = n
@@ -536,15 +536,15 @@
             torch.save(optimizers[i+1].state_dict(), join(folder, '%d' % n, 'optimizer.pth'))
 
     def forward(self, x, fast_cocr=True):
         """
         Processes an input batch
 
         :param x: input batch
-        :return: the network's output, ready to be convered to a string
+        :return: the network's output, ready to be converted to a string
         """
         scores = F.softmax(self.classifier(x), dim=2)
         res = 0
         for n in self.models:
             s = scores[:, :, n].unsqueeze(-1)
             if fast_cocr and torch.max(s) < 0.1:
                 continue
@@ -700,15 +700,15 @@
             torch.save(optimizers[i+1].state_dict(), join(folder, '%d' % n, 'optimizer.pth'))
 
     def forward(self, x):
         """
         Processes an input batch
 
         :param x: input batch
-        :return: the network's output, ready to be convered to a string
+        :return: the network's output, ready to be converted to a string
         """
         scores = F.softmax(self.classifier(x), dim=2)
         txt = 0
         for n in self.models:
             s = scores[:, :, n].unsqueeze(-1)
             y = self.models[n](x)
             txt += y * s
```

### Comparing `ocrd_froc-0.5.2/ocrd_froc/ocrd-tool.json` & `ocrd_froc-0.6.1/ocrd_froc/ocrd-tool.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8289705086580087%*

 * *Differences: {"'tools'": "{'ocrd-froc-recognize': {'parameters': {'font_class_priors': {'description': "*

 * *            '"List of font classes which are known to be present on the data when using the '*

 * *            'adaptive/SelOCR strategies. If this option is specified, any font classes not '*

 * *            "included are ignored. If 'other' is included in the list, no font classification is "*

 * *            'output and a generic model is used for transcriptions."}, \'overwrite_style\': '*

 * *            "OrderedDict([('description' […]*

```diff
@@ -10,28 +10,28 @@
             "input_file_grp": [
                 "OCR-D-SEG"
             ],
             "output_file_grp": [
                 "OCR-D-OCR"
             ],
             "parameters": {
-                "adaptive_treshold": {
+                "adaptive_threshold": {
                     "default": 95,
-                    "description": "Treshold of certitude needed to use SelOCR when using the adaptive strategy",
+                    "description": "Threshold of certitude needed to use SelOCR when using the adaptive strategy",
                     "format": "integer",
                     "type": "number"
                 },
                 "fast_cocr": {
                     "default": true,
                     "description": "Whether to use optimization steps on the COCR strategy",
                     "type": "boolean"
                 },
                 "font_class_priors": {
                     "default": [],
-                    "description": "List of font classes which are known to be present on the data when using the adaptive/SelOCR strategies. When this option is specified, every font classes not included will be ignored. If 'other' is included in the list, font classification will not be outputted and a generic model will be used for transcriptions.",
+                    "description": "List of font classes which are known to be present on the data when using the adaptive/SelOCR strategies. If this option is specified, any font classes not included are ignored. If 'other' is included in the list, no font classification is output and a generic model is used for transcriptions.",
                     "items": {
                         "enum": [
                             "antiqua",
                             "bastarda",
                             "fraktur",
                             "textura",
                             "schwabacher",
@@ -43,15 +43,22 @@
                             "rotunda",
                             "other"
                         ],
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "network": {
+                "min_score_style": {
+                    "default": 0,
+                    "description": "The minimum score of a font classification to be serialized/used as input for OCR",
+                    "format": "float",
+                    "required": false,
+                    "type": "number"
+                },
+                "model": {
                     "description": "The file name of the neural network to use, including sufficient path information. Defaults to the model bundled with ocrd_froc.",
                     "required": false,
                     "type": "string"
                 },
                 "ocr_method": {
                     "default": "none",
                     "description": "The method to use for text recognition",
@@ -59,22 +66,28 @@
                         "none",
                         "SelOCR",
                         "COCR",
                         "adaptive"
                     ],
                     "type": "string"
                 },
-                "replace_textstyle": {
+                "overwrite_style": {
                     "default": true,
-                    "description": "Whether to replace existing textStyle",
+                    "description": "Whether to overwrite existing TextStyle/@fontFamily attributes",
+                    "required": false,
+                    "type": "boolean"
+                },
+                "overwrite_text": {
+                    "default": false,
+                    "description": "Whether to remove any existing TextEquiv before adding text",
                     "required": false,
                     "type": "boolean"
                 }
             },
             "steps": [
                 "recognition/font-identification",
                 "recognition/text-recognition"
             ]
         }
     },
-    "version": "0.5.2"
+    "version": "0.6.1"
 }
```

### Comparing `ocrd_froc-0.5.2/ocrd_froc/processor.py` & `ocrd_froc-0.6.1/ocrd_froc/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Wrap FROC as an ocrd.Processor
 """
 import os
+from typing import List, Tuple
 
 from ocrd import Processor
 from ocrd_utils import (
     getLogger,
     make_file_id,
     assert_file_grp_cardinality,
     MIMETYPE_PAGE
@@ -17,51 +18,43 @@
     TextEquivType,
 )
 from json import loads
 from ocrd_utils import resource_filename, resource_string
 from ocrd_modelfactory import page_from_file
 from .froc import Froc
 
-OCRD_TOOL = loads(resource_string(__name__, 'ocrd-tool.json'))
+OCRD_TOOL = loads(resource_string(__package__, 'ocrd-tool.json'))
 
 class FROCProcessor(Processor):
 
     def __init__(self, *args, **kwargs):
         kwargs['ocrd_tool'] = OCRD_TOOL['tools']['ocrd-froc-recognize']
         kwargs['version'] = OCRD_TOOL['version']
         super().__init__(*args, **kwargs)
         if hasattr(self, 'output_file_grp'):
             # processing context
             self.setup()
 
     def setup(self):
 
-        if 'network' not in self.parameter:
-            self.parameter['network'] = str(resource_filename(f'ocrd_froc.models', 'default.froc'))
+        if 'model' not in self.parameter:
+            self.parameter['model'] = str(resource_filename(f'ocrd_froc.models', 'default.froc'))
 
-        network_file = self.resolve_resource(self.parameter['network'])
-        self.froc = Froc.load(network_file)
+        model = self.resolve_resource(self.parameter['model'])
+        self.froc = Froc.load(model)
 
     def _process_segment(self, segment, image):
-        textStyle = segment.get_TextStyle()
-        if textStyle and self.parameter['replace_textstyle']:
-            textStyle = None
-            segment.set_TextStyle(textStyle)
-        if not textStyle:
-            textStyle = TextStyleType()
-            segment.set_TextStyle(textStyle)
-
         ocr_method = self.parameter['ocr_method']
 
         result = {}
 
         if ocr_method != 'COCR':
 
             result = self.froc.classify(image)
-            classification_result = ''
+            fonts_detected : List[Tuple[str, float]] = []
 
             font_class_priors = self.parameter['font_class_priors']
             output_font = True
 
             if font_class_priors:
                 if 'other' in font_class_priors:
                     for typegroup in self.froc.classMap.cl2id:
@@ -83,40 +76,53 @@
                             result[typegroup] /= result_sum
 
             for typegroup in self.froc.classMap.cl2id:
                 score = result[typegroup]
                 score = round(100 * score)
                 if score <= 0:
                     continue
-                if classification_result != '':
-                    classification_result += ', '
-                classification_result += '%s:%d' % (typegroup, score)
+                fonts_detected.append((typegroup, score))
+
+            classification_result = ', '.join([
+                f'{family}:{score}' \
+                for family, score in fonts_detected \
+                if score > self.parameter['min_score_style']
+            ])
 
             if output_font:
-                textStyle.set_fontFamily(classification_result)
+                textStyle = segment.get_TextStyle()
+                if not textStyle or self.parameter['overwrite_style']:
+                    if not textStyle:
+                        textStyle = TextStyleType()
+                        segment.set_TextStyle(textStyle)
+                    textStyle.set_fontFamily(classification_result)
 
 
         if ocr_method == 'COCR':
             fast_cocr = self.parameter['fast_cocr']
             transcription, score = self.froc.run(image,
                                           method=ocr_method,
                                           fast_cocr=fast_cocr)
         elif ocr_method == 'SelOCR':
             transcription, score = self.froc.run(image,
                                           method=ocr_method,
                                           classification_result=result)
         else:
             fast_cocr = self.parameter['fast_cocr']
-            adaptive_treshold = self.parameter['adaptive_treshold']
+            adaptive_threshold = self.parameter['adaptive_threshold']
             transcription, score = self.froc.run(image,
                                           method=ocr_method,
                                           classification_result=result,
                                           fast_cocr=fast_cocr,
-                                          adaptive_treshold=adaptive_treshold)
-        segment.set_TextEquiv([TextEquivType(Unicode=transcription, conf=score)])
+                                          adaptive_treshold=adaptive_threshold)
+
+        if self.parameter['overwrite_text']:
+            segment.set_TextEquiv([TextEquivType(Unicode=transcription, conf=score)])
+        else:
+            segment.add_TextEquiv(TextEquivType(Unicode=transcription, conf=score))
 
 
     def process(self):  # type: ignore
         """Perform font classification and text recognition (in one step) on historic documents.
 
         Open and deserialize PAGE input files and their respective images,
         iterating over the element hierarchy down to the text line level.
```

### Comparing `ocrd_froc-0.5.2/ocrd_froc.egg-info/PKG-INFO` & `ocrd_froc-0.6.1/ocrd_froc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ocrd_froc
-Version: 0.5.2
+Version: 0.6.1
 Summary: font recognition and OCR
 Home-page: https://github.com/MegaloPat/ocrd_froc
 Author: Guillaume Carriere, Matthias Seuret, Konstantin Baierer
 Author-email: 
 License: Apache License 2.0
 Description-Content-Type: text/markdown
-Requires-Dist: ocrd>=2.22.3
+Requires-Dist: ocrd>=2.64.1
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: torch>=1.4.0
 Requires-Dist: torchvision>=0.5.0
 
 # ocrd_froc
 
@@ -84,17 +84,17 @@
    "replace_textstyle" [bool - true]
     Whether to replace existing textStyle
    "network" [string]
     The file name of the neural network to use, including sufficient path
     information. Defaults to the model bundled with ocrd_froc.
    "fast_cocr" [boolean - true]
     Whether to use optimization steps on the COCR strategy
-   "adaptive_treshold" [number - 95]
-    Treshold of certitude needed to use SelOCR when using the adaptive
+   "adaptive_threshold" [number - 95]
+    Threshold of certitude needed to use SelOCR when using the adaptive
     strategy
    "font_class_priors" [array - []]
     List of font classes which are known to be present on the data when
-    using the adaptive/SelOCR strategies. When this option is specified,
-    every font classes not included will be ignored. If 'other' is
-    included in the list, font classification will not be outputted and
-    a generic model will be used for transcriptions.
+    using the adaptive/SelOCR strategies. If this option is specified,
+    any font classes not included are ignored. If 'other' is
+    included in the list, no font classification is output and
+    a generic model is used for transcriptions.
 ```
```

### Comparing `ocrd_froc-0.5.2/setup.py` & `ocrd_froc-0.6.1/setup.py`

 * *Files identical despite different names*

