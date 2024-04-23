# Comparing `tmp/sentry-sdk-2.0.0rc4.tar.gz` & `tmp/sentry-sdk-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-sdk-2.0.0rc4.tar", last modified: Wed Apr  3 08:02:44 2024, max compression
+gzip compressed data, was "sentry-sdk-2.0.0rc5.tar", last modified: Wed Apr 10 14:23:05 2024, max compression
```

## Comparing `sentry-sdk-2.0.0rc4.tar` & `sentry-sdk-2.0.0rc5.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.946354 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.946354 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23345 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33304 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    38456 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20392 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56248 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.954354 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.954354 sentry-sdk-2.0.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31256 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.493917 sentry-sdk-2.0.0rc5/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38456 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.513918 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.513918 sentry-sdk-2.0.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_utils.py
```

### Comparing `sentry-sdk-2.0.0rc4/LICENSE` & `sentry-sdk-2.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/PKG-INFO` & `sentry-sdk-2.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc4/README.md` & `sentry-sdk-2.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/_compat.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/_lru_cache.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/_queue.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/_types.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         "crash",
         "transaction",
         "security",
         "attachment",
         "session",
         "internal",
         "profile",
-        "statsd",
+        "metric_bucket",
         "monitor",
     ]
     SessionStatus = Literal["ok", "exited", "crashed", "abnormal"]
 
     DurationUnit = Literal[
         "nanosecond",
         "microsecond",
@@ -173,7 +173,41 @@
     MetricTags = Mapping[str, MetricTagValue]
 
     # Value inside the generator for the metric value.
     FlushedMetricValue = Union[int, float]
 
     BucketKey = Tuple[MetricType, str, MeasurementUnit, MetricTagsInternal]
     MetricMetaKey = Tuple[MetricType, str, MeasurementUnit]
+
+    MonitorConfigScheduleType = Literal["crontab", "interval"]
+    MonitorConfigScheduleUnit = Literal[
+        "year",
+        "month",
+        "week",
+        "day",
+        "hour",
+        "minute",
+        "second",  # not supported in Sentry and will result in a warning
+    ]
+
+    MonitorConfigSchedule = TypedDict(
+        "MonitorConfigSchedule",
+        {
+            "type": MonitorConfigScheduleType,
+            "value": Union[int, str],
+            "unit": MonitorConfigScheduleUnit,
+        },
+        total=False,
+    )
+
+    MonitorConfig = TypedDict(
+        "MonitorConfig",
+        {
+            "schedule": MonitorConfigSchedule,
+            "timezone": str,
+            "checkin_margin": int,
+            "max_runtime": int,
+            "failure_issue_threshold": int,
+            "recovery_threshold": int,
+        },
+        total=False,
+    )
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/_werkzeug.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/api.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/attachments.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/client.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/consts.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,20 @@
     from sentry_sdk.integrations import Integration
 
     from sentry_sdk._types import (
         BreadcrumbProcessor,
         Event,
         EventProcessor,
         Hint,
+        MeasurementUnit,
         ProfilerMode,
         TracesSampler,
         TransactionProcessor,
         MetricTags,
+        MetricValue,
     )
 
     # Experiments are feature flags to enable and disable certain unstable SDK
     # functionality. Changing them from the defaults (`None`) in production
     # code is highly discouraged. They are not subject to any stability
     # guarantees such as the ones from semantic versioning.
     Experiments = TypedDict(
@@ -53,17 +55,17 @@
             "attach_explain_plans": dict[str, Any],
             "max_spans": Optional[int],
             "record_sql_params": Optional[bool],
             "otel_powered_performance": Optional[bool],
             "transport_zlib_compression_level": Optional[int],
             "transport_num_pools": Optional[int],
             "enable_metrics": Optional[bool],
-            "metrics_summary_sample_rate": Optional[float],
-            "should_summarize_metric": Optional[Callable[[str, MetricTags], bool]],
-            "before_emit_metric": Optional[Callable[[str, MetricTags], bool]],
+            "before_emit_metric": Optional[
+                Callable[[str, MetricValue, MeasurementUnit, MetricTags], bool]
+            ],
             "metric_code_locations": Optional[bool],
         },
         total=False,
     )
 
 DEFAULT_QUEUE_SIZE = 100
 DEFAULT_MAX_BREADCRUMBS = 100
@@ -339,8 +341,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.0.0rc4"
+VERSION = "2.0.0rc5"
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/crons/api.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/crons/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import uuid
 
 import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
-    from typing import Any, Dict, Optional
-    from sentry_sdk._types import Event
+    from typing import Optional
+    from sentry_sdk._types import Event, MonitorConfig
 
 
 def _create_check_in_event(
-    monitor_slug=None,
-    check_in_id=None,
-    status=None,
-    duration_s=None,
-    monitor_config=None,
+    monitor_slug=None,  # type: Optional[str]
+    check_in_id=None,  # type: Optional[str]
+    status=None,  # type: Optional[str]
+    duration_s=None,  # type: Optional[float]
+    monitor_config=None,  # type: Optional[MonitorConfig]
 ):
