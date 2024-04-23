# Comparing `tmp/bygg-0.3.2.tar.gz` & `tmp/bygg-0.4.0.tar.gz`

## Comparing `bygg-0.3.2.tar` & `bygg-0.4.0.tar`

### file list

```diff
@@ -1,84 +1,86 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bygg-0.3.2/.tool-versions
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bygg-0.3.2/Vagrantfile
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.3.2/Vagrantsetup.sh
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bygg-0.3.2/_version.py
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.3.2/bootstrap.py
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 bygg-0.3.2/mypy.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 bygg-0.3.2/noxfile.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 bygg-0.3.2/requirements-dev.in
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 bygg-0.3.2/requirements-dev.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.3.2/requirements.in
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 bygg-0.3.2/requirements.txt
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 bygg-0.3.2/.github/workflows/code_quality.yml
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.3.2/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.3.2/.vscode/extensions.json
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 bygg-0.3.2/.vscode/launch.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bygg-0.3.2/.vscode/settings.json
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/checks/Byggfile.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/.gitignore
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/Byggfile.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/Byggfile.yml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/Byggfile1.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/Byggfile2.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/requirements.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/requirements1.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/environments/requirements2.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/failing_jobs/Byggfile.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/failing_jobs/testdata/gcc.log
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/failing_jobs/testdata/go.log
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/failing_jobs/testdata/make.log
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/failing_jobs/testdata/npm.log
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/only_python/Byggfile.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/parametric/.gitignore
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/parametric/Byggfile.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/parametric/Byggfile.yml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/parametric/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/taskrunner/Byggfile.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/trivial/Byggfile.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/trivial/Byggfile.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/trivial/input1.txt
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/trivial/more_things/MoreActions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.3.2/examples/trivial/more_things/__init__.py
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 bygg-0.3.2/schemas/Byggfile_yml_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/__init__.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/action.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/apply_configuration.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/argument_unparsing.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/cache.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/common_types.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/completions.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/configuration.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/dag.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/digest.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/job_output.py
--rw-r--r--   0        0        0    18914 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/main.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/py.typed
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/runner.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/scaffolding.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/scheduler.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/status_display.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/system_helpers.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/tree.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bygg-0.3.2/src/bygg/util.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_action.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_argument_unparsing.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_cache.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_completions.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_job_output.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_main.py
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_scheduler.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_system_helpers.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_tree.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/test_utils.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/__snapshots__/test_completions.ambr
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/__snapshots__/test_job_output.ambr
--rw-r--r--   0        0        0    35252 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/__snapshots__/test_main.ambr
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/__snapshots__/test_system_helpers.ambr
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bygg-0.3.2/tests/__snapshots__/test_tree.ambr
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.3.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.3.2/LICENSE
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bygg-0.3.2/README.md
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 bygg-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 bygg-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bygg-0.4.0/.mise.toml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bygg-0.4.0/Vagrantfile
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.0/Vagrantsetup.sh
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bygg-0.4.0/_version.py
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.0/bootstrap.py
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 bygg-0.4.0/mypy.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bygg-0.4.0/noxfile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements-dev.in
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements.in
+-rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bygg-0.4.0/.github/workflows/code_quality.yml
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.4.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/launch.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/checks/Byggfile.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/.gitignore
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile1.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile2.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements1.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements2.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/Byggfile.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/gcc.log
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/go.log
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/make.log
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/npm.log
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/only_python/Byggfile.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/.gitignore
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/Byggfile.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/Byggfile.yml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/taskrunner/Byggfile.yml
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/Byggfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/Byggfile.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/input1.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/more_things/MoreActions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/more_things/__init__.py
+-rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 bygg-0.4.0/schemas/Byggfile_yml_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/py.typed
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/system_helpers.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/util.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/apply_configuration.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/argument_unparsing.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/completions.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/configuration.py
+-rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/dispatcher.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/tree.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/action.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/cache.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/common_types.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/dag.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/digest.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/runner.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/scaffolding.py
+-rw-r--r--   0        0        0     8680 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/scheduler.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/job_output.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/output.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/status_display.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_action.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_argument_unparsing.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_cache.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_completions.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_digest.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_job_output.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_main.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_system_helpers.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_tree.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_completions.ambr
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_job_output.ambr
+-rw-r--r--   0        0        0    35252 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_main.ambr
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_system_helpers.ambr
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_tree.ambr
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 bygg-0.4.0/README.md
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 bygg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 bygg-0.4.0/PKG-INFO
```

### Comparing `bygg-0.3.2/Vagrantfile` & `bygg-0.4.0/Vagrantfile`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/Vagrantsetup.sh` & `bygg-0.4.0/Vagrantsetup.sh`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/bootstrap.py` & `bygg-0.4.0/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/noxfile.py` & `bygg-0.4.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 python_versions = ["3.11", "3.12"]
 
 
 @nox.session(python=python_versions)
 def tests(session):
     session.install("-r", "requirements.txt", "-r", "requirements-dev.txt")
     session.install(".")
-    session.run("pytest")
+    session.run("pytest", "-vv")
 
 
 @nox.session(python=python_versions)
 def basics(session):
     session.install(".")
     session.run("bygg", success_codes=[1], silent=True)
     session.run("bygg", "--help", silent=True)
```

### Comparing `bygg-0.3.2/requirements-dev.txt` & `bygg-0.4.0/requirements-dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --generate-hashes requirements-dev.in
+#    uv pip compile --generate-hashes requirements-dev.in -o requirements-dev.txt
 build==1.2.1 \
     --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
     --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
@@ -67,42 +67,47 @@
     # via pytest
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via
     #   build
     #   pip-tools
-pyright==1.1.356 \
-    --hash=sha256:a101b0f375f93d7082f9046cfaa7ba15b7cf8e1939ace45e984c351f6e8feb99 \
-    --hash=sha256:f05b8b29d06b96ed4a0885dad5a31d9dff691ca12b2f658249f583d5f2754021
+pyright==1.1.359 \
+    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
+    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
 pytest==8.1.1 \
     --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
     --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
-    # via syrupy
-ruff==0.3.4 \
-    --hash=sha256:3f3860057590e810c7ffea75669bdc6927bfd91e29b4baa9258fd48b540a4365 \
-    --hash=sha256:519cf6a0ebed244dce1dc8aecd3dc99add7a2ee15bb68cf19588bb5bf58e0488 \
-    --hash=sha256:60c870a7d46efcbc8385d27ec07fe534ac32f3b251e4fc44b3cbfd9e09609ef4 \
-    --hash=sha256:64abeed785dad51801b423fa51840b1764b35d6c461ea8caef9cf9e5e5ab34d9 \
-    --hash=sha256:6810563cc08ad0096b57c717bd78aeac888a1bfd38654d9113cb3dc4d3f74232 \
-    --hash=sha256:6fc14fa742e1d8f24910e1fff0bd5e26d395b0e0e04cc1b15c7c5e5fe5b4af91 \
-    --hash=sha256:986f2377f7cf12efac1f515fc1a5b753c000ed1e0a6de96747cdf2da20a1b369 \
-    --hash=sha256:98e98300056445ba2cc27d0b325fd044dc17fcc38e4e4d2c7711585bd0a958ed \
-    --hash=sha256:af27ac187c0a331e8ef91d84bf1c3c6a5dea97e912a7560ac0cef25c526a4102 \
-    --hash=sha256:bb0acfb921030d00070539c038cd24bb1df73a2981e9f55942514af8b17be94e \
-    --hash=sha256:c4fd98e85869603e65f554fdc5cddf0712e352fe6e61d29d5a6fe087ec82b76c \
-    --hash=sha256:cf133dd744f2470b347f602452a88e70dadfbe0fcfb5fd46e093d55da65f82f7 \
-    --hash=sha256:cf187a7e7098233d0d0c71175375c5162f880126c4c716fa28a8ac418dcf3378 \
-    --hash=sha256:d3ee7880f653cc03749a3bfea720cf2a192e4f884925b0cf7eecce82f0ce5854 \
-    --hash=sha256:de0d5069b165e5a32b3c6ffbb81c350b1e3d3483347196ffdf86dc0ef9e37dd6 \
-    --hash=sha256:df52972138318bc7546d92348a1ee58449bc3f9eaf0db278906eb511889c4b50 \
-    --hash=sha256:f0f4484c6541a99862b693e13a151435a279b271cff20e37101116a21e2a1ad1
-setuptools==69.2.0 \
-    --hash=sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e \
-    --hash=sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c
+    # via
+    #   pytest-mock
+    #   syrupy
+pytest-mock==3.14.0 \
+    --hash=sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f \
+    --hash=sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0
+ruff==0.4.1 \
+    --hash=sha256:0926cefb57fc5fced629603fbd1a23d458b25418681d96823992ba975f050c2b \
+    --hash=sha256:1c859f294f8633889e7d77de228b203eb0e9a03071b72b5989d89a0cf98ee262 \
+    --hash=sha256:2c6e37f2e3cd74496a74af9a4fa67b547ab3ca137688c484749189bf3a686ceb \
+    --hash=sha256:2d9ef6231e3fbdc0b8c72404a1a0c46fd0dcea84efca83beb4681c318ea6a953 \
+    --hash=sha256:6e68d248ed688b9d69fd4d18737edcbb79c98b251bba5a2b031ce2470224bdf9 \
+    --hash=sha256:9485f54a7189e6f7433e0058cf8581bee45c31a25cd69009d2a040d1bd4bfaef \
+    --hash=sha256:a1eaf03d87e6a7cd5e661d36d8c6e874693cb9bc3049d110bc9a97b350680c43 \
+    --hash=sha256:b34510141e393519a47f2d7b8216fec747ea1f2c81e85f076e9f2910588d4b64 \
+    --hash=sha256:b90506f3d6d1f41f43f9b7b5ff845aeefabed6d2494307bc7b178360a8805252 \
+    --hash=sha256:b92f03b4aa9fa23e1799b40f15f8b95cdc418782a567d6c43def65e1bbb7f1cf \
+    --hash=sha256:baa27d9d72a94574d250f42b7640b3bd2edc4c58ac8ac2778a8c82374bb27984 \
+    --hash=sha256:c7d391e5936af5c9e252743d767c564670dc3889aff460d35c518ee76e4b26d7 \
+    --hash=sha256:d2921ac03ce1383e360e8a95442ffb0d757a6a7ddd9a5be68561a671e0e5807e \
+    --hash=sha256:d592116cdbb65f8b1b7e2a2b48297eb865f6bdc20641879aa9d7b9c11d86db79 \
+    --hash=sha256:eec8d185fe193ad053eda3a6be23069e0c8ba8c5d20bc5ace6e3b9e37d246d3f \
+    --hash=sha256:efd703a5975ac1998c2cc5e9494e13b28f31e66c616b0a76e206de2562e0843c \
+    --hash=sha256:f1ee41580bff1a651339eb3337c20c12f4037f6110a36ae4a2d864c52e5ef954
+setuptools==69.5.1 \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
     # via
     #   nodeenv
     #   pip-tools
 syrupy==4.6.1 \
     --hash=sha256:203e52f9cb9fa749cf683f29bd68f02c16c3bc7e7e5fe8f2fc59bdfe488ce133 \
     --hash=sha256:37a835c9ce7857eeef86d62145885e10b3cb9615bc6abeb4ce404b3f18e1bb36
 typing-extensions==4.10.0 \
