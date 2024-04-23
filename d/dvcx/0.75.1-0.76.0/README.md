# Comparing `tmp/dvcx-0.75.1.tar.gz` & `tmp/dvcx-0.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.75.1.tar", last modified: Mon Apr 22 02:27:33 2024, max compression
+gzip compressed data, was "dvcx-0.76.0.tar", last modified: Tue Apr 23 06:01:41 2024, max compression
```

## Comparing `dvcx-0.75.1.tar` & `dvcx-0.76.0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.540675 dvcx-0.75.1/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-22 02:27:27.000000 dvcx-0.75.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 02:27:27.000000 dvcx-0.75.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.496675 dvcx-0.75.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.496675 dvcx-0.75.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.496675 dvcx-0.75.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-22 02:27:27.000000 dvcx-0.75.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-22 02:27:27.000000 dvcx-0.75.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-22 02:27:27.000000 dvcx-0.75.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.496675 dvcx-0.75.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 02:27:27.000000 dvcx-0.75.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-22 02:27:27.000000 dvcx-0.75.1/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 02:27:27.000000 dvcx-0.75.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-22 02:27:27.000000 dvcx-0.75.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-22 02:27:27.000000 dvcx-0.75.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.496675 dvcx-0.75.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-22 02:27:27.000000 dvcx-0.75.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-22 02:27:27.000000 dvcx-0.75.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-22 02:27:27.000000 dvcx-0.75.1/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-22 02:27:33.540675 dvcx-0.75.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-22 02:27:27.000000 dvcx-0.75.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.500675 dvcx-0.75.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-22 02:27:27.000000 dvcx-0.75.1/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.500675 dvcx-0.75.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.504675 dvcx-0.75.1/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.504675 dvcx-0.75.1/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.504675 dvcx-0.75.1/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-22 02:27:27.000000 dvcx-0.75.1/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-22 02:27:27.000000 dvcx-0.75.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-22 02:27:27.000000 dvcx-0.75.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:27:33.540675 dvcx-0.75.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.492675 dvcx-0.75.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.508675 dvcx-0.75.1/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.512675 dvcx-0.75.1/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71363 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.512675 dvcx-0.75.1/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.512675 dvcx-0.75.1/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45015 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.516675 dvcx-0.75.1/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.520675 dvcx-0.75.1/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    57821 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.520675 dvcx-0.75.1/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.520675 dvcx-0.75.1/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.520675 dvcx-0.75.1/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.520675 dvcx-0.75.1/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.524675 dvcx-0.75.1/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-22 02:27:27.000000 dvcx-0.75.1/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.536675 dvcx-0.75.1/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 02:27:33.000000 dvcx-0.75.1/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.524675 dvcx-0.75.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.524675 dvcx-0.75.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.528675 dvcx-0.75.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34442 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112414 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.532675 dvcx-0.75.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.532675 dvcx-0.75.1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.532675 dvcx-0.75.1/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:27:33.532675 dvcx-0.75.1/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-22 02:27:27.000000 dvcx-0.75.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.988620 dvcx-0.76.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 06:01:32.000000 dvcx-0.76.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 06:01:32.000000 dvcx-0.76.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.940620 dvcx-0.76.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.940620 dvcx-0.76.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-23 06:01:32.000000 dvcx-0.76.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-23 06:01:32.000000 dvcx-0.76.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 06:01:32.000000 dvcx-0.76.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 06:01:32.000000 dvcx-0.76.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-23 06:01:32.000000 dvcx-0.76.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-23 06:01:32.000000 dvcx-0.76.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-23 06:01:41.988620 dvcx-0.76.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-23 06:01:32.000000 dvcx-0.76.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 06:01:32.000000 dvcx-0.76.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.952620 dvcx-0.76.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-23 06:01:32.000000 dvcx-0.76.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-23 06:01:32.000000 dvcx-0.76.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:01:41.988620 dvcx-0.76.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.932620 dvcx-0.76.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71363 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.960620 dvcx-0.76.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45015 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30640 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33101 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57821 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.972620 dvcx-0.76.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.972620 dvcx-0.76.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34442 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112414 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.976620 dvcx-0.76.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.976620 dvcx-0.76.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/utils.py
```

### Comparing `dvcx-0.75.1/.cruft.json` & `dvcx-0.76.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.76.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.76.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.github/workflows/benchmarks.yml` & `dvcx-0.76.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.github/workflows/release.yml` & `dvcx-0.76.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.github/workflows/tests.yml` & `dvcx-0.76.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.gitignore` & `dvcx-0.76.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/.pre-commit-config.yaml` & `dvcx-0.76.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/CODE_OF_CONDUCT.rst` & `dvcx-0.76.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/CONTRIBUTING.rst` & `dvcx-0.76.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/LICENSE` & `dvcx-0.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/LICENSES/Apache-2.0.txt` & `dvcx-0.76.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/LICENSES/BSD-3-Clause.txt` & `dvcx-0.76.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/LICENSES/Python-2.0.txt` & `dvcx-0.76.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/PKG-INFO` & `dvcx-0.76.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.75.1
+Version: 0.76.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.75.1/README.rst` & `dvcx-0.76.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/docs/udfs.md` & `dvcx-0.76.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/blip2_image_desc_lib.py` & `dvcx-0.76.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/clip.py` & `dvcx-0.76.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/common_sql_functions.py` & `dvcx-0.76.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/dir_expansion.py` & `dvcx-0.76.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/hf_pipeline.py` & `dvcx-0.76.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/llava2_image_desc_lib.py` & `dvcx-0.76.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/loader.py` & `dvcx-0.76.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/neurips/README` & `dvcx-0.76.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/neurips/distance_to_query.py` & `dvcx-0.76.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/neurips/llm_chat.py` & `dvcx-0.76.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/neurips/single_query.py` & `dvcx-0.76.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/neurips/text_loaders.py` & `dvcx-0.76.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/openai_image_desc_lib.py` & `dvcx-0.76.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/openimage-detect.py` & `dvcx-0.76.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/pose_detection.py` & `dvcx-0.76.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/torch-loader.py` & `dvcx-0.76.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/batching.py` & `dvcx-0.76.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/image_transformation.py` & `dvcx-0.76.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/parallel.py` & `dvcx-0.76.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/simple.py` & `dvcx-0.76.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/stateful.py` & `dvcx-0.76.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/udfs/stateful_similarity.py` & `dvcx-0.76.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/unstructured-text.py` & `dvcx-0.76.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/wds.py` & `dvcx-0.76.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/wds_filtered.py` & `dvcx-0.76.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/wds_meta.py` & `dvcx-0.76.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/zalando/zalando_clip.py` & `dvcx-0.76.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.76.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/noxfile.py` & `dvcx-0.76.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/pyproject.toml` & `dvcx-0.76.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/asyn.py` & `dvcx-0.76.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/cache.py` & `dvcx-0.76.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/catalog/catalog.py` & `dvcx-0.76.0/src/dvcx/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/catalog/datasource.py` & `dvcx-0.76.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/catalog/formats.py` & `dvcx-0.76.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/catalog/loader.py` & `dvcx-0.76.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/cli.py` & `dvcx-0.76.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/cli_utils.py` & `dvcx-0.76.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/azure.py` & `dvcx-0.76.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/fileslice.py` & `dvcx-0.76.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/fsspec.py` & `dvcx-0.76.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/gcs.py` & `dvcx-0.76.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/local.py` & `dvcx-0.76.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/client/s3.py` & `dvcx-0.76.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/config.py` & `dvcx-0.76.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/db_engine.py` & `dvcx-0.76.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/id_generator.py` & `dvcx-0.76.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/metastore.py` & `dvcx-0.76.0/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/schema.py` & `dvcx-0.76.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/serializer.py` & `dvcx-0.76.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/sqlite.py` & `dvcx-0.76.0/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,14 +591,17 @@
 
     def init_db(self, uri: StorageURI, partial_id: int) -> None:
         if not uri:
             raise ValueError("uri for init_db() cannot be empty")
         nodes_table = self.nodes_table(uri, partial_id).table
         self.db.create_table(nodes_table, if_not_exists=True)
 
