# Comparing `tmp/collider-check-0.1.7.tar.gz` & `tmp/collider_check-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collider-check-0.1.7.tar", last modified: Wed Jan 24 08:46:25 2024, max compression
+gzip compressed data, was "collider_check-0.2.0.tar", last modified: Tue Apr 23 15:41:39 2024, max compression
```

## Comparing `collider-check-0.1.7.tar` & `collider_check-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-01-24 08:46:25.922924 collider-check-0.1.7/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2023-11-15 10:21:33.000000 collider-check-0.1.7/LICENSE
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-01-24 08:46:25.922924 collider-check-0.1.7/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2023-11-15 10:21:33.000000 collider-check-0.1.7/README.md
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-01-24 08:29:14.000000 collider-check-0.1.7/pyproject.toml
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-01-24 08:46:25.922924 collider-check-0.1.7/setup.cfg
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-01-24 08:46:25.922924 collider-check-0.1.7/src/
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-01-24 08:46:25.922924 collider-check-0.1.7/src/collider_check/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-01-24 08:29:06.000000 collider-check-0.1.7/src/collider_check/__init__.py
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    26678 2024-01-24 07:57:42.000000 collider-check-0.1.7/src/collider_check/collider_check.py
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-01-24 08:46:25.922924 collider-check-0.1.7/src/collider_check.egg-info/
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-01-24 08:46:25.000000 collider-check-0.1.7/src/collider_check.egg-info/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-01-24 08:46:25.000000 collider-check-0.1.7/src/collider_check.egg-info/SOURCES.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-01-24 08:46:25.000000 collider-check-0.1.7/src/collider_check.egg-info/dependency_links.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-01-24 08:46:25.000000 collider-check-0.1.7/src/collider_check.egg-info/requires.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-01-24 08:46:25.000000 collider-check-0.1.7/src/collider_check.egg-info/top_level.txt
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-01-24 08:46:25.922924 collider-check-0.1.7/tests/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2023-11-15 10:21:33.000000 collider-check-0.1.7/tests/test_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2024-04-23 15:24:05.000000 collider_check-0.2.0/LICENSE
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-04-23 15:41:39.693974 collider_check-0.2.0/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2024-04-23 15:24:05.000000 collider_check-0.2.0/README.md
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-04-23 15:37:53.000000 collider_check-0.2.0/pyproject.toml
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-04-23 15:41:39.693974 collider_check-0.2.0/setup.cfg
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/collider_check/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-04-23 15:24:05.000000 collider_check-0.2.0/src/collider_check/__init__.py
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    27100 2024-04-23 15:36:13.000000 collider_check-0.2.0/src/collider_check/collider_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/collider_check.egg-info/
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/requires.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/top_level.txt
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/tests/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2024-04-23 15:24:05.000000 collider_check-0.2.0/tests/test_check.py
```

### Comparing `collider-check-0.1.7/LICENSE` & `collider_check-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collider-check-0.1.7/PKG-INFO` & `collider_check-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.1.7
+Version: 0.2.0
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider-check-0.1.7/README.md` & `collider_check-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `collider-check-0.1.7/pyproject.toml` & `collider_check-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = false
 
 [project]
 name = "collider-check"
-version = "0.1.7"
+version = "0.2.0"
 description = "A small package that provides functions to check the observables in a collider, using a collider built with Xsuite."
 readme = "README.md"
 authors = [{ name = "Colas Droin", email = "colas.noe.droin@cern.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `collider-check-0.1.7/src/collider_check/__init__.py` & `collider_check-0.2.0/src/collider_check/__init__.py`

 * *Files identical despite different names*

### Comparing `collider-check-0.1.7/src/collider_check/collider_check.py` & `collider_check-0.2.0/src/collider_check/collider_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,35 @@
 from scipy import constants
 
 
 # ==================================================================================================
 # --- Class definition
 # ==================================================================================================
 class ColliderCheck:
