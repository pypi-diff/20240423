# Comparing `tmp/cryoet_data_portal-3.0.1.tar.gz` & `tmp/cryoet_data_portal-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoet_data_portal-3.0.1.tar", last modified: Thu Feb 15 19:51:50 2024, max compression
+gzip compressed data, was "cryoet_data_portal-3.0.2.tar", last modified: Tue Apr 23 16:11:52 2024, max compression
```

## Comparing `cryoet_data_portal-3.0.1.tar` & `cryoet_data_portal-3.0.2.tar`

### file list

```diff
@@ -1,180 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.052067 cryoet_data_portal-3.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.044067 cryoet_data_portal-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.052067 cryoet_data_portal-3.0.1/src/cryoet_data_portal/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/_gql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33355 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.056067 cryoet_data_portal-3.0.1/src/cryoet_data_portal/data/
--rw-r--r--   0 runner    (1001) docker     (127)   216625 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal/data/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-15 19:51:49.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-02-15 19:51:50.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 19:51:49.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-15 19:51:49.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-15 19:51:49.000000 cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.056067 cryoet_data_portal-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_get_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.056067 cryoet_data_portal-3.0.1/tests/test_infra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.044067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/actions.graphql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/allow_list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/api_limits.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/backend_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/cron_triggers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.044067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_authors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_authors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_funding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_datasets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_runs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tiltseries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_authors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_voxel_spacings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomograms.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/tables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/databases.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/graphql_schema_introspection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/inherited_roles.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/metrics_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/network.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/opentelemetry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/query_collections.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/remote_schemas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/rest_endpoints.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/version.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.044067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.044067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/
--rw-r--r--   0 runner    (1001) docker     (127)    32987 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/up.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/
--rw-r--r--   0 runner    (1001) docker     (127)    17137 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/up.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)      495 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/seed_moto.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/Frames/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/Frames/frame1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.060067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.mdoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.rawtlt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.xf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/zarr_file1
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1_bin1.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/author1-mitochondria-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/author1-ribosome-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.ndjson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/zarr_file1
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.mdoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.rawtlt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.xf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.064067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/author2-ribosome-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.052067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.mdoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.rawtlt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.xf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/0/file_2.zarr
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/file_1.zarr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.048067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/author3-ribosome-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.052067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.mdoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.mrc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.rawtlt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.xf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.068067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.052067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/author4-ribosome-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/author4-spike-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/zarr_file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.mrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 19:51:50.072067 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/0/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/0/zarr_file2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 19:51:40.000000 cryoet_data_portal-3.0.1/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.577755 cryoet_data_portal-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/src/cryoet_data_portal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/_gql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33920 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.589755 cryoet_data_portal-3.0.2/src/cryoet_data_portal/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   221799 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal/data/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 16:11:52.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-23 16:11:52.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:11:52.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 16:11:52.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 16:11:52.000000 cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.589755 cryoet_data_portal-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_get_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.589755 cryoet_data_portal-3.0.2/tests/test_infra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.577755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/actions.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/allow_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/api_limits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/backend_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/cron_triggers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.577755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_authors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_authors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_funding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_datasets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_runs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tiltseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_authors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_voxel_spacings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomograms.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/tables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/databases.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/graphql_schema_introspection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/inherited_roles.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/metrics_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/network.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/opentelemetry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/query_collections.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/remote_schemas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/rest_endpoints.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.577755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/
+-rw-r--r--   0 runner    (1001) docker     (127)    32987 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/up.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/up.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/1706552817192_alter_annotation_add_tomogram_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/1706552817192_alter_annotation_add_tomogram_table/up.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      495 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/seed_moto.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.593755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/Frames/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/Frames/frame1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.mdoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.rawtlt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.xf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/zarr_file1
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1_bin1.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/author1-mitochondria-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/author1-ribosome-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.ndjson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr/zarr_file1
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN1/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN1.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.597755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.mdoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.rawtlt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.xf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TiltSeries/RUN2.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.581755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/author2-ribosome-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20001/RUN2/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN2.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.mdoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.rawtlt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.xf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/0/file_2.zarr
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TiltSeries/RUN001.zarr/file_1.zarr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/author3-ribosome-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.601755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN001/TomogramVoxelSpacing7.56/CanonicalTomogram/RUN001.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.mdoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.mrc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.rawtlt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.xf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TiltSeries/RUN002.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.585755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/author4-ribosome-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/author4-spike-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr/zarr_file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.mrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:11:52.605755 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/0/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/0/zarr_file2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 16:11:43.000000 cryoet_data_portal-3.0.2/tests/test_infra/test_files/20002/RUN002/TomogramVoxelSpacing13.48/CanonicalTomogram/RUN002.zarr/zarr_file1
```

### Comparing `cryoet_data_portal-3.0.1/LICENSE` & `cryoet_data_portal-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/Makefile` & `cryoet_data_portal-3.0.2/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 .PHONY: test
 test:
 	export AWS_REGION=us-west-2; \
 		export AWS_ACCESS_KEY_ID=test; \
 		export AWS_SECRET_ACCESS_KEY=test; \
 		export BOTO_ENDPOINT_URL=http://localhost:4000; \
 		export BOTO_SIGNATURE_VERSION=s3v4; \
