# Comparing `tmp/GRSdriver-1.0.3.tar.gz` & `tmp/grsdriver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GRSdriver-1.0.3.tar", last modified: Thu Apr 11 10:23:55 2024, max compression
+gzip compressed data, was "grsdriver-1.0.4.tar", last modified: Tue Apr 23 10:11:30 2024, max compression
```

## Comparing `GRSdriver-1.0.3.tar` & `grsdriver-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-11 10:23:55.728623 GRSdriver-1.0.3/
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-11 10:23:55.720623 GRSdriver-1.0.3/GRSdriver/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      195 2024-04-11 10:23:13.000000 GRSdriver-1.0.3/GRSdriver/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    21608 2024-04-11 10:21:28.000000 GRSdriver-1.0.3/GRSdriver/driver_S2_SAFE.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     7712 2024-04-11 10:21:28.000000 GRSdriver-1.0.3/GRSdriver/driver_landsat_col2.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-11 10:23:55.720623 GRSdriver-1.0.3/GRSdriver/rsr/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/__init__.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-11 10:23:55.724623 GRSdriver-1.0.3/GRSdriver/rsr/data/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   174535 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    81844 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/L4_TM_RSR.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    80969 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/L5_TM_RSR.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    87561 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/L7_RSR.xlsx
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   655775 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)   882434 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/rsr_landsat_8_oli.nc
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/data/rsr_landsat_9_oli.nc
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     2754 2024-02-12 15:04:09.000000 GRSdriver-1.0.3/GRSdriver/rsr/landsat_formatting.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1889 2024-04-10 17:05:28.000000 GRSdriver-1.0.3/GRSdriver/run.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     8096 2024-04-10 11:19:05.000000 GRSdriver-1.0.3/GRSdriver/visual.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-11 10:23:55.724623 GRSdriver-1.0.3/GRSdriver.egg-info/
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15472 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      773 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       50 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/entry_points.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       44 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/requires.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       35 2024-04-11 10:23:55.000000 GRSdriver-1.0.3/GRSdriver.egg-info/top_level.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 GRSdriver-1.0.3/LICENSE
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15472 2024-04-11 10:23:55.724623 GRSdriver-1.0.3/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1751 2024-04-11 10:23:13.000000 GRSdriver-1.0.3/README.md
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1238 2024-04-11 10:23:51.000000 GRSdriver-1.0.3/pyproject.toml
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-11 10:23:55.728623 GRSdriver-1.0.3/setup.cfg
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-23 10:11:30.145934 grsdriver-1.0.4/
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-23 10:11:30.133931 grsdriver-1.0.4/GRSdriver/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)      460 2024-04-18 11:44:51.000000 grsdriver-1.0.4/GRSdriver/__init__.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    21608 2024-04-11 10:21:28.000000 grsdriver-1.0.4/GRSdriver/driver_S2_SAFE.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     7796 2024-04-12 11:17:50.000000 grsdriver-1.0.4/GRSdriver/driver_landsat_col2.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-23 10:11:30.133931 grsdriver-1.0.4/GRSdriver/rsr/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/__init__.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-23 10:11:30.141933 grsdriver-1.0.4/GRSdriver/rsr/data/
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    81844 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L4_TM_RSR.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    80969 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L5_TM_RSR.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    87561 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L7_RSR.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   174535 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L8_Ball_BA_RSR.v1.2.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    34723 2024-04-12 11:14:43.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L8_TIRS_Relative_Spectral_Responses.BA_.v1.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   655775 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    34274 2024-04-12 09:45:06.000000 grsdriver-1.0.4/GRSdriver/rsr/data/L9_TIRS2_Relative_Spectral_Responses.BA.v1.0.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)   882434 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 grsdriver-1.0.4/GRSdriver/rsr/data/__init__.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-04-12 11:15:04.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_8_oli.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   298643 2024-04-12 11:15:14.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_8_oli_tirs.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    33366 2024-04-12 11:15:14.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_8_tirs.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-04-12 10:33:43.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_9_oli.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   298651 2024-04-12 10:39:43.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_9_oli_tirs.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    33366 2024-04-12 10:33:43.000000 grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_9_tirs.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     6184 2024-04-12 11:08:32.000000 grsdriver-1.0.4/GRSdriver/rsr/landsat_formatting.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     2743 2024-04-18 12:22:24.000000 grsdriver-1.0.4/GRSdriver/run.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     7474 2024-04-18 09:28:50.000000 grsdriver-1.0.4/GRSdriver/visual.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-23 10:11:30.141933 grsdriver-1.0.4/GRSdriver.egg-info/
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15472 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1084 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       50 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/entry_points.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       44 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/requires.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       35 2024-04-23 10:11:30.000000 grsdriver-1.0.4/GRSdriver.egg-info/top_level.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 grsdriver-1.0.4/LICENSE
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15472 2024-04-23 10:11:30.145934 grsdriver-1.0.4/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1751 2024-04-11 10:23:13.000000 grsdriver-1.0.4/README.md
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1238 2024-04-12 11:19:10.000000 grsdriver-1.0.4/pyproject.toml
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-23 10:11:30.145934 grsdriver-1.0.4/setup.cfg
```

### Comparing `GRSdriver-1.0.3/GRSdriver/driver_S2_SAFE.py` & `grsdriver-1.0.4/GRSdriver/driver_S2_SAFE.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/driver_landsat_col2.py` & `grsdriver-1.0.4/GRSdriver/driver_landsat_col2.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 from eoreader.bands import RAW_CLOUDS
 from eoreader.keywords import TO_REFLECTANCE
 
 from . import __package__
 
 opj = os.path.join
 
