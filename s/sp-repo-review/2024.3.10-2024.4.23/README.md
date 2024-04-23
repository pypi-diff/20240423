# Comparing `tmp/sp_repo_review-2024.3.10.tar.gz` & `tmp/sp_repo_review-2024.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar 11 02:34:33 2024, max compression
+gzip compressed data, last modified: Mon Apr 22 06:34:37 2024, max compression
```

## Comparing `sp_repo_review-2024.3.10.tar` & `sp_repo_review-2024.4.23.tar`

### file list

```diff
@@ -1,133 +1,135 @@
--rw-r--r--   0        0        0      125 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.git_archival.txt
--rw-r--r--   0        0        0       45 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.gitattributes
--rw-r--r--   0        0        0     2533 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.pre-commit-config.yaml
--rw-r--r--   0        0        0      267 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      474 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.readthedocs.yaml
--rw-r--r--   0        0        0        6 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.ruby-version
--rw-r--r--   0        0        0     1182 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/Gemfile
--rw-r--r--   0        0        0     3808 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/Gemfile.lock
--rw-r--r--   0        0        0    19090 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/README.md
--rw-r--r--   0        0        0     1106 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/_config.yml
--rw-r--r--   0        0        0      763 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/action.yml
--rw-r--r--   0        0        0     2062 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/cookiecutter.json
--rw-r--r--   0        0        0     2806 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/copier.yml
--rw-r--r--   0        0        0    15154 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/noxfile.py
--rw-r--r--   0        0        0      527 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      223 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/dependabot.yml
--rw-r--r--   0        0        0      825 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/bump.yml
--rw-r--r--   0        0        0      726 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2109 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     4752 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0     1262 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/LICENSE
--rw-r--r--   0        0        0      829 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/README.md
--rw-r--r--   0        0        0     2180 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      671 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0     2777 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_includes/pyproject.md
--rw-r--r--   0        0        0      145 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_includes/toc.html
--rw-r--r--   0        0        0      435 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_plugins/details.rb
--rw-r--r--   0        0        0      512 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_plugins/repo_review.rb
--rw-r--r--   0        0        0     1541 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_plugins/tabs.rb
--rw-r--r--   0        0        0       22 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2627 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    11199 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     4158 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/index.md
--rw-r--r--   0        0        0     5216 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0    13400 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/docs.md
--rw-r--r--   0        0        0    23210 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     8081 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     7663 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     3202 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/index.md
--rw-r--r--   0        0        0    10374 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    18538 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9814 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/packaging_compiled.md
--rw-r--r--   0        0        0     6127 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14312 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      948 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    32118 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/style.md
--rw-r--r--   0        0        0    10870 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     4260 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/patterns/backports.md
--rw-r--r--   0        0        0     7208 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0     3120 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/patterns/exports.md
--rw-r--r--   0        0        0      738 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11217 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4526 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0     4803 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/docs.md
--rw-r--r--   0        0        0     1016 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2582 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3373 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4653 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0     2124 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/helpers/cog_cc.py
--rw-r--r--   0        0        0     1825 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/helpers/cog_helpers.py
--rw-r--r--   0        0        0      699 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/helpers/extensions.py
--rw-r--r--   0        0        0      245 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      419 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0     1479 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      152 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     3434 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     7515 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4736 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     4109 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     6354 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2873 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/readthedocs.py
--rw-r--r--   0        0        0     6534 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/tests/test_cmd.py
--rw-r--r--   0        0        0      861 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/tests/test_package.py
--rw-r--r--   0        0        0      398 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/tests/test_utils.py
--rw-r--r--   0        0        0       79 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/tests/packages/ruff_extend/pyproject.toml
--rw-r--r--   0        0        0       49 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/tests/packages/ruff_extend/ruff.toml
--rw-r--r--   0        0        0      125 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     3333 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.readthedocs.yaml
--rw-r--r--   0        0        0     1689 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0     2972 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0    10426 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     3863 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}
--rw-r--r--   0        0        0      170 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
--rw-r--r--   0        0        0     2264 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
--rw-r--r--   0        0        0      536 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
--rw-r--r--   0        0        0      591 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
--rw-r--r--   0        0        0      727 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
--rw-r--r--   0        0        0      376 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
--rw-r--r--   0        0        0      266 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
--rw-r--r--   0        0        0    11380 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1559 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1089 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}
--rw-r--r--   0        0        0      102 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
--rw-r--r--   0        0        0     2516 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/dependabot.yml
--rwxr-xr-x   0        0        0      978 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
--rw-r--r--   0        0        0      668 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1955 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1138 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}
--rw-r--r--   0        0        0     1722 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}
--rw-r--r--   0        0        0      934 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      218 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0      632 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
--rw-r--r--   0        0        0      562 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
--rw-r--r--   0        0        0      725 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
--rw-r--r--   0        0        0      117 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
--rw-r--r--   0        0        0      171 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.vcs and cookiecutter.backend not in ['whey', 'mesonpy', 'poetry', 'maturin'] %}_version.pyi{% endif %}
--rw-r--r--   0        0        0      223 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0      190 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
--rw-r--r--   0        0        0     2289 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/.gitignore
--rw-r--r--   0        0        0     1525 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/LICENSE
--rw-r--r--   0        0        0     5389 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/pyproject.toml
--rw-r--r--   0        0        0    10588 2024-03-11 02:34:33.000000 sp_repo_review-2024.3.10/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.git_archival.txt
+-rw-r--r--   0        0        0       45 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.gitattributes
+-rw-r--r--   0        0        0     2541 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      267 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      474 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.readthedocs.yaml
+-rw-r--r--   0        0        0        6 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.ruby-version
+-rw-r--r--   0        0        0     1182 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/Gemfile
+-rw-r--r--   0        0        0     3808 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/Gemfile.lock
+-rw-r--r--   0        0        0    19090 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/README.md
+-rw-r--r--   0        0        0     1106 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/_config.yml
+-rw-r--r--   0        0        0      763 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/action.yml
+-rw-r--r--   0        0        0     2062 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/cookiecutter.json
+-rw-r--r--   0        0        0     2806 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/copier.yml
+-rw-r--r--   0        0        0    15205 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/noxfile.py
+-rw-r--r--   0        0        0      527 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      223 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/dependabot.yml
+-rw-r--r--   0        0        0      825 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      726 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2109 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5098 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0     1404 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/LICENSE
+-rw-r--r--   0        0        0      829 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/README.md
+-rw-r--r--   0        0        0     2180 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      671 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0     2777 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_includes/pyproject.md
+-rw-r--r--   0        0        0      145 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_includes/toc.html
+-rw-r--r--   0        0        0      435 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_plugins/details.rb
+-rw-r--r--   0        0        0      512 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_plugins/repo_review.rb
+-rw-r--r--   0        0        0     1541 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_plugins/tabs.rb
+-rw-r--r--   0        0        0       22 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2627 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    11199 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     4158 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/index.md
+-rw-r--r--   0        0        0     5216 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0    13400 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/docs.md
+-rw-r--r--   0        0        0    23941 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     8081 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     7663 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     3202 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/index.md
+-rw-r--r--   0        0        0    10374 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    18538 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9800 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/packaging_compiled.md
+-rw-r--r--   0        0        0     6127 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14312 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      948 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    32120 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/style.md
+-rw-r--r--   0        0        0    12123 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     4260 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/patterns/backports.md
+-rw-r--r--   0        0        0     7208 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0     3120 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/patterns/exports.md
+-rw-r--r--   0        0        0      738 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11217 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     5235 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0     4803 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/docs.md
+-rw-r--r--   0        0        0     1016 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2582 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3373 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4653 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0     2124 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/helpers/cog_cc.py
+-rw-r--r--   0        0        0     1825 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/helpers/cog_helpers.py
+-rw-r--r--   0        0        0      699 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/helpers/extensions.py
+-rw-r--r--   0        0        0      245 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0     1479 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      152 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     3434 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     7515 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4736 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     4109 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     6397 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2873 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/readthedocs.py
+-rw-r--r--   0        0        0     6639 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/test_cmd.py
+-rw-r--r--   0        0        0      861 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/test_package.py
+-rw-r--r--   0        0        0     2296 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/test_pyproject.py
+-rw-r--r--   0        0        0      993 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/test_ruff.py
+-rw-r--r--   0        0        0      398 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/test_utils.py
+-rw-r--r--   0        0        0       79 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/packages/ruff_extend/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/tests/packages/ruff_extend/ruff.toml
+-rw-r--r--   0        0        0      125 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     3334 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.readthedocs.yaml
+-rw-r--r--   0        0        0     1689 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0     3056 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0    10426 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     3863 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}
+-rw-r--r--   0        0        0      170 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
+-rw-r--r--   0        0        0     2264 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
+-rw-r--r--   0        0        0      536 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
+-rw-r--r--   0        0        0      591 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
+-rw-r--r--   0        0        0      727 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      376 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      266 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
+-rw-r--r--   0        0        0    11380 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1559 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1089 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0      102 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
+-rw-r--r--   0        0        0     2516 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      978 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
+-rw-r--r--   0        0        0      668 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2097 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1280 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}
+-rw-r--r--   0        0        0     1864 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}
+-rw-r--r--   0        0        0      934 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      218 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0      625 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
+-rw-r--r--   0        0        0      562 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
+-rw-r--r--   0        0        0      725 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
+-rw-r--r--   0        0        0      117 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
+-rw-r--r--   0        0        0      171 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.vcs and cookiecutter.backend not in ['whey', 'mesonpy', 'poetry', 'maturin'] %}_version.pyi{% endif %}
+-rw-r--r--   0        0        0      223 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0      190 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
+-rw-r--r--   0        0        0     2289 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/.gitignore
+-rw-r--r--   0        0        0     1525 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/LICENSE
+-rw-r--r--   0        0        0     5449 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/pyproject.toml
+-rw-r--r--   0        0        0    10686 2024-04-22 06:34:37.000000 sp_repo_review-2024.4.23/PKG-INFO
```

### Comparing `sp_repo_review-2024.3.10/.pre-commit-config.yaml` & `sp_repo_review-2024.4.23/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "style: pre-commit fixes"
   autoupdate_schedule: "quarterly"
 
 exclude: "^({{cookiecutter\\.project_name}}|hooks/pre_gen_project.py$)"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -25,38 +25,38 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==24.*]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.0"