```

### Comparing `bygg-0.3.2/requirements.txt` & `bygg-0.4.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --generate-hashes requirements.in
-argcomplete==3.2.3 \
-    --hash=sha256:bf7900329262e481be5a15f56f19736b376df6f82ed27576fa893652c5de6c23 \
-    --hash=sha256:c12355e0494c76a2a7b73e3a59b09024ca0ba1e279fb9ed6c1b82d5b74b6a70c
+#    uv pip compile --generate-hashes requirements.in --output-file requirements.txt
+argcomplete==3.3.0 \
+    --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
+    --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
 dill==0.3.8 \
     --hash=sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca \
     --hash=sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7
     # via multiprocess
 graph-theory==2023.7.6 \
     --hash=sha256:9030aee88aa1db6c778f73338c143a4c872eb9ed5fad5eb9a768ebeb75541340
 msgspec==0.18.6 \
```

### Comparing `bygg-0.3.2/.github/workflows/code_quality.yml` & `bygg-0.4.0/.github/workflows/code_quality.yml`

 * *Files 20% similar despite different names*

```diff
@@ -6,37 +6,41 @@
 permissions:
   contents: read
 
 jobs:
   nox:
     strategy:
       matrix:
-        python_version: ["3.11", "3.12"]
+        python_version: ["3.11.9", "3.12.3"]
         nox_session: [tests, basics, examples]
         os: [ubuntu-latest, macos-latest, macos-14]
+        install_uv: [0, 1]
     runs-on: ${{ matrix.os }}
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python interpreter
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python_version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install nox
+          if [ ${{ matrix.install_uv }} -eq 1 ]; then
+            pip install uv
+          fi
       - name: Test with nox
         run: |
-          nox --python ${{ matrix.python_version }} --session ${{ matrix.nox_session }}
+          nox -P ${{ matrix.python_version }} --session ${{ matrix.nox_session }} -db ${{ matrix.install_uv == 1 && 'uv' || 'virtualenv' }}
 
   pyright_and_ruff:
     strategy:
       matrix:
-        python_version: ["3.11", "3.12"]
+        python_version: ["3.11.9", "3.12.3"]
     runs-on: "ubuntu-latest"
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python_version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python_version }}
```

### Comparing `bygg-0.3.2/.github/workflows/pypi_publish.yml` & `bygg-0.4.0/.github/workflows/pypi_publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,11 +35,11 @@
   publish_github:
     permissions:
       contents: write
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Create GitHub release
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           draft: false
           generate_release_notes: true
```

### Comparing `bygg-0.3.2/.vscode/launch.json` & `bygg-0.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/checks/Byggfile.yml` & `bygg-0.4.0/examples/checks/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/failing_jobs/Byggfile.yml` & `bygg-0.4.0/examples/failing_jobs/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/failing_jobs/testdata/gcc.log` & `bygg-0.4.0/examples/failing_jobs/testdata/gcc.log`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/failing_jobs/testdata/make.log` & `bygg-0.4.0/examples/failing_jobs/testdata/make.log`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/failing_jobs/testdata/npm.log` & `bygg-0.4.0/examples/failing_jobs/testdata/npm.log`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/parametric/Byggfile.py` & `bygg-0.4.0/examples/parametric/Byggfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import random
 import subprocess
 import time
-from typing import List, Set, Tuple
 
-from bygg.action import Action, ActionContext, CommandStatus
+from bygg.core.action import Action, ActionContext, CommandStatus
 
 # Modify these constants to change aspects of the test build:
 
 # Directory for output files
 LEVELLED_DIR_PATH = "t"
 
 # How many levels to build up
@@ -26,32 +25,32 @@
 
 # Execute touch <outfile> in a shell instead of sorting the test files in Python. This
 # will cause work to be done by the process pool, but since the work is trivial, it
 # won't hardly be noticeable.
 USE_SHELL_COMMAND = False
 
 
-def calculate_first_prime_numbers(count: int) -> List[int]:
+def calculate_first_prime_numbers(count: int) -> list[int]:
     """Calculate the first n prime numbers."""
-    primes: List[int] = []
+    primes: list[int] = []
     i = 2
     while len(primes) < count:
         if all(i % prime != 0 for prime in primes):
             primes.append(i)
         i += 1
     return primes
 
 
 # Action function for sorting the input files.
 def sort_lines(ctx: ActionContext):
     if not ctx.inputs:
         return CommandStatus(1, "No inputs.", None)
 
-    changed_files: Set[str] = set()
-    output_lines: List[str] = []
+    changed_files: set[str] = set()
+    output_lines: list[str] = []
 
     for input in ctx.inputs:
         output = input[:-3]
         output_lines.append(f"{input} -> {output}")
         with open(input, "r") as f:
             lines = f.readlines()
         lines.sort()
@@ -63,30 +62,30 @@
     time.sleep(sleep_time)
 
     if GENERATE_LOAD:
         calculate_first_prime_numbers(5000)
     return CommandStatus(0, "Sorted lines.", "\n".join(output_lines))
 
 
-def shell_executor(command: str) -> Tuple[int, str]:
+def shell_executor(command: str) -> tuple[int, str]:
     process = subprocess.run(
         command,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         encoding="utf-8",
     )
     return process.returncode, process.stdout
 
 
 def call_shell_command(ctx: ActionContext):
     sleep_time = random.random() if ADD_SLEEP else 0
     time.sleep(sleep_time)
-    output_lines: List[str] = []
-    rc_list: List[int] = []
+    output_lines: list[str] = []
+    rc_list: list[int] = []
     for output_file in ctx.outputs:
         rc, output = shell_executor(f"touch {output_file}")
         rc_list.append(rc)
         output_lines.append(output)
     return CommandStatus(
         max(rc_list),
         f"Touched output file in {sleep_time:.2f} s",
@@ -102,16 +101,16 @@
             f.write("foo\nbar\nbaz\n")
         return CommandStatus(0, "Created test file.", None)
 
     return action
 
 
 def declare_test_files_actions():
-    generated_files: List[str] = []
-    generated_output_actions: List[Action] = []
+    generated_files: list[str] = []
+    generated_output_actions: list[Action] = []
 
     # Create a set of files with multiple dependency levels. In a real-world scenario,
     # these files would most likely already be present in the filesystem as source files
     # and listed out by a glob.
 
     def get_filename(level: int, file: int):
         return os.path.join(LEVELLED_DIR_PATH, f"l{level}f{file}.txt.in")
```

