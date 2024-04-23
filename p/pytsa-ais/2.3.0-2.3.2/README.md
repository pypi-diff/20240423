# Comparing `tmp/pytsa_ais-2.3.0.tar.gz` & `tmp/pytsa_ais-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsa_ais-2.3.0.tar", max compression
+gzip compressed data, was "pytsa_ais-2.3.2.tar", max compression
```

## Comparing `pytsa_ais-2.3.0.tar` & `pytsa_ais-2.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.0/LICENSE
--rw-r--r--   0        0        0    15712 2024-02-06 12:03:47.000000 pytsa_ais-2.3.0/README.md
--rw-r--r--   0        0        0      952 2024-04-10 08:15:06.583351 pytsa_ais-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-10 08:15:13.299351 pytsa_ais-2.3.0/pytsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.0/pytsa/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.0/pytsa/data/geometry/__init__.py
--rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/denmark.json
--rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/germany.json
--rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/netherlands_detailed.json
--rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/norway.json
--rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/sweden.json
--rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/__init__.py
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/diffquants.pkl
--rw-r--r--   0        0        0     8159 2024-01-18 12:40:18.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/dquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/hquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/squants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/tquants.pkl
--rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.0/pytsa/decoder/__init__.py
--rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.0/pytsa/decoder/ais_decoder.py
--rw-r--r--   0        0        0     1548 2024-01-30 09:17:11.000000 pytsa_ais-2.3.0/pytsa/decoder/filedescriptor.py
--rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.0/pytsa/logger.py
--rw-r--r--   0        0        0     5956 2024-02-09 15:42:47.000000 pytsa_ais-2.3.0/pytsa/structs.py
--rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.0/pytsa/trajectories/__init__.py
--rw-r--r--   0        0        0     7561 2024-04-09 11:43:49.471049 pytsa_ais-2.3.0/pytsa/trajectories/inspect.py
--rw-r--r--   0        0        0     5072 2024-04-10 08:13:27.591352 pytsa_ais-2.3.0/pytsa/trajectories/rules.py
--rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.0/pytsa/tsea/__init__.py
--rw-r--r--   0        0        0    28174 2024-03-19 09:36:35.324947 pytsa_ais-2.3.0/pytsa/tsea/search_agent.py
--rw-r--r--   0        0        0     5336 2024-04-08 10:43:36.000000 pytsa_ais-2.3.0/pytsa/tsea/split.py
--rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.0/pytsa/tsea/targetship.py
--rw-r--r--   0        0        0    13571 2024-04-03 18:48:40.000000 pytsa_ais-2.3.0/pytsa/utils.py
--rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.0/pytsa/visualization/__init__.py
--rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.0/pytsa/visualization/ecdf.py
--rw-r--r--   0        0        0    13488 2024-04-02 10:43:50.989572 pytsa_ais-2.3.0/pytsa/visualization/misc.py
--rw-r--r--   0        0        0    16725 1970-01-01 00:00:00.000000 pytsa_ais-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.2/LICENSE
+-rw-r--r--   0        0        0    15713 2024-04-12 09:18:41.000000 pytsa_ais-2.3.2/README.md
+-rw-r--r--   0        0        0      952 2024-04-23 07:40:02.244003 pytsa_ais-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-23 07:40:07.960003 pytsa_ais-2.3.2/pytsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.2/pytsa/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.2/pytsa/data/geometry/__init__.py
+-rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/denmark.json
+-rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/germany.json
+-rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/netherlands_detailed.json
+-rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/norway.json
+-rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/sweden.json
+-rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/__init__.py
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/diffquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/dquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/squants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/tquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/trquants.pkl
+-rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.2/pytsa/decoder/__init__.py
+-rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.2/pytsa/decoder/ais_decoder.py
+-rw-r--r--   0        0        0     1548 2024-04-19 11:16:21.000000 pytsa_ais-2.3.2/pytsa/decoder/filedescriptor.py
+-rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.2/pytsa/logger.py
+-rw-r--r--   0        0        0     6472 2024-04-19 11:52:30.000000 pytsa_ais-2.3.2/pytsa/structs.py
+-rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.2/pytsa/trajectories/__init__.py
+-rw-r--r--   0        0        0     9694 2024-04-19 08:41:02.000000 pytsa_ais-2.3.2/pytsa/trajectories/inspect.py
+-rw-r--r--   0        0        0     5813 2024-04-15 11:06:38.000000 pytsa_ais-2.3.2/pytsa/trajectories/rules.py
+-rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.2/pytsa/tsea/__init__.py
+-rw-r--r--   0        0        0    29053 2024-04-23 07:39:41.352004 pytsa_ais-2.3.2/pytsa/tsea/search_agent.py
+-rw-r--r--   0        0        0     8204 2024-04-23 07:05:46.236046 pytsa_ais-2.3.2/pytsa/tsea/split.py
+-rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.2/pytsa/tsea/targetship.py
+-rw-r--r--   0        0        0    14189 2024-04-19 11:22:56.000000 pytsa_ais-2.3.2/pytsa/utils.py
+-rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.2/pytsa/visualization/__init__.py
+-rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.2/pytsa/visualization/ecdf.py
+-rw-r--r--   0        0        0    15336 2024-04-15 13:35:43.000000 pytsa_ais-2.3.2/pytsa/visualization/misc.py
+-rw-r--r--   0        0        0    16726 1970-01-01 00:00:00.000000 pytsa_ais-2.3.2/PKG-INFO
```

### Comparing `pytsa_ais-2.3.0/LICENSE` & `pytsa_ais-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/README.md` & `pytsa_ais-2.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -323,22 +323,22 @@
 ## Citation
 
 If you use this module in your research, please consider citing this repository as follows:
 
 ```
 @misc{pytsa2024,
   author = {Paulig, Niklas},
-  title = {{PyTSA}: A Python Module for Extracting Trajectories from Raw AIS Data},
+  title = {{PyTSA}: Python Trajectory Splitting and Assessment Agent for AIS Data},
   year = {2024},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/nikpau/pytsa}},
 }
 ```
 
 ## Appendix
 
 ### Split-point procedure
 
 The split-point procedure takes place in the `pytsa.tsea.split` module. Its main function, `is_split_point()`, will be called on every pair of AIS messages in the dataset. The function returns a boolean value, indicating whether the pair of messages is a split point or not. 
 