+    rev: "v0.4.1"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.8.0"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: "(src|tests)"
         args: []
         additional_dependencies:
           - click
           - markdown-it-py
           - pytest
-          - repo-review
+          - repo-review>=0.10.6
           - rich
           - tomli
           - types-PyYAML
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.1.0"
     hooks:
```

### Comparing `sp_repo_review-2024.3.10/Gemfile` & `sp_repo_review-2024.4.23/Gemfile`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/Gemfile.lock` & `sp_repo_review-2024.4.23/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/README.md` & `sp_repo_review-2024.4.23/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/_config.yml` & `sp_repo_review-2024.4.23/_config.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/action.yml` & `sp_repo_review-2024.4.23/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/cookiecutter.json` & `sp_repo_review-2024.4.23/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/copier.yml` & `sp_repo_review-2024.4.23/copier.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/noxfile.py` & `sp_repo_review-2024.4.23/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 import zipfile
 from collections.abc import Callable
 from pathlib import Path
 from typing import Any
 
 import nox
 
-nox.needs_version = ">=2022.1.7"
+nox.needs_version = ">=2024.3.2"
 nox.options.sessions = ["rr_lint", "rr_tests", "rr_pylint", "readme"]
+nox.options.default_venv_backend = "uv|virtualenv"
 
 DIR = Path(__file__).parent.resolve()
 with DIR.joinpath("cookiecutter.json").open() as f:
     BACKENDS = json.load(f)["backend"]
 
 JOB_FILE = """\
 default_context:
```

