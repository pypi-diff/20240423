# Comparing `tmp/geocat.comp-2024.3.0.tar.gz` & `tmp/geocat_comp-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.comp-2024.3.0.tar", last modified: Fri Mar 29 17:31:22 2024, max compression
+gzip compressed data, was "geocat_comp-2024.4.0.tar", last modified: Tue Apr 23 18:46:44 2024, max compression
```

## Comparing `geocat.comp-2024.3.0.tar` & `geocat_comp-2024.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:31:22.718519 geocat.comp-2024.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-29 17:31:22.718519 geocat.comp-2024.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:31:22.714519 geocat.comp-2024.3.0/geocat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:31:22.718519 geocat.comp-2024.3.0/geocat/comp/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/climatologies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/fourier_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/gc_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    26974 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    55129 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/meteorology.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/spherical.py
--rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/geocat/comp/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:31:22.718519 geocat.comp-2024.3.0/geocat.comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 17:31:22.000000 geocat.comp-2024.3.0/geocat.comp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-29 17:31:22.718519 geocat.comp-2024.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-29 17:31:12.000000 geocat.comp-2024.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:44.412534 geocat_comp-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-23 18:46:44.412534 geocat_comp-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:44.404533 geocat_comp-2024.4.0/geocat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:44.408534 geocat_comp-2024.4.0/geocat/comp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24887 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/climatologies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/fourier_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/gc_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26972 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55129 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/meteorology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/geocat/comp/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:44.408534 geocat_comp-2024.4.0/geocat.comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 18:46:44.000000 geocat_comp-2024.4.0/geocat.comp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 18:46:44.412534 geocat_comp-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 18:46:33.000000 geocat_comp-2024.4.0/setup.py
```

### Comparing `geocat.comp-2024.3.0/.pre-commit-config.yaml` & `geocat_comp-2024.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/CODE_OF_CONDUCT.md` & `geocat_comp-2024.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/LICENSE` & `geocat_comp-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/README.md` & `geocat_comp-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/__init__.py` & `geocat_comp-2024.4.0/geocat/comp/__init__.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/climatologies.py` & `geocat_comp-2024.4.0/geocat/comp/climatologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     Returns
     -------
     computed_dset: :class:`xarray.Dataset`, :class:`xarray.DataArray`
         The data with adjusted time coordinate
 
     Notes
     -----
-    See `xarray.cftime_range <http://xarray.pydata.org/en/stable/generated/xarray.cftime_range.html>`__ for accepted values for `freq` and `calendar`.
+    See `xarray.cftime_range <https://docs.xarray.dev/en/stable/generated/xarray.cftime_range.html>`__ for accepted values for `freq` and `calendar`.
     """
 
     time_bounds = xr.cftime_range(start, end, freq=freq, calendar=calendar)
     time_bounds = time_bounds.append(time_bounds[-1:].shift(1, freq=freq))
     time =  xr.DataArray(np.vstack((time_bounds[:-1], time_bounds[1:])).T,
                          dims=[time_dim, 'nbd']) \
         .mean(dim='nbd', keep_attrs=keep_attrs)
```

### Comparing `geocat.comp-2024.3.0/geocat/comp/deprecated.py` & `geocat_comp-2024.4.0/geocat/comp/deprecated.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/fourier_filters.py` & `geocat_comp-2024.4.0/geocat/comp/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/gc_util.py` & `geocat_comp-2024.4.0/geocat/comp/gc_util.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/gradient.py` & `geocat_comp-2024.4.0/geocat/comp/gradient.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/interpolation.py` & `geocat_comp-2024.4.0/geocat/comp/interpolation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+import warnings
 
 import cf_xarray
 import metpy.interpolate
 import numpy as np
 import xarray as xr
 
 supported_types = typing.Union[xr.DataArray, np.ndarray]
@@ -126,21 +127,24 @@
     # This will be in Pa
     return hya * p0 / psfc + hyb
 
 
 def _vertical_remap(func_interpolate, new_levels, xcoords, data, interp_axis=0):
     """Execute the defined interpolation function on data."""
 
-    return func_interpolate(new_levels, xcoords, data, axis=interp_axis)
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore", r"Interpolation point out of data bounds encountered")
+        return func_interpolate(new_levels, xcoords, data, axis=interp_axis)
 
 
 def _temp_extrapolate(data, lev_dim, lev, p_sfc, ps, phi_sfc):
     r"""This helper function extrapolates temperature below ground using the
     ECMWF formulation described in `Vertical Interpolation and Truncation of
-    Model-Coordinate Data <http://dx.doi.org/10.5065/D6HX19NH>`__ by Trenberth,
+    Model-Coordinate Data <https://dx.doi.org/10.5065/D6HX19NH>`__ by Trenberth,
     Berry, & Buja [NCAR/TN-396, 1993]. Specifically equation 16 is used:
 
     .. math::
         T = T_* \left( 1 + \alpha ln \frac{p}{p_s} + \frac{1}{2}\left( \alpha ln \frac{p}{p_s} \right)^2 + \frac{1}{6} \left( \alpha ln \frac{p}{p_s} \right)^3 \right)
 
     Parameters
     ----------
