# Comparing `tmp/tessproposaltool-0.1.0.tar.gz` & `tmp/tessproposaltool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessproposaltool-0.1.0.tar", max compression
+gzip compressed data, was "tessproposaltool-0.1.1.tar", max compression
```

## Comparing `tessproposaltool-0.1.0.tar` & `tessproposaltool-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2024-04-12 21:49:48.259847 tessproposaltool-0.1.0/LICENSE
--rw-r--r--   0        0        0     1359 2024-04-12 21:56:23.748526 tessproposaltool-0.1.0/README.md
--rw-r--r--   0        0        0      673 2024-04-12 21:52:51.278659 tessproposaltool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3110 2024-04-12 21:55:02.992465 tessproposaltool-0.1.0/src/tessproposaltool/__init__.py
--rw-r--r--   0        0        0     7346 2024-04-12 21:45:59.813045 tessproposaltool-0.1.0/src/tessproposaltool/tpt.py
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 tessproposaltool-0.1.0/setup.py
--rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 tessproposaltool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-12 21:49:48.259847 tessproposaltool-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1359 2024-04-12 21:56:23.748526 tessproposaltool-0.1.1/README.md
+-rw-r--r--   0        0        0      701 2024-04-23 17:14:02.322311 tessproposaltool-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3110 2024-04-12 21:55:02.992465 tessproposaltool-0.1.1/src/tessproposaltool/__init__.py
+-rw-r--r--   0        0        0     7346 2024-04-12 21:45:59.813045 tessproposaltool-0.1.1/src/tessproposaltool/tpt.py
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 tessproposaltool-0.1.1/setup.py
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 tessproposaltool-0.1.1/PKG-INFO
```

### Comparing `tessproposaltool-0.1.0/LICENSE` & `tessproposaltool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tessproposaltool-0.1.0/README.md` & `tessproposaltool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tessproposaltool-0.1.0/pyproject.toml` & `tessproposaltool-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "tessproposaltool"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Christina Hedges <christina.l.hedges@nasa.gov>"]
 readme = "README.md"
 packages = [{include = "tessproposaltool", from = "src"}]
+include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.7.1"
 numpy = "^1.26.4"
 pandas = "^2.2.2"
 astropy = "^6.0.1"
 astroquery = "^0.4.7"
 asyncio = "^3.4.3"
 tqdm = "^4.66.2"
 lxml = "^5.2.1"
 toml = "^0.10.2"
 
-
 [tool.poetry.group.dev.dependencies]
 isort = "^5.13.2"
 black = "^24.4.0"
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 
 [build-system]
```

### Comparing `tessproposaltool-0.1.0/src/tessproposaltool/__init__.py` & `tessproposaltool-0.1.1/src/tessproposaltool/__init__.py`

 * *Files identical despite different names*

### Comparing `tessproposaltool-0.1.0/src/tessproposaltool/tpt.py` & `tessproposaltool-0.1.1/src/tessproposaltool/tpt.py`

 * *Files identical despite different names*

### Comparing `tessproposaltool-0.1.0/setup.py` & `tessproposaltool-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'tqdm>=4.66.2,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['tpt = tessproposaltool.tpt:tpt']}
 
 setup_kwargs = {
     'name': 'tessproposaltool',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '<a href="https://github.com/tessgi/tessproposaltool/actions/workflows/tests.yml"><img src="https://github.com/tessgi/tessproposaltool/workflows/pytest/badge.svg" alt="Test status"/></a> [!\n[![PyPI version](https://badge.fury.io/py/tessproposaltool.svg)](https://badge.fury.io/py/tessproposaltool)\n\n# TESS Proposal Tool\n\nUnder development tool to help create TESS proposals and target lists.\n\n## Use Case 1: Filling in missing TICs in a target list\n\nIf you have a list of RAs, Decs, and optionally TESS magnitudes and you would like to crossmatch them against TIC, you can do this with the `tessproposaltool`. You can do this from the command line using:\n\n```shell\ntpt radec_file.csv -o output.csv\n```\n\nWhich will result in a file `output.csv` that contains the corrected RA, Dec, TESS magnitude and TIC numbers.\n\nYour file should have a structure that contains RAs, Decs, and optionally TESS magnitudes, e.g.:\n\n```shell\nra,dec,tmag\n40.2986,56.7305,9.39\n110.093,-22.2673,13.51\n116.243,-30.0918,9.5\n152.633,-59.3549,10.05\n163.437,-58.4871,9.91\n165.091,-60.7688,12.974\n```\n\nTo do this inside Python you can use\n\n```python\nfrom tessproposaltool import fill_tics\n\n# read in your radecs, or convert them into a pandas dataframe\nRA, Dec, Tmag = ..., ..., ...\ndf = pd.DataFrame(np.asarray([RA, Dec, Tmag]).T, columns=[\'ra\', \'dec\', \'tmag\'])\nnew_df = fill_tics(df)\n```\n',
     'author': 'Christina Hedges',
     'author_email': 'christina.l.hedges@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['tessproposaltool'] package_data = \ {'': ['*']}
 install_requires = \ ['astropy>=6.0.1,<7.0.0', 'astroquery>=0.4.7,<0.5.0',
 'asyncio>=3.4.3,<4.0.0', 'lxml>=5.2.1,<6.0.0', 'numpy>=1.26.4,<2.0.0',
 'pandas>=2.2.2,<3.0.0', 'rich>=13.7.1,<14.0.0', 'toml>=0.10.2,<0.11.0',
 'tqdm>=4.66.2,<5.0.0'] entry_points = \ {'console_scripts': ['tpt =
 tessproposaltool.tpt:tpt']} setup_kwargs = { 'name': 'tessproposaltool',
-'version': '0.1.0', 'description': '', 'long_description': '_[_T_e_s_t_ _s_t_a_t_u_s_] [!\n
+'version': '0.1.1', 'description': '', 'long_description': '_[_T_e_s_t_ _s_t_a_t_u_s_] [!\n
 [![PyPI version](https://badge.fury.io/py/tessproposaltool.svg)](https://
 badge.fury.io/py/tessproposaltool)\n\n# TESS Proposal Tool\n\nUnder development
 tool to help create TESS proposals and target lists.\n\n## Use Case 1: Filling
 in missing TICs in a target list\n\nIf you have a list of RAs, Decs, and
 optionally TESS magnitudes and you would like to crossmatch them against TIC,
 you can do this with the `tessproposaltool`. You can do this from the command
 line using:\n\n```shell\ntpt radec_file.csv -o output.csv\n```\n\nWhich will
```

### Comparing `tessproposaltool-0.1.0/PKG-INFO` & `tessproposaltool-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessproposaltool
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Christina Hedges
 Author-email: christina.l.hedges@nasa.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tessproposaltool Version: 0.1.0 Summary: Author:
+Metadata-Version: 2.1 Name: tessproposaltool Version: 0.1.1 Summary: Author:
 Christina Hedges Author-email: christina.l.hedges@nasa.gov Requires-Python:
 >=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: astropy (>=6.0.1,<7.0.0) Requires-Dist: astroquery (>=0.4.7,<0.5.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: pandas (>=2.2.2,<3.0.0)
```