### Comparing `sp_repo_review-2024.3.10/.devcontainer/devcontainer.json` & `sp_repo_review-2024.4.23/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.github/workflows/bump.yml` & `sp_repo_review-2024.4.23/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.github/workflows/cd.yml` & `sp_repo_review-2024.4.23/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.github/workflows/ci.yml` & `sp_repo_review-2024.4.23/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2024.4.23/.github/workflows/reusable-change-detection.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2024.4.23/.github/workflows/reusable-cookie.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 name: Cookie
 
 on:
   workflow_call:
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
@@ -33,16 +35,21 @@
       - uses: actions/checkout@v4
 
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
 
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-venv: ".venv"
+
       - name: Install nox
-        run: pip install nox
+        run: uv pip install nox
 
       - name: Test setuptools
         run: nox -s 'tests(setuptools, novcs)' -s 'tests(setuptools, vcs)'
 
       - name: Test pybind11
         run: nox -s 'tests(pybind11, novcs)' -s 'tests(pybind11, vcs)'
 
@@ -93,72 +100,85 @@
   nox:
     name: Check included Noxfile
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
 
+      - uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
+
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-venv: ".venv"
+
+      - name: Install nox
+        run: uv pip install nox
+
       - name: Test setuptools
         run: |
-          pipx run nox -s 'nox(setuptools, vcs)'
-          pipx run nox -s 'nox(setuptools, vcs)' -- docs
+          nox -s 'nox(setuptools, vcs)'
+          nox -s 'nox(setuptools, vcs)' -- docs
 
       - name: Test pybind11
         run: |
-          pipx run nox -s 'nox(pybind11, vcs)'
-          pipx run nox -s 'nox(pybind11, vcs)' -- docs
+          nox -s 'nox(pybind11, vcs)'
+          nox -s 'nox(pybind11, vcs)' -- docs
 
       - name: Test scikit-build
         run: |
-          pipx run nox -s 'nox(skbuild, vcs)'
-          pipx run nox -s 'nox(skbuild, vcs)' -- docs
+          nox -s 'nox(skbuild, vcs)'
+          nox -s 'nox(skbuild, vcs)' -- docs
 
       - name: Test poetry
         run: |
-          pipx run nox -s 'nox(poetry, novcs)'
-          pipx run nox -s 'nox(poetry, novcs)' -- docs
+          nox -s 'nox(poetry, novcs)'
+          nox -s 'nox(poetry, novcs)' -- docs
 
       - name: Test flit
         run: |
-          pipx run nox -s 'nox(flit, novcs)'
-          pipx run nox -s 'nox(flit, novcs)' -- docs
+          nox -s 'nox(flit, novcs)'
+          nox -s 'nox(flit, novcs)' -- docs
 
       - name: Test pdm
         run: |
-          pipx run nox -s 'nox(pdm, vcs)'
-          pipx run nox -s 'nox(pdm, vcs)' -- docs
+          nox -s 'nox(pdm, vcs)'
+          nox -s 'nox(pdm, vcs)' -- docs
 
       - name: Test whey
         run: |
-          pipx run nox -s 'nox(whey, novcs)'
-          pipx run nox -s 'nox(whey, novcs)' -- docs
+          nox -s 'nox(whey, novcs)'
+          nox -s 'nox(whey, novcs)' -- docs
 
       - name: Test maturin
         run: |
-          pipx run nox -s 'nox(maturin, novcs)'
-          pipx run nox -s 'nox(maturin, novcs)' -- docs
+          nox -s 'nox(maturin, novcs)'
+          nox -s 'nox(maturin, novcs)' -- docs
 
       - name: Test hatch
         run: |
-          pipx run nox -s 'nox(hatch, vcs)'
-          pipx run nox -s 'nox(hatch, vcs)' -- docs
+          nox -s 'nox(hatch, vcs)'
+          nox -s 'nox(hatch, vcs)' -- docs
 
       - name: Test setuptools PEP 621
         run: |