### Comparing `bygg-0.3.2/examples/trivial/Byggfile.py` & `bygg-0.4.0/examples/trivial/Byggfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 
-from bygg.action import Action, ActionContext, action
-from bygg.common_types import CommandStatus
+from bygg.core.action import Action, ActionContext, action
+from bygg.core.common_types import CommandStatus
 import more_things.MoreActions  # noqa: F401 (imported for side effects)
 
 
 @action(
     "testfile 1",
     inputs=["input1.txt"],
     outputs=["output1.txt"],
```

### Comparing `bygg-0.3.2/examples/trivial/input1.txt` & `bygg-0.4.0/examples/trivial/input1.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/examples/trivial/more_things/MoreActions.py` & `bygg-0.4.0/examples/trivial/more_things/MoreActions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bygg.action import ActionContext, action
-from bygg.common_types import CommandStatus
+from bygg.core.action import ActionContext, action
+from bygg.core.common_types import CommandStatus
 
 
 @action("testfile 2", message="testfile 2", outputs=["output2.txt"])
 def write_foo_to_file(ctx: ActionContext):
     for filename in ctx.outputs:
         with open(filename, "w") as f:
             f.write("foo")
```

### Comparing `bygg-0.3.2/schemas/Byggfile_yml_schema.json` & `bygg-0.4.0/schemas/Byggfile_yml_schema.json`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/src/bygg/action.py` & `bygg-0.4.0/src/bygg/core/action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Iterable, Literal, Optional, Set, Tuple
+from typing import TYPE_CHECKING, Callable, Iterable, Literal, Optional
 
-from bygg.common_types import CommandStatus
+from bygg.core.common_types import CommandStatus
 
 if TYPE_CHECKING:
-    from bygg.scheduler import Scheduler
+    from bygg.core.scheduler import Scheduler
 
 SchedulingType = Literal["in-process", "processpool"]
 
 # Function that returns a string that is included in the dependency digest. Returning
 # None causes the value to be ignored.
 DynamicDependency = Callable[[], str | None]
 
 
 @dataclass
 class ActionContext:
     name: str
     message: str | None
-    inputs: Set[str]
-    outputs: Set[str]
-    dependencies: Set[str]
+    inputs: set[str]
+    outputs: set[str]
+    dependencies: set[str]
     dynamic_dependency: Optional[DynamicDependency]
     is_entrypoint: bool
     scheduling_type: SchedulingType
 
 
 Command = Callable[[ActionContext], CommandStatus]
 
@@ -60,15 +60,15 @@
         A description of the action. Default is the docstring of the command if
         provided, else None.
     """
 
     scheduler: Scheduler | None = None
 
     command: Command | None
-    dependency_files: Set[str]
+    dependency_files: set[str]
 
     def __init__(
         self,
         name: str,
         message: str | None = None,
         inputs: Optional[Iterable[str]] = None,
         outputs: Optional[Iterable[str]] = None,
@@ -133,34 +133,39 @@
     return create_action
 
 
 def action_set(
     base_name: str,
     *,
     message: Optional[str] = None,
-    file_pairs: Iterable[Tuple[str, str]],
+    file_pairs: Iterable[tuple[str, str]],
+    extra_inputs: Optional[Iterable[str]] = None,
     dependencies: Optional[Iterable[str]] = None,
     is_entrypoint: bool = False,
 ):
     """
     Decorator for creating individual Actions from a list of input-output file pairs and
     a function. Creates one Action that depends on all of the individual Actions. It has
     name = base_name, which in turn can be used as a dependency for other Actions.
     """
 
     def create_actions(func: Callable):
         action_list = []
         for input_file, output_file in file_pairs:
-            action_name = f"{base_name}_{output_file}"
+            action_name = f"{base_name}::{output_file}"
             action_list.append(action_name)
             Action(
                 action_name,
                 message,
-                inputs=[input_file],
+                inputs=[input_file] + list(extra_inputs) if extra_inputs else None,
                 outputs=[output_file],
                 dependencies=dependencies,
-                is_entrypoint=is_entrypoint,
                 command=func,
             )
-        Action(base_name, f"Action set {base_name}", dependencies=action_list)
+        Action(
+            base_name,
+            f"Action set {base_name}",
+            dependencies=action_list,
+            is_entrypoint=is_entrypoint,
+        )
 
     return create_actions
```

### Comparing `bygg-0.3.2/src/bygg/apply_configuration.py` & `bygg-0.4.0/src/bygg/cmd/apply_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 from pathlib import Path
 import shutil
 import subprocess
 import sys
 import textwrap
-from typing import List
 
-from bygg.action import Action
-from bygg.configuration import PYTHON_INPUTFILE, ByggFile, Environment
-from bygg.digest import calculate_string_digest
-from bygg.output import output_error, output_info, output_plain
+from bygg.cmd.configuration import PYTHON_INPUTFILE, ByggFile, Environment
+from bygg.core.action import Action
+from bygg.core.digest import calculate_string_digest
+from bygg.output.output import output_error, output_info, output_plain
 from bygg.util import create_shell_command
 
 
 def calculate_environment_hash(environment: Environment) -> str:
-    requirements: List[str] = []
+    requirements: list[str] = []
     requirements.append(environment.shell)
     if environment.inputs:
         for input in environment.inputs:
             with open(input, "r") as f:
                 requirements += f.readlines()
     return calculate_string_digest(" ".join(requirements))
```

### Comparing `bygg-0.3.2/src/bygg/argument_unparsing.py` & `bygg-0.4.0/src/bygg/cmd/argument_unparsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import functools
-from typing import List
 
 
 @functools.cache
 def _build_dest_to_action(parser: argparse.ArgumentParser) -> dict:
     actions = parser._get_optional_actions() + parser._get_positional_actions()
     dest_to_action = {action.dest: action for action in actions}
     return dest_to_action
@@ -19,34 +18,34 @@
     return option_strings[-1] if option_strings else ""
 
 
 def unparse_args(
     parser: argparse.ArgumentParser,
     args: argparse.Namespace,
     *,
-    drop: List[str] | None = None,
-) -> List[str]:
+    drop: list[str] | None = None,
+) -> list[str]:
     """
     Convert an argparse.Namespace back to a list of command line arguments.
 
     Parameters
     ----------
     parser : argparse.ArgumentParser
         The parser that was used to parse the command line arguments.
     args : argparse.Namespace
         The parsed command line arguments to unparse.
-    drop : List[str] | None, optional
+    drop : list[str] | None, optional
         Which dest keys to drop, by default None.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of command line arguments
     """
-    exec_list: List[str] = []
+    exec_list: list[str] = []
     for k, v in vars(args).items():
         argument = _get_argument_for_dest(parser, k)
         if drop and k in drop:
             continue
         if v is False or v is None:
             # These are arguments that were not given
             continue
```

### Comparing `bygg-0.3.2/src/bygg/cache.py` & `bygg-0.4.0/src/bygg/core/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from pathlib import Path
 import pickle
 
-from bygg.scaffolding import STATUS_DIR, make_sure_status_dir_exists
+from bygg.core.scaffolding import STATUS_DIR, make_sure_status_dir_exists
 
 DEFAULT_DB_FILE = STATUS_DIR / "cache.db"
 
 
 @dataclass
 class InputsOutputsDigests:
     inputs_digest: str
```

### Comparing `bygg-0.3.2/src/bygg/completions.py` & `bygg-0.4.0/src/bygg/cmd/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import argparse
 from pathlib import Path
 import shutil
 import sys
 import textwrap
-from typing import Any, Generator, Set
+from typing import Any, Generator
 
 from argcomplete.completers import DirectoriesCompleter
 from argcomplete.finders import CompletionFinder
-
-from bygg.output import output_plain
+from bygg.output.output import output_plain
 
 
 class ByggfileDirectoriesCompleter(DirectoriesCompleter):
     """
     A completer for directories that contain Bygg files.
     """
 
@@ -26,21 +25,21 @@
                 if b.suffix in {".py", ".yml"}
             }
         for f in sorted(list(byggfile_dirs)):
             yield f
 
 
 def construct_already_there(
-    parser: argparse.ArgumentParser | Any, options: Set[str]
-) -> Set[str]:
+    parser: argparse.ArgumentParser | Any, options: set[str]
+) -> set[str]:
     """
     Construct a set of options that are already present among the command line
     arguments. Adds both the short and long versions if they exist.
     """
-    already_there_set: Set[str] = set()
+    already_there_set: set[str] = set()
     for action in parser._get_optional_actions():
         option_strings = set(action.option_strings)
         if option_strings & options:
             already_there_set.update(option_strings)
     return already_there_set
```

### Comparing `bygg-0.3.2/src/bygg/configuration.py` & `bygg-0.4.0/src/bygg/cmd/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 import sys
-from typing import Dict, List, Optional
+from typing import Optional
 
+from bygg.output.output import Symbols, output_plain
+from bygg.output.output import TerminalStyle as TS
 import msgspec
 
-from bygg.output import Symbols, output_plain
-from bygg.output import TerminalStyle as TS
-
 PYTHON_INPUTFILE = "Byggfile.py"
 YAML_INPUTFILE = "Byggfile.yml"
 
 
 class Settings(msgspec.Struct, forbid_unknown_fields=True):
     default_action: Optional[str] = None
 
 
 class ActionItem(msgspec.Struct, forbid_unknown_fields=True):
