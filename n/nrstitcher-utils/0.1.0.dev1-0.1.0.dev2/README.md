# Comparing `tmp/nrstitcher_utils-0.1.0.dev1.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev1.tar", last modified: Tue Apr 23 06:38:05 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev2.tar", last modified: Tue Apr 23 07:49:58 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev1.tar` & `nrstitcher_utils-0.1.0.dev2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-23 06:24:16.000000 nrstitcher_utils-0.1.0.dev1/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     7807 2024-04-23 06:35:42.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:24:31.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3110 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8604 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-23 06:37:53.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      607 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev2/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev2/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-23 06:24:16.000000 nrstitcher_utils-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev2/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.148441 nrstitcher_utils-0.1.0.dev2/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8309 2024-04-23 07:48:23.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:24:31.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3220 2024-04-23 07:26:52.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8694 2024-04-23 07:27:28.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      257 2024-04-23 07:48:08.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/resources/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-23 07:49:15.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 07:49:58.152441 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      650 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-23 07:49:58.000000 nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev1/LICENSE` & `nrstitcher_utils-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev1/PKG-INFO` & `nrstitcher_utils-0.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev1/pyproject.toml` & `nrstitcher_utils-0.1.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 After adding the NRStitcher directory to the path, this script should be run from the directory where the generated stitch settings file is to be saved.
 
 """
 
 import argparse
 import glob
 import os
-import numpy as np
 import shutil
 import sys
+import logging
 
 # import from pi2 / NRstitcher -> see https://github.com/arttumiettinen/pi2/blob/master/python_scripts/default_stitch_settings.py
 from default_stitch_settings import write_stitch_settings
 from nrstitcher_utils.core.h5_settings import H5Settings
 from nrstitcher_utils.core.ht_vol import HTVol
 from nrstitcher_utils.core import utils
+from nrstitcher_utils.resources import get_config_file
+
+_logger = logging.getLogger(__name__)
 
 
 def main(argv):
 
     def get_h5file(h5_folder):
         """
         Gets the name of the h5 file associated with the experiment base directory.
@@ -106,31 +109,39 @@
     argparser.add_argument(
         "-o",
         "--output",
         default="stitch_settings.txt",
         type=str,
         help='Optional. Name of stitch_settings file. Default is "stitch_settings.txt". Will be saved in the current working directory.',
     )
+    argparser.add_argument(
+        "--debug",
+        type=bool,
+        default=False,
+        help='Optional. Name of stitch_settings file. Default is "stitch_settings.txt". Will be saved in the current working directory.',
+    )
 
     args = argparser.parse_args(argv)
     if args.distances == None:
         args.distances = [1, 2, 3, 4]
     args.distances.sort()
+    log_level = logging.DEBUG if args.debug else logging.INFO
+    logging.basicConfig(level=log_level)
 
     # Get volumes from command line input
     if len(args.volumes) > 1:
         # Do this if entire name of individual volumes given
         volNames = args.volumes
         floatVols = [os.path.join(args.base_dir, args.vol_dir) + x for x in volNames]
     else:
         # Do this if script is to take all volumes containing the given strings, can contain wildcards
         floatVols = sorted(
             glob.glob(os.path.join(args.base_dir, args.vol_dir) + args.volumes[0])
         )
-        print(floatVols)
+        _logger.debug("floatVols", floatVols)
         volNames = [os.path.basename(x) for x in floatVols]
 
     rawVols = []
 
     for volName in volNames:
         # Process the float volumes (convert to raw if not already done)
         vol = HTVol(args, volName)
@@ -194,15 +205,15 @@
         Z += dZ
 
         # Positions in units of pixels with correction in case tiles do not have the same number of pixels
         Z = round(Z / vox_size + (Zdim_ref - Zdim) / 2.0)
         Y = round(Y / vox_size + (Ydim_ref - Ydim) / 2.0)
         X = round(X / vox_size + (Xdim_ref - Xdim) / 2.0)
 
-        print(X, Y, Z)
+        logging.INFO(f"positions (in px): {X}, {Y}, {Z}")
 
         path = vol
         line = f"{path} = {X}, {Y}, {Z}"
         line_to_write += line + "\n"
 
     # Write the stitch settings file and copy slurm_config file to local directory
     write_stitch_settings(
@@ -210,17 +221,18 @@
         args.binning,
         line_to_write,
         point_spacing=100,
         coarse_block_radius=50,
         coarse_binning=2,
         cluster_name="SLURM",
     )
+    # note: write_stitch_settings always write settings to stitch_settings.txt
     os.rename("./stitch_settings.txt", "./" + args.output)
     if not os.path.isfile("./slurm_config.txt"):
         shutil.copyfile(
-            "/data/id16a/inhouse1/sware/NRstitcher/pi2-0523/pi2/bin-linux64/release-nocl/slurm_config_id16a.txt",
+            get_config_file("slurm_config_id16a.txt"),
             "./slurm_config.txt",
         )
 
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/h5_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import h5py
 from itertools import compress
