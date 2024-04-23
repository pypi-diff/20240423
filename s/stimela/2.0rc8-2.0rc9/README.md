# Comparing `tmp/stimela-2.0rc8.tar.gz` & `tmp/stimela-2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimela-2.0rc8.tar", max compression
+gzip compressed data, was "stimela-2.0rc9.tar", max compression
```

## Comparing `stimela-2.0rc8.tar` & `stimela-2.0rc9.tar`

### file list

```diff
@@ -1,107 +1,110 @@
--rw-r--r--   0        0        0    18047 2024-01-24 12:19:06.058457 stimela-2.0rc8/LICENSE
--rw-r--r--   0        0        0      645 2024-01-24 12:19:06.058457 stimela-2.0rc8/README.rst
--rw-r--r--   0        0        0     1146 2024-01-24 12:19:06.062457 stimela-2.0rc8/pyproject.toml
--rw-r--r--   0        0        0     1605 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/__init__.py
--rw-r--r--   0        0        0     1824 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/basetypes.py
--rw-r--r--   0        0        0      161 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/cab_utils.py
--rw-r--r--   0        0        0    25023 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/cargo.py
--rw-r--r--   0        0        0    11458 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/configuratt/__init__.py
--rw-r--r--   0        0        0    10076 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/configuratt/cache.py
--rw-r--r--   0        0        0      501 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/configuratt/common.py
--rw-r--r--   0        0        0     9385 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/configuratt/deps.py
--rw-r--r--   0        0        0    16993 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/configuratt/resolvers.py
--rw-r--r--   0        0        0    25108 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/evaluator.py
--rw-r--r--   0        0        0     3107 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/exceptions.py
--rw-r--r--   0        0        0     3110 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/logging_utils.py
--rw-r--r--   0        0        0      423 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/proc_utils.py
--rw-r--r--   0        0        0     8499 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/schema_utils.py
--rw-r--r--   0        0        0    20331 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/substitutions.py
--rw-r--r--   0        0        0    13003 2024-01-24 12:19:06.062457 stimela-2.0rc8/scabha/validate.py
--rw-r--r--   0        0        0      886 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/__init__.py
--rw-r--r--   0        0        0     5188 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/__init__.py
--rw-r--r--   0        0        0    12964 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/docker.py
--rw-r--r--   0        0        0     4575 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/flavours/__init__.py
--rw-r--r--   0        0        0     1376 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/flavours/binary.py
--rw-r--r--   0        0        0     3373 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/flavours/casa.py
--rw-r--r--   0        0        0     8810 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/flavours/python_flavours.py
--rw-r--r--   0        0        0    10958 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/__init__.py
--rw-r--r--   0        0        0    10354 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/daskjob.py
--rw-r--r--   0        0        0    16707 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/infrastructure.py
--rw-r--r--   0        0        0    11952 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/kube_utils.py
--rw-r--r--   0        0        0    17276 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/pod_proxy.py
--rw-r--r--   0        0        0     3677 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/run_daskjob.py
--rw-r--r--   0        0        0    28246 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/kube/run_kube.py
--rw-r--r--   0        0        0      465 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/native/__init__.py
--rw-r--r--   0        0        0     4065 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/native/run_native.py
--rw-r--r--   0        0        0     7687 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/podman.py
--rw-r--r--   0        0        0     1584 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/runner.py
--rw-r--r--   0        0        0    13862 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/singularity.py
--rw-r--r--   0        0        0     5624 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/backends/utils.py
--rw-r--r--   0        0        0      249 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/cargo/__init__.py
--rw-r--r--   0        0        0        0 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/__init__.py
--rw-r--r--   0        0        0     2249 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/build.py
--rw-r--r--   0        0        0      832 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/cabs.py
--rw-r--r--   0        0        0     2026 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/cleanup.py
--rw-r--r--   0        0        0      643 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/containers.py
--rw-r--r--   0        0        0     5847 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/doc.py
--rw-r--r--   0        0        0     1681 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/images.py
--rw-r--r--   0        0        0      371 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/kill.py
--rw-r--r--   0        0        0      640 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/ps.py
--rw-r--r--   0        0        0     1338 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/pull.py
--rw-r--r--   0        0        0     1856 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/push.py
--rw-r--r--   0        0        0    13831 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/run.py
--rw-r--r--   0        0        0     2627 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/commands/save_config.py
--rw-r--r--   0        0        0    10660 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/config.py
--rw-r--r--   0        0        0     1826 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/kitchen/__init__.py
--rw-r--r--   0        0        0      555 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/kitchen/batch.py
--rw-r--r--   0        0        0    20491 2024-01-24 12:19:06.062457 stimela-2.0rc8/stimela/kitchen/cab.py
--rw-r--r--   0        0        0    63533 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/kitchen/recipe.py
--rw-r--r--   0        0        0    30596 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/kitchen/step.py
--rw-r--r--   0        0        0    11350 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/kitchen/wranglers.py
--rw-r--r--   0        0        0     4913 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/main.py
--rw-r--r--   0        0        0       29 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/schedulers/__init__.py
--rw-r--r--   0        0        0     2238 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/schedulers/slurm.py
--rw-r--r--   0        0        0      215 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/stimela.conf
--rw-r--r--   0        0        0    15458 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/stimelogging.py
--rw-r--r--   0        0        0    13213 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/task_stats.py
--rw-r--r--   0        0        0      254 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/utils/__init__.py
--rw-r--r--   0        0        0     7438 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/utils/xrun_asyncio.py
--rw-r--r--   0        0        0     9181 2024-01-24 12:19:06.066457 stimela-2.0rc8/stimela/utils/xrun_poll.py
--rw-r--r--   0        0        0        0 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/__init__.py
--rw-r--r--   0        0        0     1965 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_configuratt.py
--rw-r--r--   0        0        0      540 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_dynschema.py
--rw-r--r--   0        0        0       70 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_include.yaml
--rw-r--r--   0        0        0       46 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_include2.yaml
--rw-r--r--   0        0        0       21 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_nest_a.yml
--rw-r--r--   0        0        0       21 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_nest_b.yml
--rw-r--r--   0        0        0       25 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_nest_c.yml
--rw-r--r--   0        0        0     1659 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_parsing.py
--rw-r--r--   0        0        0      658 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_schema.py
--rw-r--r--   0        0        0       55 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_schema.yaml
--rw-r--r--   0        0        0     5896 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/test_substitutions.py
--rw-r--r--   0        0        0      924 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/scabha_tests/testconf.yaml
--rw-r--r--   0        0        0        0 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/__init__.py
--rw-r--r--   0        0        0      240 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/example_callable.py
--rw-r--r--   0        0        0      541 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/example_dynschema.py
--rw-r--r--   0        0        0     1428 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_aliasing.yml
--rw-r--r--   0        0        0      735 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_backends.yml
--rw-r--r--   0        0        0      554 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_callables.py
--rw-r--r--   0        0        0     2033 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_callables.yml
--rw-r--r--   0        0        0     1136 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_casa.yml
--rw-r--r--   0        0        0      172 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_dask_storage_options.yaml
--rw-r--r--   0        0        0      646 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_kube.yml
--rw-r--r--   0        0        0     1485 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_kube_config.yml
--rw-r--r--   0        0        0     2228 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_kube_qc.yml
--rw-r--r--   0        0        0      862 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_kube_scatter.yml
--rw-r--r--   0        0        0     2033 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_loop_recipe.yml
--rw-r--r--   0        0        0     2154 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_loop_recipe_slurm.yml
--rw-r--r--   0        0        0     4408 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_nesting.yml
--rw-r--r--   0        0        0     3441 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_recipe.py
--rw-r--r--   0        0        0     4136 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_recipe.yml
--rw-r--r--   0        0        0     1390 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_scatter.yml
--rw-r--r--   0        0        0     1882 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_wranglers.py
--rw-r--r--   0        0        0      205 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_wranglers.txt
--rw-r--r--   0        0        0     3010 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_wranglers.yml
--rw-r--r--   0        0        0     1273 2024-01-24 12:19:06.066457 stimela-2.0rc8/tests/stimela_tests/test_xrun.yml
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 stimela-2.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    18047 2024-02-05 13:15:00.597773 stimela-2.0rc9/LICENSE
+-rw-r--r--   0        0        0      645 2024-02-05 13:15:00.597773 stimela-2.0rc9/README.rst
+-rw-r--r--   0        0        0     1150 2024-02-05 13:15:00.601773 stimela-2.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     1605 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/__init__.py
+-rw-r--r--   0        0        0     1824 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/basetypes.py
+-rw-r--r--   0        0        0      161 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/cab_utils.py
+-rw-r--r--   0        0        0    25277 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/cargo.py
+-rw-r--r--   0        0        0    11458 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/configuratt/__init__.py
+-rw-r--r--   0        0        0    10076 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/configuratt/cache.py
+-rw-r--r--   0        0        0      501 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/configuratt/common.py
+-rw-r--r--   0        0        0     9385 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/configuratt/deps.py
+-rw-r--r--   0        0        0    16993 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/configuratt/resolvers.py
+-rw-r--r--   0        0        0    25108 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/evaluator.py
+-rw-r--r--   0        0        0     3107 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/exceptions.py
+-rw-r--r--   0        0        0     3110 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/logging_utils.py
+-rw-r--r--   0        0        0      423 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/proc_utils.py
+-rw-r--r--   0        0        0     8679 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/schema_utils.py
+-rw-r--r--   0        0        0    20331 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/substitutions.py
+-rw-r--r--   0        0        0    13345 2024-02-05 13:15:00.601773 stimela-2.0rc9/scabha/validate.py
+-rw-r--r--   0        0        0      886 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/__init__.py
+-rw-r--r--   0        0        0     5481 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/__init__.py
+-rw-r--r--   0        0        0    12975 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/docker.py
+-rw-r--r--   0        0        0     4575 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/flavours/__init__.py
+-rw-r--r--   0        0        0     1376 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/flavours/binary.py
+-rw-r--r--   0        0        0     3373 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/flavours/casa.py
+-rw-r--r--   0        0        0     8810 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/flavours/python_flavours.py
+-rw-r--r--   0        0        0    11278 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/__init__.py
+-rw-r--r--   0        0        0    10486 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/daskjob.py
+-rw-r--r--   0        0        0    16707 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/infrastructure.py
+-rw-r--r--   0        0        0    11952 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/kube_utils.py
+-rw-r--r--   0        0        0    17276 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/pod_proxy.py
+-rw-r--r--   0        0        0     3677 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/run_daskjob.py
+-rw-r--r--   0        0        0    28445 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/kube/run_kube.py
+-rw-r--r--   0        0        0      476 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/native/__init__.py
+-rw-r--r--   0        0        0     4353 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/native/run_native.py
+-rw-r--r--   0        0        0     7698 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/podman.py
+-rw-r--r--   0        0        0     3167 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/runner.py
+-rw-r--r--   0        0        0    15645 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/singularity.py
+-rw-r--r--   0        0        0     2935 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/slurm.py
+-rw-r--r--   0        0        0     5967 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/backends/utils.py
+-rw-r--r--   0        0        0      249 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/cargo/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/commands/__init__.py
+-rw-r--r--   0        0        0     2386 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/commands/build.py
+-rw-r--r--   0        0        0      832 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/commands/cabs.py
+-rw-r--r--   0        0        0     2026 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/commands/cleanup.py
+-rw-r--r--   0        0        0      643 2024-02-05 13:15:00.601773 stimela-2.0rc9/stimela/commands/containers.py
+-rw-r--r--   0        0        0     5847 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/doc.py
+-rw-r--r--   0        0        0     1681 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/images.py
+-rw-r--r--   0        0        0      371 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/kill.py
+-rw-r--r--   0        0        0      640 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/ps.py
+-rw-r--r--   0        0        0     1338 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/pull.py
+-rw-r--r--   0        0        0     1856 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/push.py
+-rw-r--r--   0        0        0    14992 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/run.py
+-rw-r--r--   0        0        0     2627 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/commands/save_config.py
+-rw-r--r--   0        0        0    10660 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/config.py
+-rw-r--r--   0        0        0     1826 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/__init__.py
+-rw-r--r--   0        0        0      555 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/batch.py
+-rw-r--r--   0        0        0    20491 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/cab.py
+-rw-r--r--   0        0        0    66256 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/recipe.py
+-rw-r--r--   0        0        0    31767 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/step.py
+-rw-r--r--   0        0        0    11350 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/kitchen/wranglers.py
+-rw-r--r--   0        0        0     5046 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/main.py
+-rw-r--r--   0        0        0       29 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/schedulers/__init__.py
+-rw-r--r--   0        0        0     2238 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/schedulers/slurm.py
+-rw-r--r--   0        0        0      215 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/stimela.conf
+-rw-r--r--   0        0        0    15541 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/stimelogging.py
+-rw-r--r--   0        0        0    14187 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/task_stats.py
+-rw-r--r--   0        0        0      254 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/utils/__init__.py
+-rw-r--r--   0        0        0     7479 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/utils/xrun_asyncio.py
+-rw-r--r--   0        0        0     9181 2024-02-05 13:15:00.605773 stimela-2.0rc9/stimela/utils/xrun_poll.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/__init__.py
+-rw-r--r--   0        0        0     1965 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_configuratt.py
+-rw-r--r--   0        0        0      540 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_dynschema.py
+-rw-r--r--   0        0        0       70 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_include.yaml
+-rw-r--r--   0        0        0       46 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_include2.yaml
+-rw-r--r--   0        0        0       21 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_nest_a.yml
+-rw-r--r--   0        0        0       21 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_nest_b.yml
+-rw-r--r--   0        0        0       25 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_nest_c.yml
+-rw-r--r--   0        0        0     1659 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_parsing.py
+-rw-r--r--   0        0        0      658 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_schema.py
+-rw-r--r--   0        0        0       55 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_schema.yaml
+-rw-r--r--   0        0        0     5896 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/test_substitutions.py
+-rw-r--r--   0        0        0      924 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/scabha_tests/testconf.yaml
+-rw-r--r--   0        0        0        0 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/__init__.py
+-rw-r--r--   0        0        0      240 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/example_callable.py
+-rw-r--r--   0        0        0      541 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/example_dynschema.py
+-rw-r--r--   0        0        0     1428 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_aliasing.yml
+-rw-r--r--   0        0        0      735 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_backends.yml
+-rw-r--r--   0        0        0      554 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_callables.py
+-rw-r--r--   0        0        0     2033 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_callables.yml
+-rw-r--r--   0        0        0     1136 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_casa.yml
+-rw-r--r--   0        0        0      172 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_dask_storage_options.yaml
+-rw-r--r--   0        0        0      646 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_kube.yml
+-rw-r--r--   0        0        0     1485 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_kube_config.yml
+-rw-r--r--   0        0        0     2228 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_kube_qc.yml
+-rw-r--r--   0        0        0      862 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_kube_scatter.yml
+-rw-r--r--   0        0        0     2033 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_loop_recipe.yml
+-rw-r--r--   0        0        0     2154 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_loop_recipe_slurm.yml
+-rw-r--r--   0        0        0     4408 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_nesting.yml
+-rw-r--r--   0        0        0     3441 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_recipe.py
+-rw-r--r--   0        0        0     4136 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_recipe.yml
+-rw-r--r--   0        0        0     1390 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_scatter.yml
+-rw-r--r--   0        0        0      905 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_slurm.yml
+-rw-r--r--   0        0        0        0 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_slurm_config.yml
+-rw-r--r--   0        0        0     1882 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_wranglers.py
+-rw-r--r--   0        0        0      205 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_wranglers.txt
+-rw-r--r--   0        0        0     3010 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_wranglers.yml
+-rw-r--r--   0        0        0     1273 2024-02-05 13:15:00.605773 stimela-2.0rc9/tests/stimela_tests/test_xrun.yml
+-rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 stimela-2.0rc9/PKG-INFO
```

### Comparing `stimela-2.0rc8/LICENSE` & `stimela-2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/README.rst` & `stimela-2.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/pyproject.toml` & `stimela-2.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "stimela"
-version = "2.0rc8"
-description = "Framework for system agnostic pipelines for radio interferometry arrays"
+version = "2.0rc9"
+description = "Framework for system agnostic pipelines for (not just) radio interferometry"
 authors = ["Sphesihle Makhathini <sphemakh@gmail.com>", "Oleg Smirnov and RATT <osmirnov@gmail.com>"]
 readme = "README.rst"
 license = "GNU GPL v2"
 include = [{ path = "tests" }]
 packages = [
     {include = "stimela"},
     {include = "scabha"},
```

### Comparing `stimela-2.0rc8/scabha/__init__.py` & `stimela-2.0rc9/scabha/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/basetypes.py` & `stimela-2.0rc9/scabha/basetypes.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/cargo.py` & `stimela-2.0rc9/scabha/cargo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import re, importlib, sys
 from collections import OrderedDict
 from enum import Enum, IntEnum
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from omegaconf import MISSING, ListConfig, DictConfig, OmegaConf
 
 import rich.box
 import rich.markup
 from rich.table import Table
 from rich.markdown import Markdown
 
@@ -120,16 +120,21 @@
 
     # default value
     default: Any = _UNSET_DEFAULT
 
     # list of aliases for this parameter (i.e. references to other parameters whose schemas/values this parameter shares)
     aliases: Optional[List[str]] = ()
 
-    # if true, treat parameter as a path, and ensure that the parent directories it refers to exist
-    mkdir: bool = False
+    # if true, create parent directories of file-type outputs if needed
+    mkdir: bool = True
+
+    # if True, and parameter is a path, access to its parent directory is required
+    access_parent_dir: bool = False
+    # if True, and parameter is a path, access to its parent directory is required in writable mode
+    write_parent_dir: bool = False
 
     # for file and dir-type parameters: if True, the file(s)/dir(s) must exist. If False, they can be missing.
     # if None, then the default logic applies: inputs must exist, and outputs don't
     must_exist: Optional[bool] = None
 
     # for file and dir-type parameters: if True, ignore them when making processing logic decisions based on file freshness
     skip_freshness_checks: Optional[bool] = None
@@ -137,15 +142,15 @@
     # For output File-type parameters. If True, and the output exists, remove before running
     remove_if_exists: bool = False
 
     # if command-line option for underlying binary has a different name, specify it here
     nom_de_guerre: Optional[str] = None
 
     # policies object, specifying a non-default way to handle this parameter
-    policies: ParameterPolicies = ParameterPolicies()
+    policies: ParameterPolicies = field(default_factory=ParameterPolicies)
 
     # Parameter category, purely cosmetic, used for generating help and debug messages.
     # Assigned automatically if None, but a schema may explicitly mark parameters as e.g.
     # "obscure" or "hidden"
     category: Optional[ParameterCategory] = None
 
     # metavar corresponding to this parameter. Used when constructing command-line interfaces
```

### Comparing `stimela-2.0rc8/scabha/configuratt/__init__.py` & `stimela-2.0rc9/scabha/configuratt/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/configuratt/cache.py` & `stimela-2.0rc9/scabha/configuratt/cache.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/configuratt/deps.py` & `stimela-2.0rc9/scabha/configuratt/deps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/configuratt/resolvers.py` & `stimela-2.0rc9/scabha/configuratt/resolvers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/evaluator.py` & `stimela-2.0rc9/scabha/evaluator.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/exceptions.py` & `stimela-2.0rc9/scabha/exceptions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/logging_utils.py` & `stimela-2.0rc9/scabha/logging_utils.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/schema_utils.py` & `stimela-2.0rc9/scabha/schema_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     fields = []
 
     # convert per-section schemas into dataclasses and make list of fields for outer dataclass
     for section, content in nested.items():
         dcls = schema_to_dataclass(content, f"{class_name}_{section}",
                                     bases=section_bases, post_init=post_init_map.get(section))
 
-        fields.append((section, dcls, field(default=dcls())))
+        fields.append((section, dcls, field(default_factory=dcls)))
 
     # return the outer dataclass
     return make_dataclass(class_name, fields, bases=bases)
 
 
 _atomic_types = dict(bool=bool, str=str, int=int, float=float)
 
@@ -140,14 +140,17 @@
     if type(schemas) is str:
         schemas = OmegaConf.merge(OmegaConf.structured(Schema), 
                                OmegaConf.load(schemas))
 
     decorator_chain = None
     for io in schemas.inputs, schemas.outputs:
         for name, schema in io.items():
+            # skip outputs, unless they're named outputs
+            if io is schemas.outputs and not (schema.is_file_type and not schema.implicit):
+                continue
 
             name = name.replace("_", "-")
             optname = f"--{name}"
             dtype = schema.dtype
             validator = None
 
             # sort out option type. Atomic type?
```

### Comparing `stimela-2.0rc8/scabha/substitutions.py` & `stimela-2.0rc9/scabha/substitutions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/scabha/validate.py` & `stimela-2.0rc9/scabha/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 inputs[name] = OmegaConf.to_container(value)
 
     dcls = dataclasses.make_dataclass("Parameters", fields)
 
     # convert this to a pydantic dataclass which does validation
     pcls = pydantic.dataclasses.dataclass(dcls)
 
-    # check Files etc. and expand globs
+    # check Files etc. 
     for name, value in list(inputs.items()):
         # get schema from those that need validation, skip if not in schemas
         schema = schemas.get(name)
         if schema is None:
             continue
         # skip errors
         if value is UNSET or isinstance(value, Error):
@@ -223,14 +223,16 @@
                         files = [value]
                 except Exception as exc:
                     files = [value]
             elif isinstance(value, (list, tuple)):
                 files = value
             else:
                 raise ParameterValidationError(f"'{mkname(name)}={value}': invalid type '{type(value)}'")
+            # expand ~
+            files = [os.path.expanduser(f) for f in files]
           
             # check for existence of all files in list, if needed
             if must_exist: 
                 if not files:
                     raise ParameterValidationError(f"'{mkname(name)}': file(s) don't exist")
                 not_exists = [f for f in files if not os.path.exists(f)]
                 if not_exists:
@@ -285,16 +287,24 @@
         schema = schemas[name]
         if schema.choices and value not in schema.choices:
             raise ParameterValidationError(f"{mkname(name)}: invalid value '{value}'")
 
     # check for mkdir directives
     if create_dirs:
         for name, value in validated.items():
-            if schemas[name].mkdir and isinstance(value, str):
-                dirname = os.path.dirname(value)
-                if dirname and not os.path.exists(dirname):
-                    os.makedirs(dirname, exist_ok=True)
+            schema = schemas[name]
+            if schema.is_output and schema.mkdir:
+                if schema.is_file_type:
+                    files = [value]
+                elif schema.is_file_list_type:
+                    files = value
+                else:
+                    continue
+                for path in files:
+                    dirname = os.path.dirname(path)
+                    if dirname and not os.path.exists(dirname):
+                        os.makedirs(dirname, exist_ok=True)
 
     # add in unresolved values
     validated.update(**unresolved)
 
     return validated
```

### Comparing `stimela-2.0rc8/stimela/__init__.py` & `stimela-2.0rc9/stimela/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/__init__.py` & `stimela-2.0rc9/stimela/backends/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,34 @@
 from stimela.exceptions import BackendSpecificationError, BackendError
 from stimela.stimelogging import log_exception
 from scabha.basetypes import EmptyDictDefault
 
 from .singularity import SingularityBackendOptions
 from .kube import KubeBackendOptions
 from .native import NativeBackendOptions
+from .slurm import SlurmOptions
 
 import stimela
 
 ## left as memo to self
 # Backend = Enum("Backend", "docker singularity podman kubernetes native", module=__name__)
 Backend = Enum("Backend", "singularity kube native", module=__name__)
 
 SUPPORTED_BACKENDS = set(Backend.__members__)
 
 
-def get_backend(name: str):
+def get_backend(name: str, backend_opts: Optional[Dict] = None):
+    """
+    Gets backend, given a name and an optional set of options for that backend.
+    Returns backend module, or None if it is not available.
+    """
     if name not in SUPPORTED_BACKENDS:
         return None
     backend = __import__(f"stimela.backends.{name}", fromlist=[name])
-    if backend.is_available():
+    if backend.is_available(backend_opts):
         return backend
     return None
 
 
 def get_backend_status(name: str):
     if name not in SUPPORTED_BACKENDS:
         return "unknown backend"
@@ -44,15 +49,15 @@
     
     select: Any = ""   # should be Union[str, List[str]], but OmegaConf doesn't support it, so handle in __post_init__ for now
     
     singularity: Optional[SingularityBackendOptions] = None
     kube: Optional[KubeBackendOptions] = None
     native: Optional[NativeBackendOptions] = None 
     docker: Optional[Dict] = None  # placeholder for future impl
-    slurm: Optional[Dict] = None   # placeholder for future impl
+    slurm: Optional[SlurmOptions] = None   
 
     ## Resource limits applied during run -- see resource module
     rlimits: Dict[str, Any] = EmptyDictDefault()
 
     def __post_init__(self):
         # resolve "select" field
         if type(self.select) is str:
@@ -67,14 +72,16 @@
         # provide default options for available backends
         if self.singularity is None and get_backend("singularity"):
             self.singularity = SingularityBackendOptions()
         if self.native is None and get_backend("native"):
             self.native = NativeBackendOptions()
         if self.kube is None and get_backend("kube"):
             self.kube = KubeBackendOptions()
+        if self.slurm is None:
+            self.slurm = SlurmOptions()
 
 StimelaBackendSchema = OmegaConf.structured(StimelaBackendOptions)
 
 
 def resolve_image_name(backend: StimelaBackendOptions, image: 'stimela.kitchen.Cab.ImageInfo'):
     """
     Resolves image name -- applies override registries, if any exist
@@ -102,15 +109,15 @@
     if type(selected) is str:
         selected = [selected]
 
     for engine in selected: 
         # check that backend has not been disabled
         opts = getattr(backend_opts, engine, None)
         if not opts or opts.enable:
-            backend = get_backend(engine)
+            backend = get_backend(engine, opts)
             func = backend and getattr(backend, method, None)
             if func:
                 try:
                     func(backend_opts, log)
                 except BackendError as exc:
                     exc1 = BackendError(f"error {desc} {engine} backend", exc)
                     if raise_exc:
```

### Comparing `stimela-2.0rc8/stimela/backends/docker.py` & `stimela-2.0rc9/stimela/backends/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import stimela
 from stimela.exceptions import *
 from stimela import log_exception
 
 STATUS = VERSION = BINARY = None
 
-def is_available():
+def is_available(opts = None):
     global STATUS, VERSION, BINARY
     if STATUS is None:
         BINARY = which("docker")
         if BINARY:
             __version_string = subprocess.check_output([BINARY, "--version"]).decode("utf8")
             STATUS = VERSION = __version_string.strip().split()[-1]
             # if VERSION < "3.0.0":
```

### Comparing `stimela-2.0rc8/stimela/backends/flavours/__init__.py` & `stimela-2.0rc9/stimela/backends/flavours/__init__.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/flavours/binary.py` & `stimela-2.0rc9/stimela/backends/flavours/binary.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/flavours/casa.py` & `stimela-2.0rc9/stimela/backends/flavours/casa.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/flavours/python_flavours.py` & `stimela-2.0rc9/stimela/backends/flavours/python_flavours.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/kube/__init__.py` & `stimela-2.0rc9/stimela/backends/kube/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Any
+from typing import Dict, List, Optional, Any, Callable
 from enum import Enum
 from omegaconf import OmegaConf
 from dataclasses import dataclass
 import time
 import yaml
 import json
 import secrets
@@ -32,60 +32,14 @@
 except ImportError:
     AVAILABLE = False
     STATUS = "please reinstall with the optional kube dependency (stimela[kube])"
 
     def run(*args, **kw):
         raise RuntimeError(f"kubernetes backend {STATUS}")
     
-def is_available():
-    return AVAILABLE
-
-def get_status():
-    return STATUS
-
-def is_remote():
-    return True
-
-def init(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
-    from . import infrastructure
-    global AVAILABLE, STATUS
-    if not infrastructure.init(backend, log):
-        AVAILABLE = False
-        STATUS = "initialization error"
-
-def close(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
-    from . import infrastructure
-    if AVAILABLE:
-        infrastructure.close(backend, log)
-
-def cleanup(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
-    from . import infrastructure
-    infrastructure.cleanup(backend, log)
-
-def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
-        backend: 'stimela.backend.StimelaBackendOptions',
-        log: logging.Logger, subst: Optional[Dict[str, Any]] = None):
-    from . import run_kube
-    return run_kube.run(cab=cab, params=params, fqname=fqname, backend=backend, log=log, subst=subst)
-
-_kube_client = _kube_config = _kube_context = None
-
-def get_kube_api(context: Optional[str]=None):
-    global _kube_client
-    global _kube_config
-    global _kube_context
-
-    if _kube_config is None:
-        _kube_config = True
-        _kube_context = context
-        kubernetes.config.load_kube_config(context=context)
-    elif context != _kube_context:
-        raise BackendError(f"k8s context has changed (was {_kube_context}, now {context}), this is not permitted")
-
-    return core_v1_api.CoreV1Api(), CustomObjectsApi()
 
 
 # dict of methods for converting an object to text format
 InjectedFileFormatters = dict(
     yaml = yaml.dump,
     json = json.dumps,
     txt = str
@@ -106,16 +60,14 @@
     type:           Optional[str] = None
     # memory limit/requirement
     memory:         Optional[PodLimits] = None
     cpu:            Optional[PodLimits] = None
     # arbitrary additional structure copied into the pod spec
     custom_pod_spec:  Dict[str, Any] = EmptyDictDefault()
 
-
-
 @dataclass
 class KubeBackendOptions(object):
     """
     Kube backend options class. Note that this can be defined globally in options, and 
     redefined/augmented at cab and step level.
     """
 
@@ -182,14 +134,15 @@
     @dataclass
     class DaskCluster(object):
         capture_logs: bool = True
         capture_logs_style: Optional[str] = "blue"
         name: Optional[str] = None
         num_workers: int = 0
         threads_per_worker: int = 1
+        memory_limit: Optional[str] = None
         worker_pod: KubePodSpec = KubePodSpec()
         scheduler_pod: KubePodSpec = KubePodSpec()
         forward_dashboard_port: int = 8787          # set to non-0 to forward the http dashboard to this local port
 
     @dataclass
     class FileInjection(object):
         format: InjectedFileFormats = "txt"
@@ -263,14 +216,65 @@
     user: UserInfo = UserInfo()
     
     # user-defined set of pod types -- each is a pod spec structure keyed by pod_type
     predefined_pod_specs: Dict[str, Dict[str, Any]] = EmptyDictDefault()
 
 
 KubeBackendSchema = OmegaConf.structured(KubeBackendOptions)
+    
+def is_available(opts: Optional[KubeBackendOptions]= None):
+    return AVAILABLE
+
+def get_status():
+    return STATUS
+
+def is_remote():
+    return True
+
+def init(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
+    from . import infrastructure
+    global AVAILABLE, STATUS
+    if not infrastructure.init(backend, log):
+        AVAILABLE = False
+        STATUS = "initialization error"
+
+def close(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
+    from . import infrastructure
+    if AVAILABLE:
+        infrastructure.close(backend, log)
+
+def cleanup(backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger):
+    from . import infrastructure
+    infrastructure.cleanup(backend, log)
+
+def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
+        backend: 'stimela.backend.StimelaBackendOptions',
+        log: logging.Logger, subst: Optional[Dict[str, Any]] = None,
+        command_wrapper: Optional[Callable] = None):
+    # normally runner.py won't allow this, but check just in case
+    if command_wrapper:
+        raise BackendError(f"kube backend cannot be used with a command wrapper")
+    from . import run_kube
+    return run_kube.run(cab=cab, params=params, fqname=fqname, backend=backend, log=log, subst=subst)
+
+_kube_client = _kube_config = _kube_context = None
+
+def get_kube_api(context: Optional[str]=None):
+    global _kube_client
+    global _kube_config
+    global _kube_context
+
+    if _kube_config is None:
+        _kube_config = True
+        _kube_context = context
+        kubernetes.config.load_kube_config(context=context)
+    elif context != _kube_context:
+        raise BackendError(f"k8s context has changed (was {_kube_context}, now {context}), this is not permitted")
+
+    return core_v1_api.CoreV1Api(), CustomObjectsApi()
 
 _uid = os.getuid()
 _gid = os.getgid()
 
 session_user_info = KubeBackendOptions.UserInfo(
     name=session_user,
     group=grp.getgrgid(_gid).gr_name,
```

### Comparing `stimela-2.0rc8/stimela/backends/kube/daskjob.py` & `stimela-2.0rc9/stimela/backends/kube/daskjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     p.add_argument(
         "-s",
         "--service-account",
         default="compute-runner",
         help="The kubernetes service account which will run the job",
     )
     p.add_argument(
+        "--pull-policy",
+        default="Always",
+        help="imagePullPolicy setting for pods",
+    )
+    p.add_argument(
         "-f",
         "--mount-file",
         nargs="*",
         help=(
             "Configuration files that will be mounted into the pod. "
             "Can be of the form /path/to/file.yaml or "
             "/host/file.yaml:/container/file.yaml. "
@@ -127,15 +132,15 @@
                                     "env": [
                                         {
                                             "name": "SCHEDULER_ENV",
                                             "value": "hello-world",
                                         }
                                     ],
                                     "image": args.image,
-                                    "imagePullPolicy": "IfNotPresent",
+                                    "imagePullPolicy": args.pull_policy,
                                     "livenessProbe": {
                                         "httpGet": {
                                             "path": "/health",
                                             "port": "http-dashboard",
                                         },
                                         "initialDelaySeconds": 15,
                                         "periodSeconds": 20,
@@ -180,29 +185,29 @@
                                         "--memory-limit", str(args.memory_limit),
                                         "$(DASK_SCHEDULER_ADDRESS)",
                                     ],
                                     "env": [
                                         {"name": "WORKER_ENV", "value": "hello-world"}
                                     ],
                                     "image": args.image,
-                                    "imagePullPolicy": "IfNotPresent",
+                                    "imagePullPolicy": args.pull_policy,
                                     "name": "worker",
                                 }
                             ],
                         },
                     },
                 }
             },
             "job": {
                 "metadata": { "labels": labels},
                 "spec": {
                     "containers": [
                         {
                             "image": args.image,
-                            "imagePullPolicy": "IfNotPresent",
+                            "imagePullPolicy": args.pull_policy,
                             "name": "job",
                         }
                     ],
                 }
             },
         },
     }
```

### Comparing `stimela-2.0rc8/stimela/backends/kube/infrastructure.py` & `stimela-2.0rc9/stimela/backends/kube/infrastructure.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/kube/kube_utils.py` & `stimela-2.0rc9/stimela/backends/kube/kube_utils.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/kube/pod_proxy.py` & `stimela-2.0rc9/stimela/backends/kube/pod_proxy.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/kube/run_daskjob.py` & `stimela-2.0rc9/stimela/backends/kube/run_daskjob.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/backends/kube/run_kube.py` & `stimela-2.0rc9/stimela/backends/kube/run_kube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging, time, json, datetime, os.path, pathlib, secrets, shlex
-from typing import Dict, Optional, Any, List
+from typing import Dict, Optional, Any, List, Callable
 from dataclasses import fields
 from datetime import timedelta
 from requests import ConnectionError
 from urllib3.exceptions import HTTPError
 import threading, subprocess
 import rich
 import traceback
@@ -40,21 +40,21 @@
         subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
 
     Returns:
         Any: return value (e.g. exit code) of content
     """
 
     if not cab.image:
-        raise StimelaCabRuntimeError(f"kube runner requires cab.image to be set")
+        raise BackendError(f"kube backend requires cab.image to be set")
 
     kube = backend.kube
 
     namespace = kube.namespace
     if not namespace:
-        raise StimelaCabRuntimeError(f"runtime.kube.namespace must be set")
+        raise BackendError(f"runtime.kube.namespace must be set")
 
     args = cab.flavour.get_arguments(cab, params, subst, check_executable=False)
     log.debug(f"command line is {args}")
 
     cabstat = cab.reset_status()
 
     command_name = cab.flavour.command_name
@@ -133,15 +133,17 @@
                 from . import daskjob
                 dask_job_name = f"dj-{token_hex}"
                 dask_job_spec = daskjob.render(OmegaConf.create(dict(
                     job_name=dask_job_name,
                     labels=pod_labels,
                     namespace=namespace,
                     image=image_name,
-                    memory_limit=kube.dask_cluster.worker_pod.memory and kube.dask_cluster.worker_pod.memory.limit,
+                    pull_policy='Always' if kube.always_pull_images else 'IfNotPresent',
+                    memory_limit=kube.dask_cluster.memory_limit if kube.dask_cluster.memory_limit is not None 
+                                    else kube.dask_cluster.worker_pod.memory and kube.dask_cluster.worker_pod.memory.limit,
                     nworkers=kube.dask_cluster.num_workers,
                     threads_per_worker=kube.dask_cluster.threads_per_worker,
                     # cmdline=["/bin/sh", "-c", "while true;do date;sleep 5; done"],
                     service_account=kube.service_account,
                     mount_file=None,
                 )))
```

### Comparing `stimela-2.0rc8/stimela/backends/native/run_native.py` & `stimela-2.0rc9/stimela/backends/native/run_native.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging, datetime, resource, os.path
 
-from typing import Dict, Optional, Any, List
+from typing import Dict, Optional, Any, List, Callable
 
 import stimela
 import stimela.kitchen
 from stimela.utils.xrun_asyncio import xrun
 from stimela.exceptions import StimelaProcessRuntimeError, BackendSpecificationError
 from scabha.substitutions import substitutions_from
 
@@ -33,22 +33,26 @@
 def build_command_line(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], subst: Optional[Dict[str, Any]] = None,
                         virtual_env: Optional[str] = None):
     return cab.flavour.get_arguments(cab, params, subst, virtual_env=virtual_env)
 
 
 def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
         backend: 'stimela.backend.StimelaBackendOptions',