-
     """
     This is a representation of the Action class used for deserialising from YAML.
 
     Parameters
     ----------
     name : str
         The name of the action.
@@ -43,56 +41,56 @@
     shell : str, optional
         The shell command to execute when the action is run. Default is None.
     """
 
     name: str
     description: Optional[str] = None
     message: Optional[str] = None
-    inputs: Optional[List[str]] = None
-    outputs: Optional[List[str]] = None
-    dependencies: Optional[List[str]] = None
+    inputs: Optional[list[str]] = None
+    outputs: Optional[list[str]] = None
+    dependencies: Optional[list[str]] = None
     is_entrypoint: Optional[bool] = None
     environment: Optional[str] = "default"
     shell: Optional[str] = None
 
 
 class Environment(msgspec.Struct, forbid_unknown_fields=True):
     """
     A class used to represent a virtual environment that actions can be run in.
 
     Attributes
     ----------
     byggfile : str
         The Python Byggfile that uses this environment.
-    inputs : List[str]
+    inputs : list[str]
         A list of files that are used as input to the environment. Typically pip
         requirements files, but can be any files.
     venv_directory : str
         The directory where the virtual environment is located. Will be recreated by
         Bygg if any of the inputs are modified.
     shell : str
         The shell command for creating the environment.
     description : str, optional
         A description of the environment. Used in e.g. help messages, by default None
     message : str, optional
         A message related to the environment, by default None
     """
 
     byggfile: str
-    inputs: List[str]
+    inputs: list[str]
     venv_directory: str
     shell: str
     description: Optional[str] = None
     message: Optional[str] = None
 
 
 class ByggFile(msgspec.Struct, forbid_unknown_fields=True):
-    actions: List[ActionItem]
+    actions: list[ActionItem]
     settings: Settings = msgspec.field(default_factory=Settings)
-    environments: Dict[str, Environment] = msgspec.field(default_factory=dict)
+    environments: dict[str, Environment] = msgspec.field(default_factory=dict)
 
 
 def read_config_file() -> ByggFile:
     if not os.path.isfile(YAML_INPUTFILE):
         return ByggFile(actions=[], settings=Settings(), environments={})
 
     try:
```

### Comparing `bygg-0.3.2/src/bygg/dag.py` & `bygg-0.4.0/src/bygg/core/dag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from abc import ABCMeta, abstractmethod
 from collections import deque
-from typing import Any, Dict, Iterable, List
+from typing import Any, Iterable
 
-from bygg.action import Action
+from bygg.core.action import Action
 
 
 class Dag(metaclass=ABCMeta):
     def __len__(self) -> int:
         return 0
 
-    def clear(self):
-        ...
+    def clear(self): ...
 
-    def remove_node(self, node: str):
-        ...
+    def remove_node(self, node: str): ...
 
-    def build_action_graph(self, build_actions: Dict[str, Action], action: Action):
-        ...
+    def build_action_graph(self, build_actions: dict[str, Action], action: Action): ...
 
     @abstractmethod
     def get_ready_jobs(
         self,
-        finished_jobs: Dict[str, Any],
-        running_jobs: Dict[str, Any],
-    ) -> List[str]:
-        ...
+        finished_jobs: dict[str, Any],
+        running_jobs: dict[str, Any],
+    ) -> list[str]: ...
 
     @abstractmethod
-    def get_all_jobs(self) -> Iterable[str]:
-        ...
+    def get_all_jobs(self) -> Iterable[str]: ...
 
 
 class GtDag(Dag):
     def __init__(self):
         import graph  # type: ignore
 
         self.graph = graph.Graph()
@@ -49,32 +44,32 @@
             return
         for n in nodes:
             self.graph.del_node(n)
 
     def remove_node(self, node: str):
         self.graph.del_node(node)
 
-    def build_action_graph(self, build_actions: Dict[str, Action], action: Action):
+    def build_action_graph(self, build_actions: dict[str, Action], action: Action):
         """Build the action graph."""
         queue = deque([action])
         while len(queue) > 0:
             a = queue.popleft()
             self.graph.add_node(a.name)
             for dependency in a.dependencies:
                 dependency_action = build_actions.get(dependency)
                 if not dependency_action:
                     raise ValueError(f"Action '{dependency}' not found")
                 queue.append(dependency_action)
                 self.graph.add_edge(a.name, dependency)
 
     def get_ready_jobs(
         self,
-        finished_jobs: Dict[str, Any],
-        running_jobs: Dict[str, Any],
-    ) -> List[str]:
+        finished_jobs: dict[str, Any],
+        running_jobs: dict[str, Any],
+    ) -> list[str]:
         nodes = self.graph.nodes()
         if nodes is None:
             return []
         if len(nodes) == 1 and (
             nodes[0] not in finished_jobs and nodes[0] not in running_jobs
         ):
             return nodes
```

### Comparing `bygg-0.3.2/src/bygg/digest.py` & `bygg-0.4.0/src/bygg/core/digest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 import dis
 import functools
 import hashlib
 import io
 import os
-from typing import Callable, List, Set, Tuple
+from typing import Callable
 
 DIGEST_TYPE = "sha1"
 
-# If True, cache the file digest in memory based on the content and stat.mtime_ns of the
-# file.
+# If True, cache the file digest in memory based on the filename, stat.ctime_ns,
+# stat.mtime_ns and stat.size of the file.
 ALLOW_DIGEST_CACHING = True
 
 
-@functools.cache
-def file_digest_memo(file: str, mtime: int) -> str | None:
+def file_digest(file: str) -> str:
     with open(file, "rb") as f:
         return hashlib.file_digest(f, DIGEST_TYPE).hexdigest()
 
 
+@functools.cache
+def file_digest_memo(
+    file: str, st_ctime_ns: int, st_mtime_ns: int, st_size: int
+) -> str:
+    """
+    Cache a file's digest based on the content, stat.ctime_ns, stat.mtime_ns and
+    stat.size of the file.
+    """
+    return file_digest(file)
+
+
 def calculate_file_digest(file: str) -> str | None:
     """
     Calculate the digest of a file.
 
     file: The file to calculate the digest of.
     Returns: The digest of the file as a hex string, or None if the file does not exist.
 
     """
-    if os.path.isfile(file):
-        s = os.stat(file)
-        with open(file, "rb") as f:
-            if ALLOW_DIGEST_CACHING:
-                return file_digest_memo(file, s.st_mtime_ns)
-            return hashlib.file_digest(f, DIGEST_TYPE).hexdigest()
+    real_path = os.path.realpath(file)
+    if os.path.isfile(real_path):
+        if ALLOW_DIGEST_CACHING:
+            st = os.stat(real_path)
+            return file_digest_memo(
+                real_path, st.st_ctime_ns, st.st_mtime_ns, st.st_size
+            )
+        return file_digest(real_path)
 
 
-def calculate_dependency_digest(filenames: Set[str]) -> Tuple[str, bool]:
+def calculate_dependency_digest(filenames: set[str]) -> tuple[str, bool]:
     """
     Calculate the digest of a set of files.
     filenames: The files to calculate the digest of.
     Returns: The digest of the files as a hex string.
     """
 
-    files_were_missing = False
-
-    digests = sorted(
-        filter(None, [calculate_file_digest(filename) for filename in filenames])
-    )
-
-    # if len(digests) == 0:
-    #     return ""
+    file_digests = [calculate_file_digest(filename) for filename in filenames]
+    digests = sorted(filter(None, file_digests))
+    files_were_missing = len(file_digests) != len(digests)
 
     return (
         hashlib.new(DIGEST_TYPE, "".join(digests).encode()).hexdigest(),
         files_were_missing,
     )
 
 
-def calculate_digest(items: List[str]) -> str:
+def calculate_digest(items: list[str]) -> str:
     digests = sorted(
         filter(
             None,
             [hashlib.new(DIGEST_TYPE, item.encode()).hexdigest() for item in items],
         )
     )
```

### Comparing `bygg-0.3.2/src/bygg/job_output.py` & `bygg-0.4.0/src/bygg/output/job_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass
 import re
-from typing import List
 
-from bygg.output import TerminalStyle as TS
-from bygg.output import isatty, output_plain
-from bygg.scheduler import Job
+from bygg.core.scheduler import Job
+from bygg.output.output import TerminalStyle as TS
+from bygg.output.output import isatty, output_plain
 
 
 @dataclass
 class HighlightConfig:
     pattern: str | re.Pattern[str]
     start: str
     end: str
@@ -22,18 +21,18 @@
 
 error_hl_config = HighlightConfig(
     pattern=r"(error\w*:?|ERR!)",
     start=TS.Bg.RED,
     end=TS.Fg.RESET + TS.Bg.RESET,
 )
 
-default_highlight_config: List[HighlightConfig] = [warning_hl_config, error_hl_config]
+default_highlight_config: list[HighlightConfig] = [warning_hl_config, error_hl_config]
 
 
-def highlight_log(message: str, config: List[HighlightConfig] | None = None):
+def highlight_log(message: str, config: list[HighlightConfig] | None = None):
     """
     Highlights the message according to the regexes and styles. Regexes are applied
     per line.
     """
     if not config:
         return message
 
