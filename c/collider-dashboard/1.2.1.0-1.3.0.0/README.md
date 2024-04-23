# Comparing `tmp/collider_dashboard-1.2.1.0.tar.gz` & `tmp/collider_dashboard-1.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collider_dashboard-1.2.1.0.tar", max compression
+gzip compressed data, was "collider_dashboard-1.3.0.0.tar", max compression
```

## Comparing `collider_dashboard-1.2.1.0.tar` & `collider_dashboard-1.3.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-10-24 11:48:04.875018 collider_dashboard-1.2.1.0/LICENSE
--rw-r--r--   0        0        0     3395 2023-11-20 15:12:51.209426 collider_dashboard-1.2.1.0/README.md
--rw-r--r--   0        0        0     1362 2023-11-15 08:57:20.035624 collider_dashboard-1.2.1.0/collider_dashboard/__init__.py
--rw-r--r--   0        0        0     4086 2023-11-20 14:21:19.619257 collider_dashboard-1.2.1.0/collider_dashboard/__main__.py
--rw-r--r--   0        0        0   263006 2023-07-12 14:17:34.166444 collider_dashboard-1.2.1.0/collider_dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     3741 2023-07-12 14:17:34.166444 collider_dashboard-1.2.1.0/collider_dashboard/assets/style.css
--rw-r--r--   0        0        0        0 2023-10-31 10:48:04.031937 collider_dashboard-1.2.1.0/collider_dashboard/backend/__init__.py
--rw-r--r--   0        0        0    23698 2024-02-27 15:21:31.433442 collider_dashboard-1.2.1.0/collider_dashboard/backend/compute_globals.py
--rw-r--r--   0        0        0       71 2023-11-07 10:48:49.664970 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/__init__.py
--rw-r--r--   0        0        0    24744 2023-11-07 10:48:49.680971 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py
--rw-r--r--   0        0        0      214 2023-11-07 10:55:40.460126 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/disclaimer.md
--rw-r--r--   0        0        0     1458 2023-11-07 10:48:49.680971 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/dotdict.py
--rw-r--r--   0        0        0    11712 2023-11-07 10:48:49.680971 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py
--rw-r--r--   0        0        0    14291 2023-11-07 10:48:49.680971 collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/mystyle.py
--rw-r--r--   0        0        0    58560 2023-11-20 13:42:41.003136 collider_dashboard-1.2.1.0/collider_dashboard/backend/plot.py
--rw-r--r--   0        0        0     6799 2023-10-30 15:41:06.612463 collider_dashboard-1.2.1.0/collider_dashboard/backend/resonance.py
--rw-r--r--   0        0        0    12544 2023-11-20 14:29:36.814973 collider_dashboard-1.2.1.0/collider_dashboard/callbacks.py
--rw-r--r--   0        0        0     1648 2023-11-16 16:32:10.235791 collider_dashboard-1.2.1.0/collider_dashboard/dashboard.py
--rw-r--r--   0        0        0    21406 2023-11-02 15:35:17.252062 collider_dashboard-1.2.1.0/collider_dashboard/data/25ns_2464b_2452_1842_1821_236bpi_12inj_hybrid_converted.json
--rw-r--r--   0        0        0    21406 2024-02-21 12:52:56.845294 collider_dashboard-1.2.1.0/collider_dashboard/data/8b4e_1972b_1960_1178_1886_224bpi_12inj_800ns_bs200ns.json
--rw-r--r--   0        0        0 31122700 2024-01-24 09:55:11.869415 collider_dashboard-1.2.1.0/collider_dashboard/data/collider.json
--rw-r--r--   0        0        0      764 2023-11-20 14:22:51.013393 collider_dashboard-1.2.1.0/collider_dashboard/layout/__init__.py
--rw-r--r--   0        0        0     1990 2023-11-20 14:12:59.127295 collider_dashboard-1.2.1.0/collider_dashboard/layout/configuration.py
--rw-r--r--   0        0        0     1822 2023-10-30 14:14:19.025522 collider_dashboard-1.2.1.0/collider_dashboard/layout/filling.py
--rw-r--r--   0        0        0     5185 2023-10-30 14:14:34.581925 collider_dashboard-1.2.1.0/collider_dashboard/layout/footprint.py
--rw-r--r--   0        0        0     3896 2023-11-20 14:38:34.671795 collider_dashboard-1.2.1.0/collider_dashboard/layout/header.py
--rw-r--r--   0        0        0     2220 2023-11-20 14:30:08.139717 collider_dashboard-1.2.1.0/collider_dashboard/layout/knob.py
--rw-r--r--   0        0        0     1546 2023-10-30 14:43:13.835252 collider_dashboard-1.2.1.0/collider_dashboard/layout/main.py
--rw-r--r--   0        0        0     2385 2023-10-30 14:49:30.513242 collider_dashboard-1.2.1.0/collider_dashboard/layout/optics.py
--rw-r--r--   0        0        0    11416 2024-02-27 15:23:41.257017 collider_dashboard-1.2.1.0/collider_dashboard/layout/sanity.py
--rw-r--r--   0        0        0     3931 2023-10-30 14:51:24.176257 collider_dashboard-1.2.1.0/collider_dashboard/layout/separation.py
--rw-r--r--   0        0        0     4588 2023-11-08 10:41:12.594720 collider_dashboard-1.2.1.0/collider_dashboard/layout/separation_3D.py
--rw-r--r--   0        0        0     5274 2023-10-30 14:51:51.948994 collider_dashboard-1.2.1.0/collider_dashboard/layout/survey.py
--rw-r--r--   0        0        0     1586 2023-10-30 15:05:24.770559 collider_dashboard-1.2.1.0/collider_dashboard/layout/tables.py
--rw-r--r--   0        0        0        0 2023-07-12 14:17:34.166444 collider_dashboard-1.2.1.0/collider_dashboard/temp/.gitkeep
--rw-r--r--   0        0        0     1111 2024-02-27 15:41:30.062548 collider_dashboard-1.2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 collider_dashboard-1.2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-10-24 11:48:04.875018 collider_dashboard-1.3.0.0/LICENSE
+-rw-r--r--   0        0        0     3581 2024-04-23 15:22:44.060082 collider_dashboard-1.3.0.0/README.md
+-rw-r--r--   0        0        0     1362 2023-11-15 08:57:20.035624 collider_dashboard-1.3.0.0/collider_dashboard/__init__.py
+-rw-r--r--   0        0        0     4449 2024-04-23 15:21:15.025736 collider_dashboard-1.3.0.0/collider_dashboard/__main__.py
+-rw-r--r--   0        0        0   263006 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     3741 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/assets/style.css
+-rw-r--r--   0        0        0        0 2023-10-31 10:48:04.031937 collider_dashboard-1.3.0.0/collider_dashboard/backend/__init__.py
+-rw-r--r--   0        0        0    23874 2024-04-23 15:18:16.757038 collider_dashboard-1.3.0.0/collider_dashboard/backend/compute_globals.py
+-rw-r--r--   0        0        0       71 2023-11-07 10:48:49.664970 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/__init__.py
+-rw-r--r--   0        0        0    24744 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py
+-rw-r--r--   0        0        0      214 2023-11-07 10:55:40.460126 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/disclaimer.md
+-rw-r--r--   0        0        0     1458 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/dotdict.py
+-rw-r--r--   0        0        0    11712 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py
+-rw-r--r--   0        0        0    14291 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/mystyle.py
+-rw-r--r--   0        0        0    58560 2023-11-20 13:42:41.003136 collider_dashboard-1.3.0.0/collider_dashboard/backend/plot.py
+-rw-r--r--   0        0        0     6799 2023-10-30 15:41:06.612463 collider_dashboard-1.3.0.0/collider_dashboard/backend/resonance.py
+-rw-r--r--   0        0        0    12620 2024-04-23 15:15:30.012642 collider_dashboard-1.3.0.0/collider_dashboard/callbacks.py
+-rw-r--r--   0        0        0     1716 2024-04-23 15:18:45.249790 collider_dashboard-1.3.0.0/collider_dashboard/dashboard.py
+-rw-r--r--   0        0        0    21406 2023-11-02 15:35:17.252062 collider_dashboard-1.3.0.0/collider_dashboard/data/25ns_2464b_2452_1842_1821_236bpi_12inj_hybrid_converted.json
+-rw-r--r--   0        0        0    21406 2024-02-21 12:52:56.845294 collider_dashboard-1.3.0.0/collider_dashboard/data/8b4e_1972b_1960_1178_1886_224bpi_12inj_800ns_bs200ns.json
+-rw-r--r--   0        0        0 31122700 2024-01-24 09:55:11.869415 collider_dashboard-1.3.0.0/collider_dashboard/data/collider.json
+-rw-r--r--   0        0        0      764 2023-11-20 14:22:51.013393 collider_dashboard-1.3.0.0/collider_dashboard/layout/__init__.py
+-rw-r--r--   0        0        0     1990 2023-11-20 14:12:59.127295 collider_dashboard-1.3.0.0/collider_dashboard/layout/configuration.py
+-rw-r--r--   0        0        0     1822 2023-10-30 14:14:19.025522 collider_dashboard-1.3.0.0/collider_dashboard/layout/filling.py
+-rw-r--r--   0        0        0     5185 2023-10-30 14:14:34.581925 collider_dashboard-1.3.0.0/collider_dashboard/layout/footprint.py
+-rw-r--r--   0        0        0     3896 2023-11-20 14:38:34.671795 collider_dashboard-1.3.0.0/collider_dashboard/layout/header.py
+-rw-r--r--   0        0        0     2220 2023-11-20 14:30:08.139717 collider_dashboard-1.3.0.0/collider_dashboard/layout/knob.py
+-rw-r--r--   0        0        0     1546 2023-10-30 14:43:13.835252 collider_dashboard-1.3.0.0/collider_dashboard/layout/main.py
+-rw-r--r--   0        0        0     2385 2023-10-30 14:49:30.513242 collider_dashboard-1.3.0.0/collider_dashboard/layout/optics.py
+-rw-r--r--   0        0        0    11401 2024-04-23 15:13:00.436694 collider_dashboard-1.3.0.0/collider_dashboard/layout/sanity.py
+-rw-r--r--   0        0        0     3931 2023-10-30 14:51:24.176257 collider_dashboard-1.3.0.0/collider_dashboard/layout/separation.py
+-rw-r--r--   0        0        0     4588 2023-11-08 10:41:12.594720 collider_dashboard-1.3.0.0/collider_dashboard/layout/separation_3D.py
+-rw-r--r--   0        0        0     5274 2023-10-30 14:51:51.948994 collider_dashboard-1.3.0.0/collider_dashboard/layout/survey.py
+-rw-r--r--   0        0        0     1586 2023-10-30 15:05:24.770559 collider_dashboard-1.3.0.0/collider_dashboard/layout/tables.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/temp/.gitkeep
+-rw-r--r--   0        0        0     1111 2024-04-23 15:23:35.413434 collider_dashboard-1.3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 collider_dashboard-1.3.0.0/PKG-INFO
```

### Comparing `collider_dashboard-1.2.1.0/LICENSE` & `collider_dashboard-1.3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/README.md` & `collider_dashboard-1.3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,23 +35,24 @@
 ```
 
 ## Usage
 
 For personal usage, the simplest way to use the dashboard is to run the package as a development server from the command line, providing a few arguments:
 
 ```bash