-BAND_NAMES = np.array(['B01', 'B02', 'B03', 'B08', 'B04', 'B05', 'B09', 'B06', 'B07'])
+BAND_NAMES = np.array(['B01', 'B02', 'B03', 'B08', 'B04', 'B05', 'B09', 'B06', 'B07','B08','B09'])
 BAND_NAMES_EOREADER = np.array(['CA', 'BLUE', 'GREEN', 'PAN', 'RED', 'NIR',
-                                'SWIR_CIRRUS', 'SWIR_1', 'SWIR_2'])
+                                'SWIR_CIRRUS', 'SWIR_1', 'SWIR_2','TIR_1','TIR_2'])
 
 BAND_ID = [b.replace('B', '') for b in BAND_NAMES]
-NATIVE_RESOLUTION = [30, 30, 30, 15, 30, 30, 30, 30, 30]
-WAVELENGTH = np.array([443, 490, 560, 590, 665, 865, 1370, 1610, 2190])
-BAND_WIDTH = [25, 60, 60, 173, 33, 28, 21, 95, 287]
+NATIVE_RESOLUTION = [30, 30, 30, 15, 30, 30, 30, 30, 30,100,100]
+WAVELENGTH = np.array([443, 490, 560, 590, 665, 865, 1370, 1610, 2190,11000,12000])
+BAND_WIDTH = [25, 60, 60, 173, 33, 28, 21, 95, 287,590,1010]
 
 INFO = pd.DataFrame({'bandId': range(len(BAND_NAMES)),
                      'ESA': BAND_NAMES,
                      'EOREADER': BAND_NAMES_EOREADER,
                      'Wavelength (nm)': WAVELENGTH,
                      'Band width (nm)': BAND_WIDTH,
                      'Resolution (m)': NATIVE_RESOLUTION}).set_index('bandId').T
@@ -91,17 +91,17 @@
         self.transform = Affine(resolution, 0., minx, 0., -resolution, maxy)
 
         # --------------------------------
         # Spectral Response Functions
         # --------------------------------
 
         if '8' in self.satellite:
-            srf_file = files(__package__+'.rsr.data').joinpath('rsr_landsat_8_oli.nc')
+            srf_file = files(__package__+'.rsr.data').joinpath('rsr_landsat_8_oli_tirs.nc')
         elif '9' in self.satellite:
-            srf_file = files(__package__+'.rsr.data').joinpath('rsr_landsat_9_oli.nc')
+            srf_file = files(__package__+'.rsr.data').joinpath('rsr_landsat_9_oli_tirs.nc')
         else:
             print('Problem to fetch spectral response functions for ', self.satellite)
 
         self.SRFs = xr.open_dataset(srf_file)
 
     def load_product(self, add_time=True, **kwargs):
 
