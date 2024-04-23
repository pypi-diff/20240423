# Comparing `tmp/torchmate-0.1.0.tar.gz` & `tmp/torchmate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmate-0.1.0.tar", last modified: Mon Feb 26 11:36:48 2024, max compression
+gzip compressed data, was "torchmate-0.1.1.tar", last modified: Tue Apr 23 21:10:28 2024, max compression
```

## Comparing `torchmate-0.1.0.tar` & `torchmate-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.488447 torchmate-0.1.0/
--rw-r--r--   0 saihan    (1000) saihan    (1000)     1077 2024-02-19 13:08:20.000000 torchmate-0.1.0/LICENSE.txt
--rw-r--r--   0 saihan    (1000) saihan    (1000)     6538 2024-02-26 11:36:48.487447 torchmate-0.1.0/PKG-INFO
--rw-r--r--   0 saihan    (1000) saihan    (1000)     5610 2024-02-26 11:33:19.000000 torchmate-0.1.0/README.md
--rw-r--r--   0 saihan    (1000) saihan    (1000)      449 2024-02-24 22:49:25.000000 torchmate-0.1.0/pyproject.toml
--rw-r--r--   0 saihan    (1000) saihan    (1000)       38 2024-02-26 11:36:48.489447 torchmate-0.1.0/setup.cfg
--rw-r--r--   0 saihan    (1000) saihan    (1000)     4356 2024-02-26 11:35:13.000000 torchmate-0.1.0/setup.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.484447 torchmate-0.1.0/torchmate/
--rw-r--r--   0 saihan    (1000) saihan    (1000)      142 2024-02-23 13:55:22.000000 torchmate-0.1.0/torchmate/__init__.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)       63 2024-02-26 11:33:19.000000 torchmate-0.1.0/torchmate/__version__.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.486447 torchmate-0.1.0/torchmate/callbacks/
--rw-r--r--   0 saihan    (1000) saihan    (1000)     1896 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/__init__.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     3569 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/callback.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2395 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/csv_logger.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2734 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/early_stopper.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     1349 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/gradient_accumulator.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2354 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/gradient_clipper.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     4651 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/model_checkpoint.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)      869 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/wandb_logger.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     5083 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/callbacks/wandb_model_checkpoint.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.486447 torchmate-0.1.0/torchmate/modules/
--rw-r--r--   0 saihan    (1000) saihan    (1000)      712 2024-02-26 09:39:19.000000 torchmate-0.1.0/torchmate/modules/__init__.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2742 2024-02-26 09:39:19.000000 torchmate-0.1.0/torchmate/modules/refined_self_attention_sagan.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     6359 2024-02-26 09:39:19.000000 torchmate-0.1.0/torchmate/modules/squeeze_and_excitation.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.486447 torchmate-0.1.0/torchmate/trainer/
--rw-r--r--   0 saihan    (1000) saihan    (1000)      777 2024-02-26 09:50:33.000000 torchmate-0.1.0/torchmate/trainer/__init__.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)    21729 2024-02-22 06:58:10.000000 torchmate-0.1.0/torchmate/trainer/trainer.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.487447 torchmate-0.1.0/torchmate/utils/
--rw-r--r--   0 saihan    (1000) saihan    (1000)      470 2024-02-26 10:33:03.000000 torchmate-0.1.0/torchmate/utils/__init__.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2309 2024-02-26 10:33:03.000000 torchmate-0.1.0/torchmate/utils/check_model_info.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     2848 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/utils/color_text.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     6961 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/utils/history_plotter.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)     3811 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/utils/progress_bar.py
--rw-r--r--   0 saihan    (1000) saihan    (1000)      596 2024-02-21 19:08:41.000000 torchmate-0.1.0/torchmate/utils/running_average.py
-drwxr-xr-x   0 saihan    (1000) saihan    (1000)        0 2024-02-26 11:36:48.484447 torchmate-0.1.0/torchmate.egg-info/
--rw-r--r--   0 saihan    (1000) saihan    (1000)     6538 2024-02-26 11:36:48.000000 torchmate-0.1.0/torchmate.egg-info/PKG-INFO
--rw-r--r--   0 saihan    (1000) saihan    (1000)      976 2024-02-26 11:36:48.000000 torchmate-0.1.0/torchmate.egg-info/SOURCES.txt
--rw-r--r--   0 saihan    (1000) saihan    (1000)        1 2024-02-26 11:36:48.000000 torchmate-0.1.0/torchmate.egg-info/dependency_links.txt
--rw-r--r--   0 saihan    (1000) saihan    (1000)     1126 2024-02-26 11:36:48.000000 torchmate-0.1.0/torchmate.egg-info/requires.txt
--rw-r--r--   0 saihan    (1000) saihan    (1000)       10 2024-02-26 11:36:48.000000 torchmate-0.1.0/torchmate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.613484 torchmate-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 21:10:19.000000 torchmate-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-23 21:10:28.613484 torchmate-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-23 21:10:19.000000 torchmate-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-23 21:10:19.000000 torchmate-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:10:28.613484 torchmate-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-23 21:10:19.000000 torchmate-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/gradient_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/gradient_clipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/callbacks/wandb_model_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/modules/refined_self_attention_sagan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/modules/squeeze_and_excitation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21729 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/check_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/color_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/history_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 21:10:19.000000 torchmate-0.1.1/torchmate/utils/running_average.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:10:28.609485 torchmate-0.1.1/torchmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-23 21:10:28.000000 torchmate-0.1.1/torchmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 21:10:28.000000 torchmate-0.1.1/torchmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:10:28.000000 torchmate-0.1.1/torchmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-23 21:10:28.000000 torchmate-0.1.1/torchmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 21:10:28.000000 torchmate-0.1.1/torchmate.egg-info/top_level.txt
```

### Comparing `torchmate-0.1.0/LICENSE.txt` & `torchmate-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/PKG-INFO` & `torchmate-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: torchmate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torchmate: A High level PyTorch Training Library
+Home-page: UNKNOWN
 Author: Abdullah Saihan Taki
 Author-email: saihan0176@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/SaihanTaki/torchmate
 Project-URL: Documentation, https://torchmate.readthedocs.io/en/latest/
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,19 +28,23 @@
 
 
 <div align="center">
  
 ![logo](https://i.ibb.co/tzsKgkR/Torchmate-logo-v1.png)  
 **A High level PyTorch Training and Utility Library**
 
-[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue)](https://torchmate.readthedocs.io/en/latest/)
-[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat)](https://pypi.org/project/torchmate/)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat)](https://github.com/SaihanTaki/torchmate/blob/master/LICENSE.txt)
-[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat)](https://www.python.org/)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml) 
+[![Codecov](https://img.shields.io/codecov/c/github/SaihanTaki/Torchmate?logo=codecov&labelColor=3B434B)](https://app.codecov.io/gh/SaihanTaki/Torchmate)
+[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue&labelColor=3B434B)](https://torchmate.readthedocs.io/en/latest/)
+
+[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat&labelColor=3B434B)](https://pypi.org/project/torchmate/)
+[![Code Style](https://img.shields.io/badge/codestyle-black-black?style=flat&label=code%20style&labelColor=3B434B)](https://github.com/psf/black)
+[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat&labelColor=3B434B)](https://github.com/SaihanTaki/Torchmate/blob/main/LICENSE.txt)
+[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat&labelColor=3B434B)](https://www.python.org/)
  
 
 </div>
 
 ### [📚 Project Documentation](https://torchmate.readthedocs.io/en/latest/)
 
 Visit [Torchmate's Read The Docs Project Page](https://torchmate.readthedocs.io/en/latest/) or read following README to know more about Torchmate library
@@ -133,7 +139,8 @@
 
 ```
 
 
 
 ### 🛡️ License <a name="license"></a>
 Torchmate is distributed under [MIT License](https://github.com/SaihanTaki/torchmate/blob/master/LICENSE.txt)
+
```

### Comparing `torchmate-0.1.0/README.md` & `torchmate-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 <div align="center">
  
 ![logo](https://i.ibb.co/tzsKgkR/Torchmate-logo-v1.png)  
 **A High level PyTorch Training and Utility Library**
 
-[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue)](https://torchmate.readthedocs.io/en/latest/)
-[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat)](https://pypi.org/project/torchmate/)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat)](https://github.com/SaihanTaki/torchmate/blob/master/LICENSE.txt)
-[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat)](https://www.python.org/)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml) 
+[![Codecov](https://img.shields.io/codecov/c/github/SaihanTaki/Torchmate?logo=codecov&labelColor=3B434B)](https://app.codecov.io/gh/SaihanTaki/Torchmate)
+[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue&labelColor=3B434B)](https://torchmate.readthedocs.io/en/latest/)
+
+[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat&labelColor=3B434B)](https://pypi.org/project/torchmate/)
+[![Code Style](https://img.shields.io/badge/codestyle-black-black?style=flat&label=code%20style&labelColor=3B434B)](https://github.com/psf/black)
+[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat&labelColor=3B434B)](https://github.com/SaihanTaki/Torchmate/blob/main/LICENSE.txt)
+[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat&labelColor=3B434B)](https://www.python.org/)
  
 
 </div>
 
 ### [📚 Project Documentation](https://torchmate.readthedocs.io/en/latest/)
 
 Visit [Torchmate's Read The Docs Project Page](https://torchmate.readthedocs.io/en/latest/) or read following README to know more about Torchmate library
```

### Comparing `torchmate-0.1.0/setup.py` & `torchmate-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "isort>=5.13.2",
 ]
 
 REQUIRES_TESTS = [
     "pytest>=8.0.1",
     "pytest-mock>=3.12.0",
     "coverage>=7.4.1",
+    "pytest-cov>=5.0.0",
     "six>=1.16.0",
 ]
 
 REQUIRES_DOCS = [
     "Sphinx==7.2.6",
     "sphinx-copybutton==0.5.2",
     "sphinx-notfound-page==1.0.0",
@@ -103,32 +104,36 @@
     """Support setup.py upload."""
 
     description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
-        """Prints things in bold."""
-        print(s)
+        """Prints things in color."""
+        BG = "\033[46m"
+        FG = "\033[30m"
+        RESET = "\033[0m"
+        print(FG + BG + s + RESET)
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
             self.status("Removing previous builds...")
+            print("\n")
             shutil.rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
         self.status("Building Source and Wheel (universal) distribution...")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+        os.system(f"{sys.executable} setup.py sdist bdist_wheel --universal")
 
         # updated before uploading to main pypi
         self.status("Uploading the package to PyPI via Twine...")
         os.system(f"twine upload dist/*")
 
         # self.status("Pushing git tags...")
         # os.system("git tag v{0}".format(about["__version__"]))
```

### Comparing `torchmate-0.1.0/torchmate/callbacks/__init__.py` & `torchmate-0.1.1/torchmate/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/callback.py` & `torchmate-0.1.1/torchmate/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/csv_logger.py` & `torchmate-0.1.1/torchmate/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/early_stopper.py` & `torchmate-0.1.1/torchmate/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/gradient_accumulator.py` & `torchmate-0.1.1/torchmate/callbacks/gradient_accumulator.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/gradient_clipper.py` & `torchmate-0.1.1/torchmate/callbacks/gradient_clipper.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/model_checkpoint.py` & `torchmate-0.1.1/torchmate/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/wandb_logger.py` & `torchmate-0.1.1/torchmate/callbacks/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/callbacks/wandb_model_checkpoint.py` & `torchmate-0.1.1/torchmate/callbacks/wandb_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/modules/__init__.py` & `torchmate-0.1.1/torchmate/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/modules/refined_self_attention_sagan.py` & `torchmate-0.1.1/torchmate/modules/refined_self_attention_sagan.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/modules/squeeze_and_excitation.py` & `torchmate-0.1.1/torchmate/modules/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/trainer/__init__.py` & `torchmate-0.1.1/torchmate/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/trainer/trainer.py` & `torchmate-0.1.1/torchmate/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/utils/check_model_info.py` & `torchmate-0.1.1/torchmate/utils/check_model_info.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/utils/color_text.py` & `torchmate-0.1.1/torchmate/utils/color_text.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/utils/history_plotter.py` & `torchmate-0.1.1/torchmate/utils/history_plotter.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/utils/progress_bar.py` & `torchmate-0.1.1/torchmate/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate/utils/running_average.py` & `torchmate-0.1.1/torchmate/utils/running_average.py`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate.egg-info/PKG-INFO` & `torchmate-0.1.1/torchmate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: torchmate
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torchmate: A High level PyTorch Training Library
+Home-page: UNKNOWN
 Author: Abdullah Saihan Taki
 Author-email: saihan0176@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/SaihanTaki/torchmate
 Project-URL: Documentation, https://torchmate.readthedocs.io/en/latest/
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,19 +28,23 @@
 
 
 <div align="center">
  
 ![logo](https://i.ibb.co/tzsKgkR/Torchmate-logo-v1.png)  
 **A High level PyTorch Training and Utility Library**
 
-[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue)](https://torchmate.readthedocs.io/en/latest/)
-[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat)](https://pypi.org/project/torchmate/)
-[![Code style: black](https://img.shields.io/badge/Code%20Style-black-000000.svg)](https://github.com/psf/black)
-[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat)](https://github.com/SaihanTaki/torchmate/blob/master/LICENSE.txt)
-[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat)](https://www.python.org/)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/pypi.yml)
+[![GitHub Workflow Status (branch)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml/badge.svg)](https://github.com/SaihanTaki/Torchmate/actions/workflows/tests.yml) 
+[![Codecov](https://img.shields.io/codecov/c/github/SaihanTaki/Torchmate?logo=codecov&labelColor=3B434B)](https://app.codecov.io/gh/SaihanTaki/Torchmate)
+[![Read the Docs](https://img.shields.io/readthedocs/torchmate?style=flat&logo=readthedocs&logoColor=orange&color=blue&labelColor=3B434B)](https://torchmate.readthedocs.io/en/latest/)
+
+[![PyPI](https://img.shields.io/pypi/v/torchmate?style=flat&labelColor=3B434B)](https://pypi.org/project/torchmate/)
+[![Code Style](https://img.shields.io/badge/codestyle-black-black?style=flat&label=code%20style&labelColor=3B434B)](https://github.com/psf/black)
+[![MIT License](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=flat&labelColor=3B434B)](https://github.com/SaihanTaki/Torchmate/blob/main/LICENSE.txt)
+[![Python Version](https://img.shields.io/pypi/pyversions/torchmate?style=flat&labelColor=3B434B)](https://www.python.org/)
  
 
 </div>
 
 ### [📚 Project Documentation](https://torchmate.readthedocs.io/en/latest/)
 
 Visit [Torchmate's Read The Docs Project Page](https://torchmate.readthedocs.io/en/latest/) or read following README to know more about Torchmate library
@@ -133,7 +139,8 @@
 
 ```
 
 
 
 ### 🛡️ License <a name="license"></a>
 Torchmate is distributed under [MIT License](https://github.com/SaihanTaki/torchmate/blob/master/LICENSE.txt)
+
```

### Comparing `torchmate-0.1.0/torchmate.egg-info/SOURCES.txt` & `torchmate-0.1.1/torchmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchmate-0.1.0/torchmate.egg-info/requires.txt` & `torchmate-0.1.1/torchmate.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 wandb>=0.16.3
 matplotlib>=3.8.3
 
 [all]
 pytest>=8.0.1
 pytest-mock>=3.12.0
 coverage>=7.4.1
+pytest-cov>=5.0.0
 six>=1.16.0
 pre-commit>=3.6.2
 black>=24.1.1
 flake8>=7.0.0
 isort>=5.13.2
 Sphinx==7.2.6
 sphinx-copybutton==0.5.2
@@ -25,14 +26,15 @@
 autodocsumm==0.2.12
 nbsphinx==0.9.3
 
 [dev]
 pytest>=8.0.1
 pytest-mock>=3.12.0
 coverage>=7.4.1
+pytest-cov>=5.0.0
 six>=1.16.0
 pre-commit>=3.6.2
 black>=24.1.1
 flake8>=7.0.0
 isort>=5.13.2
 
 [docs]
@@ -56,8 +58,9 @@
 flake8>=7.0.0
 isort>=5.13.2
 
 [tests]
 pytest>=8.0.1
 pytest-mock>=3.12.0
 coverage>=7.4.1
+pytest-cov>=5.0.0
 six>=1.16.0
```

