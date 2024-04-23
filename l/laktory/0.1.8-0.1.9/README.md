# Comparing `tmp/laktory-0.1.8.tar.gz` & `tmp/laktory-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.1.8.tar", last modified: Mon Mar 25 06:25:37 2024, max compression
+gzip compressed data, was "laktory-0.1.9.tar", last modified: Wed Apr 17 05:20:29 2024, max compression
```

## Comparing `laktory-0.1.8.tar` & `laktory-0.1.9.tar`

### file list

```diff
@@ -1,331 +1,337 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.189410 laktory-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.125410 laktory-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-25 06:25:25.000000 laktory-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-25 06:25:25.000000 laktory-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-03-25 06:25:25.000000 laktory-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-25 06:25:25.000000 laktory-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-25 06:25:25.000000 laktory-0.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-25 06:25:37.189410 laktory-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-25 06:25:25.000000 laktory-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.125410 laktory-0.1.8/bundles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/bundles/stocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-25 06:25:25.000000 laktory-0.1.8/bundles/stocks/databricks.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:25.000000 laktory-0.1.8/bundles/stocks/template_brz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.133411 laktory-0.1.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.137410 laktory-0.1.8/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.137410 laktory-0.1.8/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/basemodel.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.141410 laktory-0.1.8/docs/api/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/databricks/workspacefile.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/dataeventheader.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.141410 laktory-0.1.8/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/datasources/eventdatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/datasources/tabledatasource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.141410 laktory-0.1.8/docs/api/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/providers/databricks.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.141410 laktory-0.1.8/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/resources/baseresource.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.145410 laktory-0.1.8/docs/api/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/tableaggregation.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/tableexpectation.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/tablejoin.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/tablewindowfilter.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/sql/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.145410 laktory-0.1.8/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.125410 laktory-0.1.8/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.145410 laktory-0.1.8/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/dataframe/show_string.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.149410 laktory-0.1.8/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/power.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.149410 laktory-0.1.8/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/governance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/table.md
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.149410 laktory-0.1.8/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.157410 laktory-0.1.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    83413 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/table_builder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.157410 laktory-0.1.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-25 06:25:25.000000 laktory-0.1.8/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.161410 laktory-0.1.8/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.161410 laktory-0.1.8/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.161410 laktory-0.1.8/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/cli/_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19933 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.165410 laktory-0.1.8/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.165410 laktory-0.1.8/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.165410 laktory-0.1.8/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.169410 laktory-0.1.8/laktory/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/databricks/workspacefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/dataeventheader.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.169410 laktory-0.1.8/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/datasources/eventdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.173410 laktory-0.1.8/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/grants/volumegrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.173410 laktory-0.1.8/laktory/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/providers/databricksprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.173410 laktory-0.1.8/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/tableaggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/tablebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/tableexpectation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/tablejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/tablewindowfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/sql/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.129410 laktory-0.1.8/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/resources/notebooks/dlt_brz_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/resources/notebooks/dlt_gld_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/resources/notebooks/dlt_slv_star_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/resources/notebooks/dlt_slv_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.177410 laktory-0.1.8/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/dataframe/show_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.181410 laktory-0.1.8/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-25 06:25:25.000000 laktory-0.1.8/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.185410 laktory-0.1.8/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 06:25:37.000000 laktory-0.1.8/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-03-25 06:25:25.000000 laktory-0.1.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-25 06:25:25.000000 laktory-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.181410 laktory-0.1.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-25 06:25:25.000000 laktory-0.1.8/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 06:25:25.000000 laktory-0.1.8/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.181410 laktory-0.1.8/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 06:25:25.000000 laktory-0.1.8/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 06:25:37.189410 laktory-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:37.185410 laktory-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    16749 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_table_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-25 06:25:25.000000 laktory-0.1.8/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.630675 laktory-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.570675 laktory-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 05:20:21.000000 laktory-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-17 05:20:21.000000 laktory-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 05:20:21.000000 laktory-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 05:20:21.000000 laktory-0.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-17 05:20:29.626675 laktory-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 05:20:21.000000 laktory-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.570675 laktory-0.1.9/bundles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/bundles/stocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-17 05:20:21.000000 laktory-0.1.9/bundles/stocks/databricks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:21.000000 laktory-0.1.9/bundles/stocks/template_brz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/basemodel.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/workspacefile.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataeventheader.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/eventdatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/tabledatasource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/databricks.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/baseresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tableaggregation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tableexpectation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablejoin.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablewindowfilter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.574675 laktory-0.1.9/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/show_string.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.594675 laktory-0.1.9/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/governance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.594675 laktory-0.1.9/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83413 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/table_builder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19933 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/basemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.610675 laktory-0.1.9/laktory/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/workspacefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataeventheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.610675 laktory-0.1.9/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/eventdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/volumegrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/databricksprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableaggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableexpectation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableunion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablewindowfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.574675 laktory-0.1.9/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_brz_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_gld_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_slv_star_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_slv_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/show_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.626675 laktory-0.1.9/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-17 05:20:21.000000 laktory-0.1.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-17 05:20:21.000000 laktory-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 05:20:21.000000 laktory-0.1.9/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 05:20:21.000000 laktory-0.1.9/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 05:20:21.000000 laktory-0.1.9/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:29.630675 laktory-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.626675 laktory-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_table_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_workspacefile.py
```

### Comparing `laktory-0.1.8/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.1.9/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.1.9/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.github/scripts/bump_version.py` & `laktory-0.1.9/.github/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.github/scripts/write_release_body.py` & `laktory-0.1.9/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.github/workflows/release.yml` & `laktory-0.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.github/workflows/test.yml` & `laktory-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/.gitignore` & `laktory-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/CHANGELOG.md` & `laktory-0.1.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # Release History
 
-## [0.1.8] - Unreleased
+## [0.1.9] - Unreleased
 ### Added
-* `getstarted` CLI command to initialize a Laktory stack.
+* Support for table unions in table builder
+* New column property `raise_missing_arg_exception` to allow for some spark function inputs to be missing
+* `add`, `sub`, `mul` and `div` spark functions
+
+### Breaking Change
+* Renamed `power` spark function to `scaled_power` to prevent conflict with native spark function 
+
+## [0.1.8] - 2024-03-25
+### Added
+* `quickstart` CLI command to initialize a sample Laktory stack.
 * Databricks DBFS file model
 
 ## [0.1.7] - 2024-03-15
 ### Added
 * show_version_info() method for bugs reporting
 * Git issues templates