-python -m collider_dashboard --collider-path path_to_collider.json --filling-path path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss --debug
+python -m collider_dashboard --collider-path path_to_collider.json --filling-path path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss --type-particles proton --debug
 ```
 
 - `--collider-path`, or `-c`, sets the path to the collider configuration file. Default value to the path of a dummy collider used for testing.
 - `--filling-path`, or `-f`, sets the path to the filling scheme, instead of using the one in the collider configuration file. Optional.
 - `--port`, or `-p`, sets the port on which the dashboard will be deployed. Default value to `8080``.
 - `--force-reload`, or `-r`,  sets a boolean indicating whether the collider dashboard data should be reloaded if already existing. Optional.
 - `--ignore-footprint`, or `-i`, sets a boolean indicating whether the footprint should be ignored to gain computation time. Optional.
 - `--full-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey tables should be computed fully (not removing duplicates and entry/exit elements), at the expense of computation time. Optional.
+- `--type-particles`, or `-a`, sets the type of particles to be used for the collider. Default value to `proton`.
 - `--debug`, or `-d`, sets a boolean indicating whether the dashboard should be run in debug mode. Optional.
 
 After computing some temporary variables (this may take a while the first time), this will deploy a local server and open the dashboard in a browser window.
 
 Alternatively, one can import the dashboard as a module and use it in a custom script:
 
 ```python
