# Comparing `tmp/pinjected-0.2.39.tar.gz` & `tmp/pinjected-0.2.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.39.tar", max compression
+gzip compressed data, was "pinjected-0.2.40.tar", max compression
```

## Comparing `pinjected-0.2.39.tar` & `pinjected-0.2.40.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.39/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.39/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.39/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.39/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.39/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.39/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.39/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5690 2024-04-19 03:54:09.818158 pinjected-0.2.39/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.39/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.39/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.39/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.39/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.39/pinjected/di/decorators.py
--rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.39/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.39/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.39/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.39/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.39/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.39/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.39/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.39/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.39/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.39/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.39/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.39/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.39/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.39/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.39/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.39/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.39/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.39/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.39/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.39/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.39/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.39/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.39/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.39/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.39/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.39/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.39/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.39/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.39/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.39/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.39/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.39/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.39/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.39/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.39/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.39/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.39/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.39/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.39/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7287 2024-04-16 09:18:34.207695 pinjected-0.2.39/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.39/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.39/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.39/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.39/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.39/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.39/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.39/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.39/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.39/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.39/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4862 2024-04-16 09:26:56.419338 pinjected-0.2.39/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.39/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.39/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.39/pinjected/providable.py
--rw-r--r--   0        0        0    21282 2024-04-16 13:12:25.671565 pinjected-0.2.39/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.39/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.39/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.39/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.39/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.39/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.39/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.39/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.39/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.39/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.39/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.39/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.39/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.39/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.39/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.39/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.39/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.39/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.39/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.39/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.39/pinjected/with_context.py
--rw-r--r--   0        0        0      627 2024-04-19 03:54:13.159938 pinjected-0.2.39/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.39/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.40/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.40/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.40/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.40/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.40/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.40/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.40/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5690 2024-04-19 03:54:09.818158 pinjected-0.2.40/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.40/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.40/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.40/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.40/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.40/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14618 2024-04-23 08:38:19.296348 pinjected-0.2.40/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.40/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.40/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.40/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.40/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.40/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.40/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.40/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.40/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.40/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.40/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.40/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.40/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.40/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.40/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.40/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.40/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.40/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.40/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.40/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.40/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.40/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.40/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.40/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.40/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.40/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.40/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.40/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.40/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.40/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.40/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.40/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.40/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.40/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.40/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.40/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.40/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.40/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.40/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7322 2024-04-23 08:38:19.297785 pinjected-0.2.40/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.40/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.40/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.40/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.40/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.40/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.40/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.40/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.40/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.40/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.40/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.40/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.40/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.40/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.40/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.40/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.40/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.40/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.40/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.40/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9546 2024-04-23 08:38:19.299938 pinjected-0.2.40/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.40/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.40/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.40/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.40/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.40/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.40/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.40/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.40/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.40/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.40/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.40/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.40/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.40/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.40/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.40/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.40/pinjected/with_context.py
+-rw-r--r--   0        0        0      627 2024-04-23 08:39:11.894857 pinjected-0.2.40/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.40/PKG-INFO
```

### Comparing `pinjected-0.2.39/LICENSE` & `pinjected-0.2.40/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/decoration.py` & `pinjected-0.2.40/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/demo.py` & `pinjected-0.2.40/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/app_designed.py` & `pinjected-0.2.40/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/app_injected.py` & `pinjected-0.2.40/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/applicative.py` & `pinjected-0.2.40/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/ast.py` & `pinjected-0.2.40/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/decorators.py` & `pinjected-0.2.40/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/design.py` & `pinjected-0.2.40/pinjected/di/design.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import inspect
 from copy import copy
 from dataclasses import dataclass, field, replace
 from functools import wraps
+from pathlib import Path
+from pprint import pformat
 from typing import TypeVar, List, Dict, Union, Callable, Type, Self
 
 from cytoolz import merge
 from makefun import create_function
 
 from pinjected.di.graph import DependencyResolver
 from pinjected.di.implicit_globals import IMPLICIT_BINDINGS
 from pinjected.di.injected import Injected
 from pinjected.di.injected import extract_dependency_including_self, InjectedPure, InjectedFunction
 # from pinjected.di.util import get_class_aware_args, get_dict_diff, check_picklable
 from pinjected.di.proxiable import DelegatedVar
