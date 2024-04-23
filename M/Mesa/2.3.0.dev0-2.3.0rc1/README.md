# Comparing `tmp/mesa-2.3.0.dev0.tar.gz` & `tmp/mesa-2.3.0rc1.tar.gz`

## Comparing `mesa-2.3.0.dev0.tar` & `mesa-2.3.0rc1.tar`

### file list

```diff
@@ -1,126 +1,140 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.codespellignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.coveragerc
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.readthedocs.yml
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/CITATION.bib
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/Dockerfile
--rw-r--r--   0        0        0    54682 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/HISTORY.md
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/codecov.yaml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docker-compose.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mypy.ini
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/dependabot.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/release.yml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/ISSUE_TEMPLATE/asking-help.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/workflows/build_lint.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/compare_timings.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/configurations.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/global_benchmark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/Flocking/__init__.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/Flocking/flocking.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/Schelling/__init__.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/Schelling/schelling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/WolfSheep/__init__.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/benchmarks/WolfSheep/wolf_sheep.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/Makefile
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/README.md
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/best-practices.md
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/conf.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/howto.md
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/index.md
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/make.bat
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/mesa.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/mesa.visualization.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/mesa.visualization.modules.md
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/modular-visualization.md
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/overview.md
--rw-r--r--   0        0        0    10924 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/packages.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/api_main.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/batchrunner.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/datacollection.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/init.md
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/space.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/time.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/apis/visualization.md
--rw-r--r--   0        0        0    72557 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/Mesa_Screenshot.png
--rw-r--r--   0        0        0    25726 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/mesa_logo.ico
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/mesa_logo.png
--rw-r--r--   0        0        0   162931 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/br_ginis.png
--rw-r--r--   0        0        0   105856 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/dc_endwealth.png
--rw-r--r--   0        0        0    77022 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/dc_gini.png
--rw-r--r--   0        0        0    82335 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/dc_oneagent.png
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/first_hist.png
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/multirun_hist.png
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/numpy_grid.png
--rw-r--r--   0        0        0   181755 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/viz_chart.png
--rw-r--r--   0        0        0   120132 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/viz_empty.png
--rw-r--r--   0        0        0   146952 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/viz_greycircles.png
--rw-r--r--   0        0        0    41024 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/viz_histogram.png
--rw-r--r--   0        0        0   143683 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/images/tutorial/viz_redcircles.png
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/MoneyModel.py
--rw-r--r--   0        0        0    26121 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/adv_tutorial_legacy.ipynb
--rw-r--r--   0        0        0    63607 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/intro_tutorial.ipynb
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/visualization_tutorial.ipynb
--rw-r--r--   0        0        0    95322 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_chart.png
--rw-r--r--   0        0        0   120132 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_empty.png
--rw-r--r--   0        0        0    76400 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_greycircles.png
--rw-r--r--   0        0        0    41024 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_histogram.png
--rw-r--r--   0        0        0    88661 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_redcircles.png
--rw-r--r--   0        0        0    89934 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/docs/tutorials/files/viz_slider.png
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/__init__.py
--rw-r--r--   0        0        0    13794 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/agent.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/batchrunner.py
--rw-r--r--   0        0        0    11194 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/datacollection.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/main.py
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/model.py
--rw-r--r--   0        0        0    61935 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/space.py
--rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/time.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/cookiecutter.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/hooks/post_gen_project.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/README.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/run.pytemplate
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/setup.pytemplate
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/__init__.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.pytemplate
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.pytemplate
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/experimental/UserParam.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/experimental/__init__.py
--rw-r--r--   0        0        0    13007 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/experimental/jupyter_viz.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/experimental/components/altair.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/experimental/components/matplotlib.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/flat/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/flat/visualization.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/visualization/ModularVisualization.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/visualization/TextVisualization.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/visualization/UserParam.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/visualization/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/mesa/visualization/modules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/read_requirements.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_agent.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_batch_run.py
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_datacollector.py
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_end_to_end_viz.sh
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_examples.py
--rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_grid.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_import_namespace.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_jupyter_viz.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_lifespan.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_main.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_model.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_scaffold.py
--rw-r--r--   0        0        0    38359 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_space.py
--rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_time.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_tornado.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_usersettableparam.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/tests/test_visualization.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/.gitignore
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/LICENSE
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/README.md
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 mesa-2.3.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.codespellignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.coveragerc
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.readthedocs.yml
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/CITATION.bib
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/Dockerfile
+-rw-r--r--   0        0        0    64264 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/HISTORY.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/codecov.yaml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docker-compose.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mypy.ini
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/release.yml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/ISSUE_TEMPLATE/asking-help.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/workflows/build_lint.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/compare_timings.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/configurations.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/global_benchmark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/Flocking/__init__.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/Flocking/flocking.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/Schelling/__init__.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/Schelling/schelling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/WolfSheep/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/benchmarks/WolfSheep/wolf_sheep.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/Makefile
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/README.md
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/best-practices.md
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/conf.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/howto.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/index.md
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/make.bat
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/mesa.md
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/mesa.visualization.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/mesa.visualization.modules.md
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/modular-visualization.md
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/overview.md
+-rw-r--r--   0        0        0    10924 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/packages.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/api_main.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/batchrunner.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/datacollection.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/init.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/space.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/time.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/apis/visualization.md
+-rw-r--r--   0        0        0    72557 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/Mesa_Screenshot.png
+-rw-r--r--   0        0        0    25726 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/mesa_logo.ico
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/mesa_logo.png
+-rw-r--r--   0        0        0   162931 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/br_ginis.png
+-rw-r--r--   0        0        0   105856 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/dc_endwealth.png
+-rw-r--r--   0        0        0    77022 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/dc_gini.png
+-rw-r--r--   0        0        0    82335 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/dc_oneagent.png
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/first_hist.png
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/multirun_hist.png
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/numpy_grid.png
+-rw-r--r--   0        0        0   181755 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/viz_chart.png
+-rw-r--r--   0        0        0   120132 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/viz_empty.png
+-rw-r--r--   0        0        0   146952 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/viz_greycircles.png
+-rw-r--r--   0        0        0    41024 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/viz_histogram.png
+-rw-r--r--   0        0        0   143683 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/images/tutorial/viz_redcircles.png
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/MoneyModel.py
+-rw-r--r--   0        0        0    26121 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/adv_tutorial_legacy.ipynb
+-rw-r--r--   0        0        0    63611 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/intro_tutorial.ipynb
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/visualization_tutorial.ipynb
+-rw-r--r--   0        0        0    95322 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_chart.png
+-rw-r--r--   0        0        0   120132 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_empty.png
+-rw-r--r--   0        0        0    76400 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_greycircles.png
+-rw-r--r--   0        0        0    41024 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_histogram.png
+-rw-r--r--   0        0        0    88661 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_redcircles.png
+-rw-r--r--   0        0        0    89934 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/docs/tutorials/files/viz_slider.png
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/__init__.py
+-rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/agent.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/batchrunner.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/datacollection.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/main.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/model.py
+-rw-r--r--   0        0        0    62429 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/space.py
+-rw-r--r--   0        0        0    15243 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/time.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/cookiecutter.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/hooks/post_gen_project.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/README.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/run.pytemplate
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/setup.pytemplate
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/__init__.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.pytemplate
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.pytemplate
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/UserParam.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/__init__.py
+-rw-r--r--   0        0        0    13444 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/jupyter_viz.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/__init__.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/cell.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/cell_agent.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/cell_collection.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/discrete_space.py
+-rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/grid.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/cell_space/network.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/components/altair.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/components/matplotlib.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/devs/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/devs/eventlist.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/devs/simulator.py
+-rw-r--r--   0        0        0     9667 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/devs/examples/epstein_civil_violence.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/experimental/devs/examples/wolf_sheep.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/flat/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/flat/visualization.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/visualization/ModularVisualization.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/visualization/TextVisualization.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/visualization/UserParam.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/visualization/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/mesa/visualization/modules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/read_requirements.py
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_agent.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_batch_run.py
+-rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_cell_space.py
+-rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_datacollector.py
+-rw-r--r--   0        0        0     7041 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_devs.py
+-rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_end_to_end_viz.sh
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_examples.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_grid.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_import_namespace.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_jupyter_viz.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_lifespan.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_main.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_model.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_scaffold.py
+-rw-r--r--   0        0        0    38151 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_space.py
+-rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_time.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_tornado.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_usersettableparam.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/tests/test_visualization.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/.gitignore
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/LICENSE
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/README.md
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 mesa-2.3.0rc1/PKG-INFO
```

### Comparing `mesa-2.3.0.dev0/.pre-commit-config.yaml` & `mesa-2.3.0rc1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ci:
     autoupdate_schedule: 'monthly'
 
 repos:
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.2.0
+  rev: v0.3.5
   hooks:
     # Run the linter.
     - id: ruff
       types_or: [ python, pyi, jupyter ]
       args: [ --fix ]
     # Run the formatter.
     - id: ruff-format
       types_or: [ python, pyi, jupyter ]
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0  # Use the ref you want to point at
     hooks:
     -   id: trailing-whitespace
