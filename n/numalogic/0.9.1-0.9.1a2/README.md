# Comparing `tmp/numalogic-0.9.1.tar.gz` & `tmp/numalogic-0.9.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1.tar", max compression
+gzip compressed data, was "numalogic-0.9.1a2.tar", max compression
```

## Comparing `numalogic-0.9.1.tar` & `numalogic-0.9.1a2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-17 16:46:22.438792 numalogic-0.9.1/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-17 16:46:22.438792 numalogic-0.9.1/README.md
--rw-r--r--   0        0        0      676 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    15499 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-17 16:46:22.458792 numalogic-0.9.1/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/_config.py
--rw-r--r--   0        0        0     7327 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1709 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2119 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10245 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/tools/types.py
--rw-r--r--   0        0        0     1344 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     1861 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     2600 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-04-17 16:46:22.462792 numalogic-0.9.1/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7328 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2181 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15308 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9297 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5563 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14873 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13722 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5178 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3807 2024-04-17 16:46:22.466792 numalogic-0.9.1/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-04-17 16:46:22.466792 numalogic-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 numalogic-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-22 22:41:41.751486 numalogic-0.9.1a2/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-22 22:41:41.751486 numalogic-0.9.1a2/README.md
+-rw-r--r--   0        0        0      676 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15806 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7510 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2119 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1417 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     3905 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     2250 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     4737 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7349 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15595 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9286 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13821 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5187 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-04-22 22:41:41.779486 numalogic-0.9.1a2/pyproject.toml
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a2/PKG-INFO
```

### Comparing `numalogic-0.9.1/LICENSE` & `numalogic-0.9.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/README.md` & `numalogic-0.9.1a2/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/__init__.py` & `numalogic-0.9.1a2/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/_constants.py` & `numalogic-0.9.1a2/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/backtest/_prom.py` & `numalogic-0.9.1a2/numalogic/backtest/_prom.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from numalogic.backtest._constants import DEFAULT_SEQUENCE_LEN
 from numalogic.config import (
     NumalogicConf,
     ModelFactory,
     PreprocessFactory,
     PostprocessFactory,
     ThresholdFactory,
+    AggregatorConf,
 )
+from numalogic.config._config import AggMethod
 from numalogic.connectors import ConnectorType
 from numalogic.connectors.prometheus import PrometheusFetcher
 from numalogic.tools.data import StreamingDataset, inverse_window
 from numalogic.tools.types import artifact_t
 from numalogic.udfs import UDFFactory, StreamConf, MLPipelineConf
 
 DEFAULT_OUTPUT_DIR = os.path.join(BASE_DIR, ".btoutput")
@@ -234,14 +236,16 @@
 
         n_feat = x_scaled.shape[1]
 
         ds = StreamingDataset(x_scaled, seq_len=self.seq_len, stride=self.nlconf.trainer.ds_stride)
 
         x_recon = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
         raw_scores = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
+        unified_raw_scores = np.zeros((len(ds), 1), dtype=np.float32)
+
         feature_scores = np.zeros((len(ds), n_feat), dtype=np.float32)
         unified_scores = np.zeros((len(ds), 1), dtype=np.float32)
 
         postproc_func = PostprocessFactory().get_instance(self.nlconf.postprocess)
 
         # Model Inference
         for idx, arr in enumerate(ds):
@@ -249,20 +253,25 @@
 
             # TODO support for multivariate thresholding functions
             thresh_out = postproc_udf.compute_threshold(artifacts["threshold_clf"], x_recon[idx])
             raw_scores[idx] = thresh_out
 
             winscores = postproc_udf.compute_feature_scores(
                 raw_scores[idx], self.nlconf.score.window_agg
+            )  # (nfeat,)
+
+            unified_raw_scores[idx] = postproc_udf.compute_unified_score(
+                winscores,
+                AggregatorConf(method=AggMethod.MEAN),
             )
 
             feature_scores[idx] = postproc_udf.compute_postprocess(postproc_func, winscores)
 