```

### Comparing `laktory-0.1.8/LICENSE` & `laktory-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/PKG-INFO` & `laktory-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.1.8/README.md` & `laktory-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/bundles/stocks/databricks.yml` & `laktory-0.1.9/bundles/stocks/databricks.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/api/models/databricks/cluster.md` & `laktory-0.1.9/docs/api/models/databricks/cluster.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/api/models/databricks/grants.md` & `laktory-0.1.9/docs/api/models/databricks/grants.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/api/models/databricks/job.md` & `laktory-0.1.9/docs/api/models/databricks/job.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/api/models/databricks/metastoredataaccess.md` & `laktory-0.1.9/docs/api/models/databricks/metastoredataaccess.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/cli.md` & `laktory-0.1.9/docs/concepts/cli.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/dataevent.md` & `laktory-0.1.9/docs/concepts/dataevent.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/deployment.md` & `laktory-0.1.9/docs/concepts/deployment.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/design.md` & `laktory-0.1.9/docs/concepts/design.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/governance.md` & `laktory-0.1.9/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/models.md` & `laktory-0.1.9/docs/concepts/models.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/pipeline.md` & `laktory-0.1.9/docs/concepts/pipeline.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/spark.md` & `laktory-0.1.9/docs/concepts/spark.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/stack.md` & `laktory-0.1.9/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/table.md` & `laktory-0.1.9/docs/concepts/table.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/concepts/tablebuilder.md` & `laktory-0.1.9/docs/concepts/tablebuilder.md`

 * *Files 13% similar despite different names*

```diff
@@ -154,14 +154,56 @@
 The source table `slv_stock_prices` acts as the left table in a LEFT JOIN with table `slv_stock_metadata` for which only the `symbol`, `currency` and `first_traded` columns are selected. 
 The `selects` statement can also be defined as a dictionary to remap the other column names into new column names before doing the join.
 
 The `joins` argument is a list of joins such that multiple joins can be chained one after the other.
 
 Spark [structured streaming joins](https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html) are supported using a combination of `read_as_stream` options and watermarks declaration. 
 
+### Unions
+??? "API Documentation"
+    [`laktory.models.TableUnion`][laktory.models.TableUnion]<br>
+For silver star and gold tables, we may want to union multiple tables into one large table.
+```py
+from laktory import models
+
+table = models.Table(
+    name="slv_star_stock_prices",
+    builder={
+        "layer": "SILVER",
+        "table_source": {
+            "name": "slv_stock_prices_googl",
+        },
+        "unions": [
+            {
+                "other": {
+                    "name": "slv_stock_prices_aapl",
+                }
+            },
+            {
+                "other": {
+                    "name": "slv_stock_prices_amzn",
+                }
+            },
+        ],
+    },
+)
+
+# Read
+df = table.builder.read_source(spark)
+
+# Process
+df = table.builder.process(df, spark)
+```
+
+The source table `slv_stock_prices_googl` acts as the left table in a UNION with tables `slv_stock_prices_aapl` and `slv_stock_prices_amzn`.
+
+The `unions` argument is a list of unions such that multiple unions can be chained one after the other.
+
+Spark [dataframe union](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.DataFrame.union.html) is used to execute the joins. 
+
 ### Aggregations
 ??? "API Documentation"
     [`laktory.models.TableAggregation`][laktory.models.TableAggregation]<br>
 Gold tables are all about aggregations. 
 
 ```py
 from laktory import models
```

### Comparing `laktory-0.1.8/docs/concepts/variables.md` & `laktory-0.1.9/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/databricks.png` & `laktory-0.1.9/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/delta_live_tables.png` & `laktory-0.1.9/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/dlt_debug.png` & `laktory-0.1.9/docs/images/dlt_debug.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/kappa.png` & `laktory-0.1.9/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/lakehouse.png` & `laktory-0.1.9/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/logo_sg.png` & `laktory-0.1.9/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/logo_sg_ltb.png` & `laktory-0.1.9/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/logo_sw.png` & `laktory-0.1.9/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/logo_sw_ltw.png` & `laktory-0.1.9/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/medaillon_complex.png` & `laktory-0.1.9/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/medallion.png` & `laktory-0.1.9/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/okube.png` & `laktory-0.1.9/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/pl_stock_prices.png` & `laktory-0.1.9/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/pl_stock_prices_simple.png` & `laktory-0.1.9/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/pulumi.png` & `laktory-0.1.9/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/stock_prices_lineage.png` & `laktory-0.1.9/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/table_builder.png` & `laktory-0.1.9/docs/images/table_builder.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/terraform.png` & `laktory-0.1.9/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/images/what_is_laktory.png` & `laktory-0.1.9/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/index.md` & `laktory-0.1.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/install.md` & `laktory-0.1.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/lakehouseascode.md` & `laktory-0.1.9/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/quickstart.md` & `laktory-0.1.9/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/docs/stylesheets/mkdocstrings.css` & `laktory-0.1.9/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/__init__.py` & `laktory-0.1.9/laktory/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/_logger.py` & `laktory-0.1.9/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/_parsers.py` & `laktory-0.1.9/laktory/_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/_settings.py` & `laktory-0.1.9/laktory/_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/_testing/stackvalidator.py` & `laktory-0.1.9/laktory/_testing/stackvalidator.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/_testing/stockprices.py` & `laktory-0.1.9/laktory/_testing/stockprices.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/cli/app.py` & `laktory-0.1.9/laktory/cli/app.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/constants.py` & `laktory-0.1.9/laktory/constants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/dlt/__init__.py` & `laktory-0.1.9/laktory/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/azurenative/storageblob.py` & `laktory-0.1.9/laktory/models/azurenative/storageblob.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/basemodel.py` & `laktory-0.1.9/laktory/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/__init__.py` & `laktory-0.1.9/laktory/models/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/accesscontrol.py` & `laktory-0.1.9/laktory/models/databricks/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/cluster.py` & `laktory-0.1.9/laktory/models/databricks/cluster.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/dbfsfile.py` & `laktory-0.1.9/laktory/models/databricks/dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/directory.py` & `laktory-0.1.9/laktory/models/databricks/directory.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/externallocation.py` & `laktory-0.1.9/laktory/models/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/grants.py` & `laktory-0.1.9/laktory/models/databricks/grants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/group.py` & `laktory-0.1.9/laktory/models/databricks/group.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/groupmember.py` & `laktory-0.1.9/laktory/models/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/job.py` & `laktory-0.1.9/laktory/models/databricks/job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/metastore.py` & `laktory-0.1.9/laktory/models/databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/metastoreassignment.py` & `laktory-0.1.9/laktory/models/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/metastoredataaccess.py` & `laktory-0.1.9/laktory/models/databricks/metastoredataaccess.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/mwspermissionassignment.py` & `laktory-0.1.9/laktory/models/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/notebook.py` & `laktory-0.1.9/laktory/models/databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/permissions.py` & `laktory-0.1.9/laktory/models/databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/pipeline.py` & `laktory-0.1.9/laktory/models/databricks/pipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/secret.py` & `laktory-0.1.9/laktory/models/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/secretacl.py` & `laktory-0.1.9/laktory/models/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/secretscope.py` & `laktory-0.1.9/laktory/models/databricks/secretscope.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/serviceprincipal.py` & `laktory-0.1.9/laktory/models/databricks/serviceprincipal.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/serviceprincipalrole.py` & `laktory-0.1.9/laktory/models/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/sqlquery.py` & `laktory-0.1.9/laktory/models/databricks/sqlquery.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/user.py` & `laktory-0.1.9/laktory/models/databricks/user.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/userrole.py` & `laktory-0.1.9/laktory/models/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/warehouse.py` & `laktory-0.1.9/laktory/models/databricks/warehouse.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/databricks/workspacefile.py` & `laktory-0.1.9/laktory/models/databricks/workspacefile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/dataevent.py` & `laktory-0.1.9/laktory/models/dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/dataeventheader.py` & `laktory-0.1.9/laktory/models/dataeventheader.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/dataproducer.py` & `laktory-0.1.9/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/datasources/basedatasource.py` & `laktory-0.1.9/laktory/models/datasources/basedatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/datasources/eventdatasource.py` & `laktory-0.1.9/laktory/models/datasources/eventdatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/datasources/tabledatasource.py` & `laktory-0.1.9/laktory/models/datasources/tabledatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/__init__.py` & `laktory-0.1.9/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/cataloggrant.py` & `laktory-0.1.9/laktory/models/grants/cataloggrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/connectiongrant.py` & `laktory-0.1.9/laktory/models/grants/connectiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/externallocationgrant.py` & `laktory-0.1.9/laktory/models/grants/externallocationgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/functiongrant.py` & `laktory-0.1.9/laktory/models/grants/functiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/metastoregrant.py` & `laktory-0.1.9/laktory/models/grants/metastoregrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.1.9/laktory/models/grants/registeredmodelgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/schemagrant.py` & `laktory-0.1.9/laktory/models/grants/schemagrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/sharegrant.py` & `laktory-0.1.9/laktory/models/grants/sharegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.1.9/laktory/models/grants/storagecredentialgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/tablegrant.py` & `laktory-0.1.9/laktory/models/grants/tablegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/viewgrant.py` & `laktory-0.1.9/laktory/models/grants/viewgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/grants/volumegrant.py` & `laktory-0.1.9/laktory/models/grants/volumegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/providers/awsprovider.py` & `laktory-0.1.9/laktory/models/providers/awsprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/providers/azureprovider.py` & `laktory-0.1.9/laktory/models/providers/azureprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/providers/azurepulumiprovider.py` & `laktory-0.1.9/laktory/models/providers/azurepulumiprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/providers/baseprovider.py` & `laktory-0.1.9/laktory/models/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/providers/databricksprovider.py` & `laktory-0.1.9/laktory/models/providers/databricksprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/resources/baseresource.py` & `laktory-0.1.9/laktory/models/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/resources/pulumiresource.py` & `laktory-0.1.9/laktory/models/resources/pulumiresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/resources/terraformresource.py` & `laktory-0.1.9/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/catalog.py` & `laktory-0.1.9/laktory/models/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/column.py` & `laktory-0.1.9/laktory/models/sql/column.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,17 @@
         Name of the catalog string the column table
     comment:
         Text description of the column
     name:
         Name of the column
     pii:
         If `True`, the column is flagged as Personally Identifiable Information