-        log: logging.Logger, subst: Optional[Dict[str, Any]] = None):
-    """Runs cab contents
+        log: logging.Logger, subst: Optional[Dict[str, Any]] = None,
+        command_wrapper: Optional[Callable] = None):
+    """
+    Runs cab contents
 
     Args:
-        cab (Cab): cab object
+        cab: cab object
+        params: cab parameters
+        backend: backed settings object
         log (logger): logger to use
         subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
-
+        command_wrapper (Callable): takes a list of args and returns modified list of args
     Returns:
         Any: return value (e.g. exit code) of content
     """
     update_rlimits(backend.rlimits, log)
 
     venv = search = None
     if backend.native and backend.native.virtual_env:
@@ -75,14 +79,17 @@
     # run command
     start_time = datetime.datetime.now()
     def elapsed(since=None):
         """Returns string representing elapsed time"""
         return str(datetime.datetime.now() - (since or start_time)).split('.', 1)[0]
 
     # log.info(f"argument lengths are {[len(a) for a in args]}")
+    
+    if command_wrapper:
+        args = command_wrapper(args)
 
     retcode = xrun(args[0], args[1:], shell=False, log=log,
                 output_wrangler=cabstat.apply_wranglers,
                 return_errcode=True, command_name=command_name, 
                 gentle_ctrl_c=True,
                 log_command=True if cab.flavour.log_full_command else command_name, 
                 log_result=False)
```

### Comparing `stimela-2.0rc8/stimela/backends/podman.py` & `stimela-2.0rc9/stimela/backends/podman.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from stimela import utils
 import json
 import stimela
 import time
 import datetime
 import tempfile
 
-def is_available():
+def is_available(opts = None):
     return False
 
 def get_status():
     return "not yet implemented"
 
 def is_remote():
     return False
```

### Comparing `stimela-2.0rc8/stimela/backends/singularity.py` & `stimela-2.0rc9/stimela/backends/singularity.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import logging
 from stimela import utils
 import stimela
 from shutil import which
 from dataclasses import dataclass
 from omegaconf import OmegaConf
-from typing import Dict, List, Any, Optional, Tuple
+from typing import Dict, List, Any, Optional, Callable
 from contextlib import ExitStack
 from scabha.basetypes import EmptyListDefault
 import datetime
 from stimela.utils.xrun_asyncio import xrun
 
 from stimela.exceptions import BackendError
 
@@ -19,44 +19,49 @@
 
 @dataclass
 class SingularityBackendOptions(object):
     enable: bool = True
     image_dir: str = os.path.expanduser("~/.singularity")
     auto_build: bool = True
     rebuild: bool = False
-    auto_update: bool = False
+    auto_update: bool = False      # currently unused
     executable: Optional[str] = None
+    remote_only: bool = False      # if True, won't look for singularity on local system -- useful in combination with slurm wrapper
 
     # @dataclass
     # class EmptyVolume(object):
     #     name: str
     #     mount: str
 
     # tmp_dirs: List[EmptyVolume] = EmptyListDefault()
 
 SingularityBackendSchema = OmegaConf.structured(SingularityBackendOptions)
 
 STATUS = VERSION = BINARY = None
 
-_auto_updated_images = set()
+# images rebuilt in this run
+_rebuilt_images = set()
 
-def is_available():
+def is_available(opts: Optional[SingularityBackendOptions] = None):
     global STATUS, VERSION, BINARY
     if STATUS is None:
-        BINARY = which("singularity")
-        if BINARY:
-            __version_string = subprocess.check_output([BINARY, "--version"]).decode("utf8")
-            STATUS = VERSION = __version_string.strip().split()[-1]
-            # if VERSION < "3.0.0":
-            #     suffix = ".img"
-            # else:
-            #     suffix = ".sif"
+        if opts and opts.remote_only:
+            STATUS = VERSION = "remote"
         else:
-            STATUS = "not installed"
-            VERSION = None    
+            BINARY = (opts and opts.executable) or which("singularity")
+            if BINARY:
+                __version_string = subprocess.check_output([BINARY, "--version"]).decode("utf8")
+                STATUS = VERSION = __version_string.strip().split()[-1]
+                # if VERSION < "3.0.0":
+                #     suffix = ".img"
+                # else:
+                #     suffix = ".sif"
+            else:
+                STATUS = "not installed"
+                VERSION = None    
     return VERSION is not None
 
 def get_status():
     is_available()
     return STATUS
 
 def is_remote():
@@ -91,153 +96,188 @@
     # convert to filename
     simg_name = image_name.replace("/", "-") + ".simg"
     simg_path = os.path.join(backend.singularity.image_dir, simg_name) 
 
     return image_name, simg_path, True
 
 
-def build_command_line(cab: 'stimela.kitchen.cab.Cab', backend: 'stimela.backend.StimelaBackendOptions',
-                        params: Dict[str, Any], 
-                        binds: List[Any],
-                        subst: Optional[Dict[str, Any]] = None,
-                        binary: Optional[str] = None,
-                        simg_path: Optional[str] = None):
-    args = cab.flavour.get_arguments(cab, params, subst, check_executable=False)
-
-    if simg_path is None:
-        _, simg_path = get_image_info(cab, backend)
-
-    cwd = os.getcwd()
-
-    return [binary or backend.singularity.executable or BINARY, 
-            "exec", 
-            "--containall",
-            "--bind", f"{cwd}:{cwd}",
-            "--pwd", cwd,
-            simg_path] + args
-
-
-
-def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
-        backend: 'stimela.backend.StimelaBackendOptions',
-        log: logging.Logger, subst: Optional[Dict[str, Any]] = None):
-    """Runs cab contents
+def build(cab: 'stimela.kitchen.cab.Cab', backend: 'stimela.backend.StimelaBackendOptions', log: logging.Logger,
+          command_wrapper: Optional[Callable]=None,
+          build=True, rebuild=False):
+    """Builds image for cab, if necessary.
 
-    Args:
-        cab (Cab): cab object
-        log (logger): logger to use
-        subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
+    build: if True, build missing images regardless of backend settings
+    rebuild: if True, rebuild all images regardless of backend settings
 
     Returns:
-        Any: return value (e.g. exit code) of content
+        str: path to corresponding singularity image
     """
