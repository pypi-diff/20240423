# Comparing `tmp/boario-0.5.8.tar.gz` & `tmp/boario-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boario-0.5.8.tar", max compression
+gzip compressed data, was "boario-0.5.9.tar", max compression
```

## Comparing `boario-0.5.8.tar` & `boario-0.5.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-03-07 07:52:20.849427 boario-0.5.8/LICENSE
--rw-r--r--   0        0        0     5510 2024-04-16 12:01:59.867821 boario-0.5.8/README.rst
--rw-r--r--   0        0        0     2082 2024-04-16 12:01:59.867821 boario-0.5.8/boario/__init__.py
--rw-r--r--   0        0        0    58513 2024-04-16 12:01:59.867821 boario-0.5.8/boario/event.py
--rw-r--r--   0        0        0     8076 2024-04-16 12:01:59.867821 boario-0.5.8/boario/extended_models.py
--rw-r--r--   0        0        0    70939 2024-04-16 12:01:59.871821 boario-0.5.8/boario/model_base.py
--rw-r--r--   0        0        0    42008 2024-04-16 12:01:59.871821 boario-0.5.8/boario/simulation.py
--rw-r--r--   0        0        0     3568 2024-04-14 08:59:21.723881 boario-0.5.8/boario/utils/__pycache__/misc.cpython-310.pyc
--rw-r--r--   0        0        0     3977 2024-03-14 07:49:40.040054 boario-0.5.8/boario/utils/__pycache__/recovery_functions.cpython-310.pyc
--rw-r--r--   0        0        0     4894 2024-04-16 12:01:59.871821 boario-0.5.8/boario/utils/misc.py
--rw-r--r--   0        0        0     4066 2024-03-07 07:52:20.849427 boario-0.5.8/boario/utils/recovery_functions.py
--rw-r--r--   0        0        0     2474 2024-04-16 12:01:59.871821 boario-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 boario-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-07 07:52:20.849427 boario-0.5.9/LICENSE
+-rw-r--r--   0        0        0     5510 2024-04-16 12:01:59.867821 boario-0.5.9/README.rst
+-rw-r--r--   0        0        0     2082 2024-04-16 12:01:59.867821 boario-0.5.9/boario/__init__.py
+-rw-r--r--   0        0        0    59491 2024-04-23 12:26:09.742204 boario-0.5.9/boario/event.py
+-rw-r--r--   0        0        0     8076 2024-04-22 14:36:39.385312 boario-0.5.9/boario/extended_models.py
+-rw-r--r--   0        0        0    70939 2024-04-22 14:36:40.961340 boario-0.5.9/boario/model_base.py
+-rw-r--r--   0        0        0    42008 2024-04-16 12:01:59.871821 boario-0.5.9/boario/simulation.py
+-rw-r--r--   0        0        0     3568 2024-04-16 15:04:40.077013 boario-0.5.9/boario/utils/__pycache__/misc.cpython-310.pyc
+-rw-r--r--   0        0        0     3977 2024-03-14 07:49:40.040054 boario-0.5.9/boario/utils/__pycache__/recovery_functions.cpython-310.pyc
+-rw-r--r--   0        0        0      736 2024-04-22 13:05:08.110181 boario-0.5.9/boario/utils/__pycache__/singleton.cpython-310.pyc
+-rw-r--r--   0        0        0     4894 2024-04-16 12:01:59.871821 boario-0.5.9/boario/utils/misc.py
+-rw-r--r--   0        0        0     4066 2024-03-07 07:52:20.849427 boario-0.5.9/boario/utils/recovery_functions.py
+-rw-r--r--   0        0        0     2486 2024-04-23 12:26:09.746204 boario-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 boario-0.5.9/PKG-INFO
```

### Comparing `boario-0.5.8/LICENSE` & `boario-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/README.rst` & `boario-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/__init__.py` & `boario-0.5.9/boario/__init__.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/event.py` & `boario-0.5.9/boario/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
+
 
 from boario import logger
 from boario.utils.recovery_functions import (
     concave_recovery,
     convexe_recovery,
     convexe_recovery_scaled,
     linear_recovery,
@@ -186,40 +188,41 @@
     def _instantiate(
         cls,
         impact: pd.Series,
         *,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
+        **_,
     ):
         return cls(impact=impact, occurrence=occurrence, duration=duration, name=name)
 
     @classmethod
     def from_series(
         cls,
         impact: pd.Series,
         *,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
-        **kwarg,
+        **kwargs,
     ) -> Event:
         """Create an event for an impact given as a pd.Series.
 
         Parameters
         ----------
         impact : pd.Series
             A pd.Series defining the impact per (region, sector)
         occurrence : int
             The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
         duration : int
             The duration of the event (entire impact applied during this number of steps). Defaults to 1.
         name : Optional[str]
             A possible name for the event, for convenience. Defaults to None.
-        **kwarg :
+        **kwargs :
             Keyword arguments keyword arguments to pass to the instantiating method
         (depends on the type of event).
 
         Returns
         -------
         Event
             An Event object or one of its subclass
@@ -256,40 +259,40 @@
             logger.debug(f"Impact has negative values:\n{impact}\n{impact[impact<0]}")
             raise ValueError("Impact has negative values")
         return cls._instantiate(
             impact=impact,
             occurrence=occurrence,
             duration=duration,
             name=name,
-            **kwarg,
+            **kwargs,
         )
 
     @classmethod
     def from_dataframe(
         cls,
         impact: pd.DataFrame,
         *,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
-        **kwarg,
+        **kwargs,
     ) -> Event:
         """Convenience function for DataFrames. See :meth:`~boario.event.Event.from_series`. This constructor only apply ``.squeeze()`` to the given DataFrame.
 
         Parameters
         ----------
         impact : pd.DataFrame
            A pd.DataFrame defining the impact per (region, sector)
         occurrence : int
             The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
         duration : int
             The duration of the event (entire impact applied during this number of steps). Defaults to 1.
         name : Optional[str]
             A possible name for the event, for convenience. Defaults to None.
-        **kwarg :
+        **kwargs :
             Keyword arguments
             Other keyword arguments to pass to the instantiate method (depends on the type of event)
 
         Raises
         ------
         ValueError
             If impact cannot be squeezed to a Series
@@ -304,15 +307,15 @@
             raise ValueError("Could not squeeze impact dataframe to a serie.")
 
         return cls.from_series(
             impact=impact,
             occurrence=occurrence,
             duration=duration,
             name=name,
-            **kwarg,
+            **kwargs,
         )
 
     @classmethod
     def distribute_impact_by_gva(cls, impact_vec: pd.Series) -> pd.Series:
         """Distribute a vector of impact by the GVA of affected industries.
 
         Each values of the given impact are mutliplied by the share of the GVA
@@ -361,15 +364,15 @@
         *,
         industries: IndustriesList,
         impact_industries_distrib: Optional[npt.ArrayLike] = None,
         gva_distrib: Optional[bool] = False,
         occurrence: Optional[int] = 1,
         duration: Optional[int] = 1,
         name: Optional[str] = None,
-        **kwarg,
+        **kwargs,
     ) -> Event:
         """Creates an Event from a scalar and a list of industries affected.
 
         The scalar impact is distributed evenly by default. Otherwise it can
         be distributed proportionnaly to the GVA of affected industries, or to
         a custom distribution.
 
@@ -386,15 +389,15 @@
             A boolean stating if the impact should be distributed proportionnaly to GVA. Defaults to False.
         occurrence : Optional[int]
             The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
         duration : Optional[int]
             The duration of the event (entire impact applied during this number of steps). Defaults to 1.
         name : Optional[str]
             A possible name for the event, for convenience. Defaults to None.
-        **kwarg :
+        **kwargs :
             Keyword arguments
             Other keyword arguments to pass to the instantiate method (depends on the type of event)
 
         Raises
         ------
         ValueError
             Raised if Impact is null, if len(industries) < 1 or if the sum of impact_industries_distrib differs from 1.0.
@@ -431,30 +434,30 @@
             impact_vec = cls.distribute_impact_equally(impact_vec)
 
         return cls.from_series(
             impact=impact_vec,
             occurrence=occurrence,
             duration=duration,
             name=name,
-            **kwarg,
+            **kwargs,
         )
 
     @classmethod
     def from_scalar_regions_sectors(
         cls,
         impact: ScalarImpact,
         *,
         regions: RegionsList,
         sectors: SectorsList,
         impact_regional_distrib: Optional[npt.ArrayLike] = None,
         impact_sectoral_distrib: Optional[Union[str, npt.ArrayLike]] = None,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
-        **kwarg,
+        **kwargs,
     ) -> Event:
         """Creates an Event from a scalar, a list of regions and a list of sectors affected.
 
         Parameters
         ----------
         impact : ScalarImpact
             The scalar impact.
@@ -473,15 +476,15 @@
 
         occurrence : int, optional
             The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
         duration : int, optional
             The duration of the event (entire impact applied during this number of steps). Defaults to 1.
         name : Optional[str], optional
             A possible name for the event, for convenience. Defaults to None.
-        **kwarg :
+        **kwargs :
             Keyword arguments
             Other keyword arguments to pass to the instantiate method (depends on the type of event)
 
         Raises
         ------
         ValueError
             Raise if Impact is null, if len(regions) or len(sectors) < 1,
@@ -588,15 +591,15 @@
         impact_vec *= industries_distrib
 
         return cls.from_series(
             impact=impact_vec,
             occurrence=occurrence,
             duration=duration,
             name=name,
-            **kwarg,
+            **kwargs,
         )
 
     @property
     def impact_df(self) -> pd.Series:
         r"""A pandas Series with all possible industries as index, holding the impact vector of the event. The impact is defined for each sectors in each region."""
         return self._impact_df
 
@@ -843,14 +846,15 @@
         impact: pd.Series,
         *,
         recovery_time: int = 1,
         recovery_function: str = "linear",
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
+        **_,
     ):
         return cls(
             impact=impact,
             occurrence=occurrence,
             duration=duration,
             name=name,
             recovery_time=recovery_time,
@@ -1174,14 +1178,15 @@
         self._rebuildable = False
         self.rebuild_tau = rebuild_tau
         self.rebuilding_sectors = rebuilding_sectors
         self.rebuilding_factor = rebuilding_factor
 
         industrial_rebuilding_demand = np.zeros(shape=self.z_shape)
         tmp = np.zeros(self.z_shape, dtype="float")
+
         mask = np.ix_(
             np.union1d(
                 self._rebuilding_industries_RoW_idx, self._rebuilding_industries_idx
             ),
             self._aff_industries_idx,
         )
         industrial_rebuilding_demand = np.outer(
@@ -1232,28 +1237,43 @@
         occurrence: int = 1,
         duration: int = 1,
         name: str | None = None,
         event_monetary_factor: Optional[int] = None,
         rebuild_tau: int,
         rebuilding_sectors: dict[str, float] | pd.Series,
         rebuilding_factor: float = 1.0,
+        **_,
     ):
         return cls(
             impact=impact,
             households_impact=households_impact,
             occurrence=occurrence,
             duration=duration,
             name=name,
             event_monetary_factor=event_monetary_factor,
             rebuild_tau=rebuild_tau,
             rebuilding_sectors=rebuilding_sectors,
             rebuilding_factor=rebuilding_factor,
         )
 
     @property
+    def rebuild_tau(self) -> int:
+        r"""The characteristic time for rebuilding."""
+        return self._rebuild_tau
+
+    @rebuild_tau.setter
+    def rebuild_tau(self, value: int):
+        if not isinstance(value, int) or value < 1:
+            raise ValueError(
+                f"``rebuild_tau`` should be a strictly positive integer. Value given is {value}."
+            )
+        else:
+            self._rebuild_tau = value
+
+    @property
     def rebuilding_sectors(self) -> pd.Index:
         r"""The (optional) array of rebuilding sectors"""
         return self._rebuilding_sectors
 
     @property
     def rebuilding_sectors_idx(self) -> npt.NDArray:
         r"""The (optional) array of indexes of the rebuilding sectors (in lexicographic order)"""
@@ -1266,15 +1286,20 @@
 
     @rebuilding_sectors.setter
     def rebuilding_sectors(self, value: dict[str, float] | pd.Series):
         if isinstance(value, dict):
             reb_sectors = pd.Series(value)
         else:
             reb_sectors = value
-        assert np.isclose(reb_sectors.sum(), 1.0)
+        if not is_numeric_dtype(reb_sectors):
+            raise TypeError(
+                "Rebuilding sectors should be given as ``dict[str, float] | pd.Series``."
+            )
+        if not np.isclose(reb_sectors.sum(), 1.0):
+            raise ValueError(f"Reconstruction shares among sectors do not sum up to 1.")
         impossible_sectors = np.setdiff1d(reb_sectors.index, self.possible_sectors)
         if impossible_sectors.size > 0:
             raise ValueError(
                 "These sectors are not in the model : {}".format(impossible_sectors)
             )
         else:
             self._rebuilding_sectors = reb_sectors.index
@@ -1284,33 +1309,36 @@
 
             self._rebuilding_sectors_shares = np.zeros(self.x_shape)
             self._rebuilding_industries_idx = np.array(
                 [
                     np.size(self.possible_sectors) * ri + si
                     for ri in self._aff_regions_idx
                     for si in self._rebuilding_sectors_idx
-                ]
+                ],
+                dtype="int64",
             )
             self._rebuilding_industries_RoW_idx = np.array(
                 [
                     np.size(self.possible_sectors) * ri + si
                     for ri in range(np.size(self.possible_regions))
                     if ri not in self._aff_regions_idx
                     for si in self._rebuilding_sectors_idx
-                ]
+                ],
+                dtype="int64",
             )
             self._rebuilding_sectors_shares[self._rebuilding_industries_idx] = np.tile(
                 np.array(reb_sectors.values), np.size(self.aff_regions)
             )
-            self._rebuilding_sectors_shares[self._rebuilding_industries_RoW_idx] = (
-                np.tile(
-                    np.array(reb_sectors.values),
-                    (np.size(self.possible_regions) - np.size(self.aff_regions)),
+            if self._rebuilding_industries_RoW_idx.size != 0:
+                self._rebuilding_sectors_shares[self._rebuilding_industries_RoW_idx] = (
+                    np.tile(
+                        np.array(reb_sectors.values),
+                        (np.size(self.possible_regions) - np.size(self.aff_regions)),
+                    )
                 )
-            )
 
     @property
     def rebuilding_demand_house(self) -> npt.NDArray:
         r"""The optional array of rebuilding demand from households"""
         return self._rebuilding_demand_house
 
     @rebuilding_demand_house.setter
@@ -1411,14 +1439,15 @@
         households_impact: Optional[Impact] = None,
         occurrence: int = 1,
         duration: int = 1,
         name: str | None = None,
         event_monetary_factor: Optional[int] = None,
         recovery_time: int,
         recovery_function: str = "linear",
+        **_,
     ):
         return cls(
             impact=impact,
             households_impact=households_impact,
             occurrence=occurrence,
             duration=duration,
             name=name,
```

### Comparing `boario-0.5.8/boario/extended_models.py` & `boario-0.5.9/boario/extended_models.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/model_base.py` & `boario-0.5.9/boario/model_base.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/simulation.py` & `boario-0.5.9/boario/simulation.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/utils/__pycache__/misc.cpython-310.pyc` & `boario-0.5.9/boario/utils/__pycache__/misc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 14 08:59:20 2024 UTC, .py size: 4894 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e89a 1b66 1e13 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 b768 1e66 1e13 0000  o........h.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c05 5a05 6400 6401 6c06  ..d.d.l.Z.d.d.l.
 00000060: 5a06 4700 6403 6404 8400 6404 6505 6a07  Z.G.d.d...d.e.j.
 00000070: 8303 5a08 4700 6405 6406 8400 6406 6500  ..Z.G.d.d...d.e.
```

### Comparing `boario-0.5.8/boario/utils/__pycache__/recovery_functions.cpython-310.pyc` & `boario-0.5.9/boario/utils/__pycache__/recovery_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/utils/misc.py` & `boario-0.5.9/boario/utils/misc.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/boario/utils/recovery_functions.py` & `boario-0.5.9/boario/utils/recovery_functions.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.8/pyproject.toml` & `boario-0.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "boario"
-version = "0.5.8"
+version = "0.5.9"
 description = "BoARIO : The Adaptative Regional Input Output model in python."
 authors = ["Samuel Juhel <pro@sjuhel.org>"]
 license = "GNU General Public License v3 or later (GPLv3+)"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python=">=3.9,<4.0"
 coloredlogs = "^15.0.1"
 country-converter = "^1.0.0"
 dask = ">=2023"
-numpy = "<1.24"
+numpy = "<1.27"
 odfpy = "^1.4.1"
 pandas = ">=1.5"
 progressbar2 = "^4.2.0"
 pyarrow = ">=11"
 pymrio = ">=0.4"
 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = ">=7.3.1,<9.0.0"
 pygit2 = "^1.12.1"
 ipykernel = "^6.23.0"
 black = ">=23.3,<25.0"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-autoapi = ">=2.1,<4.0"
 sphinx-automodapi = "^0.15.0"
 sphinx-copybutton = "^0.5.2"
 pydata-sphinx-theme = ">=0.13.3,<0.16.0"
 nbsphinx = "^0.9.2"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 isort = "^5.13.2"
 flake8 = "^7.0.0"
 flake8-pyproject = "^1.2.3"
 safety = "^3.0.1"
 pydoclint = "^0.4.1"
 autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^2.0.0"
```

### Comparing `boario-0.5.8/PKG-INFO` & `boario-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: boario
-Version: 0.5.8
+Version: 0.5.9
 Summary: BoARIO : The Adaptative Regional Input Output model in python.
 License: GNU General Public License v3 or later (GPLv3+)
 Author: Samuel Juhel
 Author-email: pro@sjuhel.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: country-converter (>=1.0.0,<2.0.0)
 Requires-Dist: dask (>=2023)
-Requires-Dist: numpy (<1.24)
+Requires-Dist: numpy (<1.27)
 Requires-Dist: odfpy (>=1.4.1,<2.0.0)
 Requires-Dist: pandas (>=1.5)
 Requires-Dist: progressbar2 (>=4.2.0,<5.0.0)
 Requires-Dist: pyarrow (>=11)
 Requires-Dist: pymrio (>=0.4)
 Description-Content-Type: text/x-rst
```