-In case you want to adapt the split-point procedure to your dataset, you can use the `pytsa.tsea.split` module as a starting point.
+In case you want to adapt the split-point procedure to your dataset, you can use the `pytsa.tsea.split` module as a starting point.
```

### Comparing `pytsa_ais-2.3.0/pyproject.toml` & `pytsa_ais-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytsa-ais"
-version = "2.3.0"
+version = "2.3.2"
 description = "Toolbox for extracting trajectories and monitoring vessels from raw AIS records."
 authors = ["Niklas Paulig <niklas.paulig@tu-dresden.de>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytsa_ais-2.3.0/pytsa/data/geometry/denmark.json` & `pytsa_ais-2.3.2/pytsa/data/geometry/denmark.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/data/geometry/germany.json` & `pytsa_ais-2.3.2/pytsa/data/geometry/germany.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/data/geometry/netherlands_detailed.json` & `pytsa_ais-2.3.2/pytsa/data/geometry/netherlands_detailed.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/data/geometry/norway.json` & `pytsa_ais-2.3.2/pytsa/data/geometry/norway.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/data/geometry/sweden.json` & `pytsa_ais-2.3.2/pytsa/data/geometry/sweden.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/decoder/ais_decoder.py` & `pytsa_ais-2.3.2/pytsa/decoder/ais_decoder.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/decoder/filedescriptor.py` & `pytsa_ais-2.3.2/pytsa/decoder/filedescriptor.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 If you are using a different data set, please
 change the values accordingly.
 """
 from enum import Enum
 
 class BaseColumns(Enum):
     """
-    For the decoder to work, both the
-    Dynamic and Static source files
-    must feature the following identical 
-    column names.
+    Column names that must be present in both
+    the dynamic and static source files,
+    otherwise the decoder will raise an error.
     """
     __order__ = (
         "TIMESTAMP MESSAGE_ID "
         "RAW_MESSAGE RAW_MESSAGE1 "
         "RAW_MESSAGE2"
     )
     TIMESTAMP: str = "timestamp"
```

### Comparing `pytsa_ais-2.3.0/pytsa/logger.py` & `pytsa_ais-2.3.2/pytsa/logger.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/structs.py` & `pytsa_ais-2.3.2/pytsa/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 import ciso8601
 from typing import List, Union
-import numpy as np
 
 Latitude  = float
 Longitude = float
 MMSI = int
 UNIX_TIMESTAMP = int | float
 
-
-
 class NONAME_TYPE:
     pass
 NONAME = NONAME_TYPE()
 
 class NOINDEX_TYPE:
     pass
 NOINDEX = NOINDEX_TYPE()
 
 class ShellError(Exception):
     pass
 
+def _mflatten(l):
+    """
+    Flatten a mixed list
+    of numbers and lists
+    """
+    for el in l:
+        if isinstance(el, (list,range)):
+            yield from _mflatten(el)
+        else:
+            yield el
+
 @dataclass
 class AISMessage:
     """
     AIS Message object
     """
     sender: MMSI
     timestamp: UNIX_TIMESTAMP
@@ -90,22 +98,22 @@
     MILITARY = 35
     SAILING = 36
     PLEASURE = 37
     HSC = range(40,50) # High speed craft
     PASSENGER = range(60,70)
     CARGO = range(70,80)
     TANKER = range(80,90)
-    OTHER = range(90,100)
+    OTHER = list(_mflatten([33,34,50,51,list(range(52,60)),list(range(90,100))]))
     
-    def from_value(self, value: int) -> ShipType:
+    def from_value(value: int) -> ShipType:
         """
         Return the ship type from a value
         """
         for st in ShipType:
-            if isinstance(st.value, range):
+            if isinstance(st.value, (list,range)):
                 if value in st.value:
                     return st
             else:         
                 if value == st.value:
                     return st
         raise ValueError(f"Ship type {value} not found.")
 
@@ -161,14 +169,23 @@
 
     def _aspect_ratio(self) -> float:
         """
         Return the aspect ratio of the bounding box
         """
         return (self.LONMAX-self.LONMIN)/(self.LATMAX-self.LATMIN)
 
+    def contains(self, message: AISMessage) -> bool:
+        """
+        Check if a position is within the bounding box
+        """
+        return (
+            self.LATMIN <= message.lat <= self.LATMAX and
+            self.LONMIN <= message.lon <= self.LONMAX
+        )
+
 @dataclass
 class Position:
     """
     Position object for a geographical point.
     """
     lat: Latitude
     lon: Longitude
```

### Comparing `pytsa_ais-2.3.0/pytsa/trajectories/inspect.py` & `pytsa_ais-2.3.2/pytsa/trajectories/inspect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 """
-Trajectory Splitter.
+Trajectory Inspector.
 ====================
 
-This module contains the class for splitting trajectories
-according to a set of rules.
+This module contains the Inspector class, which is used to filter
+trajectories based on a set of rules. The rules are defined in the
+:mod:`pytsa.trajectories.rules` module.
+
+The module also contains a set of functions that can be used to
+calculate the smoothness and change of course of a navigational
+track. These functions can be used as rules in the Inspector class.
+
 """
 import numpy as np
 import multiprocessing as mp
 from copy import deepcopy
 
 from ..logger import logger
 from ..structs import Track
-from ..tsea.targetship import TargetShip, AISMessage, Targets
+from ..tsea.targetship import TargetShip, Targets
 from .rules import Recipe
 
 def print_rejection_rate(n_rejected: int, n_total: int) -> None:
     if n_total == 0:
         logger.warning("No trajectories to filter.")
         return
     logger.info(
         f"Filtered {n_total} trajectories. "
         f"{(n_rejected)/n_total*100:.2f}% rejected."
     )
 
 class Inspector:
     """
-    The Inspector takes a dictionary of rules 
-    and applies them to the trajectories of 
-    a `Targets` type dictionary passed to it.
-    
-    The dict passed to the inspector
-    is expected to have the following structure:
-        dict[MMSI,TargetVessel]
-    and will most likely be the output of the
-    :meth:`SearchAgent.get_all_ships()` method.
+    The Inspector is the central class for assessing 
+    properties of trajectories, based on a set of 
+    rules bundled in a Recipe object. The Inspector
+    class applies the rules to a set of target ships
+    and returns the accepted and rejected trajectories.
     
-    For how to create a recipe, see the 
-    :mod:`pytsa.trajectories.rules` module.
+    Parameters:
+    - data (Targets): A dictionary of TargetShip objects, 
+        where the keys are the MMSI numbers of the target 
+        ships.
+        
+    - recipe (Recipe): A Recipe object containing the rules
+        to be applied to the trajectories.
     """
     def __init__(self, data: Targets, recipe: Recipe) -> None:
         self.data = data
         self.condition = recipe.cook()
         self.rejected: Targets = {}
         self.accepted: Targets = {}
     
-    def inspect(self, njobs: int = 4) -> tuple[Targets,Targets]:
+    def inspect(self, njobs: int = 1) -> tuple[Targets,Targets]:
         """
         Inspects TargetShips in `data` and returns two dictionaries:
         - Accepted: Trajectories evalutating to False for the recipe
         - Rejected: Trajectories evalutating to True for the recipe
         
         The accepted and rejected dictionaries can contain the same MMSIs, 
         if the target ship has multiple tracks, and only some of them
@@ -132,77 +139,117 @@
         if vessel.mmsi not in target:
             target[vessel.mmsi] = deepcopy(vessel)
             target[vessel.mmsi].tracks = []
         target[vessel.mmsi].tracks.append(track)
 
 def cosine_of_angle_between(track: Track) -> float:
     """
-    Return the cosine of the angle between a track
-    of AIS Messages.
+    Return the cosines for all three consecutive
+    AIS Messages in a track.
     """
     positions = np.array([(msg.lon,msg.lat) for msg in track])
-    v1 = positions[:-2] - positions[1:-1] # p0 - p1 
+    v1 = positions[1:-1] - positions[:-2] # p1 - p0 
     v2 = positions[2:] - positions[1:-1] # p2 - p1
     
     # Dot product
     dot_product = np.einsum('ij,ij->i',v1,v2)
     # Norms
     norms = np.linalg.norm(v1,axis=1) * np.linalg.norm(v2,axis=1)
     
     return dot_product / norms
 
 def angle_between(track: Track) -> float:
     """
-    Return the angle between the track
-    of three AIS Messages.
+    Return the angles between each three consecutive
+    AIS Messages in a track.
     """
     _cos = cosine_of_angle_between(track)        
     return np.arccos(np.round(_cos,6)) # Round to avoid floating point errors
     
-def average_smoothness(track: Track, tau: int = 1) -> float:
-    """
-    Calculate the average smoothness of a navigational 
-    track.
-
-    This function computes the average smoothness of a 
-    path represented  by a list of AISMessage objects.  
-    It evaluates the smoothness based on the angles 
-    formed at each point along the path, where each 
-    angle is determined by a sequence of three consecutive 
-    AISMessage points. The smoothness is a measure of 
-    how straight or curved the path is, with larger 
-    angles indicating a smoother path.
-
-    The angle at each point is normalized by dividing it 
-    by π, with the function 'angle_between' used to 
-    calculate these angles. Since 'angle_between' returns 
-    values from 0 to π, the normalized angles will range 
-    from 0 (representing a U-turn)  to 1 (representing a 
-    straight line).
+# def average_smoothness(track: Track) -> float:
+#     """
+#     Calculate the average smoothness of a navigational 
+#     track.
+
+#     This function computes the average smoothness of a 
+#     path represented  by a list of AISMessage objects.  
+#     It evaluates the smoothness based on the angles 
+#     formed at each point along the path, where each 
+#     angle is determined by a sequence of three consecutive 
+#     AISMessage points. The smoothness is a measure of 
+#     how straight or curved the path is, with larger 
+#     angles indicating a smoother path.
+
+#     The angle at each point is normalized by dividing it 
+#     by π, with the function 'angle_between' used to 
+#     calculate these angles. Since 'angle_between' returns 
+#     values from 0 to π, the normalized angles will range 
+#     from 0 (representing a U-turn)  to 1 (representing a 
+#     straight line).
+
+#     Parameters:
+#     - track (Track): A list of AISMessage objects 
+#       representing the navigational path. Each AISMessage 
+#       contains positional data necessary for angle calculation.
+
+#     Returns:
+#     - float: The average smoothness of the track, 
+#       represented as a float. This value is the mean 
+#       of the normalized angles along the track, where 
+#       a larger values indicates a smoother track.
+
+#     Note:
+#     - The function assumes that the track has at least three 
+#        AISMessage points to form at least one angle. If the 
+#        track has fewer than three points, the behavior of the 
+#        function is unspecified.
+#     """
+#     if len(track) < 3:
+#         raise ValueError(
+#             "Average smoothness requires at "
+#             "least three messages per track. "
+#             "{} were given".format(len(track))
+#         )
+#     angles = angle_between(track)
+#     normalized_angles = (angles / np.pi)
+#     return np.mean(normalized_angles)
+
+def average_absolute_change_of_course(track: Track, degrees: bool = False) -> float:
+    """
+    Calculate the average absolute change of course 
+    of a navigational track.
+
+    This function computes the average absolute change 
+    of course of a path represented by a list of AISMessage 
+    objects. It evaluates the change of course based on 
+    the angles formed at each point along the path, where 
+    each angle is determined by a sequence of three 
+    consecutive AISMessage points. The change of course 
+    is a measure of how much the path changes direction 
+    at each point, with larger angles indicating a greater 
+    change of course.
 
     Parameters:
-    - track (Track): A list of AISMessage objects 
-      representing the navigational path. Each AISMessage 
-      contains positional data necessary for angle calculation.
+    - track (Track): A list of AISMessage objects
+        representing the navigational path. Each AISMessage 
+        contains positional data necessary for angle calculation.
+    
+    - degrees (bool): A boolean flag indicating whether
+        the output should be in degrees or radians. If 
+        True, the output will be in degrees; if False, 
+        the output will be in radians. The default value 
+        is False.
 
     Returns:
-    - float: The average smoothness of the track, 
-      represented as a float. This value is the mean 
-      of the normalized angles along the track, where 
-      a larger values indicates a smoother track.
+    - float: The average absolute change of course of the 
+      track in degrees or radians. This value is the mean 
+      of the absolute differences between consecutive 
+      normalized angles along the track, where a larger 
+      value indicates a greater change of course.
 
     Note:
-    - The function assumes that the track has at least three 
-       AISMessage points to form at least one angle. If the 
-       track has fewer than three points, the behavior of the 
-       function is unspecified.
-    """
-    assert tau > 0, "Tau must be a positive integer."
-    if len(track) < 3:
-        raise ValueError(
-            "Average smoothness requires at "
-            "least three messages per track. "
-            "{} were given".format(len(track))
-        )
-    angles = angle_between(track)
-    normalized_angles = (angles / np.pi)**tau
-    return np.mean(normalized_angles)
+    - The function requires that the track has at least three 
+       AISMessage points to form at least one angle.
+    """
+    assert len(track) >= 3, "Track must have at least three messages."
+    aacog = np.mean(angle_between(track))
+    return np.degrees(aacog) if degrees else aacog
```

### Comparing `pytsa_ais-2.3.0/pytsa/trajectories/rules.py` & `pytsa_ais-2.3.2/pytsa/trajectories/rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 from typing import Callable
 from inspect import signature
 from functools import partial
 from scipy.spatial import ConvexHull
 
 from ..structs import Track
+from ..logger import logger
 
 class Recipe:
     """
     Rule recipe class.
     =================
     
     This class is used to define a recipe for the TrajectorySplitter class.
@@ -130,26 +131,47 @@
     of the track of the given vessel is smaller than `span`.
     (Not used in the paper)
     """
     lat_span = np.ptp([v.lat for v in track])
     lon_span = np.ptp([v.lon for v in track])
     return lat_span > span and lon_span > span
 
-def convex_hull_area(track: Track, area: float) -> bool:
+def convex_hull_area(track: Track, area: float | tuple) -> bool:
     """
-    Return True if the area of the convex hull of the
-    track of the given vessel is smaller than `area`.
-    (Not used in the paper)
+    Reject a track if the area of the convex hull of the
+    track is smaller than `area`. If `area` is a tuple,
+    reject the track if the area is not within the range
+    of the tuple.
     """
     assert len(track) > 2, "Need at least 3 points to calculate convex hull"
     res = utm.from_latlon(
         np.array([p.lat for p in track]),
         np.array([p.lon for p in track])
     )
     points = np.array([res[0],res[1]]).T
-    return ConvexHull(points).area < area
+    # Convex hull calculation can fail for 
+    # some tracks, e.g. if all points are 
+    # colinear. In this case, we reject the track.
+    try:
+        _cvharea = ConvexHull(points).area
+        if isinstance(area,float):
+            return _cvharea < area
+        elif isinstance(area,tuple):
+            lower, upper = area
+            return not lower < _cvharea < upper
+        else:
+            raise TypeError(
+                f"Expected area to be a float or tuple, "
+                f"got {type(area)}"
+            )
+    except Exception as e:
+        logger.error(
+            f"Error in convex hull calculation: {e}"
+            "Rejecting track."
+            )
+        return True
 
 # Example recipe---------------------------------------------------------------
 ExampleRecipe = Recipe(
     partial(too_few_obs, n=100),
     partial(convex_hull_area, area=3e4)
 )
```

### Comparing `pytsa_ais-2.3.0/pytsa/tsea/__init__.py` & `pytsa_ais-2.3.2/pytsa/tsea/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/tsea/search_agent.py` & `pytsa_ais-2.3.2/pytsa/tsea/search_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import multiprocessing as mp
 import numpy as np
 import pandas as pd
 from scipy.spatial import cKDTree
 from ..logger import logger
 from ..structs import (
     BoundingBox, TimePosition,
-    UNIX_TIMESTAMP
+    UNIX_TIMESTAMP, ShipType
 )
 from . import split
 from ..decoder.filedescriptor import (
     BaseColumns, Msg12318Columns, Msg5Columns
 )
 from .targetship import (
     TargetShip, AISMessage, 
@@ -120,17 +120,16 @@
             distance_upper_bound=sr
         )
         # Sort out any infinite distances
         res = [indices[i] for i,j in enumerate(d) if j != float("inf")]
 
         return filtered.iloc[res]
     
-
-    def _time_filter(self, 
-                     df: pd.DataFrame, 
+    @staticmethod
+    def _time_filter(df: pd.DataFrame, 
                      date: UNIX_TIMESTAMP, 
                      delta: int) -> pd.DataFrame:
         """
         Filter a pandas dataframe to only return 
         rows whose `Timestamp` is not more than 
         `delta` minutes apart from imput `date`.
         """
@@ -233,18 +232,14 @@
 
         self.neighborhood = NeighborhoodTreeSearch(
             self.data_loader,
             self.time_delta,
             self.max_tgt_ships
         )
         
-        self.constructor = TargetShipConstructor(
-            self.data_loader
-        )
-        
         # Flag indicating whether the input data
         # is already decoded or not
         self.decoded = decoded
         
         # Length of the original AIS message dataframe
         self._n_original = 0
         # Length of the filtered AIS message dataframe
@@ -279,46 +274,61 @@
                 all vessels whose track is within the time delta of the
                 queried timestamp are returned.
         """
         assert interpolation in ["linear","spline","auto"], \
             "Interpolation method must be either 'linear', 'spline' or 'auto'"
         # Get neighbors
         neighbors = self.neighborhood.get_neighbors(tpos,search_radius)
-        tgts = self.constructor._sp_construct_target_vessels(neighbors,tpos,True)
+
+        constructor = TargetShipConstructor(
+            self.data_loader,
+            split.Splitter()
+        )
+        tgts = constructor._sp_construct_target_vessels(neighbors,tpos,True)
         # Contruct Splines for all target ships
         tgts = self._interpolate_trajectories(tgts,mode=interpolation)
         return tgts
     
     def extract_all(self,
                     njobs: int = 4, 
+                    alpha: float = 0.05,
                     skip_tsplit: bool = False) -> Targets:
         """
         Extracts a dictionary of all target ships in the
         frame of the search agent using the split-point
         method as described in the paper. 
         
         Parameters:
         ----------
         njobs: int
             Number of jobs to use for multiprocessing.
+        alpha: float
+            The significance level for the quantiles used
+            in the split point detection. Default is 0.05.
         skip_tsplit: bool
             If True, the split-point method is not used
             to split the tracks of the target ships.
             Instead, all vessels will only have one track,
             containing all time-ordered AIS messages
             comning from the same MMSI.
             
         Returns:
         --------
         dict: A dictionary of dict[MMSI,TargetShip]. 
         """
-        targets = self.constructor._mp_construct_target_vessels(
+        splitter = split.Splitter(alpha)
+        constructor = TargetShipConstructor(
+            self.data_loader,
+            splitter
+        )
+        targets = constructor._mp_construct_target_vessels(
             njobs,skip_tsplit
         )
-        self.constructor.print_trex_stats()
+        constructor.print_trex_stats()
+        splitter.print_split_stats()
         return targets
 
     def _interpolate_trajectories(self, 
                            tgts: Targets,
                            mode: str = "auto") -> Targets:
         """
         Interpolate all target ships' trajectories.
@@ -337,23 +347,30 @@
     A class for constructing TargetShip 
     objects from raw AIS messages.
 
     Attributes:
         `data_loader`: 
             An instance of the `pytsa.utils.DataLoader` 
             class used to load AIS message data.
+        `splitter`:
+            An instance of the `pytsa.tsea.split.Splitter`
+            class used to determine split points in
+            trajectories.
 
     Methods:
         `construct_target_vessels`: 
             Constructs TargetVessel objects from 
             a given DataFrame.
     """
-    def __init__(self, data_loader: DataLoader) -> None:
+    def __init__(self, 
+                 data_loader: DataLoader,
+                 splitter: split.Splitter) -> None:
         
         self.data_loader = data_loader
+        self.splitter = splitter
         
         # Statistics
         self._n_split_points = 0
         self._n_rejoined_tracks = 0
         self._n_duplicates = 0
         self._n_obs_raw = 0
         self._n_trajectories = 0
@@ -371,19 +388,20 @@
     def _impl_construct_target_vessel(self, 
                                       dyn: pd.DataFrame,
                                       stat: pd.DataFrame) -> Targets:
         """
         Construct a single TargetVessel object from a given dataframe.
         """
         MMSI = int(dyn[Msg12318Columns.MMSI.value].iloc[0])
+        ts = dyn[BaseColumns.TIMESTAMP.value].iloc[0].to_pydatetime().timestamp()
         # Initialize TargetVessel object
         tv =  TargetShip(
             ts = None,
             mmsi=MMSI,
-            ship_type=self._get_ship_type(stat,MMSI),
+            ship_type=self._get_ship_type(stat,MMSI,ts),
             length=self._get_ship_length(stat,MMSI),
             tracks=[[]]
         )
         first = True
                 
         dyn = dyn.sort_values(by=BaseColumns.TIMESTAMP.value)
         
@@ -525,15 +543,15 @@
         logger.info("Rejoining tracks...")
         for tgt in targets.values():
             rejoined = []
             for i, track in enumerate(tgt.tracks):
                 if i == 0:
                     rejoined.append(track)
                     continue
-                if not split.is_split_point(rejoined[-1][-1],track[0]):
+                if not self.splitter.is_split_point(rejoined[-1][-1],track[0]):
                     rejoined[-1].extend(track)
                     self._n_rejoined_tracks += 1
                 else:
                     rejoined.append(track)
             tgt.tracks = rejoined
         logger.info(f"Rejoined {self._n_rejoined_tracks} tracks.")
         return targets
@@ -553,15 +571,15 @@
             )
             ctr += 1
             for track in tgt.tracks:
                 track.sort(key=lambda x: x.timestamp)
                 _itracks = [] # Intermediary track
                 tstartidx = 0
                 for i, (msg_t0,msg_t1) in enumerate(pairwise(track)):
-                    if split.is_split_point(msg_t0,msg_t1):
+                    if self.splitter.is_split_point(msg_t0,msg_t1):
                         _itracks.append(track[tstartidx:i+1])
                         tstartidx = i+1
                         self._n_split_points += 1
             # Only keep tracks with more than one observation
             tgt.tracks = [track for track in _itracks if len(track) > 2]
             # If no tracks are left, remove target ship
             if not tgt.tracks:
@@ -601,34 +619,34 @@
             neighbors[Msg12318Columns.MMSI.value], 
             neighbors[BaseColumns.TIMESTAMP.value],
             neighbors[Msg12318Columns.LAT.value],  
             neighbors[Msg12318Columns.LON.value],
             neighbors[Msg12318Columns.SPEED.value],
             neighbors[Msg12318Columns.COURSE.value]):
             
