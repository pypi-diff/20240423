# Comparing `tmp/numalogic-0.9.1a3.tar.gz` & `tmp/numalogic-0.9.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1a3.tar", max compression
+gzip compressed data, was "numalogic-0.9.1a4.tar", max compression
```

## Comparing `numalogic-0.9.1a3.tar` & `numalogic-0.9.1a4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-22 23:47:49.739781 numalogic-0.9.1a3/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-22 23:47:49.739781 numalogic-0.9.1a3/README.md
--rw-r--r--   0        0        0      676 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    15806 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/_config.py
--rw-r--r--   0        0        0     7543 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1709 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2119 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10245 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/types.py
--rw-r--r--   0        0        0     1418 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     2252 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     4772 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7349 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2196 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15595 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9286 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5581 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14920 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13821 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5187 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3816 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-04-22 23:47:49.771782 numalogic-0.9.1a3/pyproject.toml
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 20:28:41.758324 numalogic-0.9.1a4/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-23 20:28:41.758324 numalogic-0.9.1a4/README.md
+-rw-r--r--   0        0        0      676 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15806 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7543 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-23 20:28:41.778324 numalogic-0.9.1a4/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2745 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1418 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     2252 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     4772 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7349 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15595 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9286 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-04-23 20:28:41.782324 numalogic-0.9.1a4/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-23 20:28:41.786324 numalogic-0.9.1a4/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13821 2024-04-23 20:28:41.786324 numalogic-0.9.1a4/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5187 2024-04-23 20:28:41.786324 numalogic-0.9.1a4/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-04-23 20:28:41.786324 numalogic-0.9.1a4/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-04-23 20:28:41.786324 numalogic-0.9.1a4/pyproject.toml
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a4/PKG-INFO
```

### Comparing `numalogic-0.9.1a3/LICENSE` & `numalogic-0.9.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/README.md` & `numalogic-0.9.1a4/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/__init__.py` & `numalogic-0.9.1a4/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/_constants.py` & `numalogic-0.9.1a4/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/backtest/_prom.py` & `numalogic-0.9.1a4/numalogic/backtest/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/base.py` & `numalogic-0.9.1a4/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/blocks/__init__.py` & `numalogic-0.9.1a4/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/blocks/_base.py` & `numalogic-0.9.1a4/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/blocks/_nn.py` & `numalogic-0.9.1a4/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/blocks/_transform.py` & `numalogic-0.9.1a4/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/blocks/pipeline.py` & `numalogic-0.9.1a4/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/config/__init__.py` & `numalogic-0.9.1a4/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/config/_config.py` & `numalogic-0.9.1a4/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/config/factory.py` & `numalogic-0.9.1a4/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/__init__.py` & `numalogic-0.9.1a4/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/_base.py` & `numalogic-0.9.1a4/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/_config.py` & `numalogic-0.9.1a4/numalogic/connectors/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1a4/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1a4/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1a4/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/prometheus.py` & `numalogic-0.9.1a4/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/rds/_base.py` & `numalogic-0.9.1a4/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.1a4/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.1a4/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.1a4/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/redis.py` & `numalogic-0.9.1a4/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/connectors/utils/enum.py` & `numalogic-0.9.1a4/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1a4/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1a4/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1a4/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/threshold/_median.py` & `numalogic-0.9.1a4/numalogic/models/threshold/_median.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,70 @@
 import numpy as np
 import numpy.typing as npt
 from typing_extensions import Self, Final
 
 from numalogic.base import BaseThresholdModel
 from numalogic.tools.exceptions import InvalidDataShapeError, ModelInitializationError
 
+import logging
+
+LOGGER = logging.getLogger(__name__)
 _INLIER: Final[int] = 0
 _OUTLIER: Final[int] = 1
 _INPUT_DIMS: Final[int] = 2
 
 
 class MaxPercentileThreshold(BaseThresholdModel):
     """
     Percentile based Thresholding estimator.
 
     Args:
         max_inlier_percentile: Max percentile greater than which will be treated as outlier
         min_threshold:  Value to be used if threshold is less than this
     """
 
-    __slots__ = ("_max_percentile", "_min_thresh", "_thresh", "_is_fitted")
+    __slots__ = ("_max_percentile", "_min_thresh", "_thresh", "_is_fitted", "_adjust_threshold")
 
     def __init__(
         self,
         max_inlier_percentile: float = 96.0,
         min_threshold: float = 1e-4,
+        adjust_threshold: bool = False,
     ):
         super().__init__()
         self._max_percentile = max_inlier_percentile
         self._min_thresh = min_threshold
         self._thresh = None
         self._is_fitted = False
