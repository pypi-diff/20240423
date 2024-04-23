# Comparing `tmp/qsharp-1.3.6.dev0-cp37-abi3-win_arm64.whl.zip` & `tmp/qsharp-1.4.0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1596621 bytes, number of entries: 14
--rw-r--r--  4.6 unx     2098 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3090 b- defN 24-Apr-17 19:23 qsharp/.data/qsharp_codemirror.js
--rw-r--r--  4.6 unx    38836 b- defN 24-Apr-17 19:23 qsharp/estimator/_estimator.py
--rw-r--r--  4.6 unx      859 b- defN 24-Apr-17 19:23 qsharp/estimator/__init__.py
--rw-r--r--  4.6 unx     1706 b- defN 24-Apr-17 19:23 qsharp/utils/_utils.py
--rw-r--r--  4.6 unx      146 b- defN 24-Apr-17 19:23 qsharp/utils/__init__.py
--rw-r--r--  4.6 unx      864 b- defN 24-Apr-17 19:23 qsharp/_fs.py
--rw-r--r--  4.6 unx     1848 b- defN 24-Apr-17 19:23 qsharp/_ipython.py
--rw-r--r--  4.6 unx     6375 b- defN 24-Apr-17 19:23 qsharp/_native.pyi
--rw-r--r--  4.6 unx    11512 b- defN 24-Apr-17 19:23 qsharp/_qsharp.py
--rw-r--r--  4.6 unx      902 b- defN 24-Apr-17 19:23 qsharp/__init__.py
--rwxr-xr-x  4.6 unx  3882496 b- defN 24-Apr-17 19:23 qsharp/_native.pyd
--rw-r--r--  4.6 unx     1085 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/RECORD
-14 files, 3951911 bytes uncompressed, 1594851 bytes compressed:  59.7%
+Zip file size: 1603175 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     2093 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3090 b- defN 24-Apr-23 18:12 qsharp/.data/qsharp_codemirror.js
+-rw-r--r--  4.6 unx    38836 b- defN 24-Apr-23 18:12 qsharp/estimator/_estimator.py
+-rw-r--r--  4.6 unx      859 b- defN 24-Apr-23 18:12 qsharp/estimator/__init__.py
+-rw-r--r--  4.6 unx     1706 b- defN 24-Apr-23 18:12 qsharp/utils/_utils.py
+-rw-r--r--  4.6 unx      146 b- defN 24-Apr-23 18:12 qsharp/utils/__init__.py
+-rw-r--r--  4.6 unx      864 b- defN 24-Apr-23 18:12 qsharp/_fs.py
+-rw-r--r--  4.6 unx     1848 b- defN 24-Apr-23 18:12 qsharp/_ipython.py
+-rw-r--r--  4.6 unx     6375 b- defN 24-Apr-23 18:12 qsharp/_native.pyi
+-rw-r--r--  4.6 unx    13210 b- defN 24-Apr-23 18:12 qsharp/_qsharp.py
+-rw-r--r--  4.6 unx      902 b- defN 24-Apr-23 18:12 qsharp/__init__.py
+-rwxr-xr-x  4.6 unx  3898880 b- defN 24-Apr-23 18:12 qsharp/_native.pyd
+-rw-r--r--  4.6 unx     1070 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/RECORD
+14 files, 3969973 bytes uncompressed, 1601435 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: qsharp-1.3.6.dev0.dist-info/METADATA
+Filename: qsharp-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp-1.3.6.dev0.dist-info/WHEEL
+Filename: qsharp-1.4.0.dist-info/WHEEL
 Comment: 
 
 Filename: qsharp/.data/qsharp_codemirror.js
 Comment: 
 
 Filename: qsharp/estimator/_estimator.py
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: qsharp/__init__.py
 Comment: 
 
 Filename: qsharp/_native.pyd
 Comment: 
 
-Filename: qsharp-1.3.6.dev0.dist-info/RECORD
+Filename: qsharp-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp/_qsharp.py