+from pinjected.module_var_path import ModuleVarPath
 from pinjected.v2.binds import IBind, BindInjected
 from pinjected.v2.keys import IBindKey, StrBindKey
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
@@ -174,15 +177,15 @@
     def bind_provider(self, **kwargs: Union[Callable, Injected]):
         bindings = dict()
         for k, v in kwargs.items():
             # logger.info(f"binding provider:{k}=>{v}")
             from loguru import logger
             match v:
                 case type():
-                    #logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
+                    # logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
                     bindings[StrBindKey(k)] = BindInjected(Injected.bind(v))
                 case Injected():
                     bindings[StrBindKey(k)] = BindInjected(v)
                 case DelegatedVar():
                     bindings[StrBindKey(k)] = BindInjected(v.eval())
                 case non_func if not callable(non_func):
                     logger.warning(
@@ -334,50 +337,81 @@
         :return:
         """
         # ah sometimes the deps require 'session'
         # and we don't know if the session has enough bindings to provide the target.
         resolver = DependencyResolver(self)
         return resolver.purified_design(target).unbind('__resolver__').unbind('session').unbind('__design__')
 
+    def __enter__(self):
+        frame = inspect.currentframe().f_back
+        DESIGN_OVERRIDES_STORE.add(frame, self)
+        # %% hmm, I want track the global vars on parent frame. but how?
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        frame = inspect.currentframe().f_back
+        DESIGN_OVERRIDES_STORE.pop(frame)
+
+
+@dataclass
+class DesignOverridesStore:
+    bindings: dict[ModuleVarPath, Design] = field(default_factory=dict)
+    stack: List['DesignOverrideContext'] = field(default_factory=list)
+
+    def add(self, frame: inspect.FrameInfo, design: "Design"):
+        cxt = DesignOverrideContext(design, frame)
+        self.stack.append(cxt)
+
+    def pop(self, frame: inspect.FrameInfo):
+        cxt = self.stack.pop()
+        acc_d = sum([cxt.src for cxt in self.stack], start=Design()) + cxt.src
+        target_vars = cxt.exit(frame)
+        for mvp in target_vars:
+            if mvp not in self.bindings:
+                self.bindings[mvp] = acc_d
+
+    def get_overrides(self,tgt:ModuleVarPath):
+        return self.bindings.get(tgt,Design())
+
+
+DESIGN_OVERRIDES_STORE = DesignOverridesStore()
+
 
 @dataclass
 class DesignOverrideContext:
     src: Design
-    callback: Callable[[Self], None]
-    depth: int
-    target_vars: dict = field(default_factory=dict)
+    init_frame: inspect.FrameInfo
 
-    def __enter__(self):
-        frame = inspect.currentframe()
-        parent = frame.f_back
+    def __post_init__(self):
         # get parent global variables
-        parent_globals = parent.f_globals
+        parent_globals = self.init_frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
         from loguru import logger
-        logger.debug(global_ids)
+        #logger.debug(f"enter->\n"+pformat(global_ids))
         self.last_global_ids = global_ids
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def exit(self, frame:inspect.FrameInfo) -> list[ModuleVarPath]:
         from loguru import logger
-        frame = inspect.currentframe()
-        parent = frame.f_back
         # get parent global variables
-        parent_globals = parent.f_globals
+        parent_globals = frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
+        from loguru import logger
+        #logger.debug("exit->\n"+pformat(global_ids))
         changed_keys = []
         for k in global_ids:
             if k in self.last_global_ids:
                 if global_ids[k] != self.last_global_ids[k]:
                     changed_keys.append(k)
             else:
                 changed_keys.append(k)
-        logger.debug(f"global_ids:{global_ids}")
+        #logger.debug(f"global_ids:{global_ids}")
         # find instance of DelegatedVar and Injected in the changed globals
         target_vars = dict()
         for k in changed_keys:
             v = parent_globals[k]
             if isinstance(v, DelegatedVar):
                 target_vars[k] = v
             if isinstance(v, Injected):
                 target_vars[k] = v
-        self.target_vars = target_vars
-        self.callback(self)
+        mod_name = inspect.getmodule(frame).__name__
+        #logger.info(f"found targets:\n{pformat(target_vars)}")
+        return [ModuleVarPath(mod_name+"."+v) for v in target_vars.keys()]
```

### Comparing `pinjected-0.2.39/pinjected/di/designed.py` & `pinjected-0.2.40/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.40/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/graph.py` & `pinjected-0.2.40/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/injected.py` & `pinjected-0.2.40/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/injected_analysis.py` & `pinjected-0.2.40/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/modular_injected.py` & `pinjected-0.2.40/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/overload_experimental.py` & `pinjected-0.2.40/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/proxiable.py` & `pinjected-0.2.40/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/session.py` & `pinjected-0.2.40/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/sessioned.py` & `pinjected-0.2.40/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/static_proxy.py` & `pinjected-0.2.40/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.40/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/test_graph.py` & `pinjected-0.2.40/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/test_injected.py` & `pinjected-0.2.40/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/tools/add_overload.py` & `pinjected-0.2.40/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/di/util.py` & `pinjected-0.2.40/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/exceptions.py` & `pinjected-0.2.40/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.40/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.40/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/graph_inspection.py` & `pinjected-0.2.40/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/helper_structure.py` & `pinjected-0.2.40/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/helpers.py` & `pinjected-0.2.40/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.40/pinjected/ide_supports/console_run_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,25 +61,15 @@
             # Get the source code of the import
             import_source = ast.get_source_segment(file_content, node)
             # Store the import source code in the list
             func_and_imports['imports'].append(import_source)
     return func_and_imports
 
 
-def create_run_design(script_path: str):
-    """
-    This command should load the __meta_design__ and return the final design.
-    :param script_path:
-    :return:
-    """
-    from pinjected.helper_structure import MetaContext
-    __design__ = MetaContext.gather_from_path(Path(script_path)).accumulated
-    __graph__ = __design__.to_graph().auto_sync()
-    # mc:MetaContext = MetaContext.gather_from_path(Path(script_path))
-    # return mc.accumulated
+
 
 
 class WithBlockVisitor(ast.NodeVisitor):
     def __init__(self):
         self.result = {}
 
     def visit_With(self, node):
```

### Comparing `pinjected-0.2.39/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.40/pinjected/ide_supports/create_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     """
     if not "__meta_design__" in Path(context_module_file_path).read_text():
         raise ValueError(f"{context_module_file_path} does not contain __meta_design__")
     meta_context = MetaContext.gather_from_path(context_module_file_path)
     instance_overrides = instances(
         module_path=context_module_file_path,
         interpreter_path=sys.executable,
-        meta_context=meta_context
+        meta_context=meta_context,
+        default_design_paths = []
     ) + instances(**kwargs)
     return run_injected("get", var_path, design_path, return_result=True,
                         overrides=meta_context.accumulated + instance_overrides,
                         notifier=logger.info
                         )
```

### Comparing `pinjected-0.2.39/pinjected/ide_supports/default_design.py` & `pinjected-0.2.40/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.40/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.40/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/main_impl.py` & `pinjected-0.2.40/pinjected/main_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 
     :param var_path: the path to the variable to be injected: e.g. "my_module.my_var"
     :param design_path: the path to the design to be used: e.g. "my_module.my_design"
     :param ovr: a string that can be converted to an Design in some way. This will gets concatenated to the design.
     :param kwargs: overrides for the design. e.g. "api_key=1234"
 
     """
-    # TODO parse overrides
-    # TODO parse kwargs from cli.
     kwargs_overrides = parse_kwargs_as_design(**kwargs)
     ovr = instances()
     if meta_context_path is not None:
         mc = MetaContext.gather_from_path(Path(meta_context_path))
         ovr += mc.final_design
     ovr += parse_overrides(overrides)
     ovr += kwargs_overrides
+    """
+    We need a functionality to get the design for a variable path.
+    Currently, the metacontext only gathers a context for the module.
+    So, I need another implementation in addition to MetaContext.
+    """
     return run_injected("get", var_path, design_path, return_result=True, overrides=ovr)
 
 
 def check_config():
     from loguru import logger
     from pprint import pformat
     default:Design = load_user_default_design()
```

### Comparing `pinjected-0.2.39/pinjected/maybe_patch.py` & `pinjected-0.2.40/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/module_helper.py` & `pinjected-0.2.40/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/module_inspector.py` & `pinjected-0.2.40/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/module_var_path.py` & `pinjected-0.2.40/pinjected/module_var_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import importlib
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 
 
-@dataclass
+@dataclass(frozen=True)
 class ModuleVarPath:
     """
     represents a path where a variable is defined.
     like a.b.c.d
     """
     path: str
```

### Comparing `pinjected-0.2.39/pinjected/notification.py` & `pinjected-0.2.40/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/nx_graph_util.py` & `pinjected-0.2.40/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/run_config_utils.py` & `pinjected-0.2.40/pinjected/run_config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,16 @@
     match meta:
         case Success({"default_design_path": ddp}):
             ddps.append(ddp)
     ddps += default_design_paths
     results = defaultdict(list)
 
     if not ddps:
-        logger.warning(f"no default design path provided for {tgt.var_path}")
+        logger.warning(f"no default design path provided for {tgt.var_path}, using pinjected.EmptyDesign")
+        ddps.append('pinjected.EmptyDesign')
 
     for ddp in ddps:
         args = extract_args_for_runnable(tgt, ddp, meta)
         # this, viz_branch should not be created by this function, but an injected function.
         if args is not None:
             ddp_name = ddp.split(".")[-1]
             config = dict(
```

### Comparing `pinjected-0.2.39/pinjected/run_config_utils_v2.py` & `pinjected-0.2.40/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/run_helpers/config.py` & `pinjected-0.2.40/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.40/pinjected/run_helpers/run_injected.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from typing import Coroutine, Awaitable
 
 from loguru import logger
 from returns.result import safe, Result
 
 from pinjected import instances, Injected, Design, providers, Designed
+from pinjected.di.design import DESIGN_OVERRIDES_STORE
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.helper_structure import MetaContext
 from pinjected.helpers import get_design_path_from_var_path
 from pinjected.module_var_path import ModuleVarPath, load_variable_by_module_path
 from pinjected.logging_helper import disable_internal_logging
 from pinjected.notification import notify
 from pinjected.run_config_utils import load_variable_from_script
@@ -94,14 +95,19 @@
         """
         I need to get the design overrides from with context and add it to the overrides
         """
 
         meta_design = instances(overrides=instances()) + meta_cxt.accumulated
         meta_overrides = meta_design.provide("overrides") + meta_overrides
 
+        # add overrides from with block
+        meta_overrides += DESIGN_OVERRIDES_STORE.get_overrides(ModuleVarPath(var_path))
+
+
+
     design += (meta_overrides + overrides)
     logger.info(f"running target:{var} with {design_path} + {overrides}")
     logger.debug(design.keys())
     # logger.info(f"running target:{var} with cmd {cmd}, args {args}, kwargs {kwargs}")
     # logger.info(f"metadata obtained from pinjected: {meta}")
 
     # here we load the defaults and overrides from the user's environment
```

### Comparing `pinjected-0.2.39/pinjected/runnables.py` & `pinjected-0.2.40/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/test_package/__init__.py` & `pinjected-0.2.40/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/test_package/child/module1.py` & `pinjected-0.2.40/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/v2/ainjected.py` & `pinjected-0.2.40/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/v2/binds.py` & `pinjected-0.2.40/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/v2/di.py` & `pinjected-0.2.40/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/v2/resolver.py` & `pinjected-0.2.40/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pinjected/visualize_di.py` & `pinjected-0.2.40/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.39/pyproject.toml` & `pinjected-0.2.40/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.39"
+version = "0.2.40"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.39/PKG-INFO` & `pinjected-0.2.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.39
+Version: 0.2.40
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