```

### Comparing `mesa-2.3.0.dev0/.readthedocs.yml` & `mesa-2.3.0rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/CITATION.bib` & `mesa-2.3.0rc1/CITATION.bib`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/CONTRIBUTING.md` & `mesa-2.3.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/Dockerfile` & `mesa-2.3.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/HISTORY.md` & `mesa-2.3.0rc1/HISTORY.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,125 @@
 ---
 title: Release History
 ---
+# 2.3.0-rc1 (2024-04-18)
+## Highlights
+The 2.3.0-rc1 release is our first release candidate pre-release, meant to test all the new features and enhancement for the upcoming 2.3.0 release.
+
+There are two main new features:
+- The experimental cell-centric discrete spaces, as added in #1994. It allows having cells with not only properties but also active behaviors: the `CellAgent`. Its inspired by NetLogo's [patches](https://ccl.northwestern.edu/netlogo/bind/primitive/patches.html) but extend and generalize this concept further.
+- Full support for discrete event scheduling, as added in #2066. It allows scheduling events (like Agent actions) at any time, including non-integer timesteps.
+
+There are a lot of other features: The Jupyter visualisation now supports easier way to specify sliders, `NetworkGrid.get_neighbors()` supports a radius, `AgentSet.get()` can retrieve multiple attributes and there are now benchmarks to track Mesa performance during development.
+
+Finally, 2.3.0 stabilizes the `AgentSet` (including `model.agents`), making it the first experimental Mesa feature that is taken out of it's experimental phase.
+
+Install this pre-release with:
+```
+pip install --pre mesa
+```
+We would love feedback before we release 2.3.0 stable in ~1 week.
+
+## What's Changed
+### 🧪 Experimental features
+* Add cell-centric discrete spaces (experimental) by @Corvince in https://github.com/projectmesa/mesa/pull/1994
+### 🎉 New features added
+* Add performance benchmarking scripts by @EwoutH in https://github.com/projectmesa/mesa/pull/1979
+* feat: Implement Slider class for JupyterViz by @rht in https://github.com/projectmesa/mesa/pull/1972
+* Stabilize AgentSet by @EwoutH in https://github.com/projectmesa/mesa/pull/2065
+* Support discrete event scheduling by @quaquel in https://github.com/projectmesa/mesa/pull/2066
+### 🛠 Enhancements made
+* JupyterViz: Automatically deduce display name from model class by @rht in https://github.com/projectmesa/mesa/pull/1975
+* Add radius argument to NetworkGrid.get_neighbors() by @EwoutH in https://github.com/projectmesa/mesa/pull/1973
+* Speedup of Agentset.shuffle by @quaquel in https://github.com/projectmesa/mesa/pull/2010
+* feat: Let mesa runserver detect server.py as fallback by @rht in https://github.com/projectmesa/mesa/pull/2015
+* JupyterViz: {Convert make_plot & prepare ColorCard} to become Solara component by @rht in https://github.com/projectmesa/mesa/pull/2020
+* new feature: AgentSet.get can retrieve one or more then one attribute by @quaquel in https://github.com/projectmesa/mesa/pull/2044
+* Update CODE_OF_CONDUCT.md to version 2+ of contrib convenant by @jackiekazil in https://github.com/projectmesa/mesa/pull/2052
+* Improve flocking benchmark  by @coderbeta1 in https://github.com/projectmesa/mesa/pull/2054
+* Remove JupyterViz Altair marker overlap for huge grid size by @rht in https://github.com/projectmesa/mesa/pull/2062
+* Add tooltip option to Altair chart by @FoFFolo in https://github.com/projectmesa/mesa/pull/2082
+* feat: Display model seed & allow user to specify it in JupyterViz by @rht in https://github.com/projectmesa/mesa/pull/2069
+* warn if placing already placed agent by @puer-robustus in https://github.com/projectmesa/mesa/pull/2083
+### 🐛 Bugs fixed
+* fix: Apply default value to slider by @rht in https://github.com/projectmesa/mesa/pull/2016
+* fix: Initialize model _steps and _time during __new__ by @rht in https://github.com/projectmesa/mesa/pull/2026
+* fix: Use model.schedule only when it is not None by @rht in https://github.com/projectmesa/mesa/pull/2050
+* fix: Remove JupyterViz grid marker overlap for huge grid size by @rht in https://github.com/projectmesa/mesa/pull/2049
+### 📜 Documentation improvements
+* Improve readability of badges by @rht in https://github.com/projectmesa/mesa/pull/2009
+* More pythonic implementation of wolf sheep by @quaquel in https://github.com/projectmesa/mesa/pull/2011
+* Adding super().__init__() to MoneyModel tutorial by @sw23 in https://github.com/projectmesa/mesa/pull/2025
+* docs: Convert howto.rst -> howto.md via rst2myst by @rht in https://github.com/projectmesa/mesa/pull/2033
+* docs: Convert best-practices,overview,packages,mesa,index to .md via rst2myst by @rht in https://github.com/projectmesa/mesa/pull/2034
+* docs: Convert api/*.rst -> api/*.md via rst2myst by @rht in https://github.com/projectmesa/mesa/pull/2035
+* docs: Rewrite howto.md using ChatGPT for clarity and conciseness by @rht in https://github.com/projectmesa/mesa/pull/2037
+* docs: Corrected Contributing Guide Link to Ensure Accessibility by @sahusiddharth in https://github.com/projectmesa/mesa/pull/2057
+* Rename links to internal .rst files to .md by @rht in https://github.com/projectmesa/mesa/pull/2058
+* docs: improve introductory tutorial by @puer-robustus in https://github.com/projectmesa/mesa/pull/2087
+### 🔧 Maintenance
+* Quality of Life: Make codecov less meticulous by @Corvince in https://github.com/projectmesa/mesa/pull/1966
+* Add CI workflow for performance benchmarks by @EwoutH in https://github.com/projectmesa/mesa/pull/1983
+* tests: Resolve warnings by defining PropertyLayer dtypes by @EwoutH in https://github.com/projectmesa/mesa/pull/1987
+* benchmarks.yml: Fix PR branch checkout when triggered by comment by @EwoutH in https://github.com/projectmesa/mesa/pull/1998
+* Quality of life: automatically fix ruff errors by @Corvince in https://github.com/projectmesa/mesa/pull/2004
+* benchmarks.yml: Run on addition of label instead of comment by @EwoutH in https://github.com/projectmesa/mesa/pull/2002
+* ci: Move codespell to pre-commit by @rht in https://github.com/projectmesa/mesa/pull/2040
+* Schelling by @coderbeta1 in https://github.com/projectmesa/mesa/pull/2053
+* Move ruff lint settings into dedicated section by @Corvince in https://github.com/projectmesa/mesa/pull/2073
+* ci: Use uv pip for faster build by @rht in https://github.com/projectmesa/mesa/pull/2038
+* test: Remove place_agent duplicate warnings by @rht in https://github.com/projectmesa/mesa/pull/2086
+### Other changes
+* Minor edits to benchmarking code by @quaquel in https://github.com/projectmesa/mesa/pull/1985
+* build(deps): bump codecov/codecov-action from 3 to 4 by @dependabot in https://github.com/projectmesa/mesa/pull/2030
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/projectmesa/mesa/pull/2029
+* tests: Speed up test_batch_run by @rht in https://github.com/projectmesa/mesa/pull/2039
+* Update benchmarks.yml by @Corvince in https://github.com/projectmesa/mesa/pull/2043
+* docs: Convert visualization .rst -> .md via rst2myst by @rht in https://github.com/projectmesa/mesa/pull/2036
+* docs: Convert CONTRIBUTING .rst -> .md via rst2myst by @rht in https://github.com/projectmesa/mesa/pull/2041
+* Correct wolf energy gained from eating sheep by @JackAtOmenApps in https://github.com/projectmesa/mesa/pull/2048
+* feat: Implement Altair version of grid visualization by @rht in https://github.com/projectmesa/mesa/pull/1991
+
+## New Contributors
+* @sw23 made their first contribution in https://github.com/projectmesa/mesa/pull/2025
+* @JackAtOmenApps made their first contribution in https://github.com/projectmesa/mesa/pull/2048
+* @coderbeta1 made their first contribution in https://github.com/projectmesa/mesa/pull/2054
+* @sahusiddharth made their first contribution in https://github.com/projectmesa/mesa/pull/2057
+* @FoFFolo made their first contribution in https://github.com/projectmesa/mesa/pull/2082
+* @puer-robustus made their first contribution in https://github.com/projectmesa/mesa/pull/2083
+
+**Full Changelog**: https://github.com/projectmesa/mesa/compare/v2.2.4...2.3.0-rc1
+
+# 2.2.4 (2024-01-26)
+## Highlights
+Mesa v2.2.4 is a small but important bugfix release for the 2.2 release series. It fixes an essential bug in where agents weren't shuffled in the `BaseScheduler`, affecting mainly the `RandomActivation` scheduler (effectively making it sequential activation)([#2007](https://github.com/projectmesa/mesa/pull/2007)). It also fixes a small behaviour change in `RandomActivationByType.agents_by_type()` ([#1996](https://github.com/projectmesa/mesa/pull/1996)). Furthermore, this release adds an internal clock to the `Model`, which allows to use a Mesa model without a scheduler (using the `AgentSet` API)([#1942](https://github.com/projectmesa/mesa/pull/1942)).
+
+Updating from previous 2.2 releases is highly recommended, especially when using the `RandomActivation` scheduler.
+
+## What's Changed
+### 🛠 Enhancements made
+* refactor: Remove dependence on model.schedule, add clock to Model by @rht in https://github.com/projectmesa/mesa/pull/1942
+### 🐛 Bugs fixed
+* Fix AgentSet inplace shuffle (and thus RandomActivation), add tests by @EwoutH and @quaquel in https://github.com/projectmesa/mesa/pull/2007
+* fix: Reverse dict key and value for agents_by_type by @rht in https://github.com/projectmesa/mesa/pull/1996
+
+**Full Changelog**: https://github.com/projectmesa/mesa/compare/v2.2.3...v2.2.4
+
+# 2.2.3 (2024-01-22)
+## Highlights
+Mesa 2.2.3 is a small release with two improvements to the experimental Solara visualisation, on request of one of our contributors. No stable features have changed.
+
+## What's Changed
+### 🧪 Experimental features
+* solara_viz: Add borders around ContinuousSpace by @EwoutH in https://github.com/projectmesa/mesa/pull/1988
+### 🐛 Bugs fixed
+* fix: Explicitly specify JupyterViz space view limits by @rht in https://github.com/projectmesa/mesa/pull/1984
+
+**Full Changelog**: https://github.com/projectmesa/mesa/compare/v2.2.2...v2.2.3
+
 # 2.2.2 (2024-01-22)
 
 ## Highlights
 
 Mesa 2.2.2 is a small bugfix release, for models in which users had defined  `Model.agents` (`self.agents` in a Model (sub)class). This is deprecated, but for now allowed. See [#1919 (comment)](https://github.com/projectmesa/mesa/discussions/1919#discussioncomment-8141844).
 
 ## What's Changed
```

### Comparing `mesa-2.3.0.dev0/docker-compose.yml` & `mesa-2.3.0rc1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/.github/release.yml` & `mesa-2.3.0rc1/.github/release.yml`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/.github/ISSUE_TEMPLATE/bug-report.md` & `mesa-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/.github/workflows/benchmarks.yml` & `mesa-2.3.0rc1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/.github/workflows/release.yml` & `mesa-2.3.0rc1/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     steps:
       - name: Checkout source
         uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
+          cache: 'pip'
       - name: Install dependencies
         run: pip install -U pip hatch
       - name: Build distributions
         run: hatch build
       - name: Upload package as artifact to GitHub
         if: github.repository == 'projectmesa/mesa' && startsWith(github.ref, 'refs/tags')
         uses: actions/upload-artifact@v4
```

### Comparing `mesa-2.3.0.dev0/benchmarks/compare_timings.py` & `mesa-2.3.0rc1/benchmarks/compare_timings.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/benchmarks/configurations.py` & `mesa-2.3.0rc1/benchmarks/configurations.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/benchmarks/Flocking/flocking.py` & `mesa-2.3.0rc1/benchmarks/Flocking/flocking.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,51 +16,48 @@
 
     The agent follows three behaviors to flock:
         - Cohesion: steering towards neighboring agents.
         - Separation: avoiding getting too close to any other agent.
         - Alignment: try to fly in the same direction as the neighbors.
 
     Boids have a vision that defines the radius in which they look for their
-    neighbors to flock with. Their speed (a scalar) and velocity (a vector)
+    neighbors to flock with. Their speed (a scalar) and direction (a vector)
     define their movement. Separation is their desired minimum distance from
     any other Boid.
     """
 
     def __init__(
         self,
         unique_id,
         model,
-        pos,
         speed,
-        velocity,
+        direction,
         vision,
         separation,
         cohere=0.03,
         separate=0.015,
         match=0.05,
     ):
         """
         Create a new Boid flocker agent.
 
         Args:
             unique_id: Unique agent identifier.
-            pos: Starting position
             speed: Distance to move per step.
-            heading: numpy vector for the Boid's direction of movement.
+            direction: numpy vector for the Boid's direction of movement.
             vision: Radius to look around for nearby Boids.
             separation: Minimum distance to maintain from other Boids.
             cohere: the relative importance of matching neighbors' positions
             separate: the relative importance of avoiding close neighbors
-            match: the relative importance of matching neighbors' headings
+            match: the relative importance of matching neighbors' directions
 
         """
         super().__init__(unique_id, model)
-        self.pos = np.array(pos)
         self.speed = speed
-        self.velocity = velocity
+        self.direction = direction
         self.vision = vision
         self.separation = separation
         self.cohere_factor = cohere
         self.separate_factor = separate
         self.match_factor = match
 
     def step(self):
@@ -73,95 +70,97 @@
         match_vector, separation_vector, cohere = np.zeros((3, 2))
         for neighbor in neighbors:
             n += 1
             heading = self.model.space.get_heading(self.pos, neighbor.pos)
             cohere += heading
             if self.model.space.get_distance(self.pos, neighbor.pos) < self.separation:
                 separation_vector -= heading
-            match_vector += neighbor.velocity
+            match_vector += neighbor.direction
         n = max(n, 1)
         cohere = cohere * self.cohere_factor
         separation_vector = separation_vector * self.separate_factor
         match_vector = match_vector * self.match_factor
-        self.velocity += (cohere + separation_vector + match_vector) / n
-        self.velocity /= np.linalg.norm(self.velocity)
-        new_pos = self.pos + self.velocity * self.speed
+        self.direction += (cohere + separation_vector + match_vector) / n
+        self.direction /= np.linalg.norm(self.direction)
+        new_pos = self.pos + self.direction * self.speed
         self.model.space.move_agent(self, new_pos)
 
 
 class BoidFlockers(mesa.Model):
     """
     Flocker model class. Handles agent creation, placement and scheduling.
     """
 
     def __init__(
         self,
-        seed,
-        population,
-        width,
-        height,
-        vision,
+        seed=None,
+        population=100,
+        width=100,
+        height=100,
+        vision=10,
         speed=1,
         separation=1,
         cohere=0.03,
         separate=0.015,
         match=0.05,
+        simulator=None,
     ):
         """
         Create a new Flockers model.
 
         Args:
             population: Number of Boids
             width, height: Size of the space.
             speed: How fast should the Boids move.
             vision: How far around should each Boid look for its neighbors
             separation: What's the minimum distance each Boid will attempt to
                     keep from any other
             cohere, separate, match: factors for the relative importance of
-                    the three drives."""
+                    the three drives.
+        """
         super().__init__(seed=seed)
         self.population = population
-        self.vision = vision
-        self.speed = speed
-        self.separation = separation
+        self.width = width
+        self.height = height
+        self.simulator = simulator
+
         self.schedule = mesa.time.RandomActivation(self)
-        self.space = mesa.space.ContinuousSpace(width, height, True)
-        self.factors = {"cohere": cohere, "separate": separate, "match": match}
-        self.make_agents()
+        self.space = mesa.space.ContinuousSpace(self.width, self.height, True)
+        self.factors = {
+            "cohere": cohere,
+            "separate": separate,
+            "match": match,
+        }
 
-    def make_agents(self):
-        """
-        Create self.population agents, with random positions and starting headings.
-        """
         for i in range(self.population):
             x = self.random.random() * self.space.x_max
             y = self.random.random() * self.space.y_max
             pos = np.array((x, y))
-            velocity = np.random.random(2) * 2 - 1
+            direction = np.random.random(2) * 2 - 1
             boid = Boid(
-                i,
-                self,
-                pos,
-                self.speed,
-                velocity,
-                self.vision,
-                self.separation,
+                unique_id=i,
+                model=self,
+                pos=pos,
+                speed=speed,
+                direction=direction,
+                vision=vision,
+                separation=separation,
                 **self.factors,
             )
             self.space.place_agent(boid, pos)
             self.schedule.add(boid)
 
     def step(self):
         self.schedule.step()
 
 
 if __name__ == "__main__":
     import time
 
-    # model = BoidFlockers(15, 200, 100, 100, 5)
-    model = BoidFlockers(15, 400, 100, 100, 15)
+    # model = BoidFlockers(seed=15, population=200, width=100, height=100, vision=5)
+    model = BoidFlockers(seed=15, population=400, width=100, height=100, vision=15)
 
     start_time = time.perf_counter()
     for _ in range(100):
         model.step()
 
     print(time.perf_counter() - start_time)
```

### Comparing `mesa-2.3.0.dev0/benchmarks/Schelling/schelling.py` & `mesa-2.3.0rc1/tests/test_lifespan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,95 @@
-import mesa
+import unittest
 
+import numpy as np
 
-class SchellingAgent(mesa.Agent):
-    """
-    Schelling segregation agent
-    """
+from mesa import Agent, Model
+from mesa.datacollection import DataCollector
+from mesa.time import RandomActivation
 
-    def __init__(self, unique_id, model, agent_type):
-        """
-        Create a new Schelling agent.
-        Args:
-           unique_id: Unique identifier for the agent.
-           x, y: Agent initial location.
-           agent_type: Indicator for the agent's type (minority=1, majority=0)
-        """
-        super().__init__(unique_id, model)
-        self.type = agent_type
 
-    def step(self):
-        similar = 0
-        for neighbor in self.model.grid.iter_neighbors(
-            self.pos, moore=True, radius=self.model.radius
-        ):
-            if neighbor.type == self.type:
-                similar += 1
-
-        # If unhappy, move:
-        if similar < self.model.homophily:
-            self.model.grid.move_to_empty(self)
-        else:
-            self.model.happy += 1
+class LifeTimeModel(Model):
+    """Simple model for running models with a finite life"""
 