@@ -146,15 +146,15 @@
         self.prod = bands.assign_coords(wl=('bands', self.INFO.loc['Wavelength (nm)'])). \
             swap_dims({'bands': 'wl'}).drop({'band', 'bands', 'variable'})
         self.prod = self.prod.assign_coords(bandID=('wl', self.INFO.loc['ESA'].values))
         self.prod = self.prod.to_dataset(name='bands', promote_attrs=True)
         self.prod.attrs['wl_to_process'] = WAVELENGTH[self.band_tbp_idx]
 
         # add spectral response function
-        self.prod = xr.merge([self.prod, self.SRFs.sel(wl=self.prod.wl.values)]).drop_vars('bandID')
+        self.prod = xr.merge([self.prod, self.SRFs.sel(wl=self.prod.wl.values,method="nearest")]).drop_vars('bandID')
 
         # compute central wavelengths
         wl_true = []
         for wl_, srf in self.prod.SRF.groupby('wl'):
             srf = srf.dropna('wl_hr')
             wl_true.append((srf.wl_hr * srf).integrate('wl_hr') / srf.integrate('wl_hr'))
         wl_true = xr.concat(wl_true, dim='wl')
```

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/L8_Ball_BA_RSR.v1.2.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/L4_TM_RSR.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/L4_TM_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/L5_TM_RSR.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/L5_TM_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/L7_RSR.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/L7_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx` & `grsdriver-1.0.4/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/rsr_landsat_8_oli.nc` & `grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_8_oli.nc`

 * *Files 2% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_7401nk8k_/tmpja3o34hz_TarContainer/0/15.nc" {