@@ -167,15 +171,15 @@
     result: :class:`xarray.DataArray`
         The extrapolated temperatures at the provided pressure levels.
     """
     R_d = 287.04  # dry air gas constant
     g_inv = 1 / 9.80616  # inverse of gravity
     alpha = 0.0065 * R_d * g_inv
 
-    tstar = data.isel(**{lev_dim: -1}) * (1 + alpha * (ps / p_sfc - 1))
+    tstar = data.isel({lev_dim: -1}, drop=True) * (1 + alpha * (ps / p_sfc - 1))
     hgt = phi_sfc * g_inv
     t0 = tstar + 0.0065 * hgt
     tplat = xr.apply_ufunc(np.minimum, 298, t0, dask='parallelized')
 
     tprime0 = xr.where((2000 <= hgt) & (hgt <= 2500),
                        0.002 * ((2500 - hgt) * t0 + ((hgt - 2000) * tplat)),
                        np.nan)
@@ -187,15 +191,15 @@
 
     return tstar * (1 + alnp + (0.5 * (alnp**2)) + (1 / 6 * (alnp**3)))
 
 
 def _geo_height_extrapolate(t_bot, lev, p_sfc, ps, phi_sfc):
     r"""This helper function extrapolates geopotential height below ground using
     the ECMWF formulation described in `Vertical Interpolation and Truncation
-    of Model-Coordinate Data <http://dx.doi.org/10.5065/D6HX19NH>`__ by
+    of Model-Coordinate Data <https://dx.doi.org/10.5065/D6HX19NH>`__ by
     Trenberth, Berry, & Buja [NCAR/TN-396, 1993]. Specifically equation 15 is
     used:
 
     .. math::
         \Phi = \Phi_s - R_d T_* ln \frac{p}{p_s} \left[ 1 + \frac{1}{2}\alpha ln\frac{p}{p_s} + \frac{1}{6} \left( \alpha ln \frac{p}{p_s} \right)^2 \right]
 
     Parameters
