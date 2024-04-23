# Comparing `tmp/kestrel_jupyter-1.8.2.tar.gz` & `tmp/kestrel_jupyter-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel_jupyter-1.8.2.tar", last modified: Fri Feb 23 18:50:15 2024, max compression
+gzip compressed data, was "kestrel_jupyter-1.8.3.tar", last modified: Mon Apr 22 18:07:23 2024, max compression
```

## Comparing `kestrel_jupyter-1.8.2.tar` & `kestrel_jupyter-1.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.382564 kestrel_jupyter-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.382564 kestrel_jupyter-1.8.2/src/kestrel_ipython/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_ipython/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-23 18:50:15.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:15.386564 kestrel_jupyter-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/tests/test_kernel_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-23 18:49:59.000000 kestrel_jupyter-1.8.2/tests/test_notebook_syntax_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.033968 kestrel_jupyter-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-04-22 18:07:23.033968 kestrel_jupyter-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:07:23.033968 kestrel_jupyter-1.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.029968 kestrel_jupyter-1.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.029968 kestrel_jupyter-1.8.3/src/kestrel_ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_ipython/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.033968 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 18:07:23.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.029968 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.029968 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:23.033968 kestrel_jupyter-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/tests/test_kernel_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-22 18:07:08.000000 kestrel_jupyter-1.8.3/tests/test_notebook_syntax_gen.py
```

### Comparing `kestrel_jupyter-1.8.2/PKG-INFO` & `kestrel_jupyter-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,44 @@
 Metadata-Version: 2.1
 Name: kestrel_jupyter
-Version: 1.8.2
+Version: 1.8.3
 Summary: Kestrel Jupyter Kernel
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,Jupyter,kernel
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: kestrel_core==1.8.1
+Requires-Dist: kestrel_core==1.8.2
 Requires-Dist: kestrel_datasource_stixbundle==1.8.0
-Requires-Dist: kestrel_datasource_stixshifter==1.8.1
+Requires-Dist: kestrel_datasource_stixshifter==1.8.2
 Requires-Dist: kestrel_analytics_python==1.8.0
-Requires-Dist: kestrel_analytics_docker==1.8.0
+Requires-Dist: kestrel_analytics_docker==1.8.1
 Requires-Dist: jupyterlab-server
 Requires-Dist: jupyterlab
 Requires-Dist: jupyter_client
 Requires-Dist: nbclassic
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.png
    :width: 460
    :alt: Kestrel Threat Hunting Language
 
-.. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
-        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/v/kestrel-jupyter
-        :target: https://pypi.python.org/pypi/kestrel-jupyter
-        :alt: Latest Version
-
-.. image:: https://img.shields.io/pypi/dm/kestrel-core
-        :target: https://pypistats.org/packages/kestrel-core
-        :alt: PyPI Downloads
-
-.. image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
-        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
-        :alt: Code Coverage
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        :target: https://github.com/psf/black
-        :alt: Code Style: Black
-
 |
 
-**[News]** Kestrel session at `Black Hat USA 2023`_
+|readthedocs| |pypi| |downloads| |codecoverage| |black|
 
---------
+|
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
 shareable hunt-flow. Starting with:
 
 #. `Black Hat USA 2022 session recording`_
 #. `Black Hat USA 2022 Kestrel hunting lab`_
@@ -239,7 +219,28 @@
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
+
+
+.. |readthedocs| image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
+        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/kestrel-jupyter
+        :target: https://pypi.python.org/pypi/kestrel-jupyter
+        :alt: Latest Version
+
+.. |downloads| image:: https://img.shields.io/pypi/dm/kestrel-core
+        :target: https://pypistats.org/packages/kestrel-core
+        :alt: PyPI Downloads
+
+.. |codecoverage| image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
+        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
+        :alt: Code Coverage
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/psf/black
+        :alt: Code Style: Black
```

### Comparing `kestrel_jupyter-1.8.2/README.rst` & `kestrel_jupyter-1.8.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,16 @@
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.png
    :width: 460
    :alt: Kestrel Threat Hunting Language
 
-.. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
-        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/v/kestrel-jupyter
-        :target: https://pypi.python.org/pypi/kestrel-jupyter
-        :alt: Latest Version
-
-.. image:: https://img.shields.io/pypi/dm/kestrel-core
-        :target: https://pypistats.org/packages/kestrel-core
-        :alt: PyPI Downloads
-
-.. image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
-        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
-        :alt: Code Coverage
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        :target: https://github.com/psf/black
-        :alt: Code Style: Black
-
 |
 
-**[News]** Kestrel session at `Black Hat USA 2023`_
+|readthedocs| |pypi| |downloads| |codecoverage| |black|
 
---------
+|
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
 shareable hunt-flow. Starting with:
 
 #. `Black Hat USA 2022 session recording`_
 #. `Black Hat USA 2022 Kestrel hunting lab`_