+import logging
+
+_logger = logging.getLogger(__name__)
 
 
 class H5Settings:
 
     def __init__(self, h5_filename, volume_name, scan_suffix):
         self.filename = h5_filename
         self.file = h5py.File(self.filename, "r")
@@ -17,25 +20,25 @@
 
         found = False
 
         for entry in entry_list:
             prefix = entry.split(" ")[-1].replace(scan_suffix, "")
             if prefix in volume_name:
                 self.root = self.file[entry]
-                print(volume_name)
+                _logger.info("will treat volume", volume_name)
                 found = True
 
         if found == False:
             for entry in entry_list:
                 tmp = entry.split(" ")[-1]
                 prefix = "".join(tmp.rsplit(scan_suffix, 1))
 
                 if prefix in volume_name:
                     self.root = self.file[entry]
-                    print(volume_name)
+                    _logger.info("will treat volume", volume_name)
 
     def toList(self, group):
         """
         Write h5 file entries to a list.
 
         Arguments:
         group: Required group in h5 file
```

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/ht_vol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
+import logging
 from pi2py2 import ImageDataType, Pi2
 
 
+_logger = logging.getLogger(__name__)
+
+
 class HTVol:
     """Half-tomo volume"""
 
     def __init__(self, args, volName):
 
         self.pi = Pi2()
 
@@ -103,15 +107,15 @@
         ) and os.path.isfile(infoFileName):
             raw_info = self.get_vol_info(infoFileName)
 
             raw_vmin = int(float(raw_info["ValMin"]))
             raw_vmax = int(float(raw_info["ValMax"]))
 
             if raw_vmin == int(self.tomin) and raw_vmax == int(self.tomax):
-                print(
+                _logger.info(
                     os.path.join(self.savePath, self.saveFileName)
                     + " already exists. Skipping."
                 )
                 return True
 
         return False
 
@@ -122,15 +126,15 @@
         Arguments:
         None
 
         Returns:
 
         """
 
-        print("Reading volume " + self.volName)
+        _logger.info("Reading volume " + self.volName)
         self.volfloat = self.pi.read(self.volName)
 
     def create_vol(self, dtype):
         """
         Create a new pi2 image of specified datatype and dimensions.
 
         Arguments:
@@ -159,15 +163,15 @@
         None
 
         Returns:
 
         """
 
         intbits = {"uint32": 32, "uint16": 16, "uint8": 8}
-        print("Converting to " + str(intbits[self.toType]) + " bits.")
+        _logger.info("Converting to " + str(intbits[self.toType]) + " bits.")
 
         self.vmax = self.tomax
         self.vmin = self.tomin
         self.vmin -= 1 / (
             2 ** intbits[self.toType] - 1
         )  # Zero-valued pixels (eg. pixels outside the reconstructed cylinder) should retain their zero-value after the conversion
 
@@ -196,15 +200,15 @@
         Arguments:
         None
 
         Returns:
 
         """
 
-        print("Rescaling to " + str(self.rescaleTo) + " nm pixel/voxel size.")
+        _logger.info("Rescaling to " + str(self.rescaleTo) + " nm pixel/voxel size.")
         tmp = self.create_vol(self.toType)
         self.pi.scale(self.volfloat, tmp, [0, 0, 0], False, "Nearest")
         self.volfloat.set_data(tmp.get_data())
         del tmp
         self.modified = True
 
     def reslice(self, direction):
@@ -231,15 +235,15 @@
         Arguments:
         None
 
         Returns:
 
         """
 
-        print("Writing to " + os.path.join(self.savePath, self.saveFileName))
+        _logger.info("Writing to " + os.path.join(self.savePath, self.saveFileName))
 
         self.pi.writeraw(self.volfloat, os.path.join(self.savePath, self.saveFile))
         self.write_raw_info()
 
     def write_raw_info(self):
         """
         Write a .raw.info file containing the parameters of the processed volume.
```

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-0.1.0.dev2/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 src/nrstitcher_utils.egg-info/requires.txt
 src/nrstitcher_utils.egg-info/top_level.txt
 src/nrstitcher_utils/app/__init__.py
 src/nrstitcher_utils/app/nrs_config_id16a_ht.py
 src/nrstitcher_utils/core/__init__.py
 src/nrstitcher_utils/core/h5_settings.py
 src/nrstitcher_utils/core/ht_vol.py
-src/nrstitcher_utils/core/utils.py
+src/nrstitcher_utils/core/utils.py
+src/nrstitcher_utils/resources/__init__.py
```

