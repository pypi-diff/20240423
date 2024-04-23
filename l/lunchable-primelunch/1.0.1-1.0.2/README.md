# Comparing `tmp/lunchable_primelunch-1.0.1.tar.gz` & `tmp/lunchable_primelunch-1.0.2.tar.gz`

## Comparing `lunchable_primelunch-1.0.1.tar` & `lunchable_primelunch-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.releaserc.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/mkdocs.yaml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements.txt
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/dependabot.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/docs/contributing.md
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/docs/gen_pages.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/docs/index.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/__about__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/__main__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/cli.py
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/primelunch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/lunchable_primelunch/py.typed
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-all.py3.10.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-all.py3.11.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-all.py3.12.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-all.py3.8.txt
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-all.py3.9.txt
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-lint.txt
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/requirements/requirements-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/LICENSE
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/README.md
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.releaserc.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/mkdocs.yaml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/docs/contributing.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/docs/gen_pages.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/docs/index.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/__about__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/__main__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/cli.py
+-rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/primelunch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/lunchable_primelunch/py.typed
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-all.py3.10.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-all.py3.11.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-all.py3.12.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-all.py3.8.txt
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-all.py3.9.txt
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-lint.txt
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/requirements/requirements-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/README.md
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 lunchable_primelunch-1.0.2/PKG-INFO
```

### Comparing `lunchable_primelunch-1.0.1/.pre-commit-config.yaml` & `lunchable_primelunch-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.releaserc.json` & `lunchable_primelunch-1.0.2/.releaserc.json`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/mkdocs.yaml` & `lunchable_primelunch-1.0.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements.txt` & `lunchable_primelunch-1.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.github/semantic_release/package-lock.json` & `lunchable_primelunch-1.0.2/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.github/workflows/lint.yaml` & `lunchable_primelunch-1.0.2/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.github/workflows/publish.yaml` & `lunchable_primelunch-1.0.2/.github/workflows/publish.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 name: Publishing
 on:
     release:
         types:
             - published
+    workflow_dispatch:
 jobs:
     pypi-publish:
         name: PyPI
-        if: github.repository_owner == 'juftin'
+        if: github.repository_owner == 'juftin' && (github.event_name == 'release' || (github.event_name == 'workflow_dispatch' && github.actor == 'juftin'))
         runs-on: ubuntu-latest
         concurrency:
             group: ${{ github.workflow }}-${{ github.job }}
             cancel-in-progress: false
+        environment:
+          name: pypi
+          url: https://pypi.org/p/lunchable-primelunch
+        permissions:
+          id-token: write
         steps:
             - name: Check out the repository
               uses: actions/checkout@v4
               with:
                   fetch-depth: 2
             - name: Set up Python
               uses: actions/setup-python@v5
@@ -25,11 +31,8 @@
                   python -m pip install --upgrade pip
                   python -m pip install -q hatch pre-commit
                   hatch --version
             - name: Build package
               run: |
                   hatch build
             - name: Publish package on PyPI
-              uses: pypa/gh-action-pypi-publish@v1.8.11
-              with:
-                  user: __token__
-                  password: ${{ secrets.PYPI_TOKEN }}
+              uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `lunchable_primelunch-1.0.1/.github/workflows/release.yaml` & `lunchable_primelunch-1.0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.github/workflows/tests.yaml` & `lunchable_primelunch-1.0.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/docs/contributing.md` & `lunchable_primelunch-1.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/docs/gen_pages.py` & `lunchable_primelunch-1.0.2/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/docs/index.md` & `lunchable_primelunch-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/lunchable_primelunch/cli.py` & `lunchable_primelunch-1.0.2/lunchable_primelunch/cli.py`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/lunchable_primelunch/primelunch.py` & `lunchable_primelunch-1.0.2/lunchable_primelunch/primelunch.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,19 +81,39 @@
         List[LunchableModel]
         """
         array_df = df.copy()
         array_df = array_df.replace(np.NaN, None)
         model_array = array_df.to_dict(orient="records")
         return [model_type.model_validate(item) for item in model_array]
 
+    def _remove_subtotal_row(self, amazon_df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Inspect the last row of the dataframe and delete it if any of its values
+        contain the string "=SUBTOTAL".
+
+        Parameters
+        ----------
+        amazon_df : pd.DataFrame
+            The dataframe to inspect and potentially modify.
+
+        Returns
+        -------
+        pd.DataFrame
+            The potentially modified dataframe.
+        """
+        if amazon_df.iloc[-1].astype(str).str.contains("=SUBTOTAL").any():
+            amazon_df = amazon_df[:-1]
+        return amazon_df
+
     def amazon_to_df(self) -> pd.DataFrame:
         """
         Read an Amazon Data File to a DataFrame
 
         This is pretty simple, except duplicate header rows need to be cleaned
+        If the exporter included a "subtotal" row, it is removed
 
         Returns
         -------
         pd.DataFrame
         """
         dt64: np.dtype[datetime64] = np.dtype("datetime64[ns]")
         expected_columns = {
@@ -112,14 +132,17 @@
             usecols=expected_columns.keys(),
         )
         header_row_eval = pd.concat(
             [amazon_df[item] == item for item in expected_columns.keys()], axis=1
         ).all(axis=1)
         duplicate_header_rows = np.where(header_row_eval)[0]
         amazon_df.drop(duplicate_header_rows, axis=0, inplace=True)
+
+        amazon_df = self._remove_subtotal_row(amazon_df)
+
         amazon_df["total"] = (
             amazon_df["total"].astype("string").str.replace(",", "").astype(np.float64)
         )
         amazon_df = amazon_df.astype(dtype=expected_columns, copy=True, errors="raise")
         logger.info("Amazon Data File loaded: %s", self.file_path)
         return amazon_df
```

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-all.py3.10.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-all.py3.10.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-all.py3.11.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-all.py3.11.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-all.py3.12.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-all.py3.12.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-all.py3.8.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-all.py3.8.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-all.py3.9.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-all.py3.9.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-docs.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/requirements/requirements-test.txt` & `lunchable_primelunch-1.0.2/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/.gitignore` & `lunchable_primelunch-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/LICENSE` & `lunchable_primelunch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/README.md` & `lunchable_primelunch-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/pyproject.toml` & `lunchable_primelunch-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lunchable_primelunch-1.0.1/PKG-INFO` & `lunchable_primelunch-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lunchable-primelunch
-Version: 1.0.1
+Version: 1.0.2
 Summary: LunchMoney Amazon Transaction Updater
 Project-URL: Documentation, https://juftin.github.io/lunchable-primelunch
 Project-URL: Issues, https://github.com/juftin/lunchable-primelunch/issues
 Project-URL: Source, https://github.com/juftin/lunchable-primelunch
 Author-email: Justin Flannery <juftin@juftin.com>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lunchable-primelunch Version: 1.0.1 Summary:
+Metadata-Version: 2.3 Name: lunchable-primelunch Version: 1.0.2 Summary:
 LunchMoney Amazon Transaction Updater Project-URL: Documentation, https://
 juftin.github.io/lunchable-primelunch Project-URL: Issues, https://github.com/
 juftin/lunchable-primelunch/issues Project-URL: Source, https://github.com/
 juftin/lunchable-primelunch Author-email: Justin Flannery
 juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