+    def __init__(self, agent_lifetime=1, n_agents=10):
+        super().__init__()
 
-class Schelling(mesa.Model):
-    """
-    Model class for the Schelling segregation model.
-    """
+        self.agent_lifetime = agent_lifetime
+        self.n_agents = n_agents
+
+        # keep track of the the remaining life of an agent and
+        # how many ticks it has seen
+        self.datacollector = DataCollector(
+            agent_reporters={
+                "remaining_life": lambda a: a.remaining_life,
+                "steps": lambda a: a.steps,
+            }
+        )
+
+        self.current_ID = 0
+        self.schedule = RandomActivation(self)
 
-    def __init__(
-        self, seed, height, width, homophily, radius, density, minority_pc=0.5
-    ):
-        """ """
-        super().__init__(seed=seed)
-        self.height = height
-        self.width = width
-        self.density = density
-        self.minority_pc = minority_pc
-        self.homophily = homophily
-        self.radius = radius
-
-        self.schedule = mesa.time.RandomActivation(self)
-        self.grid = mesa.space.SingleGrid(height, width, torus=True)
-
-        self.happy = 0
-
-        # Set up agents
-        # We use a grid iterator that returns
-        # the coordinates of a cell as well as
-        # its contents. (coord_iter)
-        for _cont, pos in self.grid.coord_iter():
-            if self.random.random() < self.density:
-                agent_type = 1 if self.random.random() < self.minority_pc else 0
-                agent = SchellingAgent(self.next_id(), self, agent_type)
-                self.grid.place_agent(agent, pos)
-                self.schedule.add(agent)
+        for _ in range(n_agents):
+            self.schedule.add(
+                FiniteLifeAgent(self.next_id(), self.agent_lifetime, self)
+            )
 
     def step(self):
-        """
-        Run one step of the model.
-        """
-        self.happy = 0  # Reset counter of happy agents
+        """Add agents back to n_agents in each step"""
+        self.datacollector.collect(self)
         self.schedule.step()
 
+        if len(self.schedule.agents) < self.n_agents:
+            for _ in range(self.n_agents - len(self.schedule.agents)):
+                self.schedule.add(
+                    FiniteLifeAgent(self.next_id(), self.agent_lifetime, self)
+                )
+
+    def run_model(self, step_count=100):
+        for _ in range(step_count):
+            self.step()
 
-if __name__ == "__main__":
-    import time
 
-    # model = Schelling(15, 40, 40, 3, 1, 0.625)
-    model = Schelling(15, 100, 100, 8, 2, 0.8)
+class FiniteLifeAgent(Agent):
+    """An agent that is supposed to live for a finite number of ticks.
+    Also has a 10% chance of dying in each tick.
+    """
 
-    start_time = time.perf_counter()
-    for _ in range(100):
-        model.step()
+    def __init__(self, unique_id, lifetime, model):
+        super().__init__(unique_id, model)
+        self.remaining_life = lifetime
+        self.steps = 0
+        self.model = model
 
-    print(time.perf_counter() - start_time)
+    def step(self):
+        inactivated = self.inactivate()
+        if not inactivated:
+            self.steps += 1  # keep track of how many ticks are seen
+            if np.random.binomial(1, 0.1) != 0:  # 10% chance of dying
+                self.model.schedule.remove(self)
+
+    def inactivate(self):
+        self.remaining_life -= 1
+        if self.remaining_life < 0:
+            self.model.schedule.remove(self)
+            return True
+        return False
+
+
+class TestAgentLifespan(unittest.TestCase):
+    def setUp(self):
+        self.model = LifeTimeModel()
+        self.model.run_model()
+        self.df = self.model.datacollector.get_agent_vars_dataframe()
+        self.df = self.df.reset_index()
+
+    def test_ticks_seen(self):
+        """Each agent should be activated no more than one time"""
+        assert self.df.steps.max() == 1
+
+    def test_agent_lifetime(self):
+        lifetimes = self.df.groupby(["AgentID"]).agg({"Step": len})
+        assert lifetimes.Step.max() == 2
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mesa-2.3.0.dev0/benchmarks/WolfSheep/wolf_sheep.py` & `mesa-2.3.0rc1/benchmarks/WolfSheep/wolf_sheep.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,49 +5,46 @@
 Replication of the model found in NetLogo:
     Wilensky, U. (1997). NetLogo Wolf Sheep Predation model.
     http://ccl.northwestern.edu/netlogo/models/WolfSheepPredation.
     Center for Connected Learning and Computer-Based Modeling,
     Northwestern University, Evanston, IL.
 """
 
-import mesa
+import math
 
+from mesa import Model
+from mesa.experimental.cell_space import CellAgent, OrthogonalVonNeumannGrid
+from mesa.experimental.devs import ABMSimulator
 
-class Animal(mesa.Agent):
-    def __init__(self, unique_id, model, moore, energy, p_reproduce, energy_from_food):
+
+class Animal(CellAgent):
+    def __init__(self, unique_id, model, energy, p_reproduce, energy_from_food):
         super().__init__(unique_id, model)
         self.energy = energy
         self.p_reproduce = p_reproduce
         self.energy_from_food = energy_from_food
-        self.moore = moore
 
     def random_move(self):
-        next_moves = self.model.grid.get_neighborhood(self.pos, self.moore, True)
-        next_move = self.random.choice(next_moves)
-        # Now move:
-        self.model.grid.move_agent(self, next_move)
+        self.move_to(self.cell.neighborhood().select_random_cell())
 
     def spawn_offspring(self):
         self.energy /= 2
         offspring = self.__class__(
             self.model.next_id(),
             self.model,
-            self.moore,
             self.energy,
             self.p_reproduce,
             self.energy_from_food,
         )
-        self.model.grid.place_agent(offspring, self.pos)
-        self.model.schedule.add(offspring)
+        offspring.move_to(self.cell)
 
-    def feed(self):
-        ...
+    def feed(self): ...
 
     def die(self):
-        self.model.grid.remove_agent(self)
+        self.cell.remove_agent(self)
         self.remove()
 
     def step(self):
         self.random_move()
         self.energy -= 1
 
         self.feed()
@@ -63,159 +60,195 @@
     A sheep that walks around, reproduces (asexually) and gets eaten.
 
     The init is the same as the RandomWalker.
     """
 
     def feed(self):
         # If there is grass available, eat it
-        agents = self.model.grid.get_cell_list_contents(self.pos)
-        grass_patch = next(obj for obj in agents if isinstance(obj, GrassPatch))
+        grass_patch = next(
+            obj for obj in self.cell.agents if isinstance(obj, GrassPatch)
+        )
         if grass_patch.fully_grown:
             self.energy += self.energy_from_food
             grass_patch.fully_grown = False
 
 
 class Wolf(Animal):
     """
     A wolf that walks around, reproduces (asexually) and eats sheep.
     """
 
     def feed(self):
-        agents = self.model.grid.get_cell_list_contents(self.pos)
-        sheep = [obj for obj in agents if isinstance(obj, Sheep)]
+        sheep = [obj for obj in self.cell.agents if isinstance(obj, Sheep)]
         if len(sheep) > 0:
             sheep_to_eat = self.random.choice(sheep)
             self.energy += self.energy_from_food
 
             # Kill the sheep
             sheep_to_eat.die()
 
 
-class GrassPatch(mesa.Agent):
+class GrassPatch(CellAgent):
     """
     A patch of grass that grows at a fixed rate and it is eaten by sheep
     """
 
-    def __init__(self, unique_id, model, fully_grown, countdown):
+    @property
+    def fully_grown(self):
+        return self._fully_grown
+
+    @fully_grown.setter
+    def fully_grown(self, value: bool) -> None:
+        self._fully_grown = value
+
+        if not value:
+            self.model.simulator.schedule_event_relative(
+                setattr,
+                self.grass_regrowth_time,
+                function_args=[self, "fully_grown", True],
+            )
+
+    def __init__(self, unique_id, model, fully_grown, countdown, grass_regrowth_time):
         """
+        TODO:: fully grown can just be an int --> so one less param (i.e. countdown)
+
         Creates a new patch of grass
 
         Args:
-            grown: (boolean) Whether the patch of grass is fully grown or not
+            fully_grown: (boolean) Whether the patch of grass is fully grown or not
             countdown: Time for the patch of grass to be fully grown again
+            grass_regrowth_time : time to fully regrow grass
+            countdown : Time for the patch of grass to be fully regrown if fully grown is False
         """
         super().__init__(unique_id, model)
-        self.fully_grown = fully_grown
-        self.countdown = countdown
+        self._fully_grown = fully_grown
+        self.grass_regrowth_time = grass_regrowth_time
 
-    def step(self):
         if not self.fully_grown:
-            if self.countdown <= 0:
-                # Set as fully grown
-                self.fully_grown = True
-                self.countdown = self.model.grass_regrowth_time
-            else:
-                self.countdown -= 1
+            self.model.simulator.schedule_event_relative(
+                setattr, countdown, function_args=[self, "fully_grown", True]
+            )
 
 
-class WolfSheep(mesa.Model):
+class WolfSheep(Model):
     """
     Wolf-Sheep Predation Model
 
     A model for simulating wolf and sheep (predator-prey) ecosystem modelling.
     """
 
     def __init__(
         self,
-        seed,
+        simulator,
         height,
         width,
         initial_sheep,
         initial_wolves,
         sheep_reproduce,
         wolf_reproduce,
         grass_regrowth_time,
         wolf_gain_from_food=13,
         sheep_gain_from_food=5,
-        moore=False,
+        seed=None,
     ):
         """
         Create a new Wolf-Sheep model with the given parameters.
 
         Args:
+            simulator: ABMSimulator instance
             initial_sheep: Number of sheep to start with
             initial_wolves: Number of wolves to start with
             sheep_reproduce: Probability of each sheep reproducing each step
             wolf_reproduce: Probability of each wolf reproducing each step
             wolf_gain_from_food: Energy a wolf gains from eating a sheep
-            grass: Whether to have the sheep eat grass for energy
             grass_regrowth_time: How long it takes for a grass patch to regrow
                                  once it is eaten
             sheep_gain_from_food: Energy sheep gain from grass, if enabled.
-            moore:
+            seed : the random seed
         """
         super().__init__(seed=seed)
         # Set parameters
         self.height = height
         self.width = width
+        self.simulator = simulator
+
         self.initial_sheep = initial_sheep
         self.initial_wolves = initial_wolves
-        self.grass_regrowth_time = grass_regrowth_time
 
-        self.schedule = mesa.time.RandomActivationByType(self)
-        self.grid = mesa.space.MultiGrid(self.height, self.width, torus=False)
+        self.grid = OrthogonalVonNeumannGrid(
+            [self.height, self.width],
+            torus=False,
+            capacity=math.inf,
+            random=self.random,
+        )
 
+        # Create sheep:
         for _ in range(self.initial_sheep):
             pos = (
                 self.random.randrange(self.width),
                 self.random.randrange(self.height),
             )
             energy = self.random.randrange(2 * sheep_gain_from_food)
             sheep = Sheep(
                 self.next_id(),
                 self,
-                moore,
                 energy,
                 sheep_reproduce,
                 sheep_gain_from_food,
             )
-            self.grid.place_agent(sheep, pos)
-            self.schedule.add(sheep)
+            sheep.move_to(self.grid[pos])
 
         # Create wolves
         for _ in range(self.initial_wolves):
             pos = (
                 self.random.randrange(self.width),
                 self.random.randrange(self.height),
             )
             energy = self.random.randrange(2 * wolf_gain_from_food)
             wolf = Wolf(
-                self.next_id(), self, moore, energy, wolf_reproduce, wolf_gain_from_food
+                self.next_id(),
+                self,
+                energy,
+                wolf_reproduce,
+                wolf_gain_from_food,
             )
-            self.grid.place_agent(wolf, pos)
-            self.schedule.add(wolf)
+            wolf.move_to(self.grid[pos])
 
         # Create grass patches
         possibly_fully_grown = [True, False]
-        for _agent, pos in self.grid.coord_iter():
+        for cell in self.grid:
             fully_grown = self.random.choice(possibly_fully_grown)
             if fully_grown:
-                countdown = self.grass_regrowth_time
+                countdown = grass_regrowth_time
             else:
-                countdown = self.random.randrange(self.grass_regrowth_time)
-            patch = GrassPatch(self.next_id(), self, fully_grown, countdown)
-            self.grid.place_agent(patch, pos)
-            self.schedule.add(patch)
+                countdown = self.random.randrange(grass_regrowth_time)
+            patch = GrassPatch(
+                self.next_id(), self, fully_grown, countdown, grass_regrowth_time
+            )
+            patch.move_to(cell)
 
     def step(self):
-        self.schedule.step()
+        self.get_agents_of_type(Sheep).shuffle(inplace=True).do("step")
+        self.get_agents_of_type(Wolf).shuffle(inplace=True).do("step")
 
 
 if __name__ == "__main__":
     import time
 
-    model = WolfSheep(15, 25, 25, 60, 40, 0.2, 0.1, 20)
+    simulator = ABMSimulator()
+    model = WolfSheep(
+        simulator,
+        25,
+        25,
+        60,
+        40,
+        0.2,
+        0.1,
+        20,
+        seed=15,
+    )
+
+    simulator.setup(model)
 
     start_time = time.perf_counter()
-    for _ in range(100):
-        model.step()
+    simulator.run(100)
     print("Time:", time.perf_counter() - start_time)
