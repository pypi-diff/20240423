# Comparing `tmp/redis-5.1.0b3.tar.gz` & `tmp/redis-5.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.1.0b3.tar", last modified: Mon Jan 15 15:54:29 2024, max compression
+gzip compressed data, was "redis-5.1.0b4.tar", last modified: Thu Feb 29 12:39:46 2024, max compression
```

## Comparing `redis-5.1.0b3.tar` & `redis-5.1.0b4.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.842056 redis-5.1.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-15 15:54:18.000000 redis-5.1.0b3/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-15 15:54:18.000000 redis-5.1.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-15 15:54:18.000000 redis-5.1.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-01-15 15:54:29.842056 redis-5.1.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-01-15 15:54:18.000000 redis-5.1.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.814056 redis-5.1.0b3/redis/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.818056 redis-5.1.0b3/redis/_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    27958 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/_parsers/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.818056 redis-5.1.0b3/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61024 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64393 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    49514 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59629 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    93497 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.822056 redis-5.1.0b3/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.822056 redis-5.1.0b3/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    31542 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)   224568 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.822056 redis-5.1.0b3/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.822056 redis-5.1.0b3/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.822056 redis-5.1.0b3/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36751 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.826056 redis-5.1.0b3/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34191 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55655 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/ocsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-01-15 15:54:18.000000 redis-5.1.0b3/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.818056 redis-5.1.0b3/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-01-15 15:54:29.000000 redis-5.1.0b3/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-15 15:54:29.000000 redis-5.1.0b3/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 15:54:29.000000 redis-5.1.0b3/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-15 15:54:29.000000 redis-5.1.0b3/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-15 15:54:29.000000 redis-5.1.0b3/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 15:54:29.842056 redis-5.1.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-01-15 15:54:18.000000 redis-5.1.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.830056 redis-5.1.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/ssl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.834056 redis-5.1.0b3/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19099 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)   119850 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)   128154 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_cwe_404.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15843 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    36704 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    39645 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (127)    56983 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    27355 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.834056 redis-5.1.0b3/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    98632 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)  2069623 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)   128208 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)   184496 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31827 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.838056 redis-5.1.0b3/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    47601 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    43247 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (127)    81082 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    32821 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:54:29.838056 redis-5.1.0b3/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    98632 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)  2069623 2024-01-15 15:54:18.000000 redis-5.1.0b3/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.202771 redis-5.1.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-29 12:39:33.000000 redis-5.1.0b4/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-29 12:39:33.000000 redis-5.1.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-29 12:39:33.000000 redis-5.1.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-02-29 12:39:46.202771 redis-5.1.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-02-29 12:39:33.000000 redis-5.1.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.174771 redis-5.1.0b4/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.178771 redis-5.1.0b4/redis/_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27958 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/_parsers/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.178771 redis-5.1.0b4/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64518 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50189 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60002 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93614 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.182771 redis-5.1.0b4/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.182771 redis-5.1.0b4/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)   224568 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.182771 redis-5.1.0b4/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.182771 redis-5.1.0b4/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.186771 redis-5.1.0b4/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36751 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.186771 redis-5.1.0b4/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34191 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56066 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-29 12:39:33.000000 redis-5.1.0b4/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.178771 redis-5.1.0b4/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-02-29 12:39:46.000000 redis-5.1.0b4/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-02-29 12:39:46.000000 redis-5.1.0b4/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 12:39:46.000000 redis-5.1.0b4/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-29 12:39:46.000000 redis-5.1.0b4/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 12:39:46.000000 redis-5.1.0b4/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 12:39:46.202771 redis-5.1.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-29 12:39:33.000000 redis-5.1.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.190771 redis-5.1.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/ssl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.194771 redis-5.1.0b4/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119850 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128154 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_cwe_404.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15403 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39645 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56983 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26849 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.194771 redis-5.1.0b4/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98632 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2069623 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129318 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184496 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31827 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.198771 redis-5.1.0b4/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47601 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43247 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81082 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32821 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 12:39:46.198771 redis-5.1.0b4/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98632 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2069623 2024-02-29 12:39:33.000000 redis-5.1.0b4/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.1.0b3/LICENSE` & `redis-5.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/PKG-INFO` & `redis-5.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.1.0b3
+Version: 5.1.0b4
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.1.0b3/README.md` & `redis-5.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/__init__.py` & `redis-5.1.0b4/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_cache.py` & `redis-5.1.0b4/redis/_cache.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/__init__.py` & `redis-5.1.0b4/redis/_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/base.py` & `redis-5.1.0b4/redis/_parsers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     async def can_read_destructive(self) -> bool:
         if not self._connected:
             raise RedisError("Buffer is closed.")
         if self._buffer:
             return True
         try:
             async with async_timeout(0):
-                return await self._stream.read(1)
+                return self._stream.at_eof()
         except TimeoutError:
             return False
 
     async def _read(self, length: int) -> bytes:
         """
         Read `length` bytes of data.  These are assumed to be followed
         by a '\r\n' terminator which is subsequently discarded.
```

### Comparing `redis-5.1.0b3/redis/_parsers/commands.py` & `redis-5.1.0b4/redis/_parsers/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/encoders.py` & `redis-5.1.0b4/redis/_parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/helpers.py` & `redis-5.1.0b4/redis/_parsers/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/hiredis.py` & `redis-5.1.0b4/redis/_parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/resp2.py` & `redis-5.1.0b4/redis/_parsers/resp2.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/_parsers/resp3.py` & `redis-5.1.0b4/redis/_parsers/resp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,17 @@
         elif byte == b">":
             response = [
                 self._read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
                 for _ in range(int(response))
             ]
-            self.handle_push_response(response, disable_decoding, push_request)
+            response = self.handle_push_response(
+                response, disable_decoding, push_request
+            )
         else:
             raise InvalidResponse(f"Protocol Error: {raw!r}")
 
         if isinstance(response, bytes) and disable_decoding is False:
             response = self.encoder.decode(response)
         return response
 
@@ -255,15 +257,17 @@
                 (
                     await self._read_response(
                         disable_decoding=disable_decoding, push_request=push_request
                     )
                 )
                 for _ in range(int(response))
             ]
-            await self.handle_push_response(response, disable_decoding, push_request)
+            response = await self.handle_push_response(
+                response, disable_decoding, push_request
+            )
         else:
             raise InvalidResponse(f"Protocol Error: {raw!r}")
 
         if isinstance(response, bytes) and disable_decoding is False:
             response = self.encoder.decode(response)
         return response
```

### Comparing `redis-5.1.0b3/redis/_parsers/socket.py` & `redis-5.1.0b4/redis/_parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/asyncio/__init__.py` & `redis-5.1.0b4/redis/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/asyncio/client.py` & `redis-5.1.0b4/redis/asyncio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import copy
 import inspect
 import re
+import ssl
 import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
@@ -222,14 +223,15 @@
         ssl: bool = False,
         ssl_keyfile: Optional[str] = None,
         ssl_certfile: Optional[str] = None,
         ssl_cert_reqs: str = "required",
         ssl_ca_certs: Optional[str] = None,
         ssl_ca_data: Optional[str] = None,
         ssl_check_hostname: bool = False,
+        ssl_min_version: Optional[ssl.TLSVersion] = None,
         max_connections: Optional[int] = None,
         single_connection_client: bool = False,
         health_check_interval: int = 0,
         client_name: Optional[str] = None,
         lib_name: Optional[str] = "redis-py",
         lib_version: Optional[str] = get_lib_version(),
         username: Optional[str] = None,
@@ -328,14 +330,15 @@
                             "connection_class": SSLConnection,
                             "ssl_keyfile": ssl_keyfile,
                             "ssl_certfile": ssl_certfile,
                             "ssl_cert_reqs": ssl_cert_reqs,
                             "ssl_ca_certs": ssl_ca_certs,
                             "ssl_ca_data": ssl_ca_data,
                             "ssl_check_hostname": ssl_check_hostname,
+                            "ssl_min_version": ssl_min_version,
                         }
                     )
             # This arg only used if no pool is passed in
             self.auto_close_connection_pool = auto_close_connection_pool
             connection_pool = ConnectionPool(**kwargs)
         else:
             # If a pool is passed in, do not close it
@@ -622,33 +625,35 @@
         """Execute a command and return a parsed response"""
         await self.initialize()
         command_name = args[0]
         keys = options.pop("keys", None)  # keys are used only for client side caching
         pool = self.connection_pool
         conn = self.connection or await pool.get_connection(command_name, **options)
         response_from_cache = await conn._get_from_local_cache(args)
-        if response_from_cache is not None:
-            return response_from_cache
-        else:
-            if self.single_connection_client:
-                await self._single_conn_lock.acquire()
-            try:
-                response = await conn.retry.call_with_retry(
-                    lambda: self._send_command_parse_response(
-                        conn, command_name, *args, **options
-                    ),
-                    lambda error: self._disconnect_raise(conn, error),
-                )
-                conn._add_to_local_cache(args, response, keys)
-                return response
-            finally:
-                if self.single_connection_client:
-                    self._single_conn_lock.release()
-                if not self.connection:
-                    await pool.release(conn)
+        try:
+            if response_from_cache is not None:
+                return response_from_cache
+            else:
+                try:
+                    if self.single_connection_client:
+                        await self._single_conn_lock.acquire()
+                    response = await conn.retry.call_with_retry(
+                        lambda: self._send_command_parse_response(
+                            conn, command_name, *args, **options
+                        ),
+                        lambda error: self._disconnect_raise(conn, error),
+                    )
+                    conn._add_to_local_cache(args, response, keys)
+                    return response
+                finally:
+                    if self.single_connection_client:
+                        self._single_conn_lock.release()
+        finally:
+            if not self.connection:
+                await pool.release(conn)
 
     async def parse_response(
         self, connection: Connection, command_name: Union[str, bytes], **options
     ):
         """Parses a response from the Redis server"""
         try:
             if NEVER_DECODE in options:
@@ -920,19 +925,23 @@
             await self.connection.connect()
         if self.push_handler_func is not None and not HIREDIS_AVAILABLE:
             self.connection._parser.set_pubsub_push_handler(self.push_handler_func)
 
     async def _disconnect_raise_connect(self, conn, error):
         """
         Close the connection and raise an exception
-        if retry_on_timeout is not set or the error
-        is not a TimeoutError. Otherwise, try to reconnect
+        if retry_on_error is not set or the error is not one
+        of the specified error types. Otherwise, try to
+        reconnect
         """
         await conn.disconnect()
-        if not (conn.retry_on_timeout and isinstance(error, TimeoutError)):
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
+        ):
             raise error
         await conn.connect()
 
     async def _execute(self, conn, command, *args, **kwargs):
         """
         Connect manually upon disconnection. If the Redis server is down,
         this will fail and raise a ConnectionError as desired.
@@ -1337,29 +1346,32 @@
             return self.immediate_execute_command(*args, **kwargs)
         return self.pipeline_execute_command(*args, **kwargs)
 
     async def _disconnect_reset_raise(self, conn, error):
         """
         Close the connection, reset watching state and
         raise an exception if we were watching,
-        retry_on_timeout is not set,
-        or the error is not a TimeoutError
+        if retry_on_error is not set or the error is not one
+        of the specified error types.
         """
         await conn.disconnect()
         # if we were already watching a variable, the watch is no longer
         # valid since this connection has died. raise a WatchError, which
         # indicates the user should retry this transaction.
         if self.watching:
             await self.aclose()
             raise WatchError(
                 "A ConnectionError occurred on while watching one or more keys"
             )
-        # if retry_on_timeout is not set, or the error is not
-        # a TimeoutError, raise it
-        if not (conn.retry_on_timeout and isinstance(error, TimeoutError)):
+        # if retry_on_error is not set or the error is not one
+        # of the specified error types, raise it
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
+        ):
             await self.aclose()
             raise
 
     async def immediate_execute_command(self, *args, **options):
         """
         Execute a command immediately, but don't auto-retry on a
         ConnectionError if we're already WATCHing a variable. Used when
@@ -1526,28 +1538,31 @@
             for s, exist in zip(scripts, exists):
                 if not exist:
                     s.sha = await immediate("SCRIPT LOAD", s.script)
 
     async def _disconnect_raise_reset(self, conn: Connection, error: Exception):
         """
         Close the connection, raise an exception if we were watching,
-        and raise an exception if retry_on_timeout is not set,
-        or the error is not a TimeoutError
+        and raise an exception if retry_on_error is not set or the
+        error is not one of the specified error types.
         """
         await conn.disconnect()
         # if we were watching a variable, the watch is no longer valid
         # since this connection has died. raise a WatchError, which
         # indicates the user should retry this transaction.
         if self.watching:
             raise WatchError(
                 "A ConnectionError occurred on while watching one or more keys"
             )
-        # if retry_on_timeout is not set, or the error is not
-        # a TimeoutError, raise it
-        if not (conn.retry_on_timeout and isinstance(error, TimeoutError)):
+        # if retry_on_error is not set or the error is not one
+        # of the specified error types, raise it
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
+        ):
             await self.reset()
             raise
 
     async def execute(self, raise_on_error: bool = True):
         """Execute all the commands in the current pipeline"""
         stack = self.command_stack
         if not stack and not self.watching:
```

### Comparing `redis-5.1.0b3/redis/asyncio/cluster.py` & `redis-5.1.0b4/redis/asyncio/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import collections
 import random
 import socket
+import ssl
 import warnings
 from typing import (
     Any,
     Callable,
     Deque,
     Dict,
     Generator,
@@ -267,14 +268,15 @@
         ssl: bool = False,
         ssl_ca_certs: Optional[str] = None,
         ssl_ca_data: Optional[str] = None,
         ssl_cert_reqs: str = "required",
         ssl_certfile: Optional[str] = None,
         ssl_check_hostname: bool = False,
         ssl_keyfile: Optional[str] = None,
+        ssl_min_version: Optional[ssl.TLSVersion] = None,
         protocol: Optional[int] = 2,
         address_remap: Optional[Callable[[str, int], Tuple[str, int]]] = None,
         cache_enabled: bool = False,
         client_cache: Optional[AbstractCache] = None,
         cache_max_size: int = 100,
         cache_ttl: int = 0,
         cache_policy: str = DEFAULT_EVICTION_POLICY,
@@ -340,14 +342,15 @@
                     "connection_class": SSLConnection,
                     "ssl_ca_certs": ssl_ca_certs,
                     "ssl_ca_data": ssl_ca_data,
                     "ssl_cert_reqs": ssl_cert_reqs,
                     "ssl_certfile": ssl_certfile,
                     "ssl_check_hostname": ssl_check_hostname,
                     "ssl_keyfile": ssl_keyfile,
+                    "ssl_min_version": ssl_min_version,
                 }
             )
 
         if read_from_replicas:
             # Call our on_connect function to configure READONLY mode
             kwargs["redis_connect_func"] = self.on_connect
```

### Comparing `redis-5.1.0b3/redis/asyncio/connection.py` & `redis-5.1.0b4/redis/asyncio/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,15 +681,15 @@
 
         if pieces:
             output.append(SYM_EMPTY.join(pieces))
         return output
 
     def _socket_is_empty(self):
         """Check if the socket is empty"""
-        return not self._reader.at_eof()
+        return len(self._reader._buffer) == 0
 
     def _cache_invalidation_process(
         self, data: List[Union[str, Optional[List[str]]]]
     ) -> None:
         """
         Invalidate (delete) all redis commands associated with a specific key.
         `data` is a list of strings, where the first string is the invalidation message
