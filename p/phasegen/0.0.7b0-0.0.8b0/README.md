# Comparing `tmp/phasegen-0.0.7b0.tar.gz` & `tmp/phasegen-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasegen-0.0.7b0.tar", max compression
+gzip compressed data, was "phasegen-0.0.8b0.tar", max compression
```

## Comparing `phasegen-0.0.7b0.tar` & `phasegen-0.0.8b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      725 2024-04-15 08:39:53.445649 phasegen-0.0.7b0/README.md
--rw-r--r--   0        0        0     4814 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/__init__.py
--rw-r--r--   0        0        0    15044 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/coalescent_models.py
--rw-r--r--   0        0        0    14488 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/comparison.py
--rw-r--r--   0        0        0    37050 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/demography.py
--rw-r--r--   0        0        0    85927 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/distributions.py
--rw-r--r--   0        0        0     3278 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/expm.py
--rw-r--r--   0        0        0    27043 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/inference.py
--rw-r--r--   0        0        0     2378 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/lineage.py
--rw-r--r--   0        0        0     2751 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/locus.py
--rw-r--r--   0        0        0     2653 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/norms.py
--rw-r--r--   0        0        0    18837 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/rewards.py
--rw-r--r--   0        0        0     1121 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/serialization.py
--rw-r--r--   0        0        0    11106 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/spectrum.py
--rw-r--r--   0        0        0    29578 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/state_space.py
--rw-r--r--   0        0        0    53044 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/state_space_old.py
--rw-r--r--   0        0        0     1229 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/utils.py
--rw-r--r--   0        0        0     4478 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/visualization.py
--rw-r--r--   0        0        0      931 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/pyproject.toml
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.7b0/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-04-23 11:44:03.428096 phasegen-0.0.8b0/README.md
+-rw-r--r--   0        0        0     4814 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/__init__.py
+-rw-r--r--   0        0        0    15356 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/coalescent_models.py
+-rw-r--r--   0        0        0    14488 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/comparison.py
+-rw-r--r--   0        0        0    37050 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/demography.py
+-rw-r--r--   0        0        0    85998 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/distributions.py
+-rw-r--r--   0        0        0     3278 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/expm.py
+-rw-r--r--   0        0        0    27043 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/inference.py
+-rw-r--r--   0        0        0     2378 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/lineage.py
+-rw-r--r--   0        0        0     2751 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/locus.py
+-rw-r--r--   0        0        0     2653 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/norms.py
+-rw-r--r--   0        0        0    18837 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/rewards.py
+-rw-r--r--   0        0        0     1121 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/serialization.py
+-rw-r--r--   0        0        0    11106 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/spectrum.py
+-rw-r--r--   0        0        0    29757 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/state_space.py
+-rw-r--r--   0        0        0    53044 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/state_space_old.py
+-rw-r--r--   0        0        0     1229 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/utils.py
+-rw-r--r--   0        0        0     4478 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/phasegen/visualization.py
+-rw-r--r--   0        0        0      931 2024-04-23 11:44:03.444096 phasegen-0.0.8b0/pyproject.toml
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.8b0/PKG-INFO
```

### Comparing `phasegen-0.0.7b0/README.md` & `phasegen-0.0.8b0/README.md`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/__init__.py` & `phasegen-0.0.8b0/phasegen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PhaseGen package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-04-09"
 
-__version__ = '0.0.7-beta'
+__version__ = '0.0.8-beta'
 
 import logging
 import os
 import sys
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 from tqdm import tqdm
```

### Comparing `phasegen-0.0.7b0/phasegen/coalescent_models.py` & `phasegen-0.0.8b0/phasegen/coalescent_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,37 @@
     def get_rate(self, s1: int, s2: int) -> float:
         """
         Get rate for a merger collapsing k1 lineages into k2 lineages.
 
         :param s1: Number of lineages in the first state.
         :param s2: Number of lineages in the second state.
         :return: The rate.
+        :meta private:
         """
         # not possible
         if s2 > s1:
             return 0
 
         return self._get_rate(b=s1, k=s1 + 1 - s2)
 
     def get_rate_block_counting(self, n: int, s1: np.ndarray, s2: np.ndarray) -> float:
         r"""
         Get (positive) rate between two block counting states.
-        :math:`{ (a_1,...,a_n) \in \mathbb{Z}^+ : \sum_{i=1}^{n} a_i = n \}`.
+
+        A block counting state is a vector of length ``n`` where each element represents the number of lineages
+        subtending ``i`` lineages in the coalescent tree.
+
+        .. math::
+            (a_1,...,a_n) \in \mathbb{Z}_+^n : \sum_{i=1}^{n} a_i = n.
 
         :param n: Number of lineages.
         :param s1: Block configuration 1, a vector of length n.
         :param s2: Block configuration 2, a vector of length n.
         :return: The rate.
+        :meta private:
         """
         diff = s2 - s1
 
         # make sure only one class has one more lineage
         if np.sum(diff == 1) == 1 and n == s1.shape[0]:
 
             # get the index for the class that lost lineages