```

### Comparing `mesa-2.3.0.dev0/docs/Makefile` & `mesa-2.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/README.md` & `mesa-2.3.0rc1/docs/README.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/best-practices.md` & `mesa-2.3.0rc1/docs/best-practices.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/conf.py` & `mesa-2.3.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/howto.md` & `mesa-2.3.0rc1/docs/howto.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/index.md` & `mesa-2.3.0rc1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 # Indices and tables
 
 - {ref}`genindex`
 - {ref}`modindex`
 - {ref}`search`
 
-[contributors guide]: https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.rst
+[contributors guide]: https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.md
 [email list]: https://groups.google.com/d/forum/projectmesa
 [github]: https://github.com/projectmesa/mesa/
 [github issue tracker]: https://github.com/projectmesa/mesa/issues
 [mesa]: https://github.com/projectmesa/mesa/
 [mesa introductory tutorial]: tutorials/intro_tutorial.html
 [mesa visualization tutorial]: tutorials/visualization_tutorial.html
 [pypi]: https://pypi.python.org/pypi/Mesa/
```

### Comparing `mesa-2.3.0.dev0/docs/make.bat` & `mesa-2.3.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/mesa.md` & `mesa-2.3.0rc1/docs/mesa.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/mesa.visualization.md` & `mesa-2.3.0rc1/docs/mesa.visualization.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/mesa.visualization.modules.md` & `mesa-2.3.0rc1/docs/mesa.visualization.modules.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/modular-visualization.md` & `mesa-2.3.0rc1/docs/modular-visualization.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/overview.md` & `mesa-2.3.0rc1/docs/overview.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/packages.md` & `mesa-2.3.0rc1/docs/packages.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/apis/visualization.md` & `mesa-2.3.0rc1/docs/apis/visualization.md`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/Mesa_Screenshot.png` & `mesa-2.3.0rc1/docs/images/Mesa_Screenshot.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/mesa_logo.ico` & `mesa-2.3.0rc1/docs/images/mesa_logo.ico`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/mesa_logo.png` & `mesa-2.3.0rc1/docs/images/mesa_logo.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/br_ginis.png` & `mesa-2.3.0rc1/docs/images/tutorial/br_ginis.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/dc_endwealth.png` & `mesa-2.3.0rc1/docs/images/tutorial/dc_endwealth.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/dc_gini.png` & `mesa-2.3.0rc1/docs/images/tutorial/dc_gini.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/dc_oneagent.png` & `mesa-2.3.0rc1/docs/images/tutorial/dc_oneagent.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/first_hist.png` & `mesa-2.3.0rc1/docs/images/tutorial/first_hist.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/multirun_hist.png` & `mesa-2.3.0rc1/docs/images/tutorial/multirun_hist.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/numpy_grid.png` & `mesa-2.3.0rc1/docs/images/tutorial/numpy_grid.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/viz_chart.png` & `mesa-2.3.0rc1/docs/images/tutorial/viz_chart.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/viz_empty.png` & `mesa-2.3.0rc1/docs/images/tutorial/viz_empty.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/viz_greycircles.png` & `mesa-2.3.0rc1/docs/images/tutorial/viz_greycircles.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/viz_histogram.png` & `mesa-2.3.0rc1/docs/images/tutorial/viz_histogram.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/images/tutorial/viz_redcircles.png` & `mesa-2.3.0rc1/docs/images/tutorial/viz_redcircles.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/MoneyModel.py` & `mesa-2.3.0rc1/docs/tutorials/MoneyModel.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/adv_tutorial_legacy.ipynb` & `mesa-2.3.0rc1/docs/tutorials/adv_tutorial_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/intro_tutorial.ipynb` & `mesa-2.3.0rc1/docs/tutorials/intro_tutorial.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992306694553885%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(0, '### Import Dependencies\\n')], delete: [0]}}, 12: "*

 * *            "{'source': {insert: [(7, '**Code implementation:** The technical details about the "*

 * *            'timer object can be found in the [mesa '*

 * *            'repo](https://github.com/projectmesa/mesa/blob/main/mesa/time.py). Mesa offers a few '*

 * *            'different built-in scheduler classes, with a common interface. That makes it easy to '*

 * *            'change the activation regime a given model uses, and […]*

```diff
@@ -132,15 +132,15 @@
                 "*Code will be added as the tutorial progresses.*\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Import Dependencies\n",
+                "### Import Dependencies\n",
                 "This includes importing of dependencies needed for the tutorial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -239,15 +239,15 @@
                 "### Adding the Scheduler\n",
                 "Now the model will be modified to add a scheduler.\n",
                 "\n",
                 "**Background:** The scheduler controls the order in which agents are activated, causing the agent to take their defined action. The scheduler is also responsible for advancing the model by one step. A step is the smallest unit of time in the model, and is often referred to as a tick. The scheduler can be configured to activate agents in different orders. This can be important as the order in which agents are activated can impact the results of the model [Comer2014]. At each step of the model, one or more of the agents -- usually all of them -- are activated and take their own step, changing internally and/or interacting with one another or the environment.\n",
                 "\n",
                 "**Model-specific information:** A new class is named `RandomActivationByAgent` is created which extends `mesa.time.RandomActivation` creating a subclass of  the `RandomActivation` class from Mesa. This class activates all the agents once per step, in random order. Every agent is expected to have a ``step`` method. The step method is the action the agent takes when it is activated by the model schedule. We add an agent to the schedule using the `add` method; when we call the schedule's `step` method, the model shuffles the order of the agents, then activates and executes each agent's ```step``` method. The scheduler is then added to the model.\n",
                 "\n",
-                "**Code implementation:** The technical details about the timer object can be found in the [mesa repo](https://github.com/projectmesa/mesa/blob/main/mesa/time.py). Mesa offers a few different built-in scheduler classes, with a common interface. That makes it easy to change the activation regime a given model uses, and see whether it changes the model behavior. The details pertaining to the scheduler interface can be located the same [mesa repo](https://github.com/projectmesa/mesa/blob/main/mesa/time.py).\n",
+                "**Code implementation:** The technical details about the timer object can be found in the [mesa repo](https://github.com/projectmesa/mesa/blob/main/mesa/time.py). Mesa offers a few different built-in scheduler classes, with a common interface. That makes it easy to change the activation regime a given model uses, and see whether it changes the model behavior. The details pertaining to the scheduler interface can be located in the same [mesa repo](https://github.com/projectmesa/mesa/blob/main/mesa/time.py).\n",
                 "\n",
                 "With that in mind, the `MoneyAgent` code is modified below to visually show when a new agent is created. The MoneyModel code is modified by adding the RandomActivation method to the model. with the scheduler added looks like this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -539,15 +539,15 @@
                 "\n",
                 "Many ABMs have a spatial element, with agents moving around and interacting with nearby neighbors. Mesa currently supports two overall kinds of spaces: grid, and continuous. Grids are divided into cells, and agents can only be on a particular cell, like pieces on a chess board. Continuous space, in contrast, allows agents to have any arbitrary position. Both grids and continuous spaces are frequently [toroidal](https://en.wikipedia.org/wiki/Toroidal_graph), meaning that the edges wrap around, with cells on the right edge connected to those on the left edge, and the top to the bottom. This prevents some cells having fewer neighbors than others, or agents being able to go off the edge of the environment.\n",
                 "\n",
                 "Let's add a simple spatial element to our model by putting our agents on a grid and make them walk around at random. Instead of giving their unit of money to any random agent, they'll give it to an agent on the same cell.\n",
                 "\n",
                 "Mesa has two main types of grids: `SingleGrid` and `MultiGrid`*. `SingleGrid` enforces at most one agent per cell; `MultiGrid` allows multiple agents to be in the same cell. Since we want agents to be able to share a cell, we use `MultiGrid`.\n",
                 "\n",
-                "*However there are more types of space to include `HexGrid`, `NetworkGrid`, and the previously mentioned `ContinuousSpace`. Similar to `mesa.time` context is retained with `mesa.space.[enter class]`. You can see the different classes as [mesa.space](https://github.com/projectmesa/mesa/blob/main/mesa/space.py) "
+                "*However there are more types of space to include `HexGrid`, `NetworkGrid`, and the previously mentioned `ContinuousSpace`. Similar to `mesa.time` context is retained with `mesa.space.[enter class]`. You can inspect the different classes at [mesa.space](https://github.com/projectmesa/mesa/blob/main/mesa/space.py)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We instantiate a grid with width and height parameters, and a boolean as to whether the grid is toroidal. Let's make width and height model parameters, in addition to the number of agents, and have the grid always be toroidal. We can place agents on a grid with the grid's `place_agent` method, which takes an agent and an (x, y) tuple of the coordinates to place the agent."
@@ -825,17 +825,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "At every step of the model, the datacollector will collect and store the model-level current Gini coefficient, as well as each agent's wealth, associating each with the current step.\n",
                 "\n",
-                "We run the model just as we did above. Now is when an interactive session, especially via a Notebook, comes in handy: the DataCollector can export the data its collected as a pandas\\* DataFrame, for easy interactive analysis. \n",
+                "We run the model just as we did above. Now is when an interactive session, especially via a Notebook, comes in handy: the DataCollector can export the data its collected as a pandas* DataFrame, for easy interactive analysis. \n",
                 "\n",
-                "\\*If you are new to Python, please be aware that pandas is already installed as a dependency of Mesa and that [pandas](https://pandas.pydata.org/docs/) is a \"fast, powerful, flexible and easy to use open source data analysis and manipulation tool\". pandas is great resource to help analyze the data collected in your models "
+                "*If you are new to Python, please be aware that pandas is already installed as a dependency of Mesa and that [pandas](https://pandas.pydata.org/docs/) is a \"fast, powerful, flexible and easy to use open source data analysis and manipulation tool\". pandas is great resource to help analyze the data collected in your models."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1140,15 +1140,15 @@
                 "Note: The total number of runs is 245 (= 49 different populations * 5 iterations per population). However, the resulting list of dictionaries will be of length 6186250 (= 250 average agents per population * 49 different populations * 5 iterations per population * 101 steps per iteration). "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "**Note for Windows OS users:** If you are running this tutorial in Jupyter, make sure that you set `number_processes = 1` (single process). If `number_processes` is greater than 1, it is less straightforward to set up. You can read [Mesa's how-to guide](https://github.com/projectmesa/mesa/blob/main/docs/howto.rst), in 'Using multi-process `batch_run` on Windows' section for how to do it."
+                "**Note for Windows OS users:** If you are running this tutorial in Jupyter, make sure that you set `number_processes = 1` (single process). If `number_processes` is greater than 1, it is less straightforward to set up. You can read [Mesa's how-to guide](https://github.com/projectmesa/mesa/blob/main/docs/howto.md), in 'Using multi-process `batch_run` on Windows' section for how to do it."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1287,15 +1287,15 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "### Analyzing model reporters: Comparing 5 scenarios\n",
-                "Other insight might be gathered when we compare the Gini coefficient of different scenarios. For example, we can compare the Gini coefficient of a population with 25 agents to the Gini coefficient of a population with 400 agents. While doing this, we increase the number of iterations to 25 to get a better estimate of the Gini coefficient for each population size and get usable error estimations."
+                "Other insights might be gathered when we compare the Gini coefficient of different scenarios. For example, we can compare the Gini coefficient of a population with 25 agents to the Gini coefficient of a population with 400 agents. While doing this, we increase the number of iterations to 25 to get a better estimate of the Gini coefficient for each population size and get usable error estimations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
```

### Comparing `mesa-2.3.0.dev0/docs/tutorials/visualization_tutorial.ipynb` & `mesa-2.3.0rc1/docs/tutorials/visualization_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_chart.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_chart.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_empty.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_empty.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_greycircles.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_greycircles.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_histogram.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_histogram.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_redcircles.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_redcircles.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/docs/tutorials/files/viz_slider.png` & `mesa-2.3.0rc1/docs/tutorials/files/viz_slider.png`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/__init__.py` & `mesa-2.3.0rc1/mesa/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Mesa Agent-Based Modeling Framework
 
 Core Objects: Model, and Agent.
 """
+
 import datetime
 
 import mesa.space as space
 import mesa.time as time
 import mesa.visualization as visualization
 from mesa.agent import Agent
 from mesa.batchrunner import batch_run
@@ -21,11 +22,11 @@
     "visualization",
     "DataCollector",
     "batch_run",
     "experimental",
 ]
 
 __title__ = "mesa"
-__version__ = "2.3.0-dev"
+__version__ = "2.3.0-rc1"
 __license__ = "Apache 2.0"
 _this_year = datetime.datetime.now(tz=datetime.timezone.utc).date().year
 __copyright__ = f"Copyright {_this_year} Project Mesa Team"
```

### Comparing `mesa-2.3.0.dev0/mesa/agent.py` & `mesa-2.3.0rc1/mesa/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The agent class for Mesa framework.
 
 Core Objects: Agent
 """
+
 # Mypy; for the `|` operator purpose
 # Remove this __future__ import once the oldest supported Python is 3.10
 from __future__ import annotations
 
 import contextlib
 import copy
 import operator