@@ -819,23 +819,25 @@
         self,
         ssl_keyfile: Optional[str] = None,
         ssl_certfile: Optional[str] = None,
         ssl_cert_reqs: str = "required",
         ssl_ca_certs: Optional[str] = None,
         ssl_ca_data: Optional[str] = None,
         ssl_check_hostname: bool = False,
+        ssl_min_version: Optional[ssl.TLSVersion] = None,
         **kwargs,
     ):
         self.ssl_context: RedisSSLContext = RedisSSLContext(
             keyfile=ssl_keyfile,
             certfile=ssl_certfile,
             cert_reqs=ssl_cert_reqs,
             ca_certs=ssl_ca_certs,
             ca_data=ssl_ca_data,
             check_hostname=ssl_check_hostname,
+            min_version=ssl_min_version,
         )
         super().__init__(**kwargs)
 
     def _connection_arguments(self) -> Mapping:
         kwargs = super()._connection_arguments()
         kwargs["ssl"] = self.ssl_context.get()
         return kwargs
@@ -860,34 +862,40 @@
     def ca_data(self):
         return self.ssl_context.ca_data
 
     @property
     def check_hostname(self):
         return self.ssl_context.check_hostname
 
+    @property
+    def min_version(self):
+        return self.ssl_context.min_version
+
 
 class RedisSSLContext:
     __slots__ = (
         "keyfile",
         "certfile",
         "cert_reqs",
         "ca_certs",
         "ca_data",
         "context",
         "check_hostname",
+        "min_version",
     )
 
     def __init__(
         self,
         keyfile: Optional[str] = None,
         certfile: Optional[str] = None,
         cert_reqs: Optional[str] = None,
         ca_certs: Optional[str] = None,
         ca_data: Optional[str] = None,
         check_hostname: bool = False,
+        min_version: Optional[ssl.TLSVersion] = None,
     ):
         self.keyfile = keyfile
         self.certfile = certfile
         if cert_reqs is None:
             self.cert_reqs = ssl.CERT_NONE
         elif isinstance(cert_reqs, str):
             CERT_REQS = {
@@ -899,25 +907,28 @@
                 raise RedisError(
                     f"Invalid SSL Certificate Requirements Flag: {cert_reqs}"
                 )
             self.cert_reqs = CERT_REQS[cert_reqs]
         self.ca_certs = ca_certs
         self.ca_data = ca_data
         self.check_hostname = check_hostname
+        self.min_version = min_version
         self.context: Optional[ssl.SSLContext] = None
 
     def get(self) -> ssl.SSLContext:
         if not self.context:
             context = ssl.create_default_context()
             context.check_hostname = self.check_hostname
             context.verify_mode = self.cert_reqs
             if self.certfile and self.keyfile:
                 context.load_cert_chain(certfile=self.certfile, keyfile=self.keyfile)
             if self.ca_certs or self.ca_data:
                 context.load_verify_locations(cafile=self.ca_certs, cadata=self.ca_data)
+            if self.min_version is not None:
+                context.minimum_version = self.min_version
             self.context = context
         return self.context
 
 
 class UnixDomainSocketConnection(AbstractConnection):
     "Manages UDS communication to and from a Redis server"
 
@@ -1177,20 +1188,26 @@
     def make_connection(self):
         """Create a new connection.  Can be overridden by child classes."""
         return self.connection_class(**self.connection_kwargs)
 
     async def ensure_connection(self, connection: AbstractConnection):
         """Ensure that the connection object is connected and valid"""
         await connection.connect()
-        # connections that the pool provides should be ready to send
-        # a command. if not, the connection was either returned to the
+        # if client caching is not enabled connections that the pool
+        # provides should be ready to send a command.
+        # if not, the connection was either returned to the
         # pool before all data has been read or the socket has been
         # closed. either way, reconnect and verify everything is good.
+        # (if caching enabled the connection will not always be ready
+        # to send a command because it may contain invalidation messages)
         try:
-            if await connection.can_read_destructive():
+            if (
+                await connection.can_read_destructive()
+                and connection.client_cache is None
+            ):
                 raise ConnectionError("Connection has data") from None
         except (ConnectionError, OSError):
             await connection.disconnect()
             await connection.connect()
             if await connection.can_read_destructive():
                 raise ConnectionError("Connection not ready") from None
 
@@ -1276,15 +1293,15 @@
     it maintains a pool of reusable connections that can be shared by
     multiple async redis clients.
 
     The difference is that, in the event that a client tries to get a
     connection from the pool when all of connections are in use, rather than
     raising a :py:class:`~redis.ConnectionError` (as the default
     :py:class:`~redis.asyncio.ConnectionPool` implementation does), it
-    makes blocks the current `Task` for a specified number of seconds until
+    blocks the current `Task` for a specified number of seconds until
     a connection becomes available.
 
     Use ``max_connections`` to increase / decrease the pool size::
 
         >>> pool = BlockingConnectionPool(max_connections=10)
 
     Use ``timeout`` to tell it either how many seconds to wait for a connection
```

### Comparing `redis-5.1.0b3/redis/asyncio/lock.py` & `redis-5.1.0b4/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/asyncio/retry.py` & `redis-5.1.0b4/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/asyncio/sentinel.py` & `redis-5.1.0b4/redis/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/asyncio/utils.py` & `redis-5.1.0b4/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/backoff.py` & `redis-5.1.0b4/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/client.py` & `redis-5.1.0b4/redis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 )
 from redis.commands import (
     CoreCommands,
     RedisModuleCommands,
     SentinelCommands,
     list_or_args,
 )
-from redis.connection import ConnectionPool, SSLConnection, UnixDomainSocketConnection
+from redis.connection import (
+    AbstractConnection,
+    ConnectionPool,
+    SSLConnection,
+    UnixDomainSocketConnection,
+)
 from redis.credentials import CredentialProvider
 from redis.exceptions import (
     ConnectionError,
     ExecAbortError,
     PubSubError,
     RedisError,
     ResponseError,
@@ -194,14 +199,15 @@
         ssl_ca_data=None,
         ssl_check_hostname=False,
         ssl_password=None,
         ssl_validate_ocsp=False,
         ssl_validate_ocsp_stapled=False,
         ssl_ocsp_context=None,
         ssl_ocsp_expected_cert=None,
+        ssl_min_version=None,
         max_connections=None,
         single_connection_client=False,
         health_check_interval=0,
         client_name=None,
         lib_name="redis-py",
         lib_version=get_lib_version(),
         username=None,
@@ -307,14 +313,15 @@
                             "ssl_check_hostname": ssl_check_hostname,
                             "ssl_password": ssl_password,
                             "ssl_ca_path": ssl_ca_path,
                             "ssl_validate_ocsp_stapled": ssl_validate_ocsp_stapled,
                             "ssl_validate_ocsp": ssl_validate_ocsp,
                             "ssl_ocsp_context": ssl_ocsp_context,
                             "ssl_ocsp_expected_cert": ssl_ocsp_expected_cert,
+                            "ssl_min_version": ssl_min_version,
                         }
                     )
             connection_pool = ConnectionPool(**kwargs)
             self.auto_close_connection_pool = True
         else:
             self.auto_close_connection_pool = False
 
@@ -552,29 +559,29 @@
     def execute_command(self, *args, **options):
         """Execute a command and return a parsed response"""
         command_name = args[0]
         keys = options.pop("keys", None)
         pool = self.connection_pool
         conn = self.connection or pool.get_connection(command_name, **options)
         response_from_cache = conn._get_from_local_cache(args)
-        if response_from_cache is not None:
-            return response_from_cache
-        else:
-            try:
+        try:
+            if response_from_cache is not None:
+                return response_from_cache
+            else:
                 response = conn.retry.call_with_retry(
                     lambda: self._send_command_parse_response(
                         conn, command_name, *args, **options
                     ),
                     lambda error: self._disconnect_raise(conn, error),
                 )
                 conn._add_to_local_cache(args, response, keys)
                 return response
-            finally:
-                if not self.connection:
-                    pool.release(conn)
+        finally:
+            if not self.connection:
+                pool.release(conn)
 
     def parse_response(self, connection, command_name, **options):
         """Parses a response from the Redis server"""
         try:
             if NEVER_DECODE in options:
                 response = connection.read_response(disable_decoding=True)
                 options.pop(NEVER_DECODE)
@@ -833,19 +840,23 @@
                         "execute_command: {0}".format(response)
                     )
             ttl -= 1
 
     def _disconnect_raise_connect(self, conn, error) -> None:
         """
         Close the connection and raise an exception
-        if retry_on_timeout is not set or the error
-        is not a TimeoutError. Otherwise, try to reconnect
+        if retry_on_error is not set or the error is not one
+        of the specified error types. Otherwise, try to
+        reconnect
         """
         conn.disconnect()
-        if not (conn.retry_on_timeout and isinstance(error, TimeoutError)):
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
+        ):
             raise error
         conn.connect()
 
     def _execute(self, conn, command, *args, **kwargs):
         """
         Connect manually upon disconnection. If the Redis server is down,
         this will fail and raise a ConnectionError as desired.
@@ -1314,29 +1325,32 @@
             return self.immediate_execute_command(*args, **kwargs)
         return self.pipeline_execute_command(*args, **kwargs)
 
     def _disconnect_reset_raise(self, conn, error) -> None:
         """
         Close the connection, reset watching state and
         raise an exception if we were watching,
-        retry_on_timeout is not set,
-        or the error is not a TimeoutError
+        if retry_on_error is not set or the error is not one
+        of the specified error types.
         """
         conn.disconnect()
         # if we were already watching a variable, the watch is no longer
         # valid since this connection has died. raise a WatchError, which
         # indicates the user should retry this transaction.
         if self.watching:
             self.reset()
             raise WatchError(
                 "A ConnectionError occurred on while watching one or more keys"
             )
-        # if retry_on_timeout is not set, or the error is not
-        # a TimeoutError, raise it
-        if not (conn.retry_on_timeout and isinstance(error, TimeoutError)):
+        # if retry_on_error is not set or the error is not one
+        # of the specified error types, raise it
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
+        ):
             self.reset()
             raise
 
     def immediate_execute_command(self, *args, **options):
         """
         Execute a command immediately, but don't auto-retry on a
         ConnectionError if we're already WATCHing a variable. Used when
@@ -1486,33 +1500,39 @@
         # get buffered in the pipeline.
         exists = immediate("SCRIPT EXISTS", *shas)
         if not all(exists):
             for s, exist in zip(scripts, exists):
                 if not exist:
                     s.sha = immediate("SCRIPT LOAD", s.script)
 
-    def _disconnect_raise_reset(self, conn: Redis, error: Exception) -> None:
+    def _disconnect_raise_reset(
+        self,
+        conn: AbstractConnection,
+        error: Exception,
+    ) -> None:
         """
         Close the connection, raise an exception if we were watching,
-        and raise an exception if TimeoutError is not part of retry_on_error,
-        or the error is not a TimeoutError
+        and raise an exception if retry_on_error is not set or the
+        error is not one of the specified error types.
         """
         conn.disconnect()
         # if we were watching a variable, the watch is no longer valid
         # since this connection has died. raise a WatchError, which
         # indicates the user should retry this transaction.
         if self.watching:
             raise WatchError(
                 "A ConnectionError occurred on while watching one or more keys"
             )
