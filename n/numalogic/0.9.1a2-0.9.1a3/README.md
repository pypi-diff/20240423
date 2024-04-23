# Comparing `tmp/numalogic-0.9.1a2.tar.gz` & `tmp/numalogic-0.9.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1a2.tar", max compression
+gzip compressed data, was "numalogic-0.9.1a3.tar", max compression
```

## Comparing `numalogic-0.9.1a2.tar` & `numalogic-0.9.1a3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-22 22:41:41.751486 numalogic-0.9.1a2/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-22 22:41:41.751486 numalogic-0.9.1a2/README.md
--rw-r--r--   0        0        0      676 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    15806 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/_config.py
--rw-r--r--   0        0        0     7510 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1709 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-04-22 22:41:41.771486 numalogic-0.9.1a2/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2119 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10245 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/tools/types.py
--rw-r--r--   0        0        0     1417 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     3905 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     2250 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     4737 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7349 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2196 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15595 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9286 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5581 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14920 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13821 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5187 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3816 2024-04-22 22:41:41.775486 numalogic-0.9.1a2/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-04-22 22:41:41.779486 numalogic-0.9.1a2/pyproject.toml
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-22 23:47:49.739781 numalogic-0.9.1a3/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-22 23:47:49.739781 numalogic-0.9.1a3/README.md
+-rw-r--r--   0        0        0      676 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15806 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7543 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-22 23:47:49.763781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2119 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1418 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     2252 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     4772 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7349 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15595 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9286 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13821 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5187 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-04-22 23:47:49.767781 numalogic-0.9.1a3/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-04-22 23:47:49.771782 numalogic-0.9.1a3/pyproject.toml
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a3/PKG-INFO
```

### Comparing `numalogic-0.9.1a2/LICENSE` & `numalogic-0.9.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/README.md` & `numalogic-0.9.1a3/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/__init__.py` & `numalogic-0.9.1a3/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/_constants.py` & `numalogic-0.9.1a3/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/backtest/_prom.py` & `numalogic-0.9.1a3/numalogic/backtest/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/base.py` & `numalogic-0.9.1a3/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/blocks/__init__.py` & `numalogic-0.9.1a3/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/blocks/_base.py` & `numalogic-0.9.1a3/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/blocks/_nn.py` & `numalogic-0.9.1a3/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/blocks/_transform.py` & `numalogic-0.9.1a3/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/blocks/pipeline.py` & `numalogic-0.9.1a3/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/config/__init__.py` & `numalogic-0.9.1a3/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/config/_config.py` & `numalogic-0.9.1a3/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/config/factory.py` & `numalogic-0.9.1a3/numalogic/config/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         StaticPowerTransformer,
         TanhScaler,
         DataClipper,
         GaussianNoiseAdder,
         DifferenceTransform,
         FlattenVector,
         PercentileScaler,
-        ExpMovingAverage
+        ExpMovingAverage,
     )
 
     _CLS_MAP: ClassVar[dict] = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
         "RobustScaler": RobustScaler,
@@ -64,15 +64,15 @@
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
         "DataClipper": DataClipper,
         "GaussianNoiseAdder": GaussianNoiseAdder,
         "DifferenceTransform": DifferenceTransform,
         "FlattenVector": FlattenVector,
         "PercentileScaler": PercentileScaler,
-        "ExpMovingAverage": ExpMovingAverage
+        "ExpMovingAverage": ExpMovingAverage,
     }
 
     def get_pipeline_instance(self, objs_info: list[ModelInfo]):
         preproc_clfs = []
         for obj_info in objs_info:
             _clf = self.get_instance(obj_info)
             preproc_clfs.append(_clf)
@@ -84,15 +84,19 @@
 
 
 class PostprocessFactory(_ObjectFactory):
     """Factory class to create postprocess instances."""
 
     from numalogic.transforms import TanhNorm, ExpMovingAverage, SigmoidNorm
 
-    _CLS_MAP: ClassVar[dict] = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage, "SigmoidNorm": SigmoidNorm}
+    _CLS_MAP: ClassVar[dict] = {
+        "TanhNorm": TanhNorm,
+        "ExpMovingAverage": ExpMovingAverage,
+        "SigmoidNorm": SigmoidNorm,
+    }
 
 
 class ThresholdFactory(_ObjectFactory):
     """Factory class to create threshold instances."""
 
     from numalogic.models.threshold import (
         StdDevThreshold,
```

### Comparing `numalogic-0.9.1a2/numalogic/connectors/__init__.py` & `numalogic-0.9.1a3/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/_base.py` & `numalogic-0.9.1a3/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/_config.py` & `numalogic-0.9.1a3/numalogic/connectors/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1a3/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1a3/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1a3/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/prometheus.py` & `numalogic-0.9.1a3/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/rds/_base.py` & `numalogic-0.9.1a3/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.1a3/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.1a3/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.1a3/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/redis.py` & `numalogic-0.9.1a3/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/connectors/utils/enum.py` & `numalogic-0.9.1a3/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1a3/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1a3/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1a3/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/threshold/_median.py` & `numalogic-0.9.1a3/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/threshold/_static.py` & `numalogic-0.9.1a3/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/threshold/_std.py` & `numalogic-0.9.1a3/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/vae/base.py` & `numalogic-0.9.1a3/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/vae/layer.py` & `numalogic-0.9.1a3/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1a3/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/monitoring/__init__.py` & `numalogic-0.9.1a3/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/monitoring/metrics.py` & `numalogic-0.9.1a3/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/__init__.py` & `numalogic-0.9.1a3/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/_serialize.py` & `numalogic-0.9.1a3/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/artifact.py` & `numalogic-0.9.1a3/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1a3/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/localcache.py` & `numalogic-0.9.1a3/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1a3/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/registry/redis_registry.py` & `numalogic-0.9.1a3/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/synthetic/__init__.py` & `numalogic-0.9.1a3/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1a3/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1a3/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1a3/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/aggregators.py` & `numalogic-0.9.1a3/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/callbacks.py` & `numalogic-0.9.1a3/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/data.py` & `numalogic-0.9.1a3/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/exceptions.py` & `numalogic-0.9.1a3/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/trainer.py` & `numalogic-0.9.1a3/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/tools/types.py` & `numalogic-0.9.1a3/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/transforms/__init__.py` & `numalogic-0.9.1a3/numalogic/transforms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     "expmov_avg_aggregator",
     "TanhNorm",
     "tanh_norm",
     "GaussianNoiseAdder",
     "DifferenceTransform",
     "FlattenVector",
     "PercentileScaler",
-    "SigmoidNorm"
+    "SigmoidNorm",
 ]