@@ -77,20 +78,14 @@
     @property
     def random(self) -> Random:
         return self.model.random
 
 
 class AgentSet(MutableSet, Sequence):
     """
-    .. warning::
-        The AgentSet is experimental. It may be changed or removed in any and all future releases, including
-        patch releases.
-        We would love to hear what you think about this new feature. If you have any thoughts, share them with
-        us here: https://github.com/projectmesa/mesa/discussions/1919
-
     A collection class that represents an ordered set of agents within an agent-based model (ABM). This class
     extends both MutableSet and Sequence, providing set-like functionality with order preservation and
     sequence operations.
 
     Attributes:
         model (Model): The ABM model instance to which this AgentSet belongs.
 
@@ -111,25 +106,16 @@
         """
         Initializes the AgentSet with a collection of agents and a reference to the model.
 
         Args:
             agents (Iterable[Agent]): An iterable of Agent objects to be included in the set.
             model (Model): The ABM model instance to which this AgentSet belongs.
         """
-        self.model = model
-
-        if not self.__class__.agentset_experimental_warning_given:
-            self.__class__.agentset_experimental_warning_given = True
-            warnings.warn(
-                "The AgentSet is experimental. It may be changed or removed in any and all future releases, including patch releases.\n"
-                "We would love to hear what you think about this new feature. If you have any thoughts, share them with us here: https://github.com/projectmesa/mesa/discussions/1919",
-                FutureWarning,
-                stacklevel=2,
-            )
 
+        self.model = model
         self._agents = weakref.WeakKeyDictionary({agent: None for agent in agents})
 
     def __len__(self) -> int:
         """Return the number of agents in the AgentSet."""
         return len(self._agents)
 
     def __iter__(self) -> Iterator[Agent]:
```

### Comparing `mesa-2.3.0.dev0/mesa/batchrunner.py` & `mesa-2.3.0rc1/mesa/batchrunner.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/datacollection.py` & `mesa-2.3.0rc1/mesa/datacollection.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 Finally, DataCollector can create a pandas DataFrame from each collection.
 
 The default DataCollector here makes several assumptions:
     * The model has an agent list called agents
     * For collecting agent-level variables, agents must have a unique_id
 """
+
 import contextlib
 import itertools
 import types
 from functools import partial
 
 with contextlib.suppress(ImportError):
     import pandas as pd
```

### Comparing `mesa-2.3.0.dev0/mesa/main.py` & `mesa-2.3.0rc1/mesa/main.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/model.py` & `mesa-2.3.0rc1/mesa/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The model class for Mesa framework.
 
 Core Objects: Model
 """
+
 # Mypy; for the `|` operator purpose
 # Remove this __future__ import once the oldest supported Python is 3.10
 from __future__ import annotations
 
 import itertools
 import random
 import warnings
@@ -51,15 +52,15 @@
     def __new__(cls, *args: Any, **kwargs: Any) -> Any:
         """Create a new model object and instantiate its RNG automatically."""
         obj = object.__new__(cls)
         obj._seed = kwargs.get("seed")
         if obj._seed is None:
             # We explicitly specify the seed here so that we know its value in
             # advance.
-            obj._seed = random.random()  # noqa: S311
+            obj._seed = random.random()
         obj.random = random.Random(obj._seed)
         # TODO: Remove these 2 lines just before Mesa 3.0
         obj._steps = 0
         obj._time = 0
         return obj
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -72,17 +73,14 @@
         self.schedule = None
         self.current_id = 0
         self.agents_: defaultdict[type, dict] = defaultdict(dict)
 
         self._steps: int = 0
         self._time: TimeT = 0  # the model's clock
 
-        # Warning flags for current experimental features. These make sure a warning is only printed once per model.
-        self.agentset_experimental_warning_given = False
-
     @property
     def agents(self) -> AgentSet:
         """Provides an AgentSet of all agents in the model, combining agents from all types."""
 
         if hasattr(self, "_agents"):
             return self._agents
         else:
```

### Comparing `mesa-2.3.0.dev0/mesa/space.py` & `mesa-2.3.0rc1/mesa/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,29 @@
 
 
 def is_integer(x: Real) -> bool:
     # Check if x is either a CPython integer or Numpy integer.
     return isinstance(x, _types_integer)
 
 
+def warn_if_agent_has_position_already(placement_func):
+    def wrapper(self, agent, *args, **kwargs):
+        if agent.pos is not None:
+            warnings.warn(
+                f"""Agent {agent.unique_id} is being placed with
+place_agent() despite already having the position {agent.pos}. In most
+cases, you'd want to clear the current position with remove_agent()
+before placing the agent again.""",
+                stacklevel=2,
+            )
+        placement_func(self, agent, *args, **kwargs)
+
+    return wrapper
+
+
 class _Grid:
     """Base class for a rectangular grid.
 
     Grid cells are indexed by [x, y], where [0, 0] is assumed to be the
     bottom-left and [width-1, height-1] is the top-right. If a grid is
     toroidal, the top and bottom, and left and right, edges wrap to each other
 
@@ -131,22 +146,20 @@
                 self.is_cell_empty,
                 itertools.product(range(self.width), range(self.height)),
             )
         )
         self._empties_built = True
 
     @overload
-    def __getitem__(self, index: int | Sequence[Coordinate]) -> list[GridContent]:
-        ...
+    def __getitem__(self, index: int | Sequence[Coordinate]) -> list[GridContent]: ...
 
     @overload
     def __getitem__(
         self, index: tuple[int | slice, int | slice]
-    ) -> GridContent | list[GridContent]:
-        ...
+    ) -> GridContent | list[GridContent]: ...
 
     def __getitem__(self, index):
         """Access contents from the grid."""
 
         if isinstance(index, int):
             # grid[x]
             return self._grid[index]
@@ -401,19 +414,17 @@
             cell_list: Array-like of (x, y) tuples, or single tuple.
 
         Returns:
             A list of the agents contained in the cells identified in `cell_list`.
         """
         return list(self.iter_cell_list_contents(cell_list))
 
-    def place_agent(self, agent: Agent, pos: Coordinate) -> None:
-        ...
+    def place_agent(self, agent: Agent, pos: Coordinate) -> None: ...
 
-    def remove_agent(self, agent: Agent) -> None:
-        ...
+    def remove_agent(self, agent: Agent) -> None: ...
 
     def move_agent(self, agent: Agent, pos: Coordinate) -> None:
         """Move an agent from its current position to a new position.
 
         Args:
             agent: Agent object to move. Assumed to have its current location
                    stored in a 'pos' tuple.
@@ -759,24 +770,22 @@
     The `_PropertyGrid` extends the capabilities of a basic grid by allowing each cell
     to have multiple properties, each represented by a separate PropertyLayer.
     These properties can be used to model complex environments where each cell
     has multiple attributes or states.
 
     Attributes:
         properties (dict): A dictionary mapping property layer names to PropertyLayer instances.
-        empty_mask: Returns a boolean mask indicating empty cells on the grid.
+        empty_mask (np.ndarray): A boolean array indicating empty cells on the grid.
 
     Methods:
         add_property_layer(property_layer): Adds a new property layer to the grid.
         remove_property_layer(property_name): Removes a property layer from the grid by its name.
         get_neighborhood_mask(pos, moore, include_center, radius): Generates a boolean mask of the neighborhood.
-        select_cells_by_properties(conditions, mask, return_list): Selects cells based on multiple property conditions,
-            optionally with a mask, returning either a list of coordinates or a mask.
-        select_extreme_value_cells(property_name, mode, mask, return_list): Selects cells with extreme values of a property,
-            optionally with a mask, returning either a list of coordinates or a mask.
+        select_cells(conditions, extreme_values, masks, only_empty, return_list): Selects cells based on multiple conditions,
+            extreme values, masks, with an option to select only empty cells, returning either a list of coordinates or a mask.
 
     Mask Usage:
         Several methods in this class accept a mask as an input, which is a NumPy ndarray of boolean values. This mask
         specifies the cells to be considered (True) or ignored (False) in operations. Users can create custom masks,
         including neighborhood masks, to apply specific conditions or constraints. Additionally, methods that deal with
         cell selection or agent movement can return either a list of cell coordinates or a mask, based on the 'return_list'
         parameter. This flexibility allows for more nuanced control and customization of grid operations, catering to a wide
@@ -974,14 +983,15 @@
         width, height: The grid's width and height.
         torus: Boolean which determines whether to treat the grid as a torus.
         empties: Returns a set of (x, y) tuples for all empty cells. This set is
                  maintained internally and provides a performant way to query
                  the grid for empty spaces.
     """
 
+    @warn_if_agent_has_position_already
     def place_agent(self, agent: Agent, pos: Coordinate) -> None:
         """Place the agent at the specified location, and set its pos variable."""
         if self.is_cell_empty(pos):
             x, y = pos
             self._grid[x][y] = agent
             if self._empties_built:
                 self._empties.discard(pos)
@@ -1022,14 +1032,15 @@
     grid: list[list[MultiGridContent]]
 
     @staticmethod
     def default_val() -> MultiGridContent:
         """Default value for new cell elements."""
         return []
 
+    @warn_if_agent_has_position_already
     def place_agent(self, agent: Agent, pos: Coordinate) -> None:
         """Place the agent at the specified location, and set its pos variable."""
         x, y = pos
         if agent.pos is None or agent not in self._grid[x][y]:
             self._grid[x][y].append(agent)
             agent.pos = pos
             if self._empties_built:
@@ -1353,14 +1364,15 @@
         self._agent_points = np.array([agent.pos for agent in self._agent_to_index])
 
     def _invalidate_agent_cache(self):
         """Clear cached data of agents and positions in the space."""
         self._agent_points = None
         self._index_to_agent = {}
 
+    @warn_if_agent_has_position_already
     def place_agent(self, agent: Agent, pos: FloatCoordinate) -> None:
         """Place a new agent in the space.
 
         Args:
             agent: Agent object to place.
             pos: Coordinate tuple for where to place the agent.
         """
@@ -1513,14 +1525,15 @@
             g.nodes[node_id]["agent"] = self.default_val()
 
     @staticmethod
     def default_val() -> list:
         """Default value for a new node."""
         return []
 
+    @warn_if_agent_has_position_already
     def place_agent(self, agent: Agent, node_id: int) -> None:
         """Place an agent in a node."""
         self.G.nodes[node_id]["agent"].append(agent)
         agent.pos = node_id
 
     def get_neighborhood(
         self, node_id: int, include_center: bool = False, radius: int = 1
```

### Comparing `mesa-2.3.0.dev0/mesa/time.py` & `mesa-2.3.0rc1/mesa/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     model has taken.
 """
 
 # Mypy; for the `|` operator purpose
 # Remove this __future__ import once the oldest supported Python is 3.10
 from __future__ import annotations
 
-import heapq
 import warnings
-import weakref
 from collections import defaultdict
 from collections.abc import Iterable
 
 # mypy
 from typing import Union
 
 from mesa.agent import Agent, AgentSet
@@ -389,127 +387,22 @@
         Returns the current number of agents of certain type in the queue.
         """
         return len(self._agents_by_type[agenttype])
 
 
 class DiscreteEventScheduler(BaseScheduler):
     """