-        # if TimeoutError is not part of retry_on_error, or the error
-        # is not a TimeoutError, raise it
-        if not (
-            TimeoutError in conn.retry_on_error and isinstance(error, TimeoutError)
+        # if retry_on_error is not set or the error is not one
+        # of the specified error types, raise it
+        if (
+            conn.retry_on_error is None
+            or isinstance(error, tuple(conn.retry_on_error)) is False
         ):
+
             self.reset()
             raise error
 
     def execute(self, raise_on_error=True):
         """Execute all the commands in the current pipeline"""
         stack = self.command_stack
         if not stack and not self.watching:
```

### Comparing `redis-5.1.0b3/redis/cluster.py` & `redis-5.1.0b4/redis/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -2139,14 +2139,16 @@
                 # we can build a list of commands for each node.
                 node_name = node.name
                 if node_name not in nodes:
                     redis_node = self.get_redis_connection(node)
                     try:
                         connection = get_connection(redis_node, c.args)
                     except ConnectionError:
+                        for n in nodes.values():
+                            n.connection_pool.release(n.connection)
                         # Connection retries are being handled in the node's
                         # Retry object. Reinitialize the node -> slot table.
                         self.nodes_manager.initialize()
                         if is_default_node:
                             self.replace_default_node()
                         raise
                     nodes[node_name] = NodeCommands(
```

### Comparing `redis-5.1.0b3/redis/commands/__init__.py` & `redis-5.1.0b4/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/bf/__init__.py` & `redis-5.1.0b4/redis/commands/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/bf/commands.py` & `redis-5.1.0b4/redis/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/bf/info.py` & `redis-5.1.0b4/redis/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/cluster.py` & `redis-5.1.0b4/redis/commands/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     GearsCommands,
     ManagementCommands,
     ModuleCommands,
     PubSubCommands,
     ScriptCommands,
 )
 from .helpers import list_or_args
-from .redismodules import RedisModuleCommands
+from .redismodules import AsyncRedisModuleCommands, RedisModuleCommands
 
 if TYPE_CHECKING:
     from redis.asyncio.cluster import TargetNodesT
 
 # Not complete, but covers the major ones
 # https://redis.io/commands
 READ_COMMANDS = frozenset(
@@ -903,14 +903,15 @@
     AsyncClusterManagementCommands,
     AsyncACLCommands,
     AsyncClusterDataAccessCommands,
     AsyncScriptCommands,
     AsyncFunctionCommands,
     AsyncGearsCommands,
     AsyncModuleCommands,
+    AsyncRedisModuleCommands,
 ):
     """
     A class for all Redis Cluster commands
 
     For key-based commands, the target node(s) will be internally determined
     by the keys' hash slot.
     Non-key-based commands can be executed with the 'target_nodes' argument to
```

### Comparing `redis-5.1.0b3/redis/commands/core.py` & `redis-5.1.0b4/redis/commands/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2007,15 +2007,15 @@
         """
         from redis.client import EMPTY_RESPONSE
 
         args = list_or_args(keys, args)
         options = {}
         if not args:
             options[EMPTY_RESPONSE] = []
-        options["keys"] = keys
+        options["keys"] = args
         return self.execute_command("MGET", *args, **options)
 
     def mset(self, mapping: Mapping[AnyKeyT, EncodableT]) -> ResponseT:
         """
         Sets key/values based on a mapping. Mapping is a dictionary of
         key/value pairs. Both keys and values should be strings or types that
         can be cast to a string via str().
```

### Comparing `redis-5.1.0b3/redis/commands/graph/__init__.py` & `redis-5.1.0b4/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/commands.py` & `redis-5.1.0b4/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/edge.py` & `redis-5.1.0b4/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/execution_plan.py` & `redis-5.1.0b4/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/node.py` & `redis-5.1.0b4/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/path.py` & `redis-5.1.0b4/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/graph/query_result.py` & `redis-5.1.0b4/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/helpers.py` & `redis-5.1.0b4/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/json/__init__.py` & `redis-5.1.0b4/redis/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/json/commands.py` & `redis-5.1.0b4/redis/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/json/decoders.py` & `redis-5.1.0b4/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/redismodules.py` & `redis-5.1.0b4/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/__init__.py` & `redis-5.1.0b4/redis/commands/search/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/aggregation.py` & `redis-5.1.0b4/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/commands.py` & `redis-5.1.0b4/redis/commands/search/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/field.py` & `redis-5.1.0b4/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/indexDefinition.py` & `redis-5.1.0b4/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/query.py` & `redis-5.1.0b4/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/querystring.py` & `redis-5.1.0b4/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/reducers.py` & `redis-5.1.0b4/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/result.py` & `redis-5.1.0b4/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/search/suggestion.py` & `redis-5.1.0b4/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/sentinel.py` & `redis-5.1.0b4/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/timeseries/__init__.py` & `redis-5.1.0b4/redis/commands/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/timeseries/commands.py` & `redis-5.1.0b4/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/timeseries/info.py` & `redis-5.1.0b4/redis/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/commands/timeseries/utils.py` & `redis-5.1.0b4/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/connection.py` & `redis-5.1.0b4/redis/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import os
-import select
 import socket
 import ssl
 import sys
 import threading
 import weakref
 from abc import abstractmethod
 from itertools import chain
@@ -447,15 +446,15 @@
         self._sock = None
         if conn_sock is None:
             return
 
         if os.getpid() == self.pid:
             try:
                 conn_sock.shutdown(socket.SHUT_RDWR)
-            except OSError:
+            except (OSError, TypeError):
                 pass
 
         try:
             conn_sock.close()
         except OSError:
             pass
 
@@ -605,19 +604,14 @@
                     pieces.append(chunk)
                     buffer_length += chunklen
 
         if pieces:
             output.append(SYM_EMPTY.join(pieces))
         return output
 
-    def _socket_is_empty(self):
-        """Check if the socket is empty"""
-        r, _, _ = select.select([self._sock], [], [], 0)
-        return not bool(r)
-
     def _cache_invalidation_process(
         self, data: List[Union[str, Optional[List[str]]]]
     ) -> None:
         """
         Invalidate (delete) all redis commands associated with a specific key.
         `data` is a list of strings, where the first string is the invalidation message
         and the second string is the list of keys to invalidate.
@@ -635,15 +629,15 @@
         """
         if (
             self.client_cache is None
             or command[0] in self.cache_blacklist
             or command[0] not in self.cache_whitelist
         ):
             return None
-        while not self._socket_is_empty():
+        while self.can_read():
             self.read_response(push_request=True)
         return self.client_cache.get(command)
 
     def _add_to_local_cache(
         self, command: Tuple[str], response: ResponseT, keys: List[KeysT]
     ):
         """
@@ -765,14 +759,15 @@
         ssl_check_hostname=False,
         ssl_ca_path=None,
         ssl_password=None,
         ssl_validate_ocsp=False,
         ssl_validate_ocsp_stapled=False,
         ssl_ocsp_context=None,
         ssl_ocsp_expected_cert=None,
+        ssl_min_version=None,
         **kwargs,
     ):
         """Constructor
 
         Args:
             ssl_keyfile: Path to an ssl private key. Defaults to None.
             ssl_certfile: Path to an ssl certificate. Defaults to None.
@@ -783,14 +778,15 @@
             ssl_ca_path: The path to a directory containing several CA certificates in PEM format. Defaults to None.
             ssl_password: Password for unlocking an encrypted private key. Defaults to None.
 
             ssl_validate_ocsp: If set, perform a full ocsp validation (i.e not a stapled verification)
             ssl_validate_ocsp_stapled: If set, perform a validation on a stapled ocsp response
             ssl_ocsp_context: A fully initialized OpenSSL.SSL.Context object to be used in verifying the ssl_ocsp_expected_cert
             ssl_ocsp_expected_cert: A PEM armoured string containing the expected certificate to be returned from the ocsp verification service.
+            ssl_min_version: The lowest supported SSL version. It affects the supported SSL versions of the SSLContext. None leaves the default provided by ssl module.
 
         Raises:
             RedisError
         """  # noqa
         if not SSL_AVAILABLE:
             raise RedisError("Python wasn't built with SSL support")
 
@@ -815,14 +811,15 @@
         self.ca_path = ssl_ca_path
         self.check_hostname = ssl_check_hostname
         self.certificate_password = ssl_password
         self.ssl_validate_ocsp = ssl_validate_ocsp
         self.ssl_validate_ocsp_stapled = ssl_validate_ocsp_stapled
         self.ssl_ocsp_context = ssl_ocsp_context
         self.ssl_ocsp_expected_cert = ssl_ocsp_expected_cert
+        self.ssl_min_version = ssl_min_version
         super().__init__(**kwargs)
 
     def _connect(self):
         "Wrap the socket with SSL support"
         sock = super()._connect()
         context = ssl.create_default_context()
         context.check_hostname = self.check_hostname
@@ -837,14 +834,16 @@
             self.ca_certs is not None
             or self.ca_path is not None
             or self.ca_data is not None
         ):
             context.load_verify_locations(
                 cafile=self.ca_certs, capath=self.ca_path, cadata=self.ca_data
             )