+    raise_missing_arg_exception:
+        If `True`, an exception is raised when one of the spark function
+        argument is missing. Otherwise, only warning is issued.
     schema_name:
         Name of the schema storing the column table
     spark_func_args:
         List of arguments to be passed to the spark function to build the
         column.
     spark_func_kwargs:
         List of keyword arguments to be passed to the spark function to build
@@ -149,14 +152,15 @@
     ```
     """
 
     catalog_name: Union[str, None] = None
     comment: Union[str, None] = None
     name: str
     pii: Union[bool, None] = None
+    raise_missing_arg_exception: Union[bool, None] = True
     schema_name: Union[str, None] = None
     spark_func_args: list[Union[str, SparkFuncArg]] = []
     spark_func_kwargs: dict[str, Union[Any, SparkFuncArg]] = {}
     spark_func_name: Union[str, None] = None
     sql_expression: Union[str, None] = None
     table_name: Union[str, None] = None
     type: str = "string"
@@ -298,30 +302,46 @@
 
         # Build args
         args = []
         for i, _arg in enumerate(_args):
             if df is not None:
                 if _arg.is_column and not has_column(df, _arg.value):
                     logger.info(f"Column '{_arg.value}' not available")
-                    if raise_exception:
-                        raise ValueError(
-                            f"Input column {_args} for {self.name} is not available"
-                        )
+
+                    if self.raise_missing_arg_exception:
+                        if raise_exception:
+                            raise ValueError(
+                                f"Input column {_arg.value} missing. Abort building {self.name}."
+                            )
+                        else:
+                            logger.info(
+                                f"Input column {_arg.value} missing. Skip building {self.name}"
+                            )
+                            return None
                     else:
-                        logger.info("Input columns not available. Skipping")
-                        return None
+                        continue
 
             args += [_arg.to_spark()]
 
+        if len(_args) > 0 and len(args) < 1:
+            if raise_exception:
+                raise ValueError(
+                    f"All input columns are  missing. Abort building {self.name}"
+                )
+            else:
+                logger.info(f"All input columns are missing. Skip building {self.name}")
+                return None
+
         # Build kwargs
         kwargs = {}
         for k, _arg in _kwargs.items():
             kwargs[k] = _arg.to_spark()
 
         # Function call
+        logger.info(f"   {self.name}[{self.type}] as {func_name}({args}, {kwargs})")
         col = f(*args, **kwargs)
 
         # Type Casting
         if self.type not in ["_any"]:
             col = col.cast(self.type)
 
         return col
```

### Comparing `laktory-0.1.8/laktory/models/sql/schema.py` & `laktory-0.1.9/laktory/models/sql/schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/table.py` & `laktory-0.1.9/laktory/models/sql/table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/tableaggregation.py` & `laktory-0.1.9/laktory/models/sql/tableaggregation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/tablebuilder.py` & `laktory-0.1.9/laktory/models/sql/tablebuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from laktory.models.basemodel import BaseModel
 from laktory.models.datasources.basedatasource import BaseDataSource
 from laktory.models.datasources import EventDataSource
 from laktory.models.datasources import TableDataSource
 from laktory.models.sql.column import Column
 from laktory.models.sql.tableaggregation import TableAggregation
 from laktory.models.sql.tablejoin import TableJoin
+from laktory.models.sql.tableunion import TableUnion
 from laktory.models.sql.tablewindowfilter import TableWindowFilter
 from laktory.spark import DataFrame
 
 logger = get_logger(__name__)
 
 
 class TableBuilder(BaseModel):
@@ -57,14 +58,16 @@
         Columns to select from the output dataframe. A list of colum names or
         a map for renaming the columns.
     table_source:
         Definition of the table data source if applicable
     template:
         Key indicating which notebook to use for building the table in the
         context of a data pipeline.