@@ -109,14 +116,15 @@
     def coalesce(self, n: int, blocks: np.ndarray) -> List[Tuple[np.ndarray, float]]:
         """
         Coalesce a state.
 
         :param n: The total number of lineages.
         :param blocks: The lineages in each block.
         :return: List of coalesced states and their rates.
+        :meta private:
         """
         pass
 
 
 class StandardCoalescent(CoalescentModel):
     """
     Standard (Kingman) coalescent model. Refer to
@@ -174,14 +182,15 @@
     def coalesce(self, n: int, blocks: np.ndarray[int]) -> List[Tuple[np.ndarray, float]]:
         """
         Coalesce a state.
 
         :param n: The total number of lineages.
         :param blocks: The lineages in each block.
         :return: List of coalesced states and their rates.
+        :meta private:
         """
         n_blocks = len(blocks)
         states = []
 
         # default state space
         if n_blocks == 1:
             if blocks[0] > 1:
@@ -231,14 +240,15 @@
     def coalesce(self, n: int, blocks: np.ndarray[int]) -> List[Tuple[np.ndarray, float]]:
         """
         Coalesce a state.
 
         :param n: The total number of lineages.
         :param blocks: The lineages in each block.
         :return: List of coalesced states and their rates.
+        :meta private:
         """
         n_blocks = len(blocks)
         states = []
 
         # default state space
         if n_blocks == 1:
             for k in range(1, blocks[0]):
@@ -374,18 +384,18 @@
         """
         super().__init__()
 
         if not 0 < psi < 1:
             raise ValueError("Psi must be between 0 and 1.")
 
         #: The fraction of the population replaced by offspring in one large reproduction event
-        self.psi = psi
+        self.psi: float = psi
 
         #: The rate of potential multiple merger events.
-        self.c = c
+        self.c: float = c
 
         #: Whether to scale coalescence time
         self.scale_time: bool = scale_time
 
         #: The standard coalescent model
         self._standard = StandardCoalescent()