-          pipx run nox -s 'nox(setuptools621, vcs)'
-          pipx run nox -s 'nox(setuptools621, vcs)' -- docs
+          nox -s 'nox(setuptools621, vcs)'
+          nox -s 'nox(setuptools621, vcs)' -- docs
 
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
 
       - name: Test meson-python
         run: |
-          pipx run nox -s 'nox(mesonpy, novcs)'
-          pipx run nox -s 'nox(mesonpy, novcs)' -- docs
+          nox -s 'nox(mesonpy, novcs)'
+          nox -s 'nox(mesonpy, novcs)' -- docs
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
```

### Comparing `sp_repo_review-2024.3.10/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2024.4.23/.github/workflows/reusable-rr-tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 name: RR
 
 on:
   workflow_call:
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
```

### Comparing `sp_repo_review-2024.3.10/docs/README.md` & `sp_repo_review-2024.4.23/docs/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_includes/head.html` & `sp_repo_review-2024.4.23/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_includes/head_custom.html` & `sp_repo_review-2024.4.23/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_includes/interactive_repo_review.html` & `sp_repo_review-2024.4.23/docs/_includes/interactive_repo_review.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
   );
   root.render(
     <App
       header={false}
       deps={[
         "repo-review~=0.10.0",
         "sp-repo-review==2024.03.10",
-        "validate-pyproject-schema-store==2024.03.11",
+        "validate-pyproject-schema-store==2024.04.20",
         "validate-pyproject[all]~=0.16.0",
       ]}
     />,
   );
 </script>
```

### Comparing `sp_repo_review-2024.3.10/docs/_includes/pyproject.md` & `sp_repo_review-2024.4.23/docs/_includes/pyproject.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_plugins/repo_review.rb` & `sp_repo_review-2024.4.23/docs/_plugins/repo_review.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_plugins/tabs.rb` & `sp_repo_review-2024.4.23/docs/_plugins/tabs.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/_sass/custom/custom.scss` & `sp_repo_review-2024.4.23/docs/_sass/custom/custom.scss`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/assets/favicon.ico` & `sp_repo_review-2024.4.23/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/assets/images/logo.svg` & `sp_repo_review-2024.4.23/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/assets/js/tabs.js` & `sp_repo_review-2024.4.23/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/assets/js/webapp.js` & `sp_repo_review-2024.4.23/docs/assets/js/webapp.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/index.md` & `sp_repo_review-2024.4.23/docs/pages/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/coverage.md` & `sp_repo_review-2024.4.23/docs/pages/guides/coverage.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 uploading coverage reports through your workflow, which should be more than
 enough for a simple testing suite, can be written as follows:
 
 {% raw %}
 
 ```yaml
 - name: Upload coverage report
-  uses: codecov/codecov-action@v4.1.0
+  uses: codecov/codecov-action@v4.3.0
   with:
     token: ${{ secrets.CODECOV_TOKEN }}
 ```
 
 {% endraw %}
 
 The lines above should be added after the step that runs your tests with the
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/docs.md` & `sp_repo_review-2024.4.23/docs/pages/guides/docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/gha_basic.md` & `sp_repo_review-2024.4.23/docs/pages/guides/gha_basic.md`

 * *Files 2% similar despite different names*

```diff
@@ -257,29 +257,40 @@
   Setup any version of CMake on almost any image.
 - [wntrblm/nox](https://github.com/wntrblm/nox): Setup all versions of Python
   and provide nox.
 - [pre-commit/action](https://github.com/pre-commit/action): Run pre-commit with
   built-in caching.
 - [conda-incubator/setup-miniconda](https://github.com/conda-incubator/setup-miniconda):
   Setup conda or mamba on GitHub Actions.
+- [prefix-dev/setup-pixi](https://github.com/prefix-dev/setup-pixi): Set up pixi
+  and install your environment(s). Try `cache: false` if saving/loading the
+  cache is slow.
 - [ruby/setup-ruby](https://github.com/ruby/setup-ruby): Setup Ruby if you need
   it for something.
 - [peter-evans/create-pull-request](https://github.com/peter-evans/create-pull-request):
   Make a new PR with the current changes (more options than just using `gh`).
   You can even auto-merge PRs with `run: gh pr merge --merge --auto "1"`
   afterwards.
+- [yezz123/setup-uv](https://github.com/yezz123/setup-uv): Set up `uv`. Has a
+  handy `uv-venv` option that will also set up and activate a virtual
+  environment for you.
+- [gautamkrishnar/keepalive-workflow](https://github.com/gautamkrishnar/keepalive-workflow):
+  Keep GitHub actions alive for more than 60 days. Not usually needed if you've
+  set up the other suggestions here, like dependabot and pre-commit.
 
 A couple more from Python developers; note these do not provide `vX` moving tags
 like the official actions and most other actions, but instead have `release/vX`
 branches that you can use.
 
 - [pypa/gh-action-pypi-publish](https://github.com/pypa/gh-action-pypi-publish):
   Publish Python packages to PyPI. Supports trusted publisher deployment.
 - [re-actors/alls-green](https://github.com/re-actors/alls-green): Tooling to
   check to see if all jobs passed (supports allowed failures, too).
+- [sigstore/gh-action-sigstore-python](https://github.com/sigstore/gh-action-sigstore-python):
+  Signing files in GitHub Actions with sigstore.
 
 There are also a few useful tools installed which can really simplify your
 workflow or adding custom actions. This includes system package managers (like
 brew, chocolaty, NuGet, Vcpkg, etc), as well as a fantastic cross platform one:
 
 - [pipx](https://github.com/pypa/pipx): This is pre-installed on all runners
   (GitHub uses to set up other things), and is kept up to date. It enables you
@@ -641,15 +652,15 @@
 
 Now you'll want three custom actions in your `steps:`. First, you need to
 configure Pages.
 
 ```yaml
 - name: Setup Pages
   id: pages