+    unions:
+        Definition of the table(s) to be unioned to the data source
     window_filter:
         Definition of rows filter based on a time spark window. Applied after
         joins.
     """
 
     aggregation: Union[TableAggregation, None] = None
     as_dlt_view: bool = False
@@ -76,14 +79,15 @@
     joins: list[TableJoin] = []
     joins_post_aggregation: list[TableJoin] = []
     layer: Literal["BRONZE", "SILVER", "SILVER_STAR", "GOLD"] = None
     pipeline_name: Union[str, None] = None
     selects: Union[list[str], dict[str, str], None] = None
     table_source: Union[TableDataSource, None] = None
     template: Union[str, bool, None] = None
+    unions: list[TableUnion] = []
     window_filter: Union[TableWindowFilter, None] = None
     _columns_to_build = []
     _table: Any = None
 
     @model_validator(mode="after")
     def default_options(self) -> Any:
         """
@@ -156,14 +160,24 @@
 
     @property
     def has_joins(self) -> bool:
         """Joins defined flag"""
         return len(self.joins) > 0
 
     @property
+    def has_unions(self) -> bool:
+        """Unions defined flag"""
+        return len(self.unions) > 0
+
+    @property
+    def has_aggregation(self) -> bool:
+        """Has aggregation"""
+        return self.aggregation is not None
+
+    @property
     def has_joins_post_aggregation(self) -> bool:
         """Post-aggregation joins defined flag"""
         return len(self.joins_post_aggregation) > 0
 
     def _get_layer_columns(self, layer, df=None) -> list[columns]:
         from laktory.spark.dataframe import has_column
 
@@ -304,57 +318,83 @@
             output Spark DataFrame
         """
         import pyspark.sql.functions as F
 
         logger.info(f"Applying {self.layer} transformations")
 
         # Build columns
-        self._columns_to_build = self.columns + self._get_layer_columns(
-            layer=self.layer, df=df
-        )
+        self._columns_to_build = [c for c in self.columns]
         column_names = [c.name for c in self._columns_to_build]
         df = self.build_columns(
-            df, udfs=udfs, raise_exception=not (self.has_joins or self.aggregation)
+            df, udfs=udfs, raise_exception=not (self.has_joins or self.has_aggregation)
         )
 
-        # Make joins
+        # Execute unions
+        logger.info(f"Executing unions...")
+        for i, union in enumerate(self.unions):
+            if i == 0:
+                name = self.source.name
+            else:
+                name = "previous_union"
+            union.left = TableDataSource(name=name)
+            union.left._df = df
+            df = union.execute(spark)
+
+        # Execute joins
+        logger.info(f"Executing joins...")
         for i, join in enumerate(self.joins):
             if i == 0:
                 name = self.source.name
             else:
                 name = "previous_join"
             join.left = TableDataSource(name=name)
             join.left._df = df
             df = join.execute(spark)
 
             # Build remaining columns again (in case inputs are found in joins)
             df = self.build_columns(
                 df, udfs=udfs, raise_exception=i == len(self.joins) - 1
             )
 
+        # Add layer columns
+        logger.info(f"Adding layer columns...")
+        layer_columns = self._get_layer_columns(layer=self.layer, df=df)
+        self._columns_to_build += layer_columns
+        column_names += [c.name for c in layer_columns]
+        df = self.build_columns(
+            df,
+            udfs=udfs,
+            raise_exception=not (
+                self.has_joins_post_aggregation or self.has_aggregation
+            ),
+        )
+
         # Window filtering
         if self.window_filter:
+            logger.info(f"Window filtering...")
             df = self.window_filter.execute(df)
 
         # Drop source columns
         if self.drop_source_columns:
             logger.info(f"Dropping source columns...")
             df = df.select(column_names)
 
         if self.aggregation:
+            logger.info(f"Executing Aggregations...")
             df = self.aggregation.execute(df, udfs=udfs)
             self._columns_to_build += self._get_layer_columns(layer=self.layer, df=df)
 
         # Build columns after aggregation
         df = self.build_columns(
             df, udfs=udfs, raise_exception=not self.has_joins_post_aggregation
         )
 
         # Make post-aggregation joins
         for i, join in enumerate(self.joins_post_aggregation):
+            logger.info(f"Post-aggregation joins...")
             if i == 0:
                 name = self.source.name
             else:
                 name = "previous_join"
             join.left = TableDataSource(name=name)
             join.left._df = df
             df = join.execute(spark)
@@ -367,14 +407,15 @@
         # Apply filter
         if self.filter:
             df = df.filter(self.filter)
 
         # Select columns
         cols = []
         if self.selects:
+            logger.info(f"Selecting columns...")
             if isinstance(self.selects, list):
                 cols += [F.col(c) for c in self.selects]
             elif isinstance(self.selects, dict):
                 cols += [F.col(k).alias(v) for k, v in self.selects.items()]
             df = df.select(cols)
 
         # Drop columns
```

### Comparing `laktory-0.1.8/laktory/models/sql/tableexpectation.py` & `laktory-0.1.9/laktory/models/sql/tableexpectation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/tablejoin.py` & `laktory-0.1.9/laktory/models/sql/tablejoin.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/tablewindowfilter.py` & `laktory-0.1.9/laktory/models/sql/tablewindowfilter.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/sql/volume.py` & `laktory-0.1.9/laktory/models/sql/volume.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/stacks/pulumistack.py` & `laktory-0.1.9/laktory/models/stacks/pulumistack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/stacks/stack.py` & `laktory-0.1.9/laktory/models/stacks/stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/models/stacks/terraformstack.py` & `laktory-0.1.9/laktory/models/stacks/terraformstack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/resources/data/stock_prices.json` & `laktory-0.1.9/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/resources/notebooks/dlt_brz_template.py` & `laktory-0.1.9/laktory/resources/notebooks/dlt_brz_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/resources/notebooks/dlt_gld_template.py` & `laktory-0.1.9/laktory/resources/notebooks/dlt_gld_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/resources/notebooks/dlt_slv_star_template.py` & `laktory-0.1.9/laktory/resources/notebooks/dlt_slv_star_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/resources/notebooks/dlt_slv_template.py` & `laktory-0.1.9/laktory/resources/notebooks/dlt_slv_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/dataframe/__init__.py` & `laktory-0.1.9/laktory/spark/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/dataframe/has_column.py` & `laktory-0.1.9/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/dataframe/schema_flat.py` & `laktory-0.1.9/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/dataframe/show_string.py` & `laktory-0.1.9/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/functions/_common.py` & `laktory-0.1.9/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/functions/logical.py` & `laktory-0.1.9/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/spark/functions/math.py` & `laktory-0.1.9/laktory/spark/functions/string.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,102 @@
 import pyspark.sql.functions as F
+
 from pyspark.sql.column import Column
 from laktory.spark.functions._common import (
     COLUMN_OR_NAME,
     INT_OR_COLUMN,
     FLOAT_OR_COLUMN,
     STRING_OR_COLUMN,
     _col,
     _lit,
 )
 
 __all__ = [
-    "poly1",
-    "poly2",
-    "power",
-    "roundp",
+    "string_split",
+    "uuid",
 ]
 
 
 # --------------------------------------------------------------------------- #
-# Polynomials                                                                 #
+# string_split                                                                #
 # --------------------------------------------------------------------------- #
 
 
-def poly1(
+def string_split(
     x: COLUMN_OR_NAME,
-    a: FLOAT_OR_COLUMN = 1.0,
-    b: FLOAT_OR_COLUMN = 0.0,
+    pattern: str,
+    key: int,
 ) -> Column:
     """
