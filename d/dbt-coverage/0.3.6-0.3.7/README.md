# Comparing `tmp/dbt_coverage-0.3.6.tar.gz` & `tmp/dbt_coverage-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coverage-0.3.6.tar", max compression
+gzip compressed data, was "dbt_coverage-0.3.7.tar", max compression
```

## Comparing `dbt_coverage-0.3.6.tar` & `dbt_coverage-0.3.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2021-11-22 15:44:35.000000 dbt_coverage-0.3.6/LICENSE.md
--rw-r--r--   0        0        0    11927 2024-03-13 14:01:20.668559 dbt_coverage-0.3.6/README.md
--rw-r--r--   0        0        0    32974 2024-02-22 08:57:25.257601 dbt_coverage-0.3.6/dbt_coverage/__init__.py
--rw-r--r--   0        0        0     2185 2024-03-13 14:04:08.857667 dbt_coverage-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    13044 1970-01-01 00:00:00.000000 dbt_coverage-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-11-22 15:44:35.000000 dbt_coverage-0.3.7/LICENSE.md
+-rw-r--r--   0        0        0    11722 2024-04-23 10:44:08.300731 dbt_coverage-0.3.7/README.md
+-rw-r--r--   0        0        0    32974 2024-02-22 08:57:25.257601 dbt_coverage-0.3.7/dbt_coverage/__init__.py
+-rw-r--r--   0        0        0     2185 2024-04-23 10:44:08.302388 dbt_coverage-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    12839 1970-01-01 00:00:00.000000 dbt_coverage-0.3.7/PKG-INFO
```

### Comparing `dbt_coverage-0.3.6/LICENSE.md` & `dbt_coverage-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_coverage-0.3.6/README.md` & `dbt_coverage-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <a href="https://pypi.org/project/dbt-coverage/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dbt-coverage"></a>
 <a href="https://pepy.tech/project/dbt-coverage"><img alt="Downloads" src="https://pepy.tech/badge/dbt-coverage"></a>
 ![GitHub last commit](https://img.shields.io/github/last-commit/slidoapp/dbt-coverage)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-coverage)
 ![PyPI - Format](https://img.shields.io/pypi/format/dbt-coverage)
 ![dbt versions](https://img.shields.io/badge/dbt-1.0-blue)
 <a href="https://github.com/slidoapp/dbt-coverage/blob/main/LICENSE.md"><img alt="License: MIT" src="https://img.shields.io/github/license/slidoapp/dbt-coverage"></a>
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield)
 
 
 _One-stop-shop for docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._
 
 Optimized for dbt 1.0, see [full support matrix](#supported-dbt-versions).
 
 ## Why do I need something like this?
```

#### html2text {}

```diff
@@ -1,36 +1,33 @@
 # dbt-coverage _[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]![GitHub last commit](https://img.shields.io/
 github/last-commit/slidoapp/dbt-coverage) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/dbt-coverage) ![PyPI - Format](https://
 img.shields.io/pypi/format/dbt-coverage) ![dbt versions](https://
-img.shields.io/badge/dbt-1.0-blue) _[_L_i_c_e_n_s_e_:_ _M_I_T_][![FOSSA Status](https://
-app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
-coverage.svg?type=shield)](https://app.fossa.com/projects/
-git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield) _One-stop-shop for
-docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._
-Optimized for dbt 1.0, see [full support matrix](#supported-dbt-versions). ##
-Why do I need something like this? _**[`dbt-coverage`](https://github.com/
-slidoapp/dbt-coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what
-[`coverage.py`](https://github.com/nedbat/coveragepy) and [`interrogate`]
-(https://interrogate.readthedocs.io/en/latest/) are to Python.**_ It is a
-single CLI tool which checks your `dbt` project for missing documentation and
-tests. Keeping documentation and tests close to the actual SQL code that
-generates the final model is one of the best design choices of `dbt`. It
-ensures documentation is actually useful and tests are actually used. But how
-do you make adding those a habit in your [`dbt`](https://github.com/dbt-labs/
-dbt) project? That is exactly where `dbt-coverage` comes in. It will - Give you
-a better sense of the level of documentation and test coverage in your project;
-- Help your CI/CD pipeline make sure new changes include documentation and
-tests; - Let you quickly assess the documentation and tests of a new `dbt`
-project you get your hands on. Still not convinced? Here are some more
-features: - â¨ **zero-config**: just install it and run it, there is nothing
-to set up - ð **minimal dependences**: the only dependencies are [`click`]
-(https://click.palletsprojects.com/en/8.0.x/) (already installed with [`dbt`]
-(https://github.com/dbt-labs/dbt)) and [`typer`](https://typer.tiangolo.com/
-tutorial/) - ð¦ **very small**: at ~480 [SLOC](https://en.wikipedia.org/wiki/
+img.shields.io/badge/dbt-1.0-blue) _[_L_i_c_e_n_s_e_:_ _M_I_T_]_One-stop-shop for docs and
+test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._ Optimized
+for dbt 1.0, see [full support matrix](#supported-dbt-versions). ## Why do I
+need something like this? _**[`dbt-coverage`](https://github.com/slidoapp/dbt-
+coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what [`coverage.py`]
+(https://github.com/nedbat/coveragepy) and [`interrogate`](https://
+interrogate.readthedocs.io/en/latest/) are to Python.**_ It is a single CLI
+tool which checks your `dbt` project for missing documentation and tests.
+Keeping documentation and tests close to the actual SQL code that generates the
+final model is one of the best design choices of `dbt`. It ensures
+documentation is actually useful and tests are actually used. But how do you
+make adding those a habit in your [`dbt`](https://github.com/dbt-labs/dbt)
+project? That is exactly where `dbt-coverage` comes in. It will - Give you a
+better sense of the level of documentation and test coverage in your project; -
+Help your CI/CD pipeline make sure new changes include documentation and tests;
+- Let you quickly assess the documentation and tests of a new `dbt` project you
+get your hands on. Still not convinced? Here are some more features: - â¨
+**zero-config**: just install it and run it, there is nothing to set up - ð
+**minimal dependences**: the only dependencies are [`click`](https://
+click.palletsprojects.com/en/8.0.x/) (already installed with [`dbt`](https://
+github.com/dbt-labs/dbt)) and [`typer`](https://typer.tiangolo.com/tutorial/) -
+ð¦ **very small**: at ~480 [SLOC](https://en.wikipedia.org/wiki/
 Source_lines_of_code), you can easily validate it works as advertised ## Demo
 The package was presented during [Coalesce](https://coalesce.getdbt.com/), the
 annual dbt conference, as a part of the talk [_From 100 spreadsheets to 100
 data analysts: the story of dbt at Slido_](https://www.getdbt.com/coalesce-
 2021/from-spreadsheets-to-data-analysts-the-story-of-dbt-at-slido/). Watch a
 demo in the video below. [![Demo video](assets/demo.png)](https://youtu.be/
 YA0yqYSs9BQ?t=936) ## Installation ``` pip install dbt-coverage ``` ## Usage
```

### Comparing `dbt_coverage-0.3.6/dbt_coverage/__init__.py` & `dbt_coverage-0.3.7/dbt_coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_coverage-0.3.6/pyproject.toml` & `dbt_coverage-0.3.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-coverage"
-version = "0.3.6"
+version = "0.3.7"
 description = "One-stop-shop for docs and test coverage of dbt projects"
 authors = ["Andrej Švec <asvec@slido.com>"]
 readme = 'README.md'
 license = "MIT"
 repository = "https://github.com/slidoapp/dbt-coverage"
 homepage = "https://github.com/slidoapp/dbt-coverage"
 documentation = "https://github.com/slidoapp/dbt-coverage"
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 typer = ">=0.4,<1"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "==24.2.0", python = ">=3.8"}  # Use the same version as in .pre-commit-config.yaml
 isort = {version = "==5.13.2", python = ">=3.8"}  # Use the same version as in .pre-commit-config.yaml
 pre-commit = {version = "^3.6.2", python = ">=3.9"}
```

### Comparing `dbt_coverage-0.3.6/PKG-INFO` & `dbt_coverage-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: dbt-coverage
-Version: 0.3.6
+Version: 0.3.7
 Summary: One-stop-shop for docs and test coverage of dbt projects
 Home-page: https://github.com/slidoapp/dbt-coverage
 License: MIT
 Author: Andrej Švec
 Author-email: asvec@slido.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: typer (>=0.4,<1)
 Project-URL: Documentation, https://github.com/slidoapp/dbt-coverage
 Project-URL: Repository, https://github.com/slidoapp/dbt-coverage
 Description-Content-Type: text/markdown
 
 # dbt-coverage
 
 <a href="https://pypi.org/project/dbt-coverage/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dbt-coverage"></a>
 <a href="https://pepy.tech/project/dbt-coverage"><img alt="Downloads" src="https://pepy.tech/badge/dbt-coverage"></a>
 ![GitHub last commit](https://img.shields.io/github/last-commit/slidoapp/dbt-coverage)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-coverage)
 ![PyPI - Format](https://img.shields.io/pypi/format/dbt-coverage)
 ![dbt versions](https://img.shields.io/badge/dbt-1.0-blue)
 <a href="https://github.com/slidoapp/dbt-coverage/blob/main/LICENSE.md"><img alt="License: MIT" src="https://img.shields.io/github/license/slidoapp/dbt-coverage"></a>
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield)
 
 
 _One-stop-shop for docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._
 
 Optimized for dbt 1.0, see [full support matrix](#supported-dbt-versions).
 
 ## Why do I need something like this?
```

#### html2text {}

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1 Name: dbt-coverage Version: 0.3.6 Summary: One-stop-shop
+Metadata-Version: 2.1 Name: dbt-coverage Version: 0.3.7 Summary: One-stop-shop
 for docs and test coverage of dbt projects Home-page: https://github.com/
 slidoapp/dbt-coverage License: MIT Author: Andrej Å vec Author-email:
-asvec@slido.com Requires-Python: >=3.6,<4.0 Classifier: Development Status :: 4
+asvec@slido.com Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Dist: typer (>=0.4,<1) Project-URL: Documentation, https://
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.6 Requires-Dist: typer (>=0.4,<1) Project-URL: Documentation, https://
 github.com/slidoapp/dbt-coverage Project-URL: Repository, https://github.com/
 slidoapp/dbt-coverage Description-Content-Type: text/markdown # dbt-coverage
 _[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]![GitHub last commit](https://img.shields.io/github/last-
 commit/slidoapp/dbt-coverage) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/dbt-coverage) ![PyPI - Format](https://img.shields.io/pypi/
 format/dbt-coverage) ![dbt versions](https://img.shields.io/badge/dbt-1.0-blue)
-_[_L_i_c_e_n_s_e_:_ _M_I_T_][![FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://
-app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
-coverage?ref=badge_shield) _One-stop-shop for docs and test coverage of [`dbt`]
-(https://github.com/dbt-labs/dbt) projects._ Optimized for dbt 1.0, see [full
-support matrix](#supported-dbt-versions). ## Why do I need something like this?
-_**[`dbt-coverage`](https://github.com/slidoapp/dbt-coverage) is to [`dbt`]
-(https://github.com/dbt-labs/dbt) what [`coverage.py`](https://github.com/
-nedbat/coveragepy) and [`interrogate`](https://interrogate.readthedocs.io/en/
-latest/) are to Python.**_ It is a single CLI tool which checks your `dbt`
-project for missing documentation and tests. Keeping documentation and tests
-close to the actual SQL code that generates the final model is one of the best
-design choices of `dbt`. It ensures documentation is actually useful and tests
-are actually used. But how do you make adding those a habit in your [`dbt`]
-(https://github.com/dbt-labs/dbt) project? That is exactly where `dbt-coverage`
-comes in. It will - Give you a better sense of the level of documentation and
-test coverage in your project; - Help your CI/CD pipeline make sure new changes
+_[_L_i_c_e_n_s_e_:_ _M_I_T_]_One-stop-shop for docs and test coverage of [`dbt`](https://
+github.com/dbt-labs/dbt) projects._ Optimized for dbt 1.0, see [full support
+matrix](#supported-dbt-versions). ## Why do I need something like this? _**
+[`dbt-coverage`](https://github.com/slidoapp/dbt-coverage) is to [`dbt`](https:
+//github.com/dbt-labs/dbt) what [`coverage.py`](https://github.com/nedbat/
+coveragepy) and [`interrogate`](https://interrogate.readthedocs.io/en/latest/
+) are to Python.**_ It is a single CLI tool which checks your `dbt` project for
+missing documentation and tests. Keeping documentation and tests close to the
+actual SQL code that generates the final model is one of the best design
+choices of `dbt`. It ensures documentation is actually useful and tests are
+actually used. But how do you make adding those a habit in your [`dbt`](https:/
+/github.com/dbt-labs/dbt) project? That is exactly where `dbt-coverage` comes
+in. It will - Give you a better sense of the level of documentation and test
+coverage in your project; - Help your CI/CD pipeline make sure new changes
 include documentation and tests; - Let you quickly assess the documentation and
 tests of a new `dbt` project you get your hands on. Still not convinced? Here
 are some more features: - â¨ **zero-config**: just install it and run it,
 there is nothing to set up - ð **minimal dependences**: the only
 dependencies are [`click`](https://click.palletsprojects.com/en/8.0.x/)
 (already installed with [`dbt`](https://github.com/dbt-labs/dbt)) and [`typer`]
 (https://typer.tiangolo.com/tutorial/) - ð¦ **very small**: at ~480 [SLOC]
```