-		pytest -vvv -s .
+		pytest -vvv -s . $(TEST)
```

### Comparing `cryoet_data_portal-3.0.1/PKG-INFO` & `cryoet_data_portal-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet_data_portal
-Version: 3.0.1
+Version: 3.0.2
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-3.0.1/README.md` & `cryoet_data_portal-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/pyproject.toml` & `cryoet_data_portal-3.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/__init__.py` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/_client.py` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from gql import Client as GQLClient
 from gql.dsl import DSLQuery, DSLSchema, dsl_gql
 from gql.transport.requests import RequestsHTTPTransport
 
 
 class Client:
-    """A GraphQL Client library that can traverse all of the metadata in the CryoET Data Portal
+    """A GraphQL Client library that can traverse all the metadata in the CryoET Data Portal
 
     Args:
         url (Optional[str]): The API URL to connect to, defaults to "https://graphql.cryoetdataportal.cziscience.com/v1/graphql"
 
     Returns:
         A GraphQL API Client library
```

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/_file_tools.py` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/_file_tools.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/_gql_base.py` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/_gql_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,23 @@
     def __init__(self, field: "GQLField", operator, value: Optional[Any]):
         self.field = field
         self.operator = operator
         self.value = value
 
     def to_gql(self) -> Dict[str, Any]:
         fieldname = self.field.to_gql()
+        if self.field.is_relationship():
+            related_cls = self.field.get_related_class()
+            scalar_fields = related_cls._get_scalar_fields()
+            if isinstance(fieldname, str):
+                fieldname = [fieldname]
+
+            raise Exception(
+                f"\"{'.'.join(fieldname)}\" is an object and can't be compared directly. Please filter on one of its scalar attributes instead: {', '.join(scalar_fields)}",
+            )
         gql = {}
         if isinstance(fieldname, list):
             for item in fieldname[::-1]:
                 if not gql:
                     gql = {item: {self.operator: self.value}}
                     continue
                 gql = {item: gql}
@@ -59,14 +68,19 @@
     def _in(self, value) -> GQLExpression:
         return GQLExpression(self, "_in", value)
 
     def configure(self, cls, name):
         self._cls = cls
         self._name = name
 
+    def is_relationship(self):
+        if isinstance(self, Relationship):
+            return True
+        return False
+
     def to_gql(self):
         return self._name
 
 
 class BaseField(GQLField):
     def __init__(self, cls: Optional[type] = None, name: Optional[str] = None):
         self._cls = cls
@@ -106,14 +120,22 @@
         self.__name = [relationship._name, attr]
 
     def __getattr__(self, attr):
         self.__current_query = getattr(self.__current_query, attr)
         self.__name.append(attr)
         return self
 
+    def is_relationship(self):
+        if isinstance(self.__current_query, Relationship):
+            return True
+        return False
+
+    def get_related_class(self):
+        return self.__current_query.get_related_class()
+
     def to_gql(self):
         return self.__name
 
 
 class Relationship(GQLField):
     descriptor_class: type
 
@@ -129,14 +151,17 @@
         self.source_field = source_field
         self.dest_field = dest_field
 
         # Helpers for resolving GQL field names.
         self._cls = cls
         self._name = name
 
+    def get_related_class(self):
+        return self.related_class
+
     def resolve_class(self):
         if type(self.related_class) is not type:
             module = import_module(f"{__package__}._models")
             self.related_class = getattr(module, self.related_class)
 
     # If we're trying to chain fields when generating a query, let's hand that
     # functionality off to QueryChain to handle
@@ -215,16 +240,24 @@
         client: Client,
         query_filters: Optional[Iterable[GQLExpression]] = None,
     ):
         """Find objects based on a set of search filters.
 
         Search filters are combined with *and* so all results will match all filters.
 
-        Expressions must be in the format:
+        Expressions with python-native operators (``==``, ``!=``, ``>``, ``>=``, ``<``, ``<=``) must be in the format:
             ``ModelSubclass.field`` ``{operator}`` ``{value}``
+        Example:
+            - ``Tomogram.voxel_spacing.run.name == "RUN1"``
+
+        Expressions with method operators (``like``, ``ilike``, ``_in``) must be in the format:
+            ``ModelSubclass.field.{operator}({value})``
+        Examples:
+            - ``Tomogram.voxel_spacing.run.name.like("%RUN1%")``
+            - ``Tomogram.voxel_spacing.run.name._in(["RUN1", "RUN2"])``
 
         Supported operators are: ``==``, ``!=``, ``>``, ``>=``, ``<``, ``<=``, ``like``, ``ilike``, ``_in``
 
         - ``like`` is a partial match, with the `%` character being a wildcard
         - ``ilike`` is similar to ``like`` but case-insensitive
         - ``_in`` accepts a list of values that are acceptable matches.
 
@@ -243,14 +276,15 @@
             Matching Model objects.
 
         Examples:
 
             Filter runs by attributes, including attributes in related models:
 
             >>> runs = Run.find(client, query_filters=[Run.name == "TS_026", Run.dataset.id == 10000])
+            >>> runs = Run.find(client, query_filters=[Run.name._in(['TS_026', 'TS_027']), Run.tomogram_voxel_spacings.annotations.object_name.ilike('%membrane%')])
 
             Get all results for this type:
 
             >>> runs = Run.find(client)
         """
         filters = {}
         if query_filters:
```

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/_models.py` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,17 +255,16 @@
 class Tomogram(Model):
     """Metadata for a tomogram
 
     Attributes:
         id (int): Numeric identifier for this tomogram (this may change!)
         affine_transformation_matrix (str): The flip or rotation transformation of this author submitted tomogram is indicated here
         ctf_corrected (bool): Whether this tomogram is CTF corrected
-        dataset (Dataset): An object relationship with the dataset this tomogram is a part of
-        dataset_id (int): Reference to the dataset this tomogram is a part of
         fiducial_alignment_status (str): Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
+        deposition_id (int): If the tomogram is part of a deposition, the related deposition's id
         https_mrc_scale0 (str): HTTPS path to this tomogram in MRC format (no scaling)
         https_omezarr_dir (str): HTTPS path to this tomogram in multiscale OME-Zarr format
         is_canonical (bool): Is this tomogram considered the canonical tomogram for the run experiment? True=Yes
         key_photo_thumbnail_url (str): URL for the thumbnail of key photo
         key_photo_url (str): URL for the key photo
         name (str): Short name for this tomogram
         neuroglancer_config (str): the compact json of neuroglancer config
@@ -297,14 +296,15 @@
         "tomogram_voxel_spacing_id",
         "id",
     )
 
     id: int = IntField()
     affine_transformation_matrix: str = StringField()
     ctf_corrected: int = BooleanField()
+    deposition_id: int = IntField()
     fiducial_alignment_status: str = StringField()
     https_mrc_scale0: str = StringField()
     https_omezarr_dir: str = StringField()
     is_canonical: int = BooleanField()
     key_photo_thumbnail_url: str = StringField()
     key_photo_url: str = StringField()
     name: str = StringField()
@@ -413,18 +413,21 @@
         annotation_method (str): Describe how the annotation is made (e.g. Manual, crYoLO, Positive Unlabeled Learning, template matching)
         annotation_publication (str): DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
         annotation_software (str): Software used for generating this annotation
         authors (list[Author]): An array relationship with the authors of this annotation
         confidence_precision (float): Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
         confidence_recall (float): Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
         deposition_date (date): Date when an annotation set is initially received by the Data Portal.
+        deposition_id (int): If the annotation is part of a deposition, the related deposition's id
+        files (list[AnnotationFile]): An array relationship with the files of this annotation
         ground_truth_status (bool): Whether an annotation is considered ground truth, as determined by the annotator.
         ground_truth_used (str): Annotation filename used as ground truth for precision and recall
         https_metadata_path (str): HTTPS path for the metadata json file for this annotation
         last_modified_date (date): Date when an annotation was last modified in the Data Portal
+        method_type (str): The method type for generating the annotation (eg. manual, hybrid, automated)
         object_count (int): Number of objects identified
         object_description (str): A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
         object_id (str): Gene Ontology Cellular Component identifier for the annotation object
         object_name (str): Name of the object being annotated (e.g. ribosome, nuclear pore complex, actin filament, membrane)
         object_state (str): Molecule state annotated (e.g. open, closed)
         release_date (date): Date when annotation data is made public by the Data Portal.
         tomogram_voxel_spacing (TomogramVoxelSpacing): An object relationship with a specific voxel spacing for this annotation
@@ -442,20 +445,22 @@
 
     annotation_method: str = StringField()
     annotation_publication: str = StringField()
     annotation_software: str = StringField()
     confidence_precision: float = FloatField()
     confidence_recall: float = FloatField()
     deposition_date: date = DateField()
+    deposition_id: int = IntField()
     ground_truth_status: int = BooleanField()
     ground_truth_used: str = StringField()
     https_metadata_path: str = StringField()
     id: int = IntField()
     is_curator_recommended: bool = BooleanField()
     last_modified_date: date = DateField()
+    method_type: str = StringField()
     object_count: int = IntField()
     object_description: str = StringField()
     object_id: str = StringField()
     object_name: str = StringField()
     object_state: str = StringField()
     release_date: date = DateField()
     s3_metadata_path: str = StringField()
@@ -481,30 +486,34 @@
         """Download annotation files for a given format and/or shape
 
         Args:
             dest_path (Optional[str], optional): Choose a destination directory. Defaults to $CWD.
             shape (Optional[str], optional): Choose a specific shape type to download (e.g.: OrientedPoint, SegmentationMask)
             format (Optional[str], optional): Choose a specific file format to download (e.g.: mrc, ndjson)
         """
-        download_https(self.https_metadata_path, dest_path)
+        download_metadata = False
         for file in self.files:
             if format and file.format != format:
                 continue
             if shape and file.shape_type != shape:
                 continue
             file.download(dest_path)
+            download_metadata = True
+        if download_metadata:
+            download_https(self.https_metadata_path, dest_path)
 
 
 class AnnotationFile(Model):
     """Metadata for an annotation file
 
     Attributes:
         id (int): Numeric identifier (May change!)
         format (str): File format for this file
         https_path (str): HTTPS url for the annotation file
+        is_visualization_default (bool): Is this annotation shape displayed in visualization tools by default
         s3_path (str): S3 path for the annotation file
         shape_type (str): Describe whether this is a Point, OrientedPoint, or SegmentationMask file
         annotation_id (int): Reference to the annotation this file applies to
         Annotation (Annotation): The annotation this file is a part of
     """
 
     _gql_type = "annotation_files"
@@ -512,18 +521,18 @@
     annotation: "Annotation" = ItemRelationship(
         "Annotation",
         "annotation_id",
         "id",
     )
 
     id: int = IntField()
-    format: str = StringField()
-    https_path: str = StringField()
     annotation_id: int = IntField()
+    format: str = StringField()
     https_path: str = StringField()
+    is_visualization_default: bool = BooleanField()
     s3_path: str = StringField()
     shape_type: str = StringField()
 
     def download(self, dest_path: Optional[str] = None):
         if self.format == "zarr":
             recursive_prefix = "/".join(self.s3_path.split("/")[:-1]) + "/"
             download_directory(self.s3_path, recursive_prefix, dest_path)
```

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal/data/schema.graphql` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal/data/schema.graphql`

 * *Files 3% similar despite different names*

