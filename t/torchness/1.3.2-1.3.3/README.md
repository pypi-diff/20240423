# Comparing `tmp/torchness-1.3.2.tar.gz` & `tmp/torchness-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchness-1.3.2.tar", last modified: Sat Apr  6 18:51:43 2024, max compression
+gzip compressed data, was "torchness-1.3.3.tar", last modified: Tue Apr 23 11:25:43 2024, max compression
```

## Comparing `torchness-1.3.2.tar` & `torchness-1.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-06 18:51:43.329340 torchness-1.3.2/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      308 2024-04-06 18:17:30.000000 torchness-1.3.2/README.md
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-06 18:51:43.329340 torchness-1.3.2/setup.cfg
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      493 2024-04-06 18:51:41.000000 torchness-1.3.2/setup.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.325340 torchness-1.3.2/tests/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3608 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_base_elements.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3917 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_devices.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)    16816 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_encoders.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     1852 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_grad_clipping.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2355 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_layers.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)    19732 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_motorch.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      715 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_tbwr.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.325340 torchness-1.3.2/torchness/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     4726 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/base_elements.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness/comoneural/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      501 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/avg_probs.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6458 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/batcher.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2761 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/zeroes_processor.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     7157 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/devices.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)    27977 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/encoders.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3140 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/grad_clipping.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     7236 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/layers.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness/models/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3173 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/simple_feats_classifier.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     4372 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/simple_text_classifier.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2825 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/text_embbeder.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)    41563 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/motorch.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2194 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/scaled_LR.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2090 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/tbwr.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      502 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/types.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness.egg-info/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      855 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/SOURCES.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/dependency_links.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       84 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/requires.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       10 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/top_level.txt
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.982609 torchness-1.3.3/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-23 11:25:43.982609 torchness-1.3.3/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      308 2024-04-06 18:17:30.000000 torchness-1.3.3/README.md
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-23 11:25:43.982609 torchness-1.3.3/setup.cfg
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      493 2024-04-23 11:25:41.000000 torchness-1.3.3/setup.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.978609 torchness-1.3.3/tests/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3608 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_base_elements.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4647 2024-04-23 11:20:22.000000 torchness-1.3.3/tests/test_devices.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    16816 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_encoders.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1852 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_grad_clipping.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2355 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_layers.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    19732 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_motorch.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      715 2024-04-06 18:17:30.000000 torchness-1.3.3/tests/test_tbwr.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.978609 torchness-1.3.3/torchness/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4726 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/base_elements.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.978609 torchness-1.3.3/torchness/comoneural/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/comoneural/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      501 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/comoneural/avg_probs.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6458 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/comoneural/batcher.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2761 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/comoneural/zeroes_processor.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     7951 2024-04-23 11:23:12.000000 torchness-1.3.3/torchness/devices.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    27977 2024-04-10 17:10:57.000000 torchness-1.3.3/torchness/encoders.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3140 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/grad_clipping.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     7236 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/layers.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.982609 torchness-1.3.3/torchness/models/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/models/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3173 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/models/simple_feats_classifier.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4372 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/models/simple_text_classifier.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2825 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/models/text_embbeder.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    41563 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/motorch.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2194 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/scaled_LR.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2090 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/tbwr.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      502 2024-04-06 18:17:30.000000 torchness-1.3.3/torchness/types.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:25:43.982609 torchness-1.3.3/torchness.egg-info/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-23 11:25:43.000000 torchness-1.3.3/torchness.egg-info/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      855 2024-04-23 11:25:43.000000 torchness-1.3.3/torchness.egg-info/SOURCES.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-23 11:25:43.000000 torchness-1.3.3/torchness.egg-info/dependency_links.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       84 2024-04-23 11:25:43.000000 torchness-1.3.3/torchness.egg-info/requires.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       10 2024-04-23 11:25:43.000000 torchness-1.3.3/torchness.egg-info/top_level.txt
```

### Comparing `torchness-1.3.2/tests/test_base_elements.py` & `torchness-1.3.3/tests/test_base_elements.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/tests/test_devices.py` & `torchness-1.3.3/tests/test_devices.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,122 +1,133 @@
 import unittest
 
 import torch
 