-            unified_scores[idx] = postproc_udf.compute_unified_score(
-                feature_scores[idx], self.nlconf.score.feature_agg
+            unified_scores[idx] = postproc_udf.compute_postprocess(
+                postproc_func, unified_raw_scores[idx]
             )
 
         x_recon = self.window_inverse(x_recon)
         raw_scores = self.window_inverse(raw_scores)
 
         feature_scores = np.vstack(
             [
```

### Comparing `numalogic-0.9.1/numalogic/base.py` & `numalogic-0.9.1a2/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/blocks/__init__.py` & `numalogic-0.9.1a2/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/blocks/_base.py` & `numalogic-0.9.1a2/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/blocks/_nn.py` & `numalogic-0.9.1a2/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/blocks/_transform.py` & `numalogic-0.9.1a2/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/blocks/pipeline.py` & `numalogic-0.9.1a2/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/config/__init__.py` & `numalogic-0.9.1a2/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/config/_config.py` & `numalogic-0.9.1a2/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/config/factory.py` & `numalogic-0.9.1a2/numalogic/config/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,28 +47,32 @@
         LogTransformer,
         StaticPowerTransformer,
         TanhScaler,
         DataClipper,
         GaussianNoiseAdder,
         DifferenceTransform,
         FlattenVector,
+        PercentileScaler,
+        ExpMovingAverage
     )
 
     _CLS_MAP: ClassVar[dict] = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
         "RobustScaler": RobustScaler,
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
         "DataClipper": DataClipper,
         "GaussianNoiseAdder": GaussianNoiseAdder,
         "DifferenceTransform": DifferenceTransform,
         "FlattenVector": FlattenVector,
+        "PercentileScaler": PercentileScaler,
+        "ExpMovingAverage": ExpMovingAverage
     }
 
     def get_pipeline_instance(self, objs_info: list[ModelInfo]):
         preproc_clfs = []
         for obj_info in objs_info:
             _clf = self.get_instance(obj_info)
             preproc_clfs.append(_clf)
@@ -78,17 +82,17 @@
             return preproc_clfs[0]
         return make_pipeline(*preproc_clfs)
 
 
 class PostprocessFactory(_ObjectFactory):
     """Factory class to create postprocess instances."""
 
-    from numalogic.transforms import TanhNorm, ExpMovingAverage
+    from numalogic.transforms import TanhNorm, ExpMovingAverage, SigmoidNorm
 
-    _CLS_MAP: ClassVar[dict] = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
+    _CLS_MAP: ClassVar[dict] = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage, "SigmoidNorm": SigmoidNorm}
 
 
 class ThresholdFactory(_ObjectFactory):
     """Factory class to create threshold instances."""
 
     from numalogic.models.threshold import (
         StdDevThreshold,
```

### Comparing `numalogic-0.9.1/numalogic/connectors/__init__.py` & `numalogic-0.9.1a2/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/_base.py` & `numalogic-0.9.1a2/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/_config.py` & `numalogic-0.9.1a2/numalogic/connectors/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1a2/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1a2/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1a2/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/prometheus.py` & `numalogic-0.9.1a2/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/rds/_base.py` & `numalogic-0.9.1a2/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.1a2/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.1a2/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.1a2/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/redis.py` & `numalogic-0.9.1a2/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/connectors/utils/enum.py` & `numalogic-0.9.1a2/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1a2/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1a2/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/threshold/_median.py` & `numalogic-0.9.1a2/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/threshold/_static.py` & `numalogic-0.9.1a2/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/threshold/_std.py` & `numalogic-0.9.1a2/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/vae/base.py` & `numalogic-0.9.1a2/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/vae/layer.py` & `numalogic-0.9.1a2/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1a2/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/monitoring/__init__.py` & `numalogic-0.9.1a2/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/monitoring/metrics.py` & `numalogic-0.9.1a2/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/__init__.py` & `numalogic-0.9.1a2/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/_serialize.py` & `numalogic-0.9.1a2/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/artifact.py` & `numalogic-0.9.1a2/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1a2/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/localcache.py` & `numalogic-0.9.1a2/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1a2/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/registry/redis_registry.py` & `numalogic-0.9.1a2/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/synthetic/__init__.py` & `numalogic-0.9.1a2/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1a2/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1a2/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1a2/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/aggregators.py` & `numalogic-0.9.1a2/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/callbacks.py` & `numalogic-0.9.1a2/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/data.py` & `numalogic-0.9.1a2/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/exceptions.py` & `numalogic-0.9.1a2/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/trainer.py` & `numalogic-0.9.1a2/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/tools/types.py` & `numalogic-0.9.1a2/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/transforms/__init__.py` & `numalogic-0.9.1a2/numalogic/transforms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 # limitations under the License.
 
 """
 Module to provide timeseries transformations needed for preprocessing,
 feature engineering and postprocessing.
 """
 
-from numalogic.transforms._scaler import TanhScaler
+from numalogic.transforms._scaler import TanhScaler, PercentileScaler
 from numalogic.transforms._stateless import (
     LogTransformer,
     StaticPowerTransformer,
     DataClipper,
     GaussianNoiseAdder,
     DifferenceTransform,
     FlattenVector,
 )
 from numalogic.transforms._movavg import ExpMovingAverage, expmov_avg_aggregator
-from numalogic.transforms._postprocess import TanhNorm, tanh_norm
+from numalogic.transforms._postprocess import TanhNorm, tanh_norm, SigmoidNorm
 
 __all__ = [
     "TanhScaler",
     "LogTransformer",
     "StaticPowerTransformer",
     "DataClipper",
     "ExpMovingAverage",
     "expmov_avg_aggregator",
     "TanhNorm",
     "tanh_norm",
     "GaussianNoiseAdder",
     "DifferenceTransform",
     "FlattenVector",
+    "PercentileScaler",
+    "SigmoidNorm"
 ]
```

### Comparing `numalogic-0.9.1/numalogic/transforms/_movavg.py` & `numalogic-0.9.1a2/numalogic/transforms/_movavg.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
+import pandas as pd
 
 from numalogic.base import StatelessTransformer
 from numalogic.tools.exceptions import InvalidDataShapeError
 import numpy.typing as npt
 
 
 def _allow_only_single_feature(data: npt.NDArray[float]) -> None:
@@ -82,64 +83,33 @@
 
     Without bias correction, early values can tend more towards zero, since V(0) = 0
     Bias correction helps inhibit this issue by dividing with (1 - beta**i)
 
     Args:
     ----
         beta: how much weight to give to the previous weighted average
-        bias_correction: flag to perform bias correction (default: true)
-
-    Note: this only supports single feature input array.
 
     Raises
     ------
         ValueError: if beta is not between 0 and 1
     """
 
-    __slots__ = ("beta", "bias_correction")
+    __slots__ = ("alpha",)
 
-    def __init__(self, beta: float, bias_correction: bool = True):
+    def __init__(self, beta: float = 0.5):
         if beta <= 0.0 or beta >= 1.0:
             raise ValueError("beta only accepts values between 0 and 1 (not inclusive)")
-        self.beta = beta
-        self.bias_correction = bias_correction
+        self.alpha = 1.0 - beta
 
-    def transform(self, input_: npt.NDArray[float], **__):
+    def transform(self, input_: npt.NDArray[float], **__) -> npt.NDArray[float]:
         r"""Returns transformed output.
 
         Args:
         ----
             input_: input column vector
 
         Raises
         ------
             InvalidDataShapeError: if input array is not single featured
         """
-        _allow_only_single_feature(input_)
-
-        # alpha is the weight given to the latest element
-        alpha = 1.0 - self.beta
-        n = len(input_)
-
-        theta = input_.reshape(-1, 1)
-        theta_tril = np.multiply(theta.T, np.tril(np.ones((n, n))))
-        powers = np.arange(1, n + 1).reshape(-1, 1)
-
-        # Calculate increasing powers of beta of the form,
-        # [beta, beta**2, .., beta**n]
-        beta_powers = np.power(self.beta, powers)
-
-        # Calculate the array of reciprocals of beta powers of form,
-        # [beta**(-1), beta**(-2), .., beta**(-n)]
-        beta_arr_inv = np.reciprocal(beta_powers)
-
-        # Calculate the summation of the ratio between (theta(i) / beta**i),
-        # [ theta(1)/beta, sum(theta(1)/beta, theta(2)/beta**2), .., ]
-        theta_beta_ratio = theta_tril @ beta_arr_inv
-
-        # Elemental multiply with beta powers
-        exp_avg = alpha * np.multiply(beta_powers, theta_beta_ratio)
-        if not self.bias_correction:
-            return exp_avg
-
-        # Calculate array of 1 / (1 - beta**i) values
-        return np.divide(exp_avg, 1.0 - beta_powers)
+        x_df = pd.DataFrame(input_)
+        return x_df.ewm(alpha=self.alpha).mean().to_numpy(dtype=np.float32)
```

### Comparing `numalogic-0.9.1/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1a2/numalogic/transforms/_postprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,7 +44,17 @@
 
     def __init__(self, scale_factor=10, smooth_factor=10):
         self.scale_factor = scale_factor
         self.smooth_factor = smooth_factor
 
     def transform(self, input_: npt.NDArray[float], **__) -> npt.NDArray[float]:
         return tanh_norm(input_, scale_factor=self.scale_factor, smooth_factor=self.smooth_factor)
+
+
+class SigmoidNorm(StatelessTransformer):
+    def __init__(self, scale_factor: float = 10., smooth_factor: float = 0.5):
+        super().__init__()
+        self.scale_factor = scale_factor
+        self.smooth_factor = smooth_factor
+
+    def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
+        return self.scale_factor / (1.0 + np.exp(5 - (self.smooth_factor * x)))
```

### Comparing `numalogic-0.9.1/numalogic/transforms/_stateless.py` & `numalogic-0.9.1a2/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/README.md` & `numalogic-0.9.1a2/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/__init__.py` & `numalogic-0.9.1a2/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/__main__.py` & `numalogic-0.9.1a2/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/_base.py` & `numalogic-0.9.1a2/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/_config.py` & `numalogic-0.9.1a2/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/_logger.py` & `numalogic-0.9.1a2/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/_metrics.py` & `numalogic-0.9.1a2/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/entities.py` & `numalogic-0.9.1a2/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/factory.py` & `numalogic-0.9.1a2/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1/numalogic/udfs/inference.py` & `numalogic-0.9.1a2/numalogic/udfs/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             datum: Datum object
 
         Returns
         -------
             Messages instance
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
         json_data_payload = orjson.loads(datum.value)
         payload = StreamPayload(**json_data_payload)
         _metric_label_values = (
             payload.metadata["numalogic_opex_tags"]["source"],
             self._vtx,
@@ -117,15 +117,15 @@
             payload.pipeline_id,
         )
         _increment_counter(counter=MSG_IN_COUNTER, labels=_metric_label_values)
 
         _stream_conf = self.get_stream_conf(payload.config_id)
         _conf = _stream_conf.ml_pipelines[payload.pipeline_id]
 
-        log = log_data_payload_values(log, json_data_payload)
+        logger = log_data_payload_values(logger, json_data_payload)
 
         artifact_data, payload = _load_artifact(
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, _conf.numalogic_conf.model.name],
             payload=payload,
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
@@ -133,24 +133,24 @@
         )
 
         # Send training request if artifact loading is not successful
         if not artifact_data:
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
-            log.exception("Artifact model not loaded!")
+            logger.exception("Artifact model not loaded!")
             return msgs
 
         # Perform inference
         try:
             x_inferred = self.compute(artifact_data.artifact, payload.get_data())
             _update_info_metric(x_inferred, payload.metrics, _metric_label_values)
         except RuntimeError:
             _increment_counter(counter=RUNTIME_ERROR_COUNTER, labels=_metric_label_values)
-            log.exception(
+            logger.exception(
                 "Runtime inference error!",
                 keys=payload.composite_keys,
                 metrics=payload.metrics,
             )
             # Send training request if inference fails
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
@@ -170,21 +170,21 @@
             metadata={
                 "model_version": int(artifact_data.extras.get("version")),
                 **payload.metadata,
             },
         )
         # Send trainer message if artifact is stale
         if status == Status.ARTIFACT_STALE:
-            log.info("Inference artifact found is stale")
+            logger.info("Inference artifact found is stale")
             msgs.append(get_trainer_message(keys, _stream_conf, payload, *_metric_label_values))
 
         _increment_counter(counter=MSG_PROCESSED_COUNTER, labels=_metric_label_values)
         msgs.append(Message(keys=keys, value=payload.to_json(), tags=["postprocess"]))
 
-        log.info(
+        logger.info(
             "Successfully inferred!",
             keys=payload.composite_keys,
             metrics=payload.metrics,
             execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
         )
         return msgs
```

### Comparing `numalogic-0.9.1/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1a2/numalogic/udfs/payloadtx.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         # check message sanity
         try:
             data_payload = orjson.loads(datum.value)
         except (orjson.JSONDecodeError, KeyError):  # catch json decode error only
-            log.exception("Error while decoding input json")
+            logger.exception("Error while decoding input json")
             return Messages(Message.to_drop())
 
         _stream_conf = self.get_stream_conf(data_payload["config_id"])
 
         # create a new message for each ML pipeline
         messages = Messages()
         for pipeline in _stream_conf.ml_pipelines:
             data_payload["pipeline_id"] = pipeline
             messages.append(Message(keys=keys, value=orjson.dumps(data_payload)))
 
-        log = log_data_payload_values(log, data_payload)
-        log.info(
+        logger = log_data_payload_values(logger, data_payload)
+        logger.info(
             "Appended pipeline id to the payload",
             keys=keys,
             execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
         )
         return messages
```

### Comparing `numalogic-0.9.1/numalogic/udfs/postprocess.py` & `numalogic-0.9.1a2/numalogic/udfs/postprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
         json_payload = orjson.loads(datum.value)
         payload = StreamPayload(**json_payload)
         _metric_label_values = (
             payload.composite_keys,
             self._vtx,
@@ -107,15 +107,15 @@
 
         # load configs
         _stream_conf = self.get_stream_conf(payload.config_id)
         _conf = _stream_conf.ml_pipelines[payload.pipeline_id]
         thresh_cfg = _conf.numalogic_conf.threshold
         postprocess_cfg = _conf.numalogic_conf.postprocess
 
-        log = log_data_payload_values(log, json_payload)
+        logger = log_data_payload_values(logger, json_payload)
 
         # load artifact
         thresh_artifact, payload = _load_artifact(
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, thresh_cfg.name],
             payload=payload,
             model_registry=self.model_registry,
@@ -131,37 +131,32 @@
             # Send training request if artifact loading is not successful
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
             if _conf.numalogic_conf.score.adjust:
                 msgs.append(get_static_thresh_message(keys, payload))
             return msgs
 
         if payload.header == Header.STATIC_INFERENCE:
-            log.warning("Static inference not supported in postprocess yet")
+            logger.warning("Static inference not supported in postprocess yet")
 
         #  Postprocess payload
         try:
-            # Compute anomaly scores per feature
-            a_features = self.compute(
+            # Compute anomaly scores
+            a_unified, a_features = self.compute(
                 model=thresh_artifact.artifact,
                 input_=payload.get_data(),
                 score_conf=_conf.numalogic_conf.score,
                 postproc_tx=postproc_tx,
             )  # (nfeat,)
 
-            # Compute unified score
-            a_unified = self.compute_unified_score(
-                a_features, feat_agg_conf=_conf.numalogic_conf.score.feature_agg
-            )
-
             # Calculate adjusted unified score
             a_adjusted, y_unified, y_features = self._adjust_score(_conf, a_unified, payload)
 
         except RuntimeError:
             _increment_counter(RUNTIME_ERROR_COUNTER, _metric_label_values)
-            log.exception(
+            logger.exception(
                 "Runtime postprocess error!",
                 uuid=payload.uuid,
                 composite_keys=payload.composite_keys,
                 payload_metrics=payload.metrics,
             )
             # Send training request if postprocess fails
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
@@ -195,15 +190,15 @@
         )
 
         _increment_counter(
             MSG_PROCESSED_COUNTER,
             labels=_metric_label_values,
         )
 
-        log.info(
+        logger.info(
             "Successfully post-processed!",
             composite_keys=out_payload.composite_keys,
             unified_anomaly=out_payload.unified_anomaly,
             a_unified=a_unified,
             y_features=y_features,
             y_unified=y_unified,
             a_features=a_features.tolist(),
@@ -298,44 +293,54 @@
     def compute(
         cls,
         model: artifact_t,
         input_: NDArray[float],
         postproc_tx=None,
         score_conf: Optional[ScoreConf] = None,
         **_,
-    ) -> NDArray[float]:
+    ) -> tuple[float, NDArray[float]]:
         """
         Compute thresholding, window aggregation followed by postprocess.
 
         Args:
         -------
         model: Threshold model instance
         input_: Input data (Shape: seq_len x n_features)
         postproc_tx: Postprocess transform
         score_conf: Score Config
 
         Returns
         -------
-        Output data of shape (n_features, )
+        Tuple of combined/unified score (float), and feature scores of shape (n_features,)
 
         Raises
         ------
             RuntimeError: If threshold model or postproc function fails
         """
         if score_conf is None:
             _struct_log.warning("Score config not provided, using default values")
             score_conf = ScoreConf()
 
-        scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
-        win_scores = cls.compute_feature_scores(
-            scores, win_agg_conf=score_conf.window_agg
+        thresh_scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
+
+        # Aggregate over the sequence length
+        raw_scores = cls.compute_feature_scores(
+            thresh_scores, win_agg_conf=score_conf.window_agg
         )  # (nfeat,)
+
+        # Aggregate over the features
+        unified_raw_score = cls.compute_unified_score(raw_scores, score_conf.feature_agg)  # float
+
         if postproc_tx:
-            win_scores = cls.compute_postprocess(postproc_tx, win_scores)  # (nfeat,)
-        return win_scores  # (nfeat, )
+            # Postprocess the raw scores
+            feature_scores = cls.compute_postprocess(postproc_tx, raw_scores)  # (nfeat,)
+            unified_score = cls.compute_postprocess(postproc_tx, unified_raw_score)  # float
+            return unified_score, feature_scores
+
+        return unified_raw_score, raw_scores
 
     @classmethod
     def compute_threshold(cls, model: artifact_t, input_: NDArray[float]) -> NDArray[float]:
         """
         Compute raw anomaly scores using the threshold model.
 
         Args:
```

### Comparing `numalogic-0.9.1/numalogic/udfs/preprocess.py` & `numalogic-0.9.1a2/numalogic/udfs/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,28 +97,28 @@
 
         Returns
         -------
         Messages instance
 
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         # check message sanity
         try:
             data_payload = orjson.loads(datum.value)
         except (orjson.JSONDecodeError, KeyError):  # catch json decode error only
-            log.exception("Error while decoding input json")
+            logger.exception("Error while decoding input json")
             return Messages(Message.to_drop())
 
         _stream_conf = self.get_stream_conf(data_payload["config_id"])
         _conf = _stream_conf.ml_pipelines[data_payload.get("pipeline_id", "default")]
         raw_df, timestamps = get_df(data_payload=data_payload, stream_conf=_stream_conf)
 
-        log = log_data_payload_values(log, data_payload)
+        logger = log_data_payload_values(logger, data_payload)
 
         source = NUMALOGIC_METRICS
         if (
             "numalogic_opex_tags" in data_payload["metadata"]
             and "source" in data_payload["metadata"]["numalogic_opex_tags"]
         ):
             source = data_payload["metadata"]["numalogic_opex_tags"]["source"]
@@ -130,17 +130,15 @@
             data_payload["config_id"],
             data_payload.get("pipeline_id", "default"),
         )
 
         _increment_counter(counter=MSG_IN_COUNTER, labels=_metric_label_values)
         # Drop message if dataframe shape conditions are not met
         if raw_df.shape[0] < _stream_conf.window_size or raw_df.shape[1] != len(_conf.metrics):