```diff
@@ -682,14 +682,19 @@
   """Format of the annotation object file"""
   format: String!
 
   """https path of the annotation file"""
   https_path: String!
   id: Int!
 
+  """
+  Data curator’s subjective choice of default annotation to display in visualization for an object
+  """
+  is_visualization_default: Boolean
+
   """s3 path of the annotation file"""
   s3_path: String!
 
   """The type of the annotation"""
   shape_type: String!
 }
 
@@ -698,17 +703,33 @@
 """
 type annotation_files_aggregate {
   aggregate: annotation_files_aggregate_fields
   nodes: [annotation_files!]!
 }
 
 input annotation_files_aggregate_bool_exp {
+  bool_and: annotation_files_aggregate_bool_exp_bool_and
+  bool_or: annotation_files_aggregate_bool_exp_bool_or
   count: annotation_files_aggregate_bool_exp_count
 }
 
+input annotation_files_aggregate_bool_exp_bool_and {
+  arguments: annotation_files_select_column_annotation_files_aggregate_bool_exp_bool_and_arguments_columns!
+  distinct: Boolean
+  filter: annotation_files_bool_exp
+  predicate: Boolean_comparison_exp!
+}
+
+input annotation_files_aggregate_bool_exp_bool_or {
+  arguments: annotation_files_select_column_annotation_files_aggregate_bool_exp_bool_or_arguments_columns!
+  distinct: Boolean
+  filter: annotation_files_bool_exp
+  predicate: Boolean_comparison_exp!
+}
+
 input annotation_files_aggregate_bool_exp_count {
   arguments: [annotation_files_select_column!]
   distinct: Boolean
   filter: annotation_files_bool_exp
   predicate: Int_comparison_exp!
 }
 
@@ -768,14 +789,15 @@
   _not: annotation_files_bool_exp
   _or: [annotation_files_bool_exp!]
   annotation: annotations_bool_exp
   annotation_id: Int_comparison_exp
   format: String_comparison_exp
   https_path: String_comparison_exp
   id: Int_comparison_exp
+  is_visualization_default: Boolean_comparison_exp
   s3_path: String_comparison_exp
   shape_type: String_comparison_exp
 }
 
 """aggregate max on columns"""
 type annotation_files_max_fields {
   annotation_id: Int
@@ -855,14 +877,15 @@
 """Ordering options when selecting data from "annotation_files"."""
 input annotation_files_order_by {
   annotation: annotations_order_by
   annotation_id: order_by
   format: order_by
   https_path: order_by
   id: order_by
+  is_visualization_default: order_by
   s3_path: order_by
   shape_type: order_by
 }
 
 """
 select columns of table "annotation_files"
 """
@@ -876,20 +899,39 @@
   """column name"""
   https_path
 
   """column name"""
   id
 
   """column name"""
+  is_visualization_default
+
+  """column name"""
   s3_path
 
   """column name"""
   shape_type
 }
 
+"""
+select "annotation_files_aggregate_bool_exp_bool_and_arguments_columns" columns of table "annotation_files"
+"""
+enum annotation_files_select_column_annotation_files_aggregate_bool_exp_bool_and_arguments_columns {
+  """column name"""
+  is_visualization_default
+}
+
+"""
+select "annotation_files_aggregate_bool_exp_bool_or_arguments_columns" columns of table "annotation_files"
+"""
+enum annotation_files_select_column_annotation_files_aggregate_bool_exp_bool_or_arguments_columns {
+  """column name"""
+  is_visualization_default
+}
+
 """aggregate stddev on columns"""
 type annotation_files_stddev_fields {
   annotation_id: Float
   id: Float
 }
 
 """
@@ -946,14 +988,19 @@
   """Format of the annotation object file"""
   format: String
 
   """https path of the annotation file"""
   https_path: String
   id: Int
 
+  """
+  Data curator’s subjective choice of default annotation to display in visualization for an object
+  """
+  is_visualization_default: Boolean
+
   """s3 path of the annotation file"""
   s3_path: String
 
   """The type of the annotation"""
   shape_type: String
 }
 
@@ -1071,14 +1118,17 @@
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: numeric
 
   """Date when an annotation set is initially received by the Data Portal."""
   deposition_date: date!
 
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """An array relationship"""
   files(
     """distinct select on columns"""
     distinct_on: [annotation_files_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
@@ -1129,14 +1179,17 @@
   Data curator’s subjective choice as the best annotation of the same annotation object ID
   """
   is_curator_recommended: Boolean
 
   """Date when an annotation was last modified in the Data Portal"""
   last_modified_date: date
 
+  """Provides information on the method type used for generating annotation"""
+  method_type: String
+
   """Number of objects identified"""
   object_count: Int!
 
   """
   A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
   """
   object_description: String
@@ -1240,14 +1293,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1262,14 +1318,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1285,22 +1344,24 @@
   annotation_publication: String_comparison_exp
   annotation_software: String_comparison_exp
   authors: annotation_authors_bool_exp
   authors_aggregate: annotation_authors_aggregate_bool_exp
   confidence_precision: numeric_comparison_exp
   confidence_recall: numeric_comparison_exp
   deposition_date: date_comparison_exp
+  deposition_id: Int_comparison_exp
   files: annotation_files_bool_exp
   files_aggregate: annotation_files_aggregate_bool_exp
   ground_truth_status: Boolean_comparison_exp
   ground_truth_used: String_comparison_exp
   https_metadata_path: String_comparison_exp
   id: Int_comparison_exp
   is_curator_recommended: Boolean_comparison_exp
   last_modified_date: date_comparison_exp
+  method_type: String_comparison_exp
   object_count: Int_comparison_exp
   object_description: String_comparison_exp
   object_id: String_comparison_exp
   object_name: String_comparison_exp
   object_state: String_comparison_exp
   release_date: date_comparison_exp
   s3_metadata_path: String_comparison_exp
@@ -1330,26 +1391,32 @@
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: numeric
 
   """Date when an annotation set is initially received by the Data Portal."""
   deposition_date: date
 
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """Annotation filename used as ground truth for precision and recall"""
   ground_truth_used: String
 
   """https path for the metadata json file for this annotation"""
   https_metadata_path: String
 
   """Numeric identifier (May change!)"""
   id: Int
 
   """Date when an annotation was last modified in the Data Portal"""
   last_modified_date: date
 
+  """Provides information on the method type used for generating annotation"""
+  method_type: String
+
   """Number of objects identified"""
   object_count: Int
 
   """
   A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
   """
   object_description: String
@@ -1397,26 +1464,32 @@
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
   """Date when an annotation set is initially received by the Data Portal."""
   deposition_date: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Annotation filename used as ground truth for precision and recall"""
   ground_truth_used: order_by
 
   """https path for the metadata json file for this annotation"""
   https_metadata_path: order_by
 
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Date when an annotation was last modified in the Data Portal"""
   last_modified_date: order_by
 
+  """Provides information on the method type used for generating annotation"""
+  method_type: order_by
+
   """Number of objects identified"""
   object_count: order_by
 
   """
   A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
   """
   object_description: order_by
@@ -1462,26 +1535,32 @@
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: numeric
 
   """Date when an annotation set is initially received by the Data Portal."""
   deposition_date: date
 
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """Annotation filename used as ground truth for precision and recall"""
   ground_truth_used: String
 
   """https path for the metadata json file for this annotation"""
   https_metadata_path: String
 
   """Numeric identifier (May change!)"""
   id: Int
 
   """Date when an annotation was last modified in the Data Portal"""
   last_modified_date: date
 
+  """Provides information on the method type used for generating annotation"""
+  method_type: String
+
   """Number of objects identified"""
   object_count: Int
 
   """
   A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
   """
   object_description: String
@@ -1529,26 +1608,32 @@
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
   """Date when an annotation set is initially received by the Data Portal."""
   deposition_date: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Annotation filename used as ground truth for precision and recall"""
   ground_truth_used: order_by
 
   """https path for the metadata json file for this annotation"""
   https_metadata_path: order_by
 
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Date when an annotation was last modified in the Data Portal"""
   last_modified_date: order_by
 
+  """Provides information on the method type used for generating annotation"""
+  method_type: order_by
+
   """Number of objects identified"""
   object_count: order_by
 
   """
   A textual description of the annotation object, can be a longer description to include additional information not covered by the Annotation object name and state.
   """
   object_description: order_by
@@ -1577,21 +1662,23 @@
   annotation_method: order_by
   annotation_publication: order_by
   annotation_software: order_by
   authors_aggregate: annotation_authors_aggregate_order_by
   confidence_precision: order_by
   confidence_recall: order_by
   deposition_date: order_by
+  deposition_id: order_by
   files_aggregate: annotation_files_aggregate_order_by
   ground_truth_status: order_by
   ground_truth_used: order_by
   https_metadata_path: order_by
   id: order_by
   is_curator_recommended: order_by
   last_modified_date: order_by
+  method_type: order_by
   object_count: order_by
   object_description: order_by
   object_id: order_by
   object_name: order_by
   object_state: order_by
   release_date: order_by
   s3_metadata_path: order_by
@@ -1618,14 +1705,17 @@
   """column name"""
   confidence_recall
 
   """column name"""
   deposition_date
 
   """column name"""
+  deposition_id
+
+  """column name"""
   ground_truth_status
 
   """column name"""
   ground_truth_used
 
   """column name"""
   https_metadata_path
@@ -1636,14 +1726,17 @@
   """column name"""
   is_curator_recommended
 
   """column name"""
   last_modified_date
 
   """column name"""
+  method_type
+
+  """column name"""
   object_count
 
   """column name"""
   object_description
 
   """column name"""
   object_id
@@ -1694,14 +1787,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1716,14 +1812,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1736,14 +1835,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1758,14 +1860,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1778,14 +1883,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1800,14 +1908,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1820,14 +1931,17 @@
   confidence_precision: numeric
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: numeric
 
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """Numeric identifier (May change!)"""
   id: Int
 
   """Number of objects identified"""
   object_count: Int
   tomogram_voxel_spacing_id: Int
 }
@@ -1842,14 +1956,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1862,14 +1979,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1884,14 +2004,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1904,14 +2027,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1926,14 +2052,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -1946,14 +2075,17 @@
   confidence_precision: Float
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: Float
 
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier (May change!)"""
   id: Float
 
   """Number of objects identified"""
   object_count: Float
   tomogram_voxel_spacing_id: Float
 }
@@ -1968,14 +2100,17 @@
   confidence_precision: order_by
 
   """
   Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
   """
   confidence_recall: order_by
 
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier (May change!)"""
   id: order_by
 
   """Number of objects identified"""
   object_count: order_by
   tomogram_voxel_spacing_id: order_by
 }
@@ -7247,14 +7382,17 @@
     order_by: [tomogram_authors_order_by!]
 
     """filter the rows returned"""
     where: tomogram_authors_bool_exp
   ): tomogram_authors_aggregate!
   ctf_corrected: Boolean
 
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String!
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String!
@@ -7413,14 +7551,17 @@
   var_pop: tomograms_var_pop_order_by
   var_samp: tomograms_var_samp_order_by
   variance: tomograms_variance_order_by
 }
 
 """aggregate avg on columns"""
 type tomograms_avg_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -7445,14 +7586,17 @@
   voxel_spacing: Float
 }
 
 """
 order by avg() on columns of table "tomograms"
 """
 input tomograms_avg_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -7484,14 +7628,15 @@
   _and: [tomograms_bool_exp!]
   _not: tomograms_bool_exp
   _or: [tomograms_bool_exp!]
   affine_transformation_matrix: _numeric_comparison_exp
   authors: tomogram_authors_bool_exp
   authors_aggregate: tomogram_authors_aggregate_bool_exp
   ctf_corrected: Boolean_comparison_exp
+  deposition_id: Int_comparison_exp
   fiducial_alignment_status: String_comparison_exp
   https_mrc_scale0: String_comparison_exp
   https_omezarr_dir: String_comparison_exp
   id: Int_comparison_exp
   is_canonical: Boolean_comparison_exp
   key_photo_thumbnail_url: String_comparison_exp
   key_photo_url: String_comparison_exp
@@ -7518,14 +7663,17 @@
   tomogram_voxel_spacing_id: Int_comparison_exp
   type: tomogram_type_enum_comparison_exp
   voxel_spacing: numeric_comparison_exp
 }
 
 """aggregate max on columns"""
 type tomograms_max_fields {
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String
@@ -7605,14 +7753,17 @@
   voxel_spacing: numeric
 }
 
 """
 order by max() on columns of table "tomograms"
 """
 input tomograms_max_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: order_by
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: order_by
@@ -7690,14 +7841,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate min on columns"""
 type tomograms_min_fields {
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String
@@ -7777,14 +7931,17 @@
   voxel_spacing: numeric
 }
 
 """
 order by min() on columns of table "tomograms"
 """
 input tomograms_min_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: order_by
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: order_by
@@ -7865,14 +8022,15 @@
 }
 
 """Ordering options when selecting data from "tomograms"."""
 input tomograms_order_by {
   affine_transformation_matrix: order_by
   authors_aggregate: tomogram_authors_aggregate_order_by
   ctf_corrected: order_by
+  deposition_id: order_by
   fiducial_alignment_status: order_by
   https_mrc_scale0: order_by
   https_omezarr_dir: order_by
   id: order_by
   is_canonical: order_by
   key_photo_thumbnail_url: order_by
   key_photo_url: order_by
@@ -7908,14 +8066,17 @@
   """column name"""
   affine_transformation_matrix
 
   """column name"""
   ctf_corrected
 
   """column name"""
+  deposition_id
+
+  """column name"""
   fiducial_alignment_status
 
   """column name"""
   https_mrc_scale0
 
   """column name"""
   https_omezarr_dir
@@ -8016,14 +8177,17 @@
 
   """column name"""
   is_canonical
 }
 
 """aggregate stddev on columns"""
 type tomograms_stddev_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8048,14 +8212,17 @@
   voxel_spacing: Float
 }
 
 """
 order by stddev() on columns of table "tomograms"
 """
 input tomograms_stddev_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8078,14 +8245,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate stddev_pop on columns"""
 type tomograms_stddev_pop_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8110,14 +8280,17 @@
   voxel_spacing: Float
 }
 
 """
 order by stddev_pop() on columns of table "tomograms"
 """
 input tomograms_stddev_pop_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8140,14 +8313,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate stddev_samp on columns"""
 type tomograms_stddev_samp_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8172,14 +8348,17 @@
   voxel_spacing: Float
 }
 
 """
 order by stddev_samp() on columns of table "tomograms"
 """
 input tomograms_stddev_samp_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8202,14 +8381,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate sum on columns"""
 type tomograms_sum_fields {
+  """id of the associated deposition."""
+  deposition_id: Int
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Int
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Int
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8234,14 +8416,17 @@
   voxel_spacing: numeric
 }
 
 """
 order by sum() on columns of table "tomograms"
 """
 input tomograms_sum_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8264,14 +8449,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate var_pop on columns"""
 type tomograms_var_pop_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8296,14 +8484,17 @@
   voxel_spacing: Float
 }
 
 """
 order by var_pop() on columns of table "tomograms"
 """
 input tomograms_var_pop_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8326,14 +8517,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate var_samp on columns"""
 type tomograms_var_samp_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8358,14 +8552,17 @@
   voxel_spacing: Float
 }
 
 """
 order by var_samp() on columns of table "tomograms"
 """
 input tomograms_var_samp_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8388,14 +8585,17 @@
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate variance on columns"""
 type tomograms_variance_fields {
+  """id of the associated deposition."""
+  deposition_id: Float
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: Float
 
   """y offset data relative to the canonical tomogram in pixels"""
@@ -8420,14 +8620,17 @@
   voxel_spacing: Float
 }
 
 """
 order by variance() on columns of table "tomograms"
 """
 input tomograms_variance_order_by {
+  """id of the associated deposition."""
+  deposition_id: order_by
+
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
   """x offset data relative to the canonical tomogram in pixels"""
   offset_x: order_by
 
   """y offset data relative to the canonical tomogram in pixels"""
```

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/PKG-INFO` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet_data_portal
-Version: 3.0.1
+Version: 3.0.2
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-3.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt` & `cryoet_data_portal-3.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/cryoet_data_portal.egg-info/requires.txt
 src/cryoet_data_portal.egg-info/top_level.txt
 src/cryoet_data_portal/data/schema.graphql
 tests/README.md
 tests/conftest.py
 tests/docker-compose.yml
 tests/test_downloads.py
+tests/test_filters.py
 tests/test_get_client.py
 tests/test_infra/seed_moto.sh
 tests/test_infra/hasura/metadata/actions.graphql
 tests/test_infra/hasura/metadata/actions.yaml
 tests/test_infra/hasura/metadata/allow_list.yaml
 tests/test_infra/hasura/metadata/api_limits.yaml
 tests/test_infra/hasura/metadata/backend_configs.yaml
@@ -47,14 +48,15 @@
 tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_authors.yaml
 tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_type.yaml
 tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_voxel_spacings.yaml
 tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomograms.yaml
 tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/tables.yaml
 tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/up.sql
 tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/up.sql
+tests/test_infra/hasura/migrations/cryoetdataportal/1706552817192_alter_annotation_add_tomogram_table/up.sql
 tests/test_infra/test_files/20001/RUN1/Frames/frame1
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.mdoc
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.rawtlt
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.xf
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1_bin1.mrc
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/zarr_file1
 tests/test_infra/test_files/20001/RUN1/TiltSeries/RUN1.zarr/0/zarr_file2
```