@@ -211,7 +191,28 @@
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
+
+
+.. |readthedocs| image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
+        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/kestrel-jupyter
+        :target: https://pypi.python.org/pypi/kestrel-jupyter
+        :alt: Latest Version
+
+.. |downloads| image:: https://img.shields.io/pypi/dm/kestrel-core
+        :target: https://pypistats.org/packages/kestrel-core
+        :alt: PyPI Downloads
+
+.. |codecoverage| image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
+        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
+        :alt: Code Coverage
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/psf/black
+        :alt: Code Style: Black
```

### Comparing `kestrel_jupyter-1.8.2/pyproject.toml` & `kestrel_jupyter-1.8.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.2.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kestrel_jupyter"
-version = "1.8.2"
+version = "1.8.3"
 description = "Kestrel Jupyter Kernel"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "Apache 2.0 License"}
 maintainers = [
     {name = "Xiaokui Shu", email = "xiaokui.shu@ibm.com"},
     {name = "Paul Coccoli", email = "pcoccoli@us.ibm.com"},
@@ -22,19 +22,19 @@
     "Topic :: Security",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
-    "kestrel_core==1.8.1",
+    "kestrel_core==1.8.2",
     "kestrel_datasource_stixbundle==1.8.0",
-    "kestrel_datasource_stixshifter==1.8.1",
+    "kestrel_datasource_stixshifter==1.8.2",
     "kestrel_analytics_python==1.8.0",
-    "kestrel_analytics_docker==1.8.0",
+    "kestrel_analytics_docker==1.8.1",
     "jupyterlab-server",
     "jupyterlab",
     "jupyter_client",
     "nbclassic",
 ]
 
 [project.optional-dependencies]
```

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_ipython/magic.py` & `kestrel_jupyter-1.8.3/src/kestrel_ipython/magic.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/PKG-INFO` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,44 @@
 Metadata-Version: 2.1
 Name: kestrel_jupyter
-Version: 1.8.2
+Version: 1.8.3
 Summary: Kestrel Jupyter Kernel
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,Jupyter,kernel
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: kestrel_core==1.8.1
+Requires-Dist: kestrel_core==1.8.2
 Requires-Dist: kestrel_datasource_stixbundle==1.8.0
-Requires-Dist: kestrel_datasource_stixshifter==1.8.1
+Requires-Dist: kestrel_datasource_stixshifter==1.8.2
 Requires-Dist: kestrel_analytics_python==1.8.0
-Requires-Dist: kestrel_analytics_docker==1.8.0
+Requires-Dist: kestrel_analytics_docker==1.8.1
 Requires-Dist: jupyterlab-server
 Requires-Dist: jupyterlab
 Requires-Dist: jupyter_client
 Requires-Dist: nbclassic
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.png
    :width: 460
    :alt: Kestrel Threat Hunting Language
 
-.. image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
-        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/v/kestrel-jupyter
-        :target: https://pypi.python.org/pypi/kestrel-jupyter
-        :alt: Latest Version
-
-.. image:: https://img.shields.io/pypi/dm/kestrel-core
-        :target: https://pypistats.org/packages/kestrel-core
-        :alt: PyPI Downloads
-
-.. image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
-        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
-        :alt: Code Coverage
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        :target: https://github.com/psf/black
-        :alt: Code Style: Black
-
 |
 
-**[News]** Kestrel session at `Black Hat USA 2023`_
+|readthedocs| |pypi| |downloads| |codecoverage| |black|
 
---------
+|
 
 Kestrel is a threat hunting language aiming to make cyber threat hunting *fast*
 by providing a layer of abstraction to build reusable, composable, and
 shareable hunt-flow. Starting with:
 
 #. `Black Hat USA 2022 session recording`_
 #. `Black Hat USA 2022 Kestrel hunting lab`_
@@ -239,7 +219,28 @@
 
 .. _slack invitation: https://join.slack.com/t/open-cybersecurity/shared_invite/zt-19pliofsm-L7eSSB8yzABM2Pls1nS12w
 .. _Open Cybersecurity Alliance workspace: https://open-cybersecurity.slack.com/
 .. _GitHub Issue: https://github.com/opencybersecurityalliance/kestrel-lang/issues
 .. _contributing guideline: CONTRIBUTING.rst
 .. _governance documentation: GOVERNANCE.rst
 .. _Apache License 2.0: LICENSE.md
+
+
+.. |readthedocs| image:: https://readthedocs.org/projects/kestrel/badge/?version=latest
+        :target: https://kestrel.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/kestrel-jupyter
+        :target: https://pypi.python.org/pypi/kestrel-jupyter
+        :alt: Latest Version
+
+.. |downloads| image:: https://img.shields.io/pypi/dm/kestrel-core
+        :target: https://pypistats.org/packages/kestrel-core
+        :alt: PyPI Downloads
+
+.. |codecoverage| image:: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang/branch/develop/graph/badge.svg?token=HM4ax10IW3
+        :target: https://codecov.io/gh/opencybersecurityalliance/kestrel-lang
+        :alt: Code Coverage
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/psf/black
+        :alt: Code Style: Black
```

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter.egg-info/SOURCES.txt` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/codemirror/setup.py` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/codemirror/setup.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/kernel.py` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.2/src/kestrel_jupyter_kernel/setup.py` & `kestrel_jupyter-1.8.3/src/kestrel_jupyter_kernel/setup.py`

 * *Files identical despite different names*

