# Comparing `tmp/datature-1.7.0.tar.gz` & `tmp/datature-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datature-1.7.0.tar", last modified: Fri Apr 19 10:47:26 2024, max compression
+gzip compressed data, was "datature-1.7.1b1.tar", last modified: Tue Apr 23 10:49:52 2024, max compression
```

## Comparing `datature-1.7.0.tar` & `datature-1.7.1b1.tar`

### file list

```diff
@@ -1,121 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.838978 datature-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-19 10:47:20.000000 datature-1.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 10:47:20.000000 datature-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 10:47:20.000000 datature-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 10:47:26.838978 datature-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-19 10:47:20.000000 datature-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.810978 datature-1.7.0/datature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.810978 datature-1.7.0/datature/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/import_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/client_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/nexus/medical/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/nii_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    41184 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/nexus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/file_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/experimental/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32462 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/tensorrt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.838978 datature-1.7.0/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.806978 datature-1.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/msgspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 10:47:20.000000 datature-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:47:26.838978 datature-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 10:47:20.000000 datature-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_annotation_import_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/fixture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/artifact_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/asset_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/frame_fixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.830978 datature-1.7.0/tests/unit/fixture/data/medical/
--rw-r--r--   0 runner    (1001) docker     (127)  1702398 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/0002.DCM
--rw-r--r--   0 runner    (1001) docker     (127)  1049988 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/0015.DCM
--rw-r--r--   0 runner    (1001) docker     (127)  4765024 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/MR_Gd.nii
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/projects_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_file_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_medical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.819096 datature-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-23 10:49:44.000000 datature-1.7.1b1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 10:49:44.000000 datature-1.7.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 10:49:44.000000 datature-1.7.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-23 10:49:52.815096 datature-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-23 10:49:44.000000 datature-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.779096 datature-1.7.1b1/datature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.783096 datature-1.7.1b1/datature/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.783096 datature-1.7.1b1/datature/nexus/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.783096 datature-1.7.1b1/datature/nexus/api/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/annotation/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/annotation/import_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/nexus/api/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/api/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/nexus/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/cli/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/client_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/nexus/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/medical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/medical/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/medical/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/medical/nii_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41184 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/nexus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/utils/file_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/nexus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.787096 datature-1.7.1b1/datature/utils/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.791096 datature-1.7.1b1/datature/utils/experimental/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32462 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/convert/tensorrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.791096 datature-1.7.1b1/datature/utils/experimental/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-23 10:49:44.000000 datature-1.7.1b1/datature/utils/experimental/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.815096 datature-1.7.1b1/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 10:49:52.000000 datature-1.7.1b1/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.775096 datature-1.7.1b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.791096 datature-1.7.1b1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/msgspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-23 10:49:44.000000 datature-1.7.1b1/docs/source/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 10:49:44.000000 datature-1.7.1b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:49:52.819096 datature-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-23 10:49:44.000000 datature-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.791096 datature-1.7.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.795096 datature-1.7.1b1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.795096 datature-1.7.1b1/tests/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_annotation_import_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/api/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.795096 datature-1.7.1b1/tests/unit/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.799096 datature-1.7.1b1/tests/unit/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/artifact_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/asset_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/frame_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.803096 datature-1.7.1b1/tests/unit/fixture/data/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)  1702398 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/medical/0002.DCM
+-rw-r--r--   0 runner    (1001) docker     (127)  1049988 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/medical/0015.DCM
+-rw-r--r--   0 runner    (1001) docker     (127)  4765024 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/medical/MR_Gd.nii
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/projects_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.811096 datature-1.7.1b1/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.815096 datature-1.7.1b1/tests/unit/model/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.815096 datature-1.7.1b1/tests/unit/model/configs/bbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/bbox/invalid_input_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/bbox/invalid_output_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/bbox/missing_input_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/bbox/missing_output_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/bbox/pristine.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.815096 datature-1.7.1b1/tests/unit/model/configs/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/classification/invalid_input_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/classification/invalid_output_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/classification/missing_input_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/classification/missing_output_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/classification/pristine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/empty_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/invalid_task.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/missing_inputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/missing_outputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/missing_task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:49:52.815096 datature-1.7.1b1/tests/unit/model/configs/semantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/semantic/invalid_input_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/semantic/invalid_output_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/semantic/missing_input_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/semantic/missing_output_field.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/configs/semantic/pristine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/model/test_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/test_file_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/test_medical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-23 10:49:44.000000 datature-1.7.1b1/tests/unit/test_utils.py
```

### Comparing `datature-1.7.0/CHANGELOG.md` & `datature-1.7.1b1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/LICENSE` & `datature-1.7.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/PKG-INFO` & `datature-1.7.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.7.0
+Version: 1.7.1b1
 Summary: Python bindings for the Datature API
 Author: Datature
 Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/
 Project-URL: Documentation, https://developers.datature.io/docs/python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datature Version: 1.7.0 Summary: Python bindings
+Metadata-Version: 2.1 Name: datature Version: 1.7.1b1 Summary: Python bindings
 for the Datature API Author: Datature Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/ Project-URL: Documentation,
 https://developers.datature.io/docs/python-sdk Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