```

### Comparing `phasegen-0.0.7b0/phasegen/comparison.py` & `phasegen-0.0.8b0/phasegen/comparison.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/demography.py` & `phasegen-0.0.8b0/phasegen/demography.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/distributions.py` & `phasegen-0.0.8b0/phasegen/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 Probability distributions.
 """
 
 import copy
 import itertools
 import logging
 from abc import ABC, abstractmethod
-from collections import Counter
 from collections.abc import Mapping
 from functools import cached_property, cache
-from math import comb
 from math import factorial
 from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator
 
 import numpy as np
 from scipy.ndimage import gaussian_filter1d
 
 from .coalescent_models import StandardCoalescent, CoalescentModel, BetaCoalescent, DiracCoalescent
@@ -559,14 +557,15 @@
     @cached_property
     def loci(self) -> MarginalLocusDistributions:
         """
         Marginal distributions over each locus.
         """
         return MarginalLocusDistributions(self)
 
+    @cache
     def moment(
             self,
             k: int,
             rewards: Tuple[Reward, ...] = None,
             start_time: float = None,
             end_time: float = None,
             center: bool = True,
@@ -595,42 +594,48 @@
 
         if k == 0:
             return 1
 
         # center moments around the mean
         if center and k > 1:
 
-            # center moment
-            if len(set(rewards)) == 1:
-
-                reward = list(rewards)[0]
-                components = []
-
-                for i in range(k + 1):
-                    mu_i = PhaseTypeDistribution.moment(self, i, (reward,) * i, start_time, end_time, False)
-                    mu1_k_i = PhaseTypeDistribution.moment(self, 1, (reward,), start_time, end_time, False) ** (k - i)
-
-                    components += [comb(k, i) * (-1) ** (k - i) * mu_i * mu1_k_i]
+            components = []
 
-                return sum(components)
+            # first order moments
+            means = [
+                PhaseTypeDistribution.moment(
+                    self,
+                    k=1,
+                    rewards=(rewards[i],),
+                    start_time=start_time,
+                    end_time=end_time
+                ) for i in range(k)
+            ]
+
+            for i in range(k + 1):
+                # iterate over all possible subsets of rewards of size i
+                for indices in itertools.combinations(range(k), i):
+
+                    # joint moment
+                    mu_i = PhaseTypeDistribution.moment(
+                        self,
+                        k=i,
+                        rewards=tuple(rewards[j] for j in indices),
+                        start_time=start_time,
+                        end_time=end_time,
+                        center=False,
+                        permute=permute
+                    )
 
-            # center cross-moment
-            else:
-
-                cross_components = []
+                    # product of means of remaining rewards
+                    mu1 = np.prod([means[j] for j in range(k) if j not in indices])
 
-                # count number of different rewards
-                for reward, count in Counter(rewards).items():
-                    cross_components += [
-                        PhaseTypeDistribution.moment(self, count, (reward,) * count, start_time, end_time, True)
-                    ]
+                    components += [(-1) ** (k - i) * mu_i * mu1]
 
-                uncentered = PhaseTypeDistribution.moment(self, k, rewards, start_time, end_time, False)
-
-                return uncentered - np.prod(cross_components)
+            return sum(components)
 
         if permute:
             # get all possible permutations of rewards
             permutations = list(itertools.permutations(rewards))
 
             # compute average over all permutations
             return sum(self._raw_moment(k, r, start_time, end_time) for r in permutations) / len(permutations)
@@ -2187,14 +2192,15 @@
         return PhaseTypeDistribution(
             reward=UnitReward(),
             tree_height=self.tree_height,
             state_space=state_space,
             demography=self.demography
         )
 
+    @cache
     def moment(
             self,
             k: int = 1,
             rewards: Tuple[Reward, ...] = None,
             start_time: float = None,
             end_time: float = None,
             center: bool = True,
```

### Comparing `phasegen-0.0.7b0/phasegen/expm.py` & `phasegen-0.0.8b0/phasegen/expm.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/inference.py` & `phasegen-0.0.8b0/phasegen/inference.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/lineage.py` & `phasegen-0.0.8b0/phasegen/lineage.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/locus.py` & `phasegen-0.0.8b0/phasegen/locus.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/norms.py` & `phasegen-0.0.8b0/phasegen/norms.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/rewards.py` & `phasegen-0.0.8b0/phasegen/rewards.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/serialization.py` & `phasegen-0.0.8b0/phasegen/serialization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/spectrum.py` & `phasegen-0.0.8b0/phasegen/spectrum.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/state_space.py` & `phasegen-0.0.8b0/phasegen/state_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,20 @@
             epoch=self.epoch
         )
 
 
 class BlockCountingStateSpace(StateSpace):
     r"""
     Rate matrix for block counting state space where there is one state per sample configuration:
-    :math:`{ (a_1,...,a_n) \in \mathbb{Z}^+ : \sum_{i=1}^{n} a_i = n \}`,
+
+    A block counting state is a vector of length ``n`` where each element represents the number of lineages
+    subtending ``i`` lineages in the coalescent tree.
+
+        .. math::
+            (a_1,...,a_n) \in \mathbb{Z}_+^n : \sum_{i=1}^{n} a_i = n.
 
     per deme and per locus. This state space can distinguish between different tree topologies
     and is thus used when computing statistics based on the SFS.
     """
 
     def __init__(
             self,
```

### Comparing `phasegen-0.0.7b0/phasegen/state_space_old.py` & `phasegen-0.0.8b0/phasegen/state_space_old.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/utils.py` & `phasegen-0.0.8b0/phasegen/utils.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/phasegen/visualization.py` & `phasegen-0.0.8b0/phasegen/visualization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.7b0/pyproject.toml` & `phasegen-0.0.8b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phasegen"
-version = "0.0.7-beta"
+version = "0.0.8-beta"
 description = "Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `phasegen-0.0.7b0/PKG-INFO` & `phasegen-0.0.8b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasegen
-Version: 0.0.7b0
+Version: 0.0.8b0
 Summary: Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