```

### Comparing `numalogic-0.9.1a2/numalogic/transforms/_movavg.py` & `numalogic-0.9.1a3/numalogic/transforms/_movavg.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,9 +107,10 @@
         ----
             input_: input column vector
 
         Raises
         ------
             InvalidDataShapeError: if input array is not single featured
         """
-        x_df = pd.DataFrame(input_)
-        return x_df.ewm(alpha=self.alpha).mean().to_numpy(dtype=np.float32)
+        x_df = pd.DataFrame(input_, dtype=np.float32, copy=True)
+        x_smoothed = x_df.ewm(alpha=self.alpha).mean().to_numpy(dtype=np.float32)
+        return np.ascontiguousarray(x_smoothed, dtype=np.float32)
```

### Comparing `numalogic-0.9.1a2/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1a3/numalogic/transforms/_postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,14 @@
         self.smooth_factor = smooth_factor
 
     def transform(self, input_: npt.NDArray[float], **__) -> npt.NDArray[float]:
         return tanh_norm(input_, scale_factor=self.scale_factor, smooth_factor=self.smooth_factor)
 
 
 class SigmoidNorm(StatelessTransformer):
-    def __init__(self, scale_factor: float = 10., smooth_factor: float = 0.5):
+    def __init__(self, scale_factor: float = 10.0, smooth_factor: float = 0.5):
         super().__init__()
         self.scale_factor = scale_factor
         self.smooth_factor = smooth_factor
 
     def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
-        return self.scale_factor / (1.0 + np.exp(5 - (self.smooth_factor * x)))
+        return self.scale_factor / (1.0 + np.exp(5 - (self.smooth_factor * x)))
```

### Comparing `numalogic-0.9.1a2/numalogic/transforms/_scaler.py` & `numalogic-0.9.1a3/numalogic/transforms/_scaler.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,17 @@
             Default is 99.
         min_percentile: float, optional
             The lower percentile to clip the data.
             If None, minimum value of the data is used.
             Default is None.
     """
 
-    def __init__(self, max_percentile: float = 99, min_percentile: Optional[float] = None, eps: float = 1e-2):
+    def __init__(
+        self, max_percentile: float = 99, min_percentile: Optional[float] = None, eps: float = 1e-2
+    ):
         self._max_px = max_percentile
         self._min_px = min_percentile
         self.tx = MinMaxScaler()
 
         self._data_pth_max = None
         self._data_pth_min = None
         self._eps = eps
@@ -116,16 +118,17 @@
             data_min_px = np.percentile(x, self._min_px, axis=0)
 
         p_ranges = data_max_px - data_min_px
 
         for idx, _range in enumerate(p_ranges):
             if _range <= self._eps:
                 LOGGER.warning(
-                    "Max and Min percentile difference is less than "
-                    "epsilon: %s for column %s", self._eps, idx
+                    "Max and Min percentile difference is less than " "epsilon: %s for column %s",
+                    self._eps,
+                    idx,
                 )
                 data_max_px[idx] = data_max[idx]
 
         self._data_pth_max = data_max_px
         self._data_pth_min = data_min_px
 
         x_clipped = DataClipper(lower=data_min_px, upper=data_max_px).transform(x)
```

### Comparing `numalogic-0.9.1a2/numalogic/transforms/_stateless.py` & `numalogic-0.9.1a3/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/README.md` & `numalogic-0.9.1a3/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/__init__.py` & `numalogic-0.9.1a3/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/__main__.py` & `numalogic-0.9.1a3/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/_base.py` & `numalogic-0.9.1a3/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/_config.py` & `numalogic-0.9.1a3/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/_logger.py` & `numalogic-0.9.1a3/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/_metrics.py` & `numalogic-0.9.1a3/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/entities.py` & `numalogic-0.9.1a3/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/factory.py` & `numalogic-0.9.1a3/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/inference.py` & `numalogic-0.9.1a3/numalogic/udfs/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1a3/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/postprocess.py` & `numalogic-0.9.1a3/numalogic/udfs/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/preprocess.py` & `numalogic-0.9.1a3/numalogic/udfs/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1a3/numalogic/udfs/staticthresh.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/tools.py` & `numalogic-0.9.1a3/numalogic/udfs/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1a3/numalogic/udfs/trainer/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1a3/numalogic/udfs/trainer/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1a3/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a2/pyproject.toml` & `numalogic-0.9.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1a2"
+version = "0.9.1a3"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.9.1a2/PKG-INFO` & `numalogic-0.9.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1a2
+Version: 0.9.1a3
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

