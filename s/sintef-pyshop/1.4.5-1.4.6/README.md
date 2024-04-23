# Comparing `tmp/sintef-pyshop-1.4.5.tar.gz` & `tmp/sintef_pyshop-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.5.tar", last modified: Wed Oct  4 09:16:31 2023, max compression
+gzip compressed data, was "sintef_pyshop-1.4.6.tar", last modified: Tue Apr 23 14:26:49 2024, max compression
```

## Comparing `sintef-pyshop-1.4.5.tar` & `sintef_pyshop-1.4.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.248174 sintef-pyshop-1.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6203 2023-10-04 09:16:31.248174 sintef-pyshop-1.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.243174 sintef-pyshop-1.4.5/pyshop/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.244174 sintef-pyshop-1.4.5/pyshop/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/helpers/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/helpers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/helpers/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.245174 sintef-pyshop-1.4.5/pyshop/lp_model/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/lp_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/lp_model/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/lp_model/lp_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10661 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/lp_model/row.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/lp_model/var.py
--rw-rw-rw-   0 root         (0) root         (0)    13872 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shop_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.246174 sintef-pyshop-1.4.5/pyshop/shopcore/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/command_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    24862 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/model_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    13037 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/script_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    15331 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/shop_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-04 09:16:31.248174 sintef-pyshop-1.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-10-03 12:59:03.000000 sintef-pyshop-1.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.247174 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6203 2023-10-04 09:16:31.000000 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-10-04 09:16:31.000000 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-04 09:16:31.000000 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-10-04 09:16:31.000000 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-10-04 09:16:31.000000 sintef-pyshop-1.4.5/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 09:16:31.248174 sintef-pyshop-1.4.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/tests/test_helpers_command.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/tests/test_helpers_time.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2023-09-28 12:53:49.000000 sintef-pyshop-1.4.5/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.621832 sintef_pyshop-1.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7891 2024-04-23 14:26:49.620832 sintef_pyshop-1.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6640 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.556831 sintef_pyshop-1.4.6/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.561831 sintef_pyshop-1.4.6/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.565831 sintef_pyshop-1.4.6/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    14630 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.585831 sintef_pyshop-1.4.6/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    25028 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13037 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15331 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 14:26:49.621832 sintef_pyshop-1.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.620832 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7891 2024-04-23 14:26:49.000000 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2024-04-23 14:26:49.000000 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 14:26:49.000000 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-23 14:26:49.000000 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-23 14:26:49.000000 sintef_pyshop-1.4.6/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:26:49.615832 sintef_pyshop-1.4.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-04-23 08:45:47.000000 sintef_pyshop-1.4.6/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.5/LICENSE` & `sintef_pyshop-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/PKG-INFO` & `sintef_pyshop-1.4.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: sintef-pyshop
-Version: 1.4.5
-Summary: Python interface to SHOP
-Home-page: http://www.sintef.no/programvare/SHOP
-Author: SINTEF Energy Research
-Author-email: support.energy@sintef.no
-License: MIT
-Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
-Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
-Project-URL: Tracker, https://shop.sintef.energy/tickets
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: graphviz
-Requires-Dist: pybind11
-Requires-Dist: requests
-
 # pyshop
 
 Status:
 
 [![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
 [![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
 [![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
@@ -79,23 +46,23 @@
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
 
-- cplex2010.dll
-- shop_cplex_interface.dll
-- shop_pybind.pyd
+- `cplex2010.dll`
+- `shop_cplex_interface.dll`
+- `shop_pybind.pyd`
 
 Linux:
 
-- libcplex2010.so
-- shop_cplex_interface.so
-- shop_pybind.so
+- `libcplex2010.so`
+- `shop_cplex_interface.so`
+- `shop_pybind.so`
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
 
 The SHOP license file, `SHOP_license.dat`, must always be located in the directory specified by the environment variable `ICC_COMMAND_PATH`. The `ICC_COMMAND_PATH` can be added as a persistent environment variable in the regular ways, or it can be set by pyshop on a session basis. If the keyword argument `license_path` is specified when creating an instance of the ShopSession class (see step 4), the environment variable is overridden in the local environment of the executing process. If SHOP complains about not finding the license file, it is likely an issue with the `ICC_COMMAND_PATH` not being correctly specified.
 
@@ -105,14 +72,35 @@
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
 
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
 
-    #Set time resolution
-    #Build topolgy
-    #Add temporal input
-    #Run model
-    #Retreive results
-
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
+
+## Visual Studio Code Dev Containers
+
+[Visual Studio Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers) lets you run a fully functional development environment using Docker and Visual Studio Code. This might simplyfy setting up pyshop for new users. Follow the guide below to setup the devcontainer for pyshop.
+
+### Installation
+
+Install the following dependencies:
+
+1. Install the code editor called [Visual Studio Code](https://code.visualstudio.com/Download). Visual Studio Code is free
+2. Install a Docker GUI: [Docker desktop](https://www.docker.com/products/docker-desktop/) (might require a paid license depending on your organization), or a free alternative called [Podman](https://podman.io/)
+
+### Setup
+
+1. Create a folder called `.devcontainer` in your root directory with a file called `devcontainer.json`. Your folder structure should look like the example below:
+
+   ![Devcontainer folder setup](docs/images/devcontainer-folder.png)
+
+2. Copy and paste the contents of [devcontainer.json](.devcontainer/devcontainer.json) into your `devcontainer.json` file.
+3. Create a folder called `bin` in your root directory and add the following files: `libcplex2010.so`, `shop_cplex_interface.so`, your shop license e.g `SHOP_license.dat`, shop pybind e.g `shop_pybind.cpython-312-x86_64-linux-gnu.so`. Your bin folder should now look like:
+
+   ![Binary folder with the required files](docs/images/bin-folder.png)
+
+4. Open your project using the devcontainer config files by running the command:
+   ![Searching for devcontainer command](docs/images/dev-containers-reopen.png)
+
+More in depth guides on how to customize devcontainers can be found in the [devcontainer documentation](https://code.visualstudio.com/docs/devcontainers/create-dev-container)
```

### Comparing `sintef-pyshop-1.4.5/pyshop/helpers/commands.py` & `sintef_pyshop-1.4.6/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/helpers/time.py` & `sintef_pyshop-1.4.6/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/helpers/timeseries.py` & `sintef_pyshop-1.4.6/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/helpers/typing_annotations.py` & `sintef_pyshop-1.4.6/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/lp_model/index.py` & `sintef_pyshop-1.4.6/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/lp_model/lp_model.py` & `sintef_pyshop-1.4.6/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/lp_model/row.py` & `sintef_pyshop-1.4.6/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/lp_model/var.py` & `sintef_pyshop-1.4.6/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/shop_runner.py` & `sintef_pyshop-1.4.6/pyshop/shop_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,19 +77,22 @@
             else:
                 sys.path.insert(1, os.environ['ICC_COMMAND_PATH'])
 
             import shop_pybind as pb
 
             silent_console = silent
             silent_log = suppress_log
-            if log_file:
-                self.shop_api = pb.ShopCore(silent_console, silent_log, log_file, log_gets)
-            else:
-                self.shop_api = pb.ShopCore(silent_console, silent_log)
 
+            try:
+                settings = {"silent_console":silent_console,"silent_log":silent_log,"log_file":log_file,"log_gets":log_gets, "license_path":license_path}
+                self.shop_api = pb.ShopCore(settings)
+            #Backwards compatibility before license path could be set through ShopCore constructor
+            except TypeError:
+                self.shop_api = pb.ShopCore(silent_console, silent_log, log_file, log_gets)
+        
             # Override where SHOP will look for solver dlls
             if solver_path:
                 self.shop_api.OverrideDllPath(solver_path)
 
         self.model = ModelBuilderType(self.shop_api)
         self.lp_model = LpModelBuilder(self)
         self._commands = {x.replace(' ', '_'): x for x in self.shop_api.GetCommandTypesInSystem()}
@@ -212,14 +215,24 @@
     def dump_yaml(self, file_path:str='', input_only:bool=True, compress_txy:bool=True, compress_connection:bool=True) -> str:
         if file_path != '':
             self.shop_api.DumpYamlCase(file_path, input_only, compress_txy, compress_connection)
             return f'YAML case is dumped to the provided file path: "{file_path}"'
         else:
             return self.shop_api.DumpYamlString(input_only, compress_txy, compress_connection)
 
+    def load_json(self, json_file_path:str='', json_string:str='') -> None:
+        if json_file_path != '' and json_string != '':
+            raise ValueError('Provide either a file path or a json string, not both')
+        if json_file_path != '':
+            with open(json_file_path, 'r', encoding='utf8') as f:
+                json_file_string = f.read()
+                self.shop_api.ReadJsonString(json_file_string)
+        elif json_string != '':
+            self.shop_api.ReadJsonString(json_string)
+
     def dump_pyshop(self, file_path:str, static_data_only:bool=False) -> None:
         
         write_pyshop_model_file(file_path,self.shop_api,static_data_only)
 
     def run_command_file(self, folder:str, command_file:str, break_before_opt:bool = False, skip_reading_input:bool = False) -> None:
         
         with open(os.path.join(folder, command_file), 'r', encoding='iso-8859-1') as run_file:
```

### Comparing `sintef-pyshop-1.4.5/pyshop/shopcore/command_builder.py` & `sintef_pyshop-1.4.6/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/shopcore/model_builder.py` & `sintef_pyshop-1.4.6/pyshop/shopcore/model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,19 @@
     def __dir__(self) -> List[str]:
         return [x for x in super().__dir__() if x[0] != '_'] + self._names
 
     def __getitem__(self, item:str) -> Optional['AttributeBuilderObject']:
         return self.__getattr__(item)
 
     def add_object(self, name:str) -> Optional['AttributeBuilderObject']:
-        self._shop_api.AddObject(self._type, name)
+        add_object_result = self._shop_api.AddObject(self._type, name)
+
+        if (add_object_result < 0):
+            raise ValueError(f'Unable to add object "{self._type}/{name}". Check license and/or spelling.')
+
         if name in self._shop_api.GetObjectNamesInSystem():
             self._add_object_name(name)
         return self._parent.__getattr__(self._type).__getattr__(name)
 
     def _add_object_name(self, name:str) -> None:
         self._names.append(name)
```

### Comparing `sintef-pyshop-1.4.5/pyshop/shopcore/script_generator.py` & `sintef_pyshop-1.4.6/pyshop/shopcore/script_generator.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/shopcore/shop_api.py` & `sintef_pyshop-1.4.6/pyshop/shopcore/shop_api.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/pyshop/shopcore/shop_rest.py` & `sintef_pyshop-1.4.6/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/setup.py` & `sintef_pyshop-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/sintef_pyshop.egg-info/PKG-INFO` & `sintef_pyshop-1.4.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
@@ -79,23 +79,23 @@
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
 
-- cplex2010.dll
-- shop_cplex_interface.dll
-- shop_pybind.pyd
+- `cplex2010.dll`
+- `shop_cplex_interface.dll`
+- `shop_pybind.pyd`
 
 Linux:
 
-- libcplex2010.so
-- shop_cplex_interface.so
-- shop_pybind.so
+- `libcplex2010.so`
+- `shop_cplex_interface.so`
+- `shop_pybind.so`
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
 
 The SHOP license file, `SHOP_license.dat`, must always be located in the directory specified by the environment variable `ICC_COMMAND_PATH`. The `ICC_COMMAND_PATH` can be added as a persistent environment variable in the regular ways, or it can be set by pyshop on a session basis. If the keyword argument `license_path` is specified when creating an instance of the ShopSession class (see step 4), the environment variable is overridden in the local environment of the executing process. If SHOP complains about not finding the license file, it is likely an issue with the `ICC_COMMAND_PATH` not being correctly specified.
 
@@ -105,14 +105,35 @@
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
 
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
 
-    #Set time resolution
-    #Build topolgy
-    #Add temporal input
-    #Run model
-    #Retreive results
-
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
+
+## Visual Studio Code Dev Containers
+
+[Visual Studio Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers) lets you run a fully functional development environment using Docker and Visual Studio Code. This might simplyfy setting up pyshop for new users. Follow the guide below to setup the devcontainer for pyshop.
+
+### Installation
+
+Install the following dependencies:
+
+1. Install the code editor called [Visual Studio Code](https://code.visualstudio.com/Download). Visual Studio Code is free
+2. Install a Docker GUI: [Docker desktop](https://www.docker.com/products/docker-desktop/) (might require a paid license depending on your organization), or a free alternative called [Podman](https://podman.io/)
+
+### Setup
+
+1. Create a folder called `.devcontainer` in your root directory with a file called `devcontainer.json`. Your folder structure should look like the example below:
+
+   ![Devcontainer folder setup](docs/images/devcontainer-folder.png)
+
+2. Copy and paste the contents of [devcontainer.json](.devcontainer/devcontainer.json) into your `devcontainer.json` file.
+3. Create a folder called `bin` in your root directory and add the following files: `libcplex2010.so`, `shop_cplex_interface.so`, your shop license e.g `SHOP_license.dat`, shop pybind e.g `shop_pybind.cpython-312-x86_64-linux-gnu.so`. Your bin folder should now look like:
+
+   ![Binary folder with the required files](docs/images/bin-folder.png)
+
+4. Open your project using the devcontainer config files by running the command:
+   ![Searching for devcontainer command](docs/images/dev-containers-reopen.png)
+
+More in depth guides on how to customize devcontainers can be found in the [devcontainer documentation](https://code.visualstudio.com/docs/devcontainers/create-dev-container)
```

### Comparing `sintef-pyshop-1.4.5/sintef_pyshop.egg-info/SOURCES.txt` & `sintef_pyshop-1.4.6/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/tests/test_helpers_command.py` & `sintef_pyshop-1.4.6/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/tests/test_helpers_time.py` & `sintef_pyshop-1.4.6/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.5/tests/test_shop_api.py` & `sintef_pyshop-1.4.6/tests/test_shop_api.py`

 * *Files identical despite different names*