-            log.critical(
-                "Dataframe shape: (%f, %f) conditions not met ", raw_df.shape[0], raw_df.shape[1]
-            )
+            logger.critical("Dataframe shape conditions not met ", raw_df_shape=raw_df.shape)
             _increment_counter(
                 counter=DATASHAPE_ERROR_COUNTER,
                 labels=_metric_label_values,
             )
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=_metric_label_values,
@@ -164,28 +162,28 @@
                 model_registry=self.model_registry,
                 load_latest=LOAD_LATEST,
                 vertex=self._vtx,
             )
             if preproc_artifact:
                 preproc_clf = preproc_artifact.artifact
                 payload = replace(payload, status=Status.ARTIFACT_FOUND)
-                log = log.bind(artifact_source=preproc_artifact.extras.get("source"))
+                logger = logger.bind(artifact_source=preproc_artifact.extras.get("source"))
             else:
                 msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
                 if _conf.numalogic_conf.score.adjust:
                     msgs.append(get_static_thresh_message(keys, payload))
-                log.exception("Artifact model not loaded!")
+                logger.exception("Artifact model not loaded!")
                 return msgs
         # Model will not be in registry
         else:
             # Load configuration for the config_id
             _increment_counter(SOURCE_COUNTER, labels=("config", *_metric_label_values))
             preproc_clf = self._load_model_from_config(_conf.numalogic_conf.preprocess)
             payload = replace(payload, status=Status.ARTIFACT_FOUND)
