# Comparing `tmp/auto_walrus-0.3.3.tar.gz` & `tmp/auto_walrus-0.3.4.tar.gz`

## Comparing `auto_walrus-0.3.3.tar` & `auto_walrus-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/auto_walrus.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/requirements-dev.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/tox.ini
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/.github/workflows/tox.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/tests/main_test.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/utils/bump_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/LICENSE
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/README.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 auto_walrus-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/auto_walrus.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/requirements-dev.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/tox.ini
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.github/workflows/tox.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/tests/main_test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/utils/bump_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 auto_walrus-0.3.4/PKG-INFO
```

### Comparing `auto_walrus-0.3.3/.pre-commit-config.yaml` & `auto_walrus-0.3.4/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 repos:
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.3.5'
+  rev: 'v0.4.1'
   hooks:
     # Run the formatter.
     - id: ruff-format
     # Run the linter.
     - id: ruff
       args: [--fix]
 - repo: https://github.com/pre-commit/mirrors-mypy
```

### Comparing `auto_walrus-0.3.3/auto_walrus.py` & `auto_walrus-0.3.4/auto_walrus.py`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.3/.github/workflows/publish_to_pypi.yml` & `auto_walrus-0.3.4/.github/workflows/publish_to_pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
           build
           --user
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -38,15 +38,15 @@
       name: pypi
       url: https://pypi.org/p/auto-walrus # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write # IMPORTANT: mandatory for trusted publishing
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -59,20 +59,20 @@
 
     permissions:
       contents: write # IMPORTANT: mandatory for making GitHub Releases
       id-token: write # IMPORTANT: mandatory for sigstore
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
       - name: Sign the dists with Sigstore
-        uses: sigstore/gh-action-sigstore-python@v1.2.3
+        uses: sigstore/gh-action-sigstore-python@v2.1.1
         with:
           inputs: >-
             ./dist/*.tar.gz
             ./dist/*.whl
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `auto_walrus-0.3.3/tests/main_test.py` & `auto_walrus-0.3.4/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     # |   ├── submodule2/
     # |   |   └── a.py
     # |   └── b.py
     # ├── submodule3/
     # |   └── c.py
     # └── pyproject.toml
 
-    if (config_content := request.node.get_closest_marker("config_content")):
+    if config_content := request.node.get_closest_marker("config_content"):
         (tmp_path / "pyproject.toml").write_text(config_content.args[0])
 
     python_files = [
         tmp_path / "submodule1" / "submodule2" / "a.py",
         tmp_path / "submodule1" / "b.py",
         tmp_path / "submodule3" / "c.py",
     ]
```

### Comparing `auto_walrus-0.3.3/utils/bump_version.py` & `auto_walrus-0.3.4/utils/bump_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,10 +16,19 @@
     version = ".".join(version[:-2] + [str(int(version[-2]) + 1), "0"])
 elif how == "major":
     version = ".".join([str(int(version[0]) + 1), "0", "0"])
 content = content.replace(f'version = "{old_version}"', f'version = "{version}"')
 with open("pyproject.toml", "w", encoding="utf-8") as f:
     f.write(content)
 
+with open("README.md", encoding="utf-8") as f:
+    content = f.read()
+content = content.replace(
+    f"rev: {old_version}",
+    f"rev: {version}",
+)
+with open("README.md", "w", encoding="utf-8") as f:
+    f.write(content)
+
 subprocess.run(["git", "commit", "-a", "-m", f"Bump version to {version}"])
 subprocess.run(["git", "tag", "-a", version, "-m", version])
 subprocess.run(["git", "push", "--follow-tags"])
```

### Comparing `auto_walrus-0.3.3/LICENSE` & `auto_walrus-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_walrus-0.3.3/README.md` & `auto_walrus-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/MarcoGorelli/auto-walrus
-    rev: v0.2.2
+    rev: 0.3.4
     hooks:
     -   id: auto-walrus
 ```
 
 ## Command-line example
 
 ```console
```

### Comparing `auto_walrus-0.3.3/pyproject.toml` & `auto_walrus-0.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto-walrus"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Automatically apply the awesome walrus operator"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    'tomli; python_version<"3.11"',
+]
 
 [project.scripts]
 auto-walrus = "auto_walrus:main"
 
 [project.urls]
 "Homepage" = "https://github.com/MarcoGorelli/auto-walrus"
 "Bug Tracker" = "https://github.com/MarcoGorelli/auto-walrus"
```

### Comparing `auto_walrus-0.3.3/PKG-INFO` & `auto_walrus-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: auto-walrus
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automatically apply the awesome walrus operator
 Project-URL: Homepage, https://github.com/MarcoGorelli/auto-walrus
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/auto-walrus
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 auto-walrus
 </h1>
 
 <p align="center">
@@ -40,15 +41,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/MarcoGorelli/auto-walrus
-    rev: v0.2.2
+    rev: 0.3.4
     hooks:
     -   id: auto-walrus
 ```
 
 ## Command-line example
 
 ```console
```