-            ts: pd.Timestamp # make type hinting happy
+            ts: UNIX_TIMESTAMP = ts.to_pydatetime().timestamp() # Convert to unix
             
             msg = AISMessage(
                 sender=mmsi,
-                timestamp=ts.to_pydatetime().timestamp(), # Convert to unix
+                timestamp=ts,
                 lat=lat,lon=lon,
                 COG=cog,SOG=sog
             )
             
             if mmsi not in targets:
                 targets[mmsi] = TargetShip(
                     ts = tpos.timestamp if tpos is not None else None,
                     mmsi=mmsi,
-                    ship_type=self._get_ship_type(self.data_loader.static_data,mmsi),
+                    ship_type=self._get_ship_type(self.data_loader.static_data,mmsi,ts),
                     length=self._get_ship_length(self.data_loader.static_data,mmsi),
                     tracks=[[msg]]
                 )
             else:
-                # Split track if change in speed or heading is too large
-                if split.is_split_point(targets[mmsi].tracks[-1][-1],msg):
+                # Split track
+                if self.splitter.is_split_point(targets[mmsi].tracks[-1][-1],msg):
                     targets[mmsi].tracks.append([])
                 v = targets[mmsi]
                 v.tracks[-1].append(msg)
 
         for tgt in targets.values():
             tgt.find_shell() # Find shell (start/end of traj) of target ship
         