+        if self.ssl_min_version is not None:
+            context.minimum_version = self.ssl_min_version
         sslsock = context.wrap_socket(sock, server_hostname=self.host)
         if self.ssl_validate_ocsp is True and CRYPTOGRAPHY_AVAILABLE is False:
             raise RedisError("cryptography is not installed.")
 
         if self.ssl_validate_ocsp_stapled and self.ssl_validate_ocsp:
             raise RedisError(
                 "Either an OCSP staple or pure OCSP connection must be validated "
@@ -1178,20 +1177,23 @@
             except IndexError:
                 connection = self.make_connection()
             self._in_use_connections.add(connection)
 
         try:
             # ensure this connection is connected to Redis
             connection.connect()
-            # connections that the pool provides should be ready to send
-            # a command. if not, the connection was either returned to the
+            # if client caching is not enabled connections that the pool
+            # provides should be ready to send a command.
+            # if not, the connection was either returned to the
             # pool before all data has been read or the socket has been
             # closed. either way, reconnect and verify everything is good.
+            # (if caching enabled the connection will not always be ready
+            # to send a command because it may contain invalidation messages)
             try:
-                if connection.can_read():
+                if connection.can_read() and connection.client_cache is None:
                     raise ConnectionError("Connection has data")
             except (ConnectionError, OSError):
                 connection.disconnect()
                 connection.connect()
                 if connection.can_read():
                     raise ConnectionError("Connection not ready")
         except BaseException:
```

### Comparing `redis-5.1.0b3/redis/crc.py` & `redis-5.1.0b4/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/credentials.py` & `redis-5.1.0b4/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/exceptions.py` & `redis-5.1.0b4/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/lock.py` & `redis-5.1.0b4/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/ocsp.py` & `redis-5.1.0b4/redis/ocsp.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/retry.py` & `redis-5.1.0b4/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/sentinel.py` & `redis-5.1.0b4/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/typing.py` & `redis-5.1.0b4/redis/typing.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis/utils.py` & `redis-5.1.0b4/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/redis.egg-info/PKG-INFO` & `redis-5.1.0b4/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.1.0b3
+Version: 5.1.0b4
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.1.0b3/redis.egg-info/SOURCES.txt` & `redis-5.1.0b4/redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/setup.py` & `redis-5.1.0b4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.1.0b3",
+    version="5.1.0b4",
     packages=find_packages(
         include=[
             "redis",
             "redis._parsers",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
@@ -32,15 +32,14 @@
         "Code": "https://github.com/redis/redis-py",
         "Issue tracker": "https://github.com/redis/redis-py/issues",
     },
     author="Redis Inc.",
     author_email="oss@redis.com",
     python_requires=">=3.8",
     install_requires=[
-        'typing-extensions; python_version<"3.8"',
         'async-timeout>=4.0.3',
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `redis-5.1.0b3/tests/conftest.py` & `redis-5.1.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/mocks.py` & `redis-5.1.0b4/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/ssl_utils.py` & `redis-5.1.0b4/tests/ssl_utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/conftest.py` & `redis-5.1.0b4/tests/test_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/mocks.py` & `redis-5.1.0b4/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_bloom.py` & `redis-5.1.0b4/tests/test_asyncio/test_bloom.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,49 +11,45 @@
 )
 
 
 def intlist(obj):
     return [int(v) for v in obj]
 
 
-@pytest.mark.redismod
 async def test_create(decoded_r: redis.Redis):
     """Test CREATE/RESERVE calls"""
     assert await decoded_r.bf().create("bloom", 0.01, 1000)
     assert await decoded_r.bf().create("bloom_e", 0.01, 1000, expansion=1)
     assert await decoded_r.bf().create("bloom_ns", 0.01, 1000, noScale=True)
     assert await decoded_r.cf().create("cuckoo", 1000)
     assert await decoded_r.cf().create("cuckoo_e", 1000, expansion=1)
     assert await decoded_r.cf().create("cuckoo_bs", 1000, bucket_size=4)
     assert await decoded_r.cf().create("cuckoo_mi", 1000, max_iterations=10)
     assert await decoded_r.cms().initbydim("cmsDim", 100, 5)
     assert await decoded_r.cms().initbyprob("cmsProb", 0.01, 0.01)
     assert await decoded_r.topk().reserve("topk", 5, 100, 5, 0.9)
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_create(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 100)
 
 
-@pytest.mark.redismod
 async def test_bf_add(decoded_r: redis.Redis):
     assert await decoded_r.bf().create("bloom", 0.01, 1000)
     assert 1 == await decoded_r.bf().add("bloom", "foo")
     assert 0 == await decoded_r.bf().add("bloom", "foo")
     assert [0] == intlist(await decoded_r.bf().madd("bloom", "foo"))
     assert [0, 1] == await decoded_r.bf().madd("bloom", "foo", "bar")
     assert [0, 0, 1] == await decoded_r.bf().madd("bloom", "foo", "bar", "baz")
     assert 1 == await decoded_r.bf().exists("bloom", "foo")
     assert 0 == await decoded_r.bf().exists("bloom", "noexist")
     assert [1, 0] == intlist(await decoded_r.bf().mexists("bloom", "foo", "noexist"))
 
 
-@pytest.mark.redismod
 async def test_bf_insert(decoded_r: redis.Redis):
     assert await decoded_r.bf().create("bloom", 0.01, 1000)
     assert [1] == intlist(await decoded_r.bf().insert("bloom", ["foo"]))
     assert [0, 1] == intlist(await decoded_r.bf().insert("bloom", ["foo", "bar"]))
     assert [1] == intlist(await decoded_r.bf().insert("captest", ["foo"], capacity=10))
     assert [1] == intlist(await decoded_r.bf().insert("errtest", ["foo"], error=0.01))
     assert 1 == await decoded_r.bf().exists("bloom", "foo")
@@ -76,15 +72,14 @@
         decoded_r,
         1,
         info.get("filterNum"),
         info.get("Number of filters"),
     )
 
 
-@pytest.mark.redismod
 async def test_bf_scandump_and_loadchunk(decoded_r: redis.Redis):
     # Store a filter
     await decoded_r.bf().create("myBloom", "0.0001", "1000")
 
     # test is probabilistic and might fail. It is OK to change variables if
     # certain to not break anything
     async def do_verify():
@@ -128,15 +123,14 @@
     assert prev_info == cur_info
     await do_verify()
 
     await decoded_r.bf().client.delete("myBloom")
     await decoded_r.bf().create("myBloom", "0.0001", "10000000")
 
 
-@pytest.mark.redismod
 async def test_bf_info(decoded_r: redis.Redis):
     expansion = 4
     # Store a filter
     await decoded_r.bf().create("nonscaling", "0.0001", "1000", noScale=True)
     info = await decoded_r.bf().info("nonscaling")
     assert_resp_response(
         decoded_r,
@@ -160,30 +154,28 @@
             "myBloom", "0.0001", "1000", expansion=expansion, noScale=True
         )
         assert False
     except RedisError:
         assert True
 
 
-@pytest.mark.redismod
 async def test_bf_card(decoded_r: redis.Redis):
     # return 0 if the key does not exist
     assert await decoded_r.bf().card("not_exist") == 0
 
     # Store a filter
     assert await decoded_r.bf().add("bf1", "item_foo") == 1
     assert await decoded_r.bf().card("bf1") == 1
 
     # Error when key is of a type other than Bloom filtedecoded_r.
     with pytest.raises(redis.ResponseError):
         await decoded_r.set("setKey", "value")
         await decoded_r.bf().card("setKey")
 
 
-@pytest.mark.redismod
 async def test_cf_add_and_insert(decoded_r: redis.Redis):
     assert await decoded_r.cf().create("cuckoo", 1000)
     assert await decoded_r.cf().add("cuckoo", "filter")
     assert not await decoded_r.cf().addnx("cuckoo", "filter")
     assert 1 == await decoded_r.cf().addnx("cuckoo", "newItem")
     assert [1] == await decoded_r.cf().insert("captest", ["foo"])
     assert [1] == await decoded_r.cf().insert("captest", ["foo"], capacity=1000)
@@ -201,27 +193,25 @@
         decoded_r, 0, info.get("deletedNum"), info.get("Number of items deleted")
     )
     assert_resp_response(
         decoded_r, 1, info.get("filterNum"), info.get("Number of filters")
     )
 
 
-@pytest.mark.redismod
 async def test_cf_exists_and_del(decoded_r: redis.Redis):
     assert await decoded_r.cf().create("cuckoo", 1000)
     assert await decoded_r.cf().add("cuckoo", "filter")
     assert await decoded_r.cf().exists("cuckoo", "filter")
     assert not await decoded_r.cf().exists("cuckoo", "notexist")
     assert 1 == await decoded_r.cf().count("cuckoo", "filter")
     assert 0 == await decoded_r.cf().count("cuckoo", "notexist")
     assert await decoded_r.cf().delete("cuckoo", "filter")
     assert 0 == await decoded_r.cf().count("cuckoo", "filter")
 
 
-@pytest.mark.redismod
 async def test_cms(decoded_r: redis.Redis):
     assert await decoded_r.cms().initbydim("dim", 1000, 5)
     assert await decoded_r.cms().initbyprob("prob", 0.01, 0.01)
     assert await decoded_r.cms().incrby("dim", ["foo"], [5])
     assert [0] == await decoded_r.cms().query("dim", "notexist")
     assert [5] == await decoded_r.cms().query("dim", "foo")
     assert [10, 15] == await decoded_r.cms().incrby("dim", ["foo", "bar"], [5, 15])
@@ -229,15 +219,14 @@
     info = await decoded_r.cms().info("dim")
     assert info["width"]
     assert 1000 == info["width"]
     assert 5 == info["depth"]
     assert 25 == info["count"]
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_cms_merge(decoded_r: redis.Redis):
     assert await decoded_r.cms().initbydim("A", 1000, 5)
     assert await decoded_r.cms().initbydim("B", 1000, 5)
     assert await decoded_r.cms().initbydim("C", 1000, 5)
     assert await decoded_r.cms().incrby("A", ["foo", "bar", "baz"], [5, 3, 9])
     assert await decoded_r.cms().incrby("B", ["foo", "bar", "baz"], [2, 3, 1])
@@ -247,15 +236,14 @@
     assert [7, 6, 10] == await decoded_r.cms().query("C", "foo", "bar", "baz")
     assert await decoded_r.cms().merge("C", 2, ["A", "B"], ["1", "2"])
     assert [9, 9, 11] == await decoded_r.cms().query("C", "foo", "bar", "baz")
     assert await decoded_r.cms().merge("C", 2, ["A", "B"], ["2", "3"])
     assert [16, 15, 21] == await decoded_r.cms().query("C", "foo", "bar", "baz")
 
 
-@pytest.mark.redismod
 async def test_topk(decoded_r: redis.Redis):
     # test list with empty buckets
     assert await decoded_r.topk().reserve("topk", 3, 50, 4, 0.9)
     assert [
         None,
         None,
         None,
@@ -328,30 +316,28 @@
     info = await decoded_r.topk().info("topklist")
     assert 3 == info["k"]
     assert 50 == info["width"]
     assert 3 == info["depth"]
     assert 0.9 == round(float(info["decay"]), 1)
 
 
-@pytest.mark.redismod
 async def test_topk_incrby(decoded_r: redis.Redis):
     await decoded_r.flushdb()
     assert await decoded_r.topk().reserve("topk", 3, 10, 3, 1)
     assert [None, None, None] == await decoded_r.topk().incrby(
         "topk", ["bar", "baz", "42"], [3, 6, 2]
     )
     res = await decoded_r.topk().incrby("topk", ["42", "xyzzy"], [8, 4])
     assert [None, "bar"] == res
     with pytest.deprecated_call():
         assert [3, 6, 10, 4, 0] == await decoded_r.topk().count(
             "topk", "bar", "baz", "42", "xyzzy", 4
         )
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_reset(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 10)
     # reset on empty histogram
     assert await decoded_r.tdigest().reset("tDigest")
     # insert data-points into sketch
     assert await decoded_r.tdigest().add("tDigest", list(range(10)))
@@ -360,15 +346,14 @@
     # assert we have 0 unmerged nodes
     info = await decoded_r.tdigest().info("tDigest")
     assert_resp_response(
         decoded_r, 0, info.get("unmerged_nodes"), info.get("Unmerged nodes")
     )
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_tdigest_merge(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("to-tDigest", 10)
     assert await decoded_r.tdigest().create("from-tDigest", 10)
     # insert data-points into sketch
     assert await decoded_r.tdigest().add("from-tDigest", [1.0] * 10)
     assert await decoded_r.tdigest().add("to-tDigest", [2.0] * 10)
@@ -388,26 +373,24 @@
     assert await decoded_r.tdigest().merge(
         "to-tDigest", 2, "from-override", "from-override-2", override=True
     )
     assert 3.0 == await decoded_r.tdigest().min("to-tDigest")
     assert 4.0 == await decoded_r.tdigest().max("to-tDigest")
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_min_and_max(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 100)
     # insert data-points into sketch
     assert await decoded_r.tdigest().add("tDigest", [1, 2, 3])
     # min/max
     assert 3 == await decoded_r.tdigest().max("tDigest")
     assert 1 == await decoded_r.tdigest().min("tDigest")
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 @skip_ifmodversion_lt("2.4.0", "bf")
 async def test_tdigest_quantile(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 500)
     # insert data-points into sketch
     assert await decoded_r.tdigest().add(
         "tDigest", list([x * 0.01 for x in range(1, 10000)])
@@ -428,84 +411,77 @@
     # test multiple quantiles
     assert await decoded_r.tdigest().create("t-digest", 100)
     assert await decoded_r.tdigest().add("t-digest", [1, 2, 3, 4, 5])
     res = await decoded_r.tdigest().quantile("t-digest", 0.5, 0.8)
     assert [3.0, 5.0] == res
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_cdf(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 100)
     # insert data-points into sketch
     assert await decoded_r.tdigest().add("tDigest", list(range(1, 10)))
     assert 0.1 == round((await decoded_r.tdigest().cdf("tDigest", 1.0))[0], 1)
     assert 0.9 == round((await decoded_r.tdigest().cdf("tDigest", 9.0))[0], 1)
     res = await decoded_r.tdigest().cdf("tDigest", 1.0, 9.0)
     assert [0.1, 0.9] == [round(x, 1) for x in res]
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 @skip_ifmodversion_lt("2.4.0", "bf")
 async def test_tdigest_trimmed_mean(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("tDigest", 100)
     # insert data-points into sketch
     assert await decoded_r.tdigest().add("tDigest", list(range(1, 10)))
     assert 5 == await decoded_r.tdigest().trimmed_mean("tDigest", 0.1, 0.9)
     assert 4.5 == await decoded_r.tdigest().trimmed_mean("tDigest", 0.4, 0.5)
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_rank(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("t-digest", 500)
     assert await decoded_r.tdigest().add("t-digest", list(range(0, 20)))
     assert -1 == (await decoded_r.tdigest().rank("t-digest", -1))[0]
     assert 0 == (await decoded_r.tdigest().rank("t-digest", 0))[0]
     assert 10 == (await decoded_r.tdigest().rank("t-digest", 10))[0]
     assert [-1, 20, 9] == await decoded_r.tdigest().rank("t-digest", -20, 20, 9)
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_revrank(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("t-digest", 500)
     assert await decoded_r.tdigest().add("t-digest", list(range(0, 20)))
     assert -1 == (await decoded_r.tdigest().revrank("t-digest", 20))[0]
     assert 19 == (await decoded_r.tdigest().revrank("t-digest", 0))[0]
     assert [-1, 19, 9] == await decoded_r.tdigest().revrank("t-digest", 21, 0, 10)
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_byrank(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("t-digest", 500)
     assert await decoded_r.tdigest().add("t-digest", list(range(1, 11)))
     assert 1 == (await decoded_r.tdigest().byrank("t-digest", 0))[0]
     assert 10 == (await decoded_r.tdigest().byrank("t-digest", 9))[0]
     assert (await decoded_r.tdigest().byrank("t-digest", 100))[0] == inf
     with pytest.raises(redis.ResponseError):
         (await decoded_r.tdigest().byrank("t-digest", -1))[0]
 
 
-@pytest.mark.redismod
 @pytest.mark.experimental
 async def test_tdigest_byrevrank(decoded_r: redis.Redis):
     assert await decoded_r.tdigest().create("t-digest", 500)
     assert await decoded_r.tdigest().add("t-digest", list(range(1, 11)))
     assert 10 == (await decoded_r.tdigest().byrevrank("t-digest", 0))[0]
     assert 1 == (await decoded_r.tdigest().byrevrank("t-digest", 9))[0]
     assert (await decoded_r.tdigest().byrevrank("t-digest", 100))[0] == -inf
     with pytest.raises(redis.ResponseError):
         (await decoded_r.tdigest().byrevrank("t-digest", -1))[0]
 
 
-# @pytest.mark.redismod
-# async def test_pipeline(decoded_r: redis.Redis):
+# # async def test_pipeline(decoded_r: redis.Redis):
 #     pipeline = await decoded_r.bf().pipeline()
 #     assert not await decoded_r.bf().execute_command("get pipeline")
 #
 #     assert await decoded_r.bf().create("pipeline", 0.01, 1000)
 #     for i in range(100):
 #         pipeline.add("pipeline", i)
 #     for i in range(100):
```

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_cache.py` & `redis-5.1.0b4/tests/test_asyncio/test_cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -138,14 +138,56 @@
         assert await r.lrange("mylist", 0, -1) == [b"baz", b"bar", b"foo"]
         res = cache.get(("LRANGE", "mylist", 0, -1))
         assert res == [b"baz", b"bar", b"foo"]
         res.append(b"new")
         check = cache.get(("LRANGE", "mylist", 0, -1))
         assert check == [b"baz", b"bar", b"foo"]
 
+    @pytest.mark.onlynoncluster
+    @pytest.mark.parametrize(
+        "r",
+        [{"cache": _LocalCache(), "kwargs": {"decode_responses": True}}],
+        indirect=True,
+    )
+    async def test_csc_not_cause_disconnects(self, r):
+        r, cache = r
+        id1 = await r.client_id()
+        await r.mset({"a": 1, "b": 1, "c": 1, "d": 1, "e": 1})
+        assert await r.mget("a", "b", "c", "d", "e") == ["1", "1", "1", "1", "1"]
+        id2 = await r.client_id()
+
+        # client should get value from client cache
+        assert await r.mget("a", "b", "c", "d", "e") == ["1", "1", "1", "1", "1"]
+        assert cache.get(("MGET", "a", "b", "c", "d", "e")) == [
+            "1",
+            "1",
+            "1",
+            "1",
+            "1",
+        ]
+
+        await r.mset({"a": 2, "b": 2, "c": 2, "d": 2, "e": 2})
+        id3 = await r.client_id()
+        # client should get value from redis server post invalidate messages
+        assert await r.mget("a", "b", "c", "d", "e") == ["2", "2", "2", "2", "2"]
+
+        await r.mset({"a": 3, "b": 3, "c": 3, "d": 3, "e": 3})
+        # need to check that we get correct value 3 and not 2
+        assert await r.mget("a", "b", "c", "d", "e") == ["3", "3", "3", "3", "3"]
+        # client should get value from client cache
+        assert await r.mget("a", "b", "c", "d", "e") == ["3", "3", "3", "3", "3"]
+
+        await r.mset({"a": 4, "b": 4, "c": 4, "d": 4, "e": 4})
+        # need to check that we get correct value 4 and not 3
+        assert await r.mget("a", "b", "c", "d", "e") == ["4", "4", "4", "4", "4"]
+        # client should get value from client cache
+        assert await r.mget("a", "b", "c", "d", "e") == ["4", "4", "4", "4", "4"]
+        id4 = await r.client_id()
+        assert id1 == id2 == id3 == id4
+
 
 @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
 @pytest.mark.onlycluster
 class TestClusterLocalCache:
     @pytest.mark.parametrize("r", [{"cache": _LocalCache()}], indirect=True)
     async def test_get_from_cache(self, r, r2):
         r, cache = r
```

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_cluster.py` & `redis-5.1.0b4/tests/test_asyncio/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_commands.py` & `redis-5.1.0b4/tests/test_asyncio/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_connection.py` & `redis-5.1.0b4/tests/test_asyncio/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_connection_pool.py` & `redis-5.1.0b4/tests/test_asyncio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_credentials.py` & `redis-5.1.0b4/tests/test_asyncio/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_cwe_404.py` & `redis-5.1.0b4/tests/test_asyncio/test_cwe_404.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_encoding.py` & `redis-5.1.0b4/tests/test_asyncio/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_graph.py` & `redis-5.1.0b4/tests/test_asyncio/test_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 import redis.asyncio as redis
 from redis.commands.graph import Edge, Node, Path
 from redis.commands.graph.execution_plan import Operation
 from redis.exceptions import ResponseError
 from tests.conftest import skip_if_redis_enterprise
 
 
-@pytest.mark.redismod
 async def test_bulk(decoded_r):
     with pytest.raises(NotImplementedError):
         await decoded_r.graph().bulk()
         await decoded_r.graph().bulk(foo="bar!")
 
 
-@pytest.mark.redismod
 async def test_graph_creation(decoded_r: redis.Redis):
     graph = decoded_r.graph()
 
     john = Node(
         label="person",
         properties={
             "name": "John Doe",
@@ -54,15 +52,14 @@
     result = await graph.query(query)
     assert [1, 2.3, "4", True, False, None] == result.result_set[0][0]
 
     # All done, remove graph.
     await graph.delete()
 
 
-@pytest.mark.redismod
 async def test_array_functions(decoded_r: redis.Redis):
     graph = decoded_r.graph()
 
     query = """CREATE (p:person{name:'a',age:32, array:[0,1,2]})"""
     await graph.query(query)
 
     query = """WITH [0,1,2] as x return x"""
@@ -77,15 +74,14 @@
         label="person",
         properties={"name": "a", "age": 32, "array": [0, 1, 2]},
     )
 
     assert [a] == result.result_set[0][0]
 
 
-@pytest.mark.redismod
 async def test_path(decoded_r: redis.Redis):
     node0 = Node(node_id=0, label="L1")
     node1 = Node(node_id=1, label="L1")
     edge01 = Edge(node0, "R1", node1, edge_id=0, properties={"value": 1})
 
     graph = decoded_r.graph()
     graph.add_node(node0)
@@ -97,25 +93,23 @@
     expected_results = [[path01]]
 
     query = "MATCH p=(:L1)-[:R1]->(:L1) RETURN p ORDER BY p"
     result = await graph.query(query)
     assert expected_results == result.result_set
 
 
-@pytest.mark.redismod
 async def test_param(decoded_r: redis.Redis):
     params = [1, 2.3, "str", True, False, None, [0, 1, 2]]
     query = "RETURN $param"
     for param in params:
         result = await decoded_r.graph().query(query, {"param": param})
         expected_results = [[param]]
         assert expected_results == result.result_set
 
 
-@pytest.mark.redismod
 async def test_map(decoded_r: redis.Redis):
     query = "RETURN {a:1, b:'str', c:NULL, d:[1,2,3], e:True, f:{x:1, y:2}}"
 
     actual = (await decoded_r.graph().query(query)).result_set[0][0]
     expected = {
         "a": 1,
         "b": "str",
@@ -124,15 +118,14 @@
         "e": True,
         "f": {"x": 1, "y": 2},
     }
 
     assert actual == expected
 
 
-@pytest.mark.redismod
 async def test_point(decoded_r: redis.Redis):
     query = "RETURN point({latitude: 32.070794860, longitude: 34.820751118})"
     expected_lat = 32.070794860
     expected_lon = 34.820751118
     actual = (await decoded_r.graph().query(query)).result_set[0][0]
     assert abs(actual["latitude"] - expected_lat) < 0.001
     assert abs(actual["longitude"] - expected_lon) < 0.001
@@ -141,30 +134,28 @@
     expected_lat = 32
     expected_lon = 34
     actual = (await decoded_r.graph().query(query)).result_set[0][0]
     assert abs(actual["latitude"] - expected_lat) < 0.001
     assert abs(actual["longitude"] - expected_lon) < 0.001
 
 
-@pytest.mark.redismod
 async def test_index_response(decoded_r: redis.Redis):
     result_set = await decoded_r.graph().query("CREATE INDEX ON :person(age)")
     assert 1 == result_set.indices_created
 
     result_set = await decoded_r.graph().query("CREATE INDEX ON :person(age)")
     assert 0 == result_set.indices_created
 
     result_set = await decoded_r.graph().query("DROP INDEX ON :person(age)")
     assert 1 == result_set.indices_deleted
 
     with pytest.raises(ResponseError):
         await decoded_r.graph().query("DROP INDEX ON :person(age)")
 
 
-@pytest.mark.redismod
 async def test_stringify_query_result(decoded_r: redis.Redis):
     graph = decoded_r.graph()
 
     john = Node(
         alias="a",
         label="person",
         properties={
@@ -210,15 +201,14 @@
     )
     assert str(visit) == """()-[:visited{purpose:"pleasure"}]->()"""
     assert str(country) == """(:country{name:"Japan"})"""
 
     await graph.delete()
 
 
-@pytest.mark.redismod
 async def test_optional_match(decoded_r: redis.Redis):
     # Build a graph of form (a)-[R]->(b)
     node0 = Node(node_id=0, label="L1", properties={"value": "a"})
     node1 = Node(node_id=1, label="L1", properties={"value": "b"})
 
     edge01 = Edge(node0, "R", node1, edge_id=0)
 
@@ -235,15 +225,14 @@
 
     result = await graph.query(query)
     assert expected_results == result.result_set
 
     await graph.delete()
 
 
-@pytest.mark.redismod
 async def test_cached_execution(decoded_r: redis.Redis):
     await decoded_r.graph().query("CREATE ()")
 
     uncached_result = await decoded_r.graph().query(
         "MATCH (n) RETURN n, $param", {"param": [0]}
     )
     assert uncached_result.cached_execution is False
@@ -255,67 +244,62 @@
         )
         assert uncached_result.result_set == cached_result.result_set
 
     # should be cached on all threads by now
     assert cached_result.cached_execution
 
 
-@pytest.mark.redismod
 async def test_slowlog(decoded_r: redis.Redis):
     create_query = """CREATE
     (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
     (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
     (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
     await decoded_r.graph().query(create_query)
 
     results = await decoded_r.graph().slowlog()
     assert results[0][1] == "GRAPH.QUERY"
     assert results[0][2] == create_query
 
 
-@pytest.mark.redismod
 @pytest.mark.xfail(strict=False)
 async def test_query_timeout(decoded_r: redis.Redis):
     # Build a sample graph with 1000 nodes.
     await decoded_r.graph().query("UNWIND range(0,1000) as val CREATE ({v: val})")
     # Issue a long-running query with a 1-millisecond timeout.
     with pytest.raises(ResponseError):
         await decoded_r.graph().query("MATCH (a), (b), (c), (d) RETURN *", timeout=1)
         assert False is False
 
     with pytest.raises(Exception):
         await decoded_r.graph().query("RETURN 1", timeout="str")
         assert False is False
 
 
-@pytest.mark.redismod
 async def test_read_only_query(decoded_r: redis.Redis):
     with pytest.raises(Exception):
         # Issue a write query, specifying read-only true,
         # this call should fail.
         await decoded_r.graph().query("CREATE (p:person {name:'a'})", read_only=True)
         assert False is False
 
 
-@pytest.mark.redismod
 async def test_profile(decoded_r: redis.Redis):
     q = """UNWIND range(1, 3) AS x CREATE (p:Person {v:x})"""
     profile = (await decoded_r.graph().profile(q)).result_set
     assert "Create | Records produced: 3" in profile
     assert "Unwind | Records produced: 3" in profile
 
     q = "MATCH (p:Person) WHERE p.v > 1 RETURN p"
     profile = (await decoded_r.graph().profile(q)).result_set
     assert "Results | Records produced: 2" in profile
     assert "Project | Records produced: 2" in profile
     assert "Filter | Records produced: 2" in profile
     assert "Node By Label Scan | (p:Person) | Records produced: 3" in profile
 
 
-@pytest.mark.redismod
 @skip_if_redis_enterprise()
 async def test_config(decoded_r: redis.Redis):
     config_name = "RESULTSET_SIZE"
     config_value = 3
 
     # Set configuration
     response = await decoded_r.graph().config(config_name, config_value, set=True)
@@ -339,15 +323,14 @@
     assert response == expected_response
 
     # reset to default
     await decoded_r.graph().config("QUERY_MEM_CAPACITY", 0, set=True)
     await decoded_r.graph().config("RESULTSET_SIZE", -100, set=True)
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_list_keys(decoded_r: redis.Redis):
     result = await decoded_r.graph().list_keys()
     assert result == []
 
     await decoded_r.graph("G").query("CREATE (n)")
     result = await decoded_r.graph().list_keys()
@@ -363,15 +346,14 @@
     assert result == ["Z"]
 
     await decoded_r.delete("Z")
     result = await decoded_r.graph().list_keys()
     assert result == []
 
 
-@pytest.mark.redismod
 async def test_multi_label(decoded_r: redis.Redis):
     redis_graph = decoded_r.graph("g")
 
     node = Node(label=["l", "ll"])
     redis_graph.add_node(node)
     await redis_graph.commit()
 
@@ -389,15 +371,14 @@
     try:
         Node(label=["l", 1])
         assert False
     except AssertionError:
         assert True
 
 
-@pytest.mark.redismod
 async def test_execution_plan(decoded_r: redis.Redis):
     redis_graph = decoded_r.graph("execution_plan")
     create_query = """CREATE
     (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
     (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
     (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
     await redis_graph.query(create_query)
@@ -408,15 +389,14 @@
     )
     expected = "Results\n    Project\n        Conditional Traverse | (t)->(r:Rider)\n            Filter\n                Node By Label Scan | (t:Team)"  # noqa
     assert result == expected
 
     await redis_graph.delete()
 
 
-@pytest.mark.redismod
 async def test_explain(decoded_r: redis.Redis):
     redis_graph = decoded_r.graph("execution_plan")
     # graph creation / population
     create_query = """CREATE
 (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
 (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
 (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
```

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_json.py` & `redis-5.1.0b4/tests/test_asyncio/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 import pytest
 import redis.asyncio as redis
 from redis import exceptions
 from redis.commands.json.path import Path
 from tests.conftest import assert_resp_response, skip_ifmodversion_lt
 
 
-@pytest.mark.redismod
 async def test_json_setbinarykey(decoded_r: redis.Redis):
     d = {"hello": "world", b"some": "value"}
     with pytest.raises(TypeError):
         decoded_r.json().set("somekey", Path.root_path(), d)
     assert await decoded_r.json().set("somekey", Path.root_path(), d, decode_keys=True)
 
 
-@pytest.mark.redismod
 async def test_json_setgetdeleteforget(decoded_r: redis.Redis):
     assert await decoded_r.json().set("foo", Path.root_path(), "bar")
     assert_resp_response(decoded_r, await decoded_r.json().get("foo"), "bar", [["bar"]])
     assert await decoded_r.json().get("baz") is None
     assert await decoded_r.json().delete("foo") == 1
     assert await decoded_r.json().forget("foo") == 0  # second delete
     assert await decoded_r.exists("foo") == 0
 
 
-@pytest.mark.redismod
 async def test_jsonget(decoded_r: redis.Redis):
     await decoded_r.json().set("foo", Path.root_path(), "bar")
     assert_resp_response(decoded_r, await decoded_r.json().get("foo"), "bar", [["bar"]])
 
 
-@pytest.mark.redismod
 async def test_json_get_jset(decoded_r: redis.Redis):
     assert await decoded_r.json().set("foo", Path.root_path(), "bar")
     assert_resp_response(decoded_r, await decoded_r.json().get("foo"), "bar", [["bar"]])
     assert await decoded_r.json().get("baz") is None
     assert 1 == await decoded_r.json().delete("foo")
     assert await decoded_r.exists("foo") == 0
 
 
-@pytest.mark.redismod
 async def test_nonascii_setgetdelete(decoded_r: redis.Redis):
     assert await decoded_r.json().set("notascii", Path.root_path(), "hyvää-élève")
     res = "hyvää-élève"
     assert_resp_response(
         decoded_r, await decoded_r.json().get("notascii", no_escape=True), res, [[res]]
     )
     assert 1 == await decoded_r.json().delete("notascii")
     assert await decoded_r.exists("notascii") == 0
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("2.6.0", "ReJSON")
 async def test_json_merge(decoded_r: redis.Redis):
     # Test with root path $
     assert await decoded_r.json().set(
         "person_data",
         "$",
         {"person1": {"personal_data": {"name": "John"}}},
@@ -80,15 +74,14 @@
         "person_data", "$.person1.personal_data", {"name": None}
     )
     assert await decoded_r.json().get("person_data") == {
         "person1": {"personal_data": {"country": "Israel", "hobbies": "reading"}}
     }
 
 
-@pytest.mark.redismod
 async def test_jsonsetexistentialmodifiersshouldsucceed(decoded_r: redis.Redis):
     obj = {"foo": "bar"}
     assert await decoded_r.json().set("obj", Path.root_path(), obj)
 
     # Test that flags prevent updates when conditions are unmet
     assert await decoded_r.json().set("obj", Path("foo"), "baz", nx=True) is None
     assert await decoded_r.json().set("obj", Path("qaz"), "baz", xx=True) is None
@@ -98,155 +91,141 @@
     assert await decoded_r.json().set("obj", Path("qaz"), "baz", nx=True)
 
     # Test that flags are mutually exlusive
     with pytest.raises(Exception):
         await decoded_r.json().set("obj", Path("foo"), "baz", nx=True, xx=True)
 
 
-@pytest.mark.redismod
 async def test_mgetshouldsucceed(decoded_r: redis.Redis):
     await decoded_r.json().set("1", Path.root_path(), 1)
     await decoded_r.json().set("2", Path.root_path(), 2)
     assert await decoded_r.json().mget(["1"], Path.root_path()) == [1]
 
     assert await decoded_r.json().mget([1, 2], Path.root_path()) == [1, 2]
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 @skip_ifmodversion_lt("2.6.0", "ReJSON")
 async def test_mset(decoded_r: redis.Redis):
     await decoded_r.json().mset(
         [("1", Path.root_path(), 1), ("2", Path.root_path(), 2)]
     )
 
     assert await decoded_r.json().mget(["1"], Path.root_path()) == [1]
     assert await decoded_r.json().mget(["1", "2"], Path.root_path()) == [1, 2]
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 async def test_clear(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 1 == await decoded_r.json().clear("arr", Path.root_path())
     assert_resp_response(decoded_r, await decoded_r.json().get("arr"), [], [[[]]])
 
 
-@pytest.mark.redismod
 async def test_type(decoded_r: redis.Redis):
     await decoded_r.json().set("1", Path.root_path(), 1)
     assert_resp_response(
         decoded_r,
         await decoded_r.json().type("1", Path.root_path()),
         "integer",
         ["integer"],
     )
     assert_resp_response(
         decoded_r, await decoded_r.json().type("1"), "integer", ["integer"]
     )
 
 
-@pytest.mark.redismod
 async def test_numincrby(decoded_r):
     await decoded_r.json().set("num", Path.root_path(), 1)
     assert_resp_response(
         decoded_r, await decoded_r.json().numincrby("num", Path.root_path(), 1), 2, [2]
     )
     res = await decoded_r.json().numincrby("num", Path.root_path(), 0.5)
     assert_resp_response(decoded_r, res, 2.5, [2.5])
     res = await decoded_r.json().numincrby("num", Path.root_path(), -1.25)
     assert_resp_response(decoded_r, res, 1.25, [1.25])
 
 
-@pytest.mark.redismod
 async def test_nummultby(decoded_r: redis.Redis):
     await decoded_r.json().set("num", Path.root_path(), 1)
 
     with pytest.deprecated_call():
         res = await decoded_r.json().nummultby("num", Path.root_path(), 2)
         assert_resp_response(decoded_r, res, 2, [2])
         res = await decoded_r.json().nummultby("num", Path.root_path(), 2.5)
         assert_resp_response(decoded_r, res, 5, [5])
         res = await decoded_r.json().nummultby("num", Path.root_path(), 0.5)
         assert_resp_response(decoded_r, res, 2.5, [2.5])
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 async def test_toggle(decoded_r: redis.Redis):
     await decoded_r.json().set("bool", Path.root_path(), False)
     assert await decoded_r.json().toggle("bool", Path.root_path())
     assert await decoded_r.json().toggle("bool", Path.root_path()) is False
     # check non-boolean value
     await decoded_r.json().set("num", Path.root_path(), 1)
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().toggle("num", Path.root_path())
 
 
-@pytest.mark.redismod
 async def test_strappend(decoded_r: redis.Redis):
     await decoded_r.json().set("jsonkey", Path.root_path(), "foo")
     assert 6 == await decoded_r.json().strappend("jsonkey", "bar")
     res = await decoded_r.json().get("jsonkey", Path.root_path())
     assert_resp_response(decoded_r, res, "foobar", [["foobar"]])
 
 
-@pytest.mark.redismod
 async def test_strlen(decoded_r: redis.Redis):
     await decoded_r.json().set("str", Path.root_path(), "foo")
     assert 3 == await decoded_r.json().strlen("str", Path.root_path())
     await decoded_r.json().strappend("str", "bar", Path.root_path())
     assert 6 == await decoded_r.json().strlen("str", Path.root_path())
     assert 6 == await decoded_r.json().strlen("str")
 
 
-@pytest.mark.redismod
 async def test_arrappend(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [1])
     assert 2 == await decoded_r.json().arrappend("arr", Path.root_path(), 2)
     assert 4 == await decoded_r.json().arrappend("arr", Path.root_path(), 3, 4)
     assert 7 == await decoded_r.json().arrappend("arr", Path.root_path(), *[5, 6, 7])
 
 
-@pytest.mark.redismod
 async def test_arrindex(decoded_r: redis.Redis):
     r_path = Path.root_path()
     await decoded_r.json().set("arr", r_path, [0, 1, 2, 3, 4])
     assert 1 == await decoded_r.json().arrindex("arr", r_path, 1)
     assert -1 == await decoded_r.json().arrindex("arr", r_path, 1, 2)
     assert 4 == await decoded_r.json().arrindex("arr", r_path, 4)
     assert 4 == await decoded_r.json().arrindex("arr", r_path, 4, start=0)
     assert 4 == await decoded_r.json().arrindex("arr", r_path, 4, start=0, stop=5000)
     assert -1 == await decoded_r.json().arrindex("arr", r_path, 4, start=0, stop=-1)
     assert -1 == await decoded_r.json().arrindex("arr", r_path, 4, start=1, stop=3)
 
 
-@pytest.mark.redismod
 async def test_arrinsert(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 4])
     assert 5 == await decoded_r.json().arrinsert("arr", Path.root_path(), 1, *[1, 2, 3])
     res = [0, 1, 2, 3, 4]
     assert_resp_response(decoded_r, await decoded_r.json().get("arr"), res, [[res]])
 
     # test prepends
     await decoded_r.json().set("val2", Path.root_path(), [5, 6, 7, 8, 9])
     await decoded_r.json().arrinsert("val2", Path.root_path(), 0, ["some", "thing"])
     res = [["some", "thing"], 5, 6, 7, 8, 9]
     assert_resp_response(decoded_r, await decoded_r.json().get("val2"), res, [[res]])
 
 
-@pytest.mark.redismod
 async def test_arrlen(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 5 == await decoded_r.json().arrlen("arr", Path.root_path())
     assert 5 == await decoded_r.json().arrlen("arr")
     assert await decoded_r.json().arrlen("fakekey") is None
 
 
-@pytest.mark.redismod
 async def test_arrpop(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 4 == await decoded_r.json().arrpop("arr", Path.root_path(), 4)
     assert 3 == await decoded_r.json().arrpop("arr", Path.root_path(), -1)
     assert 2 == await decoded_r.json().arrpop("arr", Path.root_path())
     assert 0 == await decoded_r.json().arrpop("arr", Path.root_path(), 0)
     assert_resp_response(decoded_r, await decoded_r.json().get("arr"), [1], [[[1]]])
@@ -256,15 +235,14 @@
     assert 4 == await decoded_r.json().arrpop("arr", Path.root_path(), 99)
 
     # none test
     await decoded_r.json().set("arr", Path.root_path(), [])
     assert await decoded_r.json().arrpop("arr") is None
 
 
-@pytest.mark.redismod
 async def test_arrtrim(decoded_r: redis.Redis):
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 3 == await decoded_r.json().arrtrim("arr", Path.root_path(), 1, 3)
     res = await decoded_r.json().get("arr")
     assert_resp_response(decoded_r, res, [1, 2, 3], [[[1, 2, 3]]])
 
     # <0 test, should be 0 equivalent
@@ -280,25 +258,23 @@
     assert 0 == await decoded_r.json().arrtrim("arr", Path.root_path(), 9, 1)
 
     # all larger
     await decoded_r.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 0 == await decoded_r.json().arrtrim("arr", Path.root_path(), 9, 11)
 
 
-@pytest.mark.redismod
 async def test_resp(decoded_r: redis.Redis):
     obj = {"foo": "bar", "baz": 1, "qaz": True}
     await decoded_r.json().set("obj", Path.root_path(), obj)
     assert "bar" == await decoded_r.json().resp("obj", Path("foo"))
     assert 1 == await decoded_r.json().resp("obj", Path("baz"))
     assert await decoded_r.json().resp("obj", Path("qaz"))
     assert isinstance(await decoded_r.json().resp("obj"), list)
 
 
-@pytest.mark.redismod
 async def test_objkeys(decoded_r: redis.Redis):
     obj = {"foo": "bar", "baz": "qaz"}
     await decoded_r.json().set("obj", Path.root_path(), obj)
     keys = await decoded_r.json().objkeys("obj", Path.root_path())
     keys.sort()
     exp = list(obj.keys())
     exp.sort()
@@ -307,15 +283,14 @@
     await decoded_r.json().set("obj", Path.root_path(), obj)
     keys = await decoded_r.json().objkeys("obj")
     assert keys == list(obj.keys())
 
     assert await decoded_r.json().objkeys("fakekey") is None
 
 
-@pytest.mark.redismod
 async def test_objlen(decoded_r: redis.Redis):
     obj = {"foo": "bar", "baz": "qaz"}
     await decoded_r.json().set("obj", Path.root_path(), obj)
     assert len(obj) == await decoded_r.json().objlen("obj", Path.root_path())
 
     await decoded_r.json().set("obj", Path.root_path(), obj)
     assert len(obj) == await decoded_r.json().objlen("obj")
@@ -341,15 +316,14 @@
 #     p.exists("notarealkey")
 #     p.delete("foo")
 #     assert [True, d, 0, 1] == p.execute()
 #     assert await decoded_r.keys() == []
 #     assert await decoded_r.get("foo") is None
 
 
-@pytest.mark.redismod
 async def test_json_delete_with_dollar(decoded_r: redis.Redis):
     doc1 = {"a": 1, "nested": {"a": 2, "b": 3}}
     assert await decoded_r.json().set("doc1", "$", doc1)
     assert await decoded_r.json().delete("doc1", "$..a") == 2
     res = [{"nested": {"b": 3}}]
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
@@ -395,15 +369,14 @@
     # Test async default path
     assert await decoded_r.json().delete("doc3") == 1
     assert await decoded_r.json().get("doc3", "$") is None
 
     await decoded_r.json().delete("not_a_document", "..a")
 
 
-@pytest.mark.redismod
 async def test_json_forget_with_dollar(decoded_r: redis.Redis):
     doc1 = {"a": 1, "nested": {"a": 2, "b": 3}}
     assert await decoded_r.json().set("doc1", "$", doc1)
     assert await decoded_r.json().forget("doc1", "$..a") == 2
     res = [{"nested": {"b": 3}}]
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
@@ -448,15 +421,15 @@
     # Test async default path
     assert await decoded_r.json().forget("doc3") == 1
     assert await decoded_r.json().get("doc3", "$") is None
 
     await decoded_r.json().forget("not_a_document", "..a")
 
 
-@pytest.mark.redismod
+@pytest.mark.onlynoncluster
 async def test_json_mget_dollar(decoded_r: redis.Redis):
     # Test mget with multi paths
     await decoded_r.json().set(
         "doc1",
         "$",
         {"a": 1, "b": 2, "nested": {"a": 3}, "c": None, "nested2": {"a": None}},
     )
@@ -484,15 +457,14 @@
     # Test missing key
     res = await decoded_r.json().mget(["doc1", "missing_doc"], "$..a")
     assert res == [[1, 3, None], None]
     res = await decoded_r.json().mget(["missing_doc1", "missing_doc2"], "$..a")
     assert res == [None, None]
 
 
-@pytest.mark.redismod
 async def test_numby_commands_dollar(decoded_r: redis.Redis):
     # Test NUMINCRBY
     await decoded_r.json().set(
         "doc1", "$", {"a": "b", "b": [{"a": 2}, {"a": 5.0}, {"a": "c"}]}
     )
     # Test multi
     assert await decoded_r.json().numincrby("doc1", "$..a", 2) == [None, 4, 7.0, None]
@@ -539,15 +511,14 @@
         "doc1", "$", {"a": "b", "b": [{"a": 2}, {"a": 5.0}, {"a": "c"}]}
     )
 
     with pytest.deprecated_call():
         await decoded_r.json().nummultby("doc1", ".b[0].a", 3) == 6
 
 
-@pytest.mark.redismod
 async def test_strappend_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1", "$", {"a": "foo", "nested1": {"a": "hello"}, "nested2": {"a": 31}}
     )
     # Test multi
     await decoded_r.json().strappend("doc1", "bar", "$..a") == [6, 8, None]
 
@@ -570,15 +541,14 @@
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
     # Test missing path
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().strappend("doc1", "piu")
 
 
-@pytest.mark.redismod
 async def test_strlen_dollar(decoded_r: redis.Redis):
     # Test multi
     await decoded_r.json().set(
         "doc1", "$", {"a": "foo", "nested1": {"a": "hello"}, "nested2": {"a": 31}}
     )
     assert await decoded_r.json().strlen("doc1", "$..a") == [3, 5, None]
 
@@ -591,15 +561,14 @@
     await decoded_r.json().strlen("doc1", "$.nested2.a") == [None]
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().strlen("non_existing_doc", "$..a")
 
 
-@pytest.mark.redismod
 async def test_arrappend_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
@@ -665,15 +634,14 @@
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().arrappend("non_existing_doc", "$..a")
 
 
-@pytest.mark.redismod
 async def test_arrinsert_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
@@ -704,15 +672,14 @@
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().arrappend("non_existing_doc", "$..a")
 
 
-@pytest.mark.redismod
 async def test_arrlen_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
@@ -750,15 +717,14 @@
     # Test single
     assert await decoded_r.json().arrlen("doc1", ".nested1.a") == 6
 
     # Test missing key
     assert await decoded_r.json().arrlen("non_existing_doc", "..a") is None
 
 
-@pytest.mark.redismod
 async def test_arrpop_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
@@ -792,15 +758,14 @@
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
     # # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().arrpop("non_existing_doc", "..a")
 
 
-@pytest.mark.redismod
 async def test_arrtrim_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
@@ -844,15 +809,14 @@
     assert_resp_response(decoded_r, await decoded_r.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().arrtrim("non_existing_doc", "..a", 1, 1)
 
 
-@pytest.mark.redismod
 async def test_objkeys_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "nested1": {"a": {"foo": 10, "bar": 20}},
             "a": ["foo"],
@@ -874,15 +838,14 @@
     # Test non existing doc
     with pytest.raises(exceptions.ResponseError):
         assert await decoded_r.json().objkeys("non_existing_doc", "$..a") == []
 
     assert await decoded_r.json().objkeys("doc1", "$..nowhere") == []
 
 
-@pytest.mark.redismod
 async def test_objlen_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "nested1": {"a": {"foo": 10, "bar": 20}},
             "a": ["foo"],
@@ -910,15 +873,14 @@
     assert await decoded_r.json().objlen("non_existing_doc", "..a") is None
 
     # Test missing path
     # with pytest.raises(exceptions.ResponseError):
     await decoded_r.json().objlen("doc1", ".nowhere")
 
 
-@pytest.mark.redismod
 def load_types_data(nested_key_name):
     td = {
         "object": {},
         "array": [],
         "string": "str",
         "integer": 42,
         "number": 1.2,
@@ -930,15 +892,14 @@
     for i, (k, v) in zip(range(1, len(td) + 1), iter(td.items())):
         jdata["nested" + str(i)] = {nested_key_name: v}
         types.append(k)
 
     return jdata, types
 
 
-@pytest.mark.redismod
 async def test_type_dollar(decoded_r: redis.Redis):
     jdata, jtypes = load_types_data("a")
     await decoded_r.json().set("doc1", "$", jdata)
     # Test multi
     assert_resp_response(
         decoded_r, await decoded_r.json().type("doc1", "$..a"), jtypes, [jtypes]
     )
@@ -949,15 +910,14 @@
 
     # Test missing key
     assert_resp_response(
         decoded_r, await decoded_r.json().type("non_existing_doc", "..a"), None, [None]
     )
 
 
-@pytest.mark.redismod
 async def test_clear_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "nested1": {"a": {"foo": 10, "bar": 20}},
             "a": ["foo"],
@@ -1003,15 +963,14 @@
     )
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         await decoded_r.json().clear("non_existing_doc", "$..a")
 
 
-@pytest.mark.redismod
 async def test_toggle_dollar(decoded_r: redis.Redis):
     await decoded_r.json().set(
         "doc1",
         "$",
         {
             "a": ["foo"],
             "nested1": {"a": False},
```

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_lock.py` & `redis-5.1.0b4/tests/test_asyncio/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_monitor.py` & `redis-5.1.0b4/tests/test_asyncio/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_pipeline.py` & `redis-5.1.0b4/tests/test_asyncio/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_pubsub.py` & `redis-5.1.0b4/tests/test_asyncio/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_retry.py` & `redis-5.1.0b4/tests/test_asyncio/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_scripting.py` & `redis-5.1.0b4/tests/test_asyncio/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_search.py` & `redis-5.1.0b4/tests/test_asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_sentinel.py` & `redis-5.1.0b4/tests/test_asyncio/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.1.0b4/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/test_timeseries.py` & `redis-5.1.0b4/tests/test_asyncio/test_timeseries.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from tests.conftest import (
     assert_resp_response,
     is_resp2_connection,
     skip_ifmodversion_lt,
 )
 
 
-@pytest.mark.redismod
 async def test_create(decoded_r: redis.Redis):
     assert await decoded_r.ts().create(1)
     assert await decoded_r.ts().create(2, retention_msecs=5)
     assert await decoded_r.ts().create(3, labels={"Redis": "Labs"})
     assert await decoded_r.ts().create(4, retention_msecs=20, labels={"Time": "Series"})
     info = await decoded_r.ts().info(4)
     assert_resp_response(
@@ -24,15 +23,14 @@
 
     # Test for a chunk size of 128 Bytes
     assert await decoded_r.ts().create("time-serie-1", chunk_size=128)
     info = await decoded_r.ts().info("time-serie-1")
     assert_resp_response(decoded_r, 128, info.get("chunk_size"), info.get("chunkSize"))
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("1.4.0", "timeseries")
 async def test_create_duplicate_policy(decoded_r: redis.Redis):
     # Test for duplicate policy
     for duplicate_policy in ["block", "last", "first", "min", "max"]:
         ts_name = f"time-serie-ooo-{duplicate_policy}"
         assert await decoded_r.ts().create(ts_name, duplicate_policy=duplicate_policy)
         info = await decoded_r.ts().info(ts_name)
@@ -40,15 +38,14 @@
             decoded_r,
             duplicate_policy,
             info.get("duplicate_policy"),
             info.get("duplicatePolicy"),
         )
 
 
-@pytest.mark.redismod
 async def test_alter(decoded_r: redis.Redis):
     assert await decoded_r.ts().create(1)
     res = await decoded_r.ts().info(1)
     assert_resp_response(
         decoded_r, 0, res.get("retention_msecs"), res.get("retentionTime")
     )
     assert await decoded_r.ts().alter(1, retention_msecs=10)
@@ -63,30 +60,28 @@
     assert "Series" == (await decoded_r.ts().info(1))["labels"]["Time"]
     info = await decoded_r.ts().info(1)
     assert_resp_response(
         decoded_r, 10, info.get("retention_msecs"), info.get("retentionTime")
     )
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("1.4.0", "timeseries")
 async def test_alter_diplicate_policy(decoded_r: redis.Redis):
     assert await decoded_r.ts().create(1)
     info = await decoded_r.ts().info(1)
     assert_resp_response(
         decoded_r, None, info.get("duplicate_policy"), info.get("duplicatePolicy")
     )
     assert await decoded_r.ts().alter(1, duplicate_policy="min")
     info = await decoded_r.ts().info(1)
     assert_resp_response(
         decoded_r, "min", info.get("duplicate_policy"), info.get("duplicatePolicy")
     )
 
 
-@pytest.mark.redismod
 async def test_add(decoded_r: redis.Redis):
     assert 1 == await decoded_r.ts().add(1, 1, 1)
     assert 2 == await decoded_r.ts().add(2, 2, 3, retention_msecs=10)
     assert 3 == await decoded_r.ts().add(3, 3, 2, labels={"Redis": "Labs"})
     assert 4 == await decoded_r.ts().add(
         4, 4, 2, retention_msecs=10, labels={"Redis": "Labs", "Time": "Series"}
     )
@@ -101,15 +96,14 @@
 
     # Test for a chunk size of 128 Bytes on TS.ADD
     assert await decoded_r.ts().add("time-serie-1", 1, 10.0, chunk_size=128)
     info = await decoded_r.ts().info("time-serie-1")
     assert_resp_response(decoded_r, 128, info.get("chunk_size"), info.get("chunkSize"))
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("1.4.0", "timeseries")
 async def test_add_duplicate_policy(r: redis.Redis):
     # Test for duplicate policy BLOCK
     assert 1 == await r.ts().add("time-serie-add-ooo-block", 1, 5.0)
     with pytest.raises(Exception):
         await r.ts().add("time-serie-add-ooo-block", 1, 5.0, duplicate_policy="block")
 
@@ -142,23 +136,21 @@
     assert 1 == await r.ts().add(
         "time-serie-add-ooo-min", 1, 10.0, duplicate_policy="min"
     )
     res = await r.ts().get("time-serie-add-ooo-min")
     assert 5.0 == res[1]
 
 
-@pytest.mark.redismod
 async def test_madd(decoded_r: redis.Redis):
     await decoded_r.ts().create("a")
     assert [1, 2, 3] == await decoded_r.ts().madd(
         [("a", 1, 5), ("a", 2, 10), ("a", 3, 15)]
     )
 
 
-@pytest.mark.redismod
 async def test_incrby_decrby(decoded_r: redis.Redis):
     for _ in range(100):
         assert await decoded_r.ts().incrby(1, 1)
         sleep(0.001)
     assert 100 == (await decoded_r.ts().get(1))[1]
     for _ in range(100):
         assert await decoded_r.ts().decrby(1, 1)
@@ -179,15 +171,14 @@
 
     # Test for a chunk size of 128 Bytes on TS.DECRBY
     assert await decoded_r.ts().decrby("time-serie-2", 10, chunk_size=128)
     info = await decoded_r.ts().info("time-serie-2")
     assert_resp_response(decoded_r, 128, info.get("chunk_size"), info.get("chunkSize"))
 
 
-@pytest.mark.redismod
 async def test_create_and_delete_rule(decoded_r: redis.Redis):
     # test rule creation
     time = 100
     await decoded_r.ts().create(1)
     await decoded_r.ts().create(2)
     await decoded_r.ts().createrule(1, 2, "avg", 100)
     for i in range(50):
@@ -203,15 +194,14 @@
 
     # test rule deletion
     await decoded_r.ts().deleterule(1, 2)
     info = await decoded_r.ts().info(1)
     assert not info["rules"]
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "timeseries")
 async def test_del_range(decoded_r: redis.Redis):
     try:
         await decoded_r.ts().delete("test", 0, 100)
     except Exception as e:
         assert e.__str__() != ""
 
@@ -220,30 +210,28 @@
     assert 22 == await decoded_r.ts().delete(1, 0, 21)
     assert [] == await decoded_r.ts().range(1, 0, 21)
     assert_resp_response(
         decoded_r, await decoded_r.ts().range(1, 22, 22), [(22, 1.0)], [[22, 1.0]]
     )
 
 
-@pytest.mark.redismod
 async def test_range(r: redis.Redis):
     for i in range(100):
         await r.ts().add(1, i, i % 7)
     assert 100 == len(await r.ts().range(1, 0, 200))
     for i in range(100):
         await r.ts().add(1, i + 200, i % 7)
     assert 200 == len(await r.ts().range(1, 0, 500))
     # last sample isn't returned
     assert 20 == len(
         await r.ts().range(1, 0, 500, aggregation_type="avg", bucket_size_msec=10)
     )
     assert 10 == len(await r.ts().range(1, 0, 500, count=10))
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "timeseries")
 async def test_range_advanced(decoded_r: redis.Redis):
     for i in range(100):
         await decoded_r.ts().add(1, i, i % 7)
         await decoded_r.ts().add(1, i + 200, i % 7)
 
     assert 2 == len(
@@ -266,15 +254,14 @@
     assert_resp_response(decoded_r, res, [(0, 5.0), (5, 6.0)], [[0, 5.0], [5, 6.0]])
     res = await decoded_r.ts().range(
         1, 0, 10, aggregation_type="twa", bucket_size_msec=10
     )
     assert_resp_response(decoded_r, res, [(0, 2.55), (10, 3.0)], [[0, 2.55], [10, 3.0]])
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "timeseries")
 async def test_rev_range(decoded_r: redis.Redis):
     for i in range(100):
         await decoded_r.ts().add(1, i, i % 7)
     assert 100 == len(await decoded_r.ts().range(1, 0, 200))
     for i in range(100):
         await decoded_r.ts().add(1, i + 200, i % 7)
@@ -310,15 +297,14 @@
             1, 0, 10, aggregation_type="count", bucket_size_msec=10, align=1
         ),
         [(1, 10.0), (0, 1.0)],
         [[1, 10.0], [0, 1.0]],
     )
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_multi_range(decoded_r: redis.Redis):
     await decoded_r.ts().create(1, labels={"Test": "This", "team": "ny"})
     await decoded_r.ts().create(
         2, labels={"Test": "This", "Taste": "That", "team": "sf"}
     )
     for i in range(100):
@@ -365,15 +351,14 @@
         assert {} == res["1"][0]
         res = await decoded_r.ts().mrange(
             0, 200, filters=["Test=This"], with_labels=True
         )
         assert {"Test": "This", "team": "ny"} == res["1"][0]
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 @skip_ifmodversion_lt("99.99.99", "timeseries")
 async def test_multi_range_advanced(decoded_r: redis.Redis):
     await decoded_r.ts().create(1, labels={"Test": "This", "team": "ny"})
     await decoded_r.ts().create(
         2, labels={"Test": "This", "Taste": "That", "team": "sf"}
     )
@@ -483,15 +468,14 @@
             aggregation_type="count",
             bucket_size_msec=10,
             align=5,
         )
         assert [[0, 5.0], [5, 6.0]] == res["1"][2]
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 @skip_ifmodversion_lt("99.99.99", "timeseries")
 async def test_multi_reverse_range(decoded_r: redis.Redis):
     await decoded_r.ts().create(1, labels={"Test": "This", "team": "ny"})
     await decoded_r.ts().create(
         2, labels={"Test": "This", "Taste": "That", "team": "sf"}
     )
@@ -647,26 +631,24 @@
             aggregation_type="count",
             bucket_size_msec=10,
             align=1,
         )
         assert [[1, 10.0], [0, 1.0]] == res["1"][2]
 
 
-@pytest.mark.redismod
 async def test_get(decoded_r: redis.Redis):
     name = "test"
     await decoded_r.ts().create(name)
     assert not await decoded_r.ts().get(name)
     await decoded_r.ts().add(name, 2, 3)
     assert 2 == (await decoded_r.ts().get(name))[0]
     await decoded_r.ts().add(name, 3, 4)
     assert 4 == (await decoded_r.ts().get(name))[1]
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_mget(decoded_r: redis.Redis):
     await decoded_r.ts().create(1, labels={"Test": "This"})
     await decoded_r.ts().create(2, labels={"Test": "This", "Taste": "That"})
     act_res = await decoded_r.ts().mget(["Test=This"])
     exp_res = [{"1": [{}, None, None]}, {"2": [{}, None, None]}]
     exp_res_resp3 = {"1": [{}, []], "2": [{}, []]}
@@ -694,27 +676,25 @@
     res = await decoded_r.ts().mget(["Taste=That"], with_labels=True)
     if is_resp2_connection(decoded_r):
         assert {"Taste": "That", "Test": "This"} == res[0]["2"][0]
     else:
         assert {"Taste": "That", "Test": "This"} == res["2"][0]
 
 
-@pytest.mark.redismod
 async def test_info(decoded_r: redis.Redis):
     await decoded_r.ts().create(
         1, retention_msecs=5, labels={"currentLabel": "currentData"}
     )
     info = await decoded_r.ts().info(1)
     assert_resp_response(
         decoded_r, 5, info.get("retention_msecs"), info.get("retentionTime")
     )
     assert info["labels"]["currentLabel"] == "currentData"
 
 
-@pytest.mark.redismod
 @skip_ifmodversion_lt("1.4.0", "timeseries")
 async def testInfoDuplicatePolicy(decoded_r: redis.Redis):
     await decoded_r.ts().create(
         1, retention_msecs=5, labels={"currentLabel": "currentData"}
     )
     info = await decoded_r.ts().info(1)
     assert_resp_response(
@@ -724,41 +704,38 @@
     await decoded_r.ts().create("time-serie-2", duplicate_policy="min")
     info = await decoded_r.ts().info("time-serie-2")
     assert_resp_response(
         decoded_r, "min", info.get("duplicate_policy"), info.get("duplicatePolicy")
     )
 
 
-@pytest.mark.redismod
 @pytest.mark.onlynoncluster
 async def test_query_index(decoded_r: redis.Redis):
     await decoded_r.ts().create(1, labels={"Test": "This"})
     await decoded_r.ts().create(2, labels={"Test": "This", "Taste": "That"})
     assert 2 == len(await decoded_r.ts().queryindex(["Test=This"]))
     assert 1 == len(await decoded_r.ts().queryindex(["Taste=That"]))
     assert_resp_response(
         decoded_r, await decoded_r.ts().queryindex(["Taste=That"]), [2], {"2"}
     )
 
 
-# @pytest.mark.redismod
-# async def test_pipeline(r: redis.Redis):
+# # async def test_pipeline(r: redis.Redis):
 #     pipeline = await r.ts().pipeline()
 #     pipeline.create("with_pipeline")
 #     for i in range(100):
 #         pipeline.add("with_pipeline", i, 1.1 * i)
 #     pipeline.execute()
 
 #     info = await r.ts().info("with_pipeline")
 #     assert info.lastTimeStamp == 99
 #     assert info.total_samples == 100
 #     assert await r.ts().get("with_pipeline")[1] == 99 * 1.1
 
 
-@pytest.mark.redismod
 async def test_uncompressed(decoded_r: redis.Redis):
     await decoded_r.ts().create("compressed")
     await decoded_r.ts().create("uncompressed", uncompressed=True)
     compressed_info = await decoded_r.ts().info("compressed")
     uncompressed_info = await decoded_r.ts().info("uncompressed")
     if is_resp2_connection(decoded_r):
         assert compressed_info.memory_usage != uncompressed_info.memory_usage
```

### Comparing `redis-5.1.0b3/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.1.0b4/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/testdata/titles.csv` & `redis-5.1.0b4/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.1.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_bloom.py` & `redis-5.1.0b4/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_cache.py` & `redis-5.1.0b4/tests/test_cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -142,14 +142,57 @@
         assert r.lrange("mylist", 0, -1) == [b"baz", b"bar", b"foo"]
         res = cache.get(("LRANGE", "mylist", 0, -1))
         assert res == [b"baz", b"bar", b"foo"]
         res.append(b"new")
         check = cache.get(("LRANGE", "mylist", 0, -1))
         assert check == [b"baz", b"bar", b"foo"]
 
+    @pytest.mark.onlynoncluster
+    @pytest.mark.parametrize(
+        "r",
+        [{"cache": _LocalCache(), "kwargs": {"decode_responses": True}}],
+        indirect=True,
+    )
+    def test_csc_not_cause_disconnects(self, r):
+        r, cache = r
+        id1 = r.client_id()
+        r.mset({"a": 1, "b": 1, "c": 1, "d": 1, "e": 1, "f": 1})
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["1", "1", "1", "1", "1", "1"]
+        id2 = r.client_id()
+
+        # client should get value from client cache
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["1", "1", "1", "1", "1", "1"]
+        assert cache.get(("MGET", "a", "b", "c", "d", "e", "f")) == [
+            "1",
+            "1",
+            "1",
+            "1",
+            "1",
+            "1",
+        ]
+
+        r.mset({"a": 2, "b": 2, "c": 2, "d": 2, "e": 2, "f": 2})
+        id3 = r.client_id()
+        # client should get value from redis server post invalidate messages
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["2", "2", "2", "2", "2", "2"]
+
+        r.mset({"a": 3, "b": 3, "c": 3, "d": 3, "e": 3, "f": 3})
+        # need to check that we get correct value 3 and not 2
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["3", "3", "3", "3", "3", "3"]
+        # client should get value from client cache
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["3", "3", "3", "3", "3", "3"]
+
+        r.mset({"a": 4, "b": 4, "c": 4, "d": 4, "e": 4, "f": 4})
+        # need to check that we get correct value 4 and not 3
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["4", "4", "4", "4", "4", "4"]
+        # client should get value from client cache
+        assert r.mget("a", "b", "c", "d", "e", "f") == ["4", "4", "4", "4", "4", "4"]
+        id4 = r.client_id()
+        assert id1 == id2 == id3 == id4
+
 
 @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
 @pytest.mark.onlycluster
 class TestClusterLocalCache:
     @pytest.mark.parametrize("r", [{"cache": _LocalCache()}], indirect=True)
     def test_get_from_cache(self, r, r2):
         r, cache = r
```

### Comparing `redis-5.1.0b3/tests/test_cluster.py` & `redis-5.1.0b4/tests/test_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import threading
 import warnings
 from queue import LifoQueue, Queue
 from time import sleep
 from unittest.mock import DEFAULT, Mock, call, patch
 
 import pytest
+import redis
 from redis import Redis
 from redis._parsers import CommandsParser
 from redis.backoff import ExponentialBackoff, NoBackoff, default_backoff
 from redis.cluster import (
     PRIMARY,
     REDIS_CLUSTER_HASH_SLOTS,
     REPLICA,
@@ -3246,14 +3247,39 @@
             mock_node_resp_func(first_node, raise_ask_error)
             mock_node_resp(ask_node, "MOCK_OK")
             res = pipe.get(key).execute()
             assert first_node.redis_connection.connection.read_response.called
             assert ask_node.redis_connection.connection.read_response.called
             assert res == ["MOCK_OK"]
 
+    def test_return_previously_acquired_connections(self, r):
+        # in order to ensure that a pipeline will make use of connections
+        #   from different nodes
+        assert r.keyslot("a") != r.keyslot("b")
+
+        orig_func = redis.cluster.get_connection
+        with patch("redis.cluster.get_connection") as get_connection:
+
+            def raise_error(target_node, *args, **kwargs):
+                if get_connection.call_count == 2:
+                    raise ConnectionError("mocked error")
+                else:
+                    return orig_func(target_node, *args, **kwargs)
+
+            get_connection.side_effect = raise_error
+
+            r.pipeline().get("a").get("b").execute()
+
+        # 4 = 2 get_connections per execution * 2 executions
+        assert get_connection.call_count == 4
+        for cluster_node in r.nodes_manager.nodes_cache.values():
+            connection_pool = cluster_node.redis_connection.connection_pool
+            num_of_conns = len(connection_pool._available_connections)
+            assert num_of_conns == connection_pool._created_connections
+
     def test_empty_stack(self, r):
         """
         If pipeline is executed with no commands it should
         return a empty list.
         """
         p = r.pipeline()
         result = p.execute()
```

### Comparing `redis-5.1.0b3/tests/test_command_parser.py` & `redis-5.1.0b4/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_commands.py` & `redis-5.1.0b4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_connect.py` & `redis-5.1.0b4/tests/test_connect.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import socket
 import socketserver
 import ssl
 import threading
 
 import pytest
 from redis.connection import Connection, SSLConnection, UnixDomainSocketConnection
+from redis.exceptions import ConnectionError
 
 from .ssl_utils import get_ssl_filename
 
 _logger = logging.getLogger(__name__)
 
 
 _CLIENT_NAME = "test-suite-client"
@@ -41,55 +42,96 @@
 def test_uds_connect(uds_address):
     path = str(uds_address)
     conn = UnixDomainSocketConnection(path, client_name=_CLIENT_NAME, socket_timeout=10)
     _assert_connect(conn, path)
 
 
 @pytest.mark.ssl
-def test_tcp_ssl_connect(tcp_address):
+@pytest.mark.parametrize(
+    "ssl_min_version",
+    [
+        ssl.TLSVersion.TLSv1_2,
+        pytest.param(
+            ssl.TLSVersion.TLSv1_3,
+            marks=pytest.mark.skipif(not ssl.HAS_TLSv1_3, reason="requires TLSv1.3"),
+        ),
+    ],
+)
+def test_tcp_ssl_connect(tcp_address, ssl_min_version):
     host, port = tcp_address
     certfile = get_ssl_filename("server-cert.pem")
     keyfile = get_ssl_filename("server-key.pem")
     conn = SSLConnection(
         host=host,
         port=port,
         client_name=_CLIENT_NAME,
         ssl_ca_certs=certfile,
         socket_timeout=10,
+        ssl_min_version=ssl_min_version,
     )
     _assert_connect(conn, tcp_address, certfile=certfile, keyfile=keyfile)
 
 
-def _assert_connect(conn, server_address, certfile=None, keyfile=None):
+@pytest.mark.ssl
+@pytest.mark.skipif(not ssl.HAS_TLSv1_3, reason="requires TLSv1.3")
+def test_tcp_ssl_version_mismatch(tcp_address):
+    host, port = tcp_address
+    certfile = get_ssl_filename("server-cert.pem")
+    keyfile = get_ssl_filename("server-key.pem")
+    conn = SSLConnection(
+        host=host,
+        port=port,
+        client_name=_CLIENT_NAME,
+        ssl_ca_certs=certfile,
+        socket_timeout=10,
+        ssl_min_version=ssl.TLSVersion.TLSv1_3,
+    )
+    with pytest.raises(ConnectionError):
+        _assert_connect(
+            conn,
+            tcp_address,
+            certfile=certfile,
+            keyfile=keyfile,
+            ssl_version=ssl.PROTOCOL_TLSv1_2,
+        )
+
+
+def _assert_connect(conn, server_address, **tcp_kw):
     if isinstance(server_address, str):
         if not _RedisUDSServer:
             pytest.skip("Unix domain sockets are not supported on this platform")
         server = _RedisUDSServer(server_address, _RedisRequestHandler)
     else:
-        server = _RedisTCPServer(
-            server_address, _RedisRequestHandler, certfile=certfile, keyfile=keyfile
-        )
+        server = _RedisTCPServer(server_address, _RedisRequestHandler, **tcp_kw)
     with server as aserver:
         t = threading.Thread(target=aserver.serve_forever)
         t.start()
         try:
             aserver.wait_online()
             conn.connect()
             conn.disconnect()
         finally:
             aserver.stop()
             t.join(timeout=5)
 
 
 class _RedisTCPServer(socketserver.TCPServer):
-    def __init__(self, *args, certfile=None, keyfile=None, **kw) -> None:
+    def __init__(
+        self,
+        *args,
+        certfile=None,
+        keyfile=None,
+        ssl_version=ssl.PROTOCOL_TLS,
+        **kw,
+    ) -> None:
         self._ready_event = threading.Event()
         self._stop_requested = False
         self._certfile = certfile
         self._keyfile = keyfile
+        self._ssl_version = ssl_version
         super().__init__(*args, **kw)
 
     def service_actions(self):
         self._ready_event.set()
 
     def wait_online(self):
         self._ready_event.wait()
@@ -106,15 +148,15 @@
             return super().get_request()
         newsocket, fromaddr = self.socket.accept()
         connstream = ssl.wrap_socket(
             newsocket,
             server_side=True,
             certfile=self._certfile,
             keyfile=self._keyfile,
-            ssl_version=ssl.PROTOCOL_TLSv1_2,
+            ssl_version=self._ssl_version,
         )
         return connstream, fromaddr
 
 
 if hasattr(socketserver, "UnixStreamServer"):
 
     class _RedisUDSServer(socketserver.UnixStreamServer):
```

### Comparing `redis-5.1.0b3/tests/test_connection.py` & `redis-5.1.0b4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_connection_pool.py` & `redis-5.1.0b4/tests/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_credentials.py` & `redis-5.1.0b4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_encoding.py` & `redis-5.1.0b4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_function.py` & `redis-5.1.0b4/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_graph.py` & `redis-5.1.0b4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_graph_utils/test_edge.py` & `redis-5.1.0b4/tests/test_graph_utils/test_edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_graph_utils/test_node.py` & `redis-5.1.0b4/tests/test_graph_utils/test_node.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_graph_utils/test_path.py` & `redis-5.1.0b4/tests/test_graph_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_helpers.py` & `redis-5.1.0b4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_json.py` & `redis-5.1.0b4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_lock.py` & `redis-5.1.0b4/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_monitor.py` & `redis-5.1.0b4/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_multiprocessing.py` & `redis-5.1.0b4/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_pipeline.py` & `redis-5.1.0b4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_pubsub.py` & `redis-5.1.0b4/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_retry.py` & `redis-5.1.0b4/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_scripting.py` & `redis-5.1.0b4/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_search.py` & `redis-5.1.0b4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_sentinel.py` & `redis-5.1.0b4/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/test_ssl.py` & `redis-5.1.0b4/tests/test_ssl.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,44 +22,48 @@
     SERVER_KEY = get_ssl_filename("server-key.pem")
 
     def test_ssl_with_invalid_cert(self, request):
         ssl_url = request.config.option.redis_ssl_url
         sslclient = redis.from_url(ssl_url)
         with pytest.raises(ConnectionError) as e:
             sslclient.ping()
-            assert "SSL: CERTIFICATE_VERIFY_FAILED" in str(e)
+        assert "SSL: CERTIFICATE_VERIFY_FAILED" in str(e)
+        sslclient.close()
 
     def test_ssl_connection(self, request):
         ssl_url = request.config.option.redis_ssl_url
         p = urlparse(ssl_url)[1].split(":")
         r = redis.Redis(host=p[0], port=p[1], ssl=True, ssl_cert_reqs="none")
         assert r.ping()
+        r.close()
 
     def test_ssl_connection_without_ssl(self, request):
         ssl_url = request.config.option.redis_ssl_url
         p = urlparse(ssl_url)[1].split(":")
         r = redis.Redis(host=p[0], port=p[1], ssl=False)
 
         with pytest.raises(ConnectionError) as e:
             r.ping()
-            assert "Connection closed by server" in str(e)
+        assert "Connection closed by server" in str(e)
+        r.close()
 
     def test_validating_self_signed_certificate(self, request):
         ssl_url = request.config.option.redis_ssl_url
         p = urlparse(ssl_url)[1].split(":")
         r = redis.Redis(
             host=p[0],
             port=p[1],
             ssl=True,
             ssl_certfile=self.SERVER_CERT,
             ssl_keyfile=self.SERVER_KEY,
             ssl_cert_reqs="required",
             ssl_ca_certs=self.SERVER_CERT,
         )
         assert r.ping()
+        r.close()
 
     def test_validating_self_signed_string_certificate(self, request):
         with open(self.SERVER_CERT) as f:
             cert_data = f.read()
         ssl_url = request.config.option.redis_ssl_url
         p = urlparse(ssl_url)[1].split(":")
         r = redis.Redis(
@@ -68,14 +72,15 @@
             ssl=True,
             ssl_certfile=self.SERVER_CERT,
             ssl_keyfile=self.SERVER_KEY,
             ssl_cert_reqs="required",
             ssl_ca_data=cert_data,
         )
         assert r.ping()
+        r.close()
 
     def _create_oscp_conn(self, request):
         ssl_url = request.config.option.redis_ssl_url
         p = urlparse(ssl_url)[1].split(":")
         r = redis.Redis(
             host=p[0],
             port=p[1],
@@ -88,30 +93,33 @@
         )
         return r
 
     @skip_if_cryptography()
     def test_ssl_ocsp_called(self, request):
         r = self._create_oscp_conn(request)
         with pytest.raises(RedisError) as e:
-            assert r.ping()
-            assert "cryptography not installed" in str(e)
+            r.ping()
+        assert "cryptography is not installed" in str(e)
+        r.close()
 
     @skip_if_nocryptography()
     def test_ssl_ocsp_called_withcrypto(self, request):
         r = self._create_oscp_conn(request)
         with pytest.raises(ConnectionError) as e:
             assert r.ping()
-            assert "No AIA information present in ssl certificate" in str(e)
+        assert "No AIA information present in ssl certificate" in str(e)
+        r.close()
 
         # rediss://, url based
         ssl_url = request.config.option.redis_ssl_url
         sslclient = redis.from_url(ssl_url)
         with pytest.raises(ConnectionError) as e:
             sslclient.ping()
-            assert "No AIA information present in ssl certificate" in str(e)
+        assert "No AIA information present in ssl certificate" in str(e)
+        sslclient.close()
 
     @skip_if_nocryptography()
     def test_valid_ocsp_cert_http(self):
         from redis.ocsp import OCSPVerifier
 
         hostnames = ["github.com", "aws.amazon.com", "ynet.co.il"]
         for hostname in hostnames:
@@ -128,15 +136,15 @@
         context = ssl.create_default_context()
         hostname = "revoked.badssl.com"
         with socket.create_connection((hostname, 443)) as sock:
             with context.wrap_socket(sock, server_hostname=hostname) as wrapped:
                 ocsp = OCSPVerifier(wrapped, hostname, 443)
                 with pytest.raises(ConnectionError) as e:
                     assert ocsp.is_valid()
-                    assert "REVOKED" in str(e)
+                assert "REVOKED" in str(e)
 
     @skip_if_nocryptography()
     def test_unauthorized_ocsp(self):
         from redis.ocsp import OCSPVerifier
 
         context = ssl.create_default_context()
         hostname = "stackoverflow.com"
@@ -153,15 +161,15 @@
         context = ssl.create_default_context()
         hostname = "google.co.il"
         with socket.create_connection((hostname, 443)) as sock:
             with context.wrap_socket(sock, server_hostname=hostname) as wrapped:
                 ocsp = OCSPVerifier(wrapped, hostname, 443)
                 with pytest.raises(ConnectionError) as e:
                     assert ocsp.is_valid()
-                    assert "from the" in str(e)
+                assert "from the" in str(e)
 
     @skip_if_nocryptography()
     def test_unauthorized_then_direct(self):
         from redis.ocsp import OCSPVerifier
 
         # these certificates on the socket end return unauthorized
         # then the second call succeeds
@@ -189,14 +197,15 @@
             ssl_ca_certs=self.SERVER_CERT,
             ssl_validate_ocsp=True,
             ssl_ocsp_context=p,  # just needs to not be none
         )
 
         with pytest.raises(RedisError):
             r.ping()
+        r.close()
 
         ctx = OpenSSL.SSL.Context(OpenSSL.SSL.SSLv23_METHOD)
         ctx.use_certificate_file(self.SERVER_CERT)
         ctx.use_privatekey_file(self.SERVER_KEY)
 
         r = redis.Redis(
             host=p[0],
@@ -209,23 +218,25 @@
             ssl_ocsp_context=ctx,
             ssl_ocsp_expected_cert=open(self.SERVER_KEY, "rb").read(),
             ssl_validate_ocsp_stapled=True,
         )
 
         with pytest.raises(ConnectionError) as e:
             r.ping()
-            assert "no ocsp response present" in str(e)
+        assert "no ocsp response present" in str(e)
+        r.close()
 
         r = redis.Redis(
             host=p[0],
             port=p[1],
             ssl=True,
             ssl_certfile=self.SERVER_CERT,
             ssl_keyfile=self.SERVER_KEY,
             ssl_cert_reqs="required",
             ssl_ca_certs=self.SERVER_CERT,
             ssl_validate_ocsp_stapled=True,
         )
 
         with pytest.raises(ConnectionError) as e:
             r.ping()
-            assert "no ocsp response present" in str(e)
+        assert "no ocsp response present" in str(e)
+        r.close()
```

### Comparing `redis-5.1.0b3/tests/test_timeseries.py` & `redis-5.1.0b4/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/testdata/jsontestdata.py` & `redis-5.1.0b4/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/testdata/titles.csv` & `redis-5.1.0b4/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.1.0b3/tests/testdata/will_play_text.csv.bz2` & `redis-5.1.0b4/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