### Comparing `datature-1.7.0/README.md` & `datature-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/annotation/annotation.py` & `datature-1.7.1b1/datature/nexus/api/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/annotation/import_session.py` & `datature-1.7.1b1/datature/nexus/api/annotation/import_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/artifact.py` & `datature-1.7.1b1/datature/nexus/api/artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/asset/asset.py` & `datature-1.7.1b1/datature/nexus/api/asset/asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/asset/upload_session.py` & `datature-1.7.1b1/datature/nexus/api/asset/upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/deployment.py` & `datature-1.7.1b1/datature/nexus/api/deployment.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/ontology.py` & `datature-1.7.1b1/datature/nexus/api/ontology.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/operation.py` & `datature-1.7.1b1/datature/nexus/api/operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/project.py` & `datature-1.7.1b1/datature/nexus/api/project.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/run.py` & `datature-1.7.1b1/datature/nexus/api/run.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/tag.py` & `datature-1.7.1b1/datature/nexus/api/tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/types.py` & `datature-1.7.1b1/datature/nexus/api/types.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/api/workflow.py` & `datature-1.7.1b1/datature/nexus/api/workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/cli/commands.py` & `datature-1.7.1b1/datature/nexus/cli/commands.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/cli/config.py` & `datature-1.7.1b1/datature/nexus/cli/config.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/cli/functions.py` & `datature-1.7.1b1/datature/nexus/cli/functions.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/cli/main.py` & `datature-1.7.1b1/datature/nexus/cli/main.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/cli/messages.py` & `datature-1.7.1b1/datature/nexus/cli/messages.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/client.py` & `datature-1.7.1b1/datature/nexus/client.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/client_context.py` & `datature-1.7.1b1/datature/nexus/client_context.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/config.py` & `datature-1.7.1b1/datature/nexus/config.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/error.py` & `datature-1.7.1b1/datature/nexus/error.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/medical/__init__.py` & `datature-1.7.1b1/datature/nexus/medical/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/medical/base_processor.py` & `datature-1.7.1b1/datature/nexus/medical/base_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/medical/dicom_processor.py` & `datature-1.7.1b1/datature/nexus/medical/dicom_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/medical/nii_processor.py` & `datature-1.7.1b1/datature/nexus/medical/nii_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/models.py` & `datature-1.7.1b1/datature/nexus/models.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/requester.py` & `datature-1.7.1b1/datature/nexus/requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/utils/file_signature.py` & `datature-1.7.1b1/datature/nexus/utils/file_signature.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/nexus/utils/utils.py` & `datature-1.7.1b1/datature/nexus/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/converter.py` & `datature-1.7.1b1/datature/utils/experimental/convert/converter.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/logger.py` & `datature-1.7.1b1/datature/utils/experimental/convert/logger.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/params.py` & `datature-1.7.1b1/datature/utils/experimental/convert/params.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/prediction_utils.py` & `datature-1.7.1b1/datature/utils/experimental/convert/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/predictor.py` & `datature-1.7.1b1/datature/utils/experimental/convert/predictor.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature/utils/experimental/convert/tensorrt.py` & `datature-1.7.1b1/datature/utils/experimental/convert/tensorrt.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/datature.egg-info/PKG-INFO` & `datature-1.7.1b1/datature.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.7.0
+Version: 1.7.1b1
 Summary: Python bindings for the Datature API
 Author: Datature
 Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/
 Project-URL: Documentation, https://developers.datature.io/docs/python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datature Version: 1.7.0 Summary: Python bindings
+Metadata-Version: 2.1 Name: datature Version: 1.7.1b1 Summary: Python bindings
 for the Datature API Author: Datature Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/ Project-URL: Documentation,
 https://developers.datature.io/docs/python-sdk Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

### Comparing `datature-1.7.0/docs/source/conf.py` & `datature-1.7.1b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/docs/source/functions.rst` & `datature-1.7.1b1/docs/source/functions.rst`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/docs/source/readme.rst` & `datature-1.7.1b1/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/docs/source/types.rst` & `datature-1.7.1b1/docs/source/types.rst`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/setup.py` & `datature-1.7.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_annotation.py` & `datature-1.7.1b1/tests/unit/api/test_annotation.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_annotation_import_session.py` & `datature-1.7.1b1/tests/unit/api/test_annotation_import_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_artifact.py` & `datature-1.7.1b1/tests/unit/api/test_artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_asset.py` & `datature-1.7.1b1/tests/unit/api/test_asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_asset_upload_session.py` & `datature-1.7.1b1/tests/unit/api/test_asset_upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_client.py` & `datature-1.7.1b1/tests/unit/api/test_client.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_deploy.py` & `datature-1.7.1b1/tests/unit/api/test_deploy.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_ontology.py` & `datature-1.7.1b1/tests/unit/api/test_ontology.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_operation.py` & `datature-1.7.1b1/tests/unit/api/test_operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_project.py` & `datature-1.7.1b1/tests/unit/api/test_project.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_run.py` & `datature-1.7.1b1/tests/unit/api/test_run.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_tag.py` & `datature-1.7.1b1/tests/unit/api/test_tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/api/test_workflow.py` & `datature-1.7.1b1/tests/unit/api/test_workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/artifact_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/artifact_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/asset_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/asset_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/error_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/error_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/frame_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/frame_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/medical/0002.DCM` & `datature-1.7.1b1/tests/unit/fixture/data/medical/0002.DCM`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/medical/0015.DCM` & `datature-1.7.1b1/tests/unit/fixture/data/medical/0015.DCM`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/medical/MR_Gd.nii` & `datature-1.7.1b1/tests/unit/fixture/data/medical/MR_Gd.nii`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/operation_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/operation_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/projects_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/projects_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/data/upload_session_fixture.py` & `datature-1.7.1b1/tests/unit/fixture/data/upload_session_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/fixture/mock.py` & `datature-1.7.1b1/tests/unit/fixture/mock.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/test_file_signature.py` & `datature-1.7.1b1/tests/unit/test_file_signature.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/test_medical.py` & `datature-1.7.1b1/tests/unit/test_medical.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/test_requester.py` & `datature-1.7.1b1/tests/unit/test_requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.7.0/tests/unit/test_utils.py` & `datature-1.7.1b1/tests/unit/test_utils.py`

 * *Files identical despite different names*