@@ -672,31 +690,33 @@
         Return True if the track of the given vessel
         overlaps with the queried timestamp.
         """
         return (track[0].timestamp < tpos.timestamp < track[-1].timestamp)
 
     def _get_ship_type(self, 
                        static_msgs: pd.DataFrame,
-                       mmsi: int) -> list[int]:
+                       mmsi: int,
+                       date: UNIX_TIMESTAMP) -> ShipType:
         """
         Return the ship type of a given MMSI number.
 
         If more than one ship type is found, the first
         one is returned and a warning is logged.
         """
+        st = NeighborhoodTreeSearch._time_filter(static_msgs,date,15)
         st = static_msgs[static_msgs[Msg5Columns.MMSI.value] == mmsi]\
             [Msg5Columns.SHIPTYPE.value].values
         st:np.ndarray = np.unique(st)
         if st.size > 1:
             logger.debug(
-                f"More than one ship type found for MMSI {mmsi}. "
-                f"Found {st}.")
-            return st
-        else:
-            return list(st)
+                f"More than one ship type found for MMSI {mmsi} "
+                f"in a 30 minute window. Found {st}.\n"
+                f"Returning the first one.")
+        if st.size == 0: return ShipType.NOTAVAILABLE
+        return ShipType.from_value(st[0])
 
     def _get_ship_length(self, 
                          static_msgs: pd.DataFrame,
                          mmsi: int) -> list[int]:
         """
         Return the ship length of a given MMSI number.