+        self._adjust_threshold = adjust_threshold
 
     @property
     def threshold(self):
         return self._thresh
 
     @staticmethod
     def _validate_input(x: npt.NDArray[float]) -> None:
         """Validate the input matrix shape."""
         if x.ndim != _INPUT_DIMS:
             raise InvalidDataShapeError(f"Input matrix should have 2 dims, given shape: {x.shape}.")
 
     def fit(self, x: npt.NDArray[float]) -> Self:
         self._validate_input(x)
         self._thresh = np.percentile(x, self._max_percentile, axis=0)
+
+        if self._adjust_threshold:
+            for idx, _ in enumerate(self._thresh):
+                if self._thresh[idx] / self._min_thresh < 1e-2:
+                    LOGGER.info(
+                        "Min threshold is less than 1e-2 times the "
+                        "threshold for column %s; Using mean instead.",
+                        idx,
+                    )
+                    self._thresh[idx] = np.mean(x[:, idx]) + (3 * np.std(x[:, idx]))
+
         self._thresh[self._thresh < self._min_thresh] = self._min_thresh
         self._is_fitted = True
         return self
 
     def predict(self, x: npt.NDArray[float]) -> npt.NDArray[int]:
         if not self._is_fitted:
             raise ModelInitializationError("Model not fitted yet.")
```

### Comparing `numalogic-0.9.1a3/numalogic/models/threshold/_static.py` & `numalogic-0.9.1a4/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/threshold/_std.py` & `numalogic-0.9.1a4/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/vae/base.py` & `numalogic-0.9.1a4/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/vae/layer.py` & `numalogic-0.9.1a4/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1a4/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/monitoring/__init__.py` & `numalogic-0.9.1a4/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/monitoring/metrics.py` & `numalogic-0.9.1a4/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/__init__.py` & `numalogic-0.9.1a4/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/_serialize.py` & `numalogic-0.9.1a4/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/artifact.py` & `numalogic-0.9.1a4/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1a4/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/localcache.py` & `numalogic-0.9.1a4/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1a4/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/registry/redis_registry.py` & `numalogic-0.9.1a4/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/synthetic/__init__.py` & `numalogic-0.9.1a4/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1a4/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1a4/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1a4/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/aggregators.py` & `numalogic-0.9.1a4/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/callbacks.py` & `numalogic-0.9.1a4/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/data.py` & `numalogic-0.9.1a4/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/exceptions.py` & `numalogic-0.9.1a4/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/trainer.py` & `numalogic-0.9.1a4/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/tools/types.py` & `numalogic-0.9.1a4/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/transforms/__init__.py` & `numalogic-0.9.1a4/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/transforms/_movavg.py` & `numalogic-0.9.1a4/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1a4/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/transforms/_scaler.py` & `numalogic-0.9.1a4/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/transforms/_stateless.py` & `numalogic-0.9.1a4/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/README.md` & `numalogic-0.9.1a4/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/__init__.py` & `numalogic-0.9.1a4/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/__main__.py` & `numalogic-0.9.1a4/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/_base.py` & `numalogic-0.9.1a4/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/_config.py` & `numalogic-0.9.1a4/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/_logger.py` & `numalogic-0.9.1a4/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/_metrics.py` & `numalogic-0.9.1a4/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/entities.py` & `numalogic-0.9.1a4/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/factory.py` & `numalogic-0.9.1a4/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/inference.py` & `numalogic-0.9.1a4/numalogic/udfs/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1a4/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/postprocess.py` & `numalogic-0.9.1a4/numalogic/udfs/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/preprocess.py` & `numalogic-0.9.1a4/numalogic/udfs/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1a4/numalogic/udfs/staticthresh.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/tools.py` & `numalogic-0.9.1a4/numalogic/udfs/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1a4/numalogic/udfs/trainer/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1a4/numalogic/udfs/trainer/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1a4/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a3/pyproject.toml` & `numalogic-0.9.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1a3"
+version = "0.9.1a4"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.9.1a3/PKG-INFO` & `numalogic-0.9.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1a3
+Version: 0.9.1a4
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