```diff
@@ -6,15 +6,15 @@
     TargetProfile,
     StateDumpData,
     QSharpError,
     Output,
     Circuit,
 )
 from warnings import warn
-from typing import Any, Callable, Dict, Optional, TypedDict, Union, List
+from typing import Any, Callable, Dict, Optional, Tuple, TypedDict, Union, List
 from .estimator._estimator import EstimatorResult, EstimatorParams
 import json
 
 _interpreter = None
 
 
 class Config:
@@ -345,14 +345,47 @@
 
     def __str__(self) -> str:
         return self.__data.__str__()
 
     def _repr_html_(self) -> str:
         return self.__data._repr_html_()
 
+    def check_eq(
+        self, state: Union[Dict[int, complex], List[complex]], tolerance: float = 1e-10
+    ) -> bool:
+        """
+        Checks if the state dump is equal to the given state. This is not mathematical equality,
+        as the check ignores global phase.
+
+        :param state: The state to check against, provided either as a dictionary of state indices to complex amplitudes,
+            or as a list of real amplitudes.
+        :param tolerance: The tolerance for the check. Defaults to 1e-10.
+        """
+        phase = None
+        # Convert a dense list of real amplitudes to a dictionary of state indices to complex amplitudes
+        if isinstance(state, list):
+            state = {i: state[i] for i in range(len(state))}
+        # Filter out zero states from the state dump and the given state based on tolerance
+        state = {k: v for k, v in state.items() if abs(v) > tolerance}
+        inner_state = {k: v for k, v in self.__inner.items() if abs(v) > tolerance}
+        if len(state) != len(inner_state):
+            return False
+        for key in state:
+            if key not in inner_state:
+                return False
+            if phase is None:
+                # Calculate the phase based on the first state pair encountered.
+                # Every pair of states after this must have the same phase for the states to be equivalent.
+                phase = inner_state[key] / state[key]
+            elif abs(phase - inner_state[key] / state[key]) > tolerance:
+                # This pair of states does not have the same phase,
+                # within tolerance, so the equivalence check fails.
+                return False
+        return True
+
 
 def dump_machine() -> StateDump:
     """
     Returns the sparse state vector of the simulator as a StateDump object.
 
     :returns: The state of the simulator.
     """
```

## Comparing `qsharp-1.3.6.dev0.dist-info/METADATA` & `qsharp-1.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp
-Version: 1.3.6.dev0
+Version: 1.4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `qsharp-1.3.6.dev0.dist-info/RECORD` & `qsharp-1.4.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-qsharp-1.3.6.dev0.dist-info/METADATA,sha256=ds9Xe3pp7phe62a97KpEmjT4P_DItAxuDbA0BBo5Cj8,2098
-qsharp-1.3.6.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
+qsharp-1.4.0.dist-info/METADATA,sha256=ZEpIxSR52tfMtiXNU1HDRJnTlr82FC71QTi2AJ8VFs0,2093
+qsharp-1.4.0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
 qsharp/.data/qsharp_codemirror.js,sha256=72E3fTxGxfBe_bBhPD5-8ul_S61MLVA_JmMJwOXgmhc,3090
 qsharp/estimator/_estimator.py,sha256=LMTJg2xPwhvswlc0ts0zsjRPd82mF5KzYgmHyFFl2PE,38836
 qsharp/estimator/__init__.py,sha256=JK6oDnNX_rgsPnfyFsK0yxMBRinmW8jlc8183BydxXA,859
 qsharp/utils/_utils.py,sha256=s3ausLf4wp08rgRDrcdzSXOYPRQ63isX0umCA9MIq7M,1706
 qsharp/utils/__init__.py,sha256=ejBPCXRttEGKCDehjldx8SryqQfNHXsgsRFK5O-zRU8,146
 qsharp/_fs.py,sha256=RGhwMRUwfxGoPVEPaP39FxyRcPeZoyhB0kb4MwzxE54,864
 qsharp/_ipython.py,sha256=x8J7HatTw15xTg9Ppd-yRmhNz9eY8cBAhruRiHo46bQ,1848
 qsharp/_native.pyi,sha256=w0bBah7mtOnoLcchXMfMoH6PJaf1Bm0lmSJe8574s4U,6375
-qsharp/_qsharp.py,sha256=h3zPZ91r85sTvJJU7y-L9HNJeQZTzO3MVI4uzfrCWb0,11512
+qsharp/_qsharp.py,sha256=JcD5z7mFKtvhZ9cX8xUWrGd268tEmyTHJGSWq5gclOs,13210
 qsharp/__init__.py,sha256=-KmJgZV8ZRqWSIOENAhyE39vYF5eZ_p4W04XZ29YKfs,902
-qsharp/_native.pyd,sha256=0GpYp8Ct26jaz7sv40allwuwe_FpeD9M5e5g8BJtM5s,3882496
-qsharp-1.3.6.dev0.dist-info/RECORD,,
+qsharp/_native.pyd,sha256=9zxfJEZMxSv1YGvpXDGBsIq8s2RNkfGBdhhOApn_EG8,3898880
+qsharp-1.4.0.dist-info/RECORD,,
```