### Comparing `cryoet_data_portal-3.0.1/tests/README.md` & `cryoet_data_portal-3.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/conftest.py` & `cryoet_data_portal-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/docker-compose.yml` & `cryoet_data_portal-3.0.2/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_downloads.py` & `cryoet_data_portal-3.0.2/tests/test_downloads.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,21 +19,39 @@
         yield tmpdirname
 
 
 def test_download_annotations(tmp_dir, client) -> None:
     """download a single annotation file for a dataset, using format/shape filters"""
     annos = Annotation.find(
         client,
-        [Annotation.tomogram_voxel_spacing.run.dataset.id == 20001],
+        [
+            Annotation.tomogram_voxel_spacing.run.name == "RUN2",
+            Annotation.object_name.ilike("%ribosome%"),
+        ],
     )
     anno = annos[0]
     assert anno
-    anno.download(tmp_dir, "json", "OrientedPoint")
+    anno.download(tmp_dir, "ndjson", "OrientedPoint")
     files = os.listdir(tmp_dir)
-    assert files == ["author2-ribosome-1.0.json"]
+    assert set(files) == {"author2-ribosome-1.0.json", "ribosome.ndjson"}
+
+
+def test_download_tomo_annotations_with_shape_filter(tmp_dir, client) -> None:
+    """Make sure downloading annotations for a specific shape type doesn't download"""
+    """metadata for other annotations without this shape type"""
+    tomo = Tomogram.find(
+        client,
+        [
+            Tomogram.tomogram_voxel_spacing.run.name == "RUN1",
+        ],
+    )[0]
+    assert tomo
+    tomo.download_all_annotations(dest_path=tmp_dir, format="ndjson", shape="Point")
+    files = os.listdir(tmp_dir)
+    assert set(files) == {"ribosome.ndjson", "author1-ribosome-1.0.json"}
 
 
 def test_download_all_annotations_including_zarr(tmp_dir, client) -> None:
     """Download all files for a particular annotation. Using ds 20001 because it has a zarr."""
     anno = Annotation.find(
         client,
         [
@@ -59,48 +77,62 @@
     # Change the process' CWD to the tmp dir
     os.chdir(tmp_dir)
     subdir_name = "my_test_subdir"
     dest_dir = os.path.join(tmp_dir, subdir_name)
     os.makedirs(dest_dir)
     tomo = Tomogram.find(
         client,
-        [Tomogram.tomogram_voxel_spacing.run.dataset_id == 20001],
+        [
+            Tomogram.tomogram_voxel_spacing.run.dataset_id == 20001,
+            Tomogram.tomogram_voxel_spacing.run.name == "RUN2",
+        ],
     )[0]
     assert tomo
-    tomo.download_all_annotations(subdir_name, "json")
+    tomo.download_all_annotations(subdir_name)
     files = os.listdir(dest_dir)
-    assert files == ["author2-ribosome-1.0.json"]
+    assert set(files) == {
+        "author2-ribosome-1.0.json",
+        "ribosome.mrc",
+        "ribosome.ndjson",
+        "ribosome.zarr",
+    }
 
 
 def test_download_without_path(tmp_dir, client) -> None:
     """Download files *without specifying a path* (should default to CWD)"""
     # Change the process' CWD to the tmp dir
     os.chdir(tmp_dir)
     tomo = Tomogram.find(
         client,
-        [Tomogram.tomogram_voxel_spacing.run.dataset_id == 20001],
+        [
+            Tomogram.tomogram_voxel_spacing.run.dataset_id == 20001,
+            Tomogram.tomogram_voxel_spacing.run.name == "RUN2",
+        ],
     )[0]
     assert tomo
-    tomo.download_all_annotations(format="json")
+    tomo.download_all_annotations(format="ndjson")
     files = os.listdir(tmp_dir)
-    assert files == ["author2-ribosome-1.0.json"]
+    assert set(files) == {
+        "author2-ribosome-1.0.json",
+        "ribosome.ndjson",
+    }
 
 
 def test_download_default_dir(tmp_dir, client) -> None:
     """Download files with no dest dir specified (defaults to CWD)"""
     # Change the process' CWD to the tmp dir
     os.chdir(tmp_dir)
     tomo = Tomogram.find(
         client,
-        [Tomogram.tomogram_voxel_spacing.run.dataset_id == 20001],
+        [Tomogram.tomogram_voxel_spacing.run.name == "RUN2"],
     )[0]
     assert tomo
-    tomo.download_all_annotations(None, "json")
+    tomo.download_all_annotations(None, "ndjson")
     files = os.listdir(tmp_dir)
-    assert files == ["author2-ribosome-1.0.json"]
+    assert set(files) == {"author2-ribosome-1.0.json", "ribosome.ndjson"}
 
 
 def test_tiltseries_downloaders(tmp_dir, client):
     ts = TiltSeries.find(client, [TiltSeries.run.name == "RUN1"])[0]
     assert ts
     ts.download_collection_metadata(tmp_dir)
     ts.download_angle_list(tmp_dir)
```

### Comparing `cryoet_data_portal-3.0.1/tests/test_get_client.py` & `cryoet_data_portal-3.0.2/tests/test_get_client.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_authors.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotation_authors.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotations.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_annotations.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,22 @@
       columns:
         - annotation_method
         - annotation_publication
         - annotation_software
         - confidence_precision
         - confidence_recall
         - deposition_date
+        - deposition_id
         - ground_truth_status
         - ground_truth_used
         - https_metadata_path
         - id
         - is_curator_recommended
         - last_modified_date
+        - method_type
         - object_count
         - object_description
         - object_id
         - object_name
         - object_state
         - release_date
         - s3_metadata_path
```

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_authors.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_dataset_authors.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_datasets.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_datasets.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_runs.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_runs.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tiltseries.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tiltseries.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_authors.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_authors.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_voxel_spacings.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomogram_voxel_spacings.yaml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomograms.yaml` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/metadata/databases/cryoetdataportal/tables/public_tomograms.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
           schema: public
 select_permissions:
   - role: anonymous
     permission:
       columns:
         - affine_transformation_matrix
         - ctf_corrected
+        - deposition_id
         - fiducial_alignment_status
         - https_mrc_scale0
         - https_omezarr_dir
         - id
         - is_canonical
         - key_photo_thumbnail_url
         - key_photo_url
```

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/up.sql` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000000_init/up.sql`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-3.0.1/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/up.sql` & `cryoet_data_portal-3.0.2/tests/test_infra/hasura/migrations/cryoetdataportal/0000000000001_data/up.sql`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 INSERT INTO public.annotation_authors VALUES (58, 45, 'Author 7', '0000-0000-0000-0079', false, true, NULL, NULL, NULL, NULL, NULL);
 INSERT INTO public.annotation_authors VALUES (59, 45, 'Author 8', '0000-0000-0000-0089', false, true, NULL, NULL, NULL, NULL, NULL);
 
 
 INSERT INTO public.annotation_files VALUES (70, 40, 'OrientedPoint', 'ndjson', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.ndjson', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.ndjson');
 INSERT INTO public.annotation_files VALUES (71, 40, 'SegmentationMask', 'mrc', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.mrc', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.mrc');
 INSERT INTO public.annotation_files VALUES (72, 40, 'SegmentationMask', 'zarr', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/mitochondria.zarr');
-INSERT INTO public.annotation_files VALUES (73, 41, 'OrientedPoint', 'ndjson', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson');
+INSERT INTO public.annotation_files VALUES (73, 41, 'Point', 'ndjson', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson');
 INSERT INTO public.annotation_files VALUES (74, 41, 'SegmentationMask', 'mrc', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.mrc');
 INSERT INTO public.annotation_files VALUES (75, 41, 'SegmentationMask', 'zarr', 'http://localhost:4444/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr', 's3://test-public-bucket/20001/RUN1/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr');
 INSERT INTO public.annotation_files VALUES (76, 42, 'OrientedPoint', 'ndjson', 'http://localhost:4444/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson', 's3://test-public-bucket/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson');
 INSERT INTO public.annotation_files VALUES (77, 42, 'SegmentationMask', 'mrc', 'http://localhost:4444/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.mrc', 's3://test-public-bucket/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.mrc');
 INSERT INTO public.annotation_files VALUES (78, 42, 'SegmentationMask', 'zarr', 'http://localhost:4444/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr', 's3://test-public-bucket/20001/RUN2/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr');
 INSERT INTO public.annotation_files VALUES (79, 43, 'OrientedPoint', 'ndjson', 'http://localhost:4444/20002/RUN001/TomogramVoxelSpacing7.56/Annotations/ribosome.ndjson', 's3://test-public-bucket/20002/RUN001/TomogramVoxelSpacing13.48/Annotations/ribosome.ndjson');
 INSERT INTO public.annotation_files VALUES (80, 44, 'SegmentationMask', 'zarr', 'http://localhost:4444/20002/RUN002/TomogramVoxelSpacing7.56/Annotations/ribosome.zarr', 's3://test-public-bucket/20002/RUN002/TomogramVoxelSpacing13.48/Annotations/ribosome.zarr');
```