-            log = log.bind(model_from_config=preproc_clf)
+            logger = logger.bind(model_from_config=preproc_clf)
         try:
             x_scaled = self.compute(model=preproc_clf, input_=payload.get_data())
 
             # make metrics list matching same shape as data
             payload = replace(
                 payload, metrics=_get_updated_metrics(payload.metrics, x_scaled.shape)
             )
@@ -193,27 +191,27 @@
             _update_info_metric(x_scaled, payload.metrics, _metric_label_values)
             payload = replace(
                 payload,
                 data=x_scaled,
                 status=Status.ARTIFACT_FOUND,
                 header=Header.MODEL_INFERENCE,
             )
-            log.info(
+            logger.info(
                 "Successfully preprocessed!",
                 keys=keys,
                 payload_metrics=payload.metrics,
                 x_scaled=np.array2string(x_scaled),
                 execution_time_ms=round((time.perf_counter() - _start_time) * 1000, 4),
             )
         except RuntimeError:
             _increment_counter(
                 counter=RUNTIME_ERROR_COUNTER,
                 labels=_metric_label_values,
             )
-            log.exception(
+            logger.exception(
                 "Runtime preprocess error!",
                 status=Status.RUNTIME_ERROR,
                 payload_metrics=payload.metrics,
                 composite_keys=payload.composite_keys,
             )
             # TODO check again what error is causing this and if retraining is required
             payload = replace(
```

### Comparing `numalogic-0.9.1/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1a2/numalogic/udfs/staticthresh.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,42 +42,42 @@
         Messages instance
         """
         json_data_payload = orjson.loads(datum.value)
         payload = StreamPayload(**json_data_payload)
         conf = self.get_ml_pipeline_conf(payload.config_id, payload.pipeline_id)
         adjust_conf = conf.numalogic_conf.score.adjust
 
-        log = _struct_log.bind(udf_vertex=self._vtx)
-        log = log_data_payload_values(log, json_data_payload)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
+        logger = log_data_payload_values(logger, json_data_payload)
 
         if not adjust_conf:
-            log.warning("No score adjust config found")
+            logger.warning("No score adjust config found")
             return Messages(Message.to_drop())
 
         try:
             y_features = self.compute(
                 input_=payload.get_data(original=True, metrics=list(adjust_conf.upper_limits)),
                 adjust_conf=adjust_conf,
             )
             y_unified = self.compute_unified_score(y_features, adjust_conf.feature_agg)
         except RuntimeError:
-            log.exception("Error occurred while computing static anomaly scores")
+            logger.exception("Error occurred while computing static anomaly scores")
             return Messages(Message.to_drop())
 
         out_payload = OutputPayload(
             uuid=payload.uuid,
             config_id=payload.config_id,
             pipeline_id=payload.pipeline_id,
             composite_keys=payload.composite_keys,
             timestamp=payload.end_ts,
             unified_anomaly=y_unified,
             data=self._additional_scores(adjust_conf, y_features, y_unified),
             metadata=payload.metadata,
         )
-        log.info(
+        logger.info(
             "Sending output payload",
             keys=out_payload.composite_keys,
             y_unified=y_unified,
             y_features=y_features,
         )
         return Messages(Message(keys=keys, value=out_payload.to_json(), tags=["output"]))
```

### Comparing `numalogic-0.9.1/numalogic/udfs/tools.py` & `numalogic-0.9.1a2/numalogic/udfs/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,55 +163,55 @@
         payload.metadata["numalogic_opex_tags"]["source"],
         vertex,
         ":".join(skeys),
         payload.config_id,
         payload.pipeline_id,
     )
 
-    log = _struct_log.bind(
+    logger = _struct_log.bind(
         uuid=payload.uuid, skeys=skeys, dkeys=dkeys, payload_metrics=payload.metrics
     )
 
     version_to_load = "-1"
     if payload.artifact_versions:
         artifact_version = payload.artifact_versions
         key = ":".join(dkeys)
         if key in artifact_version:
             version_to_load = artifact_version[key]
-            log.debug("Found version info for keys")
+            logger.debug("Found version info for keys")
         else:
-            log.debug("Could not find what version of model to load")
+            logger.debug("Could not find what version of model to load")
     else:
-        log.debug(
+        logger.debug(
             "No version info passed on! Loading latest artifact version, "
             "if one present in the registry"
         )
         load_latest = True
     try:
         if load_latest:
             artifact_data = model_registry.load(skeys=skeys, dkeys=dkeys)
         else:
             artifact_data = model_registry.load(
                 skeys=skeys, dkeys=dkeys, latest=False, version=version_to_load
             )
     except RedisRegistryError:
         _increment_counter(REDIS_ERROR_COUNTER, labels=_metric_label_values)
-        log.warning("Error while fetching artifact")
+        logger.warning("Error while fetching artifact")
         return None, payload
 
     except Exception:
         _increment_counter(EXCEPTION_COUNTER, labels=_metric_label_values)
-        log.exception("Unhandled exception while fetching artifact")
+        logger.exception("Unhandled exception while fetching artifact")
         return None, payload
     else:
-        log = log.bind(
+        logger = logger.bind(
             artifact_source=artifact_data.extras.get("source"),
             artifact_version=artifact_data.extras.get("version"),
         )
-        log.debug("Loaded Model!")
+        logger.debug("Loaded Model!")
         _increment_counter(
             counter=SOURCE_COUNTER,
             labels=(artifact_data.extras.get("source"), *_metric_label_values),
         )
         _add_info(
             info=MODEL_INFO,
             labels=(
@@ -291,15 +291,15 @@
         except Exception:
             _struct_log.exception(
                 "Problem while updating _msg_train_records information for the key",
                 uuid=uuid,
                 key=key,
             )
             return False
-        _struct_log.debug("Acknowledging insufficient data for the key", uuid, key)
+        _struct_log.debug("Acknowledging insufficient data for the key", uuid=uuid, key=key)
         return True
 
     def ack_read(
         self,
         key: KEYS,
         uuid: str,
         retrain_freq: int = 24,
@@ -335,18 +335,18 @@
             _msg_train_records
             and _msg_read_ts
             and _curr_time - float(_msg_read_ts)
             < (min_train_records - int(_msg_train_records)) * data_freq
         ):
             _struct_log.debug(
                 "There was insufficient data for the key in the past. Retrying fetching"
-                " and training after %s secs",
-                uuid,
-                key,
-                ((min_train_records - int(_msg_train_records)) * data_freq)
+                " and training after secs",
+                uuid=uuid,
+                key=key,
+                secs=((min_train_records - int(_msg_train_records)) * data_freq)
                 - _curr_time
                 + float(_msg_read_ts),
             )
 
             return False
 
         # Check if the model is being trained by another process
```

### Comparing `numalogic-0.9.1/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1a2/numalogic/udfs/trainer/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             datum: Datum object
 
         Returns
         -------
             Messages instance (no forwarding)
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         # Construct payload object
         json_payload = orjson.loads(datum.value)
         payload = TrainerPayload(**json_payload)
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
@@ -167,15 +167,15 @@
             config_id=payload.config_id, pipeline_id=payload.pipeline_id
         )
         _increment_counter(
             counter=MSG_IN_COUNTER,
             labels=[self._vtx, *_metric_label_values],
         )
 
-        log = log_data_payload_values(log, json_payload)
+        logger = log_data_payload_values(logger, json_payload)
 
         # set the retry and retrain_freq
         retrain_freq_ts = _conf.numalogic_conf.trainer.retrain_freq_hr
         retry_ts = _conf.numalogic_conf.trainer.retry_sec
         if not self.train_msg_deduplicator.ack_read(
             key=[*payload.composite_keys, payload.pipeline_id],
             uuid=payload.uuid,
@@ -196,25 +196,25 @@
         # Retry the training if df is returning None due to some errors/exception
         # while fetching the data
         if df is None:
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=(self._vtx, *_metric_label_values),
             )
-            log.warning(
+            logger.warning(
                 "Caught exception/error while fetching from source",
                 uuid=payload.uuid,
                 keys=payload.composite_keys,
             )
 
             return Messages(Message.to_drop())
 
         # Check if data is sufficient
         if not self._is_data_sufficient(payload, df):
-            log.warning(
+            logger.warning(
                 "Insufficient data found",
                 uuid=payload.uuid,
                 keys=payload.composite_keys,
                 shape=df.shape,
             )
             _increment_counter(
                 counter=INSUFFICIENT_DATA_COUNTER,
@@ -222,15 +222,15 @@
             )
             _increment_counter(
                 counter=MSG_DROPPED_COUNTER,
                 labels=(self._vtx, *_metric_label_values),
             )
             return Messages(Message.to_drop())
 
-        log.debug("Data fetched", uuid=payload.uuid, shape=df.shape)
+        logger.debug("Data fetched", uuid=payload.uuid, shape=df.shape)
 
         # Construct feature array
         x_train, nan_counter, inf_counter = self.get_feature_arr(df, _conf.metrics)
         _add_summary(
             summary=NAN_SUMMARY,
             labels=_metric_label_values,
             data=nan_counter,
@@ -260,22 +260,22 @@
 
         self.artifacts_to_save(
             skeys=payload.composite_keys,
             dict_artifacts=dict_artifacts,
             model_registry=self.model_registry,
             payload=payload,
             vertex_name=self._vtx,
-            log=log,
+            logger=logger,
         )
         if self.train_msg_deduplicator.ack_train(
             key=[*payload.composite_keys, payload.pipeline_id], uuid=payload.uuid
         ):
-            log.info("Model trained and saved successfully", uuid=payload.uuid)
+            logger.info("Model trained and saved successfully", uuid=payload.uuid)
 
-        log.debug(
+        logger.debug(
             "Time taken in trainer", execution_time_secs=round(time.perf_counter() - _start_time, 4)
         )
         _increment_counter(
             counter=MSG_PROCESSED_COUNTER,
             labels=(
                 self._vtx,
                 *_metric_label_values,
@@ -299,15 +299,15 @@
     @staticmethod
     def artifacts_to_save(
         skeys: KEYS,
         dict_artifacts: dict[str, KeyedArtifact],
         model_registry,
         payload: TrainerPayload,
         vertex_name: str,
-        log,
+        logger,
     ) -> None:
         """
         Save artifacts.
         Args:
         _______
         skeys: list keys
         dict_artifacts: artifact_tuple which has dkeys and artifact as fields
@@ -331,18 +331,22 @@
                 uuid=payload.uuid,
             )
         except RedisRegistryError:
             _increment_counter(
                 counter=REDIS_ERROR_COUNTER,
                 labels=(vertex_name, ":".join(payload.composite_keys), payload.config_id),
             )
-            log.exception("Error while saving artifact with skeys", uuid=payload.uuid, skeys=skeys)
+            logger.exception(
+                "Error while saving artifact with skeys", uuid=payload.uuid, skeys=skeys
+            )
 
         else:
-            log.info("Artifact saved with with versions", uuid=payload.uuid, version_dict=ver_dict)
+            logger.info(
+                "Artifact saved with with versions", uuid=payload.uuid, version_dict=ver_dict
+            )
 
     def _is_data_sufficient(self, payload: TrainerPayload, df: pd.DataFrame) -> bool:
         _conf = self.get_ml_pipeline_conf(
             config_id=payload.config_id, pipeline_id=payload.pipeline_id
         )
         if len(df) < _conf.numalogic_conf.trainer.min_train_size:
             _ = self.train_msg_deduplicator.ack_insufficient_data(
```

### Comparing `numalogic-0.9.1/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1a2/numalogic/udfs/trainer/_druid.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             payload: TrainerPayload object
 
         Returns
         -------
             Dataframe
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
@@ -129,24 +129,24 @@
                 hours=_conf.numalogic_conf.trainer.train_hours,
             )
         except DruidFetcherError:
             _increment_counter(
                 counter=FETCH_EXCEPTION_COUNTER,
                 labels=_metric_label_values,
             )
-            log.exception("Error while fetching data from druid")
+            logger.exception("Error while fetching data from druid")
             return None
         _end_time = time.perf_counter() - _start_time
         _add_summary(
             FETCH_TIME_SUMMARY,
             labels=_metric_label_values,
             data=_end_time,
         )
 
-        log.info(
+        logger.info(
             "Fetched data from druid",
             uuid=payload.uuid,
             config_id=payload.config_id,
             pipeline_id=payload.pipeline_id,
             keys=payload.composite_keys,
             df_shape=_df.shape,
             execution_time_ms=round(_end_time * 1000, 4),
```

### Comparing `numalogic-0.9.1/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1a2/numalogic/udfs/trainer/_prom.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             payload: TrainerPayload object
 
         Returns
         -------
             Dataframe
         """
         _start_time = time.perf_counter()
-        log = _struct_log.bind(udf_vertex=self._vtx)
+        logger = _struct_log.bind(udf_vertex=self._vtx)
 
         _metric_label_values = (
             payload.composite_keys,
             ":".join(payload.composite_keys),
             payload.config_id,
             payload.pipeline_id,
         )
@@ -88,23 +88,23 @@
                 },
             )
         except PrometheusFetcherError:
             _increment_counter(
                 counter=FETCH_EXCEPTION_COUNTER,
                 labels=_metric_label_values,
             )
-            log.exception("Error while fetching data from Prometheus", uuid=payload.uuid)
+            logger.exception("Error while fetching data from Prometheus", uuid=payload.uuid)
             return None
         _end_time = time.perf_counter() - _start_time
         _add_summary(
             FETCH_TIME_SUMMARY,
             labels=_metric_label_values,
             data=_end_time,
         )
-        log.info(
+        logger.info(
             "Fetched data from Prometheus",
             uuid=payload.uuid,
             config_id=payload.config_id,
             pipeline_id=payload.pipeline_id,
             keys=payload.composite_keys,
             df_shape=_df.shape,
             execution_time_ms=round(_end_time * 1000, 4),
```

### Comparing `numalogic-0.9.1/pyproject.toml` & `numalogic-0.9.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1"
+version = "0.9.1a2"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -29,22 +29,20 @@
 pandas = { version = "^2.0", extras = ["performance"] }
 scikit-learn = "^1.3"
 omegaconf = "^2.3.0"
 cachetools = "^5.3.0"
 orjson = "^3.9"
 pynumaflow = "~0.6"
 prometheus_client = "^0.18.0"
+structlog = "^24.1.0"
 
 # extras
 mlflow-skinny = { version = "^2.0", optional = true }
 redis = { extras = ["hiredis"], version = "^5.0", optional = true }
 boto3 = { version = "^1.24.64", optional = true }
-
-structlog = "^24.1.0"
-
 pydruid = { version = "^0.6", optional = true }
 PyMySQL = { version = "^1.1.0", optional = true }
 
 
 [tool.poetry.extras]
 mlflow = ["mlflow-skinny"]
 redis = ["redis"]
```

### Comparing `numalogic-0.9.1/PKG-INFO` & `numalogic-0.9.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1
+Version: 0.9.1a2
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