-    Polynomial function of first degree
+    Get substring using separator `pat`.
 
     Parameters
     ----------
     x:
-        Input column
-    a:
-        Slope
-    b:
-        y-intercept
+        Input text series to split
+    pattern:
+        String or regular expression to split on. If not specified, split on whitespace.
+    key:
+        Split index to return
 
     Returns
     -------
     :
-        Output column
+        Result
 
     Examples
     --------
     ```py
-    import laktory  # noqa: F401
+    from pyspark.sql import SparkSession
+    import pyspark.sql.functions as F
     import laktory.spark.functions as LF
 
-    df = spark.createDataFrame([[9]], ["x"])
-    df = df.withColumn("y", LF.poly1("x", a=-1, b=2))
-    print(df.show_string())
-    '''
-    +---+---+
-    |  x|  y|
-    +---+---+
-    |  9| -7|
-    +---+---+
-    '''
-    ```
-    """
-    return _lit(a) * _col(x) + _lit(b)
+    spark = SparkSession.builder.getOrCreate()
 
-
-def poly2(
-    x: COLUMN_OR_NAME,
-    a: FLOAT_OR_COLUMN = 1.0,
-    b: FLOAT_OR_COLUMN = 0.0,
-    c: FLOAT_OR_COLUMN = 0.0,
-) -> Column:
-    """
-    Polynomial function of second degree
-
-    Parameters
-    ------
-    x:
-        Input column
-    a:
-        x**2 coefficient
-    b:
-        x**1 coefficient
-    c:
-        x**0 coefficient
-
-    Returns
-    -------
-    :
-        Output column
-
-
-    Examples
-    --------
-    ```py
-    import laktory.spark.functions as LF
-
-    df = spark.createDataFrame([[9]], ["x"])
-    df = df.withColumn("y", LF.poly2("x", a=-1, b=2))
+    df = spark.range(1).withColumn("x", F.lit("price_close"))
+    df = df.withColumn("y", LF.string_split("x", pattern="_", key=1))
     print(df.show_string())
     '''
-    +---+-----+
-    |  x|    y|
-    +---+-----+
-    |  9|-63.0|
-    +---+-----+
+    +---+-----------+-----+
+    | id|          x|    y|
+    +---+-----------+-----+
+    |  0|price_close|close|
+    +---+-----------+-----+
     '''
     ```
     """
-    return _lit(a) * _col(x) ** 2 + _lit(b) * _col(x) + _lit(c)
+    return F.split(_col(x), pattern=pattern).getItem(key)
 
 
 # --------------------------------------------------------------------------- #
-# Power                                                                       #
+# uuid                                                                        #
 # --------------------------------------------------------------------------- #
 
 
-def power(
-    x: COLUMN_OR_NAME,
-    a: FLOAT_OR_COLUMN = 1.0,
-    n: FLOAT_OR_COLUMN = 0.0,
-) -> Column:
+def uuid() -> Column:
     """
-    Power function
-
-    Parameters
-    ------
-    x:
-        Input column
-    a:
-        Coefficient
-    n:
-        Exponent
+    Create a unique id for each row.
 
     Returns
     -------
     :
         Output column
 