-    def __init__(self, collider, path_filling_scheme=None):
+    def __init__(self, collider, path_filling_scheme=None, type_particles="proton"):
         """Initialize the ColliderCheck class directly from a collider, potentially embedding a
         configuration file."""
 
         # Store the collider
         self.collider = collider
 
         # Store the filling scheme path
         self.path_filling_scheme = path_filling_scheme
+        
+        # Check the type of particles and store
+        if type_particles in ["proton", "lead"]:
+            self.type_particles = type_particles
+        else:
+            raise ValueError("type_particles must be either 'proton' or 'lead'.") 
+        
+        # Record cross-section correspondinlgy
+        if self.type_particles == "proton":
+            self.cross_section = 81e-27
+        elif self.type_particles == "lead":
+            self.cross_section = 281e-24
 
         # Define the configuration through a property since it might not be there
         self._configuration = None
         self.configuration_str = None
 
         # Beam energy
         self.energy = self.collider.lhcb1.particle_ref._p0c[0] / 1e9
@@ -46,20 +58,17 @@
     @property
     def configuration(self):
         """Loads the configuration, as well as the luminosity and filling scheme arrays, if they're
         not already loaded."""
 
         if self._configuration is not None:
             return self._configuration
-        else:
-            # Get the corresponding configuration if it's there
-            if hasattr(self.collider, "metadata"):
-                if self.collider.metadata != {}:
-                    self.configuration = self.collider.metadata
-
+        # Get the corresponding configuration if it's there
+        if hasattr(self.collider, "metadata") and self.collider.metadata != {}:
+            self.configuration = self.collider.metadata
         return self._configuration
 
     @configuration.setter
     def configuration(self, configuration_dict):
         """This function is used to update the configuration, and the attributes that depend on it."""
         self._configuration = configuration_dict
         self._update_attributes_configuration()
@@ -81,25 +90,23 @@
         # Clean cache for separation computation
         self.compute_separation_variables.cache_clear()
 
     @property
     def nemitt_x(self):
         if self.configuration is not None:
             return self.configuration["config_collider"]["config_beambeam"]["nemitt_x"]
-        else:
-            print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_x.")
-            return 2.2e-6
+        print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_x.")
+        return 2.2e-6
 
     @property
     def nemitt_y(self):
         if self.configuration is not None:
             return self.configuration["config_collider"]["config_beambeam"]["nemitt_y"]
-        else:
-            print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_y.")
-            return 2.2e-6
+        print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_y.")
+        return 2.2e-6
 
     def _check_configuration(self):
         if self.configuration is None:
             raise ValueError(
                 "No configuration has been provided when instantiating the ColliderCheck object."
             )
 
@@ -114,35 +121,33 @@
         if self.path_filling_scheme is None:
             # Get the filling scheme path (should already be an absolute path)
             self.path_filling_scheme = self.configuration["config_collider"]["config_beambeam"][
                 "mask_with_filling_pattern"
             ]["pattern_fname"]
 
             # Check if filling scheme file exists, and replace it by local if not
-            if os.path.isfile(self.path_filling_scheme):
-                pass
-
-            # Else check if it is called from data folder of collider_dashboard
-            else:
+            if not os.path.isfile(self.path_filling_scheme):
                 try:
                     package_path = str(files("collider_dashboard"))
-                except NameError:
+                except NameError as e:
                     raise ValueError(
                         "collider_dashboard not installed... Filling scheme file could not be"
                         " loaded from the path in the configuration or locally."
-                    )
+                    ) from e
                 if os.path.isfile(
-                    package_path + "/data/" + self.path_filling_scheme.split("/")[-1]
+                    f"{package_path}/data/"
+                    + self.path_filling_scheme.split("/")[-1]
                 ):
                     print(
                         "Filling scheme file could not be loaded from the path in the"
                         " configuration. Loading it locally."
                     )
                     self.path_filling_scheme = (
-                        package_path + "/data/" + self.path_filling_scheme.split("/")[-1]
+                        f"{package_path}/data/"
+                        + self.path_filling_scheme.split("/")[-1]
                     )
                 else:
                     raise ValueError(
                         "Filling scheme file could not be loaded from the path in the configuration"
                         " or locally."
                     )
 