-from torchness.devices import get_cuda_mem, get_available_cuda_id, report_cuda, _get_devices_pypaq, get_devices, mask_cuda, mask_cuda_devices
+from torchness.devices import get_cuda_mem, get_available_cuda_id, report_cuda, _get_devices_torchness, get_devices, mask_cuda, mask_cuda_devices
 
 
 class TestDevices(unittest.TestCase):
 
     def test_get_cuda_mem(self):
         mem = get_cuda_mem()
         print(mem)
 
-
     def test_get_available_cuda_id(self):
-        av_cuda = get_available_cuda_id()
+        av_cuda = get_available_cuda_id(max_load=0.1, max_mem=0.2)
+        print(av_cuda)
+        av_cuda = get_available_cuda_id(max_load=0.5, max_mem=0.5)
+        print(av_cuda)
+        av_cuda = get_available_cuda_id(max_load=1.0, max_mem=1.0)
         print(av_cuda)
-
 
     def test_report_cuda(self):
         print(report_cuda())
 
+    def test_get_devices_torchness(self):
 
-    def test_get_devices_pypaq(self):
-
-        d = _get_devices_pypaq(0)
+        d = _get_devices_torchness(0)
         print(d)
         self.assertTrue(d == [0])
 
-        d = _get_devices_pypaq(1)
+        d = _get_devices_torchness(1)
         print(d)
         self.assertTrue(d == [1])
 
-        d = _get_devices_pypaq(13)
+        d = _get_devices_torchness(13)
         print(d)
         self.assertTrue(d == [13])
 
-        d = _get_devices_pypaq(-1)
+        d = _get_devices_torchness(-1)
         print(d)
         self.assertTrue(type(d) is list and (not d or len(d) == 1 and ((type(d[0]) is int and d[0] >= 0) or d[0] is None)))
 
-        d = _get_devices_pypaq([])
+        d = _get_devices_torchness([])
         print(d)
         self.assertTrue(d == [] or list(set([type(e) for e in d]))[0] in [int, None])
 
-        d = _get_devices_pypaq(None)
+        d = _get_devices_torchness(None)
         print(d)
         self.assertTrue(d == [None])
 
-        d = _get_devices_pypaq(0.7)
+        d = _get_devices_torchness(0.7)
         print(len(d), d)
         self.assertTrue(type(d) is list and len(d)>=1 and d[0] is None)
 
-        d = _get_devices_pypaq(-0.5)
+        d = _get_devices_torchness(-0.5)
         print(d)
         self.assertTrue(d == [None])
 
-        d = _get_devices_pypaq('all')
+        d = _get_devices_torchness('all')
         print(len(d), d)
         self.assertTrue(type(d) is list and len(d) >= 1 and d[0] is None)
 
-        d = _get_devices_pypaq('cuda')
+        d = _get_devices_torchness('cuda')
         print(d)
         self.assertTrue(d == [0])
 
-        d = _get_devices_pypaq('cuda:0')
+        d = _get_devices_torchness('cuda:0')
         print(d)
         self.assertTrue(d == [0])
 
-        d = _get_devices_pypaq('cuda:1')
+        d = _get_devices_torchness('cuda:1')
         print(d)
         self.assertTrue(d == [1])
 
         d = torch.device('cpu')
-        d = _get_devices_pypaq(d)
+        d = _get_devices_torchness(d)
         print(d)
         self.assertTrue(d == [None])
 
         d = torch.device('cuda')
-        d = _get_devices_pypaq(d)
+        d = _get_devices_torchness(d)
         print(d)
         self.assertTrue(d == [0])
 
         d = torch.device('cuda:1')
-        d = _get_devices_pypaq(d)
+        d = _get_devices_torchness(d)
         print(d)
         self.assertTrue(d == [1])
 
         d = torch.device('cuda:8')
-        d = _get_devices_pypaq(d)
+        d = _get_devices_torchness(d)
         print(d)
         self.assertTrue(d == [8])
 
-        d = _get_devices_pypaq([0, 'all'])
+        d = _get_devices_torchness([0, 'all'])
         print(d)
         self.assertTrue(None in d and 0 in d and len(d)>1)
 
-        d = _get_devices_pypaq([0, [], None])
+        d = _get_devices_torchness([0, [], None])
         print(len(d), d)
         self.assertTrue(None in d and 0 in d and len(d)>1)
 