@@ -281,34 +285,32 @@
         The geopotential at the lowest level of the model.
 
     Returns
     -------
     output: :class:`xarray.DataArray`
         A DataArray containing the data after extrapolation.
     """
-    sfc_index = pressure[lev_dim].argmax().data  # index of the model surface
-    p_sfc = pressure.isel(**dict({lev_dim: sfc_index
-                                 }))  # extract pressure at lowest level
 
-    if variable == 'temperature':
-        for lev in new_levels:
-            output.loc[dict(plev=lev)] = xr.where(
-                lev <= p_sfc, output.sel(plev=lev),
-                _temp_extrapolate(data, lev_dim, lev, p_sfc, ps, phi_sfc))
+    sfc_index = pressure[lev_dim].argmax(
+        dim=lev_dim)  # index of the model surface
+    p_sfc = pressure.isel({lev_dim: sfc_index},
+                          drop=True)  # extract pressure at lowest level
 
+    if variable == 'temperature':
+        output = output.where(
+            output.plev <= p_sfc,
+            _temp_extrapolate(data, lev_dim, output.plev, p_sfc, ps, phi_sfc))
     elif variable == 'geopotential':
-        for lev in new_levels:
-            output.loc[dict(plev=lev)] = xr.where(
-                lev <= p_sfc, output.sel(plev=lev),
-                _geo_height_extrapolate(t_bot, lev, p_sfc, ps, phi_sfc))
+        output = output.where(
+            output.plev <= p_sfc,
+            _geo_height_extrapolate(t_bot, output.plev, p_sfc, ps, phi_sfc))
     else:
-        for lev in new_levels:
-            output.loc[dict(plev=lev)] = xr.where(
-                lev <= p_sfc, output.sel(plev=lev),
-                data.isel(**dict({lev_dim: sfc_index})))
+        output = output.where(output.plev <= p_sfc,
+                              data.isel({lev_dim: sfc_index}, drop=True))
+
     return output
 
 
 def interp_hybrid_to_pressure(data: xr.DataArray,
                               ps: xr.DataArray,
                               hyam: xr.DataArray,
                               hybm: xr.DataArray,
@@ -354,15 +356,15 @@
         String that is the name of level dimension in data. Defaults to "lev".
 
     method : str, optional
         String that is the interpolation method; can be either "linear" or "log". Defaults to "linear".
 
     extrapolate : bool, optional
         If True, below ground extrapolation for ``variable`` will be done using
-        an `ECMWF formulation <http://dx.doi.org/10.5065/D6HX19NH>`__. Defaults
+        an `ECMWF formulation <https://dx.doi.org/10.5065/D6HX19NH>`__. Defaults
         to False.
 
     variable : str, optional
         String representing what variable is extrapolated below surface level.
         Temperature extrapolation = "temperature". Geopotential height
         extrapolation = "geopotential". All other variables = "other". If
         "other", the value of ``data`` at the lowest model level will be used
@@ -463,15 +465,15 @@
     if data.chunks is None:
         data_chunk = dict([
             (k, v) for (k, v) in zip(list(data.dims), list(data.shape))
         ])
         data = data.chunk(data_chunk)
 
     # Chunk pressure equal to data's chunks
-    pressure = pressure.chunk(data.chunks)
+    pressure = pressure.chunk(data.chunksizes)
 
     # Output data structure elements
     out_chunks = list(data.chunks)
     out_chunks[interp_axis] = (new_levels.size,)
     out_chunks = tuple(out_chunks)
     # ''' end of boilerplate
```

### Comparing `geocat.comp-2024.3.0/geocat/comp/meteorology.py` & `geocat_comp-2024.4.0/geocat/comp/meteorology.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/spherical.py` & `geocat_comp-2024.4.0/geocat/comp/spherical.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat/comp/stats.py` & `geocat_comp-2024.4.0/geocat/comp/stats.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/geocat.comp.egg-info/SOURCES.txt` & `geocat_comp-2024.4.0/geocat.comp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocat.comp-2024.3.0/setup.cfg` & `geocat_comp-2024.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 license_files = file: LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = >=3.9, <3.13
+python_requires = >=3.10, <3.13
 packages = find_namespace:
 setup_requires = 
 	setuptools_scm
 	setuptools
 	pip
 install_requires = 
 	cf_xarray>=0.3.1
+	numpy<2.0
 	cftime
 	eofs
 	metpy
 	scipy
 	xarray
 	xskillscore
 	packaging
```