-    # type: (Optional[str], Optional[str], Optional[str], Optional[float], Optional[Dict[str, Any]]) -> Event
+    # type: (...) -> Event
     options = sentry_sdk.get_client().options
     check_in_id = check_in_id or uuid.uuid4().hex  # type: str
 
     check_in = {
         "type": "check_in",
         "monitor_slug": monitor_slug,
         "check_in_id": check_in_id,
@@ -33,21 +33,21 @@
     if monitor_config:
         check_in["monitor_config"] = monitor_config
 
     return check_in
 
 
 def capture_checkin(
-    monitor_slug=None,
-    check_in_id=None,
-    status=None,
-    duration=None,
-    monitor_config=None,
+    monitor_slug=None,  # type: Optional[str]
+    check_in_id=None,  # type: Optional[str]
+    status=None,  # type: Optional[str]
+    duration=None,  # type: Optional[float]
+    monitor_config=None,  # type: Optional[MonitorConfig]
 ):
-    # type: (Optional[str], Optional[str], Optional[str], Optional[float], Optional[Dict[str, Any]]) -> str
+    # type: (...) -> str
     check_in_event = _create_check_in_event(
         monitor_slug=monitor_slug,
         check_in_id=check_in_id,
         status=status,
         duration_s=duration,
         monitor_config=monitor_config,
     )
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/crons/decorator.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/crons/decorator.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.crons import capture_checkin
 from sentry_sdk.crons.consts import MonitorStatus
 from sentry_sdk.utils import now
 
 if TYPE_CHECKING:
+    from collections.abc import Awaitable, Callable
     from types import TracebackType
     from typing import (
         Any,
-        Awaitable,
-        Callable,
         Optional,
         ParamSpec,
         Type,
         TypeVar,
         Union,
+        cast,
+        overload,
     )
+    from sentry_sdk._types import MonitorConfig
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
 
 class monitor:  # noqa: N801
     """
@@ -49,15 +51,15 @@
     def test(arg):
         with sentry_sdk.monitor(monitor_slug='my-fancy-slug'):
             print(arg)
     ```
     """
 
     def __init__(self, monitor_slug=None, monitor_config=None):
-        # type: (Optional[str], Optional[dict[str, Any]]) -> None
+        # type: (Optional[str], Optional[MonitorConfig]) -> None
         self.monitor_slug = monitor_slug
         self.monitor_config = monitor_config
 
     def __enter__(self):
         # type: () -> None
         self.start_timestamp = now()
         self.check_in_id = capture_checkin(
@@ -79,26 +81,54 @@
             monitor_slug=self.monitor_slug,
             check_in_id=self.check_in_id,
             status=status,
             duration=duration_s,
             monitor_config=self.monitor_config,
         )
 
-    def __call__(self, fn):
-        # type: (Callable[P, R]) -> Callable[P, Union[R, Awaitable[R]]]
-        if iscoroutinefunction(fn):
+    if TYPE_CHECKING:
 
-            @wraps(fn)
-            async def inner(*args: "P.args", **kwargs: "P.kwargs"):
-                # type: (...) -> R
-                with self:
-                    return await fn(*args, **kwargs)
+        @overload
+        def __call__(self, fn):
+            # type: (Callable[P, Awaitable[Any]]) -> Callable[P, Awaitable[Any]]
+            # Unfortunately, mypy does not give us any reliable way to type check the
+            # return value of an Awaitable (i.e. async function) for this overload,
+            # since calling iscouroutinefunction narrows the type to Callable[P, Awaitable[Any]].
+            ...
+
+        @overload
+        def __call__(self, fn):
+            # type: (Callable[P, R]) -> Callable[P, R]
+            ...
+
+    def __call__(
+        self,
+        fn,  # type: Union[Callable[P, R], Callable[P, Awaitable[Any]]]
+    ):
+        # type: (...) -> Union[Callable[P, R], Callable[P, Awaitable[Any]]]
+        if iscoroutinefunction(fn):
+            return self._async_wrapper(fn)
 
         else:
+            if TYPE_CHECKING:
+                fn = cast("Callable[P, R]", fn)
+            return self._sync_wrapper(fn)
+
+    def _async_wrapper(self, fn):
+        # type: (Callable[P, Awaitable[Any]]) -> Callable[P, Awaitable[Any]]
+        @wraps(fn)
+        async def inner(*args: "P.args", **kwargs: "P.kwargs"):
+            # type: (...) -> R
+            with self:
+                return await fn(*args, **kwargs)
+
+        return inner
 
-            @wraps(fn)
-            def inner(*args: "P.args", **kwargs: "P.kwargs"):
-                # type: (...) -> R
-                with self:
-                    return fn(*args, **kwargs)
+    def _sync_wrapper(self, fn):
+        # type: (Callable[P, R]) -> Callable[P, R]
+        @wraps(fn)
+        def inner(*args: "P.args", **kwargs: "P.kwargs"):
+            # type: (...) -> R
+            with self:
+                return fn(*args, **kwargs)
 
         return inner
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/django.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/debug.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/envelope.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/envelope.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         elif ty == "event":
             return "error"
         elif ty == "client_report":
             return "internal"
         elif ty == "profile":
             return "profile"
         elif ty == "statsd":
-            return "statsd"
+            return "metric_bucket"
         elif ty == "check_in":
             return "monitor"
         else:
             return "default"
 
     def get_bytes(self):
         # type: (...) -> bytes
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/hub.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_asgi_common.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_wsgi_common.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aiohttp.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/argv.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/ariadne.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/arq.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asgi.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncio.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncpg.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/atexit.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aws_lambda.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/beam.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/boto3.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/bottle.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/beat.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/beat.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     logger,
     match_regex_list,
 )
 
 if TYPE_CHECKING:
-    from typing import Any
-    from typing import Callable
-    from typing import Dict
-    from typing import Optional
-    from typing import TypeVar
-    from typing import Union
+    from collections.abc import Callable
+    from typing import Any, Optional, TypeVar, Union
+    from sentry_sdk._types import (
+        MonitorConfig,
+        MonitorConfigScheduleType,
+        MonitorConfigScheduleUnit,
+    )
 
     F = TypeVar("F", bound=Callable[..., Any])
 
 
 try:
     from celery import Task, Celery  # type: ignore
     from celery.beat import Scheduler  # type: ignore
@@ -38,33 +39,33 @@
 try:
     from redbeat.schedulers import RedBeatScheduler  # type: ignore
 except ImportError:
     RedBeatScheduler = None
 
 
 def _get_headers(task):
-    # type: (Task) -> Dict[str, Any]
+    # type: (Task) -> dict[str, Any]
     headers = task.request.get("headers") or {}
 
     # flatten nested headers
     if "headers" in headers:
         headers.update(headers["headers"])
         del headers["headers"]
 
     headers.update(task.request.get("properties") or {})
 
     return headers
 
 
 def _get_monitor_config(celery_schedule, app, monitor_name):
-    # type: (Any, Celery, str) -> Dict[str, Any]
-    monitor_config = {}  # type: Dict[str, Any]
-    schedule_type = None  # type: Optional[str]
+    # type: (Any, Celery, str) -> MonitorConfig
+    monitor_config = {}  # type: MonitorConfig
+    schedule_type = None  # type: Optional[MonitorConfigScheduleType]
     schedule_value = None  # type: Optional[Union[str, int]]
-    schedule_unit = None  # type: Optional[str]
+    schedule_unit = None  # type: Optional[MonitorConfigScheduleUnit]
 
     if isinstance(celery_schedule, crontab):
         schedule_type = "crontab"
         schedule_value = (
             "{0._orig_minute} "
             "{0._orig_hour} "
             "{0._orig_day_of_month} "
@@ -238,15 +239,15 @@
     # type: () -> None
     task_success.connect(crons_task_success)
     task_failure.connect(crons_task_failure)
     task_retry.connect(crons_task_retry)
 
 
 def crons_task_success(sender, **kwargs):
-    # type: (Task, Dict[Any, Any]) -> None
+    # type: (Task, dict[Any, Any]) -> None
     logger.debug("celery_task_success %s", sender)
     headers = _get_headers(sender)
 
     if "sentry-monitor-slug" not in headers:
         return
 
     monitor_config = headers.get("sentry-monitor-config", {})
@@ -259,15 +260,15 @@
         check_in_id=headers["sentry-monitor-check-in-id"],
         duration=_now_seconds_since_epoch() - start_timestamp_s,
         status=MonitorStatus.OK,
     )
 
 
 def crons_task_failure(sender, **kwargs):
-    # type: (Task, Dict[Any, Any]) -> None
+    # type: (Task, dict[Any, Any]) -> None
     logger.debug("celery_task_failure %s", sender)
     headers = _get_headers(sender)
 
     if "sentry-monitor-slug" not in headers:
         return
 
     monitor_config = headers.get("sentry-monitor-config", {})
@@ -280,15 +281,15 @@
         check_in_id=headers["sentry-monitor-check-in-id"],
         duration=_now_seconds_since_epoch() - start_timestamp_s,
         status=MonitorStatus.ERROR,
     )
 
 
 def crons_task_retry(sender, **kwargs):
-    # type: (Task, Dict[Any, Any]) -> None
+    # type: (Task, dict[Any, Any]) -> None
     logger.debug("celery_task_retry %s", sender)
     headers = _get_headers(sender)
 
     if "sentry-monitor-slug" not in headers:
         return
 
     monitor_config = headers.get("sentry-monitor-config", {})
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/utils.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import time
+from typing import cast
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Any
-    from typing import Tuple
+    from typing import Any, Tuple
+    from sentry_sdk._types import MonitorConfigScheduleUnit
 
 
 def _now_seconds_since_epoch():
     # type: () -> float
     # We cannot use `time.perf_counter()` when dealing with the duration
     # of a Celery task, because the start of a Celery task and
     # the end are recorded in different processes.
     # Start happens in the Celery Beat process,
     # the end in a Celery Worker process.
     return time.time()
 
 
 def _get_humanized_interval(seconds):