-  uses: actions/configure-pages@v4
+  uses: actions/configure-pages@v5
 ```
 
 {% raw %}
 
 Notice this action sets an `id:`; this will allow you to use the outputs from
 this action later; specifically, may want to use
 `${{ steps.pages.outputs.base_path }}` when building (you can also get `origin`,
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/gha_pure.md` & `sp_repo_review-2024.4.23/docs/pages/guides/gha_pure.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2024.4.23/docs/pages/guides/gha_wheels.md`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
   steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.16
+    - uses: pypa/cibuildwheel@v2.17
 
     - name: Upload wheels
       uses: actions/upload-artifact@v4
       with:
         name: cibw-wheels-${{ matrix.os }}
         path: wheelhouse/*.whl
 ```
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/index.md` & `sp_repo_review-2024.4.23/docs/pages/guides/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/mypy.md` & `sp_repo_review-2024.4.23/docs/pages/guides/mypy.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2024.4.23/docs/pages/guides/packaging_classic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/packaging_compiled.md` & `sp_repo_review-2024.4.23/docs/pages/guides/packaging_compiled.md`

 * *Files 2% similar despite different names*

```diff
@@ -221,16 +221,15 @@
   )pbdoc";
 
   m.def("add", &add, R"pbdoc(
       Add two numbers
       Some other explanation about the add function.
   )pbdoc");
 
-  m.def(
-      "subtract", [](int i, int j) { return i - j; }, R"pbdoc(
+  m.def("subtract", [](int i, int j) { return i - j; }, R"pbdoc(
       Subtract two numbers
       Some other explanation about the subtract function.
   )pbdoc");
 }
 ```
 <!-- prettier-ignore-end -->
 <!-- [[[end]]] -->
@@ -263,16 +262,15 @@
   )pbdoc";
 
   m.def("add", &add, R"pbdoc(
       Add two numbers
       Some other explanation about the add function.
   )pbdoc");
 
-  m.def(
-      "subtract", [](int i, int j) { return i - j; }, R"pbdoc(
+  m.def("subtract", [](int i, int j) { return i - j; }, R"pbdoc(
       Subtract two numbers
       Some other explanation about the subtract function.
   )pbdoc");
 }
 ```
 <!-- prettier-ignore-end -->
 <!-- [[[end]]] -->
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2024.4.23/docs/pages/guides/packaging_simple.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/pytest.md` & `sp_repo_review-2024.4.23/docs/pages/guides/pytest.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/repo_review.md` & `sp_repo_review-2024.4.23/docs/pages/guides/repo_review.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/style.md` & `sp_repo_review-2024.4.23/docs/pages/guides/style.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 {% rr PC100 %} Here is a minimal `.pre-commit-config.yaml` file with some handy
 options:
 
 ```yaml
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -107,15 +107,15 @@
 Ruff, the powerful Rust-based linter, has a formatter that is designed with the
 help of some of the Black authors to look 99.9% like Black, but run 30x faster.
 Here is the snippet to add the formatter to your `.pre-commit-config.yml`
 (combine with the Ruff linter below):
 
 ```yaml
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.3.0"
+  rev: "v0.4.1"
   hooks:
     #  id: ruff would go here if using both
     - id: ruff-format
 ```
 
 As you likely will be using Ruff if you follow this guide, the formatter is
 recommended as well.
@@ -137,15 +137,15 @@
 
 {% endtab %} {% tab black Black %}
 
 Here is the snippet to add Black to your `.pre-commit-config.yml`:
 
 ```yaml
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: "24.2.0"
+  rev: "24.4.0"
   hooks:
     - id: black
 ```
 
 {% details You can add a Black badge to your repo as well %}
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -197,15 +197,15 @@
 pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
 [ruff]: https://github.com/astral-sh/ruff
 
 ```yaml
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.3.0"
+  rev: "v0.4.1"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
 {% rr PC191 %} The `--fix` argument is optional, but recommended, since you can
 inspect and undo changes in git.
@@ -486,15 +486,15 @@
 style syntax. Most useful to keep Python 2 outdated constructs out, it can even
 do some code updates for different versions of Python 3, like adding f-strings
 when clearly better (please always use them, they are faster) if you set
 `--py36-plus` (for example). This is a recommended addition for any project.
 
 ```yaml
 - repo: https://github.com/asottile/pyupgrade
-  rev: "v3.15.1"
+  rev: "v3.15.2"
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 ```
 
 [pyupgrade]: https://github.com/asottile/pyupgrade
 
@@ -531,15 +531,15 @@
 
 Read more about type checking on the [dedicated page][mypy page].
 
 The MyPy addition for pre-commit:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v1.8.0"
+  rev: "v1.9.0"
   hooks:
     - id: mypy
       files: src
       args: []
 ```
 
 You should always specify args, as the hook's default hides issues - it's
@@ -578,15 +578,15 @@
 `# mypy: <option>` at the top of a file. You can also pass `--strict` on the
 command line. `strict = true` is now allowed in config files, too
 {% rr MY101 %}.
 
 The extra strict options shown above, like `warn_unreachable` {% rr MY103 %},
 and `ignore-without-code` {% rr MY104 %}, `redundant-expr` {% rr MY105 %}, and
 `truthy-bool` {% rr MY106 %} can trigger too often (like on `sys.platform`
-checks) and have to be ignored occasionally, but can find some signifiant logic
+checks) and have to be ignored occasionally, but can find some significant logic
 errors in your typing.
 
 [mypy page]: {% link pages/guides/mypy.md %}
 
 ## Setuptools specific checks
 
 If you use setuptools, these checks are useful:
@@ -743,15 +743,15 @@
 ## Clang-format (C++ only)
 
 If you have C++ code, you should have a `.clang-format` file and use the
 following pre-commit config:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-clang-format
-  rev: "v17.0.6"
+  rev: "v18.1.4"
   hooks:
     - id: clang-format
       types_or: [c++, c, cuda]
 ```
 
 This will use 1-2 MB binary wheels from PyPI on all common platforms. You can
 generated such a file using
@@ -760,15 +760,15 @@
 ## Shellcheck (shell scripts only)
 
 If you have shell scripts, you can protect against common mistakes using
 [shellcheck](https://github.com/koalaman/shellcheck).
 
 ```yaml
 - repo: https://github.com/shellcheck-py/shellcheck-py
-  rev: "v0.9.0.6"
+  rev: "v0.10.0.1"
   hooks:
     - id: shellcheck
 ```
 
 ## Prettier
 
 {% rr PC180 %} The [prettier](https://prettier.io) tool can format a large
@@ -820,15 +820,15 @@
 supports a variety of common files built-in ([see the docs][cjs-common]) like
 various CI configuration files. You can also write/provide your own schemas and
 validate using those - [SchemaStore][] provides a few hundred different common
 schemas, and you can load them via URL. It work on JSON, YAML, and TOML.
 
 ```yaml
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: "0.28.0"
+  rev: "0.28.2"
   hooks:
     - id: check-dependabot
     - id: check-github-workflows
     - id: check-readthedocs
 ```
 
 ## PyLint (noisy)
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/guides/tasks.md` & `sp_repo_review-2024.4.23/docs/pages/guides/tasks.md`

 * *Files 13% similar despite different names*

```diff
@@ -71,24 +71,24 @@
 `nox`.
 
 On GitHub Actions or Azure, pipx is available by default, so you should use
 `pipx run nox`. To give it access to all Python versions, you can use this
 action:
 
 ```yaml
-- uses: wntrblm/nox@2024.03.02
+- uses: wntrblm/nox@2024.04.15
 ```
 
 You can now access all current versions of Python from nox. At least in GitHub
 Actions, you should add `--forcecolor` to your nox runs to get color output in
-your logs, or set `env: FORCE_COLOR: 3`. If you'd like to customise the versions
-of Python prepared for you, then use input like this:
+your logs, or set `env: FORCE_COLOR: 3`[^force_color]. If you'd like to
+customize the versions of Python prepared for you, then use input like this:
 
 ```yaml
-- uses: wntrblm/nox@2024.03.02
+- uses: wntrblm/nox@2024.04.15
   with:
     python-versions: "3.8, 3.9, 3.10, 3.11, 3.12, pypy-3.9, pypy-3.10"
 ```
 
 ### Introduction
 
 Nox is a tool for running tasks, called "sessions", inside temporary virtual
@@ -310,14 +310,44 @@
 
     session.install("build")
     session.run("python", "-m", "build")
 ```
 <!-- prettier-ignore-end -->
 <!-- [[[end]]] -->
 
+(Removing the build directory is helpful for setuptools)
+
+### Faster with uv
+
+The [uv](https://github.com/astral-sh/uv) project is a Rust reimplementation of
+pip, pip-tools, and venv that is very, very fast. You can tell nox to use `uv`
+if it is on your system by adding the following to your `noxfile.py`:
+
+```python
+nox.needs_version = ">=2024.3.2"
+nox.options.default_venv_backend = "uv|virtualenv"
+```
+
+You can install `uv` with `pipx`, `brew`, etc. If you want to use uv in GitHub
+Actions, one way is to use this:
+
+```yaml
+- name: Setup uv
+  uses: yezz123/setup-uv@v4
+```
+
+You do not need to set `with: uv-venv: ".venv"` for `nox` to be able to use
+`uv`.
+
+Check your jobs with `uv`; most things do not need to change. The main
+difference is `uv` doesn't install `pip` unless you ask it to. If you want to
+interact with uv, nox might be getting uv from it's environment instead of the
+system environment, so you can install `uv` if `shutil.which("uv")` returns
+`None`.
+
 ### Examples
 
 A standard
 [powered by nox](https://github.com/scikit-hep/hist/blob/main/noxfile.py)
 package in Pure Python can be found in the Hist project of Scikit-HEP.
 
 A package that happens to use PDM (like Poetry but better) is Scikit-HEP UHI,
@@ -337,7 +367,13 @@
 as providing a standard interface to update Python and project listing update
 scripts. The docs job there runs mkdocs instead of Sphinx. Other PyPA projects
 using nox include [pip](https://github.com/pypa/pip/blob/main/noxfile.py),
 [pipx](https://github.com/pypa/pipx/blob/main/noxfile.py),
 [manylinux](https://github.com/pypa/manylinux/blob/main/noxfile.py),
 [packaging](https://github.com/pypa/packaging/blob/main/noxfile.py), and
 [packaging.python.org](https://github.com/pypa/packaging.python.org/blob/main/noxfile.py).
+
+[^force_color]:
+    Many color libraries just need `FORCE_COLOR` to be set to any value, but at
+    least [one](https://pypi.org/project/plumbum/) distinguishes color depth,
+    where "3" -> "256-bit color". For many use cases, using `FORCE_COLOR: 1` is
+    fine.
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/patterns/backports.md` & `sp_repo_review-2024.4.23/docs/pages/patterns/backports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/patterns/data_files.md` & `sp_repo_review-2024.4.23/docs/pages/patterns/data_files.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/patterns/exports.md` & `sp_repo_review-2024.4.23/docs/pages/patterns/exports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/patterns/index.md` & `sp_repo_review-2024.4.23/docs/pages/patterns/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/principles/design.md` & `sp_repo_review-2024.4.23/docs/pages/principles/design.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/principles/index.md` & `sp_repo_review-2024.4.23/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/principles/process.md` & `sp_repo_review-2024.4.23/docs/pages/principles/process.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/dev-environment.md`

 * *Files 15% similar despite different names*

```diff
@@ -83,14 +83,24 @@
 {: .highlight-title }
 
 > For Advanced Users Using Custom Shells
 >
 > If you like a different shell, like fish, there are several `activate`
 > scripts; the default one expects a bash-like shell.
 
+{: .note-title }
+
+> Fast alternative
+>
+> You can also consider the [uv][] package, which is much, much faster version
+> of pip and venv implemented in Rust. Just put `uv` in front of the commands
+> you'd normally use; as long as you use venvs, it should be nearly the same.
+
+[uv]: https://github.com/astral-sh/uv
+
 ### Option 2: Using conda
 
 You can also develop in conda. This is an especially good option if:
 
 - You want an easy way to choose a specific version of Python
 - Your project will depend on complex software libraries that are not readily
   pip-installable
@@ -109,14 +119,24 @@
 
 ```bash
 conda activate env_name
 ```
 
 To deactivate, use `conda deactivate`, or leave your shell.
 
+> Modern faster alternative
+>
+> You can also consider the [pixi][] package, which is much, much faster version
+> of conda implemented in Rust. It has been completely redesigned to work around
+> projects with a `pixi.toml` file instead of global environments. It's a new
+> way to work (more similar to pdm/hatch/poetry from Python), but very powerful
+> if you learn it.
+
+[pixi]: https://pixi.sh
+
 ## Choosing an Editor
 
 Any plain text editor will serve our purposes for this guide. Bare bones editors
 like Notepad or `nano` will do the job. More feature-rich Integrated Development
 Environments (IDEs) such as [PyCharm][] or [Visual Studio Code][] can provide
 useful additions, such as syntax highlighting, tab completion, and more. Classic
 text editors like [`vim`][] and [`emacs`][] can do the same with configuration,
```

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/docs.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/index.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/module.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/module.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/packaging.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/packaging.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/docs/pages/tutorials/test.md` & `sp_repo_review-2024.4.23/docs/pages/tutorials/test.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/helpers/cog_cc.py` & `sp_repo_review-2024.4.23/helpers/cog_cc.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/helpers/cog_helpers.py` & `sp_repo_review-2024.4.23/helpers/cog_helpers.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/helpers/extensions.py` & `sp_repo_review-2024.4.23/helpers/extensions.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/families.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/families.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/general.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/github.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,18 @@
 
         ```toml
         [tool.pytest.ini_options]
         minversion = "7"
         ```
         """
         options = pyproject["tool"]["pytest"]["ini_options"]
-        return "minversion" in options and int(options["minversion"].split(".")[0]) >= 6
+        return (
+            "minversion" in options
+            and int(str(options["minversion"]).split(".")[0]) >= 6
+        )
 
 
 class PP303(PyProject):
     "Sets the test paths"
 
     requires = {"PP301"}
     url = mk_url("pytest")
@@ -185,15 +188,15 @@
     def check(pyproject: dict[str, Any]) -> bool:
         """
         `--strict-markers` should be in `addopts = [...]`. This forces all
         markers to be specified in config, avoiding misspellings.
 
         ```toml
         [tool.pytest.ini_options]
-        addops = ["-ra", "--strict-config", "--strict-markers"]
+        addopts = ["-ra", "--strict-config", "--strict-markers"]
         ```
         """
         options = pyproject["tool"]["pytest"]["ini_options"]
         return "--strict-markers" in options.get("addopts", [])
 
 
 class PP308(PyProject):
@@ -206,15 +209,15 @@
     def check(pyproject: dict[str, Any]) -> bool:
         """
         An explicit summary flag like `-ra` should be in `addopts = [...]`
         (print summary of all fails/errors).
 
         ```toml
         [tool.pytest.ini_options]
-        addops = ["-ra", "--strict-config", "--strict-markers"]
+        addopts = ["-ra", "--strict-config", "--strict-markers"]
         ```
         """
         options = pyproject["tool"]["pytest"]["ini_options"]
         return any(opt.startswith("-r") for opt in options.get("addopts", []))
 
 
 class PP309(PyProject):
```

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/readthedocs.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/readthedocs.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2024.4.23/src/sp_repo_review/checks/ruff.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,20 @@
     def check(pyproject: dict[str, Any], ruff: dict[str, Any]) -> bool | str:
         """
         Must select a minimum version to target. Affects pyupgrade, isort, and
         others. Will be inferred from `project.requires-python`.
         """
 
         match pyproject:
+            case {
+                "project": {"requires-python": str()},
+                "tool": {"ruff": {"target-version": object()}},
+            }:
+                return "You have both Ruff's `target-version` and `project.requires-python`. You only need the latter."
             case {"project": {"requires-python": str()}}:
-                if "target-version" in ruff:
-                    return "You have both Ruff's `target-version` and `project.requires-python`. You only need the later."
                 return True
             case _:
                 return "target-version" in ruff
 
 
 class RF003(Ruff):
     "src directory specified if used"
```

### Comparing `sp_repo_review-2024.3.10/tests/test_package.py` & `sp_repo_review-2024.4.23/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==24.*]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -36,15 +36,15 @@
     rev: "v3.1.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.0"
+    rev: "v0.4.1"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
 {%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
 
@@ -55,37 +55,37 @@
         args: [--include-version-classifiers, --max-py-version=3.12]
 
 {%- endif %}
 
 {%- if cookiecutter.backend in ["pybind11", "skbuild", "mesonpy"] %}
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: "v17.0.6"
+    rev: "v18.1.4"
     hooks:
       - id: clang-format
         types_or: [c++, c, cuda]
 
 {%- endif %}
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.8.0"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: src|tests
         args: []
         additional_dependencies:
           - pytest
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
@@ -114,15 +114,15 @@
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: "v0.16"
     hooks:
       - id: validate-pyproject
         additional_dependencies: ["validate-pyproject-schema-store[all]"]
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: "0.28.0"
+    rev: "0.28.2"
     hooks:
 {%- if cookiecutter.__ci == "github" %}
       - id: check-dependabot
       - id: check-github-workflows
 {%- elif cookiecutter.__ci == "gitlab" %}
       - id: check-gitlab-ci
 {%- endif %}
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import nox
 
 {% if cookiecutter.backend != "pybind11" -%}
 DIR = Path(__file__).parent.resolve()
 
 {% endif -%}
 
+nox.needs_version = ">=2024.3.2"
 nox.options.sessions = ["lint", "pylint", "tests"]
+nox.options.default_venv_backend = "uv|virtualenv"
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
       - main
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
@@ -70,10 +72,10 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.0
         with:
           token: {% raw %}${{ secrets.CODECOV_TOKEN }}{% endraw %}
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
       - published
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
       - published
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   make_sdist:
     name: Make SDist
     runs-on: ubuntu-latest
     steps:
@@ -39,15 +41,15 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: pypa/cibuildwheel@v2.16
+      - uses: pypa/cibuildwheel@v2.17
 
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-{% raw %}${{ matrix.os }}-${{ strategy.job-index }}{% endraw %}
           path: wheelhouse/*.whl
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/docs/conf.py` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}`

 * *Files 18% similar despite different names*

```diff
@@ -16,13 +16,12 @@
   )pbdoc";
 
   m.def("add", &add, R"pbdoc(
       Add two numbers
       Some other explanation about the add function.
   )pbdoc");
 
-  m.def(
-      "subtract", [](int i, int j) { return i - j; }, R"pbdoc(
+  m.def("subtract", [](int i, int j) { return i - j; }, R"pbdoc(
       Subtract two numbers
       Some other explanation about the subtract function.
   )pbdoc");
 }
```

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py` & `sp_repo_review-2024.4.23/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/.gitignore` & `sp_repo_review-2024.4.23/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/LICENSE` & `sp_repo_review-2024.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2024.3.10/pyproject.toml` & `sp_repo_review-2024.4.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,24 @@
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed",
 ]
 dynamic = ["version", "readme"]
 dependencies = [
   "pyyaml",
   "repo-review",
+  "tomli; python_version<'3.11'",
 ]
 
 [project.optional-dependencies]
 cli = [
   "repo-review[cli]",
 ]
 test = [
   "pytest >=7",
+  "repo-review >=0.10.6",
 ]
 dev = [
   "pytest >=7",
 ]
 pyproject = [
   "validate-pyproject-schema-store[all]",
 ]
```

### Comparing `sp_repo_review-2024.3.10/PKG-INFO` & `sp_repo_review-2024.4.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sp_repo_review
-Version: 2024.3.10
+Version: 2024.4.23
 Summary: Review repos for compliance to the Scientific-Python development guidelines
 Project-URL: Guide, https://learn.scientific-python.org/development
 Project-URL: Homepage, https://github.com/scientific-python/cookie
 Project-URL: Preview, https://scientific-python-cookie.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/cookie
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
@@ -23,22 +23,24 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: pyyaml
 Requires-Dist: repo-review
+Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: cli
 Requires-Dist: repo-review[cli]; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: pytest>=7; extra == 'dev'
 Provides-Extra: pyproject
 Requires-Dist: validate-pyproject-schema-store[all]; extra == 'pyproject'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
+Requires-Dist: repo-review>=0.10.6; extra == 'test'
 Description-Content-Type: text/markdown
 
 
 
 `sp-repo-review` provides checks based on the [Scientific-Python Development
 Guide][] at [scientific-python/cookie][] for [repo-review][].
```

