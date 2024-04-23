# Comparing `tmp/github_custom_actions-1.3.0.tar.gz` & `tmp/github_custom_actions-2.0.0.tar.gz`

## Comparing `github_custom_actions-1.3.0.tar` & `github_custom_actions-2.0.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.dev.in
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.dev.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.in
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.txt
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/static.yml
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/mkdocs.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/input_output_typed.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/install_pipx_macos.sh
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/quick_start.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/github_env_vars.md
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/index.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/inputs.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/installation.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/reference.md
--rw-r--r--   0        0        0    52770 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/github_env_vars.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/index.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/installation.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/attr_dict_vars.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/env_attr_dict_vars.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/file_attr_dict_vars.py
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_action_base.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_env_attr_dict_vars.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_file_attr_dict_vars.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_github_vars.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.dev.in
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.txt
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/input_output_typed.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/install_pipx_macos.sh
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/quick_start.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/github_env_vars.md
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/index.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/inputs.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/installation.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/outputs.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/reference.md
+-rw-r--r--   0        0        0    80255 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/github_env_vars.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/inputs.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/installation.md
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/outputs.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/attr_dict_vars.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/env_attr_dict_vars.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/file_attr_dict_vars.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_action_base.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_env_attr_dict_vars.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_file_attr_dict_vars.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/PKG-INFO
```

### Comparing `github_custom_actions-1.3.0/.pre-commit-config.yaml` & `github_custom_actions-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/activate.sh` & `github_custom_actions-2.0.0/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/requirements.dev.txt` & `github_custom_actions-2.0.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/tasks.py` & `github_custom_actions-2.0.0/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 import sys
 
 from invoke import task, Context, Collection
 import subprocess
 
 
 def get_allowed_doc_languages():
@@ -62,14 +63,18 @@
 
 def docs_task_factory(language: str):
     @task
     def docs(c: Context):
         """Docs preview for the language specified."""
         c.run("open -a 'Google Chrome' http://127.0.0.1:8000/github-custom-actions/")
         c.run(f"scripts/docs-render-config.sh {language}")
+        if language != "en":
+            shutil.rmtree(f"./docs/src/{language}/images", ignore_errors=True)
+            shutil.copytree("./docs/src/en/images", f"./docs/src/{language}/images")
+            shutil.copy("./docs/src/en/reference.md", f"./docs/src/{language}/reference.md")
         c.run("mkdocs serve -f docs/_mkdocs.yml")
 
     return docs
 
 
 @task
 def uv(c: Context):
```

### Comparing `github_custom_actions-1.3.0/.github/workflows/ci.yml` & `github_custom_actions-2.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/.github/workflows/docs.yml` & `github_custom_actions-2.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/.github/workflows/pip_publish.yml` & `github_custom_actions-2.0.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/.github/workflows/static.yml` & `github_custom_actions-2.0.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/docs/mkdocs.yml` & `github_custom_actions-2.0.0/docs/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs_dir: 'src/LANGUAGE'
 site_dir: '../site/SITE_PREFIX'
 
 nav:
   - index.md
   - installation.md
   - inputs.md
+  - outputs.md
   - github_env_vars.md
 
 plugins:
   - awesome-pages
   - search:
       lang: LANGUAGE
   - mkdocstrings:
```

### Comparing `github_custom_actions-1.3.0/docs/includes/input_output_typed.py` & `github_custom_actions-2.0.0/docs/includes/input_output_typed.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     inputs: MyInputs
     outputs: MyOutputs
 
     def main(self):
         if self.inputs.my_path is None:
             raise ValueError("my-path is required")
         self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs.runner_os = self.vars.runner_os
+        self.outputs.runner_os = self.env.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day, {{ inputs['name'] }}!"
             )
         )
```

### Comparing `github_custom_actions-1.3.0/docs/src/en/index.md` & `github_custom_actions-2.0.0/docs/src/en/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # github-custom-actions
 
 Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
 
-It works with Python 3.7 and up, so even those dusty old self-hosted action runners can handle it like champs.
+It works with Python 3.7 and up, so even those dusty old self-hosted action runners can 
+handle it like champs.
 
 ### Quick start
 
 ```python
 --8<-- "quick_start.py"
 ```
 
 This example uses the `runner_os` variable from GitHub environment variables. 