-    native.update_rlimits(backend.rlimits, log)
 
-    image_name, simg_path, auto_update = get_image_info(cab, backend)
+    image_name, simg_path, auto_update_allowed = get_image_info(cab, backend)
 
-    rebuild = backend.singularity.rebuild  
+    # this is True if we're allowed to build missing images
+    build = build or rebuild or backend.singularity.auto_build or backend.singularity.auto_update    
+    # this is True if we're asked to force-rebuild images
+    rebuild = rebuild or backend.singularity.rebuild
+    
     cached_image_exists = os.path.exists(simg_path)
 
     # no image? Better have builds enabled then
     if not cached_image_exists:
         log.info(f"singularity image {simg_path} does not exist")
-        rebuild = rebuild or backend.singularity.auto_build or backend.singularity.auto_update
-        if not rebuild:
+        if not build:
             raise BackendError(f"no image, and singularity build options not enabled")
-
-    # check if existing image needs to be rebuilt
-    if auto_update and backend.singularity.auto_update and not rebuild:
-        if image_name in _auto_updated_images:
-            log.info("image was used earlier in this run, not checking for auto-updates again")
+    # else we have an image
+    # if rebuild is enabled, delete it
+    elif rebuild:
+        if simg_path in _rebuilt_images:
+            log.info(f"singularity image {simg_path} was rebuilt earlier")
         else:
-            _auto_updated_images.add(image_name)
-            # force check of docker binary
-            docker.is_available()
-            if docker.BINARY is None:
-                log.warn("a docker runtime is required for auto-update of singularity images: forcing unconditional rebuild")
-                rebuild = True
-            else:
-                log.info("singularity auto-update: pulling and inspecting docker image")
-                # pull image from hub
-                retcode = xrun(docker.BINARY, ["pull", image_name], 
-                            shell=False, log=log,
-                                return_errcode=True, command_name="(docker pull)", 
-                                log_command=True, 
-                                log_result=True)
-                if retcode != 0:
-                    raise BackendError(f"docker pull failed with return code {retcode}") 
-                if os.path.exists(simg_path):
-                    # check timestamp
-                    result = subprocess.run(
-                            [docker.BINARY, "inspect", "-f", "{{ .Created }}", image_name],
-                            capture_output=True)
-                    if result.returncode != 0:
-                        for line in result.stdout.split("\n"):
-                            log.warn(f"docker inpect stdout: {line}")
-                        for line in result.stderr.split("\n"):
-                            log.error(f"docker inpect stderr: {line}")
-                        raise BackendError(f"docker inspect failed with return code {result.returncode}")
-                    timestamp = result.stdout.decode().strip()
-                    log.info(f"docker inspect returns timestamp {timestamp}")
-                    # parse timestamps like '2023-04-07T13:39:19.187572398Z'
-                    # Pre-3.11 pythons don't do it natively so we mess around...
-                    match = re.fullmatch("(.*)T([^.]*)(\.\d+)?Z?", timestamp)
-                    if not match:
-                        raise BackendError(f"docker inspect returned invalid timestamp '{timestamp}'")
-                    try:
-                        dt = datetime.datetime.fromisoformat(f'{match.group(1)} {match.group(2)} +00:00')
-                    except ValueError as exc:
-                        raise BackendError(f"docker inspect returned invalid timestamp '{timestamp}', exc")
-
-                    if dt.timestamp() > os.path.getmtime(simg_path):
-                        log.warn("docker image is newer than cached singularity image, rebuilding")
-                        rebuild = True
-                    else:
-                        log.info("cached singularity image appears to be up-to-date")
-
-    # delete image if rebuild is being forced
-    if cached_image_exists and rebuild:
-        os.unlink(simg_path)        
-        cached_image_exists = False
+            log.info(f"singularity image {simg_path} exists but a rebuild was specified")
+            os.unlink(simg_path)        
+            cached_image_exists = False
+    else:
+        log.info(f"singularity image {simg_path} exists")
+
+    ## OMS: taking this out for now, need some better auto-update logic, let's come back to it later
+        
+    # # else check if it need to be auto-updated
+    # elif auto_update_allowed and backend.singularity.auto_update:
+    #     if image_name in _auto_updated_images:
+    #         log.info("image was used earlier in this run, not checking for auto-updates again")
+    #     else:
+    #         _auto_updated_images.add(image_name)
+    #         # force check of docker binary
+    #         docker.is_available()
+    #         if docker.BINARY is None:
+    #             log.warn("a docker runtime is required for auto-update of singularity images: forcing unconditional rebuild")
+    #             build = True
+    #         else:
+    #             log.info("singularity auto-update: pulling and inspecting docker image")
+    #             # pull image from hub
+    #             retcode = xrun(docker.BINARY, ["pull", image_name], 
+    #                         shell=False, log=log,
+    #                             return_errcode=True, command_name="(docker pull)", 
+    #                             log_command=True, 
+    #                             log_result=True)
+    #             if retcode != 0:
+    #                 raise BackendError(f"docker pull failed with return code {retcode}") 
+    #             if os.path.exists(simg_path):
+    #                 # check timestamp
+    #                 result = subprocess.run(
+    #                         [docker.BINARY, "inspect", "-f", "{{ .Created }}", image_name],
+    #                         capture_output=True)
+    #                 if result.returncode != 0:
+    #                     for line in result.stdout.split("\n"):
+    #                         log.warn(f"docker inpect stdout: {line}")
+    #                     for line in result.stderr.split("\n"):
+    #                         log.error(f"docker inpect stderr: {line}")
+    #                     raise BackendError(f"docker inspect failed with return code {result.returncode}")
+    #                 timestamp = result.stdout.decode().strip()
+    #                 log.info(f"docker inspect returns timestamp {timestamp}")
+    #                 # parse timestamps like '2023-04-07T13:39:19.187572398Z'
+    #                 # Pre-3.11 pythons don't do it natively so we mess around...
+    #                 match = re.fullmatch("(.*)T([^.]*)(\.\d+)?Z?", timestamp)
+    #                 if not match:
+    #                     raise BackendError(f"docker inspect returned invalid timestamp '{timestamp}'")
+    #                 try:
+    #                     dt = datetime.datetime.fromisoformat(f'{match.group(1)} {match.group(2)} +00:00')
+    #                 except ValueError as exc:
+    #                     raise BackendError(f"docker inspect returned invalid timestamp '{timestamp}', exc")
+
+    #                 if dt.timestamp() > os.path.getmtime(simg_path):
+    #                     log.warn("docker image is newer than cached singularity image, rebuilding")
+    #                     os.unlink(simg_path)        
+    #                     cached_image_exists = False
+    #                 else:
+    #                     log.info("cached singularity image appears to be up-to-date")
 
     # if image doesn't exist, build it. We will have already checked for build settings
     # being enabled above
     if not cached_image_exists:
         log.info(f"(re)building image {simg_path}")
 
         args = [BINARY, "build", simg_path, f"docker://{image_name}"]
 
+        if command_wrapper:
+            args = command_wrapper(args, log=log)
+
         retcode = xrun(args[0], args[1:], shell=False, log=log,
                     return_errcode=True, command_name="(singularity build)", 
                     gentle_ctrl_c=True,
                     log_command=True, 
                     log_result=True)
 
         if retcode:
             raise BackendError(f"singularity build returns {retcode}")
 
         if not os.path.exists(simg_path):
             raise BackendError(f"singularity build did not return an error code, but the image did not appear")
+        
+        _rebuilt_images.add(simg_path)
+        
+    return simg_path
+
+
+
+def run(cab: 'stimela.kitchen.cab.Cab', params: Dict[str, Any], fqname: str,
+        backend: 'stimela.backend.StimelaBackendOptions',
+        log: logging.Logger, subst: Optional[Dict[str, Any]] = None,
+        command_wrapper: Optional[Callable] = None):
+
+    """Runs cab contents
+
+    Args:
+        cab (Cab): cab object
+        log (logger): logger to use
+        subst (Optional[Dict[str, Any]]): Substitution dict for commands etc., if any.
+
+    Returns:
+        Any: return value (e.g. exit code) of content
+    """
+    from .utils import resolve_required_mounts
+
+    native.update_rlimits(backend.rlimits, log)
+
+    # get path to image, rebuilding if backend options allow this
+    simg_path = build(cab, backend=backend, log=log, build=False)
+
+    # build up command line    
+    cwd = os.getcwd()
+    args = [backend.singularity.executable or BINARY, 
+            "exec", 
+            "--containall",
+            "--pwd", cwd]
     
-    args = build_command_line(cab, backend, params, subst, simg_path=simg_path)
+    # initial set of mounts has cwd as read-write
+    mounts = {cwd: True}
+    # get extra required filesystem bindings
+    resolve_required_mounts(mounts, params, cab.inputs, cab.outputs)
+    for path, rw in mounts.items():
+        args += ["--bind", f"{path}:{path}:{'rw' if rw else 'ro'}"]
 
+    args += [simg_path]
+    args += cab.flavour.get_arguments(cab, params, subst, check_executable=False)
     log.debug(f"command line is {args}")
 
     cabstat = cab.reset_status()
 
     command_name = f"{cab.flavour.command_name}"
 
     # run command
     start_time = datetime.datetime.now()
     def elapsed(since=None):
         """Returns string representing elapsed time"""
         return str(datetime.datetime.now() - (since or start_time)).split('.', 1)[0]
 
     # log.info(f"argument lengths are {[len(a) for a in args]}")
 
+    if command_wrapper:
+        args = command_wrapper(args, fqname=fqname, log=log)
+
     retcode = xrun(args[0], args[1:], shell=False, log=log,
                 output_wrangler=cabstat.apply_wranglers,
                 return_errcode=True, command_name=command_name, 
                 gentle_ctrl_c=True,
                 log_command=True if cab.flavour.log_full_command else command_name, 
                 log_result=False)
```

### Comparing `stimela-2.0rc8/stimela/backends/utils.py` & `stimela-2.0rc9/stimela/backends/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,47 +4,28 @@
 from stimela.kitchen.cab import Cab, Parameter
 from scabha.exceptions import SchemaError
 from stimela.exceptions import BackendError
 from scabha.basetypes import File, Directory, MS
 
 ## commenting out for now -- will need to fix when we reactive the kube backend (and have tests for it)
 