-
     Examples
     --------
     ```py
     import laktory.spark.functions as LF
 
-    df = spark.createDataFrame([[9]], ["x"])
-    df = df.withColumn("y", LF.power("x", a=-3, n=2))
-    print(df.show_string())
-    '''
-    +---+------+
-    |  x|     y|
-    +---+------+
-    |  9|-243.0|
-    +---+------+
-    '''
-    ```
-    """
-    return _lit(a) * _col(x) ** _lit(n)
-
-
-# --------------------------------------------------------------------------- #
-# Rounding                                                                    #
-# --------------------------------------------------------------------------- #
-
-
-def roundp(
-    x: COLUMN_OR_NAME,
-    p: FLOAT_OR_COLUMN = 1.0,
-) -> Column:
-    """
-    Evenly round to the given precision
-
-    Parameters
-    ------
-    x:
-        Input column
-    p:
-        Precision
-
-    Returns
-    -------
-    :
-        Output column
-
-    Examples
-    --------
-    ```py
-    import laktory.spark.functions as LF
-
-    df = spark.createDataFrame([[0.781], [13.0]], ["x"])
-    df = df.withColumn("y", LF.roundp("x", p=5))
-    print(df.show_string())
-    '''
-    +-----+----+
-    |    x|   y|
-    +-----+----+
-    |0.781| 0.0|
-    | 13.0|15.0|
-    +-----+----+
-    '''
-
-    df = df.withColumn("y", LF.roundp("x", p=0.25))
-    print(df.show_string())
+    df = spark.range(3)
+    df = df.withColumn("uuid", LF.uuid())
     '''
-    +-----+----+
-    |    x|   y|
-    +-----+----+
-    |0.781|0.75|
-    | 13.0|13.0|
-    +-----+----+
+    +---+--------------------+
+    | id|                uuid|
+    +---+--------------------+
+    |  0|acc0b53e-a36f-4f8...|
+    |  1|56cdeb41-6828-486...|
+    |  2|64a7d2bf-5e1d-41a...|
+    +---+--------------------+
     '''
     ```
     """
-    # eps0 = 1.0e-16
-    # precision = float(precision)
-    # if precision < eps0:
-    #     raise ValueError("Precision must be greater than 1.0e-16")
-    return F.round(_col(x) / _lit(p)) * _lit(p)
+    return F.expr("uuid()")
```

### Comparing `laktory-0.1.8/laktory/spark/functions/units.py` & `laktory-0.1.9/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory/version.py` & `laktory-0.1.9/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/laktory.egg-info/PKG-INFO` & `laktory-0.1.9/laktory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.1.8/laktory.egg-info/SOURCES.txt` & `laktory-0.1.9/laktory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,24 @@
 docs/api/models/stacks/pulumistack.md
 docs/api/models/stacks/stack.md
 docs/api/models/stacks/terraformstack.md
 docs/api/spark/dataframe/has_column.md
 docs/api/spark/dataframe/schema_flat.md
 docs/api/spark/dataframe/show_string.md
 docs/api/spark/functions/_constants.md
+docs/api/spark/functions/add.md
 docs/api/spark/functions/convert_units.md
+docs/api/spark/functions/div.md
+docs/api/spark/functions/mul.md
 docs/api/spark/functions/poly1.md
 docs/api/spark/functions/poly2.md
-docs/api/spark/functions/power.md
 docs/api/spark/functions/roundp.md
+docs/api/spark/functions/scaled_power.md
 docs/api/spark/functions/string_split.md
+docs/api/spark/functions/sub.md
 docs/api/spark/functions/uuid.md
 docs/concepts/cli.md
 docs/concepts/dataevent.md
 docs/concepts/deployment.md
 docs/concepts/design.md
 docs/concepts/governance.md
 docs/concepts/models.md
@@ -116,14 +120,15 @@
 docs/images/logo_sg.png
 docs/images/logo_sg_ltb.png
 docs/images/logo_sw.png
 docs/images/logo_sw_ltw.png
 docs/images/medaillon_complex.png
 docs/images/medallion.png
 docs/images/okube.png
+docs/images/pl_quickstart.png
 docs/images/pl_stock_prices.png
 docs/images/pl_stock_prices_simple.png
 docs/images/pulumi.png
 docs/images/stock_prices_lineage.png
 docs/images/table_builder.png
 docs/images/terraform.png
 docs/images/what_is_laktory.png
@@ -215,14 +220,15 @@
 laktory/models/sql/column.py
 laktory/models/sql/schema.py
 laktory/models/sql/table.py
 laktory/models/sql/tableaggregation.py
 laktory/models/sql/tablebuilder.py
 laktory/models/sql/tableexpectation.py
 laktory/models/sql/tablejoin.py
+laktory/models/sql/tableunion.py
 laktory/models/sql/tablewindowfilter.py
 laktory/models/sql/volume.py
 laktory/models/stacks/__init__.py
 laktory/models/stacks/pulumistack.py
 laktory/models/stacks/stack.py
 laktory/models/stacks/terraformstack.py
 laktory/resources/data/stock_prices.json
```

### Comparing `laktory-0.1.8/mkdocs.yml` & `laktory-0.1.9/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -209,20 +209,24 @@
     - Spark:
       - DataFrame:
         - has_column: api/spark/dataframe/has_column.md
         - schema_flat: api/spark/dataframe/schema_flat.md
         - show_string: api/spark/dataframe/show_string.md
       - Functions:
         - constants: api/spark/functions/_constants.md
+        - add: api/spark/functions/add.md
         - convert_units: api/spark/functions/convert_units.md
+        - div: api/spark/functions/div.md
+        - mul: api/spark/functions/mul.md
         - poly1: api/spark/functions/poly1.md
         - poly2: api/spark/functions/poly2.md
-        - power: api/spark/functions/power.md
         - roundp: api/spark/functions/roundp.md
+        - scaled_power: api/spark/functions/scaled_power.md
         - string_split: api/spark/functions/string_split.md
+        - sub: api/spark/functions/sub.md
         - uuid: api/spark/functions/uuid.md
     - DLT:
       - apply_changes: api/dlt/apply_changes.md
       - get_df: api/dlt/get_df.md
       - is_debug: api/dlt/is_debug.md
       - is_mocked: api/dlt/is_mocked.md
       - read: api/dlt/read.md
```

### Comparing `laktory-0.1.8/pyproject.toml` & `laktory-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/stack.yaml` & `laktory-0.1.9/tests/stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_basemodel.py` & `laktory-0.1.9/tests/test_basemodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,15 @@
                 "builder": {
                     "aggregation": None,
                     "filter": None,
                     "joins": [],
                     "layer": None,
                     "selects": None,
                     "template": None,
+                    "unions": [],
                     "asDltView": False,
                     "dropColumns": [],
                     "dropDuplicates": None,
                     "dropSourceColumns": None,
                     "eventSource": None,
                     "joinsPostAggregation": [],
                     "pipelineName": None,
@@ -128,14 +129,15 @@
                     {
                         "comment": None,
                         "name": "open",
                         "pii": None,
                         "type": "double",
                         "unit": None,
                         "catalogName": None,
+                        "raiseMissingArgException": True,
                         "schemaName": None,
                         "sparkFuncArgs": [],
                         "sparkFuncKwargs": {
                             "window_length": {
                                 "value": 2,
                                 "isColumn": False,
                                 "toLit": True,
@@ -149,14 +151,15 @@
                     {
                         "comment": None,
                         "name": "${resources.close.id}",
                         "pii": None,
                         "type": "double",
                         "unit": None,
                         "catalogName": None,
+                        "raiseMissingArgException": True,
                         "schemaName": None,
                         "sparkFuncArgs": [],
                         "sparkFuncKwargs": {},
                         "sparkFuncName": None,
                         "sqlExpression": None,
                         "tableName": "AAPL",
                     },
@@ -179,14 +182,15 @@
                 "builder": {
                     "aggregation": None,
                     "filter": None,
                     "joins": [],
                     "layer": None,
                     "selects": None,
                     "template": None,
+                    "unions": [],
                     "asDltView": False,
                     "dropColumns": [],
                     "dropDuplicates": None,
                     "dropSourceColumns": None,
                     "eventSource": None,
                     "joinsPostAggregation": [],
                     "pipelineName": None,
@@ -197,28 +201,30 @@
                     {
                         "comment": None,
                         "name": "${vars.dynamic_column}",
                         "pii": None,
                         "type": "double",
                         "unit": None,
                         "catalogName": None,
+                        "raiseMissingArgException": True,
                         "schemaName": None,
                         "sparkFuncArgs": [],
                         "sparkFuncKwargs": {},
                         "sparkFuncName": None,
                         "sqlExpression": None,
                         "tableName": "GOOGL",
                     },
                     {
                         "comment": None,
                         "name": "high",
                         "pii": None,
                         "type": "double",
                         "unit": None,
                         "catalogName": None,
+                        "raiseMissingArgException": True,
                         "schemaName": None,
                         "sparkFuncArgs": [],
                         "sparkFuncKwargs": {},
                         "sparkFuncName": None,
                         "sqlExpression": None,
                         "tableName": "GOOGL",
                     },
```

### Comparing `laktory-0.1.8/tests/test_baseresource.py` & `laktory-0.1.9/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_catalog.py` & `laktory-0.1.9/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_cli.py` & `laktory-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_column.py` & `laktory-0.1.9/tests/test_column.py`

 * *Files 19% similar despite different names*

```diff
@@ -154,14 +154,60 @@
     )
     cs = c.to_spark(df)
     s = df.withColumn(c.name, cs).toPandas()[c.name].tolist()
     assert cs.__repr__() == "Column<'regexp_replace(data.symbol, O, 0, 1)'>"
     assert s == ["G00GL", "G00GL", "G00GL", "G00GL", "G00GL"]
 
 
+def test_spark_missing_column():
+    # All columns are missing
+    with pytest.raises(ValueError):
+        c = Column(name="x", spark_func_args=("x",)).to_spark(df)
+
+    # Single column is missing
+    with pytest.raises(ValueError):
+        c = Column(
+            name="x",
+            spark_func_args=(
+                "name",
+                "x",
+            ),
+        ).to_spark(df)
+
+    # One column is missing, but missing is allowed
+    c = Column(
+        name="x",
+        spark_func_args=(
+            "name",
+            "x",
+        ),
+        raise_missing_arg_exception=False,
+    )
+    cs = c.to_spark(df)
+    s = df.withColumn(c.name, cs).toPandas()[c.name].tolist()
+    assert s == [
+        "stock_price",
+        "stock_price",
+        "stock_price",
+        "stock_price",
+        "stock_price",
+    ]
+
+    # Missing are allowed, but all inputs are missing
+    with pytest.raises(ValueError):
+        c = Column(
+            name="x",
+            spark_func_args=(
+                "m1",
+                "m2",
+            ),
+            raise_missing_arg_exception=False,
+        ).to_spark(df)
+
+
 def test_spark_udf():
     def x2(x):
         return 2 * x
 
     def x_square(x):
         return x * x
 
@@ -185,8 +231,9 @@
     ]
 
 
 if __name__ == "__main__":
     test_model()
     test_read()
     test_spark()
+    test_spark_missing_column()
     test_spark_udf()
```

### Comparing `laktory-0.1.8/tests/test_dataevent.py` & `laktory-0.1.9/tests/test_dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_datasources.py` & `laktory-0.1.9/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_dbfsfile.py` & `laktory-0.1.9/tests/test_dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_docstrings.py` & `laktory-0.1.9/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_job.py` & `laktory-0.1.9/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_metastore.py` & `laktory-0.1.9/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_notebook.py` & `laktory-0.1.9/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_parsers.py` & `laktory-0.1.9/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_pipeline.py` & `laktory-0.1.9/tests/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                     "joins": [],
                     "joins_post_aggregation": [],
                     "layer": "BRONZE",
                     "pipeline_name": "pl-stock-prices",
                     "selects": None,
                     "table_source": None,
                     "template": "BRONZE",
+                    "unions": [],
                     "window_filter": None,
                 },
                 "catalog_name": None,
                 "columns": [],
                 "comment": None,
                 "data": None,
                 "data_source_format": "DELTA",
@@ -92,23 +93,25 @@
                         "from_pipeline": True,
                         "name": "brz_stock_prices",
                         "path": None,
                         "schema_name": "markets",
                         "watermark": None,
                     },
                     "template": "SILVER",
+                    "unions": [],
                     "window_filter": None,
                 },
                 "catalog_name": None,
                 "columns": [
                     {
                         "catalog_name": None,
                         "comment": None,
                         "name": "created_at",
                         "pii": None,
+                        "raise_missing_arg_exception": True,
                         "schema_name": None,
                         "spark_func_args": [
                             {
                                 "value": "data._created_at",
                                 "is_column": True,
                                 "to_lit": False,
                                 "to_expr": True,
@@ -122,14 +125,15 @@
                         "unit": None,
                     },
                     {
                         "catalog_name": None,
                         "comment": None,
                         "name": "symbol",
                         "pii": None,
+                        "raise_missing_arg_exception": True,
                         "schema_name": None,
                         "spark_func_args": [
                             {
                                 "value": "data.symbol",
                                 "is_column": True,
                                 "to_lit": False,
                                 "to_expr": True,
@@ -143,14 +147,15 @@
                         "unit": None,
                     },
                     {
                         "catalog_name": None,
                         "comment": None,
                         "name": "open",
                         "pii": None,
+                        "raise_missing_arg_exception": True,
                         "schema_name": None,
                         "spark_func_args": [
                             {
                                 "value": "data.open",
                                 "is_column": True,
                                 "to_lit": False,
                                 "to_expr": True,
@@ -164,14 +169,15 @@
                         "unit": None,
                     },
                     {
                         "catalog_name": None,
                         "comment": None,
                         "name": "close",
                         "pii": None,
+                        "raise_missing_arg_exception": True,
                         "schema_name": None,
                         "spark_func_args": [],
                         "spark_func_kwargs": {},
                         "spark_func_name": None,
                         "sql_expression": "data.open",
                         "table_name": "slv_stock_prices",
                         "type": "double",
```

### Comparing `laktory-0.1.8/tests/test_schema.py` & `laktory-0.1.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_settings.py` & `laktory-0.1.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_spark_dataframe.py` & `laktory-0.1.9/tests/test_spark_dataframe.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_spark_functions.py` & `laktory-0.1.9/tests/test_spark_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     assert pdf["poly1_1"].tolist() == [0, -1, -2]
     assert pdf["poly1_2"].tolist() == [3, -2, 5]
     assert pdf["poly1_2"].tolist() == [3, -2, 5]
     assert pdf["poly2"].tolist() == [0, 3, 8]
 
 
 def test_power(df0=df0):
-    df = df0.withColumn("power", LF.power("x", n=F.col("b")))
+    df = df0.withColumn("power", LF.scaled_power("x", n=F.col("b")))
     pdf = df.toPandas()
 
     assert pdf["power"].tolist() == [1, 1, 9]
 
 
 def test_roundp(df0=df0):
     df = df0.withColumn("roundp_1", LF.roundp("pi", p=0.2))
```

### Comparing `laktory-0.1.8/tests/test_sql_query.py` & `laktory-0.1.9/tests/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_stack.py` & `laktory-0.1.9/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.8/tests/test_table.py` & `laktory-0.1.9/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,25 @@
                 "from_pipeline": True,
                 "name": "brz_stock_prices",
                 "path": None,
                 "schema_name": "markets",
                 "watermark": None,
             },
             "template": "SILVER",
+            "unions": [],
             "window_filter": None,
         },
         "catalog_name": "dev",
         "columns": [
             {
                 "catalog_name": "dev",
                 "comment": None,
                 "name": "created_at",
                 "pii": None,
+                "raise_missing_arg_exception": True,
                 "schema_name": "markets",
                 "spark_func_args": [
                     {
                         "value": "data._created_at",
                         "is_column": True,
                         "to_lit": False,
                         "to_expr": True,
@@ -78,14 +80,15 @@
                 "unit": None,
             },
             {
                 "catalog_name": "dev",
                 "comment": None,
                 "name": "symbol",
                 "pii": None,
+                "raise_missing_arg_exception": True,
                 "schema_name": "markets",
                 "spark_func_args": [
                     {
                         "value": "data.symbol",
                         "is_column": True,
                         "to_lit": False,
                         "to_expr": True,
@@ -99,14 +102,15 @@
                 "unit": None,
             },
             {
                 "catalog_name": "dev",
                 "comment": None,
                 "name": "open",
                 "pii": None,
+                "raise_missing_arg_exception": True,
                 "schema_name": "markets",
                 "spark_func_args": [
                     {
                         "value": "data.open",
                         "is_column": True,
                         "to_lit": False,
                         "to_expr": True,
@@ -120,14 +124,15 @@
                 "unit": None,
             },
             {
                 "catalog_name": "dev",
                 "comment": None,
                 "name": "close",
                 "pii": None,
+                "raise_missing_arg_exception": True,
                 "schema_name": "markets",
                 "spark_func_args": [],
                 "spark_func_kwargs": {},
                 "spark_func_name": None,
                 "sql_expression": "data.open",
                 "table_name": "slv_stock_prices",
                 "type": "double",
@@ -360,23 +365,25 @@
                 "from_pipeline": True,
                 "name": "slv_stock_prices",
                 "path": None,
                 "schema_name": "markets",
                 "watermark": None,
             },
             "template": "SILVER_STAR",
+            "unions": [],
             "window_filter": None,
         },
         "catalog_name": "dev",
         "columns": [
             {
                 "catalog_name": "dev",
                 "comment": None,
                 "name": "symbol3",
                 "pii": None,
+                "raise_missing_arg_exception": True,
                 "schema_name": "markets",
                 "spark_func_args": [
                     {
                         "value": "symbol",
                         "is_column": True,
                         "to_lit": False,
                         "to_expr": True,
```

### Comparing `laktory-0.1.8/tests/test_table_builder.py` & `laktory-0.1.9/tests/test_table_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import pytest
 from pyspark.sql import types as T
 from pyspark.sql import functions as F
 from pyspark.sql import SparkSession
 import pandas as pd
 import datetime
 
 from laktory._testing import EventsManager
 from laktory._testing import df_meta
 from laktory._testing import table_brz
 from laktory._testing import table_slv
 from laktory._testing import table_slv_star
 from laktory._testing import table_gld
 from laktory.models import Table
 from laktory.models import TableJoin
+from laktory.models import TableUnion
 from laktory.models import TableWindowFilter
 from laktory.models import TableAggregation
 
 manager = EventsManager()
 manager.build_events()
 
 # Spark
@@ -163,14 +165,73 @@
             "currency": "USD",
             "first_traded": "2004-08-19T13:30:00.00Z",
             "symbol": "GOOGL",
         },
     ]
 
 
+def test_table_union():
+    join = TableUnion(
+        left={
+            "name": "slv_stock_prices",
+        },
+        other={
+            "name": "slv_stock_prices",
+        },
+    )
+    join.left._df = table_slv.to_df(spark)
+    join.other._df = table_slv.to_df(spark)
+
+    df = join.execute(spark)
+    data = df.toPandas().to_dict(orient="records")
+    print(data[:4])
+    assert (
+        data
+        == [
+            {
+                "created_at": "2023-11-01T00:00:00Z",
+                "symbol": "AAPL",
+                "open": 1,
+                "close": 2,
+            },
+            {
+                "created_at": "2023-11-01T01:00:00Z",
+                "symbol": "AAPL",
+                "open": 3,
+                "close": 4,
+            },
+            {
+                "created_at": "2023-11-01T00:00:00Z",
+                "symbol": "GOOGL",
+                "open": 3,
+                "close": 4,
+            },
+            {
+                "created_at": "2023-11-01T01:00:00Z",
+                "symbol": "GOOGL",
+                "open": 5,
+                "close": 6,
+            },
+        ]
+        * 2
+    )
+
+    # slv_tmp.builder.drop_duplicates = True
+    # df2 = slv_tmp.builder.process(df1)
+    # df2.show()
+    #
+    # # Remove duplicates using only symbol and _bronze_at
+    # slv_tmp.builder.drop_duplicates = ["symbol", "_bronze_at"]
+    # df3 = slv_tmp.builder.process(df1)
+    #
+    # assert df1.count() == 160
+    # assert df2.count() == 80
+    # assert df3.count() == 4
+
+
 def test_table_agg():
     agg = TableAggregation(
         groupby_columns=["symbol"],
         agg_expressions=[
             {"name": "min_open", "spark_func_name": "min", "spark_func_args": ["open"]},
             {
                 "name": "max_open",
@@ -380,14 +441,99 @@
     df3 = slv_tmp.builder.process(df1)
 
     assert df1.count() == 160
     assert df2.count() == 80
     assert df3.count() == 4
 
 
+def test_builder_agg():
+    # Get Data
+    df0 = manager.to_spark_df()
+    df1 = table_brz.builder.process(df0)
+    df2 = table_slv.builder.process(df1)
+    df2.show()
+
+    # Set table that needs to aggregate on input column and create new column
+    # on aggregated result
+    table_agg = Table(
+        name="table_agg",
+        catalog_name="dev",
+        schema_name="markets",
+        columns=[
+            {
+                "name": "close_mean_2",
+                "spark_func_name": "scaled_power",
+                "spark_func_args": [
+                    "close_mean",
+                    {
+                        "value": 2,
+                        "to_lit": True,
+                    },
+                    {
+                        "value": 1,
+                        "to_lit": True,
+                    },
+                ],
+            }
+        ],
+        builder={
+            "aggregation": {
+                "groupby_columns": ["symbol"],
+                "agg_expressions": [
+                    {
+                        "name": "close_mean",
+                        "spark_func_name": "mean",
+                        "spark_func_args": ["close"],
+                    },
+                ],
+            }
+        },
+    )
+
+    # Process Data
+    df3 = table_agg.builder.process(df2)
+    df3.show()
+
+    # Test
+    pdf = df3.toPandas()
+    s0 = pdf["close_mean"].tolist()
+    s1 = (0.5 * pdf["close_mean_2"].astype(float)).tolist()
+
+    assert s1 == pytest.approx(s0)
+
+
+def test_builder_union():
+    # Set table using union
+    df0 = manager.to_spark_df()
+    df1 = table_brz.builder.process(df0)
+
+    # Table union
+    table_union = Table(
+        name="table_union",
+        catalog_name="dev",
+        schema_name="markets",
+        builder={
+            "layer": "SILVER",
+            "drop_source_columns": False,
+            "table_source": {
+                "name": "slv_stock_prices",
+            },
+            "unions": [{"other": {"name": "brz_stock_prices"}}],
+        },
+    )
+    table_union.builder.unions[0].other._df = df1
+
+    df1.show()
+
+    df2 = table_union.builder.process(df1)
+    df2.show()
+
+    assert df2.count() == df1.count() * 2
+
+
 def test_cdc():
     table = Table(
         name="brz_users_type1",
         builder={
             "table_source": {
                 "name": "brz_users_cdc",
                 "cdc": {
@@ -432,16 +578,19 @@
     # df_cdc.show()
 
 
 if __name__ == "__main__":
     test_table_join()
     test_table_join_expression()
     test_table_join_outer()
+    test_table_union()
     test_table_agg()
     test_table_agg_window()
     test_table_window_filter()
     test_bronze()
     test_silver()
     test_silver_star()
     test_gold()
     test_cdc()
     test_drop_duplicates()
+    test_builder_union()
+    test_builder_agg()
```

### Comparing `laktory-0.1.8/tests/test_workspacefile.py` & `laktory-0.1.9/tests/test_workspacefile.py`

 * *Files identical despite different names*