-        d = _get_devices_pypaq([0, 2, [], None, -1])
+        d = _get_devices_torchness([0, 2, [], None, -1])
         print(len(d), d)
         self.assertTrue(None in d and 0 in d and -1 not in d and len(d)>1)
 
-        d = _get_devices_pypaq([1, 2, [], None, -1, 'all', 'cuda:0'])
+        d = _get_devices_torchness([1, 2, [], None, -1, 'all', 'cuda:0'])
         print(len(d), d)
         self.assertTrue(None in d and 0 in d and -1 not in d and len(d)>3)
 
+    def test_get_devices(self):
+        devices = get_devices(eventually_cpu=True)
+        print(devices)
+        devices = get_devices(max_load=1.0, max_mem=1.0)
+        print(devices)
+        devices = get_devices(devices=[0,1], max_load=1.0, max_mem=1.0)
+        print(devices)
+        devices = get_devices(devices=[], max_load=1.0, max_mem=1.0)
+        print(devices)
+        devices = get_devices(devices=[0,1])
+        print(devices)
 
     def test_get_devices_exceptions(self):
         self.assertRaises(Exception, get_devices, 'alll') # wrong device
         self.assertRaises(Exception, get_devices, (0,1))  # wrong device
 
-
     def test_get_devices_torch(self):
 
         d = get_devices(0)
         print(d)
         self.assertTrue(d == [] or 'cuda' in d[0])
 
         d = get_devices(-1)
```

### Comparing `torchness-1.3.2/tests/test_encoders.py` & `torchness-1.3.3/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/tests/test_grad_clipping.py` & `torchness-1.3.3/tests/test_grad_clipping.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/tests/test_layers.py` & `torchness-1.3.3/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/tests/test_motorch.py` & `torchness-1.3.3/tests/test_motorch.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/tests/test_tbwr.py` & `torchness-1.3.3/tests/test_tbwr.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/base_elements.py` & `torchness-1.3.3/torchness/base_elements.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/comoneural/batcher.py` & `torchness-1.3.3/torchness/comoneural/batcher.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/comoneural/zeroes_processor.py` & `torchness-1.3.3/torchness/comoneural/zeroes_processor.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/devices.py` & `torchness-1.3.3/torchness/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,54 +39,63 @@
 DevicesTorchness: Union[int, None, float, str, torch.device, List[Union[int,None,float,str,torch.device]]] = -1
 
 
 
 def get_cuda_mem():
     """ returns cuda memory size (system first device) """
     devs = GPUtil.getGPUs()
-    if devs: return devs[0].memoryTotal
-    else: return 0
+    return devs[0].memoryTotal if devs else 0
 
 
-def get_available_cuda_id(max_mem=None) -> List[int]: # None sets automatic, otherwise (0,1.1] (above 1 for all)
-    """ returns list of available GPUs ids """
-    if not max_mem:
-        tot_mem = get_cuda_mem()
-        if tot_mem < 5000:  max_mem=0.35 # small GPU case, probably system single GPU
-        else:               max_mem=0.2
-    return GPUtil.getAvailable(limit=20, maxMemory=max_mem)
+def get_available_cuda_id(
+        max_load: float=            0.5,
+        max_mem: Optional[float]=   None,
+) -> List[int]:
+    """ returns list of available GPUs ids
+    max_load - <0.0 - 1.0> factor of GPU utilization
+              to still consider GPU as an available one,
+    max_mem - <0.0 - 1.0> factor of GPU memory that may be used (occupied already)
+              to still consider GPU as an available one,
+              for None sets auto """
+    if max_mem is None:
+        # small GPU (<5000) may be used by the system significantly, but still available
+        max_mem = 0.35 if get_cuda_mem() < 5000 else 0.2
+    return GPUtil.getAvailable(limit=20, maxLoad=max_load, maxMemory=max_mem)
 
 
 def report_cuda() -> str:
     """ prints report of system cuda devices """
     rp = 'System CUDA devices:'
     for device in GPUtil.getGPUs():
         rp += f'\n > id: {device.id}, name: {device.name}, MEM: {int(device.memoryUsed)}/{int(device.memoryTotal)} (U/T)'
     return rp
 
 
 def _get_devices_torchness(
         devices: DevicesTorchness=  -1,
-        logger=                 None,
-        loglevel=               20,
+        max_load: float=            0.5,
+        max_mem: Optional[float]=   None,
+        logger=                     None,
+        loglevel=                   20,
 ) -> List[Union[int,None]]:
-    """ returns torchness representation of given devices """
+    """ returns torchness representation of given devices
+    max_load and max_mem are used only when requesting AVAILABLE CUDA (with -int or []) """
 
     if not logger:
         logger = get_pylogger(name='_get_devices_torchness', level=loglevel)
 
     if type(devices) is not list: devices = [devices]  # first convert to list
 
     cpu_count = sys_res_nfo()['cpu_count']
     logger.debug(f'got {cpu_count} CPU devices in a system')
 
     # try to get available CUDA
     available_cuda_id = []
     try:
-        available_cuda_id = get_available_cuda_id()
+        available_cuda_id = get_available_cuda_id(max_load=max_load, max_mem=max_mem)
     except Exception as e:
         logger.warning(f'could not get CUDA devices, got EXCEPTION: {e}')
 
     if devices == []:
         return available_cuda_id
 
     devices_base = []
@@ -141,45 +150,52 @@
             raise TorchnessException(msg)
 
     return devices_base
 
 
 def get_devices(
         devices: DevicesTorchness=  -1,
-        torch_namespace: bool=  True,
-        logger=                 None,
-        loglevel=               20,
+        max_load: float=            0.5,
+        max_mem: Optional[float]=   None,
+        eventually_cpu: bool=       False,
+        torch_namespace: bool=      True,
+        logger=                     None,
+        loglevel=                   20,
 ) -> List[Union[int,None,str]]:
-    """ resolves representation given with DevicesTorchness
-    into dev_torchness base form or List[str] (PyTorch namespace) """
+    """ resolves representation given with devices (DevicesTorchness)
+    max_load and max_mem are used only when requesting AVAILABLE CUDA (with -int or []) """
 
     if not logger:
         logger = get_pylogger(name='get_devices', level=loglevel)
 
-    devices_base = _get_devices_torchness(devices=devices, logger=logger)
-
-    if not torch_namespace:
-        return devices_base
-    else:
-        return [f'cuda:{dev}' if type(dev) is int else 'cpu' for dev in devices_base]
+    devices_base = _get_devices_torchness(
+        devices=    devices,
+        max_load=   max_load,
+        max_mem=    max_mem,
+        logger=     logger)
+
+    d = [f'cuda:{dev}' if type(dev) is int else 'cpu' for dev in devices_base] if torch_namespace else devices_base
+    if not d and eventually_cpu:
+        d = ['cpu']
+    return d
 
 
 def mask_cuda(ids: Optional[List[int] or int]=None):
     """ masks GPUs from given list of ids or single one """
     if ids is None: ids = []
     if type(ids) is int: ids = [ids]
     mask = ''
     for id in ids: mask += f'{int(id)},'
     if len(mask) > 1: mask = mask[:-1]
     os.environ["CUDA_VISIBLE_DEVICES"] = mask
 
 
 def mask_cuda_devices(
         devices: DevicesTorchness=  -1,
-        logger=                 None):
+        logger=                     None):
     """ wraps mask_cuda to hold DevicesTorchness """
     devices = get_devices(devices, torch_namespace=False, logger=logger)
     ids = [d for d in devices if type(d) is int]
     mask_cuda(ids)
 
 
 def monitor(pause:float=0.1, print_n:int=10):
```

### Comparing `torchness-1.3.2/torchness/encoders.py` & `torchness-1.3.3/torchness/encoders.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/grad_clipping.py` & `torchness-1.3.3/torchness/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/layers.py` & `torchness-1.3.3/torchness/layers.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/models/simple_feats_classifier.py` & `torchness-1.3.3/torchness/models/simple_feats_classifier.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/models/simple_text_classifier.py` & `torchness-1.3.3/torchness/models/simple_text_classifier.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/models/text_embbeder.py` & `torchness-1.3.3/torchness/models/text_embbeder.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/motorch.py` & `torchness-1.3.3/torchness/motorch.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/scaled_LR.py` & `torchness-1.3.3/torchness/scaled_LR.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness/tbwr.py` & `torchness-1.3.3/torchness/tbwr.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.2/torchness.egg-info/SOURCES.txt` & `torchness-1.3.3/torchness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