-    A scheduler for discrete event simulation in Mesa.
-
-    This scheduler manages events where each event is associated with a
-    specific time and agent. The scheduler advances time not in fixed
-    increments, but to the moment the next event is scheduled to occur.
-
-    This implementation uses a priority queue (heapq) to manage events. Each
-    event is a tuple of the form (time, random_value, agent), where:
-        - time (float): The scheduled time for the event.
-        - random_value (float): A secondary sorting criterion to randomize
-          the order of events that are scheduled for the same time.
-        - agent (Agent): The agent associated with the event.
-
-    The random value for secondary sorting ensures that when two events are
-    scheduled for the same time, their execution order is randomized, thus
-    preventing direct comparison issues between different types of agents and
-    maintaining the integrity of the simulation's randomness.
-
-    Attributes:
-        model (Model): The model instance associated with the scheduler.
-        event_queue (list): A priority queue of scheduled events.
-        time_step (int or float): The fixed time period by which the model advances
-                                  on each step. Defaults to 1.
-
-    Methods:
-        schedule_event(time, agent): Schedule an event for a specific time.
-        schedule_in(delay, agent): Schedule an event after a specified delay.
-        step(): Execute all events within the next time_step period.
-        get_next_event_time(): Returns the time of the next scheduled event.
-
-    Usage:
-        1. Instantiate the DiscreteEventScheduler with a model instance and a time_step period.
-        2. Add agents to the scheduler using schedule.add(). With schedule_now=True (default),
-              the first event for the agent will be scheduled immediately.
-        3. In the Agent step() method, schedule the next event for the agent
-              (using schedule_in or schedule_event).
-        3. Add self.schedule.step() to the model's step() method, as usual.
-
-    Now, with each model step, the scheduler will execute all events within the
-    next time_step period, and advance time one time_step forward.
+    This class has been deprecated and replaced by the functionality provided by experimental.devs
     """
 
     def __init__(self, model: Model, time_step: TimeT = 1) -> None:
         """
 
         Args:
             model (Model): The model to which the schedule belongs
             time_step (TimeT): The fixed time step between steps
 
         """
         super().__init__(model)
-        self.event_queue: list[tuple[TimeT, float, weakref.ref]] = []
-        self.time_step: TimeT = time_step  # Fixed time period for each step
-
-        warnings.warn(
-            "The DiscreteEventScheduler is experimental. It may be changed or removed in any and all future releases, including patch releases.\n"
-            "We would love to hear what you think about this new feature. If you have any thoughts, share them with us here: https://github.com/projectmesa/mesa/discussions/1923",
-            FutureWarning,
-            stacklevel=2,
+        raise Exception(
+            "DiscreteEventScheduler is deprecated in favor of the functionality provided by experimental.devs"
         )
-
-    def schedule_event(self, time: TimeT, agent: Agent) -> None:
-        """Schedule an event for an agent at a specific time."""
-        if time < self.time:
-            raise ValueError(
-                f"Scheduled time ({time}) must be >= the current time ({self.time})"
-            )
-        if agent not in self._agents:
-            raise ValueError(
-                "trying to schedule an event for agent which is not known to the scheduler"
-            )
-
-        # Create an event, sorted first on time, secondary on a random value
-        event = (time, self.model.random.random(), weakref.ref(agent))
-        heapq.heappush(self.event_queue, event)
-
-    def schedule_in(self, delay: TimeT, agent: Agent) -> None:
-        """Schedule an event for an agent after a specified delay."""
-        if delay < 0:
-            raise ValueError("Delay must be non-negative")
-        event_time = self.time + delay
-        self.schedule_event(event_time, agent)
-
-    def step(self) -> None:
-        """Execute the next event and advance the time."""
-        end_time = self.time + self.time_step
-
-        while self.event_queue and self.event_queue[0][0] <= end_time:
-            # Get the next event (ignore the random value during unpacking)
-            time, _, agent = heapq.heappop(self.event_queue)
-            agent = agent()  # unpack weakref
-
-            if agent:
-                # Advance time to the event's time
-                self.time = time
-                # Execute the event
-                agent.step()
-
-        # After processing events, advance time by the time_step
-        self.time = end_time
-        self.steps += 1
-
-    def get_next_event_time(self) -> TimeT | None:
-        """Returns the time of the next scheduled event."""
-        if not self.event_queue:
-            return None
-        return self.event_queue[0][0]
-
-    def add(self, agent: Agent, schedule_now: bool = True) -> None:
-        """Add an Agent object to the schedule and optionally schedule its first event.
-
-        Args:
-            agent: An Agent to be added to the schedule. Must have a step() method.
-            schedule_now: If True, schedules the first event for the agent immediately.
-        """
-        super().add(agent)  # Call the add method from BaseScheduler
-
-        if schedule_now:
-            # Schedule the first event immediately
-            self.schedule_event(self.time, agent)
```

### Comparing `mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.pytemplate` & `mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.pytemplate`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.pytemplate` & `mesa-2.3.0rc1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.pytemplate`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/experimental/UserParam.py` & `mesa-2.3.0rc1/mesa/experimental/UserParam.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/mesa/experimental/jupyter_viz.py` & `mesa-2.3.0rc1/mesa/experimental/jupyter_viz.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,158 +13,179 @@
 # Avoid interactive backend
 plt.switch_backend("agg")
 
 
 # TODO: Turn this function into a Solara component once the current_step.value
 # dependency is passed to measure()
 def Card(
-    model, measures, agent_portrayal, space_drawer, current_step, color, layout_type
+    model, measures, agent_portrayal, space_drawer, dependencies, color, layout_type
 ):
     with rv.Card(
         style_=f"background-color: {color}; width: 100%; height: 100%"
     ) as main:
         if "Space" in layout_type:
             rv.CardTitle(children=["Space"])
             if space_drawer == "default":
                 # draw with the default implementation
                 components_matplotlib.SpaceMatplotlib(
-                    model, agent_portrayal, dependencies=[current_step.value]
+                    model, agent_portrayal, dependencies=dependencies
                 )
             elif space_drawer == "altair":
                 components_altair.SpaceAltair(
-                    model, agent_portrayal, dependencies=[current_step.value]
+                    model, agent_portrayal, dependencies=dependencies
                 )
             elif space_drawer:
                 # if specified, draw agent space with an alternate renderer
                 space_drawer(model, agent_portrayal)
         elif "Measure" in layout_type:
             rv.CardTitle(children=["Measure"])
             measure = measures[layout_type["Measure"]]
             if callable(measure):
                 # Is a custom object
                 measure(model)
             else:
                 components_matplotlib.PlotMatplotlib(
-                    model, measure, dependencies=[current_step.value]
+                    model, measure, dependencies=dependencies
                 )
     return main
 
 
 @solara.component
 def JupyterViz(
     model_class,
     model_params,
     measures=None,
     name=None,
     agent_portrayal=None,
     space_drawer="default",
     play_interval=150,
+    seed=None,
 ):
     """Initialize a component to visualize a model.
     Args:
         model_class: class of the model to instantiate
         model_params: parameters for initializing the model
         measures: list of callables or data attributes to plot
         name: name for display
         agent_portrayal: options for rendering agents (dictionary)
         space_drawer: method to render the agent space for
             the model; default implementation is the `SpaceMatplotlib` component;
             simulations with no space to visualize should
             specify `space_drawer=False`
         play_interval: play interval (default: 150)
+        seed: the random seed used to initialize the model
     """
     if name is None:
         name = model_class.__name__
 
     current_step = solara.use_reactive(0)
 
     # 1. Set up model parameters
+    reactive_seed = solara.use_reactive(0)
     user_params, fixed_params = split_model_params(model_params)
     model_parameters, set_model_parameters = solara.use_state(
         {**fixed_params, **{k: v.get("value") for k, v in user_params.items()}}
     )
 
     # 2. Set up Model
     def make_model():
-        model = model_class(**model_parameters)
+        model = model_class.__new__(
+            model_class, **model_parameters, seed=reactive_seed.value
+        )
+        model.__init__(**model_parameters)
         current_step.value = 0
         return model
 
     reset_counter = solara.use_reactive(0)
     model = solara.use_memo(
-        make_model, dependencies=[*list(model_parameters.values()), reset_counter.value]
+        make_model,
+        dependencies=[
+            *list(model_parameters.values()),
+            reset_counter.value,
+            reactive_seed.value,
+        ],
     )
 
     def handle_change_model_params(name: str, value: any):
         set_model_parameters({**model_parameters, name: value})
 
     # 3. Set up UI
 
     with solara.AppBar():
         solara.AppBarTitle(name)
 
     # render layout and plot
+    def do_reseed():
+        reactive_seed.value = model.random.random()
 
     # jupyter
+    dependencies = [current_step.value, reactive_seed.value]
+
     def render_in_jupyter():
         with solara.GridFixed(columns=2):
             UserInputs(user_params, on_change=handle_change_model_params)
             ModelController(model, play_interval, current_step, reset_counter)
             solara.Markdown(md_text=f"###Step - {current_step}")
 
         with solara.GridFixed(columns=2):
             # 4. Space
             if space_drawer == "default":
                 # draw with the default implementation
                 components_matplotlib.SpaceMatplotlib(
-                    model, agent_portrayal, dependencies=[current_step.value]
+                    model, agent_portrayal, dependencies=dependencies
                 )
             elif space_drawer == "altair":
                 components_altair.SpaceAltair(
-                    model, agent_portrayal, dependencies=[current_step.value]
+                    model, agent_portrayal, dependencies=dependencies
                 )
             elif space_drawer:
                 # if specified, draw agent space with an alternate renderer
                 space_drawer(model, agent_portrayal)
             # otherwise, do nothing (do not draw space)
 
             # 5. Plots
             for measure in measures:
                 if callable(measure):
                     # Is a custom object
                     measure(model)
                 else:
                     components_matplotlib.PlotMatplotlib(
-                        model, measure, dependencies=[current_step.value]
+                        model, measure, dependencies=dependencies
                     )
 
     def render_in_browser():
         # if space drawer is disabled, do not include it
         layout_types = [{"Space": "default"}] if space_drawer else []
 
         if measures:
             layout_types += [{"Measure": elem} for elem in range(len(measures))]
 
-        grid_layout_initial = get_initial_grid_layout(layout_types=layout_types)
+        grid_layout_initial = make_initial_grid_layout(layout_types=layout_types)
         grid_layout, set_grid_layout = solara.use_state(grid_layout_initial)
 
         with solara.Sidebar():
             with solara.Card("Controls", margin=1, elevation=2):
+                solara.InputText(
+                    label="Seed",
+                    value=reactive_seed,
+                    continuous_update=True,
+                )
                 UserInputs(user_params, on_change=handle_change_model_params)
                 ModelController(model, play_interval, current_step, reset_counter)
-            with solara.Card("Progress", margin=1, elevation=2):
-                solara.Markdown(md_text=f"####Step - {current_step}")
+                solara.Button(label="Reseed", color="primary", on_click=do_reseed)
+            with solara.Card("Information", margin=1, elevation=2):
+                solara.Markdown(md_text=f"Step - {current_step}")
 
         items = [
             Card(
                 model,
                 measures,
                 agent_portrayal,
                 space_drawer,
-                current_step,
+                dependencies,
                 color="white",
                 layout_type=layout_types[i],
             )
             for i in range(len(layout_types))
         ]
         solara.GridDraggable(
             items=items,
@@ -237,15 +258,19 @@
     with solara.Row():
         solara.Button(label="Step", color="primary", on_click=do_step)
         # This style is necessary so that the play widget has almost the same
         # height as typical Solara buttons.
         solara.Style(
             """
         .widget-play {
-            height: 30px;
+            height: 35px;
+        }
+        .widget-play button {
+            color: white;
+            background-color: #1976D2;  // Solara blue color
         }
         """
         )
         widgets.Play(
             value=0,
             interval=play_interval,
             repeat=True,
@@ -357,24 +382,19 @@
 def make_text(renderer):
     def function(model):
         solara.Markdown(renderer(model))
 
     return function
 
 
-def get_initial_grid_layout(layout_types):
-    grid_lay = []
-    y_coord = 0
-    for ii in range(len(layout_types)):
-        template_layout = {"h": 10, "i": 0, "moved": False, "w": 6, "y": 0, "x": 0}
-        if ii == 0:
-            grid_lay.append(template_layout)
-        else:
-            template_layout.update({"i": ii})
-            if ii % 2 == 0:
-                template_layout.update({"x": 0})
-                y_coord += 16
-            else:
-                template_layout.update({"x": 6})
-            template_layout.update({"y": y_coord})
-            grid_lay.append(template_layout)
-    return grid_lay
+def make_initial_grid_layout(layout_types):
+    return [
+        {
+            "i": i,
+            "w": 6,
+            "h": 10,
+            "moved": False,
+            "x": 6 * (i % 2),
+            "y": 16 * (i - i % 2),
+        }
+        for i in range(len(layout_types))
+    ]
```

### Comparing `mesa-2.3.0.dev0/mesa/experimental/components/altair.py` & `mesa-2.3.0rc1/mesa/experimental/components/altair.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,41 @@
     chart = _draw_grid(space, agent_portrayal)
     solara.FigureAltair(chart)
 
 
 def _draw_grid(space, agent_portrayal):
     def portray(g):
         all_agent_data = []
-        for content, (x, y) in space.coord_iter():
+        for content, (x, y) in g.coord_iter():
             if not content:
                 continue
             if not hasattr(content, "__iter__"):
                 # Is a single grid
                 content = [content]  # noqa: PLW2901
             for agent in content:
                 # use all data from agent portrayal, and add x,y coordinates
                 agent_data = agent_portrayal(agent)
                 agent_data["x"] = x
                 agent_data["y"] = y
                 all_agent_data.append(agent_data)
         return all_agent_data
 
     all_agent_data = portray(space)
+    invalid_tooltips = ["color", "size", "x", "y"]
+
     encoding_dict = {
         # no x-axis label
         "x": alt.X("x", axis=None, type="ordinal"),
         # no y-axis label
         "y": alt.Y("y", axis=None, type="ordinal"),
+        "tooltip": [
+            alt.Tooltip(key, type=alt.utils.infer_vegalite_type([value]))
+            for key, value in all_agent_data[0].items()
+            if key not in invalid_tooltips
+        ],
     }
     has_color = "color" in all_agent_data[0]
     if has_color:
         encoding_dict["color"] = alt.Color("color", type="nominal")
     has_size = "size" in all_agent_data[0]
     if has_size:
         encoding_dict["size"] = alt.Size("size", type="quantitative")
@@ -52,9 +59,14 @@
         alt.Chart(
             alt.Data(values=all_agent_data), encoding=alt.Encoding(**encoding_dict)
         )
         .mark_point(filled=True)
         .properties(width=280, height=280)
         # .configure_view(strokeOpacity=0)  # hide grid/chart lines
     )
+    # This is the default value for the marker size, which auto-scales
+    # according to the grid area.
+    if not has_size:
+        length = min(space.width, space.height)
+        chart = chart.mark_point(size=30000 / length**2, filled=True)
 
     return chart
```

### Comparing `mesa-2.3.0.dev0/mesa/experimental/components/matplotlib.py` & `mesa-2.3.0rc1/mesa/experimental/components/matplotlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
                     x.append(i)
                     y.append(j)
                     if "size" in data:
                         s.append(data["size"])
                     if "color" in data:
                         c.append(data["color"])
         out = {"x": x, "y": y}
+        # This is the default value for the marker size, which auto-scales
+        # according to the grid area.
+        out["s"] = (180 / min(g.width, g.height)) ** 2
         if len(s) > 0:
             out["s"] = s
         if len(c) > 0:
             out["c"] = c
         return out
 
     space_ax.set_xlim(-1, space.width)
```

### Comparing `mesa-2.3.0.dev0/tests/test_agent.py` & `mesa-2.3.0rc1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_batch_run.py` & `mesa-2.3.0rc1/tests/test_batch_run.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_datacollector.py` & `mesa-2.3.0rc1/tests/test_datacollector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the DataCollector
 """
+
 import unittest
 
 from mesa import Agent, Model
 from mesa.time import BaseScheduler
 
 
 class MockAgent(Agent):
```

### Comparing `mesa-2.3.0.dev0/tests/test_examples.py` & `mesa-2.3.0rc1/tests/test_examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,20 @@
             if hasattr(self, f"test_{example.replace('-', '_')}"):
                 # non-standard example; tested below
                 continue
 
             print(f"testing example {example!r}")
             with self.active_example_dir(example):
                 try:
-                    # model.py at the top level
+                    # epstein_civil_violence.py at the top level
                     mod = importlib.import_module("model")
                     server = importlib.import_module("server")
                     server.server.render_model()
                 except ImportError:
-                    # <example>/model.py
+                    # <example>/epstein_civil_violence.py
                     mod = importlib.import_module(f"{example.replace('-', '_')}.model")
                     server = importlib.import_module(
                         f"{example.replace('-', '_')}.server"
                     )
                     server.server.render_model()
                 model_class = getattr(mod, classcase(example))
                 model = model_class()
