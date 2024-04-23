# Comparing `tmp/torch_trandsforms-0.3.5.tar.gz` & `tmp/torch_trandsforms-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_trandsforms-0.3.5.tar", max compression
+gzip compressed data, was "torch_trandsforms-0.3.6.tar", max compression
```

## Comparing `torch_trandsforms-0.3.5.tar` & `torch_trandsforms-0.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1090 2023-11-01 13:01:21.612709 torch_trandsforms-0.3.5/LICENSE
--rw-r--r--   0        0        0     6786 2023-12-04 10:07:17.475509 torch_trandsforms-0.3.5/README.md
--rw-r--r--   0        0        0     3659 2023-12-14 12:27:11.869529 torch_trandsforms-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1123 2023-11-20 07:18:12.608614 torch_trandsforms-0.3.5/torch_trandsforms/__init__.py
--rw-r--r--   0        0        0    11667 2023-11-17 13:52:29.408965 torch_trandsforms-0.3.5/torch_trandsforms/_functional.py
--rw-r--r--   0        0        0     6562 2023-11-17 21:14:00.045759 torch_trandsforms-0.3.5/torch_trandsforms/_utils.py
--rw-r--r--   0        0        0     7467 2023-11-07 13:14:08.777679 torch_trandsforms-0.3.5/torch_trandsforms/base.py
--rw-r--r--   0        0        0     5431 2023-11-07 10:36:16.439166 torch_trandsforms-0.3.5/torch_trandsforms/ops.py
--rw-r--r--   0        0        0     4818 2023-11-17 21:18:20.310007 torch_trandsforms-0.3.5/torch_trandsforms/rotation.py
--rw-r--r--   0        0        0    10630 2023-12-01 09:45:33.248146 torch_trandsforms-0.3.5/torch_trandsforms/shape.py
--rw-r--r--   0        0        0     4662 2023-12-01 09:45:33.248146 torch_trandsforms-0.3.5/torch_trandsforms/structure.py
--rw-r--r--   0        0        0    13698 2023-12-14 12:21:20.730758 torch_trandsforms-0.3.5/torch_trandsforms/value.py
--rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 torch_trandsforms-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-11-01 13:01:21.612709 torch_trandsforms-0.3.6/LICENSE
+-rw-r--r--   0        0        0     7056 2024-04-11 11:00:47.704914 torch_trandsforms-0.3.6/README.md
+-rw-r--r--   0        0        0     3658 2024-04-11 11:25:13.924566 torch_trandsforms-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1163 2024-04-23 09:26:37.652687 torch_trandsforms-0.3.6/torch_trandsforms/__init__.py
+-rw-r--r--   0        0        0    11667 2023-11-17 13:52:29.408965 torch_trandsforms-0.3.6/torch_trandsforms/_functional.py
+-rw-r--r--   0        0        0     6562 2023-11-17 21:14:00.045759 torch_trandsforms-0.3.6/torch_trandsforms/_utils.py
+-rw-r--r--   0        0        0     7467 2023-11-07 13:14:08.777679 torch_trandsforms-0.3.6/torch_trandsforms/base.py
+-rw-r--r--   0        0        0     5431 2023-11-07 10:36:16.439166 torch_trandsforms-0.3.6/torch_trandsforms/ops.py
+-rw-r--r--   0        0        0     4818 2023-11-17 21:18:20.310007 torch_trandsforms-0.3.6/torch_trandsforms/rotation.py
+-rw-r--r--   0        0        0    12651 2024-04-09 07:57:18.744562 torch_trandsforms-0.3.6/torch_trandsforms/shape.py
+-rw-r--r--   0        0        0     4662 2023-12-01 09:45:33.248146 torch_trandsforms-0.3.6/torch_trandsforms/structure.py
+-rw-r--r--   0        0        0    13771 2024-04-09 07:57:18.744562 torch_trandsforms-0.3.6/torch_trandsforms/value.py
+-rw-r--r--   0        0        0     8124 1970-01-01 00:00:00.000000 torch_trandsforms-0.3.6/PKG-INFO
```

### Comparing `torch_trandsforms-0.3.5/LICENSE` & `torch_trandsforms-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/README.md` & `torch_trandsforms-0.3.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: torch-trandsforms
+Version: 0.3.6
+Summary: A pytorch-first transform library for ND data, such as multi-channel 3D volumes
+Home-page: https://github.com/alexandrainst/torch-trandsforms
+License: MIT
+Keywords: pytorch,transforms,torchvision,data
+Author: Oliver Hjermitslev
+Author-email: oliver.gyldenberg@alexandra.dk
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: torch (>=1.13.1)
+Requires-Dist: torchvision (>=0.14.0)
+Project-URL: Repository, https://github.com/alexandrainst/torch-trandsforms
+Description-Content-Type: text/markdown
+
 # torch traNDsforms
 
 <div align="center">
 
 [![build](https://github.com/alexandrainst/torch-trandsforms/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/alexandrainst/torch-trandsforms/actions/workflows/build.yml?query=branch%3Amain)
 [![Python Version](https://img.shields.io/pypi/pyversions/torch-trandsforms.svg)](https://pypi.org/project/torch-trandsforms/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/alexandrainst/torch-trandsforms/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
@@ -43,80 +68,68 @@
 
 ```bash
 conda install torch_trandsforms
 ```
 
 ## Usage
 
-Creating the RandomRotate90 class, as an example of customizing your own transform:
+Creating a single transform that rotates both input data and ground truth data. The data is considered 3D with a leading channel dimension.
+
+![RandomRotate](./examples/figures/RandomRotate.png)
 
 ```python
 import torch
-from torch_trandsforms.base import BaseTransform
+from torch_trandsforms import RandomRotate
 
-class RandomRotate90(BaseTransform):  # note the use of BaseTransform as base class here
-    """
-    Rotates the input 90 degrees around a randomly determined axis
-    NOTE: This is the not actual implementation of RandomRotate90
-    """
-    def __init__(self, nd=3, p=0.5):
-        super().__init__(p = p, nd = nd)
-        self.options = self._get_options(nd)
-
-    def _get_options(self, nd):
-        """
-        Create potential rotations based on the nd argument
-        This can be lower than the number of dimensions of the actual input
-            in case you do not want a leading dimension to be rotated
-        """
-        options = []
-
-        for i in range(nd):
-            for j in range(nd):
-                if not i == j:
-                    options.append((-i-1, -j-1))
-
-        return options
-    
-    def get_parameters(self, **inputs):
-        """
-        overrides the base get_parameters to choose a random
-            rotation option for each input
-        """
-        rotation = random.choice(self.options)
-        return {'rot':rotation}
-    
-    def apply(self, input, **params):
-        """
-        apply MUST be overwritten 
-        It is applied to each input sequentially, and thus must have
-            parameters that are exactly equal for each instance,
-            meaning most likely NO randomization here
-        """
-        rot = params['rot']
-        return torch.rot90(input, dims=rot)
-```
+# create data and target
+input_tensor = torch.rand((3,16,16,16), device="cuda", dtype=torch.float32)
+target_tensor = torch.rand((1,16,16,16), device="cuda", dtype=torch.float32)
 
-And we can now use our class to demonstrate the library functionality:
+# create our random rotator, which rotates dim -3 from -90 to 90, dim -2 from -90 to 90, and dim -1 from -180 to 180
+# this operates only on inputs with the keynames "input" or "target" and in the trailing 3 dimensions
+rotator = RandomRotate((90,90,180), nd=3, keys=["input", "target"], align_corners=True)
 
-```python
-torch.manual_seed(451)  # all randomization uses torch.random in the actual implementation
+# transform the data and target
+transformed = rotator(input=input_tensor, target=target_tensor)
 
-tensor = torch.arange(16).view(2,2,2,2)  # create a 4D tensor
-another_tensor = torch.arange(16).view(2,2,2,2)  # create an exactly equal tensor for demonstration
+# the data is recovered using the same keys as in the input
+data = transformed["input"]
+target = transformed["target"]
+```
 
-print(tensor)
-print(another_tensor)
+Create a Compose object to run a sequence of transforms one after another:
 
-random_rotator = RandomRotate90(nd=2, p=1.)  # we only want the last two dimensions to be rotateable but it should rotate every time (p=1)
+![ComposeExample](./examples/figures/Compose.png)
 
-transformed = random_rotator(data=tensor, foo=another_tensor)  # "data" is arbitrary, it is the key that will be returned, demonstrated by "foo"
+```python
+import torch
+from torch_trandsforms import Compose, RandomResize, RandomRotate, RandomCrop, RandomApply, UniformNoise, GaussianNoise, SaltAndPepperNoise
 
-print(transformed['data'])
-print(transformed['foo'])
+# create data and target
+input_tensor = torch.rand((3,16,16,16), device="cuda", dtype=torch.float32)
+target_tensor = torch.rand((16,16,16), device="cuda").round()
+
+# create our transform pipeline using some shape/size augmentation on both input and target, as well as some noise on the input
+transform = Compose([
+    RandomResize(0.3, p=0.75, keys="*"),  # keys="*" is the same as keys=["foo", "bar"] here
+    RandomRotate([180,180,180], sample_mode="nearest", p=0.9, nd=3, keys=["foo", "bar"]),
+    RandomCrop(16, padding=0, p=1.0, keys="*"),  # nd is 3 by default - but nd=1,2,3 all work here, just on the trailing dimensions
+    RandomApply([
+        UniformNoise(p=1.0, low=-0.2, hi=0.2, keys=["foo"]),  # for most noise transforms, we only want the data to be augmented
+        GaussianNoise(mean=torch.tensor(0.0, device="cuda"), std=0.05, p=1.0, keys=["foo"]),
+        SaltAndPepperNoise(0.2, low=0.0, hi=1.0, a=torch.tensor(0.5, device="cuda"), p=1.0, copy_input=True, keys=["foo"])
+    ], min=1, max=1)  # apply exactly 1 of the above three transforms each time
+])
+
+# transform the data and target
+transformed = transform(foo=input_tensor, bar=target_tensor)
+
+# the data is recovered using the same keys as in the input
+data = transformed["foo"]
+target = transformed["bar"]
 ```
 
 For more examples of use, see [EXAMPLES.md](https://github.com/alexandrainst/torch-trandsforms/blob/main/examples/EXAMPLES.md)
 
 ## Speed
 
 Please see [TIMING.md](https://github.com/alexandrainst/torch-trandsforms/blob/main/TIMING.md) for timings. See [test_speed.py](https://github.com/alexandrainst/torch-trandsforms/blob/main/test_speed.py) for methodology.
@@ -142,14 +155,15 @@
 
 Later additions (and reasons for postponing):
  - [ ] Arbitrary rotations (missing ND affine_grid and grid_sample)
  - [ ] Gaussian Blur (missing implementation of ND convolution)
  - [ ] Affine transformations (missing efficient ND computation)
 
 Potential additions:
+ - [ ] ND Bounding Boxes
  - [ ] Geometric operations using PyTorch Geometric
  - [ ] Point clouds, meshes using PyTorch 3D
  - [ ] Data loading, sampling, and structures
  - [ ] torchscript compatibility
 
 ## Contributing
 
@@ -175,7 +189,8 @@
   title = {A pytorch-first transform library for ND data, such as multi-channel 3D volumes},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/alexandrainst/torch-trandsforms}}
 }
 ```
+
```

### Comparing `torch_trandsforms-0.3.5/pyproject.toml` & `torch_trandsforms-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "torch-trandsforms"
-version = "0.3.5"
+version = "0.3.6"
 description = "A pytorch-first transform library for ND data, such as multi-channel 3D volumes"
 readme = "README.md"
 authors = ["Oliver Hjermitslev <oliver.gyldenberg@alexandra.dk>"]
 license = "MIT"
 repository = "https://github.com/alexandrainst/torch-trandsforms"
 homepage = "https://github.com/alexandrainst/torch-trandsforms"
 
@@ -35,15 +35,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = ">= 1.13.1"
 torchvision = ">= 0.14.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
-black = {version = "^22.10", allow-prereleases = true}
+black = {version = "^24.3", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^1.0"
 mypy-extensions = "^1.0.0"
 pre-commit = "^3.5.0"
 pydocstyle = "^6.1.1"
 pylint = "^3.0.2"
```

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/__init__.py` & `torch_trandsforms-0.3.6/torch_trandsforms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A pytorch-first transform library for ND data, such as multi-channel 3D volumes"""
 
 import sys
 from importlib import metadata as importlib_metadata
 
 from .ops import Cast, ConvertDtype, To, ToDevice
 from .rotation import RandomRotate, RandomRotate90
-from .shape import CenterCrop, RandomCrop, RandomFlip, RandomResize, Resize
+from .shape import CenterCrop, RandomCrop, RandomFlip, RandomPadding, RandomResize, Resize
 from .structure import Compose, RandomApply
 from .value import AdditiveBetaNoise, GaussianNoise, Normalize, SaltAndPepperNoise, UniformNoise
 
 __all__ = sorted(
     [
         "RandomRotate90",
         "Compose",
@@ -25,14 +25,15 @@
         "GaussianNoise",
         "CenterCrop",
         "RandomCrop",
         "RandomFlip",
         "RandomRotate",
         "Resize",
         "RandomResize",
+        "RandomPadding",
     ]
 )
 
 
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
```

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/_functional.py` & `torch_trandsforms-0.3.6/torch_trandsforms/_functional.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/_utils.py` & `torch_trandsforms-0.3.6/torch_trandsforms/_utils.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/base.py` & `torch_trandsforms-0.3.6/torch_trandsforms/base.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/ops.py` & `torch_trandsforms-0.3.6/torch_trandsforms/ops.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/rotation.py` & `torch_trandsforms-0.3.6/torch_trandsforms/rotation.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/shape.py` & `torch_trandsforms-0.3.6/torch_trandsforms/shape.py`

 * *Files 13% similar despite different names*

```diff
@@ -225,7 +225,45 @@
                 input, size=params["size"], scale_factor=None, mode=self.interpolation_mode, align_corners=self.align_corners
             )
             return scaled.view(*sh[: -self.nd], *scaled.shape[-self.nd :])
         scaled = F_t.interpolate(
             input, size=None, scale_factor=params["scale_factor"], mode=self.interpolation_mode, align_corners=self.align_corners
         )
         return scaled.view(*sh[: -self.nd], *scaled.shape[-self.nd :])
+
+
+class RandomPadding(KeyedNdTransform):
+    """
+    Introduces random edge padding for the trailing `nd` dimensions.
+    Each side is padded individually from `min_pad` to `max_pad`
+
+    Args:
+        min_pad (int): Minimum padding for each side
+        max_pad (int): Maximum padding (inclusive) for each side
+        value (float, str, or torch.tensor): If number, does constant fill with the value. If str, attempts to use https://pytorch.org/docs/stable/generated/torch.nn.functional.pad.html padding modes (implemented for <=3 dimensions of padding)
+            If torch.tensor, fills the new padded area with the given value(s).
+            This works in ND, i.e. padding in 3 dimensions with a 0, 1, or 2D value works for a 5D input.
+            However, for ND tensors the input must be directly broadcastable to the leading N dimensions of the input (i.e. dimensions must be 1 or equal to input dimension)
+            Most of the time, a 0D-value is equivalent (but slower) to a scalar value (so choose `0.0` over torch.tensor(0.0))
+    """
+
+    def __init__(self, min_pad=0, max_pad=3, pad_val=0.0, p=0.5, nd=3, keys="*"):
+        super().__init__(p, nd, keys)
+
+        assert (
+            isinstance(min_pad, int) and min_pad >= 0
+        ), f"min_pad must be a positive or 0 integer, found {min_pad} with dtype {type(min_pad)}"
+        assert (
+            isinstance(max_pad, int) and max_pad >= 0
+        ), f"max_pad must be a positive or 0 integer, found {max_pad} with dtype {type(max_pad)}"
+        assert max_pad >= min_pad, f"max_pad must be greater than or equal to min_pad, found max_pad = {max_pad} and min_pad = {min_pad}"
+
+        self.min_pad = min_pad
+        self.max_pad = max_pad
+        self.pad_val = pad_val
+
+    def get_parameters(self, **inputs):
+        return {"padding": tuple(torch.randint(self.min_pad, self.max_pad + 1, (2 * self.nd,)).numpy())}
+
+    def apply(self, input, **params):
+        padding = params["padding"]
+        return F.pad(input, padding, value=self.pad_val)
```

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/structure.py` & `torch_trandsforms-0.3.6/torch_trandsforms/structure.py`

 * *Files identical despite different names*

### Comparing `torch_trandsforms-0.3.5/torch_trandsforms/value.py` & `torch_trandsforms-0.3.6/torch_trandsforms/value.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         assert isinstance(low, (int, float, torch.Tensor)), f"low must be a number (got {type(low)})"
         assert isinstance(hi, (int, float, torch.Tensor)), f"hi must be a number or tensor (got {type(hi)})"
 
         if isinstance(hi, (int, float)) and isinstance(low, (int, float)):
             assert low < hi, f"hi ({hi}) must be a number greater than low ({low})"
         else:
             diff = low < hi
-            assert isinstance(diff, torch.Tensor), f"this should never run - mypy check"
+            assert isinstance(diff, torch.Tensor), f"this should never fail - mypy check"
             assert torch.all(diff), f"hi ({hi}) must be a number greater than low ({low})"
 
         if isinstance(low, torch.Tensor) and low.ndim > 0:
             low = low.view(*low.shape, *[1] * self.nd)
 
         self.low = low
 
@@ -173,15 +173,16 @@
         assert isinstance(a, (float, torch.Tensor)) and 0 < a, f"a must be a float or tensor greater than 0"
         assert isinstance(b, (float, torch.Tensor)) and 0 < b, f"b must be a float or tensor greater than 0"
         self.dist = torch.distributions.beta.Beta(a, b)
 
         self.copy_input = copy_input
 
     def apply(self, input, **params):
-        probs = torch.broadcast_to(torch.rand(*input.shape[-self.nd :], device=self.dist.concentration1.device) < self.prob, input.shape)
+        probs: torch.Tensor = torch.rand(*input.shape[-self.nd :], device=self.dist.concentration1.device) < self.prob
+        probs = torch.broadcast_to(probs, input.shape)
         values = torch.broadcast_to((self.low - self.hi) * self.dist.sample(input.shape[-self.nd :]) + self.hi, input.shape)
         if self.copy_input:
             input = input.clone()
         input[probs] = values[probs]
         return input
 
 
@@ -205,15 +206,16 @@
         >>>
         >>> image = torch.rand(3, 224, 224)  # image of size 224x224 (CxHxW)
         >>> noiser = AdditiveBetaNoise(prob=0.1, nd=2)  # generates probabilities on a pixel-level (i.e. additive greyscale noise)
         >>> noiser = AdditiveBetaNoise(prob=0.1, nd=3)  # generates probabilities on a color-level (i.e. additive R/G/B noise)
     """
 
     def apply(self, input, **params):
-        probs = torch.broadcast_to(torch.rand(*input.shape[-self.nd :], device=self.dist.concentration1.device) < self.prob, input.shape)
+        probs: torch.Tensor = torch.rand(*input.shape[-self.nd :], device=self.dist.concentration1.device) < self.prob
+        probs = torch.broadcast_to(probs, input.shape)
         values = torch.broadcast_to((self.low - self.hi) * self.dist.sample(input.shape[-self.nd :]) + self.hi, input.shape)
         if self.copy_input:
             input = input.clone()
         input[probs] += values[probs]
         return input
```

### Comparing `torch_trandsforms-0.3.5/PKG-INFO` & `torch_trandsforms-0.3.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: torch-trandsforms
-Version: 0.3.5
-Summary: A pytorch-first transform library for ND data, such as multi-channel 3D volumes
-Home-page: https://github.com/alexandrainst/torch-trandsforms
-License: MIT
-Keywords: pytorch,transforms,torchvision,data
-Author: Oliver Hjermitslev
-Author-email: oliver.gyldenberg@alexandra.dk
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: torch (>=1.13.1)
-Requires-Dist: torchvision (>=0.14.0)
-Project-URL: Repository, https://github.com/alexandrainst/torch-trandsforms
-Description-Content-Type: text/markdown
-
 # torch traNDsforms
 
 <div align="center">
 
 [![build](https://github.com/alexandrainst/torch-trandsforms/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/alexandrainst/torch-trandsforms/actions/workflows/build.yml?query=branch%3Amain)
 [![Python Version](https://img.shields.io/pypi/pyversions/torch-trandsforms.svg)](https://pypi.org/project/torch-trandsforms/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/alexandrainst/torch-trandsforms/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
@@ -68,80 +43,68 @@
 
 ```bash
 conda install torch_trandsforms
 ```
 
 ## Usage
 
-Creating the RandomRotate90 class, as an example of customizing your own transform:
+Creating a single transform that rotates both input data and ground truth data. The data is considered 3D with a leading channel dimension.
+
+![RandomRotate](./examples/figures/RandomRotate.png)
 
 ```python
 import torch
-from torch_trandsforms.base import BaseTransform
+from torch_trandsforms import RandomRotate
 
-class RandomRotate90(BaseTransform):  # note the use of BaseTransform as base class here
-    """
-    Rotates the input 90 degrees around a randomly determined axis
-    NOTE: This is the not actual implementation of RandomRotate90
-    """
-    def __init__(self, nd=3, p=0.5):
-        super().__init__(p = p, nd = nd)
-        self.options = self._get_options(nd)
-
-    def _get_options(self, nd):
-        """
-        Create potential rotations based on the nd argument
-        This can be lower than the number of dimensions of the actual input
-            in case you do not want a leading dimension to be rotated
-        """
-        options = []
-
-        for i in range(nd):
-            for j in range(nd):
-                if not i == j:
-                    options.append((-i-1, -j-1))
-
-        return options
-    
-    def get_parameters(self, **inputs):
-        """
-        overrides the base get_parameters to choose a random
-            rotation option for each input
-        """
-        rotation = random.choice(self.options)
-        return {'rot':rotation}
-    
-    def apply(self, input, **params):
-        """
-        apply MUST be overwritten 
-        It is applied to each input sequentially, and thus must have
-            parameters that are exactly equal for each instance,
-            meaning most likely NO randomization here
-        """
-        rot = params['rot']
-        return torch.rot90(input, dims=rot)
-```
+# create data and target
+input_tensor = torch.rand((3,16,16,16), device="cuda", dtype=torch.float32)
+target_tensor = torch.rand((1,16,16,16), device="cuda", dtype=torch.float32)
 
-And we can now use our class to demonstrate the library functionality:
+# create our random rotator, which rotates dim -3 from -90 to 90, dim -2 from -90 to 90, and dim -1 from -180 to 180
+# this operates only on inputs with the keynames "input" or "target" and in the trailing 3 dimensions
+rotator = RandomRotate((90,90,180), nd=3, keys=["input", "target"], align_corners=True)
 
-```python
-torch.manual_seed(451)  # all randomization uses torch.random in the actual implementation
+# transform the data and target
+transformed = rotator(input=input_tensor, target=target_tensor)
 
-tensor = torch.arange(16).view(2,2,2,2)  # create a 4D tensor
-another_tensor = torch.arange(16).view(2,2,2,2)  # create an exactly equal tensor for demonstration
+# the data is recovered using the same keys as in the input
+data = transformed["input"]
+target = transformed["target"]
+```
 
-print(tensor)
-print(another_tensor)
+Create a Compose object to run a sequence of transforms one after another:
 
-random_rotator = RandomRotate90(nd=2, p=1.)  # we only want the last two dimensions to be rotateable but it should rotate every time (p=1)
+![ComposeExample](./examples/figures/Compose.png)
 
-transformed = random_rotator(data=tensor, foo=another_tensor)  # "data" is arbitrary, it is the key that will be returned, demonstrated by "foo"
+```python
+import torch
+from torch_trandsforms import Compose, RandomResize, RandomRotate, RandomCrop, RandomApply, UniformNoise, GaussianNoise, SaltAndPepperNoise
 
-print(transformed['data'])
-print(transformed['foo'])
+# create data and target
+input_tensor = torch.rand((3,16,16,16), device="cuda", dtype=torch.float32)
+target_tensor = torch.rand((16,16,16), device="cuda").round()
+
+# create our transform pipeline using some shape/size augmentation on both input and target, as well as some noise on the input
+transform = Compose([
+    RandomResize(0.3, p=0.75, keys="*"),  # keys="*" is the same as keys=["foo", "bar"] here
+    RandomRotate([180,180,180], sample_mode="nearest", p=0.9, nd=3, keys=["foo", "bar"]),
+    RandomCrop(16, padding=0, p=1.0, keys="*"),  # nd is 3 by default - but nd=1,2,3 all work here, just on the trailing dimensions
+    RandomApply([
+        UniformNoise(p=1.0, low=-0.2, hi=0.2, keys=["foo"]),  # for most noise transforms, we only want the data to be augmented
+        GaussianNoise(mean=torch.tensor(0.0, device="cuda"), std=0.05, p=1.0, keys=["foo"]),
+        SaltAndPepperNoise(0.2, low=0.0, hi=1.0, a=torch.tensor(0.5, device="cuda"), p=1.0, copy_input=True, keys=["foo"])
+    ], min=1, max=1)  # apply exactly 1 of the above three transforms each time
+])
+
+# transform the data and target
+transformed = transform(foo=input_tensor, bar=target_tensor)
+
+# the data is recovered using the same keys as in the input
+data = transformed["foo"]
+target = transformed["bar"]
 ```
 
 For more examples of use, see [EXAMPLES.md](https://github.com/alexandrainst/torch-trandsforms/blob/main/examples/EXAMPLES.md)
 
 ## Speed
 
 Please see [TIMING.md](https://github.com/alexandrainst/torch-trandsforms/blob/main/TIMING.md) for timings. See [test_speed.py](https://github.com/alexandrainst/torch-trandsforms/blob/main/test_speed.py) for methodology.
@@ -167,14 +130,15 @@
 
 Later additions (and reasons for postponing):
  - [ ] Arbitrary rotations (missing ND affine_grid and grid_sample)
  - [ ] Gaussian Blur (missing implementation of ND convolution)
  - [ ] Affine transformations (missing efficient ND computation)
 
 Potential additions:
+ - [ ] ND Bounding Boxes
  - [ ] Geometric operations using PyTorch Geometric
  - [ ] Point clouds, meshes using PyTorch 3D
  - [ ] Data loading, sampling, and structures
  - [ ] torchscript compatibility
 
 ## Contributing
 
@@ -200,8 +164,7 @@
   title = {A pytorch-first transform library for ND data, such as multi-channel 3D volumes},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/alexandrainst/torch-trandsforms}}
 }
 ```
-
```

