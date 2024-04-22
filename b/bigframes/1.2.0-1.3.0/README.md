# Comparing `tmp/bigframes-1.2.0.tar.gz` & `tmp/bigframes-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigframes-1.2.0.tar", last modified: Tue Apr 16 17:11:39 2024, max compression
+gzip compressed data, was "bigframes-1.3.0.tar", last modified: Mon Apr 22 23:20:04 2024, max compression
```

## Comparing `bigframes-1.2.0.tar` & `bigframes-1.3.0.tar`

### file list

```diff
@@ -1,377 +1,379 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.986379 bigframes-1.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      914 2024-04-16 17:09:14.000000 bigframes-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4650 2024-04-16 17:11:39.986379 bigframes-1.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2256 2024-04-16 17:09:14.000000 bigframes-1.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.906391 bigframes-1.2.0/bigframes/
--rw-rw-r--   0 root         (0)     1003     1111 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.906391 bigframes-1.2.0/bigframes/_config/
--rw-rw-r--   0 root         (0)     1003     2453 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     8228 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/bigquery_options.py
--rw-rw-r--   0 root         (0)     1003     2141 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/compute_options.py
--rw-rw-r--   0 root         (0)     1003     1661 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/display_options.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/_config/sampling_options.py
--rw-rw-r--   0 root         (0)     1003     7152 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/clients.py
--rw-rw-r--   0 root         (0)     1003     2637 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/constants.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/
--rw-rw-r--   0 root         (0)     1003    15308 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/__init__.py
--rw-rw-r--   0 root         (0)     1003    29614 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/block_transforms.py
--rw-rw-r--   0 root         (0)     1003    91658 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/blocks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/compile/
--rw-rw-r--   0 root         (0)     1003      832 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/__init__.py
--rw-rw-r--   0 root         (0)     1003    17255 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/aggregate_compiler.py
--rw-rw-r--   0 root         (0)     1003    62857 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/compiled.py
--rw-rw-r--   0 root         (0)     1003     6694 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/compiler.py
--rw-rw-r--   0 root         (0)     1003     3356 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/concat.py
--rw-rw-r--   0 root         (0)     1003    47483 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/scalar_op_compiler.py
--rw-rw-r--   0 root         (0)     1003     7121 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/compile/single_column.py
--rw-rw-r--   0 root         (0)     1003     2369 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/convert.py
--rw-rw-r--   0 root         (0)     1003     2495 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/eval.py
--rw-rw-r--   0 root         (0)     1003     6768 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/expression.py
--rw-rw-r--   0 root         (0)     1003     1846 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/global_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.914389 bigframes-1.2.0/bigframes/core/groupby/
--rw-rw-r--   0 root         (0)     1003    22543 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/groupby/__init__.py
--rw-rw-r--   0 root         (0)     1003      716 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/guid.py
--rw-rw-r--   0 root         (0)     1003    18056 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/indexes/
--rw-rw-r--   0 root         (0)     1003      719 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003    16223 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     1720 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     1597 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/join_def.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/joins/
--rw-rw-r--   0 root         (0)     1003      691 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/joins/__init__.py
--rw-rw-r--   0 root         (0)     1003     2132 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/joins/merge.py
--rw-rw-r--   0 root         (0)     1003     2218 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/local_data.py
--rw-rw-r--   0 root         (0)     1003     2255 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/log_adapter.py
--rw-rw-r--   0 root         (0)     1003    21172 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/nodes.py
--rw-rw-r--   0 root         (0)     1003     9392 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/ordering.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/reshape/
--rw-rw-r--   0 root         (0)     1003     6872 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003    10722 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/rewrite.py
--rw-rw-r--   0 root         (0)     1003      746 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/scalar.py
--rw-rw-r--   0 root         (0)     1003     2144 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/schema.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/tools/
--rw-rw-r--   0 root         (0)     1003      664 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2515 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tools/datetimes.py
--rw-rw-r--   0 root         (0)     1003     3002 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/tree_properties.py
--rw-rw-r--   0 root         (0)     1003     5483 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/core/window/
--rw-rw-r--   0 root         (0)     1003     3075 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1286 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/core/window_spec.py
--rw-rw-r--   0 root         (0)     1003   130958 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/dataframe.py
--rw-rw-r--   0 root         (0)     1003    27474 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/dtypes.py
--rw-rw-r--   0 root         (0)     1003     1273 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/features.py
--rw-rw-r--   0 root         (0)     1003    11179 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/formatting_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.918389 bigframes-1.2.0/bigframes/functions/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003    39370 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/functions/remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.922388 bigframes-1.2.0/bigframes/ml/
--rw-rw-r--   0 root         (0)     1003      877 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     8542 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/base.py
--rw-rw-r--   0 root         (0)     1003     6659 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/cluster.py
--rw-rw-r--   0 root         (0)     1003     7984 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/compose.py
--rw-rw-r--   0 root         (0)     1003    15995 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/core.py
--rw-rw-r--   0 root         (0)     1003     6807 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/decomposition.py
--rw-rw-r--   0 root         (0)     1003    24746 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/ensemble.py
--rw-rw-r--   0 root         (0)     1003    15998 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/forecasting.py
--rw-rw-r--   0 root         (0)     1003     1141 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/globals.py
--rw-rw-r--   0 root         (0)     1003    10844 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/imported.py
--rw-rw-r--   0 root         (0)     1003    13818 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/linear_model.py
--rw-rw-r--   0 root         (0)     1003    27172 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/llm.py
--rw-rw-r--   0 root         (0)     1003     4899 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/loader.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/ml/metrics/
--rw-rw-r--   0 root         (0)     1003     1066 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/__init__.py
--rw-rw-r--   0 root         (0)     1003    11096 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/_metrics.py
--rw-rw-r--   0 root         (0)     1003     2373 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     3747 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/model_selection.py
--rw-rw-r--   0 root         (0)     1003     5067 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/pipeline.py
--rw-rw-r--   0 root         (0)     1003    22667 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/preprocessing.py
--rw-rw-r--   0 root         (0)     1003     5754 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/remote.py
--rw-rw-r--   0 root         (0)     1003    13312 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/sql.py
--rw-rw-r--   0 root         (0)     1003     2403 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/ml/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/operations/
--rw-rw-r--   0 root         (0)     1003    23014 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/operations/_matplotlib/
--rw-rw-r--   0 root         (0)     1003     1022 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/__init__.py
--rw-rw-r--   0 root         (0)     1003     4477 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/core.py
--rw-rw-r--   0 root         (0)     1003     5970 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/_matplotlib/hist.py
--rw-rw-r--   0 root         (0)     1003    12880 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/aggregations.py
--rw-rw-r--   0 root         (0)     1003     8273 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/base.py
--rw-rw-r--   0 root         (0)     1003     3079 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/datetimes.py
--rw-rw-r--   0 root         (0)     1003     2814 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/plotting.py
--rw-rw-r--   0 root         (0)     1003     9009 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/strings.py
--rw-rw-r--   0 root         (0)     1003     1679 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/structs.py
--rw-rw-r--   0 root         (0)     1003     7613 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/operations/type.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/pandas/
--rw-rw-r--   0 root         (0)     1003    23224 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/pandas/__init__.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/py.typed
--rw-rw-r--   0 root         (0)     1003    64129 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.926388 bigframes-1.2.0/bigframes/session/
--rw-rw-r--   0 root         (0)     1003    81282 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.930387 bigframes-1.2.0/bigframes/session/_io/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/__init__.py
--rw-rw-r--   0 root         (0)     1003     8040 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/bigquery.py
--rw-rw-r--   0 root         (0)     1003     4345 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/_io/pandas.py
--rw-rw-r--   0 root         (0)     1003     8043 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/session/clients.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/typing.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-16 17:09:14.000000 bigframes-1.2.0/bigframes/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/bigframes.egg-info/
--rw-r--r--   0 root         (0)     1003     4650 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    12253 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      732 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       29 2024-04-16 17:11:39.000000 bigframes-1.2.0/bigframes.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       81 2024-04-16 17:09:14.000000 bigframes-1.2.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003       67 2024-04-16 17:11:39.986379 bigframes-1.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     4428 2024-04-16 17:09:14.000000 bigframes-1.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.930387 bigframes-1.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/data/
--rw-rw-r--   0 root         (0)     1003      619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/hockey_players.json
--rw-rw-r--   0 root         (0)     1003     1250 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/hockey_players.jsonl
--rw-rw-r--   0 root         (0)     1003      340 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_2by3.json
--rw-rw-r--   0 root         (0)     1003       80 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_2by3.jsonl
--rw-rw-r--   0 root         (0)     1003      421 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_3by4.json
--rw-rw-r--   0 root         (0)     1003      154 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/matrix_3by4.jsonl
--rw-rw-r--   0 root         (0)     1003    33350 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/nested.jsonl
--rw-rw-r--   0 root         (0)     1003      966 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/nested_schema.json
--rw-rw-r--   0 root         (0)     1003    58869 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/penguins.jsonl
--rw-rw-r--   0 root         (0)     1003      636 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/penguins_schema.json
--rw-rw-r--   0 root         (0)     1003     3909 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/scalars.jsonl
--rw-rw-r--   0 root         (0)     1003     1458 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/scalars_schema.json
--rw-rw-r--   0 root         (0)     1003    23424 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/time_series.jsonl
--rw-rw-r--   0 root         (0)     1003      192 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/data/time_series_schema.json
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003    37000 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.934387 bigframes-1.2.0/tests/system/large/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.938386 bigframes-1.2.0/tests/system/large/ml/
--rw-rw-r--   0 root         (0)     1003     5411 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003     5391 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     6401 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6487 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    14451 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     4366 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     8408 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    30362 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003     4079 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_location.py
--rw-rw-r--   0 root         (0)     1003    49163 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003     1908 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/large/test_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.938386 bigframes-1.2.0/tests/system/load/
--rw-rw-r--   0 root         (0)     1003     2664 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/load/test_large_tables.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.942386 bigframes-1.2.0/tests/system/small/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003    11773 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/conftest.py
--rw-rw-r--   0 root         (0)     1003     7074 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003    13810 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6764 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    17015 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     6859 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     4983 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_imported.py
--rw-rw-r--   0 root         (0)     1003     8788 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    11541 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_llm.py
--rw-rw-r--   0 root         (0)     1003    25138 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_metrics.py
--rw-rw-r--   0 root         (0)     1003     2224 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_metrics_pairwise.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_model_selection.py
--rw-rw-r--   0 root         (0)     1003    27150 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_preprocessing.py
--rw-rw-r--   0 root         (0)     1003     2570 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_register.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/ml/test_remote.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/operations/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003    10399 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_datetimes.py
--rw-rw-r--   0 root         (0)     1003    12453 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_plotting.py
--rw-rw-r--   0 root         (0)     1003    15770 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/operations/test_strings.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.946385 bigframes-1.2.0/tests/system/small/regression/
--rw-rw-r--   0 root         (0)     1003     1999 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/regression/test_issue355_merge_after_filter.py
--rw-rw-r--   0 root         (0)     1003   139084 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003    18961 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_dataframe_io.py
--rw-rw-r--   0 root         (0)     1003    10570 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_encryption.py
--rw-rw-r--   0 root         (0)     1003    12922 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_groupby.py
--rw-rw-r--   0 root         (0)     1003     1558 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_ibis.py
--rw-rw-r--   0 root         (0)     1003    13328 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_index.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_ipython.py
--rw-rw-r--   0 root         (0)     1003    41010 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_multiindex.py
--rw-rw-r--   0 root         (0)     1003     4190 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_numpy.py
--rw-rw-r--   0 root         (0)     1003    19608 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     9533 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_pandas_options.py
--rw-rw-r--   0 root         (0)     1003     4126 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_progress_bar.py
--rw-rw-r--   0 root         (0)     1003    26485 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003      913 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_scalar.py
--rw-rw-r--   0 root         (0)     1003   107873 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_series.py
--rw-rw-r--   0 root         (0)     1003    40359 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_session.py
--rw-rw-r--   0 root         (0)     1003     3343 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/small/test_window.py
--rw-rw-r--   0 root         (0)     1003    12113 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/system/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.950384 bigframes-1.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.950384 bigframes-1.2.0/tests/unit/_config/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     2733 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/_config/test_bigquery_options.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/core/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/__init__.py
--rw-rw-r--   0 root         (0)     1003     1619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_bf_utils.py
--rw-rw-r--   0 root         (0)     1003     2966 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_blocks.py
--rw-rw-r--   0 root         (0)     1003     1553 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_expression.py
--rw-rw-r--   0 root         (0)     1003     1813 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/core/test_log_adapter.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     2323 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_api_primitives.py
--rw-rw-r--   0 root         (0)     1003     6555 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     7426 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_golden_sql.py
--rw-rw-r--   0 root         (0)     1003     4058 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003    13063 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/ml/test_sql.py
--rw-rw-r--   0 root         (0)     1003     4842 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.954384 bigframes-1.2.0/tests/unit/session/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/__init__.py
--rw-rw-r--   0 root         (0)     1003     4347 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_clients.py
--rw-rw-r--   0 root         (0)     1003     7809 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_io_bigquery.py
--rw-rw-r--   0 root         (0)     1003    18664 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_io_pandas.py
--rw-rw-r--   0 root         (0)     1003     6619 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/session/test_session.py
--rw-rw-r--   0 root         (0)     1003     1744 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_clients.py
--rw-rw-r--   0 root         (0)     1003     1056 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_compute_options.py
--rw-rw-r--   0 root         (0)     1003     6648 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_core.py
--rw-rw-r--   0 root         (0)     1003     2136 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003     8819 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_dtypes.py
--rw-rw-r--   0 root         (0)     1003     1577 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_features.py
--rw-rw-r--   0 root         (0)     1003      528 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_formatting_helper.py
--rw-rw-r--   0 root         (0)     1003     1655 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_formatting_helpers.py
--rw-rw-r--   0 root         (0)     1003     4055 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     1207 2024-04-16 17:09:14.000000 bigframes-1.2.0/tests/unit/test_remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.894392 bigframes-1.2.0/third_party/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/cpython/
--rw-rw-r--   0 root         (0)     1003     2339 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/__init__.py
--rw-rw-r--   0 root         (0)     1003    18854 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/cpython/_pprint.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     5290 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    14045 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/LICENSE.txt
--rw-rw-r--   0 root         (0)     1003    11663 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.958383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/
--rw-rw-r--   0 root         (0)     1003      184 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2091 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
--rw-rw-r--   0 root         (0)     1003     6600 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
--rw-rw-r--   0 root         (0)     1003     1582 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/
--rw-rw-r--   0 root         (0)     1003      464 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003      536 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
--rw-rw-r--   0 root         (0)     1003      276 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
--rw-rw-r--   0 root         (0)     1003      263 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
--rw-rw-r--   0 root         (0)     1003      690 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/pandas/
--rw-rw-r--   0 root         (0)     1003     2284 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/AUTHORS.md
--rw-rw-r--   0 root         (0)     1003     1634 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/LICENSE
--rw-rw-r--   0 root         (0)     1003    10620 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.962383 bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/
--rw-rw-r--   0 root         (0)     1003     1347 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.966382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
--rw-rw-r--   0 root         (0)     1003     2824 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
--rw-rw-r--   0 root         (0)     1003     3689 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
--rw-rw-r--   0 root         (0)     1003     2086 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/common.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/
--rw-rw-r--   0 root         (0)     1003     6944 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/align.py
--rw-rw-r--   0 root         (0)     1003     1543 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/common.py
--rw-rw-r--   0 root         (0)     1003     2295 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
--rw-rw-r--   0 root         (0)     1003    12685 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
--rw-rw-r--   0 root         (0)     1003    25132 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
--rw-rw-r--   0 root         (0)     1003    16244 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
--rw-rw-r--   0 root         (0)     1003     6477 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
--rw-rw-r--   0 root         (0)     1003    10303 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
--rw-rw-r--   0 root         (0)     1003     4394 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/config_init.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/
--rw-rw-r--   0 root         (0)     1003      707 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
--rw-rw-r--   0 root         (0)     1003   224405 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/frame.py
--rw-rw-r--   0 root         (0)     1003    40214 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/generic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/
--rw-rw-r--   0 root         (0)     1003    12988 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003     9588 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
--rw-rw-r--   0 root         (0)     1003    11461 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     2941 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     2909 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003     4372 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
--rw-rw-r--   0 root         (0)     1003     3804 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
--rw-rw-r--   0 root         (0)     1003     3220 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
--rw-rw-r--   0 root         (0)     1003     5844 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
--rw-rw-r--   0 root         (0)     1003   130169 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.970382 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/strings/
--rw-rw-r--   0 root         (0)     1003    37771 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2964 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1350 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/__init__.py
--rw-rw-r--   0 root         (0)     1003     1269 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/common.py
--rw-rw-r--   0 root         (0)     1003     6612 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/gbq.py
--rw-rw-r--   0 root         (0)     1003     1428 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parquet.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
--rw-rw-r--   0 root         (0)     1003    10553 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
--rw-rw-r--   0 root         (0)     1003     3130 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/pickle.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/
--rw-rw-r--   0 root         (0)     1003    12353 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/
--rw-rw-r--   0 root         (0)     1003    11128 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/_core.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.974381 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/
--rw-rw-r--   0 root         (0)     1003      765 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
--rw-rw-r--   0 root         (0)     1003     1573 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_validators.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/
--rw-rw-r--   0 root         (0)     1003     1532 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/COPYING
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/__init__.py
--rw-rw-r--   0 root         (0)     1003     6211 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/base.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/
--rw-rw-r--   0 root         (0)     1003     5924 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/
--rw-rw-r--   0 root         (0)     1003     2014 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/
--rw-rw-r--   0 root         (0)     1003     5387 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
--rw-rw-r--   0 root         (0)     1003     8979 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/
--rw-rw-r--   0 root         (0)     1003     5417 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
--rw-rw-r--   0 root         (0)     1003     4348 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.978381 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/
--rw-rw-r--   0 root         (0)     1003     9779 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
--rw-rw-r--   0 root         (0)     1003     6347 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
--rw-rw-r--   0 root         (0)     1003     3550 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
--rw-rw-r--   0 root         (0)     1003     2121 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     2973 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/pipeline.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/
--rw-rw-r--   0 root         (0)     1003     4980 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
--rw-rw-r--   0 root         (0)     1003     1523 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
--rw-rw-r--   0 root         (0)     1003     3753 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
--rw-rw-r--   0 root         (0)     1003     2085 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 17:11:39.982380 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/__init__.py
--rw-rw-r--   0 root         (0)     1003     6921 2024-04-16 17:09:14.000000 bigframes-1.2.0/third_party/bigframes_vendored/xgboost/sklearn.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.639690 bigframes-1.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      914 2024-04-22 23:17:27.000000 bigframes-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4650 2024-04-22 23:20:04.639690 bigframes-1.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2256 2024-04-22 23:17:27.000000 bigframes-1.3.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.563684 bigframes-1.3.0/bigframes/
+-rw-rw-r--   0 root         (0)     1003     1111 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.563684 bigframes-1.3.0/bigframes/_config/
+-rw-rw-r--   0 root         (0)     1003     2453 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8953 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/bigquery_options.py
+-rw-rw-r--   0 root         (0)     1003     2141 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/compute_options.py
+-rw-rw-r--   0 root         (0)     1003     1661 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/display_options.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/_config/sampling_options.py
+-rw-rw-r--   0 root         (0)     1003     7152 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/clients.py
+-rw-rw-r--   0 root         (0)     1003     2709 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/constants.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/
+-rw-rw-r--   0 root         (0)     1003    18183 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30768 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/block_transforms.py
+-rw-rw-r--   0 root         (0)     1003    91562 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/blocks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/compile/
+-rw-rw-r--   0 root         (0)     1003      832 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17475 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/aggregate_compiler.py
+-rw-rw-r--   0 root         (0)     1003    51565 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/compiled.py
+-rw-rw-r--   0 root         (0)     1003     6341 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/compiler.py
+-rw-rw-r--   0 root         (0)     1003     3356 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/concat.py
+-rw-rw-r--   0 root         (0)     1003    48952 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/scalar_op_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7121 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/compile/single_column.py
+-rw-rw-r--   0 root         (0)     1003     2369 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/convert.py
+-rw-rw-r--   0 root         (0)     1003     2495 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/eval.py
+-rw-rw-r--   0 root         (0)     1003     6685 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/expression.py
+-rw-rw-r--   0 root         (0)     1003     1846 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/global_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    23982 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/groupby/__init__.py
+-rw-rw-r--   0 root         (0)     1003      716 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/guid.py
+-rw-rw-r--   0 root         (0)     1003    18056 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.571685 bigframes-1.3.0/bigframes/core/indexes/
+-rw-rw-r--   0 root         (0)     1003      719 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16223 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     1720 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     1730 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/join_def.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/joins/
+-rw-rw-r--   0 root         (0)     1003      691 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/joins/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2132 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/joins/merge.py
+-rw-rw-r--   0 root         (0)     1003     2218 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/local_data.py
+-rw-rw-r--   0 root         (0)     1003     2255 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/log_adapter.py
+-rw-rw-r--   0 root         (0)     1003    18515 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/nodes.py
+-rw-rw-r--   0 root         (0)     1003     9392 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/ordering.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/reshape/
+-rw-rw-r--   0 root         (0)     1003     6872 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10722 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/rewrite.py
+-rw-rw-r--   0 root         (0)     1003      746 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/scalar.py
+-rw-rw-r--   0 root         (0)     1003     2144 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/schema.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/tools/
+-rw-rw-r--   0 root         (0)     1003      664 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2515 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tools/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     3002 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/tree_properties.py
+-rw-rw-r--   0 root         (0)     1003     5483 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/core/window/
+-rw-rw-r--   0 root         (0)     1003     3075 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1286 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/core/window_spec.py
+-rw-rw-r--   0 root         (0)     1003   131677 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/dataframe.py
+-rw-rw-r--   0 root         (0)     1003    27474 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/dtypes.py
+-rw-rw-r--   0 root         (0)     1003      666 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1273 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/features.py
+-rw-rw-r--   0 root         (0)     1003    11179 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/formatting_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.575685 bigframes-1.3.0/bigframes/functions/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40641 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/functions/remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.579686 bigframes-1.3.0/bigframes/ml/
+-rw-rw-r--   0 root         (0)     1003      877 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8542 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/base.py
+-rw-rw-r--   0 root         (0)     1003     6659 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/cluster.py
+-rw-rw-r--   0 root         (0)     1003     7984 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/compose.py
+-rw-rw-r--   0 root         (0)     1003    17608 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/core.py
+-rw-rw-r--   0 root         (0)     1003     6807 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/decomposition.py
+-rw-rw-r--   0 root         (0)     1003    24746 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/ensemble.py
+-rw-rw-r--   0 root         (0)     1003    15998 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/forecasting.py
+-rw-rw-r--   0 root         (0)     1003     1141 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/globals.py
+-rw-rw-r--   0 root         (0)     1003    10844 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/imported.py
+-rw-rw-r--   0 root         (0)     1003    13818 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/linear_model.py
+-rw-rw-r--   0 root         (0)     1003    29649 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/llm.py
+-rw-rw-r--   0 root         (0)     1003     4899 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/loader.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.579686 bigframes-1.3.0/bigframes/ml/metrics/
+-rw-rw-r--   0 root         (0)     1003     1066 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11096 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2373 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     3748 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/model_selection.py
+-rw-rw-r--   0 root         (0)     1003     5067 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/pipeline.py
+-rw-rw-r--   0 root         (0)     1003    22667 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     5754 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/remote.py
+-rw-rw-r--   0 root         (0)     1003    13949 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/sql.py
+-rw-rw-r--   0 root         (0)     1003     2403 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/ml/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/operations/
+-rw-rw-r--   0 root         (0)     1003    23377 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/operations/_matplotlib/
+-rw-rw-r--   0 root         (0)     1003     1022 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4477 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/core.py
+-rw-rw-r--   0 root         (0)     1003     5970 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/_matplotlib/hist.py
+-rw-rw-r--   0 root         (0)     1003    13202 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/aggregations.py
+-rw-rw-r--   0 root         (0)     1003     8273 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/base.py
+-rw-rw-r--   0 root         (0)     1003     3079 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     2814 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/plotting.py
+-rw-rw-r--   0 root         (0)     1003     9009 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/strings.py
+-rw-rw-r--   0 root         (0)     1003     2089 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/structs.py
+-rw-rw-r--   0 root         (0)     1003     7613 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/operations/type.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/pandas/
+-rw-rw-r--   0 root         (0)     1003    23314 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/pandas/__init__.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/py.typed
+-rw-rw-r--   0 root         (0)     1003    64553 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/session/
+-rw-rw-r--   0 root         (0)     1003    82333 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.583686 bigframes-1.3.0/bigframes/session/_io/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9139 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/bigquery.py
+-rw-rw-r--   0 root         (0)     1003     4345 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/_io/pandas.py
+-rw-rw-r--   0 root         (0)     1003     8043 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/session/clients.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/typing.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-22 23:17:27.000000 bigframes-1.3.0/bigframes/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/bigframes.egg-info/
+-rw-r--r--   0 root         (0)     1003     4650 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    12307 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      732 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       29 2024-04-22 23:20:04.000000 bigframes-1.3.0/bigframes.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       81 2024-04-22 23:17:27.000000 bigframes-1.3.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-22 23:20:04.639690 bigframes-1.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4428 2024-04-22 23:17:27.000000 bigframes-1.3.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.587686 bigframes-1.3.0/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.587686 bigframes-1.3.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003      619 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/hockey_players.json
+-rw-rw-r--   0 root         (0)     1003     1250 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/hockey_players.jsonl
+-rw-rw-r--   0 root         (0)     1003      340 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_2by3.json
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_2by3.jsonl
+-rw-rw-r--   0 root         (0)     1003      421 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_3by4.json
+-rw-rw-r--   0 root         (0)     1003      154 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/matrix_3by4.jsonl
+-rw-rw-r--   0 root         (0)     1003    33350 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/nested.jsonl
+-rw-rw-r--   0 root         (0)     1003      966 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/nested_schema.json
+-rw-rw-r--   0 root         (0)     1003    58869 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/penguins.jsonl
+-rw-rw-r--   0 root         (0)     1003      636 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/penguins_schema.json
+-rw-rw-r--   0 root         (0)     1003     3909 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/scalars.jsonl
+-rw-rw-r--   0 root         (0)     1003     1458 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/scalars_schema.json
+-rw-rw-r--   0 root         (0)     1003    23424 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/time_series.jsonl
+-rw-rw-r--   0 root         (0)     1003      192 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/data/time_series_schema.json
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37000 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/large/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.591686 bigframes-1.3.0/tests/system/large/ml/
+-rw-rw-r--   0 root         (0)     1003     5411 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003     5391 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     6401 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6487 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    14451 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     4366 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     8408 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    30362 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003     4079 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_location.py
+-rw-rw-r--   0 root         (0)     1003    50275 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003     1908 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/large/test_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.595687 bigframes-1.3.0/tests/system/load/
+-rw-rw-r--   0 root         (0)     1003     2664 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/load/test_large_tables.py
+-rw-rw-r--   0 root         (0)     1003     2970 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/load/test_llm.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.599687 bigframes-1.3.0/tests/system/small/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11773 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/conftest.py
+-rw-rw-r--   0 root         (0)     1003     7074 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003    13810 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6764 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    17015 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     6859 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     4983 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_imported.py
+-rw-rw-r--   0 root         (0)     1003     8788 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    11541 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_llm.py
+-rw-rw-r--   0 root         (0)     1003    25138 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2224 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_metrics_pairwise.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_model_selection.py
+-rw-rw-r--   0 root         (0)     1003    27150 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     2570 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_register.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/ml/test_remote.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/operations/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10399 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_datetimes.py
+-rw-rw-r--   0 root         (0)     1003    12453 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_plotting.py
+-rw-rw-r--   0 root         (0)     1003    15770 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/operations/test_strings.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.603687 bigframes-1.3.0/tests/system/small/regression/
+-rw-rw-r--   0 root         (0)     1003     1999 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/regression/test_issue355_merge_after_filter.py
+-rw-rw-r--   0 root         (0)     1003   140298 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003    18961 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_dataframe_io.py
+-rw-rw-r--   0 root         (0)     1003    10570 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_encryption.py
+-rw-rw-r--   0 root         (0)     1003    13974 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_groupby.py
+-rw-rw-r--   0 root         (0)     1003     1558 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_ibis.py
+-rw-rw-r--   0 root         (0)     1003    13328 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_index.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_ipython.py
+-rw-rw-r--   0 root         (0)     1003    41010 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_multiindex.py
+-rw-rw-r--   0 root         (0)     1003     4190 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_numpy.py
+-rw-rw-r--   0 root         (0)     1003    19608 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     9533 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_pandas_options.py
+-rw-rw-r--   0 root         (0)     1003     4126 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_progress_bar.py
+-rw-rw-r--   0 root         (0)     1003    26485 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003      913 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_scalar.py
+-rw-rw-r--   0 root         (0)     1003   108974 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_series.py
+-rw-rw-r--   0 root         (0)     1003    40386 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_session.py
+-rw-rw-r--   0 root         (0)     1003     3343 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/small/test_window.py
+-rw-rw-r--   0 root         (0)     1003    12113 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/system/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/_config/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4218 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/_config/test_bigquery_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.607688 bigframes-1.3.0/tests/unit/core/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1619 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_bf_utils.py
+-rw-rw-r--   0 root         (0)     1003     2966 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_blocks.py
+-rw-rw-r--   0 root         (0)     1003     1553 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_expression.py
+-rw-rw-r--   0 root         (0)     1003     1813 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/core/test_log_adapter.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/tests/unit/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2323 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_api_primitives.py
+-rw-rw-r--   0 root         (0)     1003     6555 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     7426 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_golden_sql.py
+-rw-rw-r--   0 root         (0)     1003     4058 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003    13789 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/ml/test_sql.py
+-rw-rw-r--   0 root         (0)     1003     4931 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/tests/unit/session/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4347 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     7809 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_io_bigquery.py
+-rw-rw-r--   0 root         (0)     1003    18664 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_io_pandas.py
+-rw-rw-r--   0 root         (0)     1003     8099 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/session/test_session.py
+-rw-rw-r--   0 root         (0)     1003     1744 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     1056 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_compute_options.py
+-rw-rw-r--   0 root         (0)     1003     6648 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_core.py
+-rw-rw-r--   0 root         (0)     1003     2136 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003     8819 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1577 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_features.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_formatting_helper.py
+-rw-rw-r--   0 root         (0)     1003     1655 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_formatting_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4055 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     1207 2024-04-22 23:17:27.000000 bigframes-1.3.0/tests/unit/test_remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.551684 bigframes-1.3.0/third_party/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/cpython/
+-rw-rw-r--   0 root         (0)     1003     2339 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18854 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/cpython/_pprint.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5290 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.611688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14045 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/LICENSE.txt
+-rw-rw-r--   0 root         (0)     1003    11663 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/
+-rw-rw-r--   0 root         (0)     1003      184 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2091 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
+-rw-rw-r--   0 root         (0)     1003     6600 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.615688 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/
+-rw-rw-r--   0 root         (0)     1003      464 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      536 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
+-rw-rw-r--   0 root         (0)     1003      276 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
+-rw-rw-r--   0 root         (0)     1003      263 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
+-rw-rw-r--   0 root         (0)     1003      690 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/
+-rw-rw-r--   0 root         (0)     1003     2284 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/AUTHORS.md
+-rw-rw-r--   0 root         (0)     1003     1634 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/LICENSE
+-rw-rw-r--   0 root         (0)     1003    10620 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/
+-rw-rw-r--   0 root         (0)     1003     1347 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.619688 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3831 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
+-rw-rw-r--   0 root         (0)     1003     3689 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
+-rw-rw-r--   0 root         (0)     1003     2086 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/common.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/
+-rw-rw-r--   0 root         (0)     1003     6944 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/align.py
+-rw-rw-r--   0 root         (0)     1003     1543 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/common.py
+-rw-rw-r--   0 root         (0)     1003     2295 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
+-rw-rw-r--   0 root         (0)     1003    12685 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
+-rw-rw-r--   0 root         (0)     1003    25132 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
+-rw-rw-r--   0 root         (0)     1003    16244 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
+-rw-rw-r--   0 root         (0)     1003     6477 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
+-rw-rw-r--   0 root         (0)     1003    10303 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
+-rw-rw-r--   0 root         (0)     1003     4394 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/config_init.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/
+-rw-rw-r--   0 root         (0)     1003      707 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
+-rw-rw-r--   0 root         (0)     1003   225813 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/frame.py
+-rw-rw-r--   0 root         (0)     1003    40215 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/generic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    14023 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.623689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9589 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
+-rw-rw-r--   0 root         (0)     1003    11461 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     2941 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     2909 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4372 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
+-rw-rw-r--   0 root         (0)     1003     3804 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
+-rw-rw-r--   0 root         (0)     1003     3220 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
+-rw-rw-r--   0 root         (0)     1003     5844 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
+-rw-rw-r--   0 root         (0)     1003   131185 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/
+-rw-rw-r--   0 root         (0)     1003    37771 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2964 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1269 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/common.py
+-rw-rw-r--   0 root         (0)     1003     7071 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/gbq.py
+-rw-rw-r--   0 root         (0)     1003     1428 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parquet.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10553 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
+-rw-rw-r--   0 root         (0)     1003     3130 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/pickle.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/
+-rw-rw-r--   0 root         (0)     1003    12353 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.627689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/_core.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/
+-rw-rw-r--   0 root         (0)     1003      765 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1573 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_validators.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/
+-rw-rw-r--   0 root         (0)     1003     1532 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/COPYING
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6212 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/base.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/
+-rw-rw-r--   0 root         (0)     1003     5924 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/
+-rw-rw-r--   0 root         (0)     1003     2014 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/
+-rw-rw-r--   0 root         (0)     1003     5387 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8979 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/
+-rw-rw-r--   0 root         (0)     1003     5417 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
+-rw-rw-r--   0 root         (0)     1003     4348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.631689 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/
+-rw-rw-r--   0 root         (0)     1003     9783 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
+-rw-rw-r--   0 root         (0)     1003     6347 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
+-rw-rw-r--   0 root         (0)     1003     3550 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
+-rw-rw-r--   0 root         (0)     1003     2121 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     2980 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/pipeline.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/
+-rw-rw-r--   0 root         (0)     1003     4980 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
+-rw-rw-r--   0 root         (0)     1003     1523 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
+-rw-rw-r--   0 root         (0)     1003     4064 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
+-rw-rw-r--   0 root         (0)     1003     2085 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-22 23:20:04.635690 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6921 2024-04-22 23:17:27.000000 bigframes-1.3.0/third_party/bigframes_vendored/xgboost/sklearn.py
```

### Comparing `bigframes-1.2.0/LICENSE` & `bigframes-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/MANIFEST.in` & `bigframes-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/PKG-INFO` & `bigframes-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.2.0
+Version: 1.3.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: fsspec>=2023.3.0
 Requires-Dist: gcsfs>=2023.3.0
 Requires-Dist: geopandas>=0.12.2
 Requires-Dist: google-auth<3.0dev,>=2.15.0
-Requires-Dist: google-cloud-bigquery[bqstorage,pandas]>=3.10.0
+Requires-Dist: google-cloud-bigquery[bqstorage,pandas]>=3.16.0
 Requires-Dist: google-cloud-functions>=1.12.0
 Requires-Dist: google-cloud-bigquery-connection>=1.12.0
 Requires-Dist: google-cloud-iam>=2.12.1
 Requires-Dist: google-cloud-resource-manager>=1.10.3
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: ibis-framework[bigquery]<9.0.0dev,>=8.0.0
 Requires-Dist: pandas>=1.5.0
```

### Comparing `bigframes-1.2.0/README.rst` & `bigframes-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/__init__.py` & `bigframes-1.3.0/bigframes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/_config/__init__.py` & `bigframes-1.3.0/bigframes/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/_config/bigquery_options.py` & `bigframes-1.3.0/bigframes/_config/bigquery_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,41 @@
 
 from typing import Optional
 import warnings
 
 import google.api_core.exceptions
 import google.auth.credentials
 
+import bigframes.constants
+import bigframes.exceptions
+
 SESSION_STARTED_MESSAGE = (
     "Cannot change '{attribute}' once a session has started. "
     "Call bigframes.pandas.close_session() first, if you are using the bigframes.pandas API."
 )
 
+UNKNOWN_LOCATION_MESSAGE = "The location '{location}' is set to an unknown value."
+
+
+def _validate_location(value: Optional[str]):
+
+    if value is None:
+        return
+
+    if value not in bigframes.constants.ALL_BIGQUERY_LOCATIONS:
+        warnings.warn(
+            UNKNOWN_LOCATION_MESSAGE.format(location=value),
+            # There are many layers before we get to (possibly) the user's code:
+            # -> bpd.options.bigquery.location = "us-central-1"
+            # -> location.setter
+            # -> _validate_location
+            stacklevel=3,
+            category=bigframes.exceptions.UnknownLocationWarning,
+        )
+
 
 class BigQueryOptions:
     """Encapsulates configuration for working with a session."""
 
     def __init__(
         self,
         credentials: Optional[google.auth.credentials.Credentials] = None,
@@ -89,14 +111,15 @@
         """
         return self._location
 
     @location.setter
     def location(self, value: Optional[str]):
         if self._session_started and self._location != value:
             raise ValueError(SESSION_STARTED_MESSAGE.format(attribute="location"))
+        _validate_location(value)
         self._location = value
 
     @property
     def project(self) -> Optional[str]:
         """Google Cloud project ID to use for billing and as the default project."""
         return self._project
```

### Comparing `bigframes-1.2.0/bigframes/_config/compute_options.py` & `bigframes-1.3.0/bigframes/_config/compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/_config/display_options.py` & `bigframes-1.3.0/bigframes/_config/display_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/_config/sampling_options.py` & `bigframes-1.3.0/bigframes/_config/sampling_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/clients.py` & `bigframes-1.3.0/bigframes/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/constants.py` & `bigframes-1.3.0/bigframes/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,7 +88,10 @@
     }
 )
 
 # https://cloud.google.com/storage/docs/locational-endpoints
 LEP_ENABLED_BIGQUERY_LOCATIONS = frozenset(
     ALL_BIGQUERY_LOCATIONS - REP_ENABLED_BIGQUERY_LOCATIONS
 )
+
+# BigQuery default is 10000, leave 100 for overhead
+MAX_COLUMNS = 9900
```

### Comparing `bigframes-1.2.0/bigframes/core/__init__.py` & `bigframes-1.3.0/bigframes/core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -350,44 +350,106 @@
         row_labels: typing.Sequence[typing.Hashable],
         unpivot_columns: typing.Sequence[
             typing.Tuple[str, typing.Tuple[typing.Optional[str], ...]]
         ],
         *,
         passthrough_columns: typing.Sequence[str] = (),
         index_col_ids: typing.Sequence[str] = ["index"],
-        dtype: typing.Union[
-            bigframes.dtypes.Dtype, typing.Tuple[bigframes.dtypes.Dtype, ...]
-        ] = pandas.Float64Dtype(),
-        how: typing.Literal["left", "right"] = "left",
+        join_side: typing.Literal["left", "right"] = "left",
     ) -> ArrayValue:
         """
         Unpivot ArrayValue columns.
 
         Args:
             row_labels: Identifies the source of the row. Must be equal to length to source column list in unpivot_columns argument.
             unpivot_columns: Mapping of column id to list of input column ids. Lists of input columns may use None.
             passthrough_columns: Columns that will not be unpivoted. Column id will be preserved.
             index_col_id (str): The column id to be used for the row labels.
-            dtype (dtype or list of dtype): Dtype to use for the unpivot columns. If list, must be equal in number to unpivot_columns.
 
         Returns:
             ArrayValue: The unpivoted ArrayValue
         """
+        # There will be N labels, used to disambiguate which of N source columns produced each output row
+        explode_offsets_id = bigframes.core.guid.generate_guid("unpivot_offsets_")
+        labels_array = self._create_unpivot_labels_array(row_labels, index_col_ids)
+        labels_array = labels_array.promote_offsets(explode_offsets_id)
+
+        # Unpivot creates N output rows for each input row, labels disambiguate these N rows
+        joined_array = self._cross_join_w_labels(labels_array, join_side)
+
+        # Build the output rows as a case statment that selects between the N input columns
+        unpivot_exprs = []
+        # Supports producing multiple stacked ouput columns for stacking only part of hierarchical index
+        for col_id, input_ids in unpivot_columns:
+            # row explode offset used to choose the input column
+            # we use offset instead of label as labels are not necessarily unique
+            cases = tuple(
+                (
+                    ops.eq_op.as_expr(explode_offsets_id, ex.const(i)),
+                    ex.free_var(id_or_null)
+                    if (id_or_null is not None)
+                    else ex.const(None),
+                )
+                for i, id_or_null in enumerate(input_ids)
+            )
+            col_expr = ops.case_when_op.as_expr(*cases)
+            unpivot_exprs.append((col_expr, col_id))
+
+        label_exprs = ((ex.free_var(id), id) for id in index_col_ids)
+        # passthrough columns are unchanged, just repeated N times each
+        passthrough_exprs = ((ex.free_var(id), id) for id in passthrough_columns)
         return ArrayValue(
-            nodes.UnpivotNode(
-                child=self.node,
-                row_labels=tuple(row_labels),
-                unpivot_columns=tuple(unpivot_columns),
-                passthrough_columns=tuple(passthrough_columns),
-                index_col_ids=tuple(index_col_ids),
-                dtype=dtype,
-                how=how,
+            nodes.ProjectionNode(
+                child=joined_array.node,
+                assignments=(*label_exprs, *unpivot_exprs, *passthrough_exprs),
             )
         )
 
+    def _cross_join_w_labels(
+        self, labels_array: ArrayValue, join_side: typing.Literal["left", "right"]
+    ) -> ArrayValue:
+        """
+        Convert each row in self to N rows, one for each label in labels array.
+        """
+        table_join_side = (
+            join_def.JoinSide.LEFT if join_side == "left" else join_def.JoinSide.RIGHT
+        )
+        labels_join_side = table_join_side.inverse()
+        labels_mappings = tuple(
+            join_def.JoinColumnMapping(labels_join_side, id, id)
+            for id in labels_array.schema.names
+        )
+        table_mappings = tuple(
+            join_def.JoinColumnMapping(table_join_side, id, id)
+            for id in self.schema.names
+        )
+        join = join_def.JoinDefinition(
+            conditions=(), mappings=(*labels_mappings, *table_mappings), type="cross"
+        )
+        if join_side == "left":
+            joined_array = self.join(labels_array, join_def=join)
+        else:
+            joined_array = labels_array.join(self, join_def=join)
+        return joined_array
+
+    def _create_unpivot_labels_array(
+        self,
+        former_column_labels: typing.Sequence[typing.Hashable],
+        col_ids: typing.Sequence[str],
+    ) -> ArrayValue:
+        """Create an ArrayValue from a list of label tuples."""
+        rows = []
+        for row_offset in range(len(former_column_labels)):
+            row_label = former_column_labels[row_offset]
+            row_label = (row_label,) if not isinstance(row_label, tuple) else row_label
+            row = {col_ids[i]: row_label[i] for i in range(len(col_ids))}
+            rows.append(row)
+
+        return ArrayValue.from_pyarrow(pa.Table.from_pylist(rows), session=self.session)
+
     def join(
         self,
         other: ArrayValue,
         join_def: join_def.JoinDefinition,
         allow_row_identity_join: bool = False,
     ):
         join_node = nodes.JoinNode(
```

### Comparing `bigframes-1.2.0/bigframes/core/block_transforms.py` & `bigframes-1.3.0/bigframes/core/block_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import functools
 import typing
+from typing import Sequence
 
 import pandas as pd
 
 import bigframes.constants as constants
 import bigframes.core as core
 import bigframes.core.blocks as blocks
 import bigframes.core.expression as ex
@@ -101,14 +102,48 @@
                 val_count_col_id,
             )
         ),
         duplicate_indicator,
     )
 
 
+def quantile(
+    block: blocks.Block,
+    columns: Sequence[str],
+    qs: Sequence[float],
+    grouping_column_ids: Sequence[str] = (),
+    dropna: bool = False,
+) -> blocks.Block:
+    # TODO: handle windowing and more interpolation methods
+    window = core.WindowSpec(
+        grouping_keys=tuple(grouping_column_ids),
+    )
+    quantile_cols = []
+    labels = []
+    if len(columns) * len(qs) > constants.MAX_COLUMNS:
+        raise NotImplementedError("Too many aggregates requested.")
+    for col in columns:
+        for q in qs:
+            label = block.col_id_to_label[col]
+            new_label = (*label, q) if isinstance(label, tuple) else (label, q)
+            labels.append(new_label)
+            block, quantile_col = block.apply_window_op(
+                col,
+                agg_ops.QuantileOp(q),
+                window_spec=window,
+            )
+            quantile_cols.append(quantile_col)
+    block, results = block.aggregate(
+        grouping_column_ids,
+        tuple((col, agg_ops.AnyValueOp()) for col in quantile_cols),
+        dropna=dropna,
+    )
+    return block.select_columns(results).with_column_labels(labels)
+
+
 def interpolate(block: blocks.Block, method: str = "linear") -> blocks.Block:
     supported_methods = [
         "linear",
         "values",
         "index",
         "nearest",
         "zero",
@@ -819,9 +854,9 @@
 
     block = block.select_columns(result_cols).with_column_labels(
         original_block.column_labels
     )
     # Stack the entire column axis to produce single-column result
     # Assumption: uniform dtype for stackability
     return block.aggregate_all_and_stack(
-        agg_ops.AnyValueOp(), dtype=block.dtypes[0]
+        agg_ops.AnyValueOp(),
     ).with_column_labels([original_block.index.name])
```

### Comparing `bigframes-1.2.0/bigframes/core/blocks.py` & `bigframes-1.3.0/bigframes/core/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,32 +910,28 @@
     def aggregate_all_and_stack(
         self,
         operation: agg_ops.UnaryAggregateOp,
         *,
         axis: int | str = 0,
         value_col_id: str = "values",
         dropna: bool = True,
-        dtype: typing.Union[
-            bigframes.dtypes.Dtype, typing.Tuple[bigframes.dtypes.Dtype, ...]
-        ] = pd.Float64Dtype(),
     ) -> Block:
         axis_n = utils.get_axis_number(axis)
         if axis_n == 0:
             aggregations = [
                 (ex.UnaryAggregation(operation, ex.free_var(col_id)), col_id)
                 for col_id in self.value_columns
             ]
             index_col_ids = [
                 guid.generate_guid() for i in range(self.column_labels.nlevels)
             ]
             result_expr = self.expr.aggregate(aggregations, dropna=dropna).unpivot(
                 row_labels=self.column_labels.to_list(),
                 index_col_ids=index_col_ids,
                 unpivot_columns=tuple([(value_col_id, tuple(self.value_columns))]),
-                dtype=dtype,
             )
             return Block(
                 result_expr,
                 index_columns=index_col_ids,
                 column_labels=[None],
                 index_labels=self.column_labels.names,
             )
@@ -945,15 +941,14 @@
             offset_col = guid.generate_guid()
             expr_with_offsets = self.expr.promote_offsets(offset_col)
             stacked_expr = expr_with_offsets.unpivot(
                 row_labels=self.column_labels.to_list(),
                 index_col_ids=[guid.generate_guid()],
                 unpivot_columns=[(value_col_id, tuple(self.value_columns))],
                 passthrough_columns=[*self.index_columns, offset_col],
-                dtype=dtype,
             )
             index_aggregations = [
                 (ex.UnaryAggregation(agg_ops.AnyValueOp(), ex.free_var(col_id)), col_id)
                 for col_id in [*self.index_columns]
             ]
             main_aggregation = (
                 ex.UnaryAggregation(operation, ex.free_var(value_col_id)),
@@ -1494,39 +1489,40 @@
         # These are the values that will be turned into rows
 
         col_labels, row_labels = utils.split_index(self.column_labels, levels=levels)
         row_labels = row_labels.drop_duplicates()
 
         row_label_tuples = utils.index_as_tuples(row_labels)
 
-        if col_labels is not None:
+        if col_labels is None:
+            result_index: pd.Index = pd.Index([None])
+            result_col_labels: Sequence[Tuple] = list([()])
+        elif (col_labels.nlevels == 1) and all(
+            col_labels.isna()
+        ):  # isna not implemented for MultiIndex for newer pandas versions
+            result_index = pd.Index([None])
+            result_col_labels = utils.index_as_tuples(col_labels.drop_duplicates())
+        else:
             result_index = col_labels.drop_duplicates().dropna(how="all")
             result_col_labels = utils.index_as_tuples(result_index)
-        else:
-            result_index = pd.Index([None])
-            result_col_labels = list([()])
 
         # Get matching columns
         unpivot_columns: List[Tuple[str, List[str]]] = []
-        dtypes = []
         for val in result_col_labels:
             col_id = guid.generate_guid("unpivot_")
             input_columns, dtype = self._create_stack_column(val, row_label_tuples)
             unpivot_columns.append((col_id, input_columns))
-            if dtype:
-                dtypes.append(dtype or pd.Float64Dtype())
 
         added_index_columns = [guid.generate_guid() for _ in range(row_labels.nlevels)]
         unpivot_expr = self._expr.unpivot(
             row_labels=row_label_tuples,
             passthrough_columns=self.index_columns,
             unpivot_columns=unpivot_columns,
             index_col_ids=added_index_columns,
-            dtype=tuple(dtypes),
-            how=how,
+            join_side=how,
         )
         new_index_level_names = self.column_labels.names[-levels:]
         if how == "left":
             index_columns = [*self.index_columns, *added_index_columns]
             index_labels = [*self._index_labels, *new_index_level_names]
         else:
             index_columns = [*added_index_columns, *self.index_columns]
@@ -1550,23 +1546,20 @@
         unpivot_col_id = guid.generate_guid()
         var_col_ids = tuple([guid.generate_guid() for _ in var_names])
         # single unpivot col
         unpivot_col = (unpivot_col_id, tuple(value_vars))
         value_labels = [self.col_id_to_label[col_id] for col_id in value_vars]
         id_labels = [self.col_id_to_label[col_id] for col_id in id_vars]
 
-        dtype = self._expr.get_column_type(value_vars[0])
-
         unpivot_expr = self._expr.unpivot(
             row_labels=value_labels,
             passthrough_columns=id_vars,
             unpivot_columns=(unpivot_col,),
             index_col_ids=var_col_ids,
-            dtype=dtype,
-            how="right",
+            join_side="right",
         )
         index_id = guid.generate_guid()
         unpivot_expr = unpivot_expr.promote_offsets(index_id)
         # Need to reorder to get id_vars before var_col and unpivot_col
         unpivot_expr = unpivot_expr.select_columns(
             [index_id, *id_vars, *var_col_ids, unpivot_col_id]
         )
```

### Comparing `bigframes-1.2.0/bigframes/core/compile/__init__.py` & `bigframes-1.3.0/bigframes/core/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/compile/aggregate_compiler.py` & `bigframes-1.3.0/bigframes/core/compile/aggregate_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,22 @@
     ).to_expr()[op.quartile]
     return cast(ibis_types.NumericValue, value)
 
 
 @compile_unary_agg.register
 @numeric_op
 def _(
+    op: agg_ops.QuantileOp, column: ibis_types.NumericColumn, window=None
+) -> ibis_types.NumericValue:
+    return _apply_window_if_present(column.quantile(op.q), window)
+
+
+@compile_unary_agg.register
+@numeric_op
+def _(
     op: agg_ops.MeanOp, column: ibis_types.NumericColumn, window=None
 ) -> ibis_types.NumericValue:
     return _apply_window_if_present(column.mean(), window)
 
 
 @compile_unary_agg.register
 @numeric_op
```

### Comparing `bigframes-1.2.0/bigframes/core/compile/compiled.py` & `bigframes-1.3.0/bigframes/core/compile/compiled.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,16 @@
     ascending_over,
     encode_order_string,
     ExpressionOrdering,
     IntegerEncoding,
     OrderingExpression,
 )
 import bigframes.core.schema as schemata
-import bigframes.core.utils as utils
 from bigframes.core.window_spec import WindowSpec
 import bigframes.dtypes
-import bigframes.operations as ops
 import bigframes.operations.aggregations as agg_ops
 
 ORDER_ID_COLUMN = "bigframes_ordering_id"
 PREDICATE_COLUMN = "bigframes_predicate"
 
 
 T = typing.TypeVar("T", bound="BaseIbisIR")
@@ -106,44 +104,14 @@
 
     @abc.abstractmethod
     def filter(self: T, predicate: ex.Expression) -> T:
         """Filter the table on a given expression, the predicate must be a boolean expression."""
         ...
 
     @abc.abstractmethod
-    def unpivot(
-        self: T,
-        row_labels: typing.Sequence[typing.Hashable],
-        unpivot_columns: typing.Sequence[
-            typing.Tuple[str, typing.Sequence[typing.Optional[str]]]
-        ],
-        *,
-        passthrough_columns: typing.Sequence[str] = (),
-        index_col_ids: typing.Sequence[str] = ["index"],
-        dtype: typing.Union[
-            bigframes.dtypes.Dtype, typing.Sequence[bigframes.dtypes.Dtype]
-        ] = pandas.Float64Dtype(),
-        how="left",
-    ) -> T:
-        """
-        Unpivot ArrayValue columns.
-
-        Args:
-            row_labels: Identifies the source of the row. Must be equal to length to source column list in unpivot_columns argument.
-            unpivot_columns: Mapping of column id to list of input column ids. Lists of input columns may use None.
-            passthrough_columns: Columns that will not be unpivoted. Column id will be preserved.
-            index_col_id (str): The column id to be used for the row labels.
-            dtype (dtype or list of dtype): Dtype to use for the unpivot columns. If list, must be equal in number to unpivot_columns.
-
-        Returns:
-            ArrayValue: The unpivoted ArrayValue
-        """
-        ...
-
-    @abc.abstractmethod
     def _reproject_to_table(self: T) -> T:
         """
         Internal operators that projects the internal representation into a
         new ibis table expression where each value column is a direct
         reference to a column in that table expression. Needed after
         some operations such as window operations that cannot be used
         recursively in projections.
@@ -328,123 +296,14 @@
 
     def _filter(self, predicate_value: ibis_types.BooleanValue) -> UnorderedIR:
         """Filter the table on a given expression, the predicate must be a boolean series aligned with the table expression."""
         expr = self.builder()
         expr.predicates = [*self._predicates, predicate_value]
         return expr.build()
 
-    def unpivot(
-        self,
-        row_labels: typing.Sequence[typing.Hashable],
-        unpivot_columns: typing.Sequence[
-            typing.Tuple[str, typing.Sequence[typing.Optional[str]]]
-        ],
-        *,
-        passthrough_columns: typing.Sequence[str] = (),
-        index_col_ids: typing.Sequence[str] = ["index"],
-        dtype: typing.Union[
-            bigframes.dtypes.Dtype, typing.Sequence[bigframes.dtypes.Dtype]
-        ] = pandas.Float64Dtype(),
-        how="left",
-    ) -> UnorderedIR:
-        if how not in ("left", "right"):
-            raise ValueError("'how' must be 'left' or 'right'")
-        table = self._to_ibis_expr()
-        row_n = len(row_labels)
-        if not all(
-            len(source_columns) == row_n for _, source_columns in unpivot_columns
-        ):
-            raise ValueError("Columns and row labels must all be same length.")
-
-        unpivot_offset_id = bigframes.core.guid.generate_guid("unpivot_offsets_")
-        unpivot_table = table.cross_join(
-            ibis.memtable({unpivot_offset_id: range(row_n)})
-        )
-        # Use ibis memtable to infer type of rowlabels (if possible)
-        # TODO: Allow caller to specify dtype
-        if isinstance(row_labels[0], tuple):
-            labels_table = ibis.memtable(row_labels)
-            labels_ibis_types = [
-                labels_table[col].type() for col in labels_table.columns
-            ]
-        else:
-            labels_ibis_types = [ibis.memtable({"col": row_labels})["col"].type()]
-        labels_dtypes = [
-            bigframes.dtypes.ibis_dtype_to_bigframes_dtype(ibis_type)
-            for ibis_type in labels_ibis_types
-        ]
-
-        label_columns = []
-        for label_part, (col_id, label_dtype) in enumerate(
-            zip(index_col_ids, labels_dtypes)
-        ):
-            # interpret as tuples even if it wasn't originally so can apply same logic for multi-column labels
-            labels_as_tuples = [
-                label if isinstance(label, tuple) else (label,) for label in row_labels
-            ]
-            cases = [
-                (
-                    i,
-                    bigframes.dtypes.literal_to_ibis_scalar(
-                        label_tuple[label_part],  # type:ignore
-                        force_dtype=label_dtype,  # type:ignore
-                    ),
-                )
-                for i, label_tuple in enumerate(labels_as_tuples)
-            ]
-            labels_value = (
-                typing.cast(ibis_types.IntegerColumn, unpivot_table[unpivot_offset_id])
-                .cases(cases, default=None)  # type:ignore
-                .name(col_id)
-            )
-            label_columns.append(labels_value)
-
-        unpivot_values = []
-        for j in range(len(unpivot_columns)):
-            col_dtype = dtype[j] if utils.is_list_like(dtype) else dtype
-            result_col, source_cols = unpivot_columns[j]
-            null_value = bigframes.dtypes.literal_to_ibis_scalar(
-                None, force_dtype=col_dtype
-            )
-            ibis_values = [
-                op_compiler.compile_row_op(
-                    ops.AsTypeOp(col_dtype), (unpivot_table[col],)
-                )
-                if col is not None
-                else null_value
-                for col in source_cols
-            ]
-            cases = [(i, ibis_values[i]) for i in range(len(ibis_values))]
-            unpivot_value = typing.cast(
-                ibis_types.IntegerColumn, unpivot_table[unpivot_offset_id]
-            ).cases(
-                cases, default=null_value  # type:ignore
-            )
-            unpivot_values.append(unpivot_value.name(result_col))
-
-        unpivot_table = unpivot_table.select(
-            passthrough_columns,
-            *label_columns,
-            *unpivot_values,
-            unpivot_offset_id,
-        )
-
-        value_columns = [
-            unpivot_table[value_col_id] for value_col_id, _ in unpivot_columns
-        ]
-        passthrough_values = [unpivot_table[col] for col in passthrough_columns]
-        return UnorderedIR(
-            table=unpivot_table,
-            columns=[
-                *[unpivot_table[col_id] for col_id in index_col_ids],
-                *value_columns,
-                *passthrough_values,
-            ],
-        )
-
     def aggregate(
         self,
         aggregations: typing.Sequence[typing.Tuple[ex.Aggregation, str]],
         by_column_ids: typing.Sequence[str] = (),
         dropna: bool = True,
     ) -> OrderedIR:
         """
@@ -916,157 +775,14 @@
             case_statement = case_statement.else_(window_op).end()  # type: ignore
             window_op = case_statement
 
         result = self._set_or_replace_by_id(output_name or column_name, window_op)
         # TODO(tbergeron): Automatically track analytic expression usage and defer reprojection until required for valid query generation.
         return result._reproject_to_table() if not skip_reproject_unsafe else result
 
-    def unpivot(
-        self,
-        row_labels: typing.Sequence[typing.Hashable],
-        unpivot_columns: typing.Sequence[
-            typing.Tuple[str, typing.Sequence[typing.Optional[str]]]
-        ],
-        *,
-        passthrough_columns: typing.Sequence[str] = (),
-        index_col_ids: typing.Sequence[str] = ["index"],
-        dtype: typing.Union[
-            bigframes.dtypes.Dtype, typing.Sequence[bigframes.dtypes.Dtype]
-        ] = pandas.Float64Dtype(),
-        how="left",
-    ) -> OrderedIR:
-        if how not in ("left", "right"):
-            raise ValueError("'how' must be 'left' or 'right'")
-        table = self._to_ibis_expr(ordering_mode="unordered", expose_hidden_cols=True)
-        row_n = len(row_labels)
-        hidden_col_ids = self._hidden_ordering_column_names.keys()
-        if not all(
-            len(source_columns) == row_n for _, source_columns in unpivot_columns
-        ):
-            raise ValueError("Columns and row labels must all be same length.")
-
-        unpivot_offset_id = bigframes.core.guid.generate_guid("unpivot_offsets_")
-        unpivot_table = table.cross_join(
-            ibis.memtable({unpivot_offset_id: range(row_n)})
-        )
-        # Use ibis memtable to infer type of rowlabels (if possible)
-        # TODO: Allow caller to specify dtype
-        if isinstance(row_labels[0], tuple):
-            labels_table = ibis.memtable(row_labels)
-            labels_ibis_types = [
-                labels_table[col].type() for col in labels_table.columns
-            ]
-        else:
-            labels_ibis_types = [ibis.memtable({"col": row_labels})["col"].type()]
-        labels_dtypes = [
-            bigframes.dtypes.ibis_dtype_to_bigframes_dtype(ibis_type)
-            for ibis_type in labels_ibis_types
-        ]
-
-        label_columns = []
-        for label_part, (col_id, label_dtype) in enumerate(
-            zip(index_col_ids, labels_dtypes)
-        ):
-            # interpret as tuples even if it wasn't originally so can apply same logic for multi-column labels
-            labels_as_tuples = [
-                label if isinstance(label, tuple) else (label,) for label in row_labels
-            ]
-            cases = [
-                (
-                    i,
-                    bigframes.dtypes.literal_to_ibis_scalar(
-                        label_tuple[label_part],  # type:ignore
-                        force_dtype=label_dtype,  # type:ignore
-                    ),
-                )
-                for i, label_tuple in enumerate(labels_as_tuples)
-            ]
-            labels_value = (
-                typing.cast(ibis_types.IntegerColumn, unpivot_table[unpivot_offset_id])
-                .cases(cases, default=None)  # type:ignore
-                .name(col_id)
-            )
-            label_columns.append(labels_value)
-
-        unpivot_values = []
-        for j in range(len(unpivot_columns)):
-            col_dtype = dtype[j] if utils.is_list_like(dtype) else dtype
-            result_col, source_cols = unpivot_columns[j]
-            null_value = bigframes.dtypes.literal_to_ibis_scalar(
-                None, force_dtype=col_dtype
-            )
-            ibis_values = [
-                op_compiler.compile_row_op(
-                    ops.AsTypeOp(col_dtype), (unpivot_table[col],)
-                )
-                if col is not None
-                else null_value
-                for col in source_cols
-            ]
-            cases = [(i, ibis_values[i]) for i in range(len(ibis_values))]
-            unpivot_value = typing.cast(
-                ibis_types.IntegerColumn, unpivot_table[unpivot_offset_id]
-            ).cases(
-                cases, default=null_value  # type:ignore
-            )
-            unpivot_values.append(unpivot_value.name(result_col))
-
-        unpivot_table = unpivot_table.select(
-            passthrough_columns,
-            *label_columns,
-            *unpivot_values,
-            *hidden_col_ids,
-            unpivot_offset_id,
-        )
-
-        # Extend the original ordering using unpivot_offset_id
-        old_ordering = self._ordering
-        if how == "left":
-            new_ordering = ExpressionOrdering(
-                ordering_value_columns=tuple(
-                    [
-                        *old_ordering.ordering_value_columns,
-                        ascending_over(unpivot_offset_id),
-                    ]
-                ),
-                total_ordering_columns=frozenset(
-                    [*old_ordering.total_ordering_columns, unpivot_offset_id]
-                ),
-            )
-        else:  # how=="right"
-            new_ordering = ExpressionOrdering(
-                ordering_value_columns=tuple(
-                    [
-                        ascending_over(unpivot_offset_id),
-                        *old_ordering.ordering_value_columns,
-                    ]
-                ),
-                total_ordering_columns=frozenset(
-                    [*old_ordering.total_ordering_columns, unpivot_offset_id]
-                ),
-            )
-        value_columns = [
-            unpivot_table[value_col_id] for value_col_id, _ in unpivot_columns
-        ]
-        passthrough_values = [unpivot_table[col] for col in passthrough_columns]
-        hidden_ordering_columns = [
-            unpivot_table[unpivot_offset_id],
-            *[unpivot_table[hidden_col] for hidden_col in hidden_col_ids],
-        ]
-        return OrderedIR(
-            table=unpivot_table,
-            columns=[
-                *[unpivot_table[col_id] for col_id in index_col_ids],
-                *value_columns,
-                *passthrough_values,
-            ],
-            hidden_ordering_columns=hidden_ordering_columns,
-            ordering=new_ordering,
-        )
-
     def _reproject_to_table(self) -> OrderedIR:
         table = self._to_ibis_expr(
             ordering_mode="unordered",
             expose_hidden_cols=True,
         )
         columns = [table[column_name] for column_name in self._column_names]
         ordering_col_ids = list(
```

### Comparing `bigframes-1.2.0/bigframes/core/compile/compiler.py` & `bigframes-1.3.0/bigframes/core/compile/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,26 +176,14 @@
 
 @_compile_node.register
 def compile_reproject(node: nodes.ReprojectOpNode, ordered: bool = True):
     return compile_node(node.child, ordered)._reproject_to_table()
 
 
 @_compile_node.register
-def compile_unpivot(node: nodes.UnpivotNode, ordered: bool = True):
-    return compile_node(node.child, ordered).unpivot(
-        node.row_labels,
-        node.unpivot_columns,
-        passthrough_columns=node.passthrough_columns,
-        index_col_ids=node.index_col_ids,
-        dtype=node.dtype,
-        how=node.how,
-    )
-
-
-@_compile_node.register
 def compiler_explode(node: nodes.ExplodeNode, ordered: bool = True):
     return compile_node(node.child, ordered).explode(node.column_ids)
 
 
 @_compile_node.register
 def compiler_random_sample(node: nodes.RandomSampleNode, ordered: bool = True):
     return compile_node(node.child, ordered)._uniform_sampling(node.fraction)
```

### Comparing `bigframes-1.2.0/bigframes/core/compile/concat.py` & `bigframes-1.3.0/bigframes/core/compile/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/compile/scalar_op_compiler.py` & `bigframes-1.3.0/bigframes/core/compile/scalar_op_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,33 @@
                 return impl(args[0], args[1], args[2])
 
             self._register(key, normalized_impl)
             return impl
 
         return decorator
 
+    def register_nary_op(self, op_ref: typing.Union[ops.NaryOp, type[ops.NaryOp]]):
+        """
+        Decorator to register a nary op implementation.
+
+        Args:
+            op_ref (NaryOp or NaryOp type):
+                Class or instance of operator that is implemented by the decorated function.
+        """
+        key = typing.cast(str, op_ref.name)
+
+        def decorator(impl: typing.Callable[..., ibis_types.Value]):
+            def normalized_impl(args: typing.Sequence[ibis_types.Value], op: ops.RowOp):
+                return impl(*args)
+
+            self._register(key, normalized_impl)
+            return impl
+
+        return decorator
+
     def _register(
         self,
         op_name: str,
         impl: typing.Callable[
             [typing.Sequence[ibis_types.Value], ops.RowOp], ibis_types.Value
         ],
     ):
@@ -1342,14 +1361,33 @@
             .when(lower.isnull() | (original < lower), lower)
             .when(upper.isnull() | (original > upper), upper)
             .else_(original)
             .end()
         )
 
 
+@scalar_op_compiler.register_nary_op(ops.case_when_op)
+def switch_op(*cases_and_outputs: ibis_types.Value) -> ibis_types.Value:
+    # ibis can handle most type coercions, but we need to force bool -> int
+    # TODO: dispatch coercion depending on bigframes dtype schema
+    result_values = cases_and_outputs[1::2]
+    do_upcast_bool = any(t.type().is_numeric() for t in result_values)
+    if do_upcast_bool:
+        # Just need to upcast to int, ibis can handle further coercion
+        result_values = tuple(
+            val.cast(ibis_dtypes.int64) if val.type().is_boolean() else val
+            for val in result_values
+        )
+
+    case_val = ibis.case()
+    for predicate, output in zip(cases_and_outputs[::2], result_values):
+        case_val = case_val.when(predicate, output)
+    return case_val.end()
+
+
 # Helpers
 def is_null(value) -> bool:
     # float NaN/inf should be treated as distinct from 'true' null values
     return typing.cast(bool, pd.isna(value)) and not isinstance(value, float)
 
 
 def _ibis_num(number: float):
```

### Comparing `bigframes-1.2.0/bigframes/core/compile/single_column.py` & `bigframes-1.3.0/bigframes/core/compile/single_column.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/convert.py` & `bigframes-1.3.0/bigframes/core/convert.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/eval.py` & `bigframes-1.3.0/bigframes/core/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/expression.py` & `bigframes-1.3.0/bigframes/core/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,17 +186,14 @@
 @dataclasses.dataclass(frozen=True)
 class OpExpression(Expression):
     """An expression representing a scalar operation applied to 1 or more argument sub-expressions."""
 
     op: bigframes.operations.RowOp
     inputs: typing.Tuple[Expression, ...]
 
-    def __post_init__(self):
-        assert self.op.arguments == len(self.inputs)
-
     @property
     def unbound_variables(self) -> typing.Tuple[str, ...]:
         return tuple(
             itertools.chain.from_iterable(
                 map(lambda x: x.unbound_variables, self.inputs)
             )
         )
```

### Comparing `bigframes-1.2.0/bigframes/core/global_session.py` & `bigframes-1.3.0/bigframes/core/global_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/groupby/__init__.py` & `bigframes-1.3.0/bigframes/core/groupby/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing
+from typing import Sequence, Union
 
 import bigframes_vendored.pandas.core.groupby as vendored_pandas_groupby
 import pandas as pd
 
 import bigframes.constants as constants
 from bigframes.core import log_adapter
 import bigframes.core as core
@@ -108,25 +109,45 @@
         return self._aggregate_all(agg_ops.sum_op, numeric_only=True)
 
     def mean(self, numeric_only: bool = False, *args) -> df.DataFrame:
         if not numeric_only:
             self._raise_on_non_numeric("mean")
         return self._aggregate_all(agg_ops.mean_op, numeric_only=True)
 
-    def median(
-        self, numeric_only: bool = False, *, exact: bool = False
-    ) -> df.DataFrame:
-        if exact:
-            raise NotImplementedError(
-                f"Only approximate median is supported. {constants.FEEDBACK_LINK}"
-            )
+    def median(self, numeric_only: bool = False, *, exact: bool = True) -> df.DataFrame:
         if not numeric_only:
             self._raise_on_non_numeric("median")
+        if exact:
+            return self.quantile(0.5)
         return self._aggregate_all(agg_ops.median_op, numeric_only=True)
 
+    def quantile(
+        self, q: Union[float, Sequence[float]] = 0.5, *, numeric_only: bool = False
+    ) -> df.DataFrame:
+        if not numeric_only:
+            self._raise_on_non_numeric("quantile")
+        q_cols = tuple(
+            col
+            for col in self._selected_cols
+            if self._column_type(col) in dtypes.NUMERIC_BIGFRAMES_TYPES_PERMISSIVE
+        )
+        multi_q = utils.is_list_like(q)
+        result = block_ops.quantile(
+            self._block,
+            q_cols,
+            qs=tuple(q) if multi_q else (q,),  # type: ignore
+            grouping_column_ids=self._by_col_ids,
+            dropna=self._dropna,
+        )
+        result_df = df.DataFrame(result)
+        if multi_q:
+            return result_df.stack()
+        else:
+            return result_df.droplevel(-1, 1)
+
     def min(self, numeric_only: bool = False, *args) -> df.DataFrame:
         return self._aggregate_all(agg_ops.min_op, numeric_only=numeric_only)
 
     def max(self, numeric_only: bool = False, *args) -> df.DataFrame:
         return self._aggregate_all(agg_ops.max_op, numeric_only=numeric_only)
 
     def std(
@@ -462,16 +483,40 @@
 
     def sum(self, *args) -> series.Series:
         return self._aggregate(agg_ops.sum_op)
 
     def mean(self, *args) -> series.Series:
         return self._aggregate(agg_ops.mean_op)
 
-    def median(self, *args, **kwargs) -> series.Series:
-        return self._aggregate(agg_ops.mean_op)
+    def median(
+        self,
+        *args,
+        exact: bool = True,
+        **kwargs,
+    ) -> series.Series:
+        if exact:
+            return self.quantile(0.5)
+        else:
+            return self._aggregate(agg_ops.median_op)
+
+    def quantile(
+        self, q: Union[float, Sequence[float]] = 0.5, *, numeric_only: bool = False
+    ) -> series.Series:
+        multi_q = utils.is_list_like(q)
+        result = block_ops.quantile(
+            self._block,
+            (self._value_column,),
+            qs=tuple(q) if multi_q else (q,),  # type: ignore
+            grouping_column_ids=self._by_col_ids,
+            dropna=self._dropna,
+        )
+        if multi_q:
+            return series.Series(result.stack())
+        else:
+            return series.Series(result.stack()).droplevel(-1)
 
     def std(self, *args, **kwargs) -> series.Series:
         return self._aggregate(agg_ops.std_op)
 
     def var(self, *args, **kwargs) -> series.Series:
         return self._aggregate(agg_ops.var_op)
```

### Comparing `bigframes-1.2.0/bigframes/core/guid.py` & `bigframes-1.3.0/bigframes/core/guid.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/indexers.py` & `bigframes-1.3.0/bigframes/core/indexers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/indexes/__init__.py` & `bigframes-1.3.0/bigframes/core/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/indexes/base.py` & `bigframes-1.3.0/bigframes/core/indexes/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/indexes/multi.py` & `bigframes-1.3.0/bigframes/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/join_def.py` & `bigframes-1.3.0/bigframes/core/join_def.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 from typing import Literal, Mapping, NamedTuple, Tuple
 
 
 class JoinSide(enum.Enum):
     LEFT = 0
     RIGHT = 1
 
+    def inverse(self) -> JoinSide:
+        if self == JoinSide.LEFT:
+            return JoinSide.RIGHT
+        return JoinSide.LEFT
+
 
 JoinType = Literal["inner", "outer", "left", "right", "cross"]
 
 
 class JoinCondition(NamedTuple):
     left_id: str
     right_id: str
```

### Comparing `bigframes-1.2.0/bigframes/core/joins/__init__.py` & `bigframes-1.3.0/bigframes/core/joins/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/joins/merge.py` & `bigframes-1.3.0/bigframes/core/joins/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/local_data.py` & `bigframes-1.3.0/bigframes/core/local_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/log_adapter.py` & `bigframes-1.3.0/bigframes/core/log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/nodes.py` & `bigframes-1.3.0/bigframes/core/nodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 import abc
 from dataclasses import dataclass, field, fields, replace
 import functools
 import itertools
 import typing
 from typing import Callable, Tuple
 
-import pandas
-
 import bigframes.core.expression as ex
 import bigframes.core.guid
 from bigframes.core.join_def import JoinColumnMapping, JoinDefinition, JoinSide
 from bigframes.core.ordering import OrderingExpression
 import bigframes.core.schema as schemata
 import bigframes.core.window_spec as window
 import bigframes.dtypes
@@ -576,96 +574,14 @@
     @property
     def relation_ops_created(self) -> int:
         # This op is not a real transformation, just a hint to the sql generator
         return 0
 
 
 @dataclass(frozen=True)
-class UnpivotNode(UnaryNode):
-    # TODO: Refactor unpivot
-    row_labels: typing.Tuple[typing.Hashable, ...]
-    unpivot_columns: typing.Tuple[
-        typing.Tuple[str, typing.Tuple[typing.Optional[str], ...]], ...
-    ]
-    passthrough_columns: typing.Tuple[str, ...] = ()
-    index_col_ids: typing.Tuple[str, ...] = ("index",)
-    dtype: typing.Union[
-        bigframes.dtypes.Dtype, typing.Tuple[bigframes.dtypes.Dtype, ...]
-    ] = (pandas.Float64Dtype(),)
-    how: typing.Literal["left", "right"] = "left"
-
-    def __hash__(self):
-        return self._node_hash
-
-    @property
-    def row_preserving(self) -> bool:
-        return False
-
-    @property
-    def non_local(self) -> bool:
-        return True
-
-    @property
-    def joins(self) -> bool:
-        return True
-
-    @functools.cached_property
-    def schema(self) -> schemata.ArraySchema:
-        def infer_dtype(
-            values: typing.Iterable[typing.Hashable],
-        ) -> bigframes.dtypes.Dtype:
-            item_types = map(lambda x: bigframes.dtypes.infer_literal_type(x), values)
-            etype = functools.reduce(
-                lambda t1, t2: bigframes.dtypes.lcd_type(t1, t2)
-                if (t1 and t2)
-                else None,
-                item_types,
-            )
-            return bigframes.dtypes.dtype_for_etype(etype)
-
-        label_tuples = [
-            label if isinstance(label, tuple) else (label,) for label in self.row_labels
-        ]
-        idx_dtypes = [
-            infer_dtype(map(lambda x: typing.cast(tuple, x)[i], label_tuples))
-            for i in range(len(self.index_col_ids))
-        ]
-
-        index_items = [
-            schemata.SchemaItem(id, dtype)
-            for id, dtype in zip(self.index_col_ids, idx_dtypes)
-        ]
-        value_dtypes = (
-            self.dtype
-            if isinstance(self.dtype, tuple)
-            else (self.dtype,) * len(self.unpivot_columns)
-        )
-        value_items = [
-            schemata.SchemaItem(col[0], dtype)
-            for col, dtype in zip(self.unpivot_columns, value_dtypes)
-        ]
-        passthrough_items = [
-            schemata.SchemaItem(id, self.child.schema.get_type(id))
-            for id in self.passthrough_columns
-        ]
-        return schemata.ArraySchema((*index_items, *value_items, *passthrough_items))
-
-    @property
-    def variables_introduced(self) -> int:
-        return (
-            len(self.schema.items) - len(self.passthrough_columns) + OVERHEAD_VARIABLES
-        )
-
-    @property
-    def relation_ops_created(self) -> int:
-        # Unpivot is essentially a cross join and a projection.
-        return 2
-
-
-@dataclass(frozen=True)
 class RandomSampleNode(UnaryNode):
     fraction: float
 
     @property
     def deterministic(self) -> bool:
         return False
```

### Comparing `bigframes-1.2.0/bigframes/core/ordering.py` & `bigframes-1.3.0/bigframes/core/ordering.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/reshape/__init__.py` & `bigframes-1.3.0/bigframes/core/reshape/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/rewrite.py` & `bigframes-1.3.0/bigframes/core/rewrite.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/scalar.py` & `bigframes-1.3.0/bigframes/core/scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/schema.py` & `bigframes-1.3.0/bigframes/core/schema.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/tools/__init__.py` & `bigframes-1.3.0/bigframes/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/tools/datetimes.py` & `bigframes-1.3.0/bigframes/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/tree_properties.py` & `bigframes-1.3.0/bigframes/core/tree_properties.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/utils.py` & `bigframes-1.3.0/bigframes/core/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/window/__init__.py` & `bigframes-1.3.0/bigframes/core/window/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/core/window_spec.py` & `bigframes-1.3.0/bigframes/core/window_spec.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/dataframe.py` & `bigframes-1.3.0/bigframes/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1957,29 +1957,25 @@
         axis: typing.Union[str, int] = 0,
         bool_only: bool = False,
     ) -> bigframes.series.Series:
         if not bool_only:
             frame = self._raise_on_non_boolean("any")
         else:
             frame = self._drop_non_bool()
-        block = frame._block.aggregate_all_and_stack(
-            agg_ops.any_op, dtype=pandas.BooleanDtype(), axis=axis
-        )
+        block = frame._block.aggregate_all_and_stack(agg_ops.any_op, axis=axis)
         return bigframes.series.Series(block.select_column("values"))
 
     def all(
         self, axis: typing.Union[str, int] = 0, *, bool_only: bool = False
     ) -> bigframes.series.Series:
         if not bool_only:
             frame = self._raise_on_non_boolean("all")
         else:
             frame = self._drop_non_bool()
-        block = frame._block.aggregate_all_and_stack(
-            agg_ops.all_op, dtype=pandas.BooleanDtype(), axis=axis
-        )
+        block = frame._block.aggregate_all_and_stack(agg_ops.all_op, axis=axis)
         return bigframes.series.Series(block.select_column("values"))
 
     def sum(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("sum")
@@ -1995,26 +1991,50 @@
             frame = self._raise_on_non_numeric("mean")
         else:
             frame = self._drop_non_numeric()
         block = frame._block.aggregate_all_and_stack(agg_ops.mean_op, axis=axis)
         return bigframes.series.Series(block.select_column("values"))
 
     def median(
-        self, *, numeric_only: bool = False, exact: bool = False
+        self, *, numeric_only: bool = False, exact: bool = True
     ) -> bigframes.series.Series:
+        if not numeric_only:
+            frame = self._raise_on_non_numeric("median")
+        else:
+            frame = self._drop_non_numeric()
         if exact:
-            raise NotImplementedError(
-                f"Only approximate median is supported. {constants.FEEDBACK_LINK}"
-            )
+            result = frame.quantile()
+            result.name = None
+            return result
+        else:
+            block = frame._block.aggregate_all_and_stack(agg_ops.median_op)
+            return bigframes.series.Series(block.select_column("values"))
+
+    def quantile(
+        self, q: Union[float, Sequence[float]] = 0.5, *, numeric_only: bool = False
+    ):
         if not numeric_only:
             frame = self._raise_on_non_numeric("median")
         else:
             frame = self._drop_non_numeric()
-        block = frame._block.aggregate_all_and_stack(agg_ops.median_op)
-        return bigframes.series.Series(block.select_column("values"))
+        multi_q = utils.is_list_like(q)
+        result = block_ops.quantile(
+            frame._block, frame._block.value_columns, qs=tuple(q) if multi_q else (q,)  # type: ignore
+        )
+        if multi_q:
+            return DataFrame(result.stack()).droplevel(0)
+        else:
+            result_df = (
+                DataFrame(result)
+                .stack(list(range(0, frame.columns.nlevels)))
+                .droplevel(0)
+            )
+            result_series = bigframes.series.Series(result_df._block)
+            result_series.name = q
+            return result_series
 
     def std(
         self, axis: typing.Union[str, int] = 0, *, numeric_only: bool = False
     ) -> bigframes.series.Series:
         if not numeric_only:
             frame = self._raise_on_non_numeric("std")
         else:
```

### Comparing `bigframes-1.2.0/bigframes/dtypes.py` & `bigframes-1.3.0/bigframes/dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/features.py` & `bigframes-1.3.0/bigframes/features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/formatting_helpers.py` & `bigframes-1.3.0/bigframes/formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/functions/__init__.py` & `bigframes-1.3.0/bigframes/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/functions/remote_function.py` & `bigframes-1.3.0/bigframes/functions/remote_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,21 @@
         self._bq_connection_id = bq_connection_id
         self._bq_connection_manager = bq_connection_manager
         self._cloud_function_service_account = cloud_function_service_account
         self._cloud_function_kms_key_name = cloud_function_kms_key_name
         self._cloud_function_docker_repository = cloud_function_docker_repository
 
     def create_bq_remote_function(
-        self, input_args, input_types, output_type, endpoint, bq_function_name
+        self,
+        input_args,
+        input_types,
+        output_type,
+        endpoint,
+        bq_function_name,
+        max_batching_rows,
     ):
         """Create a BigQuery remote function given the artifacts of a user defined
         function and the http endpoint of a corresponding cloud function."""
         if self._bq_connection_manager:
             self._bq_connection_manager.create_bq_connection(
                 self._gcp_project_id,
                 self._bq_location,
@@ -165,22 +171,33 @@
         )
 
         # We are expecting the input type annotations to be 1:1 with the input args
         for idx, name in enumerate(input_args):
             bq_function_args.append(
                 f"{name} {third_party_ibis_bqtypes.BigQueryType.from_ibis(input_types[idx])}"
             )
+
+        remote_function_options = {
+            "endpoint": endpoint,
+            "max_batching_rows": max_batching_rows,
+        }
+
+        remote_function_options_str = ", ".join(
+            [
+                f'{key}="{val}"' if isinstance(val, str) else f"{key}={val}"
+                for key, val in remote_function_options.items()
+                if val is not None
+            ]
+        )
+
         create_function_ddl = f"""
             CREATE OR REPLACE FUNCTION `{self._gcp_project_id}.{self._bq_dataset}`.{bq_function_name}({','.join(bq_function_args)})
             RETURNS {bq_function_return_type}
             REMOTE WITH CONNECTION `{self._gcp_project_id}.{self._bq_location}.{self._bq_connection_id}`
-            OPTIONS (
-              endpoint = "{endpoint}",
-              max_batching_rows = 1000
-            )"""
+            OPTIONS ({remote_function_options_str})"""
 
         logger.info(f"Creating BQ remote function: {create_function_ddl}")
 
         # Make sure the dataset exists. I.e. if it doesn't exist, go ahead and
         # create it
         dataset = bigquery.Dataset(
             bigquery.DatasetReference.from_string(
@@ -434,14 +451,15 @@
         self,
         def_,
         input_types,
         output_type,
         reuse,
         name,
         package_requirements,
+        max_batching_rows,
     ):
         """Provision a BigQuery remote function."""
         # If reuse of any existing function with the same name (indicated by the
         # same hash of its source code) is not intended, then attach a unique
         # suffix to the intended function name to make it unique.
         uniq_suffix = None
         if not reuse:
@@ -481,15 +499,20 @@
         ):
             input_args = inspect.getargs(def_.__code__).args
             if len(input_args) != len(input_types):
                 raise ValueError(
                     "Exactly one type should be provided for every input arg."
                 )
             self.create_bq_remote_function(
-                input_args, input_types, output_type, cf_endpoint, remote_function_name
+                input_args,
+                input_types,
+                output_type,
+                cf_endpoint,
+                remote_function_name,
+                max_batching_rows,
             )
         else:
             logger.info(f"Remote function {remote_function_name} already exists.")
 
         return remote_function_name, cloud_function_name
 
     def get_remote_function_specs(self, remote_function_name):
@@ -603,14 +626,15 @@
     bigquery_connection: Optional[str] = None,
     reuse: bool = True,
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
+    max_batching_rows: Optional[int] = 1000,
 ):
     """Decorator to turn a user defined function into a BigQuery remote function.
 
     .. deprecated:: 0.0.1
        This is an internal method. Please use :func:`bigframes.pandas.remote_function` instead.
 
     .. note::
@@ -719,14 +743,23 @@
         cloud_function_docker_repository (str, Optional):
             Docker repository created with the same encryption key as
             `cloud_function_kms_key_name` to store encrypted artifacts
             created to support the cloud function. This is of the format
             projects/PROJECT_ID/locations/LOCATION/repositories/REPOSITORY_NAME.
             For more details see
             https://cloud.google.com/functions/docs/securing/cmek#before_you_begin.
+        max_batching_rows (int, Optional):
+            The maximum number of rows to be batched for processing in the
+            BQ remote function. Default value is 1000. A lower number can be
+            passed to avoid timeouts in case the user code is too complex to
+            process large number of rows fast enough. A higher number can be
+            used to increase throughput in case the user code is fast enough.
+            `None` can be passed to let BQ remote functions service apply
+            default batching. See for more details
+            https://cloud.google.com/bigquery/docs/remote-functions#limiting_number_of_rows_in_a_batch_request.
     """
     import bigframes.pandas as bpd
 
     session = session or bpd.get_global_session()
 
     # A BigQuery client is required to perform BQ operations
     if not bigquery_client:
@@ -842,14 +875,15 @@
         rf_name, cf_name = remote_function_client.provision_bq_remote_function(
             f,
             ibis_signature.input_types,
             ibis_signature.output_type,
             reuse,
             name,
             packages,
+            max_batching_rows,
         )
 
         # TODO: Move ibis logic to compiler step
         node = ibis.udf.scalar.builtin(
             f,
             name=rf_name,
             schema=f"{dataset_ref.project}.{dataset_ref.dataset_id}",
```

### Comparing `bigframes-1.2.0/bigframes/ml/__init__.py` & `bigframes-1.3.0/bigframes/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/base.py` & `bigframes-1.3.0/bigframes/ml/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/cluster.py` & `bigframes-1.3.0/bigframes/ml/cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/compose.py` & `bigframes-1.3.0/bigframes/ml/compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/core.py` & `bigframes-1.3.0/bigframes/ml/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,14 +317,54 @@
             model_ref=model_ref,
             transforms=transforms,
             options=options,
         )
 
         return self._create_model_with_sql(session=session, sql=sql)
 
+    def create_llm_remote_model(
+        self,
+        X_train: bpd.DataFrame,
+        y_train: bpd.DataFrame,
+        connection_name: str,
+        options: Mapping[str, Union[str, int, float, Iterable[str]]] = {},
+    ) -> BqmlModel:
+        """Create a session-temporary BQML model with the CREATE OR REPLACE MODEL statement
+
+        Args:
+            X_train: features columns for training
+            y_train: labels columns for training
+            options: a dict of options to configure the model. Generates a BQML OPTIONS
+                clause
+            connection_name:
+                a BQ connection to talk with Vertex AI, of the format <PROJECT_NUMBER>.<REGION>.<CONNECTION_NAME>. https://cloud.google.com/bigquery/docs/create-cloud-resource-connection
+
+        Returns: a BqmlModel, wrapping a trained model in BigQuery
+        """
+        options = dict(options)
+        # Cache dataframes to make sure base table is not a snapshot
+        # cached dataframe creates a full copy, never uses snapshot
+        input_data = X_train._cached(force=True).join(
+            y_train._cached(force=True), how="outer"
+        )
+        options.update({"INPUT_LABEL_COLS": y_train.columns.tolist()})
+
+        session = X_train._session
+
+        model_ref = self._create_model_ref(session._anonymous_dataset)
+
+        sql = self._model_creation_sql_generator.create_llm_remote_model(
+            source_df=input_data,
+            model_ref=model_ref,
+            options=options,
+            connection_name=connection_name,
+        )
+
+        return self._create_model_with_sql(session=session, sql=sql)
+
     def create_time_series_model(
         self,
         X_train: bpd.DataFrame,
         y_train: bpd.DataFrame,
         transforms: Optional[Iterable[str]] = None,
         options: Mapping[str, Union[str, int, float, Iterable[str]]] = {},
     ) -> BqmlModel:
```

### Comparing `bigframes-1.2.0/bigframes/ml/decomposition.py` & `bigframes-1.3.0/bigframes/ml/decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/ensemble.py` & `bigframes-1.3.0/bigframes/ml/ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/forecasting.py` & `bigframes-1.3.0/bigframes/ml/forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/globals.py` & `bigframes-1.3.0/bigframes/ml/globals.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/imported.py` & `bigframes-1.3.0/bigframes/ml/imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/linear_model.py` & `bigframes-1.3.0/bigframes/ml/linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/llm.py` & `bigframes-1.3.0/bigframes/ml/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
 import bigframes
 from bigframes import clients, constants
 from bigframes.core import blocks, log_adapter
 from bigframes.ml import base, core, globals, utils
 import bigframes.pandas as bpd
 
+_BQML_PARAMS_MAPPING = {
+    "max_iterations": "maxIterations",
+}
+
 _TEXT_GENERATOR_BISON_ENDPOINT = "text-bison"
 _TEXT_GENERATOR_BISON_32K_ENDPOINT = "text-bison-32k"
 _TEXT_GENERATOR_ENDPOINTS = (
     _TEXT_GENERATOR_BISON_ENDPOINT,
     _TEXT_GENERATOR_BISON_32K_ENDPOINT,
 )
 
@@ -58,25 +62,29 @@
             Default to "text-bison".
         session (bigframes.Session or None):
             BQ session to create the model. If None, use the global default session.
         connection_name (str or None):
             Connection to connect with remote service. str of the format <PROJECT_NUMBER/PROJECT_ID>.<LOCATION>.<CONNECTION_ID>.
             if None, use default connection in session context. BigQuery DataFrame will try to create the connection and attach
             permission if the connection isn't fully setup.
+        max_iterations (Optional[int], Default to 300):
+            The number of steps to run when performing supervised tuning.
     """
 
     def __init__(
         self,
         *,
         model_name: Literal["text-bison", "text-bison-32k"] = "text-bison",
         session: Optional[bigframes.Session] = None,
         connection_name: Optional[str] = None,
+        max_iterations: int = 300,
     ):
         self.model_name = model_name
         self.session = session or bpd.get_global_session()
+        self.max_iterations = max_iterations
         self._bq_connection_manager = self.session.bqconnectionmanager
 
         connection_name = connection_name or self.session._bq_connection
         self.connection_name = clients.resolve_full_bq_connection_name(
             connection_name,
             default_project=self.session._project,
             default_location=self.session._location,
@@ -128,20 +136,81 @@
         assert "connection" in model._properties["remoteModelInfo"]
 
         # Parse the remote model endpoint
         bqml_endpoint = model._properties["remoteModelInfo"]["endpoint"]
         model_connection = model._properties["remoteModelInfo"]["connection"]
         model_endpoint = bqml_endpoint.split("/")[-1]
 
+        # Get the optional params
+        kwargs: dict = {}
+        last_fitting = model.training_runs[-1]["trainingOptions"]
+
+        dummy_text_generator = cls()
+        for bf_param, _ in dummy_text_generator.__dict__.items():
+            bqml_param = _BQML_PARAMS_MAPPING.get(bf_param)
+            if bqml_param in last_fitting:
+                # Convert types
+                if bf_param in ["max_iterations"]:
+                    kwargs[bf_param] = int(last_fitting[bqml_param])
+
         text_generator_model = cls(
-            session=session, model_name=model_endpoint, connection_name=model_connection
+            **kwargs,
+            session=session,
+            model_name=model_endpoint,
+            connection_name=model_connection,
         )
         text_generator_model._bqml_model = core.BqmlModel(session, model)
         return text_generator_model
 
+    @property
+    def _bqml_options(self) -> dict:
+        """The model options as they will be set for BQML"""
+        options = {
+            "max_iterations": self.max_iterations,
+            "data_split_method": "NO_SPLIT",
+        }
+        return options
+
+    def fit(
+        self,
+        X: Union[bpd.DataFrame, bpd.Series],
+        y: Union[bpd.DataFrame, bpd.Series],
+    ) -> PaLM2TextGenerator:
+        """Fine tune PaLM2TextGenerator model.
+
+        .. note::
+
+            This product or feature is subject to the "Pre-GA Offerings Terms" in the General Service Terms section of the
+            Service Specific Terms(https://cloud.google.com/terms/service-terms#1). Pre-GA products and features are available "as is"
+            and might have limited support. For more information, see the launch stage descriptions
+            (https://cloud.google.com/products#product-launch-stages).
+
+        Args:
+            X (bigframes.dataframe.DataFrame or bigframes.series.Series):
+                DataFrame of shape (n_samples, n_features). Training data.
+            y (bigframes.dataframe.DataFrame or bigframes.series.Series:
+                Training labels.
+
+        Returns:
+            PaLM2TextGenerator: Fitted Estimator.
+        """
+        X, y = utils.convert_to_dataframe(X, y)
+
+        options = self._bqml_options
+        options["endpoint"] = self.model_name + "@001"
+        options["prompt_col"] = X.columns.tolist()[0]
+
+        self._bqml_model = self._bqml_model_factory.create_llm_remote_model(
+            X,
+            y,
+            options=options,
+            connection_name=self.connection_name,
+        )
+        return self
+
     def predict(
         self,
         X: Union[bpd.DataFrame, bpd.Series],
         *,
         temperature: float = 0.0,
         max_output_tokens: int = 128,
         top_k: int = 40,
```

### Comparing `bigframes-1.2.0/bigframes/ml/loader.py` & `bigframes-1.3.0/bigframes/ml/loader.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/metrics/__init__.py` & `bigframes-1.3.0/bigframes/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/metrics/_metrics.py` & `bigframes-1.3.0/bigframes/ml/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/metrics/pairwise.py` & `bigframes-1.3.0/bigframes/ml/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/model_selection.py` & `bigframes-1.3.0/bigframes/ml/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     random_state: Union[int, None] = None,
 ) -> List[Union[bpd.DataFrame, bpd.Series]]:
     """Splits dataframes or series into random train and test subsets.
 
     Args:
         *arrays (bigframes.dataframe.DataFrame or bigframes.series.Series):
             A sequence of BigQuery DataFrames or Series that can be joined on
-            their indexes
+            their indexes.
         test_size (default None):
             The proportion of the dataset to include in the test split. If
             None, this will default to the complement of train_size. If both
             are none, it will be set to 0.25.
         train_size (default None):
             The proportion of the dataset to include in the train split. If
             None, this will default to the complement of test_size.
```

### Comparing `bigframes-1.2.0/bigframes/ml/pipeline.py` & `bigframes-1.3.0/bigframes/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/preprocessing.py` & `bigframes-1.3.0/bigframes/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/remote.py` & `bigframes-1.3.0/bigframes/ml/remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/ml/sql.py` & `bigframes-1.3.0/bigframes/ml/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,31 @@
         if transforms:
             parts.append(self.transform(*transforms))
         if options:
             parts.append(self.options(**options))
         parts.append(f"AS {source_sql}")
         return "\n".join(parts)
 
+    def create_llm_remote_model(
+        self,
+        source_df: bpd.DataFrame,
+        connection_name: str,
+        model_ref: google.cloud.bigquery.ModelReference,
+        options: Mapping[str, Union[str, int, float, Iterable[str]]] = {},
+    ) -> str:
+        """Encode the CREATE OR REPLACE MODEL statement for BQML"""
+        source_sql = source_df.sql
+
+        parts = [f"CREATE OR REPLACE MODEL {self._model_id_sql(model_ref)}"]
+        parts.append(self.connection(connection_name))
+        if options:
+            parts.append(self.options(**options))
+        parts.append(f"AS {source_sql}")
+        return "\n".join(parts)
+
     def create_remote_model(
         self,
         connection_name: str,
         model_ref: google.cloud.bigquery.ModelReference,
         input: Mapping[str, str] = {},
         output: Mapping[str, str] = {},
         options: Mapping[str, Union[str, int, float, Iterable[str]]] = {},
```

### Comparing `bigframes-1.2.0/bigframes/ml/utils.py` & `bigframes-1.3.0/bigframes/ml/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/__init__.py` & `bigframes-1.3.0/bigframes/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import dataclasses
+import functools
 import typing
+from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 
 import bigframes.dtypes as dtypes
 import bigframes.operations.type as op_typing
@@ -30,71 +32,62 @@
 
 
 class RowOp(typing.Protocol):
     @property
     def name(self) -> str:
         ...
 
-    @property
-    def arguments(self) -> int:
-        """The number of column argument the operation takes"""
-        ...
-
     def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
         ...
 
     @property
     def order_preserving(self) -> bool:
         """Whether the row operation preserves total ordering. Can be pruned from ordering expressions."""
         ...
 
 
-# These classes can be used to create simple ops that don't take local parameters
-# All is needed is a unique name, and to register an implementation in ibis_mappings.py
 @dataclasses.dataclass(frozen=True)
-class UnaryOp:
+class NaryOp:
     @property
     def name(self) -> str:
         raise NotImplementedError("RowOp abstract base class has no implementation")
 
+    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
+        raise NotImplementedError("Abstract operation has no output type")
+
+    @property
+    def order_preserving(self) -> bool:
+        """Whether the row operation preserves total ordering. Can be pruned from ordering expressions."""
+        return False
+
+
+# These classes can be used to create simple ops that don't take local parameters
+# All is needed is a unique name, and to register an implementation in ibis_mappings.py
+@dataclasses.dataclass(frozen=True)
+class UnaryOp(NaryOp):
     @property
     def arguments(self) -> int:
         return 1
 
-    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
-        raise NotImplementedError("Abstract operation has no output type")
-
     def as_expr(
         self, input_id: typing.Union[str, bigframes.core.expression.Expression] = "arg"
     ) -> bigframes.core.expression.Expression:
         import bigframes.core.expression
 
         return bigframes.core.expression.OpExpression(
             self, (_convert_expr_input(input_id),)
         )
 
-    @property
-    def order_preserving(self) -> bool:
-        """Whether the row operation preserves total ordering. Can be pruned from ordering expressions."""
-        return False
-
 
 @dataclasses.dataclass(frozen=True)
-class BinaryOp:
-    @property
-    def name(self) -> str:
-        raise NotImplementedError("RowOp abstract base class has no implementation")
-
+class BinaryOp(NaryOp):
     @property
     def arguments(self) -> int:
         return 2
 
-    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
-        raise NotImplementedError("Abstract operation has no output type")
-
     def as_expr(
         self,
         left_input: typing.Union[str, bigframes.core.expression.Expression] = "arg1",
         right_input: typing.Union[str, bigframes.core.expression.Expression] = "arg2",
     ) -> bigframes.core.expression.Expression:
         import bigframes.core.expression
 
@@ -102,33 +95,21 @@
             self,
             (
                 _convert_expr_input(left_input),
                 _convert_expr_input(right_input),
             ),
         )
 
-    @property
-    def order_preserving(self) -> bool:
-        """Whether the row operation preserves total ordering. Can be pruned from ordering expressions."""
-        return False
-
 
 @dataclasses.dataclass(frozen=True)
-class TernaryOp:
-    @property
-    def name(self) -> str:
-        raise NotImplementedError("RowOp abstract base class has no implementation")
-
+class TernaryOp(NaryOp):
     @property
     def arguments(self) -> int:
         return 3
 
-    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
-        raise NotImplementedError("Abstract operation has no output type")
-
     def as_expr(
         self,
         input1: typing.Union[str, bigframes.core.expression.Expression] = "arg1",
         input2: typing.Union[str, bigframes.core.expression.Expression] = "arg2",
         input3: typing.Union[str, bigframes.core.expression.Expression] = "arg3",
     ) -> bigframes.core.expression.Expression:
         import bigframes.core.expression
@@ -138,19 +119,14 @@
             (
                 _convert_expr_input(input1),
                 _convert_expr_input(input2),
                 _convert_expr_input(input3),
             ),
         )
 
-    @property
-    def order_preserving(self) -> bool:
-        """Whether the row operation preserves total ordering. Can be pruned from ordering expressions."""
-        return False
-
 
 def _convert_expr_input(
     input: typing.Union[str, bigframes.core.expression.Expression]
 ) -> bigframes.core.expression.Expression:
     """Allows creating free variables with just a string"""
     import bigframes.core.expression
 
@@ -660,14 +636,54 @@
         return dtypes.coerce_to_common(
             input_types[0], dtypes.coerce_to_common(input_types[1], input_types[2])
         )
 
 
 clip_op = ClipOp()
 
+
+class CaseWhenOp(NaryOp):
+    name: typing.ClassVar[str] = "switch"
+
+    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
+        assert len(input_types) % 2 == 0
+        # predicate1, output1, predicate2, output2...
+        if not all(map(lambda x: x == dtypes.BOOL_DTYPE, input_types[::2])):
+            raise TypeError(f"Case inputs {input_types[::2]} must be boolean-valued")
+        output_expr_types = input_types[1::2]
+        return functools.reduce(
+            lambda t1, t2: dtypes.coerce_to_common(t1, t2),
+            output_expr_types,
+        )
+
+    def as_expr(
+        self,
+        *case_output_pairs: Tuple[
+            Union[str | bigframes.core.expression.Expression],
+            Union[str | bigframes.core.expression.Expression],
+        ],
+    ) -> bigframes.core.expression.Expression:
+        import bigframes.core.expression
+
+        # Keep this in sync with output_type and compilers
+        inputs: list[bigframes.core.expression.Expression] = []
+
+        for case, output in case_output_pairs:
+            inputs.append(_convert_expr_input(case))
+            inputs.append(_convert_expr_input(output))
+
+        return bigframes.core.expression.OpExpression(
+            self,
+            tuple(inputs),
+        )
+
+
+case_when_op = CaseWhenOp()
+
+
 # Just parameterless unary ops for now
 # TODO: Parameter mappings
 NUMPY_TO_OP: typing.Final = {
     np.sin: sin_op,
     np.cos: cos_op,
     np.tan: tan_op,
     np.arcsin: arcsin_op,
```

### Comparing `bigframes-1.2.0/bigframes/operations/_matplotlib/__init__.py` & `bigframes-1.3.0/bigframes/operations/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/_matplotlib/core.py` & `bigframes-1.3.0/bigframes/operations/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/_matplotlib/hist.py` & `bigframes-1.3.0/bigframes/operations/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/aggregations.py` & `bigframes-1.3.0/bigframes/operations/aggregations.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,26 @@
         if pd.api.types.is_bool_dtype(input_types[0]):
             return dtypes.INT_DTYPE
         else:
             return input_types[0]
 
 
 @dataclasses.dataclass(frozen=True)
+class QuantileOp(UnaryAggregateOp):
+    q: float
+
+    @property
+    def name(self):
+        return f"{int(self.q*100)}%"
+
+    def output_type(self, *input_types: dtypes.ExpressionType) -> dtypes.ExpressionType:
+        return signatures.UNARY_REAL_NUMERIC.output_type(input_types[0])
+
+
+@dataclasses.dataclass(frozen=True)
 class ApproxQuartilesOp(UnaryAggregateOp):
     quartile: int
 
     @property
     def name(self):
         return f"{self.quartile*25}%"
```

### Comparing `bigframes-1.2.0/bigframes/operations/base.py` & `bigframes-1.3.0/bigframes/operations/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/datetimes.py` & `bigframes-1.3.0/bigframes/operations/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/plotting.py` & `bigframes-1.3.0/bigframes/operations/plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/strings.py` & `bigframes-1.3.0/bigframes/operations/strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/operations/structs.py` & `bigframes-1.3.0/bigframes/operations/structs.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import bigframes_vendored.pandas.core.arrays.arrow.accessors as vendoracessors
+import pandas as pd
 
 from bigframes.core import log_adapter
 import bigframes.dataframe
+import bigframes.dtypes
 import bigframes.operations
 import bigframes.operations.base
 import bigframes.series
 
 
 @log_adapter.class_logger
 class StructAccessor(
@@ -41,7 +43,17 @@
     def explode(self) -> bigframes.dataframe.DataFrame:
         import bigframes.pandas
 
         pa_type = self._dtype.pyarrow_dtype
         return bigframes.pandas.concat(
             [self.field(i) for i in range(pa_type.num_fields)], axis="columns"
         )
+
+    def dtypes(self) -> pd.Series:
+        pa_type = self._dtype.pyarrow_dtype
+        return pd.Series(
+            data=[
+                bigframes.dtypes.arrow_dtype_to_bigframes_dtype(pa_type.field(i).type)
+                for i in range(pa_type.num_fields)
+            ],
+            index=[pa_type.field(i).name for i in range(pa_type.num_fields)],
+        )
```

### Comparing `bigframes-1.2.0/bigframes/operations/type.py` & `bigframes-1.3.0/bigframes/operations/type.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/pandas/__init__.py` & `bigframes-1.3.0/bigframes/pandas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,27 +639,29 @@
     bigquery_connection: Optional[str] = None,
     reuse: bool = True,
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
+    max_batching_rows: Optional[int] = 1000,
 ):
     return global_session.with_default_session(
         bigframes.session.Session.remote_function,
         input_types=input_types,
         output_type=output_type,
         dataset=dataset,
         bigquery_connection=bigquery_connection,
         reuse=reuse,
         name=name,
         packages=packages,
         cloud_function_service_account=cloud_function_service_account,
         cloud_function_kms_key_name=cloud_function_kms_key_name,
         cloud_function_docker_repository=cloud_function_docker_repository,
+        max_batching_rows=max_batching_rows,
     )
 
 
 remote_function.__doc__ = inspect.getdoc(bigframes.session.Session.remote_function)
 
 
 def read_gbq_function(function_name: str):
```

### Comparing `bigframes-1.2.0/bigframes/series.py` & `bigframes-1.3.0/bigframes/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import functools
 import inspect
 import itertools
 import numbers
 import os
 import textwrap
 import typing
-from typing import Any, Literal, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, cast, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import bigframes_vendored.pandas.core.series as vendored_pandas_series
 import google.cloud.bigquery as bigquery
 import numpy
 import pandas
 import pandas.core.dtypes.common
 import typing_extensions
@@ -962,20 +962,29 @@
         block = block.select_column(self._value_column).with_column_labels([self.name])
         mode_values_series = Series(block.select_column(self._value_column))
         return typing.cast(Series, mode_values_series)
 
     def mean(self) -> float:
         return typing.cast(float, self._apply_aggregation(agg_ops.mean_op))
 
-    def median(self, *, exact: bool = False) -> float:
+    def median(self, *, exact: bool = True) -> float:
         if exact:
-            raise NotImplementedError(
-                f"Only approximate median is supported. {constants.FEEDBACK_LINK}"
-            )
-        return typing.cast(float, self._apply_aggregation(agg_ops.median_op))
+            return typing.cast(float, self.quantile(0.5))
+        else:
+            return typing.cast(float, self._apply_aggregation(agg_ops.median_op))
+
+    def quantile(self, q: Union[float, Sequence[float]] = 0.5) -> Union[Series, float]:
+        qs = tuple(q) if utils.is_list_like(q) else (q,)
+        result = block_ops.quantile(self._block, (self._value_column,), qs=qs)
+        if utils.is_list_like(q):
+            result = result.stack()
+            result = result.drop_levels([result.index_columns[0]])
+            return Series(result)
+        else:
+            return cast(float, Series(result).to_pandas().squeeze())
 
     def sum(self) -> float:
         return typing.cast(float, self._apply_aggregation(agg_ops.sum_op))
 
     def prod(self) -> float:
         return typing.cast(float, self._apply_aggregation(agg_ops.product_op))
```

### Comparing `bigframes-1.2.0/bigframes/session/__init__.py` & `bigframes-1.3.0/bigframes/session/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1642,3440 +1642,3505 @@
 00006690: 7b73 656c 662e 5f6c 6f63 6174 696f 6e7d  {self._location}
 000066a0: 2062 7574 2064 6174 6173 6574 2027 7b74   but dataset '{t
 000066b0: 6162 6c65 2e70 726f 6a65 6374 7d2e 7b74  able.project}.{t
 000066c0: 6162 6c65 2e64 6174 6173 6574 5f69 647d  able.dataset_id}
 000066d0: 2720 6973 206c 6f63 6174 6564 2069 6e20  ' is located in 
 000066e0: 7b74 6162 6c65 2e6c 6f63 6174 696f 6e7d  {table.location}
 000066f0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00006700: 0a20 2020 2020 2020 2023 2054 4f44 4f28  .        # TODO(
-00006710: 622f 3330 3532 3634 3135 3329 3a20 5573  b/305264153): Us
-00006720: 6520 7075 626c 6963 2070 726f 7065 7274  e public propert
-00006730: 6965 7320 746f 2066 6574 6368 2070 7269  ies to fetch pri
-00006740: 6d61 7279 206b 6579 7320 6f6e 6365 0a20  mary keys once. 
-00006750: 2020 2020 2020 2023 2061 6464 6564 2074         # added t
-00006760: 6f20 676f 6f67 6c65 2d63 6c6f 7564 2d62  o google-cloud-b
-00006770: 6967 7175 6572 792e 0a20 2020 2020 2020  igquery..       
-00006780: 2070 7269 6d61 7279 5f6b 6579 7320 3d20   primary_keys = 
-00006790: 280a 2020 2020 2020 2020 2020 2020 7461  (.            ta
-000067a0: 626c 652e 5f70 726f 7065 7274 6965 732e  ble._properties.
-000067b0: 6765 7428 2274 6162 6c65 436f 6e73 7472  get("tableConstr
-000067c0: 6169 6e74 7322 2c20 7b7d 290a 2020 2020  aints", {}).    
-000067d0: 2020 2020 2020 2020 2e67 6574 2822 7072          .get("pr
-000067e0: 696d 6172 794b 6579 222c 207b 7d29 0a20  imaryKey", {}). 
-000067f0: 2020 2020 2020 2020 2020 202e 6765 7428             .get(
-00006800: 2263 6f6c 756d 6e73 2229 0a20 2020 2020  "columns").     
-00006810: 2020 2029 0a0a 2020 2020 2020 2020 6a6f     )..        jo
-00006820: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
-00006830: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
-00006840: 6967 2829 0a20 2020 2020 2020 206a 6f62  ig().        job
-00006850: 5f63 6f6e 6669 672e 6c61 6265 6c73 5b22  _config.labels["
-00006860: 6269 6766 7261 6d65 732d 6170 6922 5d20  bigframes-api"] 
-00006870: 3d20 6170 695f 6e61 6d65 0a20 2020 2020  = api_name.     
-00006880: 2020 2069 6620 7573 655f 6361 6368 6520     if use_cache 
-00006890: 616e 6420 7461 626c 655f 7265 6620 696e  and table_ref in
-000068a0: 2073 656c 662e 5f64 665f 736e 6170 7368   self._df_snapsh
-000068b0: 6f74 2e6b 6579 7328 293a 0a20 2020 2020  ot.keys():.     
-000068c0: 2020 2020 2020 2073 6e61 7073 686f 745f         snapshot_
-000068d0: 7469 6d65 7374 616d 7020 3d20 7365 6c66  timestamp = self
-000068e0: 2e5f 6466 5f73 6e61 7073 686f 745b 7461  ._df_snapshot[ta
-000068f0: 626c 655f 7265 665d 0a0a 2020 2020 2020  ble_ref]..      
-00006900: 2020 2020 2020 2320 4361 6368 6520 6869        # Cache hi
-00006910: 7420 636f 756c 6420 6265 2075 6e65 7870  t could be unexp
-00006920: 6563 7465 642e 2053 6565 2069 6e74 6572  ected. See inter
-00006930: 6e61 6c20 6973 7375 6520 3332 3935 3435  nal issue 329545
-00006940: 3830 352e 0a20 2020 2020 2020 2020 2020  805..           
-00006950: 2023 2052 6169 7365 2061 2077 6172 6e69   # Raise a warni
-00006960: 6e67 2077 6974 6820 6d6f 7265 2069 6e66  ng with more inf
-00006970: 6f72 6d61 7469 6f6e 2061 626f 7574 2068  ormation about h
-00006980: 6f77 2074 6f20 6176 6f69 6420 7468 650a  ow to avoid the.
-00006990: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
-000069a0: 6f62 6c65 6d73 2077 6974 6820 7468 6520  oblems with the 
-000069b0: 6361 6368 652e 0a20 2020 2020 2020 2020  cache..         
-000069c0: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-000069d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000069e0: 2020 6622 5265 6164 696e 6720 6361 6368    f"Reading cach
-000069f0: 6564 2074 6162 6c65 2066 726f 6d20 7b73  ed table from {s
-00006a00: 6e61 7073 686f 745f 7469 6d65 7374 616d  napshot_timestam
-00006a10: 707d 2074 6f20 6176 6f69 6420 220a 2020  p} to avoid ".  
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00006a30: 6e63 6f6d 7061 7469 6269 6c69 6573 2077  ncompatibilies w
-00006a40: 6974 6820 7072 6576 696f 7573 2072 6561  ith previous rea
-00006a50: 6473 206f 6620 7468 6973 2074 6162 6c65  ds of this table
-00006a60: 2e20 546f 2072 6561 6420 220a 2020 2020  . To read ".    
-00006a70: 2020 2020 2020 2020 2020 2020 2274 6865              "the
-00006a80: 206c 6174 6573 7420 7665 7273 696f 6e2c   latest version,
-00006a90: 2073 6574 2060 7573 655f 6361 6368 653d   set `use_cache=
-00006aa0: 4661 6c73 6560 206f 7220 636c 6f73 6520  False` or close 
-00006ab0: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
-00006ac0: 2020 2020 2020 2263 7572 7265 6e74 2073        "current s
-00006ad0: 6573 7369 6f6e 2077 6974 6820 5365 7373  ession with Sess
-00006ae0: 696f 6e2e 636c 6f73 6528 2920 6f72 2022  ion.close() or "
-00006af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b00: 2022 6269 6766 7261 6d65 732e 7061 6e64   "bigframes.pand
-00006b10: 6173 2e63 6c6f 7365 5f73 6573 7369 6f6e  as.close_session
-00006b20: 2829 2e22 2c0a 2020 2020 2020 2020 2020  ().",.          
-00006b30: 2020 2020 2020 2320 5468 6572 6520 6172        # There ar
-00006b40: 6520 6d61 6e79 206c 6179 6572 7320 6265  e many layers be
-00006b50: 666f 7265 2077 6520 6765 7420 746f 2028  fore we get to (
-00006b60: 706f 7373 6962 6c79 2920 7468 6520 7573  possibly) the us
-00006b70: 6572 2773 2063 6f64 653a 0a20 2020 2020  er's code:.     
-00006b80: 2020 2020 2020 2020 2020 2023 2070 616e             # pan
-00006b90: 6461 732e 7265 6164 5f67 6271 5f74 6162  das.read_gbq_tab
-00006ba0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
-00006bb0: 2020 2023 202d 3e20 7769 7468 5f64 6566     # -> with_def
-00006bc0: 6175 6c74 5f73 6573 7369 6f6e 0a20 2020  ault_session.   
-00006bd0: 2020 2020 2020 2020 2020 2020 2023 202d               # -
-00006be0: 3e20 5365 7373 696f 6e2e 7265 6164 5f67  > Session.read_g
-00006bf0: 6271 5f74 6162 6c65 0a20 2020 2020 2020  bq_table.       
-00006c00: 2020 2020 2020 2020 2023 202d 3e20 5f72           # -> _r
-00006c10: 6561 645f 6762 715f 7461 626c 650a 2020  ead_gbq_table.  
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006c30: 2d3e 205f 6765 745f 736e 6170 7368 6f74  -> _get_snapshot
-00006c40: 5f73 716c 5f61 6e64 5f70 7269 6d61 7279  _sql_and_primary
-00006c50: 5f6b 6579 0a20 2020 2020 2020 2020 2020  _key.           
-00006c60: 2020 2020 2073 7461 636b 6c65 7665 6c3d       stacklevel=
-00006c70: 362c 0a20 2020 2020 2020 2020 2020 2029  6,.            )
-00006c80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00006c90: 2020 2020 2020 2020 2020 2073 6e61 7073             snaps
-00006ca0: 686f 745f 7469 6d65 7374 616d 7020 3d20  hot_timestamp = 
-00006cb0: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
-00006cc0: 2020 2020 2020 7365 6c66 2e62 7163 6c69        self.bqcli
-00006cd0: 656e 742e 7175 6572 7928 0a20 2020 2020  ent.query(.     
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006cf0: 5345 4c45 4354 2043 5552 5245 4e54 5f54  SELECT CURRENT_T
-00006d00: 494d 4553 5441 4d50 2829 2041 5320 6063  IMESTAMP() AS `c
-00006d10: 7572 7265 6e74 5f74 696d 6573 7461 6d70  urrent_timestamp
-00006d20: 6022 2c0a 2020 2020 2020 2020 2020 2020  `",.            
-00006d30: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-00006d40: 6967 3d6a 6f62 5f63 6f6e 6669 672c 0a20  ig=job_config,. 
-00006d50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006d60: 2e72 6573 756c 7428 290a 2020 2020 2020  .result().      
-00006d70: 2020 2020 2020 295b 305d 5b30 5d0a 2020        )[0][0].  
-00006d80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00006d90: 6466 5f73 6e61 7073 686f 745b 7461 626c  df_snapshot[tabl
-00006da0: 655f 7265 665d 203d 2073 6e61 7073 686f  e_ref] = snapsho
-00006db0: 745f 7469 6d65 7374 616d 700a 0a20 2020  t_timestamp..   
-00006dc0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00006dd0: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
-00006de0: 6573 7369 6f6e 203d 2073 656c 662e 6962  ession = self.ib
-00006df0: 6973 5f63 6c69 656e 742e 7371 6c28 0a20  is_client.sql(. 
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00006e10: 6967 6672 616d 6573 5f69 6f2e 6372 6561  igframes_io.crea
-00006e20: 7465 5f73 6e61 7073 686f 745f 7371 6c28  te_snapshot_sql(
-00006e30: 7461 626c 655f 7265 662c 2073 6e61 7073  table_ref, snaps
-00006e40: 686f 745f 7469 6d65 7374 616d 7029 0a20  hot_timestamp). 
-00006e50: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00006e60: 2020 2020 2065 7863 6570 7420 676f 6f67       except goog
-00006e70: 6c65 2e61 7069 5f63 6f72 652e 6578 6365  le.api_core.exce
-00006e80: 7074 696f 6e73 2e46 6f72 6269 6464 656e  ptions.Forbidden
-00006e90: 2061 7320 6578 3a0a 2020 2020 2020 2020   as ex:.        
-00006ea0: 2020 2020 6966 2022 4472 6976 6520 6372      if "Drive cr
-00006eb0: 6564 656e 7469 616c 7322 2069 6e20 6578  edentials" in ex
-00006ec0: 2e6d 6573 7361 6765 3a0a 2020 2020 2020  .message:.      
-00006ed0: 2020 2020 2020 2020 2020 6578 2e6d 6573            ex.mes
-00006ee0: 7361 6765 202b 3d20 225c 6e43 6865 636b  sage += "\nCheck
-00006ef0: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-00006f00: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
-00006f10: 7279 2f64 6f63 732f 7175 6572 792d 6472  ry/docs/query-dr
-00006f20: 6976 652d 6461 7461 2347 6f6f 676c 655f  ive-data#Google_
-00006f30: 4472 6976 655f 7065 726d 6973 7369 6f6e  Drive_permission
-00006f40: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
-00006f50: 7261 6973 650a 0a20 2020 2020 2020 2072  raise..        r
-00006f60: 6574 7572 6e20 7461 626c 655f 6578 7072  eturn table_expr
-00006f70: 6573 7369 6f6e 2c20 7072 696d 6172 795f  ession, primary_
-00006f80: 6b65 7973 0a0a 2020 2020 6465 6620 5f72  keys..    def _r
-00006f90: 6561 645f 6762 715f 7461 626c 6528 0a20  ead_gbq_table(. 
-00006fa0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00006fb0: 2020 2020 2071 7565 7279 3a20 7374 722c       query: str,
-00006fc0: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00006fd0: 2020 2020 696e 6465 785f 636f 6c3a 2049      index_col: I
-00006fe0: 7465 7261 626c 655b 7374 725d 207c 2073  terable[str] | s
-00006ff0: 7472 203d 2028 292c 0a20 2020 2020 2020  tr = (),.       
-00007000: 2063 6f6c 756d 6e73 3a20 4974 6572 6162   columns: Iterab
-00007010: 6c65 5b73 7472 5d20 3d20 2829 2c0a 2020  le[str] = (),.  
-00007020: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
-00007030: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-00007040: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00007050: 2061 7069 5f6e 616d 653a 2073 7472 2c0a   api_name: str,.
-00007060: 2020 2020 2020 2020 7573 655f 6361 6368          use_cach
-00007070: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
-00007080: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
-00007090: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
-000070a0: 2020 2020 2020 696d 706f 7274 2062 6967        import big
-000070b0: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
-000070c0: 2061 7320 6461 7461 6672 616d 650a 0a20   as dataframe.. 
-000070d0: 2020 2020 2020 2069 6620 6d61 785f 7265         if max_re
-000070e0: 7375 6c74 7320 616e 6420 6d61 785f 7265  sults and max_re
-000070f0: 7375 6c74 7320 3c3d 2030 3a0a 2020 2020  sults <= 0:.    
-00007100: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00007110: 6c75 6545 7272 6f72 2822 606d 6178 5f72  lueError("`max_r
-00007120: 6573 756c 7473 6020 7368 6f75 6c64 2062  esults` should b
-00007130: 6520 6120 706f 7369 7469 7665 206e 756d  e a positive num
-00007140: 6265 722e 2229 0a0a 2020 2020 2020 2020  ber.")..        
-00007150: 7461 626c 655f 7265 6620 3d20 6269 6771  table_ref = bigq
-00007160: 7565 7279 2e74 6162 6c65 2e54 6162 6c65  uery.table.Table
-00007170: 5265 6665 7265 6e63 652e 6672 6f6d 5f73  Reference.from_s
-00007180: 7472 696e 6728 0a20 2020 2020 2020 2020  tring(.         
-00007190: 2020 2071 7565 7279 2c20 6465 6661 756c     query, defaul
-000071a0: 745f 7072 6f6a 6563 743d 7365 6c66 2e62  t_project=self.b
-000071b0: 7163 6c69 656e 742e 7072 6f6a 6563 740a  qclient.project.
-000071c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000071d0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-000071e0: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
-000071f0: 6e2c 0a20 2020 2020 2020 2020 2020 2074  n,.            t
-00007200: 6f74 616c 5f6f 7264 6572 696e 675f 636f  otal_ordering_co
-00007210: 6c73 2c0a 2020 2020 2020 2020 2920 3d20  ls,.        ) = 
-00007220: 7365 6c66 2e5f 6765 745f 736e 6170 7368  self._get_snapsh
-00007230: 6f74 5f73 716c 5f61 6e64 5f70 7269 6d61  ot_sql_and_prima
-00007240: 7279 5f6b 6579 280a 2020 2020 2020 2020  ry_key(.        
-00007250: 2020 2020 7461 626c 655f 7265 662c 2061      table_ref, a
-00007260: 7069 5f6e 616d 653d 6170 695f 6e61 6d65  pi_name=api_name
-00007270: 2c20 7573 655f 6361 6368 653d 7573 655f  , use_cache=use_
-00007280: 6361 6368 650a 2020 2020 2020 2020 290a  cache.        ).
-00007290: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-000072a0: 2069 6e20 636f 6c75 6d6e 733a 0a20 2020   in columns:.   
-000072b0: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
-000072c0: 6e6f 7420 696e 2074 6162 6c65 5f65 7870  not in table_exp
-000072d0: 7265 7373 696f 6e2e 636f 6c75 6d6e 733a  ression.columns:
-000072e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000072f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00007300: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00007310: 2020 2020 2020 2066 2243 6f6c 756d 6e20         f"Column 
-00007320: 277b 6b65 797d 2720 6f66 2060 636f 6c75  '{key}' of `colu
-00007330: 6d6e 7360 206e 6f74 2066 6f75 6e64 2069  mns` not found i
-00007340: 6e20 7468 6973 2074 6162 6c65 2e22 0a20  n this table.". 
-00007350: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007360: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-00007370: 6e73 7461 6e63 6528 696e 6465 785f 636f  nstance(index_co
-00007380: 6c2c 2073 7472 293a 0a20 2020 2020 2020  l, str):.       
-00007390: 2020 2020 2069 6e64 6578 5f63 6f6c 733a       index_cols:
-000073a0: 204c 6973 745b 7374 725d 203d 205b 696e   List[str] = [in
-000073b0: 6465 785f 636f 6c5d 0a20 2020 2020 2020  dex_col].       
-000073c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000073d0: 2020 2069 6e64 6578 5f63 6f6c 7320 3d20     index_cols = 
-000073e0: 6c69 7374 2869 6e64 6578 5f63 6f6c 290a  list(index_col).
-000073f0: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-00007400: 2069 6e20 696e 6465 785f 636f 6c73 3a0a   in index_cols:.
-00007410: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00007420: 6579 206e 6f74 2069 6e20 7461 626c 655f  ey not in table_
-00007430: 6578 7072 6573 7369 6f6e 2e63 6f6c 756d  expression.colum
-00007440: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00007450: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00007460: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00007470: 2020 2020 2020 2020 2020 6622 436f 6c75            f"Colu
-00007480: 6d6e 2060 7b6b 6579 7d60 206f 6620 6069  mn `{key}` of `i
-00007490: 6e64 6578 5f63 6f6c 6020 6e6f 7420 666f  ndex_col` not fo
-000074a0: 756e 6420 696e 2074 6869 7320 7461 626c  und in this tabl
-000074b0: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
-000074c0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-000074d0: 6620 636f 6c75 6d6e 733a 0a20 2020 2020  f columns:.     
-000074e0: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
-000074f0: 7265 7373 696f 6e20 3d20 7461 626c 655f  ression = table_
-00007500: 6578 7072 6573 7369 6f6e 2e73 656c 6563  expression.selec
-00007510: 7428 5b2a 696e 6465 785f 636f 6c73 2c20  t([*index_cols, 
-00007520: 2a63 6f6c 756d 6e73 5d29 0a0a 2020 2020  *columns])..    
-00007530: 2020 2020 2320 4966 2074 6865 2069 6e64      # If the ind
-00007540: 6578 2069 7320 756e 6971 7565 2061 6e64  ex is unique and
-00007550: 2073 6f72 7461 626c 652c 2074 6865 6e20   sortable, then 
-00007560: 7765 2064 6f6e 2774 206e 6565 6420 746f  we don't need to
-00007570: 2067 656e 6572 6174 650a 2020 2020 2020   generate.      
-00007580: 2020 2320 616e 206f 7264 6572 696e 6720    # an ordering 
-00007590: 636f 6c75 6d6e 2e0a 2020 2020 2020 2020  column..        
-000075a0: 6f72 6465 7269 6e67 203d 204e 6f6e 650a  ordering = None.
-000075b0: 2020 2020 2020 2020 6966 2074 6f74 616c          if total
-000075c0: 5f6f 7264 6572 696e 675f 636f 6c73 2069  _ordering_cols i
-000075d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000075e0: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
-000075f0: 6375 7272 656e 746c 792c 2061 2074 6162  currently, a tab
-00007600: 6c65 2068 6173 2061 2074 6f74 616c 206f  le has a total o
-00007610: 7264 6572 696e 6720 6f6e 6c79 2077 6865  rdering only whe
-00007620: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
-00007630: 2020 2320 7072 696d 6172 7920 6b65 7928    # primary key(
-00007640: 7329 2061 7265 2073 6574 206f 6e20 6120  s) are set on a 
-00007650: 7461 626c 652e 2054 6865 2071 7565 7279  table. The query
-00007660: 2065 6e67 696e 6520 6173 7375 6d65 7320   engine assumes 
-00007670: 7375 6368 0a20 2020 2020 2020 2020 2020  such.           
-00007680: 2023 2063 6f6c 756d 6e73 2061 7265 2075   # columns are u
-00007690: 6e69 7175 652c 2065 7665 6e20 6966 206e  nique, even if n
-000076a0: 6f74 2065 6e66 6f72 6365 642e 0a20 2020  ot enforced..   
-000076b0: 2020 2020 2020 2020 206f 7264 6572 696e           orderin
-000076c0: 6720 3d20 6f72 6465 722e 4578 7072 6573  g = order.Expres
-000076d0: 7369 6f6e 4f72 6465 7269 6e67 280a 2020  sionOrdering(.  
-000076e0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-000076f0: 6465 7269 6e67 5f76 616c 7565 5f63 6f6c  dering_value_col
-00007700: 756d 6e73 3d74 7570 6c65 280a 2020 2020  umns=tuple(.    
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 6f72 6465 722e 6173 6365 6e64 696e 675f  order.ascending_
-00007730: 6f76 6572 2863 6f6c 756d 6e5f 6964 2920  over(column_id) 
-00007740: 666f 7220 636f 6c75 6d6e 5f69 6420 696e  for column_id in
-00007750: 2074 6f74 616c 5f6f 7264 6572 696e 675f   total_ordering_
-00007760: 636f 6c73 0a20 2020 2020 2020 2020 2020  cols.           
-00007770: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00007780: 2020 2020 2020 2020 746f 7461 6c5f 6f72          total_or
-00007790: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d66  dering_columns=f
-000077a0: 726f 7a65 6e73 6574 2874 6f74 616c 5f6f  rozenset(total_o
-000077b0: 7264 6572 696e 675f 636f 6c73 292c 0a20  rdering_cols),. 
-000077c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000077d0: 2020 2020 2020 2020 2063 6f6c 756d 6e5f           column_
-000077e0: 7661 6c75 6573 203d 205b 7461 626c 655f  values = [table_
-000077f0: 6578 7072 6573 7369 6f6e 5b63 6f6c 5d20  expression[col] 
-00007800: 666f 7220 636f 6c20 696e 2074 6162 6c65  for col in table
-00007810: 5f65 7870 7265 7373 696f 6e2e 636f 6c75  _expression.colu
-00007820: 6d6e 735d 0a20 2020 2020 2020 2020 2020  mns].           
-00007830: 2061 7272 6179 5f76 616c 7565 203d 2063   array_value = c
-00007840: 6f72 652e 4172 7261 7956 616c 7565 2e66  ore.ArrayValue.f
-00007850: 726f 6d5f 6962 6973 280a 2020 2020 2020  rom_ibis(.      
-00007860: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00007890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000078a0: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
-000078b0: 5f76 616c 7565 732c 0a20 2020 2020 2020  _values,.       
-000078c0: 2020 2020 2020 2020 2068 6964 6465 6e5f           hidden_
-000078d0: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
-000078e0: 3d5b 5d2c 0a20 2020 2020 2020 2020 2020  =[],.           
-000078f0: 2020 2020 206f 7264 6572 696e 673d 6f72       ordering=or
-00007900: 6465 7269 6e67 2c0a 2020 2020 2020 2020  dering,.        
-00007910: 2020 2020 290a 0a20 2020 2020 2020 2065      )..        e
-00007920: 6c69 6620 6c65 6e28 696e 6465 785f 636f  lif len(index_co
-00007930: 6c73 2920 213d 2030 3a0a 2020 2020 2020  ls) != 0:.      
-00007940: 2020 2020 2020 2320 5765 2068 6176 6520        # We have 
-00007950: 696e 6465 7820 636f 6c75 6d6e 732c 206c  index columns, l
-00007960: 6574 7320 7365 6520 6966 2074 686f 7365  ets see if those
-00007970: 2061 7265 2061 6374 7561 6c6c 7920 746f   are actually to
-00007980: 7461 6c5f 6f72 6465 725f 636f 6c75 6d6e  tal_order_column
-00007990: 730a 2020 2020 2020 2020 2020 2020 6f72  s.            or
-000079a0: 6465 7269 6e67 203d 206f 7264 6572 2e45  dering = order.E
-000079b0: 7870 7265 7373 696f 6e4f 7264 6572 696e  xpressionOrderin
-000079c0: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-000079d0: 2020 206f 7264 6572 696e 675f 7661 6c75     ordering_valu
-000079e0: 655f 636f 6c75 6d6e 733d 7475 706c 6528  e_columns=tuple(
-000079f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a00: 2020 2020 205b 6f72 6465 722e 6173 6365       [order.asce
-00007a10: 6e64 696e 675f 6f76 6572 2863 6f6c 756d  nding_over(colum
-00007a20: 6e5f 6964 2920 666f 7220 636f 6c75 6d6e  n_id) for column
-00007a30: 5f69 6420 696e 2069 6e64 6578 5f63 6f6c  _id in index_col
-00007a40: 735d 0a20 2020 2020 2020 2020 2020 2020  s].             
-00007a50: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00007a60: 2020 2020 2020 746f 7461 6c5f 6f72 6465        total_orde
-00007a70: 7269 6e67 5f63 6f6c 756d 6e73 3d66 726f  ring_columns=fro
-00007a80: 7a65 6e73 6574 2869 6e64 6578 5f63 6f6c  zenset(index_col
-00007a90: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00007aa0: 290a 2020 2020 2020 2020 2020 2020 6973  ).            is
-00007ab0: 5f74 6f74 616c 5f6f 7264 6572 696e 6720  _total_ordering 
-00007ac0: 3d20 7365 6c66 2e5f 6368 6563 6b5f 696e  = self._check_in
-00007ad0: 6465 785f 756e 6971 7565 6e65 7373 280a  dex_uniqueness(.
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007af0: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00007b00: 2c20 696e 6465 785f 636f 6c73 0a20 2020  , index_cols.   
-00007b10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00007b20: 2020 2020 2020 2069 6620 6973 5f74 6f74         if is_tot
-00007b30: 616c 5f6f 7264 6572 696e 673a 0a20 2020  al_ordering:.   
-00007b40: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00007b50: 756d 6e5f 7661 6c75 6573 203d 205b 0a20  umn_values = [. 
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
-00007b80: 696f 6e5b 636f 6c5d 2066 6f72 2063 6f6c  ion[col] for col
-00007b90: 2069 6e20 7461 626c 655f 6578 7072 6573   in table_expres
-00007ba0: 7369 6f6e 2e63 6f6c 756d 6e73 0a20 2020  sion.columns.   
-00007bb0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00007bd0: 7272 6179 5f76 616c 7565 203d 2063 6f72  rray_value = cor
-00007be0: 652e 4172 7261 7956 616c 7565 2e66 726f  e.ArrayValue.fro
-00007bf0: 6d5f 6962 6973 280a 2020 2020 2020 2020  m_ibis(.        
-00007c00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007c20: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
-00007c30: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
-00007c40: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00007c50: 6d6e 733d 636f 6c75 6d6e 5f76 616c 7565  mns=column_value
-00007c60: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00007c70: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
-00007c80: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d5b  dering_columns=[
-00007c90: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00007ca0: 2020 2020 2020 206f 7264 6572 696e 673d         ordering=
-00007cb0: 6f72 6465 7269 6e67 2c0a 2020 2020 2020  ordering,.      
-00007cc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007cd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00007cf0: 7261 795f 7661 6c75 6520 3d20 7365 6c66  ray_value = self
-00007d00: 2e5f 6372 6561 7465 5f74 6f74 616c 5f6f  ._create_total_o
-00007d10: 7264 6572 696e 6728 7461 626c 655f 6578  rdering(table_ex
-00007d20: 7072 6573 7369 6f6e 290a 2020 2020 2020  pression).      
-00007d30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007d40: 2020 2020 6172 7261 795f 7661 6c75 6520      array_value 
-00007d50: 3d20 7365 6c66 2e5f 6372 6561 7465 5f74  = self._create_t
-00007d60: 6f74 616c 5f6f 7264 6572 696e 6728 7461  otal_ordering(ta
-00007d70: 626c 655f 6578 7072 6573 7369 6f6e 290a  ble_expression).
-00007d80: 0a20 2020 2020 2020 2076 616c 7565 5f63  .        value_c
-00007d90: 6f6c 756d 6e73 203d 205b 636f 6c20 666f  olumns = [col fo
-00007da0: 7220 636f 6c20 696e 2061 7272 6179 5f76  r col in array_v
-00007db0: 616c 7565 2e63 6f6c 756d 6e5f 6964 7320  alue.column_ids 
-00007dc0: 6966 2063 6f6c 206e 6f74 2069 6e20 696e  if col not in in
-00007dd0: 6465 785f 636f 6c73 5d0a 2020 2020 2020  dex_cols].      
-00007de0: 2020 626c 6f63 6b20 3d20 626c 6f63 6b73    block = blocks
-00007df0: 2e42 6c6f 636b 280a 2020 2020 2020 2020  .Block(.        
-00007e00: 2020 2020 6172 7261 795f 7661 6c75 652c      array_value,
-00007e10: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-00007e20: 6578 5f63 6f6c 756d 6e73 3d69 6e64 6578  ex_columns=index
-00007e30: 5f63 6f6c 732c 0a20 2020 2020 2020 2020  _cols,.         
-00007e40: 2020 2063 6f6c 756d 6e5f 6c61 6265 6c73     column_labels
-00007e50: 3d76 616c 7565 5f63 6f6c 756d 6e73 2c0a  =value_columns,.
-00007e60: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00007e70: 785f 6c61 6265 6c73 3d69 6e64 6578 5f63  x_labels=index_c
-00007e80: 6f6c 732c 0a20 2020 2020 2020 2029 0a20  ols,.        ). 
-00007e90: 2020 2020 2020 2069 6620 6d61 785f 7265         if max_re
-00007ea0: 7375 6c74 733a 0a20 2020 2020 2020 2020  sults:.         
-00007eb0: 2020 2062 6c6f 636b 203d 2062 6c6f 636b     block = block
-00007ec0: 2e73 6c69 6365 2873 746f 703d 6d61 785f  .slice(stop=max_
-00007ed0: 7265 7375 6c74 7329 0a20 2020 2020 2020  results).       
-00007ee0: 2064 6620 3d20 6461 7461 6672 616d 652e   df = dataframe.
-00007ef0: 4461 7461 4672 616d 6528 626c 6f63 6b29  DataFrame(block)
-00007f00: 0a0a 2020 2020 2020 2020 2320 4966 2075  ..        # If u
-00007f10: 7365 7220 7072 6f76 6964 6564 2069 6e64  ser provided ind
-00007f20: 6578 2063 6f6c 756d 6e73 2c20 7368 6f75  ex columns, shou
-00007f30: 6c64 2073 6f72 7420 6f76 6572 2069 740a  ld sort over it.
-00007f40: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
-00007f50: 6e64 6578 5f63 6f6c 7329 203e 2030 3a0a  ndex_cols) > 0:.
-00007f60: 2020 2020 2020 2020 2020 2020 6466 2e73              df.s
-00007f70: 6f72 745f 696e 6465 7828 290a 2020 2020  ort_index().    
-00007f80: 2020 2020 7265 7475 726e 2064 660a 0a20      return df.. 
-00007f90: 2020 2064 6566 205f 6368 6563 6b5f 696e     def _check_in
-00007fa0: 6465 785f 756e 6971 7565 6e65 7373 280a  dex_uniqueness(.
-00007fb0: 2020 2020 2020 2020 7365 6c66 2c20 7461          self, ta
-00007fc0: 626c 653a 2069 6269 735f 7479 7065 732e  ble: ibis_types.
-00007fd0: 5461 626c 652c 2069 6e64 6578 5f63 6f6c  Table, index_col
-00007fe0: 733a 204c 6973 745b 7374 725d 0a20 2020  s: List[str].   
-00007ff0: 2029 202d 3e20 626f 6f6c 3a0a 2020 2020   ) -> bool:.    
-00008000: 2020 2020 6469 7374 696e 6374 5f74 6162      distinct_tab
-00008010: 6c65 203d 2074 6162 6c65 2e73 656c 6563  le = table.selec
-00008020: 7428 2a69 6e64 6578 5f63 6f6c 7329 2e64  t(*index_cols).d
-00008030: 6973 7469 6e63 7428 290a 2020 2020 2020  istinct().      
-00008040: 2020 6973 5f75 6e69 7175 655f 7371 6c20    is_unique_sql 
-00008050: 3d20 6622 2222 5749 5448 2066 756c 6c5f  = f"""WITH full_
-00008060: 7461 626c 6520 4153 2028 0a20 2020 2020  table AS (.     
-00008070: 2020 2020 2020 207b 7365 6c66 2e69 6269         {self.ibi
-00008080: 735f 636c 6965 6e74 2e63 6f6d 7069 6c65  s_client.compile
-00008090: 2874 6162 6c65 297d 0a20 2020 2020 2020  (table)}.       
-000080a0: 2029 2c0a 2020 2020 2020 2020 6469 7374   ),.        dist
-000080b0: 696e 6374 5f74 6162 6c65 2041 5320 280a  inct_table AS (.
-000080c0: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
-000080d0: 662e 6962 6973 5f63 6c69 656e 742e 636f  f.ibis_client.co
-000080e0: 6d70 696c 6528 6469 7374 696e 6374 5f74  mpile(distinct_t
-000080f0: 6162 6c65 297d 0a20 2020 2020 2020 2029  able)}.        )
-00008100: 0a0a 2020 2020 2020 2020 5345 4c45 4354  ..        SELECT
-00008110: 2028 5345 4c45 4354 2043 4f55 4e54 282a   (SELECT COUNT(*
-00008120: 2920 4652 4f4d 2066 756c 6c5f 7461 626c  ) FROM full_tabl
-00008130: 6529 2041 5320 6074 6f74 616c 5f63 6f75  e) AS `total_cou
-00008140: 6e74 602c 0a20 2020 2020 2020 2028 5345  nt`,.        (SE
-00008150: 4c45 4354 2043 4f55 4e54 282a 2920 4652  LECT COUNT(*) FR
-00008160: 4f4d 2064 6973 7469 6e63 745f 7461 626c  OM distinct_tabl
-00008170: 6529 2041 5320 6064 6973 7469 6e63 745f  e) AS `distinct_
-00008180: 636f 756e 7460 0a20 2020 2020 2020 2022  count`.        "
-00008190: 2222 0a20 2020 2020 2020 2072 6573 756c  "".        resul
-000081a0: 7473 2c20 5f20 3d20 7365 6c66 2e5f 7374  ts, _ = self._st
-000081b0: 6172 745f 7175 6572 7928 6973 5f75 6e69  art_query(is_uni
-000081c0: 7175 655f 7371 6c29 0a20 2020 2020 2020  que_sql).       
-000081d0: 2072 6f77 203d 206e 6578 7428 6974 6572   row = next(iter
-000081e0: 2872 6573 756c 7473 2929 0a0a 2020 2020  (results))..    
-000081f0: 2020 2020 746f 7461 6c5f 636f 756e 7420      total_count 
-00008200: 3d20 726f 775b 2274 6f74 616c 5f63 6f75  = row["total_cou
-00008210: 6e74 225d 0a20 2020 2020 2020 2064 6973  nt"].        dis
-00008220: 7469 6e63 745f 636f 756e 7420 3d20 726f  tinct_count = ro
-00008230: 775b 2264 6973 7469 6e63 745f 636f 756e  w["distinct_coun
-00008240: 7422 5d0a 2020 2020 2020 2020 7265 7475  t"].        retu
-00008250: 726e 2074 6f74 616c 5f63 6f75 6e74 203d  rn total_count =
-00008260: 3d20 6469 7374 696e 6374 5f63 6f75 6e74  = distinct_count
-00008270: 0a0a 2020 2020 6465 6620 5f72 6561 645f  ..    def _read_
-00008280: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
-00008290: 6228 0a20 2020 2020 2020 2073 656c 662c  b(.        self,
-000082a0: 0a20 2020 2020 2020 2066 696c 6570 6174  .        filepat
-000082b0: 685f 6f72 5f62 7566 6665 723a 2073 7472  h_or_buffer: str
-000082c0: 207c 2049 4f5b 2262 7974 6573 225d 2c0a   | IO["bytes"],.
-000082d0: 2020 2020 2020 2020 7461 626c 653a 2055          table: U
-000082e0: 6e69 6f6e 5b62 6967 7175 6572 792e 5461  nion[bigquery.Ta
-000082f0: 626c 652c 2062 6967 7175 6572 792e 5461  ble, bigquery.Ta
-00008300: 626c 6552 6566 6572 656e 6365 5d2c 0a20  bleReference],. 
-00008310: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00008320: 2020 6a6f 625f 636f 6e66 6967 3a20 6269    job_config: bi
-00008330: 6771 7565 7279 2e4c 6f61 644a 6f62 436f  gquery.LoadJobCo
-00008340: 6e66 6967 2c0a 2020 2020 2020 2020 696e  nfig,.        in
-00008350: 6465 785f 636f 6c3a 2049 7465 7261 626c  dex_col: Iterabl
-00008360: 655b 7374 725d 207c 2073 7472 203d 2028  e[str] | str = (
-00008370: 292c 0a20 2020 2020 2020 2063 6f6c 756d  ),.        colum
-00008380: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
-00008390: 5d20 3d20 2829 2c0a 2020 2020 2920 2d3e  ] = (),.    ) ->
-000083a0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
-000083b0: 7261 6d65 3a0a 2020 2020 2020 2020 6966  rame:.        if
-000083c0: 2069 7369 6e73 7461 6e63 6528 696e 6465   isinstance(inde
-000083d0: 785f 636f 6c2c 2073 7472 293a 0a20 2020  x_col, str):.   
-000083e0: 2020 2020 2020 2020 2069 6e64 6578 5f63           index_c
-000083f0: 6f6c 7320 3d20 5b69 6e64 6578 5f63 6f6c  ols = [index_col
-00008400: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-00008410: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00008420: 785f 636f 6c73 203d 206c 6973 7428 696e  x_cols = list(in
-00008430: 6465 785f 636f 6c29 0a0a 2020 2020 2020  dex_col)..      
-00008440: 2020 6966 206e 6f74 206a 6f62 5f63 6f6e    if not job_con
-00008450: 6669 672e 636c 7573 7465 7269 6e67 5f66  fig.clustering_f
-00008460: 6965 6c64 7320 616e 6420 696e 6465 785f  ields and index_
-00008470: 636f 6c73 3a0a 2020 2020 2020 2020 2020  cols:.          
-00008480: 2020 6a6f 625f 636f 6e66 6967 2e63 6c75    job_config.clu
-00008490: 7374 6572 696e 675f 6669 656c 6473 203d  stering_fields =
-000084a0: 2069 6e64 6578 5f63 6f6c 735b 3a5f 4d41   index_cols[:_MA
-000084b0: 585f 434c 5553 5445 525f 434f 4c55 4d4e  X_CLUSTER_COLUMN
-000084c0: 535d 0a0a 2020 2020 2020 2020 6966 2069  S]..        if i
-000084d0: 7369 6e73 7461 6e63 6528 6669 6c65 7061  sinstance(filepa
-000084e0: 7468 5f6f 725f 6275 6666 6572 2c20 7374  th_or_buffer, st
-000084f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00008500: 6966 2066 696c 6570 6174 685f 6f72 5f62  if filepath_or_b
-00008510: 7566 6665 722e 7374 6172 7473 7769 7468  uffer.startswith
-00008520: 2822 6773 3a2f 2f22 293a 0a20 2020 2020  ("gs://"):.     
-00008530: 2020 2020 2020 2020 2020 206c 6f61 645f             load_
-00008540: 6a6f 6220 3d20 7365 6c66 2e62 7163 6c69  job = self.bqcli
-00008550: 656e 742e 6c6f 6164 5f74 6162 6c65 5f66  ent.load_table_f
-00008560: 726f 6d5f 7572 6928 0a20 2020 2020 2020  rom_uri(.       
-00008570: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00008580: 6570 6174 685f 6f72 5f62 7566 6665 722c  epath_or_buffer,
-00008590: 2074 6162 6c65 2c20 6a6f 625f 636f 6e66   table, job_conf
-000085a0: 6967 3d6a 6f62 5f63 6f6e 6669 670a 2020  ig=job_config.  
-000085b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000085c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000085d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000085e0: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
-000085f0: 7061 7468 5f6f 725f 6275 6666 6572 2c20  path_or_buffer, 
-00008600: 2272 6222 2920 6173 2073 6f75 7263 655f  "rb") as source_
-00008610: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-00008620: 2020 2020 2020 2020 2020 6c6f 6164 5f6a            load_j
-00008630: 6f62 203d 2073 656c 662e 6271 636c 6965  ob = self.bqclie
-00008640: 6e74 2e6c 6f61 645f 7461 626c 655f 6672  nt.load_table_fr
-00008650: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
-00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008670: 2073 6f75 7263 655f 6669 6c65 2c20 7461   source_file, ta
-00008680: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
-00008690: 6a6f 625f 636f 6e66 6967 0a20 2020 2020  job_config.     
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000086b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000086c0: 2020 2020 2020 2020 2020 206c 6f61 645f             load_
-000086d0: 6a6f 6220 3d20 7365 6c66 2e62 7163 6c69  job = self.bqcli
-000086e0: 656e 742e 6c6f 6164 5f74 6162 6c65 5f66  ent.load_table_f
-000086f0: 726f 6d5f 6669 6c65 280a 2020 2020 2020  rom_file(.      
-00008700: 2020 2020 2020 2020 2020 6669 6c65 7061            filepa
-00008710: 7468 5f6f 725f 6275 6666 6572 2c20 7461  th_or_buffer, ta
-00008720: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
-00008730: 6a6f 625f 636f 6e66 6967 0a20 2020 2020  job_config.     
-00008740: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00008750: 2020 7365 6c66 2e5f 7374 6172 745f 6765    self._start_ge
-00008760: 6e65 7269 635f 6a6f 6228 6c6f 6164 5f6a  neric_job(load_j
-00008770: 6f62 290a 2020 2020 2020 2020 7461 626c  ob).        tabl
-00008780: 655f 6964 203d 2066 227b 7461 626c 652e  e_id = f"{table.
-00008790: 7072 6f6a 6563 747d 2e7b 7461 626c 652e  project}.{table.
-000087a0: 6461 7461 7365 745f 6964 7d2e 7b74 6162  dataset_id}.{tab
-000087b0: 6c65 2e74 6162 6c65 5f69 647d 220a 0a20  le.table_id}".. 
-000087c0: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
-000087d0: 7468 6520 7461 626c 6520 6578 7069 7261  the table expira
-000087e0: 7469 6f6e 2073 6f20 7765 2061 7265 6e27  tion so we aren'
-000087f0: 7420 6c69 6d69 7465 6420 746f 2074 6865  t limited to the
-00008800: 2064 6566 6175 6c74 2032 340a 2020 2020   default 24.    
-00008810: 2020 2020 2320 686f 7572 7320 6f66 2074      # hours of t
-00008820: 6865 2061 6e6f 6e79 6d6f 7573 2064 6174  he anonymous dat
-00008830: 6173 6574 2e0a 2020 2020 2020 2020 7461  aset..        ta
-00008840: 626c 655f 6578 7069 7261 7469 6f6e 203d  ble_expiration =
-00008850: 2062 6967 7175 6572 792e 5461 626c 6528   bigquery.Table(
-00008860: 7461 626c 655f 6964 290a 2020 2020 2020  table_id).      
-00008870: 2020 7461 626c 655f 6578 7069 7261 7469    table_expirati
-00008880: 6f6e 2e65 7870 6972 6573 203d 2028 0a20  on.expires = (. 
-00008890: 2020 2020 2020 2020 2020 2064 6174 6574             datet
-000088a0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-000088b0: 2864 6174 6574 696d 652e 7469 6d65 7a6f  (datetime.timezo
-000088c0: 6e65 2e75 7463 2920 2b20 636f 6e73 7461  ne.utc) + consta
-000088d0: 6e74 732e 4445 4641 554c 545f 4558 5049  nts.DEFAULT_EXPI
-000088e0: 5241 5449 4f4e 0a20 2020 2020 2020 2029  RATION.        )
-000088f0: 0a20 2020 2020 2020 2073 656c 662e 6271  .        self.bq
-00008900: 636c 6965 6e74 2e75 7064 6174 655f 7461  client.update_ta
-00008910: 626c 6528 7461 626c 655f 6578 7069 7261  ble(table_expira
-00008920: 7469 6f6e 2c20 5b22 6578 7069 7265 7322  tion, ["expires"
-00008930: 5d29 0a0a 2020 2020 2020 2020 2320 5468  ])..        # Th
-00008940: 6520 4269 6751 7565 7279 2052 4553 5420  e BigQuery REST 
-00008950: 4150 4920 666f 7220 7461 626c 6573 2e67  API for tables.g
-00008960: 6574 2064 6f65 736e 2774 2074 616b 6520  et doesn't take 
-00008970: 6120 7365 7373 696f 6e20 4944 2c20 736f  a session ID, so
-00008980: 2077 650a 2020 2020 2020 2020 2320 6361   we.        # ca
-00008990: 6e27 7420 6765 7420 7468 6520 7363 6865  n't get the sche
-000089a0: 6d61 2066 6f72 2061 2074 656d 7020 7461  ma for a temp ta
-000089b0: 626c 6520 7468 6174 2077 6179 2e0a 2020  ble that way..  
-000089c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000089d0: 662e 7265 6164 5f67 6271 5f74 6162 6c65  f.read_gbq_table
-000089e0: 280a 2020 2020 2020 2020 2020 2020 7461  (.            ta
-000089f0: 626c 655f 6964 2c0a 2020 2020 2020 2020  ble_id,.        
-00008a00: 2020 2020 696e 6465 785f 636f 6c3d 696e      index_col=in
-00008a10: 6465 785f 636f 6c2c 0a20 2020 2020 2020  dex_col,.       
-00008a20: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
-00008a30: 756d 6e73 2c0a 2020 2020 2020 2020 290a  umns,.        ).
-00008a40: 0a20 2020 2064 6566 2072 6561 645f 6762  .    def read_gb
-00008a50: 715f 6d6f 6465 6c28 7365 6c66 2c20 6d6f  q_model(self, mo
-00008a60: 6465 6c5f 6e61 6d65 3a20 7374 7229 3a0a  del_name: str):.
-00008a70: 2020 2020 2020 2020 2222 224c 6f61 6473          """Loads
-00008a80: 2061 2042 6967 5175 6572 7920 4d4c 206d   a BigQuery ML m
-00008a90: 6f64 656c 2066 726f 6d20 4269 6751 7565  odel from BigQue
-00008aa0: 7279 2e0a 0a20 2020 2020 2020 202a 2a45  ry...        **E
-00008ab0: 7861 6d70 6c65 733a 2a2a 0a0a 2020 2020  xamples:**..    
-00008ac0: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
-00008ad0: 7274 2062 6967 6672 616d 6573 2e70 616e  rt bigframes.pan
-00008ae0: 6461 7320 6173 2062 7064 0a20 2020 2020  das as bpd.     
-00008af0: 2020 2020 2020 203e 3e3e 2062 7064 2e6f         >>> bpd.o
-00008b00: 7074 696f 6e73 2e64 6973 706c 6179 2e70  ptions.display.p
-00008b10: 726f 6772 6573 735f 6261 7220 3d20 4e6f  rogress_bar = No
-00008b20: 6e65 0a0a 2020 2020 2020 2020 5265 6164  ne..        Read
-00008b30: 2061 6e20 6578 6973 7469 6e67 2042 6967   an existing Big
-00008b40: 5175 6572 7920 4d4c 206d 6f64 656c 2e0a  Query ML model..
-00008b50: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00008b60: 206d 6f64 656c 5f6e 616d 6520 3d20 2262   model_name = "b
-00008b70: 6967 6672 616d 6573 2d64 6576 2e62 716d  igframes-dev.bqm
-00008b80: 6c5f 7475 746f 7269 616c 2e70 656e 6775  l_tutorial.pengu
-00008b90: 696e 735f 6d6f 6465 6c22 0a20 2020 2020  ins_model".     
-00008ba0: 2020 2020 2020 203e 3e3e 206d 6f64 656c         >>> model
-00008bb0: 203d 2062 7064 2e72 6561 645f 6762 715f   = bpd.read_gbq_
-00008bc0: 6d6f 6465 6c28 6d6f 6465 6c5f 6e61 6d65  model(model_name
-00008bd0: 290a 0a20 2020 2020 2020 2041 7267 733a  )..        Args:
-00008be0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-00008bf0: 656c 5f6e 616d 6520 2873 7472 293a 0a20  el_name (str):. 
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00008c10: 6865 206d 6f64 656c 2773 206e 616d 6520  he model's name 
-00008c20: 696e 2042 6967 5175 6572 7920 696e 2074  in BigQuery in t
-00008c30: 6865 2066 6f72 6d61 740a 2020 2020 2020  he format.      
-00008c40: 2020 2020 2020 2020 2020 6070 726f 6a65            `proje
-00008c50: 6374 5f69 642e 6461 7461 7365 745f 6964  ct_id.dataset_id
-00008c60: 2e6d 6f64 656c 5f69 6460 2c20 6f72 206a  .model_id`, or j
-00008c70: 7573 7420 6064 6174 6173 6574 5f69 642e  ust `dataset_id.
-00008c80: 6d6f 6465 6c5f 6964 600a 2020 2020 2020  model_id`.      
-00008c90: 2020 2020 2020 2020 2020 746f 206c 6f61            to loa
-00008ca0: 6420 6672 6f6d 2074 6865 2064 6566 6175  d from the defau
-00008cb0: 6c74 2070 726f 6a65 6374 2e0a 0a20 2020  lt project...   
-00008cc0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00008cd0: 2020 2020 2020 2020 2020 4120 6269 6766            A bigf
-00008ce0: 7261 6d65 732e 6d6c 204d 6f64 656c 2c20  rames.ml Model, 
-00008cf0: 5472 616e 7366 6f72 6d65 7220 6f72 2050  Transformer or P
-00008d00: 6970 656c 696e 6520 7772 6170 7069 6e67  ipeline wrapping
-00008d10: 2074 6865 206d 6f64 656c 2e0a 2020 2020   the model..    
-00008d20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008d30: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
-00008d40: 2e6d 6c2e 6c6f 6164 6572 0a0a 2020 2020  .ml.loader..    
-00008d50: 2020 2020 6d6f 6465 6c5f 7265 6620 3d20      model_ref = 
-00008d60: 6269 6771 7565 7279 2e4d 6f64 656c 5265  bigquery.ModelRe
-00008d70: 6665 7265 6e63 652e 6672 6f6d 5f73 7472  ference.from_str
-00008d80: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00008d90: 206d 6f64 656c 5f6e 616d 652c 2064 6566   model_name, def
-00008da0: 6175 6c74 5f70 726f 6a65 6374 3d73 656c  ault_project=sel
-00008db0: 662e 6271 636c 6965 6e74 2e70 726f 6a65  f.bqclient.proje
-00008dc0: 6374 0a20 2020 2020 2020 2029 0a20 2020  ct.        ).   
-00008dd0: 2020 2020 206d 6f64 656c 203d 2073 656c       model = sel
-00008de0: 662e 6271 636c 6965 6e74 2e67 6574 5f6d  f.bqclient.get_m
-00008df0: 6f64 656c 286d 6f64 656c 5f72 6566 290a  odel(model_ref).
-00008e00: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00008e10: 6967 6672 616d 6573 2e6d 6c2e 6c6f 6164  igframes.ml.load
-00008e20: 6572 2e66 726f 6d5f 6271 2873 656c 662c  er.from_bq(self,
-00008e30: 206d 6f64 656c 290a 0a20 2020 2040 7479   model)..    @ty
-00008e40: 7069 6e67 2e6f 7665 726c 6f61 640a 2020  ping.overload.  
-00008e50: 2020 6465 6620 7265 6164 5f70 616e 6461    def read_panda
-00008e60: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00008e70: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-00008e80: 653a 2070 616e 6461 732e 496e 6465 780a  e: pandas.Index.
-00008e90: 2020 2020 2920 2d3e 2062 6967 6672 616d      ) -> bigfram
-00008ea0: 6573 2e63 6f72 652e 696e 6465 7865 732e  es.core.indexes.
-00008eb0: 496e 6465 783a 0a20 2020 2020 2020 202e  Index:.        .
-00008ec0: 2e2e 0a0a 2020 2020 4074 7970 696e 672e  ....    @typing.
-00008ed0: 6f76 6572 6c6f 6164 0a20 2020 2064 6566  overload.    def
-00008ee0: 2072 6561 645f 7061 6e64 6173 2873 656c   read_pandas(sel
-00008ef0: 662c 2070 616e 6461 735f 6461 7461 6672  f, pandas_datafr
-00008f00: 616d 653a 2070 616e 6461 732e 5365 7269  ame: pandas.Seri
-00008f10: 6573 2920 2d3e 2062 6967 6672 616d 6573  es) -> bigframes
-00008f20: 2e73 6572 6965 732e 5365 7269 6573 3a0a  .series.Series:.
-00008f30: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
-00008f40: 2040 7479 7069 6e67 2e6f 7665 726c 6f61   @typing.overloa
-00008f50: 640a 2020 2020 6465 6620 7265 6164 5f70  d.    def read_p
-00008f60: 616e 6461 7328 7365 6c66 2c20 7061 6e64  andas(self, pand
-00008f70: 6173 5f64 6174 6166 7261 6d65 3a20 7061  as_dataframe: pa
-00008f80: 6e64 6173 2e44 6174 6146 7261 6d65 2920  ndas.DataFrame) 
-00008f90: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
-00008fa0: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-00008fb0: 2e2e 2e0a 0a20 2020 2064 6566 2072 6561  .....    def rea
-00008fc0: 645f 7061 6e64 6173 280a 2020 2020 2020  d_pandas(.      
-00008fd0: 2020 7365 6c66 2c20 7061 6e64 6173 5f64    self, pandas_d
-00008fe0: 6174 6166 7261 6d65 3a20 556e 696f 6e5b  ataframe: Union[
-00008ff0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00009000: 2c20 7061 6e64 6173 2e53 6572 6965 732c  , pandas.Series,
-00009010: 2070 616e 6461 732e 496e 6465 785d 0a20   pandas.Index]. 
-00009020: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00009030: 224c 6f61 6473 2044 6174 6146 7261 6d65  "Loads DataFrame
-00009040: 2066 726f 6d20 6120 7061 6e64 6173 2044   from a pandas D
-00009050: 6174 6146 7261 6d65 2e0a 0a20 2020 2020  ataFrame...     
-00009060: 2020 2054 6865 2070 616e 6461 7320 4461     The pandas Da
-00009070: 7461 4672 616d 6520 7769 6c6c 2062 6520  taFrame will be 
-00009080: 7065 7273 6973 7465 6420 6173 2061 2074  persisted as a t
-00009090: 656d 706f 7261 7279 2042 6967 5175 6572  emporary BigQuer
-000090a0: 7920 7461 626c 652c 2077 6869 6368 2063  y table, which c
-000090b0: 616e 2062 650a 2020 2020 2020 2020 6175  an be.        au
-000090c0: 746f 6d61 7469 6361 6c6c 7920 7265 6379  tomatically recy
-000090d0: 636c 6564 2061 6674 6572 2074 6865 2053  cled after the S
-000090e0: 6573 7369 6f6e 2069 7320 636c 6f73 6564  ession is closed
-000090f0: 2e0a 0a20 2020 2020 2020 202a 2a45 7861  ...        **Exa
-00009100: 6d70 6c65 733a 2a2a 0a0a 2020 2020 2020  mples:**..      
-00009110: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00009120: 2062 6967 6672 616d 6573 2e70 616e 6461   bigframes.panda
-00009130: 7320 6173 2062 7064 0a20 2020 2020 2020  s as bpd.       
-00009140: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-00009150: 7061 6e64 6173 2061 7320 7064 0a20 2020  pandas as pd.   
-00009160: 2020 2020 2020 2020 203e 3e3e 2062 7064           >>> bpd
-00009170: 2e6f 7074 696f 6e73 2e64 6973 706c 6179  .options.display
-00009180: 2e70 726f 6772 6573 735f 6261 7220 3d20  .progress_bar = 
-00009190: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
-000091a0: 2020 3e3e 3e20 6420 3d20 7b27 636f 6c31    >>> d = {'col1
-000091b0: 273a 205b 312c 2032 5d2c 2027 636f 6c32  ': [1, 2], 'col2
-000091c0: 273a 205b 332c 2034 5d7d 0a20 2020 2020  ': [3, 4]}.     
-000091d0: 2020 2020 2020 203e 3e3e 2070 616e 6461         >>> panda
-000091e0: 735f 6466 203d 2070 642e 4461 7461 4672  s_df = pd.DataFr
-000091f0: 616d 6528 6461 7461 3d64 290a 2020 2020  ame(data=d).    
-00009200: 2020 2020 2020 2020 3e3e 3e20 6466 203d          >>> df =
-00009210: 2062 7064 2e72 6561 645f 7061 6e64 6173   bpd.read_pandas
-00009220: 2870 616e 6461 735f 6466 290a 2020 2020  (pandas_df).    
-00009230: 2020 2020 2020 2020 3e3e 3e20 6466 0a20          >>> df. 
-00009240: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00009250: 6c31 2020 636f 6c32 0a20 2020 2020 2020  l1  col2.       
-00009260: 2020 2020 2030 2020 2020 2031 2020 2020       0     1    
-00009270: 2033 0a20 2020 2020 2020 2020 2020 2031   3.            1
-00009280: 2020 2020 2032 2020 2020 2034 0a20 2020       2     4.   
-00009290: 2020 2020 2020 2020 203c 424c 414e 4b4c           <BLANKL
-000092a0: 494e 453e 0a20 2020 2020 2020 2020 2020  INE>.           
-000092b0: 205b 3220 726f 7773 2078 2032 2063 6f6c   [2 rows x 2 col
-000092c0: 756d 6e73 5d0a 0a20 2020 2020 2020 2041  umns]..        A
-000092d0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000092e0: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-000092f0: 6520 2870 616e 6461 732e 4461 7461 4672  e (pandas.DataFr
-00009300: 616d 652c 2070 616e 6461 732e 5365 7269  ame, pandas.Seri
-00009310: 6573 2c20 6f72 2070 616e 6461 732e 496e  es, or pandas.In
-00009320: 6465 7829 3a0a 2020 2020 2020 2020 2020  dex):.          
-00009330: 2020 2020 2020 6120 7061 6e64 6173 2044        a pandas D
-00009340: 6174 6146 7261 6d65 2f53 6572 6965 732f  ataFrame/Series/
-00009350: 496e 6465 7820 6f62 6a65 6374 2074 6f20  Index object to 
-00009360: 6265 206c 6f61 6465 642e 0a0a 2020 2020  be loaded...    
-00009370: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00009380: 2020 2020 2020 2020 2041 6e20 6571 7569           An equi
-00009390: 7661 6c65 6e74 2062 6967 6672 616d 6573  valent bigframes
-000093a0: 2e70 616e 6461 732e 2844 6174 6146 7261  .pandas.(DataFra
-000093b0: 6d65 2f53 6572 6965 732f 496e 6465 7829  me/Series/Index)
-000093c0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
-000093d0: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
-000093e0: 7274 2062 6967 6672 616d 6573 2e73 6572  rt bigframes.ser
-000093f0: 6965 7320 6173 2073 6572 6965 730a 0a20  ies as series.. 
-00009400: 2020 2020 2020 2023 2054 7279 2074 6f20         # Try to 
-00009410: 6861 6e64 6c65 206e 6f6e 2d64 6174 6166  handle non-dataf
-00009420: 7261 6d65 2070 616e 6461 7320 6f62 6a65  rame pandas obje
-00009430: 6374 7320 6173 2077 656c 6c0a 2020 2020  cts as well.    
-00009440: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00009450: 6528 7061 6e64 6173 5f64 6174 6166 7261  e(pandas_datafra
-00009460: 6d65 2c20 7061 6e64 6173 2e53 6572 6965  me, pandas.Serie
-00009470: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00009480: 6266 5f64 6620 3d20 7365 6c66 2e5f 7265  bf_df = self._re
-00009490: 6164 5f70 616e 6461 7328 7061 6e64 6173  ad_pandas(pandas
-000094a0: 2e44 6174 6146 7261 6d65 2870 616e 6461  .DataFrame(panda
-000094b0: 735f 6461 7461 6672 616d 6529 2c20 2272  s_dataframe), "r
-000094c0: 6561 645f 7061 6e64 6173 2229 0a20 2020  ead_pandas").   
-000094d0: 2020 2020 2020 2020 2062 665f 7365 7269           bf_seri
-000094e0: 6573 203d 2074 7970 696e 672e 6361 7374  es = typing.cast
-000094f0: 2873 6572 6965 732e 5365 7269 6573 2c20  (series.Series, 
-00009500: 6266 5f64 665b 6266 5f64 662e 636f 6c75  bf_df[bf_df.colu
-00009510: 6d6e 735b 305d 5d29 0a20 2020 2020 2020  mns[0]]).       
-00009520: 2020 2020 2023 2077 7261 7070 696e 6720       # wrapping 
-00009530: 696e 746f 2064 6620 6361 6e20 7365 7420  into df can set 
-00009540: 6e61 6d65 2074 6f20 3020 736f 2072 6573  name to 0 so res
-00009550: 6574 2074 6f20 6f72 6967 696e 616c 206f  et to original o
-00009560: 626a 6563 7420 6e61 6d65 0a20 2020 2020  bject name.     
-00009570: 2020 2020 2020 2062 665f 7365 7269 6573         bf_series
-00009580: 2e6e 616d 6520 3d20 7061 6e64 6173 5f64  .name = pandas_d
-00009590: 6174 6166 7261 6d65 2e6e 616d 650a 2020  ataframe.name.  
-000095a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000095b0: 2062 665f 7365 7269 6573 0a20 2020 2020   bf_series.     
-000095c0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000095d0: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
-000095e0: 652c 2070 616e 6461 732e 496e 6465 7829  e, pandas.Index)
-000095f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009600: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
-00009610: 7061 6e64 6173 280a 2020 2020 2020 2020  pandas(.        
-00009620: 2020 2020 2020 2020 7061 6e64 6173 2e44          pandas.D
-00009630: 6174 6146 7261 6d65 2869 6e64 6578 3d70  ataFrame(index=p
-00009640: 616e 6461 735f 6461 7461 6672 616d 6529  andas_dataframe)
-00009650: 2c20 2272 6561 645f 7061 6e64 6173 220a  , "read_pandas".
-00009660: 2020 2020 2020 2020 2020 2020 292e 696e              ).in
-00009670: 6465 780a 2020 2020 2020 2020 6966 2069  dex.        if i
-00009680: 7369 6e73 7461 6e63 6528 7061 6e64 6173  sinstance(pandas
-00009690: 5f64 6174 6166 7261 6d65 2c20 7061 6e64  _dataframe, pand
-000096a0: 6173 2e44 6174 6146 7261 6d65 293a 0a20  as.DataFrame):. 
-000096b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000096c0: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
-000096d0: 6461 7328 7061 6e64 6173 5f64 6174 6166  das(pandas_dataf
-000096e0: 7261 6d65 2c20 2272 6561 645f 7061 6e64  rame, "read_pand
-000096f0: 6173 2229 0a20 2020 2020 2020 2065 6c73  as").        els
-00009700: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00009710: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00009720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009730: 2066 2272 6561 645f 7061 6e64 6173 2829   f"read_pandas()
-00009740: 2065 7870 6563 7473 2061 2070 616e 6461   expects a panda
-00009750: 732e 4461 7461 4672 616d 652c 2062 7574  s.DataFrame, but
-00009760: 2067 6f74 2061 207b 7479 7065 2870 616e   got a {type(pan
-00009770: 6461 735f 6461 7461 6672 616d 6529 7d22  das_dataframe)}"
-00009780: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00009790: 2020 2020 6465 6620 5f72 6561 645f 7061      def _read_pa
-000097a0: 6e64 6173 280a 2020 2020 2020 2020 7365  ndas(.        se
-000097b0: 6c66 2c20 7061 6e64 6173 5f64 6174 6166  lf, pandas_dataf
-000097c0: 7261 6d65 3a20 7061 6e64 6173 2e44 6174  rame: pandas.Dat
-000097d0: 6146 7261 6d65 2c20 6170 695f 6e61 6d65  aFrame, api_name
-000097e0: 3a20 7374 720a 2020 2020 2920 2d3e 2064  : str.    ) -> d
-000097f0: 6174 6166 7261 6d65 2e44 6174 6146 7261  ataframe.DataFra
-00009800: 6d65 3a0a 2020 2020 2020 2020 696d 706f  me:.        impo
-00009810: 7274 2062 6967 6672 616d 6573 2e64 6174  rt bigframes.dat
-00009820: 6166 7261 6d65 2061 7320 6461 7461 6672  aframe as datafr
-00009830: 616d 650a 0a20 2020 2020 2020 2069 6620  ame..        if 
-00009840: 6973 696e 7374 616e 6365 2870 616e 6461  isinstance(panda
-00009850: 735f 6461 7461 6672 616d 652c 2064 6174  s_dataframe, dat
-00009860: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
-00009870: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00009880: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00009890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098a0: 2022 7265 6164 5f70 616e 6461 7328 2920   "read_pandas() 
-000098b0: 6578 7065 6374 7320 6120 7061 6e64 6173  expects a pandas
-000098c0: 2e44 6174 6146 7261 6d65 2c20 6275 7420  .DataFrame, but 
-000098d0: 676f 7420 6120 220a 2020 2020 2020 2020  got a ".        
-000098e0: 2020 2020 2020 2020 2262 6967 6672 616d          "bigfram
-000098f0: 6573 2e70 616e 6461 732e 4461 7461 4672  es.pandas.DataFr
-00009900: 616d 652e 220a 2020 2020 2020 2020 2020  ame.".          
-00009910: 2020 290a 0a20 2020 2020 2020 2069 6e6c    )..        inl
-00009920: 696e 655f 6466 203d 2073 656c 662e 5f72  ine_df = self._r
-00009930: 6561 645f 7061 6e64 6173 5f69 6e6c 696e  ead_pandas_inlin
-00009940: 6528 7061 6e64 6173 5f64 6174 6166 7261  e(pandas_datafra
-00009950: 6d65 290a 2020 2020 2020 2020 6966 2069  me).        if i
-00009960: 6e6c 696e 655f 6466 2069 7320 6e6f 7420  nline_df is not 
-00009970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009980: 2020 7265 7475 726e 2069 6e6c 696e 655f    return inline_
-00009990: 6466 0a20 2020 2020 2020 2074 7279 3a0a  df.        try:.
-000099a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000099b0: 726e 2073 656c 662e 5f72 6561 645f 7061  rn self._read_pa
-000099c0: 6e64 6173 5f6c 6f61 645f 6a6f 6228 7061  ndas_load_job(pa
-000099d0: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
-000099e0: 6170 695f 6e61 6d65 290a 2020 2020 2020  api_name).      
-000099f0: 2020 6578 6365 7074 2070 612e 4172 726f    except pa.Arro
-00009a00: 7749 6e76 616c 6964 2061 7320 653a 0a20  wInvalid as e:. 
-00009a10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00009a20: 2070 612e 4172 726f 7749 6e76 616c 6964   pa.ArrowInvalid
-00009a30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00009a40: 2020 6622 436f 756c 6420 6e6f 7420 636f    f"Could not co
-00009a50: 6e76 6572 7420 7769 7468 2061 2042 6967  nvert with a Big
-00009a60: 5175 6572 7920 7479 7065 3a20 607b 657d  Query type: `{e}
-00009a70: 602e 2022 0a20 2020 2020 2020 2020 2020  `. ".           
-00009a80: 2029 2066 726f 6d20 650a 0a20 2020 2064   ) from e..    d
-00009a90: 6566 205f 7265 6164 5f70 616e 6461 735f  ef _read_pandas_
-00009aa0: 696e 6c69 6e65 280a 2020 2020 2020 2020  inline(.        
-00009ab0: 7365 6c66 2c20 7061 6e64 6173 5f64 6174  self, pandas_dat
-00009ac0: 6166 7261 6d65 3a20 7061 6e64 6173 2e44  aframe: pandas.D
-00009ad0: 6174 6146 7261 6d65 0a20 2020 2029 202d  ataFrame.    ) -
-00009ae0: 3e20 4f70 7469 6f6e 616c 5b64 6174 6166  > Optional[dataf
-00009af0: 7261 6d65 2e44 6174 6146 7261 6d65 5d3a  rame.DataFrame]:
-00009b00: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00009b10: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
-00009b20: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
-00009b30: 0a0a 2020 2020 2020 2020 6966 2070 616e  ..        if pan
-00009b40: 6461 735f 6461 7461 6672 616d 652e 6d65  das_dataframe.me
-00009b50: 6d6f 7279 5f75 7361 6765 2864 6565 703d  mory_usage(deep=
-00009b60: 5472 7565 292e 7375 6d28 2920 3e20 4d41  True).sum() > MA
-00009b70: 585f 494e 4c49 4e45 5f44 465f 4259 5445  X_INLINE_DF_BYTE
-00009b80: 533a 0a20 2020 2020 2020 2020 2020 2072  S:.            r
-00009b90: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00009ba0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00009bb0: 2020 2020 2069 6e6c 696e 655f 6466 203d       inline_df =
-00009bc0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
-00009bd0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
-00009be0: 2020 2020 2020 626c 6f63 6b73 2e42 6c6f        blocks.Blo
-00009bf0: 636b 2e66 726f 6d5f 6c6f 6361 6c28 7061  ck.from_local(pa
-00009c00: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
-00009c10: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
-00009c20: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
-00009c30: 7074 2070 612e 4172 726f 7749 6e76 616c  pt pa.ArrowInval
-00009c40: 6964 2061 7320 653a 0a20 2020 2020 2020  id as e:.       
-00009c50: 2020 2020 2072 6169 7365 2070 612e 4172       raise pa.Ar
-00009c60: 726f 7749 6e76 616c 6964 280a 2020 2020  rowInvalid(.    
-00009c70: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
-00009c80: 756c 6420 6e6f 7420 636f 6e76 6572 7420  uld not convert 
-00009c90: 7769 7468 2061 2042 6967 5175 6572 7920  with a BigQuery 
-00009ca0: 7479 7065 3a20 607b 657d 602e 2022 0a20  type: `{e}`. ". 
-00009cb0: 2020 2020 2020 2020 2020 2029 2066 726f             ) fro
-00009cc0: 6d20 650a 2020 2020 2020 2020 6578 6365  m e.        exce
-00009cd0: 7074 2056 616c 7565 4572 726f 723a 2020  pt ValueError:  
-00009ce0: 2320 5468 726f 776e 2062 7920 6962 6973  # Thrown by ibis
-00009cf0: 2066 6f72 2073 6f6d 6520 756e 6861 6e64   for some unhand
-00009d00: 6c65 6420 7479 7065 730a 2020 2020 2020  led types.      
-00009d10: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00009d20: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
-00009d30: 2070 612e 4172 726f 7754 7970 6545 7272   pa.ArrowTypeErr
-00009d40: 6f72 3a20 2023 2054 6872 6f77 6e20 6279  or:  # Thrown by
-00009d50: 2061 7272 6f77 2066 6f72 2074 7970 6573   arrow for types
-00009d60: 2077 6974 686f 7574 206d 6170 7069 6e67   without mapping
-00009d70: 2028 6765 6f29 2e0a 2020 2020 2020 2020   (geo)..        
-00009d80: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00009d90: 0a20 2020 2020 2020 2069 6e6c 696e 655f  .        inline_
-00009da0: 7479 7065 7320 3d20 696e 6c69 6e65 5f64  types = inline_d
-00009db0: 662e 5f62 6c6f 636b 2e65 7870 722e 7363  f._block.expr.sc
-00009dc0: 6865 6d61 2e64 7479 7065 730a 2020 2020  hema.dtypes.    
-00009dd0: 2020 2020 2320 4962 6973 2068 6173 2070      # Ibis has p
-00009de0: 726f 626c 656d 7320 6573 6361 7069 6e67  roblems escaping
-00009df0: 2062 7974 6573 206c 6974 6572 616c 732c   bytes literals,
-00009e00: 2077 6869 6368 2077 696c 6c20 6361 7573   which will caus
-00009e10: 6520 7379 6e74 6178 2065 7272 6f72 7320  e syntax errors 
-00009e20: 7365 7276 6572 2d73 6964 652e 0a20 2020  server-side..   
-00009e30: 2020 2020 2069 6620 616c 6c28 6474 7970       if all(dtyp
-00009e40: 6520 696e 2049 4e4c 494e 4142 4c45 5f44  e in INLINABLE_D
-00009e50: 5459 5045 5320 666f 7220 6474 7970 6520  TYPES for dtype 
-00009e60: 696e 2069 6e6c 696e 655f 7479 7065 7329  in inline_types)
-00009e70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009e80: 7475 726e 2069 6e6c 696e 655f 6466 0a20  turn inline_df. 
-00009e90: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00009ea0: 6e65 0a0a 2020 2020 6465 6620 5f72 6561  ne..    def _rea
-00009eb0: 645f 7061 6e64 6173 5f6c 6f61 645f 6a6f  d_pandas_load_jo
-00009ec0: 6228 0a20 2020 2020 2020 2073 656c 662c  b(.        self,
-00009ed0: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-00009ee0: 653a 2070 616e 6461 732e 4461 7461 4672  e: pandas.DataFr
-00009ef0: 616d 652c 2061 7069 5f6e 616d 653a 2073  ame, api_name: s
-00009f00: 7472 0a20 2020 2029 202d 3e20 6461 7461  tr.    ) -> data
-00009f10: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
-00009f20: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00009f30: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
-00009f40: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
-00009f50: 0a0a 2020 2020 2020 2020 636f 6c5f 696e  ..        col_in
-00009f60: 6465 7820 3d20 7061 6e64 6173 5f64 6174  dex = pandas_dat
-00009f70: 6166 7261 6d65 2e63 6f6c 756d 6e73 2e63  aframe.columns.c
-00009f80: 6f70 7928 290a 2020 2020 2020 2020 636f  opy().        co
-00009f90: 6c5f 6c61 6265 6c73 2c20 6964 785f 6c61  l_labels, idx_la
-00009fa0: 6265 6c73 203d 2028 0a20 2020 2020 2020  bels = (.       
-00009fb0: 2020 2020 2063 6f6c 5f69 6e64 6578 2e74       col_index.t
-00009fc0: 6f5f 6c69 7374 2829 2c0a 2020 2020 2020  o_list(),.      
-00009fd0: 2020 2020 2020 7061 6e64 6173 5f64 6174        pandas_dat
-00009fe0: 6166 7261 6d65 2e69 6e64 6578 2e6e 616d  aframe.index.nam
-00009ff0: 6573 2c0a 2020 2020 2020 2020 290a 2020  es,.        ).  
-0000a000: 2020 2020 2020 6e65 775f 636f 6c5f 6964        new_col_id
-0000a010: 732c 206e 6577 5f69 6478 5f69 6473 203d  s, new_idx_ids =
-0000a020: 2075 7469 6c73 2e67 6574 5f73 7461 6e64   utils.get_stand
-0000a030: 6172 6469 7a65 645f 6964 7328 0a20 2020  ardized_ids(.   
-0000a040: 2020 2020 2020 2020 2063 6f6c 5f6c 6162           col_lab
-0000a050: 656c 732c 0a20 2020 2020 2020 2020 2020  els,.           
-0000a060: 2069 6478 5f6c 6162 656c 732c 0a20 2020   idx_labels,.   
-0000a070: 2020 2020 2020 2020 2023 204c 6f61 6469           # Loadi
-0000a080: 6e67 2070 6172 7175 6574 2066 696c 6573  ng parquet files
-0000a090: 2069 6e74 6f20 4269 6751 7565 7279 2077   into BigQuery w
-0000a0a0: 6974 6820 7370 6563 6961 6c20 636f 6c75  ith special colu
-0000a0b0: 6d6e 206e 616d 6573 0a20 2020 2020 2020  mn names.       
-0000a0c0: 2020 2020 2023 2069 7320 6f6e 6c79 2073       # is only s
-0000a0d0: 7570 706f 7274 6564 2075 6e64 6572 2061  upported under a
-0000a0e0: 6e20 616c 6c6f 776c 6973 742e 0a20 2020  n allowlist..   
-0000a0f0: 2020 2020 2020 2020 2073 7472 6963 743d           strict=
-0000a100: 5472 7565 2c0a 2020 2020 2020 2020 290a  True,.        ).
-0000a110: 0a20 2020 2020 2020 2023 2041 6464 206f  .        # Add o
-0000a120: 7264 6572 2063 6f6c 756d 6e20 746f 2070  rder column to p
-0000a130: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
-0000a140: 746f 2070 7265 7365 7276 6520 6f72 6465  to preserve orde
-0000a150: 7220 696e 2042 6967 5175 6572 790a 2020  r in BigQuery.  
-0000a160: 2020 2020 2020 6f72 6465 7269 6e67 5f63        ordering_c
-0000a170: 6f6c 203d 2022 726f 7769 6422 0a20 2020  ol = "rowid".   
-0000a180: 2020 2020 2063 6f6c 756d 6e73 203d 2066       columns = f
-0000a190: 726f 7a65 6e73 6574 2863 6f6c 5f6c 6162  rozenset(col_lab
-0000a1a0: 656c 7320 2b20 6964 785f 6c61 6265 6c73  els + idx_labels
-0000a1b0: 290a 2020 2020 2020 2020 7375 6666 6978  ).        suffix
-0000a1c0: 203d 2032 0a20 2020 2020 2020 2077 6869   = 2.        whi
-0000a1d0: 6c65 206f 7264 6572 696e 675f 636f 6c20  le ordering_col 
-0000a1e0: 696e 2063 6f6c 756d 6e73 3a0a 2020 2020  in columns:.    
-0000a1f0: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
-0000a200: 5f63 6f6c 203d 2066 2272 6f77 6964 5f7b  _col = f"rowid_{
-0000a210: 7375 6666 6978 7d22 0a20 2020 2020 2020  suffix}".       
-0000a220: 2020 2020 2073 7566 6669 7820 2b3d 2031       suffix += 1
-0000a230: 0a0a 2020 2020 2020 2020 7061 6e64 6173  ..        pandas
-0000a240: 5f64 6174 6166 7261 6d65 5f63 6f70 7920  _dataframe_copy 
-0000a250: 3d20 7061 6e64 6173 5f64 6174 6166 7261  = pandas_datafra
-0000a260: 6d65 2e63 6f70 7928 290a 2020 2020 2020  me.copy().      
-0000a270: 2020 7061 6e64 6173 5f64 6174 6166 7261    pandas_datafra
-0000a280: 6d65 5f63 6f70 792e 696e 6465 782e 6e61  me_copy.index.na
-0000a290: 6d65 7320 3d20 6e65 775f 6964 785f 6964  mes = new_idx_id
-0000a2a0: 730a 2020 2020 2020 2020 7061 6e64 6173  s.        pandas
-0000a2b0: 5f64 6174 6166 7261 6d65 5f63 6f70 792e  _dataframe_copy.
-0000a2c0: 636f 6c75 6d6e 7320 3d20 7061 6e64 6173  columns = pandas
-0000a2d0: 2e49 6e64 6578 286e 6577 5f63 6f6c 5f69  .Index(new_col_i
-0000a2e0: 6473 290a 2020 2020 2020 2020 7061 6e64  ds).        pand
-0000a2f0: 6173 5f64 6174 6166 7261 6d65 5f63 6f70  as_dataframe_cop
-0000a300: 795b 6f72 6465 7269 6e67 5f63 6f6c 5d20  y[ordering_col] 
-0000a310: 3d20 6e70 2e61 7261 6e67 6528 7061 6e64  = np.arange(pand
-0000a320: 6173 5f64 6174 6166 7261 6d65 5f63 6f70  as_dataframe_cop
-0000a330: 792e 7368 6170 655b 305d 290a 0a20 2020  y.shape[0])..   
-0000a340: 2020 2020 206a 6f62 5f63 6f6e 6669 6720       job_config 
-0000a350: 3d20 7365 6c66 2e5f 7072 6570 6172 655f  = self._prepare_
-0000a360: 6c6f 6164 5f6a 6f62 5f63 6f6e 6669 6728  load_job_config(
-0000a370: 290a 0a20 2020 2020 2020 2023 2053 7065  )..        # Spe
-0000a380: 6369 6679 2074 6865 2064 6174 6574 696d  cify the datetim
-0000a390: 6520 6474 7970 6573 2c20 7768 6963 6820  e dtypes, which 
-0000a3a0: 6973 2061 7574 6f2d 6465 7465 6374 6564  is auto-detected
-0000a3b0: 2061 7320 7469 6d65 7374 616d 7020 7479   as timestamp ty
-0000a3c0: 7065 732e 0a20 2020 2020 2020 2073 6368  pes..        sch
-0000a3d0: 656d 613a 206c 6973 745b 6269 6771 7565  ema: list[bigque
-0000a3e0: 7279 2e53 6368 656d 6146 6965 6c64 5d20  ry.SchemaField] 
-0000a3f0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-0000a400: 2063 6f6c 756d 6e2c 2064 7479 7065 2069   column, dtype i
-0000a410: 6e20 7a69 7028 6e65 775f 636f 6c5f 6964  n zip(new_col_id
-0000a420: 732c 2070 616e 6461 735f 6461 7461 6672  s, pandas_datafr
-0000a430: 616d 652e 6474 7970 6573 293a 0a20 2020  ame.dtypes):.   
-0000a440: 2020 2020 2020 2020 2069 6620 6474 7970           if dtyp
-0000a450: 6520 3d3d 2022 7469 6d65 7374 616d 705b  e == "timestamp[
-0000a460: 7573 5d5b 7079 6172 726f 775d 223a 0a20  us][pyarrow]":. 
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a480: 6368 656d 612e 6170 7065 6e64 280a 2020  chema.append(.  
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 6269 6771 7565 7279 2e53 6368 656d    bigquery.Schem
-0000a4b0: 6146 6965 6c64 2863 6f6c 756d 6e2c 2062  aField(column, b
-0000a4c0: 6967 7175 6572 792e 656e 756d 732e 5371  igquery.enums.Sq
-0000a4d0: 6c54 7970 654e 616d 6573 2e44 4154 4554  lTypeNames.DATET
-0000a4e0: 494d 4529 0a20 2020 2020 2020 2020 2020  IME).           
-0000a4f0: 2020 2020 2029 0a20 2020 2020 2020 206a       ).        j
-0000a500: 6f62 5f63 6f6e 6669 672e 7363 6865 6d61  ob_config.schema
-0000a510: 203d 2073 6368 656d 610a 0a20 2020 2020   = schema..     
-0000a520: 2020 2023 2043 6c75 7374 6572 696e 6720     # Clustering 
-0000a530: 7072 6f62 6162 6c79 206e 6f74 206e 6565  probably not nee
-0000a540: 6465 6420 616e 7977 6179 7320 6173 2070  ded anyways as p
-0000a550: 616e 6461 7320 7461 626c 6573 2061 7265  andas tables are
-0000a560: 2073 6d61 6c6c 0a20 2020 2020 2020 2063   small.        c
-0000a570: 6c75 7374 6572 5f63 6f6c 7320 3d20 5b6f  luster_cols = [o
-0000a580: 7264 6572 696e 675f 636f 6c5d 0a20 2020  rdering_col].   
-0000a590: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
-0000a5a0: 636c 7573 7465 7269 6e67 5f66 6965 6c64  clustering_field
-0000a5b0: 7320 3d20 636c 7573 7465 725f 636f 6c73  s = cluster_cols
-0000a5c0: 0a0a 2020 2020 2020 2020 6a6f 625f 636f  ..        job_co
-0000a5d0: 6e66 6967 2e6c 6162 656c 7320 3d20 7b22  nfig.labels = {"
-0000a5e0: 6269 6766 7261 6d65 732d 6170 6922 3a20  bigframes-api": 
-0000a5f0: 6170 695f 6e61 6d65 7d0a 0a20 2020 2020  api_name}..     
-0000a600: 2020 206c 6f61 645f 7461 626c 655f 6465     load_table_de
-0000a610: 7374 696e 6174 696f 6e20 3d20 6269 6766  stination = bigf
-0000a620: 7261 6d65 735f 696f 2e72 616e 646f 6d5f  rames_io.random_
-0000a630: 7461 626c 6528 7365 6c66 2e5f 616e 6f6e  table(self._anon
-0000a640: 796d 6f75 735f 6461 7461 7365 7429 0a20  ymous_dataset). 
-0000a650: 2020 2020 2020 206c 6f61 645f 6a6f 6220         load_job 
-0000a660: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
-0000a670: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
-0000a680: 6461 7461 6672 616d 6528 0a20 2020 2020  dataframe(.     
-0000a690: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
-0000a6a0: 7461 6672 616d 655f 636f 7079 2c0a 2020  taframe_copy,.  
-0000a6b0: 2020 2020 2020 2020 2020 6c6f 6164 5f74            load_t
-0000a6c0: 6162 6c65 5f64 6573 7469 6e61 7469 6f6e  able_destination
-0000a6d0: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
-0000a6e0: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
-0000a6f0: 6669 672c 0a20 2020 2020 2020 2029 0a20  fig,.        ). 
-0000a700: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
-0000a710: 7274 5f67 656e 6572 6963 5f6a 6f62 286c  rt_generic_job(l
-0000a720: 6f61 645f 6a6f 6229 0a0a 2020 2020 2020  oad_job)..      
-0000a730: 2020 6f72 6465 7269 6e67 203d 206f 7264    ordering = ord
-0000a740: 6572 2e45 7870 7265 7373 696f 6e4f 7264  er.ExpressionOrd
-0000a750: 6572 696e 6728 0a20 2020 2020 2020 2020  ering(.         
-0000a760: 2020 206f 7264 6572 696e 675f 7661 6c75     ordering_valu
-0000a770: 655f 636f 6c75 6d6e 733d 7475 706c 6528  e_columns=tuple(
-0000a780: 5b6f 7264 6572 2e61 7363 656e 6469 6e67  [order.ascending
-0000a790: 5f6f 7665 7228 6f72 6465 7269 6e67 5f63  _over(ordering_c
-0000a7a0: 6f6c 295d 292c 0a20 2020 2020 2020 2020  ol)]),.         
-0000a7b0: 2020 2074 6f74 616c 5f6f 7264 6572 696e     total_orderin
-0000a7c0: 675f 636f 6c75 6d6e 733d 6672 6f7a 656e  g_columns=frozen
-0000a7d0: 7365 7428 5b6f 7264 6572 696e 675f 636f  set([ordering_co
-0000a7e0: 6c5d 292c 0a20 2020 2020 2020 2020 2020  l]),.           
-0000a7f0: 2069 6e74 6567 6572 5f65 6e63 6f64 696e   integer_encodin
-0000a800: 673d 496e 7465 6765 7245 6e63 6f64 696e  g=IntegerEncodin
-0000a810: 6728 5472 7565 2c20 6973 5f73 6571 7565  g(True, is_seque
-0000a820: 6e74 6961 6c3d 5472 7565 292c 0a20 2020  ntial=True),.   
-0000a830: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
-0000a840: 6162 6c65 5f65 7870 7265 7373 696f 6e20  able_expression 
-0000a850: 3d20 7365 6c66 2e69 6269 735f 636c 6965  = self.ibis_clie
-0000a860: 6e74 2e74 6162 6c65 2820 2023 2074 7970  nt.table(  # typ
-0000a870: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-0000a880: 2020 2020 2020 6c6f 6164 5f74 6162 6c65        load_table
-0000a890: 5f64 6573 7469 6e61 7469 6f6e 2e74 6162  _destination.tab
-0000a8a0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
-0000a8b0: 2020 2073 6368 656d 613d 6c6f 6164 5f74     schema=load_t
-0000a8c0: 6162 6c65 5f64 6573 7469 6e61 7469 6f6e  able_destination
-0000a8d0: 2e64 6174 6173 6574 5f69 642c 0a20 2020  .dataset_id,.   
-0000a8e0: 2020 2020 2020 2020 2064 6174 6162 6173           databas
-0000a8f0: 653d 6c6f 6164 5f74 6162 6c65 5f64 6573  e=load_table_des
-0000a900: 7469 6e61 7469 6f6e 2e70 726f 6a65 6374  tination.project
-0000a910: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000a920: 2020 2020 2023 2062 2f32 3937 3539 3031       # b/2975901
-0000a930: 3738 2050 6f74 656e 7469 616c 6c79 2061  78 Potentially a
-0000a940: 2062 7567 2069 6e20 6271 636c 6965 6e74   bug in bqclient
-0000a950: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
-0000a960: 5f64 6174 6166 7261 6d65 2829 2c20 7468  _dataframe(), th
-0000a970: 6174 206f 6e6c 7920 7768 656e 2074 6865  at only when the
-0000a980: 2044 4620 6973 2065 6d70 7479 2c20 7468   DF is empty, th
-0000a990: 6520 696e 6465 7820 636f 6c75 6d6e 7320  e index columns 
-0000a9a0: 6469 7361 7070 6561 7220 696e 2074 6162  disappear in tab
-0000a9b0: 6c65 5f65 7870 7265 7373 696f 6e2e 0a20  le_expression.. 
-0000a9c0: 2020 2020 2020 2069 6620 616e 7928 0a20         if any(. 
-0000a9d0: 2020 2020 2020 2020 2020 205b 6e65 775f             [new_
-0000a9e0: 6964 785f 6964 206e 6f74 2069 6e20 7461  idx_id not in ta
-0000a9f0: 626c 655f 6578 7072 6573 7369 6f6e 2e63  ble_expression.c
-0000aa00: 6f6c 756d 6e73 2066 6f72 206e 6577 5f69  olumns for new_i
-0000aa10: 6478 5f69 6420 696e 206e 6577 5f69 6478  dx_id in new_idx
-0000aa20: 5f69 6473 5d0a 2020 2020 2020 2020 293a  _ids].        ):
-0000aa30: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0000aa40: 5f69 6478 5f69 6473 2c20 6964 785f 6c61  _idx_ids, idx_la
-0000aa50: 6265 6c73 203d 205b 5d2c 205b 5d0a 0a20  bels = [], [].. 
-0000aa60: 2020 2020 2020 2063 6f6c 756d 6e5f 7661         column_va
-0000aa70: 6c75 6573 203d 205b 0a20 2020 2020 2020  lues = [.       
-0000aa80: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-0000aa90: 7373 696f 6e5b 636f 6c5d 0a20 2020 2020  ssion[col].     
-0000aaa0: 2020 2020 2020 2066 6f72 2063 6f6c 2069         for col i
-0000aab0: 6e20 7461 626c 655f 6578 7072 6573 7369  n table_expressi
-0000aac0: 6f6e 2e63 6f6c 756d 6e73 0a20 2020 2020  on.columns.     
-0000aad0: 2020 2020 2020 2069 6620 636f 6c20 213d         if col !=
-0000aae0: 206f 7264 6572 696e 675f 636f 6c0a 2020   ordering_col.  
-0000aaf0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0000ab00: 6172 7261 795f 7661 6c75 6520 3d20 636f  array_value = co
-0000ab10: 7265 2e41 7272 6179 5661 6c75 652e 6672  re.ArrayValue.fr
-0000ab20: 6f6d 5f69 6269 7328 0a20 2020 2020 2020  om_ibis(.       
-0000ab30: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000ab40: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
-0000ab50: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
-0000ab60: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
-0000ab70: 756d 6e5f 7661 6c75 6573 2c0a 2020 2020  umn_values,.    
-0000ab80: 2020 2020 2020 2020 6869 6464 656e 5f6f          hidden_o
-0000ab90: 7264 6572 696e 675f 636f 6c75 6d6e 733d  rdering_columns=
-0000aba0: 5b74 6162 6c65 5f65 7870 7265 7373 696f  [table_expressio
-0000abb0: 6e5b 6f72 6465 7269 6e67 5f63 6f6c 5d5d  n[ordering_col]]
-0000abc0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-0000abd0: 6465 7269 6e67 3d6f 7264 6572 696e 672c  dering=ordering,
-0000abe0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000abf0: 2020 2020 626c 6f63 6b20 3d20 626c 6f63      block = bloc
-0000ac00: 6b73 2e42 6c6f 636b 280a 2020 2020 2020  ks.Block(.      
-0000ac10: 2020 2020 2020 6172 7261 795f 7661 6c75        array_valu
-0000ac20: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
-0000ac30: 6e64 6578 5f63 6f6c 756d 6e73 3d6e 6577  ndex_columns=new
-0000ac40: 5f69 6478 5f69 6473 2c0a 2020 2020 2020  _idx_ids,.      
-0000ac50: 2020 2020 2020 636f 6c75 6d6e 5f6c 6162        column_lab
-0000ac60: 656c 733d 636f 6c5f 696e 6465 782c 0a20  els=col_index,. 
-0000ac70: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-0000ac80: 5f6c 6162 656c 733d 6964 785f 6c61 6265  _labels=idx_labe
-0000ac90: 6c73 2c0a 2020 2020 2020 2020 290a 2020  ls,.        ).  
-0000aca0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
-0000acb0: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
-0000acc0: 2862 6c6f 636b 290a 0a20 2020 2064 6566  (block)..    def
-0000acd0: 2072 6561 645f 6373 7628 0a20 2020 2020   read_csv(.     
-0000ace0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000acf0: 2066 696c 6570 6174 685f 6f72 5f62 7566   filepath_or_buf
-0000ad00: 6665 723a 2073 7472 207c 2049 4f5b 2262  fer: str | IO["b
-0000ad10: 7974 6573 225d 2c0a 2020 2020 2020 2020  ytes"],.        
-0000ad20: 2a2c 0a20 2020 2020 2020 2073 6570 3a20  *,.        sep: 
-0000ad30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000ad40: 222c 222c 0a20 2020 2020 2020 2068 6561  ",",.        hea
-0000ad50: 6465 723a 204f 7074 696f 6e61 6c5b 696e  der: Optional[in
-0000ad60: 745d 203d 2030 2c0a 2020 2020 2020 2020  t] = 0,.        
-0000ad70: 6e61 6d65 733a 204f 7074 696f 6e61 6c5b  names: Optional[
-0000ad80: 0a20 2020 2020 2020 2020 2020 2055 6e69  .            Uni
-0000ad90: 6f6e 5b4d 7574 6162 6c65 5365 7175 656e  on[MutableSequen
-0000ada0: 6365 5b41 6e79 5d2c 206e 702e 6e64 6172  ce[Any], np.ndar
-0000adb0: 7261 795b 416e 792c 2041 6e79 5d2c 2054  ray[Any, Any], T
-0000adc0: 7570 6c65 5b41 6e79 2c20 2e2e 2e5d 2c20  uple[Any, ...], 
-0000add0: 7261 6e67 655d 0a20 2020 2020 2020 205d  range].        ]
-0000ade0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000adf0: 2069 6e64 6578 5f63 6f6c 3a20 4f70 7469   index_col: Opti
-0000ae00: 6f6e 616c 5b0a 2020 2020 2020 2020 2020  onal[.          
-0000ae10: 2020 556e 696f 6e5b 696e 742c 2073 7472    Union[int, str
-0000ae20: 2c20 5365 7175 656e 6365 5b55 6e69 6f6e  , Sequence[Union
-0000ae30: 5b73 7472 2c20 696e 745d 5d2c 204c 6974  [str, int]], Lit
-0000ae40: 6572 616c 5b46 616c 7365 5d5d 0a20 2020  eral[False]].   
-0000ae50: 2020 2020 205d 203d 204e 6f6e 652c 0a20       ] = None,. 
-0000ae60: 2020 2020 2020 2075 7365 636f 6c73 3a20         usecols: 
-0000ae70: 4f70 7469 6f6e 616c 5b0a 2020 2020 2020  Optional[.      
-0000ae80: 2020 2020 2020 556e 696f 6e5b 0a20 2020        Union[.   
-0000ae90: 2020 2020 2020 2020 2020 2020 204d 7574               Mut
-0000aea0: 6162 6c65 5365 7175 656e 6365 5b73 7472  ableSequence[str
-0000aeb0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000aec0: 2020 2054 7570 6c65 5b73 7472 2c20 2e2e     Tuple[str, ..
-0000aed0: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-0000aee0: 2020 2020 5365 7175 656e 6365 5b69 6e74      Sequence[int
-0000aef0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000af00: 2020 2070 616e 6461 732e 5365 7269 6573     pandas.Series
-0000af10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000af20: 2020 7061 6e64 6173 2e49 6e64 6578 2c0a    pandas.Index,.
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af40: 6e70 2e6e 6461 7272 6179 5b41 6e79 2c20  np.ndarray[Any, 
-0000af50: 416e 795d 2c0a 2020 2020 2020 2020 2020  Any],.          
-0000af60: 2020 2020 2020 4361 6c6c 6162 6c65 5b5b        Callable[[
-0000af70: 416e 795d 2c20 626f 6f6c 5d2c 0a20 2020  Any], bool],.   
-0000af80: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-0000af90: 2020 205d 203d 204e 6f6e 652c 0a20 2020     ] = None,.   
-0000afa0: 2020 2020 2064 7479 7065 3a20 4f70 7469       dtype: Opti
-0000afb0: 6f6e 616c 5b44 6963 745d 203d 204e 6f6e  onal[Dict] = Non
-0000afc0: 652c 0a20 2020 2020 2020 2065 6e67 696e  e,.        engin
-0000afd0: 653a 204f 7074 696f 6e61 6c5b 0a20 2020  e: Optional[.   
-0000afe0: 2020 2020 2020 2020 204c 6974 6572 616c           Literal
-0000aff0: 5b22 6322 2c20 2270 7974 686f 6e22 2c20  ["c", "python", 
-0000b000: 2270 7961 7272 6f77 222c 2022 7079 7468  "pyarrow", "pyth
-0000b010: 6f6e 2d66 7766 222c 2022 6269 6771 7565  on-fwf", "bigque
-0000b020: 7279 225d 0a20 2020 2020 2020 205d 203d  ry"].        ] =
-0000b030: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-0000b040: 6e63 6f64 696e 673a 204f 7074 696f 6e61  ncoding: Optiona
-0000b050: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000b060: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-0000b070: 0a20 2020 2029 202d 3e20 6461 7461 6672  .    ) -> datafr
-0000b080: 616d 652e 4461 7461 4672 616d 653a 0a20  ame.DataFrame:. 
-0000b090: 2020 2020 2020 2074 6162 6c65 203d 2062         table = b
-0000b0a0: 6967 6672 616d 6573 5f69 6f2e 7261 6e64  igframes_io.rand
-0000b0b0: 6f6d 5f74 6162 6c65 2873 656c 662e 5f61  om_table(self._a
-0000b0c0: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
-0000b0d0: 290a 0a20 2020 2020 2020 2069 6620 656e  )..        if en
-0000b0e0: 6769 6e65 2069 7320 6e6f 7420 4e6f 6e65  gine is not None
-0000b0f0: 2061 6e64 2065 6e67 696e 6520 3d3d 2022   and engine == "
-0000b100: 6269 6771 7565 7279 223a 0a20 2020 2020  bigquery":.     
-0000b110: 2020 2020 2020 2069 6620 616e 7928 7061         if any(pa
-0000b120: 7261 6d20 6973 206e 6f74 204e 6f6e 6520  ram is not None 
-0000b130: 666f 7220 7061 7261 6d20 696e 2028 6474  for param in (dt
-0000b140: 7970 652c 206e 616d 6573 2929 3a0a 2020  ype, names)):.  
-0000b150: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-0000b160: 745f 7375 7070 6f72 7465 6420 3d20 2822  t_supported = ("
-0000b170: 6474 7970 6522 2c20 226e 616d 6573 2229  dtype", "names")
-0000b180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b190: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000b1a0: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 6622 4269 6751 7565 7279 2065 6e67 696e  f"BigQuery engin
-0000b1d0: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
-0000b1e0: 7274 2074 6865 7365 2061 7267 756d 656e  rt these argumen
-0000b1f0: 7473 3a20 7b6e 6f74 5f73 7570 706f 7274  ts: {not_support
-0000b200: 6564 7d2e 2022 0a20 2020 2020 2020 2020  ed}. ".         
-0000b210: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
-0000b220: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
-0000b230: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
-0000b240: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000b250: 2020 2020 2020 2069 6620 696e 6465 785f         if index_
-0000b260: 636f 6c20 6973 206e 6f74 204e 6f6e 6520  col is not None 
-0000b270: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-0000b280: 2020 2020 2020 6e6f 7420 696e 6465 785f        not index_
-0000b290: 636f 6c20 6f72 206e 6f74 2069 7369 6e73  col or not isins
-0000b2a0: 7461 6e63 6528 696e 6465 785f 636f 6c2c  tance(index_col,
-0000b2b0: 2073 7472 290a 2020 2020 2020 2020 2020   str).          
-0000b2c0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000b2d0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-0000b2e0: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
-0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b300: 2020 2020 2242 6967 5175 6572 7920 656e      "BigQuery en
-0000b310: 6769 6e65 206f 6e6c 7920 7375 7070 6f72  gine only suppor
-0000b320: 7473 2061 2073 696e 676c 6520 636f 6c75  ts a single colu
-0000b330: 6d6e 206e 616d 6520 666f 7220 6069 6e64  mn name for `ind
-0000b340: 6578 5f63 6f6c 602e 2022 0a20 2020 2020  ex_col`. ".     
-0000b350: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000b360: 227b 636f 6e73 7461 6e74 732e 4645 4544  "{constants.FEED
-0000b370: 4241 434b 5f4c 494e 4b7d 220a 2020 2020  BACK_LINK}".    
-0000b380: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000b390: 2020 2020 2020 2020 2020 2023 204e 6f6e             # Non
-0000b3a0: 6520 7661 6c75 6520 666f 7220 696e 6465  e value for inde
-0000b3b0: 785f 636f 6c20 6361 6e6e 6f74 2062 6520  x_col cannot be 
-0000b3c0: 7061 7373 6564 2074 6f20 7265 6164 5f67  passed to read_g
-0000b3d0: 6271 0a20 2020 2020 2020 2020 2020 2069  bq.            i
-0000b3e0: 6620 696e 6465 785f 636f 6c20 6973 204e  f index_col is N
-0000b3f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b400: 2020 2020 2069 6e64 6578 5f63 6f6c 203d       index_col =
-0000b410: 2028 290a 0a20 2020 2020 2020 2020 2020   ()..           
-0000b420: 2023 2075 7365 636f 6c73 2073 686f 756c   # usecols shoul
-0000b430: 6420 6f6e 6c79 2062 6520 616e 2069 7465  d only be an ite
-0000b440: 7261 626c 6520 6f66 2073 7472 696e 6773  rable of strings
-0000b450: 2028 636f 6c75 6d6e 206e 616d 6573 2920   (column names) 
-0000b460: 666f 7220 7573 6520 6173 2063 6f6c 756d  for use as colum
-0000b470: 6e73 2069 6e20 7265 6164 5f67 6271 2e0a  ns in read_gbq..
-0000b480: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0000b490: 6d6e 733a 2054 7570 6c65 5b41 6e79 2c20  mns: Tuple[Any, 
-0000b4a0: 2e2e 2e5d 203d 2074 7570 6c65 2829 0a20  ...] = tuple(). 
-0000b4b0: 2020 2020 2020 2020 2020 2069 6620 7573             if us
-0000b4c0: 6563 6f6c 7320 6973 206e 6f74 204e 6f6e  ecols is not Non
-0000b4d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000b4e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000b4f0: 2875 7365 636f 6c73 2c20 4974 6572 6162  (usecols, Iterab
-0000b500: 6c65 2920 616e 6420 616c 6c28 0a20 2020  le) and all(.   
-0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b520: 2069 7369 6e73 7461 6e63 6528 636f 6c2c   isinstance(col,
-0000b530: 2073 7472 2920 666f 7220 636f 6c20 696e   str) for col in
-0000b540: 2075 7365 636f 6c73 0a20 2020 2020 2020   usecols.       
-0000b550: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b570: 636f 6c75 6d6e 7320 3d20 7475 706c 6528  columns = tuple(
-0000b580: 636f 6c20 666f 7220 636f 6c20 696e 2075  col for col in u
-0000b590: 7365 636f 6c73 290a 2020 2020 2020 2020  secols).        
-0000b5a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000b5d0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5f0: 2020 2020 2022 4269 6751 7565 7279 2065       "BigQuery e
-0000b600: 6e67 696e 6520 6f6e 6c79 2073 7570 706f  ngine only suppo
-0000b610: 7274 7320 616e 2069 7465 7261 626c 6520  rts an iterable 
-0000b620: 6f66 2073 7472 696e 6773 2066 6f72 2060  of strings for `
-0000b630: 7573 6563 6f6c 7360 2e20 220a 2020 2020  usecols`. ".    
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2020 6622 7b63 6f6e 7374 616e 7473      f"{constants
-0000b660: 2e46 4545 4442 4143 4b5f 4c49 4e4b 7d22  .FEEDBACK_LINK}"
-0000b670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b680: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b690: 2020 2020 6966 2065 6e63 6f64 696e 6720      if encoding 
-0000b6a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000b6b0: 656e 636f 6469 6e67 206e 6f74 2069 6e20  encoding not in 
-0000b6c0: 5f56 414c 4944 5f45 4e43 4f44 494e 4753  _VALID_ENCODINGS
-0000b6d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b6e0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000b6f0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 2066 2242 6967 5175 6572 7920 656e 6769   f"BigQuery engi
-0000b720: 6e65 206f 6e6c 7920 7375 7070 6f72 7473  ne only supports
-0000b730: 2074 6865 2066 6f6c 6c6f 7769 6e67 2065   the following e
-0000b740: 6e63 6f64 696e 6773 3a20 7b5f 5641 4c49  ncodings: {_VALI
-0000b750: 445f 454e 434f 4449 4e47 537d 2e20 220a  D_ENCODINGS}. ".
-0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b770: 2020 2020 6622 7b63 6f6e 7374 616e 7473      f"{constants
-0000b780: 2e46 4545 4442 4143 4b5f 4c49 4e4b 7d22  .FEEDBACK_LINK}"
-0000b790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7a0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000b7b0: 6a6f 625f 636f 6e66 6967 203d 2073 656c  job_config = sel
-0000b7c0: 662e 5f70 7265 7061 7265 5f6c 6f61 645f  f._prepare_load_
-0000b7d0: 6a6f 625f 636f 6e66 6967 2829 0a20 2020  job_config().   
-0000b7e0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000b7f0: 6669 672e 6372 6561 7465 5f64 6973 706f  fig.create_dispo
-0000b800: 7369 7469 6f6e 203d 2062 6967 7175 6572  sition = bigquer
-0000b810: 792e 4372 6561 7465 4469 7370 6f73 6974  y.CreateDisposit
-0000b820: 696f 6e2e 4352 4541 5445 5f49 465f 4e45  ion.CREATE_IF_NE
-0000b830: 4544 4544 0a20 2020 2020 2020 2020 2020  EDED.           
-0000b840: 206a 6f62 5f63 6f6e 6669 672e 736f 7572   job_config.sour
-0000b850: 6365 5f66 6f72 6d61 7420 3d20 6269 6771  ce_format = bigq
-0000b860: 7565 7279 2e53 6f75 7263 6546 6f72 6d61  uery.SourceForma
-0000b870: 742e 4353 560a 2020 2020 2020 2020 2020  t.CSV.          
-0000b880: 2020 6a6f 625f 636f 6e66 6967 2e77 7269    job_config.wri
-0000b890: 7465 5f64 6973 706f 7369 7469 6f6e 203d  te_disposition =
-0000b8a0: 2062 6967 7175 6572 792e 5772 6974 6544   bigquery.WriteD
-0000b8b0: 6973 706f 7369 7469 6f6e 2e57 5249 5445  isposition.WRITE
-0000b8c0: 5f45 4d50 5459 0a20 2020 2020 2020 2020  _EMPTY.         
-0000b8d0: 2020 206a 6f62 5f63 6f6e 6669 672e 6175     job_config.au
-0000b8e0: 746f 6465 7465 6374 203d 2054 7275 650a  todetect = True.
-0000b8f0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000b900: 636f 6e66 6967 2e66 6965 6c64 5f64 656c  config.field_del
-0000b910: 696d 6974 6572 203d 2073 6570 0a20 2020  imiter = sep.   
-0000b920: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000b930: 6669 672e 656e 636f 6469 6e67 203d 2065  fig.encoding = e
-0000b940: 6e63 6f64 696e 670a 2020 2020 2020 2020  ncoding.        
-0000b950: 2020 2020 6a6f 625f 636f 6e66 6967 2e6c      job_config.l
-0000b960: 6162 656c 7320 3d20 7b22 6269 6766 7261  abels = {"bigfra
-0000b970: 6d65 732d 6170 6922 3a20 2272 6561 645f  mes-api": "read_
-0000b980: 6373 7622 7d0a 0a20 2020 2020 2020 2020  csv"}..         
-0000b990: 2020 2023 2057 6520 7761 6e74 2074 6f20     # We want to 
-0000b9a0: 6d61 7463 6820 7061 6e64 6173 2062 6568  match pandas beh
-0000b9b0: 6176 696f 722e 2049 6620 6865 6164 6572  avior. If header
-0000b9c0: 2069 7320 302c 206e 6f20 726f 7773 2073   is 0, no rows s
-0000b9d0: 686f 756c 6420 6265 2073 6b69 7070 6564  hould be skipped
-0000b9e0: 2c20 736f 2077 650a 2020 2020 2020 2020  , so we.        
-0000b9f0: 2020 2020 2320 646f 206e 6f74 206e 6565      # do not nee
-0000ba00: 6420 746f 2073 6574 2060 736b 6970 5f6c  d to set `skip_l
-0000ba10: 6561 6469 6e67 5f72 6f77 7360 2e20 4966  eading_rows`. If
-0000ba20: 2068 6561 6465 7220 6973 204e 6f6e 652c   header is None,
-0000ba30: 2074 6865 6e20 7468 6572 6520 6973 206e   then there is n
-0000ba40: 6f20 6865 6164 6572 2e0a 2020 2020 2020  o header..      
-0000ba50: 2020 2020 2020 2320 5365 7474 696e 6720        # Setting 
-0000ba60: 736b 6970 5f6c 6561 6469 6e67 5f72 6f77  skip_leading_row
-0000ba70: 7320 746f 2030 2064 6f65 7320 7468 6174  s to 0 does that
-0000ba80: 2e20 4966 2068 6561 6465 723d 4e20 616e  . If header=N an
-0000ba90: 6420 4e3e 302c 2077 6520 7761 6e74 2074  d N>0, we want t
-0000baa0: 6f20 736b 6970 204e 2072 6f77 732e 0a20  o skip N rows.. 
-0000bab0: 2020 2020 2020 2020 2020 2069 6620 6865             if he
-0000bac0: 6164 6572 2069 7320 4e6f 6e65 3a0a 2020  ader is None:.  
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000bae0: 625f 636f 6e66 6967 2e73 6b69 705f 6c65  b_config.skip_le
-0000baf0: 6164 696e 675f 726f 7773 203d 2030 0a20  ading_rows = 0. 
-0000bb00: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000bb10: 6865 6164 6572 203e 2030 3a0a 2020 2020  header > 0:.    
-0000bb20: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000bb30: 636f 6e66 6967 2e73 6b69 705f 6c65 6164  config.skip_lead
-0000bb40: 696e 675f 726f 7773 203d 2068 6561 6465  ing_rows = heade
-0000bb50: 720a 0a20 2020 2020 2020 2020 2020 2072  r..            r
-0000bb60: 6574 7572 6e20 7365 6c66 2e5f 7265 6164  eturn self._read
-0000bb70: 5f62 6967 7175 6572 795f 6c6f 6164 5f6a  _bigquery_load_j
-0000bb80: 6f62 280a 2020 2020 2020 2020 2020 2020  ob(.            
-0000bb90: 2020 2020 6669 6c65 7061 7468 5f6f 725f      filepath_or_
-0000bba0: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
-0000bbb0: 2020 2020 2020 2020 7461 626c 652c 0a20          table,. 
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-0000bbd0: 6f62 5f63 6f6e 6669 673d 6a6f 625f 636f  ob_config=job_co
-0000bbe0: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
-0000bbf0: 2020 2020 2020 696e 6465 785f 636f 6c3d        index_col=
-0000bc00: 696e 6465 785f 636f 6c2c 0a20 2020 2020  index_col,.     
-0000bc10: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000bc20: 6e73 3d63 6f6c 756d 6e73 2c0a 2020 2020  ns=columns,.    
-0000bc30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000bc40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000bc50: 2020 2020 6966 2061 6e79 2861 7267 2069      if any(arg i
-0000bc60: 6e20 6b77 6172 6773 2066 6f72 2061 7267  n kwargs for arg
-0000bc70: 2069 6e20 2822 6368 756e 6b73 697a 6522   in ("chunksize"
-0000bc80: 2c20 2269 7465 7261 746f 7222 2929 3a0a  , "iterator")):.
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-0000bcb0: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000bcd0: 2763 6875 6e6b 7369 7a65 2720 616e 6420  'chunksize' and 
-0000bce0: 2769 7465 7261 746f 7227 2061 7267 756d  'iterator' argum
-0000bcf0: 656e 7473 2061 7265 206e 6f74 2073 7570  ents are not sup
-0000bd00: 706f 7274 6564 2e20 220a 2020 2020 2020  ported. ".      
-0000bd10: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000bd20: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
-0000bd30: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
-0000bd40: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000bd50: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000bd60: 6e73 7461 6e63 6528 6669 6c65 7061 7468  nstance(filepath
-0000bd70: 5f6f 725f 6275 6666 6572 2c20 7374 7229  _or_buffer, str)
-0000bd80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bd90: 2020 7365 6c66 2e5f 6368 6563 6b5f 6669    self._check_fi
-0000bda0: 6c65 5f73 697a 6528 6669 6c65 7061 7468  le_size(filepath
-0000bdb0: 5f6f 725f 6275 6666 6572 290a 2020 2020  _or_buffer).    
-0000bdc0: 2020 2020 2020 2020 7061 6e64 6173 5f64          pandas_d
-0000bdd0: 6620 3d20 7061 6e64 6173 2e72 6561 645f  f = pandas.read_
-0000bde0: 6373 7628 0a20 2020 2020 2020 2020 2020  csv(.           
-0000bdf0: 2020 2020 2066 696c 6570 6174 685f 6f72       filepath_or
-0000be00: 5f62 7566 6665 722c 0a20 2020 2020 2020  _buffer,.       
-0000be10: 2020 2020 2020 2020 2073 6570 3d73 6570           sep=sep
-0000be20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000be30: 2020 6865 6164 6572 3d68 6561 6465 722c    header=header,
-0000be40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000be50: 206e 616d 6573 3d6e 616d 6573 2c0a 2020   names=names,.  
-0000be60: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000be70: 6465 785f 636f 6c3d 696e 6465 785f 636f  dex_col=index_co
-0000be80: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-0000be90: 2020 2075 7365 636f 6c73 3d75 7365 636f     usecols=useco
-0000bea0: 6c73 2c20 2023 2074 7970 653a 2069 676e  ls,  # type: ign
-0000beb0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
-0000bec0: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
-0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bee0: 2065 6e67 696e 653d 656e 6769 6e65 2c0a   engine=engine,.
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 656e 636f 6469 6e67 3d65 6e63 6f64 696e  encoding=encodin
-0000bf10: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
-0000bf20: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
-0000bf30: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000bf40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000bf50: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
-0000bf60: 7061 6e64 6173 5f64 662c 2022 7265 6164  pandas_df, "read
-0000bf70: 5f63 7376 2229 2020 2320 7479 7065 3a20  _csv")  # type: 
-0000bf80: 6967 6e6f 7265 0a0a 2020 2020 6465 6620  ignore..    def 
-0000bf90: 7265 6164 5f70 6963 6b6c 6528 0a20 2020  read_pickle(.   
-0000bfa0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000bfb0: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
-0000bfc0: 7566 6665 723a 2046 696c 6550 6174 6820  uffer: FilePath 
-0000bfd0: 7c20 5265 6164 5069 636b 6c65 4275 6666  | ReadPickleBuff
-0000bfe0: 6572 2c0a 2020 2020 2020 2020 636f 6d70  er,.        comp
-0000bff0: 7265 7373 696f 6e3a 2043 6f6d 7072 6573  ression: Compres
-0000c000: 7369 6f6e 4f70 7469 6f6e 7320 3d20 2269  sionOptions = "i
-0000c010: 6e66 6572 222c 0a20 2020 2020 2020 2073  nfer",.        s
-0000c020: 746f 7261 6765 5f6f 7074 696f 6e73 3a20  torage_options: 
-0000c030: 5374 6f72 6167 654f 7074 696f 6e73 203d  StorageOptions =
-0000c040: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0000c050: 2020 2020 2020 7061 6e64 6173 5f6f 626a        pandas_obj
-0000c060: 203d 2070 616e 6461 732e 7265 6164 5f70   = pandas.read_p
-0000c070: 6963 6b6c 6528 0a20 2020 2020 2020 2020  ickle(.         
-0000c080: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
-0000c090: 7566 6665 722c 0a20 2020 2020 2020 2020  uffer,.         
-0000c0a0: 2020 2063 6f6d 7072 6573 7369 6f6e 3d63     compression=c
-0000c0b0: 6f6d 7072 6573 7369 6f6e 2c0a 2020 2020  ompression,.    
-0000c0c0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-0000c0d0: 6f70 7469 6f6e 733d 7374 6f72 6167 655f  options=storage_
-0000c0e0: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
-0000c0f0: 2029 0a0a 2020 2020 2020 2020 6966 2069   )..        if i
-0000c100: 7369 6e73 7461 6e63 6528 7061 6e64 6173  sinstance(pandas
-0000c110: 5f6f 626a 2c20 7061 6e64 6173 2e53 6572  _obj, pandas.Ser
-0000c120: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
-0000c130: 2020 6966 2070 616e 6461 735f 6f62 6a2e    if pandas_obj.
-0000c140: 6e61 6d65 2069 7320 4e6f 6e65 3a0a 2020  name is None:.  
-0000c150: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000c160: 6e64 6173 5f6f 626a 2e6e 616d 6520 3d20  ndas_obj.name = 
-0000c170: 2230 220a 2020 2020 2020 2020 2020 2020  "0".            
-0000c180: 6269 6766 7261 6d65 735f 6466 203d 2073  bigframes_df = s
-0000c190: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
-0000c1a0: 2870 616e 6461 735f 6f62 6a2e 746f 5f66  (pandas_obj.to_f
-0000c1b0: 7261 6d65 2829 2c20 2272 6561 645f 7069  rame(), "read_pi
-0000c1c0: 636b 6c65 2229 0a20 2020 2020 2020 2020  ckle").         
-0000c1d0: 2020 2072 6574 7572 6e20 6269 6766 7261     return bigfra
-0000c1e0: 6d65 735f 6466 5b62 6967 6672 616d 6573  mes_df[bigframes
-0000c1f0: 5f64 662e 636f 6c75 6d6e 735b 305d 5d0a  _df.columns[0]].
-0000c200: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000c210: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
-0000c220: 2870 616e 6461 735f 6f62 6a2c 2022 7265  (pandas_obj, "re
-0000c230: 6164 5f70 6963 6b6c 6522 290a 0a20 2020  ad_pickle")..   
-0000c240: 2064 6566 2072 6561 645f 7061 7271 7565   def read_parque
-0000c250: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-0000c260: 0a20 2020 2020 2020 2070 6174 683a 2073  .        path: s
-0000c270: 7472 207c 2049 4f5b 2262 7974 6573 225d  tr | IO["bytes"]
-0000c280: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-0000c290: 2020 2020 2065 6e67 696e 653a 2073 7472       engine: str
-0000c2a0: 203d 2022 6175 746f 222c 0a20 2020 2029   = "auto",.    )
-0000c2b0: 202d 3e20 6461 7461 6672 616d 652e 4461   -> dataframe.Da
-0000c2c0: 7461 4672 616d 653a 0a20 2020 2020 2020  taFrame:.       
-0000c2d0: 2074 6162 6c65 203d 2062 6967 6672 616d   table = bigfram
-0000c2e0: 6573 5f69 6f2e 7261 6e64 6f6d 5f74 6162  es_io.random_tab
-0000c2f0: 6c65 2873 656c 662e 5f61 6e6f 6e79 6d6f  le(self._anonymo
-0000c300: 7573 5f64 6174 6173 6574 290a 0a20 2020  us_dataset)..   
-0000c310: 2020 2020 2069 6620 656e 6769 6e65 203d       if engine =
-0000c320: 3d20 2262 6967 7175 6572 7922 3a0a 2020  = "bigquery":.  
-0000c330: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-0000c340: 6e66 6967 203d 2073 656c 662e 5f70 7265  nfig = self._pre
-0000c350: 7061 7265 5f6c 6f61 645f 6a6f 625f 636f  pare_load_job_co
-0000c360: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
-0000c370: 2020 206a 6f62 5f63 6f6e 6669 672e 6372     job_config.cr
-0000c380: 6561 7465 5f64 6973 706f 7369 7469 6f6e  eate_disposition
-0000c390: 203d 2062 6967 7175 6572 792e 4372 6561   = bigquery.Crea
-0000c3a0: 7465 4469 7370 6f73 6974 696f 6e2e 4352  teDisposition.CR
-0000c3b0: 4541 5445 5f49 465f 4e45 4544 4544 0a20  EATE_IF_NEEDED. 
-0000c3c0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000c3d0: 6f6e 6669 672e 736f 7572 6365 5f66 6f72  onfig.source_for
-0000c3e0: 6d61 7420 3d20 6269 6771 7565 7279 2e53  mat = bigquery.S
-0000c3f0: 6f75 7263 6546 6f72 6d61 742e 5041 5251  ourceFormat.PARQ
-0000c400: 5545 540a 2020 2020 2020 2020 2020 2020  UET.            
-0000c410: 6a6f 625f 636f 6e66 6967 2e77 7269 7465  job_config.write
-0000c420: 5f64 6973 706f 7369 7469 6f6e 203d 2062  _disposition = b
-0000c430: 6967 7175 6572 792e 5772 6974 6544 6973  igquery.WriteDis
-0000c440: 706f 7369 7469 6f6e 2e57 5249 5445 5f45  position.WRITE_E
-0000c450: 4d50 5459 0a20 2020 2020 2020 2020 2020  MPTY.           
-0000c460: 206a 6f62 5f63 6f6e 6669 672e 6c61 6265   job_config.labe
-0000c470: 6c73 203d 207b 2262 6967 6672 616d 6573  ls = {"bigframes
-0000c480: 2d61 7069 223a 2022 7265 6164 5f70 6172  -api": "read_par
-0000c490: 7175 6574 227d 0a0a 2020 2020 2020 2020  quet"}..        
-0000c4a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000c4b0: 5f72 6561 645f 6269 6771 7565 7279 5f6c  _read_bigquery_l
-0000c4c0: 6f61 645f 6a6f 6228 7061 7468 2c20 7461  oad_job(path, ta
-0000c4d0: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
-0000c4e0: 6a6f 625f 636f 6e66 6967 290a 2020 2020  job_config).    
-0000c4f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c500: 2020 2020 2020 7265 6164 5f70 6172 7175        read_parqu
-0000c510: 6574 5f6b 7761 7267 733a 2044 6963 745b  et_kwargs: Dict[
-0000c520: 7374 722c 2041 6e79 5d20 3d20 7b7d 0a20  str, Any] = {}. 
-0000c530: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
-0000c540: 6e64 6173 2e5f 5f76 6572 7369 6f6e 5f5f  ndas.__version__
-0000c550: 2e73 7461 7274 7377 6974 6828 2231 2e22  .startswith("1."
-0000c560: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c570: 2020 2072 6561 645f 7061 7271 7565 745f     read_parquet_
-0000c580: 6b77 6172 6773 5b22 7573 655f 6e75 6c6c  kwargs["use_null
-0000c590: 6162 6c65 5f64 7479 7065 7322 5d20 3d20  able_dtypes"] = 
-0000c5a0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000c5b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000c5c0: 2020 2020 2020 2072 6561 645f 7061 7271         read_parq
-0000c5d0: 7565 745f 6b77 6172 6773 5b22 6474 7970  uet_kwargs["dtyp
-0000c5e0: 655f 6261 636b 656e 6422 5d20 3d20 2270  e_backend"] = "p
-0000c5f0: 7961 7272 6f77 220a 0a20 2020 2020 2020  yarrow"..       
-0000c600: 2020 2020 2070 616e 6461 735f 6f62 6a20       pandas_obj 
-0000c610: 3d20 7061 6e64 6173 2e72 6561 645f 7061  = pandas.read_pa
-0000c620: 7271 7565 7428 0a20 2020 2020 2020 2020  rquet(.         
-0000c630: 2020 2020 2020 2070 6174 682c 0a20 2020         path,.   
-0000c640: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
-0000c650: 696e 653d 656e 6769 6e65 2c20 2023 2074  ine=engine,  # t
-0000c660: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0000c670: 2020 2020 2020 2020 2020 2020 2a2a 7265              **re
-0000c680: 6164 5f70 6172 7175 6574 5f6b 7761 7267  ad_parquet_kwarg
-0000c690: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
-0000c6a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000c6b0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f70  urn self._read_p
-0000c6c0: 616e 6461 7328 7061 6e64 6173 5f6f 626a  andas(pandas_obj
-0000c6d0: 2c20 2272 6561 645f 7061 7271 7565 7422  , "read_parquet"
-0000c6e0: 290a 0a20 2020 2064 6566 2072 6561 645f  )..    def read_
-0000c6f0: 6a73 6f6e 280a 2020 2020 2020 2020 7365  json(.        se
-0000c700: 6c66 2c0a 2020 2020 2020 2020 7061 7468  lf,.        path
-0000c710: 5f6f 725f 6275 663a 2073 7472 207c 2049  _or_buf: str | I
-0000c720: 4f5b 2262 7974 6573 225d 2c0a 2020 2020  O["bytes"],.    
-0000c730: 2020 2020 2a2c 0a20 2020 2020 2020 206f      *,.        o
-0000c740: 7269 656e 743a 204c 6974 6572 616c 5b0a  rient: Literal[.
-0000c750: 2020 2020 2020 2020 2020 2020 2273 706c              "spl
-0000c760: 6974 222c 2022 7265 636f 7264 7322 2c20  it", "records", 
-0000c770: 2269 6e64 6578 222c 2022 636f 6c75 6d6e  "index", "column
-0000c780: 7322 2c20 2276 616c 7565 7322 2c20 2274  s", "values", "t
-0000c790: 6162 6c65 220a 2020 2020 2020 2020 5d20  able".        ] 
-0000c7a0: 3d20 2263 6f6c 756d 6e73 222c 0a20 2020  = "columns",.   
-0000c7b0: 2020 2020 2064 7479 7065 3a20 4f70 7469       dtype: Opti
-0000c7c0: 6f6e 616c 5b44 6963 745d 203d 204e 6f6e  onal[Dict] = Non
-0000c7d0: 652c 0a20 2020 2020 2020 2065 6e63 6f64  e,.        encod
-0000c7e0: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
-0000c7f0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000c800: 2020 206c 696e 6573 3a20 626f 6f6c 203d     lines: bool =
-0000c810: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000c820: 656e 6769 6e65 3a20 4c69 7465 7261 6c5b  engine: Literal[
-0000c830: 2275 6a73 6f6e 222c 2022 7079 6172 726f  "ujson", "pyarro
-0000c840: 7722 2c20 2262 6967 7175 6572 7922 5d20  w", "bigquery"] 
-0000c850: 3d20 2275 6a73 6f6e 222c 0a20 2020 2020  = "ujson",.     
-0000c860: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
-0000c870: 2029 202d 3e20 6461 7461 6672 616d 652e   ) -> dataframe.
-0000c880: 4461 7461 4672 616d 653a 0a20 2020 2020  DataFrame:.     
-0000c890: 2020 2074 6162 6c65 203d 2062 6967 6672     table = bigfr
-0000c8a0: 616d 6573 5f69 6f2e 7261 6e64 6f6d 5f74  ames_io.random_t
-0000c8b0: 6162 6c65 2873 656c 662e 5f61 6e6f 6e79  able(self._anony
-0000c8c0: 6d6f 7573 5f64 6174 6173 6574 290a 0a20  mous_dataset).. 
-0000c8d0: 2020 2020 2020 2069 6620 656e 6769 6e65         if engine
-0000c8e0: 203d 3d20 2262 6967 7175 6572 7922 3a0a   == "bigquery":.
-0000c8f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c900: 6474 7970 6520 6973 206e 6f74 204e 6f6e  dtype is not Non
-0000c910: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000c920: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-0000c930: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
-0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c950: 2020 2242 6967 5175 6572 7920 656e 6769    "BigQuery engi
-0000c960: 6e65 2064 6f65 7320 6e6f 7420 7375 7070  ne does not supp
-0000c970: 6f72 7420 7468 6520 6474 7970 6520 6172  ort the dtype ar
-0000c980: 6775 6d65 6e74 732e 220a 2020 2020 2020  guments.".      
-0000c990: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000c9a0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000c9b0: 6c69 6e65 733a 0a20 2020 2020 2020 2020  lines:.         
-0000c9c0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-0000c9d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-0000c9e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c9f0: 2020 2020 2020 224f 6e6c 7920 6e65 776c        "Only newl
-0000ca00: 696e 6520 6465 6c69 6d69 7465 6420 4a53  ine delimited JS
-0000ca10: 4f4e 2066 6f72 6d61 7420 6973 2073 7570  ON format is sup
-0000ca20: 706f 7274 6564 2e22 0a20 2020 2020 2020  ported.".       
-0000ca30: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000ca40: 2020 2020 2020 2020 6966 2065 6e63 6f64          if encod
-0000ca50: 696e 6720 6973 206e 6f74 204e 6f6e 6520  ing is not None 
-0000ca60: 616e 6420 656e 636f 6469 6e67 206e 6f74  and encoding not
-0000ca70: 2069 6e20 5f56 414c 4944 5f45 4e43 4f44   in _VALID_ENCOD
-0000ca80: 494e 4753 3a0a 2020 2020 2020 2020 2020  INGS:.          
-0000ca90: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-0000caa0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cac0: 2020 2020 2066 2242 6967 5175 6572 7920       f"BigQuery 
-0000cad0: 656e 6769 6e65 206f 6e6c 7920 7375 7070  engine only supp
-0000cae0: 6f72 7473 2074 6865 2066 6f6c 6c6f 7769  orts the followi
-0000caf0: 6e67 2065 6e63 6f64 696e 6773 3a20 7b5f  ng encodings: {_
-0000cb00: 5641 4c49 445f 454e 434f 4449 4e47 537d  VALID_ENCODINGS}
-0000cb10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000cb20: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-0000cb30: 2069 6620 6c69 6e65 7320 616e 6420 6f72   if lines and or
-0000cb40: 6965 6e74 2021 3d20 2272 6563 6f72 6473  ient != "records
-0000cb50: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000cb60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000cb70: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000cb80: 2020 2020 2020 2020 2022 276c 696e 6573           "'lines
-0000cb90: 2720 6b65 7977 6f72 6420 6973 206f 6e6c  ' keyword is onl
-0000cba0: 7920 7661 6c69 6420 7768 656e 2027 6f72  y valid when 'or
-0000cbb0: 6965 6e74 2720 6973 2027 7265 636f 7264  ient' is 'record
-0000cbc0: 7327 2e22 0a20 2020 2020 2020 2020 2020  s'.".           
-0000cbd0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000cbe0: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
-0000cbf0: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
-0000cc00: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
-0000cc10: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000cc20: 5f63 6f6e 6669 672e 6372 6561 7465 5f64  _config.create_d
-0000cc30: 6973 706f 7369 7469 6f6e 203d 2062 6967  isposition = big
-0000cc40: 7175 6572 792e 4372 6561 7465 4469 7370  query.CreateDisp
-0000cc50: 6f73 6974 696f 6e2e 4352 4541 5445 5f49  osition.CREATE_I
-0000cc60: 465f 4e45 4544 4544 0a20 2020 2020 2020  F_NEEDED.       
-0000cc70: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
-0000cc80: 736f 7572 6365 5f66 6f72 6d61 7420 3d20  source_format = 
-0000cc90: 6269 6771 7565 7279 2e53 6f75 7263 6546  bigquery.SourceF
-0000cca0: 6f72 6d61 742e 4e45 574c 494e 455f 4445  ormat.NEWLINE_DE
-0000ccb0: 4c49 4d49 5445 445f 4a53 4f4e 0a20 2020  LIMITED_JSON.   
-0000ccc0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000ccd0: 6669 672e 7772 6974 655f 6469 7370 6f73  fig.write_dispos
-0000cce0: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
-0000ccf0: 2e57 7269 7465 4469 7370 6f73 6974 696f  .WriteDispositio
-0000cd00: 6e2e 5752 4954 455f 454d 5054 590a 2020  n.WRITE_EMPTY.  
+00006700: 0a20 2020 2020 2020 2070 7269 6d61 7279  .        primary
+00006710: 5f6b 6579 7320 3d20 4e6f 6e65 0a20 2020  _keys = None.   
+00006720: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00006730: 2020 2020 2020 2874 6162 6c65 5f63 6f6e        (table_con
+00006740: 7374 7261 696e 7473 203a 3d20 6765 7461  straints := geta
+00006750: 7474 7228 7461 626c 652c 2022 7461 626c  ttr(table, "tabl
+00006760: 655f 636f 6e73 7472 6169 6e74 7322 2c20  e_constraints", 
+00006770: 4e6f 6e65 2929 2069 7320 6e6f 7420 4e6f  None)) is not No
+00006780: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
+00006790: 6e64 2028 7072 696d 6172 795f 6b65 7920  nd (primary_key 
+000067a0: 3a3d 2074 6162 6c65 5f63 6f6e 7374 7261  := table_constra
+000067b0: 696e 7473 2e70 7269 6d61 7279 5f6b 6579  ints.primary_key
+000067c0: 2920 6973 206e 6f74 204e 6f6e 650a 2020  ) is not None.  
+000067d0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+000067e0: 2077 696c 6c20 6265 2046 616c 7365 2066   will be False f
+000067f0: 6f72 2065 6974 6865 7220 4e6f 6e65 206f  or either None o
+00006800: 7220 656d 7074 7920 6c69 7374 2e0a 2020  r empty list..  
+00006810: 2020 2020 2020 2020 2020 2320 5765 2077            # We w
+00006820: 616e 7420 7072 696d 6172 795f 6b65 7973  ant primary_keys
+00006830: 203d 204e 6f6e 6520 6966 206e 6f20 7072   = None if no pr
+00006840: 696d 6172 7920 6b65 7973 2061 7265 2073  imary keys are s
+00006850: 6574 2e0a 2020 2020 2020 2020 2020 2020  et..            
+00006860: 616e 6420 2863 6f6c 756d 6e73 203a 3d20  and (columns := 
+00006870: 7072 696d 6172 795f 6b65 792e 636f 6c75  primary_key.colu
+00006880: 6d6e 7329 0a20 2020 2020 2020 2029 3a0a  mns).        ):.
+00006890: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+000068a0: 6172 795f 6b65 7973 203d 2063 6f6c 756d  ary_keys = colum
+000068b0: 6e73 0a0a 2020 2020 2020 2020 6a6f 625f  ns..        job_
+000068c0: 636f 6e66 6967 203d 2062 6967 7175 6572  config = bigquer
+000068d0: 792e 5175 6572 794a 6f62 436f 6e66 6967  y.QueryJobConfig
+000068e0: 2829 0a20 2020 2020 2020 206a 6f62 5f63  ().        job_c
+000068f0: 6f6e 6669 672e 6c61 6265 6c73 5b22 6269  onfig.labels["bi
+00006900: 6766 7261 6d65 732d 6170 6922 5d20 3d20  gframes-api"] = 
+00006910: 6170 695f 6e61 6d65 0a20 2020 2020 2020  api_name.       
+00006920: 2069 6620 7573 655f 6361 6368 6520 616e   if use_cache an
+00006930: 6420 7461 626c 655f 7265 6620 696e 2073  d table_ref in s
+00006940: 656c 662e 5f64 665f 736e 6170 7368 6f74  elf._df_snapshot
+00006950: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00006960: 2020 2020 2073 6e61 7073 686f 745f 7469       snapshot_ti
+00006970: 6d65 7374 616d 7020 3d20 7365 6c66 2e5f  mestamp = self._
+00006980: 6466 5f73 6e61 7073 686f 745b 7461 626c  df_snapshot[tabl
+00006990: 655f 7265 665d 0a0a 2020 2020 2020 2020  e_ref]..        
+000069a0: 2020 2020 2320 4361 6368 6520 6869 7420      # Cache hit 
+000069b0: 636f 756c 6420 6265 2075 6e65 7870 6563  could be unexpec
+000069c0: 7465 642e 2053 6565 2069 6e74 6572 6e61  ted. See interna
+000069d0: 6c20 6973 7375 6520 3332 3935 3435 3830  l issue 32954580
+000069e0: 352e 0a20 2020 2020 2020 2020 2020 2023  5..            #
+000069f0: 2052 6169 7365 2061 2077 6172 6e69 6e67   Raise a warning
+00006a00: 2077 6974 6820 6d6f 7265 2069 6e66 6f72   with more infor
+00006a10: 6d61 7469 6f6e 2061 626f 7574 2068 6f77  mation about how
+00006a20: 2074 6f20 6176 6f69 6420 7468 650a 2020   to avoid the.  
+00006a30: 2020 2020 2020 2020 2020 2320 7072 6f62            # prob
+00006a40: 6c65 6d73 2077 6974 6820 7468 6520 6361  lems with the ca
+00006a50: 6368 652e 0a20 2020 2020 2020 2020 2020  che..           
+00006a60: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 6622 5265 6164 696e 6720 6361 6368 6564  f"Reading cached
+00006a90: 2074 6162 6c65 2066 726f 6d20 7b73 6e61   table from {sna
+00006aa0: 7073 686f 745f 7469 6d65 7374 616d 707d  pshot_timestamp}
+00006ab0: 2074 6f20 6176 6f69 6420 220a 2020 2020   to avoid ".    
+00006ac0: 2020 2020 2020 2020 2020 2020 2269 6e63              "inc
+00006ad0: 6f6d 7061 7469 6269 6c69 6573 2077 6974  ompatibilies wit
+00006ae0: 6820 7072 6576 696f 7573 2072 6561 6473  h previous reads
+00006af0: 206f 6620 7468 6973 2074 6162 6c65 2e20   of this table. 
+00006b00: 546f 2072 6561 6420 220a 2020 2020 2020  To read ".      
+00006b10: 2020 2020 2020 2020 2020 2274 6865 206c            "the l
+00006b20: 6174 6573 7420 7665 7273 696f 6e2c 2073  atest version, s
+00006b30: 6574 2060 7573 655f 6361 6368 653d 4661  et `use_cache=Fa
+00006b40: 6c73 6560 206f 7220 636c 6f73 6520 7468  lse` or close th
+00006b50: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+00006b60: 2020 2020 2263 7572 7265 6e74 2073 6573      "current ses
+00006b70: 7369 6f6e 2077 6974 6820 5365 7373 696f  sion with Sessio
+00006b80: 6e2e 636c 6f73 6528 2920 6f72 2022 0a20  n.close() or ". 
+00006b90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006ba0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
+00006bb0: 2e63 6c6f 7365 5f73 6573 7369 6f6e 2829  .close_session()
+00006bc0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00006bd0: 2020 2020 2320 5468 6572 6520 6172 6520      # There are 
+00006be0: 6d61 6e79 206c 6179 6572 7320 6265 666f  many layers befo
+00006bf0: 7265 2077 6520 6765 7420 746f 2028 706f  re we get to (po
+00006c00: 7373 6962 6c79 2920 7468 6520 7573 6572  ssibly) the user
+00006c10: 2773 2063 6f64 653a 0a20 2020 2020 2020  's code:.       
+00006c20: 2020 2020 2020 2020 2023 2070 616e 6461           # panda
+00006c30: 732e 7265 6164 5f67 6271 5f74 6162 6c65  s.read_gbq_table
+00006c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c50: 2023 202d 3e20 7769 7468 5f64 6566 6175   # -> with_defau
+00006c60: 6c74 5f73 6573 7369 6f6e 0a20 2020 2020  lt_session.     
+00006c70: 2020 2020 2020 2020 2020 2023 202d 3e20             # -> 
+00006c80: 5365 7373 696f 6e2e 7265 6164 5f67 6271  Session.read_gbq
+00006c90: 5f74 6162 6c65 0a20 2020 2020 2020 2020  _table.         
+00006ca0: 2020 2020 2020 2023 202d 3e20 5f72 6561         # -> _rea
+00006cb0: 645f 6762 715f 7461 626c 650a 2020 2020  d_gbq_table.    
+00006cc0: 2020 2020 2020 2020 2020 2020 2320 2d3e              # ->
+00006cd0: 205f 6765 745f 736e 6170 7368 6f74 5f73   _get_snapshot_s
+00006ce0: 716c 5f61 6e64 5f70 7269 6d61 7279 5f6b  ql_and_primary_k
+00006cf0: 6579 0a20 2020 2020 2020 2020 2020 2020  ey.             
+00006d00: 2020 2073 7461 636b 6c65 7665 6c3d 362c     stacklevel=6,
+00006d10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00006d20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006d30: 2020 2020 2020 2020 2073 6e61 7073 686f           snapsho
+00006d40: 745f 7469 6d65 7374 616d 7020 3d20 6c69  t_timestamp = li
+00006d50: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+00006d60: 2020 2020 7365 6c66 2e62 7163 6c69 656e      self.bqclien
+00006d70: 742e 7175 6572 7928 0a20 2020 2020 2020  t.query(.       
+00006d80: 2020 2020 2020 2020 2020 2020 2022 5345               "SE
+00006d90: 4c45 4354 2043 5552 5245 4e54 5f54 494d  LECT CURRENT_TIM
+00006da0: 4553 5441 4d50 2829 2041 5320 6063 7572  ESTAMP() AS `cur
+00006db0: 7265 6e74 5f74 696d 6573 7461 6d70 6022  rent_timestamp`"
+00006dc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006dd0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00006de0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
+00006df0: 2020 2020 2020 2020 2020 2020 2029 2e72               ).r
+00006e00: 6573 756c 7428 290a 2020 2020 2020 2020  esult().        
+00006e10: 2020 2020 295b 305d 5b30 5d0a 2020 2020      )[0][0].    
+00006e20: 2020 2020 2020 2020 7365 6c66 2e5f 6466          self._df
+00006e30: 5f73 6e61 7073 686f 745b 7461 626c 655f  _snapshot[table_
+00006e40: 7265 665d 203d 2073 6e61 7073 686f 745f  ref] = snapshot_
+00006e50: 7469 6d65 7374 616d 700a 0a20 2020 2020  timestamp..     
+00006e60: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00006e70: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
+00006e80: 7369 6f6e 203d 2073 656c 662e 6962 6973  sion = self.ibis
+00006e90: 5f63 6c69 656e 742e 7371 6c28 0a20 2020  _client.sql(.   
+00006ea0: 2020 2020 2020 2020 2020 2020 2062 6967               big
+00006eb0: 6672 616d 6573 5f69 6f2e 6372 6561 7465  frames_io.create
+00006ec0: 5f73 6e61 7073 686f 745f 7371 6c28 7461  _snapshot_sql(ta
+00006ed0: 626c 655f 7265 662c 2073 6e61 7073 686f  ble_ref, snapsho
+00006ee0: 745f 7469 6d65 7374 616d 7029 0a20 2020  t_timestamp).   
+00006ef0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00006f00: 2020 2065 7863 6570 7420 676f 6f67 6c65     except google
+00006f10: 2e61 7069 5f63 6f72 652e 6578 6365 7074  .api_core.except
+00006f20: 696f 6e73 2e46 6f72 6269 6464 656e 2061  ions.Forbidden a
+00006f30: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
+00006f40: 2020 6966 2022 4472 6976 6520 6372 6564    if "Drive cred
+00006f50: 656e 7469 616c 7322 2069 6e20 6578 2e6d  entials" in ex.m
+00006f60: 6573 7361 6765 3a0a 2020 2020 2020 2020  essage:.        
+00006f70: 2020 2020 2020 2020 6578 2e6d 6573 7361          ex.messa
+00006f80: 6765 202b 3d20 225c 6e43 6865 636b 2068  ge += "\nCheck h
+00006f90: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
+00006fa0: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
+00006fb0: 2f64 6f63 732f 7175 6572 792d 6472 6976  /docs/query-driv
+00006fc0: 652d 6461 7461 2347 6f6f 676c 655f 4472  e-data#Google_Dr
+00006fd0: 6976 655f 7065 726d 6973 7369 6f6e 732e  ive_permissions.
+00006fe0: 220a 2020 2020 2020 2020 2020 2020 7261  ".            ra
+00006ff0: 6973 650a 0a20 2020 2020 2020 2072 6574  ise..        ret
+00007000: 7572 6e20 7461 626c 655f 6578 7072 6573  urn table_expres
+00007010: 7369 6f6e 2c20 7072 696d 6172 795f 6b65  sion, primary_ke
+00007020: 7973 0a0a 2020 2020 6465 6620 5f72 6561  ys..    def _rea
+00007030: 645f 6762 715f 7461 626c 6528 0a20 2020  d_gbq_table(.   
+00007040: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00007050: 2020 2071 7565 7279 3a20 7374 722c 0a20     query: str,. 
+00007060: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00007070: 2020 696e 6465 785f 636f 6c3a 2049 7465    index_col: Ite
+00007080: 7261 626c 655b 7374 725d 207c 2073 7472  rable[str] | str
+00007090: 203d 2028 292c 0a20 2020 2020 2020 2063   = (),.        c
+000070a0: 6f6c 756d 6e73 3a20 4974 6572 6162 6c65  olumns: Iterable
+000070b0: 5b73 7472 5d20 3d20 2829 2c0a 2020 2020  [str] = (),.    
+000070c0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
+000070d0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000070e0: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
+000070f0: 7069 5f6e 616d 653a 2073 7472 2c0a 2020  pi_name: str,.  
+00007100: 2020 2020 2020 7573 655f 6361 6368 653a        use_cache:
+00007110: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+00007120: 2020 2920 2d3e 2064 6174 6166 7261 6d65    ) -> dataframe
+00007130: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
+00007140: 2020 2020 696d 706f 7274 2062 6967 6672      import bigfr
+00007150: 616d 6573 2e64 6174 6166 7261 6d65 2061  ames.dataframe a
+00007160: 7320 6461 7461 6672 616d 650a 0a20 2020  s dataframe..   
+00007170: 2020 2020 2069 6620 6d61 785f 7265 7375       if max_resu
+00007180: 6c74 7320 616e 6420 6d61 785f 7265 7375  lts and max_resu
+00007190: 6c74 7320 3c3d 2030 3a0a 2020 2020 2020  lts <= 0:.      
+000071a0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000071b0: 6545 7272 6f72 2822 606d 6178 5f72 6573  eError("`max_res
+000071c0: 756c 7473 6020 7368 6f75 6c64 2062 6520  ults` should be 
+000071d0: 6120 706f 7369 7469 7665 206e 756d 6265  a positive numbe
+000071e0: 722e 2229 0a0a 2020 2020 2020 2020 7461  r.")..        ta
+000071f0: 626c 655f 7265 6620 3d20 6269 6771 7565  ble_ref = bigque
+00007200: 7279 2e74 6162 6c65 2e54 6162 6c65 5265  ry.table.TableRe
+00007210: 6665 7265 6e63 652e 6672 6f6d 5f73 7472  ference.from_str
+00007220: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00007230: 2071 7565 7279 2c20 6465 6661 756c 745f   query, default_
+00007240: 7072 6f6a 6563 743d 7365 6c66 2e62 7163  project=self.bqc
+00007250: 6c69 656e 742e 7072 6f6a 6563 740a 2020  lient.project.  
+00007260: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00007270: 2028 7461 626c 655f 6578 7072 6573 7369   (table_expressi
+00007280: 6f6e 2c20 7072 696d 6172 795f 6b65 7973  on, primary_keys
+00007290: 2c29 203d 2073 656c 662e 5f67 6574 5f73  ,) = self._get_s
+000072a0: 6e61 7073 686f 745f 7371 6c5f 616e 645f  napshot_sql_and_
+000072b0: 7072 696d 6172 795f 6b65 7928 0a20 2020  primary_key(.   
+000072c0: 2020 2020 2020 2020 2074 6162 6c65 5f72           table_r
+000072d0: 6566 2c20 6170 695f 6e61 6d65 3d61 7069  ef, api_name=api
+000072e0: 5f6e 616d 652c 2075 7365 5f63 6163 6865  _name, use_cache
+000072f0: 3d75 7365 5f63 6163 6865 0a20 2020 2020  =use_cache.     
+00007300: 2020 2029 0a20 2020 2020 2020 2074 6f74     ).        tot
+00007310: 616c 5f6f 7264 6572 696e 675f 636f 6c73  al_ordering_cols
+00007320: 203d 2070 7269 6d61 7279 5f6b 6579 730a   = primary_keys.
+00007330: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007340: 696e 6465 785f 636f 6c20 616e 6420 7072  index_col and pr
+00007350: 696d 6172 795f 6b65 7973 2069 7320 6e6f  imary_keys is no
+00007360: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00007370: 2020 2020 696e 6465 785f 636f 6c20 3d20      index_col = 
+00007380: 7072 696d 6172 795f 6b65 7973 0a0a 2020  primary_keys..  
+00007390: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+000073a0: 2063 6f6c 756d 6e73 3a0a 2020 2020 2020   columns:.      
+000073b0: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
+000073c0: 2069 6e20 7461 626c 655f 6578 7072 6573   in table_expres
+000073d0: 7369 6f6e 2e63 6f6c 756d 6e73 3a0a 2020  sion.columns:.  
+000073e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000073f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007410: 2020 2020 6622 436f 6c75 6d6e 2027 7b6b      f"Column '{k
+00007420: 6579 7d27 206f 6620 6063 6f6c 756d 6e73  ey}' of `columns
+00007430: 6020 6e6f 7420 666f 756e 6420 696e 2074  ` not found in t
+00007440: 6869 7320 7461 626c 652e 220a 2020 2020  his table.".    
+00007450: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00007460: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00007470: 616e 6365 2869 6e64 6578 5f63 6f6c 2c20  ance(index_col, 
+00007480: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00007490: 2020 696e 6465 785f 636f 6c73 3a20 4c69    index_cols: Li
+000074a0: 7374 5b73 7472 5d20 3d20 5b69 6e64 6578  st[str] = [index
+000074b0: 5f63 6f6c 5d0a 2020 2020 2020 2020 656c  _col].        el
+000074c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000074d0: 696e 6465 785f 636f 6c73 203d 206c 6973  index_cols = lis
+000074e0: 7428 696e 6465 785f 636f 6c29 0a0a 2020  t(index_col)..  
+000074f0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00007500: 2069 6e64 6578 5f63 6f6c 733a 0a20 2020   index_cols:.   
+00007510: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+00007520: 6e6f 7420 696e 2074 6162 6c65 5f65 7870  not in table_exp
+00007530: 7265 7373 696f 6e2e 636f 6c75 6d6e 733a  ression.columns:
+00007540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007550: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00007560: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00007570: 2020 2020 2020 2066 2243 6f6c 756d 6e20         f"Column 
+00007580: 607b 6b65 797d 6020 6f66 2060 696e 6465  `{key}` of `inde
+00007590: 785f 636f 6c60 206e 6f74 2066 6f75 6e64  x_col` not found
+000075a0: 2069 6e20 7468 6973 2074 6162 6c65 2e22   in this table."
+000075b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000075c0: 2029 0a0a 2020 2020 2020 2020 6966 2063   )..        if c
+000075d0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+000075e0: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
+000075f0: 7369 6f6e 203d 2074 6162 6c65 5f65 7870  sion = table_exp
+00007600: 7265 7373 696f 6e2e 7365 6c65 6374 285b  ression.select([
+00007610: 2a69 6e64 6578 5f63 6f6c 732c 202a 636f  *index_cols, *co
+00007620: 6c75 6d6e 735d 290a 0a20 2020 2020 2020  lumns])..       
+00007630: 2023 2049 6620 7468 6520 696e 6465 7820   # If the index 
+00007640: 6973 2075 6e69 7175 6520 616e 6420 736f  is unique and so
+00007650: 7274 6162 6c65 2c20 7468 656e 2077 6520  rtable, then we 
+00007660: 646f 6e27 7420 6e65 6564 2074 6f20 6765  don't need to ge
+00007670: 6e65 7261 7465 0a20 2020 2020 2020 2023  nerate.        #
+00007680: 2061 6e20 6f72 6465 7269 6e67 2063 6f6c   an ordering col
+00007690: 756d 6e2e 0a20 2020 2020 2020 206f 7264  umn..        ord
+000076a0: 6572 696e 6720 3d20 4e6f 6e65 0a20 2020  ering = None.   
+000076b0: 2020 2020 2069 6620 746f 7461 6c5f 6f72       if total_or
+000076c0: 6465 7269 6e67 5f63 6f6c 7320 6973 206e  dering_cols is n
+000076d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000076e0: 2020 2020 2023 204e 6f74 653a 2063 7572       # Note: cur
+000076f0: 7265 6e74 6c79 2c20 6120 7461 626c 6520  rently, a table 
+00007700: 6861 7320 6120 746f 7461 6c20 6f72 6465  has a total orde
+00007710: 7269 6e67 206f 6e6c 7920 7768 656e 2074  ring only when t
+00007720: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
+00007730: 2070 7269 6d61 7279 206b 6579 2873 2920   primary key(s) 
+00007740: 6172 6520 7365 7420 6f6e 2061 2074 6162  are set on a tab
+00007750: 6c65 2e20 5468 6520 7175 6572 7920 656e  le. The query en
+00007760: 6769 6e65 2061 7373 756d 6573 2073 7563  gine assumes suc
+00007770: 680a 2020 2020 2020 2020 2020 2020 2320  h.            # 
+00007780: 636f 6c75 6d6e 7320 6172 6520 756e 6971  columns are uniq
+00007790: 7565 2c20 6576 656e 2069 6620 6e6f 7420  ue, even if not 
+000077a0: 656e 666f 7263 6564 2e0a 2020 2020 2020  enforced..      
+000077b0: 2020 2020 2020 6f72 6465 7269 6e67 203d        ordering =
+000077c0: 206f 7264 6572 2e45 7870 7265 7373 696f   order.Expressio
+000077d0: 6e4f 7264 6572 696e 6728 0a20 2020 2020  nOrdering(.     
+000077e0: 2020 2020 2020 2020 2020 206f 7264 6572             order
+000077f0: 696e 675f 7661 6c75 655f 636f 6c75 6d6e  ing_value_column
+00007800: 733d 7475 706c 6528 0a20 2020 2020 2020  s=tuple(.       
+00007810: 2020 2020 2020 2020 2020 2020 206f 7264               ord
+00007820: 6572 2e61 7363 656e 6469 6e67 5f6f 7665  er.ascending_ove
+00007830: 7228 636f 6c75 6d6e 5f69 6429 2066 6f72  r(column_id) for
+00007840: 2063 6f6c 756d 6e5f 6964 2069 6e20 746f   column_id in to
+00007850: 7461 6c5f 6f72 6465 7269 6e67 5f63 6f6c  tal_ordering_col
+00007860: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00007870: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00007880: 2020 2020 2074 6f74 616c 5f6f 7264 6572       total_order
+00007890: 696e 675f 636f 6c75 6d6e 733d 6672 6f7a  ing_columns=froz
+000078a0: 656e 7365 7428 746f 7461 6c5f 6f72 6465  enset(total_orde
+000078b0: 7269 6e67 5f63 6f6c 7329 2c0a 2020 2020  ring_cols),.    
+000078c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000078d0: 2020 2020 2020 636f 6c75 6d6e 5f76 616c        column_val
+000078e0: 7565 7320 3d20 5b74 6162 6c65 5f65 7870  ues = [table_exp
+000078f0: 7265 7373 696f 6e5b 636f 6c5d 2066 6f72  ression[col] for
+00007900: 2063 6f6c 2069 6e20 7461 626c 655f 6578   col in table_ex
+00007910: 7072 6573 7369 6f6e 2e63 6f6c 756d 6e73  pression.columns
+00007920: 5d0a 2020 2020 2020 2020 2020 2020 6172  ].            ar
+00007930: 7261 795f 7661 6c75 6520 3d20 636f 7265  ray_value = core
+00007940: 2e41 7272 6179 5661 6c75 652e 6672 6f6d  .ArrayValue.from
+00007950: 5f69 6269 7328 0a20 2020 2020 2020 2020  _ibis(.         
+00007960: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007970: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+00007980: 6c65 5f65 7870 7265 7373 696f 6e2c 0a20  le_expression,. 
+00007990: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000079a0: 6f6c 756d 6e73 3d63 6f6c 756d 6e5f 7661  olumns=column_va
+000079b0: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
+000079c0: 2020 2020 2020 6869 6464 656e 5f6f 7264        hidden_ord
+000079d0: 6572 696e 675f 636f 6c75 6d6e 733d 5b5d  ering_columns=[]
+000079e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000079f0: 2020 6f72 6465 7269 6e67 3d6f 7264 6572    ordering=order
+00007a00: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00007a10: 2029 0a0a 2020 2020 2020 2020 656c 6966   )..        elif
+00007a20: 206c 656e 2869 6e64 6578 5f63 6f6c 7329   len(index_cols)
+00007a30: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
+00007a40: 2020 2023 2057 6520 6861 7665 2069 6e64     # We have ind
+00007a50: 6578 2063 6f6c 756d 6e73 2c20 6c65 7473  ex columns, lets
+00007a60: 2073 6565 2069 6620 7468 6f73 6520 6172   see if those ar
+00007a70: 6520 6163 7475 616c 6c79 2074 6f74 616c  e actually total
+00007a80: 5f6f 7264 6572 5f63 6f6c 756d 6e73 0a20  _order_columns. 
+00007a90: 2020 2020 2020 2020 2020 206f 7264 6572             order
+00007aa0: 696e 6720 3d20 6f72 6465 722e 4578 7072  ing = order.Expr
+00007ab0: 6573 7369 6f6e 4f72 6465 7269 6e67 280a  essionOrdering(.
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 6f72 6465 7269 6e67 5f76 616c 7565 5f63  ordering_value_c
+00007ae0: 6f6c 756d 6e73 3d74 7570 6c65 280a 2020  olumns=tuple(.  
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 2020 5b6f 7264 6572 2e61 7363 656e 6469    [order.ascendi
+00007b10: 6e67 5f6f 7665 7228 636f 6c75 6d6e 5f69  ng_over(column_i
+00007b20: 6429 2066 6f72 2063 6f6c 756d 6e5f 6964  d) for column_id
+00007b30: 2069 6e20 696e 6465 785f 636f 6c73 5d0a   in index_cols].
+00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00007b60: 2020 2074 6f74 616c 5f6f 7264 6572 696e     total_orderin
+00007b70: 675f 636f 6c75 6d6e 733d 6672 6f7a 656e  g_columns=frozen
+00007b80: 7365 7428 696e 6465 785f 636f 6c73 292c  set(index_cols),
+00007b90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007ba0: 2020 2020 2020 2020 2020 2069 735f 746f             is_to
+00007bb0: 7461 6c5f 6f72 6465 7269 6e67 203d 2073  tal_ordering = s
+00007bc0: 656c 662e 5f63 6865 636b 5f69 6e64 6578  elf._check_index
+00007bd0: 5f75 6e69 7175 656e 6573 7328 0a20 2020  _uniqueness(.   
+00007be0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+00007bf0: 6c65 5f65 7870 7265 7373 696f 6e2c 2069  le_expression, i
+00007c00: 6e64 6578 5f63 6f6c 730a 2020 2020 2020  ndex_cols.      
+00007c10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007c20: 2020 2020 6966 2069 735f 746f 7461 6c5f      if is_total_
+00007c30: 6f72 6465 7269 6e67 3a0a 2020 2020 2020  ordering:.      
+00007c40: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00007c50: 5f76 616c 7565 7320 3d20 5b0a 2020 2020  _values = [.    
+00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c70: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+00007c80: 5b63 6f6c 5d20 666f 7220 636f 6c20 696e  [col] for col in
+00007c90: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
+00007ca0: 6e2e 636f 6c75 6d6e 730a 2020 2020 2020  n.columns.      
+00007cb0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00007cc0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+00007cd0: 795f 7661 6c75 6520 3d20 636f 7265 2e41  y_value = core.A
+00007ce0: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
+00007cf0: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
+00007d00: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
+00007d30: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00007d40: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00007d50: 3d63 6f6c 756d 6e5f 7661 6c75 6573 2c0a  =column_values,.
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 2020 2020 6869 6464 656e 5f6f 7264 6572      hidden_order
+00007d80: 696e 675f 636f 6c75 6d6e 733d 5b5d 2c0a  ing_columns=[],.
+00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007da0: 2020 2020 6f72 6465 7269 6e67 3d6f 7264      ordering=ord
+00007db0: 6572 696e 672c 0a20 2020 2020 2020 2020  ering,.         
+00007dc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00007dd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00007de0: 2020 2020 2020 2020 2020 2061 7272 6179             array
+00007df0: 5f76 616c 7565 203d 2073 656c 662e 5f63  _value = self._c
+00007e00: 7265 6174 655f 746f 7461 6c5f 6f72 6465  reate_total_orde
+00007e10: 7269 6e67 2874 6162 6c65 5f65 7870 7265  ring(table_expre
+00007e20: 7373 696f 6e29 0a20 2020 2020 2020 2065  ssion).        e
+00007e30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007e40: 2061 7272 6179 5f76 616c 7565 203d 2073   array_value = s
+00007e50: 656c 662e 5f63 7265 6174 655f 746f 7461  elf._create_tota
+00007e60: 6c5f 6f72 6465 7269 6e67 2874 6162 6c65  l_ordering(table
+00007e70: 5f65 7870 7265 7373 696f 6e29 0a0a 2020  _expression)..  
+00007e80: 2020 2020 2020 7661 6c75 655f 636f 6c75        value_colu
+00007e90: 6d6e 7320 3d20 5b63 6f6c 2066 6f72 2063  mns = [col for c
+00007ea0: 6f6c 2069 6e20 6172 7261 795f 7661 6c75  ol in array_valu
+00007eb0: 652e 636f 6c75 6d6e 5f69 6473 2069 6620  e.column_ids if 
+00007ec0: 636f 6c20 6e6f 7420 696e 2069 6e64 6578  col not in index
+00007ed0: 5f63 6f6c 735d 0a20 2020 2020 2020 2062  _cols].        b
+00007ee0: 6c6f 636b 203d 2062 6c6f 636b 732e 426c  lock = blocks.Bl
+00007ef0: 6f63 6b28 0a20 2020 2020 2020 2020 2020  ock(.           
+00007f00: 2061 7272 6179 5f76 616c 7565 2c0a 2020   array_value,.  
+00007f10: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+00007f20: 636f 6c75 6d6e 733d 696e 6465 785f 636f  columns=index_co
+00007f30: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00007f40: 636f 6c75 6d6e 5f6c 6162 656c 733d 7661  column_labels=va
+00007f50: 6c75 655f 636f 6c75 6d6e 732c 0a20 2020  lue_columns,.   
+00007f60: 2020 2020 2020 2020 2069 6e64 6578 5f6c           index_l
+00007f70: 6162 656c 733d 696e 6465 785f 636f 6c73  abels=index_cols
+00007f80: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00007f90: 2020 2020 6966 206d 6178 5f72 6573 756c      if max_resul
+00007fa0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00007fb0: 626c 6f63 6b20 3d20 626c 6f63 6b2e 736c  block = block.sl
+00007fc0: 6963 6528 7374 6f70 3d6d 6178 5f72 6573  ice(stop=max_res
+00007fd0: 756c 7473 290a 2020 2020 2020 2020 6466  ults).        df
+00007fe0: 203d 2064 6174 6166 7261 6d65 2e44 6174   = dataframe.Dat
+00007ff0: 6146 7261 6d65 2862 6c6f 636b 290a 0a20  aFrame(block).. 
+00008000: 2020 2020 2020 2023 2049 6620 7573 6572         # If user
+00008010: 2070 726f 7669 6465 6420 696e 6465 7820   provided index 
+00008020: 636f 6c75 6d6e 732c 2073 686f 756c 6420  columns, should 
+00008030: 736f 7274 206f 7665 7220 6974 0a20 2020  sort over it.   
+00008040: 2020 2020 2069 6620 6c65 6e28 696e 6465       if len(inde
+00008050: 785f 636f 6c73 2920 3e20 303a 0a20 2020  x_cols) > 0:.   
+00008060: 2020 2020 2020 2020 2064 662e 736f 7274           df.sort
+00008070: 5f69 6e64 6578 2829 0a20 2020 2020 2020  _index().       
+00008080: 2072 6574 7572 6e20 6466 0a0a 2020 2020   return df..    
+00008090: 6465 6620 5f63 6865 636b 5f69 6e64 6578  def _check_index
+000080a0: 5f75 6e69 7175 656e 6573 7328 0a20 2020  _uniqueness(.   
+000080b0: 2020 2020 2073 656c 662c 2074 6162 6c65       self, table
+000080c0: 3a20 6962 6973 5f74 7970 6573 2e54 6162  : ibis_types.Tab
+000080d0: 6c65 2c20 696e 6465 785f 636f 6c73 3a20  le, index_cols: 
+000080e0: 4c69 7374 5b73 7472 5d0a 2020 2020 2920  List[str].    ) 
+000080f0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00008100: 2064 6973 7469 6e63 745f 7461 626c 6520   distinct_table 
+00008110: 3d20 7461 626c 652e 7365 6c65 6374 282a  = table.select(*
+00008120: 696e 6465 785f 636f 6c73 292e 6469 7374  index_cols).dist
+00008130: 696e 6374 2829 0a20 2020 2020 2020 2069  inct().        i
+00008140: 735f 756e 6971 7565 5f73 716c 203d 2066  s_unique_sql = f
+00008150: 2222 2257 4954 4820 6675 6c6c 5f74 6162  """WITH full_tab
+00008160: 6c65 2041 5320 280a 2020 2020 2020 2020  le AS (.        
+00008170: 2020 2020 7b73 656c 662e 6962 6973 5f63      {self.ibis_c
+00008180: 6c69 656e 742e 636f 6d70 696c 6528 7461  lient.compile(ta
+00008190: 626c 6529 7d0a 2020 2020 2020 2020 292c  ble)}.        ),
+000081a0: 0a20 2020 2020 2020 2064 6973 7469 6e63  .        distinc
+000081b0: 745f 7461 626c 6520 4153 2028 0a20 2020  t_table AS (.   
+000081c0: 2020 2020 2020 2020 207b 7365 6c66 2e69           {self.i
+000081d0: 6269 735f 636c 6965 6e74 2e63 6f6d 7069  bis_client.compi
+000081e0: 6c65 2864 6973 7469 6e63 745f 7461 626c  le(distinct_tabl
+000081f0: 6529 7d0a 2020 2020 2020 2020 290a 0a20  e)}.        ).. 
+00008200: 2020 2020 2020 2053 454c 4543 5420 2853         SELECT (S
+00008210: 454c 4543 5420 434f 554e 5428 2a29 2046  ELECT COUNT(*) F
+00008220: 524f 4d20 6675 6c6c 5f74 6162 6c65 2920  ROM full_table) 
+00008230: 4153 2060 746f 7461 6c5f 636f 756e 7460  AS `total_count`
+00008240: 2c0a 2020 2020 2020 2020 2853 454c 4543  ,.        (SELEC
+00008250: 5420 434f 554e 5428 2a29 2046 524f 4d20  T COUNT(*) FROM 
+00008260: 6469 7374 696e 6374 5f74 6162 6c65 2920  distinct_table) 
+00008270: 4153 2060 6469 7374 696e 6374 5f63 6f75  AS `distinct_cou
+00008280: 6e74 600a 2020 2020 2020 2020 2222 220a  nt`.        """.
+00008290: 2020 2020 2020 2020 7265 7375 6c74 732c          results,
+000082a0: 205f 203d 2073 656c 662e 5f73 7461 7274   _ = self._start
+000082b0: 5f71 7565 7279 2869 735f 756e 6971 7565  _query(is_unique
+000082c0: 5f73 716c 290a 2020 2020 2020 2020 726f  _sql).        ro
+000082d0: 7720 3d20 6e65 7874 2869 7465 7228 7265  w = next(iter(re
+000082e0: 7375 6c74 7329 290a 0a20 2020 2020 2020  sults))..       
+000082f0: 2074 6f74 616c 5f63 6f75 6e74 203d 2072   total_count = r
+00008300: 6f77 5b22 746f 7461 6c5f 636f 756e 7422  ow["total_count"
+00008310: 5d0a 2020 2020 2020 2020 6469 7374 696e  ].        distin
+00008320: 6374 5f63 6f75 6e74 203d 2072 6f77 5b22  ct_count = row["
+00008330: 6469 7374 696e 6374 5f63 6f75 6e74 225d  distinct_count"]
+00008340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008350: 746f 7461 6c5f 636f 756e 7420 3d3d 2064  total_count == d
+00008360: 6973 7469 6e63 745f 636f 756e 740a 0a20  istinct_count.. 
+00008370: 2020 2064 6566 205f 7265 6164 5f62 6967     def _read_big
+00008380: 7175 6572 795f 6c6f 6164 5f6a 6f62 280a  query_load_job(.
+00008390: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000083a0: 2020 2020 2020 6669 6c65 7061 7468 5f6f        filepath_o
+000083b0: 725f 6275 6666 6572 3a20 7374 7220 7c20  r_buffer: str | 
+000083c0: 494f 5b22 6279 7465 7322 5d2c 0a20 2020  IO["bytes"],.   
+000083d0: 2020 2020 2074 6162 6c65 3a20 556e 696f       table: Unio
+000083e0: 6e5b 6269 6771 7565 7279 2e54 6162 6c65  n[bigquery.Table
+000083f0: 2c20 6269 6771 7565 7279 2e54 6162 6c65  , bigquery.Table
+00008400: 5265 6665 7265 6e63 655d 2c0a 2020 2020  Reference],.    
+00008410: 2020 2020 2a2c 0a20 2020 2020 2020 206a      *,.        j
+00008420: 6f62 5f63 6f6e 6669 673a 2062 6967 7175  ob_config: bigqu
+00008430: 6572 792e 4c6f 6164 4a6f 6243 6f6e 6669  ery.LoadJobConfi
+00008440: 672c 0a20 2020 2020 2020 2069 6e64 6578  g,.        index
+00008450: 5f63 6f6c 3a20 4974 6572 6162 6c65 5b73  _col: Iterable[s
+00008460: 7472 5d20 7c20 7374 7220 3d20 2829 2c0a  tr] | str = (),.
+00008470: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00008480: 2049 7465 7261 626c 655b 7374 725d 203d   Iterable[str] =
+00008490: 2028 292c 0a20 2020 2029 202d 3e20 6461   (),.    ) -> da
+000084a0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
+000084b0: 653a 0a20 2020 2020 2020 2069 6620 6973  e:.        if is
+000084c0: 696e 7374 616e 6365 2869 6e64 6578 5f63  instance(index_c
+000084d0: 6f6c 2c20 7374 7229 3a0a 2020 2020 2020  ol, str):.      
+000084e0: 2020 2020 2020 696e 6465 785f 636f 6c73        index_cols
+000084f0: 203d 205b 696e 6465 785f 636f 6c5d 0a20   = [index_col]. 
+00008500: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008510: 2020 2020 2020 2020 2069 6e64 6578 5f63           index_c
+00008520: 6f6c 7320 3d20 6c69 7374 2869 6e64 6578  ols = list(index
+00008530: 5f63 6f6c 290a 0a20 2020 2020 2020 2069  _col)..        i
+00008540: 6620 6e6f 7420 6a6f 625f 636f 6e66 6967  f not job_config
+00008550: 2e63 6c75 7374 6572 696e 675f 6669 656c  .clustering_fiel
+00008560: 6473 2061 6e64 2069 6e64 6578 5f63 6f6c  ds and index_col
+00008570: 733a 0a20 2020 2020 2020 2020 2020 206a  s:.            j
+00008580: 6f62 5f63 6f6e 6669 672e 636c 7573 7465  ob_config.cluste
+00008590: 7269 6e67 5f66 6965 6c64 7320 3d20 696e  ring_fields = in
+000085a0: 6465 785f 636f 6c73 5b3a 5f4d 4158 5f43  dex_cols[:_MAX_C
+000085b0: 4c55 5354 4552 5f43 4f4c 554d 4e53 5d0a  LUSTER_COLUMNS].
+000085c0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+000085d0: 7374 616e 6365 2866 696c 6570 6174 685f  stance(filepath_
+000085e0: 6f72 5f62 7566 6665 722c 2073 7472 293a  or_buffer, str):
+000085f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008600: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+00008610: 6572 2e73 7461 7274 7377 6974 6828 2267  er.startswith("g
+00008620: 733a 2f2f 2229 3a0a 2020 2020 2020 2020  s://"):.        
+00008630: 2020 2020 2020 2020 6c6f 6164 5f6a 6f62          load_job
+00008640: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
+00008650: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
+00008660: 5f75 7269 280a 2020 2020 2020 2020 2020  _uri(.          
+00008670: 2020 2020 2020 2020 2020 6669 6c65 7061            filepa
+00008680: 7468 5f6f 725f 6275 6666 6572 2c20 7461  th_or_buffer, ta
+00008690: 626c 652c 206a 6f62 5f63 6f6e 6669 673d  ble, job_config=
+000086a0: 6a6f 625f 636f 6e66 6967 0a20 2020 2020  job_config.     
+000086b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000086c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000086d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000086e0: 6974 6820 6f70 656e 2866 696c 6570 6174  ith open(filepat
+000086f0: 685f 6f72 5f62 7566 6665 722c 2022 7262  h_or_buffer, "rb
+00008700: 2229 2061 7320 736f 7572 6365 5f66 696c  ") as source_fil
+00008710: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008720: 2020 2020 2020 206c 6f61 645f 6a6f 6220         load_job 
+00008730: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
+00008740: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
+00008750: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
+00008760: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00008770: 7572 6365 5f66 696c 652c 2074 6162 6c65  urce_file, table
+00008780: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
+00008790: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
+000087a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000087b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000087c0: 2020 2020 2020 2020 6c6f 6164 5f6a 6f62          load_job
+000087d0: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
+000087e0: 2e6c 6f61 645f 7461 626c 655f 6672 6f6d  .load_table_from
+000087f0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
+00008800: 2020 2020 2020 2066 696c 6570 6174 685f         filepath_
+00008810: 6f72 5f62 7566 6665 722c 2074 6162 6c65  or_buffer, table
+00008820: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
+00008830: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
+00008840: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+00008850: 656c 662e 5f73 7461 7274 5f67 656e 6572  elf._start_gener
+00008860: 6963 5f6a 6f62 286c 6f61 645f 6a6f 6229  ic_job(load_job)
+00008870: 0a20 2020 2020 2020 2074 6162 6c65 5f69  .        table_i
+00008880: 6420 3d20 6622 7b74 6162 6c65 2e70 726f  d = f"{table.pro
+00008890: 6a65 6374 7d2e 7b74 6162 6c65 2e64 6174  ject}.{table.dat
+000088a0: 6173 6574 5f69 647d 2e7b 7461 626c 652e  aset_id}.{table.
+000088b0: 7461 626c 655f 6964 7d22 0a0a 2020 2020  table_id}"..    
+000088c0: 2020 2020 2320 5570 6461 7465 2074 6865      # Update the
+000088d0: 2074 6162 6c65 2065 7870 6972 6174 696f   table expiratio
+000088e0: 6e20 736f 2077 6520 6172 656e 2774 206c  n so we aren't l
+000088f0: 696d 6974 6564 2074 6f20 7468 6520 6465  imited to the de
+00008900: 6661 756c 7420 3234 0a20 2020 2020 2020  fault 24.       
+00008910: 2023 2068 6f75 7273 206f 6620 7468 6520   # hours of the 
+00008920: 616e 6f6e 796d 6f75 7320 6461 7461 7365  anonymous datase
+00008930: 742e 0a20 2020 2020 2020 2074 6162 6c65  t..        table
+00008940: 5f65 7870 6972 6174 696f 6e20 3d20 6269  _expiration = bi
+00008950: 6771 7565 7279 2e54 6162 6c65 2874 6162  gquery.Table(tab
+00008960: 6c65 5f69 6429 0a20 2020 2020 2020 2074  le_id).        t
+00008970: 6162 6c65 5f65 7870 6972 6174 696f 6e2e  able_expiration.
+00008980: 6578 7069 7265 7320 3d20 280a 2020 2020  expires = (.    
+00008990: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+000089a0: 2e64 6174 6574 696d 652e 6e6f 7728 6461  .datetime.now(da
+000089b0: 7465 7469 6d65 2e74 696d 657a 6f6e 652e  tetime.timezone.
+000089c0: 7574 6329 202b 2063 6f6e 7374 616e 7473  utc) + constants
+000089d0: 2e44 4546 4155 4c54 5f45 5850 4952 4154  .DEFAULT_EXPIRAT
+000089e0: 494f 4e0a 2020 2020 2020 2020 290a 2020  ION.        ).  
+000089f0: 2020 2020 2020 7365 6c66 2e62 7163 6c69        self.bqcli
+00008a00: 656e 742e 7570 6461 7465 5f74 6162 6c65  ent.update_table
+00008a10: 2874 6162 6c65 5f65 7870 6972 6174 696f  (table_expiratio
+00008a20: 6e2c 205b 2265 7870 6972 6573 225d 290a  n, ["expires"]).
+00008a30: 0a20 2020 2020 2020 2023 2054 6865 2042  .        # The B
+00008a40: 6967 5175 6572 7920 5245 5354 2041 5049  igQuery REST API
+00008a50: 2066 6f72 2074 6162 6c65 732e 6765 7420   for tables.get 
+00008a60: 646f 6573 6e27 7420 7461 6b65 2061 2073  doesn't take a s
+00008a70: 6573 7369 6f6e 2049 442c 2073 6f20 7765  ession ID, so we
+00008a80: 0a20 2020 2020 2020 2023 2063 616e 2774  .        # can't
+00008a90: 2067 6574 2074 6865 2073 6368 656d 6120   get the schema 
+00008aa0: 666f 7220 6120 7465 6d70 2074 6162 6c65  for a temp table
+00008ab0: 2074 6861 7420 7761 792e 0a20 2020 2020   that way..     
+00008ac0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
+00008ad0: 6561 645f 6762 715f 7461 626c 6528 0a20  ead_gbq_table(. 
+00008ae0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00008af0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00008b00: 2069 6e64 6578 5f63 6f6c 3d69 6e64 6578   index_col=index
+00008b10: 5f63 6f6c 2c0a 2020 2020 2020 2020 2020  _col,.          
+00008b20: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
+00008b30: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
+00008b40: 2020 6465 6620 7265 6164 5f67 6271 5f6d    def read_gbq_m
+00008b50: 6f64 656c 2873 656c 662c 206d 6f64 656c  odel(self, model
+00008b60: 5f6e 616d 653a 2073 7472 293a 0a20 2020  _name: str):.   
+00008b70: 2020 2020 2022 2222 4c6f 6164 7320 6120       """Loads a 
+00008b80: 4269 6751 7565 7279 204d 4c20 6d6f 6465  BigQuery ML mode
+00008b90: 6c20 6672 6f6d 2042 6967 5175 6572 792e  l from BigQuery.
+00008ba0: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
+00008bb0: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
+00008bc0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+00008bd0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
+00008be0: 2061 7320 6270 640a 2020 2020 2020 2020   as bpd.        
+00008bf0: 2020 2020 3e3e 3e20 6270 642e 6f70 7469      >>> bpd.opti
+00008c00: 6f6e 732e 6469 7370 6c61 792e 7072 6f67  ons.display.prog
+00008c10: 7265 7373 5f62 6172 203d 204e 6f6e 650a  ress_bar = None.
+00008c20: 0a20 2020 2020 2020 2052 6561 6420 616e  .        Read an
+00008c30: 2065 7869 7374 696e 6720 4269 6751 7565   existing BigQue
+00008c40: 7279 204d 4c20 6d6f 6465 6c2e 0a0a 2020  ry ML model...  
+00008c50: 2020 2020 2020 2020 2020 3e3e 3e20 6d6f            >>> mo
+00008c60: 6465 6c5f 6e61 6d65 203d 2022 6269 6766  del_name = "bigf
+00008c70: 7261 6d65 732d 6465 762e 6271 6d6c 5f74  rames-dev.bqml_t
+00008c80: 7574 6f72 6961 6c2e 7065 6e67 7569 6e73  utorial.penguins
+00008c90: 5f6d 6f64 656c 220a 2020 2020 2020 2020  _model".        
+00008ca0: 2020 2020 3e3e 3e20 6d6f 6465 6c20 3d20      >>> model = 
+00008cb0: 6270 642e 7265 6164 5f67 6271 5f6d 6f64  bpd.read_gbq_mod
+00008cc0: 656c 286d 6f64 656c 5f6e 616d 6529 0a0a  el(model_name)..
+00008cd0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00008ce0: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00008cf0: 6e61 6d65 2028 7374 7229 3a0a 2020 2020  name (str):.    
+00008d00: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00008d10: 6d6f 6465 6c27 7320 6e61 6d65 2069 6e20  model's name in 
+00008d20: 4269 6751 7565 7279 2069 6e20 7468 6520  BigQuery in the 
+00008d30: 666f 726d 6174 0a20 2020 2020 2020 2020  format.         
+00008d40: 2020 2020 2020 2060 7072 6f6a 6563 745f         `project_
+00008d50: 6964 2e64 6174 6173 6574 5f69 642e 6d6f  id.dataset_id.mo
+00008d60: 6465 6c5f 6964 602c 206f 7220 6a75 7374  del_id`, or just
+00008d70: 2060 6461 7461 7365 745f 6964 2e6d 6f64   `dataset_id.mod
+00008d80: 656c 5f69 6460 0a20 2020 2020 2020 2020  el_id`.         
+00008d90: 2020 2020 2020 2074 6f20 6c6f 6164 2066         to load f
+00008da0: 726f 6d20 7468 6520 6465 6661 756c 7420  rom the default 
+00008db0: 7072 6f6a 6563 742e 0a0a 2020 2020 2020  project...      
+00008dc0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00008dd0: 2020 2020 2020 2041 2062 6967 6672 616d         A bigfram
+00008de0: 6573 2e6d 6c20 4d6f 6465 6c2c 2054 7261  es.ml Model, Tra
+00008df0: 6e73 666f 726d 6572 206f 7220 5069 7065  nsformer or Pipe
+00008e00: 6c69 6e65 2077 7261 7070 696e 6720 7468  line wrapping th
+00008e10: 6520 6d6f 6465 6c2e 0a20 2020 2020 2020  e model..       
+00008e20: 2022 2222 0a20 2020 2020 2020 2069 6d70   """.        imp
+00008e30: 6f72 7420 6269 6766 7261 6d65 732e 6d6c  ort bigframes.ml
+00008e40: 2e6c 6f61 6465 720a 0a20 2020 2020 2020  .loader..       
+00008e50: 206d 6f64 656c 5f72 6566 203d 2062 6967   model_ref = big
+00008e60: 7175 6572 792e 4d6f 6465 6c52 6566 6572  query.ModelRefer
+00008e70: 656e 6365 2e66 726f 6d5f 7374 7269 6e67  ence.from_string
+00008e80: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
+00008e90: 6465 6c5f 6e61 6d65 2c20 6465 6661 756c  del_name, defaul
+00008ea0: 745f 7072 6f6a 6563 743d 7365 6c66 2e62  t_project=self.b
+00008eb0: 7163 6c69 656e 742e 7072 6f6a 6563 740a  qclient.project.
+00008ec0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00008ed0: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e62    model = self.b
+00008ee0: 7163 6c69 656e 742e 6765 745f 6d6f 6465  qclient.get_mode
+00008ef0: 6c28 6d6f 6465 6c5f 7265 6629 0a20 2020  l(model_ref).   
+00008f00: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
+00008f10: 7261 6d65 732e 6d6c 2e6c 6f61 6465 722e  rames.ml.loader.
+00008f20: 6672 6f6d 5f62 7128 7365 6c66 2c20 6d6f  from_bq(self, mo
+00008f30: 6465 6c29 0a0a 2020 2020 4074 7970 696e  del)..    @typin
+00008f40: 672e 6f76 6572 6c6f 6164 0a20 2020 2064  g.overload.    d
+00008f50: 6566 2072 6561 645f 7061 6e64 6173 280a  ef read_pandas(.
+00008f60: 2020 2020 2020 2020 7365 6c66 2c20 7061          self, pa
+00008f70: 6e64 6173 5f64 6174 6166 7261 6d65 3a20  ndas_dataframe: 
+00008f80: 7061 6e64 6173 2e49 6e64 6578 0a20 2020  pandas.Index.   
+00008f90: 2029 202d 3e20 6269 6766 7261 6d65 732e   ) -> bigframes.
+00008fa0: 636f 7265 2e69 6e64 6578 6573 2e49 6e64  core.indexes.Ind
+00008fb0: 6578 3a0a 2020 2020 2020 2020 2e2e 2e0a  ex:.        ....
+00008fc0: 0a20 2020 2040 7479 7069 6e67 2e6f 7665  .    @typing.ove
+00008fd0: 726c 6f61 640a 2020 2020 6465 6620 7265  rload.    def re
+00008fe0: 6164 5f70 616e 6461 7328 7365 6c66 2c20  ad_pandas(self, 
+00008ff0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+00009000: 3a20 7061 6e64 6173 2e53 6572 6965 7329  : pandas.Series)
+00009010: 202d 3e20 6269 6766 7261 6d65 732e 7365   -> bigframes.se
+00009020: 7269 6573 2e53 6572 6965 733a 0a20 2020  ries.Series:.   
+00009030: 2020 2020 202e 2e2e 0a0a 2020 2020 4074       .....    @t
+00009040: 7970 696e 672e 6f76 6572 6c6f 6164 0a20  yping.overload. 
+00009050: 2020 2064 6566 2072 6561 645f 7061 6e64     def read_pand
+00009060: 6173 2873 656c 662c 2070 616e 6461 735f  as(self, pandas_
+00009070: 6461 7461 6672 616d 653a 2070 616e 6461  dataframe: panda
+00009080: 732e 4461 7461 4672 616d 6529 202d 3e20  s.DataFrame) -> 
+00009090: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+000090a0: 616d 653a 0a20 2020 2020 2020 202e 2e2e  ame:.        ...
+000090b0: 0a0a 2020 2020 6465 6620 7265 6164 5f70  ..    def read_p
+000090c0: 616e 6461 7328 0a20 2020 2020 2020 2073  andas(.        s
+000090d0: 656c 662c 2070 616e 6461 735f 6461 7461  elf, pandas_data
+000090e0: 6672 616d 653a 2055 6e69 6f6e 5b70 616e  frame: Union[pan
+000090f0: 6461 732e 4461 7461 4672 616d 652c 2070  das.DataFrame, p
+00009100: 616e 6461 732e 5365 7269 6573 2c20 7061  andas.Series, pa
+00009110: 6e64 6173 2e49 6e64 6578 5d0a 2020 2020  ndas.Index].    
+00009120: 293a 0a20 2020 2020 2020 2022 2222 4c6f  ):.        """Lo
+00009130: 6164 7320 4461 7461 4672 616d 6520 6672  ads DataFrame fr
+00009140: 6f6d 2061 2070 616e 6461 7320 4461 7461  om a pandas Data
+00009150: 4672 616d 652e 0a0a 2020 2020 2020 2020  Frame...        
+00009160: 5468 6520 7061 6e64 6173 2044 6174 6146  The pandas DataF
+00009170: 7261 6d65 2077 696c 6c20 6265 2070 6572  rame will be per
+00009180: 7369 7374 6564 2061 7320 6120 7465 6d70  sisted as a temp
+00009190: 6f72 6172 7920 4269 6751 7565 7279 2074  orary BigQuery t
+000091a0: 6162 6c65 2c20 7768 6963 6820 6361 6e20  able, which can 
+000091b0: 6265 0a20 2020 2020 2020 2061 7574 6f6d  be.        autom
+000091c0: 6174 6963 616c 6c79 2072 6563 7963 6c65  atically recycle
+000091d0: 6420 6166 7465 7220 7468 6520 5365 7373  d after the Sess
+000091e0: 696f 6e20 6973 2063 6c6f 7365 642e 0a0a  ion is closed...
+000091f0: 2020 2020 2020 2020 2a2a 4578 616d 706c          **Exampl
+00009200: 6573 3a2a 2a0a 0a20 2020 2020 2020 2020  es:**..         
+00009210: 2020 203e 3e3e 2069 6d70 6f72 7420 6269     >>> import bi
+00009220: 6766 7261 6d65 732e 7061 6e64 6173 2061  gframes.pandas a
+00009230: 7320 6270 640a 2020 2020 2020 2020 2020  s bpd.          
+00009240: 2020 3e3e 3e20 696d 706f 7274 2070 616e    >>> import pan
+00009250: 6461 7320 6173 2070 640a 2020 2020 2020  das as pd.      
+00009260: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
+00009270: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
+00009280: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
+00009290: 650a 0a20 2020 2020 2020 2020 2020 203e  e..            >
+000092a0: 3e3e 2064 203d 207b 2763 6f6c 3127 3a20  >> d = {'col1': 
+000092b0: 5b31 2c20 325d 2c20 2763 6f6c 3227 3a20  [1, 2], 'col2': 
+000092c0: 5b33 2c20 345d 7d0a 2020 2020 2020 2020  [3, 4]}.        
+000092d0: 2020 2020 3e3e 3e20 7061 6e64 6173 5f64      >>> pandas_d
+000092e0: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+000092f0: 2864 6174 613d 6429 0a20 2020 2020 2020  (data=d).       
+00009300: 2020 2020 203e 3e3e 2064 6620 3d20 6270       >>> df = bp
+00009310: 642e 7265 6164 5f70 616e 6461 7328 7061  d.read_pandas(pa
+00009320: 6e64 6173 5f64 6629 0a20 2020 2020 2020  ndas_df).       
+00009330: 2020 2020 203e 3e3e 2064 660a 2020 2020       >>> df.    
+00009340: 2020 2020 2020 2020 2020 2063 6f6c 3120             col1 
+00009350: 2063 6f6c 320a 2020 2020 2020 2020 2020   col2.          
+00009360: 2020 3020 2020 2020 3120 2020 2020 330a    0     1     3.
+00009370: 2020 2020 2020 2020 2020 2020 3120 2020              1   
+00009380: 2020 3220 2020 2020 340a 2020 2020 2020    2     4.      
+00009390: 2020 2020 2020 3c42 4c41 4e4b 4c49 4e45        <BLANKLINE
+000093a0: 3e0a 2020 2020 2020 2020 2020 2020 5b32  >.            [2
+000093b0: 2072 6f77 7320 7820 3220 636f 6c75 6d6e   rows x 2 column
+000093c0: 735d 0a0a 2020 2020 2020 2020 4172 6773  s]..        Args
+000093d0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+000093e0: 6e64 6173 5f64 6174 6166 7261 6d65 2028  ndas_dataframe (
+000093f0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00009400: 2c20 7061 6e64 6173 2e53 6572 6965 732c  , pandas.Series,
+00009410: 206f 7220 7061 6e64 6173 2e49 6e64 6578   or pandas.Index
+00009420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009430: 2020 2061 2070 616e 6461 7320 4461 7461     a pandas Data
+00009440: 4672 616d 652f 5365 7269 6573 2f49 6e64  Frame/Series/Ind
+00009450: 6578 206f 626a 6563 7420 746f 2062 6520  ex object to be 
+00009460: 6c6f 6164 6564 2e0a 0a20 2020 2020 2020  loaded...       
+00009470: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00009480: 2020 2020 2020 416e 2065 7175 6976 616c        An equival
+00009490: 656e 7420 6269 6766 7261 6d65 732e 7061  ent bigframes.pa
+000094a0: 6e64 6173 2e28 4461 7461 4672 616d 652f  ndas.(DataFrame/
+000094b0: 5365 7269 6573 2f49 6e64 6578 2920 6f62  Series/Index) ob
+000094c0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+000094d0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+000094e0: 6269 6766 7261 6d65 732e 7365 7269 6573  bigframes.series
+000094f0: 2061 7320 7365 7269 6573 0a0a 2020 2020   as series..    
+00009500: 2020 2020 2320 5472 7920 746f 2068 616e      # Try to han
+00009510: 646c 6520 6e6f 6e2d 6461 7461 6672 616d  dle non-datafram
+00009520: 6520 7061 6e64 6173 206f 626a 6563 7473  e pandas objects
+00009530: 2061 7320 7765 6c6c 0a20 2020 2020 2020   as well.       
+00009540: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
+00009550: 616e 6461 735f 6461 7461 6672 616d 652c  andas_dataframe,
+00009560: 2070 616e 6461 732e 5365 7269 6573 293a   pandas.Series):
+00009570: 0a20 2020 2020 2020 2020 2020 2062 665f  .            bf_
+00009580: 6466 203d 2073 656c 662e 5f72 6561 645f  df = self._read_
+00009590: 7061 6e64 6173 2870 616e 6461 732e 4461  pandas(pandas.Da
+000095a0: 7461 4672 616d 6528 7061 6e64 6173 5f64  taFrame(pandas_d
+000095b0: 6174 6166 7261 6d65 292c 2022 7265 6164  ataframe), "read
+000095c0: 5f70 616e 6461 7322 290a 2020 2020 2020  _pandas").      
+000095d0: 2020 2020 2020 6266 5f73 6572 6965 7320        bf_series 
+000095e0: 3d20 7479 7069 6e67 2e63 6173 7428 7365  = typing.cast(se
+000095f0: 7269 6573 2e53 6572 6965 732c 2062 665f  ries.Series, bf_
+00009600: 6466 5b62 665f 6466 2e63 6f6c 756d 6e73  df[bf_df.columns
+00009610: 5b30 5d5d 290a 2020 2020 2020 2020 2020  [0]]).          
+00009620: 2020 2320 7772 6170 7069 6e67 2069 6e74    # wrapping int
+00009630: 6f20 6466 2063 616e 2073 6574 206e 616d  o df can set nam
+00009640: 6520 746f 2030 2073 6f20 7265 7365 7420  e to 0 so reset 
+00009650: 746f 206f 7269 6769 6e61 6c20 6f62 6a65  to original obje
+00009660: 6374 206e 616d 650a 2020 2020 2020 2020  ct name.        
+00009670: 2020 2020 6266 5f73 6572 6965 732e 6e61      bf_series.na
+00009680: 6d65 203d 2070 616e 6461 735f 6461 7461  me = pandas_data
+00009690: 6672 616d 652e 6e61 6d65 0a20 2020 2020  frame.name.     
+000096a0: 2020 2020 2020 2072 6574 7572 6e20 6266         return bf
+000096b0: 5f73 6572 6965 730a 2020 2020 2020 2020  _series.        
+000096c0: 6966 2069 7369 6e73 7461 6e63 6528 7061  if isinstance(pa
+000096d0: 6e64 6173 5f64 6174 6166 7261 6d65 2c20  ndas_dataframe, 
+000096e0: 7061 6e64 6173 2e49 6e64 6578 293a 0a20  pandas.Index):. 
+000096f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009700: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
+00009710: 6461 7328 0a20 2020 2020 2020 2020 2020  das(.           
+00009720: 2020 2020 2070 616e 6461 732e 4461 7461       pandas.Data
+00009730: 4672 616d 6528 696e 6465 783d 7061 6e64  Frame(index=pand
+00009740: 6173 5f64 6174 6166 7261 6d65 292c 2022  as_dataframe), "
+00009750: 7265 6164 5f70 616e 6461 7322 0a20 2020  read_pandas".   
+00009760: 2020 2020 2020 2020 2029 2e69 6e64 6578           ).index
+00009770: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00009780: 7374 616e 6365 2870 616e 6461 735f 6461  stance(pandas_da
+00009790: 7461 6672 616d 652c 2070 616e 6461 732e  taframe, pandas.
+000097a0: 4461 7461 4672 616d 6529 3a0a 2020 2020  DataFrame):.    
+000097b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000097c0: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
+000097d0: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
+000097e0: 652c 2022 7265 6164 5f70 616e 6461 7322  e, "read_pandas"
+000097f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00009800: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009810: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00009820: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00009830: 7265 6164 5f70 616e 6461 7328 2920 6578  read_pandas() ex
+00009840: 7065 6374 7320 6120 7061 6e64 6173 2e44  pects a pandas.D
+00009850: 6174 6146 7261 6d65 2c20 6275 7420 676f  ataFrame, but go
+00009860: 7420 6120 7b74 7970 6528 7061 6e64 6173  t a {type(pandas
+00009870: 5f64 6174 6166 7261 6d65 297d 220a 2020  _dataframe)}".  
+00009880: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00009890: 2064 6566 205f 7265 6164 5f70 616e 6461   def _read_panda
+000098a0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+000098b0: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
+000098c0: 653a 2070 616e 6461 732e 4461 7461 4672  e: pandas.DataFr
+000098d0: 616d 652c 2061 7069 5f6e 616d 653a 2073  ame, api_name: s
+000098e0: 7472 0a20 2020 2029 202d 3e20 6461 7461  tr.    ) -> data
+000098f0: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
+00009900: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+00009910: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
+00009920: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
+00009930: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+00009940: 6e73 7461 6e63 6528 7061 6e64 6173 5f64  nstance(pandas_d
+00009950: 6174 6166 7261 6d65 2c20 6461 7461 6672  ataframe, datafr
+00009960: 616d 652e 4461 7461 4672 616d 6529 3a0a  ame.DataFrame):.
+00009970: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009980: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00009990: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000099a0: 6561 645f 7061 6e64 6173 2829 2065 7870  ead_pandas() exp
+000099b0: 6563 7473 2061 2070 616e 6461 732e 4461  ects a pandas.Da
+000099c0: 7461 4672 616d 652c 2062 7574 2067 6f74  taFrame, but got
+000099d0: 2061 2022 0a20 2020 2020 2020 2020 2020   a ".           
+000099e0: 2020 2020 2022 6269 6766 7261 6d65 732e       "bigframes.
+000099f0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00009a00: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+00009a10: 0a0a 2020 2020 2020 2020 696e 6c69 6e65  ..        inline
+00009a20: 5f64 6620 3d20 7365 6c66 2e5f 7265 6164  _df = self._read
+00009a30: 5f70 616e 6461 735f 696e 6c69 6e65 2870  _pandas_inline(p
+00009a40: 616e 6461 735f 6461 7461 6672 616d 6529  andas_dataframe)
+00009a50: 0a20 2020 2020 2020 2069 6620 696e 6c69  .        if inli
+00009a60: 6e65 5f64 6620 6973 206e 6f74 204e 6f6e  ne_df is not Non
+00009a70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00009a80: 6574 7572 6e20 696e 6c69 6e65 5f64 660a  eturn inline_df.
+00009a90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00009aa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009ab0: 7365 6c66 2e5f 7265 6164 5f70 616e 6461  self._read_panda
+00009ac0: 735f 6c6f 6164 5f6a 6f62 2870 616e 6461  s_load_job(panda
+00009ad0: 735f 6461 7461 6672 616d 652c 2061 7069  s_dataframe, api
+00009ae0: 5f6e 616d 6529 0a20 2020 2020 2020 2065  _name).        e
+00009af0: 7863 6570 7420 7061 2e41 7272 6f77 496e  xcept pa.ArrowIn
+00009b00: 7661 6c69 6420 6173 2065 3a0a 2020 2020  valid as e:.    
+00009b10: 2020 2020 2020 2020 7261 6973 6520 7061          raise pa
+00009b20: 2e41 7272 6f77 496e 7661 6c69 6428 0a20  .ArrowInvalid(. 
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00009b40: 2243 6f75 6c64 206e 6f74 2063 6f6e 7665  "Could not conve
+00009b50: 7274 2077 6974 6820 6120 4269 6751 7565  rt with a BigQue
+00009b60: 7279 2074 7970 653a 2060 7b65 7d60 2e20  ry type: `{e}`. 
+00009b70: 220a 2020 2020 2020 2020 2020 2020 2920  ".            ) 
+00009b80: 6672 6f6d 2065 0a0a 2020 2020 6465 6620  from e..    def 
+00009b90: 5f72 6561 645f 7061 6e64 6173 5f69 6e6c  _read_pandas_inl
+00009ba0: 696e 6528 0a20 2020 2020 2020 2073 656c  ine(.        sel
+00009bb0: 662c 2070 616e 6461 735f 6461 7461 6672  f, pandas_datafr
+00009bc0: 616d 653a 2070 616e 6461 732e 4461 7461  ame: pandas.Data
+00009bd0: 4672 616d 650a 2020 2020 2920 2d3e 204f  Frame.    ) -> O
+00009be0: 7074 696f 6e61 6c5b 6461 7461 6672 616d  ptional[datafram
+00009bf0: 652e 4461 7461 4672 616d 655d 3a0a 2020  e.DataFrame]:.  
+00009c00: 2020 2020 2020 696d 706f 7274 2062 6967        import big
+00009c10: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
+00009c20: 2061 7320 6461 7461 6672 616d 650a 0a20   as dataframe.. 
+00009c30: 2020 2020 2020 2069 6620 7061 6e64 6173         if pandas
+00009c40: 5f64 6174 6166 7261 6d65 2e6d 656d 6f72  _dataframe.memor
+00009c50: 795f 7573 6167 6528 6465 6570 3d54 7275  y_usage(deep=Tru
+00009c60: 6529 2e73 756d 2829 203e 204d 4158 5f49  e).sum() > MAX_I
+00009c70: 4e4c 494e 455f 4446 5f42 5954 4553 3a0a  NLINE_DF_BYTES:.
+00009c80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009c90: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
+00009ca0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00009cb0: 2020 696e 6c69 6e65 5f64 6620 3d20 6461    inline_df = da
+00009cc0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
+00009cd0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00009ce0: 2020 2062 6c6f 636b 732e 426c 6f63 6b2e     blocks.Block.
+00009cf0: 6672 6f6d 5f6c 6f63 616c 2870 616e 6461  from_local(panda
+00009d00: 735f 6461 7461 6672 616d 652c 2073 656c  s_dataframe, sel
+00009d10: 6629 0a20 2020 2020 2020 2020 2020 2029  f).            )
+00009d20: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00009d30: 7061 2e41 7272 6f77 496e 7661 6c69 6420  pa.ArrowInvalid 
+00009d40: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00009d50: 2020 7261 6973 6520 7061 2e41 7272 6f77    raise pa.Arrow
+00009d60: 496e 7661 6c69 6428 0a20 2020 2020 2020  Invalid(.       
+00009d70: 2020 2020 2020 2020 2066 2243 6f75 6c64           f"Could
+00009d80: 206e 6f74 2063 6f6e 7665 7274 2077 6974   not convert wit
+00009d90: 6820 6120 4269 6751 7565 7279 2074 7970  h a BigQuery typ
+00009da0: 653a 2060 7b65 7d60 2e20 220a 2020 2020  e: `{e}`. ".    
+00009db0: 2020 2020 2020 2020 2920 6672 6f6d 2065          ) from e
+00009dc0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00009dd0: 5661 6c75 6545 7272 6f72 3a20 2023 2054  ValueError:  # T
+00009de0: 6872 6f77 6e20 6279 2069 6269 7320 666f  hrown by ibis fo
+00009df0: 7220 736f 6d65 2075 6e68 616e 646c 6564  r some unhandled
+00009e00: 2074 7970 6573 0a20 2020 2020 2020 2020   types.         
+00009e10: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00009e20: 2020 2020 2020 2065 7863 6570 7420 7061         except pa
+00009e30: 2e41 7272 6f77 5479 7065 4572 726f 723a  .ArrowTypeError:
+00009e40: 2020 2320 5468 726f 776e 2062 7920 6172    # Thrown by ar
+00009e50: 726f 7720 666f 7220 7479 7065 7320 7769  row for types wi
+00009e60: 7468 6f75 7420 6d61 7070 696e 6720 2867  thout mapping (g
+00009e70: 656f 292e 0a20 2020 2020 2020 2020 2020  eo)..           
+00009e80: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00009e90: 2020 2020 2020 696e 6c69 6e65 5f74 7970        inline_typ
+00009ea0: 6573 203d 2069 6e6c 696e 655f 6466 2e5f  es = inline_df._
+00009eb0: 626c 6f63 6b2e 6578 7072 2e73 6368 656d  block.expr.schem
+00009ec0: 612e 6474 7970 6573 0a20 2020 2020 2020  a.dtypes.       
+00009ed0: 2023 2049 6269 7320 6861 7320 7072 6f62   # Ibis has prob
+00009ee0: 6c65 6d73 2065 7363 6170 696e 6720 6279  lems escaping by
+00009ef0: 7465 7320 6c69 7465 7261 6c73 2c20 7768  tes literals, wh
+00009f00: 6963 6820 7769 6c6c 2063 6175 7365 2073  ich will cause s
+00009f10: 796e 7461 7820 6572 726f 7273 2073 6572  yntax errors ser
+00009f20: 7665 722d 7369 6465 2e0a 2020 2020 2020  ver-side..      
+00009f30: 2020 6966 2061 6c6c 2864 7479 7065 2069    if all(dtype i
+00009f40: 6e20 494e 4c49 4e41 424c 455f 4454 5950  n INLINABLE_DTYP
+00009f50: 4553 2066 6f72 2064 7479 7065 2069 6e20  ES for dtype in 
+00009f60: 696e 6c69 6e65 5f74 7970 6573 293a 0a20  inline_types):. 
+00009f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009f80: 6e20 696e 6c69 6e65 5f64 660a 2020 2020  n inline_df.    
+00009f90: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00009fa0: 0a20 2020 2064 6566 205f 7265 6164 5f70  .    def _read_p
+00009fb0: 616e 6461 735f 6c6f 6164 5f6a 6f62 280a  andas_load_job(.
+00009fc0: 2020 2020 2020 2020 7365 6c66 2c20 7061          self, pa
+00009fd0: 6e64 6173 5f64 6174 6166 7261 6d65 3a20  ndas_dataframe: 
+00009fe0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00009ff0: 2c20 6170 695f 6e61 6d65 3a20 7374 720a  , api_name: str.
+0000a000: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
+0000a010: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
+0000a020: 2020 2020 2020 696d 706f 7274 2062 6967        import big
+0000a030: 6672 616d 6573 2e64 6174 6166 7261 6d65  frames.dataframe
+0000a040: 2061 7320 6461 7461 6672 616d 650a 0a20   as dataframe.. 
+0000a050: 2020 2020 2020 2063 6f6c 5f69 6e64 6578         col_index
+0000a060: 203d 2070 616e 6461 735f 6461 7461 6672   = pandas_datafr
+0000a070: 616d 652e 636f 6c75 6d6e 732e 636f 7079  ame.columns.copy
+0000a080: 2829 0a20 2020 2020 2020 2063 6f6c 5f6c  ().        col_l
+0000a090: 6162 656c 732c 2069 6478 5f6c 6162 656c  abels, idx_label
+0000a0a0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
+0000a0b0: 2020 636f 6c5f 696e 6465 782e 746f 5f6c    col_index.to_l
+0000a0c0: 6973 7428 292c 0a20 2020 2020 2020 2020  ist(),.         
+0000a0d0: 2020 2070 616e 6461 735f 6461 7461 6672     pandas_datafr
+0000a0e0: 616d 652e 696e 6465 782e 6e61 6d65 732c  ame.index.names,
+0000a0f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000a100: 2020 206e 6577 5f63 6f6c 5f69 6473 2c20     new_col_ids, 
+0000a110: 6e65 775f 6964 785f 6964 7320 3d20 7574  new_idx_ids = ut
+0000a120: 696c 732e 6765 745f 7374 616e 6461 7264  ils.get_standard
+0000a130: 697a 6564 5f69 6473 280a 2020 2020 2020  ized_ids(.      
+0000a140: 2020 2020 2020 636f 6c5f 6c61 6265 6c73        col_labels
+0000a150: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
+0000a160: 785f 6c61 6265 6c73 2c0a 2020 2020 2020  x_labels,.      
+0000a170: 2020 2020 2020 2320 4c6f 6164 696e 6720        # Loading 
+0000a180: 7061 7271 7565 7420 6669 6c65 7320 696e  parquet files in
+0000a190: 746f 2042 6967 5175 6572 7920 7769 7468  to BigQuery with
+0000a1a0: 2073 7065 6369 616c 2063 6f6c 756d 6e20   special column 
+0000a1b0: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
+0000a1c0: 2020 2320 6973 206f 6e6c 7920 7375 7070    # is only supp
+0000a1d0: 6f72 7465 6420 756e 6465 7220 616e 2061  orted under an a
+0000a1e0: 6c6c 6f77 6c69 7374 2e0a 2020 2020 2020  llowlist..      
+0000a1f0: 2020 2020 2020 7374 7269 6374 3d54 7275        strict=Tru
+0000a200: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+0000a210: 2020 2020 2020 2320 4164 6420 6f72 6465        # Add orde
+0000a220: 7220 636f 6c75 6d6e 2074 6f20 7061 6e64  r column to pand
+0000a230: 6173 2044 6174 6146 7261 6d65 2074 6f20  as DataFrame to 
+0000a240: 7072 6573 6572 7665 206f 7264 6572 2069  preserve order i
+0000a250: 6e20 4269 6751 7565 7279 0a20 2020 2020  n BigQuery.     
+0000a260: 2020 206f 7264 6572 696e 675f 636f 6c20     ordering_col 
+0000a270: 3d20 2272 6f77 6964 220a 2020 2020 2020  = "rowid".      
+0000a280: 2020 636f 6c75 6d6e 7320 3d20 6672 6f7a    columns = froz
+0000a290: 656e 7365 7428 636f 6c5f 6c61 6265 6c73  enset(col_labels
+0000a2a0: 202b 2069 6478 5f6c 6162 656c 7329 0a20   + idx_labels). 
+0000a2b0: 2020 2020 2020 2073 7566 6669 7820 3d20         suffix = 
+0000a2c0: 320a 2020 2020 2020 2020 7768 696c 6520  2.        while 
+0000a2d0: 6f72 6465 7269 6e67 5f63 6f6c 2069 6e20  ordering_col in 
+0000a2e0: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+0000a2f0: 2020 2020 206f 7264 6572 696e 675f 636f       ordering_co
+0000a300: 6c20 3d20 6622 726f 7769 645f 7b73 7566  l = f"rowid_{suf
+0000a310: 6669 787d 220a 2020 2020 2020 2020 2020  fix}".          
+0000a320: 2020 7375 6666 6978 202b 3d20 310a 0a20    suffix += 1.. 
+0000a330: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
+0000a340: 7461 6672 616d 655f 636f 7079 203d 2070  taframe_copy = p
+0000a350: 616e 6461 735f 6461 7461 6672 616d 652e  andas_dataframe.
+0000a360: 636f 7079 2829 0a20 2020 2020 2020 2070  copy().        p
+0000a370: 616e 6461 735f 6461 7461 6672 616d 655f  andas_dataframe_
+0000a380: 636f 7079 2e69 6e64 6578 2e6e 616d 6573  copy.index.names
+0000a390: 203d 206e 6577 5f69 6478 5f69 6473 0a20   = new_idx_ids. 
+0000a3a0: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
+0000a3b0: 7461 6672 616d 655f 636f 7079 2e63 6f6c  taframe_copy.col
+0000a3c0: 756d 6e73 203d 2070 616e 6461 732e 496e  umns = pandas.In
+0000a3d0: 6465 7828 6e65 775f 636f 6c5f 6964 7329  dex(new_col_ids)
+0000a3e0: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
+0000a3f0: 6461 7461 6672 616d 655f 636f 7079 5b6f  dataframe_copy[o
+0000a400: 7264 6572 696e 675f 636f 6c5d 203d 206e  rdering_col] = n
+0000a410: 702e 6172 616e 6765 2870 616e 6461 735f  p.arange(pandas_
+0000a420: 6461 7461 6672 616d 655f 636f 7079 2e73  dataframe_copy.s
+0000a430: 6861 7065 5b30 5d29 0a0a 2020 2020 2020  hape[0])..      
+0000a440: 2020 6a6f 625f 636f 6e66 6967 203d 2073    job_config = s
+0000a450: 656c 662e 5f70 7265 7061 7265 5f6c 6f61  elf._prepare_loa
+0000a460: 645f 6a6f 625f 636f 6e66 6967 2829 0a0a  d_job_config()..
+0000a470: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
+0000a480: 7920 7468 6520 6461 7465 7469 6d65 2064  y the datetime d
+0000a490: 7479 7065 732c 2077 6869 6368 2069 7320  types, which is 
+0000a4a0: 6175 746f 2d64 6574 6563 7465 6420 6173  auto-detected as
+0000a4b0: 2074 696d 6573 7461 6d70 2074 7970 6573   timestamp types
+0000a4c0: 2e0a 2020 2020 2020 2020 7363 6865 6d61  ..        schema
+0000a4d0: 3a20 6c69 7374 5b62 6967 7175 6572 792e  : list[bigquery.
+0000a4e0: 5363 6865 6d61 4669 656c 645d 203d 205b  SchemaField] = [
+0000a4f0: 5d0a 2020 2020 2020 2020 666f 7220 636f  ].        for co
+0000a500: 6c75 6d6e 2c20 6474 7970 6520 696e 207a  lumn, dtype in z
+0000a510: 6970 286e 6577 5f63 6f6c 5f69 6473 2c20  ip(new_col_ids, 
+0000a520: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+0000a530: 2e64 7479 7065 7329 3a0a 2020 2020 2020  .dtypes):.      
+0000a540: 2020 2020 2020 6966 2064 7479 7065 203d        if dtype =
+0000a550: 3d20 2274 696d 6573 7461 6d70 5b75 735d  = "timestamp[us]
+0000a560: 5b70 7961 7272 6f77 5d22 3a0a 2020 2020  [pyarrow]":.    
+0000a570: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+0000a580: 6d61 2e61 7070 656e 6428 0a20 2020 2020  ma.append(.     
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000a5a0: 6967 7175 6572 792e 5363 6865 6d61 4669  igquery.SchemaFi
+0000a5b0: 656c 6428 636f 6c75 6d6e 2c20 6269 6771  eld(column, bigq
+0000a5c0: 7565 7279 2e65 6e75 6d73 2e53 716c 5479  uery.enums.SqlTy
+0000a5d0: 7065 4e61 6d65 732e 4441 5445 5449 4d45  peNames.DATETIME
+0000a5e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a5f0: 2020 290a 2020 2020 2020 2020 6a6f 625f    ).        job_
+0000a600: 636f 6e66 6967 2e73 6368 656d 6120 3d20  config.schema = 
+0000a610: 7363 6865 6d61 0a0a 2020 2020 2020 2020  schema..        
+0000a620: 2320 436c 7573 7465 7269 6e67 2070 726f  # Clustering pro
+0000a630: 6261 626c 7920 6e6f 7420 6e65 6564 6564  bably not needed
+0000a640: 2061 6e79 7761 7973 2061 7320 7061 6e64   anyways as pand
+0000a650: 6173 2074 6162 6c65 7320 6172 6520 736d  as tables are sm
+0000a660: 616c 6c0a 2020 2020 2020 2020 636c 7573  all.        clus
+0000a670: 7465 725f 636f 6c73 203d 205b 6f72 6465  ter_cols = [orde
+0000a680: 7269 6e67 5f63 6f6c 5d0a 2020 2020 2020  ring_col].      
+0000a690: 2020 6a6f 625f 636f 6e66 6967 2e63 6c75    job_config.clu
+0000a6a0: 7374 6572 696e 675f 6669 656c 6473 203d  stering_fields =
+0000a6b0: 2063 6c75 7374 6572 5f63 6f6c 730a 0a20   cluster_cols.. 
+0000a6c0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+0000a6d0: 672e 6c61 6265 6c73 203d 207b 2262 6967  g.labels = {"big
+0000a6e0: 6672 616d 6573 2d61 7069 223a 2061 7069  frames-api": api
+0000a6f0: 5f6e 616d 657d 0a0a 2020 2020 2020 2020  _name}..        
+0000a700: 6c6f 6164 5f74 6162 6c65 5f64 6573 7469  load_table_desti
+0000a710: 6e61 7469 6f6e 203d 2062 6967 6672 616d  nation = bigfram
+0000a720: 6573 5f69 6f2e 7261 6e64 6f6d 5f74 6162  es_io.random_tab
+0000a730: 6c65 2873 656c 662e 5f61 6e6f 6e79 6d6f  le(self._anonymo
+0000a740: 7573 5f64 6174 6173 6574 290a 2020 2020  us_dataset).    
+0000a750: 2020 2020 6c6f 6164 5f6a 6f62 203d 2073      load_job = s
+0000a760: 656c 662e 6271 636c 6965 6e74 2e6c 6f61  elf.bqclient.loa
+0000a770: 645f 7461 626c 655f 6672 6f6d 5f64 6174  d_table_from_dat
+0000a780: 6166 7261 6d65 280a 2020 2020 2020 2020  aframe(.        
+0000a790: 2020 2020 7061 6e64 6173 5f64 6174 6166      pandas_dataf
+0000a7a0: 7261 6d65 5f63 6f70 792c 0a20 2020 2020  rame_copy,.     
+0000a7b0: 2020 2020 2020 206c 6f61 645f 7461 626c         load_tabl
+0000a7c0: 655f 6465 7374 696e 6174 696f 6e2c 0a20  e_destination,. 
+0000a7d0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000a7e0: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
+0000a7f0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0000a800: 2020 2020 7365 6c66 2e5f 7374 6172 745f      self._start_
+0000a810: 6765 6e65 7269 635f 6a6f 6228 6c6f 6164  generic_job(load
+0000a820: 5f6a 6f62 290a 0a20 2020 2020 2020 206f  _job)..        o
+0000a830: 7264 6572 696e 6720 3d20 6f72 6465 722e  rdering = order.
+0000a840: 4578 7072 6573 7369 6f6e 4f72 6465 7269  ExpressionOrderi
+0000a850: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000a860: 6f72 6465 7269 6e67 5f76 616c 7565 5f63  ordering_value_c
+0000a870: 6f6c 756d 6e73 3d74 7570 6c65 285b 6f72  olumns=tuple([or
+0000a880: 6465 722e 6173 6365 6e64 696e 675f 6f76  der.ascending_ov
+0000a890: 6572 286f 7264 6572 696e 675f 636f 6c29  er(ordering_col)
+0000a8a0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0000a8b0: 746f 7461 6c5f 6f72 6465 7269 6e67 5f63  total_ordering_c
+0000a8c0: 6f6c 756d 6e73 3d66 726f 7a65 6e73 6574  olumns=frozenset
+0000a8d0: 285b 6f72 6465 7269 6e67 5f63 6f6c 5d29  ([ordering_col])
+0000a8e0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+0000a8f0: 7465 6765 725f 656e 636f 6469 6e67 3d49  teger_encoding=I
+0000a900: 6e74 6567 6572 456e 636f 6469 6e67 2854  ntegerEncoding(T
+0000a910: 7275 652c 2069 735f 7365 7175 656e 7469  rue, is_sequenti
+0000a920: 616c 3d54 7275 6529 2c0a 2020 2020 2020  al=True),.      
+0000a930: 2020 290a 2020 2020 2020 2020 7461 626c    ).        tabl
+0000a940: 655f 6578 7072 6573 7369 6f6e 203d 2073  e_expression = s
+0000a950: 656c 662e 6962 6973 5f63 6c69 656e 742e  elf.ibis_client.
+0000a960: 7461 626c 6528 2020 2320 7479 7065 3a20  table(  # type: 
+0000a970: 6967 6e6f 7265 0a20 2020 2020 2020 2020  ignore.         
+0000a980: 2020 206c 6f61 645f 7461 626c 655f 6465     load_table_de
+0000a990: 7374 696e 6174 696f 6e2e 7461 626c 655f  stination.table_
+0000a9a0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000a9b0: 7363 6865 6d61 3d6c 6f61 645f 7461 626c  schema=load_tabl
+0000a9c0: 655f 6465 7374 696e 6174 696f 6e2e 6461  e_destination.da
+0000a9d0: 7461 7365 745f 6964 2c0a 2020 2020 2020  taset_id,.      
+0000a9e0: 2020 2020 2020 6461 7461 6261 7365 3d6c        database=l
+0000a9f0: 6f61 645f 7461 626c 655f 6465 7374 696e  oad_table_destin
+0000aa00: 6174 696f 6e2e 7072 6f6a 6563 742c 0a20  ation.project,. 
+0000aa10: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000aa20: 2020 2320 622f 3239 3735 3930 3137 3820    # b/297590178 
+0000aa30: 506f 7465 6e74 6961 6c6c 7920 6120 6275  Potentially a bu
+0000aa40: 6720 696e 2062 7163 6c69 656e 742e 6c6f  g in bqclient.lo
+0000aa50: 6164 5f74 6162 6c65 5f66 726f 6d5f 6461  ad_table_from_da
+0000aa60: 7461 6672 616d 6528 292c 2074 6861 7420  taframe(), that 
+0000aa70: 6f6e 6c79 2077 6865 6e20 7468 6520 4446  only when the DF
+0000aa80: 2069 7320 656d 7074 792c 2074 6865 2069   is empty, the i
+0000aa90: 6e64 6578 2063 6f6c 756d 6e73 2064 6973  ndex columns dis
+0000aaa0: 6170 7065 6172 2069 6e20 7461 626c 655f  appear in table_
+0000aab0: 6578 7072 6573 7369 6f6e 2e0a 2020 2020  expression..    
+0000aac0: 2020 2020 6966 2061 6e79 280a 2020 2020      if any(.    
+0000aad0: 2020 2020 2020 2020 5b6e 6577 5f69 6478          [new_idx
+0000aae0: 5f69 6420 6e6f 7420 696e 2074 6162 6c65  _id not in table
+0000aaf0: 5f65 7870 7265 7373 696f 6e2e 636f 6c75  _expression.colu
+0000ab00: 6d6e 7320 666f 7220 6e65 775f 6964 785f  mns for new_idx_
+0000ab10: 6964 2069 6e20 6e65 775f 6964 785f 6964  id in new_idx_id
+0000ab20: 735d 0a20 2020 2020 2020 2029 3a0a 2020  s].        ):.  
+0000ab30: 2020 2020 2020 2020 2020 6e65 775f 6964            new_id
+0000ab40: 785f 6964 732c 2069 6478 5f6c 6162 656c  x_ids, idx_label
+0000ab50: 7320 3d20 5b5d 2c20 5b5d 0a0a 2020 2020  s = [], []..    
+0000ab60: 2020 2020 636f 6c75 6d6e 5f76 616c 7565      column_value
+0000ab70: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+0000ab80: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
+0000ab90: 6f6e 5b63 6f6c 5d0a 2020 2020 2020 2020  on[col].        
+0000aba0: 2020 2020 666f 7220 636f 6c20 696e 2074      for col in t
+0000abb0: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
+0000abc0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+0000abd0: 2020 2020 6966 2063 6f6c 2021 3d20 6f72      if col != or
+0000abe0: 6465 7269 6e67 5f63 6f6c 0a20 2020 2020  dering_col.     
+0000abf0: 2020 205d 0a20 2020 2020 2020 2061 7272     ].        arr
+0000ac00: 6179 5f76 616c 7565 203d 2063 6f72 652e  ay_value = core.
+0000ac10: 4172 7261 7956 616c 7565 2e66 726f 6d5f  ArrayValue.from_
+0000ac20: 6962 6973 280a 2020 2020 2020 2020 2020  ibis(.          
+0000ac30: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000ac40: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
+0000ac50: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+0000ac60: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
+0000ac70: 5f76 616c 7565 732c 0a20 2020 2020 2020  _values,.       
+0000ac80: 2020 2020 2068 6964 6465 6e5f 6f72 6465       hidden_orde
+0000ac90: 7269 6e67 5f63 6f6c 756d 6e73 3d5b 7461  ring_columns=[ta
+0000aca0: 626c 655f 6578 7072 6573 7369 6f6e 5b6f  ble_expression[o
+0000acb0: 7264 6572 696e 675f 636f 6c5d 5d2c 0a20  rdering_col]],. 
+0000acc0: 2020 2020 2020 2020 2020 206f 7264 6572             order
+0000acd0: 696e 673d 6f72 6465 7269 6e67 2c0a 2020  ing=ordering,.  
+0000ace0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000acf0: 2062 6c6f 636b 203d 2062 6c6f 636b 732e   block = blocks.
+0000ad00: 426c 6f63 6b28 0a20 2020 2020 2020 2020  Block(.         
+0000ad10: 2020 2061 7272 6179 5f76 616c 7565 2c0a     array_value,.
+0000ad20: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000ad30: 785f 636f 6c75 6d6e 733d 6e65 775f 6964  x_columns=new_id
+0000ad40: 785f 6964 732c 0a20 2020 2020 2020 2020  x_ids,.         
+0000ad50: 2020 2063 6f6c 756d 6e5f 6c61 6265 6c73     column_labels
+0000ad60: 3d63 6f6c 5f69 6e64 6578 2c0a 2020 2020  =col_index,.    
+0000ad70: 2020 2020 2020 2020 696e 6465 785f 6c61          index_la
+0000ad80: 6265 6c73 3d69 6478 5f6c 6162 656c 732c  bels=idx_labels,
+0000ad90: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000ada0: 2020 2072 6574 7572 6e20 6461 7461 6672     return datafr
+0000adb0: 616d 652e 4461 7461 4672 616d 6528 626c  ame.DataFrame(bl
+0000adc0: 6f63 6b29 0a0a 2020 2020 6465 6620 7265  ock)..    def re
+0000add0: 6164 5f63 7376 280a 2020 2020 2020 2020  ad_csv(.        
+0000ade0: 7365 6c66 2c0a 2020 2020 2020 2020 6669  self,.        fi
+0000adf0: 6c65 7061 7468 5f6f 725f 6275 6666 6572  lepath_or_buffer
+0000ae00: 3a20 7374 7220 7c20 494f 5b22 6279 7465  : str | IO["byte
+0000ae10: 7322 5d2c 0a20 2020 2020 2020 202a 2c0a  s"],.        *,.
+0000ae20: 2020 2020 2020 2020 7365 703a 204f 7074          sep: Opt
+0000ae30: 696f 6e61 6c5b 7374 725d 203d 2022 2c22  ional[str] = ","
+0000ae40: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0000ae50: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0000ae60: 3d20 302c 0a20 2020 2020 2020 206e 616d  = 0,.        nam
+0000ae70: 6573 3a20 4f70 7469 6f6e 616c 5b0a 2020  es: Optional[.  
+0000ae80: 2020 2020 2020 2020 2020 556e 696f 6e5b            Union[
+0000ae90: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
+0000aea0: 416e 795d 2c20 6e70 2e6e 6461 7272 6179  Any], np.ndarray
+0000aeb0: 5b41 6e79 2c20 416e 795d 2c20 5475 706c  [Any, Any], Tupl
+0000aec0: 655b 416e 792c 202e 2e2e 5d2c 2072 616e  e[Any, ...], ran
+0000aed0: 6765 5d0a 2020 2020 2020 2020 5d20 3d20  ge].        ] = 
+0000aee0: 4e6f 6e65 2c0a 2020 2020 2020 2020 696e  None,.        in
+0000aef0: 6465 785f 636f 6c3a 204f 7074 696f 6e61  dex_col: Optiona
+0000af00: 6c5b 0a20 2020 2020 2020 2020 2020 2055  l[.            U
+0000af10: 6e69 6f6e 5b69 6e74 2c20 7374 722c 2053  nion[int, str, S
+0000af20: 6571 7565 6e63 655b 556e 696f 6e5b 7374  equence[Union[st
+0000af30: 722c 2069 6e74 5d5d 2c20 4c69 7465 7261  r, int]], Litera
+0000af40: 6c5b 4661 6c73 655d 5d0a 2020 2020 2020  l[False]].      
+0000af50: 2020 5d20 3d20 4e6f 6e65 2c0a 2020 2020    ] = None,.    
+0000af60: 2020 2020 7573 6563 6f6c 733a 204f 7074      usecols: Opt
+0000af70: 696f 6e61 6c5b 0a20 2020 2020 2020 2020  ional[.         
+0000af80: 2020 2055 6e69 6f6e 5b0a 2020 2020 2020     Union[.      
+0000af90: 2020 2020 2020 2020 2020 4d75 7461 626c            Mutabl
+0000afa0: 6553 6571 7565 6e63 655b 7374 725d 2c0a  eSequence[str],.
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afc0: 5475 706c 655b 7374 722c 202e 2e2e 5d2c  Tuple[str, ...],
+0000afd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000afe0: 2053 6571 7565 6e63 655b 696e 745d 2c0a   Sequence[int],.
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 7061 6e64 6173 2e53 6572 6965 732c 0a20  pandas.Series,. 
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b020: 616e 6461 732e 496e 6465 782c 0a20 2020  andas.Index,.   
+0000b030: 2020 2020 2020 2020 2020 2020 206e 702e               np.
+0000b040: 6e64 6172 7261 795b 416e 792c 2041 6e79  ndarray[Any, Any
+0000b050: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000b060: 2020 2043 616c 6c61 626c 655b 5b41 6e79     Callable[[Any
+0000b070: 5d2c 2062 6f6f 6c5d 2c0a 2020 2020 2020  ], bool],.      
+0000b080: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000b090: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000b0a0: 2020 6474 7970 653a 204f 7074 696f 6e61    dtype: Optiona
+0000b0b0: 6c5b 4469 6374 5d20 3d20 4e6f 6e65 2c0a  l[Dict] = None,.
+0000b0c0: 2020 2020 2020 2020 656e 6769 6e65 3a20          engine: 
+0000b0d0: 4f70 7469 6f6e 616c 5b0a 2020 2020 2020  Optional[.      
+0000b0e0: 2020 2020 2020 4c69 7465 7261 6c5b 2263        Literal["c
+0000b0f0: 222c 2022 7079 7468 6f6e 222c 2022 7079  ", "python", "py
+0000b100: 6172 726f 7722 2c20 2270 7974 686f 6e2d  arrow", "python-
+0000b110: 6677 6622 2c20 2262 6967 7175 6572 7922  fwf", "bigquery"
+0000b120: 5d0a 2020 2020 2020 2020 5d20 3d20 4e6f  ].        ] = No
+0000b130: 6e65 2c0a 2020 2020 2020 2020 656e 636f  ne,.        enco
+0000b140: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
+0000b150: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000b160: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
+0000b170: 2020 2920 2d3e 2064 6174 6166 7261 6d65    ) -> dataframe
+0000b180: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
+0000b190: 2020 2020 7461 626c 6520 3d20 6269 6766      table = bigf
+0000b1a0: 7261 6d65 735f 696f 2e72 616e 646f 6d5f  rames_io.random_
+0000b1b0: 7461 626c 6528 7365 6c66 2e5f 616e 6f6e  table(self._anon
+0000b1c0: 796d 6f75 735f 6461 7461 7365 7429 0a0a  ymous_dataset)..
+0000b1d0: 2020 2020 2020 2020 6966 2065 6e67 696e          if engin
+0000b1e0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+0000b1f0: 6420 656e 6769 6e65 203d 3d20 2262 6967  d engine == "big
+0000b200: 7175 6572 7922 3a0a 2020 2020 2020 2020  query":.        
+0000b210: 2020 2020 6966 2061 6e79 2870 6172 616d      if any(param
+0000b220: 2069 7320 6e6f 7420 4e6f 6e65 2066 6f72   is not None for
+0000b230: 2070 6172 616d 2069 6e20 2864 7479 7065   param in (dtype
+0000b240: 2c20 6e61 6d65 7329 293a 0a20 2020 2020  , names)):.     
+0000b250: 2020 2020 2020 2020 2020 206e 6f74 5f73             not_s
+0000b260: 7570 706f 7274 6564 203d 2028 2264 7479  upported = ("dty
+0000b270: 7065 222c 2022 6e61 6d65 7322 290a 2020  pe", "names").  
+0000b280: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000b290: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+0000b2a0: 6564 4572 726f 7228 0a20 2020 2020 2020  edError(.       
+0000b2b0: 2020 2020 2020 2020 2020 2020 2066 2242               f"B
+0000b2c0: 6967 5175 6572 7920 656e 6769 6e65 2064  igQuery engine d
+0000b2d0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+0000b2e0: 7468 6573 6520 6172 6775 6d65 6e74 733a  these arguments:
+0000b2f0: 207b 6e6f 745f 7375 7070 6f72 7465 647d   {not_supported}
+0000b300: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+0000b310: 2020 2020 2020 2020 6622 7b63 6f6e 7374          f"{const
+0000b320: 616e 7473 2e46 4545 4442 4143 4b5f 4c49  ants.FEEDBACK_LI
+0000b330: 4e4b 7d22 0a20 2020 2020 2020 2020 2020  NK}".           
+0000b340: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b350: 2020 2020 6966 2069 6e64 6578 5f63 6f6c      if index_col
+0000b360: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000b370: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000b380: 2020 206e 6f74 2069 6e64 6578 5f63 6f6c     not index_col
+0000b390: 206f 7220 6e6f 7420 6973 696e 7374 616e   or not isinstan
+0000b3a0: 6365 2869 6e64 6578 5f63 6f6c 2c20 7374  ce(index_col, st
+0000b3b0: 7229 0a20 2020 2020 2020 2020 2020 2029  r).            )
+0000b3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b3d0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000b3e0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 2022 4269 6751 7565 7279 2065 6e67 696e   "BigQuery engin
+0000b410: 6520 6f6e 6c79 2073 7570 706f 7274 7320  e only supports 
+0000b420: 6120 7369 6e67 6c65 2063 6f6c 756d 6e20  a single column 
+0000b430: 6e61 6d65 2066 6f72 2060 696e 6465 785f  name for `index_
+0000b440: 636f 6c60 2e20 220a 2020 2020 2020 2020  col`. ".        
+0000b450: 2020 2020 2020 2020 2020 2020 6622 7b63              f"{c
+0000b460: 6f6e 7374 616e 7473 2e46 4545 4442 4143  onstants.FEEDBAC
+0000b470: 4b5f 4c49 4e4b 7d22 0a20 2020 2020 2020  K_LINK}".       
+0000b480: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000b490: 2020 2020 2020 2020 2320 4e6f 6e65 2076          # None v
+0000b4a0: 616c 7565 2066 6f72 2069 6e64 6578 5f63  alue for index_c
+0000b4b0: 6f6c 2063 616e 6e6f 7420 6265 2070 6173  ol cannot be pas
+0000b4c0: 7365 6420 746f 2072 6561 645f 6762 710a  sed to read_gbq.
+0000b4d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000b4e0: 6e64 6578 5f63 6f6c 2069 7320 4e6f 6e65  ndex_col is None
+0000b4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b500: 2020 696e 6465 785f 636f 6c20 3d20 2829    index_col = ()
+0000b510: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000b520: 7573 6563 6f6c 7320 7368 6f75 6c64 206f  usecols should o
+0000b530: 6e6c 7920 6265 2061 6e20 6974 6572 6162  nly be an iterab
+0000b540: 6c65 206f 6620 7374 7269 6e67 7320 2863  le of strings (c
+0000b550: 6f6c 756d 6e20 6e61 6d65 7329 2066 6f72  olumn names) for
+0000b560: 2075 7365 2061 7320 636f 6c75 6d6e 7320   use as columns 
+0000b570: 696e 2072 6561 645f 6762 712e 0a20 2020  in read_gbq..   
+0000b580: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+0000b590: 3a20 5475 706c 655b 416e 792c 202e 2e2e  : Tuple[Any, ...
+0000b5a0: 5d20 3d20 7475 706c 6528 290a 2020 2020  ] = tuple().    
+0000b5b0: 2020 2020 2020 2020 6966 2075 7365 636f          if useco
+0000b5c0: 6c73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ls is not None:.
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 6966 2069 7369 6e73 7461 6e63 6528 7573  if isinstance(us
+0000b5f0: 6563 6f6c 732c 2049 7465 7261 626c 6529  ecols, Iterable)
+0000b600: 2061 6e64 2061 6c6c 280a 2020 2020 2020   and all(.      
+0000b610: 2020 2020 2020 2020 2020 2020 2020 6973                is
+0000b620: 696e 7374 616e 6365 2863 6f6c 2c20 7374  instance(col, st
+0000b630: 7229 2066 6f72 2063 6f6c 2069 6e20 7573  r) for col in us
+0000b640: 6563 6f6c 730a 2020 2020 2020 2020 2020  ecols.          
+0000b650: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000b660: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0000b670: 756d 6e73 203d 2074 7570 6c65 2863 6f6c  umns = tuple(col
+0000b680: 2066 6f72 2063 6f6c 2069 6e20 7573 6563   for col in usec
+0000b690: 6f6c 7329 0a20 2020 2020 2020 2020 2020  ols).           
+0000b6a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b6c0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+0000b6d0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 2242 6967 5175 6572 7920 656e 6769    "BigQuery engi
+0000b700: 6e65 206f 6e6c 7920 7375 7070 6f72 7473  ne only supports
+0000b710: 2061 6e20 6974 6572 6162 6c65 206f 6620   an iterable of 
+0000b720: 7374 7269 6e67 7320 666f 7220 6075 7365  strings for `use
+0000b730: 636f 6c73 602e 2022 0a20 2020 2020 2020  cols`. ".       
+0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b750: 2066 227b 636f 6e73 7461 6e74 732e 4645   f"{constants.FE
+0000b760: 4544 4241 434b 5f4c 494e 4b7d 220a 2020  EDBACK_LINK}".  
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000b790: 2069 6620 656e 636f 6469 6e67 2069 7320   if encoding is 
+0000b7a0: 6e6f 7420 4e6f 6e65 2061 6e64 2065 6e63  not None and enc
+0000b7b0: 6f64 696e 6720 6e6f 7420 696e 205f 5641  oding not in _VA
+0000b7c0: 4c49 445f 454e 434f 4449 4e47 533a 0a20  LID_ENCODINGS:. 
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b7e0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+0000b7f0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
+0000b800: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000b810: 4269 6751 7565 7279 2065 6e67 696e 6520  BigQuery engine 
+0000b820: 6f6e 6c79 2073 7570 706f 7274 7320 7468  only supports th
+0000b830: 6520 666f 6c6c 6f77 696e 6720 656e 636f  e following enco
+0000b840: 6469 6e67 733a 207b 5f56 414c 4944 5f45  dings: {_VALID_E
+0000b850: 4e43 4f44 494e 4753 7d2e 2022 0a20 2020  NCODINGS}. ".   
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2066 227b 636f 6e73 7461 6e74 732e 4645   f"{constants.FE
+0000b880: 4544 4241 434b 5f4c 494e 4b7d 220a 2020  EDBACK_LINK}".  
+0000b890: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000b8a0: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+0000b8b0: 5f63 6f6e 6669 6720 3d20 7365 6c66 2e5f  _config = self._
+0000b8c0: 7072 6570 6172 655f 6c6f 6164 5f6a 6f62  prepare_load_job
+0000b8d0: 5f63 6f6e 6669 6728 290a 2020 2020 2020  _config().      
+0000b8e0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+0000b8f0: 2e63 7265 6174 655f 6469 7370 6f73 6974  .create_disposit
+0000b900: 696f 6e20 3d20 6269 6771 7565 7279 2e43  ion = bigquery.C
+0000b910: 7265 6174 6544 6973 706f 7369 7469 6f6e  reateDisposition
+0000b920: 2e43 5245 4154 455f 4946 5f4e 4545 4445  .CREATE_IF_NEEDE
+0000b930: 440a 2020 2020 2020 2020 2020 2020 6a6f  D.            jo
+0000b940: 625f 636f 6e66 6967 2e73 6f75 7263 655f  b_config.source_
+0000b950: 666f 726d 6174 203d 2062 6967 7175 6572  format = bigquer
+0000b960: 792e 536f 7572 6365 466f 726d 6174 2e43  y.SourceFormat.C
+0000b970: 5356 0a20 2020 2020 2020 2020 2020 206a  SV.            j
+0000b980: 6f62 5f63 6f6e 6669 672e 7772 6974 655f  ob_config.write_
+0000b990: 6469 7370 6f73 6974 696f 6e20 3d20 6269  disposition = bi
+0000b9a0: 6771 7565 7279 2e57 7269 7465 4469 7370  gquery.WriteDisp
+0000b9b0: 6f73 6974 696f 6e2e 5752 4954 455f 454d  osition.WRITE_EM
+0000b9c0: 5054 590a 2020 2020 2020 2020 2020 2020  PTY.            
+0000b9d0: 6a6f 625f 636f 6e66 6967 2e61 7574 6f64  job_config.autod
+0000b9e0: 6574 6563 7420 3d20 5472 7565 0a20 2020  etect = True.   
+0000b9f0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000ba00: 6669 672e 6669 656c 645f 6465 6c69 6d69  fig.field_delimi
+0000ba10: 7465 7220 3d20 7365 700a 2020 2020 2020  ter = sep.      
+0000ba20: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+0000ba30: 2e65 6e63 6f64 696e 6720 3d20 656e 636f  .encoding = enco
+0000ba40: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
+0000ba50: 206a 6f62 5f63 6f6e 6669 672e 6c61 6265   job_config.labe
+0000ba60: 6c73 203d 207b 2262 6967 6672 616d 6573  ls = {"bigframes
+0000ba70: 2d61 7069 223a 2022 7265 6164 5f63 7376  -api": "read_csv
+0000ba80: 227d 0a0a 2020 2020 2020 2020 2020 2020  "}..            
+0000ba90: 2320 5765 2077 616e 7420 746f 206d 6174  # We want to mat
+0000baa0: 6368 2070 616e 6461 7320 6265 6861 7669  ch pandas behavi
+0000bab0: 6f72 2e20 4966 2068 6561 6465 7220 6973  or. If header is
+0000bac0: 2030 2c20 6e6f 2072 6f77 7320 7368 6f75   0, no rows shou
+0000bad0: 6c64 2062 6520 736b 6970 7065 642c 2073  ld be skipped, s
+0000bae0: 6f20 7765 0a20 2020 2020 2020 2020 2020  o we.           
+0000baf0: 2023 2064 6f20 6e6f 7420 6e65 6564 2074   # do not need t
+0000bb00: 6f20 7365 7420 6073 6b69 705f 6c65 6164  o set `skip_lead
+0000bb10: 696e 675f 726f 7773 602e 2049 6620 6865  ing_rows`. If he
+0000bb20: 6164 6572 2069 7320 4e6f 6e65 2c20 7468  ader is None, th
+0000bb30: 656e 2074 6865 7265 2069 7320 6e6f 2068  en there is no h
+0000bb40: 6561 6465 722e 0a20 2020 2020 2020 2020  eader..         
+0000bb50: 2020 2023 2053 6574 7469 6e67 2073 6b69     # Setting ski
+0000bb60: 705f 6c65 6164 696e 675f 726f 7773 2074  p_leading_rows t
+0000bb70: 6f20 3020 646f 6573 2074 6861 742e 2049  o 0 does that. I
+0000bb80: 6620 6865 6164 6572 3d4e 2061 6e64 204e  f header=N and N
+0000bb90: 3e30 2c20 7765 2077 616e 7420 746f 2073  >0, we want to s
+0000bba0: 6b69 7020 4e20 726f 7773 2e0a 2020 2020  kip N rows..    
+0000bbb0: 2020 2020 2020 2020 6966 2068 6561 6465          if heade
+0000bbc0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+0000bbd0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000bbe0: 6f6e 6669 672e 736b 6970 5f6c 6561 6469  onfig.skip_leadi
+0000bbf0: 6e67 5f72 6f77 7320 3d20 300a 2020 2020  ng_rows = 0.    
+0000bc00: 2020 2020 2020 2020 656c 6966 2068 6561          elif hea
+0000bc10: 6465 7220 3e20 303a 0a20 2020 2020 2020  der > 0:.       
+0000bc20: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000bc30: 6669 672e 736b 6970 5f6c 6561 6469 6e67  fig.skip_leading
+0000bc40: 5f72 6f77 7320 3d20 6865 6164 6572 0a0a  _rows = header..
+0000bc50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bc60: 726e 2073 656c 662e 5f72 6561 645f 6269  rn self._read_bi
+0000bc70: 6771 7565 7279 5f6c 6f61 645f 6a6f 6228  gquery_load_job(
+0000bc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc90: 2066 696c 6570 6174 685f 6f72 5f62 7566   filepath_or_buf
+0000bca0: 6665 722c 0a20 2020 2020 2020 2020 2020  fer,.           
+0000bcb0: 2020 2020 2074 6162 6c65 2c0a 2020 2020       table,.    
+0000bcc0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+0000bcd0: 636f 6e66 6967 3d6a 6f62 5f63 6f6e 6669  config=job_confi
+0000bce0: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+0000bcf0: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
+0000bd00: 6578 5f63 6f6c 2c0a 2020 2020 2020 2020  ex_col,.        
+0000bd10: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
+0000bd20: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
+0000bd30: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+0000bd40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000bd50: 2069 6620 616e 7928 6172 6720 696e 206b   if any(arg in k
+0000bd60: 7761 7267 7320 666f 7220 6172 6720 696e  wargs for arg in
+0000bd70: 2028 2263 6875 6e6b 7369 7a65 222c 2022   ("chunksize", "
+0000bd80: 6974 6572 6174 6f72 2229 293a 0a20 2020  iterator")):.   
+0000bd90: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000bda0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+0000bdb0: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
+0000bdc0: 2020 2020 2020 2020 2020 2020 2227 6368              "'ch
+0000bdd0: 756e 6b73 697a 6527 2061 6e64 2027 6974  unksize' and 'it
+0000bde0: 6572 6174 6f72 2720 6172 6775 6d65 6e74  erator' argument
+0000bdf0: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
+0000be00: 7465 642e 2022 0a20 2020 2020 2020 2020  ted. ".         
+0000be10: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
+0000be20: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
+0000be30: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
+0000be40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000be50: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000be60: 616e 6365 2866 696c 6570 6174 685f 6f72  ance(filepath_or
+0000be70: 5f62 7566 6665 722c 2073 7472 293a 0a20  _buffer, str):. 
+0000be80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000be90: 656c 662e 5f63 6865 636b 5f66 696c 655f  elf._check_file_
+0000bea0: 7369 7a65 2866 696c 6570 6174 685f 6f72  size(filepath_or
+0000beb0: 5f62 7566 6665 7229 0a20 2020 2020 2020  _buffer).       
+0000bec0: 2020 2020 2070 616e 6461 735f 6466 203d       pandas_df =
+0000bed0: 2070 616e 6461 732e 7265 6164 5f63 7376   pandas.read_csv
+0000bee0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000bef0: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
+0000bf00: 6666 6572 2c0a 2020 2020 2020 2020 2020  ffer,.          
+0000bf10: 2020 2020 2020 7365 703d 7365 702c 0a20        sep=sep,. 
+0000bf20: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000bf30: 6561 6465 723d 6865 6164 6572 2c0a 2020  eader=header,.  
+0000bf40: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+0000bf50: 6d65 733d 6e61 6d65 732c 0a20 2020 2020  mes=names,.     
+0000bf60: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0000bf70: 5f63 6f6c 3d69 6e64 6578 5f63 6f6c 2c0a  _col=index_col,.
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 7573 6563 6f6c 733d 7573 6563 6f6c 732c  usecols=usecols,
+0000bfa0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+0000bfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bfc0: 2064 7479 7065 3d64 7479 7065 2c0a 2020   dtype=dtype,.  
+0000bfd0: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000bfe0: 6769 6e65 3d65 6e67 696e 652c 0a20 2020  gine=engine,.   
+0000bff0: 2020 2020 2020 2020 2020 2020 2065 6e63               enc
+0000c000: 6f64 696e 673d 656e 636f 6469 6e67 2c0a  oding=encoding,.
+0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c020: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
+0000c030: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000c040: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000c050: 5f72 6561 645f 7061 6e64 6173 2870 616e  _read_pandas(pan
+0000c060: 6461 735f 6466 2c20 2272 6561 645f 6373  das_df, "read_cs
+0000c070: 7622 2920 2023 2074 7970 653a 2069 676e  v")  # type: ign
+0000c080: 6f72 650a 0a20 2020 2064 6566 2072 6561  ore..    def rea
+0000c090: 645f 7069 636b 6c65 280a 2020 2020 2020  d_pickle(.      
+0000c0a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000c0b0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+0000c0c0: 6572 3a20 4669 6c65 5061 7468 207c 2052  er: FilePath | R
+0000c0d0: 6561 6450 6963 6b6c 6542 7566 6665 722c  eadPickleBuffer,
+0000c0e0: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
+0000c0f0: 7369 6f6e 3a20 436f 6d70 7265 7373 696f  sion: Compressio
+0000c100: 6e4f 7074 696f 6e73 203d 2022 696e 6665  nOptions = "infe
+0000c110: 7222 2c0a 2020 2020 2020 2020 7374 6f72  r",.        stor
+0000c120: 6167 655f 6f70 7469 6f6e 733a 2053 746f  age_options: Sto
+0000c130: 7261 6765 4f70 7469 6f6e 7320 3d20 4e6f  rageOptions = No
+0000c140: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0000c150: 2020 2070 616e 6461 735f 6f62 6a20 3d20     pandas_obj = 
+0000c160: 7061 6e64 6173 2e72 6561 645f 7069 636b  pandas.read_pick
+0000c170: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+0000c180: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+0000c190: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000c1a0: 636f 6d70 7265 7373 696f 6e3d 636f 6d70  compression=comp
+0000c1b0: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
+0000c1c0: 2020 2020 2073 746f 7261 6765 5f6f 7074       storage_opt
+0000c1d0: 696f 6e73 3d73 746f 7261 6765 5f6f 7074  ions=storage_opt
+0000c1e0: 696f 6e73 2c0a 2020 2020 2020 2020 290a  ions,.        ).
+0000c1f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0000c200: 7374 616e 6365 2870 616e 6461 735f 6f62  stance(pandas_ob
+0000c210: 6a2c 2070 616e 6461 732e 5365 7269 6573  j, pandas.Series
+0000c220: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000c230: 6620 7061 6e64 6173 5f6f 626a 2e6e 616d  f pandas_obj.nam
+0000c240: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+0000c250: 2020 2020 2020 2020 2020 2070 616e 6461             panda
+0000c260: 735f 6f62 6a2e 6e61 6d65 203d 2022 3022  s_obj.name = "0"
+0000c270: 0a20 2020 2020 2020 2020 2020 2062 6967  .            big
+0000c280: 6672 616d 6573 5f64 6620 3d20 7365 6c66  frames_df = self
+0000c290: 2e5f 7265 6164 5f70 616e 6461 7328 7061  ._read_pandas(pa
+0000c2a0: 6e64 6173 5f6f 626a 2e74 6f5f 6672 616d  ndas_obj.to_fram
+0000c2b0: 6528 292c 2022 7265 6164 5f70 6963 6b6c  e(), "read_pickl
+0000c2c0: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+0000c2d0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
+0000c2e0: 5f64 665b 6269 6766 7261 6d65 735f 6466  _df[bigframes_df
+0000c2f0: 2e63 6f6c 756d 6e73 5b30 5d5d 0a20 2020  .columns[0]].   
+0000c300: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000c310: 2e5f 7265 6164 5f70 616e 6461 7328 7061  ._read_pandas(pa
+0000c320: 6e64 6173 5f6f 626a 2c20 2272 6561 645f  ndas_obj, "read_
+0000c330: 7069 636b 6c65 2229 0a0a 2020 2020 6465  pickle")..    de
+0000c340: 6620 7265 6164 5f70 6172 7175 6574 280a  f read_parquet(.
+0000c350: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000c360: 2020 2020 2020 7061 7468 3a20 7374 7220        path: str 
+0000c370: 7c20 494f 5b22 6279 7465 7322 5d2c 0a20  | IO["bytes"],. 
+0000c380: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0000c390: 2020 656e 6769 6e65 3a20 7374 7220 3d20    engine: str = 
+0000c3a0: 2261 7574 6f22 2c0a 2020 2020 2920 2d3e  "auto",.    ) ->
+0000c3b0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
+0000c3c0: 7261 6d65 3a0a 2020 2020 2020 2020 7461  rame:.        ta
+0000c3d0: 626c 6520 3d20 6269 6766 7261 6d65 735f  ble = bigframes_
+0000c3e0: 696f 2e72 616e 646f 6d5f 7461 626c 6528  io.random_table(
+0000c3f0: 7365 6c66 2e5f 616e 6f6e 796d 6f75 735f  self._anonymous_
+0000c400: 6461 7461 7365 7429 0a0a 2020 2020 2020  dataset)..      
+0000c410: 2020 6966 2065 6e67 696e 6520 3d3d 2022    if engine == "
+0000c420: 6269 6771 7565 7279 223a 0a20 2020 2020  bigquery":.     
+0000c430: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+0000c440: 6720 3d20 7365 6c66 2e5f 7072 6570 6172  g = self._prepar
+0000c450: 655f 6c6f 6164 5f6a 6f62 5f63 6f6e 6669  e_load_job_confi
+0000c460: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+0000c470: 6a6f 625f 636f 6e66 6967 2e63 7265 6174  job_config.creat
+0000c480: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
+0000c490: 6269 6771 7565 7279 2e43 7265 6174 6544  bigquery.CreateD
+0000c4a0: 6973 706f 7369 7469 6f6e 2e43 5245 4154  isposition.CREAT
+0000c4b0: 455f 4946 5f4e 4545 4445 440a 2020 2020  E_IF_NEEDED.    
+0000c4c0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000c4d0: 6967 2e73 6f75 7263 655f 666f 726d 6174  ig.source_format
+0000c4e0: 203d 2062 6967 7175 6572 792e 536f 7572   = bigquery.Sour
+0000c4f0: 6365 466f 726d 6174 2e50 4152 5155 4554  ceFormat.PARQUET
+0000c500: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+0000c510: 5f63 6f6e 6669 672e 7772 6974 655f 6469  _config.write_di
+0000c520: 7370 6f73 6974 696f 6e20 3d20 6269 6771  sposition = bigq
+0000c530: 7565 7279 2e57 7269 7465 4469 7370 6f73  uery.WriteDispos
+0000c540: 6974 696f 6e2e 5752 4954 455f 454d 5054  ition.WRITE_EMPT
+0000c550: 590a 2020 2020 2020 2020 2020 2020 6a6f  Y.            jo
+0000c560: 625f 636f 6e66 6967 2e6c 6162 656c 7320  b_config.labels 
+0000c570: 3d20 7b22 6269 6766 7261 6d65 732d 6170  = {"bigframes-ap
+0000c580: 6922 3a20 2272 6561 645f 7061 7271 7565  i": "read_parque
+0000c590: 7422 7d0a 0a20 2020 2020 2020 2020 2020  t"}..           
+0000c5a0: 2072 6574 7572 6e20 7365 6c66 2e5f 7265   return self._re
+0000c5b0: 6164 5f62 6967 7175 6572 795f 6c6f 6164  ad_bigquery_load
+0000c5c0: 5f6a 6f62 2870 6174 682c 2074 6162 6c65  _job(path, table
+0000c5d0: 2c20 6a6f 625f 636f 6e66 6967 3d6a 6f62  , job_config=job
+0000c5e0: 5f63 6f6e 6669 6729 0a20 2020 2020 2020  _config).       
+0000c5f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000c600: 2020 2072 6561 645f 7061 7271 7565 745f     read_parquet_
+0000c610: 6b77 6172 6773 3a20 4469 6374 5b73 7472  kwargs: Dict[str
+0000c620: 2c20 416e 795d 203d 207b 7d0a 2020 2020  , Any] = {}.    
+0000c630: 2020 2020 2020 2020 6966 2070 616e 6461          if panda
+0000c640: 732e 5f5f 7665 7273 696f 6e5f 5f2e 7374  s.__version__.st
+0000c650: 6172 7473 7769 7468 2822 312e 2229 3a0a  artswith("1."):.
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 7265 6164 5f70 6172 7175 6574 5f6b 7761  read_parquet_kwa
+0000c680: 7267 735b 2275 7365 5f6e 756c 6c61 626c  rgs["use_nullabl
+0000c690: 655f 6474 7970 6573 225d 203d 2054 7275  e_dtypes"] = Tru
+0000c6a0: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+0000c6b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c6c0: 2020 2020 7265 6164 5f70 6172 7175 6574      read_parquet
+0000c6d0: 5f6b 7761 7267 735b 2264 7479 7065 5f62  _kwargs["dtype_b
+0000c6e0: 6163 6b65 6e64 225d 203d 2022 7079 6172  ackend"] = "pyar
+0000c6f0: 726f 7722 0a0a 2020 2020 2020 2020 2020  row"..          
+0000c700: 2020 7061 6e64 6173 5f6f 626a 203d 2070    pandas_obj = p
+0000c710: 616e 6461 732e 7265 6164 5f70 6172 7175  andas.read_parqu
+0000c720: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000c730: 2020 2020 7061 7468 2c0a 2020 2020 2020      path,.      
+0000c740: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
+0000c750: 3d65 6e67 696e 652c 2020 2320 7479 7065  =engine,  # type
+0000c760: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+0000c770: 2020 2020 2020 2020 202a 2a72 6561 645f           **read_
+0000c780: 7061 7271 7565 745f 6b77 6172 6773 2c0a  parquet_kwargs,.
+0000c790: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000c7a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c7b0: 2073 656c 662e 5f72 6561 645f 7061 6e64   self._read_pand
+0000c7c0: 6173 2870 616e 6461 735f 6f62 6a2c 2022  as(pandas_obj, "
+0000c7d0: 7265 6164 5f70 6172 7175 6574 2229 0a0a  read_parquet")..
+0000c7e0: 2020 2020 6465 6620 7265 6164 5f6a 736f      def read_jso
+0000c7f0: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
+0000c800: 0a20 2020 2020 2020 2070 6174 685f 6f72  .        path_or
+0000c810: 5f62 7566 3a20 7374 7220 7c20 494f 5b22  _buf: str | IO["
+0000c820: 6279 7465 7322 5d2c 0a20 2020 2020 2020  bytes"],.       
+0000c830: 202a 2c0a 2020 2020 2020 2020 6f72 6965   *,.        orie
+0000c840: 6e74 3a20 4c69 7465 7261 6c5b 0a20 2020  nt: Literal[.   
+0000c850: 2020 2020 2020 2020 2022 7370 6c69 7422           "split"
+0000c860: 2c20 2272 6563 6f72 6473 222c 2022 696e  , "records", "in
+0000c870: 6465 7822 2c20 2263 6f6c 756d 6e73 222c  dex", "columns",
+0000c880: 2022 7661 6c75 6573 222c 2022 7461 626c   "values", "tabl
+0000c890: 6522 0a20 2020 2020 2020 205d 203d 2022  e".        ] = "
+0000c8a0: 636f 6c75 6d6e 7322 2c0a 2020 2020 2020  columns",.      
+0000c8b0: 2020 6474 7970 653a 204f 7074 696f 6e61    dtype: Optiona
+0000c8c0: 6c5b 4469 6374 5d20 3d20 4e6f 6e65 2c0a  l[Dict] = None,.
+0000c8d0: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
+0000c8e0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000c8f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000c900: 6c69 6e65 733a 2062 6f6f 6c20 3d20 4661  lines: bool = Fa
+0000c910: 6c73 652c 0a20 2020 2020 2020 2065 6e67  lse,.        eng
+0000c920: 696e 653a 204c 6974 6572 616c 5b22 756a  ine: Literal["uj
+0000c930: 736f 6e22 2c20 2270 7961 7272 6f77 222c  son", "pyarrow",
+0000c940: 2022 6269 6771 7565 7279 225d 203d 2022   "bigquery"] = "
+0000c950: 756a 736f 6e22 2c0a 2020 2020 2020 2020  ujson",.        
+0000c960: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+0000c970: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
+0000c980: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+0000c990: 7461 626c 6520 3d20 6269 6766 7261 6d65  table = bigframe
+0000c9a0: 735f 696f 2e72 616e 646f 6d5f 7461 626c  s_io.random_tabl
+0000c9b0: 6528 7365 6c66 2e5f 616e 6f6e 796d 6f75  e(self._anonymou
+0000c9c0: 735f 6461 7461 7365 7429 0a0a 2020 2020  s_dataset)..    
+0000c9d0: 2020 2020 6966 2065 6e67 696e 6520 3d3d      if engine ==
+0000c9e0: 2022 6269 6771 7565 7279 223a 0a0a 2020   "bigquery":..  
+0000c9f0: 2020 2020 2020 2020 2020 6966 2064 7479            if dty
+0000ca00: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca20: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+0000ca30: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ca50: 4269 6751 7565 7279 2065 6e67 696e 6520  BigQuery engine 
+0000ca60: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+0000ca70: 2074 6865 2064 7479 7065 2061 7267 756d   the dtype argum
+0000ca80: 656e 7473 2e22 0a20 2020 2020 2020 2020  ents.".         
+0000ca90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000caa0: 2020 2020 2020 6966 206e 6f74 206c 696e        if not lin
+0000cab0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000cac0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+0000cad0: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
+0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caf0: 2020 2022 4f6e 6c79 206e 6577 6c69 6e65     "Only newline
+0000cb00: 2064 656c 696d 6974 6564 204a 534f 4e20   delimited JSON 
+0000cb10: 666f 726d 6174 2069 7320 7375 7070 6f72  format is suppor
+0000cb20: 7465 642e 220a 2020 2020 2020 2020 2020  ted.".          
+0000cb30: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000cb40: 2020 2020 2069 6620 656e 636f 6469 6e67       if encoding
+0000cb50: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000cb60: 2065 6e63 6f64 696e 6720 6e6f 7420 696e   encoding not in
+0000cb70: 205f 5641 4c49 445f 454e 434f 4449 4e47   _VALID_ENCODING
+0000cb80: 533a 0a20 2020 2020 2020 2020 2020 2020  S:.             
+0000cb90: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+0000cba0: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 6622 4269 6751 7565 7279 2065 6e67    f"BigQuery eng
+0000cbd0: 696e 6520 6f6e 6c79 2073 7570 706f 7274  ine only support
+0000cbe0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+0000cbf0: 656e 636f 6469 6e67 733a 207b 5f56 414c  encodings: {_VAL
+0000cc00: 4944 5f45 4e43 4f44 494e 4753 7d22 0a20  ID_ENCODINGS}". 
+0000cc10: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000cc20: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000cc30: 206c 696e 6573 2061 6e64 206f 7269 656e   lines and orien
+0000cc40: 7420 213d 2022 7265 636f 7264 7322 3a0a  t != "records":.
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000cc70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000cc80: 2020 2020 2020 2227 6c69 6e65 7327 206b        "'lines' k
+0000cc90: 6579 776f 7264 2069 7320 6f6e 6c79 2076  eyword is only v
+0000cca0: 616c 6964 2077 6865 6e20 276f 7269 656e  alid when 'orien
+0000ccb0: 7427 2069 7320 2772 6563 6f72 6473 272e  t' is 'records'.
+0000ccc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000ccd0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000cce0: 206a 6f62 5f63 6f6e 6669 6720 3d20 7365   job_config = se
+0000ccf0: 6c66 2e5f 7072 6570 6172 655f 6c6f 6164  lf._prepare_load
+0000cd00: 5f6a 6f62 5f63 6f6e 6669 6728 290a 2020  _job_config().  
 0000cd10: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-0000cd20: 6e66 6967 2e61 7574 6f64 6574 6563 7420  nfig.autodetect 
-0000cd30: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-0000cd40: 2020 206a 6f62 5f63 6f6e 6669 672e 656e     job_config.en
-0000cd50: 636f 6469 6e67 203d 2065 6e63 6f64 696e  coding = encodin
-0000cd60: 670a 2020 2020 2020 2020 2020 2020 6a6f  g.            jo
-0000cd70: 625f 636f 6e66 6967 2e6c 6162 656c 7320  b_config.labels 
-0000cd80: 3d20 7b22 6269 6766 7261 6d65 732d 6170  = {"bigframes-ap
-0000cd90: 6922 3a20 2272 6561 645f 6a73 6f6e 227d  i": "read_json"}
-0000cda0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000cdb0: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
-0000cdc0: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
-0000cdd0: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
-0000cde0: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 7461 626c 652c 0a20 2020 2020 2020 2020  table,.         
+0000cd20: 6e66 6967 2e63 7265 6174 655f 6469 7370  nfig.create_disp
+0000cd30: 6f73 6974 696f 6e20 3d20 6269 6771 7565  osition = bigque
+0000cd40: 7279 2e43 7265 6174 6544 6973 706f 7369  ry.CreateDisposi
+0000cd50: 7469 6f6e 2e43 5245 4154 455f 4946 5f4e  tion.CREATE_IF_N
+0000cd60: 4545 4445 440a 2020 2020 2020 2020 2020  EEDED.          
+0000cd70: 2020 6a6f 625f 636f 6e66 6967 2e73 6f75    job_config.sou
+0000cd80: 7263 655f 666f 726d 6174 203d 2062 6967  rce_format = big
+0000cd90: 7175 6572 792e 536f 7572 6365 466f 726d  query.SourceForm
+0000cda0: 6174 2e4e 4557 4c49 4e45 5f44 454c 494d  at.NEWLINE_DELIM
+0000cdb0: 4954 4544 5f4a 534f 4e0a 2020 2020 2020  ITED_JSON.      
+0000cdc0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+0000cdd0: 2e77 7269 7465 5f64 6973 706f 7369 7469  .write_dispositi
+0000cde0: 6f6e 203d 2062 6967 7175 6572 792e 5772  on = bigquery.Wr
+0000cdf0: 6974 6544 6973 706f 7369 7469 6f6e 2e57  iteDisposition.W
+0000ce00: 5249 5445 5f45 4d50 5459 0a20 2020 2020  RITE_EMPTY.     
 0000ce10: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-0000ce20: 673d 6a6f 625f 636f 6e66 6967 2c0a 2020  g=job_config,.  
-0000ce30: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000ce40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ce50: 2020 2020 2020 6966 2061 6e79 2861 7267        if any(arg
-0000ce60: 2069 6e20 6b77 6172 6773 2066 6f72 2061   in kwargs for a
-0000ce70: 7267 2069 6e20 2822 6368 756e 6b73 697a  rg in ("chunksiz
-0000ce80: 6522 2c20 2269 7465 7261 746f 7222 2929  e", "iterator"))
-0000ce90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cea0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000ceb0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ced0: 2022 2763 6875 6e6b 7369 7a65 2720 616e   "'chunksize' an
-0000cee0: 6420 2769 7465 7261 746f 7227 2061 7267  d 'iterator' arg
-0000cef0: 756d 656e 7473 2061 7265 206e 6f74 2073  uments are not s
-0000cf00: 7570 706f 7274 6564 2e22 0a20 2020 2020  upported.".     
-0000cf10: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000cf20: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000cf30: 6e73 7461 6e63 6528 7061 7468 5f6f 725f  nstance(path_or_
-0000cf40: 6275 662c 2073 7472 293a 0a20 2020 2020  buf, str):.     
-0000cf50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cf60: 5f63 6865 636b 5f66 696c 655f 7369 7a65  _check_file_size
-0000cf70: 2870 6174 685f 6f72 5f62 7566 290a 0a20  (path_or_buf).. 
-0000cf80: 2020 2020 2020 2020 2020 2069 6620 656e             if en
-0000cf90: 6769 6e65 203d 3d20 2275 6a73 6f6e 223a  gine == "ujson":
-0000cfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cfb0: 2070 616e 6461 735f 6466 203d 2070 616e   pandas_df = pan
-0000cfc0: 6461 732e 7265 6164 5f6a 736f 6e28 2020  das.read_json(  
-0000cfd0: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 6f72 6965 6e74 3d6f 7269 656e      orient=orien
-0000d020: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000d030: 2020 2020 2020 2064 7479 7065 3d64 7479         dtype=dty
-0000d040: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-0000d050: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
-0000d060: 3d65 6e63 6f64 696e 672c 0a20 2020 2020  =encoding,.     
-0000d070: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d080: 696e 6573 3d6c 696e 6573 2c0a 2020 2020  ines=lines,.    
-0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0a0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
-0000d0b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000d0c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d0e0: 616e 6461 735f 6466 203d 2070 616e 6461  andas_df = panda
-0000d0f0: 732e 7265 6164 5f6a 736f 6e28 2020 2320  s.read_json(  # 
-0000d100: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2070 6174 685f 6f72 5f62 7566 2c0a 2020   path_or_buf,.  
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2020 6f72 6965 6e74 3d6f 7269 656e 742c    orient=orient,
-0000d150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d160: 2020 2020 2064 7479 7065 3d64 7479 7065       dtype=dtype
-0000d170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d180: 2020 2020 2020 656e 636f 6469 6e67 3d65        encoding=e
-0000d190: 6e63 6f64 696e 672c 0a20 2020 2020 2020  ncoding,.       
-0000d1a0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-0000d1b0: 6573 3d6c 696e 6573 2c0a 2020 2020 2020  es=lines,.      
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000d1d0: 6769 6e65 3d65 6e67 696e 652c 0a20 2020  gine=engine,.   
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1f0: 202a 2a6b 7761 7267 732c 0a20 2020 2020   **kwargs,.     
-0000d200: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d210: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000d220: 7365 6c66 2e5f 7265 6164 5f70 616e 6461  self._read_panda
-0000d230: 7328 7061 6e64 6173 5f64 662c 2022 7265  s(pandas_df, "re
-0000d240: 6164 5f6a 736f 6e22 290a 0a20 2020 2064  ad_json")..    d
-0000d250: 6566 205f 6368 6563 6b5f 6669 6c65 5f73  ef _check_file_s
-0000d260: 697a 6528 7365 6c66 2c20 6669 6c65 7061  ize(self, filepa
-0000d270: 7468 3a20 7374 7229 3a0a 2020 2020 2020  th: str):.      
-0000d280: 2020 6d61 785f 7369 7a65 203d 2031 3032    max_size = 102
-0000d290: 3420 2a20 3130 3234 202a 2031 3032 3420  4 * 1024 * 1024 
-0000d2a0: 2023 2031 2047 4220 696e 2062 7974 6573   # 1 GB in bytes
-0000d2b0: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
-0000d2c0: 7061 7468 2e73 7461 7274 7377 6974 6828  path.startswith(
-0000d2d0: 2267 733a 2f2f 2229 3a20 2023 2047 4353  "gs://"):  # GCS
-0000d2e0: 2066 696c 6520 7061 7468 0a20 2020 2020   file path.     
-0000d2f0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
-0000d300: 7374 6f72 6167 652e 436c 6965 6e74 2829  storage.Client()
-0000d310: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
-0000d320: 6b65 745f 6e61 6d65 2c20 626c 6f62 5f6e  ket_name, blob_n
-0000d330: 616d 6520 3d20 6669 6c65 7061 7468 2e73  ame = filepath.s
-0000d340: 706c 6974 2822 2f22 2c20 3329 5b32 3a5d  plit("/", 3)[2:]
-0000d350: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
-0000d360: 6b65 7420 3d20 636c 6965 6e74 2e62 7563  ket = client.buc
-0000d370: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-0000d380: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-0000d390: 6220 3d20 6275 636b 6574 2e62 6c6f 6228  b = bucket.blob(
-0000d3a0: 626c 6f62 5f6e 616d 6529 0a20 2020 2020  blob_name).     
-0000d3b0: 2020 2020 2020 2062 6c6f 622e 7265 6c6f         blob.relo
-0000d3c0: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
-0000d3d0: 2066 696c 655f 7369 7a65 203d 2062 6c6f   file_size = blo
-0000d3e0: 622e 7369 7a65 0a20 2020 2020 2020 2065  b.size.        e
-0000d3f0: 6c73 653a 2020 2320 6c6f 6361 6c20 6669  lse:  # local fi
-0000d400: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
-0000d410: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
-0000d420: 6f73 2e70 6174 682e 6765 7473 697a 6528  os.path.getsize(
-0000d430: 6669 6c65 7061 7468 290a 0a20 2020 2020  filepath)..     
-0000d440: 2020 2069 6620 6669 6c65 5f73 697a 6520     if file_size 
-0000d450: 3e20 6d61 785f 7369 7a65 3a0a 2020 2020  > max_size:.    
-0000d460: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-0000d470: 7420 746f 2047 420a 2020 2020 2020 2020  t to GB.        
-0000d480: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
-0000d490: 726f 756e 6428 6669 6c65 5f73 697a 6520  round(file_size 
-0000d4a0: 2f20 2831 3032 342a 2a33 292c 2031 290a  / (1024**3), 1).
-0000d4b0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-0000d4c0: 7369 7a65 203d 2069 6e74 286d 6178 5f73  size = int(max_s
-0000d4d0: 697a 6520 2f20 3130 3234 2a2a 3329 0a20  ize / 1024**3). 
-0000d4e0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000d4f0: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
-0000d500: 2020 2020 2020 2020 2020 2066 2246 696c             f"Fil
-0000d510: 6520 7369 7a65 207b 6669 6c65 5f73 697a  e size {file_siz
-0000d520: 657d 4742 2065 7863 6565 6473 207b 6d61  e}GB exceeds {ma
-0000d530: 785f 7369 7a65 7d47 422e 2022 0a20 2020  x_size}GB. ".   
-0000d540: 2020 2020 2020 2020 2020 2020 2022 4974               "It
-0000d550: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
-0000d560: 746f 2075 7365 2065 6e67 696e 653d 2762  to use engine='b
-0000d570: 6967 7175 6572 7927 2022 0a20 2020 2020  igquery' ".     
-0000d580: 2020 2020 2020 2020 2020 2022 666f 7220             "for 
-0000d590: 6c61 7267 6520 6669 6c65 7320 746f 2061  large files to a
-0000d5a0: 766f 6964 206c 6f61 6469 6e67 2074 6865  void loading the
-0000d5b0: 2066 696c 6520 696e 746f 206c 6f63 616c   file into local
-0000d5c0: 206d 656d 6f72 792e 220a 2020 2020 2020   memory.".      
-0000d5d0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000d5e0: 205f 6372 6561 7465 5f65 6d70 7479 5f74   _create_empty_t
-0000d5f0: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
-0000d600: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000d610: 2073 6368 656d 613a 2049 7465 7261 626c   schema: Iterabl
-0000d620: 655b 6269 6771 7565 7279 2e53 6368 656d  e[bigquery.Schem
-0000d630: 6146 6965 6c64 5d2c 0a20 2020 2020 2020  aField],.       
-0000d640: 2063 6c75 7374 6572 5f63 6f6c 733a 204c   cluster_cols: L
-0000d650: 6973 745b 7374 725d 2c0a 2020 2020 2920  ist[str],.    ) 
-0000d660: 2d3e 2062 6967 7175 6572 792e 5461 626c  -> bigquery.Tabl
-0000d670: 6552 6566 6572 656e 6365 3a0a 2020 2020  eReference:.    
-0000d680: 2020 2020 2320 4361 6e27 7420 7365 7420      # Can't set 
-0000d690: 6120 7461 626c 6520 696e 205f 5345 5353  a table in _SESS
-0000d6a0: 494f 4e20 6173 2064 6573 7469 6e61 7469  ION as destinati
-0000d6b0: 6f6e 2076 6961 2071 7565 7279 206a 6f62  on via query job
-0000d6c0: 2041 5049 2c20 736f 2077 650a 2020 2020   API, so we.    
-0000d6d0: 2020 2020 2320 7275 6e20 4444 4c2c 2069      # run DDL, i
-0000d6e0: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
-0000d6f0: 6461 7461 7365 7420 3d20 7365 6c66 2e5f  dataset = self._
-0000d700: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
-0000d710: 740a 2020 2020 2020 2020 6578 7069 7261  t.        expira
-0000d720: 7469 6f6e 203d 2028 0a20 2020 2020 2020  tion = (.       
-0000d730: 2020 2020 2064 6174 6574 696d 652e 6461       datetime.da
-0000d740: 7465 7469 6d65 2e6e 6f77 2864 6174 6574  tetime.now(datet
-0000d750: 696d 652e 7469 6d65 7a6f 6e65 2e75 7463  ime.timezone.utc
-0000d760: 2920 2b20 636f 6e73 7461 6e74 732e 4445  ) + constants.DE
-0000d770: 4641 554c 545f 4558 5049 5241 5449 4f4e  FAULT_EXPIRATION
-0000d780: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000d790: 2020 2020 7461 626c 6520 3d20 6269 6766      table = bigf
-0000d7a0: 7261 6d65 735f 696f 2e63 7265 6174 655f  rames_io.create_
-0000d7b0: 7465 6d70 5f74 6162 6c65 280a 2020 2020  temp_table(.    
-0000d7c0: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-0000d7d0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-0000d7e0: 2020 2064 6174 6173 6574 2c0a 2020 2020     dataset,.    
-0000d7f0: 2020 2020 2020 2020 6578 7069 7261 7469          expirati
-0000d800: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-0000d810: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-0000d820: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-0000d830: 6572 5f63 6f6c 756d 6e73 3d63 6c75 7374  er_columns=clust
-0000d840: 6572 5f63 6f6c 732c 0a20 2020 2020 2020  er_cols,.       
-0000d850: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0000d860: 6e20 6269 6771 7565 7279 2e54 6162 6c65  n bigquery.Table
-0000d870: 5265 6665 7265 6e63 652e 6672 6f6d 5f73  Reference.from_s
-0000d880: 7472 696e 6728 7461 626c 6529 0a0a 2020  tring(table)..  
-0000d890: 2020 6465 6620 5f63 7265 6174 655f 746f    def _create_to
-0000d8a0: 7461 6c5f 6f72 6465 7269 6e67 280a 2020  tal_ordering(.  
-0000d8b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000d8c0: 2020 2020 7461 626c 653a 2069 6269 735f      table: ibis_
-0000d8d0: 7479 7065 732e 5461 626c 652c 0a20 2020  types.Table,.   
-0000d8e0: 2029 202d 3e20 636f 7265 2e41 7272 6179   ) -> core.Array
-0000d8f0: 5661 6c75 653a 0a20 2020 2020 2020 2023  Value:.        #
-0000d900: 2053 696e 6365 2074 6869 7320 6d69 6768   Since this migh
-0000d910: 7420 616c 736f 2062 6520 7573 6564 2061  t also be used a
-0000d920: 7320 7468 6520 696e 6465 782c 2064 6f6e  s the index, don
-0000d930: 2774 2075 7365 2074 6865 2064 6566 6175  't use the defau
-0000d940: 6c74 0a20 2020 2020 2020 2023 2022 6f72  lt.        # "or
-0000d950: 6465 7269 6e67 2049 4422 206e 616d 652e  dering ID" name.
-0000d960: 0a20 2020 2020 2020 206f 7264 6572 696e  .        orderin
-0000d970: 675f 6861 7368 5f70 6172 7420 3d20 6775  g_hash_part = gu
-0000d980: 6964 2e67 656e 6572 6174 655f 6775 6964  id.generate_guid
-0000d990: 2822 6269 6766 7261 6d65 735f 6f72 6465  ("bigframes_orde
-0000d9a0: 7269 6e67 5f22 290a 2020 2020 2020 2020  ring_").        
-0000d9b0: 6f72 6465 7269 6e67 5f72 616e 645f 7061  ordering_rand_pa
-0000d9c0: 7274 203d 2067 7569 642e 6765 6e65 7261  rt = guid.genera
-0000d9d0: 7465 5f67 7569 6428 2262 6967 6672 616d  te_guid("bigfram
-0000d9e0: 6573 5f6f 7264 6572 696e 675f 2229 0a0a  es_ordering_")..
-0000d9f0: 2020 2020 2020 2020 2320 416c 6c20 696e          # All in
-0000da00: 7075 7473 2069 6e74 6f20 6861 7368 206d  puts into hash m
-0000da10: 7573 7420 6265 206e 6f6e 2d6e 756c 6c20  ust be non-null 
-0000da20: 6f72 2072 6573 756c 7469 6e67 2068 6173  or resulting has
-0000da30: 6820 7769 6c6c 2062 6520 6e75 6c6c 0a20  h will be null. 
-0000da40: 2020 2020 2020 2073 7472 5f76 616c 7565         str_value
-0000da50: 7320 3d20 6c69 7374 280a 2020 2020 2020  s = list(.      
-0000da60: 2020 2020 2020 6d61 7028 6c61 6d62 6461        map(lambda
-0000da70: 2063 6f6c 3a20 5f63 6f6e 7665 7274 5f74   col: _convert_t
-0000da80: 6f5f 6e6f 6e6e 756c 6c5f 7374 7269 6e67  o_nonnull_string
-0000da90: 2874 6162 6c65 5b63 6f6c 5d29 2c20 7461  (table[col]), ta
-0000daa0: 626c 652e 636f 6c75 6d6e 7329 0a20 2020  ble.columns).   
-0000dab0: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
-0000dac0: 756c 6c5f 726f 775f 7374 7220 3d20 280a  ull_row_str = (.
-0000dad0: 2020 2020 2020 2020 2020 2020 7374 725f              str_
-0000dae0: 7661 6c75 6573 5b30 5d2e 636f 6e63 6174  values[0].concat
-0000daf0: 282a 7374 725f 7661 6c75 6573 5b31 3a5d  (*str_values[1:]
-0000db00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000db10: 206c 656e 2873 7472 5f76 616c 7565 7329   len(str_values)
-0000db20: 203e 2031 0a20 2020 2020 2020 2020 2020   > 1.           
-0000db30: 2065 6c73 6520 7374 725f 7661 6c75 6573   else str_values
-0000db40: 5b30 5d0a 2020 2020 2020 2020 290a 2020  [0].        ).  
-0000db50: 2020 2020 2020 6675 6c6c 5f72 6f77 5f68        full_row_h
-0000db60: 6173 6820 3d20 6675 6c6c 5f72 6f77 5f73  ash = full_row_s
-0000db70: 7472 2e68 6173 6828 292e 6e61 6d65 286f  tr.hash().name(o
-0000db80: 7264 6572 696e 675f 6861 7368 5f70 6172  rdering_hash_par
-0000db90: 7429 0a20 2020 2020 2020 2023 2055 7365  t).        # Use
-0000dba0: 6420 746f 2064 6973 616d 6269 6775 6174  d to disambiguat
-0000dbb0: 6520 6265 7477 6565 6e20 6964 656e 7469  e between identi
-0000dbc0: 6361 6c20 726f 7773 2028 7768 6963 6820  cal rows (which 
-0000dbd0: 7769 6c6c 2068 6176 6520 6964 656e 7469  will have identi
-0000dbe0: 6361 6c20 6861 7368 290a 2020 2020 2020  cal hash).      
-0000dbf0: 2020 7261 6e64 6f6d 5f76 616c 7565 203d    random_value =
-0000dc00: 2069 6269 732e 7261 6e64 6f6d 2829 2e6e   ibis.random().n
-0000dc10: 616d 6528 6f72 6465 7269 6e67 5f72 616e  ame(ordering_ran
-0000dc20: 645f 7061 7274 290a 0a20 2020 2020 2020  d_part)..       
-0000dc30: 206f 7269 6769 6e61 6c5f 636f 6c75 6d6e   original_column
-0000dc40: 5f69 6473 203d 2074 6162 6c65 2e63 6f6c  _ids = table.col
-0000dc50: 756d 6e73 0a20 2020 2020 2020 2074 6162  umns.        tab
-0000dc60: 6c65 5f77 6974 685f 6f72 6465 7269 6e67  le_with_ordering
-0000dc70: 203d 2074 6162 6c65 2e73 656c 6563 7428   = table.select(
-0000dc80: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0000dc90: 7274 6f6f 6c73 2e63 6861 696e 286f 7269  rtools.chain(ori
-0000dca0: 6769 6e61 6c5f 636f 6c75 6d6e 5f69 6473  ginal_column_ids
-0000dcb0: 2c20 5b66 756c 6c5f 726f 775f 6861 7368  , [full_row_hash
-0000dcc0: 2c20 7261 6e64 6f6d 5f76 616c 7565 5d29  , random_value])
-0000dcd0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000dce0: 2020 2020 6f72 6465 7269 6e67 5f72 6566      ordering_ref
-0000dcf0: 3120 3d20 6f72 6465 722e 6173 6365 6e64  1 = order.ascend
-0000dd00: 696e 675f 6f76 6572 286f 7264 6572 696e  ing_over(orderin
-0000dd10: 675f 6861 7368 5f70 6172 7429 0a20 2020  g_hash_part).   
-0000dd20: 2020 2020 206f 7264 6572 696e 675f 7265       ordering_re
-0000dd30: 6632 203d 206f 7264 6572 2e61 7363 656e  f2 = order.ascen
-0000dd40: 6469 6e67 5f6f 7665 7228 6f72 6465 7269  ding_over(orderi
-0000dd50: 6e67 5f72 616e 645f 7061 7274 290a 2020  ng_rand_part).  
-0000dd60: 2020 2020 2020 6f72 6465 7269 6e67 203d        ordering =
-0000dd70: 206f 7264 6572 2e45 7870 7265 7373 696f   order.Expressio
-0000dd80: 6e4f 7264 6572 696e 6728 0a20 2020 2020  nOrdering(.     
-0000dd90: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
-0000dda0: 7661 6c75 655f 636f 6c75 6d6e 733d 286f  value_columns=(o
-0000ddb0: 7264 6572 696e 675f 7265 6631 2c20 6f72  rdering_ref1, or
-0000ddc0: 6465 7269 6e67 5f72 6566 3229 2c0a 2020  dering_ref2),.  
-0000ddd0: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-0000dde0: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
-0000ddf0: 3d66 726f 7a65 6e73 6574 285b 6f72 6465  =frozenset([orde
-0000de00: 7269 6e67 5f68 6173 685f 7061 7274 2c20  ring_hash_part, 
-0000de10: 6f72 6465 7269 6e67 5f72 616e 645f 7061  ordering_rand_pa
-0000de20: 7274 5d29 2c0a 2020 2020 2020 2020 290a  rt]),.        ).
-0000de30: 2020 2020 2020 2020 636f 6c75 6d6e 7320          columns 
-0000de40: 3d20 5b74 6162 6c65 5f77 6974 685f 6f72  = [table_with_or
-0000de50: 6465 7269 6e67 5b63 6f6c 5d20 666f 7220  dering[col] for 
-0000de60: 636f 6c20 696e 206f 7269 6769 6e61 6c5f  col in original_
-0000de70: 636f 6c75 6d6e 5f69 6473 5d0a 2020 2020  column_ids].    
-0000de80: 2020 2020 6869 6464 656e 5f63 6f6c 756d      hidden_colum
-0000de90: 6e73 203d 205b 0a20 2020 2020 2020 2020  ns = [.         
-0000dea0: 2020 2074 6162 6c65 5f77 6974 685f 6f72     table_with_or
-0000deb0: 6465 7269 6e67 5b6f 7264 6572 696e 675f  dering[ordering_
-0000dec0: 6861 7368 5f70 6172 745d 2c0a 2020 2020  hash_part],.    
-0000ded0: 2020 2020 2020 2020 7461 626c 655f 7769          table_wi
-0000dee0: 7468 5f6f 7264 6572 696e 675b 6f72 6465  th_ordering[orde
-0000def0: 7269 6e67 5f72 616e 645f 7061 7274 5d2c  ring_rand_part],
-0000df00: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0000df10: 2020 2072 6574 7572 6e20 636f 7265 2e41     return core.A
-0000df20: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
-0000df30: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
-0000df40: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0000df50: 2020 2074 6162 6c65 5f77 6974 685f 6f72     table_with_or
-0000df60: 6465 7269 6e67 2c0a 2020 2020 2020 2020  dering,.        
-0000df70: 2020 2020 636f 6c75 6d6e 732c 0a20 2020      columns,.   
-0000df80: 2020 2020 2020 2020 2068 6964 6465 6e5f           hidden_
-0000df90: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
-0000dfa0: 3d68 6964 6465 6e5f 636f 6c75 6d6e 732c  =hidden_columns,
-0000dfb0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-0000dfc0: 6572 696e 673d 6f72 6465 7269 6e67 2c0a  ering=ordering,.
-0000dfd0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000dfe0: 6566 205f 6962 6973 5f74 6f5f 7465 6d70  ef _ibis_to_temp
-0000dff0: 5f74 6162 6c65 280a 2020 2020 2020 2020  _table(.        
-0000e000: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
-0000e010: 626c 653a 2069 6269 735f 7479 7065 732e  ble: ibis_types.
-0000e020: 5461 626c 652c 0a20 2020 2020 2020 2063  Table,.        c
-0000e030: 6c75 7374 6572 5f63 6f6c 733a 2049 7465  luster_cols: Ite
-0000e040: 7261 626c 655b 7374 725d 2c0a 2020 2020  rable[str],.    
-0000e050: 2020 2020 6170 695f 6e61 6d65 3a20 7374      api_name: st
-0000e060: 722c 0a20 2020 2029 202d 3e20 6269 6771  r,.    ) -> bigq
-0000e070: 7565 7279 2e54 6162 6c65 5265 6665 7265  uery.TableRefere
-0000e080: 6e63 653a 0a20 2020 2020 2020 2064 6573  nce:.        des
-0000e090: 7469 6e61 7469 6f6e 2c20 5f20 3d20 7365  tination, _ = se
-0000e0a0: 6c66 2e5f 7175 6572 795f 746f 5f64 6573  lf._query_to_des
-0000e0b0: 7469 6e61 7469 6f6e 280a 2020 2020 2020  tination(.      
-0000e0c0: 2020 2020 2020 7365 6c66 2e69 6269 735f        self.ibis_
-0000e0d0: 636c 6965 6e74 2e63 6f6d 7069 6c65 2874  client.compile(t
-0000e0e0: 6162 6c65 292c 0a20 2020 2020 2020 2020  able),.         
-0000e0f0: 2020 2069 6e64 6578 5f63 6f6c 733d 6c69     index_cols=li
-0000e100: 7374 2863 6c75 7374 6572 5f63 6f6c 7329  st(cluster_cols)
-0000e110: 2c0a 2020 2020 2020 2020 2020 2020 6170  ,.            ap
-0000e120: 695f 6e61 6d65 3d61 7069 5f6e 616d 652c  i_name=api_name,
-0000e130: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000e140: 2020 2023 2054 6865 7265 2073 686f 756c     # There shoul
-0000e150: 6420 616c 7761 7973 2062 6520 6120 6465  d always be a de
-0000e160: 7374 696e 6174 696f 6e20 7461 626c 6520  stination table 
-0000e170: 666f 7220 7468 6973 2071 7565 7279 2074  for this query t
-0000e180: 7970 652e 0a20 2020 2020 2020 2072 6574  ype..        ret
-0000e190: 7572 6e20 7479 7069 6e67 2e63 6173 7428  urn typing.cast(
-0000e1a0: 6269 6771 7565 7279 2e54 6162 6c65 5265  bigquery.TableRe
-0000e1b0: 6665 7265 6e63 652c 2064 6573 7469 6e61  ference, destina
-0000e1c0: 7469 6f6e 290a 0a20 2020 2064 6566 2072  tion)..    def r
-0000e1d0: 656d 6f74 655f 6675 6e63 7469 6f6e 280a  emote_function(.
-0000e1e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000e1f0: 2020 2020 2020 696e 7075 745f 7479 7065        input_type
-0000e200: 733a 204c 6973 745b 7479 7065 5d2c 0a20  s: List[type],. 
-0000e210: 2020 2020 2020 206f 7574 7075 745f 7479         output_ty
-0000e220: 7065 3a20 7479 7065 2c0a 2020 2020 2020  pe: type,.      
-0000e230: 2020 6461 7461 7365 743a 204f 7074 696f    dataset: Optio
-0000e240: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000e250: 0a20 2020 2020 2020 2062 6967 7175 6572  .        bigquer
-0000e260: 795f 636f 6e6e 6563 7469 6f6e 3a20 4f70  y_connection: Op
-0000e270: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000e280: 6e65 2c0a 2020 2020 2020 2020 7265 7573  ne,.        reus
-0000e290: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
-0000e2a0: 2020 2020 2020 2020 6e61 6d65 3a20 4f70          name: Op
-0000e2b0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000e2c0: 6e65 2c0a 2020 2020 2020 2020 7061 636b  ne,.        pack
-0000e2d0: 6167 6573 3a20 4f70 7469 6f6e 616c 5b53  ages: Optional[S
-0000e2e0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
-0000e2f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636c  None,.        cl
-0000e300: 6f75 645f 6675 6e63 7469 6f6e 5f73 6572  oud_function_ser
-0000e310: 7669 6365 5f61 6363 6f75 6e74 3a20 4f70  vice_account: Op
-0000e320: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000e330: 6e65 2c0a 2020 2020 2020 2020 636c 6f75  ne,.        clou
-0000e340: 645f 6675 6e63 7469 6f6e 5f6b 6d73 5f6b  d_function_kms_k
-0000e350: 6579 5f6e 616d 653a 204f 7074 696f 6e61  ey_name: Optiona
-0000e360: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000e370: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-0000e380: 6374 696f 6e5f 646f 636b 6572 5f72 6570  ction_docker_rep
-0000e390: 6f73 6974 6f72 793a 204f 7074 696f 6e61  ository: Optiona
-0000e3a0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000e3b0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000e3c0: 2244 6563 6f72 6174 6f72 2074 6f20 7475  "Decorator to tu
-0000e3d0: 726e 2061 2075 7365 7220 6465 6669 6e65  rn a user define
-0000e3e0: 6420 6675 6e63 7469 6f6e 2069 6e74 6f20  d function into 
-0000e3f0: 6120 4269 6751 7565 7279 2072 656d 6f74  a BigQuery remot
-0000e400: 6520 6675 6e63 7469 6f6e 2e20 4368 6563  e function. Chec
-0000e410: 6b20 6f75 740a 2020 2020 2020 2020 7468  k out.        th
-0000e420: 6520 636f 6465 2073 616d 706c 6573 2061  e code samples a
-0000e430: 743a 2068 7474 7073 3a2f 2f63 6c6f 7564  t: https://cloud
-0000e440: 2e67 6f6f 676c 652e 636f 6d2f 6269 6771  .google.com/bigq
-0000e450: 7565 7279 2f64 6f63 732f 7265 6d6f 7465  uery/docs/remote
-0000e460: 2d66 756e 6374 696f 6e73 2362 6967 7175  -functions#bigqu
-0000e470: 6572 792d 6461 7461 6672 616d 6573 2e0a  ery-dataframes..
-0000e480: 0a20 2020 2020 2020 202e 2e20 6e6f 7465  .        .. note
-0000e490: 3a3a 0a20 2020 2020 2020 2020 2020 2050  ::.            P
-0000e4a0: 6c65 6173 6520 6d61 6b65 2073 7572 6520  lease make sure 
-0000e4b0: 666f 6c6c 6f77 696e 6720 6973 2073 6574  following is set
-0000e4c0: 7570 2062 6566 6f72 6520 7573 696e 6720  up before using 
-0000e4d0: 7468 6973 2041 5049 3a0a 0a20 2020 2020  this API:..     
-0000e4e0: 2020 2031 2e20 4861 7665 2074 6865 2062     1. Have the b
-0000e4f0: 656c 6f77 2041 5049 7320 656e 6162 6c65  elow APIs enable
-0000e500: 6420 666f 7220 796f 7572 2070 726f 6a65  d for your proje
-0000e510: 6374 3a0a 0a20 2020 2020 2020 2020 2020  ct:..           
-0000e520: 202a 2042 6967 5175 6572 7920 436f 6e6e   * BigQuery Conn
-0000e530: 6563 7469 6f6e 2041 5049 0a20 2020 2020  ection API.     
-0000e540: 2020 2020 2020 202a 2043 6c6f 7564 2046         * Cloud F
-0000e550: 756e 6374 696f 6e73 2041 5049 0a20 2020  unctions API.   
-0000e560: 2020 2020 2020 2020 202a 2043 6c6f 7564           * Cloud
-0000e570: 2052 756e 2041 5049 0a20 2020 2020 2020   Run API.       
-0000e580: 2020 2020 202a 2043 6c6f 7564 2042 7569       * Cloud Bui
-0000e590: 6c64 2041 5049 0a20 2020 2020 2020 2020  ld API.         
-0000e5a0: 2020 202a 2041 7274 6966 6163 7420 5265     * Artifact Re
-0000e5b0: 6769 7374 7279 2041 5049 0a20 2020 2020  gistry API.     
-0000e5c0: 2020 2020 2020 202a 2043 6c6f 7564 2052         * Cloud R
-0000e5d0: 6573 6f75 7263 6520 4d61 6e61 6765 7220  esource Manager 
-0000e5e0: 4150 490a 0a20 2020 2020 2020 2020 2020  API..           
-0000e5f0: 5468 6973 2063 616e 2062 6520 646f 6e65  This can be done
-0000e600: 2066 726f 6d20 7468 6520 636c 6f75 6420   from the cloud 
-0000e610: 636f 6e73 6f6c 6520 2863 6861 6e67 6520  console (change 
-0000e620: 6050 524f 4a45 4354 5f49 4460 2074 6f20  `PROJECT_ID` to 
-0000e630: 796f 7572 7329 3a0a 2020 2020 2020 2020  yours):.        
-0000e640: 2020 2068 7474 7073 3a2f 2f63 6f6e 736f     https://conso
-0000e650: 6c65 2e63 6c6f 7564 2e67 6f6f 676c 652e  le.cloud.google.
-0000e660: 636f 6d2f 6170 6973 2f65 6e61 626c 6566  com/apis/enablef
-0000e670: 6c6f 773f 6170 6969 643d 6269 6771 7565  low?apiid=bigque
-0000e680: 7279 636f 6e6e 6563 7469 6f6e 2e67 6f6f  ryconnection.goo
-0000e690: 676c 6561 7069 732e 636f 6d2c 636c 6f75  gleapis.com,clou
-0000e6a0: 6466 756e 6374 696f 6e73 2e67 6f6f 676c  dfunctions.googl
-0000e6b0: 6561 7069 732e 636f 6d2c 7275 6e2e 676f  eapis.com,run.go
-0000e6c0: 6f67 6c65 6170 6973 2e63 6f6d 2c63 6c6f  ogleapis.com,clo
-0000e6d0: 7564 6275 696c 642e 676f 6f67 6c65 6170  udbuild.googleap
-0000e6e0: 6973 2e63 6f6d 2c61 7274 6966 6163 7472  is.com,artifactr
-0000e6f0: 6567 6973 7472 792e 676f 6f67 6c65 6170  egistry.googleap
-0000e700: 6973 2e63 6f6d 2c63 6c6f 7564 7265 736f  is.com,cloudreso
-0000e710: 7572 6365 6d61 6e61 6765 722e 676f 6f67  urcemanager.goog
-0000e720: 6c65 6170 6973 2e63 6f6d 2670 726f 6a65  leapis.com&proje
-0000e730: 6374 3d50 524f 4a45 4354 5f49 440a 0a20  ct=PROJECT_ID.. 
-0000e740: 2020 2020 2020 2020 2020 4f72 2066 726f            Or fro
-0000e750: 6d20 7468 6520 6763 6c6f 7564 2043 4c49  m the gcloud CLI
-0000e760: 3a0a 0a20 2020 2020 2020 2020 2020 6024  :..           `$
-0000e770: 2067 636c 6f75 6420 7365 7276 6963 6573   gcloud services
-0000e780: 2065 6e61 626c 6520 6269 6771 7565 7279   enable bigquery
-0000e790: 636f 6e6e 6563 7469 6f6e 2e67 6f6f 676c  connection.googl
-0000e7a0: 6561 7069 732e 636f 6d20 636c 6f75 6466  eapis.com cloudf
-0000e7b0: 756e 6374 696f 6e73 2e67 6f6f 676c 6561  unctions.googlea
-0000e7c0: 7069 732e 636f 6d20 7275 6e2e 676f 6f67  pis.com run.goog
-0000e7d0: 6c65 6170 6973 2e63 6f6d 2063 6c6f 7564  leapis.com cloud
-0000e7e0: 6275 696c 642e 676f 6f67 6c65 6170 6973  build.googleapis
-0000e7f0: 2e63 6f6d 2061 7274 6966 6163 7472 6567  .com artifactreg
-0000e800: 6973 7472 792e 676f 6f67 6c65 6170 6973  istry.googleapis
-0000e810: 2e63 6f6d 2063 6c6f 7564 7265 736f 7572  .com cloudresour
-0000e820: 6365 6d61 6e61 6765 722e 676f 6f67 6c65  cemanager.google
-0000e830: 6170 6973 2e63 6f6d 600a 0a20 2020 2020  apis.com`..     
-0000e840: 2020 2032 2e20 4861 7665 2066 6f6c 6c6f     2. Have follo
-0000e850: 7769 6e67 2049 414d 2072 6f6c 6573 2065  wing IAM roles e
-0000e860: 6e61 626c 6564 2066 6f72 2079 6f75 3a0a  nabled for you:.
-0000e870: 0a20 2020 2020 2020 2020 2020 202a 2042  .            * B
-0000e880: 6967 5175 6572 7920 4461 7461 2045 6469  igQuery Data Edi
-0000e890: 746f 7220 2872 6f6c 6573 2f62 6967 7175  tor (roles/bigqu
-0000e8a0: 6572 792e 6461 7461 4564 6974 6f72 290a  ery.dataEditor).
-0000e8b0: 2020 2020 2020 2020 2020 2020 2a20 4269              * Bi
-0000e8c0: 6751 7565 7279 2043 6f6e 6e65 6374 696f  gQuery Connectio
-0000e8d0: 6e20 4164 6d69 6e20 2872 6f6c 6573 2f62  n Admin (roles/b
-0000e8e0: 6967 7175 6572 792e 636f 6e6e 6563 7469  igquery.connecti
-0000e8f0: 6f6e 4164 6d69 6e29 0a20 2020 2020 2020  onAdmin).       
-0000e900: 2020 2020 202a 2043 6c6f 7564 2046 756e       * Cloud Fun
-0000e910: 6374 696f 6e73 2044 6576 656c 6f70 6572  ctions Developer
-0000e920: 2028 726f 6c65 732f 636c 6f75 6466 756e   (roles/cloudfun
-0000e930: 6374 696f 6e73 2e64 6576 656c 6f70 6572  ctions.developer
-0000e940: 290a 2020 2020 2020 2020 2020 2020 2a20  ).            * 
-0000e950: 5365 7276 6963 6520 4163 636f 756e 7420  Service Account 
-0000e960: 5573 6572 2028 726f 6c65 732f 6961 6d2e  User (roles/iam.
-0000e970: 7365 7276 6963 6541 6363 6f75 6e74 5573  serviceAccountUs
-0000e980: 6572 2920 6f6e 2074 6865 2073 6572 7669  er) on the servi
-0000e990: 6365 2061 6363 6f75 6e74 2060 5052 4f4a  ce account `PROJ
-0000e9a0: 4543 545f 4e55 4d42 4552 2d63 6f6d 7075  ECT_NUMBER-compu
-0000e9b0: 7465 4064 6576 656c 6f70 6572 2e67 7365  te@developer.gse
-0000e9c0: 7276 6963 6561 6363 6f75 6e74 2e63 6f6d  rviceaccount.com
-0000e9d0: 600a 2020 2020 2020 2020 2020 2020 2a20  `.            * 
-0000e9e0: 5374 6f72 6167 6520 4f62 6a65 6374 2056  Storage Object V
-0000e9f0: 6965 7765 7220 2872 6f6c 6573 2f73 746f  iewer (roles/sto
-0000ea00: 7261 6765 2e6f 626a 6563 7456 6965 7765  rage.objectViewe
-0000ea10: 7229 0a20 2020 2020 2020 2020 2020 202a  r).            *
-0000ea20: 2050 726f 6a65 6374 2049 414d 2041 646d   Project IAM Adm
-0000ea30: 696e 2028 726f 6c65 732f 7265 736f 7572  in (roles/resour
-0000ea40: 6365 6d61 6e61 6765 722e 7072 6f6a 6563  cemanager.projec
-0000ea50: 7449 616d 4164 6d69 6e29 2028 4f6e 6c79  tIamAdmin) (Only
-0000ea60: 2072 6571 7569 7265 6420 6966 2074 6865   required if the
-0000ea70: 2062 6967 7175 6572 7920 636f 6e6e 6563   bigquery connec
-0000ea80: 7469 6f6e 2062 6569 6e67 2075 7365 6420  tion being used 
-0000ea90: 6973 206e 6f74 2070 7265 2d63 7265 6174  is not pre-creat
-0000eaa0: 6564 2061 6e64 2069 7320 6372 6561 7465  ed and is create
-0000eab0: 6420 6479 6e61 6d69 6361 6c6c 7920 7769  d dynamically wi
-0000eac0: 7468 2075 7365 7220 6372 6564 656e 7469  th user credenti
-0000ead0: 616c 732e 290a 0a20 2020 2020 2020 2033  als.)..        3
-0000eae0: 2e20 4569 7468 6572 2074 6865 2075 7365  . Either the use
-0000eaf0: 7220 6861 7320 7365 7449 616d 506f 6c69  r has setIamPoli
-0000eb00: 6379 2070 7269 7669 6c65 6765 206f 6e20  cy privilege on 
-0000eb10: 7468 6520 7072 6f6a 6563 742c 206f 7220  the project, or 
-0000eb20: 6120 4269 6751 7565 7279 2063 6f6e 6e65  a BigQuery conne
-0000eb30: 6374 696f 6e20 6973 2070 7265 2d63 7265  ction is pre-cre
-0000eb40: 6174 6564 2077 6974 6820 6e65 6365 7373  ated with necess
-0000eb50: 6172 7920 4941 4d20 726f 6c65 2073 6574  ary IAM role set
-0000eb60: 3a0a 0a20 2020 2020 2020 2020 2020 2031  :..            1
-0000eb70: 2e20 546f 2063 7265 6174 6520 6120 636f  . To create a co
-0000eb80: 6e6e 6563 7469 6f6e 2c20 666f 6c6c 6f77  nnection, follow
-0000eb90: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-0000eba0: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
-0000ebb0: 7279 2f64 6f63 732f 7265 6665 7265 6e63  ry/docs/referenc
-0000ebc0: 652f 7374 616e 6461 7264 2d73 716c 2f72  e/standard-sql/r
-0000ebd0: 656d 6f74 652d 6675 6e63 7469 6f6e 7323  emote-functions#
-0000ebe0: 6372 6561 7465 5f61 5f63 6f6e 6e65 6374  create_a_connect
-0000ebf0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000ec00: 322e 2054 6f20 7365 7420 7570 2049 414d  2. To set up IAM
-0000ec10: 2c20 666f 6c6c 6f77 2068 7474 7073 3a2f  , follow https:/
-0000ec20: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-0000ec30: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
-0000ec40: 7265 6665 7265 6e63 652f 7374 616e 6461  reference/standa
-0000ec50: 7264 2d73 716c 2f72 656d 6f74 652d 6675  rd-sql/remote-fu
-0000ec60: 6e63 7469 6f6e 7323 6772 616e 745f 7065  nctions#grant_pe
-0000ec70: 726d 6973 7369 6f6e 5f6f 6e5f 6675 6e63  rmission_on_func
-0000ec80: 7469 6f6e 0a0a 2020 2020 2020 2020 2020  tion..          
-0000ec90: 2020 2020 2041 6c74 6572 6e61 7469 7665       Alternative
-0000eca0: 6c79 2c20 7468 6520 4941 4d20 636f 756c  ly, the IAM coul
-0000ecb0: 6420 616c 736f 2062 6520 7365 7475 7020  d also be setup 
-0000ecc0: 7669 6120 7468 6520 6763 6c6f 7564 2043  via the gcloud C
-0000ecd0: 4c49 3a0a 0a20 2020 2020 2020 2020 2020  LI:..           
-0000ece0: 2020 2020 6024 2067 636c 6f75 6420 7072      `$ gcloud pr
-0000ecf0: 6f6a 6563 7473 2061 6464 2d69 616d 2d70  ojects add-iam-p
-0000ed00: 6f6c 6963 792d 6269 6e64 696e 6720 5052  olicy-binding PR
-0000ed10: 4f4a 4543 545f 4944 202d 2d6d 656d 6265  OJECT_ID --membe
-0000ed20: 723d 2273 6572 7669 6365 4163 636f 756e  r="serviceAccoun
-0000ed30: 743a 434f 4e4e 4543 5449 4f4e 5f53 4552  t:CONNECTION_SER
-0000ed40: 5649 4345 5f41 4343 4f55 4e54 5f49 4422  VICE_ACCOUNT_ID"
-0000ed50: 202d 2d72 6f6c 653d 2272 6f6c 6573 2f72   --role="roles/r
-0000ed60: 756e 2e69 6e76 6f6b 6572 2260 2e0a 0a20  un.invoker"`... 
-0000ed70: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000ed80: 2020 2020 2020 2020 2069 6e70 7574 5f74           input_t
-0000ed90: 7970 6573 2028 6c69 7374 2874 7970 6529  ypes (list(type)
-0000eda0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000edb0: 2020 204c 6973 7420 6f66 2069 6e70 7574     List of input
-0000edc0: 2064 6174 6120 7479 7065 7320 696e 2074   data types in t
-0000edd0: 6865 2075 7365 7220 6465 6669 6e65 6420  he user defined 
-0000ede0: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
-0000edf0: 2020 2020 2020 6f75 7470 7574 5f74 7970        output_typ
-0000ee00: 6520 2874 7970 6529 3a0a 2020 2020 2020  e (type):.      
-0000ee10: 2020 2020 2020 2020 2020 4461 7461 2074            Data t
-0000ee20: 7970 6520 6f66 2074 6865 206f 7574 7075  ype of the outpu
-0000ee30: 7420 696e 2074 6865 2075 7365 7220 6465  t in the user de
-0000ee40: 6669 6e65 6420 6675 6e63 7469 6f6e 2e0a  fined function..
-0000ee50: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000ee60: 7365 7420 2873 7472 2c20 4f70 7469 6f6e  set (str, Option
-0000ee70: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
-0000ee80: 2020 2020 2044 6174 6173 6574 2069 6e20       Dataset in 
-0000ee90: 7768 6963 6820 746f 2063 7265 6174 6520  which to create 
-0000eea0: 6120 4269 6751 7565 7279 2072 656d 6f74  a BigQuery remot
-0000eeb0: 6520 6675 6e63 7469 6f6e 2e20 4974 2073  e function. It s
-0000eec0: 686f 756c 6420 6265 2069 6e0a 2020 2020  hould be in.    
-0000eed0: 2020 2020 2020 2020 2020 2020 603c 7072              `<pr
-0000eee0: 6f6a 6563 745f 6964 3e2e 3c64 6174 6173  oject_id>.<datas
-0000eef0: 6574 5f6e 616d 653e 6020 6f72 2060 3c64  et_name>` or `<d
-0000ef00: 6174 6173 6574 5f6e 616d 653e 6020 666f  ataset_name>` fo
-0000ef10: 726d 6174 2e20 4966 2074 6869 730a 2020  rmat. If this.  
-0000ef20: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000ef30: 7261 6d65 7465 7220 6973 206e 6f74 2070  rameter is not p
-0000ef40: 726f 7669 6465 6420 7468 656e 2073 6573  rovided then ses
-0000ef50: 7369 6f6e 2064 6174 6173 6574 2069 6420  sion dataset id 
-0000ef60: 6973 2075 7365 642e 0a20 2020 2020 2020  is used..       
-0000ef70: 2020 2020 2062 6967 7175 6572 795f 636f       bigquery_co
-0000ef80: 6e6e 6563 7469 6f6e 2028 7374 722c 204f  nnection (str, O
-0000ef90: 7074 696f 6e61 6c29 3a0a 2020 2020 2020  ptional):.      
-0000efa0: 2020 2020 2020 2020 2020 4e61 6d65 206f            Name o
-0000efb0: 6620 7468 6520 4269 6751 7565 7279 2063  f the BigQuery c
-0000efc0: 6f6e 6e65 6374 696f 6e2e 2059 6f75 2073  onnection. You s
-0000efd0: 686f 756c 6420 6569 7468 6572 2068 6176  hould either hav
-0000efe0: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
-0000eff0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-0000f000: 2061 6c72 6561 6479 2063 7265 6174 6564   already created
-0000f010: 2069 6e20 7468 6520 606c 6f63 6174 696f   in the `locatio
-0000f020: 6e60 2079 6f75 2068 6176 6520 6368 6f73  n` you have chos
-0000f030: 656e 2c20 6f72 0a20 2020 2020 2020 2020  en, or.         
-0000f040: 2020 2020 2020 2079 6f75 2073 686f 756c         you shoul
-0000f050: 6420 6861 7665 2074 6865 2050 726f 6a65  d have the Proje
-0000f060: 6374 2049 414d 2041 646d 696e 2072 6f6c  ct IAM Admin rol
-0000f070: 6520 746f 2065 6e61 626c 6520 7468 6520  e to enable the 
-0000f080: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
-0000f090: 2020 2020 2020 2020 746f 2063 7265 6174          to creat
-0000f0a0: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
-0000f0b0: 2066 6f72 2079 6f75 2069 6620 796f 7520   for you if you 
-0000f0c0: 6e65 6564 2069 742e 2049 6620 7468 6973  need it. If this
-0000f0d0: 2070 6172 616d 6574 6572 2069 730a 2020   parameter is.  
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-0000f0f0: 7420 7072 6f76 6964 6564 2074 6865 6e20  t provided then 
-0000f100: 7468 6520 4269 6751 7565 7279 2063 6f6e  the BigQuery con
-0000f110: 6e65 6374 696f 6e20 6672 6f6d 2074 6865  nection from the
-0000f120: 2073 6573 7369 6f6e 2069 7320 7573 6564   session is used
-0000f130: 2e0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000f140: 7573 6520 2862 6f6f 6c2c 204f 7074 696f  use (bool, Optio
-0000f150: 6e61 6c29 3a0a 2020 2020 2020 2020 2020  nal):.          
-0000f160: 2020 2020 2020 5265 7573 6520 7468 6520        Reuse the 
-0000f170: 7265 6d6f 7465 2066 756e 6374 696f 6e20  remote function 
-0000f180: 6966 2061 6c72 6561 6479 2065 7869 7374  if already exist
-0000f190: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-0000f1a0: 2020 2060 5472 7565 6020 6279 2064 6566     `True` by def
-0000f1b0: 6175 6c74 2c20 7768 6963 6820 7769 6c6c  ault, which will
-0000f1c0: 2072 6573 756c 7420 696e 2072 6575 7369   result in reusi
-0000f1d0: 6e67 2061 6e20 6578 6973 7469 6e67 2072  ng an existing r
-0000f1e0: 656d 6f74 650a 2020 2020 2020 2020 2020  emote.          
-0000f1f0: 2020 2020 2020 6675 6e63 7469 6f6e 2061        function a
-0000f200: 6e64 2063 6f72 7265 7370 6f6e 6469 6e67  nd corresponding
-0000f210: 2063 6c6f 7564 2066 756e 6374 696f 6e20   cloud function 
-0000f220: 2869 6620 616e 7929 2074 6861 7420 7761  (if any) that wa
-0000f230: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000f240: 2020 7072 6576 696f 7573 6c79 2063 7265    previously cre
-0000f250: 6174 6564 2066 6f72 2074 6865 2073 616d  ated for the sam
-0000f260: 6520 7564 662e 0a20 2020 2020 2020 2020  e udf..         
-0000f270: 2020 2020 2020 2053 6574 7469 6e67 2069         Setting i
-0000f280: 7420 746f 2060 4661 6c73 6560 2077 6f75  t to `False` wou
-0000f290: 6c64 2066 6f72 6365 2063 7265 6174 696e  ld force creatin
-0000f2a0: 6720 6120 756e 6971 7565 2072 656d 6f74  g a unique remot
-0000f2b0: 6520 6675 6e63 7469 6f6e 2e0a 2020 2020  e function..    
-0000f2c0: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0000f2d0: 6865 2072 6571 7569 7265 6420 7265 6d6f  he required remo
-0000f2e0: 7465 2066 756e 6374 696f 6e20 646f 6573  te function does
-0000f2f0: 206e 6f74 2065 7869 7374 2074 6865 6e20   not exist then 
-0000f300: 6974 2077 6f75 6c64 2062 650a 2020 2020  it would be.    
-0000f310: 2020 2020 2020 2020 2020 2020 6372 6561              crea
-0000f320: 7465 6420 6972 7265 7370 6563 7469 7665  ted irrespective
-0000f330: 206f 6620 7468 6973 2070 6172 616d 2e0a   of this param..
-0000f340: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000f350: 2028 7374 722c 204f 7074 696f 6e61 6c29   (str, Optional)
-0000f360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f370: 2020 4578 706c 6963 6974 206e 616d 6520    Explicit name 
-0000f380: 6f66 2074 6865 2070 6572 7369 7374 6564  of the persisted
-0000f390: 2042 6967 5175 6572 7920 7265 6d6f 7465   BigQuery remote
-0000f3a0: 2066 756e 6374 696f 6e2e 2055 7365 2069   function. Use i
-0000f3b0: 7420 7769 7468 0a20 2020 2020 2020 2020  t with.         
-0000f3c0: 2020 2020 2020 2063 6175 7469 6f6e 2c20         caution, 
-0000f3d0: 6265 6361 7573 6520 7477 6f20 7573 6572  because two user
-0000f3e0: 7320 776f 726b 696e 6720 696e 2074 6865  s working in the
-0000f3f0: 2073 616d 6520 7072 6f6a 6563 7420 616e   same project an
-0000f400: 6420 6461 7461 7365 740a 2020 2020 2020  d dataset.      
-0000f410: 2020 2020 2020 2020 2020 636f 756c 6420            could 
-0000f420: 6f76 6572 7772 6974 6520 6561 6368 206f  overwrite each o
-0000f430: 7468 6572 2773 2072 656d 6f74 6520 6675  ther's remote fu
-0000f440: 6e63 7469 6f6e 7320 6966 2074 6865 7920  nctions if they 
-0000f450: 7573 6520 7468 6520 7361 6d65 0a20 2020  use the same.   
-0000f460: 2020 2020 2020 2020 2020 2020 2070 6572               per
-0000f470: 7369 7374 656e 7420 6e61 6d65 2e0a 2020  sistent name..  
-0000f480: 2020 2020 2020 2020 2020 7061 636b 6167            packag
-0000f490: 6573 2028 7374 725b 5d2c 204f 7074 696f  es (str[], Optio
-0000f4a0: 6e61 6c29 3a0a 2020 2020 2020 2020 2020  nal):.          
-0000f4b0: 2020 2020 2020 4578 706c 6963 6974 206e        Explicit n
-0000f4c0: 616d 6520 6f66 2074 6865 2065 7874 6572  ame of the exter
-0000f4d0: 6e61 6c20 7061 636b 6167 6520 6465 7065  nal package depe
-0000f4e0: 6e64 656e 6369 6573 2e20 4561 6368 2064  ndencies. Each d
-0000f4f0: 6570 656e 6465 6e63 790a 2020 2020 2020  ependency.      
-0000f500: 2020 2020 2020 2020 2020 6973 2061 6464            is add
-0000f510: 6564 2074 6f20 7468 6520 6072 6571 7569  ed to the `requi
-0000f520: 7265 6d65 6e74 732e 7478 7460 2061 7320  rements.txt` as 
-0000f530: 6973 2c20 616e 6420 6361 6e20 6265 206f  is, and can be o
-0000f540: 6620 7468 6520 666f 726d 0a20 2020 2020  f the form.     
-0000f550: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-0000f560: 7274 6564 2069 6e20 6874 7470 733a 2f2f  rted in https://
-0000f570: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
-0000f580: 7461 626c 652f 7265 6665 7265 6e63 652f  table/reference/
-0000f590: 7265 7175 6972 656d 656e 7473 2d66 696c  requirements-fil
-0000f5a0: 652d 666f 726d 6174 2f2e 0a20 2020 2020  e-format/..     
-0000f5b0: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-0000f5c0: 6374 696f 6e5f 7365 7276 6963 655f 6163  ction_service_ac
-0000f5d0: 636f 756e 7420 2873 7472 2c20 4f70 7469  count (str, Opti
-0000f5e0: 6f6e 616c 293a 0a20 2020 2020 2020 2020  onal):.         
-0000f5f0: 2020 2020 2020 2053 6572 7669 6365 2061         Service a
-0000f600: 6363 6f75 6e74 2074 6f20 7573 6520 666f  ccount to use fo
-0000f610: 7220 7468 6520 636c 6f75 6420 6675 6e63  r the cloud func
-0000f620: 7469 6f6e 732e 2049 6620 6e6f 7420 7072  tions. If not pr
-0000f630: 6f76 6964 6564 0a20 2020 2020 2020 2020  ovided.         
-0000f640: 2020 2020 2020 2074 6865 6e20 7468 6520         then the 
-0000f650: 6465 6661 756c 7420 7365 7276 6963 6520  default service 
-0000f660: 6163 636f 756e 7420 776f 756c 6420 6265  account would be
-0000f670: 2075 7365 642e 2053 6565 0a20 2020 2020   used. See.     
-0000f680: 2020 2020 2020 2020 2020 2068 7474 7073             https
-0000f690: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-0000f6a0: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
-0000f6b0: 6373 2f73 6563 7572 696e 672f 6675 6e63  cs/securing/func
-0000f6c0: 7469 6f6e 2d69 6465 6e74 6974 790a 2020  tion-identity.  
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000f6e0: 7220 6d6f 7265 2064 6574 6169 6c73 2e20  r more details. 
-0000f6f0: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
-0000f700: 2074 6865 2073 6572 7669 6365 2061 6363   the service acc
-0000f710: 6f75 6e74 2068 6173 2074 6865 0a20 2020  ount has the.   
-0000f720: 2020 2020 2020 2020 2020 2020 206e 6563               nec
-0000f730: 6573 7361 7279 2049 414d 2070 6572 6d69  essary IAM permi
-0000f740: 7373 696f 6e73 2063 6f6e 6669 6775 7265  ssions configure
-0000f750: 6420 6173 2064 6573 6372 6962 6564 2069  d as described i
-0000f760: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000f770: 2020 6874 7470 733a 2f2f 636c 6f75 642e    https://cloud.
-0000f780: 676f 6f67 6c65 2e63 6f6d 2f66 756e 6374  google.com/funct
-0000f790: 696f 6e73 2f64 6f63 732f 7265 6665 7265  ions/docs/refere
-0000f7a0: 6e63 652f 6961 6d2f 726f 6c65 7323 6164  nce/iam/roles#ad
-0000f7b0: 6469 7469 6f6e 616c 2d63 6f6e 6669 6775  ditional-configu
-0000f7c0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-0000f7d0: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-0000f7e0: 6f6e 5f6b 6d73 5f6b 6579 5f6e 616d 6520  on_kms_key_name 
-0000f7f0: 2873 7472 2c20 4f70 7469 6f6e 616c 293a  (str, Optional):
-0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f810: 2043 7573 746f 6d65 7220 6d61 6e61 6765   Customer manage
-0000f820: 6420 656e 6372 7970 7469 6f6e 206b 6579  d encryption key
-0000f830: 2074 6f20 7072 6f74 6563 7420 636c 6f75   to protect clou
-0000f840: 6420 6675 6e63 7469 6f6e 7320 616e 640a  d functions and.
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 7265 6c61 7465 6420 6461 7461 2061 7420  related data at 
-0000f870: 7265 7374 2e20 5468 6973 2069 7320 6f66  rest. This is of
-0000f880: 2074 6865 2066 6f72 6d61 740a 2020 2020   the format.    
-0000f890: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
-0000f8a0: 6563 7473 2f50 524f 4a45 4354 5f49 442f  ects/PROJECT_ID/
-0000f8b0: 6c6f 6361 7469 6f6e 732f 4c4f 4341 5449  locations/LOCATI
-0000f8c0: 4f4e 2f6b 6579 5269 6e67 732f 4b45 5952  ON/keyRings/KEYR
-0000f8d0: 494e 472f 6372 7970 746f 4b65 7973 2f4b  ING/cryptoKeys/K
-0000f8e0: 4559 2e0a 2020 2020 2020 2020 2020 2020  EY..            
-0000f8f0: 2020 2020 5265 6164 2068 7474 7073 3a2f      Read https:/
-0000f900: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-0000f910: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
-0000f920: 2f73 6563 7572 696e 672f 636d 656b 2066  /securing/cmek f
-0000f930: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-0000f940: 2020 206d 6f72 6520 6465 7461 696c 7320     more details 
-0000f950: 696e 636c 7564 696e 6720 6772 616e 7469  including granti
-0000f960: 6e67 206e 6563 6573 7361 7279 2073 6572  ng necessary ser
-0000f970: 7669 6365 2061 6363 6f75 6e74 730a 2020  vice accounts.  
-0000f980: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-0000f990: 6365 7373 2074 6f20 7468 6520 6b65 792e  cess to the key.
-0000f9a0: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
-0000f9b0: 7564 5f66 756e 6374 696f 6e5f 646f 636b  ud_function_dock
-0000f9c0: 6572 5f72 6570 6f73 6974 6f72 7920 2873  er_repository (s
-0000f9d0: 7472 2c20 4f70 7469 6f6e 616c 293a 0a20  tr, Optional):. 
-0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0000f9f0: 6f63 6b65 7220 7265 706f 7369 746f 7279  ocker repository
-0000fa00: 2063 7265 6174 6564 2077 6974 6820 7468   created with th
-0000fa10: 6520 7361 6d65 2065 6e63 7279 7074 696f  e same encryptio
-0000fa20: 6e20 6b65 7920 6173 0a20 2020 2020 2020  n key as.       
-0000fa30: 2020 2020 2020 2020 2060 636c 6f75 645f           `cloud_
-0000fa40: 6675 6e63 7469 6f6e 5f6b 6d73 5f6b 6579  function_kms_key
-0000fa50: 5f6e 616d 6560 2074 6f20 7374 6f72 6520  _name` to store 
-0000fa60: 656e 6372 7970 7465 6420 6172 7469 6661  encrypted artifa
-0000fa70: 6374 730a 2020 2020 2020 2020 2020 2020  cts.            
-0000fa80: 2020 2020 6372 6561 7465 6420 746f 2073      created to s
-0000fa90: 7570 706f 7274 2074 6865 2063 6c6f 7564  upport the cloud
-0000faa0: 2066 756e 6374 696f 6e2e 2054 6869 7320   function. This 
-0000fab0: 6973 206f 6620 7468 6520 666f 726d 6174  is of the format
-0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fad0: 2070 726f 6a65 6374 732f 5052 4f4a 4543   projects/PROJEC
-0000fae0: 545f 4944 2f6c 6f63 6174 696f 6e73 2f4c  T_ID/locations/L
-0000faf0: 4f43 4154 494f 4e2f 7265 706f 7369 746f  OCATION/reposito
-0000fb00: 7269 6573 2f52 4550 4f53 4954 4f52 595f  ries/REPOSITORY_
-0000fb10: 4e41 4d45 2e0a 2020 2020 2020 2020 2020  NAME..          
-0000fb20: 2020 2020 2020 466f 7220 6d6f 7265 2064        For more d
-0000fb30: 6574 6169 6c73 2073 6565 0a20 2020 2020  etails see.     
-0000fb40: 2020 2020 2020 2020 2020 2068 7474 7073             https
-0000fb50: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-0000fb60: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
-0000fb70: 6373 2f73 6563 7572 696e 672f 636d 656b  cs/securing/cmek
-0000fb80: 2362 6566 6f72 655f 796f 755f 6265 6769  #before_you_begi
-0000fb90: 6e2e 0a20 2020 2020 2020 2052 6574 7572  n..        Retur
-0000fba0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000fbb0: 6361 6c6c 6162 6c65 3a20 4120 7265 6d6f  callable: A remo
-0000fbc0: 7465 2066 756e 6374 696f 6e20 6f62 6a65  te function obje
-0000fbd0: 6374 2070 6f69 6e74 696e 6720 746f 2074  ct pointing to t
-0000fbe0: 6865 2063 6c6f 7564 2061 7373 6574 7320  he cloud assets 
-0000fbf0: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
-0000fc00: 2020 2020 696e 2074 6865 2062 6163 6b67      in the backg
-0000fc10: 726f 756e 6420 746f 2073 7570 706f 7274  round to support
-0000fc20: 2074 6865 2072 656d 6f74 6520 6578 6563   the remote exec
-0000fc30: 7574 696f 6e2e 2054 6865 2063 6c6f 7564  ution. The cloud
-0000fc40: 2061 7373 6574 7320 6361 6e20 6265 0a20   assets can be. 
-0000fc50: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-0000fc60: 6564 2074 6872 6f75 6768 2074 6865 2066  ed through the f
-0000fc70: 6f6c 6c6f 7769 6e67 2070 726f 7065 7274  ollowing propert
-0000fc80: 6965 7320 7365 7420 696e 2074 6865 206f  ies set in the o
-0000fc90: 626a 6563 743a 0a0a 2020 2020 2020 2020  bject:..        
-0000fca0: 2020 2020 6062 6967 6672 616d 6573 5f63      `bigframes_c
-0000fcb0: 6c6f 7564 5f66 756e 6374 696f 6e60 202d  loud_function` -
-0000fcc0: 2054 6865 2067 6f6f 676c 6520 636c 6f75   The google clou
-0000fcd0: 6420 6675 6e63 7469 6f6e 2064 6570 6c6f  d function deplo
-0000fce0: 7965 6420 666f 7220 7468 6520 7573 6572  yed for the user
-0000fcf0: 2064 6566 696e 6564 2063 6f64 652e 0a0a   defined code...
-0000fd00: 2020 2020 2020 2020 2020 2020 6062 6967              `big
-0000fd10: 6672 616d 6573 5f72 656d 6f74 655f 6675  frames_remote_fu
-0000fd20: 6e63 7469 6f6e 6020 2d20 5468 6520 6269  nction` - The bi
-0000fd30: 6771 7565 7279 2072 656d 6f74 6520 6675  gquery remote fu
-0000fd40: 6e63 7469 6f6e 2063 6170 6162 6c65 206f  nction capable o
-0000fd50: 6620 6361 6c6c 696e 6720 696e 746f 2060  f calling into `
-0000fd60: 6269 6766 7261 6d65 735f 636c 6f75 645f  bigframes_cloud_
-0000fd70: 6675 6e63 7469 6f6e 602e 0a20 2020 2020  function`..     
-0000fd80: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000fd90: 6574 7572 6e20 6269 6766 7261 6d65 735f  eturn bigframes_
-0000fda0: 7266 280a 2020 2020 2020 2020 2020 2020  rf(.            
-0000fdb0: 696e 7075 745f 7479 7065 732c 0a20 2020  input_types,.   
-0000fdc0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000fdd0: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-0000fde0: 2020 7365 7373 696f 6e3d 7365 6c66 2c0a    session=self,.
-0000fdf0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000fe00: 7365 743d 6461 7461 7365 742c 0a20 2020  set=dataset,.   
-0000fe10: 2020 2020 2020 2020 2062 6967 7175 6572           bigquer
-0000fe20: 795f 636f 6e6e 6563 7469 6f6e 3d62 6967  y_connection=big
-0000fe30: 7175 6572 795f 636f 6e6e 6563 7469 6f6e  query_connection
-0000fe40: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000fe50: 7573 653d 7265 7573 652c 0a20 2020 2020  use=reuse,.     
-0000fe60: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-0000fe70: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-0000fe80: 636b 6167 6573 3d70 6163 6b61 6765 732c  ckages=packages,
-0000fe90: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
-0000fea0: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
-0000feb0: 6963 655f 6163 636f 756e 743d 636c 6f75  ice_account=clou
-0000fec0: 645f 6675 6e63 7469 6f6e 5f73 6572 7669  d_function_servi
-0000fed0: 6365 5f61 6363 6f75 6e74 2c0a 2020 2020  ce_account,.    
-0000fee0: 2020 2020 2020 2020 636c 6f75 645f 6675          cloud_fu
-0000fef0: 6e63 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e  nction_kms_key_n
-0000ff00: 616d 653d 636c 6f75 645f 6675 6e63 7469  ame=cloud_functi
-0000ff10: 6f6e 5f6b 6d73 5f6b 6579 5f6e 616d 652c  on_kms_key_name,
-0000ff20: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
-0000ff30: 7564 5f66 756e 6374 696f 6e5f 646f 636b  ud_function_dock
-0000ff40: 6572 5f72 6570 6f73 6974 6f72 793d 636c  er_repository=cl
-0000ff50: 6f75 645f 6675 6e63 7469 6f6e 5f64 6f63  oud_function_doc
-0000ff60: 6b65 725f 7265 706f 7369 746f 7279 2c0a  ker_repository,.
-0000ff70: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000ff80: 6566 2072 6561 645f 6762 715f 6675 6e63  ef read_gbq_func
-0000ff90: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
-0000ffa0: 6c66 2c0a 2020 2020 2020 2020 6675 6e63  lf,.        func
-0000ffb0: 7469 6f6e 5f6e 616d 653a 2073 7472 2c0a  tion_name: str,.
-0000ffc0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0000ffd0: 2222 4c6f 6164 7320 6120 4269 6751 7565  ""Loads a BigQue
-0000ffe0: 7279 2066 756e 6374 696f 6e20 6672 6f6d  ry function from
-0000fff0: 2042 6967 5175 6572 792e 0a0a 2020 2020   BigQuery...    
-00010000: 2020 2020 5468 656e 2069 7420 6361 6e20      Then it can 
-00010010: 6265 2061 7070 6c69 6564 2074 6f20 6120  be applied to a 
-00010020: 4461 7461 4672 616d 6520 6f72 2053 6572  DataFrame or Ser
-00010030: 6965 732e 0a0a 2020 2020 2020 2020 2e2e  ies...        ..
-00010040: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
-00010050: 2020 2020 5468 6520 7265 7475 726e 2074      The return t
-00010060: 7970 6520 6f66 2074 6865 2066 756e 6374  ype of the funct
-00010070: 696f 6e20 6d75 7374 2062 6520 6578 706c  ion must be expl
-00010080: 6963 6974 6c79 2073 7065 6369 6669 6564  icitly specified
-00010090: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
-000100a0: 2020 2020 6675 6e63 7469 6f6e 2773 206f      function's o
-000100b0: 7269 6769 6e61 6c20 6465 6669 6e69 7469  riginal definiti
-000100c0: 6f6e 2065 7665 6e20 6966 206e 6f74 206f  on even if not o
-000100d0: 7468 6572 7769 7365 2072 6571 7569 7265  therwise require
-000100e0: 642e 0a0a 2020 2020 2020 2020 4269 6751  d...        BigQ
-000100f0: 7565 7279 2055 7469 6c73 2070 726f 7669  uery Utils provi
-00010100: 6465 7320 6d61 6e79 2070 7562 6c69 6320  des many public 
-00010110: 6675 6e63 7469 6f6e 7320 756e 6465 7220  functions under 
-00010120: 7468 6520 6060 6271 7574 696c 6060 2070  the ``bqutil`` p
-00010130: 726f 6a65 6374 206f 6e20 476f 6f67 6c65  roject on Google
-00010140: 2043 6c6f 7564 2050 6c61 7466 6f72 6d20   Cloud Platform 
-00010150: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
-00010160: 2853 6565 3a20 6874 7470 733a 2f2f 6769  (See: https://gi
-00010170: 7468 7562 2e63 6f6d 2f47 6f6f 676c 6543  thub.com/GoogleC
-00010180: 6c6f 7564 506c 6174 666f 726d 2f62 6967  loudPlatform/big
-00010190: 7175 6572 792d 7574 696c 732f 7472 6565  query-utils/tree
-000101a0: 2f6d 6173 7465 722f 7564 6673 2375 7369  /master/udfs#usi
-000101b0: 6e67 2d74 6865 2d75 6466 7329 2e0a 2020  ng-the-udfs)..  
-000101c0: 2020 2020 2020 596f 7520 6361 6e20 6368        You can ch
-000101d0: 6563 6b6f 7574 2043 6f6d 6d75 6e69 7479  eckout Community
-000101e0: 2055 4446 7320 746f 2075 7365 2063 6f6d   UDFs to use com
-000101f0: 6d75 6e69 7479 2d63 6f6e 7472 6962 7574  munity-contribut
-00010200: 6564 2066 756e 6374 696f 6e73 2e0a 2020  ed functions..  
-00010210: 2020 2020 2020 2853 6565 3a20 6874 7470        (See: http
-00010220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00010230: 6f6f 676c 6543 6c6f 7564 506c 6174 666f  oogleCloudPlatfo
-00010240: 726d 2f62 6967 7175 6572 792d 7574 696c  rm/bigquery-util
-00010250: 732f 7472 6565 2f6d 6173 7465 722f 7564  s/tree/master/ud
-00010260: 6673 2f63 6f6d 6d75 6e69 7479 2363 6f6d  fs/community#com
-00010270: 6d75 6e69 7479 2d75 6466 7329 2e0a 0a20  munity-udfs)... 
-00010280: 2020 2020 2020 202a 2a45 7861 6d70 6c65         **Example
-00010290: 733a 2a2a 0a0a 2020 2020 2020 2020 5573  s:**..        Us
-000102a0: 6520 7468 6520 6060 6377 5f6c 6f77 6572  e the ``cw_lower
-000102b0: 5f63 6173 655f 6173 6369 695f 6f6e 6c79  _case_ascii_only
-000102c0: 6060 2066 756e 6374 696f 6e20 6672 6f6d  `` function from
-000102d0: 2043 6f6d 6d75 6e69 7479 2055 4446 732e   Community UDFs.
-000102e0: 0a20 2020 2020 2020 2028 6874 7470 733a  .        (https:
-000102f0: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
-00010300: 676c 6543 6c6f 7564 506c 6174 666f 726d  gleCloudPlatform
-00010310: 2f62 6967 7175 6572 792d 7574 696c 732f  /bigquery-utils/
-00010320: 626c 6f62 2f6d 6173 7465 722f 7564 6673  blob/master/udfs
-00010330: 2f63 6f6d 6d75 6e69 7479 2f63 775f 6c6f  /community/cw_lo
-00010340: 7765 725f 6361 7365 5f61 7363 6969 5f6f  wer_case_ascii_o
-00010350: 6e6c 792e 7371 6c78 290a 0a20 2020 2020  nly.sqlx)..     
-00010360: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00010370: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
-00010380: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
-00010390: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
-000103a0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
-000103b0: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
-000103c0: 650a 0a20 2020 2020 2020 2020 2020 203e  e..            >
-000103d0: 3e3e 2064 6620 3d20 6270 642e 4461 7461  >> df = bpd.Data
-000103e0: 4672 616d 6528 7b27 6964 273a 205b 312c  Frame({'id': [1,
-000103f0: 2032 2c20 335d 2c20 276e 616d 6527 3a20   2, 3], 'name': 
-00010400: 5b27 4155 52c3 894c 4945 272c 2027 43c3  ['AUR..LIE', 'C.
-00010410: 894c 4553 5449 4e45 272c 2027 4441 5048  .LESTINE', 'DAPH
-00010420: 4ec3 8927 5d7d 290a 2020 2020 2020 2020  N..']}).        
-00010430: 2020 2020 3e3e 3e20 6466 0a20 2020 2020      >>> df.     
-00010440: 2020 2020 2020 2020 2020 6964 2020 2020            id    
-00010450: 2020 206e 616d 650a 2020 2020 2020 2020     name.        
-00010460: 2020 2020 3020 2020 3120 2020 2041 5552      0   1    AUR
-00010470: c389 4c49 450a 2020 2020 2020 2020 2020  ..LIE.          
-00010480: 2020 3120 2020 3220 2043 c389 4c45 5354    1   2  C..LEST
-00010490: 494e 450a 2020 2020 2020 2020 2020 2020  INE.            
-000104a0: 3220 2020 3320 2020 2020 4441 5048 4ec3  2   3     DAPHN.
-000104b0: 890a 2020 2020 2020 2020 2020 2020 3c42  ..            <B
-000104c0: 4c41 4e4b 4c49 4e45 3e0a 2020 2020 2020  LANKLINE>.      
-000104d0: 2020 2020 2020 5b33 2072 6f77 7320 7820        [3 rows x 
-000104e0: 3220 636f 6c75 6d6e 735d 0a0a 2020 2020  2 columns]..    
-000104f0: 2020 2020 2020 2020 3e3e 3e20 6675 6e63          >>> func
-00010500: 203d 2062 7064 2e72 6561 645f 6762 715f   = bpd.read_gbq_
-00010510: 6675 6e63 7469 6f6e 2822 6271 7574 696c  function("bqutil
-00010520: 2e66 6e2e 6377 5f6c 6f77 6572 5f63 6173  .fn.cw_lower_cas
-00010530: 655f 6173 6369 695f 6f6e 6c79 2229 0a20  e_ascii_only"). 
-00010540: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
-00010550: 6631 203d 2064 662e 6173 7369 676e 286e  f1 = df.assign(n
-00010560: 6577 5f6e 616d 653d 6466 5b27 6e61 6d65  ew_name=df['name
-00010570: 275d 2e61 7070 6c79 2866 756e 6329 290a  '].apply(func)).
-00010580: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00010590: 6466 310a 2020 2020 2020 2020 2020 2020  df1.            
-000105a0: 2020 2069 6420 2020 2020 2020 6e61 6d65     id       name
-000105b0: 2020 206e 6577 5f6e 616d 650a 2020 2020     new_name.    
-000105c0: 2020 2020 2020 2020 3020 2020 3120 2020          0   1   
-000105d0: 2041 5552 c389 4c49 4520 2020 2061 7572   AUR..LIE    aur
-000105e0: c389 6c69 650a 2020 2020 2020 2020 2020  ..lie.          
-000105f0: 2020 3120 2020 3220 2043 c389 4c45 5354    1   2  C..LEST
-00010600: 494e 4520 2063 c389 6c65 7374 696e 650a  INE  c..lestine.
-00010610: 2020 2020 2020 2020 2020 2020 3220 2020              2   
-00010620: 3320 2020 2020 4441 5048 4ec3 8920 2020  3     DAPHN..   
-00010630: 2020 6461 7068 6ec3 890a 2020 2020 2020    daphn...      
-00010640: 2020 2020 2020 3c42 4c41 4e4b 4c49 4e45        <BLANKLINE
-00010650: 3e0a 2020 2020 2020 2020 2020 2020 5b33  >.            [3
-00010660: 2072 6f77 7320 7820 3320 636f 6c75 6d6e   rows x 3 column
-00010670: 735d 0a0a 2020 2020 2020 2020 4172 6773  s]..        Args
-00010680: 3a0a 2020 2020 2020 2020 2020 2020 6675  :.            fu
-00010690: 6e63 7469 6f6e 5f6e 616d 6520 2873 7472  nction_name (str
-000106a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000106b0: 2020 2074 6865 2066 756e 6374 696f 6e27     the function'
-000106c0: 7320 6e61 6d65 2069 6e20 4269 6751 7565  s name in BigQue
-000106d0: 7279 2069 6e20 7468 6520 666f 726d 6174  ry in the format
-000106e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106f0: 2060 7072 6f6a 6563 745f 6964 2e64 6174   `project_id.dat
-00010700: 6173 6574 5f69 642e 6675 6e63 7469 6f6e  aset_id.function
-00010710: 5f6e 616d 6560 2c20 6f72 0a20 2020 2020  _name`, or.     
-00010720: 2020 2020 2020 2020 2020 2060 6461 7461             `data
-00010730: 7365 745f 6964 2e66 756e 6374 696f 6e5f  set_id.function_
-00010740: 6e61 6d65 6020 746f 206c 6f61 6420 6672  name` to load fr
-00010750: 6f6d 2074 6865 2064 6566 6175 6c74 2070  om the default p
-00010760: 726f 6a65 6374 2c20 6f72 0a20 2020 2020  roject, or.     
-00010770: 2020 2020 2020 2020 2020 2060 6675 6e63             `func
-00010780: 7469 6f6e 5f6e 616d 6560 2074 6f20 6c6f  tion_name` to lo
-00010790: 6164 2066 726f 6d20 7468 6520 6465 6661  ad from the defa
-000107a0: 756c 7420 7072 6f6a 6563 7420 616e 6420  ult project and 
-000107b0: 7468 6520 6461 7461 7365 740a 2020 2020  the dataset.    
-000107c0: 2020 2020 2020 2020 2020 2020 6173 736f              asso
-000107d0: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
-000107e0: 6375 7272 656e 7420 7365 7373 696f 6e2e  current session.
-000107f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00010800: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00010810: 616c 6c61 626c 653a 2041 2066 756e 6374  allable: A funct
-00010820: 696f 6e20 6f62 6a65 6374 2070 6f69 6e74  ion object point
-00010830: 696e 6720 746f 2074 6865 2042 6967 5175  ing to the BigQu
-00010840: 6572 7920 6675 6e63 7469 6f6e 2072 6561  ery function rea
-00010850: 640a 2020 2020 2020 2020 2020 2020 6672  d.            fr
-00010860: 6f6d 2042 6967 5175 6572 792e 0a0a 2020  om BigQuery...  
-00010870: 2020 2020 2020 2020 2020 5468 6520 6f62            The ob
-00010880: 6a65 6374 2069 7320 7369 6d69 6c61 7220  ject is similar 
-00010890: 746f 2074 6865 206f 6e65 2063 7265 6174  to the one creat
-000108a0: 6564 2062 7920 7468 6520 6072 656d 6f74  ed by the `remot
-000108b0: 655f 6675 6e63 7469 6f6e 600a 2020 2020  e_function`.    
-000108c0: 2020 2020 2020 2020 6465 636f 7261 746f          decorato
-000108d0: 722c 2069 6e63 6c75 6469 6e67 2074 6865  r, including the
-000108e0: 2060 6269 6766 7261 6d65 735f 7265 6d6f   `bigframes_remo
-000108f0: 7465 5f66 756e 6374 696f 6e60 2070 726f  te_function` pro
-00010900: 7065 7274 792c 2062 7574 0a20 2020 2020  perty, but.     
-00010910: 2020 2020 2020 206e 6f74 2069 6e63 6c75         not inclu
-00010920: 6469 6e67 2074 6865 2060 6269 6766 7261  ding the `bigfra
-00010930: 6d65 735f 636c 6f75 645f 6675 6e63 7469  mes_cloud_functi
-00010940: 6f6e 6020 7072 6f70 6572 7479 2e0a 2020  on` property..  
-00010950: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00010960: 2020 2072 6574 7572 6e20 6269 6766 7261     return bigfra
-00010970: 6d65 735f 7267 6628 0a20 2020 2020 2020  mes_rgf(.       
-00010980: 2020 2020 2066 756e 6374 696f 6e5f 6e61       function_na
-00010990: 6d65 3d66 756e 6374 696f 6e5f 6e61 6d65  me=function_name
-000109a0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-000109b0: 7373 696f 6e3d 7365 6c66 2c0a 2020 2020  ssion=self,.    
-000109c0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
-000109d0: 7072 6570 6172 655f 7175 6572 795f 6a6f  prepare_query_jo
-000109e0: 625f 636f 6e66 6967 280a 2020 2020 2020  b_config(.      
-000109f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00010a00: 6a6f 625f 636f 6e66 6967 3a20 4f70 7469  job_config: Opti
-00010a10: 6f6e 616c 5b62 6967 7175 6572 792e 5175  onal[bigquery.Qu
-00010a20: 6572 794a 6f62 436f 6e66 6967 5d20 3d20  eryJobConfig] = 
-00010a30: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2062  None,.    ) -> b
-00010a40: 6967 7175 6572 792e 5175 6572 794a 6f62  igquery.QueryJob
-00010a50: 436f 6e66 6967 3a0a 2020 2020 2020 2020  Config:.        
-00010a60: 6966 206a 6f62 5f63 6f6e 6669 6720 6973  if job_config is
-00010a70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00010a80: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
-00010a90: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00010aa0: 6243 6f6e 6669 6728 290a 2020 2020 2020  bConfig().      
-00010ab0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00010ac0: 2020 2020 2320 4372 6561 7465 2061 2063      # Create a c
-00010ad0: 6f70 7920 736f 2074 6861 7420 7765 2064  opy so that we d
-00010ae0: 6f6e 2774 206d 7574 6174 6520 7468 6520  on't mutate the 
-00010af0: 6f72 6967 696e 616c 2063 6f6e 6669 6720  original config 
-00010b00: 7061 7373 6564 0a20 2020 2020 2020 2020  passed.         
-00010b10: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
-00010b20: 7479 7069 6e67 2e63 6173 7428 0a20 2020  typing.cast(.   
-00010b30: 2020 2020 2020 2020 2020 2020 2062 6967               big
-00010b40: 7175 6572 792e 5175 6572 794a 6f62 436f  query.QueryJobCo
-00010b50: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
-00010b60: 2020 2020 2020 6269 6771 7565 7279 2e51        bigquery.Q
-00010b70: 7565 7279 4a6f 6243 6f6e 6669 672e 6672  ueryJobConfig.fr
-00010b80: 6f6d 5f61 7069 5f72 6570 7228 6a6f 625f  om_api_repr(job_
-00010b90: 636f 6e66 6967 2e74 6f5f 6170 695f 7265  config.to_api_re
-00010ba0: 7072 2829 292c 0a20 2020 2020 2020 2020  pr()),.         
-00010bb0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-00010bc0: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
-00010bd0: 6e73 2e63 6f6d 7075 7465 2e6d 6178 696d  ns.compute.maxim
-00010be0: 756d 5f62 7974 6573 5f62 696c 6c65 6420  um_bytes_billed 
-00010bf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010c00: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-00010c10: 6669 672e 6d61 7869 6d75 6d5f 6279 7465  fig.maximum_byte
-00010c20: 735f 6269 6c6c 6564 203d 2028 0a20 2020  s_billed = (.   
-00010c30: 2020 2020 2020 2020 2020 2020 2062 6967               big
-00010c40: 6672 616d 6573 2e6f 7074 696f 6e73 2e63  frames.options.c
-00010c50: 6f6d 7075 7465 2e6d 6178 696d 756d 5f62  ompute.maximum_b
-00010c60: 7974 6573 5f62 696c 6c65 640a 2020 2020  ytes_billed.    
-00010c70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00010c80: 2020 2069 6620 7365 6c66 2e5f 6271 5f6b     if self._bq_k
-00010c90: 6d73 5f6b 6579 5f6e 616d 653a 0a20 2020  ms_key_name:.   
-00010ca0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-00010cb0: 6669 672e 6465 7374 696e 6174 696f 6e5f  fig.destination_
-00010cc0: 656e 6372 7970 7469 6f6e 5f63 6f6e 6669  encryption_confi
-00010cd0: 6775 7261 7469 6f6e 203d 2028 0a20 2020  guration = (.   
-00010ce0: 2020 2020 2020 2020 2020 2020 2062 6967               big
-00010cf0: 7175 6572 792e 456e 6372 7970 7469 6f6e  query.Encryption
-00010d00: 436f 6e66 6967 7572 6174 696f 6e28 6b6d  Configuration(km
-00010d10: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
-00010d20: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
-00010d30: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00010d40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010d50: 6a6f 625f 636f 6e66 6967 0a0a 2020 2020  job_config..    
-00010d60: 6465 6620 5f70 7265 7061 7265 5f6c 6f61  def _prepare_loa
-00010d70: 645f 6a6f 625f 636f 6e66 6967 2873 656c  d_job_config(sel
-00010d80: 6629 202d 3e20 6269 6771 7565 7279 2e4c  f) -> bigquery.L
-00010d90: 6f61 644a 6f62 436f 6e66 6967 3a0a 2020  oadJobConfig:.  
-00010da0: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-00010db0: 2063 6f70 7920 736f 2074 6861 7420 7765   copy so that we
-00010dc0: 2064 6f6e 2774 206d 7574 6174 6520 7468   don't mutate th
-00010dd0: 6520 6f72 6967 696e 616c 2063 6f6e 6669  e original confi
-00010de0: 6720 7061 7373 6564 0a20 2020 2020 2020  g passed.       
-00010df0: 206a 6f62 5f63 6f6e 6669 6720 3d20 6269   job_config = bi
-00010e00: 6771 7565 7279 2e4c 6f61 644a 6f62 436f  gquery.LoadJobCo
-00010e10: 6e66 6967 2829 0a0a 2020 2020 2020 2020  nfig()..        
-00010e20: 6966 2073 656c 662e 5f62 715f 6b6d 735f  if self._bq_kms_
-00010e30: 6b65 795f 6e61 6d65 3a0a 2020 2020 2020  key_name:.      
-00010e40: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00010e50: 2e64 6573 7469 6e61 7469 6f6e 5f65 6e63  .destination_enc
-00010e60: 7279 7074 696f 6e5f 636f 6e66 6967 7572  ryption_configur
-00010e70: 6174 696f 6e20 3d20 280a 2020 2020 2020  ation = (.      
-00010e80: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
-00010e90: 7279 2e45 6e63 7279 7074 696f 6e43 6f6e  ry.EncryptionCon
-00010ea0: 6669 6775 7261 7469 6f6e 286b 6d73 5f6b  figuration(kms_k
-00010eb0: 6579 5f6e 616d 653d 7365 6c66 2e5f 6271  ey_name=self._bq
-00010ec0: 5f6b 6d73 5f6b 6579 5f6e 616d 6529 0a20  _kms_key_name). 
-00010ed0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00010ee0: 2020 2020 2020 7265 7475 726e 206a 6f62        return job
-00010ef0: 5f63 6f6e 6669 670a 0a20 2020 2064 6566  _config..    def
-00010f00: 205f 7072 6570 6172 655f 636f 7079 5f6a   _prepare_copy_j
-00010f10: 6f62 5f63 6f6e 6669 6728 7365 6c66 2920  ob_config(self) 
-00010f20: 2d3e 2062 6967 7175 6572 792e 436f 7079  -> bigquery.Copy
-00010f30: 4a6f 6243 6f6e 6669 673a 0a20 2020 2020  JobConfig:.     
-00010f40: 2020 2023 2043 7265 6174 6520 6120 636f     # Create a co
-00010f50: 7079 2073 6f20 7468 6174 2077 6520 646f  py so that we do
-00010f60: 6e27 7420 6d75 7461 7465 2074 6865 206f  n't mutate the o
-00010f70: 7269 6769 6e61 6c20 636f 6e66 6967 2070  riginal config p
-00010f80: 6173 7365 640a 2020 2020 2020 2020 6a6f  assed.        jo
-00010f90: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
-00010fa0: 6572 792e 436f 7079 4a6f 6243 6f6e 6669  ery.CopyJobConfi
-00010fb0: 6728 290a 0a20 2020 2020 2020 2069 6620  g()..        if 
-00010fc0: 7365 6c66 2e5f 6271 5f6b 6d73 5f6b 6579  self._bq_kms_key
-00010fd0: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
-00010fe0: 2020 206a 6f62 5f63 6f6e 6669 672e 6465     job_config.de
-00010ff0: 7374 696e 6174 696f 6e5f 656e 6372 7970  stination_encryp
-00011000: 7469 6f6e 5f63 6f6e 6669 6775 7261 7469  tion_configurati
-00011010: 6f6e 203d 2028 0a20 2020 2020 2020 2020  on = (.         
-00011020: 2020 2020 2020 2062 6967 7175 6572 792e         bigquery.
-00011030: 456e 6372 7970 7469 6f6e 436f 6e66 6967  EncryptionConfig
-00011040: 7572 6174 696f 6e28 6b6d 735f 6b65 795f  uration(kms_key_
-00011050: 6e61 6d65 3d73 656c 662e 5f62 715f 6b6d  name=self._bq_km
-00011060: 735f 6b65 795f 6e61 6d65 290a 2020 2020  s_key_name).    
-00011070: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00011080: 2020 2072 6574 7572 6e20 6a6f 625f 636f     return job_co
-00011090: 6e66 6967 0a0a 2020 2020 6465 6620 5f73  nfig..    def _s
-000110a0: 7461 7274 5f71 7565 7279 280a 2020 2020  tart_query(.    
-000110b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000110c0: 2020 7371 6c3a 2073 7472 2c0a 2020 2020    sql: str,.    
-000110d0: 2020 2020 6a6f 625f 636f 6e66 6967 3a20      job_config: 
-000110e0: 4f70 7469 6f6e 616c 5b62 6967 7175 6572  Optional[bigquer
-000110f0: 792e 6a6f 622e 5175 6572 794a 6f62 436f  y.job.QueryJobCo
-00011100: 6e66 6967 5d20 3d20 4e6f 6e65 2c0a 2020  nfig] = None,.  
-00011110: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
-00011120: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-00011130: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00011140: 2074 696d 656f 7574 3a20 4f70 7469 6f6e   timeout: Option
-00011150: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
-00011160: 2c0a 2020 2020 2920 2d3e 2054 7570 6c65  ,.    ) -> Tuple
-00011170: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
-00011180: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
-00011190: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
-000111a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000111b0: 2020 2020 2053 7461 7274 7320 4269 6751       Starts BigQ
-000111c0: 7565 7279 2071 7565 7279 206a 6f62 2061  uery query job a
-000111d0: 6e64 2077 6169 7473 2066 6f72 2072 6573  nd waits for res
-000111e0: 756c 7473 2e0a 2020 2020 2020 2020 2222  ults..        ""
-000111f0: 220a 2020 2020 2020 2020 6a6f 625f 636f  ".        job_co
-00011200: 6e66 6967 203d 2073 656c 662e 5f70 7265  nfig = self._pre
-00011210: 7061 7265 5f71 7565 7279 5f6a 6f62 5f63  pare_query_job_c
-00011220: 6f6e 6669 6728 6a6f 625f 636f 6e66 6967  onfig(job_config
-00011230: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011240: 2062 6967 6672 616d 6573 2e73 6573 7369   bigframes.sessi
-00011250: 6f6e 2e5f 696f 2e62 6967 7175 6572 792e  on._io.bigquery.
-00011260: 7374 6172 745f 7175 6572 795f 7769 7468  start_query_with
-00011270: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
-00011280: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
-00011290: 6e74 2c20 7371 6c2c 206a 6f62 5f63 6f6e  nt, sql, job_con
-000112a0: 6669 672c 206d 6178 5f72 6573 756c 7473  fig, max_results
-000112b0: 2c20 7469 6d65 6f75 740a 2020 2020 2020  , timeout.      
-000112c0: 2020 290a 0a20 2020 2064 6566 205f 7374    )..    def _st
-000112d0: 6172 745f 7175 6572 795f 6d6c 5f64 646c  art_query_ml_ddl
-000112e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000112f0: 2020 2020 2020 2020 7371 6c3a 2073 7472          sql: str
-00011300: 2c0a 2020 2020 2920 2d3e 2054 7570 6c65  ,.    ) -> Tuple
-00011310: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
-00011320: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
-00011330: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
-00011340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011350: 2020 2020 2053 7461 7274 7320 4269 6751       Starts BigQ
-00011360: 7565 7279 204d 4c20 4444 4c20 7175 6572  uery ML DDL quer
-00011370: 7920 6a6f 6220 2843 5245 4154 4520 4d4f  y job (CREATE MO
-00011380: 4445 4c2f 414c 5445 5220 4d4f 4445 4c2f  DEL/ALTER MODEL/
-00011390: 2e2e 2e29 2061 6e64 0a20 2020 2020 2020  ...) and.       
-000113a0: 2077 6169 7473 2066 6f72 2072 6573 756c   waits for resul
-000113b0: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
-000113c0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-000113d0: 6967 203d 2073 656c 662e 5f70 7265 7061  ig = self._prepa
-000113e0: 7265 5f71 7565 7279 5f6a 6f62 5f63 6f6e  re_query_job_con
-000113f0: 6669 6728 290a 0a20 2020 2020 2020 2023  fig()..        #
-00011400: 2042 514d 4c20 6578 7065 6374 7320 6b6d   BQML expects km
-00011410: 735f 6b65 795f 6e61 6d65 2074 6872 6f75  s_key_name throu
-00011420: 6768 204f 5054 494f 4e53 2061 6e64 206e  gh OPTIONS and n
-00011430: 6f74 2074 6872 6f75 6768 206a 6f62 2063  ot through job c
-00011440: 6f6e 6669 672c 0a20 2020 2020 2020 2023  onfig,.        #
-00011450: 2073 6f20 7765 206d 7573 7420 7265 7365   so we must rese
-00011460: 7420 616e 7920 656e 6372 7970 7469 6f6e  t any encryption
-00011470: 2073 6574 2069 6e20 7468 6520 6a6f 6220   set in the job 
-00011480: 636f 6e66 6967 0a20 2020 2020 2020 2023  config.        #
-00011490: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-000114a0: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
-000114b0: 7279 2f64 6f63 732f 6375 7374 6f6d 6572  ry/docs/customer
-000114c0: 2d6d 616e 6167 6564 2d65 6e63 7279 7074  -managed-encrypt
-000114d0: 696f 6e23 656e 6372 7970 742d 6d6f 6465  ion#encrypt-mode
-000114e0: 6c0a 2020 2020 2020 2020 6a6f 625f 636f  l.        job_co
-000114f0: 6e66 6967 2e64 6573 7469 6e61 7469 6f6e  nfig.destination
-00011500: 5f65 6e63 7279 7074 696f 6e5f 636f 6e66  _encryption_conf
-00011510: 6967 7572 6174 696f 6e20 3d20 4e6f 6e65  iguration = None
-00011520: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00011530: 2062 6967 6672 616d 6573 2e73 6573 7369   bigframes.sessi
-00011540: 6f6e 2e5f 696f 2e62 6967 7175 6572 792e  on._io.bigquery.
-00011550: 7374 6172 745f 7175 6572 795f 7769 7468  start_query_with
-00011560: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
-00011570: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
-00011580: 6e74 2c20 7371 6c2c 206a 6f62 5f63 6f6e  nt, sql, job_con
-00011590: 6669 670a 2020 2020 2020 2020 290a 0a20  fig.        ).. 
-000115a0: 2020 2064 6566 205f 6361 6368 655f 7769     def _cache_wi
-000115b0: 7468 5f63 6c75 7374 6572 5f63 6f6c 7328  th_cluster_cols(
-000115c0: 0a20 2020 2020 2020 2073 656c 662c 2061  .        self, a
-000115d0: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
-000115e0: 2e41 7272 6179 5661 6c75 652c 2063 6c75  .ArrayValue, clu
-000115f0: 7374 6572 5f63 6f6c 733a 2074 7970 696e  ster_cols: typin
-00011600: 672e 5365 7175 656e 6365 5b73 7472 5d0a  g.Sequence[str].
-00011610: 2020 2020 2920 2d3e 2063 6f72 652e 4172      ) -> core.Ar
-00011620: 7261 7956 616c 7565 3a0a 2020 2020 2020  rayValue:.      
-00011630: 2020 2222 2245 7865 6375 7465 7320 7468    """Executes th
-00011640: 6520 7175 6572 7920 616e 6420 7573 6573  e query and uses
-00011650: 2074 6865 2072 6573 756c 7469 6e67 2074   the resulting t
-00011660: 6162 6c65 2074 6f20 7265 7772 6974 6520  able to rewrite 
-00011670: 6675 7475 7265 2065 7865 6375 7469 6f6e  future execution
-00011680: 732e 2222 220a 2020 2020 2020 2020 2320  s.""".        # 
-00011690: 544f 444f 3a20 5573 6520 7468 6973 2066  TODO: Use this f
-000116a0: 6f72 2061 6c6c 2065 7865 6375 7469 6f6e  or all execution
-000116b0: 733f 2050 726f 626c 656d 2069 7320 7468  s? Problem is th
-000116c0: 6174 2063 6163 6869 6e67 206d 6174 6572  at caching mater
-000116d0: 6961 6c69 7a65 7320 6578 7472 610a 2020  ializes extra.  
-000116e0: 2020 2020 2020 2320 6f72 6465 7269 6e67        # ordering
-000116f0: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
-00011700: 2063 6f6d 7069 6c65 645f 7661 6c75 6520   compiled_value 
-00011710: 3d20 7365 6c66 2e5f 636f 6d70 696c 655f  = self._compile_
-00011720: 6f72 6465 7265 6428 6172 7261 795f 7661  ordered(array_va
-00011730: 6c75 6529 0a0a 2020 2020 2020 2020 6962  lue)..        ib
-00011740: 6973 5f65 7870 7220 3d20 636f 6d70 696c  is_expr = compil
-00011750: 6564 5f76 616c 7565 2e5f 746f 5f69 6269  ed_value._to_ibi
-00011760: 735f 6578 7072 280a 2020 2020 2020 2020  s_expr(.        
-00011770: 2020 2020 6f72 6465 7269 6e67 5f6d 6f64      ordering_mod
-00011780: 653d 2275 6e6f 7264 6572 6564 222c 2065  e="unordered", e
-00011790: 7870 6f73 655f 6869 6464 656e 5f63 6f6c  xpose_hidden_col
-000117a0: 733d 5472 7565 0a20 2020 2020 2020 2029  s=True.        )
-000117b0: 0a20 2020 2020 2020 2074 6d70 5f74 6162  .        tmp_tab
-000117c0: 6c65 203d 2073 656c 662e 5f69 6269 735f  le = self._ibis_
-000117d0: 746f 5f74 656d 705f 7461 626c 6528 0a20  to_temp_table(. 
-000117e0: 2020 2020 2020 2020 2020 2069 6269 735f             ibis_
-000117f0: 6578 7072 2c20 636c 7573 7465 725f 636f  expr, cluster_co
-00011800: 6c73 3d63 6c75 7374 6572 5f63 6f6c 732c  ls=cluster_cols,
-00011810: 2061 7069 5f6e 616d 653d 2263 6163 6865   api_name="cache
-00011820: 6422 0a20 2020 2020 2020 2029 0a20 2020  d".        ).   
-00011830: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-00011840: 7373 696f 6e20 3d20 7365 6c66 2e69 6269  ssion = self.ibi
-00011850: 735f 636c 6965 6e74 2e74 6162 6c65 280a  s_client.table(.
-00011860: 2020 2020 2020 2020 2020 2020 746d 705f              tmp_
-00011870: 7461 626c 652e 7461 626c 655f 6964 2c0a  table.table_id,.
-00011880: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00011890: 6d61 3d74 6d70 5f74 6162 6c65 2e64 6174  ma=tmp_table.dat
-000118a0: 6173 6574 5f69 642c 0a20 2020 2020 2020  aset_id,.       
-000118b0: 2020 2020 2064 6174 6162 6173 653d 746d       database=tm
-000118c0: 705f 7461 626c 652e 7072 6f6a 6563 742c  p_table.project,
-000118d0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000118e0: 2020 206e 6577 5f63 6f6c 756d 6e73 203d     new_columns =
-000118f0: 205b 7461 626c 655f 6578 7072 6573 7369   [table_expressi
-00011900: 6f6e 5b63 6f6c 756d 6e5d 2066 6f72 2063  on[column] for c
-00011910: 6f6c 756d 6e20 696e 2063 6f6d 7069 6c65  olumn in compile
-00011920: 645f 7661 6c75 652e 636f 6c75 6d6e 5f69  d_value.column_i
-00011930: 6473 5d0a 2020 2020 2020 2020 6e65 775f  ds].        new_
-00011940: 6869 6464 656e 5f63 6f6c 756d 6e73 203d  hidden_columns =
-00011950: 205b 0a20 2020 2020 2020 2020 2020 2074   [.            t
-00011960: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
-00011970: 636f 6c75 6d6e 5d0a 2020 2020 2020 2020  column].        
-00011980: 2020 2020 666f 7220 636f 6c75 6d6e 2069      for column i
-00011990: 6e20 636f 6d70 696c 6564 5f76 616c 7565  n compiled_value
-000119a0: 2e5f 6869 6464 656e 5f6f 7264 6572 696e  ._hidden_orderin
-000119b0: 675f 636f 6c75 6d6e 5f6e 616d 6573 0a20  g_column_names. 
-000119c0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-000119d0: 2023 2054 4f44 4f3a 2049 6e73 7465 6164   # TODO: Instead
-000119e0: 2c20 6b65 6570 2073 6573 7369 6f6e 2d77  , keep session-w
-000119f0: 6964 6520 6d61 7020 6f66 2063 6163 6865  ide map of cache
-00011a00: 6420 7265 7375 6c74 7320 616e 6420 6175  d results and au
-00011a10: 746f 6d61 7469 6361 6c6c 7920 7265 7573  tomatically reus
-00011a20: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00011a30: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
-00011a40: 2e66 726f 6d5f 6962 6973 280a 2020 2020  .from_ibis(.    
-00011a50: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00011a60: 2020 2020 2020 2020 2020 7461 626c 655f            table_
-00011a70: 6578 7072 6573 7369 6f6e 2c0a 2020 2020  expression,.    
-00011a80: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-00011a90: 6e65 775f 636f 6c75 6d6e 732c 0a20 2020  new_columns,.   
-00011aa0: 2020 2020 2020 2020 2068 6964 6465 6e5f           hidden_
-00011ab0: 6f72 6465 7269 6e67 5f63 6f6c 756d 6e73  ordering_columns
-00011ac0: 3d6e 6577 5f68 6964 6465 6e5f 636f 6c75  =new_hidden_colu
-00011ad0: 6d6e 732c 0a20 2020 2020 2020 2020 2020  mns,.           
-00011ae0: 206f 7264 6572 696e 673d 636f 6d70 696c   ordering=compil
-00011af0: 6564 5f76 616c 7565 2e5f 6f72 6465 7269  ed_value._orderi
-00011b00: 6e67 2c0a 2020 2020 2020 2020 290a 0a20  ng,.        ).. 
-00011b10: 2020 2064 6566 205f 6361 6368 655f 7769     def _cache_wi
-00011b20: 7468 5f6f 6666 7365 7473 2873 656c 662c  th_offsets(self,
-00011b30: 2061 7272 6179 5f76 616c 7565 3a20 636f   array_value: co
-00011b40: 7265 2e41 7272 6179 5661 6c75 6529 202d  re.ArrayValue) -
-00011b50: 3e20 636f 7265 2e41 7272 6179 5661 6c75  > core.ArrayValu
-00011b60: 653a 0a20 2020 2020 2020 2022 2222 4578  e:.        """Ex
-00011b70: 6563 7574 6573 2074 6865 2071 7565 7279  ecutes the query
-00011b80: 2061 6e64 2075 7365 7320 7468 6520 7265   and uses the re
-00011b90: 7375 6c74 696e 6720 7461 626c 6520 746f  sulting table to
-00011ba0: 2072 6577 7269 7465 2066 7574 7572 6520   rewrite future 
-00011bb0: 6578 6563 7574 696f 6e73 2e22 2222 0a20  executions.""". 
-00011bc0: 2020 2020 2020 2023 2054 4f44 4f3a 2055         # TODO: U
-00011bd0: 7365 2074 6869 7320 666f 7220 616c 6c20  se this for all 
-00011be0: 6578 6563 7574 696f 6e73 3f20 5072 6f62  executions? Prob
-00011bf0: 6c65 6d20 6973 2074 6861 7420 6361 6368  lem is that cach
-00011c00: 696e 6720 6d61 7465 7269 616c 697a 6573  ing materializes
-00011c10: 2065 7874 7261 0a20 2020 2020 2020 2023   extra.        #
-00011c20: 206f 7264 6572 696e 6720 636f 6c75 6d6e   ordering column
-00011c30: 730a 2020 2020 2020 2020 636f 6d70 696c  s.        compil
-00011c40: 6564 5f76 616c 7565 203d 2073 656c 662e  ed_value = self.
-00011c50: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
-00011c60: 2861 7272 6179 5f76 616c 7565 290a 0a20  (array_value).. 
-00011c70: 2020 2020 2020 2069 6269 735f 6578 7072         ibis_expr
-00011c80: 203d 2063 6f6d 7069 6c65 645f 7661 6c75   = compiled_valu
-00011c90: 652e 5f74 6f5f 6962 6973 5f65 7870 7228  e._to_ibis_expr(
-00011ca0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-00011cb0: 6572 696e 675f 6d6f 6465 3d22 6f66 6673  ering_mode="offs
-00011cc0: 6574 5f63 6f6c 222c 206f 7264 6572 5f63  et_col", order_c
-00011cd0: 6f6c 5f6e 616d 653d 2262 6967 6672 616d  ol_name="bigfram
-00011ce0: 6573 5f6f 6666 7365 7473 220a 2020 2020  es_offsets".    
-00011cf0: 2020 2020 290a 2020 2020 2020 2020 746d      ).        tm
-00011d00: 705f 7461 626c 6520 3d20 7365 6c66 2e5f  p_table = self._
-00011d10: 6962 6973 5f74 6f5f 7465 6d70 5f74 6162  ibis_to_temp_tab
-00011d20: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00011d30: 6962 6973 5f65 7870 722c 2063 6c75 7374  ibis_expr, clust
-00011d40: 6572 5f63 6f6c 733d 5b22 6269 6766 7261  er_cols=["bigfra
-00011d50: 6d65 735f 6f66 6673 6574 7322 5d2c 2061  mes_offsets"], a
-00011d60: 7069 5f6e 616d 653d 2263 6163 6865 6422  pi_name="cached"
-00011d70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00011d80: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
-00011d90: 696f 6e20 3d20 7365 6c66 2e69 6269 735f  ion = self.ibis_
-00011da0: 636c 6965 6e74 2e74 6162 6c65 280a 2020  client.table(.  
-00011db0: 2020 2020 2020 2020 2020 746d 705f 7461            tmp_ta
-00011dc0: 626c 652e 7461 626c 655f 6964 2c0a 2020  ble.table_id,.  
-00011dd0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00011de0: 3d74 6d70 5f74 6162 6c65 2e64 6174 6173  =tmp_table.datas
-00011df0: 6574 5f69 642c 0a20 2020 2020 2020 2020  et_id,.         
-00011e00: 2020 2064 6174 6162 6173 653d 746d 705f     database=tmp_
-00011e10: 7461 626c 652e 7072 6f6a 6563 742c 0a20  table.project,. 
-00011e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00011e30: 206e 6577 5f63 6f6c 756d 6e73 203d 205b   new_columns = [
-00011e40: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00011e50: 5b63 6f6c 756d 6e5d 2066 6f72 2063 6f6c  [column] for col
-00011e60: 756d 6e20 696e 2063 6f6d 7069 6c65 645f  umn in compiled_
-00011e70: 7661 6c75 652e 636f 6c75 6d6e 5f69 6473  value.column_ids
-00011e80: 5d0a 2020 2020 2020 2020 6e65 775f 6869  ].        new_hi
-00011e90: 6464 656e 5f63 6f6c 756d 6e73 203d 205b  dden_columns = [
-00011ea0: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00011eb0: 5b22 6269 6766 7261 6d65 735f 6f66 6673  ["bigframes_offs
-00011ec0: 6574 7322 5d5d 0a20 2020 2020 2020 2023  ets"]].        #
-00011ed0: 2054 4f44 4f3a 2049 6e73 7465 6164 2c20   TODO: Instead, 
-00011ee0: 6b65 6570 2073 6573 7369 6f6e 2d77 6964  keep session-wid
-00011ef0: 6520 6d61 7020 6f66 2063 6163 6865 6420  e map of cached 
-00011f00: 7265 7375 6c74 7320 616e 6420 6175 746f  results and auto
-00011f10: 6d61 7469 6361 6c6c 7920 7265 7573 650a  matically reuse.
-00011f20: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00011f30: 6f72 652e 4172 7261 7956 616c 7565 2e66  ore.ArrayValue.f
-00011f40: 726f 6d5f 6962 6973 280a 2020 2020 2020  rom_ibis(.      
-00011f50: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00011f60: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
-00011f70: 7072 6573 7369 6f6e 2c0a 2020 2020 2020  pression,.      
-00011f80: 2020 2020 2020 636f 6c75 6d6e 733d 6e65        columns=ne
-00011f90: 775f 636f 6c75 6d6e 732c 0a20 2020 2020  w_columns,.     
-00011fa0: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
-00011fb0: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d6e  dering_columns=n
-00011fc0: 6577 5f68 6964 6465 6e5f 636f 6c75 6d6e  ew_hidden_column
-00011fd0: 732c 0a20 2020 2020 2020 2020 2020 206f  s,.            o
-00011fe0: 7264 6572 696e 673d 6f72 6465 722e 4578  rdering=order.Ex
-00011ff0: 7072 6573 7369 6f6e 4f72 6465 7269 6e67  pressionOrdering
-00012000: 2e66 726f 6d5f 6f66 6673 6574 5f63 6f6c  .from_offset_col
-00012010: 2822 6269 6766 7261 6d65 735f 6f66 6673  ("bigframes_offs
-00012020: 6574 7322 292c 0a20 2020 2020 2020 2029  ets"),.        )
-00012030: 0a0a 2020 2020 6465 6620 5f73 696d 706c  ..    def _simpl
-00012040: 6966 795f 7769 7468 5f63 6163 6869 6e67  ify_with_caching
-00012050: 2873 656c 662c 2061 7272 6179 5f76 616c  (self, array_val
-00012060: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
-00012070: 6c75 6529 202d 3e20 636f 7265 2e41 7272  lue) -> core.Arr
-00012080: 6179 5661 6c75 653a 0a20 2020 2020 2020  ayValue:.       
-00012090: 2022 2222 4174 7465 6d70 7473 2074 6f20   """Attempts to 
-000120a0: 6861 6e64 6c65 2074 6865 2063 6f6d 706c  handle the compl
-000120b0: 6578 6974 7920 6279 2063 6163 6869 6e67  exity by caching
-000120c0: 2064 7570 6c69 6361 7465 6420 7375 6274   duplicated subt
-000120d0: 7265 6573 2061 6e64 2062 7265 616b 696e  rees and breakin
-000120e0: 6720 7468 6520 7175 6572 7920 696e 746f  g the query into
-000120f0: 2070 6965 6365 732e 2222 220a 2020 2020   pieces.""".    
-00012100: 2020 2020 6966 206e 6f74 2062 6967 6672      if not bigfr
-00012110: 616d 6573 2e6f 7074 696f 6e73 2e63 6f6d  ames.options.com
-00012120: 7075 7465 2e65 6e61 626c 655f 6d75 6c74  pute.enable_mult
-00012130: 695f 7175 6572 795f 6578 6563 7574 696f  i_query_executio
-00012140: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-00012150: 6574 7572 6e20 6172 7261 795f 7661 6c75  eturn array_valu
-00012160: 650a 2020 2020 2020 2020 6e6f 6465 203d  e.        node =
-00012170: 2061 7272 6179 5f76 616c 7565 2e6e 6f64   array_value.nod
-00012180: 650a 2020 2020 2020 2020 6966 206e 6f64  e.        if nod
-00012190: 652e 706c 616e 6e69 6e67 5f63 6f6d 706c  e.planning_compl
-000121a0: 6578 6974 7920 3c20 5155 4552 595f 434f  exity < QUERY_CO
-000121b0: 4d50 4c45 5849 5459 5f4c 494d 4954 3a0a  MPLEXITY_LIMIT:.
-000121c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000121d0: 726e 2061 7272 6179 5f76 616c 7565 0a0a  rn array_value..
-000121e0: 2020 2020 2020 2020 666f 7220 5f20 696e          for _ in
-000121f0: 2072 616e 6765 284d 4158 5f53 5542 5452   range(MAX_SUBTR
-00012200: 4545 5f46 4143 544f 5249 4e47 5329 3a0a  EE_FACTORINGS):.
-00012210: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-00012220: 7465 6420 3d20 7365 6c66 2e5f 6361 6368  ted = self._cach
-00012230: 655f 6d6f 7374 5f63 6f6d 706c 6578 5f73  e_most_complex_s
-00012240: 7562 7472 6565 286e 6f64 6529 0a20 2020  ubtree(node).   
-00012250: 2020 2020 2020 2020 2069 6620 7570 6461           if upda
-00012260: 7465 6420 6973 204e 6f6e 653a 0a20 2020  ted is None:.   
-00012270: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012280: 7572 6e20 636f 7265 2e41 7272 6179 5661  urn core.ArrayVa
-00012290: 6c75 6528 6e6f 6465 290a 2020 2020 2020  lue(node).      
-000122a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000122b0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-000122c0: 203d 2075 7064 6174 6564 0a0a 2020 2020   = updated..    
-000122d0: 2020 2020 7265 7475 726e 2063 6f72 652e      return core.
-000122e0: 4172 7261 7956 616c 7565 286e 6f64 6529  ArrayValue(node)
-000122f0: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
-00012300: 5f6d 6f73 745f 636f 6d70 6c65 785f 7375  _most_complex_su
-00012310: 6274 7265 6528 0a20 2020 2020 2020 2073  btree(.        s
-00012320: 656c 662c 206e 6f64 653a 206e 6f64 6573  elf, node: nodes
-00012330: 2e42 6967 4672 616d 654e 6f64 650a 2020  .BigFrameNode.  
-00012340: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
-00012350: 6e6f 6465 732e 4269 6746 7261 6d65 4e6f  nodes.BigFrameNo
-00012360: 6465 5d3a 0a20 2020 2020 2020 2023 2054  de]:.        # T
-00012370: 4f44 4f3a 2049 6620 7175 6572 7920 6661  ODO: If query fa
-00012380: 696c 732c 2072 6574 7279 2077 6974 6820  ils, retry with 
-00012390: 6c6f 7765 7220 636f 6d70 6c65 7869 7479  lower complexity
-000123a0: 206c 696d 6974 0a20 2020 2020 2020 2076   limit.        v
-000123b0: 616c 6964 5f63 616e 6469 6461 7465 7320  alid_candidates 
-000123c0: 3d20 7472 6176 6572 7361 6c73 2e63 6f75  = traversals.cou
-000123d0: 6e74 5f63 6f6d 706c 6578 5f6e 6f64 6573  nt_complex_nodes
-000123e0: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
-000123f0: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-00012400: 6d69 6e5f 636f 6d70 6c65 7869 7479 3d28  min_complexity=(
-00012410: 5155 4552 595f 434f 4d50 4c45 5849 5459  QUERY_COMPLEXITY
-00012420: 5f4c 494d 4954 202f 2035 3030 292c 0a20  _LIMIT / 500),. 
-00012430: 2020 2020 2020 2020 2020 206d 6178 5f63             max_c
-00012440: 6f6d 706c 6578 6974 793d 5155 4552 595f  omplexity=QUERY_
-00012450: 434f 4d50 4c45 5849 5459 5f4c 494d 4954  COMPLEXITY_LIMIT
-00012460: 2c0a 2020 2020 2020 2020 292e 6974 656d  ,.        ).item
-00012470: 7328 290a 2020 2020 2020 2020 2320 4865  s().        # He
-00012480: 7572 6973 7469 633a 2073 7562 7472 6565  uristic: subtree
-00012490: 5f63 6f6d 706c 6569 7874 7920 2a20 2863  _compleixty * (c
-000124a0: 6f70 6965 7320 6f66 2073 7562 7472 6565  opies of subtree
-000124b0: 295e 320a 2020 2020 2020 2020 6265 7374  )^2.        best
-000124c0: 5f63 616e 6469 6461 7465 203d 206d 6178  _candidate = max
-000124d0: 280a 2020 2020 2020 2020 2020 2020 7661  (.            va
-000124e0: 6c69 645f 6361 6e64 6964 6174 6573 2c0a  lid_candidates,.
-000124f0: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
-00012500: 6c61 6d62 6461 2069 3a20 695b 305d 2e70  lambda i: i[0].p
-00012510: 6c61 6e6e 696e 675f 636f 6d70 6c65 7869  lanning_complexi
-00012520: 7479 202b 2028 695b 315d 202a 2a20 3229  ty + (i[1] ** 2)
-00012530: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-00012540: 6661 756c 743d 4e6f 6e65 2c0a 2020 2020  fault=None,.    
-00012550: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00012560: 6620 6265 7374 5f63 616e 6469 6461 7465  f best_candidate
-00012570: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00012580: 2020 2020 2020 2320 4e6f 2067 6f6f 6420        # No good 
-00012590: 7375 6274 7265 6573 2074 6f20 6361 6368  subtrees to cach
-000125a0: 652c 206a 7573 7420 7265 7475 726e 206f  e, just return o
-000125b0: 7269 6769 6e61 6c20 7472 6565 0a20 2020  riginal tree.   
-000125c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000125d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
-000125e0: 544f 444f 3a20 4164 6420 636c 7573 7465  TODO: Add cluste
-000125f0: 7269 6e67 2063 6f6c 756d 6e73 2062 6173  ring columns bas
-00012600: 6564 206f 6e20 6163 6365 7373 2070 6174  ed on access pat
-00012610: 7465 726e 730a 2020 2020 2020 2020 6d61  terns.        ma
-00012620: 7465 7269 616c 697a 6564 203d 2073 656c  terialized = sel
-00012630: 662e 5f63 6163 6865 5f77 6974 685f 636c  f._cache_with_cl
-00012640: 7573 7465 725f 636f 6c73 280a 2020 2020  uster_cols(.    
-00012650: 2020 2020 2020 2020 636f 7265 2e41 7272          core.Arr
-00012660: 6179 5661 6c75 6528 6265 7374 5f63 616e  ayValue(best_can
-00012670: 6469 6461 7465 5b30 5d29 2c20 5b5d 0a20  didate[0]), []. 
-00012680: 2020 2020 2020 2029 2e6e 6f64 650a 0a20         ).node.. 
-00012690: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-000126a0: 6176 6572 7361 6c73 2e72 6570 6c61 6365  aversals.replace
-000126b0: 5f6e 6f64 6573 280a 2020 2020 2020 2020  _nodes(.        
-000126c0: 2020 2020 6e6f 6465 2c20 746f 5f72 6570      node, to_rep
-000126d0: 6c61 6365 3d62 6573 745f 6361 6e64 6964  lace=best_candid
-000126e0: 6174 655b 305d 2c20 7265 706c 6163 656d  ate[0], replacem
-000126f0: 656e 6574 3d6d 6174 6572 6961 6c69 7a65  enet=materialize
-00012700: 640a 2020 2020 2020 2020 290a 0a20 2020  d.        )..   
-00012710: 2064 6566 205f 6973 5f74 7269 7669 616c   def _is_trivial
-00012720: 6c79 5f65 7865 6375 7461 626c 6528 7365  ly_executable(se
-00012730: 6c66 2c20 6172 7261 795f 7661 6c75 653a  lf, array_value:
-00012740: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
-00012750: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012760: 2020 2020 2020 2043 616e 2074 6865 2062         Can the b
-00012770: 6c6f 636b 2062 6520 6576 616c 7561 7465  lock be evaluate
-00012780: 6420 7665 7279 2063 6865 6170 6c79 3f0a  d very cheaply?.
-00012790: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-000127a0: 2074 6865 2061 7272 6179 5f76 616c 7565   the array_value
-000127b0: 2070 726f 6261 626c 7920 6973 206e 6f74   probably is not
-000127c0: 2077 6f72 7468 2063 6163 6869 6e67 2e0a   worth caching..
-000127d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000127e0: 2020 2020 2320 4f6e 6365 2072 6577 7269      # Once rewri
-000127f0: 7469 6e67 2069 7320 6176 6169 6c61 626c  ting is availabl
-00012800: 652c 2077 696c 6c20 7761 6e74 2074 6f20  e, will want to 
-00012810: 7265 7772 6974 6520 6265 666f 7265 0a20  rewrite before. 
-00012820: 2020 2020 2020 2023 2065 7661 6c75 6174         # evaluat
-00012830: 696e 6720 6578 6563 7574 696f 6e20 636f  ing execution co
-00012840: 7374 2e0a 2020 2020 2020 2020 7265 7475  st..        retu
-00012850: 726e 2074 7261 7665 7273 616c 732e 6973  rn traversals.is
-00012860: 5f74 7269 7669 616c 6c79 5f65 7865 6375  _trivially_execu
-00012870: 7461 626c 6528 6172 7261 795f 7661 6c75  table(array_valu
-00012880: 652e 6e6f 6465 290a 0a20 2020 2064 6566  e.node)..    def
-00012890: 205f 6578 6563 7574 6528 0a20 2020 2020   _execute(.     
-000128a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000128b0: 2061 7272 6179 5f76 616c 7565 3a20 636f   array_value: co
-000128c0: 7265 2e41 7272 6179 5661 6c75 652c 0a20  re.ArrayValue,. 
-000128d0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-000128e0: 673a 204f 7074 696f 6e61 6c5b 6269 6771  g: Optional[bigq
-000128f0: 7565 7279 2e6a 6f62 2e51 7565 7279 4a6f  uery.job.QueryJo
-00012900: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
-00012910: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00012920: 2020 2020 736f 7274 6564 3a20 626f 6f6c      sorted: bool
-00012930: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-00012940: 2064 7279 5f72 756e 3d46 616c 7365 2c0a   dry_run=False,.
-00012950: 2020 2020 2020 2020 636f 6c5f 6964 5f6f          col_id_o
-00012960: 7665 7272 6964 6573 3a20 4d61 7070 696e  verrides: Mappin
-00012970: 675b 7374 722c 2073 7472 5d20 3d20 7b7d  g[str, str] = {}
-00012980: 2c0a 2020 2020 2920 2d3e 2074 7570 6c65  ,.    ) -> tuple
-00012990: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
-000129a0: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
-000129b0: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
-000129c0: 0a20 2020 2020 2020 2073 716c 203d 2073  .        sql = s
-000129d0: 656c 662e 5f74 6f5f 7371 6c28 0a20 2020  elf._to_sql(.   
-000129e0: 2020 2020 2020 2020 2061 7272 6179 5f76           array_v
-000129f0: 616c 7565 2c20 736f 7274 6564 3d73 6f72  alue, sorted=sor
-00012a00: 7465 642c 2063 6f6c 5f69 645f 6f76 6572  ted, col_id_over
-00012a10: 7269 6465 733d 636f 6c5f 6964 5f6f 7665  rides=col_id_ove
-00012a20: 7272 6964 6573 0a20 2020 2020 2020 2029  rrides.        )
-00012a30: 2020 2320 7479 7065 3a69 676e 6f72 650a    # type:ignore.
-00012a40: 2020 2020 2020 2020 6966 206a 6f62 5f63          if job_c
-00012a50: 6f6e 6669 6720 6973 204e 6f6e 653a 0a20  onfig is None:. 
-00012a60: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-00012a70: 6f6e 6669 6720 3d20 6269 6771 7565 7279  onfig = bigquery
-00012a80: 2e51 7565 7279 4a6f 6243 6f6e 6669 6728  .QueryJobConfig(
-00012a90: 6472 795f 7275 6e3d 6472 795f 7275 6e29  dry_run=dry_run)
-00012aa0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00012ab0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-00012ac0: 6f6e 6669 672e 6472 795f 7275 6e20 3d20  onfig.dry_run = 
-00012ad0: 6472 795f 7275 6e0a 2020 2020 2020 2020  dry_run.        
-00012ae0: 7265 7475 726e 2073 656c 662e 5f73 7461  return self._sta
-00012af0: 7274 5f71 7565 7279 280a 2020 2020 2020  rt_query(.      
-00012b00: 2020 2020 2020 7371 6c3d 7371 6c2c 0a20        sql=sql,. 
-00012b10: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-00012b20: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
-00012b30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00012b40: 2064 6566 205f 7065 656b 280a 2020 2020   def _peek(.    
-00012b50: 2020 2020 7365 6c66 2c20 6172 7261 795f      self, array_
-00012b60: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
-00012b70: 7956 616c 7565 2c20 6e5f 726f 7773 3a20  yValue, n_rows: 
-00012b80: 696e 740a 2020 2020 2920 2d3e 2074 7570  int.    ) -> tup
-00012b90: 6c65 5b62 6967 7175 6572 792e 7461 626c  le[bigquery.tabl
-00012ba0: 652e 526f 7749 7465 7261 746f 722c 2062  e.RowIterator, b
-00012bb0: 6967 7175 6572 792e 5175 6572 794a 6f62  igquery.QueryJob
-00012bc0: 5d3a 0a20 2020 2020 2020 2022 2222 4120  ]:.        """A 
-00012bd0: 2770 6565 6b27 2065 6666 6963 6965 6e74  'peek' efficient
-00012be0: 6c79 2061 6363 6573 7365 7320 6120 736d  ly accesses a sm
-00012bf0: 616c 6c20 6e75 6d62 6572 206f 6620 726f  all number of ro
-00012c00: 7773 2069 6e20 7468 6520 6461 7461 6672  ws in the datafr
-00012c10: 616d 652e 2222 220a 2020 2020 2020 2020  ame.""".        
-00012c20: 6966 206e 6f74 2074 7265 655f 7072 6f70  if not tree_prop
-00012c30: 6572 7469 6573 2e70 6565 6b61 626c 6528  erties.peekable(
-00012c40: 6172 7261 795f 7661 6c75 652e 6e6f 6465  array_value.node
-00012c50: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-00012c60: 6172 6e69 6e67 732e 7761 726e 2822 5065  arnings.warn("Pe
-00012c70: 656b 696e 6720 7468 6973 2076 616c 7565  eking this value
-00012c80: 2063 616e 6e6f 7420 6265 2064 6f6e 6520   cannot be done 
-00012c90: 6566 6669 6369 656e 746c 792e 2229 0a20  efficiently."). 
-00012ca0: 2020 2020 2020 2073 716c 203d 2073 656c         sql = sel
-00012cb0: 662e 5f63 6f6d 7069 6c65 5f75 6e6f 7264  f._compile_unord
-00012cc0: 6572 6564 2861 7272 6179 5f76 616c 7565  ered(array_value
-00012cd0: 292e 7065 656b 5f73 716c 286e 5f72 6f77  ).peek_sql(n_row
-00012ce0: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
-00012cf0: 6e20 7365 6c66 2e5f 7374 6172 745f 7175  n self._start_qu
-00012d00: 6572 7928 0a20 2020 2020 2020 2020 2020  ery(.           
-00012d10: 2073 716c 3d73 716c 2c0a 2020 2020 2020   sql=sql,.      
-00012d20: 2020 290a 0a20 2020 2064 6566 205f 746f    )..    def _to
-00012d30: 5f73 716c 280a 2020 2020 2020 2020 7365  _sql(.        se
-00012d40: 6c66 2c0a 2020 2020 2020 2020 6172 7261  lf,.        arra
-00012d50: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
-00012d60: 7261 7956 616c 7565 2c0a 2020 2020 2020  rayValue,.      
-00012d70: 2020 6f66 6673 6574 5f63 6f6c 756d 6e3a    offset_column:
-00012d80: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00012d90: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00012da0: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
-00012db0: 7272 6964 6573 3a20 7479 7069 6e67 2e4d  rrides: typing.M
-00012dc0: 6170 7069 6e67 5b73 7472 2c20 7374 725d  apping[str, str]
-00012dd0: 203d 207b 7d2c 0a20 2020 2020 2020 2073   = {},.        s
-00012de0: 6f72 7465 643a 2062 6f6f 6c20 3d20 4661  orted: bool = Fa
-00012df0: 6c73 652c 0a20 2020 2029 202d 3e20 7374  lse,.    ) -> st
-00012e00: 723a 0a20 2020 2020 2020 2069 6620 6f66  r:.        if of
-00012e10: 6673 6574 5f63 6f6c 756d 6e3a 0a20 2020  fset_column:.   
-00012e20: 2020 2020 2020 2020 2061 7272 6179 5f76           array_v
-00012e30: 616c 7565 203d 2061 7272 6179 5f76 616c  alue = array_val
-00012e40: 7565 2e70 726f 6d6f 7465 5f6f 6666 7365  ue.promote_offse
-00012e50: 7473 286f 6666 7365 745f 636f 6c75 6d6e  ts(offset_column
-00012e60: 290a 2020 2020 2020 2020 6966 2073 6f72  ).        if sor
-00012e70: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-00012e80: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-00012e90: 6d70 696c 655f 6f72 6465 7265 6428 6172  mpile_ordered(ar
-00012ea0: 7261 795f 7661 6c75 6529 2e74 6f5f 7371  ray_value).to_sq
-00012eb0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00012ec0: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
-00012ed0: 6465 733d 636f 6c5f 6964 5f6f 7665 7272  des=col_id_overr
-00012ee0: 6964 6573 2c20 736f 7274 6564 3d54 7275  ides, sorted=Tru
-00012ef0: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-00012f00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00012f10: 656c 662e 5f63 6f6d 7069 6c65 5f75 6e6f  elf._compile_uno
-00012f20: 7264 6572 6564 2861 7272 6179 5f76 616c  rdered(array_val
-00012f30: 7565 292e 746f 5f73 716c 280a 2020 2020  ue).to_sql(.    
-00012f40: 2020 2020 2020 2020 636f 6c5f 6964 5f6f          col_id_o
-00012f50: 7665 7272 6964 6573 3d63 6f6c 5f69 645f  verrides=col_id_
-00012f60: 6f76 6572 7269 6465 730a 2020 2020 2020  overrides.      
-00012f70: 2020 290a 0a20 2020 2064 6566 205f 636f    )..    def _co
-00012f80: 6d70 696c 655f 6f72 6465 7265 6428 0a20  mpile_ordered(. 
-00012f90: 2020 2020 2020 2073 656c 662c 2061 7272         self, arr
-00012fa0: 6179 5f76 616c 7565 3a20 636f 7265 2e41  ay_value: core.A
-00012fb0: 7272 6179 5661 6c75 650a 2020 2020 2920  rrayValue.    ) 
-00012fc0: 2d3e 2062 6967 6672 616d 6573 2e63 6f72  -> bigframes.cor
-00012fd0: 652e 636f 6d70 696c 652e 4f72 6465 7265  e.compile.Ordere
-00012fe0: 6449 523a 0a20 2020 2020 2020 2072 6574  dIR:.        ret
-00012ff0: 7572 6e20 6269 6766 7261 6d65 732e 636f  urn bigframes.co
-00013000: 7265 2e63 6f6d 7069 6c65 2e63 6f6d 7069  re.compile.compi
-00013010: 6c65 5f6f 7264 6572 6564 5f69 7228 6172  le_ordered_ir(ar
-00013020: 7261 795f 7661 6c75 652e 6e6f 6465 290a  ray_value.node).
-00013030: 0a20 2020 2064 6566 205f 636f 6d70 696c  .    def _compil
-00013040: 655f 756e 6f72 6465 7265 6428 0a20 2020  e_unordered(.   
-00013050: 2020 2020 2073 656c 662c 2061 7272 6179       self, array
-00013060: 5f76 616c 7565 3a20 636f 7265 2e41 7272  _value: core.Arr
-00013070: 6179 5661 6c75 650a 2020 2020 2920 2d3e  ayValue.    ) ->
-00013080: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
-00013090: 636f 6d70 696c 652e 556e 6f72 6465 7265  compile.Unordere
-000130a0: 6449 523a 0a20 2020 2020 2020 2072 6574  dIR:.        ret
-000130b0: 7572 6e20 6269 6766 7261 6d65 732e 636f  urn bigframes.co
-000130c0: 7265 2e63 6f6d 7069 6c65 2e63 6f6d 7069  re.compile.compi
-000130d0: 6c65 5f75 6e6f 7264 6572 6564 5f69 7228  le_unordered_ir(
-000130e0: 6172 7261 795f 7661 6c75 652e 6e6f 6465  array_value.node
-000130f0: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-00013100: 7461 626c 655f 7369 7a65 2873 656c 662c  table_size(self,
-00013110: 2064 6573 7469 6e61 7469 6f6e 5f74 6162   destination_tab
-00013120: 6c65 293a 0a20 2020 2020 2020 2074 6162  le):.        tab
-00013130: 6c65 203d 2073 656c 662e 6271 636c 6965  le = self.bqclie
-00013140: 6e74 2e67 6574 5f74 6162 6c65 2864 6573  nt.get_table(des
-00013150: 7469 6e61 7469 6f6e 5f74 6162 6c65 290a  tination_table).
-00013160: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00013170: 6162 6c65 2e6e 756d 5f62 7974 6573 0a0a  able.num_bytes..
-00013180: 2020 2020 6465 6620 5f72 6f77 735f 746f      def _rows_to
-00013190: 5f64 6174 6166 7261 6d65 280a 2020 2020  _dataframe(.    
-000131a0: 2020 2020 7365 6c66 2c20 726f 775f 6974      self, row_it
-000131b0: 6572 6174 6f72 3a20 6269 6771 7565 7279  erator: bigquery
-000131c0: 2e74 6162 6c65 2e52 6f77 4974 6572 6174  .table.RowIterat
-000131d0: 6f72 2c20 6474 7970 6573 3a20 4469 6374  or, dtypes: Dict
-000131e0: 0a20 2020 2029 202d 3e20 7061 6e64 6173  .    ) -> pandas
-000131f0: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
-00013200: 2020 2020 2320 4361 6e20 6967 6e6f 7265      # Can ignore
-00013210: 2069 6e66 6572 7265 6420 6461 7461 7479   inferred dataty
-00013220: 7065 2075 6e74 696c 2064 7479 7065 2065  pe until dtype e
-00013230: 6d75 6c61 7469 6f6e 2062 7265 616b 7320  mulation breaks 
-00013240: 313a 3120 6d61 7070 696e 6720 6265 7477  1:1 mapping betw
-00013250: 6565 6e20 4251 2074 7970 6573 2061 6e64  een BQ types and
-00013260: 2062 6967 6672 616d 6573 2074 7970 6573   bigframes types
-00013270: 0a20 2020 2020 2020 2064 7479 7065 735f  .        dtypes_
-00013280: 6672 6f6d 5f62 7120 3d20 6269 6766 7261  from_bq = bigfra
-00013290: 6d65 732e 6474 7970 6573 2e62 665f 7479  mes.dtypes.bf_ty
-000132a0: 7065 5f66 726f 6d5f 7479 7065 5f6b 696e  pe_from_type_kin
-000132b0: 6428 726f 775f 6974 6572 6174 6f72 2e73  d(row_iterator.s
-000132c0: 6368 656d 6129 0a20 2020 2020 2020 2061  chema).        a
-000132d0: 7272 6f77 5f74 6162 6c65 203d 2072 6f77  rrow_table = row
-000132e0: 5f69 7465 7261 746f 722e 746f 5f61 7272  _iterator.to_arr
-000132f0: 6f77 2829 0a20 2020 2020 2020 2072 6574  ow().        ret
-00013300: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
-00013310: 7373 696f 6e2e 5f69 6f2e 7061 6e64 6173  ssion._io.pandas
-00013320: 2e61 7272 6f77 5f74 6f5f 7061 6e64 6173  .arrow_to_pandas
-00013330: 2861 7272 6f77 5f74 6162 6c65 2c20 6474  (arrow_table, dt
-00013340: 7970 6573 5f66 726f 6d5f 6271 290a 0a20  ypes_from_bq).. 
-00013350: 2020 2064 6566 205f 7374 6172 745f 6765     def _start_ge
-00013360: 6e65 7269 635f 6a6f 6228 7365 6c66 2c20  neric_job(self, 
-00013370: 6a6f 623a 2066 6f72 6d61 7474 696e 675f  job: formatting_
-00013380: 6865 6c70 6572 732e 4765 6e65 7269 634a  helpers.GenericJ
-00013390: 6f62 293a 0a20 2020 2020 2020 2069 6620  ob):.        if 
-000133a0: 6269 6766 7261 6d65 732e 6f70 7469 6f6e  bigframes.option
-000133b0: 732e 6469 7370 6c61 792e 7072 6f67 7265  s.display.progre
-000133c0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-000133d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000133e0: 666f 726d 6174 7469 6e67 5f68 656c 7065  formatting_helpe
-000133f0: 7273 2e77 6169 745f 666f 725f 6a6f 6228  rs.wait_for_job(
-00013400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013410: 206a 6f62 2c20 6269 6766 7261 6d65 732e   job, bigframes.
-00013420: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
-00013430: 7072 6f67 7265 7373 5f62 6172 0a20 2020  progress_bar.   
-00013440: 2020 2020 2020 2020 2029 2020 2320 5761           )  # Wa
-00013450: 6974 2066 6f72 2074 6865 206a 6f62 2074  it for the job t
-00013460: 6f20 636f 6d70 6c65 7465 0a20 2020 2020  o complete.     
-00013470: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013480: 2020 2020 206a 6f62 2e72 6573 756c 7428       job.result(
-00013490: 290a 0a0a 6465 6620 636f 6e6e 6563 7428  )...def connect(
-000134a0: 636f 6e74 6578 743a 204f 7074 696f 6e61  context: Optiona
-000134b0: 6c5b 6269 6771 7565 7279 5f6f 7074 696f  l[bigquery_optio
-000134c0: 6e73 2e42 6967 5175 6572 794f 7074 696f  ns.BigQueryOptio
-000134d0: 6e73 5d20 3d20 4e6f 6e65 2920 2d3e 2053  ns] = None) -> S
-000134e0: 6573 7369 6f6e 3a0a 2020 2020 7265 7475  ession:.    retu
-000134f0: 726e 2053 6573 7369 6f6e 2863 6f6e 7465  rn Session(conte
-00013500: 7874 290a 0a0a 6465 6620 5f63 616e 5f63  xt)...def _can_c
-00013510: 6c75 7374 6572 5f62 7128 6669 656c 643a  luster_bq(field:
-00013520: 2062 6967 7175 6572 792e 5363 6865 6d61   bigquery.Schema
-00013530: 4669 656c 6429 3a0a 2020 2020 2320 6874  Field):.    # ht
-00013540: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-00013550: 6c65 2e63 6f6d 2f62 6967 7175 6572 792f  le.com/bigquery/
-00013560: 646f 6373 2f63 6c75 7374 6572 6564 2d74  docs/clustered-t
-00013570: 6162 6c65 730a 2020 2020 2320 4e6f 7461  ables.    # Nota
-00013580: 626c 792c 2066 6c6f 6174 2069 7320 6578  bly, float is ex
-00013590: 636c 7564 6564 0a20 2020 2074 7970 655f  cluded.    type_
-000135a0: 203d 2066 6965 6c64 2e66 6965 6c64 5f74   = field.field_t
-000135b0: 7970 650a 2020 2020 7265 7475 726e 2074  ype.    return t
-000135c0: 7970 655f 2069 6e20 280a 2020 2020 2020  ype_ in (.      
-000135d0: 2020 2249 4e54 4547 4552 222c 0a20 2020    "INTEGER",.   
-000135e0: 2020 2020 2022 494e 5436 3422 2c0a 2020       "INT64",.  
-000135f0: 2020 2020 2020 2253 5452 494e 4722 2c0a        "STRING",.
-00013600: 2020 2020 2020 2020 224e 554d 4552 4943          "NUMERIC
-00013610: 222c 0a20 2020 2020 2020 2022 4445 4349  ",.        "DECI
-00013620: 4d41 4c22 2c0a 2020 2020 2020 2020 2242  MAL",.        "B
-00013630: 4947 4e55 4d45 5249 4322 2c0a 2020 2020  IGNUMERIC",.    
-00013640: 2020 2020 2242 4947 4445 4349 4d41 4c22      "BIGDECIMAL"
-00013650: 2c0a 2020 2020 2020 2020 2244 4154 4522  ,.        "DATE"
-00013660: 2c0a 2020 2020 2020 2020 2244 4154 4554  ,.        "DATET
-00013670: 494d 4522 2c0a 2020 2020 2020 2020 2254  IME",.        "T
-00013680: 494d 4553 5441 4d50 222c 0a20 2020 2020  IMESTAMP",.     
-00013690: 2020 2022 424f 4f4c 222c 0a20 2020 2020     "BOOL",.     
-000136a0: 2020 2022 424f 4f4c 4541 4e22 2c0a 2020     "BOOLEAN",.  
-000136b0: 2020 290a 0a0a 6465 6620 5f63 6f6e 7665    )...def _conve
-000136c0: 7274 5f74 6f5f 6e6f 6e6e 756c 6c5f 7374  rt_to_nonnull_st
-000136d0: 7269 6e67 2863 6f6c 756d 6e3a 2069 6269  ring(column: ibi
-000136e0: 735f 7479 7065 732e 436f 6c75 6d6e 2920  s_types.Column) 
-000136f0: 2d3e 2069 6269 735f 7479 7065 732e 5374  -> ibis_types.St
-00013700: 7269 6e67 5661 6c75 653a 0a20 2020 2063  ringValue:.    c
-00013710: 6f6c 5f74 7970 6520 3d20 636f 6c75 6d6e  ol_type = column
-00013720: 2e74 7970 6528 290a 2020 2020 6966 2028  .type().    if (
-00013730: 0a20 2020 2020 2020 2063 6f6c 5f74 7970  .        col_typ
-00013740: 652e 6973 5f6e 756d 6572 6963 2829 0a20  e.is_numeric(). 
-00013750: 2020 2020 2020 206f 7220 636f 6c5f 7479         or col_ty
-00013760: 7065 2e69 735f 626f 6f6c 6561 6e28 290a  pe.is_boolean().
-00013770: 2020 2020 2020 2020 6f72 2063 6f6c 5f74          or col_t
-00013780: 7970 652e 6973 5f62 696e 6172 7928 290a  ype.is_binary().
-00013790: 2020 2020 2020 2020 6f72 2063 6f6c 5f74          or col_t
-000137a0: 7970 652e 6973 5f74 656d 706f 7261 6c28  ype.is_temporal(
-000137b0: 290a 2020 2020 293a 0a20 2020 2020 2020  ).    ):.       
-000137c0: 2072 6573 756c 7420 3d20 636f 6c75 6d6e   result = column
-000137d0: 2e63 6173 7428 6962 6973 5f64 7479 7065  .cast(ibis_dtype
-000137e0: 732e 5374 7269 6e67 286e 756c 6c61 626c  s.String(nullabl
-000137f0: 653d 5472 7565 2929 0a20 2020 2065 6c69  e=True)).    eli
-00013800: 6620 636f 6c5f 7479 7065 2e69 735f 6765  f col_type.is_ge
-00013810: 6f73 7061 7469 616c 2829 3a0a 2020 2020  ospatial():.    
-00013820: 2020 2020 7265 7375 6c74 203d 2074 7970      result = typ
-00013830: 696e 672e 6361 7374 2869 6269 735f 7479  ing.cast(ibis_ty
-00013840: 7065 732e 4765 6f53 7061 7469 616c 436f  pes.GeoSpatialCo
-00013850: 6c75 6d6e 2c20 636f 6c75 6d6e 292e 6173  lumn, column).as
-00013860: 5f74 6578 7428 290a 2020 2020 656c 6966  _text().    elif
-00013870: 2063 6f6c 5f74 7970 652e 6973 5f73 7472   col_type.is_str
-00013880: 696e 6728 293a 0a20 2020 2020 2020 2072  ing():.        r
-00013890: 6573 756c 7420 3d20 636f 6c75 6d6e 0a20  esult = column. 
-000138a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000138b0: 2023 2054 4f5f 4a53 4f4e 5f53 5452 494e   # TO_JSON_STRIN
-000138c0: 4720 776f 726b 7320 7769 7468 2061 6c6c  G works with all
-000138d0: 2064 6174 6120 7479 7065 732c 2062 7574   data types, but
-000138e0: 2069 736e 2774 2074 6865 206d 6f73 7420   isn't the most 
-000138f0: 6566 6669 6369 656e 740a 2020 2020 2020  efficient.      
-00013900: 2020 2320 4e65 6564 6564 2066 6f72 204a    # Needed for J
-00013910: 534f 4e2c 2053 5452 5543 5420 616e 6420  SON, STRUCT and 
-00013920: 4152 5241 5920 6461 7461 7479 7065 730a  ARRAY datatypes.
-00013930: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00013940: 2076 656e 646f 7265 645f 6962 6973 5f6f   vendored_ibis_o
-00013950: 7073 2e54 6f4a 736f 6e53 7472 696e 6728  ps.ToJsonString(
-00013960: 636f 6c75 6d6e 292e 746f 5f65 7870 7228  column).to_expr(
-00013970: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
-00013980: 650a 2020 2020 2320 4573 6361 7065 2062  e.    # Escape b
-00013990: 6163 6b73 6c61 7368 6573 2061 6e64 2075  ackslashes and u
-000139a0: 7365 2062 6163 6b73 6c61 7368 2061 7320  se backslash as 
-000139b0: 6465 6c69 6e65 6174 6f72 0a20 2020 2065  delineator.    e
-000139c0: 7363 6170 6564 203d 2074 7970 696e 672e  scaped = typing.
-000139d0: 6361 7374 2869 6269 735f 7479 7065 732e  cast(ibis_types.
-000139e0: 5374 7269 6e67 436f 6c75 6d6e 2c20 7265  StringColumn, re
-000139f0: 7375 6c74 2e66 696c 6c6e 6128 2222 2929  sult.fillna(""))
-00013a00: 2e72 6570 6c61 6365 2822 5c5c 222c 2022  .replace("\\", "
-00013a10: 5c5c 5c5c 2229 2020 2320 7479 7065 3a20  \\\\")  # type: 
-00013a20: 6967 6e6f 7265 0a20 2020 2072 6574 7572  ignore.    retur
-00013a30: 6e20 7479 7069 6e67 2e63 6173 7428 6962  n typing.cast(ib
-00013a40: 6973 5f74 7970 6573 2e53 7472 696e 6743  is_types.StringC
-00013a50: 6f6c 756d 6e2c 2069 6269 732e 6c69 7465  olumn, ibis.lite
-00013a60: 7261 6c28 225c 5c22 2929 2e63 6f6e 6361  ral("\\")).conca
-00013a70: 7428 6573 6361 7065 6429 0a0a 0a64 6566  t(escaped)...def
-00013a80: 205f 7472 616e 7366 6f72 6d5f 7265 6164   _transform_read
-00013a90: 5f67 6271 5f63 6f6e 6669 6775 7261 7469  _gbq_configurati
-00013aa0: 6f6e 2863 6f6e 6669 6775 7261 7469 6f6e  on(configuration
-00013ab0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-00013ac0: 2920 2d3e 2064 6963 743a 0a20 2020 2022  ) -> dict:.    "
-00013ad0: 2222 0a20 2020 2046 6f72 2062 6163 6b77  "".    For backw
-00013ae0: 6172 6473 2d63 6f6d 7061 7469 6269 6c69  ards-compatibili
-00013af0: 7479 2c20 636f 6e76 6572 7420 616e 7920  ty, convert any 
-00013b00: 7072 6576 696f 7573 6c79 2063 6c69 656e  previously clien
-00013b10: 742d 7369 6465 206f 6e6c 790a 2020 2020  t-side only.    
-00013b20: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
-00013b30: 6173 2074 696d 656f 7574 4d73 2074 6f20  as timeoutMs to 
-00013b40: 7468 6520 7072 6f70 6572 7479 206e 616d  the property nam
-00013b50: 6520 6578 7065 6374 6564 2062 7920 7468  e expected by th
-00013b60: 6520 5245 5354 2041 5049 2e0a 0a20 2020  e REST API...   
-00013b70: 204d 616b 6573 2061 2063 6f70 7920 6f66   Makes a copy of
-00013b80: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
-00013b90: 6620 6368 616e 6765 7320 6172 6520 6e65  f changes are ne
-00013ba0: 6564 6564 2e0a 2020 2020 2222 220a 0a20  eded..    """.. 
-00013bb0: 2020 2069 6620 636f 6e66 6967 7572 6174     if configurat
-00013bc0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00013bd0: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
-00013be0: 2020 2020 7469 6d65 6f75 745f 6d73 203d      timeout_ms =
-00013bf0: 2063 6f6e 6669 6775 7261 7469 6f6e 2e67   configuration.g
-00013c00: 6574 2822 7175 6572 7922 2c20 7b7d 292e  et("query", {}).
-00013c10: 6765 7428 2274 696d 656f 7574 4d73 2229  get("timeoutMs")
-00013c20: 0a20 2020 2069 6620 7469 6d65 6f75 745f  .    if timeout_
-00013c30: 6d73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ms is not None:.
-00013c40: 2020 2020 2020 2020 2320 5472 616e 7366          # Transf
-00013c50: 6f72 6d20 7469 6d65 6f75 744d 7320 746f  orm timeoutMs to
-00013c60: 2061 6e20 6163 7475 616c 2073 6572 7665   an actual serve
-00013c70: 722d 7369 6465 2063 6f6e 6669 6775 7261  r-side configura
-00013c80: 7469 6f6e 2e0a 2020 2020 2020 2020 2320  tion..        # 
-00013c90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00013ca0: 6f6d 2f67 6f6f 676c 6561 7069 732f 7079  om/googleapis/py
-00013cb0: 7468 6f6e 2d62 6967 7175 6572 792d 7061  thon-bigquery-pa
-00013cc0: 6e64 6173 2f69 7373 7565 732f 3437 390a  ndas/issues/479.
-00013cd0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00013ce0: 6174 696f 6e20 3d20 636f 7079 2e64 6565  ation = copy.dee
-00013cf0: 7063 6f70 7928 636f 6e66 6967 7572 6174  pcopy(configurat
-00013d00: 696f 6e29 0a20 2020 2020 2020 2064 656c  ion).        del
-00013d10: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
-00013d20: 7175 6572 7922 5d5b 2274 696d 656f 7574  query"]["timeout
-00013d30: 4d73 225d 0a20 2020 2020 2020 2063 6f6e  Ms"].        con
-00013d40: 6669 6775 7261 7469 6f6e 5b22 6a6f 6254  figuration["jobT
-00013d50: 696d 656f 7574 4d73 225d 203d 2074 696d  imeoutMs"] = tim
-00013d60: 656f 7574 5f6d 730a 0a20 2020 2072 6574  eout_ms..    ret
-00013d70: 7572 6e20 636f 6e66 6967 7572 6174 696f  urn configuratio
-00013d80: 6e0a                                     n.
+0000ce20: 672e 6175 746f 6465 7465 6374 203d 2054  g.autodetect = T
+0000ce30: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000ce40: 6a6f 625f 636f 6e66 6967 2e65 6e63 6f64  job_config.encod
+0000ce50: 696e 6720 3d20 656e 636f 6469 6e67 0a20  ing = encoding. 
+0000ce60: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000ce70: 6f6e 6669 672e 6c61 6265 6c73 203d 207b  onfig.labels = {
+0000ce80: 2262 6967 6672 616d 6573 2d61 7069 223a  "bigframes-api":
+0000ce90: 2022 7265 6164 5f6a 736f 6e22 7d0a 0a20   "read_json"}.. 
+0000cea0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ceb0: 6e20 7365 6c66 2e5f 7265 6164 5f62 6967  n self._read_big
+0000cec0: 7175 6572 795f 6c6f 6164 5f6a 6f62 280a  query_load_job(.
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
+0000cef0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+0000cf00: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+0000cf10: 2020 2020 6a6f 625f 636f 6e66 6967 3d6a      job_config=j
+0000cf20: 6f62 5f63 6f6e 6669 672c 0a20 2020 2020  ob_config,.     
+0000cf30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000cf40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000cf50: 2020 2069 6620 616e 7928 6172 6720 696e     if any(arg in
+0000cf60: 206b 7761 7267 7320 666f 7220 6172 6720   kwargs for arg 
+0000cf70: 696e 2028 2263 6875 6e6b 7369 7a65 222c  in ("chunksize",
+0000cf80: 2022 6974 6572 6174 6f72 2229 293a 0a20   "iterator")):. 
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000cfa0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+0000cfb0: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2227                "'
+0000cfd0: 6368 756e 6b73 697a 6527 2061 6e64 2027  chunksize' and '
+0000cfe0: 6974 6572 6174 6f72 2720 6172 6775 6d65  iterator' argume
+0000cff0: 6e74 7320 6172 6520 6e6f 7420 7375 7070  nts are not supp
+0000d000: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
+0000d010: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000d020: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000d030: 616e 6365 2870 6174 685f 6f72 5f62 7566  ance(path_or_buf
+0000d040: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000d050: 2020 2020 2020 2020 7365 6c66 2e5f 6368          self._ch
+0000d060: 6563 6b5f 6669 6c65 5f73 697a 6528 7061  eck_file_size(pa
+0000d070: 7468 5f6f 725f 6275 6629 0a0a 2020 2020  th_or_buf)..    
+0000d080: 2020 2020 2020 2020 6966 2065 6e67 696e          if engin
+0000d090: 6520 3d3d 2022 756a 736f 6e22 3a0a 2020  e == "ujson":.  
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000d0b0: 6e64 6173 5f64 6620 3d20 7061 6e64 6173  ndas_df = pandas
+0000d0c0: 2e72 6561 645f 6a73 6f6e 2820 2023 2074  .read_json(  # t
+0000d0d0: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 206f 7269 656e 743d 6f72 6965 6e74 2c0a   orient=orient,.
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
+0000d140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d150: 2020 2020 2065 6e63 6f64 696e 673d 656e       encoding=en
+0000d160: 636f 6469 6e67 2c0a 2020 2020 2020 2020  coding,.        
+0000d170: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000d180: 733d 6c69 6e65 732c 0a20 2020 2020 2020  s=lines,.       
+0000d190: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+0000d1a0: 7761 7267 732c 0a20 2020 2020 2020 2020  wargs,.         
+0000d1b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000d1c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d1d0: 2020 2020 2020 2020 2020 2020 7061 6e64              pand
+0000d1e0: 6173 5f64 6620 3d20 7061 6e64 6173 2e72  as_df = pandas.r
+0000d1f0: 6561 645f 6a73 6f6e 2820 2023 2074 7970  ead_json(  # typ
+0000d200: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
+0000d210: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000d220: 7468 5f6f 725f 6275 662c 0a20 2020 2020  th_or_buf,.     
+0000d230: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000d240: 7269 656e 743d 6f72 6965 6e74 2c0a 2020  rient=orient,.  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 6474 7970 653d 6474 7970 652c 0a20    dtype=dtype,. 
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2065 6e63 6f64 696e 673d 656e 636f     encoding=enco
+0000d290: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
+0000d2a0: 2020 2020 2020 2020 2020 6c69 6e65 733d            lines=
+0000d2b0: 6c69 6e65 732c 0a20 2020 2020 2020 2020  lines,.         
+0000d2c0: 2020 2020 2020 2020 2020 2065 6e67 696e             engin
+0000d2d0: 653d 656e 6769 6e65 2c0a 2020 2020 2020  e=engine,.      
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+0000d2f0: 6b77 6172 6773 2c0a 2020 2020 2020 2020  kwargs,.        
+0000d300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d310: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000d320: 662e 5f72 6561 645f 7061 6e64 6173 2870  f._read_pandas(p
+0000d330: 616e 6461 735f 6466 2c20 2272 6561 645f  andas_df, "read_
+0000d340: 6a73 6f6e 2229 0a0a 2020 2020 6465 6620  json")..    def 
+0000d350: 5f63 6865 636b 5f66 696c 655f 7369 7a65  _check_file_size
+0000d360: 2873 656c 662c 2066 696c 6570 6174 683a  (self, filepath:
+0000d370: 2073 7472 293a 0a20 2020 2020 2020 206d   str):.        m
+0000d380: 6178 5f73 697a 6520 3d20 3130 3234 202a  ax_size = 1024 *
+0000d390: 2031 3032 3420 2a20 3130 3234 2020 2320   1024 * 1024  # 
+0000d3a0: 3120 4742 2069 6e20 6279 7465 730a 2020  1 GB in bytes.  
+0000d3b0: 2020 2020 2020 6966 2066 696c 6570 6174        if filepat
+0000d3c0: 682e 7374 6172 7473 7769 7468 2822 6773  h.startswith("gs
+0000d3d0: 3a2f 2f22 293a 2020 2320 4743 5320 6669  ://"):  # GCS fi
+0000d3e0: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
+0000d3f0: 2020 2020 636c 6965 6e74 203d 2073 746f      client = sto
+0000d400: 7261 6765 2e43 6c69 656e 7428 290a 2020  rage.Client().  
+0000d410: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
+0000d420: 5f6e 616d 652c 2062 6c6f 625f 6e61 6d65  _name, blob_name
+0000d430: 203d 2066 696c 6570 6174 682e 7370 6c69   = filepath.spli
+0000d440: 7428 222f 222c 2033 295b 323a 5d0a 2020  t("/", 3)[2:].  
+0000d450: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
+0000d460: 203d 2063 6c69 656e 742e 6275 636b 6574   = client.bucket
+0000d470: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+0000d480: 2020 2020 2020 2020 2020 626c 6f62 203d            blob =
+0000d490: 2062 7563 6b65 742e 626c 6f62 2862 6c6f   bucket.blob(blo
+0000d4a0: 625f 6e61 6d65 290a 2020 2020 2020 2020  b_name).        
+0000d4b0: 2020 2020 626c 6f62 2e72 656c 6f61 6428      blob.reload(
+0000d4c0: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
+0000d4d0: 6c65 5f73 697a 6520 3d20 626c 6f62 2e73  le_size = blob.s
+0000d4e0: 697a 650a 2020 2020 2020 2020 656c 7365  ize.        else
+0000d4f0: 3a20 2023 206c 6f63 616c 2066 696c 6520  :  # local file 
+0000d500: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+0000d510: 2066 696c 655f 7369 7a65 203d 206f 732e   file_size = os.
+0000d520: 7061 7468 2e67 6574 7369 7a65 2866 696c  path.getsize(fil
+0000d530: 6570 6174 6829 0a0a 2020 2020 2020 2020  epath)..        
+0000d540: 6966 2066 696c 655f 7369 7a65 203e 206d  if file_size > m
+0000d550: 6178 5f73 697a 653a 0a20 2020 2020 2020  ax_size:.       
+0000d560: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
+0000d570: 6f20 4742 0a20 2020 2020 2020 2020 2020  o GB.           
+0000d580: 2066 696c 655f 7369 7a65 203d 2072 6f75   file_size = rou
+0000d590: 6e64 2866 696c 655f 7369 7a65 202f 2028  nd(file_size / (
+0000d5a0: 3130 3234 2a2a 3329 2c20 3129 0a20 2020  1024**3), 1).   
+0000d5b0: 2020 2020 2020 2020 206d 6178 5f73 697a           max_siz
+0000d5c0: 6520 3d20 696e 7428 6d61 785f 7369 7a65  e = int(max_size
+0000d5d0: 202f 2031 3032 342a 2a33 290a 2020 2020   / 1024**3).    
+0000d5e0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+0000d5f0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+0000d600: 2020 2020 2020 2020 6622 4669 6c65 2073          f"File s
+0000d610: 697a 6520 7b66 696c 655f 7369 7a65 7d47  ize {file_size}G
+0000d620: 4220 6578 6365 6564 7320 7b6d 6178 5f73  B exceeds {max_s
+0000d630: 697a 657d 4742 2e20 220a 2020 2020 2020  ize}GB. ".      
+0000d640: 2020 2020 2020 2020 2020 2249 7420 6973            "It is
+0000d650: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
+0000d660: 7573 6520 656e 6769 6e65 3d27 6269 6771  use engine='bigq
+0000d670: 7565 7279 2720 220a 2020 2020 2020 2020  uery' ".        
+0000d680: 2020 2020 2020 2020 2266 6f72 206c 6172          "for lar
+0000d690: 6765 2066 696c 6573 2074 6f20 6176 6f69  ge files to avoi
+0000d6a0: 6420 6c6f 6164 696e 6720 7468 6520 6669  d loading the fi
+0000d6b0: 6c65 2069 6e74 6f20 6c6f 6361 6c20 6d65  le into local me
+0000d6c0: 6d6f 7279 2e22 0a20 2020 2020 2020 2020  mory.".         
+0000d6d0: 2020 2029 0a0a 2020 2020 6465 6620 5f63     )..    def _c
+0000d6e0: 7265 6174 655f 656d 7074 795f 7465 6d70  reate_empty_temp
+0000d6f0: 5f74 6162 6c65 280a 2020 2020 2020 2020  _table(.        
+0000d700: 7365 6c66 2c0a 2020 2020 2020 2020 7363  self,.        sc
+0000d710: 6865 6d61 3a20 4974 6572 6162 6c65 5b62  hema: Iterable[b
+0000d720: 6967 7175 6572 792e 5363 6865 6d61 4669  igquery.SchemaFi
+0000d730: 656c 645d 2c0a 2020 2020 2020 2020 636c  eld],.        cl
+0000d740: 7573 7465 725f 636f 6c73 3a20 4c69 7374  uster_cols: List
+0000d750: 5b73 7472 5d2c 0a20 2020 2029 202d 3e20  [str],.    ) -> 
+0000d760: 6269 6771 7565 7279 2e54 6162 6c65 5265  bigquery.TableRe
+0000d770: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
+0000d780: 2023 2043 616e 2774 2073 6574 2061 2074   # Can't set a t
+0000d790: 6162 6c65 2069 6e20 5f53 4553 5349 4f4e  able in _SESSION
+0000d7a0: 2061 7320 6465 7374 696e 6174 696f 6e20   as destination 
+0000d7b0: 7669 6120 7175 6572 7920 6a6f 6220 4150  via query job AP
+0000d7c0: 492c 2073 6f20 7765 0a20 2020 2020 2020  I, so we.       
+0000d7d0: 2023 2072 756e 2044 444c 2c20 696e 7374   # run DDL, inst
+0000d7e0: 6561 642e 0a20 2020 2020 2020 2064 6174  ead..        dat
+0000d7f0: 6173 6574 203d 2073 656c 662e 5f61 6e6f  aset = self._ano
+0000d800: 6e79 6d6f 7573 5f64 6174 6173 6574 0a20  nymous_dataset. 
+0000d810: 2020 2020 2020 2065 7870 6972 6174 696f         expiratio
+0000d820: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
+0000d830: 2020 6461 7465 7469 6d65 2e64 6174 6574    datetime.datet
+0000d840: 696d 652e 6e6f 7728 6461 7465 7469 6d65  ime.now(datetime
+0000d850: 2e74 696d 657a 6f6e 652e 7574 6329 202b  .timezone.utc) +
+0000d860: 2063 6f6e 7374 616e 7473 2e44 4546 4155   constants.DEFAU
+0000d870: 4c54 5f45 5850 4952 4154 494f 4e0a 2020  LT_EXPIRATION.  
+0000d880: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000d890: 2074 6162 6c65 203d 2062 6967 6672 616d   table = bigfram
+0000d8a0: 6573 5f69 6f2e 6372 6561 7465 5f74 656d  es_io.create_tem
+0000d8b0: 705f 7461 626c 6528 0a20 2020 2020 2020  p_table(.       
+0000d8c0: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
+0000d8d0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+0000d8e0: 6461 7461 7365 742c 0a20 2020 2020 2020  dataset,.       
+0000d8f0: 2020 2020 2065 7870 6972 6174 696f 6e2c       expiration,
+0000d900: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
+0000d910: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
+0000d920: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+0000d930: 636f 6c75 6d6e 733d 636c 7573 7465 725f  columns=cluster_
+0000d940: 636f 6c73 2c0a 2020 2020 2020 2020 290a  cols,.        ).
+0000d950: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+0000d960: 6967 7175 6572 792e 5461 626c 6552 6566  igquery.TableRef
+0000d970: 6572 656e 6365 2e66 726f 6d5f 7374 7269  erence.from_stri
+0000d980: 6e67 2874 6162 6c65 290a 0a20 2020 2064  ng(table)..    d
+0000d990: 6566 205f 6372 6561 7465 5f74 6f74 616c  ef _create_total
+0000d9a0: 5f6f 7264 6572 696e 6728 0a20 2020 2020  _ordering(.     
+0000d9b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d9c0: 2074 6162 6c65 3a20 6962 6973 5f74 7970   table: ibis_typ
+0000d9d0: 6573 2e54 6162 6c65 2c0a 2020 2020 2920  es.Table,.    ) 
+0000d9e0: 2d3e 2063 6f72 652e 4172 7261 7956 616c  -> core.ArrayVal
+0000d9f0: 7565 3a0a 2020 2020 2020 2020 2320 5369  ue:.        # Si
+0000da00: 6e63 6520 7468 6973 206d 6967 6874 2061  nce this might a
+0000da10: 6c73 6f20 6265 2075 7365 6420 6173 2074  lso be used as t
+0000da20: 6865 2069 6e64 6578 2c20 646f 6e27 7420  he index, don't 
+0000da30: 7573 6520 7468 6520 6465 6661 756c 740a  use the default.
+0000da40: 2020 2020 2020 2020 2320 226f 7264 6572          # "order
+0000da50: 696e 6720 4944 2220 6e61 6d65 2e0a 2020  ing ID" name..  
+0000da60: 2020 2020 2020 6f72 6465 7269 6e67 5f68        ordering_h
+0000da70: 6173 685f 7061 7274 203d 2067 7569 642e  ash_part = guid.
+0000da80: 6765 6e65 7261 7465 5f67 7569 6428 2262  generate_guid("b
+0000da90: 6967 6672 616d 6573 5f6f 7264 6572 696e  igframes_orderin
+0000daa0: 675f 2229 0a20 2020 2020 2020 206f 7264  g_").        ord
+0000dab0: 6572 696e 675f 7261 6e64 5f70 6172 7420  ering_rand_part 
+0000dac0: 3d20 6775 6964 2e67 656e 6572 6174 655f  = guid.generate_
+0000dad0: 6775 6964 2822 6269 6766 7261 6d65 735f  guid("bigframes_
+0000dae0: 6f72 6465 7269 6e67 5f22 290a 0a20 2020  ordering_")..   
+0000daf0: 2020 2020 2023 2041 6c6c 2069 6e70 7574       # All input
+0000db00: 7320 696e 746f 2068 6173 6820 6d75 7374  s into hash must
+0000db10: 2062 6520 6e6f 6e2d 6e75 6c6c 206f 7220   be non-null or 
+0000db20: 7265 7375 6c74 696e 6720 6861 7368 2077  resulting hash w
+0000db30: 696c 6c20 6265 206e 756c 6c0a 2020 2020  ill be null.    
+0000db40: 2020 2020 7374 725f 7661 6c75 6573 203d      str_values =
+0000db50: 206c 6973 7428 0a20 2020 2020 2020 2020   list(.         
+0000db60: 2020 206d 6170 286c 616d 6264 6120 636f     map(lambda co
+0000db70: 6c3a 205f 636f 6e76 6572 745f 746f 5f6e  l: _convert_to_n
+0000db80: 6f6e 6e75 6c6c 5f73 7472 696e 6728 7461  onnull_string(ta
+0000db90: 626c 655b 636f 6c5d 292c 2074 6162 6c65  ble[col]), table
+0000dba0: 2e63 6f6c 756d 6e73 290a 2020 2020 2020  .columns).      
+0000dbb0: 2020 290a 2020 2020 2020 2020 6675 6c6c    ).        full
+0000dbc0: 5f72 6f77 5f73 7472 203d 2028 0a20 2020  _row_str = (.   
+0000dbd0: 2020 2020 2020 2020 2073 7472 5f76 616c           str_val
+0000dbe0: 7565 735b 305d 2e63 6f6e 6361 7428 2a73  ues[0].concat(*s
+0000dbf0: 7472 5f76 616c 7565 735b 313a 5d29 0a20  tr_values[1:]). 
+0000dc00: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000dc10: 6e28 7374 725f 7661 6c75 6573 2920 3e20  n(str_values) > 
+0000dc20: 310a 2020 2020 2020 2020 2020 2020 656c  1.            el
+0000dc30: 7365 2073 7472 5f76 616c 7565 735b 305d  se str_values[0]
+0000dc40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000dc50: 2020 2066 756c 6c5f 726f 775f 6861 7368     full_row_hash
+0000dc60: 203d 2066 756c 6c5f 726f 775f 7374 722e   = full_row_str.
+0000dc70: 6861 7368 2829 2e6e 616d 6528 6f72 6465  hash().name(orde
+0000dc80: 7269 6e67 5f68 6173 685f 7061 7274 290a  ring_hash_part).
+0000dc90: 2020 2020 2020 2020 2320 5573 6564 2074          # Used t
+0000dca0: 6f20 6469 7361 6d62 6967 7561 7465 2062  o disambiguate b
+0000dcb0: 6574 7765 656e 2069 6465 6e74 6963 616c  etween identical
+0000dcc0: 2072 6f77 7320 2877 6869 6368 2077 696c   rows (which wil
+0000dcd0: 6c20 6861 7665 2069 6465 6e74 6963 616c  l have identical
+0000dce0: 2068 6173 6829 0a20 2020 2020 2020 2072   hash).        r
+0000dcf0: 616e 646f 6d5f 7661 6c75 6520 3d20 6962  andom_value = ib
+0000dd00: 6973 2e72 616e 646f 6d28 292e 6e61 6d65  is.random().name
+0000dd10: 286f 7264 6572 696e 675f 7261 6e64 5f70  (ordering_rand_p
+0000dd20: 6172 7429 0a0a 2020 2020 2020 2020 6f72  art)..        or
+0000dd30: 6967 696e 616c 5f63 6f6c 756d 6e5f 6964  iginal_column_id
+0000dd40: 7320 3d20 7461 626c 652e 636f 6c75 6d6e  s = table.column
+0000dd50: 730a 2020 2020 2020 2020 7461 626c 655f  s.        table_
+0000dd60: 7769 7468 5f6f 7264 6572 696e 6720 3d20  with_ordering = 
+0000dd70: 7461 626c 652e 7365 6c65 6374 280a 2020  table.select(.  
+0000dd80: 2020 2020 2020 2020 2020 6974 6572 746f            iterto
+0000dd90: 6f6c 732e 6368 6169 6e28 6f72 6967 696e  ols.chain(origin
+0000dda0: 616c 5f63 6f6c 756d 6e5f 6964 732c 205b  al_column_ids, [
+0000ddb0: 6675 6c6c 5f72 6f77 5f68 6173 682c 2072  full_row_hash, r
+0000ddc0: 616e 646f 6d5f 7661 6c75 655d 290a 2020  andom_value]).  
+0000ddd0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000dde0: 206f 7264 6572 696e 675f 7265 6631 203d   ordering_ref1 =
+0000ddf0: 206f 7264 6572 2e61 7363 656e 6469 6e67   order.ascending
+0000de00: 5f6f 7665 7228 6f72 6465 7269 6e67 5f68  _over(ordering_h
+0000de10: 6173 685f 7061 7274 290a 2020 2020 2020  ash_part).      
+0000de20: 2020 6f72 6465 7269 6e67 5f72 6566 3220    ordering_ref2 
+0000de30: 3d20 6f72 6465 722e 6173 6365 6e64 696e  = order.ascendin
+0000de40: 675f 6f76 6572 286f 7264 6572 696e 675f  g_over(ordering_
+0000de50: 7261 6e64 5f70 6172 7429 0a20 2020 2020  rand_part).     
+0000de60: 2020 206f 7264 6572 696e 6720 3d20 6f72     ordering = or
+0000de70: 6465 722e 4578 7072 6573 7369 6f6e 4f72  der.ExpressionOr
+0000de80: 6465 7269 6e67 280a 2020 2020 2020 2020  dering(.        
+0000de90: 2020 2020 6f72 6465 7269 6e67 5f76 616c      ordering_val
+0000dea0: 7565 5f63 6f6c 756d 6e73 3d28 6f72 6465  ue_columns=(orde
+0000deb0: 7269 6e67 5f72 6566 312c 206f 7264 6572  ring_ref1, order
+0000dec0: 696e 675f 7265 6632 292c 0a20 2020 2020  ing_ref2),.     
+0000ded0: 2020 2020 2020 2074 6f74 616c 5f6f 7264         total_ord
+0000dee0: 6572 696e 675f 636f 6c75 6d6e 733d 6672  ering_columns=fr
+0000def0: 6f7a 656e 7365 7428 5b6f 7264 6572 696e  ozenset([orderin
+0000df00: 675f 6861 7368 5f70 6172 742c 206f 7264  g_hash_part, ord
+0000df10: 6572 696e 675f 7261 6e64 5f70 6172 745d  ering_rand_part]
+0000df20: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
+0000df30: 2020 2020 2063 6f6c 756d 6e73 203d 205b       columns = [
+0000df40: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
+0000df50: 696e 675b 636f 6c5d 2066 6f72 2063 6f6c  ing[col] for col
+0000df60: 2069 6e20 6f72 6967 696e 616c 5f63 6f6c   in original_col
+0000df70: 756d 6e5f 6964 735d 0a20 2020 2020 2020  umn_ids].       
+0000df80: 2068 6964 6465 6e5f 636f 6c75 6d6e 7320   hidden_columns 
+0000df90: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0000dfa0: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
+0000dfb0: 696e 675b 6f72 6465 7269 6e67 5f68 6173  ing[ordering_has
+0000dfc0: 685f 7061 7274 5d2c 0a20 2020 2020 2020  h_part],.       
+0000dfd0: 2020 2020 2074 6162 6c65 5f77 6974 685f       table_with_
+0000dfe0: 6f72 6465 7269 6e67 5b6f 7264 6572 696e  ordering[orderin
+0000dff0: 675f 7261 6e64 5f70 6172 745d 2c0a 2020  g_rand_part],.  
+0000e000: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000e010: 7265 7475 726e 2063 6f72 652e 4172 7261  return core.Arra
+0000e020: 7956 616c 7565 2e66 726f 6d5f 6962 6973  yValue.from_ibis
+0000e030: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000e040: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000e050: 7461 626c 655f 7769 7468 5f6f 7264 6572  table_with_order
+0000e060: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+0000e070: 2063 6f6c 756d 6e73 2c0a 2020 2020 2020   columns,.      
+0000e080: 2020 2020 2020 6869 6464 656e 5f6f 7264        hidden_ord
+0000e090: 6572 696e 675f 636f 6c75 6d6e 733d 6869  ering_columns=hi
+0000e0a0: 6464 656e 5f63 6f6c 756d 6e73 2c0a 2020  dden_columns,.  
+0000e0b0: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
+0000e0c0: 6e67 3d6f 7264 6572 696e 672c 0a20 2020  ng=ordering,.   
+0000e0d0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0000e0e0: 5f69 6269 735f 746f 5f74 656d 705f 7461  _ibis_to_temp_ta
+0000e0f0: 626c 6528 0a20 2020 2020 2020 2073 656c  ble(.        sel
+0000e100: 662c 0a20 2020 2020 2020 2074 6162 6c65  f,.        table
+0000e110: 3a20 6962 6973 5f74 7970 6573 2e54 6162  : ibis_types.Tab
+0000e120: 6c65 2c0a 2020 2020 2020 2020 636c 7573  le,.        clus
+0000e130: 7465 725f 636f 6c73 3a20 4974 6572 6162  ter_cols: Iterab
+0000e140: 6c65 5b73 7472 5d2c 0a20 2020 2020 2020  le[str],.       
+0000e150: 2061 7069 5f6e 616d 653a 2073 7472 2c0a   api_name: str,.
+0000e160: 2020 2020 2920 2d3e 2062 6967 7175 6572      ) -> bigquer
+0000e170: 792e 5461 626c 6552 6566 6572 656e 6365  y.TableReference
+0000e180: 3a0a 2020 2020 2020 2020 6465 7374 696e  :.        destin
+0000e190: 6174 696f 6e2c 205f 203d 2073 656c 662e  ation, _ = self.
+0000e1a0: 5f71 7565 7279 5f74 6f5f 6465 7374 696e  _query_to_destin
+0000e1b0: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
+0000e1c0: 2020 2073 656c 662e 6962 6973 5f63 6c69     self.ibis_cli
+0000e1d0: 656e 742e 636f 6d70 696c 6528 7461 626c  ent.compile(tabl
+0000e1e0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000e1f0: 696e 6465 785f 636f 6c73 3d6c 6973 7428  index_cols=list(
+0000e200: 636c 7573 7465 725f 636f 6c73 292c 0a20  cluster_cols),. 
+0000e210: 2020 2020 2020 2020 2020 2061 7069 5f6e             api_n
+0000e220: 616d 653d 6170 695f 6e61 6d65 2c0a 2020  ame=api_name,.  
+0000e230: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000e240: 2320 5468 6572 6520 7368 6f75 6c64 2061  # There should a
+0000e250: 6c77 6179 7320 6265 2061 2064 6573 7469  lways be a desti
+0000e260: 6e61 7469 6f6e 2074 6162 6c65 2066 6f72  nation table for
+0000e270: 2074 6869 7320 7175 6572 7920 7479 7065   this query type
+0000e280: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000e290: 2074 7970 696e 672e 6361 7374 2862 6967   typing.cast(big
+0000e2a0: 7175 6572 792e 5461 626c 6552 6566 6572  query.TableRefer
+0000e2b0: 656e 6365 2c20 6465 7374 696e 6174 696f  ence, destinatio
+0000e2c0: 6e29 0a0a 2020 2020 6465 6620 7265 6d6f  n)..    def remo
+0000e2d0: 7465 5f66 756e 6374 696f 6e28 0a20 2020  te_function(.   
+0000e2e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000e2f0: 2020 2069 6e70 7574 5f74 7970 6573 3a20     input_types: 
+0000e300: 4c69 7374 5b74 7970 655d 2c0a 2020 2020  List[type],.    
+0000e310: 2020 2020 6f75 7470 7574 5f74 7970 653a      output_type:
+0000e320: 2074 7970 652c 0a20 2020 2020 2020 2064   type,.        d
+0000e330: 6174 6173 6574 3a20 4f70 7469 6f6e 616c  ataset: Optional
+0000e340: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000e350: 2020 2020 2020 6269 6771 7565 7279 5f63        bigquery_c
+0000e360: 6f6e 6e65 6374 696f 6e3a 204f 7074 696f  onnection: Optio
+0000e370: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000e380: 0a20 2020 2020 2020 2072 6575 7365 3a20  .        reuse: 
+0000e390: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000e3a0: 2020 2020 206e 616d 653a 204f 7074 696f       name: Optio
+0000e3b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000e3c0: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
+0000e3d0: 733a 204f 7074 696f 6e61 6c5b 5365 7175  s: Optional[Sequ
+0000e3e0: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
+0000e3f0: 652c 0a20 2020 2020 2020 2063 6c6f 7564  e,.        cloud
+0000e400: 5f66 756e 6374 696f 6e5f 7365 7276 6963  _function_servic
+0000e410: 655f 6163 636f 756e 743a 204f 7074 696f  e_account: Optio
+0000e420: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000e430: 0a20 2020 2020 2020 2063 6c6f 7564 5f66  .        cloud_f
+0000e440: 756e 6374 696f 6e5f 6b6d 735f 6b65 795f  unction_kms_key_
+0000e450: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
+0000e460: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000e470: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+0000e480: 6f6e 5f64 6f63 6b65 725f 7265 706f 7369  on_docker_reposi
+0000e490: 746f 7279 3a20 4f70 7469 6f6e 616c 5b73  tory: Optional[s
+0000e4a0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000e4b0: 2020 2020 6d61 785f 6261 7463 6869 6e67      max_batching
+0000e4c0: 5f72 6f77 733a 204f 7074 696f 6e61 6c5b  _rows: Optional[
+0000e4d0: 696e 745d 203d 2031 3030 302c 0a20 2020  int] = 1000,.   
+0000e4e0: 2029 3a0a 2020 2020 2020 2020 2222 2244   ):.        """D
+0000e4f0: 6563 6f72 6174 6f72 2074 6f20 7475 726e  ecorator to turn
+0000e500: 2061 2075 7365 7220 6465 6669 6e65 6420   a user defined 
+0000e510: 6675 6e63 7469 6f6e 2069 6e74 6f20 6120  function into a 
+0000e520: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
+0000e530: 6675 6e63 7469 6f6e 2e20 4368 6563 6b20  function. Check 
+0000e540: 6f75 740a 2020 2020 2020 2020 7468 6520  out.        the 
+0000e550: 636f 6465 2073 616d 706c 6573 2061 743a  code samples at:
+0000e560: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
+0000e570: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
+0000e580: 7279 2f64 6f63 732f 7265 6d6f 7465 2d66  ry/docs/remote-f
+0000e590: 756e 6374 696f 6e73 2362 6967 7175 6572  unctions#bigquer
+0000e5a0: 792d 6461 7461 6672 616d 6573 2e0a 0a20  y-dataframes... 
+0000e5b0: 2020 2020 2020 202e 2e20 6e6f 7465 3a3a         .. note::
+0000e5c0: 0a20 2020 2020 2020 2020 2020 2050 6c65  .            Ple
+0000e5d0: 6173 6520 6d61 6b65 2073 7572 6520 666f  ase make sure fo
+0000e5e0: 6c6c 6f77 696e 6720 6973 2073 6574 7570  llowing is setup
+0000e5f0: 2062 6566 6f72 6520 7573 696e 6720 7468   before using th
+0000e600: 6973 2041 5049 3a0a 0a20 2020 2020 2020  is API:..       
+0000e610: 2031 2e20 4861 7665 2074 6865 2062 656c   1. Have the bel
+0000e620: 6f77 2041 5049 7320 656e 6162 6c65 6420  ow APIs enabled 
+0000e630: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+0000e640: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+0000e650: 2042 6967 5175 6572 7920 436f 6e6e 6563   BigQuery Connec
+0000e660: 7469 6f6e 2041 5049 0a20 2020 2020 2020  tion API.       
+0000e670: 2020 2020 202a 2043 6c6f 7564 2046 756e       * Cloud Fun
+0000e680: 6374 696f 6e73 2041 5049 0a20 2020 2020  ctions API.     
+0000e690: 2020 2020 2020 202a 2043 6c6f 7564 2052         * Cloud R
+0000e6a0: 756e 2041 5049 0a20 2020 2020 2020 2020  un API.         
+0000e6b0: 2020 202a 2043 6c6f 7564 2042 7569 6c64     * Cloud Build
+0000e6c0: 2041 5049 0a20 2020 2020 2020 2020 2020   API.           
+0000e6d0: 202a 2041 7274 6966 6163 7420 5265 6769   * Artifact Regi
+0000e6e0: 7374 7279 2041 5049 0a20 2020 2020 2020  stry API.       
+0000e6f0: 2020 2020 202a 2043 6c6f 7564 2052 6573       * Cloud Res
+0000e700: 6f75 7263 6520 4d61 6e61 6765 7220 4150  ource Manager AP
+0000e710: 490a 0a20 2020 2020 2020 2020 2020 5468  I..           Th
+0000e720: 6973 2063 616e 2062 6520 646f 6e65 2066  is can be done f
+0000e730: 726f 6d20 7468 6520 636c 6f75 6420 636f  rom the cloud co
+0000e740: 6e73 6f6c 6520 2863 6861 6e67 6520 6050  nsole (change `P
+0000e750: 524f 4a45 4354 5f49 4460 2074 6f20 796f  ROJECT_ID` to yo
+0000e760: 7572 7329 3a0a 2020 2020 2020 2020 2020  urs):.          
+0000e770: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
+0000e780: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
+0000e790: 6d2f 6170 6973 2f65 6e61 626c 6566 6c6f  m/apis/enableflo
+0000e7a0: 773f 6170 6969 643d 6269 6771 7565 7279  w?apiid=bigquery
+0000e7b0: 636f 6e6e 6563 7469 6f6e 2e67 6f6f 676c  connection.googl
+0000e7c0: 6561 7069 732e 636f 6d2c 636c 6f75 6466  eapis.com,cloudf
+0000e7d0: 756e 6374 696f 6e73 2e67 6f6f 676c 6561  unctions.googlea
+0000e7e0: 7069 732e 636f 6d2c 7275 6e2e 676f 6f67  pis.com,run.goog
+0000e7f0: 6c65 6170 6973 2e63 6f6d 2c63 6c6f 7564  leapis.com,cloud
+0000e800: 6275 696c 642e 676f 6f67 6c65 6170 6973  build.googleapis
+0000e810: 2e63 6f6d 2c61 7274 6966 6163 7472 6567  .com,artifactreg
+0000e820: 6973 7472 792e 676f 6f67 6c65 6170 6973  istry.googleapis
+0000e830: 2e63 6f6d 2c63 6c6f 7564 7265 736f 7572  .com,cloudresour
+0000e840: 6365 6d61 6e61 6765 722e 676f 6f67 6c65  cemanager.google
+0000e850: 6170 6973 2e63 6f6d 2670 726f 6a65 6374  apis.com&project
+0000e860: 3d50 524f 4a45 4354 5f49 440a 0a20 2020  =PROJECT_ID..   
+0000e870: 2020 2020 2020 2020 4f72 2066 726f 6d20          Or from 
+0000e880: 7468 6520 6763 6c6f 7564 2043 4c49 3a0a  the gcloud CLI:.
+0000e890: 0a20 2020 2020 2020 2020 2020 6024 2067  .           `$ g
+0000e8a0: 636c 6f75 6420 7365 7276 6963 6573 2065  cloud services e
+0000e8b0: 6e61 626c 6520 6269 6771 7565 7279 636f  nable bigqueryco
+0000e8c0: 6e6e 6563 7469 6f6e 2e67 6f6f 676c 6561  nnection.googlea
+0000e8d0: 7069 732e 636f 6d20 636c 6f75 6466 756e  pis.com cloudfun
+0000e8e0: 6374 696f 6e73 2e67 6f6f 676c 6561 7069  ctions.googleapi
+0000e8f0: 732e 636f 6d20 7275 6e2e 676f 6f67 6c65  s.com run.google
+0000e900: 6170 6973 2e63 6f6d 2063 6c6f 7564 6275  apis.com cloudbu
+0000e910: 696c 642e 676f 6f67 6c65 6170 6973 2e63  ild.googleapis.c
+0000e920: 6f6d 2061 7274 6966 6163 7472 6567 6973  om artifactregis
+0000e930: 7472 792e 676f 6f67 6c65 6170 6973 2e63  try.googleapis.c
+0000e940: 6f6d 2063 6c6f 7564 7265 736f 7572 6365  om cloudresource
+0000e950: 6d61 6e61 6765 722e 676f 6f67 6c65 6170  manager.googleap
+0000e960: 6973 2e63 6f6d 600a 0a20 2020 2020 2020  is.com`..       
+0000e970: 2032 2e20 4861 7665 2066 6f6c 6c6f 7769   2. Have followi
+0000e980: 6e67 2049 414d 2072 6f6c 6573 2065 6e61  ng IAM roles ena
+0000e990: 626c 6564 2066 6f72 2079 6f75 3a0a 0a20  bled for you:.. 
+0000e9a0: 2020 2020 2020 2020 2020 202a 2042 6967             * Big
+0000e9b0: 5175 6572 7920 4461 7461 2045 6469 746f  Query Data Edito
+0000e9c0: 7220 2872 6f6c 6573 2f62 6967 7175 6572  r (roles/bigquer
+0000e9d0: 792e 6461 7461 4564 6974 6f72 290a 2020  y.dataEditor).  
+0000e9e0: 2020 2020 2020 2020 2020 2a20 4269 6751            * BigQ
+0000e9f0: 7565 7279 2043 6f6e 6e65 6374 696f 6e20  uery Connection 
+0000ea00: 4164 6d69 6e20 2872 6f6c 6573 2f62 6967  Admin (roles/big
+0000ea10: 7175 6572 792e 636f 6e6e 6563 7469 6f6e  query.connection
+0000ea20: 4164 6d69 6e29 0a20 2020 2020 2020 2020  Admin).         
+0000ea30: 2020 202a 2043 6c6f 7564 2046 756e 6374     * Cloud Funct
+0000ea40: 696f 6e73 2044 6576 656c 6f70 6572 2028  ions Developer (
+0000ea50: 726f 6c65 732f 636c 6f75 6466 756e 6374  roles/cloudfunct
+0000ea60: 696f 6e73 2e64 6576 656c 6f70 6572 290a  ions.developer).
+0000ea70: 2020 2020 2020 2020 2020 2020 2a20 5365              * Se
+0000ea80: 7276 6963 6520 4163 636f 756e 7420 5573  rvice Account Us
+0000ea90: 6572 2028 726f 6c65 732f 6961 6d2e 7365  er (roles/iam.se
+0000eaa0: 7276 6963 6541 6363 6f75 6e74 5573 6572  rviceAccountUser
+0000eab0: 2920 6f6e 2074 6865 2073 6572 7669 6365  ) on the service
+0000eac0: 2061 6363 6f75 6e74 2060 5052 4f4a 4543   account `PROJEC
+0000ead0: 545f 4e55 4d42 4552 2d63 6f6d 7075 7465  T_NUMBER-compute
+0000eae0: 4064 6576 656c 6f70 6572 2e67 7365 7276  @developer.gserv
+0000eaf0: 6963 6561 6363 6f75 6e74 2e63 6f6d 600a  iceaccount.com`.
+0000eb00: 2020 2020 2020 2020 2020 2020 2a20 5374              * St
+0000eb10: 6f72 6167 6520 4f62 6a65 6374 2056 6965  orage Object Vie
+0000eb20: 7765 7220 2872 6f6c 6573 2f73 746f 7261  wer (roles/stora
+0000eb30: 6765 2e6f 626a 6563 7456 6965 7765 7229  ge.objectViewer)
+0000eb40: 0a20 2020 2020 2020 2020 2020 202a 2050  .            * P
+0000eb50: 726f 6a65 6374 2049 414d 2041 646d 696e  roject IAM Admin
+0000eb60: 2028 726f 6c65 732f 7265 736f 7572 6365   (roles/resource
+0000eb70: 6d61 6e61 6765 722e 7072 6f6a 6563 7449  manager.projectI
+0000eb80: 616d 4164 6d69 6e29 2028 4f6e 6c79 2072  amAdmin) (Only r
+0000eb90: 6571 7569 7265 6420 6966 2074 6865 2062  equired if the b
+0000eba0: 6967 7175 6572 7920 636f 6e6e 6563 7469  igquery connecti
+0000ebb0: 6f6e 2062 6569 6e67 2075 7365 6420 6973  on being used is
+0000ebc0: 206e 6f74 2070 7265 2d63 7265 6174 6564   not pre-created
+0000ebd0: 2061 6e64 2069 7320 6372 6561 7465 6420   and is created 
+0000ebe0: 6479 6e61 6d69 6361 6c6c 7920 7769 7468  dynamically with
+0000ebf0: 2075 7365 7220 6372 6564 656e 7469 616c   user credential
+0000ec00: 732e 290a 0a20 2020 2020 2020 2033 2e20  s.)..        3. 
+0000ec10: 4569 7468 6572 2074 6865 2075 7365 7220  Either the user 
+0000ec20: 6861 7320 7365 7449 616d 506f 6c69 6379  has setIamPolicy
+0000ec30: 2070 7269 7669 6c65 6765 206f 6e20 7468   privilege on th
+0000ec40: 6520 7072 6f6a 6563 742c 206f 7220 6120  e project, or a 
+0000ec50: 4269 6751 7565 7279 2063 6f6e 6e65 6374  BigQuery connect
+0000ec60: 696f 6e20 6973 2070 7265 2d63 7265 6174  ion is pre-creat
+0000ec70: 6564 2077 6974 6820 6e65 6365 7373 6172  ed with necessar
+0000ec80: 7920 4941 4d20 726f 6c65 2073 6574 3a0a  y IAM role set:.
+0000ec90: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
+0000eca0: 546f 2063 7265 6174 6520 6120 636f 6e6e  To create a conn
+0000ecb0: 6563 7469 6f6e 2c20 666f 6c6c 6f77 2068  ection, follow h
+0000ecc0: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
+0000ecd0: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
+0000ece0: 2f64 6f63 732f 7265 6665 7265 6e63 652f  /docs/reference/
+0000ecf0: 7374 616e 6461 7264 2d73 716c 2f72 656d  standard-sql/rem
+0000ed00: 6f74 652d 6675 6e63 7469 6f6e 7323 6372  ote-functions#cr
+0000ed10: 6561 7465 5f61 5f63 6f6e 6e65 6374 696f  eate_a_connectio
+0000ed20: 6e0a 2020 2020 2020 2020 2020 2020 322e  n.            2.
+0000ed30: 2054 6f20 7365 7420 7570 2049 414d 2c20   To set up IAM, 
+0000ed40: 666f 6c6c 6f77 2068 7474 7073 3a2f 2f63  follow https://c
+0000ed50: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
+0000ed60: 6269 6771 7565 7279 2f64 6f63 732f 7265  bigquery/docs/re
+0000ed70: 6665 7265 6e63 652f 7374 616e 6461 7264  ference/standard
+0000ed80: 2d73 716c 2f72 656d 6f74 652d 6675 6e63  -sql/remote-func
+0000ed90: 7469 6f6e 7323 6772 616e 745f 7065 726d  tions#grant_perm
+0000eda0: 6973 7369 6f6e 5f6f 6e5f 6675 6e63 7469  ission_on_functi
+0000edb0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+0000edc0: 2020 2041 6c74 6572 6e61 7469 7665 6c79     Alternatively
+0000edd0: 2c20 7468 6520 4941 4d20 636f 756c 6420  , the IAM could 
+0000ede0: 616c 736f 2062 6520 7365 7475 7020 7669  also be setup vi
+0000edf0: 6120 7468 6520 6763 6c6f 7564 2043 4c49  a the gcloud CLI
+0000ee00: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ee10: 2020 6024 2067 636c 6f75 6420 7072 6f6a    `$ gcloud proj
+0000ee20: 6563 7473 2061 6464 2d69 616d 2d70 6f6c  ects add-iam-pol
+0000ee30: 6963 792d 6269 6e64 696e 6720 5052 4f4a  icy-binding PROJ
+0000ee40: 4543 545f 4944 202d 2d6d 656d 6265 723d  ECT_ID --member=
+0000ee50: 2273 6572 7669 6365 4163 636f 756e 743a  "serviceAccount:
+0000ee60: 434f 4e4e 4543 5449 4f4e 5f53 4552 5649  CONNECTION_SERVI
+0000ee70: 4345 5f41 4343 4f55 4e54 5f49 4422 202d  CE_ACCOUNT_ID" -
+0000ee80: 2d72 6f6c 653d 2272 6f6c 6573 2f72 756e  -role="roles/run
+0000ee90: 2e69 6e76 6f6b 6572 2260 2e0a 0a20 2020  .invoker"`...   
+0000eea0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000eeb0: 2020 2020 2020 2069 6e70 7574 5f74 7970         input_typ
+0000eec0: 6573 2028 6c69 7374 2874 7970 6529 293a  es (list(type)):
+0000eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eee0: 204c 6973 7420 6f66 2069 6e70 7574 2064   List of input d
+0000eef0: 6174 6120 7479 7065 7320 696e 2074 6865  ata types in the
+0000ef00: 2075 7365 7220 6465 6669 6e65 6420 6675   user defined fu
+0000ef10: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
+0000ef20: 2020 2020 6f75 7470 7574 5f74 7970 6520      output_type 
+0000ef30: 2874 7970 6529 3a0a 2020 2020 2020 2020  (type):.        
+0000ef40: 2020 2020 2020 2020 4461 7461 2074 7970          Data typ
+0000ef50: 6520 6f66 2074 6865 206f 7574 7075 7420  e of the output 
+0000ef60: 696e 2074 6865 2075 7365 7220 6465 6669  in the user defi
+0000ef70: 6e65 6420 6675 6e63 7469 6f6e 2e0a 2020  ned function..  
+0000ef80: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+0000ef90: 7420 2873 7472 2c20 4f70 7469 6f6e 616c  t (str, Optional
+0000efa0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000efb0: 2020 2044 6174 6173 6574 2069 6e20 7768     Dataset in wh
+0000efc0: 6963 6820 746f 2063 7265 6174 6520 6120  ich to create a 
+0000efd0: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
+0000efe0: 6675 6e63 7469 6f6e 2e20 4974 2073 686f  function. It sho
+0000eff0: 756c 6420 6265 2069 6e0a 2020 2020 2020  uld be in.      
+0000f000: 2020 2020 2020 2020 2020 603c 7072 6f6a            `<proj
+0000f010: 6563 745f 6964 3e2e 3c64 6174 6173 6574  ect_id>.<dataset
+0000f020: 5f6e 616d 653e 6020 6f72 2060 3c64 6174  _name>` or `<dat
+0000f030: 6173 6574 5f6e 616d 653e 6020 666f 726d  aset_name>` form
+0000f040: 6174 2e20 4966 2074 6869 730a 2020 2020  at. If this.    
+0000f050: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0000f060: 6d65 7465 7220 6973 206e 6f74 2070 726f  meter is not pro
+0000f070: 7669 6465 6420 7468 656e 2073 6573 7369  vided then sessi
+0000f080: 6f6e 2064 6174 6173 6574 2069 6420 6973  on dataset id is
+0000f090: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
+0000f0a0: 2020 2062 6967 7175 6572 795f 636f 6e6e     bigquery_conn
+0000f0b0: 6563 7469 6f6e 2028 7374 722c 204f 7074  ection (str, Opt
+0000f0c0: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
+0000f0d0: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
+0000f0e0: 7468 6520 4269 6751 7565 7279 2063 6f6e  the BigQuery con
+0000f0f0: 6e65 6374 696f 6e2e 2059 6f75 2073 686f  nection. You sho
+0000f100: 756c 6420 6569 7468 6572 2068 6176 6520  uld either have 
+0000f110: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000f120: 2020 2020 636f 6e6e 6563 7469 6f6e 2061      connection a
+0000f130: 6c72 6561 6479 2063 7265 6174 6564 2069  lready created i
+0000f140: 6e20 7468 6520 606c 6f63 6174 696f 6e60  n the `location`
+0000f150: 2079 6f75 2068 6176 6520 6368 6f73 656e   you have chosen
+0000f160: 2c20 6f72 0a20 2020 2020 2020 2020 2020  , or.           
+0000f170: 2020 2020 2079 6f75 2073 686f 756c 6420       you should 
+0000f180: 6861 7665 2074 6865 2050 726f 6a65 6374  have the Project
+0000f190: 2049 414d 2041 646d 696e 2072 6f6c 6520   IAM Admin role 
+0000f1a0: 746f 2065 6e61 626c 6520 7468 6520 7365  to enable the se
+0000f1b0: 7276 6963 650a 2020 2020 2020 2020 2020  rvice.          
+0000f1c0: 2020 2020 2020 746f 2063 7265 6174 6520        to create 
+0000f1d0: 7468 6520 636f 6e6e 6563 7469 6f6e 2066  the connection f
+0000f1e0: 6f72 2079 6f75 2069 6620 796f 7520 6e65  or you if you ne
+0000f1f0: 6564 2069 742e 2049 6620 7468 6973 2070  ed it. If this p
+0000f200: 6172 616d 6574 6572 2069 730a 2020 2020  arameter is.    
+0000f210: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
+0000f220: 7072 6f76 6964 6564 2074 6865 6e20 7468  provided then th
+0000f230: 6520 4269 6751 7565 7279 2063 6f6e 6e65  e BigQuery conne
+0000f240: 6374 696f 6e20 6672 6f6d 2074 6865 2073  ction from the s
+0000f250: 6573 7369 6f6e 2069 7320 7573 6564 2e0a  ession is used..
+0000f260: 2020 2020 2020 2020 2020 2020 7265 7573              reus
+0000f270: 6520 2862 6f6f 6c2c 204f 7074 696f 6e61  e (bool, Optiona
+0000f280: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+0000f290: 2020 2020 5265 7573 6520 7468 6520 7265      Reuse the re
+0000f2a0: 6d6f 7465 2066 756e 6374 696f 6e20 6966  mote function if
+0000f2b0: 2061 6c72 6561 6479 2065 7869 7374 732e   already exists.
+0000f2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f2d0: 2060 5472 7565 6020 6279 2064 6566 6175   `True` by defau
+0000f2e0: 6c74 2c20 7768 6963 6820 7769 6c6c 2072  lt, which will r
+0000f2f0: 6573 756c 7420 696e 2072 6575 7369 6e67  esult in reusing
+0000f300: 2061 6e20 6578 6973 7469 6e67 2072 656d   an existing rem
+0000f310: 6f74 650a 2020 2020 2020 2020 2020 2020  ote.            
+0000f320: 2020 2020 6675 6e63 7469 6f6e 2061 6e64      function and
+0000f330: 2063 6f72 7265 7370 6f6e 6469 6e67 2063   corresponding c
+0000f340: 6c6f 7564 2066 756e 6374 696f 6e20 2869  loud function (i
+0000f350: 6620 616e 7929 2074 6861 7420 7761 730a  f any) that was.
+0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f370: 7072 6576 696f 7573 6c79 2063 7265 6174  previously creat
+0000f380: 6564 2066 6f72 2074 6865 2073 616d 6520  ed for the same 
+0000f390: 7564 662e 0a20 2020 2020 2020 2020 2020  udf..           
+0000f3a0: 2020 2020 2053 6574 7469 6e67 2069 7420       Setting it 
+0000f3b0: 746f 2060 4661 6c73 6560 2077 6f75 6c64  to `False` would
+0000f3c0: 2066 6f72 6365 2063 7265 6174 696e 6720   force creating 
+0000f3d0: 6120 756e 6971 7565 2072 656d 6f74 6520  a unique remote 
+0000f3e0: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
+0000f3f0: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+0000f400: 2072 6571 7569 7265 6420 7265 6d6f 7465   required remote
+0000f410: 2066 756e 6374 696f 6e20 646f 6573 206e   function does n
+0000f420: 6f74 2065 7869 7374 2074 6865 6e20 6974  ot exist then it
+0000f430: 2077 6f75 6c64 2062 650a 2020 2020 2020   would be.      
+0000f440: 2020 2020 2020 2020 2020 6372 6561 7465            create
+0000f450: 6420 6972 7265 7370 6563 7469 7665 206f  d irrespective o
+0000f460: 6620 7468 6973 2070 6172 616d 2e0a 2020  f this param..  
+0000f470: 2020 2020 2020 2020 2020 6e61 6d65 2028            name (
+0000f480: 7374 722c 204f 7074 696f 6e61 6c29 3a0a  str, Optional):.
+0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4a0: 4578 706c 6963 6974 206e 616d 6520 6f66  Explicit name of
+0000f4b0: 2074 6865 2070 6572 7369 7374 6564 2042   the persisted B
+0000f4c0: 6967 5175 6572 7920 7265 6d6f 7465 2066  igQuery remote f
+0000f4d0: 756e 6374 696f 6e2e 2055 7365 2069 7420  unction. Use it 
+0000f4e0: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
+0000f4f0: 2020 2020 2063 6175 7469 6f6e 2c20 6265       caution, be
+0000f500: 6361 7573 6520 7477 6f20 7573 6572 7320  cause two users 
+0000f510: 776f 726b 696e 6720 696e 2074 6865 2073  working in the s
+0000f520: 616d 6520 7072 6f6a 6563 7420 616e 6420  ame project and 
+0000f530: 6461 7461 7365 740a 2020 2020 2020 2020  dataset.        
+0000f540: 2020 2020 2020 2020 636f 756c 6420 6f76          could ov
+0000f550: 6572 7772 6974 6520 6561 6368 206f 7468  erwrite each oth
+0000f560: 6572 2773 2072 656d 6f74 6520 6675 6e63  er's remote func
+0000f570: 7469 6f6e 7320 6966 2074 6865 7920 7573  tions if they us
+0000f580: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
+0000f590: 2020 2020 2020 2020 2020 2070 6572 7369             persi
+0000f5a0: 7374 656e 7420 6e61 6d65 2e0a 2020 2020  stent name..    
+0000f5b0: 2020 2020 2020 2020 7061 636b 6167 6573          packages
+0000f5c0: 2028 7374 725b 5d2c 204f 7074 696f 6e61   (str[], Optiona
+0000f5d0: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+0000f5e0: 2020 2020 4578 706c 6963 6974 206e 616d      Explicit nam
+0000f5f0: 6520 6f66 2074 6865 2065 7874 6572 6e61  e of the externa
+0000f600: 6c20 7061 636b 6167 6520 6465 7065 6e64  l package depend
+0000f610: 656e 6369 6573 2e20 4561 6368 2064 6570  encies. Each dep
+0000f620: 656e 6465 6e63 790a 2020 2020 2020 2020  endency.        
+0000f630: 2020 2020 2020 2020 6973 2061 6464 6564          is added
+0000f640: 2074 6f20 7468 6520 6072 6571 7569 7265   to the `require
+0000f650: 6d65 6e74 732e 7478 7460 2061 7320 6973  ments.txt` as is
+0000f660: 2c20 616e 6420 6361 6e20 6265 206f 6620  , and can be of 
+0000f670: 7468 6520 666f 726d 0a20 2020 2020 2020  the form.       
+0000f680: 2020 2020 2020 2020 2073 7570 706f 7274           support
+0000f690: 6564 2069 6e20 6874 7470 733a 2f2f 7069  ed in https://pi
+0000f6a0: 702e 7079 7061 2e69 6f2f 656e 2f73 7461  p.pypa.io/en/sta
+0000f6b0: 626c 652f 7265 6665 7265 6e63 652f 7265  ble/reference/re
+0000f6c0: 7175 6972 656d 656e 7473 2d66 696c 652d  quirements-file-
+0000f6d0: 666f 726d 6174 2f2e 0a20 2020 2020 2020  format/..       
+0000f6e0: 2020 2020 2063 6c6f 7564 5f66 756e 6374       cloud_funct
+0000f6f0: 696f 6e5f 7365 7276 6963 655f 6163 636f  ion_service_acco
+0000f700: 756e 7420 2873 7472 2c20 4f70 7469 6f6e  unt (str, Option
+0000f710: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
+0000f720: 2020 2020 2053 6572 7669 6365 2061 6363       Service acc
+0000f730: 6f75 6e74 2074 6f20 7573 6520 666f 7220  ount to use for 
+0000f740: 7468 6520 636c 6f75 6420 6675 6e63 7469  the cloud functi
+0000f750: 6f6e 732e 2049 6620 6e6f 7420 7072 6f76  ons. If not prov
+0000f760: 6964 6564 0a20 2020 2020 2020 2020 2020  ided.           
+0000f770: 2020 2020 2074 6865 6e20 7468 6520 6465       then the de
+0000f780: 6661 756c 7420 7365 7276 6963 6520 6163  fault service ac
+0000f790: 636f 756e 7420 776f 756c 6420 6265 2075  count would be u
+0000f7a0: 7365 642e 2053 6565 0a20 2020 2020 2020  sed. See.       
+0000f7b0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+0000f7c0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+0000f7d0: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
+0000f7e0: 2f73 6563 7572 696e 672f 6675 6e63 7469  /securing/functi
+0000f7f0: 6f6e 2d69 6465 6e74 6974 790a 2020 2020  on-identity.    
+0000f800: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f810: 6d6f 7265 2064 6574 6169 6c73 2e20 506c  more details. Pl
+0000f820: 6561 7365 206d 616b 6520 7375 7265 2074  ease make sure t
+0000f830: 6865 2073 6572 7669 6365 2061 6363 6f75  he service accou
+0000f840: 6e74 2068 6173 2074 6865 0a20 2020 2020  nt has the.     
+0000f850: 2020 2020 2020 2020 2020 206e 6563 6573             neces
+0000f860: 7361 7279 2049 414d 2070 6572 6d69 7373  sary IAM permiss
+0000f870: 696f 6e73 2063 6f6e 6669 6775 7265 6420  ions configured 
+0000f880: 6173 2064 6573 6372 6962 6564 2069 6e0a  as described in.
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
+0000f8b0: 6f67 6c65 2e63 6f6d 2f66 756e 6374 696f  ogle.com/functio
+0000f8c0: 6e73 2f64 6f63 732f 7265 6665 7265 6e63  ns/docs/referenc
+0000f8d0: 652f 6961 6d2f 726f 6c65 7323 6164 6469  e/iam/roles#addi
+0000f8e0: 7469 6f6e 616c 2d63 6f6e 6669 6775 7261  tional-configura
+0000f8f0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+0000f900: 2020 636c 6f75 645f 6675 6e63 7469 6f6e    cloud_function
+0000f910: 5f6b 6d73 5f6b 6579 5f6e 616d 6520 2873  _kms_key_name (s
+0000f920: 7472 2c20 4f70 7469 6f6e 616c 293a 0a20  tr, Optional):. 
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+0000f940: 7573 746f 6d65 7220 6d61 6e61 6765 6420  ustomer managed 
+0000f950: 656e 6372 7970 7469 6f6e 206b 6579 2074  encryption key t
+0000f960: 6f20 7072 6f74 6563 7420 636c 6f75 6420  o protect cloud 
+0000f970: 6675 6e63 7469 6f6e 7320 616e 640a 2020  functions and.  
+0000f980: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f990: 6c61 7465 6420 6461 7461 2061 7420 7265  lated data at re
+0000f9a0: 7374 2e20 5468 6973 2069 7320 6f66 2074  st. This is of t
+0000f9b0: 6865 2066 6f72 6d61 740a 2020 2020 2020  he format.      
+0000f9c0: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
+0000f9d0: 7473 2f50 524f 4a45 4354 5f49 442f 6c6f  ts/PROJECT_ID/lo
+0000f9e0: 6361 7469 6f6e 732f 4c4f 4341 5449 4f4e  cations/LOCATION
+0000f9f0: 2f6b 6579 5269 6e67 732f 4b45 5952 494e  /keyRings/KEYRIN
+0000fa00: 472f 6372 7970 746f 4b65 7973 2f4b 4559  G/cryptoKeys/KEY
+0000fa10: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fa20: 2020 5265 6164 2068 7474 7073 3a2f 2f63    Read https://c
+0000fa30: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
+0000fa40: 6675 6e63 7469 6f6e 732f 646f 6373 2f73  functions/docs/s
+0000fa50: 6563 7572 696e 672f 636d 656b 2066 6f72  ecuring/cmek for
+0000fa60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fa70: 206d 6f72 6520 6465 7461 696c 7320 696e   more details in
+0000fa80: 636c 7564 696e 6720 6772 616e 7469 6e67  cluding granting
+0000fa90: 206e 6563 6573 7361 7279 2073 6572 7669   necessary servi
+0000faa0: 6365 2061 6363 6f75 6e74 730a 2020 2020  ce accounts.    
+0000fab0: 2020 2020 2020 2020 2020 2020 6163 6365              acce
+0000fac0: 7373 2074 6f20 7468 6520 6b65 792e 0a20  ss to the key.. 
+0000fad0: 2020 2020 2020 2020 2020 2063 6c6f 7564             cloud
+0000fae0: 5f66 756e 6374 696f 6e5f 646f 636b 6572  _function_docker
+0000faf0: 5f72 6570 6f73 6974 6f72 7920 2873 7472  _repository (str
+0000fb00: 2c20 4f70 7469 6f6e 616c 293a 0a20 2020  , Optional):.   
+0000fb10: 2020 2020 2020 2020 2020 2020 2044 6f63               Doc
+0000fb20: 6b65 7220 7265 706f 7369 746f 7279 2063  ker repository c
+0000fb30: 7265 6174 6564 2077 6974 6820 7468 6520  reated with the 
+0000fb40: 7361 6d65 2065 6e63 7279 7074 696f 6e20  same encryption 
+0000fb50: 6b65 7920 6173 0a20 2020 2020 2020 2020  key as.         
+0000fb60: 2020 2020 2020 2060 636c 6f75 645f 6675         `cloud_fu
+0000fb70: 6e63 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e  nction_kms_key_n
+0000fb80: 616d 6560 2074 6f20 7374 6f72 6520 656e  ame` to store en
+0000fb90: 6372 7970 7465 6420 6172 7469 6661 6374  crypted artifact
+0000fba0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000fbb0: 2020 6372 6561 7465 6420 746f 2073 7570    created to sup
+0000fbc0: 706f 7274 2074 6865 2063 6c6f 7564 2066  port the cloud f
+0000fbd0: 756e 6374 696f 6e2e 2054 6869 7320 6973  unction. This is
+0000fbe0: 206f 6620 7468 6520 666f 726d 6174 0a20   of the format. 
+0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000fc00: 726f 6a65 6374 732f 5052 4f4a 4543 545f  rojects/PROJECT_
+0000fc10: 4944 2f6c 6f63 6174 696f 6e73 2f4c 4f43  ID/locations/LOC
+0000fc20: 4154 494f 4e2f 7265 706f 7369 746f 7269  ATION/repositori
+0000fc30: 6573 2f52 4550 4f53 4954 4f52 595f 4e41  es/REPOSITORY_NA
+0000fc40: 4d45 2e0a 2020 2020 2020 2020 2020 2020  ME..            
+0000fc50: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
+0000fc60: 6169 6c73 2073 6565 0a20 2020 2020 2020  ails see.       
+0000fc70: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+0000fc80: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+0000fc90: 6d2f 6675 6e63 7469 6f6e 732f 646f 6373  m/functions/docs
+0000fca0: 2f73 6563 7572 696e 672f 636d 656b 2362  /securing/cmek#b
+0000fcb0: 6566 6f72 655f 796f 755f 6265 6769 6e2e  efore_you_begin.
+0000fcc0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000fcd0: 5f62 6174 6368 696e 675f 726f 7773 2028  _batching_rows (
+0000fce0: 696e 742c 204f 7074 696f 6e61 6c29 3a0a  int, Optional):.
+0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd00: 5468 6520 6d61 7869 6d75 6d20 6e75 6d62  The maximum numb
+0000fd10: 6572 206f 6620 726f 7773 2074 6f20 6265  er of rows to be
+0000fd20: 2062 6174 6368 6564 2066 6f72 2070 726f   batched for pro
+0000fd30: 6365 7373 696e 6720 696e 2074 6865 0a20  cessing in the. 
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2042                 B
+0000fd50: 5120 7265 6d6f 7465 2066 756e 6374 696f  Q remote functio
+0000fd60: 6e2e 2044 6566 6175 6c74 2076 616c 7565  n. Default value
+0000fd70: 2069 7320 3130 3030 2e20 4120 6c6f 7765   is 1000. A lowe
+0000fd80: 7220 6e75 6d62 6572 2063 616e 2062 650a  r number can be.
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fda0: 7061 7373 6564 2074 6f20 6176 6f69 6420  passed to avoid 
+0000fdb0: 7469 6d65 6f75 7473 2069 6e20 6361 7365  timeouts in case
+0000fdc0: 2074 6865 2075 7365 7220 636f 6465 2069   the user code i
+0000fdd0: 7320 746f 6f20 636f 6d70 6c65 7820 746f  s too complex to
+0000fde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fdf0: 2070 726f 6365 7373 206c 6172 6765 206e   process large n
+0000fe00: 756d 6265 7220 6f66 2072 6f77 7320 6661  umber of rows fa
+0000fe10: 7374 2065 6e6f 7567 682e 2041 2068 6967  st enough. A hig
+0000fe20: 6865 7220 6e75 6d62 6572 2063 616e 2062  her number can b
+0000fe30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000fe40: 2020 7573 6564 2074 6f20 696e 6372 6561    used to increa
+0000fe50: 7365 2074 6872 6f75 6768 7075 7420 696e  se throughput in
+0000fe60: 2063 6173 6520 7468 6520 7573 6572 2063   case the user c
+0000fe70: 6f64 6520 6973 2066 6173 7420 656e 6f75  ode is fast enou
+0000fe80: 6768 2e0a 2020 2020 2020 2020 2020 2020  gh..            
+0000fe90: 2020 2020 604e 6f6e 6560 2063 616e 2062      `None` can b
+0000fea0: 6520 7061 7373 6564 2074 6f20 6c65 7420  e passed to let 
+0000feb0: 4251 2072 656d 6f74 6520 6675 6e63 7469  BQ remote functi
+0000fec0: 6f6e 7320 7365 7276 6963 6520 6170 706c  ons service appl
+0000fed0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0000fee0: 2020 6465 6661 756c 7420 6261 7463 6869    default batchi
+0000fef0: 6e67 2e20 5365 6520 666f 7220 6d6f 7265  ng. See for more
+0000ff00: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
+0000ff10: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+0000ff20: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+0000ff30: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
+0000ff40: 7265 6d6f 7465 2d66 756e 6374 696f 6e73  remote-functions
+0000ff50: 236c 696d 6974 696e 675f 6e75 6d62 6572  #limiting_number
+0000ff60: 5f6f 665f 726f 7773 5f69 6e5f 615f 6261  _of_rows_in_a_ba
+0000ff70: 7463 685f 7265 7175 6573 742e 0a20 2020  tch_request..   
+0000ff80: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000ff90: 2020 2020 2020 2020 2020 6361 6c6c 6162            callab
+0000ffa0: 6c65 3a20 4120 7265 6d6f 7465 2066 756e  le: A remote fun
+0000ffb0: 6374 696f 6e20 6f62 6a65 6374 2070 6f69  ction object poi
+0000ffc0: 6e74 696e 6720 746f 2074 6865 2063 6c6f  nting to the clo
+0000ffd0: 7564 2061 7373 6574 7320 6372 6561 7465  ud assets create
+0000ffe0: 640a 2020 2020 2020 2020 2020 2020 696e  d.            in
+0000fff0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+00010000: 746f 2073 7570 706f 7274 2074 6865 2072  to support the r
+00010010: 656d 6f74 6520 6578 6563 7574 696f 6e2e  emote execution.
+00010020: 2054 6865 2063 6c6f 7564 2061 7373 6574   The cloud asset
+00010030: 7320 6361 6e20 6265 0a20 2020 2020 2020  s can be.       
+00010040: 2020 2020 206c 6f63 6174 6564 2074 6872       located thr
+00010050: 6f75 6768 2074 6865 2066 6f6c 6c6f 7769  ough the followi
+00010060: 6e67 2070 726f 7065 7274 6965 7320 7365  ng properties se
+00010070: 7420 696e 2074 6865 206f 626a 6563 743a  t in the object:
+00010080: 0a0a 2020 2020 2020 2020 2020 2020 6062  ..            `b
+00010090: 6967 6672 616d 6573 5f63 6c6f 7564 5f66  igframes_cloud_f
+000100a0: 756e 6374 696f 6e60 202d 2054 6865 2067  unction` - The g
+000100b0: 6f6f 676c 6520 636c 6f75 6420 6675 6e63  oogle cloud func
+000100c0: 7469 6f6e 2064 6570 6c6f 7965 6420 666f  tion deployed fo
+000100d0: 7220 7468 6520 7573 6572 2064 6566 696e  r the user defin
+000100e0: 6564 2063 6f64 652e 0a0a 2020 2020 2020  ed code...      
+000100f0: 2020 2020 2020 6062 6967 6672 616d 6573        `bigframes
+00010100: 5f72 656d 6f74 655f 6675 6e63 7469 6f6e  _remote_function
+00010110: 6020 2d20 5468 6520 6269 6771 7565 7279  ` - The bigquery
+00010120: 2072 656d 6f74 6520 6675 6e63 7469 6f6e   remote function
+00010130: 2063 6170 6162 6c65 206f 6620 6361 6c6c   capable of call
+00010140: 696e 6720 696e 746f 2060 6269 6766 7261  ing into `bigfra
+00010150: 6d65 735f 636c 6f75 645f 6675 6e63 7469  mes_cloud_functi
+00010160: 6f6e 602e 0a20 2020 2020 2020 2022 2222  on`..        """
+00010170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010180: 6269 6766 7261 6d65 735f 7266 280a 2020  bigframes_rf(.  
+00010190: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+000101a0: 7479 7065 732c 0a20 2020 2020 2020 2020  types,.         
+000101b0: 2020 206f 7574 7075 745f 7479 7065 2c0a     output_type,.
+000101c0: 2020 2020 2020 2020 2020 2020 7365 7373              sess
+000101d0: 696f 6e3d 7365 6c66 2c0a 2020 2020 2020  ion=self,.      
+000101e0: 2020 2020 2020 6461 7461 7365 743d 6461        dataset=da
+000101f0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
+00010200: 2020 2062 6967 7175 6572 795f 636f 6e6e     bigquery_conn
+00010210: 6563 7469 6f6e 3d62 6967 7175 6572 795f  ection=bigquery_
+00010220: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
+00010230: 2020 2020 2020 2020 7265 7573 653d 7265          reuse=re
+00010240: 7573 652c 0a20 2020 2020 2020 2020 2020  use,.           
+00010250: 206e 616d 653d 6e61 6d65 2c0a 2020 2020   name=name,.    
+00010260: 2020 2020 2020 2020 7061 636b 6167 6573          packages
+00010270: 3d70 6163 6b61 6765 732c 0a20 2020 2020  =packages,.     
+00010280: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
+00010290: 6374 696f 6e5f 7365 7276 6963 655f 6163  ction_service_ac
+000102a0: 636f 756e 743d 636c 6f75 645f 6675 6e63  count=cloud_func
+000102b0: 7469 6f6e 5f73 6572 7669 6365 5f61 6363  tion_service_acc
+000102c0: 6f75 6e74 2c0a 2020 2020 2020 2020 2020  ount,.          
+000102d0: 2020 636c 6f75 645f 6675 6e63 7469 6f6e    cloud_function
+000102e0: 5f6b 6d73 5f6b 6579 5f6e 616d 653d 636c  _kms_key_name=cl
+000102f0: 6f75 645f 6675 6e63 7469 6f6e 5f6b 6d73  oud_function_kms
+00010300: 5f6b 6579 5f6e 616d 652c 0a20 2020 2020  _key_name,.     
+00010310: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
+00010320: 6374 696f 6e5f 646f 636b 6572 5f72 6570  ction_docker_rep
+00010330: 6f73 6974 6f72 793d 636c 6f75 645f 6675  ository=cloud_fu
+00010340: 6e63 7469 6f6e 5f64 6f63 6b65 725f 7265  nction_docker_re
+00010350: 706f 7369 746f 7279 2c0a 2020 2020 2020  pository,.      
+00010360: 2020 2020 2020 6d61 785f 6261 7463 6869        max_batchi
+00010370: 6e67 5f72 6f77 733d 6d61 785f 6261 7463  ng_rows=max_batc
+00010380: 6869 6e67 5f72 6f77 732c 0a20 2020 2020  hing_rows,.     
+00010390: 2020 2029 0a0a 2020 2020 6465 6620 7265     )..    def re
+000103a0: 6164 5f67 6271 5f66 756e 6374 696f 6e28  ad_gbq_function(
+000103b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000103c0: 2020 2020 2020 2066 756e 6374 696f 6e5f         function_
+000103d0: 6e61 6d65 3a20 7374 722c 0a20 2020 2029  name: str,.    )
+000103e0: 3a0a 2020 2020 2020 2020 2222 224c 6f61  :.        """Loa
+000103f0: 6473 2061 2042 6967 5175 6572 7920 6675  ds a BigQuery fu
+00010400: 6e63 7469 6f6e 2066 726f 6d20 4269 6751  nction from BigQ
+00010410: 7565 7279 2e0a 0a20 2020 2020 2020 2054  uery...        T
+00010420: 6865 6e20 6974 2063 616e 2062 6520 6170  hen it can be ap
+00010430: 706c 6965 6420 746f 2061 2044 6174 6146  plied to a DataF
+00010440: 7261 6d65 206f 7220 5365 7269 6573 2e0a  rame or Series..
+00010450: 0a20 2020 2020 2020 202e 2e20 6e6f 7465  .        .. note
+00010460: 3a3a 0a20 2020 2020 2020 2020 2020 2054  ::.            T
+00010470: 6865 2072 6574 7572 6e20 7479 7065 206f  he return type o
+00010480: 6620 7468 6520 6675 6e63 7469 6f6e 206d  f the function m
+00010490: 7573 7420 6265 2065 7870 6c69 6369 746c  ust be explicitl
+000104a0: 7920 7370 6563 6966 6965 6420 696e 2074  y specified in t
+000104b0: 6865 0a20 2020 2020 2020 2020 2020 2066  he.            f
+000104c0: 756e 6374 696f 6e27 7320 6f72 6967 696e  unction's origin
+000104d0: 616c 2064 6566 696e 6974 696f 6e20 6576  al definition ev
+000104e0: 656e 2069 6620 6e6f 7420 6f74 6865 7277  en if not otherw
+000104f0: 6973 6520 7265 7175 6972 6564 2e0a 0a20  ise required... 
+00010500: 2020 2020 2020 2042 6967 5175 6572 7920         BigQuery 
+00010510: 5574 696c 7320 7072 6f76 6964 6573 206d  Utils provides m
+00010520: 616e 7920 7075 626c 6963 2066 756e 6374  any public funct
+00010530: 696f 6e73 2075 6e64 6572 2074 6865 2060  ions under the `
+00010540: 6062 7175 7469 6c60 6020 7072 6f6a 6563  `bqutil`` projec
+00010550: 7420 6f6e 2047 6f6f 676c 6520 436c 6f75  t on Google Clou
+00010560: 6420 506c 6174 666f 726d 2070 726f 6a65  d Platform proje
+00010570: 6374 0a20 2020 2020 2020 2028 5365 653a  ct.        (See:
+00010580: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00010590: 636f 6d2f 476f 6f67 6c65 436c 6f75 6450  com/GoogleCloudP
+000105a0: 6c61 7466 6f72 6d2f 6269 6771 7565 7279  latform/bigquery
+000105b0: 2d75 7469 6c73 2f74 7265 652f 6d61 7374  -utils/tree/mast
+000105c0: 6572 2f75 6466 7323 7573 696e 672d 7468  er/udfs#using-th
+000105d0: 652d 7564 6673 292e 0a20 2020 2020 2020  e-udfs)..       
+000105e0: 2059 6f75 2063 616e 2063 6865 636b 6f75   You can checkou
+000105f0: 7420 436f 6d6d 756e 6974 7920 5544 4673  t Community UDFs
+00010600: 2074 6f20 7573 6520 636f 6d6d 756e 6974   to use communit
+00010610: 792d 636f 6e74 7269 6275 7465 6420 6675  y-contributed fu
+00010620: 6e63 7469 6f6e 732e 0a20 2020 2020 2020  nctions..       
+00010630: 2028 5365 653a 2068 7474 7073 3a2f 2f67   (See: https://g
+00010640: 6974 6875 622e 636f 6d2f 476f 6f67 6c65  ithub.com/Google
+00010650: 436c 6f75 6450 6c61 7466 6f72 6d2f 6269  CloudPlatform/bi
+00010660: 6771 7565 7279 2d75 7469 6c73 2f74 7265  gquery-utils/tre
+00010670: 652f 6d61 7374 6572 2f75 6466 732f 636f  e/master/udfs/co
+00010680: 6d6d 756e 6974 7923 636f 6d6d 756e 6974  mmunity#communit
+00010690: 792d 7564 6673 292e 0a0a 2020 2020 2020  y-udfs)...      
+000106a0: 2020 2a2a 4578 616d 706c 6573 3a2a 2a0a    **Examples:**.
+000106b0: 0a20 2020 2020 2020 2055 7365 2074 6865  .        Use the
+000106c0: 2060 6063 775f 6c6f 7765 725f 6361 7365   ``cw_lower_case
+000106d0: 5f61 7363 6969 5f6f 6e6c 7960 6020 6675  _ascii_only`` fu
+000106e0: 6e63 7469 6f6e 2066 726f 6d20 436f 6d6d  nction from Comm
+000106f0: 756e 6974 7920 5544 4673 2e0a 2020 2020  unity UDFs..    
+00010700: 2020 2020 2868 7474 7073 3a2f 2f67 6974      (https://git
+00010710: 6875 622e 636f 6d2f 476f 6f67 6c65 436c  hub.com/GoogleCl
+00010720: 6f75 6450 6c61 7466 6f72 6d2f 6269 6771  oudPlatform/bigq
+00010730: 7565 7279 2d75 7469 6c73 2f62 6c6f 622f  uery-utils/blob/
+00010740: 6d61 7374 6572 2f75 6466 732f 636f 6d6d  master/udfs/comm
+00010750: 756e 6974 792f 6377 5f6c 6f77 6572 5f63  unity/cw_lower_c
+00010760: 6173 655f 6173 6369 695f 6f6e 6c79 2e73  ase_ascii_only.s
+00010770: 716c 7829 0a0a 2020 2020 2020 2020 2020  qlx)..          
+00010780: 2020 3e3e 3e20 696d 706f 7274 2062 6967    >>> import big
+00010790: 6672 616d 6573 2e70 616e 6461 7320 6173  frames.pandas as
+000107a0: 2062 7064 0a20 2020 2020 2020 2020 2020   bpd.           
+000107b0: 203e 3e3e 2062 7064 2e6f 7074 696f 6e73   >>> bpd.options
+000107c0: 2e64 6973 706c 6179 2e70 726f 6772 6573  .display.progres
+000107d0: 735f 6261 7220 3d20 4e6f 6e65 0a0a 2020  s_bar = None..  
+000107e0: 2020 2020 2020 2020 2020 3e3e 3e20 6466            >>> df
+000107f0: 203d 2062 7064 2e44 6174 6146 7261 6d65   = bpd.DataFrame
+00010800: 287b 2769 6427 3a20 5b31 2c20 322c 2033  ({'id': [1, 2, 3
+00010810: 5d2c 2027 6e61 6d65 273a 205b 2741 5552  ], 'name': ['AUR
+00010820: c389 4c49 4527 2c20 2743 c389 4c45 5354  ..LIE', 'C..LEST
+00010830: 494e 4527 2c20 2744 4150 484e c389 275d  INE', 'DAPHN..']
+00010840: 7d29 0a20 2020 2020 2020 2020 2020 203e  }).            >
+00010850: 3e3e 2064 660a 2020 2020 2020 2020 2020  >> df.          
+00010860: 2020 2020 2069 6420 2020 2020 2020 6e61       id       na
+00010870: 6d65 0a20 2020 2020 2020 2020 2020 2030  me.            0
+00010880: 2020 2031 2020 2020 4155 52c3 894c 4945     1    AUR..LIE
+00010890: 0a20 2020 2020 2020 2020 2020 2031 2020  .            1  
+000108a0: 2032 2020 43c3 894c 4553 5449 4e45 0a20   2  C..LESTINE. 
+000108b0: 2020 2020 2020 2020 2020 2032 2020 2033             2   3
+000108c0: 2020 2020 2044 4150 484e c389 0a20 2020       DAPHN...   
+000108d0: 2020 2020 2020 2020 203c 424c 414e 4b4c           <BLANKL
+000108e0: 494e 453e 0a20 2020 2020 2020 2020 2020  INE>.           
+000108f0: 205b 3320 726f 7773 2078 2032 2063 6f6c   [3 rows x 2 col
+00010900: 756d 6e73 5d0a 0a20 2020 2020 2020 2020  umns]..         
+00010910: 2020 203e 3e3e 2066 756e 6320 3d20 6270     >>> func = bp
+00010920: 642e 7265 6164 5f67 6271 5f66 756e 6374  d.read_gbq_funct
+00010930: 696f 6e28 2262 7175 7469 6c2e 666e 2e63  ion("bqutil.fn.c
+00010940: 775f 6c6f 7765 725f 6361 7365 5f61 7363  w_lower_case_asc
+00010950: 6969 5f6f 6e6c 7922 290a 2020 2020 2020  ii_only").      
+00010960: 2020 2020 2020 3e3e 3e20 6466 3120 3d20        >>> df1 = 
+00010970: 6466 2e61 7373 6967 6e28 6e65 775f 6e61  df.assign(new_na
+00010980: 6d65 3d64 665b 276e 616d 6527 5d2e 6170  me=df['name'].ap
+00010990: 706c 7928 6675 6e63 2929 0a20 2020 2020  ply(func)).     
+000109a0: 2020 2020 2020 203e 3e3e 2064 6631 0a20         >>> df1. 
+000109b0: 2020 2020 2020 2020 2020 2020 2020 6964                id
+000109c0: 2020 2020 2020 206e 616d 6520 2020 6e65         name   ne
+000109d0: 775f 6e61 6d65 0a20 2020 2020 2020 2020  w_name.         
+000109e0: 2020 2030 2020 2031 2020 2020 4155 52c3     0   1    AUR.
+000109f0: 894c 4945 2020 2020 6175 72c3 896c 6965  .LIE    aur..lie
+00010a00: 0a20 2020 2020 2020 2020 2020 2031 2020  .            1  
+00010a10: 2032 2020 43c3 894c 4553 5449 4e45 2020   2  C..LESTINE  
+00010a20: 63c3 896c 6573 7469 6e65 0a20 2020 2020  c..lestine.     
+00010a30: 2020 2020 2020 2032 2020 2033 2020 2020         2   3    
+00010a40: 2044 4150 484e c389 2020 2020 2064 6170   DAPHN..     dap
+00010a50: 686e c389 0a20 2020 2020 2020 2020 2020  hn...           
+00010a60: 203c 424c 414e 4b4c 494e 453e 0a20 2020   <BLANKLINE>.   
+00010a70: 2020 2020 2020 2020 205b 3320 726f 7773           [3 rows
+00010a80: 2078 2033 2063 6f6c 756d 6e73 5d0a 0a20   x 3 columns].. 
+00010a90: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00010aa0: 2020 2020 2020 2020 2066 756e 6374 696f           functio
+00010ab0: 6e5f 6e61 6d65 2028 7374 7229 3a0a 2020  n_name (str):.  
+00010ac0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00010ad0: 6520 6675 6e63 7469 6f6e 2773 206e 616d  e function's nam
+00010ae0: 6520 696e 2042 6967 5175 6572 7920 696e  e in BigQuery in
+00010af0: 2074 6865 2066 6f72 6d61 740a 2020 2020   the format.    
+00010b00: 2020 2020 2020 2020 2020 2020 6070 726f              `pro
+00010b10: 6a65 6374 5f69 642e 6461 7461 7365 745f  ject_id.dataset_
+00010b20: 6964 2e66 756e 6374 696f 6e5f 6e61 6d65  id.function_name
+00010b30: 602c 206f 720a 2020 2020 2020 2020 2020  `, or.          
+00010b40: 2020 2020 2020 6064 6174 6173 6574 5f69        `dataset_i
+00010b50: 642e 6675 6e63 7469 6f6e 5f6e 616d 6560  d.function_name`
+00010b60: 2074 6f20 6c6f 6164 2066 726f 6d20 7468   to load from th
+00010b70: 6520 6465 6661 756c 7420 7072 6f6a 6563  e default projec
+00010b80: 742c 206f 720a 2020 2020 2020 2020 2020  t, or.          
+00010b90: 2020 2020 2020 6066 756e 6374 696f 6e5f        `function_
+00010ba0: 6e61 6d65 6020 746f 206c 6f61 6420 6672  name` to load fr
+00010bb0: 6f6d 2074 6865 2064 6566 6175 6c74 2070  om the default p
+00010bc0: 726f 6a65 6374 2061 6e64 2074 6865 2064  roject and the d
+00010bd0: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
+00010be0: 2020 2020 2020 2061 7373 6f63 6961 7465         associate
+00010bf0: 6420 7769 7468 2074 6865 2063 7572 7265  d with the curre
+00010c00: 6e74 2073 6573 7369 6f6e 2e0a 0a20 2020  nt session...   
+00010c10: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00010c20: 2020 2020 2020 2020 2020 6361 6c6c 6162            callab
+00010c30: 6c65 3a20 4120 6675 6e63 7469 6f6e 206f  le: A function o
+00010c40: 626a 6563 7420 706f 696e 7469 6e67 2074  bject pointing t
+00010c50: 6f20 7468 6520 4269 6751 7565 7279 2066  o the BigQuery f
+00010c60: 756e 6374 696f 6e20 7265 6164 0a20 2020  unction read.   
+00010c70: 2020 2020 2020 2020 2066 726f 6d20 4269           from Bi
+00010c80: 6751 7565 7279 2e0a 0a20 2020 2020 2020  gQuery...       
+00010c90: 2020 2020 2054 6865 206f 626a 6563 7420       The object 
+00010ca0: 6973 2073 696d 696c 6172 2074 6f20 7468  is similar to th
+00010cb0: 6520 6f6e 6520 6372 6561 7465 6420 6279  e one created by
+00010cc0: 2074 6865 2060 7265 6d6f 7465 5f66 756e   the `remote_fun
+00010cd0: 6374 696f 6e60 0a20 2020 2020 2020 2020  ction`.         
+00010ce0: 2020 2064 6563 6f72 6174 6f72 2c20 696e     decorator, in
+00010cf0: 636c 7564 696e 6720 7468 6520 6062 6967  cluding the `big
+00010d00: 6672 616d 6573 5f72 656d 6f74 655f 6675  frames_remote_fu
+00010d10: 6e63 7469 6f6e 6020 7072 6f70 6572 7479  nction` property
+00010d20: 2c20 6275 740a 2020 2020 2020 2020 2020  , but.          
+00010d30: 2020 6e6f 7420 696e 636c 7564 696e 6720    not including 
+00010d40: 7468 6520 6062 6967 6672 616d 6573 5f63  the `bigframes_c
+00010d50: 6c6f 7564 5f66 756e 6374 696f 6e60 2070  loud_function` p
+00010d60: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
+00010d70: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+00010d80: 7475 726e 2062 6967 6672 616d 6573 5f72  turn bigframes_r
+00010d90: 6766 280a 2020 2020 2020 2020 2020 2020  gf(.            
+00010da0: 6675 6e63 7469 6f6e 5f6e 616d 653d 6675  function_name=fu
+00010db0: 6e63 7469 6f6e 5f6e 616d 652c 0a20 2020  nction_name,.   
+00010dc0: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+00010dd0: 3d73 656c 662c 0a20 2020 2020 2020 2029  =self,.        )
+00010de0: 0a0a 2020 2020 6465 6620 5f70 7265 7061  ..    def _prepa
+00010df0: 7265 5f71 7565 7279 5f6a 6f62 5f63 6f6e  re_query_job_con
+00010e00: 6669 6728 0a20 2020 2020 2020 2073 656c  fig(.        sel
+00010e10: 662c 0a20 2020 2020 2020 206a 6f62 5f63  f,.        job_c
+00010e20: 6f6e 6669 673a 204f 7074 696f 6e61 6c5b  onfig: Optional[
+00010e30: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
+00010e40: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
+00010e50: 0a20 2020 2029 202d 3e20 6269 6771 7565  .    ) -> bigque
+00010e60: 7279 2e51 7565 7279 4a6f 6243 6f6e 6669  ry.QueryJobConfi
+00010e70: 673a 0a20 2020 2020 2020 2069 6620 6a6f  g:.        if jo
+00010e80: 625f 636f 6e66 6967 2069 7320 4e6f 6e65  b_config is None
+00010e90: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+00010ea0: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
+00010eb0: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
+00010ec0: 6967 2829 0a20 2020 2020 2020 2065 6c73  ig().        els
+00010ed0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00010ee0: 2043 7265 6174 6520 6120 636f 7079 2073   Create a copy s
+00010ef0: 6f20 7468 6174 2077 6520 646f 6e27 7420  o that we don't 
+00010f00: 6d75 7461 7465 2074 6865 206f 7269 6769  mutate the origi
+00010f10: 6e61 6c20 636f 6e66 6967 2070 6173 7365  nal config passe
+00010f20: 640a 2020 2020 2020 2020 2020 2020 6a6f  d.            jo
+00010f30: 625f 636f 6e66 6967 203d 2074 7970 696e  b_config = typin
+00010f40: 672e 6361 7374 280a 2020 2020 2020 2020  g.cast(.        
+00010f50: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+00010f60: 2e51 7565 7279 4a6f 6243 6f6e 6669 672c  .QueryJobConfig,
+00010f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f80: 2062 6967 7175 6572 792e 5175 6572 794a   bigquery.QueryJ
+00010f90: 6f62 436f 6e66 6967 2e66 726f 6d5f 6170  obConfig.from_ap
+00010fa0: 695f 7265 7072 286a 6f62 5f63 6f6e 6669  i_repr(job_confi
+00010fb0: 672e 746f 5f61 7069 5f72 6570 7228 2929  g.to_api_repr())
+00010fc0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00010fd0: 0a20 2020 2020 2020 2069 6620 6269 6766  .        if bigf
+00010fe0: 7261 6d65 732e 6f70 7469 6f6e 732e 636f  rames.options.co
+00010ff0: 6d70 7574 652e 6d61 7869 6d75 6d5f 6279  mpute.maximum_by
+00011000: 7465 735f 6269 6c6c 6564 2069 7320 6e6f  tes_billed is no
+00011010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011020: 2020 2020 6a6f 625f 636f 6e66 6967 2e6d      job_config.m
+00011030: 6178 696d 756d 5f62 7974 6573 5f62 696c  aximum_bytes_bil
+00011040: 6c65 6420 3d20 280a 2020 2020 2020 2020  led = (.        
+00011050: 2020 2020 2020 2020 6269 6766 7261 6d65          bigframe
+00011060: 732e 6f70 7469 6f6e 732e 636f 6d70 7574  s.options.comput
+00011070: 652e 6d61 7869 6d75 6d5f 6279 7465 735f  e.maximum_bytes_
+00011080: 6269 6c6c 6564 0a20 2020 2020 2020 2020  billed.         
+00011090: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+000110a0: 2073 656c 662e 5f62 715f 6b6d 735f 6b65   self._bq_kms_ke
+000110b0: 795f 6e61 6d65 3a0a 2020 2020 2020 2020  y_name:.        
+000110c0: 2020 2020 6a6f 625f 636f 6e66 6967 2e64      job_config.d
+000110d0: 6573 7469 6e61 7469 6f6e 5f65 6e63 7279  estination_encry
+000110e0: 7074 696f 6e5f 636f 6e66 6967 7572 6174  ption_configurat
+000110f0: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
+00011100: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+00011110: 2e45 6e63 7279 7074 696f 6e43 6f6e 6669  .EncryptionConfi
+00011120: 6775 7261 7469 6f6e 286b 6d73 5f6b 6579  guration(kms_key
+00011130: 5f6e 616d 653d 7365 6c66 2e5f 6271 5f6b  _name=self._bq_k
+00011140: 6d73 5f6b 6579 5f6e 616d 6529 0a20 2020  ms_key_name).   
+00011150: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00011160: 2020 2020 7265 7475 726e 206a 6f62 5f63      return job_c
+00011170: 6f6e 6669 670a 0a20 2020 2064 6566 205f  onfig..    def _
+00011180: 7072 6570 6172 655f 6c6f 6164 5f6a 6f62  prepare_load_job
+00011190: 5f63 6f6e 6669 6728 7365 6c66 2920 2d3e  _config(self) ->
+000111a0: 2062 6967 7175 6572 792e 4c6f 6164 4a6f   bigquery.LoadJo
+000111b0: 6243 6f6e 6669 673a 0a20 2020 2020 2020  bConfig:.       
+000111c0: 2023 2043 7265 6174 6520 6120 636f 7079   # Create a copy
+000111d0: 2073 6f20 7468 6174 2077 6520 646f 6e27   so that we don'
+000111e0: 7420 6d75 7461 7465 2074 6865 206f 7269  t mutate the ori
+000111f0: 6769 6e61 6c20 636f 6e66 6967 2070 6173  ginal config pas
+00011200: 7365 640a 2020 2020 2020 2020 6a6f 625f  sed.        job_
+00011210: 636f 6e66 6967 203d 2062 6967 7175 6572  config = bigquer
+00011220: 792e 4c6f 6164 4a6f 6243 6f6e 6669 6728  y.LoadJobConfig(
+00011230: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00011240: 6c66 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e  lf._bq_kms_key_n
+00011250: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00011260: 206a 6f62 5f63 6f6e 6669 672e 6465 7374   job_config.dest
+00011270: 696e 6174 696f 6e5f 656e 6372 7970 7469  ination_encrypti
+00011280: 6f6e 5f63 6f6e 6669 6775 7261 7469 6f6e  on_configuration
+00011290: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000112a0: 2020 2020 2062 6967 7175 6572 792e 456e       bigquery.En
+000112b0: 6372 7970 7469 6f6e 436f 6e66 6967 7572  cryptionConfigur
+000112c0: 6174 696f 6e28 6b6d 735f 6b65 795f 6e61  ation(kms_key_na
+000112d0: 6d65 3d73 656c 662e 5f62 715f 6b6d 735f  me=self._bq_kms_
+000112e0: 6b65 795f 6e61 6d65 290a 2020 2020 2020  key_name).      
+000112f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00011300: 2072 6574 7572 6e20 6a6f 625f 636f 6e66   return job_conf
+00011310: 6967 0a0a 2020 2020 6465 6620 5f70 7265  ig..    def _pre
+00011320: 7061 7265 5f63 6f70 795f 6a6f 625f 636f  pare_copy_job_co
+00011330: 6e66 6967 2873 656c 6629 202d 3e20 6269  nfig(self) -> bi
+00011340: 6771 7565 7279 2e43 6f70 794a 6f62 436f  gquery.CopyJobCo
+00011350: 6e66 6967 3a0a 2020 2020 2020 2020 2320  nfig:.        # 
+00011360: 4372 6561 7465 2061 2063 6f70 7920 736f  Create a copy so
+00011370: 2074 6861 7420 7765 2064 6f6e 2774 206d   that we don't m
+00011380: 7574 6174 6520 7468 6520 6f72 6967 696e  utate the origin
+00011390: 616c 2063 6f6e 6669 6720 7061 7373 6564  al config passed
+000113a0: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
+000113b0: 6669 6720 3d20 6269 6771 7565 7279 2e43  fig = bigquery.C
+000113c0: 6f70 794a 6f62 436f 6e66 6967 2829 0a0a  opyJobConfig()..
+000113d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000113e0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
+000113f0: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+00011400: 625f 636f 6e66 6967 2e64 6573 7469 6e61  b_config.destina
+00011410: 7469 6f6e 5f65 6e63 7279 7074 696f 6e5f  tion_encryption_
+00011420: 636f 6e66 6967 7572 6174 696f 6e20 3d20  configuration = 
+00011430: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011440: 2020 6269 6771 7565 7279 2e45 6e63 7279    bigquery.Encry
+00011450: 7074 696f 6e43 6f6e 6669 6775 7261 7469  ptionConfigurati
+00011460: 6f6e 286b 6d73 5f6b 6579 5f6e 616d 653d  on(kms_key_name=
+00011470: 7365 6c66 2e5f 6271 5f6b 6d73 5f6b 6579  self._bq_kms_key
+00011480: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
+00011490: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+000114a0: 7475 726e 206a 6f62 5f63 6f6e 6669 670a  turn job_config.
+000114b0: 0a20 2020 2064 6566 205f 7374 6172 745f  .    def _start_
+000114c0: 7175 6572 7928 0a20 2020 2020 2020 2073  query(.        s
+000114d0: 656c 662c 0a20 2020 2020 2020 2073 716c  elf,.        sql
+000114e0: 3a20 7374 722c 0a20 2020 2020 2020 206a  : str,.        j
+000114f0: 6f62 5f63 6f6e 6669 673a 204f 7074 696f  ob_config: Optio
+00011500: 6e61 6c5b 6269 6771 7565 7279 2e6a 6f62  nal[bigquery.job
+00011510: 2e51 7565 7279 4a6f 6243 6f6e 6669 675d  .QueryJobConfig]
+00011520: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00011530: 206d 6178 5f72 6573 756c 7473 3a20 4f70   max_results: Op
+00011540: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00011550: 6e65 2c0a 2020 2020 2020 2020 7469 6d65  ne,.        time
+00011560: 6f75 743a 204f 7074 696f 6e61 6c5b 666c  out: Optional[fl
+00011570: 6f61 745d 203d 204e 6f6e 652c 0a20 2020  oat] = None,.   
+00011580: 2029 202d 3e20 5475 706c 655b 6269 6771   ) -> Tuple[bigq
+00011590: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
+000115a0: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
+000115b0: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
+000115c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000115d0: 5374 6172 7473 2042 6967 5175 6572 7920  Starts BigQuery 
+000115e0: 7175 6572 7920 6a6f 6220 616e 6420 7761  query job and wa
+000115f0: 6974 7320 666f 7220 7265 7375 6c74 732e  its for results.
+00011600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011610: 2020 2020 206a 6f62 5f63 6f6e 6669 6720       job_config 
+00011620: 3d20 7365 6c66 2e5f 7072 6570 6172 655f  = self._prepare_
+00011630: 7175 6572 795f 6a6f 625f 636f 6e66 6967  query_job_config
+00011640: 286a 6f62 5f63 6f6e 6669 6729 0a20 2020  (job_config).   
+00011650: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
+00011660: 7261 6d65 732e 7365 7373 696f 6e2e 5f69  rames.session._i
+00011670: 6f2e 6269 6771 7565 7279 2e73 7461 7274  o.bigquery.start
+00011680: 5f71 7565 7279 5f77 6974 685f 636c 6965  _query_with_clie
+00011690: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+000116a0: 7365 6c66 2e62 7163 6c69 656e 742c 2073  self.bqclient, s
+000116b0: 716c 2c20 6a6f 625f 636f 6e66 6967 2c20  ql, job_config, 
+000116c0: 6d61 785f 7265 7375 6c74 732c 2074 696d  max_results, tim
+000116d0: 656f 7574 0a20 2020 2020 2020 2029 0a0a  eout.        )..
+000116e0: 2020 2020 6465 6620 5f73 7461 7274 5f71      def _start_q
+000116f0: 7565 7279 5f6d 6c5f 6464 6c28 0a20 2020  uery_ml_ddl(.   
+00011700: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00011710: 2020 2073 716c 3a20 7374 722c 0a20 2020     sql: str,.   
+00011720: 2029 202d 3e20 5475 706c 655b 6269 6771   ) -> Tuple[bigq
+00011730: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
+00011740: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
+00011750: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
+00011760: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011770: 5374 6172 7473 2042 6967 5175 6572 7920  Starts BigQuery 
+00011780: 4d4c 2044 444c 2071 7565 7279 206a 6f62  ML DDL query job
+00011790: 2028 4352 4541 5445 204d 4f44 454c 2f41   (CREATE MODEL/A
+000117a0: 4c54 4552 204d 4f44 454c 2f2e 2e2e 2920  LTER MODEL/...) 
+000117b0: 616e 640a 2020 2020 2020 2020 7761 6974  and.        wait
+000117c0: 7320 666f 7220 7265 7375 6c74 732e 0a20  s for results.. 
+000117d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000117e0: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
+000117f0: 7365 6c66 2e5f 7072 6570 6172 655f 7175  self._prepare_qu
+00011800: 6572 795f 6a6f 625f 636f 6e66 6967 2829  ery_job_config()
+00011810: 0a0a 2020 2020 2020 2020 2320 4251 4d4c  ..        # BQML
+00011820: 2065 7870 6563 7473 206b 6d73 5f6b 6579   expects kms_key
+00011830: 5f6e 616d 6520 7468 726f 7567 6820 4f50  _name through OP
+00011840: 5449 4f4e 5320 616e 6420 6e6f 7420 7468  TIONS and not th
+00011850: 726f 7567 6820 6a6f 6220 636f 6e66 6967  rough job config
+00011860: 2c0a 2020 2020 2020 2020 2320 736f 2077  ,.        # so w
+00011870: 6520 6d75 7374 2072 6573 6574 2061 6e79  e must reset any
+00011880: 2065 6e63 7279 7074 696f 6e20 7365 7420   encryption set 
+00011890: 696e 2074 6865 206a 6f62 2063 6f6e 6669  in the job confi
+000118a0: 670a 2020 2020 2020 2020 2320 6874 7470  g.        # http
+000118b0: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+000118c0: 2e63 6f6d 2f62 6967 7175 6572 792f 646f  .com/bigquery/do
+000118d0: 6373 2f63 7573 746f 6d65 722d 6d61 6e61  cs/customer-mana
+000118e0: 6765 642d 656e 6372 7970 7469 6f6e 2365  ged-encryption#e
+000118f0: 6e63 7279 7074 2d6d 6f64 656c 0a20 2020  ncrypt-model.   
+00011900: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+00011910: 6465 7374 696e 6174 696f 6e5f 656e 6372  destination_encr
+00011920: 7970 7469 6f6e 5f63 6f6e 6669 6775 7261  yption_configura
+00011930: 7469 6f6e 203d 204e 6f6e 650a 0a20 2020  tion = None..   
+00011940: 2020 2020 2072 6574 7572 6e20 6269 6766       return bigf
+00011950: 7261 6d65 732e 7365 7373 696f 6e2e 5f69  rames.session._i
+00011960: 6f2e 6269 6771 7565 7279 2e73 7461 7274  o.bigquery.start
+00011970: 5f71 7565 7279 5f77 6974 685f 636c 6965  _query_with_clie
+00011980: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00011990: 7365 6c66 2e62 7163 6c69 656e 742c 2073  self.bqclient, s
+000119a0: 716c 2c20 6a6f 625f 636f 6e66 6967 0a20  ql, job_config. 
+000119b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+000119c0: 6620 5f63 6163 6865 5f77 6974 685f 636c  f _cache_with_cl
+000119d0: 7573 7465 725f 636f 6c73 280a 2020 2020  uster_cols(.    
+000119e0: 2020 2020 7365 6c66 2c20 6172 7261 795f      self, array_
+000119f0: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
+00011a00: 7956 616c 7565 2c20 636c 7573 7465 725f  yValue, cluster_
+00011a10: 636f 6c73 3a20 7479 7069 6e67 2e53 6571  cols: typing.Seq
+00011a20: 7565 6e63 655b 7374 725d 0a20 2020 2029  uence[str].    )
+00011a30: 202d 3e20 636f 7265 2e41 7272 6179 5661   -> core.ArrayVa
+00011a40: 6c75 653a 0a20 2020 2020 2020 2022 2222  lue:.        """
+00011a50: 4578 6563 7574 6573 2074 6865 2071 7565  Executes the que
+00011a60: 7279 2061 6e64 2075 7365 7320 7468 6520  ry and uses the 
+00011a70: 7265 7375 6c74 696e 6720 7461 626c 6520  resulting table 
+00011a80: 746f 2072 6577 7269 7465 2066 7574 7572  to rewrite futur
+00011a90: 6520 6578 6563 7574 696f 6e73 2e22 2222  e executions."""
+00011aa0: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
+00011ab0: 2055 7365 2074 6869 7320 666f 7220 616c   Use this for al
+00011ac0: 6c20 6578 6563 7574 696f 6e73 3f20 5072  l executions? Pr
+00011ad0: 6f62 6c65 6d20 6973 2074 6861 7420 6361  oblem is that ca
+00011ae0: 6368 696e 6720 6d61 7465 7269 616c 697a  ching materializ
+00011af0: 6573 2065 7874 7261 0a20 2020 2020 2020  es extra.       
+00011b00: 2023 206f 7264 6572 696e 6720 636f 6c75   # ordering colu
+00011b10: 6d6e 730a 2020 2020 2020 2020 636f 6d70  mns.        comp
+00011b20: 696c 6564 5f76 616c 7565 203d 2073 656c  iled_value = sel
+00011b30: 662e 5f63 6f6d 7069 6c65 5f6f 7264 6572  f._compile_order
+00011b40: 6564 2861 7272 6179 5f76 616c 7565 290a  ed(array_value).
+00011b50: 0a20 2020 2020 2020 2069 6269 735f 6578  .        ibis_ex
+00011b60: 7072 203d 2063 6f6d 7069 6c65 645f 7661  pr = compiled_va
+00011b70: 6c75 652e 5f74 6f5f 6962 6973 5f65 7870  lue._to_ibis_exp
+00011b80: 7228 0a20 2020 2020 2020 2020 2020 206f  r(.            o
+00011b90: 7264 6572 696e 675f 6d6f 6465 3d22 756e  rdering_mode="un
+00011ba0: 6f72 6465 7265 6422 2c20 6578 706f 7365  ordered", expose
+00011bb0: 5f68 6964 6465 6e5f 636f 6c73 3d54 7275  _hidden_cols=Tru
+00011bc0: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
+00011bd0: 2020 2020 746d 705f 7461 626c 6520 3d20      tmp_table = 
+00011be0: 7365 6c66 2e5f 6962 6973 5f74 6f5f 7465  self._ibis_to_te
+00011bf0: 6d70 5f74 6162 6c65 280a 2020 2020 2020  mp_table(.      
+00011c00: 2020 2020 2020 6962 6973 5f65 7870 722c        ibis_expr,
+00011c10: 2063 6c75 7374 6572 5f63 6f6c 733d 636c   cluster_cols=cl
+00011c20: 7573 7465 725f 636f 6c73 2c20 6170 695f  uster_cols, api_
+00011c30: 6e61 6d65 3d22 6361 6368 6564 220a 2020  name="cached".  
+00011c40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011c50: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+00011c60: 203d 2073 656c 662e 6962 6973 5f63 6c69   = self.ibis_cli
+00011c70: 656e 742e 7461 626c 6528 0a20 2020 2020  ent.table(.     
+00011c80: 2020 2020 2020 2074 6d70 5f74 6162 6c65         tmp_table
+00011c90: 2e74 6162 6c65 5f69 642c 0a20 2020 2020  .table_id,.     
+00011ca0: 2020 2020 2020 2073 6368 656d 613d 746d         schema=tm
+00011cb0: 705f 7461 626c 652e 6461 7461 7365 745f  p_table.dataset_
+00011cc0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00011cd0: 6461 7461 6261 7365 3d74 6d70 5f74 6162  database=tmp_tab
+00011ce0: 6c65 2e70 726f 6a65 6374 2c0a 2020 2020  le.project,.    
+00011cf0: 2020 2020 290a 2020 2020 2020 2020 6e65      ).        ne
+00011d00: 775f 636f 6c75 6d6e 7320 3d20 5b74 6162  w_columns = [tab
+00011d10: 6c65 5f65 7870 7265 7373 696f 6e5b 636f  le_expression[co
+00011d20: 6c75 6d6e 5d20 666f 7220 636f 6c75 6d6e  lumn] for column
+00011d30: 2069 6e20 636f 6d70 696c 6564 5f76 616c   in compiled_val
+00011d40: 7565 2e63 6f6c 756d 6e5f 6964 735d 0a20  ue.column_ids]. 
+00011d50: 2020 2020 2020 206e 6577 5f68 6964 6465         new_hidde
+00011d60: 6e5f 636f 6c75 6d6e 7320 3d20 5b0a 2020  n_columns = [.  
+00011d70: 2020 2020 2020 2020 2020 7461 626c 655f            table_
+00011d80: 6578 7072 6573 7369 6f6e 5b63 6f6c 756d  expression[colum
+00011d90: 6e5d 0a20 2020 2020 2020 2020 2020 2066  n].            f
+00011da0: 6f72 2063 6f6c 756d 6e20 696e 2063 6f6d  or column in com
+00011db0: 7069 6c65 645f 7661 6c75 652e 5f68 6964  piled_value._hid
+00011dc0: 6465 6e5f 6f72 6465 7269 6e67 5f63 6f6c  den_ordering_col
+00011dd0: 756d 6e5f 6e61 6d65 730a 2020 2020 2020  umn_names.      
+00011de0: 2020 5d0a 2020 2020 2020 2020 2320 544f    ].        # TO
+00011df0: 444f 3a20 496e 7374 6561 642c 206b 6565  DO: Instead, kee
+00011e00: 7020 7365 7373 696f 6e2d 7769 6465 206d  p session-wide m
+00011e10: 6170 206f 6620 6361 6368 6564 2072 6573  ap of cached res
+00011e20: 756c 7473 2061 6e64 2061 7574 6f6d 6174  ults and automat
+00011e30: 6963 616c 6c79 2072 6575 7365 0a20 2020  ically reuse.   
+00011e40: 2020 2020 2072 6574 7572 6e20 636f 7265       return core
+00011e50: 2e41 7272 6179 5661 6c75 652e 6672 6f6d  .ArrayValue.from
+00011e60: 5f69 6269 7328 0a20 2020 2020 2020 2020  _ibis(.         
+00011e70: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00011e80: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
+00011e90: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
+00011ea0: 2020 2063 6f6c 756d 6e73 3d6e 6577 5f63     columns=new_c
+00011eb0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+00011ec0: 2020 2020 6869 6464 656e 5f6f 7264 6572      hidden_order
+00011ed0: 696e 675f 636f 6c75 6d6e 733d 6e65 775f  ing_columns=new_
+00011ee0: 6869 6464 656e 5f63 6f6c 756d 6e73 2c0a  hidden_columns,.
+00011ef0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+00011f00: 7269 6e67 3d63 6f6d 7069 6c65 645f 7661  ring=compiled_va
+00011f10: 6c75 652e 5f6f 7264 6572 696e 672c 0a20  lue._ordering,. 
+00011f20: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00011f30: 6620 5f63 6163 6865 5f77 6974 685f 6f66  f _cache_with_of
+00011f40: 6673 6574 7328 7365 6c66 2c20 6172 7261  fsets(self, arra
+00011f50: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
+00011f60: 7261 7956 616c 7565 2920 2d3e 2063 6f72  rayValue) -> cor
+00011f70: 652e 4172 7261 7956 616c 7565 3a0a 2020  e.ArrayValue:.  
+00011f80: 2020 2020 2020 2222 2245 7865 6375 7465        """Execute
+00011f90: 7320 7468 6520 7175 6572 7920 616e 6420  s the query and 
+00011fa0: 7573 6573 2074 6865 2072 6573 756c 7469  uses the resulti
+00011fb0: 6e67 2074 6162 6c65 2074 6f20 7265 7772  ng table to rewr
+00011fc0: 6974 6520 6675 7475 7265 2065 7865 6375  ite future execu
+00011fd0: 7469 6f6e 732e 2222 220a 2020 2020 2020  tions.""".      
+00011fe0: 2020 2320 544f 444f 3a20 5573 6520 7468    # TODO: Use th
+00011ff0: 6973 2066 6f72 2061 6c6c 2065 7865 6375  is for all execu
+00012000: 7469 6f6e 733f 2050 726f 626c 656d 2069  tions? Problem i
+00012010: 7320 7468 6174 2063 6163 6869 6e67 206d  s that caching m
+00012020: 6174 6572 6961 6c69 7a65 7320 6578 7472  aterializes extr
+00012030: 610a 2020 2020 2020 2020 2320 6f72 6465  a.        # orde
+00012040: 7269 6e67 2063 6f6c 756d 6e73 0a20 2020  ring columns.   
+00012050: 2020 2020 2063 6f6d 7069 6c65 645f 7661       compiled_va
+00012060: 6c75 6520 3d20 7365 6c66 2e5f 636f 6d70  lue = self._comp
+00012070: 696c 655f 6f72 6465 7265 6428 6172 7261  ile_ordered(arra
+00012080: 795f 7661 6c75 6529 0a0a 2020 2020 2020  y_value)..      
+00012090: 2020 6962 6973 5f65 7870 7220 3d20 636f    ibis_expr = co
+000120a0: 6d70 696c 6564 5f76 616c 7565 2e5f 746f  mpiled_value._to
+000120b0: 5f69 6269 735f 6578 7072 280a 2020 2020  _ibis_expr(.    
+000120c0: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
+000120d0: 5f6d 6f64 653d 226f 6666 7365 745f 636f  _mode="offset_co
+000120e0: 6c22 2c20 6f72 6465 725f 636f 6c5f 6e61  l", order_col_na
+000120f0: 6d65 3d22 6269 6766 7261 6d65 735f 6f66  me="bigframes_of
+00012100: 6673 6574 7322 0a20 2020 2020 2020 2029  fsets".        )
+00012110: 0a20 2020 2020 2020 2074 6d70 5f74 6162  .        tmp_tab
+00012120: 6c65 203d 2073 656c 662e 5f69 6269 735f  le = self._ibis_
+00012130: 746f 5f74 656d 705f 7461 626c 6528 0a20  to_temp_table(. 
+00012140: 2020 2020 2020 2020 2020 2069 6269 735f             ibis_
+00012150: 6578 7072 2c20 636c 7573 7465 725f 636f  expr, cluster_co
+00012160: 6c73 3d5b 2262 6967 6672 616d 6573 5f6f  ls=["bigframes_o
+00012170: 6666 7365 7473 225d 2c20 6170 695f 6e61  ffsets"], api_na
+00012180: 6d65 3d22 6361 6368 6564 220a 2020 2020  me="cached".    
+00012190: 2020 2020 290a 2020 2020 2020 2020 7461      ).        ta
+000121a0: 626c 655f 6578 7072 6573 7369 6f6e 203d  ble_expression =
+000121b0: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
+000121c0: 742e 7461 626c 6528 0a20 2020 2020 2020  t.table(.       
+000121d0: 2020 2020 2074 6d70 5f74 6162 6c65 2e74       tmp_table.t
+000121e0: 6162 6c65 5f69 642c 0a20 2020 2020 2020  able_id,.       
+000121f0: 2020 2020 2073 6368 656d 613d 746d 705f       schema=tmp_
+00012200: 7461 626c 652e 6461 7461 7365 745f 6964  table.dataset_id
+00012210: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00012220: 7461 6261 7365 3d74 6d70 5f74 6162 6c65  tabase=tmp_table
+00012230: 2e70 726f 6a65 6374 2c0a 2020 2020 2020  .project,.      
+00012240: 2020 290a 2020 2020 2020 2020 6e65 775f    ).        new_
+00012250: 636f 6c75 6d6e 7320 3d20 5b74 6162 6c65  columns = [table
+00012260: 5f65 7870 7265 7373 696f 6e5b 636f 6c75  _expression[colu
+00012270: 6d6e 5d20 666f 7220 636f 6c75 6d6e 2069  mn] for column i
+00012280: 6e20 636f 6d70 696c 6564 5f76 616c 7565  n compiled_value
+00012290: 2e63 6f6c 756d 6e5f 6964 735d 0a20 2020  .column_ids].   
+000122a0: 2020 2020 206e 6577 5f68 6964 6465 6e5f       new_hidden_
+000122b0: 636f 6c75 6d6e 7320 3d20 5b74 6162 6c65  columns = [table
+000122c0: 5f65 7870 7265 7373 696f 6e5b 2262 6967  _expression["big
+000122d0: 6672 616d 6573 5f6f 6666 7365 7473 225d  frames_offsets"]
+000122e0: 5d0a 2020 2020 2020 2020 2320 544f 444f  ].        # TODO
+000122f0: 3a20 496e 7374 6561 642c 206b 6565 7020  : Instead, keep 
+00012300: 7365 7373 696f 6e2d 7769 6465 206d 6170  session-wide map
+00012310: 206f 6620 6361 6368 6564 2072 6573 756c   of cached resul
+00012320: 7473 2061 6e64 2061 7574 6f6d 6174 6963  ts and automatic
+00012330: 616c 6c79 2072 6575 7365 0a20 2020 2020  ally reuse.     
+00012340: 2020 2072 6574 7572 6e20 636f 7265 2e41     return core.A
+00012350: 7272 6179 5661 6c75 652e 6672 6f6d 5f69  rrayValue.from_i
+00012360: 6269 7328 0a20 2020 2020 2020 2020 2020  bis(.           
+00012370: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00012380: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
+00012390: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+000123a0: 2063 6f6c 756d 6e73 3d6e 6577 5f63 6f6c   columns=new_col
+000123b0: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
+000123c0: 2020 6869 6464 656e 5f6f 7264 6572 696e    hidden_orderin
+000123d0: 675f 636f 6c75 6d6e 733d 6e65 775f 6869  g_columns=new_hi
+000123e0: 6464 656e 5f63 6f6c 756d 6e73 2c0a 2020  dden_columns,.  
+000123f0: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
+00012400: 6e67 3d6f 7264 6572 2e45 7870 7265 7373  ng=order.Express
+00012410: 696f 6e4f 7264 6572 696e 672e 6672 6f6d  ionOrdering.from
+00012420: 5f6f 6666 7365 745f 636f 6c28 2262 6967  _offset_col("big
+00012430: 6672 616d 6573 5f6f 6666 7365 7473 2229  frames_offsets")
+00012440: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00012450: 2064 6566 205f 7369 6d70 6c69 6679 5f77   def _simplify_w
+00012460: 6974 685f 6361 6368 696e 6728 7365 6c66  ith_caching(self
+00012470: 2c20 6172 7261 795f 7661 6c75 653a 2063  , array_value: c
+00012480: 6f72 652e 4172 7261 7956 616c 7565 2920  ore.ArrayValue) 
+00012490: 2d3e 2063 6f72 652e 4172 7261 7956 616c  -> core.ArrayVal
+000124a0: 7565 3a0a 2020 2020 2020 2020 2222 2241  ue:.        """A
+000124b0: 7474 656d 7074 7320 746f 2068 616e 646c  ttempts to handl
+000124c0: 6520 7468 6520 636f 6d70 6c65 7869 7479  e the complexity
+000124d0: 2062 7920 6361 6368 696e 6720 6475 706c   by caching dupl
+000124e0: 6963 6174 6564 2073 7562 7472 6565 7320  icated subtrees 
+000124f0: 616e 6420 6272 6561 6b69 6e67 2074 6865  and breaking the
+00012500: 2071 7565 7279 2069 6e74 6f20 7069 6563   query into piec
+00012510: 6573 2e22 2222 0a20 2020 2020 2020 2069  es.""".        i
+00012520: 6620 6e6f 7420 6269 6766 7261 6d65 732e  f not bigframes.
+00012530: 6f70 7469 6f6e 732e 636f 6d70 7574 652e  options.compute.
+00012540: 656e 6162 6c65 5f6d 756c 7469 5f71 7565  enable_multi_que
+00012550: 7279 5f65 7865 6375 7469 6f6e 3a0a 2020  ry_execution:.  
+00012560: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012570: 2061 7272 6179 5f76 616c 7565 0a20 2020   array_value.   
+00012580: 2020 2020 206e 6f64 6520 3d20 6172 7261       node = arra
+00012590: 795f 7661 6c75 652e 6e6f 6465 0a20 2020  y_value.node.   
+000125a0: 2020 2020 2069 6620 6e6f 6465 2e70 6c61       if node.pla
+000125b0: 6e6e 696e 675f 636f 6d70 6c65 7869 7479  nning_complexity
+000125c0: 203c 2051 5545 5259 5f43 4f4d 504c 4558   < QUERY_COMPLEX
+000125d0: 4954 595f 4c49 4d49 543a 0a20 2020 2020  ITY_LIMIT:.     
+000125e0: 2020 2020 2020 2072 6574 7572 6e20 6172         return ar
+000125f0: 7261 795f 7661 6c75 650a 0a20 2020 2020  ray_value..     
+00012600: 2020 2066 6f72 205f 2069 6e20 7261 6e67     for _ in rang
+00012610: 6528 4d41 585f 5355 4254 5245 455f 4641  e(MAX_SUBTREE_FA
+00012620: 4354 4f52 494e 4753 293a 0a20 2020 2020  CTORINGS):.     
+00012630: 2020 2020 2020 2075 7064 6174 6564 203d         updated =
+00012640: 2073 656c 662e 5f63 6163 6865 5f6d 6f73   self._cache_mos
+00012650: 745f 636f 6d70 6c65 785f 7375 6274 7265  t_complex_subtre
+00012660: 6528 6e6f 6465 290a 2020 2020 2020 2020  e(node).        
+00012670: 2020 2020 6966 2075 7064 6174 6564 2069      if updated i
+00012680: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00012690: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+000126a0: 6f72 652e 4172 7261 7956 616c 7565 286e  ore.ArrayValue(n
+000126b0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
+000126c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000126d0: 2020 2020 2020 206e 6f64 6520 3d20 7570         node = up
+000126e0: 6461 7465 640a 0a20 2020 2020 2020 2072  dated..        r
+000126f0: 6574 7572 6e20 636f 7265 2e41 7272 6179  eturn core.Array
+00012700: 5661 6c75 6528 6e6f 6465 290a 0a20 2020  Value(node)..   
+00012710: 2064 6566 205f 6361 6368 655f 6d6f 7374   def _cache_most
+00012720: 5f63 6f6d 706c 6578 5f73 7562 7472 6565  _complex_subtree
+00012730: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00012740: 6e6f 6465 3a20 6e6f 6465 732e 4269 6746  node: nodes.BigF
+00012750: 7261 6d65 4e6f 6465 0a20 2020 2029 202d  rameNode.    ) -
+00012760: 3e20 4f70 7469 6f6e 616c 5b6e 6f64 6573  > Optional[nodes
+00012770: 2e42 6967 4672 616d 654e 6f64 655d 3a0a  .BigFrameNode]:.
+00012780: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+00012790: 4966 2071 7565 7279 2066 6169 6c73 2c20  If query fails, 
+000127a0: 7265 7472 7920 7769 7468 206c 6f77 6572  retry with lower
+000127b0: 2063 6f6d 706c 6578 6974 7920 6c69 6d69   complexity limi
+000127c0: 740a 2020 2020 2020 2020 7661 6c69 645f  t.        valid_
+000127d0: 6361 6e64 6964 6174 6573 203d 2074 7261  candidates = tra
+000127e0: 7665 7273 616c 732e 636f 756e 745f 636f  versals.count_co
+000127f0: 6d70 6c65 785f 6e6f 6465 7328 0a20 2020  mplex_nodes(.   
+00012800: 2020 2020 2020 2020 206e 6f64 652c 0a20           node,. 
+00012810: 2020 2020 2020 2020 2020 206d 696e 5f63             min_c
+00012820: 6f6d 706c 6578 6974 793d 2851 5545 5259  omplexity=(QUERY
+00012830: 5f43 4f4d 504c 4558 4954 595f 4c49 4d49  _COMPLEXITY_LIMI
+00012840: 5420 2f20 3530 3029 2c0a 2020 2020 2020  T / 500),.      
+00012850: 2020 2020 2020 6d61 785f 636f 6d70 6c65        max_comple
+00012860: 7869 7479 3d51 5545 5259 5f43 4f4d 504c  xity=QUERY_COMPL
+00012870: 4558 4954 595f 4c49 4d49 542c 0a20 2020  EXITY_LIMIT,.   
+00012880: 2020 2020 2029 2e69 7465 6d73 2829 0a20       ).items(). 
+00012890: 2020 2020 2020 2023 2048 6575 7269 7374         # Heurist
+000128a0: 6963 3a20 7375 6274 7265 655f 636f 6d70  ic: subtree_comp
+000128b0: 6c65 6978 7479 202a 2028 636f 7069 6573  leixty * (copies
+000128c0: 206f 6620 7375 6274 7265 6529 5e32 0a20   of subtree)^2. 
+000128d0: 2020 2020 2020 2062 6573 745f 6361 6e64         best_cand
+000128e0: 6964 6174 6520 3d20 6d61 7828 0a20 2020  idate = max(.   
+000128f0: 2020 2020 2020 2020 2076 616c 6964 5f63           valid_c
+00012900: 616e 6469 6461 7465 732c 0a20 2020 2020  andidates,.     
+00012910: 2020 2020 2020 206b 6579 3d6c 616d 6264         key=lambd
+00012920: 6120 693a 2069 5b30 5d2e 706c 616e 6e69  a i: i[0].planni
+00012930: 6e67 5f63 6f6d 706c 6578 6974 7920 2b20  ng_complexity + 
+00012940: 2869 5b31 5d20 2a2a 2032 292c 0a20 2020  (i[1] ** 2),.   
+00012950: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00012960: 3d4e 6f6e 652c 0a20 2020 2020 2020 2029  =None,.        )
+00012970: 0a0a 2020 2020 2020 2020 6966 2062 6573  ..        if bes
+00012980: 745f 6361 6e64 6964 6174 6520 6973 204e  t_candidate is N
+00012990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000129a0: 2023 204e 6f20 676f 6f64 2073 7562 7472   # No good subtr
+000129b0: 6565 7320 746f 2063 6163 6865 2c20 6a75  ees to cache, ju
+000129c0: 7374 2072 6574 7572 6e20 6f72 6967 696e  st return origin
+000129d0: 616c 2074 7265 650a 2020 2020 2020 2020  al tree.        
+000129e0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+000129f0: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
+00012a00: 2041 6464 2063 6c75 7374 6572 696e 6720   Add clustering 
+00012a10: 636f 6c75 6d6e 7320 6261 7365 6420 6f6e  columns based on
+00012a20: 2061 6363 6573 7320 7061 7474 6572 6e73   access patterns
+00012a30: 0a20 2020 2020 2020 206d 6174 6572 6961  .        materia
+00012a40: 6c69 7a65 6420 3d20 7365 6c66 2e5f 6361  lized = self._ca
+00012a50: 6368 655f 7769 7468 5f63 6c75 7374 6572  che_with_cluster
+00012a60: 5f63 6f6c 7328 0a20 2020 2020 2020 2020  _cols(.         
+00012a70: 2020 2063 6f72 652e 4172 7261 7956 616c     core.ArrayVal
+00012a80: 7565 2862 6573 745f 6361 6e64 6964 6174  ue(best_candidat
+00012a90: 655b 305d 292c 205b 5d0a 2020 2020 2020  e[0]), [].      
+00012aa0: 2020 292e 6e6f 6465 0a0a 2020 2020 2020    ).node..      
+00012ab0: 2020 7265 7475 726e 2074 7261 7665 7273    return travers
+00012ac0: 616c 732e 7265 706c 6163 655f 6e6f 6465  als.replace_node
+00012ad0: 7328 0a20 2020 2020 2020 2020 2020 206e  s(.            n
+00012ae0: 6f64 652c 2074 6f5f 7265 706c 6163 653d  ode, to_replace=
+00012af0: 6265 7374 5f63 616e 6469 6461 7465 5b30  best_candidate[0
+00012b00: 5d2c 2072 6570 6c61 6365 6d65 6e65 743d  ], replacemenet=
+00012b10: 6d61 7465 7269 616c 697a 6564 0a20 2020  materialized.   
+00012b20: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00012b30: 5f69 735f 7472 6976 6961 6c6c 795f 6578  _is_trivially_ex
+00012b40: 6563 7574 6162 6c65 2873 656c 662c 2061  ecutable(self, a
+00012b50: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
+00012b60: 2e41 7272 6179 5661 6c75 6529 3a0a 2020  .ArrayValue):.  
+00012b70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012b80: 2020 4361 6e20 7468 6520 626c 6f63 6b20    Can the block 
+00012b90: 6265 2065 7661 6c75 6174 6564 2076 6572  be evaluated ver
+00012ba0: 7920 6368 6561 706c 793f 0a20 2020 2020  y cheaply?.     
+00012bb0: 2020 2049 6620 5472 7565 2c20 7468 6520     If True, the 
+00012bc0: 6172 7261 795f 7661 6c75 6520 7072 6f62  array_value prob
+00012bd0: 6162 6c79 2069 7320 6e6f 7420 776f 7274  ably is not wort
+00012be0: 6820 6361 6368 696e 672e 0a20 2020 2020  h caching..     
+00012bf0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00012c00: 204f 6e63 6520 7265 7772 6974 696e 6720   Once rewriting 
+00012c10: 6973 2061 7661 696c 6162 6c65 2c20 7769  is available, wi
+00012c20: 6c6c 2077 616e 7420 746f 2072 6577 7269  ll want to rewri
+00012c30: 7465 2062 6566 6f72 650a 2020 2020 2020  te before.      
+00012c40: 2020 2320 6576 616c 7561 7469 6e67 2065    # evaluating e
+00012c50: 7865 6375 7469 6f6e 2063 6f73 742e 0a20  xecution cost.. 
+00012c60: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
+00012c70: 6176 6572 7361 6c73 2e69 735f 7472 6976  aversals.is_triv
+00012c80: 6961 6c6c 795f 6578 6563 7574 6162 6c65  ially_executable
+00012c90: 2861 7272 6179 5f76 616c 7565 2e6e 6f64  (array_value.nod
+00012ca0: 6529 0a0a 2020 2020 6465 6620 5f65 7865  e)..    def _exe
+00012cb0: 6375 7465 280a 2020 2020 2020 2020 7365  cute(.        se
+00012cc0: 6c66 2c0a 2020 2020 2020 2020 6172 7261  lf,.        arra
+00012cd0: 795f 7661 6c75 653a 2063 6f72 652e 4172  y_value: core.Ar
+00012ce0: 7261 7956 616c 7565 2c0a 2020 2020 2020  rayValue,.      
+00012cf0: 2020 6a6f 625f 636f 6e66 6967 3a20 4f70    job_config: Op
+00012d00: 7469 6f6e 616c 5b62 6967 7175 6572 792e  tional[bigquery.
+00012d10: 6a6f 622e 5175 6572 794a 6f62 436f 6e66  job.QueryJobConf
+00012d20: 6967 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ig] = None,.    
+00012d30: 2020 2020 2a2c 0a20 2020 2020 2020 2073      *,.        s
+00012d40: 6f72 7465 643a 2062 6f6f 6c20 3d20 5472  orted: bool = Tr
+00012d50: 7565 2c0a 2020 2020 2020 2020 6472 795f  ue,.        dry_
+00012d60: 7275 6e3d 4661 6c73 652c 0a20 2020 2020  run=False,.     
+00012d70: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
+00012d80: 6465 733a 204d 6170 7069 6e67 5b73 7472  des: Mapping[str
+00012d90: 2c20 7374 725d 203d 207b 7d2c 0a20 2020  , str] = {},.   
+00012da0: 2029 202d 3e20 7475 706c 655b 6269 6771   ) -> tuple[bigq
+00012db0: 7565 7279 2e74 6162 6c65 2e52 6f77 4974  uery.table.RowIt
+00012dc0: 6572 6174 6f72 2c20 6269 6771 7565 7279  erator, bigquery
+00012dd0: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
+00012de0: 2020 2020 7371 6c20 3d20 7365 6c66 2e5f      sql = self._
+00012df0: 746f 5f73 716c 280a 2020 2020 2020 2020  to_sql(.        
+00012e00: 2020 2020 6172 7261 795f 7661 6c75 652c      array_value,
+00012e10: 2073 6f72 7465 643d 736f 7274 6564 2c20   sorted=sorted, 
+00012e20: 636f 6c5f 6964 5f6f 7665 7272 6964 6573  col_id_overrides
+00012e30: 3d63 6f6c 5f69 645f 6f76 6572 7269 6465  =col_id_override
+00012e40: 730a 2020 2020 2020 2020 2920 2023 2074  s.        )  # t
+00012e50: 7970 653a 6967 6e6f 7265 0a20 2020 2020  ype:ignore.     
+00012e60: 2020 2069 6620 6a6f 625f 636f 6e66 6967     if job_config
+00012e70: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00012e80: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00012e90: 203d 2062 6967 7175 6572 792e 5175 6572   = bigquery.Quer
+00012ea0: 794a 6f62 436f 6e66 6967 2864 7279 5f72  yJobConfig(dry_r
+00012eb0: 756e 3d64 7279 5f72 756e 290a 2020 2020  un=dry_run).    
+00012ec0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012ed0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00012ee0: 2e64 7279 5f72 756e 203d 2064 7279 5f72  .dry_run = dry_r
+00012ef0: 756e 0a20 2020 2020 2020 2072 6574 7572  un.        retur
+00012f00: 6e20 7365 6c66 2e5f 7374 6172 745f 7175  n self._start_qu
+00012f10: 6572 7928 0a20 2020 2020 2020 2020 2020  ery(.           
+00012f20: 2073 716c 3d73 716c 2c0a 2020 2020 2020   sql=sql,.      
+00012f30: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00012f40: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
+00012f50: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00012f60: 5f70 6565 6b28 0a20 2020 2020 2020 2073  _peek(.        s
+00012f70: 656c 662c 2061 7272 6179 5f76 616c 7565  elf, array_value
+00012f80: 3a20 636f 7265 2e41 7272 6179 5661 6c75  : core.ArrayValu
+00012f90: 652c 206e 5f72 6f77 733a 2069 6e74 0a20  e, n_rows: int. 
+00012fa0: 2020 2029 202d 3e20 7475 706c 655b 6269     ) -> tuple[bi
+00012fb0: 6771 7565 7279 2e74 6162 6c65 2e52 6f77  gquery.table.Row
+00012fc0: 4974 6572 6174 6f72 2c20 6269 6771 7565  Iterator, bigque
+00012fd0: 7279 2e51 7565 7279 4a6f 625d 3a0a 2020  ry.QueryJob]:.  
+00012fe0: 2020 2020 2020 2222 2241 2027 7065 656b        """A 'peek
+00012ff0: 2720 6566 6669 6369 656e 746c 7920 6163  ' efficiently ac
+00013000: 6365 7373 6573 2061 2073 6d61 6c6c 206e  cesses a small n
+00013010: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
+00013020: 2074 6865 2064 6174 6166 7261 6d65 2e22   the dataframe."
+00013030: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00013040: 7420 7472 6565 5f70 726f 7065 7274 6965  t tree_propertie
+00013050: 732e 7065 656b 6162 6c65 2861 7272 6179  s.peekable(array
+00013060: 5f76 616c 7565 2e6e 6f64 6529 3a0a 2020  _value.node):.  
+00013070: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00013080: 6773 2e77 6172 6e28 2250 6565 6b69 6e67  gs.warn("Peeking
+00013090: 2074 6869 7320 7661 6c75 6520 6361 6e6e   this value cann
+000130a0: 6f74 2062 6520 646f 6e65 2065 6666 6963  ot be done effic
+000130b0: 6965 6e74 6c79 2e22 290a 2020 2020 2020  iently.").      
+000130c0: 2020 7371 6c20 3d20 7365 6c66 2e5f 636f    sql = self._co
+000130d0: 6d70 696c 655f 756e 6f72 6465 7265 6428  mpile_unordered(
+000130e0: 6172 7261 795f 7661 6c75 6529 2e70 6565  array_value).pee
+000130f0: 6b5f 7371 6c28 6e5f 726f 7773 290a 2020  k_sql(n_rows).  
+00013100: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013110: 662e 5f73 7461 7274 5f71 7565 7279 280a  f._start_query(.
+00013120: 2020 2020 2020 2020 2020 2020 7371 6c3d              sql=
+00013130: 7371 6c2c 0a20 2020 2020 2020 2029 0a0a  sql,.        )..
+00013140: 2020 2020 6465 6620 5f74 6f5f 7371 6c28      def _to_sql(
+00013150: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00013160: 2020 2020 2020 2061 7272 6179 5f76 616c         array_val
+00013170: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
+00013180: 6c75 652c 0a20 2020 2020 2020 206f 6666  lue,.        off
+00013190: 7365 745f 636f 6c75 6d6e 3a20 7479 7069  set_column: typi
+000131a0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+000131b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000131c0: 2063 6f6c 5f69 645f 6f76 6572 7269 6465   col_id_override
+000131d0: 733a 2074 7970 696e 672e 4d61 7070 696e  s: typing.Mappin
+000131e0: 675b 7374 722c 2073 7472 5d20 3d20 7b7d  g[str, str] = {}
+000131f0: 2c0a 2020 2020 2020 2020 736f 7274 6564  ,.        sorted
+00013200: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00013210: 2020 2020 2920 2d3e 2073 7472 3a0a 2020      ) -> str:.  
+00013220: 2020 2020 2020 6966 206f 6666 7365 745f        if offset_
+00013230: 636f 6c75 6d6e 3a0a 2020 2020 2020 2020  column:.        
+00013240: 2020 2020 6172 7261 795f 7661 6c75 6520      array_value 
+00013250: 3d20 6172 7261 795f 7661 6c75 652e 7072  = array_value.pr
+00013260: 6f6d 6f74 655f 6f66 6673 6574 7328 6f66  omote_offsets(of
+00013270: 6673 6574 5f63 6f6c 756d 6e29 0a20 2020  fset_column).   
+00013280: 2020 2020 2069 6620 736f 7274 6564 3a0a       if sorted:.
+00013290: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000132a0: 726e 2073 656c 662e 5f63 6f6d 7069 6c65  rn self._compile
+000132b0: 5f6f 7264 6572 6564 2861 7272 6179 5f76  _ordered(array_v
+000132c0: 616c 7565 292e 746f 5f73 716c 280a 2020  alue).to_sql(.  
+000132d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000132e0: 6c5f 6964 5f6f 7665 7272 6964 6573 3d63  l_id_overrides=c
+000132f0: 6f6c 5f69 645f 6f76 6572 7269 6465 732c  ol_id_overrides,
+00013300: 2073 6f72 7465 643d 5472 7565 0a20 2020   sorted=True.   
+00013310: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00013320: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00013330: 636f 6d70 696c 655f 756e 6f72 6465 7265  compile_unordere
+00013340: 6428 6172 7261 795f 7661 6c75 6529 2e74  d(array_value).t
+00013350: 6f5f 7371 6c28 0a20 2020 2020 2020 2020  o_sql(.         
+00013360: 2020 2063 6f6c 5f69 645f 6f76 6572 7269     col_id_overri
+00013370: 6465 733d 636f 6c5f 6964 5f6f 7665 7272  des=col_id_overr
+00013380: 6964 6573 0a20 2020 2020 2020 2029 0a0a  ides.        )..
+00013390: 2020 2020 6465 6620 5f63 6f6d 7069 6c65      def _compile
+000133a0: 5f6f 7264 6572 6564 280a 2020 2020 2020  _ordered(.      
+000133b0: 2020 7365 6c66 2c20 6172 7261 795f 7661    self, array_va
+000133c0: 6c75 653a 2063 6f72 652e 4172 7261 7956  lue: core.ArrayV
+000133d0: 616c 7565 0a20 2020 2029 202d 3e20 6269  alue.    ) -> bi
+000133e0: 6766 7261 6d65 732e 636f 7265 2e63 6f6d  gframes.core.com
+000133f0: 7069 6c65 2e4f 7264 6572 6564 4952 3a0a  pile.OrderedIR:.
+00013400: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00013410: 6967 6672 616d 6573 2e63 6f72 652e 636f  igframes.core.co
+00013420: 6d70 696c 652e 636f 6d70 696c 655f 6f72  mpile.compile_or
+00013430: 6465 7265 645f 6972 2861 7272 6179 5f76  dered_ir(array_v
+00013440: 616c 7565 2e6e 6f64 6529 0a0a 2020 2020  alue.node)..    
+00013450: 6465 6620 5f63 6f6d 7069 6c65 5f75 6e6f  def _compile_uno
+00013460: 7264 6572 6564 280a 2020 2020 2020 2020  rdered(.        
+00013470: 7365 6c66 2c20 6172 7261 795f 7661 6c75  self, array_valu
+00013480: 653a 2063 6f72 652e 4172 7261 7956 616c  e: core.ArrayVal
+00013490: 7565 0a20 2020 2029 202d 3e20 6269 6766  ue.    ) -> bigf
+000134a0: 7261 6d65 732e 636f 7265 2e63 6f6d 7069  rames.core.compi
+000134b0: 6c65 2e55 6e6f 7264 6572 6564 4952 3a0a  le.UnorderedIR:.
+000134c0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+000134d0: 6967 6672 616d 6573 2e63 6f72 652e 636f  igframes.core.co
+000134e0: 6d70 696c 652e 636f 6d70 696c 655f 756e  mpile.compile_un
+000134f0: 6f72 6465 7265 645f 6972 2861 7272 6179  ordered_ir(array
+00013500: 5f76 616c 7565 2e6e 6f64 6529 0a0a 2020  _value.node)..  
+00013510: 2020 6465 6620 5f67 6574 5f74 6162 6c65    def _get_table
+00013520: 5f73 697a 6528 7365 6c66 2c20 6465 7374  _size(self, dest
+00013530: 696e 6174 696f 6e5f 7461 626c 6529 3a0a  ination_table):.
+00013540: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+00013550: 7365 6c66 2e62 7163 6c69 656e 742e 6765  self.bqclient.ge
+00013560: 745f 7461 626c 6528 6465 7374 696e 6174  t_table(destinat
+00013570: 696f 6e5f 7461 626c 6529 0a20 2020 2020  ion_table).     
+00013580: 2020 2072 6574 7572 6e20 7461 626c 652e     return table.
+00013590: 6e75 6d5f 6279 7465 730a 0a20 2020 2064  num_bytes..    d
+000135a0: 6566 205f 726f 7773 5f74 6f5f 6461 7461  ef _rows_to_data
+000135b0: 6672 616d 6528 0a20 2020 2020 2020 2073  frame(.        s
+000135c0: 656c 662c 2072 6f77 5f69 7465 7261 746f  elf, row_iterato
+000135d0: 723a 2062 6967 7175 6572 792e 7461 626c  r: bigquery.tabl
+000135e0: 652e 526f 7749 7465 7261 746f 722c 2064  e.RowIterator, d
+000135f0: 7479 7065 733a 2044 6963 740a 2020 2020  types: Dict.    
+00013600: 2920 2d3e 2070 616e 6461 732e 4461 7461  ) -> pandas.Data
+00013610: 4672 616d 653a 0a20 2020 2020 2020 2023  Frame:.        #
+00013620: 2043 616e 2069 676e 6f72 6520 696e 6665   Can ignore infe
+00013630: 7272 6564 2064 6174 6174 7970 6520 756e  rred datatype un
+00013640: 7469 6c20 6474 7970 6520 656d 756c 6174  til dtype emulat
+00013650: 696f 6e20 6272 6561 6b73 2031 3a31 206d  ion breaks 1:1 m
+00013660: 6170 7069 6e67 2062 6574 7765 656e 2042  apping between B
+00013670: 5120 7479 7065 7320 616e 6420 6269 6766  Q types and bigf
+00013680: 7261 6d65 7320 7479 7065 730a 2020 2020  rames types.    
+00013690: 2020 2020 6474 7970 6573 5f66 726f 6d5f      dtypes_from_
+000136a0: 6271 203d 2062 6967 6672 616d 6573 2e64  bq = bigframes.d
+000136b0: 7479 7065 732e 6266 5f74 7970 655f 6672  types.bf_type_fr
+000136c0: 6f6d 5f74 7970 655f 6b69 6e64 2872 6f77  om_type_kind(row
+000136d0: 5f69 7465 7261 746f 722e 7363 6865 6d61  _iterator.schema
+000136e0: 290a 2020 2020 2020 2020 6172 726f 775f  ).        arrow_
+000136f0: 7461 626c 6520 3d20 726f 775f 6974 6572  table = row_iter
+00013700: 6174 6f72 2e74 6f5f 6172 726f 7728 290a  ator.to_arrow().
+00013710: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00013720: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00013730: 2e5f 696f 2e70 616e 6461 732e 6172 726f  ._io.pandas.arro
+00013740: 775f 746f 5f70 616e 6461 7328 6172 726f  w_to_pandas(arro
+00013750: 775f 7461 626c 652c 2064 7479 7065 735f  w_table, dtypes_
+00013760: 6672 6f6d 5f62 7129 0a0a 2020 2020 6465  from_bq)..    de
+00013770: 6620 5f73 7461 7274 5f67 656e 6572 6963  f _start_generic
+00013780: 5f6a 6f62 2873 656c 662c 206a 6f62 3a20  _job(self, job: 
+00013790: 666f 726d 6174 7469 6e67 5f68 656c 7065  formatting_helpe
+000137a0: 7273 2e47 656e 6572 6963 4a6f 6229 3a0a  rs.GenericJob):.
+000137b0: 2020 2020 2020 2020 6966 2062 6967 6672          if bigfr
+000137c0: 616d 6573 2e6f 7074 696f 6e73 2e64 6973  ames.options.dis
+000137d0: 706c 6179 2e70 726f 6772 6573 735f 6261  play.progress_ba
+000137e0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+000137f0: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+00013800: 7474 696e 675f 6865 6c70 6572 732e 7761  tting_helpers.wa
+00013810: 6974 5f66 6f72 5f6a 6f62 280a 2020 2020  it_for_job(.    
+00013820: 2020 2020 2020 2020 2020 2020 6a6f 622c              job,
+00013830: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
+00013840: 6e73 2e64 6973 706c 6179 2e70 726f 6772  ns.display.progr
+00013850: 6573 735f 6261 720a 2020 2020 2020 2020  ess_bar.        
+00013860: 2020 2020 2920 2023 2057 6169 7420 666f      )  # Wait fo
+00013870: 7220 7468 6520 6a6f 6220 746f 2063 6f6d  r the job to com
+00013880: 706c 6574 650a 2020 2020 2020 2020 656c  plete.        el
+00013890: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000138a0: 6a6f 622e 7265 7375 6c74 2829 0a0a 0a64  job.result()...d
+000138b0: 6566 2063 6f6e 6e65 6374 2863 6f6e 7465  ef connect(conte
+000138c0: 7874 3a20 4f70 7469 6f6e 616c 5b62 6967  xt: Optional[big
+000138d0: 7175 6572 795f 6f70 7469 6f6e 732e 4269  query_options.Bi
+000138e0: 6751 7565 7279 4f70 7469 6f6e 735d 203d  gQueryOptions] =
+000138f0: 204e 6f6e 6529 202d 3e20 5365 7373 696f   None) -> Sessio
+00013900: 6e3a 0a20 2020 2072 6574 7572 6e20 5365  n:.    return Se
+00013910: 7373 696f 6e28 636f 6e74 6578 7429 0a0a  ssion(context)..
+00013920: 0a64 6566 205f 6361 6e5f 636c 7573 7465  .def _can_cluste
+00013930: 725f 6271 2866 6965 6c64 3a20 6269 6771  r_bq(field: bigq
+00013940: 7565 7279 2e53 6368 656d 6146 6965 6c64  uery.SchemaField
+00013950: 293a 0a20 2020 2023 2068 7474 7073 3a2f  ):.    # https:/
+00013960: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+00013970: 6d2f 6269 6771 7565 7279 2f64 6f63 732f  m/bigquery/docs/
+00013980: 636c 7573 7465 7265 642d 7461 626c 6573  clustered-tables
+00013990: 0a20 2020 2023 204e 6f74 6162 6c79 2c20  .    # Notably, 
+000139a0: 666c 6f61 7420 6973 2065 7863 6c75 6465  float is exclude
+000139b0: 640a 2020 2020 7479 7065 5f20 3d20 6669  d.    type_ = fi
+000139c0: 656c 642e 6669 656c 645f 7479 7065 0a20  eld.field_type. 
+000139d0: 2020 2072 6574 7572 6e20 7479 7065 5f20     return type_ 
+000139e0: 696e 2028 0a20 2020 2020 2020 2022 494e  in (.        "IN
+000139f0: 5445 4745 5222 2c0a 2020 2020 2020 2020  TEGER",.        
+00013a00: 2249 4e54 3634 222c 0a20 2020 2020 2020  "INT64",.       
+00013a10: 2022 5354 5249 4e47 222c 0a20 2020 2020   "STRING",.     
+00013a20: 2020 2022 4e55 4d45 5249 4322 2c0a 2020     "NUMERIC",.  
+00013a30: 2020 2020 2020 2244 4543 494d 414c 222c        "DECIMAL",
+00013a40: 0a20 2020 2020 2020 2022 4249 474e 554d  .        "BIGNUM
+00013a50: 4552 4943 222c 0a20 2020 2020 2020 2022  ERIC",.        "
+00013a60: 4249 4744 4543 494d 414c 222c 0a20 2020  BIGDECIMAL",.   
+00013a70: 2020 2020 2022 4441 5445 222c 0a20 2020       "DATE",.   
+00013a80: 2020 2020 2022 4441 5445 5449 4d45 222c       "DATETIME",
+00013a90: 0a20 2020 2020 2020 2022 5449 4d45 5354  .        "TIMEST
+00013aa0: 414d 5022 2c0a 2020 2020 2020 2020 2242  AMP",.        "B
+00013ab0: 4f4f 4c22 2c0a 2020 2020 2020 2020 2242  OOL",.        "B
+00013ac0: 4f4f 4c45 414e 222c 0a20 2020 2029 0a0a  OOLEAN",.    )..
+00013ad0: 0a64 6566 205f 636f 6e76 6572 745f 746f  .def _convert_to
+00013ae0: 5f6e 6f6e 6e75 6c6c 5f73 7472 696e 6728  _nonnull_string(
+00013af0: 636f 6c75 6d6e 3a20 6962 6973 5f74 7970  column: ibis_typ
+00013b00: 6573 2e43 6f6c 756d 6e29 202d 3e20 6962  es.Column) -> ib
+00013b10: 6973 5f74 7970 6573 2e53 7472 696e 6756  is_types.StringV
+00013b20: 616c 7565 3a0a 2020 2020 636f 6c5f 7479  alue:.    col_ty
+00013b30: 7065 203d 2063 6f6c 756d 6e2e 7479 7065  pe = column.type
+00013b40: 2829 0a20 2020 2069 6620 280a 2020 2020  ().    if (.    
+00013b50: 2020 2020 636f 6c5f 7479 7065 2e69 735f      col_type.is_
+00013b60: 6e75 6d65 7269 6328 290a 2020 2020 2020  numeric().      
+00013b70: 2020 6f72 2063 6f6c 5f74 7970 652e 6973    or col_type.is
+00013b80: 5f62 6f6f 6c65 616e 2829 0a20 2020 2020  _boolean().     
+00013b90: 2020 206f 7220 636f 6c5f 7479 7065 2e69     or col_type.i
+00013ba0: 735f 6269 6e61 7279 2829 0a20 2020 2020  s_binary().     
+00013bb0: 2020 206f 7220 636f 6c5f 7479 7065 2e69     or col_type.i
+00013bc0: 735f 7465 6d70 6f72 616c 2829 0a20 2020  s_temporal().   
+00013bd0: 2029 3a0a 2020 2020 2020 2020 7265 7375   ):.        resu
+00013be0: 6c74 203d 2063 6f6c 756d 6e2e 6361 7374  lt = column.cast
+00013bf0: 2869 6269 735f 6474 7970 6573 2e53 7472  (ibis_dtypes.Str
+00013c00: 696e 6728 6e75 6c6c 6162 6c65 3d54 7275  ing(nullable=Tru
+00013c10: 6529 290a 2020 2020 656c 6966 2063 6f6c  e)).    elif col
+00013c20: 5f74 7970 652e 6973 5f67 656f 7370 6174  _type.is_geospat
+00013c30: 6961 6c28 293a 0a20 2020 2020 2020 2072  ial():.        r
+00013c40: 6573 756c 7420 3d20 7479 7069 6e67 2e63  esult = typing.c
+00013c50: 6173 7428 6962 6973 5f74 7970 6573 2e47  ast(ibis_types.G
+00013c60: 656f 5370 6174 6961 6c43 6f6c 756d 6e2c  eoSpatialColumn,
+00013c70: 2063 6f6c 756d 6e29 2e61 735f 7465 7874   column).as_text
+00013c80: 2829 0a20 2020 2065 6c69 6620 636f 6c5f  ().    elif col_
+00013c90: 7479 7065 2e69 735f 7374 7269 6e67 2829  type.is_string()
+00013ca0: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
+00013cb0: 203d 2063 6f6c 756d 6e0a 2020 2020 656c   = column.    el
+00013cc0: 7365 3a0a 2020 2020 2020 2020 2320 544f  se:.        # TO
+00013cd0: 5f4a 534f 4e5f 5354 5249 4e47 2077 6f72  _JSON_STRING wor
+00013ce0: 6b73 2077 6974 6820 616c 6c20 6461 7461  ks with all data
+00013cf0: 2074 7970 6573 2c20 6275 7420 6973 6e27   types, but isn'
+00013d00: 7420 7468 6520 6d6f 7374 2065 6666 6963  t the most effic
+00013d10: 6965 6e74 0a20 2020 2020 2020 2023 204e  ient.        # N
+00013d20: 6565 6465 6420 666f 7220 4a53 4f4e 2c20  eeded for JSON, 
+00013d30: 5354 5255 4354 2061 6e64 2041 5252 4159  STRUCT and ARRAY
+00013d40: 2064 6174 6174 7970 6573 0a20 2020 2020   datatypes.     
+00013d50: 2020 2072 6573 756c 7420 3d20 7665 6e64     result = vend
+00013d60: 6f72 6564 5f69 6269 735f 6f70 732e 546f  ored_ibis_ops.To
+00013d70: 4a73 6f6e 5374 7269 6e67 2863 6f6c 756d  JsonString(colum
+00013d80: 6e29 2e74 6f5f 6578 7072 2829 2020 2320  n).to_expr()  # 
+00013d90: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00013da0: 2023 2045 7363 6170 6520 6261 636b 736c   # Escape backsl
+00013db0: 6173 6865 7320 616e 6420 7573 6520 6261  ashes and use ba
+00013dc0: 636b 736c 6173 6820 6173 2064 656c 696e  ckslash as delin
+00013dd0: 6561 746f 720a 2020 2020 6573 6361 7065  eator.    escape
+00013de0: 6420 3d20 7479 7069 6e67 2e63 6173 7428  d = typing.cast(
+00013df0: 6962 6973 5f74 7970 6573 2e53 7472 696e  ibis_types.Strin
+00013e00: 6743 6f6c 756d 6e2c 2072 6573 756c 742e  gColumn, result.
+00013e10: 6669 6c6c 6e61 2822 2229 292e 7265 706c  fillna("")).repl
+00013e20: 6163 6528 225c 5c22 2c20 225c 5c5c 5c22  ace("\\", "\\\\"
+00013e30: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+00013e40: 650a 2020 2020 7265 7475 726e 2074 7970  e.    return typ
+00013e50: 696e 672e 6361 7374 2869 6269 735f 7479  ing.cast(ibis_ty
+00013e60: 7065 732e 5374 7269 6e67 436f 6c75 6d6e  pes.StringColumn
+00013e70: 2c20 6962 6973 2e6c 6974 6572 616c 2822  , ibis.literal("
+00013e80: 5c5c 2229 292e 636f 6e63 6174 2865 7363  \\")).concat(esc
+00013e90: 6170 6564 290a 0a0a 6465 6620 5f74 7261  aped)...def _tra
+00013ea0: 6e73 666f 726d 5f72 6561 645f 6762 715f  nsform_read_gbq_
+00013eb0: 636f 6e66 6967 7572 6174 696f 6e28 636f  configuration(co
+00013ec0: 6e66 6967 7572 6174 696f 6e3a 204f 7074  nfiguration: Opt
+00013ed0: 696f 6e61 6c5b 6469 6374 5d29 202d 3e20  ional[dict]) -> 
+00013ee0: 6469 6374 3a0a 2020 2020 2222 220a 2020  dict:.    """.  
+00013ef0: 2020 466f 7220 6261 636b 7761 7264 732d    For backwards-
+00013f00: 636f 6d70 6174 6962 696c 6974 792c 2063  compatibility, c
+00013f10: 6f6e 7665 7274 2061 6e79 2070 7265 7669  onvert any previ
+00013f20: 6f75 736c 7920 636c 6965 6e74 2d73 6964  ously client-sid
+00013f30: 6520 6f6e 6c79 0a20 2020 2070 6172 616d  e only.    param
+00013f40: 6574 6572 7320 7375 6368 2061 7320 7469  eters such as ti
+00013f50: 6d65 6f75 744d 7320 746f 2074 6865 2070  meoutMs to the p
+00013f60: 726f 7065 7274 7920 6e61 6d65 2065 7870  roperty name exp
+00013f70: 6563 7465 6420 6279 2074 6865 2052 4553  ected by the RES
+00013f80: 5420 4150 492e 0a0a 2020 2020 4d61 6b65  T API...    Make
+00013f90: 7320 6120 636f 7079 206f 6620 636f 6e66  s a copy of conf
+00013fa0: 6967 7572 6174 696f 6e20 6966 2063 6861  iguration if cha
+00013fb0: 6e67 6573 2061 7265 206e 6565 6465 642e  nges are needed.
+00013fc0: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
+00013fd0: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+00013fe0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013ff0: 7265 7475 726e 207b 7d0a 0a20 2020 2074  return {}..    t
+00014000: 696d 656f 7574 5f6d 7320 3d20 636f 6e66  imeout_ms = conf
+00014010: 6967 7572 6174 696f 6e2e 6765 7428 2271  iguration.get("q
+00014020: 7565 7279 222c 207b 7d29 2e67 6574 2822  uery", {}).get("
+00014030: 7469 6d65 6f75 744d 7322 290a 2020 2020  timeoutMs").    
+00014040: 6966 2074 696d 656f 7574 5f6d 7320 6973  if timeout_ms is
+00014050: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00014060: 2020 2023 2054 7261 6e73 666f 726d 2074     # Transform t
+00014070: 696d 656f 7574 4d73 2074 6f20 616e 2061  imeoutMs to an a
+00014080: 6374 7561 6c20 7365 7276 6572 2d73 6964  ctual server-sid
+00014090: 6520 636f 6e66 6967 7572 6174 696f 6e2e  e configuration.
+000140a0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+000140b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
+000140c0: 6f67 6c65 6170 6973 2f70 7974 686f 6e2d  ogleapis/python-
+000140d0: 6269 6771 7565 7279 2d70 616e 6461 732f  bigquery-pandas/
+000140e0: 6973 7375 6573 2f34 3739 0a20 2020 2020  issues/479.     
+000140f0: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
+00014100: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+00014110: 2863 6f6e 6669 6775 7261 7469 6f6e 290a  (configuration).
+00014120: 2020 2020 2020 2020 6465 6c20 636f 6e66          del conf
+00014130: 6967 7572 6174 696f 6e5b 2271 7565 7279  iguration["query
+00014140: 225d 5b22 7469 6d65 6f75 744d 7322 5d0a  "]["timeoutMs"].
+00014150: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00014160: 6174 696f 6e5b 226a 6f62 5469 6d65 6f75  ation["jobTimeou
+00014170: 744d 7322 5d20 3d20 7469 6d65 6f75 745f  tMs"] = timeout_
+00014180: 6d73 0a0a 2020 2020 7265 7475 726e 2063  ms..    return c
+00014190: 6f6e 6669 6775 7261 7469 6f6e 0a         onfiguration.
```

### Comparing `bigframes-1.2.0/bigframes/session/_io/__init__.py` & `bigframes-1.3.0/bigframes/session/_io/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/session/_io/bigquery.py` & `bigframes-1.3.0/bigframes/session/_io/bigquery.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Private module: Helpers for I/O operations."""
 
 from __future__ import annotations
 
 import datetime
 import itertools
+import os
 import textwrap
 import types
 from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
 import uuid
 
 import google.api_core.exceptions
 import google.cloud.bigquery as bigquery
@@ -30,14 +31,16 @@
 from bigframes.core import log_adapter
 import bigframes.formatting_helpers as formatting_helpers
 
 IO_ORDERING_ID = "bqdf_row_nums"
 MAX_LABELS_COUNT = 64
 TEMP_TABLE_PREFIX = "bqdf{date}_{random_id}"
 
+LOGGING_NAME_ENV_VAR = "BIGFRAMES_PERFORMANCE_LOG_NAME"
+
 
 def create_job_configs_labels(
     job_configs_labels: Optional[Dict[str, str]],
     api_methods: Sequence[str],
 ) -> Dict[str, str]:
     if job_configs_labels is None:
         job_configs_labels = {}
@@ -239,8 +242,36 @@
     opts = bigframes.options.display
     if opts.progress_bar is not None and not query_job.configuration.dry_run:
         results_iterator = formatting_helpers.wait_for_query_job(
             query_job, max_results, opts.progress_bar
         )
     else:
         results_iterator = query_job.result(max_results=max_results)
+
+    if LOGGING_NAME_ENV_VAR in os.environ:
+        # when running notebooks via pytest nbmake
+        pytest_log_job(query_job)
+
     return results_iterator, query_job
+
+
+def pytest_log_job(query_job: bigquery.QueryJob):
+    """For pytest runs only, log information about the query job
+    to a file in order to create a performance report.
+    """
+    if LOGGING_NAME_ENV_VAR not in os.environ:
+        raise EnvironmentError(
+            "Environment variable {env_var} is not set".format(
+                env_var=LOGGING_NAME_ENV_VAR
+            )
+        )
+    test_name = os.environ[LOGGING_NAME_ENV_VAR]
+    current_directory = os.getcwd()
+    bytes_processed = query_job.total_bytes_processed
+    if not isinstance(bytes_processed, int):
+        return  # filter out mocks
+    if query_job.configuration.dry_run:
+        # dry runs don't process their total_bytes_processed
+        bytes_processed = 0
+    bytes_file = os.path.join(current_directory, test_name + ".bytesprocessed")
+    with open(bytes_file, "a") as f:
+        f.write(str(bytes_processed) + "\n")
```

### Comparing `bigframes-1.2.0/bigframes/session/_io/pandas.py` & `bigframes-1.3.0/bigframes/session/_io/pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/session/clients.py` & `bigframes-1.3.0/bigframes/session/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/bigframes/version.py` & `bigframes-1.3.0/bigframes/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
```

### Comparing `bigframes-1.2.0/bigframes.egg-info/PKG-INFO` & `bigframes-1.3.0/bigframes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.2.0
+Version: 1.3.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: fsspec>=2023.3.0
 Requires-Dist: gcsfs>=2023.3.0
 Requires-Dist: geopandas>=0.12.2
 Requires-Dist: google-auth<3.0dev,>=2.15.0
-Requires-Dist: google-cloud-bigquery[bqstorage,pandas]>=3.10.0
+Requires-Dist: google-cloud-bigquery[bqstorage,pandas]>=3.16.0
 Requires-Dist: google-cloud-functions>=1.12.0
 Requires-Dist: google-cloud-bigquery-connection>=1.12.0
 Requires-Dist: google-cloud-iam>=2.12.1
 Requires-Dist: google-cloud-resource-manager>=1.10.3
 Requires-Dist: google-cloud-storage>=2.0.0
 Requires-Dist: ibis-framework[bigquery]<9.0.0dev,>=8.0.0
 Requires-Dist: pandas>=1.5.0
```

### Comparing `bigframes-1.2.0/bigframes.egg-info/SOURCES.txt` & `bigframes-1.3.0/bigframes.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 bigframes/__init__.py
 bigframes/clients.py
 bigframes/constants.py
 bigframes/dataframe.py
 bigframes/dtypes.py
+bigframes/exceptions.py
 bigframes/features.py
 bigframes/formatting_helpers.py
 bigframes/py.typed
 bigframes/series.py
 bigframes/typing.py
 bigframes/version.py
 bigframes.egg-info/PKG-INFO
@@ -131,14 +132,15 @@
 tests/system/large/ml/test_core.py
 tests/system/large/ml/test_decomposition.py
 tests/system/large/ml/test_ensemble.py
 tests/system/large/ml/test_forecasting.py
 tests/system/large/ml/test_linear_model.py
 tests/system/large/ml/test_pipeline.py
 tests/system/load/test_large_tables.py
+tests/system/load/test_llm.py
 tests/system/small/__init__.py
 tests/system/small/test_dataframe.py
 tests/system/small/test_dataframe_io.py
 tests/system/small/test_encryption.py
 tests/system/small/test_groupby.py
 tests/system/small/test_ibis.py
 tests/system/small/test_index.py
```

### Comparing `bigframes-1.2.0/bigframes.egg-info/requires.txt` & `bigframes-1.3.0/bigframes.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cloudpickle>=2.0.0
 fsspec>=2023.3.0
 gcsfs>=2023.3.0
 geopandas>=0.12.2
 google-auth<3.0dev,>=2.15.0
-google-cloud-bigquery[bqstorage,pandas]>=3.10.0
+google-cloud-bigquery[bqstorage,pandas]>=3.16.0
 google-cloud-functions>=1.12.0
 google-cloud-bigquery-connection>=1.12.0
 google-cloud-iam>=2.12.1
 google-cloud-resource-manager>=1.10.3
 google-cloud-storage>=2.0.0
 ibis-framework[bigquery]<9.0.0dev,>=8.0.0
 pandas>=1.5.0
```

### Comparing `bigframes-1.2.0/setup.py` & `bigframes-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 dependencies = [
     # please keep these in sync with the minimum versions in testing/constraints-3.9.txt
     "cloudpickle >= 2.0.0",
     "fsspec >=2023.3.0",
     "gcsfs >=2023.3.0",
     "geopandas >=0.12.2",
     "google-auth >=2.15.0,<3.0dev",
-    "google-cloud-bigquery[bqstorage,pandas] >=3.10.0",
+    "google-cloud-bigquery[bqstorage,pandas] >=3.16.0",
     "google-cloud-functions >=1.12.0",
     "google-cloud-bigquery-connection >=1.12.0",
     "google-cloud-iam >=2.12.1",
     "google-cloud-resource-manager >=1.10.3",
     "google-cloud-storage >=2.0.0",
     "ibis-framework[bigquery] >=8.0.0,<9.0.0dev",
     # TODO: Relax upper bound once we have fixed `system_prerelease` tests.
```

### Comparing `bigframes-1.2.0/tests/__init__.py` & `bigframes-1.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/hockey_players.json` & `bigframes-1.3.0/tests/data/hockey_players.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/hockey_players.jsonl` & `bigframes-1.3.0/tests/data/hockey_players.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/nested.jsonl` & `bigframes-1.3.0/tests/data/nested.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/nested_schema.json` & `bigframes-1.3.0/tests/data/nested_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/penguins.jsonl` & `bigframes-1.3.0/tests/data/penguins.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/penguins_schema.json` & `bigframes-1.3.0/tests/data/penguins_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/scalars.jsonl` & `bigframes-1.3.0/tests/data/scalars.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/scalars_schema.json` & `bigframes-1.3.0/tests/data/scalars_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/data/time_series.jsonl` & `bigframes-1.3.0/tests/data/time_series.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/__init__.py` & `bigframes-1.3.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/conftest.py` & `bigframes-1.3.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/__init__.py` & `bigframes-1.3.0/tests/system/large/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_cluster.py` & `bigframes-1.3.0/tests/system/large/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_compose.py` & `bigframes-1.3.0/tests/system/large/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_core.py` & `bigframes-1.3.0/tests/system/large/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_decomposition.py` & `bigframes-1.3.0/tests/system/large/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_ensemble.py` & `bigframes-1.3.0/tests/system/large/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_forecasting.py` & `bigframes-1.3.0/tests/system/large/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_linear_model.py` & `bigframes-1.3.0/tests/system/large/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/ml/test_pipeline.py` & `bigframes-1.3.0/tests/system/large/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/test_location.py` & `bigframes-1.3.0/tests/system/large/test_location.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/large/test_remote_function.py` & `bigframes-1.3.0/tests/system/large/test_remote_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1296,7 +1296,43 @@
         assert blob.kms_key_name.startswith(cmek)
 
     finally:
         # clean up the gcp assets created for the remote function
         cleanup_remote_function_assets(
             session.bqclient, session.cloudfunctionsclient, square_num
         )
+
+
+@pytest.mark.parametrize(
+    ("max_batching_rows"),
+    [
+        10_000,
+        None,
+    ],
+)
+@pytest.mark.flaky(retries=2, delay=120)
+def test_remote_function_max_batching_rows(session, scalars_dfs, max_batching_rows):
+    try:
+
+        def square(x):
+            return x * x
+
+        square_remote = session.remote_function(
+            [int], int, reuse=False, max_batching_rows=max_batching_rows
+        )(square)
+
+        bq_routine = session.bqclient.get_routine(
+            square_remote.bigframes_remote_function
+        )
+        assert bq_routine.remote_function_options.max_batching_rows == max_batching_rows
+
+        scalars_df, scalars_pandas_df = scalars_dfs
+
+        bf_result = scalars_df["int64_too"].apply(square_remote).to_pandas()
+        pd_result = scalars_pandas_df["int64_too"].apply(square)
+
+        pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
+    finally:
+        # clean up the gcp assets created for the remote function
+        cleanup_remote_function_assets(
+            session.bqclient, session.cloudfunctionsclient, square_remote
+        )
```

### Comparing `bigframes-1.2.0/tests/system/large/test_session.py` & `bigframes-1.3.0/tests/system/large/test_session.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/load/test_large_tables.py` & `bigframes-1.3.0/tests/system/load/test_large_tables.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/__init__.py` & `bigframes-1.3.0/tests/system/small/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/__init__.py` & `bigframes-1.3.0/tests/system/small/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/conftest.py` & `bigframes-1.3.0/tests/system/small/ml/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_cluster.py` & `bigframes-1.3.0/tests/system/small/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_core.py` & `bigframes-1.3.0/tests/system/small/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_decomposition.py` & `bigframes-1.3.0/tests/system/small/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_ensemble.py` & `bigframes-1.3.0/tests/system/small/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_forecasting.py` & `bigframes-1.3.0/tests/system/small/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_imported.py` & `bigframes-1.3.0/tests/system/small/ml/test_imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_linear_model.py` & `bigframes-1.3.0/tests/system/small/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_llm.py` & `bigframes-1.3.0/tests/system/small/ml/test_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_metrics.py` & `bigframes-1.3.0/tests/system/small/ml/test_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_metrics_pairwise.py` & `bigframes-1.3.0/tests/system/small/ml/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_model_selection.py` & `bigframes-1.3.0/tests/system/small/ml/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_preprocessing.py` & `bigframes-1.3.0/tests/system/small/ml/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_register.py` & `bigframes-1.3.0/tests/system/small/ml/test_register.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/ml/test_remote.py` & `bigframes-1.3.0/tests/system/small/ml/test_remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/operations/__init__.py` & `bigframes-1.3.0/tests/system/small/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/operations/test_datetimes.py` & `bigframes-1.3.0/tests/system/small/operations/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/operations/test_plotting.py` & `bigframes-1.3.0/tests/system/small/operations/test_plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/operations/test_strings.py` & `bigframes-1.3.0/tests/system/small/operations/test_strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/regression/test_issue355_merge_after_filter.py` & `bigframes-1.3.0/tests/system/small/regression/test_issue355_merge_after_filter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_dataframe.py` & `bigframes-1.3.0/tests/system/small/test_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -2500,15 +2500,18 @@
     columns = ["int64_col", "int64_too", "rowindex_2"]
 
     bf_result = scalars_df[columns].melt().to_pandas()
     pd_result = scalars_pandas_df[columns].melt()
 
     # Pandas produces int64 index, Bigframes produces Int64 (nullable)
     pd.testing.assert_frame_equal(
-        bf_result, pd_result, check_index_type=False, check_dtype=False
+        bf_result,
+        pd_result,
+        check_index_type=False,
+        check_dtype=False,
     )
 
 
 def test_df_melt_parameterized(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     # To match bigquery dataframes
     scalars_pandas_df = scalars_pandas_df.copy()
@@ -2980,18 +2983,22 @@
 def test_dataframe_aggregates(scalars_df_index, scalars_pandas_df_index, op, ordered):
     col_names = ["int64_too", "float64_col", "string_col", "int64_col", "bool_col"]
     bf_series = op(scalars_df_index[col_names])
     pd_series = op(scalars_pandas_df_index[col_names])
     bf_result = bf_series.to_pandas(ordered=ordered)
 
     # Pandas may produce narrower numeric types, but bigframes always produces Float64
-    pd_series = pd_series.astype("Float64")
     # Pandas has object index type
+    pd_series.index = pd_series.index.astype(pd.StringDtype(storage="pyarrow"))
     assert_series_equal(
-        pd_series, bf_result, check_index_type=False, ignore_order=not ordered
+        pd_series,
+        bf_result,
+        check_index_type=False,
+        ignore_order=not ordered,
+        check_dtype=False,
     )
 
 
 @pytest.mark.parametrize(
     ("op"),
     [
         (lambda x: x.sum(axis=1, numeric_only=True)),
@@ -3025,14 +3032,39 @@
     # Median is an approximation, but double-check that median is plausible.
     for col in col_names:
         assert (pd_result.loc["min", col] <= bf_result[col]) and (
             bf_result[col] <= pd_result.loc["max", col]
         )
 
 
+def test_dataframe_aggregates_quantile_mono(scalars_df_index, scalars_pandas_df_index):
+    q = 0.45
+    col_names = ["int64_too", "int64_col", "float64_col"]
+    bf_result = scalars_df_index[col_names].quantile(q=q).to_pandas()
+    pd_result = scalars_pandas_df_index[col_names].quantile(q=q)
+
+    # Pandas may produce narrower numeric types, but bigframes always produces Float64
+    pd_result = pd_result.astype("Float64")
+
+    pd.testing.assert_series_equal(bf_result, pd_result, check_index_type=False)
+
+
+def test_dataframe_aggregates_quantile_multi(scalars_df_index, scalars_pandas_df_index):
+    q = [0, 0.33, 0.67, 1.0]
+    col_names = ["int64_too", "int64_col", "float64_col"]
+    bf_result = scalars_df_index[col_names].quantile(q=q).to_pandas()
+    pd_result = scalars_pandas_df_index[col_names].quantile(q=q)
+
+    # Pandas may produce narrower numeric types, but bigframes always produces Float64
+    pd_result = pd_result.astype("Float64")
+    pd_result.index = pd_result.index.astype("Float64")
+
+    pd.testing.assert_frame_equal(bf_result, pd_result)
+
+
 @pytest.mark.parametrize(
     ("op"),
     [
         (lambda x: x.all(bool_only=True)),
         (lambda x: x.any(bool_only=True)),
         (lambda x: x.all(axis=1, bool_only=True)),
         (lambda x: x.any(axis=1, bool_only=True)),
@@ -3047,15 +3079,15 @@
     scalars_pandas_df_index = scalars_pandas_df_index.assign(
         bool_col=scalars_pandas_df_index.bool_col.fillna(False).astype("bool")
     )
     bf_series = op(scalars_df_index)
     pd_series = op(scalars_pandas_df_index).astype("boolean")
     bf_result = bf_series.to_pandas()
 
-    # Pandas has object index type
+    pd_series.index = pd_series.index.astype(bf_result.index.dtype)
     pd.testing.assert_series_equal(pd_series, bf_result, check_index_type=False)
 
 
 def test_dataframe_prod(scalars_df_index, scalars_pandas_df_index):
     col_names = ["int64_too", "float64_col"]
     bf_series = scalars_df_index[col_names].prod()
     pd_series = scalars_pandas_df_index[col_names].prod()
```

### Comparing `bigframes-1.2.0/tests/system/small/test_dataframe_io.py` & `bigframes-1.3.0/tests/system/small/test_dataframe_io.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_encryption.py` & `bigframes-1.3.0/tests/system/small/test_encryption.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_groupby.py` & `bigframes-1.3.0/tests/system/small/test_groupby.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,32 @@
     )
     bf_result_computed = bf_result.to_pandas()
     # Median is approximate. Just check for plausibility.
     assert ((pd_min <= bf_result_computed) & (bf_result_computed <= pd_max)).all().all()
 
 
 @pytest.mark.parametrize(
+    ("q"),
+    [
+        ([0.2, 0.4, 0.6, 0.8]),
+        (0.11),
+    ],
+)
+def test_dataframe_groupby_quantile(scalars_df_index, scalars_pandas_df_index, q):
+    col_names = ["int64_too", "float64_col", "int64_col", "string_col"]
+    bf_result = (
+        scalars_df_index[col_names].groupby("string_col").quantile(q)
+    ).to_pandas()
+    pd_result = scalars_pandas_df_index[col_names].groupby("string_col").quantile(q)
+    pd.testing.assert_frame_equal(
+        pd_result, bf_result, check_dtype=False, check_index_type=False
+    )
+
+
+@pytest.mark.parametrize(
     ("operator"),
     [
         (lambda x: x.count()),
         (lambda x: x.nunique()),
         (lambda x: x.any()),
         (lambda x: x.all()),
     ],
@@ -385,7 +403,24 @@
     )
     pd_result = df.groupby(["key1", "key2"]).mean()
     bf_result = bpd.DataFrame(df).groupby(["key1", "key2"]).mean().to_pandas()
 
     pd.testing.assert_frame_equal(
         pd_result, bf_result, check_index_type=False, check_dtype=False
     )
+
+
+@pytest.mark.parametrize(
+    ("q"),
+    [
+        ([0.2, 0.4, 0.6, 0.8]),
+        (0.11),
+    ],
+)
+def test_series_groupby_quantile(scalars_df_index, scalars_pandas_df_index, q):
+    bf_result = (
+        scalars_df_index.groupby("string_col")["int64_col"].quantile(q)
+    ).to_pandas()
+    pd_result = scalars_pandas_df_index.groupby("string_col")["int64_col"].quantile(q)
+    pd.testing.assert_series_equal(
+        pd_result, bf_result, check_dtype=False, check_index_type=False
+    )
```

### Comparing `bigframes-1.2.0/tests/system/small/test_ibis.py` & `bigframes-1.3.0/tests/system/small/test_ibis.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_index.py` & `bigframes-1.3.0/tests/system/small/test_index.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_ipython.py` & `bigframes-1.3.0/tests/system/small/test_ipython.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_multiindex.py` & `bigframes-1.3.0/tests/system/small/test_multiindex.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_numpy.py` & `bigframes-1.3.0/tests/system/small/test_numpy.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_pandas.py` & `bigframes-1.3.0/tests/system/small/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_pandas_options.py` & `bigframes-1.3.0/tests/system/small/test_pandas_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_progress_bar.py` & `bigframes-1.3.0/tests/system/small/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_remote_function.py` & `bigframes-1.3.0/tests/system/small/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_scalar.py` & `bigframes-1.3.0/tests/system/small/test_scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/small/test_series.py` & `bigframes-1.3.0/tests/system/small/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1316,22 +1316,42 @@
     bf_result = scalars_df[col_name].median()
     pd_max = scalars_pandas_df[col_name].max()
     pd_min = scalars_pandas_df[col_name].min()
     # Median is approximate, so just check for plausibility.
     assert pd_min < bf_result < pd_max
 
 
+def test_median_exact(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    col_name = "int64_col"
+    bf_result = scalars_df[col_name].median(exact=True)
+    pd_result = scalars_pandas_df[col_name].median()
+    assert math.isclose(pd_result, bf_result)
+
+
+def test_series_quantile(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    col_name = "int64_col"
+    bf_series = scalars_df[col_name]
+    pd_series = scalars_pandas_df[col_name]
+
+    pd_result = pd_series.quantile([0.0, 0.4, 0.6, 1.0])
+    bf_result = bf_series.quantile([0.0, 0.4, 0.6, 1.0])
+    pd.testing.assert_series_equal(
+        pd_result, bf_result.to_pandas(), check_dtype=False, check_index_type=False
+    )
+
+
 def test_numeric_literal(scalars_dfs):
     scalars_df, _ = scalars_dfs
     col_name = "numeric_col"
     assert scalars_df[col_name].dtype == pd.ArrowDtype(pa.decimal128(38, 9))
-    bf_result = scalars_df[col_name] - scalars_df[col_name].median()
+    bf_result = scalars_df[col_name] + 42
     assert bf_result.size == scalars_df[col_name].size
-    # TODO(b/323387826): The precision increased by 1 unexpectedly.
-    # assert bf_result.dtype == pd.ArrowDtype(pa.decimal128(38, 9))
+    assert bf_result.dtype == pd.ArrowDtype(pa.decimal128(38, 9))
 
 
 def test_repr(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
 
     col_name = "int64_col"
     bf_series = scalars_df[col_name]
@@ -1498,20 +1518,40 @@
     bf_result = bf_series.to_pandas()
     assert_series_equal(
         pd_series,
         bf_result,
     )
 
 
-def test_groupby_median(scalars_dfs):
+def test_groupby_median_exact(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "int64_too"
-    bf_series = (
+    bf_result = (
         scalars_df[col_name].groupby(scalars_df["string_col"], dropna=False).median()
     )
+    pd_result = (
+        scalars_pandas_df[col_name]
+        .groupby(scalars_pandas_df["string_col"], dropna=False)
+        .median()
+    )
+
+    assert_series_equal(
+        pd_result,
+        bf_result.to_pandas(),
+    )
+
+
+def test_groupby_median_inexact(scalars_dfs):
+    scalars_df, scalars_pandas_df = scalars_dfs
+    col_name = "int64_too"
+    bf_series = (
+        scalars_df[col_name]
+        .groupby(scalars_df["string_col"], dropna=False)
+        .median(exact=False)
+    )
     pd_max = (
         scalars_pandas_df[col_name]
         .groupby(scalars_pandas_df["string_col"], dropna=False)
         .max()
     )
     pd_min = (
         scalars_pandas_df[col_name]
```

### Comparing `bigframes-1.2.0/tests/system/small/test_session.py` & `bigframes-1.3.0/tests/system/small/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,22 +232,21 @@
     expected.index = expected.index.astype(result.index.dtype)
     pd.testing.assert_frame_equal(result, expected, check_dtype=False)
 
 
 def test_read_gbq_w_primary_keys_table(
     session: bigframes.Session, usa_names_grouped_table: bigquery.Table
 ):
+    # Validate that the table we're querying has a primary key.
     table = usa_names_grouped_table
-    # TODO(b/305264153): Use public properties to fetch primary keys once
-    # added to google-cloud-bigquery.
-    primary_keys = (
-        table._properties.get("tableConstraints", {})
-        .get("primaryKey", {})
-        .get("columns")
-    )
+    table_constraints = table.table_constraints
+    assert table_constraints is not None
+    primary_key = table_constraints.primary_key
+    assert primary_key is not None
+    primary_keys = primary_key.columns
     assert len(primary_keys) != 0
 
     df = session.read_gbq(f"{table.project}.{table.dataset_id}.{table.table_id}")
     result = df.head(100).to_pandas()
 
     # Verify that the DataFrame is already sorted by primary keys.
     sorted_result = result.sort_values(primary_keys)
```

### Comparing `bigframes-1.2.0/tests/system/small/test_window.py` & `bigframes-1.3.0/tests/system/small/test_window.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/system/utils.py` & `bigframes-1.3.0/tests/system/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/__init__.py` & `bigframes-1.3.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/_config/__init__.py` & `bigframes-1.3.0/tests/unit/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/_config/test_bigquery_options.py` & `bigframes-1.3.0/tests/unit/_config/test_bigquery_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
+import warnings
 
 import pytest
 
+import bigframes
 import bigframes._config.bigquery_options as bigquery_options
+import bigframes.exceptions
 
 
 @pytest.mark.parametrize(
     ["attribute", "original_value", "new_value"],
     [
         ("application_name", None, "test-partner"),
         # For credentials, the match is by reference.
@@ -74,7 +77,55 @@
     assert getattr(options, attribute) is original_object
 
     # This should work fine since we're setting the same value as before.
     options._session_started = True
     setattr(options, attribute, original_object)
 
     assert getattr(options, attribute) is original_object
+
+
+@pytest.mark.parametrize(
+    [
+        "valid_location",
+    ],
+    [
+        (None,),
+        ("us-central1",),
+    ],
+)
+def test_location_set_to_valid_no_warning(valid_location):
+    options = bigquery_options.BigQueryOptions()
+    # Ensure that no warnings are emitted.
+    # https://docs.pytest.org/en/7.0.x/how-to/capture-warnings.html#additional-use-cases-of-warnings-in-tests
+    with warnings.catch_warnings():
+        # Turn matching UnknownLocationWarning into exceptions.
+        # https://docs.python.org/3/library/warnings.html#warning-filter
+        warnings.simplefilter(
+            "error", category=bigframes.exceptions.UnknownLocationWarning
+        )
+        options.location = valid_location
+
+
+@pytest.mark.parametrize(
+    [
+        "invalid_location",
+    ],
+    [
+        # Test with common mistakes, see article.
+        # https://en.wikipedia.org/wiki/Edit_distance#Formal_definition_and_properties
+        # Substitution
+        ("us-wist-3",),
+        # Insertion
+        ("us-central-1",),
+        # Deletion
+        ("asia-suth2",),
+    ],
+)
+def test_location_set_to_invalid_warning(invalid_location):
+    options = bigquery_options.BigQueryOptions()
+    with pytest.warns(
+        bigframes.exceptions.UnknownLocationWarning,
+        match=re.escape(
+            f"The location '{invalid_location}' is set to an unknown value."
+        ),
+    ):
+        options.location = invalid_location
```

### Comparing `bigframes-1.2.0/tests/unit/core/__init__.py` & `bigframes-1.3.0/tests/unit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/core/test_bf_utils.py` & `bigframes-1.3.0/tests/unit/core/test_bf_utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/core/test_blocks.py` & `bigframes-1.3.0/tests/unit/core/test_blocks.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/core/test_expression.py` & `bigframes-1.3.0/tests/unit/core/test_expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/core/test_log_adapter.py` & `bigframes-1.3.0/tests/unit/core/test_log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/__init__.py` & `bigframes-1.3.0/tests/unit/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/test_api_primitives.py` & `bigframes-1.3.0/tests/unit/ml/test_api_primitives.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/test_compose.py` & `bigframes-1.3.0/tests/unit/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/test_golden_sql.py` & `bigframes-1.3.0/tests/unit/ml/test_golden_sql.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/test_pipeline.py` & `bigframes-1.3.0/tests/unit/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/ml/test_sql.py` & `bigframes-1.3.0/tests/unit/ml/test_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,37 @@
 OPTIONS(
   option_key1="option_value1",
   option_key2=2)
 AS input_X_y_sql"""
     )
 
 
+def test_create_llm_remote_model_correct(
+    model_creation_sql_generator: ml_sql.ModelCreationSqlGenerator,
+    mock_df: bpd.DataFrame,
+):
+    sql = model_creation_sql_generator.create_llm_remote_model(
+        source_df=mock_df,
+        connection_name="my_project.us.my_connection",
+        model_ref=bigquery.ModelReference.from_string(
+            "test-proj._anonXYZ.create_remote_model"
+        ),
+        options={"option_key1": "option_value1", "option_key2": 2},
+    )
+    assert (
+        sql
+        == """CREATE OR REPLACE MODEL `test-proj`.`_anonXYZ`.`create_remote_model`
+REMOTE WITH CONNECTION `my_project.us.my_connection`
+OPTIONS(
+  option_key1="option_value1",
+  option_key2=2)
+AS input_X_y_sql"""
+    )
+
+
 def test_create_remote_model_correct(
     model_creation_sql_generator: ml_sql.ModelCreationSqlGenerator,
 ):
     sql = model_creation_sql_generator.create_remote_model(
         connection_name="my_project.us.my_connection",
         model_ref=bigquery.ModelReference.from_string(
             "test-proj._anonXYZ.create_remote_model"
```

### Comparing `bigframes-1.2.0/tests/unit/resources.py` & `bigframes-1.3.0/tests/unit/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Sequence
 import unittest.mock as mock
 
 import google.auth.credentials
 import google.cloud.bigquery
 import ibis
 import pandas
 import pytest
@@ -33,29 +33,30 @@
 
 TEST_SCHEMA = (google.cloud.bigquery.SchemaField("col", "INTEGER"),)
 
 
 def create_bigquery_session(
     bqclient: Optional[mock.Mock] = None,
     session_id: str = "abcxyz",
+    table_schema: Sequence[google.cloud.bigquery.SchemaField] = TEST_SCHEMA,
     anonymous_dataset: Optional[google.cloud.bigquery.DatasetReference] = None,
 ) -> bigframes.Session:
     credentials = mock.create_autospec(
         google.auth.credentials.Credentials, instance=True
     )
 
     if bqclient is None:
         bqclient = mock.create_autospec(google.cloud.bigquery.Client, instance=True)
         bqclient.project = "test-project"
 
         # Mock the location.
         table = mock.create_autospec(google.cloud.bigquery.Table, instance=True)
         table._properties = {}
         type(table).location = mock.PropertyMock(return_value="test-region")
-        type(table).schema = mock.PropertyMock(return_value=TEST_SCHEMA)
+        type(table).schema = mock.PropertyMock(return_value=table_schema)
         bqclient.get_table.return_value = table
 
     if anonymous_dataset is None:
         anonymous_dataset = google.cloud.bigquery.DatasetReference(
             "test-project",
             "test_dataset",
         )
@@ -68,15 +69,15 @@
         type(query_job).session_info = google.cloud.bigquery.SessionInfo(
             {"sessionInfo": {"sessionId": session_id}},
         )
 
         if query.startswith("SELECT CURRENT_TIMESTAMP()"):
             query_job.result = mock.MagicMock(return_value=[[datetime.datetime.now()]])
         else:
-            type(query_job).schema = mock.PropertyMock(return_value=TEST_SCHEMA)
+            type(query_job).schema = mock.PropertyMock(return_value=table_schema)
 
         return query_job
 
     bqclient.query = query_mock
 
     clients_provider = mock.create_autospec(bigframes.session.clients.ClientsProvider)
     type(clients_provider).bqclient = mock.PropertyMock(return_value=bqclient)
```

### Comparing `bigframes-1.2.0/tests/unit/session/__init__.py` & `bigframes-1.3.0/tests/unit/session/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/session/test_clients.py` & `bigframes-1.3.0/tests/unit/session/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/session/test_io_bigquery.py` & `bigframes-1.3.0/tests/unit/session/test_io_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/session/test_io_pandas.py` & `bigframes-1.3.0/tests/unit/session/test_io_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_clients.py` & `bigframes-1.3.0/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_compute_options.py` & `bigframes-1.3.0/tests/unit/test_compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_core.py` & `bigframes-1.3.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_dataframe.py` & `bigframes-1.3.0/tests/unit/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_dtypes.py` & `bigframes-1.3.0/tests/unit/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_features.py` & `bigframes-1.3.0/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_formatting_helper.py` & `bigframes-1.3.0/tests/unit/test_formatting_helper.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_formatting_helpers.py` & `bigframes-1.3.0/tests/unit/test_formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_pandas.py` & `bigframes-1.3.0/tests/unit/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/tests/unit/test_remote_function.py` & `bigframes-1.3.0/tests/unit/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/cpython/LICENSE` & `bigframes-1.3.0/third_party/bigframes_vendored/cpython/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/cpython/_pprint.py` & `bigframes-1.3.0/third_party/bigframes_vendored/cpython/_pprint.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py` & `bigframes-1.3.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/LICENSE.txt` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/README.md` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Contains code from https://github.com/ibis-project/ibis/blob/master/ibis/backends/bigquery/registry.py
 """Module to convert from Ibis expression to SQL string."""
 
 import bigframes_vendored.ibis.expr.operations as vendored_ibis_ops
 from ibis.backends.bigquery.registry import OPERATION_REGISTRY
+import ibis.expr.operations.reductions as ibis_reductions
 
 
 def _approx_quantiles(translator, op: vendored_ibis_ops.ApproximateMultiQuantile):
     arg = translator.translate(op.arg)
     num_bins = translator.translate(op.num_bins)
     return f"APPROX_QUANTILES({arg}, {num_bins})"
 
@@ -27,16 +28,23 @@
 
 
 def _generate_array(translator, op: vendored_ibis_ops.GenerateArray):
     arg = translator.translate(op.arg)
     return f"GENERATE_ARRAY(0, {arg})"
 
 
+def _quantile(translator, op: ibis_reductions.Quantile):
+    arg = translator.translate(op.arg)
+    quantile = translator.translate(op.quantile)
+    return f"PERCENTILE_CONT({arg}, {quantile})"
+
+
 patched_ops = {
     vendored_ibis_ops.ApproximateMultiQuantile: _approx_quantiles,  # type:ignore
     vendored_ibis_ops.FirstNonNullValue: _first_non_null_value,  # type:ignore
     vendored_ibis_ops.LastNonNullValue: _last_non_null_value,  # type:ignore
     vendored_ibis_ops.ToJsonString: _to_json_string,  # type:ignore
     vendored_ibis_ops.GenerateArray: _generate_array,  # type:ignore
+    ibis_reductions.Quantile: _quantile,  # type:ignore
 }
 
 OPERATION_REGISTRY.update(patched_ops)
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py` & `bigframes-1.3.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/AUTHORS.md` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/LICENSE` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/README.md` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/_config/config.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/_config/config.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py`

 * *Files 26% similar despite different names*

```diff
@@ -88,7 +88,36 @@
             [3 rows x 2 columns]
 
         Returns:
             DataFrame:
                 The data corresponding to all child fields.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
+    def dtypes(self):
+        """
+        Return the dtype object of each child field of the struct.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> import pyarrow as pa
+            >>> bpd.options.display.progress_bar = None
+            >>> s = bpd.Series(
+            ...     [
+            ...         {"version": 1, "project": "pandas"},
+            ...         {"version": 2, "project": "pandas"},
+            ...         {"version": 1, "project": "numpy"},
+            ...     ],
+            ...     dtype=bpd.ArrowDtype(pa.struct(
+            ...         [("version", pa.int64()), ("project", pa.string())]
+            ...     ))
+            ... )
+            >>> s.struct.dtypes()
+            version              Int64
+            project    string[pyarrow]
+            dtype: object
+
+        Returns:
+            A *pandas* Series with the data type of all child fields.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/common.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/align.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/align.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/common.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/engines.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/engines.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/eval.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/expr.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/expr.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/ops.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/ops.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/computation/scope.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/computation/scope.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/config_init.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/config_init.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/frame.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -4323,24 +4323,24 @@
             1	3	4
             <BLANKLINE>
             [2 rows x 2 columns]
 
         Finding the minimum value in each column (the default behavior without an explicit axis parameter).
 
             >>> df.min()
-            A    1.0
-            B    2.0
-            dtype: Float64
+            A    1
+            B    2
+            dtype: Int64
 
         Finding the minimum value in each row.
 
             >>> df.min(axis=1)
-            0    1.0
-            1    3.0
-            dtype: Float64
+            0    1
+            1    3
+            dtype: Int64
 
         Args:
             axis ({index (0), columns (1)}):
                 Axis for the function to be applied on.
                 For Series this parameter is unused and defaults to 0.
             numeric_only (bool, default False):
                 Default False. Include only float, int, boolean columns.
@@ -4368,24 +4368,24 @@
             1	3	4
             <BLANKLINE>
             [2 rows x 2 columns]
 
         Finding the maximum value in each column (the default behavior without an explicit axis parameter).
 
             >>> df.max()
-            A    3.0
-            B    4.0
-            dtype: Float64
+            A    3
+            B    4
+            dtype: Int64
 
         Finding the maximum value in each row.
 
             >>> df.max(axis=1)
-            0    2.0
-            1    4.0
-            dtype: Float64
+            0    2
+            1    4
+            dtype: Int64
 
         Args:
             axis ({index (0), columns (1)}):
                 Axis for the function to be applied on.
                 For Series this parameter is unused and defaults to 0.
             numeric_only (bool. default False):
                 Default False. Include only float, int, boolean columns.
@@ -4412,24 +4412,24 @@
             1	3	4
             <BLANKLINE>
             [2 rows x 2 columns]
 
         Calculating the sum of each column (the default behavior without an explicit axis parameter).
 
             >>> df.sum()
-            A    4.0
-            B    6.0
-            dtype: Float64
+            A    4
+            B    6
+            dtype: Int64
 
         Calculating the sum of each row.
 
             >>> df.sum(axis=1)
-            0    3.0
-            1    7.0
-            dtype: Float64
+            0    3
+            1    7
+            dtype: Int64
 
         Args:
             axis ({index (0), columns (1)}):
                 Axis for the function to be applied on.
                 For Series this parameter is unused and defaults to 0.
             numeric_only (bool. default False):
                 Default False. Include only float, int, boolean columns.
@@ -4477,15 +4477,15 @@
                 Default False. Include only float, int, boolean columns.
 
         Returns:
             bigframes.series.Series: Series with the mean of values.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
-    def median(self, *, numeric_only: bool = False, exact: bool = False):
+    def median(self, *, numeric_only: bool = False, exact: bool = True):
         """Return the median of the values over colunms.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
@@ -4496,30 +4496,69 @@
             1	3	4
             <BLANKLINE>
             [2 rows x 2 columns]
 
         Finding the median value of each column.
 
             >>> df.median()
-            A    1.0
-            B    2.0
+            A    2.0
+            B    3.0
             dtype: Float64
 
         Args:
             numeric_only (bool. default False):
                 Default False. Include only float, int, boolean columns.
-            exact (bool. default False):
-                Default False. Get the exact median instead of an approximate
-                one. Note: ``exact=True`` not yet supported.
+            exact (bool. default True):
+                Default True. Get the exact median instead of an approximate
+                one.
 
         Returns:
             bigframes.series.Series: Series with the median of values.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def quantile(
+        self, q: Union[float, Sequence[float]] = 0.5, *, numeric_only: bool = False
+    ):
+        """
+        Return values at the given quantile over requested axis.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> df = bpd.DataFrame(np.array([[1, 1], [2, 10], [3, 100], [4, 100]]),
+            ...                   columns=['a', 'b'])
+            >>> df.quantile(.1)
+            a    1.3
+            b    3.7
+            Name: 0.1, dtype: Float64
+            >>> df.quantile([.1, .5])
+                   a     b
+            0.1  1.3   3.7
+            0.5  2.5  55.0
+            <BLANKLINE>
+            [2 rows x 2 columns]
+
+        Args:
+            q (float or array-like, default 0.5 (50% quantile)):
+                Value between 0 <= q <= 1, the quantile(s) to compute.
+            numeric_only (bool, default False):
+                Include only `float`, `int` or `boolean` data.
+
+        Returns:
+            Series or DataFrame:
+                If ``q`` is an array, a DataFrame will be returned where the
+                index is ``q``, the columns are the columns of self, and the
+                values are the quantiles.
+                If ``q`` is a float, a Series will be returned where the
+                index is the columns of self and the values are the quantiles.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def var(self, axis=0, *, numeric_only: bool = False):
         """Return unbiased variance over requested axis.
 
         Normalized by N-1 by default.
 
         **Examples:**
 
@@ -4706,18 +4745,18 @@
             4	 5.0	5	 5.0
             <BLANKLINE>
             [5 rows x 3 columns]
 
         Counting non-NA values for each column:
 
             >>> df.count()
-            A    4.0
-            B    5.0
-            C    3.0
-            dtype: Float64
+            A    4
+            B    5
+            C    3
+            dtype: Int64
 
         Args:
             numeric_only (bool, default False):
                 Include only `float`, `int` or `boolean` data.
 
         Returns:
             bigframes.series.Series: For each column/row the number of
@@ -5009,25 +5048,25 @@
             14	       C      5.0
             <BLANKLINE>
             [15 rows x 2 columns]
 
         Using `melt` with `id_vars` and `value_vars`:
 
             >>> df.melt(id_vars='A', value_vars=['B', 'C'])
-                   A	variable	value
-            0	 1.0	       B	    1
-            1	<NA>	       B	    2
-            2	 3.0	       B	    3
-            3	 4.0	       B	    4
-            4	 5.0	       B	    5
-            5	 1.0	       C	 <NA>
-            6	 <NA>	       C	    3
-            7	 3.0	       C	 <NA>
-            8	 4.0	       C	    4
-            9	 5.0	       C	    5
+                  A variable  value
+            0   1.0        B    1.0
+            1  <NA>        B    2.0
+            2   3.0        B    3.0
+            3   4.0        B    4.0
+            4   5.0        B    5.0
+            5   1.0        C   <NA>
+            6  <NA>        C    3.5
+            7   3.0        C   <NA>
+            8   4.0        C    4.5
+            9   5.0        C    5.0
             <BLANKLINE>
             [10 rows x 3 columns]
 
 
         Args:
             id_vars (tuple, list, or ndarray, optional):
                 Column(s) to use as identifier variables.
@@ -5060,17 +5099,17 @@
             0	3	1
             1	1	2
             2	2	2
             <BLANKLINE>
             [3 rows x 2 columns]
 
             >>> df.nunique()
-            A    3.0
-            B    2.0
-            dtype: Float64
+            A    3
+            B    2
+            dtype: Int64
 
         Returns:
             bigframes.series.Series: Series with number of distinct elements.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def cummin(self) -> DataFrame:
@@ -5271,17 +5310,17 @@
             2	2	3
             <BLANKLINE>
             [3 rows x 2 columns]
 
         Using a single function:
 
             >>> df.agg('sum')
-            A    6.0
-            B    6.0
-            dtype: Float64
+            A    6
+            B    6
+            dtype: Int64
 
         Using a list of functions:
 
             >>> df.agg(['sum', 'mean'])
                       A	  B
             sum	    6.0	6.0
             mean	2.0	2.0
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/generic.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         """
         Iterate over column axis for DataFrame, or values for Series.
 
         Returns:
             iterator
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
             >>> df = bpd.DataFrame({
             ...     'A': [1, 2, 3],
             ...     'B': [4, 5, 6],
             ... })
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,31 +64,61 @@
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     def median(
         self,
         numeric_only: bool = False,
         *,
-        exact: bool = False,
+        exact: bool = True,
     ):
         """
         Compute median of groups, excluding missing values.
 
         Args:
             numeric_only (bool, default False):
                 Include only float, int, boolean columns.
-            exact (bool, default False):
-                Calculate the exact median instead of an approximation. Note:
-                    ``exact=True`` is not supported.
+            exact (bool, default True):
+                Calculate the exact median instead of an approximation.
 
         Returns:
             pandas.Series or pandas.DataFrame: Median of groups.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def quantile(self, q=0.5, *, numeric_only: bool = False):
+        """
+        Return group values at the given quantile, a la numpy.percentile.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> df = bpd.DataFrame([
+            ...     ['a', 1], ['a', 2], ['a', 3],
+            ...     ['b', 1], ['b', 3], ['b', 5]
+            ... ], columns=['key', 'val'])
+            >>> df.groupby('key').quantile()
+                 val
+            key
+            a    2.0
+            b    3.0
+            <BLANKLINE>
+            [2 rows x 1 columns]
+
+        Args:
+            q (float or array-like, default 0.5 (50% quantile)):
+                Value(s) between 0 and 1 providing the quantile(s) to compute.
+            numeric_only (bool, default False):
+                Include only `float`, `int` or `boolean` data.
+
+        Returns:
+            Series or DataFrame: Return type determined by caller of GroupBy object.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def std(
         self,
         *,
         numeric_only: bool = False,
     ):
         """
         Compute standard deviation of groups, excluding missing values.
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
     @property
     def dayofweek(self):
         """The day of the week with Monday=0, Sunday=6.
 
         Return the day of the week. It is assumed the week starts on
-        Monday, which is denoted by 0 and ends on Sunday which is denoted
+        Monday, which is denoted by 0 and ends on Sunday, which is denoted
         by 6.
 
         **Examples:**
 
             >>> import pandas as pd
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/base.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/indexing.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/indexing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/series.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 """
 Data structure for 1-dimensional cross-sectional and time series data
 """
 from __future__ import annotations
 
-from typing import Hashable, IO, Literal, Mapping, Optional, Sequence, TYPE_CHECKING
+from typing import (
+    Hashable,
+    IO,
+    Literal,
+    Mapping,
+    Optional,
+    Sequence,
+    TYPE_CHECKING,
+    Union,
+)
 
 from bigframes_vendored.pandas.core.generic import NDFrame
 import numpy
 import numpy as np
 from pandas._libs import lib
 from pandas._typing import Axis, FilePath, NaPosition, WriteBuffer
 
@@ -580,17 +589,17 @@
             3    4
             dtype: Int64
 
             >>> s.agg('min')
             1
 
             >>> s.agg(['min', 'max'])
-            min    1.0
-            max    4.0
-            dtype: Float64
+            min    1
+            max    4
+            dtype: Int64
 
         Args:
             func (function):
                 Function to use for aggregating the data.
                 Accepted combinations are: string function name, list of
                 function names, e.g. ``['sum', 'mean']``.
 
@@ -849,14 +858,15 @@
         """
         Compute the lag-N autocorrelation.
 
         This method computes the Pearson correlation between
         the Series and its shifted self.
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> bpd.options.display.progress_bar = None
 
             >>> s = bpd.Series([0.25, 0.5, 0.2, -0.05])
             >>> s.autocorr()  # doctest: +ELLIPSIS
             0.10355...
             >>> s.autocorr(lag=2)
@@ -2799,14 +2809,15 @@
         Update null elements with value in the same location in 'other'.
 
         Combine two Series objects by filling null values in one Series with
         non-null values from the other Series. Result index will be the union
         of the two indexes.
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> import numpy as np
             >>> bpd.options.display.progress_bar = None
 
             >>> s1 = bpd.Series([1, np.nan])
             >>> s2 = bpd.Series([3, 4, 5])
             >>> s1.combine_first(s2)
@@ -2839,14 +2850,15 @@
         """
         Modify Series in place using values from passed Series.
 
         Uses non-NA values from passed Series to make updates. Aligns
         on index.
 
         **Examples:**
+
             >>> import bigframes.pandas as bpd
             >>> import pandas as pd
             >>> import numpy as np
             >>> bpd.options.display.progress_bar = None
 
             >>> s = bpd.Series([1, 2, 3])
             >>> s.update(bpd.Series([4, 5, 6]))
@@ -3134,27 +3146,59 @@
             2.0
 
         Returns:
             scalar: Scalar.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
-    def median(self, *, exact: bool = False):
+    def median(self, *, exact: bool = True):
         """Return the median of the values over the requested axis.
 
         Args:
-            exact (bool. default False):
-                Default False. Get the exact median instead of an approximate
-                one. Note: ``exact=True`` not yet supported.
+            exact (bool. default True):
+                Default True. Get the exact median instead of an approximate
+                one.
 
         Returns:
             scalar: Scalar.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
+    def quantile(
+        self,
+        q: Union[float, Sequence[float]] = 0.5,
+    ) -> Union[Series, float]:
+        """
+        Return value at the given quantile.
+
+        **Examples:**
+
+            >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
+            >>> s = bpd.Series([1, 2, 3, 4])
+            >>> s.quantile(.5)
+            2.5
+            >>> s.quantile([.25, .5, .75])
+            0.25    1.75
+            0.5      2.5
+            0.75    3.25
+            dtype: Float64
+
+        Args:
+            q (float or array-like, default 0.5 (50% quantile)):
+                The quantile(s) to compute, which can lie in range: 0 <= q <= 1.
+
+        Returns:
+            float or Series:
+                If ``q`` is an array, a Series will be returned where the
+                index is ``q`` and the values are the quantiles, otherwise
+                a float will be returned.
+        """
+        raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
+
     def prod(self):
         """Return the product of the values over the requested axis.
 
         Returns:
             scalar: Scalar.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/core/window/rolling.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/common.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/gbq.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/gbq.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,21 +23,25 @@
         max_results: Optional[int] = None,
         filters: FiltersType = (),
         use_cache: Optional[bool] = None,
         col_order: Iterable[str] = (),
     ):
         """Loads a DataFrame from BigQuery.
 
-        BigQuery tables are an unordered, unindexed data source. By default,
-        the DataFrame will have an arbitrary index and ordering.
+        BigQuery tables are an unordered, unindexed data source. To add support
+        pandas-compatibility, the following indexing options are supported:
 
-        Set the `index_col` argument to one or more columns to choose an
-        index. The resulting DataFrame is sorted by the index columns. For the
-        best performance, ensure the index columns don't contain duplicate
-        values.
+        * (Default behavior) Add an arbitrary sequential index and ordering
+          using an an analytic windowed operation that prevents filtering
+          push down.
+        * (Recommended) Set the ``index_col`` argument to one or more columns.
+          Unique values for the row labels are recommended. Duplicate labels
+          are possible, but note that joins on a non-unique index can duplicate
+          rows and operations like ``cumsum()`` that window across a non-unique
+          index can have some non-deternimism.
 
         .. note::
             By default, even SQL query inputs with an ORDER BY clause create a
             DataFrame with an arbitrary ordering. Use ``row_number() OVER
             (ORDER BY ...) AS rowindex`` in your SQL query and set
             ``index_col='rowindex'`` to preserve the desired ordering.
 
@@ -101,14 +105,17 @@
                 A SQL string to be executed or a BigQuery table to be read. The
                 table must be specified in the format of
                 `project.dataset.tablename` or `dataset.tablename`.
                 Can also take wildcard table name, such as `project.dataset.table_prefix*`.
                 In tha case, will read all the matched table as one DataFrame.
             index_col (Iterable[str] or str):
                 Name of result column(s) to use for index in results DataFrame.
+
+                **New in bigframes version 1.3.0**: If ``index_cols`` is not
+                set, the primary key(s) of the table are used as the index.
             columns (Iterable[str]):
                 List of BigQuery column names in the desired order for results
                 DataFrame.
             configuration (dict, optional):
                 Query config parameters for job processing.
                 For example: configuration = {'query': {'useQueryCache': False}}.
                 For more information see `BigQuery REST API Reference
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parquet.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parquet.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/io/pickle.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/io/pickle.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/pandas/_typing.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/pandas/_typing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/plotting/_core.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/plotting/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     """
     Make plots of Series or DataFrame with the `matplotlib` backend.
 
     **Examples:**
     For Series:
 
         >>> import bigframes.pandas as bpd
+        >>> bpd.options.display.progress_bar = None
         >>> ser = bpd.Series([1, 2, 3, 3])
         >>> plot = ser.plot(kind='hist', title="My plot")
 
     For DataFrame:
 
         >>> df = bpd.DataFrame({'length': [1.5, 0.5, 1.2, 0.9, 3],
         ...                   'width': [0.7, 0.2, 0.15, 0.2, 1.1]},
@@ -53,14 +54,15 @@
         into bins and draws all bins in one :class:`matplotlib.axes.Axes`.
         This is useful when the DataFrame's Series are in a similar scale.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
             >>> import numpy as np
+            >>> bpd.options.display.progress_bar = None
             >>> df = bpd.DataFrame(np.random.randint(1, 7, 6000), columns=['one'])
             >>> df['two'] = np.random.randint(1, 7, 6000) + np.random.randint(1, 7, 6000)
             >>> ax = df.plot.hist(bins=12, alpha=0.5)
 
         Args:
             by (str or sequence, optional):
                 Column in the DataFrame to group by. It is not supported yet.
@@ -89,14 +91,15 @@
         This function calls `pandas.plot` to generate a plot with a random sample
         of items. For consistent results, the random sampling is reproducible.
         Use the `sampling_random_state` parameter to modify the sampling seed.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
             >>> df = bpd.DataFrame(
             ...     {
             ...         'one': [1, 2, 3, 4],
             ...         'three': [3, 6, 9, 12],
             ...         'reverse_ten': [40, 30, 20, 10],
             ...     }
             ... )
@@ -156,14 +159,15 @@
         Use the `sampling_random_state` parameter to modify the sampling seed.
 
         **Examples:**
 
         Draw an area plot based on basic business metrics:
 
             >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
             >>> df = bpd.DataFrame(
             ...     {
             ...         'sales': [3, 2, 3, 9, 10, 6],
             ...         'signups': [5, 5, 6, 12, 14, 13],
             ...         'visits': [20, 42, 28, 62, 81, 50],
             ...     },
             ...     index=["01-31", "02-28", "03-31", "04-30", "05-31", "06-30"]
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_exceptions.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/pandas/util/_validators.py` & `bigframes-1.3.0/third_party/bigframes_vendored/pandas/util/_validators.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/COPYING` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/COPYING`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/base.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 Input samples.
 
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
                 Series or DataFrame of shape (n_samples,) or (n_samples, n_outputs). Default None.
                 Target values (None for unsupervised transformations).
 
         Returns:
-            bigframes.dataframe.DataFrame: DataFrame of shape (n_samples, n_features_new)
+            bigframes.dataframe.DataFrame: DataFrame of shape (n_samples, n_features_new).
                 Transformed DataFrame.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
 
 
 class MetaEstimatorMixin:
     _required_parameters = ["estimator"]
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 def recall_score(
     y_true,
     y_pred,
     average: str = "binary",
 ):
     """Compute the recall.
 
-    The recall is the ratio ``tp / (tp + fn)`` where ``tp`` is the number of
+    The recall is the ratio ``tp / (tp + fn)``, where ``tp`` is the number of
     true positives and ``fn`` the number of false negatives. The recall is
     intuitively the ability of the classifier to find all the positive samples.
 
     The best value is 1 and the worst value is 0.
 
     **Examples:**
 
@@ -166,15 +166,15 @@
 def precision_score(
     y_true,
     y_pred,
     average: str = "binary",
 ):
     """Compute the precision.
 
-    The precision is the ratio ``tp / (tp + fp)`` where ``tp`` is the number of
+    The precision is the ratio ``tp / (tp + fp)``, where ``tp`` is the number of
     true positives and ``fp`` the number of false positives. The precision is
     intuitively the ability of the classifier not to label as positive a sample
     that is negative.
 
     The best value is 1 and the worst value is 0.
 
     **Examples:**
@@ -240,17 +240,17 @@
         >>> f1_score
         0    0.8
         1    0.0
         2    0.0
         dtype: float64
 
     Args:
-        y_true: Series or DataFrame of shape (n_samples,)
+        y_true: Series or DataFrame of shape (n_samples,).
             Ground truth (correct) target values.
-        y_pred: Series or DataFrame of shape (n_samples,)
+        y_pred: Series or DataFrame of shape (n_samples,).
             Estimated targets as returned by a classifier.
         average: {'micro', 'macro', 'samples', 'weighted', 'binary'} or None, \
                 default='binary'
             This parameter is required for multiclass/multilabel targets.
             Possible values are 'None', 'micro', 'macro', 'samples', 'weighted', 'binary'.
 
     Returns:
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/pipeline.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 from bigframes import constants
 
 
 class Pipeline(BaseEstimator, metaclass=ABCMeta):
     """Pipeline of transforms with a final estimator.
 
     Sequentially apply a list of transforms and a final estimator.
-    Intermediate steps of the pipeline must be `transforms`, that is, they
+    Intermediate steps of the pipeline must be `transforms`. That is, they
     must implement `fit` and `transform` methods.
     The final estimator only needs to implement `fit`.
 
     The purpose of the pipeline is to assemble several steps that can be
-    cross-validated together while setting different parameters. This simplifies code, and allows deploying an estimator
-    and peprocessing together, e.g. with `Pipeline.to_gbq(...).`
+    cross-validated together while setting different parameters. This
+    simplifies code and allows for deploying an estimator and peprocessing
+    together, e.g. with `Pipeline.to_gbq(...).`
     """
 
     def fit(
         self,
         X,
         y,
     ):
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,29 @@
     binary columns, the encoding is a single column of `STRUCT<index INT64, value DOUBLE>`.
 
     **Examples:**
 
         Given a dataset with two features, we let the encoder find the unique
         values per feature and transform the data to a binary one-hot encoding.
 
-        .. code-block::
-
-            from bigframes.ml.preprocessing import OneHotEncoder
-            import bigframes.pandas as bpd
-
-            enc = OneHotEncoder()
-            X = bpd.DataFrame({"a": ["Male", "Female", "Female"], "b": ["1", "3", "2"]})
-            enc.fit(X)
-            print(enc.transform(bpd.DataFrame({"a": ["Female", "Male"], "b": ["1", "4"]})))
+        >>> from bigframes.ml.preprocessing import OneHotEncoder
+        >>> import bigframes.pandas as bpd
+        >>> bpd.options.display.progress_bar = None
+
+        >>> enc = OneHotEncoder()
+        >>> X = bpd.DataFrame({"a": ["Male", "Female", "Female"], "b": ["1", "3", "2"]})
+        >>> enc.fit(X)
+        OneHotEncoder()
+
+        >>> print(enc.transform(bpd.DataFrame({"a": ["Female", "Male"], "b": ["1", "4"]})))
+                        onehotencoded_a               onehotencoded_b
+        0  [{'index': 1, 'value': 1.0}]  [{'index': 1, 'value': 1.0}]
+        1  [{'index': 2, 'value': 1.0}]  [{'index': 0, 'value': 1.0}]
+        <BLANKLINE>
+        [2 rows x 2 columns]
 
     Args:
         drop (Optional[Literal["most_frequent"]], default None):
             Specifies a methodology to use to drop one of the categories per feature.
             This is useful in situations where perfectly collinear features cause problems,
             such as when feeding the resulting data into an unregularized linear regression model.
             However, dropping one category breaks the symmetry of the original representation
@@ -48,15 +54,15 @@
             Specifies the minimum frequency below which a category will be considered infrequent.
             Default None.
             int: categories with a smaller cardinality will be considered infrequent as index 0.
         max_categories (Optional[int], default None):
             Specifies an upper limit to the number of output features for each input feature
             when considering infrequent categories. If there are infrequent categories,
             max_categories includes the category representing the infrequent categories along with the frequent categories.
-            Default None, set limit to 1,000,000.
+            Default None. Set limit to 1,000,000.
     """
 
     def fit(self, X, y=None):
         """Fit OneHotEncoder to X.
 
         Args:
             X (bigframes.dataframe.DataFrame or bigframes.series.Series):
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py` & `bigframes-1.3.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             Specifies the minimum frequency below which a category will be considered infrequent.
             Default None.
             int: categories with a smaller cardinality will be considered infrequent as ßindex 0.
         max_categories (Optional[int], default None):
             Specifies an upper limit to the number of output features for each input feature
             when considering infrequent categories. If there are infrequent categories,
             max_categories includes the category representing the infrequent categories along with the frequent categories.
-            Default None, set limit to 1,000,000.
+            Default None. Set limit to 1,000,000.
     """
 
     def fit(self, y):
         """Fit label encoder.
 
         Args:
             y (bigframes.dataframe.DataFrame or bigframes.series.Series):
```

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/xgboost/LICENSE` & `bigframes-1.3.0/third_party/bigframes_vendored/xgboost/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.2.0/third_party/bigframes_vendored/xgboost/sklearn.py` & `bigframes-1.3.0/third_party/bigframes_vendored/xgboost/sklearn.py`

 * *Files identical despite different names*

