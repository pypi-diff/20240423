# Comparing `tmp/stitchee-1.0.0.tar.gz` & `tmp/stitchee-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchee-1.0.0.tar", max compression
+gzip compressed data, was "stitchee-1.1.0.tar", max compression
```

## Comparing `stitchee-1.0.0.tar` & `stitchee-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-16 17:59:19.321244 stitchee-1.0.0/LICENSE
--rw-r--r--   0        0        0     4286 2024-04-16 17:59:19.321244 stitchee-1.0.0/README.md
--rw-r--r--   0        0        0       92 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/__init__.py
--rw-r--r--   0        0        0     8580 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/attribute_handling.py
--rw-r--r--   0        0        0    14343 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/dataset_and_group_handling.py
--rw-r--r--   0        0        0     5388 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/dimension_cleanup.py
--rw-r--r--   0        0        0      282 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/file_ops.py
--rw-r--r--   0        0        0        0 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/harmony/__init__.py
--rw-r--r--   0        0        0      882 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/harmony/cli.py
--rw-r--r--   0        0        0     3578 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/harmony/download_worker.py
--rw-r--r--   0        0        0     7569 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/harmony/service_adapter.py
--rw-r--r--   0        0        0     3817 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/harmony/util.py
--rw-r--r--   0        0        0     9134 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/run_stitchee.py
--rw-r--r--   0        0        0     7741 2024-04-16 17:59:19.321244 stitchee-1.0.0/concatenator/stitchee.py
--rw-r--r--   0        0        0     1348 2024-04-16 17:59:32.649233 stitchee-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 stitchee-1.0.0/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 stitchee-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 18:53:07.650636 stitchee-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4286 2024-04-23 18:53:07.650636 stitchee-1.1.0/README.md
+-rw-r--r--   0        0        0       92 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/__init__.py
+-rw-r--r--   0        0        0     8580 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/attribute_handling.py
+-rw-r--r--   0        0        0    14343 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/dataset_and_group_handling.py
+-rw-r--r--   0        0        0     5388 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/dimension_cleanup.py
+-rw-r--r--   0        0        0      282 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/file_ops.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/cli.py
+-rw-r--r--   0        0        0     3578 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/download_worker.py
+-rw-r--r--   0        0        0     7569 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/service_adapter.py
+-rw-r--r--   0        0        0     3817 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/harmony/util.py
+-rw-r--r--   0        0        0     9134 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/run_stitchee.py
+-rw-r--r--   0        0        0     7741 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/stitchee.py
+-rw-r--r--   0        0        0     1419 2024-04-23 18:53:25.774613 stitchee-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 stitchee-1.1.0/setup.py
+-rw-r--r--   0        0        0     5123 1970-01-01 00:00:00.000000 stitchee-1.1.0/PKG-INFO
```

### Comparing `stitchee-1.0.0/LICENSE` & `stitchee-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/README.md` & `stitchee-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/attribute_handling.py` & `stitchee-1.1.0/concatenator/attribute_handling.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/dataset_and_group_handling.py` & `stitchee-1.1.0/concatenator/dataset_and_group_handling.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/dimension_cleanup.py` & `stitchee-1.1.0/concatenator/dimension_cleanup.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/harmony/cli.py` & `stitchee-1.1.0/concatenator/harmony/cli.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/harmony/download_worker.py` & `stitchee-1.1.0/concatenator/harmony/download_worker.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/harmony/service_adapter.py` & `stitchee-1.1.0/concatenator/harmony/service_adapter.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/harmony/util.py` & `stitchee-1.1.0/concatenator/harmony/util.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/run_stitchee.py` & `stitchee-1.1.0/concatenator/run_stitchee.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/concatenator/stitchee.py` & `stitchee-1.1.0/concatenator/stitchee.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.0.0/pyproject.toml` & `stitchee-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [tool.poetry]
 name = "stitchee"
-version = "1.0.0"
+version = "1.1.0"
 description = "NetCDF4 Along-existing-dimension Concatenation Service"
 authors = ["Daniel Kaufman <daniel.kaufman@nasa.gov>"]
 readme = "README.md"
+repository = "https://github.com/nasa/stitchee"
+license = "Apache-2.0"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
     { include = "concatenator" },
 ]
 