@@ -165,15 +170,15 @@
         """Computes and returns the number of collisions at the requested IP."""
 
         # Ensure configuration is defined
         self._check_configuration()
 
         # Assert that the arrays have the required length, and do the convolution
         assert len(self.array_b1) == len(self.array_b2) == 3564
-        if IP == 1 or IP == 5:
+        if IP in [1, 5]:
             return self.array_b1 @ self.array_b2
         elif IP == 2:
             return np.roll(self.array_b1, 891) @ self.array_b2
         elif IP == 8:
             return np.roll(self.array_b1, 2670) @ self.array_b2
         else:
             raise ValueError("IP must be either 1, 2, 5 or 8.")
@@ -198,26 +203,25 @@
             )
             if abs(crab_val) > 0:
                 crab = True
 
         if IP not in [1, 2, 5, 8]:
             raise ValueError("IP must be either 1, 2, 5 or 8.")
         n_col = self.return_number_of_collisions(IP=IP)
-        luminosity = xt.lumi.luminosity_from_twiss(
+        return xt.lumi.luminosity_from_twiss(
             n_colliding_bunches=n_col,
             num_particles_per_bunch=self.num_particles_per_bunch,
-            ip_name="ip" + str(IP),
+            ip_name=f"ip{str(IP)}",
             nemitt_x=self.nemitt_x,
             nemitt_y=self.nemitt_y,
             sigma_z=self.sigma_z,
             twiss_b1=self.tw_b1,
             twiss_b2=self.tw_b2,
             crab=crab,
         )
-        return luminosity
 
     def return_twiss_at_ip(self, beam=1, ip=1):
         """Returns the twiss parameters, position and angle at the requested IP."""
         if beam == 1:
             return (
                 self.tw_b1.rows[f"ip{ip}"]
                 .cols["s", "x", "px", "y", "py", "betx", "bety", "dx", "dy"]
@@ -281,23 +285,23 @@
         else:
             beam_strong = "b1"
             twiss_weak = self.tw_b2.reverse()
             twiss_strong = self.tw_b1
             survey_weak = self.dic_survey_per_ip["lhcb2"]
             survey_strong = self.dic_survey_per_ip["lhcb1"]
 
-        # Filter the twiss and surveys at the requested IP
-        survey_filtered = {}
-        twiss_filtered = {}
         my_filter_string = f"bb_(ho|lr)\.(r|l|c){ip[2]}.*"
-        survey_filtered[beam_strong] = survey_strong[ip][["X", "Y", "Z"], my_filter_string]
-        survey_filtered[beam_weak] = survey_weak[ip][["X", "Y", "Z"], my_filter_string]
-        twiss_filtered[beam_strong] = twiss_strong[:, my_filter_string]
-        twiss_filtered[beam_weak] = twiss_weak[:, my_filter_string]
-
+        survey_filtered = {
+            beam_strong: survey_strong[ip][["X", "Y", "Z"], my_filter_string],
+            beam_weak: survey_weak[ip][["X", "Y", "Z"], my_filter_string],
+        }
+        twiss_filtered = {
+            beam_strong: twiss_strong[:, my_filter_string],
+            beam_weak: twiss_weak[:, my_filter_string],
+        }
         s = survey_filtered[beam_strong]["Z"]
         d_x_weak_strong_in_meter = (
             twiss_filtered[beam_weak]["x"]
             - twiss_filtered[beam_strong]["x"]
             + survey_filtered[beam_weak]["X"]
             - survey_filtered[beam_strong]["X"]
         )
@@ -315,18 +319,25 @@
             twiss_filtered,
             survey_filtered,
             d_x_weak_strong_in_meter,
             d_y_weak_strong_in_meter,
         )
 
     def _compute_emittances_separation(self):
-        # gamma relativistic of a proton at 7 TeV
-        gamma_rel = self.energy / (
-            constants.physical_constants["proton mass energy equivalent in MeV"][0] / 1000
-        )
+        if self.type_particles == "proton":
+            # gamma relativistic of a proton
+            gamma_rel = self.energy / (
+                constants.physical_constants["proton mass energy equivalent in MeV"][0] / 1000
+            )
+        elif self.type_particles == "lead":
+            # gamma relativistic of a lead ion (value needs to be double-checked)
+            gamma_rel = self.energy / (193084.751 / 1000)
+        else:
+            raise ValueError("type_particles must be either 'proton' or 'lead'.")
+        
         # beta relativistic of a proton at 7 TeV
         beta_rel = np.sqrt(1 - 1 / gamma_rel**2)
 
         emittance_strong_x = self.nemitt_x / gamma_rel / beta_rel
         emittance_strong_y = self.nemitt_y / gamma_rel / beta_rel
 
         emittance_weak_x = self.nemitt_x / gamma_rel / beta_rel
@@ -430,16 +441,15 @@
             emittance_strong_y,
             emittance_weak_x,
             emittance_weak_y,
             d_x_weak_strong_in_meter,
             d_y_weak_strong_in_meter,
         )
 