-def resolve_required_mounts(params: Dict[str, Any], 
+def resolve_required_mounts(mounts: Dict[str, bool],
+                            params: Dict[str, Any], 
                             inputs: Dict[str, Parameter], 
                             outputs: Dict[str, Parameter],
-                            prior_mounts: Dict[str, bool]):
+                            ):
 
     mkdirs = {}
-    targets = {}
 
     # helper function to accumulate list of target paths to be mounted
-    def add_target(path, must_exist, readwrite):
+    def add_target(param_name, path, must_exist, readwrite):
         if must_exist and not os.path.exists(path):
-            raise SchemaError(f"{path} does not exist.")
-
+            raise SchemaError(f"parameter '{param_name}': path '{path}' does not exist")
         path = os.path.abspath(path)
-
-        # if path doesn't exist, mount parent dir as read/write (file will be created in there)
-        if not os.path.lexists(path):
-            add_target(os.path.dirname(path), must_exist=True, readwrite=True)
-        # else path is real
-        else:
-            # already mounted? Make sure readwrite is updated
-            if path in targets:
-                targets[path] = targets[path] or readwrite
-            else:
-                # not mounted, but is a link
-                if os.path.islink(path):
-                    # add destination as target
-                    add_target(os.path.realpath(path), must_exist=must_exist, readwrite=readwrite)
-                    # add parent dir as readonly target (to resolve the symlink)
-                    add_target(os.path.dirname(path), must_exist=True, readwrite=False)
-                # add to mounts
-                else:
-                    targets[path] = readwrite
+        mounts[path] = mounts.get(path) or readwrite
 
     # go through parameters and accumulate target paths
     for name, value in params.items():
         schema = inputs.get(name) or outputs.get(name)
         if schema is None:
             raise SchemaError(f"parameter {name} not in defined inputs or outputs for this cab. This should have been caught by validation earlier!")
 
@@ -52,41 +33,57 @@
         if dtype in (File, Directory, MS):
             files = [value]
         elif dtype in (List[File], List[Directory], List[MS]):
             files = value
         else:
             continue
 
-        must_exist = schema.must_exist
-        if must_exist is None:
-            must_exist = name in inputs            
+        must_exist = schema.must_exist and name in inputs 
         readwrite = schema.writable or name in outputs
 
-        # for symlink targets, we need to mount the parent directory
         for path in files:
-            add_target(path, must_exist=must_exist, readwrite=readwrite)
+            # check for s3:// MS references and skip them
+            if path.startswith("s3://") or path.startswith("S3://"):
+                continue
+            path = os.path.abspath(path).rstrip("/")
+            realpath = os.path.abspath(os.path.realpath(path))
+            # check if parent directory access is required
+            if schema.access_parent_dir or schema.write_parent_dir:
+                add_target(name, os.path.dirname(path), must_exist=True, readwrite=schema.write_parent_dir)
+                add_target(name, os.path.dirname(realpath), must_exist=True, readwrite=schema.write_parent_dir)
+            # for symlink targets, we need to mount the parent directory of the link too
+            if os.path.islink(path):
+                # if target is a real directory, mount it directly
+                if os.path.isdir(realpath):
+                    add_target(name, realpath, must_exist=True, readwrite=readwrite)
+                # otherwise mount its parent to allow creation of symlink target
+                else:
+                    add_target(name, os.path.dirname(realpath), must_exist=True, readwrite=readwrite)
+            # for actual targets, mount the parent, for dirs, mount the dir
+            else:
+                if os.path.isdir(path):
+                    add_target(name, path, must_exist=must_exist, readwrite=readwrite)
+                else:
+                    add_target(name, os.path.dirname(path), must_exist=True, readwrite=readwrite)
 
     
-    # now eliminate unnecessary targets (those that have a parent mount with the same read/write property)
+    # now eliminate unnecessary mounts (those that have a parent mount with no lower read/write privileges)
     skip_targets = set()
 
-    for path, readwrite in targets.items():
+    for path, readwrite in mounts.items():
         parent = os.path.dirname(path)
         while parent != "/":  
             # if parent already mounted, and is as writeable as us, skip us
-            if (parent in targets and targets[parent] >= readwrite) or \
-                (parent in prior_mounts and prior_mounts[parent] >= readwrite):
+            if parent in mounts and mounts[parent] >= readwrite:
                 skip_targets.add(path)
                 break
             parent = os.path.dirname(parent)
 
     for path in skip_targets:
-        targets.pop(path)
-
-    return targets
+        mounts.pop(path)
 
 
 def resolve_remote_mounts(params: Dict[str, Any], 
                             inputs: Dict[str, Parameter], 
                             outputs: Dict[str, Parameter],
                             cwd: str = "/",
                             mounts: set = set()):
```

### Comparing `stimela-2.0rc8/stimela/commands/build.py` & `stimela-2.0rc9/stimela/commands/push.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 import click
 from typing import List
 from stimela.main import cli
 import stimela
 
-
 @cli.command(
-    help="""(Re)build stimela base images. Specify a list of image names and versions (if a version is omitted, builds all known versions of image),
-            or else use --all to build all required base images. 
+    help="""Push stimela base images. Specify a list of image names and versions (if a version is omitted, pushes all known versions of image),
+            or else use --all to push everything. 
          """,
-    short_help="build stimela base images",
+    short_help="push stimela images to registry",
     no_args_is_help=True)
 @click.argument("images", nargs=-1, metavar="NAME[:VERSION]", required=False) 
-#                help="image/version to build (builds all versions of image by default)")
 @click.option("-a", "--all", is_flag=True, 
-                help="build all unavailable images (all images, in combination with --rebuild)")
-@click.option("-r", "--rebuild", is_flag=True, 
-                help="force rebuild of image(s)")
-def build(images: List[str], all=False, rebuild=False):
+                help="push all images")
+def push(images: List[str], all=False):
     from stimela.main import BACKEND
     from stimela import CONFIG
     log = stimela.logger()
 
     available_images = BACKEND.available_images()
-    if all:
-        build_images = CONFIG.base.keys()
-    else:
-        build_images = images
-
-    if not build_images:
-        log.info("No images specified. Run 'stimela build -h' for help.")
-        return 0
+    push_images = CONFIG.base.keys() if all else images
 
-    for imagename in build_images:
+    for imagename in push_images:
         if ':' in imagename:
             imagename, version = imagename.split(":", 1)
         else:
             version = None
 
         if imagename not in CONFIG.base:
             log.error(f"base image '{imagename}' is not known to Stimela")
             return 2
 
         image = CONFIG.base[imagename]
 
         if version is None:
-            build_versions = image.images.keys()
+            push_versions = image.images.keys()
         elif version in image.images:
-            build_versions = [version]
+            push_versions = [version]
         else:
             log.error(f"version '{version}' is not defined for base image '{imagename}'")
             return 2
 
-        # now loop over build versions
-        for version in build_versions:
-            
+        # now loop over push versions
+        for version in push_versions:
             # check if already exists
-            if imagename in available_images and version in available_images[imagename]:
-                if not rebuild:
-                    log.info(f"image '{imagename}:{version}' already exists, skipping")
-                    continue
+            if imagename not in available_images or version not in available_images[imagename] \
+                        or available_images[imagename][version].build is None:
+                log.warning(f"image '{imagename}:{version}' not found, has it been built?")
+                continue
+
+            BACKEND.push(image, version)
+
 
-            BACKEND.build(image, version)
```

### Comparing `stimela-2.0rc8/stimela/commands/cabs.py` & `stimela-2.0rc9/stimela/commands/cabs.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/cleanup.py` & `stimela-2.0rc9/stimela/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/containers.py` & `stimela-2.0rc9/stimela/commands/containers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/doc.py` & `stimela-2.0rc9/stimela/commands/doc.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/images.py` & `stimela-2.0rc9/stimela/commands/images.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/ps.py` & `stimela-2.0rc9/stimela/commands/ps.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/pull.py` & `stimela-2.0rc9/stimela/commands/pull.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/commands/run.py` & `stimela-2.0rc9/stimela/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
                 help="""Doesn't actually run anything, only prints the selected steps.""")
 @click.option("-p", "--profile", metavar="DEPTH", type=int,
                 help="""Print per-step profiling stats to this depth. 0 disables.""")
 @click.argument("what", metavar="filename.yml|cab name") 
 @click.argument("parameters", nargs=-1, metavar="[recipe name] [PARAM=VALUE] [X.Y.Z=FOO] ...", required=False) 
 def run(what: str, parameters: List[str] = [], dry_run: bool = False, last_recipe: bool = False, profile: Optional[int] = None,
     assign: List[Tuple[str, str]] = [],
-    step_ranges: List[str] = [], tags: List[str] = [], skip_tags: List[str] = [], enable_steps: List[str] = []):
+    step_ranges: List[str] = [], tags: List[str] = [], skip_tags: List[str] = [], enable_steps: List[str] = [],
+    build=False, rebuild=False, build_skips=False):
 
     log = logger()
     params = OrderedDict()
     dotlist = OrderedDict()
     errcode = 0
     recipe_name = None
 
@@ -251,24 +252,25 @@
         except Exception as exc:
             log_exception(RecipeValidationError(f"pre-validation of recipe '{recipe_name}' failed", exc))
             for line in traceback.format_exc().split("\n"):
                 log.debug(line)
             sys.exit(1)        
 
         # select recipe substeps based on command line, and exit if nothing to run
-        selection_options = []
-        for opts in (tags, skip_tags, step_ranges, enable_steps):
-            selection_options.append(set(itertools.chain(*(opt.split(",") for opt in opts))))
-        
-        try:
-            if not recipe.restrict_steps(*selection_options):
-                sys.exit(0)
-        except StepSelectionError as exc:
-            log_exception(exc)
-            sys.exit(2)
+        if not build_skips: 
+            selection_options = []
+            for opts in (tags, skip_tags, step_ranges, enable_steps):
+                selection_options.append(set(itertools.chain(*(opt.split(",") for opt in opts))))
+            
+            try:
+                if not recipe.restrict_steps(*selection_options):
+                    sys.exit(0)
+            except StepSelectionError as exc:
+                log_exception(exc)
+                sys.exit(2)
 
         logdir = stimelogging.get_logfile_dir(recipe.log) or '.'
         log.info(f"recipe logs will be saved under {logdir}")
 
         filename = os.path.join(logdir, "stimela.recipe.deps")
         stimela.config.CONFIG_DEPS.update(recipe_deps)
         stimela.config.CONFIG_DEPS.save(filename)
@@ -284,44 +286,65 @@
         log.info("dry run was requested, exiting")
         sys.exit(0)
 
     start_time = datetime.now()
     def elapsed():
         return str(datetime.now() - start_time).split('.', 1)[0]
 
-    try:
-        outputs = outer_step.run(backend=stimela.CONFIG.opts.backend)
-    except Exception as exc:
-        stimela.backends.close_backends(log)
+    # build the images
+    if build:
+        try:
+            outer_step.build(backend=stimela.CONFIG.opts.backend, rebuild=rebuild, build_skips=build_skips, log=log)
+        except Exception as exc:
+            stimela.backends.close_backends(log)
 
-        task_stats.save_profiling_stats(outer_step.log, 
-            print_depth=profile if profile is not None else stimela.CONFIG.opts.profile.print_depth,
-            unroll_loops=stimela.CONFIG.opts.profile.unroll_loops)
-        if not isinstance(exc, ScabhaBaseException) or not exc.logged:
-            log_exception(StimelaRuntimeError(f"run failed after {elapsed()}", exc, 
-                tb=not isinstance(exc, ScabhaBaseException)))
-        else:
-            log.error("run failed, exiting with error code 1")
-        for line in traceback.format_exc().split("\n"):
-            log.debug(line)
-        last_log_dir = stimelogging.get_logfile_dir(outer_step.log) or '.'
-        outer_step.log.info(f"last log directory was {stimelogging.apply_style(last_log_dir, 'bold green')}")
-        sys.exit(1)
-
-    if outputs and outer_step.log.isEnabledFor(logging.DEBUG):
-        outer_step.log.debug(f"run successful after {elapsed()}, outputs follow:")
-        for name, value in outputs.items():
-            if name in recipe.outputs:
-                outer_step.log.debug(f"  {name}: {value}")
+            if not isinstance(exc, ScabhaBaseException) or not exc.logged:
+                log_exception(StimelaRuntimeError(f"build failed after {elapsed()}", exc, 
+                    tb=not isinstance(exc, ScabhaBaseException)))
+            else:
+                log.error("build failed, exiting with error code 1")
+            for line in traceback.format_exc().split("\n"):
+                log.debug(line)
+            last_log_dir = stimelogging.get_logfile_dir(outer_step.log) or '.'
+            outer_step.log.info(f"last log directory was {stimelogging.apply_style(last_log_dir, 'bold green')}")
+            sys.exit(1)
+
+    # else run the recipe
     else:
-        outer_step.log.info(f"run successful after {elapsed()}")
+        try:
+            outputs = outer_step.run(backend=stimela.CONFIG.opts.backend)
+        except Exception as exc:
+            stimela.backends.close_backends(log)
+
+            task_stats.save_profiling_stats(outer_step.log, 
+                print_depth=profile if profile is not None else stimela.CONFIG.opts.profile.print_depth,
+                unroll_loops=stimela.CONFIG.opts.profile.unroll_loops)
+            if not isinstance(exc, ScabhaBaseException) or not exc.logged:
+                log_exception(StimelaRuntimeError(f"run failed after {elapsed()}", exc, 
+                    tb=not isinstance(exc, ScabhaBaseException)))
+            else:
+                log.error("run failed, exiting with error code 1")
+            for line in traceback.format_exc().split("\n"):
+                log.debug(line)
+            last_log_dir = stimelogging.get_logfile_dir(outer_step.log) or '.'
+            outer_step.log.info(f"last log directory was {stimelogging.apply_style(last_log_dir, 'bold green')}")
+            sys.exit(1)
+
+        if outputs and outer_step.log.isEnabledFor(logging.DEBUG):
+            outer_step.log.debug(f"run successful after {elapsed()}, outputs follow:")
+            for name, value in outputs.items():
+                if name in recipe.outputs:
+                    outer_step.log.debug(f"  {name}: {value}")
+        else:
+            outer_step.log.info(f"run successful after {elapsed()}")
 
     stimela.backends.close_backends(log)
 
-    task_stats.save_profiling_stats(outer_step.log, 
-            print_depth=profile if profile is not None else stimela.CONFIG.opts.profile.print_depth,
-            unroll_loops=stimela.CONFIG.opts.profile.unroll_loops)
+    if not build:
+        task_stats.save_profiling_stats(outer_step.log, 
+                print_depth=profile if profile is not None else stimela.CONFIG.opts.profile.print_depth,
+                unroll_loops=stimela.CONFIG.opts.profile.unroll_loops)
     
     last_log_dir = stimelogging.get_logfile_dir(outer_step.log) or '.'
     outer_step.log.info(f"last log directory was {stimelogging.apply_style(last_log_dir, 'bold green')}")
     return 0
```

### Comparing `stimela-2.0rc8/stimela/commands/save_config.py` & `stimela-2.0rc9/stimela/commands/save_config.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/config.py` & `stimela-2.0rc9/stimela/config.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/exceptions.py` & `stimela-2.0rc9/stimela/exceptions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/kitchen/batch.py` & `stimela-2.0rc9/stimela/kitchen/batch.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/kitchen/cab.py` & `stimela-2.0rc9/stimela/kitchen/cab.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/kitchen/recipe.py` & `stimela-2.0rc9/stimela/kitchen/recipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os, os.path, re, fnmatch, copy, traceback
+import os, os.path, re, fnmatch, copy, traceback, logging
 from typing import Any, Tuple, List, Dict, Optional, Union
 from dataclasses import dataclass
 from omegaconf import MISSING, OmegaConf, DictConfig, ListConfig
 from omegaconf.errors import OmegaConfBaseException
 from collections import OrderedDict
 from collections.abc import Mapping
 import rich.table
 
-from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ProcessPoolExecutor, as_completed
 
 from stimela.config import EmptyDictDefault, EmptyListDefault
 import stimela
 from stimela import log_exception, stimelogging
 from stimela.exceptions import *
 
 from scabha.validate import evaluate_and_substitute, evaluate_and_substitute_object, Unresolved, join_quote
@@ -617,15 +617,15 @@
                 log = stimela.logger().getChild(self.fqname)
                 log.propagate = True
 
             # init and/or update logger options
             self.logopts = config.opts.log.copy()
 
             # update file logger
-            logsubst = SubstitutionNS(config=config, info=dict(fqname=fqname))
+            logsubst = SubstitutionNS(config=config, info=dict(fqname=fqname, taskname=fqname))
             stimelogging.update_file_logger(log, self.logopts, nesting=nesting, subst=logsubst, location=[self.fqname])
 
             # call Cargo's finalize method
             super().finalize(config, log=log, fqname=fqname, nesting=nesting)
 
             # finalize steps
             for label, step in self.steps.items():
@@ -740,15 +740,15 @@
 
         # split parameters into our own, and per-step, and UNSET directives
         params,  unset_params = self._preprocess_parameters(params)
 
         subst_outer = subst  # outer dictionary is used to prevalidate our parameters
 
         subst = SubstitutionNS()
-        info = SubstitutionNS(fqname=self.fqname, label='', label_parts=[], suffix='')
+        info = SubstitutionNS(fqname=self.fqname, taskname=self.fqname, label='', label_parts=[], suffix='')
         # mutable=False means these sub-namespaces are not subject to {}-substitutions
         subst._add_('info', info.copy(), nosubst=True)
         subst._add_('config', self.config, nosubst=True) 
         subst._add_('steps', {}, nosubst=True)
         subst._add_('previous', {}, nosubst=True)
         subst.recipe = SubstitutionNS(**params)
         subst.recipe.log = self.logopts
@@ -1033,20 +1033,27 @@
             value (Any): value
         """
         for alias in self._alias_list.get(name, []):
             if alias.from_recipe:
                 alias.step.update_parameter(alias.param, value)
 
 
-    def _iterate_loop_worker(self, params, info, subst, backend, count, iter_var, raise_exc=True):
+    def _iterate_loop_worker(self, params, subst, backend, count, iter_var, subprocess=False, raise_exc=True):
         """"
         Needed for concurrency
         """
+        # close progress bar in subprocesses
+        if subprocess:
+            task_stats.add_subprocess_id(count)
+            task_stats.destroy_progress_bar()
+        subst.info.subprocess = task_stats.get_subprocess_id()
+        taskname = subst.info.taskname
         outputs = {}
         exception = tb = None
+        task_attrs, task_kwattrs = (), {}
         try:
             # if for-loop, assign new value
             if self.for_loop:
                 self.log.info(f"for loop iteration {count}: {self.for_loop.var} = {iter_var}")
                 print(f"for loop iteration {count}: {self.for_loop.var} = {iter_var}")
                 if self.for_loop.var in self.inputs_outputs:
                     params[self.for_loop.var] = iter_var
@@ -1064,73 +1071,95 @@
                 if self.for_loop.display_status:
                     try:
                         status = self.for_loop.display_status.format(**status_dict)
                     except Exception as exc:
                         self.log.warning(f"error formatting for-loop status: {exc}, falling back on default status display")
                 if status is None:
                     status = "{index1}/{total}".format(**status_dict)
-                stimelogging.declare_subtask_attributes(status)
-
-            for label, step in self.steps.items():
-                # update step info
-                self._prep_step(label, step, subst)
-                # reevaluate recipe level assignments (info.fqname etc. have changed)
-                self.update_assignments(subst, params=params)
-                # evaluate step-level assignments
-                self.update_assignments(subst, whose=step, params=params)
-                # step logger may have changed
-                stimelogging.update_file_logger(step.log, step.logopts, nesting=step.nesting, subst=subst, location=[step.fqname])
-                # set our info back temporarily to update log assignments
-                info_step = subst.info
-                subst.info = info.copy()
-                subst.info = info_step
-
-                if step.skip is True:
-                    self.log.debug(f"step '{label}' will be explicitly skipped")
-                else:
-                    self.log.info(f"processing step '{label}'")
-                    if step.info:
-                        self.log.info(f"  ({step.info})", extra=dict(color="GREEN", boldface=True))
-                try:
-                    #step_params = step.run(subst=subst.copy(), batch=batch)  # make a copy of the subst dict since recipe might modify
-                    step_params = step.run(backend=backend, subst=subst.copy(), parent_log=self.log)  # make a copy of the subst dict since recipe might modify
-                except ScabhaBaseException as exc:
-                    newexc = StimelaStepExecutionError(f"step '{step.fqname}' has failed, aborting the recipe", exc)
-                    if not exc.logged:
-                        log_exception(newexc, log=step.log)
-                    raise newexc
-
-                # put step parameters into previous and steps[label] again, as they may have changed based on outputs)
-                subst.previous = step_params
-                subst.steps[label] = subst.previous
-                # revert to recipe level assignments
+                task_stats.declare_subtask_status(status)
+                taskname = f"{taskname}.{count}"
+                subst.info.taskname = taskname 
+                # task_stats.declare_subtask_attributes(count)
+                # task_attrs = (count,)
+                context = task_stats.declare_subtask(f"({count})")
+            else:
+                from contextlib import nullcontext
+                context = nullcontext()
+            with context: 
+                for label, step in self.steps.items():
+                    # update step info
+                    self._prep_step(label, step, subst)
+                    subst.info.taskname = f"{taskname}.{label}"
+                    # reevaluate recipe level assignments (info.fqname etc. have changed)
+                    self.update_assignments(subst, params=params)
+                    # evaluate step-level assignments
+                    self.update_assignments(subst, whose=step, params=params)
+                    # step logger may have changed
+                    stimelogging.update_file_logger(step.log, step.logopts, nesting=step.nesting, subst=subst, location=[step.fqname])
+                    # set our info back temporarily to update log assignments
+
+                    ## OMS: note to self, I had this here but not sure why. Seems like a no-op. Something with logname fiddling.
+                    ## Leave as a puzzle to future self for a bit. Remove info from args.
+                    # info_step = subst.info
+                    # subst.info = info.copy()
+                    # subst.info = info_step
 
-                # now check for output aliases that need to be propagated down from steps
-                self.update_assignments(subst, whose=self, params=params)
-                for name, aliases in self._alias_list.items():
-                    for alias in aliases:
-                        if alias.from_step and alias.step is step:
-                            # if step was skipped, mark output as not required
-                            if alias.step._skip:
-                                self.outputs[name].required = False
-                            # if step output is validated, add it to our output 
-                            # if alias.param in alias.step.validated_params:
-                            #     outputs[name] = alias.step.validated_params[alias.param]
-                            if alias.param in step_params:
-                                outputs[name] = step_params[alias.param]
+                    if step.skip is True:
+                        self.log.debug(f"step '{label}' will be explicitly skipped")
+                    else:
+                        self.log.info(f"processing step '{label}'")
+                        if step.info:
+                            self.log.info(f"  ({step.info})", extra=dict(color="GREEN", boldface=True))
+                    try:
+                        #step_params = step.run(subst=subst.copy(), batch=batch)  # make a copy of the subst dict since recipe might modify
+                        step_params = step.run(backend=backend, subst=subst.copy(), parent_log=self.log)  # make a copy of the subst dict since recipe might modify
+                    except ScabhaBaseException as exc:
+                        newexc = StimelaStepExecutionError(f"step '{step.fqname}' has failed, aborting the recipe", exc)
+                        if not exc.logged:
+                            log_exception(newexc, log=step.log)
+                        raise newexc
+
+                    # put step parameters into previous and steps[label] again, as they may have changed based on outputs)
+                    subst.previous = step_params
+                    subst.steps[label] = subst.previous
+                    # revert to recipe level assignments
+
+                    # now check for output aliases that need to be propagated down from steps
+                    self.update_assignments(subst, whose=self, params=params)
+                    for name, aliases in self._alias_list.items():
+                        for alias in aliases:
+                            if alias.from_step and alias.step is step:
+                                # if step was skipped, mark output as not required
+                                if alias.step._skip:
+                                    self.outputs[name].required = False
+                                # if step output is validated, add it to our output 
+                                # if alias.param in alias.step.validated_params:
+                                #     outputs[name] = alias.step.validated_params[alias.param]
+                                if alias.param in step_params:
+                                    outputs[name] = step_params[alias.param]
 
         except Exception as exc:
             # raise exception up if asked to
             if raise_exc:
                 raise
             # else will be returned
             exception = exc
             tb = FormattedTraceback(sys.exc_info()[2])
 
-        return task_stats.collect_stats(), outputs, exception, tb
+        return task_attrs, task_kwattrs, task_stats.collect_stats(), outputs, exception, tb
+
+    def build(self, backend={}, rebuild=False, build_skips=False, log: Optional[logging.Logger] = None):
+        # set up backend
+        backend = OmegaConf.merge(backend, self.backend or {})
+        # build recursively
+        log = log or self.log
+        log.info(f"building image(s) for recipe '{self.fqname}'")
+        for step in self.steps.values():
+            step.build(backend, rebuild=rebuild, build_skips=build_skips, log=log)
+
 
     def _run(self, params, subst=None, backend={}) -> Dict[str, Any]:
         """Internal recipe run method. Meant to be called from a wrapper Step object (which validates the parameters, etc.)
 
         Parameters
         ----------
 
@@ -1146,16 +1175,19 @@
         # set up backend
         backend = OmegaConf.merge(backend, self.backend or {})
 
         # set up substitution namespace
         subst_outer = subst
         if subst is None:
             subst = SubstitutionNS()
+            taskname = self.name
+        else:
+            taskname = subst.info.taskname
 
-        info = SubstitutionNS(fqname=self.fqname, label='', label_parts=[], suffix='')
+        info = SubstitutionNS(fqname=self.fqname, label='', label_parts=[], suffix='', taskname=taskname)
         # nosubst=True means these sub-namespaces are not subject to {}-substitutions
         subst._add_('info', info.copy(), nosubst=True)
         subst._add_('config', self.config, nosubst=True)
         subst._add_('steps', {}, nosubst=True)
         subst._add_('previous', {}, nosubst=True)
         subst._add_('current', {}, nosubst=True)
             
@@ -1198,46 +1230,60 @@
                     self._update_aliases(name, value)
                 elif schema.required and (self.for_loop is None or name != self.for_loop.var): 
                         raise RecipeValidationError(f"recipe '{self.name}' is missing required input '{name}'", log=self.log)
 
             # form list of arguments for each invocation of the loop worker
             loop_worker_args = []
             for count, iter_var in enumerate(self._for_loop_values):
-                loop_worker_args.append((params, info, subst, backend, count, iter_var))
+                loop_worker_args.append((params, subst, backend, count, iter_var))
 
             # if scatter is enabled, use a process pool
             if self._for_loop_scatter:
                 nloop = len(loop_worker_args)
                 if self._for_loop_scatter < 0:
                     num_workers = nloop
                 else:
                     num_workers = min(self._for_loop_scatter, nloop) 