```

### Comparing `pytsa_ais-2.3.0/pytsa/tsea/targetship.py` & `pytsa_ais-2.3.2/pytsa/tsea/targetship.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/utils.py` & `pytsa_ais-2.3.2/pytsa/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         Msg12318Columns.LAT.value,
         Msg12318Columns.LON.value,
         Msg12318Columns.SPEED.value,
         Msg12318Columns.COURSE.value
     ]
     
     static_columns = [
+        BaseColumns.TIMESTAMP.value,
         Msg5Columns.MMSI.value,
         Msg5Columns.SHIPTYPE.value,
         Msg5Columns.TO_BOW.value,
         Msg5Columns.TO_STERN.value
     ]
     
     def __init__(self, 
@@ -201,33 +202,50 @@
         dyn = sorted(dyn, key=DataLoader._date_transformer)
         stat = sorted(stat, key=DataLoader._date_transformer)
 
         assert all([d.stem == s.stem for d,s in zip(dyn, stat)]),\
             "Dynamic and static messages are not in the same order."
 
         return dyn, stat
+
+    def _date_preprocessor(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Preprocess the date column of `df` to turn it into 
+        pandas datetime objects.
+        """
+        df[BaseColumns.TIMESTAMP.value] = pd.to_datetime(
+            df[BaseColumns.TIMESTAMP.value]
+        )
+        return df
     
     def _dynamic_preprocessor(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Preprocess the dynamic messages.
         """
         # Apply user-defined preprocessor and spatial filter
         df = self.preprocessor(df).query(self.spatial_filter).copy()
         # Convert timestamp to datetime
-        df[BaseColumns.TIMESTAMP.value] = pd.to_datetime(
-                df[BaseColumns.TIMESTAMP.value])
+        df = self._date_preprocessor(df)
         # Drop duplicates form multiple base stations
         df = df.drop_duplicates(
                 subset=[
                     BaseColumns.TIMESTAMP.value,
                     Msg12318Columns.MMSI.value
                 ], keep="first"
             )
         return df
     
+    def _static_preprocessor(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Preprocess the static messages.
+        """
+        # Convert timestamp to datetime
+        df = self._date_preprocessor(df)
+        return df
+    
     def from_raw(self, raw_dyn: Path, raw_stat: Path) -> tuple[pd.DataFrame,pd.DataFrame]:
         """
         Return a DataFrame containing the decoded dynamic and static
         messages.
         
         Decoding the raw AIS messages will result in a 
         DataFrame containing all fields of a NMEA message.
@@ -255,14 +273,15 @@
         self.dynamic_data = pd.DataFrame()
         self.static_data = pd.DataFrame()
         for dyn_path, stat_path in zip(self.sdyn,self.sstat):
             logger.info(f"Loading {stat_path.stem} and {dyn_path.stem}")
             d = pd.read_csv(dyn_path,sep=",",usecols=self.dynamic_columns)
             d = self._dynamic_preprocessor(d)
             s = pd.read_csv(stat_path,sep=",",usecols=self.static_columns)
+            s = self._static_preprocessor(s)
             self.dynamic_data = pd.concat([self.dynamic_data,d])
             self.static_data = pd.concat([self.static_data,s])
         logger.info("Done.")
         
         self.loaded = True
     
     def iterate_chunks(self,
@@ -310,15 +329,16 @@
                 statiter = pd.read_csv(stat_path,**stat_options)
                 
                 for i, (dc,sc) in enumerate(zip(dyniter,statiter)):
                     logger.info(
                         f"Processing chunk {i+1} of file "
                         f"{dyn_path.stem}"
                     )
-                    dc = self._dynamic_preprocessor(dc)            
+                    dc = self._dynamic_preprocessor(dc)
+                    sc = self._static_preprocessor(sc)     
                     yield dc, sc
 
 # DEPRECATED v ================================================================
 class Loader:
     def __init__(self, bb):
         """
         A loader-like context manager
```

### Comparing `pytsa_ais-2.3.0/pytsa/visualization/__init__.py` & `pytsa_ais-2.3.2/pytsa/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/visualization/ecdf.py` & `pytsa_ais-2.3.2/pytsa/visualization/ecdf.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.0/pytsa/visualization/misc.py` & `pytsa_ais-2.3.2/pytsa/visualization/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,67 @@
 have been used throughout the paper.
 
 Some functions, like the heatmap, are not
 used in the paper, but are included here
 anyways, as they might be useful for future
 work.
 """
-import pickle
+import utm
+import geopandas as gpd
+import numpy as np
+
 from pytsa import BoundingBox, TargetShip
 from pytsa.trajectories import inspect
+from pytsa.structs import Track
 from glob import glob
+from pathlib import Path
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-import geopandas as gpd
-import numpy as np
+from scipy.spatial import ConvexHull
 
 from . import plt, PLOT_FOLDER, mpl, COLORWHEEL_MAP
 from ..data.geometry import __path__ as geometry_path
 from ..tsea.targetship import Targets
 
+def _check_duplicate_file_name(filename: Path) -> Path:
+    """
+    Check if a file with the same name
+    already exists in the `PLOT_FOLDER`.
+    
+    If it does, append a number to the filename
+    and return the new filename.
+    
+    Parameters
+    ----------
+    filename : str
+        The filename to be checked.
+        
+    Returns
+    -------
+    str
+        The new filename.
+    """
+    if not (PLOT_FOLDER / filename).exists():
+        return PLOT_FOLDER / filename
+    i = 1
+    while (PLOT_FOLDER / f"{filename}_{i}").exists():
+        i += 1
+    return PLOT_FOLDER / f"{filename}_{i}"
+
+def _cvh_area(track: Track) -> float:
+    """
+    Calculate the area of the convex hull
+    of a track.
+    """
+    res = utm.from_latlon(
+        np.array([p.lat for p in track]),
+        np.array([p.lon for p in track])
+    )
+    points = np.array([res[0],res[1]]).T
+    return ConvexHull(points).area
+
 def plot_coastline(extent: BoundingBox, 
                    ax: plt.Axes = None,
                    save_plot: bool = False,
                    return_figure: bool = False) -> plt.Figure | None:
     """
     Plots the coastline of the search area.
     
@@ -60,45 +101,55 @@
         gdf.plot(ax=ax, color="#007d57", alpha=0.8,linewidth=2)
         
     # Crop the plot to the extent
     ax.set_xlim(extent.LONMIN, extent.LONMAX)
     ax.set_ylim(extent.LATMIN, extent.LATMAX)
     
     if save_plot:
-        plt.savefig(f"{PLOT_FOLDER}/coastline.png", dpi=300)
+        plt.savefig(_check_duplicate_file_name("coastline.png"), dpi=300)
     return None if not return_figure else fig
 
 def binned_heatmap(targets: Targets, 
                    bb: BoundingBox,
-                   npixels: int) -> None:
+                   npixels: int,
+                   title: str = None) -> None:
     """
     Creates a 2D heatmap of messages 
     in the search area with resolution
     `npixels x npixels`.
     
+    The targets do not need to come exactly
+    from the same area as the bounding box,
+    as the heatmap will be cropped to the
+    bounding box.
+    
     Parameters
     ----------
     targets : Targets
-        The targets to be plotted.
+        The target ships to be analyzed.
     bb : BoundingBox
-        The search area.
+        Spatial extent to be plotted on the heatmap.
     npixels : int
         The number of pixels per dimension.
+    title : str
+        The title of the heatmap.
         
     """
     # Create a grid of pixels
     x = np.linspace(bb.LONMIN,bb.LONMAX,npixels)
     y = np.linspace(bb.LATMIN,bb.LATMAX,npixels)
     xx, yy = np.meshgrid(x,y)
     
     # Count the number of messages in each pixel
     counts = np.zeros((npixels,npixels))
     for ship in targets.values():
         for track in ship.tracks:
             for msg in track:
+                if not bb.contains(msg):
+                    continue
                 # Find the closest pixel
                 i = np.argmin(np.abs(x - msg.lon))
                 j = np.argmin(np.abs(y - msg.lat))
                 counts[j,i] += 1
     
     # Plot the heatmap
     fig, ax = plt.subplots(figsize=(10,10))
@@ -137,19 +188,22 @@
     
     cbar.ax.xaxis.set_ticks_position("top")
     cbar.ax.xaxis.set_tick_params(color="black")
     plt.setp(plt.getp(cbar.ax.axes, 'xticklabels'), color="black") 
     
     ax.set_xlabel("Longitude")
     ax.set_ylabel("Latitude")
-    ax.set_title("Heatmap of messages")
+    if title:
+        ax.set_title(title)
+    else:
+        ax.set_title("Heatmap of messages")
     
     
     plt.tight_layout()
-    plt.savefig(f"{PLOT_FOLDER}/heatmap.png",dpi=300)
+    plt.savefig(_check_duplicate_file_name("heatmap.png"),dpi=300)
     
 def plot_trajectories_on_map(ships: dict[int,TargetShip], 
                              extent: BoundingBox) -> None:
     """
     Plot the trajectories of the ships in `ships`
     on a map. The map is cropped to the extent
     of the `BoundingBox`.
@@ -170,15 +224,15 @@
                 alpha=0.5, linewidth=0.3, marker = "x", markersize = 0.5,
                 color = COLORWHEEL_MAP[idx % len(COLORWHEEL_MAP)]
             )
     ax.set_xlabel("Longitude")
     ax.set_ylabel("Latitude")
     plt.title(f"Extracted Trajectories", size = 14)
     plt.tight_layout()
-    plt.savefig(f"aisstats/out/trajectories_map.png",dpi=600)
+    plt.savefig(_check_duplicate_file_name("trajectories_map.png"),dpi=600)
     plt.close()
 
 def pixelmap_average_smoothness(ships: dict[int,TargetShip],
                                 sds: np.ndarray = np.linspace(0,0.1,101),
                                 minlens: np.ndarray = np.linspace(0,100,101)) -> None:
     """
     Figure 14 in the paper. 
@@ -303,51 +357,59 @@
     )
 
     # Axes labels
     ax.set_xlabel(r"$\sigma_{\mathrm{ssd}}$",fontsize=18)
     ax.set_ylabel(r"$n_{msg}$",fontsize=18)
 
     plt.tight_layout()
-    plt.savefig(f"{PLOT_FOLDER}/pixelmap_avg_smoothness.pdf")
+    plt.savefig(_check_duplicate_file_name("pixelmap_avg_smoothness.pdf"))
     
-def ssd_range_comparison(ships: dict[int,TargetShip]) -> None:
+def cvh_range_comparison(ships: dict[int,TargetShip]) -> None:
     """
-    Figure 12 in the paper.
+    Figure 13 in the paper.
     
     Walks through the trajectories of the ships
     in `ships` and plots 100 trajectories for each
-    standard deviation range.
-    The standard deviation range is defined by
-    iterating over the `sds` array with a 
-    rolling window of size 2.
+    convex hull range.
     
     An inset is added to each plot, showing the
     center region of the trajectory, as for some
     ranges, the trajectories are too dense to
     distinguish individual trajectories.
     """
-    
-    sds = np.array([0,0.01,0.02,0.03,0.04,0.05,0.1,0.2,0.3])
+    areas = np.array(
+        [0,1000,5000,10000,20000,50000,100_000,200_000,300_000]
+    )
     
     for ship in ships.values():
-        # Center trajectory
-        # Get mean of lat and lon
+        # We need to calculate the convex hull area
+        # for each track in the ship before
+        # de-meaning the trajectories as the
+        # UTM transform will not work on flipping
+        # coorinate signs.
+        ship.cvhareas = []
         for track in ship.tracks:
+            try:
+                ship.cvhareas.append(_cvh_area(track))
+            except:
+                ship.cvhareas.append(-1)
+            # Center trajectory
+            # Get mean of lat and lon
             latmean = sum(p.lat for p in track) / len(track)
             lonmean = sum(p.lon for p in track) / len(track)
             # Subtract mean from all positions
             for msg in track:
                 msg.lat -= latmean
                 msg.lon -= lonmean
     
     ships: list[TargetShip] = list(ships.values())
             
     # Plot trajectories for different sds
     ncols = 4
-    div,mod = divmod(len(sds)-1,ncols)
+    div,mod = divmod(len(areas)-1,ncols)
     nrows = div + 1 if mod else div
     fig, axs = plt.subplots(nrows=nrows,ncols=ncols,figsize=(4*ncols,8))
     subpos = [0.55,0.55,0.4,0.4]
     axs: dict[int,plt.Axes] # type hint
     niter = 0
     idx = 0
     for row in range(nrows):
@@ -357,33 +419,34 @@
             # Find trajectories whose standard deviation
             # is within the current range
             lons, lats = [], []
             
             np.random.shuffle(ships)
             for ship in ships:
                 # Get standard deviation of lat and lon
-                for track in ship.tracks:
+                for i, track in enumerate(ship.tracks):
                     lo = [p.lon for p in track]
                     la = [p.lat for p in track]
-                    latstd = np.std(la)
-                    lonstd = np.std(lo)
+                    hullarea = ship.cvhareas[i]
+                    if hullarea == -1:
+                        continue
                     # Check if within range
-                    if sds[idx] <= (latstd + lonstd) <= sds[idx+1]:
-                        if trnr == 100:
+                    if areas[idx] <= hullarea <= areas[idx+1]:
+                        if trnr == 50:
                             break
                         trnr += 1
                         lons.append(lo)
                         lats.append(la)
                         
-
-            inset = axs[row,col].inset_axes(subpos)
-            
-            # Add lines for x and y axes
-            inset.axhline(0, color='k', linewidth=0.5)
-            inset.axvline(0, color='k', linewidth=0.5)
+            if row != 1:
+                inset = axs[row,col].inset_axes(subpos)
+                
+                # Add lines for x and y axes
+                inset.axhline(0, color='k', linewidth=0.5)
+                inset.axvline(0, color='k', linewidth=0.5)
             
             axs[row,col].axhline(0, color='k', linewidth=0.5)
             axs[row,col].axvline(0, color='k', linewidth=0.5)
 
             for la, lo in zip(lats,lons):
                 axs[row,col].plot(
                     lo,
@@ -391,43 +454,41 @@
                     alpha=0.5, 
                     marker = "x", 
                     markersize = 0.65, 
                     color = COLORWHEEL_MAP[niter % len(COLORWHEEL_MAP)],
                     linewidth = 0.6
                 )
             
-                # Plot center region in inset
-                inset.plot(    
-                    lo,la,
-                    color = COLORWHEEL_MAP[niter % len(COLORWHEEL_MAP)],
-                    linewidth = 1,
-                    marker = "x",
-                    markersize = 1
-                )
-                
+                if row != 1:
+                    # Plot center region in inset
+                    inset.plot(    
+                        lo,la,
+                        color = COLORWHEEL_MAP[niter % len(COLORWHEEL_MAP)],
+                        linewidth = 1,
+                        marker = "x",
+                        markersize = 1
+                    )
+                    
+                        
+                    # inset.set_axes_locator(ip)
+                    inset.set_xlim(-0.02,0.02)
+                    inset.set_ylim(-0.02,0.02)
                     
-                # inset.set_axes_locator(ip)
-                inset.set_xlim(-0.02,0.02)
-                inset.set_ylim(-0.02,0.02)
-                
                 niter += 1
                 
             axs[row,col].set_xlabel("Longitude")
             axs[row,col].set_ylabel("Latitude")
             axs[row,col].set_title(
-                "$\sigma_{ssd}\in$"
-                f"[{sds[row*ncols+col]:.2f},{sds[row*ncols+col+1]:.2f}]",
+                "$A^{C}\in$"
+                f"[{areas[row*ncols+col]},{areas[row*ncols+col+1]}]$m^2$",
                 fontsize=16
             )
 
             # Set limits
             axs[row,col].set_xlim(-0.25,0.65)
             axs[row,col].set_ylim(-0.25,0.65)
             
             idx += 1
             
     plt.tight_layout()
-    
-    # Pdfs are rather large, so to save space
-    # png can be used instead.
-    plt.savefig(f"aisstats/out/trjitter.pdf")
-    plt.close()
+    plt.savefig(_check_duplicate_file_name("cvhjitter.pdf"))
+    plt.close()
```

### Comparing `pytsa_ais-2.3.0/PKG-INFO` & `pytsa_ais-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytsa-ais
-Version: 2.3.0
+Version: 2.3.2
 Summary: Toolbox for extracting trajectories and monitoring vessels from raw AIS records.
 Author: Niklas Paulig
 Author-email: niklas.paulig@tu-dresden.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -349,22 +349,23 @@
 ## Citation
 
 If you use this module in your research, please consider citing this repository as follows:
 
 ```
 @misc{pytsa2024,
   author = {Paulig, Niklas},
-  title = {{PyTSA}: A Python Module for Extracting Trajectories from Raw AIS Data},
+  title = {{PyTSA}: Python Trajectory Splitting and Assessment Agent for AIS Data},
   year = {2024},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/nikpau/pytsa}},
 }
 ```
 
 ## Appendix
 
 ### Split-point procedure
 
 The split-point procedure takes place in the `pytsa.tsea.split` module. Its main function, `is_split_point()`, will be called on every pair of AIS messages in the dataset. The function returns a boolean value, indicating whether the pair of messages is a split point or not. 
 
 In case you want to adapt the split-point procedure to your dataset, you can use the `pytsa.tsea.split` module as a starting point.
+
```