@@ -61,14 +62,15 @@
 app, server = build_app(path_to_collider.json, 
                         path_scheme=path_to_scheme.json, 
                         port=8080, 
                         force_reload=False, 
                         ignore_footprint=False, 
                         debug = False, 
                         simplify_tw=True
+                        type_particles='proton'
                 )
 ```
 
 The dashboard can then be deployed e.g. with gunicorn:
 
 ```bash
 gunicorn my-awesome-dashboard:server -b :8080
```

#### html2text {}

```diff
@@ -10,31 +10,33 @@
 will install the required packages and build the application. If you haven't
 done it already, it is recommended to prebuild the Xsuite kernel to gain some
 computation time: ```bash xsuite-prebuild ``` ## Usage For personal usage, the
 simplest way to use the dashboard is to run the package as a development server
 from the command line, providing a few arguments: ```bash python -
 m collider_dashboard --collider-path path_to_collider.json --filling-path
 path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss
---debug ``` - `--collider-path`, or `-c`, sets the path to the collider
-configuration file. Default value to the path of a dummy collider used for
-testing. - `--filling-path`, or `-f`, sets the path to the filling scheme,
-instead of using the one in the collider configuration file. Optional. - `--
-port`, or `-p`, sets the port on which the dashboard will be deployed. Default
-value to `8080``. - `--force-reload`, or `-r`, sets a boolean indicating
-whether the collider dashboard data should be reloaded if already existing.
-Optional. - `--ignore-footprint`, or `-i`, sets a boolean indicating whether
-the footprint should be ignored to gain computation time. Optional. - `--full-
-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey tables
-should be computed fully (not removing duplicates and entry/exit elements), at
-the expense of computation time. Optional. - `--debug`, or `-d`, sets a boolean
-indicating whether the dashboard should be run in debug mode. Optional. After
-computing some temporary variables (this may take a while the first time), this
-will deploy a local server and open the dashboard in a browser window.
-Alternatively, one can import the dashboard as a module and use it in a custom
-script: ```python # my-awesome-dashboard.py from collider_dashboard import
-build_app app, server = build_app(path_to_collider.json,
-path_scheme=path_to_scheme.json, port=8080, force_reload=False,
-ignore_footprint=False, debug = False, simplify_tw=True ) ``` The dashboard can
-then be deployed e.g. with gunicorn: ```bash gunicorn my-awesome-dashboard:
-server -b :8080 ``` Note that, as the dashboard deals with global variables, it
-is not thread-safe. It is therefore recommended to run it with a single worker
-(it's the case by default).
+--type-particles proton --debug ``` - `--collider-path`, or `-c`, sets the path
+to the collider configuration file. Default value to the path of a dummy
+collider used for testing. - `--filling-path`, or `-f`, sets the path to the
+filling scheme, instead of using the one in the collider configuration file.
+Optional. - `--port`, or `-p`, sets the port on which the dashboard will be
+deployed. Default value to `8080``. - `--force-reload`, or `-r`, sets a boolean
+indicating whether the collider dashboard data should be reloaded if already
+existing. Optional. - `--ignore-footprint`, or `-i`, sets a boolean indicating
+whether the footprint should be ignored to gain computation time. Optional. -
+`--full-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey
+tables should be computed fully (not removing duplicates and entry/exit
+elements), at the expense of computation time. Optional. - `--type-particles`,
+or `-a`, sets the type of particles to be used for the collider. Default value
+to `proton`. - `--debug`, or `-d`, sets a boolean indicating whether the
+dashboard should be run in debug mode. Optional. After computing some temporary
+variables (this may take a while the first time), this will deploy a local
+server and open the dashboard in a browser window. Alternatively, one can
+import the dashboard as a module and use it in a custom script: ```python # my-
+awesome-dashboard.py from collider_dashboard import build_app app, server =
+build_app(path_to_collider.json, path_scheme=path_to_scheme.json, port=8080,
+force_reload=False, ignore_footprint=False, debug = False, simplify_tw=True
+type_particles='proton' ) ``` The dashboard can then be deployed e.g. with
+gunicorn: ```bash gunicorn my-awesome-dashboard:server -b :8080 ``` Note that,
+as the dashboard deals with global variables, it is not thread-safe. It is
+therefore recommended to run it with a single worker (it's the case by
+default).
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/__init__.py` & `collider_dashboard-1.3.0.0/collider_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/__main__.py` & `collider_dashboard-1.3.0.0/collider_dashboard/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def main(
     path_collider,
     path_scheme=None,
     port=8080,
     force_reload=False,
     ignore_footprint=False,
     simplify_tw=True,
+    type_particles = 'proton',
     debug=False,
 ):
 
     # Log the initial configuration
     logging.info("Launching app with the following parameters:")
     logging.info(f"Collider path: {path_collider}")
     logging.info(f"Filling path: {path_scheme}")
@@ -39,14 +40,16 @@
     # Build and run the app
     app, _ = build_app(
         path_collider,
         path_scheme=path_scheme,
         force_reload=force_reload,
         ignore_footprint=ignore_footprint,
         simplify_tw=simplify_tw,
+        type_particles=type_particles,
+        
     )  # server not needed for local deployment
     app.run_server(debug=debug, host="0.0.0.0", port=port)
 
 
 if __name__ == "__main__":
 
     # Get the example collider path
@@ -110,31 +113,41 @@
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         help="Launch the app in debugging mode.",
         required=False,
     )
+    parser.add_argument(
+        "-a",
+        "--type-particles",
+        type=str,
+        help="Types of particles to consider (proton, lead).",
+        required=False,
+        default='proton',
+    )
 
     args = parser.parse_args()
     collider_path = args.collider_path
     path_scheme = args.filling_path
     port = args.port
     force_reload = args.force_reload
     ignore_footprint = args.ignore_footprint
     simplify_tw = not args.full_twiss
+    type_particles = args.type_particles
     debug = args.debug
 
     # Warn that the default collider is used if needed
     if collider_path == example_collider_path:
         logging.warning("No collider path was provided. Launching example collider.")
 
     # Launch the app
     main(
         collider_path,
         path_scheme=path_scheme,
         port=port,
         force_reload=force_reload,
         ignore_footprint=ignore_footprint,
         simplify_tw=simplify_tw,
+        type_particles=type_particles,
         debug=debug,
     )
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/assets/favicon.ico` & `collider_dashboard-1.3.0.0/collider_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/assets/style.css` & `collider_dashboard-1.3.0.0/collider_dashboard/assets/style.css`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/compute_globals.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/compute_globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 # ==================================================================================================
 # --- Functions initialize all global variables
 # ==================================================================================================
 
 
 def init_from_collider(
-    path_collider, path_scheme=None, force_reload=False, ignore_footprint=False, simplify_tw=True
+    path_collider, path_scheme=None, force_reload=False, ignore_footprint=False, simplify_tw=True, type_particles = 'proton'
 ):
     """
     Initializes a collider from a JSON file and computes global variables from collider checks.
 
     Args:
         path_collider (str): Path to the JSON file containing the collider definition.
         force_reload (bool, optional): If False, tries to to load the global variables
@@ -88,15 +88,15 @@
         else:
             logging.warning("The collider file does not contain metadata. Using default values.")
 
         # Compute collider checks
         logging.info("Computing collider checks.")
         collider_check_with_bb = ColliderCheck(collider, path_filling_scheme=path_scheme)
         collider_check_without_bb = ColliderCheck(
-            collider_without_bb, path_filling_scheme=path_scheme
+            collider_without_bb, path_filling_scheme=path_scheme, type_particles = 'proton'
         )
 
         # Compute global variables
         dic_without_bb, dic_with_bb = compute_global_variables_from_collider_checks(
             collider_check_with_bb,
             collider_check_without_bb,
             path_pickle=path_pickle,
@@ -199,14 +199,15 @@
 
         # Get emittances
         nemitt_x = collider_check.nemitt_x
         nemitt_y = collider_check.nemitt_y
 
         # Get energy
         energy = collider_check.energy
+        cross_section = collider_check.cross_section
 
         # Get the beam-beam schedule
         logging.info("Computing beam-beam schedule.")
         patt = FillingPattern.from_json(collider_check.path_filling_scheme)
         patt.compute_beam_beam_schedule(n_lr_per_side=26)
         bbs = patt.b1.bb_schedule
 
@@ -223,14 +224,15 @@
         i_bunch_b1 = None
         i_bunch_b2 = None
         bbs = None
         polarity_alice = None
         polarity_lhcb = None
         configuration_str = None
         energy = None
+        cross_section = None
 
         # Get emittance for the computation of the normalized separation
         logging.warning("No configuration file provided, using default values for emittances.")
         nemitt_x = 2.2e-6
         nemitt_y = 2.2e-6
 
     # Get elements of the line (only done for b1, should be identical for b2)
@@ -353,14 +355,15 @@
         "i_bunch_b2": i_bunch_b2,
         "bbs": bbs,
         "footprint_b1": (array_qx1, array_qy1),
         "footprint_b2": (array_qx2, array_qy2),
         "polarity_alice": polarity_alice,
         "polarity_lhcb": polarity_lhcb,
         "energy": energy,
+        "cross_section": cross_section,
         "configuration_str": configuration_str,
         "dic_knob_str": dic_knob_str,
     }
 
     return dic_global_var
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/dotdict.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/dotdict.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/fillingpatterns/mystyle.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/mystyle.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/plot.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/plot.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/backend/resonance.py` & `collider_dashboard-1.3.0.0/collider_dashboard/backend/resonance.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/callbacks.py` & `collider_dashboard-1.3.0.0/collider_dashboard/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,26 @@
         dic_with_bb["dic_tw_b2"],
         dic_with_bb["l_lumi"],
         dic_with_bb["array_b1"],
         dic_with_bb["array_b2"],
         dic_with_bb["polarity_alice"],
         dic_with_bb["polarity_lhcb"],
         dic_with_bb["energy"],
+        dic_with_bb["cross_section"],
     )
     sanity_before_beam_beam = return_sanity_layout(
         dic_without_bb["dic_tw_b1"],
         dic_without_bb["dic_tw_b2"],
         dic_without_bb["l_lumi"],
         dic_without_bb["array_b1"],
         dic_without_bb["array_b2"],
         dic_without_bb["polarity_alice"],
         dic_without_bb["polarity_lhcb"],
         dic_with_bb["energy"],
+        dic_with_bb["cross_section"],
     )
     tabs_sanity = dmc.Tabs(
         [
             dmc.TabsList(
                 [
                     dmc.Tab(
                         "Before beam-beam",
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/dashboard.py` & `collider_dashboard-1.3.0.0/collider_dashboard/dashboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
 # ==================================================================================================
 # --- Load global variables and build app
 # ==================================================================================================
 
 
 def build_app(
-    path_collider, path_scheme=None, force_reload=False, ignore_footprint=False, simplify_tw=True
+    path_collider, path_scheme=None, force_reload=False, ignore_footprint=False, simplify_tw=True, type_particles = 'proton'
 ):
 
     # Load dashboard variables
     dic_without_bb, dic_with_bb = compute_globals.init_from_collider(
         path_collider,
         path_scheme=path_scheme,
         force_reload=force_reload,
         ignore_footprint=ignore_footprint,
         simplify_tw=simplify_tw,
+        type_particles = type_particles,
     )
 
     #################### App ####################
     logging.info("Defining app")
     app = Dash(
         __name__,
         title="Collider dashboard",
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/data/collider.json` & `collider_dashboard-1.3.0.0/collider_dashboard/data/collider.json`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/__init__.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/configuration.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/configuration.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/filling.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/filling.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/footprint.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/footprint.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/header.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/header.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/knob.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/knob.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/main.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/main.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/optics.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/optics.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/sanity.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/sanity.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     dic_tw_b2,
     l_lumi,
     array_b1,
     array_b2,
     polarity_alice,
     polarity_lhcb,
     energy,
+    cross_section_PU = 81e-27,
 ):
     """
     Returns the layout for the sanity check page of the dashboard.
 
     Args:
         dic_tw_b1 : dict
             A twiss dictionary for beam 1.
@@ -197,30 +198,28 @@
                 ),
                 html.Td(f"{l_lumi[3]:.3e}"),
             ]
         )
         body_4 = [html.Tbody([row_lumi])]
         table_4 = dmc.Table(header_3 + body_4)
 