+    def is_ready(self, timeout: Optional[int] = None) -> bool:
+        return True
+
     def create_dataset_rows_table(
         self,
         name: str,
         custom_columns: Sequence["sqlalchemy.Column"] = (),
         if_not_exists: bool = True,
     ) -> Table:
         table = self.schema.dataset_row_cls.new_table(
```

### Comparing `dvcx-0.75.1/src/dvcx/data_storage/warehouse.py` & `dvcx-0.76.0/src/dvcx/data_storage/warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,17 @@
     def init_db(self, uri: StorageURI, partial_id: int) -> None:
         """Initializes database tables for warehouse"""
 
     #
     # Query Tables
     #
 
+    @abstractmethod
+    def is_ready(self, timeout: Optional[int]) -> bool: ...
+
     @property
     def nodes(self):
         assert (
             self.current_bucket_table_name
         ), "Nodes can only be used if uri/current_bucket_table_name is set"
         if self._nodes is None:
             self._nodes = self.schema.node_cls(
```

### Comparing `dvcx-0.75.1/src/dvcx/dataset.py` & `dvcx-0.76.0/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/error.py` & `dvcx-0.76.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/cached_stream.py` & `dvcx-0.76.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/dataset.py` & `dvcx-0.76.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/feature.py` & `dvcx-0.76.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/feature_udf.py` & `dvcx-0.76.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/file.py` & `dvcx-0.76.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.76.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.76.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.76.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/image_transform.py` & `dvcx-0.76.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.76.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/param.py` & `dvcx-0.76.0/src/dvcx/lib/param.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/pytorch.py` & `dvcx-0.76.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/udf.py` & `dvcx-0.76.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/unstructured.py` & `dvcx-0.76.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/utils.py` & `dvcx-0.76.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/webdataset.py` & `dvcx-0.76.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.76.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.76.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/listing.py` & `dvcx-0.76.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/node.py` & `dvcx-0.76.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/nodes_fetcher.py` & `dvcx-0.76.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/nodes_thread_pool.py` & `dvcx-0.76.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/progress.py` & `dvcx-0.76.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/batch.py` & `dvcx-0.76.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/builtins.py` & `dvcx-0.76.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/dataset.py` & `dvcx-0.76.0/src/dvcx/query/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/dispatch.py` & `dvcx-0.76.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/schema.py` & `dvcx-0.76.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/session.py` & `dvcx-0.76.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/query/udf.py` & `dvcx-0.76.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/remote/studio.py` & `dvcx-0.76.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/default/base.py` & `dvcx-0.76.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/functions/array.py` & `dvcx-0.76.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/functions/path.py` & `dvcx-0.76.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/selectable.py` & `dvcx-0.76.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/sqlite/base.py` & `dvcx-0.76.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/sqlite/types.py` & `dvcx-0.76.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/types.py` & `dvcx-0.76.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/sql/utils.py` & `dvcx-0.76.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/storage.py` & `dvcx-0.76.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx/utils.py` & `dvcx-0.76.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.76.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.75.1
+Version: 0.76.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.75.1/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.76.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/src/dvcx.egg-info/requires.txt` & `dvcx-0.76.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/benchmarks/conftest.py` & `dvcx-0.76.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/conftest.py` & `dvcx-0.76.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/data.py` & `dvcx-0.76.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_catalog.py` & `dvcx-0.76.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_client.py` & `dvcx-0.76.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_dataset_query.py` & `dvcx-0.76.0/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_datasets.py` & `dvcx-0.76.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_ls.py` & `dvcx-0.76.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_pull.py` & `dvcx-0.76.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_pytorch.py` & `dvcx-0.76.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/func/test_query.py` & `dvcx-0.76.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/test_cli_e2e.py` & `dvcx-0.76.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_cached_stream.py` & `dvcx-0.76.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_feature.py` & `dvcx-0.76.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_feature_udf.py` & `dvcx-0.76.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_file.py` & `dvcx-0.76.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_webdataset.py` & `dvcx-0.76.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.76.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/sql/test_array.py` & `dvcx-0.76.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/sql/test_conditional.py` & `dvcx-0.76.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/sql/test_path.py` & `dvcx-0.76.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/sql/test_selectable.py` & `dvcx-0.76.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/sql/test_string.py` & `dvcx-0.76.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_asyn.py` & `dvcx-0.76.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_cache.py` & `dvcx-0.76.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_catalog.py` & `dvcx-0.76.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_catalog_formats.py` & `dvcx-0.76.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_catalog_loader.py` & `dvcx-0.76.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_cli_parsing.py` & `dvcx-0.76.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_client.py` & `dvcx-0.76.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_client_s3.py` & `dvcx-0.76.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_data_storage.py` & `dvcx-0.76.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_database_engine.py` & `dvcx-0.76.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_dataset.py` & `dvcx-0.76.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_fileslice.py` & `dvcx-0.76.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_id_generator.py` & `dvcx-0.76.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_listing.py` & `dvcx-0.76.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_metastore.py` & `dvcx-0.76.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_serializer.py` & `dvcx-0.76.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_session.py` & `dvcx-0.76.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_storage.py` & `dvcx-0.76.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_udf.py` & `dvcx-0.76.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_utils.py` & `dvcx-0.76.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/unit/test_warehouse.py` & `dvcx-0.76.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.75.1/tests/utils.py` & `dvcx-0.76.0/tests/utils.py`

 * *Files identical despite different names*