```

### Comparing `mesa-2.3.0.dev0/tests/test_grid.py` & `mesa-2.3.0rc1/tests/test_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the Grid objects.
 """
+
 import random
 import unittest
 from unittest.mock import Mock, patch
 
 from mesa.space import HexSingleGrid, MultiGrid, SingleGrid
 
 # Initial agent positions for testing
@@ -20,18 +21,18 @@
 
 
 class MockAgent:
     """
     Minimalistic agent for testing purposes.
     """
 
-    def __init__(self, unique_id, pos):
+    def __init__(self, unique_id):
         self.random = random.Random(0)
         self.unique_id = unique_id
-        self.pos = pos
+        self.pos = None
 
 
 class TestSingleGrid(unittest.TestCase):
     """
     Testing a non-toroidal singlegrid.
     """
 
@@ -49,15 +50,15 @@
         counter = 0
         for x in range(width):
             for y in range(height):
                 if TEST_GRID[x][y] == 0:
                     continue
                 counter += 1
                 # Create and place the mock agent
-                a = MockAgent(counter, None)
+                a = MockAgent(counter)
                 self.agents.append(a)
                 self.grid.place_agent(a, (x, y))
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
@@ -254,27 +255,27 @@
         counter = 0
         for x in range(width):
             for y in range(height):
                 if TEST_GRID[x][y] == 0:
                     continue
                 counter += 1
                 # Create and place the mock agent
-                a = MockAgent(counter, None)
+                a = MockAgent(counter)
                 self.agents.append(a)
                 self.grid.place_agent(a, (x, y))
         self.num_agents = len(self.agents)
 
     @patch.object(MockAgent, "model", create=True)
     def test_enforcement(self, mock_model):
         """
         Test the SingleGrid empty count and enforcement.
         """
 
         assert len(self.grid.empties) == 9
-        a = MockAgent(100, None)
+        a = MockAgent(100)
         with self.assertRaises(Exception):
             self.grid.place_agent(a, (0, 1))
 
         # Place the agent in an empty cell
         mock_model.schedule.get_agent_count = Mock(side_effect=lambda: len(self.agents))
         self.grid.move_to_empty(a)
         self.num_agents += 1
@@ -284,20 +285,20 @@
         for _i in range(10):
             self.grid.move_to_empty(a)
         assert len(self.grid.empties) == 8
 
         # Place agents until the grid is full
         empty_cells = len(self.grid.empties)
         for i in range(empty_cells):
-            a = MockAgent(101 + i, None)
+            a = MockAgent(101 + i)
             self.grid.move_to_empty(a)
             self.num_agents += 1
         assert len(self.grid.empties) == 0
 
-        a = MockAgent(110, None)
+        a = MockAgent(110)
         with self.assertRaises(Exception):
             self.grid.move_to_empty(a)
         with self.assertRaises(Exception):
             self.move_to_empty(self.agents[0])
 
 
 # Number of agents at each position for testing
@@ -330,15 +331,15 @@
         self.agents = []
         counter = 0
         for x in range(width):
             for y in range(height):
                 for _i in range(TEST_MULTIGRID[x][y]):
                     counter += 1
                     # Create and place the mock agent
-                    a = MockAgent(counter, None)
+                    a = MockAgent(counter)
                     self.agents.append(a)
                     self.grid.place_agent(a, (x, y))
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly on the MultiGrid.
         """
@@ -389,15 +390,15 @@
         counter = 0
         for x in range(width):
             for y in range(height):
                 if TEST_GRID[x][y] == 0:
                     continue
                 counter += 1
                 # Create and place the mock agent
-                a = MockAgent(counter, None)
+                a = MockAgent(counter)
                 self.agents.append(a)
                 self.grid.place_agent(a, (x, y))
 
     def test_neighbors(self):
         """
         Test the hexagonal neighborhood methods on the non-toroid.
         """
@@ -443,15 +444,15 @@
         counter = 0
         for x in range(width):
             for y in range(height):
                 if TEST_GRID[x][y] == 0:
                     continue
                 counter += 1
                 # Create and place the mock agent
-                a = MockAgent(counter, None)
+                a = MockAgent(counter)
                 self.agents.append(a)
                 self.grid.place_agent(a, (x, y))
 
     def test_neighbors(self):
         """
         Test the hexagonal neighborhood methods on the toroid.
         """
```

### Comparing `mesa-2.3.0.dev0/tests/test_import_namespace.py` & `mesa-2.3.0rc1/tests/test_import_namespace.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_jupyter_viz.py` & `mesa-2.3.0rc1/tests/test_jupyter_viz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
-from unittest.mock import Mock, patch
+from unittest.mock import Mock
 
 import ipyvuetify as vw
 import solara
 
+import mesa
 from mesa.experimental.jupyter_viz import JupyterViz, Slider, UserInputs
 
 
 class TestMakeUserInput(unittest.TestCase):
     def test_unsupported_type(self):
         @solara.component
         def Test(user_params):
@@ -77,66 +78,69 @@
         assert slider_int.v_model == options["value"]
         assert slider_int.label == "num_agents"
         assert slider_int.min is None
         assert slider_int.max is None
         assert slider_int.step is None
 
 
-class TestJupyterViz(unittest.TestCase):
-    @patch("mesa.experimental.components.matplotlib.SpaceMatplotlib")
-    def test_call_space_drawer(self, mock_space_matplotlib):
-        mock_model_class = Mock()
-        mock_model_class.__name__ = "MockModelClass"
-        agent_portrayal = {
-            "Shape": "circle",
-            "color": "gray",
-        }
-        current_step = 0
-        dependencies = [current_step]
-        # initialize with space drawer unspecified (use default)
-        # component must be rendered for code to run
+def test_call_space_drawer(mocker):
+    mock_space_matplotlib = mocker.patch(
+        "mesa.experimental.components.matplotlib.SpaceMatplotlib"
+    )
+
+    model = mesa.Model()
+    mocker.patch.object(mesa.Model, "__new__", return_value=model)
+    mocker.patch.object(mesa.Model, "__init__", return_value=None)
+
+    agent_portrayal = {
+        "Shape": "circle",
+        "color": "gray",
+    }
+    current_step = 0
+    seed = 0
+    dependencies = [current_step, seed]
+    # initialize with space drawer unspecified (use default)
+    # component must be rendered for code to run
+    solara.render(
+        JupyterViz(
+            model_class=mesa.Model,
+            model_params={},
+            agent_portrayal=agent_portrayal,
+        )
+    )
+    # should call default method with class instance and agent portrayal
+    mock_space_matplotlib.assert_called_with(
+        model, agent_portrayal, dependencies=dependencies
+    )
+
+    # specify no space should be drawn; any false value should work
+    for falsy_value in [None, False, 0]:
+        mock_space_matplotlib.reset_mock()
         solara.render(
             JupyterViz(
-                model_class=mock_model_class,
+                model_class=mesa.Model,
                 model_params={},
                 agent_portrayal=agent_portrayal,
+                space_drawer=falsy_value,
             )
         )
         # should call default method with class instance and agent portrayal
-        mock_space_matplotlib.assert_called_with(
-            mock_model_class.return_value, agent_portrayal, dependencies=dependencies
-        )
+        assert mock_space_matplotlib.call_count == 0
 