+HDF5 "/tmp/diffoscope_7401nk8k_/tmpamdyqwmn_TarContainer/0/17.nc" {
 GROUP "/" {
    ATTRIBUTE "_NCProperties" {
       DATATYPE  H5T_STRING {
          STRSIZE 34;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_ASCII;
          CTYPE H5T_C_S1;
@@ -1580,76 +1580,76 @@
       ATTRIBUTE "DIMENSION_LIST" {
          DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
          DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
          DATA {
          (0): (DATASET 662 "/wl"), (DATASET 239 "/wl_hr")
          }
       }
-      ATTRIBUTE "_FillValue" {
-         DATATYPE  H5T_IEEE_F64LE
-         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
-         DATA {
-         (0): nan
-         }
-      }
-      ATTRIBUTE "_Netcdf4Coordinates" {
-         DATATYPE  H5T_STD_I32LE
-         DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
-         DATA {
-         (0): 1, 0
-         }
-      }
-      ATTRIBUTE "description" {
+      ATTRIBUTE "OLI_description" {
          DATATYPE  H5T_STRING {
             STRSIZE 59;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
          (0): "relative spectral response functions for Landat-8 OLI bands"
          }
       }
-      ATTRIBUTE "file_creation" {
+      ATTRIBUTE "OLI_file_creation" {
          DATATYPE  H5T_STRING {
             STRSIZE 26;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
-         (0): "2023-09-14 18:20:29.135008"
+         (0): "2024-04-12 13:15:04.046971"
          }
       }
-      ATTRIBUTE "from_file" {
+      ATTRIBUTE "OLI_from_file" {
          DATATYPE  H5T_STRING {
-            STRSIZE 21;
+            STRSIZE 24;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
-         (0): "Ball_BA_RSR.v1.2.xlsx"
+         (0): "L8_Ball_BA_RSR.v1.2.xlsx"
          }
       }
-      ATTRIBUTE "long_name" {
+      ATTRIBUTE "OLI_long_name" {
          DATATYPE  H5T_STRING {
             STRSIZE 16;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
          (0): "SRF_Landat_8_OLI"
          }
       }
+      ATTRIBUTE "_FillValue" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
+         DATA {
+         (0): nan
+         }
+      }
+      ATTRIBUTE "_Netcdf4Coordinates" {
+         DATATYPE  H5T_STD_I32LE
+         DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
+         DATA {
+         (0): 1, 0
+         }
+      }
    }
    DATASET "wl" {
       DATATYPE  H5T_STD_I64LE
       DATASPACE  SIMPLE { ( 9 ) / ( 9 ) }
       DATA {
       (0): 443, 490, 560, 590, 665, 865, 1370, 1610, 2190
       }
```

### Comparing `GRSdriver-1.0.3/GRSdriver/rsr/data/rsr_landsat_9_oli.nc` & `grsdriver-1.0.4/GRSdriver/rsr/data/rsr_landsat_9_oli.nc`

 * *Files 2% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_7401nk8k_/tmpja3o34hz_TarContainer/0/16.nc" {
+HDF5 "/tmp/diffoscope_7401nk8k_/tmpamdyqwmn_TarContainer/0/20.nc" {
 GROUP "/" {
    ATTRIBUTE "_NCProperties" {
       DATATYPE  H5T_STRING {
          STRSIZE 34;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_ASCII;
          CTYPE H5T_C_S1;
@@ -1594,76 +1594,76 @@
       ATTRIBUTE "DIMENSION_LIST" {
          DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
          DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
          DATA {
          (0): (DATASET 662 "/wl"), (DATASET 239 "/wl_hr")
          }
       }
-      ATTRIBUTE "_FillValue" {
-         DATATYPE  H5T_IEEE_F64LE
-         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
-         DATA {
-         (0): nan
-         }
-      }
-      ATTRIBUTE "_Netcdf4Coordinates" {
-         DATATYPE  H5T_STD_I32LE
-         DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
-         DATA {
-         (0): 1, 0
-         }
-      }
-      ATTRIBUTE "description" {
+      ATTRIBUTE "OLI_description" {
          DATATYPE  H5T_STRING {
             STRSIZE 59;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
          (0): "relative spectral response functions for Landat-9 OLI bands"
          }
       }
-      ATTRIBUTE "file_creation" {
+      ATTRIBUTE "OLI_file_creation" {
          DATATYPE  H5T_STRING {
             STRSIZE 26;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
-         (0): "2023-09-14 18:20:30.009294"
+         (0): "2024-04-12 12:33:43.389548"
          }
       }
-      ATTRIBUTE "from_file" {
+      ATTRIBUTE "OLI_from_file" {
          DATATYPE  H5T_STRING {
             STRSIZE 30;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
          (0): "L9_OLI2_Ball_FPM_RSR.v1.0.xlsx"
          }
       }
-      ATTRIBUTE "long_name" {
+      ATTRIBUTE "OLI_long_name" {
          DATATYPE  H5T_STRING {
             STRSIZE 16;
             STRPAD H5T_STR_NULLTERM;
             CSET H5T_CSET_ASCII;
             CTYPE H5T_C_S1;
          }
          DATASPACE  SCALAR
          DATA {
          (0): "SRF_Landat_9_OLI"
          }
       }
+      ATTRIBUTE "_FillValue" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
+         DATA {
+         (0): nan
+         }
+      }
+      ATTRIBUTE "_Netcdf4Coordinates" {
+         DATATYPE  H5T_STD_I32LE
+         DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
+         DATA {
+         (0): 1, 0
+         }
+      }
    }
    DATASET "wl" {
       DATATYPE  H5T_STD_I64LE
       DATASPACE  SIMPLE { ( 9 ) / ( 9 ) }
       DATA {
       (0): 443, 490, 560, 590, 665, 865, 1370, 1610, 2190
       }
```

### Comparing `GRSdriver-1.0.3/GRSdriver/run.py` & `grsdriver-1.0.4/GRSdriver/run.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,39 +10,46 @@
   -h --help        Show this screen.
   -v --version     Show version.
 
   <input_file>     Input file to be processed
 
   -o ofile         Full (absolute or relative) path to output L2 image.
   --odir odir      Ouput directory [default: ./]
-  --rgb_bands=RGB  band number to be used in RGB [default: '4,3,1']
-
-  --resolution=res  spatial resolution of the scene pixels
+  --rgb_bands RGB  Comma separated list of band numbers to be used in RGB
+                   [default: 3,2,1]
+  --resolution res  spatial resolution of the scene pixels [default: 60]
   --no_clobber     Do not process <input_file> if <output_file> already exists.
 
 '''
 
 import os, sys
 from docopt import docopt
 import numpy as np
 import logging
+
 from GRSdriver import __package__, __version__
+import GRSdriver
 
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+from eoreader.env_vars import USE_DASK
+# Ensure EOReader uses dask
+os.environ[USE_DASK] = "1"
 
 def main():
 
     args = docopt(__doc__, version=__package__ + '_' + __version__)
     print(args)
 
     file = args['<input_file>']
 
     resolution = int(args['--resolution'])
-    RGB = np.array(args['--rgb_bands'])
+    RGB =  [int(x) for x in args['--rgb_bands'].split(',')]
     noclobber = args['--no_clobber']
-
+    print(RGB)
     ##################################
     # File naming convention
     ##################################
 
     outfile = args['-o']
     if outfile == None:
         basename = os.path.basename(file)
@@ -61,14 +68,32 @@
         print('File ' + outfile + ' already processed; skip!')
         sys.exit()
 
     logging.info('making RGB image for:' +
                  file + ', output file:' + outfile +
                  ', resolution:' + str(resolution))
 
+    # load product into l1c object
+    l1c = GRSdriver.LandsatDriver(file,
+                                  band_idx=RGB,
+                                  resolution=resolution)
+    l1c.load_bands()
+
+    # get geographic information
+    epsg = l1c.extent.crs.to_epsg()
+    str_epsg = str(epsg)
+    zone = str_epsg[-2:]
+    is_south = str_epsg[2] == 7
+    proj = ccrs.UTM(zone, is_south)
+
+    # plot RGB image
+
+    plt.figure(figsize=(15, 15))
+    p = l1c.prod.bands.isel(wl=[2,1,0]).squeeze().plot.imshow(rgb='wl', robust=True,subplot_kws=dict(projection=proj))
+    p.figure.savefig(outfile)
    # TODO implement the RGB converter
 
 
     return
 
 
 if __name__ == "__main__":
```

### Comparing `GRSdriver-1.0.3/GRSdriver/visual.py` & `grsdriver-1.0.4/GRSdriver/visual.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import panel.widgets as pnw
 import param as pm
 from shapely.geometry import Polygon
 from collections import OrderedDict as odict
 
 
 
-class utils():
+class Utils():
 
     @staticmethod
     def get_geom(aoi_stream, crs=4326):
         geom = aoi_stream.data
         ys, xs = geom['ys'][-1], geom['xs'][-1]
         polygon_geom = Polygon(zip(xs, ys))
         polygon = gpd.GeoDataFrame(index=[0], crs=3857, geometry=[polygon_geom])
@@ -54,28 +54,34 @@
         custom_formatters = {
             '@x': bokeh.models.CustomJSHover(code=formatter_code_x),
             '@y': bokeh.models.CustomJSHover(code=formatter_code_y)
         }
         return bokeh.models.HoverTool(tooltips=custom_tooltips, formatters=custom_formatters)
 
 
-class view_geo(utils):
+class ViewSpectral(Utils):
     def __init__(self, raster, dates=None,
                  bands=None,
                  reproject=False,
                  minmaxvalues=(0, 0.5),
                  minmax=(0, 1)):
-        # layout settings
-        self.width, self.height = 1200, 700
 
+        # layout settings
+        self.title ='## S2 L1C'
+        self.width, self.height = 1200, 800
         self.key_dimensions = ['x', 'y']
         self.minmaxvalues = minmaxvalues
         self.minmax = minmax
-        self.colormaps = ['CET_D13', 'bky', 'CET_D1A', 'CET_CBL2', 'CET_L10', 'CET_C6s',
+        self.colormaps = ['CET_D13', 'bky', 'rainbow4','CET_D1A', 'CET_CBL2', 'CET_L10', 'CET_C6s',
                           'kbc', 'blues_r', 'kb', 'rainbow', 'fire', 'kgy', 'bjy', 'gray']
+
+        # check if single date, if so push time as dimension to be compliant with multidates
+        if not 'time' in raster.dims:
+            raster = raster.expand_dims('time')
+
         # variables settings
         self.dates = dates
         if dates == None:
             self.dates = raster.time.dt.date.values
         self.bands = bands
         if bands == None:
             self.bands = raster.wl.values
@@ -101,31 +107,14 @@
         self.aoi_polygons = hv.Polygons([]).opts(opts.Polygons(
             fill_alpha=0.3, fill_color='white',
             line_width=1.2))  ##, active_tools=['poly_draw']))#.opts(crs.GOOGLE_MERCATOR)
         self.aoi_stream = hv.streams.PolyDraw(
             source=self.aoi_polygons, drag=True)  # , num_objects=1)#5,styles={'fill_color': aoi_colours})
         self.edit_stream = hv.streams.PolyEdit(source=self.aoi_polygons, vertex_style={'color': 'red'})
 
-    @staticmethod
-    def custom_hover():
-        formatter_code = """
-          var digits = 4;
-          var projections = Bokeh.require("core/util/projections");
-          var x = special_vars.x; var y = special_vars.y;
-          var coords = projections.wgs84_mercator.invert(x, y);
-          return "" + (Math.round(coords[%d] * 10**digits) / 10**digits).toFixed(digits)+ "";
-        """
-        formatter_code_x, formatter_code_y = formatter_code % 0, formatter_code % 1
-        custom_tooltips = [('Lon', '@x{custom}'), ('Lat', '@y{custom}'), ('Value', '@image{0.0000}')]
-        custom_formatters = {
-            '@x': bokeh.models.CustomJSHover(code=formatter_code_x),
-            '@y': bokeh.models.CustomJSHover(code=formatter_code_y)
-        }
-        return bokeh.models.HoverTool(tooltips=custom_tooltips, formatters=custom_formatters)
-
     def visu(self):
         dates = self.dates
         bands = self.bands
         hv.opts.defaults(
             hv.opts.Image(height=self.height, width=self.width,
                           colorbar=True, tools=[self.custom_hover()], active_tools=['wheel_zoom'],
                           clipping_colors={'NaN': '#00000000'}),
@@ -141,17 +130,17 @@
                 images[date, iband] = hv.Image(datasets).opts(gopts)
 
         bases = [name for name, ts in hv.element.tiles.tile_sources.items()]
         pn_band = pn.widgets.RadioButtonGroup(value=0, options=list(range(len(bands))))
         pn_colormap = pn.widgets.Select(value='CET_D13',
                                         options=self.colormaps)
         pn_opacity = pn.widgets.FloatSlider(name='Opacity', value=0.95, start=0, end=1, step=0.05)
-        range_slider = pn.widgets.RangeSlider(name='Range Slider', start=self.minmax[0], end=self.minmax[1],
-                                              value=self.minmaxvalues, step=0.0001)
-        pn_basemaps = pn.widgets.Select(value='StamenTerrainRetina', options=bases)
+        range_slider = pn.widgets.EditableRangeSlider(name='Range Slider', start=self.minmax[0], end=self.minmax[1],
+                                                      value=self.minmaxvalues, step=0.001)
+        pn_basemaps = pn.widgets.Select(value=bases[0], options=bases)
         pn_date = pn.widgets.DatePicker(value=dates[0], start=dates[0],
                                         enabled_dates=dates.tolist())  # .date, end=dates[-1],value=dates[0])
 
         @pn.depends(
             pn_date_value=pn_date.param.value,
             pn_band_value=pn_band.param.value,
             pn_colormap_value=pn_colormap.param.value,
@@ -175,15 +164,15 @@
 
         dynmap = hd.regrid(hv.DynamicMap(load_map))
         combined = (hv.DynamicMap(
             load_tiles) * dynmap * self.aoi_polygons)
 
         return pn.Column(
             pn.WidgetBox(
-                '## S2 L1C',
+                self.title,
                 pn.Column(
                     pn.Row(
                         pn.Row('### Band', pn_band),
                         pn.Row('### Date', pn_date),
                         pn.Row('#### Basemap', pn_basemaps)
                     ),
                     pn.Row(
```

### Comparing `GRSdriver-1.0.3/GRSdriver.egg-info/PKG-INFO` & `grsdriver-1.0.4/GRSdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `GRSdriver-1.0.3/LICENSE` & `grsdriver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/PKG-INFO` & `grsdriver-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `GRSdriver-1.0.3/README.md` & `grsdriver-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.3/pyproject.toml` & `grsdriver-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GRSdriver"
-version = "1.0.3"
+version = "1.0.4"
 description = "Driver for L1C satellite images dedicated to GRS processor"
 readme = "README.md"
 authors = [{ name = "Tristan Harmel", email = "tristan.harmel@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