-All variables from the GitHub environment are available in the `vars`, 
+All variables from the GitHub environment are available in the `env`, 
 with descriptions shown in your IDE on mouse hover:
 ![var_ide_hover_docstring.jpg](images/var_ide_hover_docstring.jpg)
 
 The action gets a value from the `my-input` action input and renders 
 it in the action step summary on the GitHub build summary.
 
 It also returns a value to the `runner-os` action output.
 
-The main block runs the `main()` method of the action with the necessary boilerplate to catch and report exceptions.
+The main block runs the `main()` method of the action with the necessary boilerplate 
+to catch and report exceptions.
 
 ### Explicitly defined inputs and outputs
 
 With explicitly defined inputs and outputs, you can use typo-checked code autocompletion:
 
 ```python
 --8<-- "input_output_typed.py"
@@ -33,11 +35,14 @@
 Note that you only define the types of inputs and outputs, and instances are created automatically
 upon `MyAction` initialization.
 
 Now you can utilize the attributes defined in the `inputs` and `outputs` classes of the action. 
 All attributes names are converted to `kebab-case`, allowing dot notation like `inputs.my_input`
 to replace the `inputs['my-input']`.
 
+Inputs defined as Path will be converted to `Path` objects.
+
 But still can use the `inputs['my-input']` style if you prefer.
 
 ### Example of usage
-[allure-report action](https://github.com/andgineer/allure-report)
+
+[Allure Test Report Action](hhttps://github.com/andgineer/allure-report/blob/main/src/allure_generate.py)
```

### Comparing `github_custom_actions-1.3.0/docs/src/en/installation.md` & `github_custom_actions-2.0.0/docs/src/en/installation.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/docs/src/ru/index.md` & `github_custom_actions-2.0.0/docs/src/ru/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ```python
 --8<-- "quick_start.py"
 ```
 
 Этот пример использует переменную `runner_os` из переменных окружения GitHub. 
 
-Все переменные из окружения GitHub доступны в `vars`, 
+Все переменные из окружения GitHub доступны в `env`, 
 описания которых отображаются в вашей IDE при наведении мыши:
 ![var_ide_hover_docstring.jpg](images/var_ide_hover_docstring.jpg)
 
 Action получает значение из action input `my-input` и отображает его 
 в `step summary` на странице билда GitHub.
 
 Оно также возвращает значение в action output `runner-os`.
@@ -35,12 +35,15 @@
 Обратите внимание, что вы только определяете типы входов и выходов, а экземпляры этих классов создаются автоматически
 при инициализации `MyAction`.
 
 Теперь вы можете использовать атрибуты, определенные в классах `inputs` и `outputs` действия. 
 Все имена атрибутов преобразуются в `kebab-case`, что позволяет использовать точечную нотацию, например `inputs.my_input`, 
 вместо `inputs['my-input']`.
 
+Если вы определили input как `Path`, он будет преобразован в объект `Path`.
+
 При желании вы все также можете использовать стиль `inputs['my-input']`.
 
 ### Пример использования
-[allure-report action](https://github.com/andgineer/allure-report)
+
+[Allure Test Report Action](https://github.com/andgineer/allure-report/blob/main/src/allure_generate.py)
```

### Comparing `github_custom_actions-1.3.0/docs/src/ru/installation.md` & `github_custom_actions-2.0.0/docs/src/ru/installation.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/scripts/include_pyproject_requirements.py` & `github_custom_actions-2.0.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/scripts/verup.sh` & `github_custom_actions-2.0.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/src/github_custom_actions/action_base.py` & `github_custom_actions-2.0.0/src/github_custom_actions/action_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
         """Initialize the property descriptor.
 
         `var_name` is the name of the object's `vars` attribute with the path to the file.
         """
         self.var_name = var_name
 
     def __get__(self, obj: Any, objtype: Any = None) -> str:
-        path = getattr(obj.vars, self.var_name)
+        path = getattr(obj.env, self.var_name)
         try:
             return path.read_text()  # type: ignore
         except FileNotFoundError:
             return ""
 
     def __set__(self, obj: Any, value: str) -> None:
-        path = getattr(obj.vars, self.var_name)
+        path = getattr(obj.env, self.var_name)
         try:
             path.write_text(value)
         except FileNotFoundError:
             path.parent.mkdir(parents=True, exist_ok=True)
             path.write_text(value)
 
 
@@ -39,22 +39,22 @@
     """Base class for GitHub Actions.
 
     Implement main() method in the subclass.
     """
 
     inputs: ActionInputs
     outputs: ActionOutputs
-    vars: GithubVars
+    env: GithubVars
 
     def __init__(self) -> None:
         # Initialize inputs, outputs according to the type than could be set in subclass.
         types = get_type_hints(self.__class__)
         self.inputs = types["inputs"]()
         self.outputs = types["outputs"]()
-        self.vars = GithubVars()
+        self.env = GithubVars()
 
         base_dir = Path(__file__).resolve().parent
         templates_dir = base_dir / "templates"
         self.environment = Environment(loader=FileSystemLoader(str(templates_dir)))
 
     summary = FileTextProperty("github_step_summary")
 
@@ -67,13 +67,13 @@
         try:
             self.main()
         except Exception:  # pylint: disable=broad-except
             traceback.print_exc(file=sys.stderr)
             sys.exit(1)
 
     def render(self, template: str) -> str:
-        """Render template with context including inputs, outputs, and vars."""
+        """Render template with context including inputs, outputs, and env."""
         return Template(template.replace("\\n", "\n")).render(
-            vars=self.vars,
+            env=self.env,
             inputs=self.inputs,
             outputs=self.outputs,
         )
```

### Comparing `github_custom_actions-1.3.0/src/github_custom_actions/attr_dict_vars.py` & `github_custom_actions-2.0.0/src/github_custom_actions/attr_dict_vars.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from typing import Dict, Any
 
 
 class AttrDictVars:
     """Common base class for accessing variables as attributes or dict."""
 
     _type_hints_cache: Dict[str, Dict[str, Any]] = {}
-    _external_name_prefix = ""
 
     @classmethod
     def _get_type_hints(cls) -> Dict[str, Any]:
         class_name = cls.__name__
         if class_name not in cls._type_hints_cache:
             cls._type_hints_cache[class_name] = typing.get_type_hints(cls)
         return cls._type_hints_cache[class_name]
 
     def _attr_to_var_name(self, name: str) -> str:
         return name.replace("_", "-")
+
+    def _external_name(self, name: str) -> str:
+        return name
```

### Comparing `github_custom_actions-1.3.0/src/github_custom_actions/file_attr_dict_vars.py` & `github_custom_actions-2.0.0/src/github_custom_actions/file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/src/github_custom_actions/github_vars.py` & `github_custom_actions-2.0.0/src/github_custom_actions/github_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 
 class GithubVars(EnvAttrDictVars):
     """GitHub Action environment variables.
 
     https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
 
     Usage:
+       ```python
        class MyAction:
            @property
-           def vars(self):
+           def env(self):
                return GithubVars()
 
        action = MyAction()
-       print(action.vars.github_repository)
+       print(action.env.github_repository)
+       ```
 
     Thanks to the docstrings your IDE will provide you with doc hints when you hover over the property.
     We do not load the attributes on the class init but do it Lazily.
     Once read, the value is stored in the instance dictionary and is not extracted from env anymore.
 
-    Only described Github vars are loaded.
+    Converts attribute names to uppercase.
+    Leave dict-style names unchanged.
+
     Paths and files have type Path.
     """
 
     # pylint: disable=abstract-method  # we want RO implementation that raises NotImplementedError on write
 
     def _attr_to_var_name(self, name: str) -> str:
-        return name  # leave as is
+        return name.upper()
 
     CI: str
     """Always set to true."""
 
     github_action: str
     """The name of the action currently running, or the id of a step.
     For example, for an action, __repo-owner_name-of-action-repo.
```

### Comparing `github_custom_actions-1.3.0/tests/conftest.py` & `github_custom_actions-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/tests/test_env_attr_dict_vars.py` & `github_custom_actions-2.0.0/tests/test_env_attr_dict_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     }):
         yield
 
 
 class MyTextFileVars(EnvAttrDictVars):
     documented_var: str
 
-    def __init__(self) -> None:
-        super().__init__(prefix='INPUT_')
+    def _external_name(self, name: str) -> str:
+        return "INPUT_" + name.upper()
 
 
 def test_env_attr_dict_vars_attribute_access(setup_env_vars):
     vars = MyTextFileVars()
     assert vars.documented_var == 'test_value'
```

### Comparing `github_custom_actions-1.3.0/tests/test_file_attr_dict_vars.py` & `github_custom_actions-2.0.0/tests/test_file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/tests/test_github_vars.py` & `github_custom_actions-2.0.0/tests/test_github_vars.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,28 @@
     monkeypatch.delenv("GITHUB_ACTION")
     assert vars.github_action == "test"  # Cached value
 
 
 def test_github_vars_unknown():
     vars = GithubVars()
     os.environ["GITHUB_UNKNOWN"] = "test"
+    assert vars["GITHUB_UNKNOWN"] == "test"
     with pytest.raises(AttributeError, match=r"Unknown github_unknown"):
         assert vars.github_unknown == "test"
 
 
 def test_github_vars_path_variable(monkeypatch):
     vars = GithubVars()
     monkeypatch.setenv("GITHUB_OUTPUT", "a/b")
     assert str(vars.github_output.parent) == "a"
 
 
 def test_github_vars_empty_path(monkeypatch):
     vars = GithubVars()
     monkeypatch.setenv("GITHUB_OUTPUT", "")
     assert vars.github_output is None
+
+
+def test_github_vars_dict_exact(monkeypatch):
+    vars = GithubVars()
+    monkeypatch.setenv("snake_eatsCamel-NOT-kebab", "a")
+    assert vars["snake_eatsCamel-NOT-kebab"] == "a"
```

### Comparing `github_custom_actions-1.3.0/tests/test_inputs_outputs.py` & `github_custom_actions-2.0.0/tests/test_inputs_outputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 def test_output_set_and_read(action):
     """Test setting and getting output values."""
     action.outputs["my_output"] = "output_value"
     with pytest.raises(AttributeError):
         action.outputs.my_output2 = "output_value2"
     action.outputs.my_output = "output_value2"
 
-    assert action.vars.github_output.read_text() == "my_output=output_value\nmy-output=output_value2"
+    assert action.env.github_output.read_text() == "my_output=output_value\nmy-output=output_value2"
 
 
 def test_input_caching(action, monkeypatch):
     """Test that input is loaded from env var only once."""
     monkeypatch.delenv("INPUT_MY-INPUT")
     with pytest.raises(AttributeError):
         assert action.inputs.my_input == "value1"
 
     monkeypatch.setenv("INPUT_MY-INPUT", "value1")
     assert action.inputs.my_input == "value1"
 
     monkeypatch.delenv("INPUT_MY-INPUT")
     assert action.inputs.my_input == "value1"  # from cache
+
+
+def test_output_dict_exact(action):
+    action.outputs["snake_eatsCamel-NOT-kebab"] = "a"
+    assert action.env.github_output.read_text() == "snake_eatsCamel-NOT-kebab=a"
```

### Comparing `github_custom_actions-1.3.0/LICENSE.txt` & `github_custom_actions-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/README.md` & `github_custom_actions-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #### Example of usage
 
 ```python
 from github_custom_actions import ActionBase
     
 class MyAction(ActionBase):
     def main(self):
-        self.outputs["runner-os"] = self.vars.runner_os
+        self.outputs["runner-os"] = self.env.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs['my-input'] }}.\n"
                 "Have a nice day!"
             )
         )
```

### Comparing `github_custom_actions-1.3.0/pyproject.toml` & `github_custom_actions-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.3.0/PKG-INFO` & `github_custom_actions-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 1.3.0
+Version: 2.0.0
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -43,15 +43,15 @@
 #### Example of usage
 
 ```python
 from github_custom_actions import ActionBase
     
 class MyAction(ActionBase):
     def main(self):
-        self.outputs["runner-os"] = self.vars.runner_os
+        self.outputs["runner-os"] = self.env.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs['my-input'] }}.\n"
                 "Have a nice day!"
             )
         )
```