-        # specify no space should be drawn; any false value should work
-        for falsy_value in [None, False, 0]:
-            mock_space_matplotlib.reset_mock()
-            solara.render(
-                JupyterViz(
-                    model_class=mock_model_class,
-                    model_params={},
-                    agent_portrayal=agent_portrayal,
-                    space_drawer=falsy_value,
-                )
-            )
-            # should call default method with class instance and agent portrayal
-            assert mock_space_matplotlib.call_count == 0
-
-        # specify a custom space method
-        altspace_drawer = Mock()
-        solara.render(
-            JupyterViz(
-                model_class=mock_model_class,
-                model_params={},
-                agent_portrayal=agent_portrayal,
-                space_drawer=altspace_drawer,
-            )
-        )
-        altspace_drawer.assert_called_with(
-            mock_model_class.return_value, agent_portrayal
+    # specify a custom space method
+    altspace_drawer = Mock()
+    solara.render(
+        JupyterViz(
+            model_class=mesa.Model,
+            model_params={},
+            agent_portrayal=agent_portrayal,
+            space_drawer=altspace_drawer,
         )
+    )
+    altspace_drawer.assert_called_with(model, agent_portrayal)
 
 
 def test_slider():
     slider_float = Slider("Agent density", 0.8, 0.1, 1.0, 0.1)
     assert slider_float.is_float_slider
     assert slider_float.value == 0.8
     assert slider_float.get("value") == 0.8
```

### Comparing `mesa-2.3.0.dev0/tests/test_main.py` & `mesa-2.3.0rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_model.py` & `mesa-2.3.0rc1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_scaffold.py` & `mesa-2.3.0rc1/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_space.py` & `mesa-2.3.0rc1/tests/test_space.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def test_agents_add_many(self):
         """
         Add many agents
         """
         positions = np.random.rand(TEST_AGENTS_PERF, 2)
         for i in range(TEST_AGENTS_PERF):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             pos = [positions[i, 0], positions[i, 1]]
             self.space.place_agent(a, pos)
 
 
 class TestSpaceToroidal(unittest.TestCase):
     """
     Testing a toroidal continuous space.
@@ -55,15 +55,15 @@
     def setUp(self):
         """
         Create a test space and populate with Mock Agents.
         """
         self.space = ContinuousSpace(70, 20, True, -30, -30)
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
@@ -122,15 +122,15 @@
 
     def test_bounds(self):
         """
         Test positions outside of boundary
         """
         boundary_agents = []
         for i, pos in enumerate(OUTSIDE_POSITIONS):
-            a = MockAgent(len(self.agents) + i, None)
+            a = MockAgent(len(self.agents) + i)
             boundary_agents.append(a)
             self.space.place_agent(a, pos)
 
         for a, pos in zip(boundary_agents, OUTSIDE_POSITIONS):
             adj_pos = self.space.torus_adj(pos)
             assert a.pos == adj_pos
 
@@ -148,15 +148,15 @@
     def setUp(self):
         """
         Create a test space and populate with Mock Agents.
         """
         self.space = ContinuousSpace(70, 20, False, -30, -30)
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
@@ -204,15 +204,15 @@
         assert len(neighbors_3) == 0
 
     def test_bounds(self):
         """
         Test positions outside of boundary
         """
         for i, pos in enumerate(OUTSIDE_POSITIONS):
-            a = MockAgent(len(self.agents) + i, None)
+            a = MockAgent(len(self.agents) + i)
             with self.assertRaises(Exception):
                 self.space.place_agent(a, pos)
 
         a = self.agents[0]
         for pos in OUTSIDE_POSITIONS:
             assert self.space.out_of_bounds(pos)
             with self.assertRaises(Exception):
@@ -227,15 +227,15 @@
     def setUp(self):
         """
         Create a test space and populate with Mock Agents.
         """
         self.space = ContinuousSpace(70, 50, False, -30, -30)
         self.agents = []
         for i, pos in enumerate(REMOVAL_TEST_AGENTS):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_remove_first(self):
         """
         Test removing the first entry
         """
@@ -438,15 +438,15 @@
 
 
 class TestSingleGrid(unittest.TestCase):
     def setUp(self):
         self.space = SingleGrid(50, 50, False)
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS_GRID):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
@@ -462,15 +462,15 @@
             self.space.remove_agent(a)
             assert a.pos is None
             assert self.space[pos[0]][pos[1]] is None
 
     def test_empty_cells(self):
         if self.space.exists_empty_cells():
             for i, pos in enumerate(list(self.space.empties)):
-                a = MockAgent(-i, pos)
+                a = MockAgent(-i)
                 self.space.place_agent(a, pos)
         with self.assertRaises(Exception):
             self.space.move_to_empty(a)
 
     def test_empty_mask_consistency(self):
         # Check that the empty mask is consistent with the empties set
         empty_mask = self.space.empty_mask
@@ -547,15 +547,15 @@
 
 
 class TestSingleGridTorus(unittest.TestCase):
     def setUp(self):
         self.space = SingleGrid(50, 50, True)  # Torus is True here
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS_GRID):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_move_agent_random_selection(self):
         agent = self.agents[0]
         possible_positions = [(49, 49), (1, 1), (25, 25)]
         self.space.move_agent_to_one_of(agent, possible_positions, selection="random")
@@ -639,26 +639,26 @@
 
     # Test getting masks
     def test_get_empty_mask(self):
         empty_mask = self.grid.empty_mask
         self.assertTrue(np.all(empty_mask == np.ones((10, 10), dtype=bool)))
 
     def test_get_empty_mask_with_agent(self):
-        agent = MockAgent(0, self.grid)
+        agent = MockAgent(0)
         self.grid.place_agent(agent, (4, 6))
 
         empty_mask = self.grid.empty_mask
         expected_mask = np.ones((10, 10), dtype=bool)
         expected_mask[4, 6] = False
 
         self.assertTrue(np.all(empty_mask == expected_mask))
 
     def test_get_neighborhood_mask(self):
-        agent = MockAgent(0, self.grid)
-        agent2 = MockAgent(1, self.grid)
+        agent = MockAgent(0)
+        agent2 = MockAgent(1)
         self.grid.place_agent(agent, (5, 5))
         self.grid.place_agent(agent2, (5, 6))
         neighborhood_mask = self.grid.get_neighborhood_mask((5, 5), True, False, 1)
         expected_mask = np.zeros((10, 10), dtype=bool)
         expected_mask[4:7, 4:7] = True
         expected_mask[5, 5] = False
         self.assertTrue(np.all(neighborhood_mask == expected_mask))
@@ -676,24 +676,24 @@
             return x == 0
 
         selected_mask = self.grid.select_cells({"layer1": condition}, return_list=False)
         self.assertTrue(isinstance(selected_mask, np.ndarray))
         self.assertTrue(selected_mask.all())
 
     def test_move_agent_to_cell_by_properties(self):
-        agent = MockAgent(1, self.grid)
+        agent = MockAgent(1)
         self.grid.place_agent(agent, (5, 5))
         conditions = {"layer1": lambda x: x == 0}
         target_cells = self.grid.select_cells(conditions)
         self.grid.move_agent_to_one_of(agent, target_cells)
         # Agent should move, since none of the cells match the condition
         self.assertNotEqual(agent.pos, (5, 5))
 
     def test_move_agent_no_eligible_cells(self):
-        agent = MockAgent(3, self.grid)
+        agent = MockAgent(3)
         self.grid.place_agent(agent, (5, 5))
         conditions = {"layer1": lambda x: x != 0}
         target_cells = self.grid.select_cells(conditions)
         self.grid.move_agent_to_one_of(agent, target_cells)
         self.assertEqual(agent.pos, (5, 5))
 
     # Test selecting and moving to cells based on extreme values
@@ -707,25 +707,25 @@
         target_mask = self.grid.select_cells(
             extreme_values={"layer2": "highest"}, return_list=False
         )
         self.assertTrue(isinstance(target_mask, np.ndarray))
         self.assertTrue(target_mask[3, 1])
 
     def test_move_agent_to_extreme_value_cell(self):
-        agent = MockAgent(2, self.grid)
+        agent = MockAgent(2)
         self.grid.place_agent(agent, (5, 5))
         self.grid.properties["layer2"].set_cell((3, 1), 1.1)
         target_cells = self.grid.select_cells(extreme_values={"layer2": "highest"})
         self.grid.move_agent_to_one_of(agent, target_cells)
         self.assertEqual(agent.pos, (3, 1))
 
     # Test using masks
     def test_select_cells_by_properties_with_empty_mask(self):
         self.grid.place_agent(
-            MockAgent(0, self.grid), (5, 5)
+            MockAgent(0), (5, 5)
         )  # Placing an agent to ensure some cells are not empty
         empty_mask = self.grid.empty_mask
 
         def condition(x):
             return x == 0
 
         selected_cells = self.grid.select_cells({"layer1": condition}, masks=empty_mask)
@@ -751,29 +751,29 @@
             (6, 4),
             (6, 5),
             (6, 6),
         ]  # Cells in the neighborhood of (5, 5)
         self.assertCountEqual(selected_cells, expected_selection)
 
     def test_move_agent_to_cell_by_properties_with_empty_mask(self):
-        agent = MockAgent(1, self.grid)
+        agent = MockAgent(1)
         self.grid.place_agent(agent, (5, 5))
         self.grid.place_agent(
-            MockAgent(2, self.grid), (4, 5)
+            MockAgent(2), (4, 5)
         )  # Placing another agent to create a non-empty cell
         empty_mask = self.grid.empty_mask
         conditions = {"layer1": lambda x: x == 0}
         target_cells = self.grid.select_cells(conditions, masks=empty_mask)
         self.grid.move_agent_to_one_of(agent, target_cells)
         self.assertNotEqual(
             agent.pos, (4, 5)
         )  # Agent should not move to (4, 5) as it's not empty
 
     def test_move_agent_to_cell_by_properties_with_neighborhood_mask(self):
-        agent = MockAgent(1, self.grid)
+        agent = MockAgent(1)
         self.grid.place_agent(agent, (5, 5))
         neighborhood_mask = self.grid.get_neighborhood_mask((5, 5), True, False, 1)
         conditions = {"layer1": lambda x: x == 0}
         target_cells = self.grid.select_cells(conditions, masks=neighborhood_mask)
         self.grid.move_agent_to_one_of(agent, target_cells)
         self.assertIn(
             agent.pos, [(4, 4), (4, 5), (4, 6), (5, 4), (5, 6), (6, 4), (6, 5), (6, 6)]
@@ -785,15 +785,15 @@
             return x == 0
 
         with self.assertRaises(KeyError):
             self.grid.select_cells(conditions={"nonexistent_layer": condition})
 
     # Test if coordinates means the same between the grid and the property layer
     def test_property_layer_coordinates(self):
-        agent = MockAgent(0, self.grid)
+        agent = MockAgent(0)
         correct_pos = (1, 8)
         incorrect_pos = (8, 1)
         self.grid.place_agent(agent, correct_pos)
 
         # Simple check on layer 1: set by agent, check by layer
         self.grid.properties["layer1"].set_cell(agent.pos, 2)
         self.assertEqual(self.grid.properties["layer1"].data[agent.pos], 2)
@@ -807,22 +807,22 @@
         agent_grid_value = self.grid.properties["layer2"].data[agent.pos]
 
         self.assertEqual(correct_grid_value, agent_grid_value)
         self.assertNotEqual(incorrect_grid_value, agent_grid_value)
 
     # Test selecting cells with only_empty parameter
     def test_select_cells_only_empty(self):
-        self.grid.place_agent(MockAgent(0, self.grid), (5, 5))  # Occupying a cell
+        self.grid.place_agent(MockAgent(0), (5, 5))  # Occupying a cell
         selected_cells = self.grid.select_cells(only_empty=True)
         self.assertNotIn(
             (5, 5), selected_cells
         )  # The occupied cell should not be selected
 
     def test_select_cells_only_empty_with_conditions(self):
-        self.grid.place_agent(MockAgent(1, self.grid), (5, 5))
+        self.grid.place_agent(MockAgent(1), (5, 5))
         self.grid.properties["layer1"].set_cell((5, 5), 2)
         self.grid.properties["layer1"].set_cell((6, 6), 2)
 
         def condition(x):
             return x == 2
 
         selected_cells = self.grid.select_cells({"layer1": condition}, only_empty=True)
@@ -851,15 +851,15 @@
         """
         Create a test network grid and populate with Mock Agents.
         """
         G = nx.cycle_graph(TestSingleNetworkGrid.GRAPH_SIZE)  # noqa: N806
         self.space = NetworkGrid(G)
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS_NETWORK_SINGLE):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
@@ -964,15 +964,15 @@
         """
         Create a test network grid and populate with Mock Agents.
         """
         G = nx.complete_graph(TestMultipleNetworkGrid.GRAPH_SIZE)  # noqa: N806
         self.space = NetworkGrid(G)
         self.agents = []
         for i, pos in enumerate(TEST_AGENTS_NETWORK_MULTIPLE):
-            a = MockAgent(i, None)
+            a = MockAgent(i)
             self.agents.append(a)
             self.space.place_agent(a, pos)
 
     def test_agent_positions(self):
         """
         Ensure that the agents are all placed properly.
         """
```

### Comparing `mesa-2.3.0.dev0/tests/test_tornado.py` & `mesa-2.3.0rc1/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_usersettableparam.py` & `mesa-2.3.0rc1/tests/test_usersettableparam.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/tests/test_visualization.py` & `mesa-2.3.0rc1/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/.gitignore` & `mesa-2.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/LICENSE` & `mesa-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mesa-2.3.0.dev0/README.md` & `mesa-2.3.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -110,12 +110,12 @@
 If you run into an issue, please file a [ticket](https://github.com/projectmesa/mesa/issues) for us to discuss. If
 possible, follow up with a pull request.
 
 If you would like to add a feature, please reach out via [ticket](https://github.com/projectmesa/mesa/issues) or
 join a dev session (see [Mesa discussions](https://github.com/projectmesa/mesa/discussions)). A feature is most likely
 to be added if you build it!
 
-Don't forget to checkout the [Contributors guide](https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.rst).
+Don't forget to checkout the [Contributors guide](https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.md).
 
 ## Citing Mesa
 
 To cite Mesa in your publication, you can use the [CITATION.bib](https://github.com/projectmesa/mesa/blob/main/CITATION.bib).
```

### Comparing `mesa-2.3.0.dev0/pyproject.toml` & `mesa-2.3.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -46,27 +46,28 @@
   "solara",
   "tqdm",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-  "ruff~=0.1.1",  # Update periodically
+  "ruff~=0.1.1",   # Update periodically
   "coverage",
   "pytest >= 4.6",
   "pytest-cov",
   "sphinx",
+  "pytest-mock",
 ]
 docs = [
   "sphinx",
   "ipython",
   "pydata_sphinx_theme",
   "seaborn",
   "myst-nb",
-  "myst-parser",  # Markdown in Sphinx
+  "myst-parser",         # Markdown in Sphinx
 ]
 
 [project.urls]
 homepage = "https://github.com/projectmesa/mesa"
 repository = "https://github.com/projectmesa/mesa"
 
 [project.scripts]
@@ -76,57 +77,60 @@
 packages = ["mesa"]
 
 [tool.hatch.version]
 path = "mesa/__init__.py"
 
 [tool.ruff]
 # See https://github.com/charliermarsh/ruff#rules for error code definitions.
+# Hardcode to Python 3.9.
+# Reminder to update mesa-examples if the value below is changed.
+target-version = "py39"
+extend-exclude = ["docs", "build"]
+
+[tool.ruff.lint]
 select = [
-    # "ANN", # annotations TODO
-    "B", # bugbear
-    "C4", # comprehensions
-    "DTZ", # naive datetime
-    "E", # style errors
-    "F", # flakes
-    "I", # import sorting
-    "ISC", # string concatenation
-    "N", # naming
-    "PGH", # pygrep-hooks
-    "PIE", # miscellaneous
-    "PLC", # pylint convention
-    "PLE", # pylint error
-    # "PLR", # pylint refactor TODO
-    "PLW", # pylint warning
-    "Q", # quotes
-    "RUF", # Ruff
-    "S", # security
-    "SIM", # simplify
-    "T10", # debugger
-    "UP", # upgrade
-    "W", # style warnings
-    "YTT", # sys.version
+  # "ANN", # annotations TODO
+  "B",   # bugbear
+  "C4",  # comprehensions
+  "DTZ", # naive datetime
+  "E",   # style errors
+  "F",   # flakes
+  "I",   # import sorting
+  "ISC", # string concatenation
+  "N",   # naming
+  "PGH", # pygrep-hooks
+  "PIE", # miscellaneous
+  "PLC", # pylint convention
+  "PLE", # pylint error
+  # "PLR", # pylint refactor TODO
+  "PLW", # pylint warning
+  "Q",   # quotes
+  "RUF", # Ruff
+  "S",   # security
+  "SIM", # simplify
+  "T10", # debugger
+  "UP",  # upgrade
+  "W",   # style warnings
+  "YTT", # sys.version
 ]
 # Ignore list taken from https://github.com/psf/black/blob/master/.flake8
 # E203	Whitespace before ':'
 # E266	Too many leading '#' for block comment
 # E501	Line too long (82 > 79 characters)
 # W503	Line break occurred before a binary operator
 # But we don't specify them because ruff's Black already
 # checks for it.
 # See https://github.com/charliermarsh/ruff/issues/1842#issuecomment-1381210185
 extend-ignore = [
-    "E501",
-    "S101", # Use of `assert` detected
-    "B017", # `assertRaises(Exception)` should be considered evil TODO
-    "PGH004", # Use specific rule codes when using `noqa` TODO
-    "B905", # `zip()` without an explicit `strict=` parameter
-    "N802", # Function name should be lowercase
-    "N999",  # Invalid module name. We should revisit this in the future, TODO
-    "RUF012",  # Mutable class attributes should be annotated with `typing.ClassVar` TODO
-    "S310",  # Audit URL open for permitted schemes. Allowing use of `file:` or custom schemes is often unexpected.
-    "S603",  # `subprocess` call: check for execution of untrusted input
-    "ISC001",  # ruff format asks to disable this feature
+  "E501",
+  "S101",   # Use of `assert` detected
+  "B017",   # `assertRaises(Exception)` should be considered evil TODO
+  "PGH004", # Use specific rule codes when using `noqa` TODO
+  "B905",   # `zip()` without an explicit `strict=` parameter
+  "N802",   # Function name should be lowercase
+  "N999",   # Invalid module name. We should revisit this in the future, TODO
+  "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar` TODO
+  "S310",   # Audit URL open for permitted schemes. Allowing use of `file:` or custom schemes is often unexpected.
+  "S603",   # `subprocess` call: check for execution of untrusted input
+  "ISC001", # ruff format asks to disable this feature
+  "S311",   # Standard pseudo-random generators are not suitable for cryptographic purposes
 ]
-extend-exclude = ["docs", "build"]
-# Hardcode to Python 3.9.
-# Reminder to update mesa-examples if the value below is changed.
-target-version = "py39"
```

### Comparing `mesa-2.3.0.dev0/PKG-INFO` & `mesa-2.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: Mesa
-Version: 2.3.0.dev0
+Version: 2.3.0rc1
 Summary: Agent-based modeling (ABM) in Python
 Project-URL: homepage, https://github.com/projectmesa/mesa
 Project-URL: repository, https://github.com/projectmesa/mesa
 Author-email: Project Mesa Team <projectmesa@googlegroups.com>
 License: Apache 2.0
 License-File: LICENSE
 Keywords: ABM,agent,based,model,modeling,multi-agent,simulation
@@ -30,14 +30,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: solara
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest>=4.6; extra == 'dev'
 Requires-Dist: ruff~=0.1.1; extra == 'dev'
 Requires-Dist: sphinx; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
@@ -158,12 +159,12 @@
 If you run into an issue, please file a [ticket](https://github.com/projectmesa/mesa/issues) for us to discuss. If
 possible, follow up with a pull request.
 
 If you would like to add a feature, please reach out via [ticket](https://github.com/projectmesa/mesa/issues) or
 join a dev session (see [Mesa discussions](https://github.com/projectmesa/mesa/discussions)). A feature is most likely
 to be added if you build it!
 
-Don't forget to checkout the [Contributors guide](https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.rst).
+Don't forget to checkout the [Contributors guide](https://github.com/projectmesa/mesa/blob/main/CONTRIBUTING.md).
 
 ## Citing Mesa
 
 To cite Mesa in your publication, you can use the [CITATION.bib](https://github.com/projectmesa/mesa/blob/main/CITATION.bib).
```