+                inital_task_status = f"0/{nloop} complete, {num_workers} workers"
+                task_stats.declare_subtask_status(inital_task_status)
                 with ProcessPoolExecutor(num_workers) as pool:
                     # submit each iterant to pool
-                    futures = [pool.submit(self._iterate_loop_worker, *args, raise_exc=False) for args in loop_worker_args]
-                    stats = [f.result() for f in futures]
+                    futures = [pool.submit(self._iterate_loop_worker, *args, subprocess=True, raise_exc=False) for args in loop_worker_args]
                     # update task stats, since they're recorded independently within each step, as well
                     # as get any exceptions from the nesting
                     errors = []
-                    nfail = 0
-                    for f in futures:
-                        stats, outputs, exc, tb = f.result()
+                    nfail = ncomplete = 0
+                    for f in as_completed(futures):
+                        attrs, kwattrs, stats, outputs, exc, tb = f.result()
+                        task_stats.declare_subtask_attributes(*attrs, **kwattrs)
                         task_stats.add_missing_stats(stats)
                         if exc is not None:
                             errors.append(exc)
                             if not isinstance(exc, ScabhaBaseException):
                                 errors.append(tb)
                             nfail += 1
+                        else:
+                            ncomplete += 1
+                        if ncomplete:
+                            status = f"[green]{ncomplete}[/green]/{nloop} complete"
+                        else:
+                            status = f"0/{nloop} complete"
+                        if nfail:
+                            status = f"{status}, [red]{nfail}[/red] failed"
+                        status = f"{status}, {num_workers} workers"
+                        task_stats.declare_subtask_status(status)
                     if errors:
                         pool.shutdown()
-                        raise StimelaRuntimeError(f"{nfail}/{len(loop_worker_args)} loop iterations failed", errors)
+                        raise StimelaRuntimeError(f"{nfail}/{nloop} jobs have failed", errors)
+                # drop a rendering of the progress bar onto the console, to overwrite previous garbage if it's there
+                task_stats.restate_progress()
             # else just iterate directly
             else:
                 for args in loop_worker_args:
-                    _, outputs, _, _ = self._iterate_loop_worker(*args, raise_exc=True) 
+                    _, _, _, outputs, _, _ = self._iterate_loop_worker(*args, raise_exc=True) 
             
             # either way, outputs contains output aliases from the last iteration
             params.update(**outputs)
 
             # current namespace becomes recipe again
             subst.current = subst.recipe
```

### Comparing `stimela-2.0rc8/stimela/kitchen/step.py` & `stimela-2.0rc9/stimela/kitchen/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from omegaconf import MISSING, OmegaConf, DictConfig, ListConfig
 from omegaconf.errors import OmegaConfBaseException
 from collections import OrderedDict
 from contextlib import nullcontext
 
 from stimela.config import EmptyDictDefault, EmptyListDefault
 import stimela
-from stimela import log_exception, stimelogging
+from stimela import log_exception, stimelogging, task_stats
 from stimela.backends import StimelaBackendSchema, runner
 from stimela.exceptions import *
 import scabha.exceptions
 from scabha.exceptions import SubstitutionError, SubstitutionErrorList
 from scabha.validate import evaluate_and_substitute, evaluate_and_substitute_object, Unresolved, join_quote
 from scabha.substitutions import SubstitutionNS, substitutions_from 
 from scabha.basetypes import UNSET, Placeholder, MS, File, Directory, SkippedOutput
@@ -257,15 +257,15 @@
 
             # check for valid backend
             backend_opts = OmegaConf.to_object(OmegaConf.merge(
                 StimelaBackendSchema,
                 backend or {}, 
                 self.cargo.backend or {}, 
                 self.backend or {}))
-            runner.validate_backend_settings(backend_opts)
+            runner.validate_backend_settings(backend_opts, log=log)
 
 
     def prevalidate(self, subst: Optional[SubstitutionNS]=None, root=False):
         self.finalize()
         # validate cab or recipe
         params = self.validated_params = self.cargo.prevalidate(self.params, subst, root=root)
         # add missing outputs
@@ -313,41 +313,63 @@
         else:
             try:
                 self.cargo.assign_value(key, value, override=override)
             except ScabhaBaseException as exc:
                 raise AssignmentError(f"{self.name}: invalid assignment {key}={value}", exc)
 
 
+    def build(self, backend={}, rebuild=False, build_skips=False, log: Optional[logging.Logger] = None):
+        # skipping step? ignore the build
+        if self.skip is True and not build_skips:
+            return
+        log = log or self.log
+        # recurse into sub-recipe 
+        from .recipe import Recipe
+        if type(self.cargo) is Recipe:
+            return self.cargo.build(backend, rebuild=rebuild, build_skips=build_skips, log=log)
+        # else build 
+        else:
+            # validate backend settings and call the build function
+            try:
+                backend = OmegaConf.merge(backend, self.cargo.backend or {}, self.backend or {})
+                backend = OmegaConf.to_object(OmegaConf.merge(StimelaBackendSchema, backend))
+                backend_wrapper = runner.validate_backend_settings(backend, log=log)
+            except Exception as exc:
+                newexc = BackendError("error validating backend settings", exc)
+                raise newexc from None
+            log.info(f"building image for step '{self.fqname}'")
+            with task_stats.declare_subtask(self.name):
+                return backend_wrapper.build(self.cargo, log=log, rebuild=rebuild)
+
+
     def run(self, backend={}, subst=None, parent_log=None):
         """Runs the step"""
         from .recipe import Recipe
 
         # some messages go to the parent logger -- if not defined, default to our own logger
         if parent_log is None:
             parent_log = self.log
 
         # validate backend settings
         try:
             backend = OmegaConf.merge(backend, self.cargo.backend or {}, self.backend or {})
             backend_opts = evaluate_and_substitute_object(backend, subst, recursion_level=-1, location=[self.fqname, "backend"])
             backend_opts = OmegaConf.to_object(OmegaConf.merge(StimelaBackendSchema, backend_opts))
-            backend_opts, backend_main, backend_wrapper =  runner.validate_backend_settings(backend_opts)
+            backend_wrapper = runner.validate_backend_settings(backend_opts, log=self.log)
         except Exception as exc:
             newexc = BackendError("error validating backend settings", exc)
             raise newexc from None
-            # self.log_exception(newexc)
-        remote_backend = backend_main.is_remote()
 
         # if step is being explicitly skipped, omit from profiling, and drop info/warning messages to debug level
         explicit_skip = self.skip is True 
         if explicit_skip:
             context = nullcontext()
             parent_log_info = parent_log_warning = parent_log.debug
         else:
-            context = stimelogging.declare_subtask(self.name, hide_local_metrics=remote_backend)
+            context = task_stats.declare_subtask(self.name, hide_local_metrics=backend_wrapper.is_remote)
             stimelogging.declare_chapter(f"{self.fqname}")
             parent_log_info, parent_log_warning = parent_log.info, parent_log.warning
 
         if self.validated_params is None:
             self.prevalidate(self.params)
 
         with context:
@@ -369,15 +391,15 @@
             params.update(**self.params)
 
             skip_warned = False   # becomes True when warnings are given
 
             self.log.debug(f"validating inputs {subst and list(subst.keys())}")
             validated = None
             try:
-                params = self.cargo.validate_inputs(params, loosely=skip, remote_fs=remote_backend, subst=subst)
+                params = self.cargo.validate_inputs(params, loosely=skip, remote_fs=backend_wrapper.is_remote_fs, subst=subst)
                 validated = True
 
             except ScabhaBaseException as exc:
                 severity = "warning" if skip else "error"
                 level = logging.WARNING if skip else logging.ERROR
                 if not exc.logged and not explicit_skip:
                     if type(exc) is SubstitutionErrorList:
@@ -421,15 +443,15 @@
                         parent_log_warning("since the step was skipped, this is not fatal")
                         skip_warned = True
                 else:
                     raise StepValidationError(f"step '{self.name}': invalid inputs: {join_quote(invalid)}", log=self.log)
 
             ## check if we need to skip based on existing/fresh file outputs
             ## if skip on fresh outputs is in effect, find mtime of most recent input 
-            if not remote_backend and not skip and self.skip_if_outputs:
+            if not backend_wrapper.is_remote_fs and not skip and self.skip_if_outputs:
                 # max_mtime will remain 0 if we're not echecking for freshness, or if there are no file-type inputs
                 max_mtime, max_mtime_path = 0, None
                 if self.skip_if_outputs == OUTPUTS_FRESH:
                     parent_log_info("checking if file-type outputs of step are fresh")
                     for name, value in params.items():
                         schema = self.inputs_outputs[name]
                         if schema.is_input and not schema.skip_freshness_checks:
@@ -511,28 +533,28 @@
                             parent_log_info(f"  {msg}")
                 if all_exist:
                     parent_log_info("all required outputs are OK, skipping this step")
                     skip = True
 
             if not skip:
                 # check for outputs that need removal
-                if not remote_backend:
+                if not backend_wrapper.is_remote_fs:
                     for name, schema in self.outputs.items():
                         if name in params and schema.remove_if_exists and schema.is_file_type:
                             path = params[name]
                             if type(path) is str and os.path.exists(path):
                                 if os.path.isdir(path) and not os.path.islink(path):
                                     shutil.rmtree(path)
                                 else:
                                     os.unlink(path)
 
                 if type(self.cargo) is Recipe:
                     self.cargo._run(params, subst, backend=backend)
                 elif type(self.cargo) is Cab:
-                    cabstat = backend_main.run(self.cargo, params=params, log=self.log, subst=subst, backend=backend_opts, fqname=self.fqname)
+                    cabstat = backend_wrapper.run(self.cargo, params=params, log=self.log, subst=subst, fqname=self.fqname)
                     # check for runstate
                     if cabstat.success is False:
                         raise StimelaCabRuntimeError(f"error running cab '{self.cargo.name}'", cabstat.errors)
                     for msg in cabstat.warnings:
                         self.log.warning(f"cab '{self.cargo.name}': {msg}")
                     params.update(**cabstat.outputs)
                 else:
@@ -543,15 +565,15 @@
                 else:
                     parent_log.debug("skipping step based on explicit setting")
 
             self.log.debug(f"validating outputs")
             validated = False
 
             try:
-                params = self.cargo.validate_outputs(params, loosely=skip,remote_fs=remote_backend, subst=subst)
+                params = self.cargo.validate_outputs(params, loosely=skip,remote_fs=backend_wrapper.is_remote_fs, subst=subst)
                 validated = True
             except ScabhaBaseException as exc:
                 severity = "warning" if skip else "error"
                 level = logging.WARNING if self.skip else logging.ERROR
                 if not exc.logged:
                     if type(exc) is SubstitutionErrorList:
                         self.log_exception(StepValidationError(f"unresolved {{}}-substitution(s) in inputs:", exc.nested), severity=severity)
```

### Comparing `stimela-2.0rc8/stimela/kitchen/wranglers.py` & `stimela-2.0rc9/stimela/kitchen/wranglers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/main.py` & `stimela-2.0rc9/stimela/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,44 +85,44 @@
     if stimela.CONFIG is None:
         log.error("failed to load configuration, exiting")
         sys.exit(1)
 
     if config.CONFIG_LOADED:
         log.info(f"loaded config from {config.CONFIG_LOADED}") 
 
-    # select backend
+    # select backend, passing it any config options that have been set up
     if backend:
-        if backends.get_backend(backend) is None:
+        if backends.get_backend(backend, getattr(stimela.CONFIG.opts.backend, backend, None)) is None:
             log.error(f"backend '{backend}' not available: {backends.get_backend_status(backend)}")
             sys.exit(1)
 
         stimela.CONFIG.opts.backend.select = [backend]
 
     # enable logfiles and such
     if stimela.CONFIG.opts.log.enable:
         if verbose:
             stimela.CONFIG.opts.log.level = "DEBUG"
         # setup file logging
         subst = OmegaConf.create(dict(
-                    info=OmegaConf.create(dict(fqname='stimela')), 
+                    info=OmegaConf.create(dict(fqname='stimela', taskname='stimela')), 
                     config=stimela.CONFIG))
         stimelogging.update_file_logger(log, stimela.CONFIG.opts.log, nesting=-1, subst=subst)
 
     # report dependencies
     for filename, attrs in config.CONFIG_DEPS.get_description().items():
         log.debug(f"config dependency {', '.join([filename] + attrs)}")
 
     # dump dependencies
     filename = os.path.join(stimelogging.get_logfile_dir(log) or '.', "stimela.config.deps")
     log.info(f"saving config dependencies to {filename}")
     config.CONFIG_DEPS.save(filename)
 
 
 # import commands
-from stimela.commands import doc, run, save_config, cleanup
+from stimela.commands import doc, run, build, save_config, cleanup
 
 ## These one needs to be reimplemented, current backed auto-pulls and auto-builds:
 # images, pull, build, clean
 
 ## this one is deprecated, stimela doc does the trick
 # cabs
```

### Comparing `stimela-2.0rc8/stimela/schedulers/slurm.py` & `stimela-2.0rc9/stimela/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/stimela/stimelogging.py` & `stimela-2.0rc9/stimela/stimelogging.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 import rich.logging
 from rich.tree import Tree
 from rich import print as rich_print
 from rich.markup import escape
 from rich.padding import Padding
 
 from . import task_stats