-    # type: (float) -> Tuple[int, str]
+    # type: (float) -> Tuple[int, MonitorConfigScheduleUnit]
     TIME_UNITS = (  # noqa: N806
         ("day", 60 * 60 * 24.0),
         ("hour", 60 * 60.0),
         ("minute", 60.0),
     )
 
     seconds = float(seconds)
     for unit, divider in TIME_UNITS:
         if seconds >= divider:
             interval = int(seconds / divider)
-            return (interval, unit)
+            return (interval, cast("MonitorConfigScheduleUnit", unit))
 
     return (int(seconds), "second")
 
 
 class NoOpMgr:
     def __enter__(self):
         # type: () -> None
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/chalice.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/clickhouse_driver.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/cloud_resource_context.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/dedupe.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,32 +106,35 @@
 class DjangoIntegration(Integration):
     identifier = "django"
 
     transaction_style = ""
     middleware_spans = None
     signals_spans = None
     cache_spans = None
+    signals_denylist = []  # type: list[signals.Signal]
 
     def __init__(
         self,
         transaction_style="url",
         middleware_spans=True,
         signals_spans=True,
         cache_spans=False,
+        signals_denylist=None,
     ):
-        # type: (str, bool, bool, bool) -> None
+        # type: (str, bool, bool, bool, Optional[list[signals.Signal]]) -> None
         if transaction_style not in TRANSACTION_STYLE_VALUES:
             raise ValueError(
                 "Invalid value for transaction_style: %s (must be in %s)"
                 % (transaction_style, TRANSACTION_STYLE_VALUES)
             )
         self.transaction_style = transaction_style
         self.middleware_spans = middleware_spans
         self.signals_spans = signals_spans
         self.cache_spans = cache_spans
+        self.signals_denylist = signals_denylist or []
 
     @staticmethod
     def setup_once():
         # type: () -> None
 
         if DJANGO_VERSION < (1, 8):
             raise DidNotEnable("Django 1.8 or newer is required.")
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/asgi.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/caching.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/middleware.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/signals_handlers.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,19 @@
                 ) as span:
                     span.set_data("signal", signal_name)
                     return receiver(*args, **kwargs)
 
             return wrapper
 
         integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
-        if integration and integration.signals_spans:
+        if (
+            integration
+            and integration.signals_spans
+            and self not in integration.signals_denylist
+        ):
             for idx, receiver in enumerate(sync_receivers):
                 sync_receivers[idx] = sentry_sync_receiver_wrapper(receiver)
 
         if DJANGO_VERSION >= (5, 0):
             return sync_receivers, async_receivers
         else:
             return sync_receivers
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/templates.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/transactions.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/views.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/excepthook.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/executing.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/falcon.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/fastapi.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/flask.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gcp.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gnu_backtrace.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gql.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/graphene.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/client.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/server.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/client.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/server.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/httpx.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/huey.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/logging.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/loguru.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/modules.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/openai.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pure_eval.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pymongo.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pyramid.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/quart.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/__init__.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/asyncio.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/rq.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sanic.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sanic.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,18 @@
     # type: (Union[Tuple[Optional[type], Optional[BaseException], Any], BaseException]) -> None
     with capture_internal_exceptions():
         event, hint = event_from_exception(
             exception,
             client_options=sentry_sdk.get_client().options,
             mechanism={"type": "sanic", "handled": False},
         )
+
+        if hint and hasattr(hint["exc_info"][0], "quiet") and hint["exc_info"][0].quiet:
+            return
+
         sentry_sdk.capture_event(event, hint=hint)
 
 
 def _make_request_processor(weak_request):
     # type: (Callable[[], Request]) -> EventProcessor
     def sanic_processor(event, hint):
         # type: (Event, Optional[Hint]) -> Optional[Event]
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/serverless.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/socket.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_driver.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_worker.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sqlalchemy.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlette.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlite.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/stdlib.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/strawberry.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/strawberry.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,17 @@
     def on_operation(self):
         # type: () -> Generator[None, None, None]
         self._operation_name = self.execution_context.operation_name
 
         operation_type = "query"
         op = OP.GRAPHQL_QUERY
 
+        if self.execution_context.query is None:
+            self.execution_context.query = ""
+
         if self.execution_context.query.strip().startswith("mutation"):
             operation_type = "mutation"
             op = OP.GRAPHQL_MUTATION
         elif self.execution_context.query.strip().startswith("subscription"):
             operation_type = "subscription"
             op = OP.GRAPHQL_SUBSCRIPTION
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/threading.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/tornado.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/trytond.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/wsgi.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/metrics.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,27 +50,44 @@
     from sentry_sdk._types import MetricTags
     from sentry_sdk._types import MetricTagsInternal
     from sentry_sdk._types import MetricType
     from sentry_sdk._types import MetricValue
 
 
 _in_metrics = ContextVar("in_metrics", default=False)
-_sanitize_key = partial(re.compile(r"[^a-zA-Z0-9_/.-]+").sub, "_")
-_sanitize_value = partial(re.compile(r"[^\w\d\s_:/@\.{}\[\]$-]+", re.UNICODE).sub, "")
 _set = set  # set is shadowed below
 
 GOOD_TRANSACTION_SOURCES = frozenset(
     [
         TRANSACTION_SOURCE_ROUTE,
         TRANSACTION_SOURCE_VIEW,
         TRANSACTION_SOURCE_COMPONENT,
         TRANSACTION_SOURCE_TASK,
     ]
 )
 
+_sanitize_unit = partial(re.compile(r"[^a-zA-Z0-9_]+").sub, "")
+_sanitize_metric_key = partial(re.compile(r"[^a-zA-Z0-9_\-.]+").sub, "_")
+_sanitize_tag_key = partial(re.compile(r"[^a-zA-Z0-9_\-.\/]+").sub, "")
+
+
+def _sanitize_tag_value(value):
+    # type: (str) -> str
+    table = str.maketrans(
+        {
+            "\n": "\\n",
+            "\r": "\\r",
+            "\t": "\\t",
+            "\\": "\\\\",
+            "|": "\\u{7c}",
+            ",": "\\u{2c}",
+        }
+    )
+    return value.translate(table)
+
 
 def get_code_location(stacklevel):
     # type: (int) -> Optional[Dict[str, Any]]
     try:
         frm = sys._getframe(stacklevel)
     except Exception:
         return None
@@ -271,15 +288,16 @@
     # and not during aggregation for performance reasons.  This means that the
     # envelope can in fact have duplicate buckets stored.  This is acceptable for
     # relay side emission and should not happen commonly.
 
     for timestamp, buckets in flushable_buckets:
         for bucket_key, metric in buckets.items():
             metric_type, metric_name, metric_unit, metric_tags = bucket_key
-            metric_name = _sanitize_key(metric_name)
+            metric_name = _sanitize_metric_key(metric_name)
+            metric_unit = _sanitize_unit(metric_unit)
             _write(metric_name.encode("utf-8"))
             _write(b"@")
             _write(metric_unit.encode("utf-8"))
 
             for serialized_value in metric.serialize_value():
                 _write(b":")
                 _write(str(serialized_value).encode("utf-8"))
@@ -287,39 +305,41 @@
             _write(b"|")
             _write(metric_type.encode("ascii"))
 
             if metric_tags:
                 _write(b"|#")
                 first = True
                 for tag_key, tag_value in metric_tags:
-                    tag_key = _sanitize_key(tag_key)
+                    tag_key = _sanitize_tag_key(tag_key)
                     if not tag_key:
                         continue
                     if first:
                         first = False
                     else:
                         _write(b",")
                     _write(tag_key.encode("utf-8"))
                     _write(b":")
-                    _write(_sanitize_value(tag_value).encode("utf-8"))
+                    _write(_sanitize_tag_value(tag_value).encode("utf-8"))
 
             _write(b"|T")
             _write(str(timestamp).encode("ascii"))
             _write(b"\n")
 
     return out.getvalue()
 
 
 def _encode_locations(timestamp, code_locations):
     # type: (int, Iterable[Tuple[MetricMetaKey, Dict[str, Any]]]) -> bytes
     mapping = {}  # type: Dict[str, List[Any]]
 
     for key, loc in code_locations:
         metric_type, name, unit = key
-        mri = "{}:{}@{}".format(metric_type, _sanitize_key(name), unit)
+        mri = "{}:{}@{}".format(
+            metric_type, _sanitize_metric_key(name), _sanitize_unit(unit)
+        )
 
         loc["type"] = "location"
         mapping.setdefault(mri, []).append(loc)
 
     return json_dumps({"timestamp": timestamp, "mapping": mapping})
 
 
@@ -559,14 +579,16 @@
 
             if stacklevel is not None:
                 self.record_code_location(ty, key, unit, stacklevel + 2, timestamp)
 
         # Given the new weight we consider whether we want to force flush.
         self._consider_force_flush()
 
