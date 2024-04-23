# Comparing `tmp/apipe-0.1.4.tar.gz` & `tmp/apipe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apipe-0.1.4.tar", max compression
+gzip compressed data, was "apipe-0.1.5.tar", max compression
```

## Comparing `apipe-0.1.4.tar` & `apipe-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11357 2022-03-01 07:06:43.812766 apipe-0.1.4/LICENSE
--rw-r--r--   0        0        0     2369 2022-03-01 07:06:43.812766 apipe-0.1.4/README.md
--rw-r--r--   0        0        0      273 2022-03-01 07:06:43.812766 apipe-0.1.4/apipe/__init__.py
--rw-r--r--   0        0        0    15864 2022-03-01 07:06:43.812766 apipe-0.1.4/apipe/_cached.py
--rw-r--r--   0        0        0     5203 2022-03-01 07:06:43.812766 apipe-0.1.4/apipe/_dask.py
--rw-r--r--   0        0        0     1496 2022-03-01 07:06:57.164938 apipe-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3294 2022-03-01 07:06:58.053974 apipe-0.1.4/setup.py
--rw-r--r--   0        0        0     3338 2022-03-01 07:06:58.054377 apipe-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 16:25:03.522440 apipe-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2369 2024-04-23 16:25:03.522440 apipe-0.1.5/README.md
+-rw-r--r--   0        0        0      273 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/__init__.py
+-rw-r--r--   0        0        0    15864 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/_cached.py
+-rw-r--r--   0        0        0     5203 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/_dask.py
+-rw-r--r--   0        0        0     2412 2024-04-23 16:25:20.722422 apipe-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 apipe-0.1.5/PKG-INFO
```

### Comparing `apipe-0.1.4/LICENSE` & `apipe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apipe-0.1.4/README.md` & `apipe-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apipe-0.1.4/apipe/_cached.py` & `apipe-0.1.5/apipe/_cached.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.4/apipe/_dask.py` & `apipe-0.1.5/apipe/_dask.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.4/setup.py` & `apipe-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: apipe
+Version: 0.1.5
+Summary: Data pipelines with lazy computation and caching
+Home-page: https://github.com/mysterious-ben/apipe
+License: Apache License, Version 2.0
+Keywords: python,pipeline,dask,pandas
+Author: Mysterious Ben
+Author-email: datascience@tuta.io
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cloudpickle (>=2.0.0,<3.0.0)
+Requires-Dist: dask[delayed] (>=2024.4.2,<2025.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pyarrow (>=16.0.0,<17.0.0)
+Requires-Dist: xxhash (>=3.4.1,<4.0.0)
+Project-URL: Repository, https://github.com/mysterious-ben/apipe
+Description-Content-Type: text/markdown
+
+# A-Pipe
+
+**A-Pipe** allows to create data pipelines with lazy computation and caching.
+
+**Features:**
+- Lazy computation and cache loading
+- Pickle and parquet serialization
+- Support for hashing of `numpy` arrays and `pandas` DataFrames
+- Support for `dask.Delayed` objects
+
+## Installation
+
+```shell
+pip install apipe
+```
+
+## Examples
+
+### Simple function caching
+
+```python
+import time
+import apipe
+import numpy as np
+from loguru import logger
+
+@apipe.eager_cached()
+def load_data(table: str):
+    time.sleep(1)
+    arr = np.ones(5)
+    logger.debug(f"transferred array data from table={table}")
+    return arr
+
+logger.info("start loading data")
+
+# --- First pass: transfer data and save on disk
+data = load_data("weather-ldn")
+logger.info(f"finished loading data: {load_data()}")
+
+# --- Second pass: load data from disk
+data = load_data("weather-ldn")
+logger.info(f"finished loading data: {load_data()}")
+```
+
+
+### Data pipeline with lazy execution and caching
+
+```python
+import apipe
+import pandas as pd
+import numpy as np
+from loguru import logger
+
+# --- Define data transformations via step functions (similar to dask.delayed)
+
+@apipe.delayed_cached()  # lazy computation + caching on disk
+def load_1():
+    df = pd.DataFrame({"a": [1., 2.], "b": [0.1, np.nan]})
+    logger.debug("Loaded {} records".format(len(df)))
+    return df
+
+@apipe.delayed_cached()  # lazy computation + caching on disk
+def load_2(timestamp):
+    df = pd.DataFrame({"a": [0.9, 3.], "b": [0.001, 1.]})
+    logger.debug("Loaded {} records".format(len(df)))
+    return df
+
+@apipe.delayed_cached()  # lazy computation + caching on disk
+def compute(x, y, eps):
+    assert x.shape == y.shape
+    diff = ((x - y).abs() / (y.abs()+eps)).mean().mean()
+    logger.debug("Difference is computed")
+    return diff
+
+# --- Define pipeline dependencies
+ts = pd.Timestamp(2019, 1, 1)
+eps = 0.01
+s1 = load_1()
+s2 = load_2(ts)
+diff = compute(s1, s2, eps)
+
+# --- Trigger pipeline execution (first pass: compute everything and save on disk)
+logger.info("diff: {:.3f}".format(apipe.delayed_compute((diff, ))[0]))
+
+# --- Trigger pipeline execution (second pass: load from disk the end result only)
+logger.info("diff: {:.3f}".format(apipe.delayed_compute((diff, ))[0]))
+```
 
-packages = \
-['apipe']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cloudpickle>=2.0.0,<3.0.0',
- 'dask[delayed]>=2021.01.1,<2022.0.0',
- 'loguru>=0.5.0,<0.6.0',
- 'numpy>=1.16.5,<2.0.0',
- 'pandas>=1.2.0,<2.0.0',
- 'pyarrow>=5.0.0,<6.0.0',
- 'xxhash>=2.0.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'apipe',
-    'version': '0.1.4',
-    'description': 'Data pipelines with lazy computation and caching',
-    'long_description': '# A-Pipe\n\n**A-Pipe** allows to create data pipelines with lazy computation and caching.\n\n**Features:**\n- Lazy computation and cache loading\n- Pickle and parquet serialization\n- Support for hashing of `numpy` arrays and `pandas` DataFrames\n- Support for `dask.Delayed` objects\n\n## Installation\n\n```shell\npip install apipe\n```\n\n## Examples\n\n### Simple function caching\n\n```python\nimport time\nimport apipe\nimport numpy as np\nfrom loguru import logger\n\n@apipe.eager_cached()\ndef load_data(table: str):\n    time.sleep(1)\n    arr = np.ones(5)\n    logger.debug(f"transferred array data from table={table}")\n    return arr\n\nlogger.info("start loading data")\n\n# --- First pass: transfer data and save on disk\ndata = load_data("weather-ldn")\nlogger.info(f"finished loading data: {load_data()}")\n\n# --- Second pass: load data from disk\ndata = load_data("weather-ldn")\nlogger.info(f"finished loading data: {load_data()}")\n```\n\n\n### Data pipeline with lazy execution and caching\n\n```python\nimport apipe\nimport pandas as pd\nimport numpy as np\nfrom loguru import logger\n\n# --- Define data transformations via step functions (similar to dask.delayed)\n\n@apipe.delayed_cached()  # lazy computation + caching on disk\ndef load_1():\n    df = pd.DataFrame({"a": [1., 2.], "b": [0.1, np.nan]})\n    logger.debug("Loaded {} records".format(len(df)))\n    return df\n\n@apipe.delayed_cached()  # lazy computation + caching on disk\ndef load_2(timestamp):\n    df = pd.DataFrame({"a": [0.9, 3.], "b": [0.001, 1.]})\n    logger.debug("Loaded {} records".format(len(df)))\n    return df\n\n@apipe.delayed_cached()  # lazy computation + caching on disk\ndef compute(x, y, eps):\n    assert x.shape == y.shape\n    diff = ((x - y).abs() / (y.abs()+eps)).mean().mean()\n    logger.debug("Difference is computed")\n    return diff\n\n# --- Define pipeline dependencies\nts = pd.Timestamp(2019, 1, 1)\neps = 0.01\ns1 = load_1()\ns2 = load_2(ts)\ndiff = compute(s1, s2, eps)\n\n# --- Trigger pipeline execution (first pass: compute everything and save on disk)\nlogger.info("diff: {:.3f}".format(apipe.delayed_compute((diff, ))[0]))\n\n# --- Trigger pipeline execution (second pass: load from disk the end result only)\nlogger.info("diff: {:.3f}".format(apipe.delayed_compute((diff, ))[0]))\n```\n\nSee more examples in a [notebook](https://github.com/mysterious-ben/ds-examples/blob/master/dataflows/dask_delayed_with_caching.ipynb).',
-    'author': 'Mysterious Ben',
-    'author_email': 'datascience@tuta.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mysterious-ben/apipe',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
-}
-
-
-setup(**setup_kwargs)
+See more examples in a [notebook](https://github.com/mysterious-ben/ds-examples/blob/master/dataflows/dask_delayed_with_caching.ipynb).
```