+[tool.poetry.scripts]
+stitchee_harmony = 'concatenator.harmony.cli:main'
+stitchee = 'concatenator.run_stitchee:main'
+
 [tool.poetry.dependencies]
 python = "^3.10"
 netcdf4 = "^1.6.5"
 xarray = "^2024.3.0"
 dask = "^2024.4.1"
 harmony-service-lib = "^1.0.25"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 mypy = "^1.9.0"
-black = "^24.2.0"
+black = "^24.4.0"
 ruff = "^0.3.7"
 coverage = "^7.4.4"
 pytest-cov = "^5.0.0"
 
-[tool.poetry.scripts]
-stitchee_harmony = 'concatenator.harmony.cli:main'
-stitchee = 'concatenator.run_stitchee:main'
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.mypy.overrides]]
 module = "netCDF4.*"
 ignore_missing_imports = true
```

### Comparing `stitchee-1.0.0/setup.py` & `stitchee-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 entry_points = \
 {'console_scripts': ['stitchee = concatenator.run_stitchee:main',
                      'stitchee_harmony = concatenator.harmony.cli:main']}
 
 setup_kwargs = {
     'name': 'stitchee',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'NetCDF4 Along-existing-dimension Concatenation Service',
     'long_description': '<p align="center">\n    <img alt="stitchee, a python package for concatenating netCDF data along an existing dimension"\n    src="https://github.com/danielfromearth/stitchee/assets/114174502/58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"\n    />\n</p>\n\n<p align="center">\n    <a href="https://www.repostatus.org/#active" target="_blank">\n        <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n    </a>\n    <a href="https://github.com/python/black" target="_blank">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n    </a>\n    <a href="http://mypy-lang.org/" target="_blank">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n    </a>\n    <a href="https://codecov.io/gh/nasa/stitchee">\n     <img src="https://codecov.io/gh/nasa/stitchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">\n    </a>\n</p>\n\n[//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)\n\n# Overview\n_____\n\n_STITCHEE_ (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along an existing dimension*,\nand it is deigned as both a standalone utility and for use as a service in [Harmony](https://harmony.earthdata.nasa.gov/).\n\n## Getting started, with poetry\n\n1. Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n2. Install `stitchee`, with its dependencies, by running the following from the repository directory:\n\n```shell\npoetry install\n```\n\n## How to test `stitchee` locally\n\n```shell\npoetry run pytest tests/\n```\n\n## Usage\n\n```shell\n$ poetry run stitchee --help\nusage: stitchee [-h] -o OUTPUT_PATH [--no_input_file_copies] [--keep_tmp_files] [--concat_method {xarray-concat,xarray-combine}] [--concat_dim CONCAT_DIM]\n                [--xarray_arg_compat XARRAY_ARG_COMPAT] [--xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS] [--xarray_arg_join XARRAY_ARG_JOIN] [-O]\n                [-v]\n                path/directory or path list [path/directory or path list ...]\n\nRun the along-existing-dimension concatenator.\n\noptions:\n  -h, --help            show this help message and exit\n  --no_input_file_copies\n                        By default, input files are copied into a temporary directory to avoid modification of input files. This is useful for testing,\n                        but uses more disk space. By specifying this argument, no copying is performed.\n  --keep_tmp_files      Prevents removal, after successful execution, of (1) the flattened concatenated file and (2) the input directory copy if created\n                        by \'--make_dir_copy\'.\n  --concat_method {xarray-concat,xarray-combine}\n                        Whether to use the xarray concat method or the combine-by-coords method.\n  --concat_dim CONCAT_DIM\n                        Dimension to concatenate along, if possible. This is required if using the \'xarray-concat\' method\n  --xarray_arg_compat XARRAY_ARG_COMPAT\n                        \'compat\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS\n                        \'combine_attrs\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_join XARRAY_ARG_JOIN\n                        \'join\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  -O, --overwrite       Overwrite output file if it already exists.\n  -v, --verbose         Enable verbose output to stdout; useful for debugging\n\nRequired:\n  path/directory or path list\n                        Files to be concatenated, specified via a (1) single directory containing the files to be concatenated, (2) single text file\n                        containing linebreak-separated paths of the files to be concatenated, or (3) multiple filepaths of the files to be concatenated.\n  -o OUTPUT_PATH, --output_path OUTPUT_PATH\n                        The output filename for the merged output.\n```\n\nFor example:\n\n```shell\npoetry run stitchee /path/to/netcdf/directory/ -o /path/to/output.nc\n```\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20433-1\n',
     'author': 'Daniel Kaufman',
     'author_email': 'daniel.kaufman@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/nasa/stitchee',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['concatenator', 'concatenator.harmony'] package_data = \ {'': ['*']}
 install_requires = \ ['dask>=2024.4.1,<2025.0.0', 'harmony-service-
 lib>=1.0.25,<2.0.0', 'netcdf4>=1.6.5,<2.0.0', 'xarray>=2024.3.0,<2025.0.0']
 entry_points = \ {'console_scripts': ['stitchee = concatenator.run_stitchee:
 main', 'stitchee_harmony = concatenator.harmony.cli:main']} setup_kwargs =
-{ 'name': 'stitchee', 'version': '1.0.0', 'description': 'NetCDF4 Along-
+{ 'name': 'stitchee', 'version': '1.1.0', 'description': 'NetCDF4 Along-
 existing-dimension Concatenation Service', 'long_description': '
     \n n src="https://github.com/danielfromearth/stitchee/assets/114174502/
            58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"\n />\n
 \n\n
   \n _\_n_ _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e
    _s_t_a_t_e_ _a_n_d_ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_\_n_ \n _\_n_ _[_C_o_d_e_ _s_t_y_l_e_]_\_n_ \n _\_n_ _[_M_y_p_y
                      _c_h_e_c_k_e_d_]_\_n_ \n _\_n_ _[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_\_n_ \n
@@ -50,10 +50,11 @@
 linebreak-separated paths of the files to be concatenated, or (3) multiple
 filepaths of the files to be concatenated.\n -o OUTPUT_PATH, --output_path
 OUTPUT_PATH\n The output filename for the merged output.\n```\n\nFor example:
 \n\n```shell\npoetry run stitchee /path/to/netcdf/directory/ -o /path/to/
 output.nc\n```\n\n---\nThis package is NASA Software Release Authorization
 (SRA) # LAR-20433-1\n', 'author': 'Daniel Kaufman', 'author_email':
 'daniel.kaufman@nasa.gov', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+'url': 'https://github.com/nasa/stitchee', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.10,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `stitchee-1.0.0/PKG-INFO` & `stitchee-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: stitchee
-Version: 1.0.0
+Version: 1.1.0
 Summary: NetCDF4 Along-existing-dimension Concatenation Service
+Home-page: https://github.com/nasa/stitchee
+License: Apache-2.0
 Author: Daniel Kaufman
 Author-email: daniel.kaufman@nasa.gov
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dask (>=2024.4.1,<2025.0.0)
 Requires-Dist: harmony-service-lib (>=1.0.25,<2.0.0)
 Requires-Dist: netcdf4 (>=1.6.5,<2.0.0)
 Requires-Dist: xarray (>=2024.3.0,<2025.0.0)
+Project-URL: Repository, https://github.com/nasa/stitchee
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="stitchee, a python package for concatenating netCDF data along an existing dimension"
     src="https://github.com/danielfromearth/stitchee/assets/114174502/58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"
     />
 </p>
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: stitchee Version: 1.0.0 Summary: NetCDF4 Along-
-existing-dimension Concatenation Service Author: Daniel Kaufman Author-email:
-daniel.kaufman@nasa.gov Requires-Python: >=3.10,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: dask
-(>=2024.4.1,<2025.0.0) Requires-Dist: harmony-service-lib (>=1.0.25,<2.0.0)
-Requires-Dist: netcdf4 (>=1.6.5,<2.0.0) Requires-Dist: xarray
-(>=2024.3.0,<2025.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: stitchee Version: 1.1.0 Summary: NetCDF4 Along-
+existing-dimension Concatenation Service Home-page: https://github.com/nasa/
+stitchee License: Apache-2.0 Author: Daniel Kaufman Author-email:
+daniel.kaufman@nasa.gov Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Dist: dask (>=2024.4.1,<2025.0.0)
+Requires-Dist: harmony-service-lib (>=1.0.25,<2.0.0) Requires-Dist: netcdf4
+(>=1.6.5,<2.0.0) Requires-Dist: xarray (>=2024.3.0,<2025.0.0) Project-URL:
+Repository, https://github.com/nasa/stitchee Description-Content-Type: text/
+markdown
   [stitchee, a python package for concatenating netCDF data along an existing
                                   dimension]
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
      _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 [//]: # (Using deprecated `align="center"` for the logo image and badges above,
 because of https://stackoverflow.com/a/62383408) # Overview _____ _STITCHEE_
 (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along
```