@@ -41,15 +40,15 @@
     for line in message.splitlines():
         for c in config:
             line = re.sub(c.pattern, c.start + r"\1" + c.end, line, flags=re.IGNORECASE)
         lines.append(line)
     return "\n".join(lines)
 
 
-def output_job_logs(jobs: List[Job]):
+def output_job_logs(jobs: list[Job]):
     print(
         f"\n{TS.BOLD}Showing logs for {len(jobs)} failed job{'s' if len(jobs) > 1 else ''}:{TS.RESET}\n"
     )
     for job in jobs:
         if job.status and (log := job.status.output):
             output_plain(f'{TS.BOLD}--- Start "{ job.name }" ---{TS.RESET}')
             output_plain(
```

### Comparing `bygg-0.3.2/src/bygg/main.py` & `bygg-0.4.0/src/bygg/cmd/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-# PYTHON_ARGCOMPLETE_OK
-
 import argparse
 from dataclasses import dataclass
 import os
 import shutil
 import stat
 import subprocess
 import sys
 import textwrap
 import time
-from typing import Any, List
+from typing import Any
 
-from bygg.apply_configuration import (
+from bygg.cmd.apply_configuration import (
     apply_configuration,
     register_actions_from_configuration,
 )
-from bygg.argument_unparsing import unparse_args
-from bygg.completions import (
+from bygg.cmd.argument_unparsing import unparse_args
+from bygg.cmd.completions import (
     ByggfileDirectoriesCompleter,
     do_completion,
     generate_shell_completions,
 )
-from bygg.configuration import (
+from bygg.cmd.configuration import (
     PYTHON_INPUTFILE,
     YAML_INPUTFILE,
     ByggFile,
     dump_schema,
     read_config_file,
 )
-from bygg.job_output import output_job_logs
-from bygg.output import (
+from bygg.cmd.tree import display_tree
+from bygg.core.runner import ProcessRunner
+from bygg.core.scheduler import Scheduler
+from bygg.output.job_output import output_job_logs
+from bygg.output.output import (
     TerminalStyle as TS,
 )
-from bygg.output import (
+from bygg.output.output import (
     output_error,
     output_info,
     output_ok,
     output_plain,
     output_warning,
 )
-from bygg.runner import ProcessRunner
-from bygg.scheduler import Scheduler
-from bygg.status_display import (
+from bygg.output.status_display import (
     failed_checks,
     on_job_status,
     on_runner_status,
     output_check_results,
 )
 from bygg.system_helpers import change_dir
-from bygg.tree import display_tree
 
 
 @dataclass
 class ByggContext:
     """Container for various state"""
 
     runner: ProcessRunner
@@ -80,15 +78,15 @@
     runner.runner_status_listener = on_runner_status
 
     return ByggContext(runner, scheduler, configuration)
 
 
 def build(
     ctx: ByggContext,
-    actions: List[str],
+    actions: list[str],
     job_count: int | None,
     always_make: bool,
     check: bool,
 ) -> bool:
     """
     actions: The actions to build.
 
@@ -138,15 +136,15 @@
 
     if check and failed_checks:
         return output_check_results()
 
     return True
 
 
-def clean(ctx: ByggContext, actions: List[str]):
+def clean(ctx: ByggContext, actions: list[str]):
     try:
         for action in actions:
             output_info(f"Cleaning action '{action}':")
             ctx.scheduler.prepare_run(action)
             for job_name in ctx.scheduler.job_graph.get_all_jobs():
                 job = ctx.scheduler.build_actions.get(job_name, None)
                 if job is None:
@@ -179,15 +177,15 @@
     name: str
     description: str
 
 
 NO_DESCRIPTION = "No description"
 
 
-def get_entrypoints(ctx: ByggContext) -> List[EntryPoint]:
+def get_entrypoints(ctx: ByggContext) -> list[EntryPoint]:
     return [
         EntryPoint(x.name, x.description or NO_DESCRIPTION)
         for x in ctx.scheduler.build_actions.values()
         if x.is_entrypoint
     ] or [
         EntryPoint(x.name, x.description or NO_DESCRIPTION)
         for x in ctx.configuration.actions
@@ -263,18 +261,15 @@
 
     return True
 
 
 def print_version():
     import importlib.metadata
 
-    if __package__:
-        output_info(f"{__package__} {importlib.metadata.version(__package__)}")
-    else:
-        output_error("Could not determine package name.")
+    output_info(f"bygg {importlib.metadata.version('bygg')}")
 
 
 MAKE_COMPATIBLE_PANEL = "(Roughly) Make-compatible options"
 
 
 def dispatcher():
     """
@@ -374,15 +369,15 @@
                 sys.exit(1)
         else:
             status = do_dispatch(ctx, args, partition.actions)
             if not status:
                 sys.exit(1)
 
 
-def do_dispatch(ctx: ByggContext, args: argparse.Namespace, actions: List[str]) -> bool:
+def do_dispatch(ctx: ByggContext, args: argparse.Namespace, actions: list[str]) -> bool:
     # Analysis implies building:
     always_make = args.always_make or args.check
     if args.clean:
         status = clean(ctx, actions)
     elif args.list:
         list_actions(ctx)
         status = True
@@ -405,38 +400,38 @@
     environment_name: The name of the environment that the actions should be run in.
     None means the implicit default environment, i.e. typically the base process.
 
     actions: The actions that should be run in the environment.
     """
 
     environment_name: str | None
-    actions: List[str]
+    actions: list[str]
 
 
 def partition_actions(
     configuration: ByggFile,
-    actions: List[str] | None,
-) -> List[ActionPartition] | None:
+    actions: list[str] | None,
+) -> list[ActionPartition] | None:
     """
     Partition the actions into groups that should be run in the same environment. Only
     partition the given actions that also exist in the configuration file. This is to
     not have to load the Python build files for all the environments, since installing
-    their respective requiements can take a while.
+    their respective requirements can take a while.
 
     Parameters
     ----------
     configuration : ByggFile
         The configuration file.
-    actions : List[str] | None
+    actions : list[str] | None
         The actions that should be run. If None, a partition will be created, resolved
         to the default action.
 
     Returns
     -------
-    List[ActionPartition] | None
+    list[ActionPartition] | None
         A list of ActionPartition objects, each representing a group of actions that
         should be run in the same environment. Returns None if there are no actions in
         the configuration.
     """
     if not configuration.actions:
         return None
 
@@ -602,19 +597,7 @@
     meta_group.add_argument(
         "--completions",
         action="store_true",
         help="Output instructions for how to set up shell completions via the shell's startup script.",
     )
 
     return parser
-
-
-def main():
-    try:
-        return dispatcher()
-    except KeyboardInterrupt:
-        output_warning("Interrupted by user. Aborting.")
-        return 1
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `bygg-0.3.2/src/bygg/output.py` & `bygg-0.4.0/src/bygg/output/output.py`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/src/bygg/runner.py` & `bygg-0.4.0/src/bygg/core/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os
 import signal
-from typing import Callable, List
+from typing import Callable
 
+from bygg.core.action import Action, CommandStatus
+from bygg.core.common_types import JobStatus
+from bygg.core.scheduler import Job, Scheduler
+from bygg.output.output import TerminalStyle as TS
+from bygg.output.status_display import on_check_failed
 import multiprocess.managers  # type: ignore
 from multiprocess.pool import ApplyResult, Pool  # type: ignore
 
-from bygg.action import Action, CommandStatus
-from bygg.common_types import JobStatus
-from bygg.output import TerminalStyle as TS
-from bygg.scheduler import Job, Scheduler
-from bygg.status_display import on_check_failed
-
 JobStatusListener = Callable[[str, JobStatus, Action, CommandStatus | None], None]
 RunnerStatusListener = Callable[[str], None]
 
 
 class ProcessRunner:
     scheduler: Scheduler
     job_status_listener: JobStatusListener
     runner_status_listener: RunnerStatusListener
-    failed_jobs: List[Job]
+    failed_jobs: list[Job]
 
     def __init__(self, scheduler: Scheduler):
         self.scheduler = scheduler
         self.job_status_listener = lambda *args: None
         self.runner_status_listener = lambda *args: None
         self.failed_jobs = []
 
@@ -33,16 +32,16 @@
         )
 
         def init_worker():
             """Ignore CTRL+C in the worker process."""
             signal.signal(signal.SIGINT, signal.SIG_IGN)
 
         with Pool(max_workers, init_worker) as pool:
-            scheduled_queue: List[ApplyResult] = []
-            backlog: List[Job] = []
+            scheduled_queue: list[ApplyResult] = []
+            backlog: list[Job] = []
 
             manager = multiprocess.managers.SyncManager()
             manager.start()
             qq = manager.Queue()  # type: ignore # no/bad multiprocess types
 
             def poll_msg_queue():
                 while not qq.empty():
@@ -143,16 +142,16 @@
                             "failed",
                             job_result.action,
                             job_result.status,
                         )
                         poll_msg_queue()
                         early_out = True
 
-    def check_for_missing_output_files(self, job: Job) -> List[str]:
-        missing_files: List[str] = []
+    def check_for_missing_output_files(self, job: Job) -> list[str]:
+        missing_files: list[str] = []
         for filename in job.action.outputs:
             if not os.path.exists(filename):
                 missing_files.append(filename)
         return missing_files
 
 
 def run_job(job: Job, qq):
```

### Comparing `bygg-0.3.2/src/bygg/scheduler.py` & `bygg-0.4.0/src/bygg/core/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from pathlib import Path
-from typing import Dict, List, Literal, Set
+from typing import Literal
 
+from bygg.core.action import Action, CommandStatus
+from bygg.core.cache import Cache
+from bygg.core.dag import Dag, create_dag
+from bygg.core.digest import calculate_dependency_digest, calculate_digest
+from bygg.output.status_display import on_check_failed
 import msgspec
 
-from bygg.action import Action, CommandStatus
-from bygg.cache import Cache
-from bygg.dag import Dag, create_dag
-from bygg.digest import calculate_dependency_digest, calculate_digest
-from bygg.status_display import on_check_failed
-
 
 class Job:
     name: str
     action: Action
     status: CommandStatus | None
 
     def __init__(self, action: Action):
@@ -36,25 +35,25 @@
 class ActionDigestItem(msgspec.Struct):
     inputs_digest: str
     outputs_digest: str
 
 
 class Scheduler:
     cache: Cache
-    build_actions: Dict[str, Action]
+    build_actions: dict[str, Action]
 
     job_graph: Dag
-    dirty_jobs: Set[str]
-    ready_jobs: Set[str]
-    running_jobs: Dict[str, Job]
-    finished_jobs: Dict[str, Job]
+    dirty_jobs: set[str]
+    ready_jobs: set[str]
+    running_jobs: dict[str, Job]
+    finished_jobs: dict[str, Job]
 
     started: bool
     always_make: bool
-    check_inputs_outputs_set: Set[str] | None
+    check_inputs_outputs_set: set[str] | None
 
     def __init__(self):
         Action.scheduler = self
         self.cache = Cache()
         self.build_actions = {}
         self.job_graph = create_dag()
         self.dirty_jobs = set()
@@ -74,16 +73,17 @@
         self.running_jobs = {}
         self.finished_jobs = {}
 
         self.job_graph.build_action_graph(
             self.build_actions, self.build_actions[entrypoint]
         )
 
-        # Fill the actions' _dependency_files from their dependencies
+        # Fill the actions' dependency_files from self and their dependencies
         for action in self.build_actions.values():
+            action.dependency_files.update(action.inputs)
             for dependency in action.dependencies:
                 action.dependency_files.update(self.build_actions[dependency].outputs)
             # print(f"Action {action.name} inputs: {action._dependency_files}")
 
     def start_run(
         self, entrypoint: str, *, always_make: bool = False, check: bool = False
     ):
@@ -169,15 +169,15 @@
             # The inputs have changed, so we need to rebuild
             # print(f"Job {job_name} is dirty (inputs changed)")
             return True
 
         # print(f"Job {job_name} is clean")
         return False
 
-    def get_ready_jobs(self, batch_size: int = 0) -> List[Job]:
+    def get_ready_jobs(self, batch_size: int = 0) -> list[Job]:
         """
         Create a batch of jobs and put them in the running pool. Returns all ready jobs
         if batch_size is 0.
 
         An empty job list may be returned even if there are more jobs left to run if all
         jobs in the batch were skipped. Job runners should continue polling for more
         jobs until the scheduler status is "finished".
@@ -193,15 +193,15 @@
                 else:
                     self.skip_job(job)
             self.ready_jobs.update(dirty_jobs)
 
         if len(self.ready_jobs) == 0:
             return []
 
-        job_list: List[Job] = []
+        job_list: list[Job] = []
         for _ in range(
             len(self.ready_jobs)
             if batch_size == 0
             else min(batch_size, len(self.ready_jobs))
         ):
             action = self.build_actions[self.ready_jobs.pop()]
             new_job = Job(action)
```

### Comparing `bygg-0.3.2/src/bygg/status_display.py` & `bygg-0.4.0/src/bygg/output/status_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 import shutil
-from typing import List, Literal
+from typing import Literal
 
-from bygg.action import Action
-from bygg.common_types import CommandStatus, JobStatus, Severity
-from bygg.output import (
+from bygg.core.action import Action
+from bygg.core.common_types import CommandStatus, JobStatus, Severity
+from bygg.output.output import (
     Symbols,
     output_error,
     output_info,
     output_warning,
     output_with_status_line,
 )
 
@@ -77,15 +77,15 @@
 class CheckStatus:
     rule_name: CheckRule
     action: Action
     status_text: str
     severity: Severity
 
 
-failed_checks: List[CheckStatus] = []
+failed_checks: list[CheckStatus] = []
 
 
 def on_check_failed(
     rule_name: CheckRule, action: Action, status_text: str, severity: Severity
 ):
     failed_checks.append(CheckStatus(rule_name, action, status_text, severity))
```

### Comparing `bygg-0.3.2/src/bygg/system_helpers.py` & `bygg-0.4.0/src/bygg/system_helpers.py`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/src/bygg/tree.py` & `bygg-0.4.0/src/bygg/cmd/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from itertools import chain
-from typing import List
 
-from bygg.output import TerminalStyle as TS
-from bygg.scheduler import Scheduler
+from bygg.core.scheduler import Scheduler
+from bygg.output.output import TerminalStyle as TS
 
 
 class TreeStyle:
     """Base class for tree styles."""
 
     BAR = "─"
     PIPE = "│"
@@ -37,15 +36,15 @@
     def __init__(self, indent=4):
         self.CONNECTOR = (
             f"{self.T_JOINT + self.BAR * (indent - 1 - len(self.T_JOINT)):<{indent}}"
         )
         self.HANGER = f"{self.END_CORNER + self.BAR * (indent - 1 - len(self.END_CORNER)):<{indent}}"
 
 
-def display_tree(scheduler: Scheduler, entry_points: List[str]):
+def display_tree(scheduler: Scheduler, entry_points: list[str]):
     """
     Display the dependency tree for the given entry points.
 
     Example output:
 
     all_checks
     ├── check_inputs_outputs
@@ -58,15 +57,15 @@
 
     indent = 4
     style = TreeStyleUnicode(indent)
 
     for entry_point in entry_points:
         build_actions = scheduler.build_actions
 
-        def format_children(name: str, last_sibling: bool, depth: int) -> List[str]:
+        def format_children(name: str, last_sibling: bool, depth: int) -> list[str]:
             action = build_actions[name]
             display_name = f"{TS.BOLD}{name}{TS.RESET}" if depth == 0 else name
 
             # Format children and flatten:
             children = chain.from_iterable(
                 (
                     format_children(dep, i == len(action.dependencies) - 1, depth + 1)
```

### Comparing `bygg-0.3.2/src/bygg/util.py` & `bygg-0.4.0/src/bygg/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 import re
 import subprocess
-from typing import List, Optional, Set, Tuple
+from typing import Optional
 
-from bygg.common_types import CommandStatus
+from bygg.core.common_types import CommandStatus
 
 
 def create_shell_command(shell_command: str, message: Optional[str] = None):
-    def call_shell_command(inputs: Optional[Set[str]], outputs: Optional[Set[str]]):
+    def call_shell_command(inputs: Optional[set[str]], outputs: Optional[set[str]]):
         # Map stderr onto stdout and return both as the output
         process = subprocess.run(
             shell_command,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             encoding="utf-8",
         )
         return CommandStatus(process.returncode, message, process.stdout)
 
     return lambda ctx: call_shell_command(ctx.inputs, ctx.outputs)
 
 
 def filenames_from_pattern(
-    input_files: List[str], in_pattern: str, out_pattern: str
-) -> List[Tuple[str, str]]:
+    input_files: list[str], in_pattern: str, out_pattern: str
+) -> list[tuple[str, str]]:
     """
     Generate a list of tuples with the input and output file names from a a list of
     input file names and a pattern like in Makefile pattern rules. File names that don't
     match the pattern are ignored. Example:
 
       ["/foo/bar/baz.txt.j2"], "%.txt.j2", "out_%.txt")
         => [("/foo/bar/baz.txt.j2", "/foo/bar/out_baz.txt")]
```

### Comparing `bygg-0.3.2/tests/conftest.py` & `bygg-0.4.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 import shutil
 from tempfile import mkstemp
 
-from bygg.action import Action
-from bygg.scheduler import Scheduler
+from bygg.core.action import Action
+from bygg.core.scheduler import Scheduler
 import pytest
 
 
 def get_closed_tmpfile() -> Path:
     fd, path = mkstemp()
     os.close(fd)
     return Path(path)
```

### Comparing `bygg-0.3.2/tests/test_action.py` & `bygg-0.4.0/tests/test_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bygg.action import Action, ActionContext, CommandStatus
-from bygg.scheduler import Scheduler
+from bygg.core.action import Action, ActionContext, CommandStatus
+from bygg.core.scheduler import Scheduler
 import pytest
 
 
 @pytest.fixture
 def init_scheduler():
     Scheduler()
     yield
```

### Comparing `bygg-0.3.2/tests/test_argument_unparsing.py` & `bygg-0.4.0/tests/test_argument_unparsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bygg.argument_unparsing import unparse_args
-from bygg.main import create_argument_parser
+from bygg.cmd.argument_unparsing import unparse_args
+from bygg.cmd.dispatcher import create_argument_parser
 import pytest
 
 args = [
     (["-v"], ["--version"]),
     (["--version"], ["--version"]),
     (["--clean"], ["--clean"]),
     (["-l"], ["--list"]),
```

### Comparing `bygg-0.3.2/tests/test_cache.py` & `bygg-0.4.0/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory, mkstemp
 
-from bygg.cache import Cache, InputsOutputsDigests
+from bygg.core.cache import Cache, InputsOutputsDigests
 
 
 def test_cache_load_non_existing():
     fd, path = mkstemp()
     os.close(fd)
     os.unlink(path)
```

### Comparing `bygg-0.3.2/tests/test_completions.py` & `bygg-0.4.0/tests/test_completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
-from bygg.completions import ByggCompletionFinder
-from bygg.main import create_argument_parser
+from bygg.cmd.completions import ByggCompletionFinder
+from bygg.cmd.dispatcher import create_argument_parser
 from bygg.system_helpers import change_dir
 import pytest
 
 
 def dummy_exit_method(status):
     pass
 
@@ -69,15 +69,16 @@
 directories_completions = [
     "-C ",
     "--directory ",
 ]
 
 
 @pytest.mark.parametrize("arg", directories_completions, ids=lambda x: x)
-def test_directory_completions(completion_tester, arg, snapshot):
+def test_directory_completions(completion_tester, arg, snapshot, monkeypatch):
+    monkeypatch.chdir("examples")
     testcase = arg
     testresult = completion_tester(testcase)
     assert sorted(testresult.split("\x0b")) == snapshot
 
 
 actions_completions = [p for p in Path("examples").iterdir() if p.is_dir()]
```

### Comparing `bygg-0.3.2/tests/test_job_output.py` & `bygg-0.4.0/tests/test_job_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from bygg.job_output import HighlightConfig, highlight_log
+from bygg.output.job_output import HighlightConfig, highlight_log
 import pytest
 
 short_gcc_log = """
 main.c: In function ‘main’:
 main.c:5:5: warning: implicit declaration of function ‘foo’ [-Wimplicit-function-declaration]
     foo();
     ^~~
```

### Comparing `bygg-0.3.2/tests/test_main.py` & `bygg-0.4.0/tests/test_main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 from pathlib import Path
+import re
 import subprocess
 
 import pytest
 
 
 @dataclass
 class ExampleParameters:
@@ -77,7 +78,23 @@
     process = subprocess.run(
         ["bygg", "--dump-schema"],
         capture_output=True,
         encoding="utf-8",
     )
     assert process.returncode == 0
     assert process.stdout == snapshot
+
+
+def test_version():
+    process = subprocess.run(
+        ["bygg", "--version"],
+        capture_output=True,
+        encoding="utf-8",
+    )
+    assert process.returncode == 0
+    assert process.stdout[1:7] == " bygg "
+    # Version string looks something like this when developing:
+    # 🛈 bygg 0.3.3.dev5+g900af94
+    # Clean it and check if it seems valid. However, it will vary depending on what tags
+    # are set etc, so only do a rudimentary check for numbers in a major-minor pattern.
+    cleaned_version = process.stdout[7:].strip()
+    assert re.match(r"\d+\.\d+", cleaned_version)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bygg-0.3.2/tests/test_scheduler.py` & `bygg-0.4.0/tests/test_scheduler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from bygg.action import Action, CommandStatus
+from bygg.core.action import Action, ActionContext, CommandStatus
+import pytest
+
+pytestmark = pytest.mark.scheduler
 
 
 def test_scheduler_single_action(scheduler_single_action):
     scheduler, _ = scheduler_single_action
 
     assert scheduler.run_status() == "not started"
 
@@ -300,7 +303,136 @@
     job.status = CommandStatus(0, "Executed successfully", None)
     scheduler.job_finished(job)
 
     assert scheduler.run_status() == "finished"
 
     assert len(scheduler.build_actions) == 2
     assert len(scheduler.running_jobs) == 0
+
+
+def test_scheduler_single_file(scheduler_fixture, tmp_path):
+    scheduler, cache_file = scheduler_fixture
+
+    def action1(ctx: ActionContext):
+        for output in ctx.outputs:
+            with open(output, "w") as f:
+                f.write("file content")
+        return CommandStatus(0, "Executed successfully", None)
+
+    Action(
+        name="file",
+        is_entrypoint=True,
+        inputs=[],
+        outputs=[str(tmp_path / "file1")],
+        command=action1,
+    )
+
+    scheduler.start_run("file")
+
+    job = scheduler.get_ready_jobs(1)[0]
+    job.status = job.action.command(job.action)
+    scheduler.job_finished(job)
+
+    assert len(scheduler.job_graph) == 0
+    assert scheduler.run_status() == "finished"
+
+    scheduler.shutdown()
+
+    # Second run
+
+    scheduler.__init__()
+    scheduler.init_cache(cache_file)
+
+    Action(
+        name="file",
+        is_entrypoint=True,
+        inputs=[],
+        outputs=[str(tmp_path / "file1")],
+        command=action1,
+    )
+
+    scheduler.start_run("file")
+    job_list = scheduler.get_ready_jobs(1)
+
+    assert len(job_list) == 0
+    assert len(scheduler.job_graph) == 0
+    assert scheduler.run_status() == "finished"
+
+
+def test_scheduler_single_file_changed(scheduler_fixture, tmp_path):
+    scheduler, cache_file = scheduler_fixture
+    infile = tmp_path / "file0"
+    outfile = tmp_path / "file1"
+
+    def action1(ctx: ActionContext):
+        for output in ctx.outputs:
+            with open(output, "w") as f:
+                f.write("file content")
+        return CommandStatus(0, "Executed successfully", None)
+
+    Action(
+        name="file",
+        is_entrypoint=True,
+        inputs=[str(infile)],
+        outputs=[str(outfile)],
+        command=action1,
+    )
+
+    infile.write_text("infile content")
+
+    scheduler.start_run("file")
+
+    job = scheduler.get_ready_jobs(1)[0]
+    job.status = job.action.command(job.action)
+    scheduler.job_finished(job)
+
+    assert len(scheduler.job_graph) == 0
+    assert scheduler.run_status() == "finished"
+
+    scheduler.shutdown()
+
+    # Second run
+
+    scheduler.__init__()
+    scheduler.init_cache(cache_file)
+
+    Action(
+        name="file",
+        is_entrypoint=True,
+        inputs=[str(infile)],
+        outputs=[str(outfile)],
+        command=action1,
+    )
+
+    scheduler.start_run("file")
+    job_list = scheduler.get_ready_jobs(1)
+
+    assert len(job_list) == 0
+    assert len(scheduler.job_graph) == 0
+    assert scheduler.run_status() == "finished"
+
+    # Third run, modify input file
+
+    infile.write_text("modified infile content")
+
+    scheduler.__init__()
+    scheduler.init_cache(cache_file)
+
+    Action(
+        name="file",
+        is_entrypoint=True,
+        inputs=[str(infile)],
+        outputs=[str(outfile)],
+        command=action1,
+    )
+
+    scheduler.start_run("file")
+    job_list = scheduler.get_ready_jobs(1)
+
+    assert len(job_list) == 1
+    assert len(scheduler.job_graph) == 1
+
+    job.status = job.action.command(job.action)
+    scheduler.job_finished(job)
+
+    assert len(scheduler.job_graph) == 0
+    assert scheduler.run_status() == "finished"
```

### Comparing `bygg-0.3.2/tests/test_system_helpers.py` & `bygg-0.4.0/tests/test_system_helpers.py`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/tests/test_tree.py` & `bygg-0.4.0/tests/test_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bygg.tree import display_tree
+from bygg.cmd.tree import display_tree
 
 
 def test_tree_single_action(scheduler_single_action, capsys, snapshot):
     scheduler, _ = scheduler_single_action
     display_tree(scheduler, ["action1"])
     stdout, _ = capsys.readouterr()
     assert stdout == snapshot
```

### Comparing `bygg-0.3.2/tests/test_utils.py` & `bygg-0.4.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bygg.action import Action
+from bygg.core.action import Action
 from bygg.util import create_shell_command, filenames_from_pattern
 import pytest
 
 test_cases_filenames_from_pattern = [
     (
         (
             ["/foo/bar/baz.txt.j2"],
```

### Comparing `bygg-0.3.2/tests/__snapshots__/test_completions.ambr` & `bygg-0.4.0/tests/__snapshots__/test_completions.ambr`

 * *Files 10% similar despite different names*

```diff
@@ -135,27 +135,27 @@
 # name: test_actions_completions[trivial].2
   list([
     'transform',
   ])
 # ---
 # name: test_directory_completions[--directory ]
   list([
-    'examples/checks',
-    'examples/environments',
-    'examples/failing_jobs',
-    'examples/only_python',
-    'examples/parametric',
-    'examples/taskrunner',
-    'examples/trivial',
+    'checks',
+    'environments',
+    'failing_jobs',
+    'only_python',
+    'parametric',
+    'taskrunner',
+    'trivial',
   ])
 # ---
 # name: test_directory_completions[-C ]
   list([
-    'examples/checks',
-    'examples/environments',
-    'examples/failing_jobs',
-    'examples/only_python',
-    'examples/parametric',
-    'examples/taskrunner',
-    'examples/trivial',
+    'checks',
+    'environments',
+    'failing_jobs',
+    'only_python',
+    'parametric',
+    'taskrunner',
+    'trivial',
   ])
 # ---
```

### Comparing `bygg-0.3.2/tests/__snapshots__/test_job_output.ambr` & `bygg-0.4.0/tests/__snapshots__/test_job_output.ambr`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/tests/__snapshots__/test_main.ambr` & `bygg-0.4.0/tests/__snapshots__/test_main.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
           }
         },
         "required": [],
         "additionalProperties": false
       },
       "Environment": {
         "title": "Environment",
-        "description": "A class used to represent a virtual environment that actions can be run in.\n\nAttributes\n----------\nbyggfile : str\n    The Python Byggfile that uses this environment.\ninputs : List[str]\n    A list of files that are used as input to the environment. Typically pip\n    requirements files, but can be any files.\nvenv_directory : str\n    The directory where the virtual environment is located. Will be recreated by\n    Bygg if any of the inputs are modified.\nshell : str\n    The shell command for creating the environment.\ndescription : str, optional\n    A description of the environment. Used in e.g. help messages, by default None\nmessage : str, optional\n    A message related to the environment, by default None",
+        "description": "A class used to represent a virtual environment that actions can be run in.\n\nAttributes\n----------\nbyggfile : str\n    The Python Byggfile that uses this environment.\ninputs : list[str]\n    A list of files that are used as input to the environment. Typically pip\n    requirements files, but can be any files.\nvenv_directory : str\n    The directory where the virtual environment is located. Will be recreated by\n    Bygg if any of the inputs are modified.\nshell : str\n    The shell command for creating the environment.\ndescription : str, optional\n    A description of the environment. Used in e.g. help messages, by default None\nmessage : str, optional\n    A message related to the environment, by default None",
         "type": "object",
         "properties": {
           "byggfile": {
             "type": "string"
           },
           "inputs": {
             "type": "array",
```

### Comparing `bygg-0.3.2/LICENSE` & `bygg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bygg-0.3.2/README.md` & `bygg-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 
 @action(
     "build1",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"],
     is_entrypoint=True
 )
-def a_build_command(ctx: Context):
+def a_build_command(ctx: ActionContext):
     # do stuff
     ...
 
 
 # Separate function + Action constructor:
 
-def also_a_build_command(ctx: Context):
+def also_a_build_command(ctx: ActionContext):
     # do stuff
     ...
 
 Action(
     "build2",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"],
@@ -104,15 +104,15 @@
 Bygg has support for Bash and Zsh tab completions of arguments and entrypoint
 actions. The completions will be loaded:
 
 - from `Byggfile.py` if `Byggfile.yml` doesn't exist, or if there are no
   environments declared in `Byggfile.yml`.
 - from `Byggfile.yml` if it exists and has environments. In this case, only the
   entrypoint actions listed in `Byggfile.yml` will be loaded; no Python files
-  will be loaded to look for entrypoint actions since this might require an
+  will be loaded to look for entrypoint actions since this might require a
   lengthy (in the context) install of environments.
 
 To install completions, do:
 
 ```shell
 bygg --completions
 ```
@@ -153,19 +153,24 @@
 
 ## Getting a local copy
 
 If you want to try out the examples or even develop Bygg itself, Bygg can be
 tried out and worked on without installing it globally:
 
 First, clone this repo and cd into it, then execute the commands below.
-`bootstrap.py` creates a virtual environment and installs Bygg into it together
-with its dependencies.
+
+If [uv](https://github.com/astral-sh/uv) is installed (e.g. with `pipx install uv`),
+it will be used by `bootstrap.py` and the Bygg examples where relevant.
+This will speed up project setup and test running. If `uv` is not installed,
+regular `pip` will be used.
 
 ```shell
+# Create a virtual environment and install Bygg into it together with its dependencies:
 ./bootstrap.py
+# Activate the virtual environment:
 . .venv/bin/activate
 ```
 
 Now you can try out one of the examples:
 
 ```shell
 cd examples/trivial
@@ -190,15 +195,21 @@
 
 ```shell
 pytest
 ```
 
 With the virtual environment _deactivated_, the full test suite can be run with
 [Nox](https://nox.thea.codes/en/stable/). Nox should be installed outside of
-the virtual environment since it manages its own virtual environments:
+Bygg's virtual environment since it manages its own virtual environments:
+
+```shell
+pipx install nox
+```
+
+or
 
 ```shell
 pip install --user --upgrade nox
 ```
 
 After that, run tests with
```

### Comparing `bygg-0.3.2/pyproject.toml` & `bygg-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -30,23 +30,32 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 bygg = "bygg.main:main"
-gg = "bygg.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/rikardg/bygg"
 "Bug Tracker" = "https://github.com/rikardg/bygg/issues"
 
+[tool.pyright]
+include = ["src/bygg", "tests"]
+
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib", "tests/"]
+markers = [
+  "digest: Tests for digest functionality.",
+  "scheduler: Tests for the scheduler.",
+]
 
 [tool.ruff]
-extend-select = ["I"]
+exclude = ["_version.py"]
+
+[tool.ruff.lint]
+extend-select = ["I", "UP006"]
 ignore = ["E501"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 order-by-type = true
 force-sort-within-sections = true
```

### Comparing `bygg-0.3.2/PKG-INFO` & `bygg-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bygg
-Version: 0.3.2
+Version: 0.4.0
 Summary: A small build system
 Project-URL: Homepage, https://github.com/rikardg/bygg
 Project-URL: Bug Tracker, https://github.com/rikardg/bygg/issues
 Author-email: Rikard Gillemyr <rikard.gillemyr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 rikardg
@@ -27,15 +27,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: argcomplete==3.2.3
+Requires-Dist: argcomplete==3.3.0
 Requires-Dist: dill==0.3.8
 Requires-Dist: graph-theory==2023.7.6
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: pyyaml==6.0.1
 Description-Content-Type: text/markdown
 
@@ -101,22 +101,22 @@
 
 @action(
     "build1",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"],
     is_entrypoint=True
 )
-def a_build_command(ctx: Context):
+def a_build_command(ctx: ActionContext):
     # do stuff
     ...
 
 
 # Separate function + Action constructor:
 
-def also_a_build_command(ctx: Context):
+def also_a_build_command(ctx: ActionContext):
     # do stuff
     ...
 
 Action(
     "build2",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"],
@@ -145,15 +145,15 @@
 Bygg has support for Bash and Zsh tab completions of arguments and entrypoint
 actions. The completions will be loaded:
 
 - from `Byggfile.py` if `Byggfile.yml` doesn't exist, or if there are no
   environments declared in `Byggfile.yml`.
 - from `Byggfile.yml` if it exists and has environments. In this case, only the
   entrypoint actions listed in `Byggfile.yml` will be loaded; no Python files
-  will be loaded to look for entrypoint actions since this might require an
+  will be loaded to look for entrypoint actions since this might require a
   lengthy (in the context) install of environments.
 
 To install completions, do:
 
 ```shell
 bygg --completions
 ```
@@ -194,19 +194,24 @@
 
 ## Getting a local copy
 
 If you want to try out the examples or even develop Bygg itself, Bygg can be
 tried out and worked on without installing it globally:
 
 First, clone this repo and cd into it, then execute the commands below.
-`bootstrap.py` creates a virtual environment and installs Bygg into it together
-with its dependencies.
+
+If [uv](https://github.com/astral-sh/uv) is installed (e.g. with `pipx install uv`),
+it will be used by `bootstrap.py` and the Bygg examples where relevant.
+This will speed up project setup and test running. If `uv` is not installed,
+regular `pip` will be used.
 
 ```shell
+# Create a virtual environment and install Bygg into it together with its dependencies:
 ./bootstrap.py
+# Activate the virtual environment:
 . .venv/bin/activate
 ```
 
 Now you can try out one of the examples:
 
 ```shell
 cd examples/trivial
@@ -231,15 +236,21 @@
 
 ```shell
 pytest
 ```
 
 With the virtual environment _deactivated_, the full test suite can be run with
 [Nox](https://nox.thea.codes/en/stable/). Nox should be installed outside of
-the virtual environment since it manages its own virtual environments:
+Bygg's virtual environment since it manages its own virtual environments:
+
+```shell
+pipx install nox
+```
+
+or
 
 ```shell
 pip install --user --upgrade nox
 ```
 
 After that, run tests with
```