-        # Stora all variables used dor separation computation in a dictionnary
-        dic_separation = {
+        return {
             "twiss_filtered": twiss_filtered,
             "survey_filtered": survey_filtered,
             "s": s,
             "dx_meter": d_x_weak_strong_in_meter,
             "dy_meter": d_y_weak_strong_in_meter,
             "dx_sig": dx_sig,
             "dy_sig": dy_sig,
@@ -456,16 +466,14 @@
             "energy": self.energy,
             "my_filter_string": my_filter_string,
             "beam_weak": beam_weak,
             "beam_strong": beam_strong,
             "ip": ip,
         }
 
-        return dic_separation
-
     def return_dic_position_all_ips(self):
         """This function computes all the variables needed to compute the position of the beam in
         all IRs. The variables are stored and returne in a dictionnary. The extreme positions are:
         IP1 : mqy.4l1.b1 to mqy.4r1.b1
         IP2 : mqy.b5l2.b1 to mqy.b4r2.b1
         IP5 : mqy.4l5.b1 to mqy.4r5.b1
         IP8 : mqy.b4l8.b1 to mqy.b4r8.b1
@@ -590,20 +598,18 @@
         plt.ylabel("separation in x,y [$\sigma$]")
         plt.legend()
         plt.grid(True)
         plt.show()
 
     def output_check_as_str(self, path_output=None):
         """Summarizes the collider observables in a string, and optionally to a file."""
-        str_file = ""
-
         # Check tune and chromaticity
         qx_b1, dqx_b1, qy_b1, dqy_b1 = self.return_tune_and_chromaticity(beam=1)
         qx_b2, dqx_b2, qy_b2, dqy_b2 = self.return_tune_and_chromaticity(beam=2)
-        str_file += "Tune and chromaticity\n"
+        str_file = "" + "Tune and chromaticity\n"
         str_file += (
             f"Qx_b1 = {qx_b1:.4f}, Qy_b1 = {qy_b1:.4f}, dQx_b1 = {dqx_b1:.4f}, dQy_b1 ="
             f" {dqy_b1:.4f}\n"
         )
         str_file += (
             f"Qx_b2 = {qx_b2:.4f}, Qy_b2 = {qy_b2:.4f}, dQx_b2 = {dqx_b2:.4f}, dQy_b2 ="
             f" {dqy_b2:.4f}\n"
```

### Comparing `collider-check-0.1.7/src/collider_check.egg-info/PKG-INFO` & `collider_check-0.2.0/src/collider_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.1.7
+Version: 0.2.0
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider-check-0.1.7/tests/test_check.py` & `collider_check-0.2.0/tests/test_check.py`

 * *Files identical despite different names*