-        # Pile-up
-        cross_section = 81e-27
         # Assert that the arrays have the required length, and do the convolution to get number of collisions
         assert len(array_b1) == len(array_b2) == 3564
         n_collisions_ip1_and_5 = array_b1 @ array_b2
         n_collisions_ip2 = np.roll(array_b1, 891) @ array_b2
         n_collisions_ip8 = np.roll(array_b1, 2670) @ array_b2
         l_n_collisions = [
             n_collisions_ip1_and_5,
             n_collisions_ip2,
             n_collisions_ip1_and_5,
             n_collisions_ip8,
         ]
         n_turn_per_second = 1 / dic_tw_b1["T_rev0"]
         l_PU = [
-            lumi / n_col * cross_section / n_turn_per_second
+            lumi / n_col * cross_section_PU / n_turn_per_second
             for lumi, n_col in zip(l_lumi, l_n_collisions)
         ]
 
         # PU
         header_4 = [
             html.Thead(
                 html.Tr(
```

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/separation.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/separation.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/separation_3D.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/separation_3D.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/survey.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/survey.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/collider_dashboard/layout/tables.py` & `collider_dashboard-1.3.0.0/collider_dashboard/layout/tables.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.2.1.0/pyproject.toml` & `collider_dashboard-1.3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "collider-dashboard"
-version = "1.2.1.0"
+version = "1.3.0.0"
 description = "A Dash application to visualize the observables and parameters of a collider built and configured with Xsuite."
 authors = ["Colas Droin <colas.noe.droin@cern.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ColasDroin/simulation-dashboard"
 packages = [
     { include = "collider_dashboard" },
```

### Comparing `collider_dashboard-1.2.1.0/PKG-INFO` & `collider_dashboard-1.3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: collider-dashboard
-Version: 1.2.1.0
+Version: 1.3.0.0
 Summary: A Dash application to visualize the observables and parameters of a collider built and configured with Xsuite.
 Home-page: https://github.com/ColasDroin/simulation-dashboard
 License: MIT
 Author: Colas Droin
 Author-email: colas.noe.droin@cern.ch
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: collider-check (>=0.1.7,<0.2.0)
 Requires-Dist: dash (>=2.14.1,<3.0.0)
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
 Requires-Dist: dash-mantine-components (>=0.12.1,<0.13.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
@@ -60,23 +61,24 @@
 ```
 
 ## Usage
 
 For personal usage, the simplest way to use the dashboard is to run the package as a development server from the command line, providing a few arguments:
 
 ```bash
-python -m collider_dashboard --collider-path path_to_collider.json --filling-path path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss --debug
+python -m collider_dashboard --collider-path path_to_collider.json --filling-path path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss --type-particles proton --debug
 ```
 
 - `--collider-path`, or `-c`, sets the path to the collider configuration file. Default value to the path of a dummy collider used for testing.
 - `--filling-path`, or `-f`, sets the path to the filling scheme, instead of using the one in the collider configuration file. Optional.
 - `--port`, or `-p`, sets the port on which the dashboard will be deployed. Default value to `8080``.
 - `--force-reload`, or `-r`,  sets a boolean indicating whether the collider dashboard data should be reloaded if already existing. Optional.
 - `--ignore-footprint`, or `-i`, sets a boolean indicating whether the footprint should be ignored to gain computation time. Optional.
 - `--full-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey tables should be computed fully (not removing duplicates and entry/exit elements), at the expense of computation time. Optional.
+- `--type-particles`, or `-a`, sets the type of particles to be used for the collider. Default value to `proton`.
 - `--debug`, or `-d`, sets a boolean indicating whether the dashboard should be run in debug mode. Optional.
 
 After computing some temporary variables (this may take a while the first time), this will deploy a local server and open the dashboard in a browser window.
 
 Alternatively, one can import the dashboard as a module and use it in a custom script:
 
 ```python
@@ -86,14 +88,15 @@
 app, server = build_app(path_to_collider.json, 
                         path_scheme=path_to_scheme.json, 
                         port=8080, 
                         force_reload=False, 
                         ignore_footprint=False, 
                         debug = False, 
                         simplify_tw=True
+                        type_particles='proton'
                 )
 ```
 
 The dashboard can then be deployed e.g. with gunicorn:
 
 ```bash
 gunicorn my-awesome-dashboard:server -b :8080
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: collider-dashboard Version: 1.2.1.0 Summary: A Dash
+Metadata-Version: 2.1 Name: collider-dashboard Version: 1.3.0.0 Summary: A Dash
 application to visualize the observables and parameters of a collider built and
 configured with Xsuite. Home-page: https://github.com/ColasDroin/simulation-
 dashboard License: MIT Author: Colas Droin Author-email:
 colas.noe.droin@cern.ch Requires-Python: >=3.10,<3.13 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: argparse (>=1.4.0,<2.0.0) Requires-
-Dist: collider-check (>=0.1.7,<0.2.0) Requires-Dist: dash (>=2.14.1,<3.0.0)
-Requires-Dist: dash-iconify (>=0.1.2,<0.2.0) Requires-Dist: dash-mantine-
-components (>=0.12.1,<0.13.0) Requires-Dist: numpy (>=1.26.1,<2.0.0) Requires-
-Dist: pandas (>=2.1.2,<3.0.0) Requires-Dist: seaborn (>=0.13.0,<0.14.0)
-Requires-Dist: xsuite (>=0.6.0,<0.7.0) Project-URL: Repository, https://
-github.com/ColasDroin/simulation-dashboard Description-Content-Type: text/
-markdown # Collider Dashboard
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: argparse (>=1.4.0,<2.0.0) Requires-Dist: collider-check
+(>=0.1.7,<0.2.0) Requires-Dist: dash (>=2.14.1,<3.0.0) Requires-Dist: dash-
+iconify (>=0.1.2,<0.2.0) Requires-Dist: dash-mantine-components
+(>=0.12.1,<0.13.0) Requires-Dist: numpy (>=1.26.1,<2.0.0) Requires-Dist: pandas
+(>=2.1.2,<3.0.0) Requires-Dist: seaborn (>=0.13.0,<0.14.0) Requires-Dist:
+xsuite (>=0.6.0,<0.7.0) Project-URL: Repository, https://github.com/ColasDroin/
+simulation-dashboard Description-Content-Type: text/markdown # Collider
+Dashboard
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/_l_i_c_e_n_s_e_/_M_I_T_/_b_l_u_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/
  _P_a_c_k_a_g_e_%_2_0_M_a_n_a_g_e_r_/_P_o_e_t_r_y_/_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/_D_a_s_h_/_2_._1_4_._1_/_g_r_e_e_n_]
 _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/_C_o_d_e_%_2_0_s_t_y_l_e_/_B_l_a_c_k_/_b_l_a_c_k_][https://badgen.net/github/
    release/colasdroin/collider-dashboard][https://badgen.net/github/commits/
                         colasdroin/collider-dashboard]
 A Dash application to visualize the observables and parameters of a collider
 built and configured with Xsuite. ## Installation The dashboard can be
@@ -24,31 +25,33 @@
 will install the required packages and build the application. If you haven't
 done it already, it is recommended to prebuild the Xsuite kernel to gain some
 computation time: ```bash xsuite-prebuild ``` ## Usage For personal usage, the
 simplest way to use the dashboard is to run the package as a development server
 from the command line, providing a few arguments: ```bash python -
 m collider_dashboard --collider-path path_to_collider.json --filling-path
 path_to_scheme.json --port 8080 --force-reload --ignore-footprint --full-twiss
---debug ``` - `--collider-path`, or `-c`, sets the path to the collider
-configuration file. Default value to the path of a dummy collider used for
-testing. - `--filling-path`, or `-f`, sets the path to the filling scheme,
-instead of using the one in the collider configuration file. Optional. - `--
-port`, or `-p`, sets the port on which the dashboard will be deployed. Default
-value to `8080``. - `--force-reload`, or `-r`, sets a boolean indicating
-whether the collider dashboard data should be reloaded if already existing.
-Optional. - `--ignore-footprint`, or `-i`, sets a boolean indicating whether
-the footprint should be ignored to gain computation time. Optional. - `--full-
-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey tables
-should be computed fully (not removing duplicates and entry/exit elements), at
-the expense of computation time. Optional. - `--debug`, or `-d`, sets a boolean
-indicating whether the dashboard should be run in debug mode. Optional. After
-computing some temporary variables (this may take a while the first time), this
-will deploy a local server and open the dashboard in a browser window.
-Alternatively, one can import the dashboard as a module and use it in a custom
-script: ```python # my-awesome-dashboard.py from collider_dashboard import
-build_app app, server = build_app(path_to_collider.json,
-path_scheme=path_to_scheme.json, port=8080, force_reload=False,
-ignore_footprint=False, debug = False, simplify_tw=True ) ``` The dashboard can
-then be deployed e.g. with gunicorn: ```bash gunicorn my-awesome-dashboard:
-server -b :8080 ``` Note that, as the dashboard deals with global variables, it
-is not thread-safe. It is therefore recommended to run it with a single worker
-(it's the case by default).
+--type-particles proton --debug ``` - `--collider-path`, or `-c`, sets the path
+to the collider configuration file. Default value to the path of a dummy
+collider used for testing. - `--filling-path`, or `-f`, sets the path to the
+filling scheme, instead of using the one in the collider configuration file.
+Optional. - `--port`, or `-p`, sets the port on which the dashboard will be
+deployed. Default value to `8080``. - `--force-reload`, or `-r`, sets a boolean
+indicating whether the collider dashboard data should be reloaded if already
+existing. Optional. - `--ignore-footprint`, or `-i`, sets a boolean indicating
+whether the footprint should be ignored to gain computation time. Optional. -
+`--full-twiss`, or `-t`, sets a boolean indicating whether the Twiss/Survey
+tables should be computed fully (not removing duplicates and entry/exit
+elements), at the expense of computation time. Optional. - `--type-particles`,
+or `-a`, sets the type of particles to be used for the collider. Default value
+to `proton`. - `--debug`, or `-d`, sets a boolean indicating whether the
+dashboard should be run in debug mode. Optional. After computing some temporary
+variables (this may take a while the first time), this will deploy a local
+server and open the dashboard in a browser window. Alternatively, one can
+import the dashboard as a module and use it in a custom script: ```python # my-
+awesome-dashboard.py from collider_dashboard import build_app app, server =
+build_app(path_to_collider.json, path_scheme=path_to_scheme.json, port=8080,
+force_reload=False, ignore_footprint=False, debug = False, simplify_tw=True
+type_particles='proton' ) ``` The dashboard can then be deployed e.g. with
+gunicorn: ```bash gunicorn my-awesome-dashboard:server -b :8080 ``` Note that,
+as the dashboard deals with global variables, it is not thread-safe. It is
+therefore recommended to run it with a single worker (it's the case by
+default).
```