-from .task_stats import declare_subtask, declare_subtask_attributes, \
-                        declare_subcommand, update_process_status, \
-                        run_process_status_update
 
 class FunkyMessage(object):
     """Class representing a message with two versions: funky (with markup), and boring (no markup)"""
     def __init__(self, funky, boring=None, prefix=None):
         self.funky = funky
         self.boring = boring if boring is not None else funky
         self.prefix = prefix
@@ -180,14 +177,17 @@
         scabha.set_logger(_logger)
 
     return _logger
 
 _logger_file_handlers = {}
 _logger_console_handlers = {}
 
+# keep track of all log files opened
+_previous_logfiles = set()
+
 
 def has_file_logger(log: logging.Logger):
     return log.name in _logger_file_handlers
 
 
 def disable_file_logger(log: logging.Logger):
     current_logfile, fh = _logger_file_handlers.get(log.name, (None, None))
@@ -243,17 +243,22 @@
     # does the logger need a new FileHandler created
     if current_logfile != logfile:
         log.debug(f"will switch to logfile {logfile} (previous was {current_logfile})")
         # remove old FH if so
         if fh is not None:
             fh.close()
             log.removeHandler(fh)
-
+        # if file was previously open, append, else overwrite
+        if logfile in _previous_logfiles:
+            mode = 'a'
+        else:
+            mode = 'w'
+            _previous_logfiles.add(logfile)
         # create new FH
-        fh = DelayedFileHandler(logfile, symlink, 'w')
+        fh = DelayedFileHandler(logfile, symlink, mode)
         fh.setFormatter(log_boring_formatter)
         log.addHandler(fh)
 
         _logger_file_handlers[log.name] = logfile, fh
 
         # if logging to console, disable propagation from this sub-logger, and add a console handler
         # This ensures that parent loggers that log to files to not get repeated messages
```

### Comparing `stimela-2.0rc8/stimela/task_stats.py` & `stimela-2.0rc9/stimela/task_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,81 +13,112 @@
 import rich.progress
 import rich.logging
 from rich.table import Table
 from rich.text import Text
 
 from stimela import stimelogging
 
+# this is "" for the main process, ".0", ".1", for subprocesses, ".0.0" for nested subprocesses
+_subprocess_identifier = ""
+
+def get_subprocess_id():
+    return _subprocess_identifier
+
+def add_subprocess_id(num: int):
+    global _subprocess_identifier
+    _subprocess_identifier += f".{num}"
+
 progress_bar = progress_task = None
 
 _start_time = datetime.now()
 _prev_disk_io = None, None
 
 @dataclass
 class TaskInformation(object):
     names: List[str]
+    status: str = ""
     task_attrs: List[str] = EmptyListDefault()
     command: Optional[str] = None
     status_reporter: Optional[Callable] = None
     hide_local_metrics: bool = False
 
     def __post_init__(self):
         self.names_orig = list(self.names)
 
     @property
     def description(self):
         name = '.'.join(self.names)
-        if self.task_attrs:
-            name += f"\[{', '.join(self.task_attrs)}]"
+        # if self.status:
+        #     name += f": [dim]{self.status}[/dim]"
+        ## OMS: omit attributes from task status for now
+        # if self.task_attrs:
+        #     name += f"\[{', '.join(self.task_attrs)}]"
         return name
 
 # stack of task information -- most recent subtask is at the end
 _task_stack = []
 
 def init_progress_bar(boring=False):
     global progress_console, progress_bar, progress_task
     progress_console = rich.console.Console(file=sys.stdout, highlight=False)
     progress_bar = rich.progress.Progress(
         rich.progress.SpinnerColumn(),
         "[yellow]{task.fields[elapsed_time]}[/yellow]",
         "[bold]{task.description}[/bold]",
         rich.progress.SpinnerColumn(),
+        "[dim]{task.fields[status]}[/dim]",
         "{task.fields[command]}",
         rich.progress.TimeElapsedColumn(),
         "{task.fields[cpu_info]}",
         refresh_per_second=2,
         console=progress_console,
         transient=True,
         disable=boring)
 
-    progress_task = progress_bar.add_task("stimela", command="starting", cpu_info=" ", elapsed_time="", start=True)
+    progress_task = progress_bar.add_task("stimela", status="", command="starting", cpu_info=" ", elapsed_time="", start=True)
     progress_bar.__enter__()
     atexit.register(destroy_progress_bar)
     return progress_bar, progress_console
 
 def destroy_progress_bar():
     global progress_bar
     if progress_bar is not None:
         progress_bar.__exit__(None, None, None)
         progress_bar = None
 
+def restate_progress():
+    """Renders a snapshot of the progress bar onto the console"""
+    if progress_bar is not None:
+        progress_console.print(progress_bar.get_renderable())
+        progress_console.rule()
+
+
 @contextlib.contextmanager
 def declare_subtask(subtask_name, status_reporter=None, hide_local_metrics=False):
-    task_names = (_task_stack[-1].names if _task_stack else []) + [subtask_name]
+    task_names = []
+    if _task_stack:
+        task_names = _task_stack[-1].names + \
+                    (_task_stack[-1].task_attrs or [])
+    task_names.append(subtask_name)
     _task_stack.append(
         TaskInformation(task_names, status_reporter=status_reporter, hide_local_metrics=hide_local_metrics)
     )
     update_process_status()
     try:
         yield subtask_name
     finally:
         _task_stack.pop(-1)
         update_process_status()
 
 
+def declare_subtask_status(status):
+    _task_stack[-1].status = status
+    update_process_status()
+
+
 def declare_subtask_attributes(*args, **kw):
     _task_stack[-1].task_attrs = [str(x) for x in args] + \
                                  [f"{key} {value}" for key, value in kw.items()]
     update_process_status()
 
 
 class _CommandContext(object):
@@ -142,17 +173,17 @@
             if not hasattr(self, f):
                 self.extras.append(f)
             setattr(self, f, getattr(self, f, 0) + getattr(other, f))
 
     def peak(self, other: "TaskStatsDatum"):
         for f in _taskstats_sample_names + other.extras:
             if hasattr(self, f):
-                self.extras.append(f)
                 setattr(self, f, max(getattr(self, f, -1e-9999), getattr(other, f)))
             else:
+                self.extras.append(f)
                 setattr(self, f, getattr(other, f))
 
     def averaged(self):
         avg = TaskStatsDatum(num_samples=1)
         for f in _taskstats_sample_names:
             setattr(avg, f, getattr(self, f) / self.num_samples)
         avg.insert_extra_stats(**{name: getattr(self, name) / self.num_samples for name in self.extras})
@@ -175,15 +206,15 @@
             _, sum1, peak1 = _taskstats[key1]
             sum1.add(sum)
             peak1.peak(peak)
     return _taskstats
 
 
 def add_missing_stats(stats):
-    """Adds stats that wren't recorded into dictionary"""
+    """Adds stats that weren't recorded into dictionary"""
     for key, value in stats.items():
         if key not in _taskstats:
             _taskstats[key] = value
 
 
 def stats_field_names():
     return _taskstats_sample_names
@@ -263,23 +294,24 @@
                 f"RAM [green]{round(s.mem_used):3}[/green]/[green]{round(s.mem_total)}[/green]G",
                 f"Load [green]{s.load:2.1f}[/green]" 
             ]
 
             if io is not None:
                 cpu_info += [
                     f"R [green]{s.read_count:-4}[/green] [green]{s.read_gbps:2.2f}[/green]G [green]{s.read_ms:4}[/green]ms",
-                    f"|W [green]{s.write_count:-4}[/green] [green]{s.write_gbps:2.2f}[/green]G [green]{s.write_ms:4}[/green]ms "
+                    f"W [green]{s.write_count:-4}[/green] [green]{s.write_gbps:2.2f}[/green]G [green]{s.write_ms:4}[/green]ms "
                 ]
         # add extra metering
         cpu_info += extra_metrics or []
 
         updates = dict(elapsed_time=elapsed, cpu_info="|".join(cpu_info))
 
         if ti is not None:
             updates['description'] = ti.description
+            updates['status'] = ti.status or ''
             updates['command'] = ti.command or ''
 
         progress_bar.update(progress_task, **updates)
 
     # update stats
     update_stats(now, s)
```

### Comparing `stimela-2.0rc8/stimela/utils/xrun_asyncio.py` & `stimela-2.0rc9/stimela/utils/xrun_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import signal
 import datetime
 import asyncio
 import logging
 from rich.markup import escape
 
-from stimela import stimelogging
+from stimela import stimelogging, task_stats
 
 from stimela.exceptions import StimelaCabRuntimeError, StimelaProcessRuntimeError
 
 DEBUG = 0
 
 log = None
 
@@ -29,15 +29,15 @@
     # severity = logging.WARNING if fobj is proc.stderr else logging.INFO
     severity = logging.INFO
     if style is not None:
         extra['style'] = style
     if prefix is not None:
         extra['prefix'] = prefix
     extra.setdefault('style', 'dim' if stream_name == 'stdout' else 'white')
-    extra.setdefault('prefix', "#")
+    extra.setdefault('prefix', task_stats.get_subprocess_id() + "#")
     # feed through wrangler to adjust severity and content
     if output_wrangler is not None:
         line, severity = output_wrangler(escape(line), severity)
     if line is not None:
         if severity >= logging.ERROR:
             extra['prefix'] = stimelogging.FunkyMessage("[red]:warning: [/red]", "!")
         if isinstance(line, stimelogging.FunkyMessage) and line.prefix:
@@ -76,15 +76,15 @@
     if log_command:
         if log_command is True:
             log.info(f"running {command_line}", extra=dict(prefix="###", style="dim"))
         else:
             log.info(f"running {log_command}", extra=dict(prefix="###", style="dim"))
             log.debug(f"full command line is {command_line}", extra=dict(prefix="###", style="dim"))
 
-    with stimelogging.declare_subcommand(os.path.basename(command_name)) as command_context:
+    with task_stats.declare_subcommand(os.path.basename(command_name)) as command_context:
 
         start_time = datetime.datetime.now()
         def elapsed():
             """Returns string representing elapsed time"""
             return str(datetime.datetime.now() - start_time).split('.', 1)[0]
         
         loop = asyncio.get_event_loop()
@@ -103,15 +103,15 @@
                     dispatch_to_log(log, line, command_name, stream_name, output_wrangler=output_wrangler)
 
         async def proc_awaiter(proc, *cancellables):
             await proc.wait()
             for task in cancellables:
                 task.cancel()
 
-        reporter = asyncio.Task(stimelogging.run_process_status_update())
+        reporter = asyncio.Task(task_stats.run_process_status_update())
         ctrl_c_caught = job_interrupted = False
         try:
             job = asyncio.gather(
                 proc_awaiter(proc, reporter),
                 stream_reader(proc.stdout, "stdout"),
                 stream_reader(proc.stderr, "stderr"),
                 reporter
```

### Comparing `stimela-2.0rc8/stimela/utils/xrun_poll.py` & `stimela-2.0rc9/stimela/utils/xrun_poll.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/test_configuratt.py` & `stimela-2.0rc9/tests/scabha_tests/test_configuratt.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/test_dynschema.py` & `stimela-2.0rc9/tests/scabha_tests/test_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/test_parsing.py` & `stimela-2.0rc9/tests/scabha_tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/test_schema.py` & `stimela-2.0rc9/tests/scabha_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/test_substitutions.py` & `stimela-2.0rc9/tests/scabha_tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/scabha_tests/testconf.yaml` & `stimela-2.0rc9/tests/scabha_tests/testconf.yaml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/example_dynschema.py` & `stimela-2.0rc9/tests/stimela_tests/example_dynschema.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_aliasing.yml` & `stimela-2.0rc9/tests/stimela_tests/test_aliasing.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_backends.yml` & `stimela-2.0rc9/tests/stimela_tests/test_backends.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_callables.py` & `stimela-2.0rc9/tests/stimela_tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_callables.yml` & `stimela-2.0rc9/tests/stimela_tests/test_callables.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_casa.yml` & `stimela-2.0rc9/tests/stimela_tests/test_casa.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_kube.yml` & `stimela-2.0rc9/tests/stimela_tests/test_kube.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_kube_config.yml` & `stimela-2.0rc9/tests/stimela_tests/test_kube_config.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_kube_qc.yml` & `stimela-2.0rc9/tests/stimela_tests/test_kube_qc.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_kube_scatter.yml` & `stimela-2.0rc9/tests/stimela_tests/test_kube_scatter.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_loop_recipe.yml` & `stimela-2.0rc9/tests/stimela_tests/test_loop_recipe.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_loop_recipe_slurm.yml` & `stimela-2.0rc9/tests/stimela_tests/test_loop_recipe_slurm.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_nesting.yml` & `stimela-2.0rc9/tests/stimela_tests/test_nesting.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_recipe.py` & `stimela-2.0rc9/tests/stimela_tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_recipe.yml` & `stimela-2.0rc9/tests/stimela_tests/test_recipe.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_scatter.yml` & `stimela-2.0rc9/tests/stimela_tests/test_scatter.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_wranglers.py` & `stimela-2.0rc9/tests/stimela_tests/test_wranglers.py`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_wranglers.yml` & `stimela-2.0rc9/tests/stimela_tests/test_wranglers.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/tests/stimela_tests/test_xrun.yml` & `stimela-2.0rc9/tests/stimela_tests/test_xrun.yml`

 * *Files identical despite different names*

### Comparing `stimela-2.0rc8/PKG-INFO` & `stimela-2.0rc9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stimela
-Version: 2.0rc8
-Summary: Framework for system agnostic pipelines for radio interferometry arrays
+Version: 2.0rc9
+Summary: Framework for system agnostic pipelines for (not just) radio interferometry
 License: GNU GPL v2
 Author: Sphesihle Makhathini
 Author-email: sphemakh@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