+        # For sets, we only record that a value has been added to the set but not which one.
+        # See develop docs: https://develop.sentry.dev/sdk/metrics/#sets
         if local_aggregator is not None:
             local_value = float(added if ty == "s" else value)
             local_aggregator.add(ty, key, local_value, unit, serialized_tags)
 
     def record_code_location(
         self,
         ty,  # type: MetricType
@@ -703,23 +725,21 @@
     return (
         client.metrics_aggregator
         if client is not None and client.metrics_aggregator is not None
         else None
     )
 
 
-def _get_aggregator_and_update_tags(key, tags):
-    # type: (str, Optional[MetricTags]) -> Tuple[Optional[MetricsAggregator], Optional[LocalAggregator], Optional[MetricTags]]
+def _get_aggregator_and_update_tags(key, value, unit, tags):
+    # type: (str, Optional[MetricValue], MeasurementUnit, Optional[MetricTags]) -> Tuple[Optional[MetricsAggregator], Optional[LocalAggregator], Optional[MetricTags]]
     hub = sentry_sdk.Hub.current
     client = hub.client
     if client is None or client.metrics_aggregator is None:
         return None, None, tags
 
-    experiments = client.options.get("_experiments", {})
-
     updated_tags = dict(tags or ())  # type: Dict[str, MetricTagValue]
     updated_tags.setdefault("release", client.options["release"])
     updated_tags.setdefault("environment", client.options["environment"])
 
     scope = sentry_sdk.Scope.get_current_scope()
     local_aggregator = None
 
@@ -727,55 +747,50 @@
     # this one is the same between just errors and errors + performance
     transaction_source = scope._transaction_info.get("source")
     if transaction_source in GOOD_TRANSACTION_SOURCES:
         transaction_name = scope._transaction
         if transaction_name:
             updated_tags.setdefault("transaction", transaction_name)
         if scope._span is not None:
-            sample_rate = experiments.get("metrics_summary_sample_rate")
-            # We default the sample rate of metrics summaries to 1.0 only when the sample rate is `None` since we
-            # want to honor the user's decision if they pass a valid float.
-            if sample_rate is None:
-                sample_rate = 1.0
-            should_summarize_metric_callback = experiments.get(
-                "should_summarize_metric"
-            )
-            if random.random() < sample_rate and (
-                should_summarize_metric_callback is None
-                or should_summarize_metric_callback(key, updated_tags)
-            ):
-                local_aggregator = scope._span._get_local_aggregator()
+            local_aggregator = scope._span._get_local_aggregator()
 
+    experiments = client.options.get("_experiments", {})
     before_emit_callback = experiments.get("before_emit_metric")
     if before_emit_callback is not None:
         with recursion_protection() as in_metrics:
             if not in_metrics:
-                if not before_emit_callback(key, updated_tags):
+                if not before_emit_callback(key, value, unit, updated_tags):
                     return None, None, updated_tags
 
     return client.metrics_aggregator, local_aggregator, updated_tags
 
 
-def incr(
+def increment(
     key,  # type: str
     value=1.0,  # type: float
     unit="none",  # type: MeasurementUnit
     tags=None,  # type: Optional[MetricTags]
     timestamp=None,  # type: Optional[Union[float, datetime]]
     stacklevel=0,  # type: int
 ):
     # type: (...) -> None
     """Increments a counter."""
-    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(key, tags)
+    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
+        key, value, unit, tags
+    )
     if aggregator is not None:
         aggregator.add(
             "c", key, value, unit, tags, timestamp, local_aggregator, stacklevel
         )
 
 
+# alias as incr is relatively common in python
+incr = increment
+
+
 class _Timing:
     def __init__(
         self,
         key,  # type: str
         tags,  # type: Optional[MetricTags]
         timestamp,  # type: Optional[Union[float, datetime]]
         value,  # type: Optional[float]
@@ -818,15 +833,18 @@
 
         return self
 
     def __exit__(self, exc_type, exc_value, tb):
         # type: (Any, Any, Any) -> None
         assert self._span, "did not enter"
         aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
-            self.key, self.tags
+            self.key,
+            self.value,
+            self.unit,
+            self.tags,
         )
         if aggregator is not None:
             elapsed = TIMING_FUNCTIONS[self.unit]() - self.entered  # type: ignore
             aggregator.add(
                 "d",
                 self.key,
                 elapsed,
@@ -873,15 +891,17 @@
     This method supports three forms of invocation:
 
     - when a `value` is provided, it functions similar to `distribution` but with
     - it can be used as a context manager
     - it can be used as a decorator
     """
     if value is not None:
-        aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(key, tags)
+        aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
+            key, value, unit, tags
+        )
         if aggregator is not None:
             aggregator.add(
                 "d", key, value, unit, tags, timestamp, local_aggregator, stacklevel
             )
     return _Timing(key, tags, timestamp, value, unit, stacklevel)
 
 
@@ -891,15 +911,17 @@
     unit="none",  # type: MeasurementUnit
     tags=None,  # type: Optional[MetricTags]
     timestamp=None,  # type: Optional[Union[float, datetime]]
     stacklevel=0,  # type: int
 ):
     # type: (...) -> None
     """Emits a distribution."""
-    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(key, tags)
+    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
+        key, value, unit, tags
+    )
     if aggregator is not None:
         aggregator.add(
             "d", key, value, unit, tags, timestamp, local_aggregator, stacklevel
         )
 
 
 def set(
@@ -908,15 +930,17 @@
     unit="none",  # type: MeasurementUnit
     tags=None,  # type: Optional[MetricTags]
     timestamp=None,  # type: Optional[Union[float, datetime]]
     stacklevel=0,  # type: int
 ):
     # type: (...) -> None
     """Emits a set."""
-    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(key, tags)
+    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
+        key, value, unit, tags
+    )
     if aggregator is not None:
         aggregator.add(
             "s", key, value, unit, tags, timestamp, local_aggregator, stacklevel
         )
 
 
 def gauge(
@@ -925,12 +949,14 @@
     unit="none",  # type: MeasurementUnit
     tags=None,  # type: Optional[MetricTags]
     timestamp=None,  # type: Optional[Union[float, datetime]]
     stacklevel=0,  # type: int
 ):
     # type: (...) -> None
     """Emits a gauge."""
-    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(key, tags)
+    aggregator, local_aggregator, tags = _get_aggregator_and_update_tags(
+        key, value, unit, tags
+    )
     if aggregator is not None:
         aggregator.add(
             "g", key, value, unit, tags, timestamp, local_aggregator, stacklevel
         )
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/monitor.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/profiler.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                 co_varnames
                 and co_varnames[0] == "self"
                 and "self" in frame.f_locals
             ):
                 for cls in frame.f_locals["self"].__class__.__mro__:
                     if name in cls.__dict__:
                         return "{}.{}".format(cls.__name__, name)
-        except AttributeError:
+        except (AttributeError, ValueError):
             pass
 
         # if it was a class method, (decorated with `@classmethod`)
         # we can get the class name by inspecting the f_locals for the `cls` argument
         try:
             if (
                 # the co_varnames start with the frame's positional arguments
@@ -365,15 +365,15 @@
                 co_varnames
                 and co_varnames[0] == "cls"
                 and "cls" in frame.f_locals
             ):
                 for cls in frame.f_locals["cls"].__mro__:
                     if name in cls.__dict__:
                         return "{}.{}".format(cls.__name__, name)
-        except AttributeError:
+        except (AttributeError, ValueError):
             pass
 
         # nothing we can do if it is a staticmethod (decorated with @staticmethod)
 
         # we've done all we can, time to give up and return what we have
         return name
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/scope.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/scrubber.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/serializer.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/session.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/sessions.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/spotlight.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/tracing.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/tracing_utils.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/transport.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,18 +156,30 @@
 def _parse_rate_limits(header, now=None):
     # type: (Any, Optional[datetime]) -> Iterable[Tuple[DataCategory, datetime]]
     if now is None:
         now = datetime.now(timezone.utc)
 
     for limit in header.split(","):
         try:
-            retry_after, categories, _ = limit.strip().split(":", 2)
+            parameters = limit.strip().split(":")
+            retry_after, categories = parameters[:2]
+
             retry_after = now + timedelta(seconds=int(retry_after))
             for category in categories and categories.split(";") or (None,):
-                yield category, retry_after
+                if category == "metric_bucket":
+                    try:
+                        namespaces = parameters[4].split(";")
+                    except IndexError:
+                        namespaces = []
+
+                    if not namespaces or "custom" in namespaces:
+                        yield category, retry_after
+
+                else:
+                    yield category, retry_after
         except (LookupError, ValueError):
             continue
 
 
 class HttpTransport(Transport):
     """The default HTTP transport."""
 
@@ -222,14 +234,15 @@
         quantity = 1
         if item is not None:
             data_category = item.data_category
             if data_category == "attachment":
                 # quantity of 0 is actually 1 as we do not want to count
                 # empty attachments as actually empty.
                 quantity = len(item.get_bytes()) or 1
+
         elif data_category is None:
             raise TypeError("data category not provided")
 
         self._discarded_events[data_category, reason] += quantity
 
     def _update_rate_limits(self, response):
         # type: (urllib3.BaseHTTPResponse) -> None
@@ -348,14 +361,20 @@
         if client_report is not None:
             self.capture_envelope(Envelope(items=[client_report]))
 
     def _check_disabled(self, category):
         # type: (str) -> bool
         def _disabled(bucket):
             # type: (Any) -> bool
+
+            # The envelope item type used for metrics is statsd
+            # whereas the rate limit category is metric_bucket
+            if bucket == "statsd":
+                bucket = "metric_bucket"
+
             ts = self._disabled_until.get(bucket)
             return ts is not None and ts > datetime.now(timezone.utc)
 
         return _disabled(category) or _disabled(None)
 
     def _is_rate_limited(self):
         # type: () -> bool
@@ -376,15 +395,15 @@
     ):
         # type: (...) -> None
 
         # remove all items from the envelope which are over quota
         new_items = []
         for item in envelope.items:
             if self._check_disabled(item.data_category):
-                if item.data_category in ("transaction", "error", "default"):
+                if item.data_category in ("transaction", "error", "default", "statsd"):
                     self.on_dropped_event("self_rate_limits")
                 self.record_lost_event("ratelimit_backoff", item=item)
             else:
                 new_items.append(item)
 
         # Since we're modifying the envelope here make a copy so that others
         # that hold references do not see their envelope modified.
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/types.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/utils.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,24 @@
     pass
 
 
 def get_git_revision():
     # type: () -> Optional[str]
     try:
         with open(os.path.devnull, "w+") as null:
+            # prevent command prompt windows from popping up on windows
+            startupinfo = None
+            if sys.platform == "win32" or sys.platform == "cygwin":
+                startupinfo = subprocess.STARTUPINFO()
+                startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+
             revision = (
                 subprocess.Popen(
                     ["git", "rev-parse", "HEAD"],
+                    startupinfo=startupinfo,
                     stdout=subprocess.PIPE,
                     stderr=null,
                     stdin=null,
                 )
                 .communicate()[0]
                 .strip()
                 .decode("utf-8")
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk/worker.py` & `sentry-sdk-2.0.0rc5/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/PKG-INFO` & `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/SOURCES.txt` & `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/requires.txt` & `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/setup.py` & `sentry-sdk-2.0.0rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.0.0rc4",
+    version="2.0.0rc5",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry-sdk-2.0.0rc4/tests/test_api.py` & `sentry-sdk-2.0.0rc5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_basics.py` & `sentry-sdk-2.0.0rc5/tests/test_basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
 
 @pytest.mark.skip(
     reason="This test is not valid anymore, because with the new Scopes calling bind_client on the Hub sets the client on the global scope. This test should be removed once the Hub is removed"
 )
 def test_client_initialized_within_scope(sentry_init, caplog):
     caplog.set_level(logging.WARNING)
 
-    sentry_init(debug=True)
+    sentry_init()
 
     with push_scope():
         Hub.current.bind_client(Client())
 
     (record,) = (x for x in caplog.records if x.levelname == "WARNING")
 
     assert record.msg.startswith("init() called inside of pushed scope.")
@@ -451,15 +451,15 @@
 
 @pytest.mark.skip(
     reason="This test is not valid anymore, because with the new Scopes the push_scope just returns the isolation scope. This test should be removed once the Hub is removed"
 )
 def test_scope_leaks_cleaned_up(sentry_init, caplog):
     caplog.set_level(logging.WARNING)
 
-    sentry_init(debug=True)
+    sentry_init()
 
     old_stack = list(Hub.current._stack)
 
     with push_scope():
         push_scope()
 
     assert Hub.current._stack == old_stack
@@ -471,15 +471,15 @@
 
 @pytest.mark.skip(
     reason="This test is not valid anymore, because with the new Scopes there is not pushing and popping of scopes. This test should be removed once the Hub is removed"
 )
 def test_scope_popped_too_soon(sentry_init, caplog):
     caplog.set_level(logging.ERROR)
 
-    sentry_init(debug=True)
+    sentry_init()
 
     old_stack = list(Hub.current._stack)
 
     with push_scope():
         Hub.current.pop_scope_unsafe()
 
     assert Hub.current._stack == old_stack
@@ -515,15 +515,15 @@
 
     (event,) = events
 
     assert event["message"] == "hifoobarbaz"
 
 
 def test_capture_event_with_scope_kwargs(sentry_init, capture_events):
-    sentry_init(debug=True)
+    sentry_init()
     events = capture_events()
     capture_event({}, level="info", extras={"foo": "bar"})
     (event,) = events
     assert event["level"] == "info"
     assert event["extra"]["foo"] == "bar"
```

### Comparing `sentry-sdk-2.0.0rc4/tests/test_client.py` & `sentry-sdk-2.0.0rc5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_conftest.py` & `sentry-sdk-2.0.0rc5/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_crons.py` & `sentry-sdk-2.0.0rc5/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_envelope.py` & `sentry-sdk-2.0.0rc5/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_exceptiongroup.py` & `sentry-sdk-2.0.0rc5/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_lru_cache.py` & `sentry-sdk-2.0.0rc5/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_metrics.py` & `sentry-sdk-2.0.0rc5/tests/test_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,24 +50,25 @@
         rv.append((ts, name, ty, values, tags))
     rv.sort(key=lambda x: (x[0], x[1], tuple(sorted(tags.items()))))
     return rv
 
 
 @minimum_python_37_with_gevent
 @pytest.mark.forked
-def test_incr(sentry_init, capture_envelopes, maybe_monkeypatched_threading):
+def test_increment(sentry_init, capture_envelopes, maybe_monkeypatched_threading):
     sentry_init(
         release="fun-release",
         environment="not-fun-env",
         _experiments={"enable_metrics": True, "metric_code_locations": True},
     )
     ts = time.time()
     envelopes = capture_envelopes()
 
-    metrics.incr("foobar", 1.0, tags={"foo": "bar", "blub": "blah"}, timestamp=ts)
+    metrics.increment("foobar", 1.0, tags={"foo": "bar", "blub": "blah"}, timestamp=ts)
+    # python specific alias
     metrics.incr("foobar", 2.0, tags={"foo": "bar", "blub": "blah"}, timestamp=ts)
     Hub.current.flush()
 
     (envelope,) = envelopes
     statsd_item, meta_item = envelope.items
 
     assert statsd_item.headers["type"] == "statsd"
@@ -479,16 +480,16 @@
     ts = time.time()
     envelopes = capture_envelopes()
 
     metrics.gauge("my-gauge", 10.0, tags={"x": "y"}, timestamp=ts)
     metrics.gauge("my-gauge", 20.0, tags={"x": "y"}, timestamp=ts)
     metrics.gauge("my-gauge", 30.0, tags={"x": "y"}, timestamp=ts)
     for _ in range(10):
-        metrics.incr("counter-1", 1.0, timestamp=ts)
-    metrics.incr("counter-2", 1.0, timestamp=ts)
+        metrics.increment("counter-1", 1.0, timestamp=ts)
+    metrics.increment("counter-2", 1.0, timestamp=ts)
 
     Hub.current.flush()
 
     (envelope,) = envelopes
 
     assert len(envelope.items) == 1
     assert envelope.items[0].headers["type"] == "statsd"
@@ -562,34 +563,29 @@
         "release": "fun-release@1.0.0",
         "environment": "not-fun-env",
     }
 
 
 @minimum_python_37_with_gevent
 @pytest.mark.forked
-@pytest.mark.parametrize("sample_rate", [1.0, None])
 def test_metric_summaries(
-    sentry_init, capture_envelopes, sample_rate, maybe_monkeypatched_threading
+    sentry_init, capture_envelopes, maybe_monkeypatched_threading
 ):
     sentry_init(
         release="fun-release@1.0.0",
         environment="not-fun-env",
         enable_tracing=True,
-        _experiments={
-            "enable_metrics": True,
-            "metrics_summary_sample_rate": sample_rate,
-        },
     )
     ts = time.time()
     envelopes = capture_envelopes()
 
     with start_transaction(
         op="stuff", name="/foo", source=TRANSACTION_SOURCE_ROUTE
     ) as transaction:
-        metrics.incr("root-counter", timestamp=ts)
+        metrics.increment("root-counter", timestamp=ts)
         with metrics.timing("my-timer-metric", tags={"a": "b"}, timestamp=ts):
             for x in range(10):
                 metrics.distribution("my-dist", float(x), timestamp=ts)
 
     Hub.current.flush()
 
     (transaction, envelope) = envelopes
@@ -673,204 +669,138 @@
         "release": "fun-release@1.0.0",
         "transaction": "/foo",
     }
 
 
 @minimum_python_37_with_gevent
 @pytest.mark.forked
-def test_metrics_summary_disabled(
-    sentry_init, capture_envelopes, maybe_monkeypatched_threading
-):
-    sentry_init(
-        release="fun-release@1.0.0",
-        environment="not-fun-env",
-        enable_tracing=True,
-        _experiments={"enable_metrics": True, "metrics_summary_sample_rate": 0.0},
-    )
-    ts = time.time()
-    envelopes = capture_envelopes()
-
-    with start_transaction(
-        op="stuff", name="/foo", source=TRANSACTION_SOURCE_ROUTE
-    ) as transaction:
-        with metrics.timing("my-timer-metric", tags={"a": "b"}, timestamp=ts):
-            pass
-
-    Hub.current.flush()
-
-    (transaction, envelope) = envelopes
-
-    # Metrics Emission
-    assert envelope.items[0].headers["type"] == "statsd"
-    m = parse_metrics(envelope.items[0].payload.get_bytes())
-
-    assert len(m) == 1
-    assert m[0][1] == "my-timer-metric@second"
-    assert m[0][2] == "d"
-    assert len(m[0][3]) == 1
-    assert m[0][4] == {
-        "a": "b",
-        "transaction": "/foo",
-        "release": "fun-release@1.0.0",
-        "environment": "not-fun-env",
-    }
-
-    # Measurement Attachment
-    t = transaction.items[0].get_transaction_event()
-    assert "_metrics_summary" not in t
-    assert "_metrics_summary" not in t["spans"][0]
-
-
-@minimum_python_37_with_gevent
-@pytest.mark.forked
-@pytest.mark.skip(reason="Temporarily disable to release SDK 2.0a1.")
-def test_metrics_summary_filtered(
-    sentry_init, capture_envelopes, maybe_monkeypatched_threading
+@pytest.mark.parametrize(
+    "metric_name,metric_unit,expected_name",
+    [
+        ("first-metric", "nano-second", "first-metric@nanosecond"),
+        ("another_metric?", "nano second", "another_metric_@nanosecond"),
+        (
+            "metric",
+            "nanosecond",
+            "metric@nanosecond",
+        ),
+        (
+            "my.amaze.metric I guess",
+            "nano|\nsecond",
+            "my.amaze.metric_I_guess@nanosecond",
+        ),
+        ("métríc", "nanöseconď", "m_tr_c@nansecon"),
+    ],
+)
+def test_metric_name_normalization(
+    sentry_init,
+    capture_envelopes,
+    metric_name,
+    metric_unit,
+    expected_name,
+    maybe_monkeypatched_threading,
 ):
-    def should_summarize_metric(key, tags):
-        return key == "foo"
-
     sentry_init(
-        release="fun-release@1.0.0",
-        environment="not-fun-env",
-        enable_tracing=True,
-        _experiments={
-            "enable_metrics": True,
-            "metrics_summary_sample_rate": 1.0,
-            "should_summarize_metric": should_summarize_metric,
-        },
+        _experiments={"enable_metrics": True, "metric_code_locations": False},
     )
-    ts = time.time()
     envelopes = capture_envelopes()
 
-    with start_transaction(
-        op="stuff", name="/foo", source=TRANSACTION_SOURCE_ROUTE
-    ) as transaction:
-        metrics.timing("foo", value=3.0, tags={"a": "b"}, timestamp=ts)
-        metrics.timing("foo", value=2.0, tags={"b": "c"}, timestamp=ts)
-        metrics.timing("bar", value=1.0, tags={"a": "b"}, timestamp=ts)
+    metrics.distribution(metric_name, 1.0, unit=metric_unit)
 
     Hub.current.flush()
 
-    (transaction, envelope) = envelopes
+    (envelope,) = envelopes
 
-    # Metrics Emission
+    assert len(envelope.items) == 1
     assert envelope.items[0].headers["type"] == "statsd"
-    m = parse_metrics(envelope.items[0].payload.get_bytes())
 
-    assert len(m) == 3
-    assert m[0][1] == "bar@second"
-    assert m[1][1] == "foo@second"
-    assert m[2][1] == "foo@second"
+    parsed_metrics = parse_metrics(envelope.items[0].payload.get_bytes())
+    assert len(parsed_metrics) == 1
 
-    # Measurement Attachment
-    t = transaction.items[0].get_transaction_event()["_metrics_summary"]
-    assert len(t["d:foo@second"]) == 2
-    assert {
-        "tags": {
-            "a": "b",
-            "environment": "not-fun-env",
-            "release": "fun-release@1.0.0",
-            "transaction": "/foo",
-        },
-        "min": 3.0,
-        "max": 3.0,
-        "count": 1,
-        "sum": 3.0,
-    } in t["d:foo@second"]
-    assert {
-        "tags": {
-            "b": "c",
-            "environment": "not-fun-env",
-            "release": "fun-release@1.0.0",
-            "transaction": "/foo",
-        },
-        "min": 2.0,
-        "max": 2.0,
-        "count": 1,
-        "sum": 2.0,
-    } in t["d:foo@second"]
+    name = parsed_metrics[0][1]
+    assert name == expected_name
 
 
 @minimum_python_37_with_gevent
 @pytest.mark.forked
-def test_tag_normalization(
-    sentry_init, capture_envelopes, maybe_monkeypatched_threading
+@pytest.mark.parametrize(
+    "metric_tag,expected_tag",
+    [
+        ({"f-oo|bar": "%$foo/"}, {"f-oobar": "%$foo/"}),
+        ({"foo$.$.$bar": "blah{}"}, {"foo..bar": "blah{}"}),
+        (
+            {"foö-bar": "snöwmän"},
+            {"fo-bar": "snöwmän"},
+        ),
+        ({"route": "GET /foo"}, {"route": "GET /foo"}),
+        ({"__bar__": "this | or , that"}, {"__bar__": "this \\u{7c} or \\u{2c} that"}),
+        ({"foo/": "hello!\n\r\t\\"}, {"foo/": "hello!\\n\\r\\t\\\\"}),
+    ],
+)
+def test_metric_tag_normalization(
+    sentry_init,
+    capture_envelopes,
+    metric_tag,
+    expected_tag,
+    maybe_monkeypatched_threading,
 ):
     sentry_init(
-        release="fun-release@1.0.0",
-        environment="not-fun-env",
         _experiments={"enable_metrics": True, "metric_code_locations": False},
     )
-    ts = time.time()
     envelopes = capture_envelopes()
 
-    metrics.distribution("a", 1.0, tags={"foo-bar": "%$foo"}, timestamp=ts)
-    metrics.distribution("b", 1.0, tags={"foo$$$bar": "blah{}"}, timestamp=ts)
-    metrics.distribution("c", 1.0, tags={"foö-bar": "snöwmän"}, timestamp=ts)
-    metrics.distribution("d", 1.0, tags={"route": "GET /foo"}, timestamp=ts)
+    metrics.distribution("a", 1.0, tags=metric_tag)
 
     Hub.current.flush()
 
     (envelope,) = envelopes
 
     assert len(envelope.items) == 1
     assert envelope.items[0].headers["type"] == "statsd"
-    m = parse_metrics(envelope.items[0].payload.get_bytes())
 
-    assert len(m) == 4
-    assert m[0][4] == {
-        "foo-bar": "$foo",
-        "release": "fun-release@1.0.0",
-        "environment": "not-fun-env",
-    }
-    assert m[1][4] == {
-        "foo_bar": "blah{}",
-        "release": "fun-release@1.0.0",
-        "environment": "not-fun-env",
-    }
-    assert m[2][4] == {
-        "fo_-bar": "snöwmän",
-        "release": "fun-release@1.0.0",
-        "environment": "not-fun-env",
-    }
-    assert m[3][4] == {
-        "release": "fun-release@1.0.0",
-        "environment": "not-fun-env",
-        "route": "GET /foo",
-    }
+    parsed_metrics = parse_metrics(envelope.items[0].payload.get_bytes())
+    assert len(parsed_metrics) == 1
+
+    tags = parsed_metrics[0][4]
+
+    expected_tag_key, expected_tag_value = expected_tag.popitem()
+    assert expected_tag_key in tags
+    assert tags[expected_tag_key] == expected_tag_value
 
 
 @minimum_python_37_with_gevent
 @pytest.mark.forked
 def test_before_emit_metric(
     sentry_init, capture_envelopes, maybe_monkeypatched_threading
 ):
-    def before_emit(key, tags):
-        if key == "removed-metric":
+    def before_emit(key, value, unit, tags):
+        if key == "removed-metric" or value == 47 or unit == "unsupported":
             return False
+
         tags["extra"] = "foo"
         del tags["release"]
         # this better be a noop!
-        metrics.incr("shitty-recursion")
+        metrics.increment("shitty-recursion")
         return True
 
     sentry_init(
         release="fun-release@1.0.0",
         environment="not-fun-env",
         _experiments={
             "enable_metrics": True,
             "metric_code_locations": False,
             "before_emit_metric": before_emit,
         },
     )
     envelopes = capture_envelopes()
 
-    metrics.incr("removed-metric", 1.0)
-    metrics.incr("actual-metric", 1.0)
+    metrics.increment("removed-metric", 1.0)
+    metrics.increment("another-removed-metric", 47)
+    metrics.increment("yet-another-removed-metric", 1.0, unit="unsupported")
+    metrics.increment("actual-metric", 1.0)
     Hub.current.flush()
 
     (envelope,) = envelopes
 
     assert len(envelope.items) == 1
     assert envelope.items[0].headers["type"] == "statsd"
     m = parse_metrics(envelope.items[0].payload.get_bytes())
@@ -894,15 +824,15 @@
         environment="not-fun-env",
         _experiments={
             "enable_metrics": True,
         },
     )
     envelopes = capture_envelopes()
 
-    metrics.incr("a-metric", 1.0)
+    metrics.increment("a-metric", 1.0)
     Hub.current.flush()
 
     assert len(envelopes) == 1
     assert Hub.current.client.metrics_aggregator.buckets == {}
 
 
 @minimum_python_37_with_gevent
@@ -913,15 +843,15 @@
     sentry_init(
         release="fun-release",
         environment="not-fun-env",
         _experiments={"enable_metrics": True, "metric_code_locations": False},
     )
     envelopes = capture_envelopes()
 
-    metrics.incr(
+    metrics.increment(
         "counter",
         tags={
             "no-value": None,
             "an-int": 42,
             "a-float": 23.0,
             "a-string": "blah",
             "more-than-one": [1, "zwei", "3.0", None],
@@ -958,20 +888,20 @@
     )
     envelopes = capture_envelopes()
     test_client = Hub.current.client
 
     real_capture_envelope = test_client.transport.capture_envelope
 
     def bad_capture_envelope(*args, **kwargs):
-        metrics.incr("bad-metric")
+        metrics.increment("bad-metric")
         return real_capture_envelope(*args, **kwargs)
 
     monkeypatch.setattr(test_client.transport, "capture_envelope", bad_capture_envelope)
 
-    metrics.incr("counter")
+    metrics.increment("counter")
 
     # flush twice to see the inner metric
     Hub.current.flush()
     Hub.current.flush()
 
     (envelope,) = envelopes
     m = parse_metrics(envelope.items[0].payload.get_bytes())
@@ -992,20 +922,20 @@
     )
     envelopes = capture_envelopes()
     test_client = Hub.current.client
 
     real_capture_envelope = test_client.transport.capture_envelope
 
     def bad_capture_envelope(*args, **kwargs):
-        metrics.incr("bad-metric")
+        metrics.increment("bad-metric")
         return real_capture_envelope(*args, **kwargs)
 
     monkeypatch.setattr(test_client.transport, "capture_envelope", bad_capture_envelope)
 
-    metrics.incr("counter")
+    metrics.increment("counter")
 
     # flush via sleep and flag
     Hub.current.client.metrics_aggregator._force_flush = True
     time.sleep(0.5)
 
     (envelope,) = envelopes
     m = parse_metrics(envelope.items[0].payload.get_bytes())
```

### Comparing `sentry-sdk-2.0.0rc4/tests/test_monitor.py` & `sentry-sdk-2.0.0rc5/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat.py` & `sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat_event.py` & `sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_profiler.py` & `sentry-sdk-2.0.0rc5/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_scope.py` & `sentry-sdk-2.0.0rc5/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_scrubber.py` & `sentry-sdk-2.0.0rc5/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_serializer.py` & `sentry-sdk-2.0.0rc5/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_sessions.py` & `sentry-sdk-2.0.0rc5/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_spotlight.py` & `sentry-sdk-2.0.0rc5/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_transport.py` & `sentry-sdk-2.0.0rc5/tests/test_transport.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from unittest import mock
 
 import pytest
 from pytest_localserver.http import WSGIServer
 from werkzeug.wrappers import Request, Response
 
 from sentry_sdk import Hub, Client, add_breadcrumb, capture_message, Scope
-from sentry_sdk.envelope import Envelope, parse_json
+from sentry_sdk.envelope import Envelope, Item, parse_json
 from sentry_sdk.transport import KEEP_ALIVE_SOCKET_OPTIONS, _parse_rate_limits
 from sentry_sdk.integrations.logging import LoggingIntegration, ignore_logger
 
 
 CapturedData = namedtuple("CapturedData", ["path", "event", "envelope", "compressed"])
 
 
@@ -467,7 +467,118 @@
 
     client.capture_event({"type": "transaction"})
     client.capture_event({"type": "transaction"})
     client.capture_event({"type": "event"})
     client.flush()
 
     assert len(capturing_server.captured) == 0
+
+
+@pytest.mark.parametrize("response_code", [200, 429])
+def test_metric_bucket_limits(capturing_server, response_code, make_client):
+    client = make_client()
+    capturing_server.respond_with(
+        code=response_code,
+        headers={
+            "X-Sentry-Rate-Limits": "4711:metric_bucket:organization:quota_exceeded:custom"
+        },
+    )
+
+    envelope = Envelope()
+    envelope.add_item(Item(payload=b"{}", type="statsd"))
+    client.transport.capture_envelope(envelope)
+    client.flush()
+
+    assert len(capturing_server.captured) == 1
+    assert capturing_server.captured[0].path == "/api/132/envelope/"
+    capturing_server.clear_captured()
+
+    assert set(client.transport._disabled_until) == set(["metric_bucket"])
+
+    client.transport.capture_envelope(envelope)
+    client.capture_event({"type": "transaction"})
+    client.flush()
+
+    assert len(capturing_server.captured) == 2
+
+    envelope = capturing_server.captured[0].envelope
+    assert envelope.items[0].type == "transaction"
+    envelope = capturing_server.captured[1].envelope
+    assert envelope.items[0].type == "client_report"
+    report = parse_json(envelope.items[0].get_bytes())
+    assert report["discarded_events"] == [
+        {"category": "metric_bucket", "reason": "ratelimit_backoff", "quantity": 1},
+    ]
+
+
+@pytest.mark.parametrize("response_code", [200, 429])
+def test_metric_bucket_limits_with_namespace(
+    capturing_server, response_code, make_client
+):
+    client = make_client()
+    capturing_server.respond_with(
+        code=response_code,
+        headers={
+            "X-Sentry-Rate-Limits": "4711:metric_bucket:organization:quota_exceeded:foo"
+        },
+    )
+
+    envelope = Envelope()
+    envelope.add_item(Item(payload=b"{}", type="statsd"))
+    client.transport.capture_envelope(envelope)
+    client.flush()
+
+    assert len(capturing_server.captured) == 1
+    assert capturing_server.captured[0].path == "/api/132/envelope/"
+    capturing_server.clear_captured()
+
+    assert set(client.transport._disabled_until) == set([])
+
+    client.transport.capture_envelope(envelope)
+    client.capture_event({"type": "transaction"})
+    client.flush()
+
+    assert len(capturing_server.captured) == 2
+
+    envelope = capturing_server.captured[0].envelope
+    assert envelope.items[0].type == "statsd"
+    envelope = capturing_server.captured[1].envelope
+    assert envelope.items[0].type == "transaction"
+
+
+@pytest.mark.parametrize("response_code", [200, 429])
+def test_metric_bucket_limits_with_all_namespaces(
+    capturing_server, response_code, make_client
+):
+    client = make_client()
+    capturing_server.respond_with(
+        code=response_code,
+        headers={
+            "X-Sentry-Rate-Limits": "4711:metric_bucket:organization:quota_exceeded"
+        },
+    )
+
+    envelope = Envelope()
+    envelope.add_item(Item(payload=b"{}", type="statsd"))
+    client.transport.capture_envelope(envelope)
+    client.flush()
+
+    assert len(capturing_server.captured) == 1
+    assert capturing_server.captured[0].path == "/api/132/envelope/"
+    capturing_server.clear_captured()
+
+    assert set(client.transport._disabled_until) == set(["metric_bucket"])
+
+    client.transport.capture_envelope(envelope)
+    client.capture_event({"type": "transaction"})
+    client.flush()
+
+    assert len(capturing_server.captured) == 2
+
+    envelope = capturing_server.captured[0].envelope
+    assert envelope.items[0].type == "transaction"
+    envelope = capturing_server.captured[1].envelope
+    assert envelope.items[0].type == "client_report"
+    report = parse_json(envelope.items[0].get_bytes())
+    assert report["discarded_events"] == [
+        {"category": "metric_bucket", "reason": "ratelimit_backoff", "quantity": 1},
+    ]
```

### Comparing `sentry-sdk-2.0.0rc4/tests/test_types.py` & `sentry-sdk-2.0.0rc5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc4/tests/test_utils.py` & `sentry-sdk-2.0.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

