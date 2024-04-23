# Comparing `tmp/utilmeta-2.4.1.tar.gz` & `tmp/utilmeta-2.5.2.tar.gz`

## Comparing `utilmeta-2.4.1.tar` & `utilmeta-2.5.2.tar`

### file list

```diff
@@ -1,261 +1,282 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 utilmeta-2.4.1/MANIFEST.in
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/hello.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/bmi_calc/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/bmi_calc/meta.ini
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/bmi_calc/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/config.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/meta.ini
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/blog/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/blog/api.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/blog/models.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/blog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/mini_blog/blog/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/meta.ini
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/server.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/api.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/email.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/models.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/schema.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/examples/user_auth/user/migrations/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/__init__.py
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/base.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/constant.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/meta.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/commands/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/commands/base.py
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/commands/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/__init__.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/main.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/meta.ini
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/config/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/config/conf.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/config/env.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/config/service.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/domain/__init__.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/service/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/full/service/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/lite/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/lite/meta.ini
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/bin/template/lite/server.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/base.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/env.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/http.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/pool.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/conf/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/__init__.py
--rw-r--r--   0        0        0    21785 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/base.py
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/decorator.py
--rw-r--r--   0        0        0    11959 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/endpoint.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/hook.py
--rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/route.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/plugins/__init__.py
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/plugins/cors.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/plugins/rate.py
--rw-r--r--   0        0        0    11293 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/plugins/retry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/specs/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/specs/base.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/specs/graphql.py
--rw-r--r--   0        0        0    22519 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/specs/openapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/api/specs/protobuf.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/__init__.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/base.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/basic.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/jwt.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/oauth2.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/properties.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/plugins/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/plugins/require.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/__init__.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/base.py
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/cache.py
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/cached_db.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/db.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/django.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/file.py
--rw-r--r--   0        0        0    19080 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/auth/session/schema.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/base.py
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/config.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/lock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/__init__.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/django.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/aioredis.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/config.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/entity.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/lock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/alter_amount.lua
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/batch_count.lua
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/batch_exists.lua
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/batch_relates.lua
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/batch_retrieve.lua
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/hpop_many.lua
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/pop_many.lua
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/pop_queue.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/plugins/__init__.py
--rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/plugins/api.py
--rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/plugins/base.py
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/plugins/entity.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cache/plugins/sdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/__init__.py
--rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/aiohttp.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/base.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/httpx.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/requests.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/cli/backends/urllib.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/__init__.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/base.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/bytesio.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/django.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/starlette.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/tornado.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/file/backends/werkzeug.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/__init__.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/compiler.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/context.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/encoder.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/exceptions.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/generator.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/param.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/parser.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/__init__.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/base.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/__init__.py
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/compiler.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/constant.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/database.py
--rw-r--r--   0        0        0    18192 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/deletion.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/exceptions.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/expressions.py
--rw-r--r--   0        0        0    12233 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/field.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/generator.py
--rw-r--r--   0        0        0    12523 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/model.py
--rw-r--r--   0        0        0    11453 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/models.py
--rw-r--r--   0        0        0    19361 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/query.py
--rw-r--r--   0        0        0    30344 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/queryset.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/django/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/peewee/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/peewee/example.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/peewee/peewee.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/backends/sqlalchemy/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/databases/__init__.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/databases/base.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/databases/config.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/databases/encode.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/__init__.py
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/field.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/filter.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/order.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/pagination.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/fields/scope.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/plugins/__init__.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/plugins/atomic.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/orm/plugins/relate.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/__init__.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/base.py
--rw-r--r--   0        0        0    19658 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/properties.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/var.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/aiohttp.py
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/base.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/django.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/sanic.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/starlette.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/tornado.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/request/backends/werkzeug.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/__init__.py
--rw-r--r--   0        0        0    24900 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/__init__.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/aiohttp.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/base.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/django.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/httpx.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/requests.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/sanic.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/starlette.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/tornado.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/urllib.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/response/backends/werkzeug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/__init__.py
--rw-r--r--   0        0        0    13293 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/base.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/fastapi.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/flask.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/sanic.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/starlette.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/tornado.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/werkzeug.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/__init__.py
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/adaptor.py
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/cmd.py
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/postgresql/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/server/backends/django/postgresql/base.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/websocket/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/websocket/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/websocket/properties.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/core/websocket/request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/api.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/cmd.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/config.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/connect.py
--rw-r--r--   0        0        0    28211 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/models.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/ops/schema.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/adaptor.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/base.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/context.py
--rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/datastructure.py
--rw-r--r--   0        0        0    10971 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/decorator.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/error.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/logical.py
--rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/plugin.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/constant/__init__.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/constant/data.py
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/constant/i18n.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/constant/vendor.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/constant/web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/exceptions/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/exceptions/config.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/exceptions/http.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/exceptions/runtime.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/__init__.py
--rw-r--r--   0        0        0    22748 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/data.py
--rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/orm.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/py.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/sys.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/time.py
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/functional/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/backends/__init__.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/backends/attrs.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/backends/dataclass.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/backends/pydantic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.4.1/utilmeta/utils/schema/backends/utype.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 utilmeta-2.4.1/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 utilmeta-2.4.1/LICENSE
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 utilmeta-2.4.1/README.md
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 utilmeta-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 utilmeta-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 utilmeta-2.5.2/MANIFEST.in
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/hello.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/bmi_calc/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/bmi_calc/meta.ini
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/bmi_calc/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/config.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/meta.ini
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/blog/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/blog/api.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/blog/models.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/blog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/mini_blog/blog/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/meta.ini
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/server.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/api.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/email.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/models.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/schema.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/examples/user_auth/user/migrations/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/__init__.py
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/base.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/constant.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/meta.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/commands/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/commands/base.py
+-rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/commands/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/__init__.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/main.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/meta.ini
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/config/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/config/conf.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/config/env.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/config/service.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/domain/__init__.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/service/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/full/service/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/lite/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/lite/meta.ini
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/bin/template/lite/server.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/base.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/env.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/http.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/pool.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/conf/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/__init__.py
+-rw-r--r--   0        0        0    23065 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/base.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/decorator.py
+-rw-r--r--   0        0        0    14731 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/endpoint.py
+-rw-r--r--   0        0        0     8199 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/hook.py
+-rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/route.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/plugins/__init__.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/plugins/cors.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/plugins/rate.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/plugins/retry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/specs/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/specs/base.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/specs/graphql.py
+-rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/specs/openapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/api/specs/protobuf.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/__init__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/base.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/basic.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/jwt.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/oauth2.py
+-rw-r--r--   0        0        0    12314 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/properties.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/plugins/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/plugins/require.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/__init__.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/base.py
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/cache.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/cached_db.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/db.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/django.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/file.py
+-rw-r--r--   0        0        0    19334 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/auth/session/schema.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/base.py
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/config.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/lock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/__init__.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/django.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/aioredis.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/config.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/entity.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/lock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/alter_amount.lua
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/batch_count.lua
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/batch_exists.lua
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/batch_relates.lua
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/batch_retrieve.lua
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/hpop_many.lua
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/pop_many.lua
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/pop_queue.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/plugins/__init__.py
+-rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/plugins/api.py
+-rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/plugins/base.py
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/plugins/entity.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cache/plugins/sdk.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/__init__.py
+-rw-r--r--   0        0        0    29782 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/base.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/endpoint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/__init__.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/aiohttp.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/base.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/httpx.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/requests.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/backends/urllib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/specs/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/cli/specs/openapi.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/__init__.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/base.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/bytesio.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/django.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/sanic.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/starlette.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/tornado.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/file/backends/werkzeug.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/__init__.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/compiler.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/context.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/encoder.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/exceptions.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/generator.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/param.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/parser.py
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/__init__.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/base.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/__init__.py
+-rw-r--r--   0        0        0    32125 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/compiler.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/constant.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/database.py
+-rw-r--r--   0        0        0    18192 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/deletion.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/exceptions.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/expressions.py
+-rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/field.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/generator.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/model.py
+-rw-r--r--   0        0        0    11453 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/models.py
+-rw-r--r--   0        0        0    19361 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/query.py
+-rw-r--r--   0        0        0    30477 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/django/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/peewee/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/peewee/example.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/peewee/peewee.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/backends/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/databases/__init__.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/databases/base.py
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/databases/config.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/databases/encode.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/__init__.py
+-rw-r--r--   0        0        0    15030 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/field.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/filter.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/order.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/pagination.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/fields/scope.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/plugins/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/plugins/atomic.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/orm/plugins/relate.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/__init__.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/base.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/client.py
+-rw-r--r--   0        0        0    19973 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/properties.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/var.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/aiohttp.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/base.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/django.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/sanic.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/starlette.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/tornado.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/request/backends/werkzeug.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/__init__.py
+-rw-r--r--   0        0        0    27084 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/__init__.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/aiohttp.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/base.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/django.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/httpx.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/requests.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/sanic.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/starlette.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/tornado.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/urllib.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/response/backends/werkzeug.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/__init__.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/base.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/fastapi.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/flask.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/sanic.py
+-rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/starlette.py
+-rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/tornado.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/werkzeug.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/__init__.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/adaptor.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/cmd.py
+-rw-r--r--   0        0        0    14356 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/postgresql/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/server/backends/django/postgresql/base.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/websocket/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/websocket/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/websocket/properties.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/core/websocket/request.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/__init__.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/aggregation.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/auth.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/client.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/cmd.py
+-rw-r--r--   0        0        0    11473 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/config.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/connect.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/key.py
+-rw-r--r--   0        0        0    24876 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/log.py
+-rw-r--r--   0        0        0    35419 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/models.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/monitor.py
+-rw-r--r--   0        0        0    17507 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/resources.py
+-rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/schema.py
+-rw-r--r--   0        0        0    17912 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/task.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/__init__.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/log.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/query.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/servers.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/token.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/api/utils.py
+-rw-r--r--   0        0        0    46570 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/migrations/0002_servicelog_access_token_servicelog_endpoint_ident_and_more.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/migrations/0003_aggregationlog.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/migrations/0004_alter_accesstoken_subject_alter_accesstoken_token_id_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/ops/migrations/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/adaptor.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/base.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/context.py
+-rw-r--r--   0        0        0     9734 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/datastructure.py
+-rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/decorator.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/error.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/logical.py
+-rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/plugin.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/constant/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/constant/data.py
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/constant/i18n.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/constant/vendor.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/constant/web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/exceptions/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/exceptions/config.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/exceptions/http.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/exceptions/runtime.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/__init__.py
+-rw-r--r--   0        0        0    22821 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/data.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/orm.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/py.py
+-rw-r--r--   0        0        0    19317 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/sys.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/time.py
+-rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/functional/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/backends/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/backends/attrs.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/backends/dataclass.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/backends/pydantic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utilmeta-2.5.2/utilmeta/utils/schema/backends/utype.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 utilmeta-2.5.2/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 utilmeta-2.5.2/LICENSE
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 utilmeta-2.5.2/README.md
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 utilmeta-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 utilmeta-2.5.2/PKG-INFO
```

### Comparing `utilmeta-2.4.1/examples/bmi_calc/server.py` & `utilmeta-2.5.2/examples/bmi_calc/server.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/mini_blog/blog/api.py` & `utilmeta-2.5.2/examples/mini_blog/blog/api.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/mini_blog/blog/migrations/0001_initial.py` & `utilmeta-2.5.2/examples/mini_blog/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/user_auth/server.py` & `utilmeta-2.5.2/examples/user_auth/server.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/user_auth/test.py` & `utilmeta-2.5.2/examples/user_auth/test.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/user_auth/user/api.py` & `utilmeta-2.5.2/examples/user_auth/user/api.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/user_auth/user/email.py` & `utilmeta-2.5.2/examples/user_auth/user/email.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/examples/user_auth/user/migrations/0001_initial.py` & `utilmeta-2.5.2/examples/user_auth/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/__init__.py` & `utilmeta-2.5.2/utilmeta/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .core.server.service import UtilMeta
 
 service: 'UtilMeta'     # current service in this process
 
 __website__ = 'https://utilmeta.com'
 __homepage__ = 'https://utilmeta.com/py'
-__author__ = 'Xulin Zhou (voidZXL)'
-__version__ = '2.4.1'
+__author__ = 'Xulin Zhou (@voidZXL)'
+__version__ = '2.5.2'
 
 
 def version_info() -> str:
     import platform
     import sys
     from pathlib import Path
```

### Comparing `utilmeta-2.4.1/utilmeta/bin/base.py` & `utilmeta-2.5.2/utilmeta/bin/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -200,20 +200,21 @@
                 cmd = cmd_cls
 
             args = []
             for arg in self.args:
                 arg = str(arg)
                 if arg.startswith('--'):
                     if '=' in arg:
-                        key, val = arg.split('=')
-                        kwargs[key] = val
+                        key, *values = arg.split('=')
+                        val = '='.join(values)
+                        kwargs[key] = kwargs[str(key).strip('--')] = val
                     else:
-                        kwargs[arg] = True
+                        kwargs[arg] = kwargs[str(arg).strip('--')] = True
                 elif arg.startswith('-'):
-                    kwargs[arg] = True
+                    kwargs[arg] = kwargs[arg.strip('-')] = True
                 else:
                     args.append(arg)
             return cmd(*args, **kwargs)
 
     @classmethod
     def mount(cls, cmd_cls: Type['BaseCommand'], name: str = '', *aliases: str):
         if not issubclass(cmd_cls, BaseCommand):
```

### Comparing `utilmeta-2.4.1/utilmeta/bin/constant.py` & `utilmeta-2.5.2/utilmeta/bin/constant.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/bin/meta.py` & `utilmeta-2.5.2/utilmeta/bin/meta.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/bin/commands/base.py` & `utilmeta-2.5.2/utilmeta/bin/commands/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/bin/commands/setup.py` & `utilmeta-2.5.2/utilmeta/bin/commands/setup.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/bin/template/lite/server.py` & `utilmeta-2.5.2/utilmeta/bin/template/lite/server.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/conf/base.py` & `utilmeta-2.5.2/utilmeta/conf/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from utype import DataClass
 from typing import Type, TypeVar, Optional
 
 T = TypeVar('T')
 
 
 class Config(DataClass):
+    __eager__ = False
+
     @classmethod
     def config(cls: Type[T]) -> Optional[T]:
         try:
             from utilmeta import service
         except ImportError:
             return None
         return service.get_config(cls)
```

### Comparing `utilmeta-2.4.1/utilmeta/conf/env.py` & `utilmeta-2.5.2/utilmeta/conf/env.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/conf/http.py` & `utilmeta-2.5.2/utilmeta/conf/http.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/conf/pool.py` & `utilmeta-2.5.2/utilmeta/conf/pool.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/conf/time.py` & `utilmeta-2.5.2/utilmeta/conf/time.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/api/__init__.py` & `utilmeta-2.5.2/utilmeta/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/api/base.py` & `utilmeta-2.5.2/utilmeta/core/api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union, Dict, Type, List
 from utilmeta.utils.error import Error
 from utilmeta.utils.context import ParserProperty
-from utilmeta.utils import Header, EndpointAttr, COMMON_METHODS, awaitable, classonlymethod, distinct_add
+from utilmeta.utils import Header, EndpointAttr, COMMON_METHODS, awaitable, \
+    classonlymethod, distinct_add
 from utilmeta.utils import exceptions as exc
 
 import inspect
 import warnings
 
 from functools import partial
 from utilmeta.utils import PluginEvent, PluginTarget, Property
@@ -15,14 +16,15 @@
 from ..response import Response
 from ..request import Request, var
 from .route import APIRoute
 from .endpoint import Endpoint
 from .hook import Hook, ErrorHook, BeforeHook, AfterHook
 from . import decorator
 from utype.utils.compat import is_annotated
+from utype.utils.exceptions import ParseError
 
 setup_class = PluginEvent('setup_class', synchronous_only=True)
 enter_route = PluginEvent('enter_route')
 exit_route = PluginEvent('exit_route')
 setup_instance = PluginEvent('setup_instance')
 process_response = PluginEvent('process_response', streamline_result=True)
 handle_error = PluginEvent('handle_error')
@@ -43,14 +45,17 @@
             raise TypeError(f'Invalid ref: {repr(self.ref)}, should be an API class, got {api}')
         self._api = api
         return api
 
 
 class API(PluginTarget):
     __options__ = Options()
+    # flags
+    __external__ = False
+    # ---
 
     _generator: decorator.APIGenerator
     _routes: List[APIRoute]
     _properties: Dict[str, ParserProperty]
     _annotations: Dict[str, type]
     _hook_cls: Type[Hook] = Hook
     _route_cls: Type[APIRoute] = APIRoute
@@ -173,14 +178,22 @@
                 if route.private:
                     continue
                 # route.initialize(cls)
                 routes.append(route)
                 # make the annotated key as a property that can access through instance
                 setattr(cls, key, route.make_property())
 
+            # ---------------------------------------------------
+            if inspect.isclass(val) and issubclass(val, Property):
+                # eg: logger: Logger
+                if key not in cls.__dict__:
+                    context = getattr(val, '__context__', None)
+                    if context and isinstance(context, Property):
+                        cls._make_property(key, context)
+
         for key, val in cls.__dict__.items():
             if val in handlers:
                 # already been added
                 continue
             if isinstance(val, APIRef):
                 val = val.api
 
@@ -209,15 +222,15 @@
 
                 if method:
                     # a sign to wrap it in Unit
                     # 1. @api.get                (method='get')
                     # 2. @api.parser             (method=None)
                     # 3. def get(self):          (method='get')
                     # 4. @api(method='CUSTOM')   (method='custom')
-                    val = cls._endpoint_cls.apply_for(val)
+                    val = cls._endpoint_cls.apply_for(val, cls)
                 elif hook_type:
                     val = cls._hook_cls.dispatch_for(val, hook_type)
                 else:
                     continue
 
                 setattr(cls, key, val)  # reset value
 
@@ -291,18 +304,31 @@
             options=cls.__options__,
             global_vars=cls._global_vars()
         )
 
         inst = prop.init(field)
 
         def getter(self: 'API'):
+            if name in self.__dict__:
+                return self.__dict__[name]
             value = inst.get(self.request)
             if unprovided(value):
+                default = field.get_default(cls.__options__, defer=None)
+                if not unprovided(default):
+                    # NOT CACHE
+                    return default
                 raise exc.BadRequest(f'{cls.__name__}: '
                                      f'{prop.__class__.__name__}({repr(field.name)}) not provided')
+            try:
+                value = field.parse_value(
+                    value,
+                    context=self.__options__.make_context(cls)
+                )
+            except ParseError as e:
+                raise exc.BadRequest(str(e), detail=e.get_detail()) from e
             self.__dict__[name] = value     # auto-cached
             return value
 
         getter.__field__ = prop
 
         setter = None
         if prop.setter != Property.setter:
@@ -339,28 +365,22 @@
         plugins = generator.kwargs.get('plugins')
         if plugins:
             cls._add_plugins(*plugins)
         cls._generator = generator
         return cls
 
     # @classonlymethod
-    # def __adapt__(cls, vendor_router):
-    #     # adapt a vendor (other backends) router to utilmeta
-    #     # and mount to API, also can apply before/error/after hooks and plugins
-    #     # usage
-    #     # class AdaptAPI(API):
-    #     #    ad_fastapi = API.__adapt__(fastapi.routing.APIRouter())
-    #     pass
-
-    # @classonlymethod
     @classmethod
     def __as__(cls, backend, route: str, *, asynchronous: bool = None):
         from utilmeta import UtilMeta
         from utilmeta.core.server.backends.base import ServerAdaptor
-        service = UtilMeta(None, backend=backend, name=route.strip('/'))
+        if isinstance(backend, UtilMeta):
+            service = backend
+        else:
+            service = UtilMeta(None, backend=backend, name=route.strip('/'))
         # backend can be a module name or application
         adaptor = ServerAdaptor.dispatch(service)
         return adaptor.adapt(cls, route=route, asynchronous=asynchronous)
 
     @classonlymethod
     def __mount__(cls, handler: Union[APIRoute, Type['API'], APIRef, Endpoint, str], route: str = '',
                   before_hooks: List[BeforeHook] = (),
@@ -370,68 +390,85 @@
             handler = handler.api
         if isinstance(handler, str):
             from utilmeta.utils import import_obj
             handler = import_obj(handler)
         if isinstance(handler, APIRoute):
             cls._routes.append(handler)
             return
-        cls._routes.append(cls._route_cls(
+        api_route = cls._route_cls(
             handler=handler,
             route=route,
             name=route.replace('/', '_'),
             before_hooks=before_hooks,
             after_hooks=after_hooks,
             error_hooks=error_hooks
-        ))
+        )
+        api_route.compile_route()
+        cls._routes.append(api_route)
         cls._validate_routes()     # validate each time there is a new api mount
 
     def __init__(self, request):
         super().__init__()
         self.request = self._request_cls.apply_for(request)
         self.response = getattr(self, 'response', Response)
         # set request before setup instance, cause this hook may depend on the request context
         for key, val in self.__class__.__dict__.items():
             if isinstance(val, Endpoint):
                 setattr(self, key, partial(val, self))
             if isinstance(val, Hook):
                 setattr(self, key, partial(val, self))
-        # set request params for API instance
-        # wrapper: RequestContextWrapper = getattr(self.__class__, '_wrapper', None)
-        # if wrapper:
-        #     kwargs = wrapper.parse_context(request)
-        #     for name, val in kwargs.items():
-        #         setattr(self, name, val)
+
+        self._init_properties()
         setup_instance(self)
 
+    def _init_properties(self):
+        if not self._properties:
+            return
+        context = self.__options__.make_context(cls=__class__)
+        for name, prop in self._properties.items():
+            value = prop.get(self.request)
+            if not unprovided(value):
+                try:
+                    value = prop.field.parse_value(
+                        value,
+                        context=context
+                    )
+                except ParseError as e:
+                    if self.request.is_options:
+                        # ignore parse error for OPTIONS request
+                        continue
+                    raise exc.BadRequest(str(e), detail=e.get_detail()) from e
+                self.__dict__[name] = value
+
     def _handle_error(self, error: Error, error_hooks: dict):
         hook = error.get_hook(error_hooks, exact=isinstance(error.exception, exc.Redirect))
         # hook applied before handel_error plugin event
         if hook:
             result = hook(self, error)
         else:
             result = handle_error(self, error)
             # handle_error event can throw an error, or return a valid response
             # if nothing return, it implies that follow the api default error flow
             if result is None:
                 raise error.throw()
-        return process_response(self, result)
+        return result
 
     @awaitable(_handle_error)
     async def _handle_error(self, error: Error, error_hooks: dict):
         hook = error.get_hook(error_hooks, exact=isinstance(error.exception, exc.Redirect))
         # hook applied before handel_error plugin event
         if hook:
             result = await hook(self, error)
         else:
             result = await handle_error(self, error)
             # handle_error event can throw an error, or return a valid response
             # if nothing return, it implies that follow the api default error flow
             if result is None:
                 raise error.throw()
-        return await process_response(self, result)
+        return result
 
     def _resolve(self) -> APIRoute:
         method_routes: Dict[str, APIRoute] = {}
         for route in self._routes:
             if route.match_route(self.request):
                 # path math
                 if not route.method:
@@ -440,17 +477,17 @@
                     return route
                 # elif route.method == self.request.method and not self.request.is_options:
                 #     # options/cross-origin need to collect methods to generate Allow-Methods
                 #     return route
                 # first match is 1st priority
                 method_routes.setdefault(route.method, route)
         if method_routes:
-            allow_methods = var.allow_methods.init(self.request)
-            allow_headers = var.allow_headers.init(self.request)
-            route_var = var.unmatched_route.init(self.request)
+            allow_methods = var.allow_methods.setup(self.request)
+            allow_headers = var.allow_headers.setup(self.request)
+            route_var = var.unmatched_route.setup(self.request)
             allow_methods.set(list(method_routes))
             headers = []
             for route in method_routes.values():
                 distinct_add(headers, route.header_names)
             allow_headers.set(headers)
             route_var.set('')
             if self.request.method not in method_routes:
@@ -463,43 +500,45 @@
 
     def __call__(self):
         error_hooks = self._default_error_hooks
         try:
             with self._resolve() as route:
                 error_hooks = route.error_hooks
                 result = route(self)
-                if isinstance(result, Response):
-                    result.request = self.request
-                elif Response.is_cls(getattr(self.__class__, 'response', None)):
-                    result = self.response(result, request=self.request)
-                response = process_response(self, result)
         except Exception as e:
-            response = self._handle_error(Error(e), error_hooks)
-        return response
+            result = self._handle_error(Error(e), error_hooks)
+
+        if isinstance(result, Response):
+            if not result.request:
+                result.request = self.request
+        elif Response.is_cls(getattr(self.__class__, 'response', None)):
+            result = self.response(result, request=self.request)
+
+        return process_response(self, result)
 
     @awaitable(__call__)
     async def __call__(self):
         error_hooks = self._default_error_hooks
         try:
             # async with: no
             with self._resolve() as route:
                 error_hooks = route.error_hooks
                 result = await route(self)
-                if isinstance(result, Response):
-                    result.request = self.request
-                elif Response.is_cls(getattr(self.__class__, 'response', None)):
-                    result = self.response(result, request=self.request)
-                response = await process_response(self, result)
         except Exception as e:
-            response = await self._handle_error(Error(e), error_hooks)
-        return response
+            result = await self._handle_error(Error(e), error_hooks)
+        if isinstance(result, Response):
+            if not result.request:
+                result.request = self.request
+        elif Response.is_cls(getattr(self.__class__, 'response', None)):
+            result = self.response(result, request=self.request)
+        return await process_response(self, result)
 
     def options(self):
         return Response(headers={
-            Header.ALLOW: ','.join(set([m.upper() for m in var.allow_methods.get(self.request)])),
+            Header.ALLOW: ','.join(set([m.upper() for m in var.allow_methods.getter(self.request)])),
             Header.LENGTH: '0'
         })
 
     def __serve__(self, unit):
         if isinstance(unit, Endpoint):
             return unit.serve(self)
         else:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/decorator.py` & `utilmeta-2.5.2/utilmeta/core/api/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # bare route: only for API/Module
     # 'APIDecoratorWrapper',
     # 'APIGenerator',
     # hooks
     'before',
     'after',
     'handle',
-    'plugin'
+    'plugin',
 ]
 
 
 def set_hook(f, hook_type: str, value, priority: int = None):
     if not f:
         return f
     if not inspect.isfunction(f):
@@ -52,20 +52,19 @@
 
 def set_excludes(f, excludes):
     if not excludes:
         return f
     if hasattr(f, EndpointAttr.excludes):
         return
 
-    def proc(ex):
-        return ex if isinstance(ex, str) else ex.__name__
     if multi(excludes):
-        excludes = [proc(e) for e in excludes]
+        excludes = list(excludes)
     else:
-        excludes = [proc(excludes)]
+        excludes = [excludes]
+
     setattr(f, EndpointAttr.excludes, excludes)
     return f
 
 
 def get_hook_type(f):
     for t in HOOK_TYPES:
         if getattr(f, t, None):
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/endpoint.py` & `utilmeta-2.5.2/utilmeta/core/api/endpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from utilmeta import utils
 from utilmeta.utils import exceptions as exc
-from typing import Callable, Union, TYPE_CHECKING
+from typing import Callable, Union, Type, List, TYPE_CHECKING
 from utilmeta.utils.plugin import PluginTarget, PluginEvent
 from utilmeta.utils.error import Error
 from utilmeta.utils.context import ContextWrapper, Property
 from utype.parser.base import BaseParser
 from utype.parser.func import FunctionParser
 from utype.parser.field import ParserField
+from utype.parser.rule import LogicalType
 import inspect
 from ..request import Request, var
-from ..request.properties import QueryParam
+from ..request.properties import QueryParam, PathParam
 from ..response import Response
 import utype
 
 if TYPE_CHECKING:
     from .base import API
 
 process_request = PluginEvent('process_request', streamline_result=True)
@@ -46,34 +47,25 @@
         else:
             headers = getattr(prop, 'headers', None)
             if headers and utils.multi(headers):
                 utils.distinct_add(self.header_names, [str(v).lower() for v in headers])
         return prop.init(val)
 
 
-class Endpoint(PluginTarget):
-    @classmethod
-    def apply_for(cls, func):
-        _cls = getattr(func, 'cls', None)
-        if not _cls or not issubclass(_cls, Endpoint):
-            # override current class
-            _cls = cls
-
-        kwargs = {}
-        for key, val in inspect.signature(_cls).parameters.items():
-            v = getattr(func, key, None)
-            if v is None:
-                continue
-            # func properties override the default kwargs
-            kwargs[key] = v
-        return _cls(func, **kwargs)
-
+class BaseEndpoint(PluginTarget):
     parser_cls = FunctionParser
     wrapper_cls = RequestContextWrapper
 
+    PATH_REGEX = utils.PATH_REGEX
+    PARSE_PARAMS = False
+    # params is already parsed by the request parser
+    PARSE_RESULT = False
+    # result will be parsed in the end of endpoint.serve
+    STRICT_RESULT = False
+
     def __init__(self, f: Callable, *,
                  method: str,
                  plugins: list = None,
                  idempotent: bool = None,
                  eager: bool = False
                  ):
 
@@ -83,20 +75,42 @@
             raise TypeError(f'Invalid endpoint function: {f}')
 
         self.f = f
         self.method = method
         self.idempotent = idempotent
         self.eager = eager
         self.name = self.__name__ = f.__name__
-        self.wrapper = self.wrapper_cls(self.parser_cls.apply_for(f))
+        self.path_names = self.PATH_REGEX.findall(self.route)
+        self.wrapper = self.wrapper_cls(
+            self.parser_cls.apply_for(f),
+            default_properties={
+                key: PathParam for key in self.path_names
+            }
+        )
         self.executor = self.parser.wrap(
             eager_parse=self.eager,
-            parse_params=False,
-            parse_result=True
+            parse_params=self.PARSE_PARAMS,
+            parse_result=self.PARSE_RESULT
         )
+        self.response_types: List[Type[Response]] = self.parse_responses(self.parser.return_type)
+
+    @classmethod
+    def parse_responses(cls, return_type):
+        def is_response(r):
+            return inspect.isclass(r) and issubclass(r, Response)
+
+        if is_response(return_type):
+            return [return_type]
+        elif isinstance(return_type, LogicalType):
+            values = []
+            for origin in return_type.resolve_origins():
+                if is_response(origin):
+                    values.append(origin)
+            return values
+        return []
 
     def iter_plugins(self):
         for cls, plugin in self._plugins.items():
             yield plugin
 
     def getattr(self, name: str, default=None):
         return getattr(self.f, name, default)
@@ -117,85 +131,14 @@
     def route(self):
         return '' if self.is_method else self.getattr('route', self.name)
 
     @property
     def parser(self):
         return self.wrapper.parser
 
-    def serve(self, api: 'API'):
-        retry_index = 0
-        while True:
-            try:
-                api.request.adaptor.update_context(
-                    retry_index=retry_index,
-                    idempotent=self.idempotent
-                )
-                req = self.process_request(api.request)
-                if isinstance(req, Request):
-                    api.request = req
-                    args, kwargs = self.parse_request(api.request)
-                    enter_endpoint(self, api, *args, **kwargs)
-                    response = self(api, *args, **kwargs)
-                else:
-                    response = req
-                result = self.process_response(response)
-                if isinstance(result, Request):
-                    # need another loop
-                    api.request = result
-                else:
-                    response = result
-                    break
-            except Exception as e:
-                err = Error(e)
-                result = self.handle_error(api.request, err)
-                if isinstance(result, Request):
-                    api.request = result
-                else:
-                    response = result
-                    break
-            retry_index += 1
-        exit_endpoint(self, api)
-        return response
-
-    @utils.awaitable(serve)
-    async def serve(self, api: 'API'):
-        retry_index = 0
-        while True:
-            try:
-                api.request.adaptor.update_context(
-                    retry_index=retry_index,
-                    idempotent=self.idempotent
-                )
-                req = await self.process_request(api.request)
-                if isinstance(req, Request):
-                    api.request = req
-                    args, kwargs = await self.parse_request(api.request)
-                    await enter_endpoint(self, api, *args, **kwargs)
-                    response = await self(api, *args, **kwargs)
-                else:
-                    response = req
-                result = await self.process_response(response)
-                if isinstance(result, Request):
-                    # need another loop
-                    api.request = result
-                else:
-                    response = result
-                    break
-            except Exception as e:
-                err = Error(e)
-                result = await self.handle_error(api.request, err)
-                if isinstance(result, Request):
-                    api.request = result
-                else:
-                    response = result
-                    break
-            retry_index += 1
-        await exit_endpoint(self, api)
-        return response
-
     def process_request(self, request: Request) -> Union[Request, Response]:
         for handler in process_request.iter(self):
             try:
                 req = handler(request, self)
             except NotImplementedError:
                 continue
             if isinstance(req, Response):
@@ -283,14 +226,51 @@
                 # need to invoke another request
                 return res
             if isinstance(res, Response):
                 # only take value if return value is BaseResponse objects
                 return res
         raise e.throw()
 
+
+class Endpoint(BaseEndpoint):
+    @classmethod
+    def apply_for(cls, func: Callable, api: Type['API'] = None):
+        _cls = getattr(func, 'cls', None)
+        if not _cls or not issubclass(_cls, Endpoint):
+            # override current class
+            _cls = cls
+
+        kwargs = {}
+        for key, val in inspect.signature(_cls).parameters.items():
+            v = getattr(func, key, None)
+            if v is None:
+                continue
+            # func properties override the default kwargs
+            kwargs[key] = v
+        if api:
+            kwargs.update(api=api)
+        return _cls(func, **kwargs)
+
+    def __init__(self, f: Callable, *,
+                 api: Type['API'] = None,
+                 method: str,
+                 plugins: list = None,
+                 idempotent: bool = None,
+                 eager: bool = False
+                 ):
+
+        super().__init__(
+            f,
+            plugins=plugins,
+            method=method,
+            idempotent=idempotent,
+            eager=eager
+        )
+        self.api = api
+
     def __call__(self, *args, **kwargs):
         # with self:
         r = self.executor(*args, **kwargs)
         if inspect.isawaitable(r):
             raise exc.ServerError('awaitable detected in sync function')
         return r
 
@@ -299,31 +279,129 @@
         # async with self:
         r = self.executor(*args, **kwargs)
         while inspect.isawaitable(r):
             # executor is maybe a sync function, which will not need to await
             r = await r
         return r
 
+    @property
+    def ref(self) -> str:
+        if self.api:
+            return f'{self.api.__ref__}.{self.f.__name__}'
+        if self.module_name:
+            return f'{self.module_name}.{self.f.__name__}'
+        return self.f.__name__
+
+    def make_response(self, response, request, error=None):
+        if not self.response_types:
+            return response
+        if isinstance(response, Response):
+            return response
+        for i, resp_type in enumerate(self.response_types):
+            try:
+                return resp_type(response, request=request, error=error, strict=self.STRICT_RESULT)
+            except Exception as e:
+                if i == len(self.response_types) - 1:
+                    raise e
+                continue
+        return response
+
+    def serve(self, api: 'API'):
+        # ---
+        var.endpoint_ref.setter(api.request, self.ref)
+        # ---
+        retry_index = 0
+        err = None
+        while True:
+            try:
+                api.request.adaptor.update_context(
+                    retry_index=retry_index,
+                    idempotent=self.idempotent
+                )
+                req = self.process_request(api.request)
+                if isinstance(req, Request):
+                    api.request = req
+                    args, kwargs = self.parse_request(api.request)
+                    enter_endpoint(self, api, *args, **kwargs)
+                    response = self(api, *args, **kwargs)
+                else:
+                    response = req
+                result = self.process_response(response)
+                if isinstance(result, Request):
+                    # need another loop
+                    api.request = result
+                else:
+                    response = result
+                    break
+            except Exception as e:
+                err = Error(e)
+                result = self.handle_error(api.request, err)
+                if isinstance(result, Request):
+                    api.request = result
+                else:
+                    response = result
+                    break
+            retry_index += 1
+        exit_endpoint(self, api)
+        return self.make_response(response, request=api.request, error=err)
+
+    @utils.awaitable(serve)
+    async def serve(self, api: 'API'):
+        # ---
+        var.endpoint_ref.setter(api.request, self.ref)
+        # ---
+        retry_index = 0
+        err = None
+        while True:
+            try:
+                api.request.adaptor.update_context(
+                    retry_index=retry_index,
+                    idempotent=self.idempotent
+                )
+                req = await self.process_request(api.request)
+                if isinstance(req, Request):
+                    api.request = req
+                    args, kwargs = await self.parse_request(api.request)
+                    await enter_endpoint(self, api, *args, **kwargs)
+                    response = await self(api, *args, **kwargs)
+                else:
+                    response = req
+                result = await self.process_response(response)
+                if isinstance(result, Request):
+                    # need another loop
+                    api.request = result
+                else:
+                    response = result
+                    break
+            except Exception as e:
+                err = Error(e)
+                result = await self.handle_error(api.request, err)
+                if isinstance(result, Request):
+                    api.request = result
+                else:
+                    response = result
+                    break
+            retry_index += 1
+        await exit_endpoint(self, api)
+        return self.make_response(response, request=api.request, error=err)
+
     def parse_request(self, request: Request):
         try:
-            kwargs = dict(var.path_params.get(request))
+            kwargs = dict(var.path_params.getter(request))
             kwargs.update(self.wrapper.parse_context(request))
             return self.parser.parse_params((), kwargs, context=self.parser.options.make_context())
         except utype.exc.ParseError as e:
             raise exc.BadRequest(str(e), detail=e.get_detail()) from e
 
     @utils.awaitable(parse_request)
     async def parse_request(self, request: Request):
         try:
-            kwargs = dict(await var.path_params.get(request))
+            kwargs = dict(await var.path_params.getter(request))
             kwargs.update(await self.wrapper.parse_context(request))
             return self.parser.parse_params((), kwargs, context=self.parser.options.make_context())
             # in base Endpoint, args is not supported
         except utype.exc.ParseError as e:
             raise exc.BadRequest(str(e), detail=e.get_detail()) from e
 
-    def generate_call(self):
-        pass
-
 
 enter_endpoint.register(Endpoint)
 exit_endpoint.register(Endpoint)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/hook.py` & `utilmeta-2.5.2/utilmeta/core/api/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
             r = await r
         return r
 
 
 class BeforeHook(Hook):
     hook_type = utils.EndpointAttr.before_hook
     wrapper_cls = RequestContextWrapper
-    parse_params = True
+    # parse_params = False
+    # already pared for request
 
     @classmethod
     def apply_for(cls, func: Callable) -> 'BeforeHook':
         return cls(
             func,
             hook_targets=getattr(func, cls.hook_type),
             hook_excludes=getattr(func, utils.EndpointAttr.excludes, None),
@@ -118,24 +119,24 @@
             hook_excludes=hook_excludes,
             priority=priority,
         )
         self.wrapper = self.wrapper_cls(self.parser)
 
     def parse_request(self, request: Request):
         try:
-            kwargs = dict(var.path_params.get(request))
+            kwargs = dict(var.path_params.getter(request))
             kwargs.update(self.wrapper.parse_context(request))
             return self.parser.parse_params((), kwargs, context=self.parser.options.make_context())
         except utype.exc.ParseError as e:
             raise exceptions.BadRequest(str(e), detail=e.get_detail()) from e
 
     @utils.awaitable(parse_request)
     async def parse_request(self, request: Request):
         try:
-            kwargs = dict(await var.path_params.get(request))
+            kwargs = dict(await var.path_params.getter(request))
             kwargs.update(await self.wrapper.parse_context(request))
             return self.parser.parse_params((), kwargs, context=self.parser.options.make_context())
             # in base Endpoint, args is not supported
         except utype.exc.ParseError as e:
             raise exceptions.BadRequest(str(e), detail=e.get_detail()) from e
 
     def serve(self, api: 'API'):
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/route.py` & `utilmeta-2.5.2/utilmeta/core/api/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import re
 from typing import Union, Dict, Type, List, Optional, TYPE_CHECKING
-from utilmeta.utils import awaitable, get_doc, regular, duplicate, pop, distinct_add, multi
+from utilmeta.utils import awaitable, get_doc, regular, duplicate, pop, distinct_add, multi, PATH_REGEX
 
 import inspect
 from functools import partial
 from .endpoint import Endpoint
 from .hook import Hook, ErrorHook, BeforeHook, AfterHook
 from ..request import Request, var
 from utype.parser.field import Field
 
 if TYPE_CHECKING:
     from .base import API
 
 
 class APIRoute:
-    PATH_REGEX = re.compile("{([a-zA-Z][a-zA-Z0-9_]*)}")
+    PATH_REGEX = PATH_REGEX
     DEFAULT_PATH_REGEX = '[^/]+'
 
     def __init__(self,
                  handler: Union[Type['API'], Endpoint],
                  route: Union[str, tuple],
                  name: str,
                  parent: Type['API'] = None,
@@ -232,16 +232,16 @@
 
         return property(getter)
 
     def match_route(self, request: Request):
         # /doc/{page}
         # /user/* -> UserAPI
         # /http/bin/* -> HttpBinAPI
-        route_attr = var.unmatched_route.init(request)
-        path_params_attr = var.path_params.init(request)
+        route_attr = var.unmatched_route.setup(request)
+        path_params_attr = var.path_params.setup(request)
         route = route_attr.get()
         path_params: dict = path_params_attr.get()
         for regex in self.regex_list:
             match = regex.fullmatch(route)
             if match:
                 group: dict = match.groupdict()
                 if not self.method:
@@ -251,14 +251,17 @@
                 # set path params for endpoint and API in every match
                 path_params.update(group)
                 path_params_attr.set(path_params)
                 return True
         return False
 
     def match_targets(self, targets: list):
+        if self.route in targets:
+            # str
+            return True
         if isinstance(self.handler, Endpoint):
             return self.handler in targets or self.handler.f in targets
         # otherwise, we only accept the
         # route: someAPI = api(...)(someAPI)
         return self.handler in targets
 
     def match_hook(self, hook: Hook):
@@ -291,14 +294,21 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
         # exit_route(self, exc_type, exc_val, exc_tb)
 
     def __call__(self, api: 'API'):
+        # ---
+        names_var = var.operation_names.setup(api.request)
+        names = names_var.get() or []
+        names.append(self.name)
+        names_var.set(names)
+        # ---
+
         if api.request.is_options:
             if self.is_endpoint:
                 # headers template is dict, while parser.headers can be schema class
                 # api.request.allow_headers += tuple(self.handler.parser.headers_template)
                 return api.options()
         else:
             # execute before hooks only if request method is not OPTIONS
@@ -311,14 +321,21 @@
             result = hook(api, result) or result
             result = hook.process_result(result)
 
         return result
 
     @awaitable(__call__)
     async def __call__(self, api: 'API'):
+        # ---
+        names_var = var.operation_names.setup(api.request)
+        names = await names_var.get() or []
+        names.append(self.name)
+        names_var.set(names)
+        # ---
+
         if api.request.is_options:
             if self.is_endpoint:
                 # headers template is dict, while parser.headers can be schema class
                 # TODO: allow headers
                 # api.request.allow_headers += tuple(self.handler.parser.headers_template)
                 return api.options()
         else:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/plugins/cors.py` & `utilmeta-2.5.2/utilmeta/core/api/plugins/cors.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,24 +104,24 @@
             return response
         if response.status in self.exclude_statuses:
             return response
         if self.cors_required(request):
             response.update_headers(**{
                 Header.ALLOW_ORIGIN: request.origin or '*',
                 Header.ALLOW_CREDENTIALS: 'true',
-                Header.ALLOW_METHODS: ','.join(set([m.upper() for m in var.allow_methods.get(request)])),
+                Header.ALLOW_METHODS: ','.join(set([m.upper() for m in var.allow_methods.getter(request)])),
             })
             if request.is_options:
                 if self.allow_headers == '*':
                     response.set_header(Header.ALLOW_HEADERS, '*')
                 else:
                     # request_headers = [h.strip().lower() for h in
                     #                    request.headers.get(Header.OPTIONS_HEADERS, '').split(',')]
                     allow_headers = list(self.allow_headers or [])
-                    allow_headers.extend([h.lower() for h in var.allow_headers.get(request)])
+                    allow_headers.extend([h.lower() for h in var.allow_headers.getter(request)])
                     if allow_headers:
                         response.set_header(Header.ALLOW_HEADERS, ','.join(allow_headers))
 
             if self.expose_headers:
                 response.set_header(Header.EXPOSE_HEADERS, ','.join(set([h.lower() for h in self.expose_headers])))
             if self.cors_max_age:
                 response.set_header(Header.ACCESS_MAX_AGE, self.cors_max_age)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/plugins/rate.py` & `utilmeta-2.5.2/utilmeta/core/api/plugins/rate.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/api/plugins/retry.py` & `utilmeta-2.5.2/utilmeta/core/api/plugins/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,19 @@
                 if multi(timeout):
                     timeout = timeout[min(len(timeout) - 1, current_retry)]
                 timeout = get_interval(timeout, null=True)
                 if timeout:
                     if self.retry_delta_ratio:
                         timeout = timeout + (random.random() * 2 - 1) * self.retry_delta_ratio * timeout
 
-                request.set_timeout(timeout)
+                request.adaptor.update_context(timeout=timeout)
 
-            if not request.timeout or request.timeout > delta:
-                request.set_timeout(delta)
+            to = request.adaptor.get_context('timeout')
+            if not to or to > delta:
+                request.adaptor.update_context(timeout=delta)
 
     def process_response(self, response: Response, api):
         request = response.request
         if not request:
             return response
         current_retry = request.get_context('retry_index') or 0
         if current_retry + 1 >= self.max_retries:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/api/specs/openapi.py` & `utilmeta-2.5.2/utilmeta/core/api/specs/openapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from utilmeta.utils.context import Property, ParserProperty
 from utilmeta.utils.constant import HAS_BODY_METHODS
 from utype import Schema, Field, JsonSchemaGenerator
 from utype.parser.field import ParserField
 from utype.parser.rule import LogicalType
 from utype.utils.datastructures import unprovided
 from utype.utils.functional import get_obj_name
-from typing import Type, Tuple, Dict, List, TYPE_CHECKING
+from typing import Type, Tuple, Dict, List, TYPE_CHECKING, Optional
 from .base import BaseAPISpec
 import os
 import json
 
 if TYPE_CHECKING:
     from utilmeta import UtilMeta
 
@@ -66,46 +66,54 @@
 
     def generate_for_response(self, response: Type[Response]):
         parser = getattr(response, '__parser__', None)
         result_field = parser.get_field('result') if parser else None
         headers_field = parser.get_field('headers') if parser else None
 
         result_schema = self.generate_for_field(result_field) if result_field else None
-
-        headers_schema = self.generate_for_type(headers_field.type) \
+        headers_schema = self.__class__(headers_field.type, output=True)() \
             if headers_field and headers_field.type != Headers else {}
-        headers = headers_schema.get('properties') or {}
+        # headers is different, doesn't need to generate $ref
+
+        headers_props = headers_schema.get('properties') or {}
+        headers_required = headers_schema.get('required') or []
+        headers = {}
+        for key, val_schema in headers_props.items():
+            headers[key] = {
+                'schema': val_schema,
+                'required': key in headers_required
+            }
 
         content_type = response.content_type
         # todo: headers wrapped
         if response.wrapped:
             props = {}
             if response.result_key:
                 props[response.result_key] = result_schema
             if response.message_key:
                 msg = dict(self.generate_for_type(str))
                 msg.update(
                     title='Message',
                     description='an error message of response',
                 )
                 props[response.message_key] = msg
+            if response.state_key:
+                state = dict(self.generate_for_type(str))
+                state.update(
+                    title='State',
+                    description='action state code of response',
+                )
+                props[response.state_key] = state
             if response.count_key:
                 cnt = dict(self.generate_for_type(int))
                 cnt.update(
                     title='Count',
                     description='a count of the total number of query result',
                 )
                 props[response.count_key] = cnt
-            if response.state_key:
-                state = dict(self.generate_for_type(str))
-                state.update(
-                    title='State',
-                    description='action state code of response',
-                )
-                props[response.count_key] = state
 
             data_schema = {
                 'type': 'object',
                 'properties': props,
                 'required': list(props)
             }
             content_type = JSON
@@ -226,22 +234,22 @@
             import yaml     # requires pyyaml
             return yaml.dump(schema)
 
         else:
             raise ValueError(f'format: {repr(format)} not supported')
 
     @classmethod
-    def as_api(cls, path: str = None):
+    def as_api(cls, path: str = None, private: bool = True):
         from utilmeta.core import api
 
         # if path is not specified, use local mem instead
         class OpenAPI_API(API):
             response = Response
 
-            @api.get(private=True)
+            @api.get(private=private)
             def get(self):
                 from utilmeta import service
 
                 # if path:
                 #     file_path = os.path.join(service.project_dir, path)
                 #     if os.path.exists(file_path):
                 #         return self.response(file=open(file_path, 'r'))
@@ -334,14 +342,19 @@
         if response in self.responses:
             return name
 
         gen = self.get_generator(response, output=True)
         data = gen.generate_for_response(response)
 
         while name in self.response_names:
+            resp = self.response_names.get(name)
+            resp_data = self.responses.get(resp)
+            if resp_data and str(resp_data) == str(data):
+                # exact data
+                return name
             # de-duplicate name
             name += '_1'
 
         self.responses[response] = data
         self.response_names[name] = response
         return name
 
@@ -396,18 +409,21 @@
                         body_params_required.append(key)
                     body_params[key] = generator.generate_for_field(field)
                 elif _in in self.PARAMS_IN:
                     data = {
                         'in': _in,
                         'name': key,
                         'required': prop.required,
-                        'description': prop.description,
-                        'deprecated': prop.deprecated,
                         'schema': generator(),
                     }
+                    if prop.description:
+                        data['description'] = prop.description
+                    if prop.deprecated:
+                        data['deprecated'] = True
+
                     if isinstance(field.field, properties.RequestParam):
                         if field.field.style:
                             data.update(style=field.field.style)
                     if not unprovided(field.field.example):
                         data.update(example=field.field.example)
                     params[key] = data
 
@@ -479,14 +495,20 @@
         operation_names = list(tags) + [endpoint.name]
         operation_id = '_'.join(operation_names)
 
         params, body, requires = self.parse_properties(endpoint.wrapper.properties)
         responses = dict(extra_responses or {})
 
         rt = endpoint.parser.return_type
+        # if isinstance(rt, LogicalType):
+        #     # resolve multiple responses
+        #     if inspect.isclass(rt) and issubclass(rt, Rule):
+        #         pass
+        #
+        # else:
         if inspect.isclass(rt) and issubclass(rt, Response):
             resp = rt
         elif rt is not None:
             resp = (response_cls or Response)[rt]
         else:
             resp = response_cls or Response
 
@@ -508,14 +530,18 @@
             responses=responses,
             security=self.merge_requires(extra_requires, requires)
         )
         if params:
             operation.update(parameters=list(params.values()))
         if body and endpoint.method in HAS_BODY_METHODS:
             operation.update(requestBody=body)
+        if endpoint.idempotent is not None:
+            operation.update({'x-idempotent': endpoint.idempotent})
+        if endpoint.ref:
+            operation.update({'x-ref': endpoint.ref})
         return operation
 
     def from_route(self, route: APIRoute,
                    *routes: str,
                    tags: list = (),
                    params: dict = None,
                    response_cls: Type[Response] = None,
@@ -595,15 +621,18 @@
         return path_data
 
     def from_api(self, api: Type[API], *routes,
                  tags: list = (),
                  params: dict = None,
                  response_cls: Type[Response] = None,
                  responses: dict = None,
-                 requires: list = None) -> dict:
+                 requires: list = None) -> Optional[dict]:
+        if api.__external__:
+            # external APIs will not participate in docs
+            return None
         core_data = None
         extra_params = dict(params or {})
         prop_params, body, prop_requires = self.parse_properties(api._properties)
         extra_params.update(prop_params)
 
         response_cls = getattr(api, 'response', response_cls)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/basic.py` & `utilmeta-2.5.2/utilmeta/core/auth/basic.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/jwt.py` & `utilmeta-2.5.2/utilmeta/core/auth/jwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.user_token_field = user_token_field
 
     def apply_user_model(self, user_model: ModelAdaptor):
         if self.user_token_field and not isinstance(self.user_token_field, str):
             self.user_token_field = user_model.field_adaptor_cls(self.user_token_field).name
 
     def login(self, request: Request, key: str = 'uid', expiry_age: int = None):
-        user = var.user.get(request)
+        user = var.user.getter(request)
         if not user:
             return
         import time
         from utilmeta import service
         iat = time.time()
         inv = expiry_age
         token_dict = {
@@ -92,15 +92,15 @@
         except ImportError:
             # jwt 1.7
             import jwt  # noqa
             jwt_token = jwt.encode(  # noqa
                 token_dict, self.secret_key,
                 algorithm=self.algorithm
             ).decode('ascii')
-        self.jwt_var.set(request, jwt_token)
+        self.jwt_var.setter(request, jwt_token)
         return {self.user_token_field: jwt_token} if isinstance(self.user_token_field, str) else None
         # if conf.jwt_token_field:
         #     setattr(user, conf.jwt_token_field, jwt_token)
         #     user.save(update_fields=[conf.jwt_token_field])
         # request.jwt_token = jwt_token
         # return jwt_token
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/oauth2.py` & `utilmeta-2.5.2/utilmeta/core/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/properties.py` & `utilmeta-2.5.2/utilmeta/core/auth/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,77 +15,83 @@
     DEFAULT_ID_CONTEXT_VAR = var.user_id
     DEFAULT_SCOPES_CONTEXT_VAR = var.scopes
 
     # must be awaitable ----
     def get_user_id(self, request: Request) -> Union[str, int, Any]:
         data: Mapping = self.authentication.getter(request) or {}
         if isinstance(data, Mapping):
-            return data.get(self.key)
-        return data
+            user_id = data.get(self.key)
+        else:
+            user_id = data
+        self.id_context_var.setter(request, user_id)
+        return user_id
 
     @awaitable(get_user_id)
     async def get_user_id(self, request: Request) -> Union[str, int, Any]:
         r = self.authentication.getter(request)
         if inspect.isawaitable(r):
             r = await r
         data: Mapping = r or {}
         if isinstance(data, Mapping):
-            return data.get(self.key)
-        return data
+            user_id = data.get(self.key)
+        else:
+            user_id = data
+        self.id_context_var.setter(request, user_id)
+        return user_id
 
     def get_user(self, request: Request):
         user_id = self.get_user_id(request)
         if user_id is not None and self.user_model:
             inst = self.query_user(**{self.field: user_id})
             if inst is not None:
                 # user.set(inst)
                 if self.scopes_field:
-                    self.scopes_context_var.set(request, getattr(inst, self.scopes_field, []))
+                    self.scopes_context_var.setter(request, getattr(inst, self.scopes_field, []))
+                self.context_var.setter(request, inst)
                 return inst
         return None
 
     @awaitable(get_user)
     async def get_user(self, request: Request):
         user_id = await self.get_user_id(request)
         if user_id is not None and self.user_model:
             inst = await self.aquery_user(**{self.field: user_id})
             if inst is not None:
                 # user.set(inst)
                 if self.scopes_field:
-                    self.scopes_context_var.set(request, getattr(inst, self.scopes_field, []))
+                    self.scopes_context_var.setter(request, getattr(inst, self.scopes_field, []))
+                self.context_var.setter(request, inst)
                 return inst
         return None
 
     def getter(self, request: Request, field: ParserField = None):
-        user_var = self.context_var.init(request)
+        user_var = self.context_var.setup(request)
         # even if we registered factory
         # we still need to cache here
         # because parse_context will directly call getter
         if user_var.contains():
             # already cached
             return user_var.get()
         user = self.get_user(request)
-        user_var.set(user)
         if not user:
             if field and type(None) in field.input_origins:
                 return None
             if self.required:
                 raise exc.Unauthorized
             return unprovided
         return user
 
     @awaitable(getter)
     async def getter(self, request: Request, field: ParserField = None):
-        user_var = self.context_var.init(request)
+        user_var = self.context_var.setup(request)
         if user_var.contains():
             # already cached
             # use await in async context
             return await user_var.get()
         user = await self.get_user(request)
-        user_var.set(user)
         if not user:
             if field and type(None) in field.input_origins:
                 return None
             if self.required:
                 raise exc.Unauthorized
             return unprovided
         return user
@@ -191,15 +197,15 @@
             if inst is not None:
                 return inst
         return None
 
     # @awaitable(query_user)
     async def aquery_user(self, q=None, **kwargs):
         if self.user_model:
-            inst = await self.user_model.get_instance(q, **kwargs)
+            inst = await self.user_model.aget_instance(q, **kwargs)
             if inst is not None:
                 return inst
         return None
 
     def query_login_user(self, ident: str):
         if self.login_fields:
             if len(self.login_fields) == 1:
@@ -243,29 +249,29 @@
         encoded_password = getattr(user, self.password_field)
         if not self.check_password(password, encoded_password):
             return None
         await self.alogin_user(request, user, expiry_age=expiry_age)
         return user
 
     def login_user(self, request: Request, user, expiry_age: int = None, ignore_updates: bool = False) -> None:
-        self.context_var.set(request, user)
-        self.id_context_var.set(request, getattr(user, 'pk', None) or getattr(user, 'id', None))
+        self.context_var.setter(request, user)
+        self.id_context_var.setter(request, getattr(user, 'pk', None) or getattr(user, 'id', None))
         try:
             data = self.authentication.login(request, self.key, expiry_age)
         except NotImplementedError:
             data = None
         # cls.update_fields(request, user=user)
         # rotate_token(request.get_original_request())  # reset CSRF token for security purposes
         if not ignore_updates:
             self.update_fields(request, user, data)
 
     # @awaitable(login_user)
     async def alogin_user(self, request: Request, user, expiry_age: int = None, ignore_updates: bool = False) -> None:
-        self.context_var.set(request, user)
-        self.id_context_var.set(request, getattr(user, 'pk', None) or getattr(user, 'id', None))
+        self.context_var.setter(request, user)
+        self.id_context_var.setter(request, getattr(user, 'pk', None) or getattr(user, 'id', None))
         try:
             data = self.authentication.login(request, self.key, expiry_age)
             if inspect.isawaitable(data):
                 data = await data
         except NotImplementedError:
             data = None
         if not ignore_updates:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/signature.py` & `utilmeta-2.5.2/utilmeta/core/auth/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             if access:
                 return access
         return None
 
     @awaitable(get_access_instance)
     async def get_access_instance(self, access_key: str):
         for model in self.access_models:
-            access = await model.get_instance(**{self.access_key_field: access_key})
+            access = await model.aget_instance(**{self.access_key_field: access_key})
             if access:
                 return access
         return None
 
     def openapi_scheme(self) -> dict:
         # return dict(
         #     type='apikey',
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/plugins/require.py` & `utilmeta-2.5.2/utilmeta/core/auth/plugins/require.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,66 +27,67 @@
         self.scopes = [s for s in scope_or_fns if isinstance(s, str)]
         self.functions = [f for f in scope_or_fns if callable(f)]
         super().__init__(scopes=self.scopes, functions=self.functions, name=name)
         if not scope_or_fns:
             self.functions = [self.login]
             name = name or 'login'
         self.name = name
+        # self.readonly = readonly
         # self.login = login
 
     def enter_endpoint(self, api: 'API', *args, **kwargs):
         if self.functions:
             self.validate_functions(api)
         if self.scopes:
             self.validate_scopes(api)
 
     @awaitable(enter_endpoint)
     async def enter_endpoint(self, api: 'API', *args, **kwargs):
         if self.functions:
             await self.validate_functions(api)
         if self.scopes:
-            await self.validate_scopes(api)
+            self.validate_scopes(api)
 
     def validate_scopes(self, api: 'API'):
-        scopes = self.scopes_var.get(api.request)
+        scopes = self.scopes_var.getter(api.request)
         if not set(scopes or []).issuperset(self.scopes):
             raise exceptions.PermissionDenied(
                 'insufficient scope',
-                scopes=scopes,
-                required_scopes=self.scopes,
+                scope=scopes,
+                required_scope=self.scopes,
                 name=self.name
             )
 
-    @awaitable
-    async def validate_scopes(self, api: 'API'):
-        scopes = await self.scopes_var.get(api.request)
-        if not set(scopes or []).issuperset(self.scopes):
-            raise exceptions.PermissionDenied(
-                'insufficient scope',
-                scopes=scopes,
-                required_scopes=self.scopes,
-                name=self.name
-            )
+    # @awaitable
+    # async def validate_scopes(self, api: 'API'):
+    #     scopes = await self.scopes_var.getter(api.request)
+    #     if not set(scopes or []).issuperset(self.scopes):
+    #         raise exceptions.PermissionDenied(
+    #             'insufficient scope',
+    #             scopes=scopes,
+    #             required_scopes=self.scopes,
+    #             name=self.name
+    #         )
 
     def validate_functions(self, api: 'API'):
-        user = self.user_var.get(api.request)
+        user = self.user_var.getter(api.request)
         if user is None:
             pass
         for func in self.functions:
             func: Callable
             v = func(user)
             if not v:
                 raise exceptions.PermissionDenied(
                     f'{self.name or "permission"} required',
                     name=self.name
                 )
 
     @awaitable(validate_functions)
     async def validate_functions(self, api: 'API'):
-        user = await self.user_var.get(api.request)
+        user = await self.user_var.getter(api.request)
         if user is None:
             pass
         for func in self.functions:
             func: Callable
             v = func(user)
             if inspect.isawaitable(v):
                 v = await v
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/session/base.py` & `utilmeta-2.5.2/utilmeta/core/auth/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         #     return None
         # inst = self.engine(session_key)
         # req_session.set(inst)
         # guarantee there are only one session in a request
         return (engine or self.engine)(session_key)
 
     def getter(self, request: Request, field: ParserField = None):
-        cvar = self.context_var.init(request)
+        cvar = self.context_var.setup(request)
         if cvar.contains():
             return cvar.get()
         engine = None
         if field:
             # maybe a field has its own session schema as engine
             engine = self.get_engine(field)
         session = self.get_session(request, engine)
@@ -114,15 +114,15 @@
 
     def process_response(self, response: Response):
         """
         write based on django session middleware
         you can override
         """
         request = response.request
-        cvar = self.context_var.init(request)
+        cvar = self.context_var.setup(request)
         if not cvar.contains():
             # no session initialized
             return response
         if not isinstance(response, Response):
             response = Response(response)
         session = cvar.get()
         if session is None:
@@ -135,15 +135,15 @@
         else:
             self.save_session(response, session)
         return response
 
     @awaitable(process_response)
     async def process_response(self, response: Response):
         request = response.request
-        cvar = self.context_var.init(request)
+        cvar = self.context_var.setup(request)
         if not cvar.contains():
             # no session initialized
             return response
         if not isinstance(response, Response):
             response = Response(response)
         session = await cvar.get()
         if session is None:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/session/cache.py` & `utilmeta-2.5.2/utilmeta/core/auth/session/cache.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/session/cached_db.py` & `utilmeta-2.5.2/utilmeta/core/auth/session/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,191 +1,188 @@
-# from utilmeta.utils import awaitable
-from .cache import CacheSessionSchema, CacheSession
-from .db import DBSessionSchema
-
-__all__ = ['CachedDBSessionSchema', 'CachedDBSession']
-
-
-# class AbstractCachedDBSessionSchema(CacheSessionSchema):
-#     _config: 'CachedDBSession'
-#
-#     def db_exists(self, session_key: str) -> bool:
-#         raise NotImplementedError
-#
-#     # @awaitable(db_exists)
-#     async def adb_exists(self, session_key: str) -> bool:
-#         raise NotImplementedError
-#
-#     def exists(self, session_key: str) -> bool:
-#         if not session_key:
-#             return False
-#         try:
-#             return super().exists(session_key)
-#         except Exception:
-#             return self.db_exists(session_key)
-#
-#     # @awaitable(exists)
-#     async def aexists(self, session_key: str) -> bool:
-#         if not session_key:
-#             return False
-#         try:
-#             return await super().aexists(session_key)
-#         except Exception:
-#             return await self.adb_exists(session_key)
-#
-#     def db_save(self, must_create=False) -> bool:
-#         raise NotImplementedError
-#
-#     async def adb_save(self, must_create=False) -> bool:
-#         raise NotImplementedError
-#
-#     def save(self, must_create: bool = False):
-#         if self.db_save(must_create):
-#             # skip cache
-#             return
-#         try:
-#             super().save(must_create)
-#         except Exception as e:
-#             print(f'Save with error: {e}')
-#             # ignore cache failed
-#
-#     async def asave(self, must_create: bool = False):
-#         if await self.adb_save(must_create):
-#             # skip cache
-#             return
-#         try:
-#             await super().asave(must_create)
-#         except Exception as e:
-#             print(f'Save with error: {e}')
-#             # ignore cache failed
-#
-#     def db_delete(self, session_key: str) -> bool:
-#         raise NotImplementedError
-#
-#     async def adb_delete(self, session_key: str) -> bool:
-#         raise NotImplementedError
-#
-#     def delete(self, session_key: str = None):
-#         if self.db_delete(session_key):
-#             return
-#         try:
-#             super().delete(session_key)
-#         except Exception as e:
-#             print(f'Delete with error: {e}')
-#             # ignore cache failed
-#
-#     # @awaitable(delete)
-#     async def adelete(self, session_key: str = None):
-#         if await self.adb_delete(session_key):
-#             return
-#         try:
-#             await super().adelete(session_key)
-#         except Exception as e:
-#             print(f'Delete with error: {e}')
-#             # ignore cache failed
+import inspect
 
+from .schema import BaseSessionSchema, SchemaSession, SessionCreateError
+from typing import Type, TYPE_CHECKING
+from utilmeta.utils import time_now
+from datetime import timedelta
+from utype import Field
+from utilmeta.core.orm import ModelAdaptor
+
+if TYPE_CHECKING:
+    from utilmeta.core.orm.backends.django.models import AbstractSession
+
+
+class DBSessionSchema(BaseSessionSchema):
+    _config: 'DBSession'
+    # SESSION_ID_KEY: ClassVar = '$session_id'
+    # CLIENT_IP_KEY: ClassVar = '$client_ip'
+    # CLIENT_UA_KEY: ClassVar = '$client_ua'
+
+    @property
+    def _model_cls(self):
+        return self._config.session_model
 
-class CachedDBSessionSchema(CacheSessionSchema, DBSessionSchema):
-    def exists(self, session_key: str) -> bool:
+    def db_exists(self, session_key: str) -> bool:
         if not session_key:
             return False
-        try:
-            return super().exists(session_key)
-        except Exception:
-            return self.db_exists(session_key)
+        return self._model_cls.get_queryset(session_key=session_key).exists()
 
-    async def aexists(self, session_key: str) -> bool:
+    # @awaitable(exists)
+    async def adb_exists(self, session_key: str) -> bool:
         if not session_key:
             return False
-        try:
-            return await super().aexists(session_key)
-        except Exception:
-            return await self.adb_exists(session_key)
+        return await self._model_cls.get_queryset(session_key=session_key).aexists()
 
-    def save(self, must_create: bool = False):
-        if self.db_save(must_create):
-            # skip cache
+    def exists(self, session_key: str) -> bool:
+        return self.db_exists(session_key)
+
+    # @awaitable(exists)
+    async def aexists(self, session_key: str) -> bool:
+        return await self.adb_exists(session_key)
+
+    def create(self):
+        self._session_key = self._get_new_session_key()
+        try:
+            self.save(must_create=True)
+        except SessionCreateError:
             return
+        self._modified = True
+        return
+
+    # @awaitable(create)
+    async def acreate(self):
+        self._session_key = await self._aget_new_session_key()
         try:
-            super().save(must_create)
-        except Exception as e:
-            print(f'Save with error: {e}')
-            # ignore cache failed
+            await self.asave(must_create=True)
+        except SessionCreateError:
+            return
+        self._modified = True
+        return
 
+    @property
+    @Field(no_output=True)
+    def timeout(self) -> int:
+        # if expiry_age=0 (at browser close), still means a not clear timeout
+        return self.expiry_age or self._config.cookie.age
+
+    def get_session_data(self):
+        return dict(
+            session_key=self.session_key,
+            encoded_data=self.encode(dict(self)),
+            expiry_time=time_now() + timedelta(seconds=self.timeout),
+            last_activity=time_now(),
+            created_time=self._request.time if self._request else time_now()
+        )
+
+    def load_object(self, must_create: bool = False):
+        """
+        To be inherit
+        """
+        session_id = None
+        if not self.session_key:
+            self._session_key = self._get_new_session_key()
+        elif not must_create:
+            obj = self._model_cls.get_instance(session_key=self.session_key)
+            session_id = obj.pk if obj else None
+        return self._model_cls.init_instance(
+            id=session_id,
+            **self.get_session_data()
+        )
+
+    async def aload_object(self, must_create: bool = False):
+        """
+        To be inherit
+        """
+        session_id = None
+        if not self.session_key:
+            self._session_key = await self._aget_new_session_key()
+        elif not must_create:
+            obj = await self._model_cls.aget_instance(session_key=self.session_key)
+            session_id = obj.pk if obj else None
+        data = self.get_session_data()
+        if inspect.isawaitable(data):
+            data = await data
+        return self._model_cls.init_instance(
+            id=session_id,
+            **data
+        )
+
+    def db_save(self, must_create=False, force: bool = True):
+        if self.session_key is None:
+            return self.create()
+        obj = self.load_object(must_create)
+        obj.save(force_insert=must_create, force_update=not must_create and force)
+
+    # @awaitable(db_save)
+    async def adb_save(self, must_create=False, force: bool = True):
+        if self.session_key is None:
+            return await self.acreate()
+        obj = await self.aload_object(must_create)
+        await obj.asave(force_insert=must_create, force_update=not must_create and force)
+
+    def save(self, must_create: bool = False):
+        return self.db_save(must_create)
+
+    # @awaitable(save)
     async def asave(self, must_create: bool = False):
-        if await self.adb_save(must_create):
-            # skip cache
-            return
-        try:
-            await super().asave(must_create)
-        except Exception as e:
-            print(f'Save with error: {e}')
-            # ignore cache failed
+        return await self.adb_save(must_create)
+
+    def db_delete(self, session_key=None):
+        if session_key is None:
+            if self.session_key is None:
+                return
+            session_key = self.session_key
+        self._model_cls.get_queryset(
+            session_key=session_key,
+            deleted_time=None
+        ).update(deleted_time=time_now())
+
+    # @awaitable(db_delete)
+    async def adb_delete(self, session_key=None):
+        if session_key is None:
+            if self.session_key is None:
+                return
+            session_key = self.session_key
+        await self._model_cls.get_queryset(
+            session_key=session_key,
+            deleted_time=None
+        ).aupdate(deleted_time=time_now())
 
     def delete(self, session_key: str = None):
-        if self.db_delete(session_key):
-            return
-        try:
-            super().delete(session_key)
-        except Exception as e:
-            print(f'Delete with error: {e}')
-            # ignore cache failed
+        return self.db_delete(session_key)
 
     # @awaitable(delete)
     async def adelete(self, session_key: str = None):
-        if await self.adb_delete(session_key):
-            return
-        try:
-            await super().adelete(session_key)
-        except Exception as e:
-            print(f'Delete with error: {e}')
-            # ignore cache failed
+        return await self.adb_delete(session_key)
 
-    def load_data(self):
+    def load(self):
         if not self._session_key:
             return None
         # to be inherited
-        session = self._model_cls.filter(
-            session_key=self._session_key
-        ).first()
+        session = self._model_cls.get_instance(
+            session_key=self._session_key,
+            deleted_time=None,
+        )
         if session:
-            try:
-                self.get_cache().set(
-                    self.get_key(),
-                    session.encoded_data,
-                    timeout=self.timeout,
-                )
-            except Exception as e:
-                print(f'Sync to cache failed: {e}')
-                # ignore
             return self.decode(session.encoded_data)
         return None
 
-    async def aload_data(self):
-        # to be inherited
+    async def aload(self):
         if not self._session_key:
             return None
         # to be inherited
-        session = await self._model_cls.filter(
-            session_key=self._session_key
-        ).afirst()
+        session = await self._model_cls.aget_instance(
+            session_key=self._session_key,
+            deleted_time=None
+        )
         if session:
-            try:
-                await self.get_cache().set(
-                    self.get_key(),
-                    session.encoded_data,
-                    timeout=self.timeout,
-                )
-            except Exception as e:
-                print(f'Sync to cache failed: {e}')
-                # ignore
             return self.decode(session.encoded_data)
         return None
 
 
-class CachedDBSession(CacheSession):
-    DEFAULT_ENGINE = CachedDBSessionSchema
-    schema = CachedDBSessionSchema
+class DBSession(SchemaSession):
+    DEFAULT_ENGINE = DBSessionSchema
+    schema = DBSessionSchema
 
-    def __init__(self, session_model, **kwargs):
+    def __init__(self, session_model: Type['AbstractSession'], **kwargs):
         super().__init__(**kwargs)
-        self.session_model = session_model
+        self.session_model = ModelAdaptor.dispatch(session_model)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/session/django.py` & `utilmeta-2.5.2/utilmeta/core/auth/session/django.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             'SESSION_ENGINE': self.engine,
             'SESSION_EXPIRE_AT_BROWSER_CLOSE': self.expire_at_browser_close,
             'SESSION_FILE_PATH': self.file_path,
             **self.cookie.as_django(prefix='SESSION')
         }
 
     def login(self, request, key: str, expiry_age: int = None, user_id_var=var.user_id):
-        new_user_id = user_id_var.get(request)
+        new_user_id = user_id_var.getter(request)
         if new_user_id is None:
             return
         session: SessionBase = self.getter(request)
         if not session:
             return
         user_id = session.get(key)
         if user_id is None:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/auth/session/schema.py` & `utilmeta-2.5.2/utilmeta/core/auth/session/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from utype.utils.encode import JSONSerializer
 from utype.utils.datastructures import unprovided
 from utype import Schema, Field, Options
 from utilmeta.utils import awaitable, gen_key, time_now, http_time
-import inspect
-from datetime import timedelta, datetime
+from datetime import timedelta, datetime, timezone
 from typing import Optional, TypeVar, Type, ClassVar, TYPE_CHECKING
 import warnings
 from .base import BaseSession
 from utilmeta.core.request import var, Request
 from utilmeta.core.response import Response
 
 if TYPE_CHECKING:
     from utilmeta.core.request import Request
 
 T = TypeVar('T')
+EPOCH = datetime(1970, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
 
 
 class SessionError(Exception):
     pass
 
 
 class SessionCreateError(SessionError):
@@ -94,15 +94,15 @@
         return self
 
     @classmethod
     def init(cls: Type[T], request: Request, config: 'SchemaSession') -> T:
         # for developer to directly call
         if not isinstance(config, SchemaSession):
             raise TypeError(f'Invalid session config: {config}')
-        cvar = config.context_var.init(request)
+        cvar = config.context_var.setup(request)
         if cvar.contains():
             data: BaseSessionSchema = cvar.get()
             if not isinstance(data, cls):
                 self = cls(**data)
                 self._session_key = data.session_key
                 self._config = config
                 self._request = request
@@ -119,15 +119,15 @@
         cvar.set(session)
         return session
 
     @classmethod
     async def ainit(cls: Type[T], request: Request, config: 'SchemaSession') -> T:
         if not isinstance(config, SchemaSession):
             raise TypeError(f'Invalid session config: {config}')
-        cvar = config.context_var.init(request)
+        cvar = config.context_var.setup(request)
         if cvar.contains():
             data: BaseSessionSchema = await cvar.get()
             if not isinstance(data, cls):
                 self = cls(**data)
                 self._session_key = data.session_key
                 self._config = config
                 self._request = request
@@ -386,15 +386,15 @@
         # if not session_key:
         #     return None
         session = await (engine or self.engine).ainit_from(session_key, config=self)
         session._request = request
         return session
 
     def getter(self, request: Request, field=None):
-        cvar = self.context_var.init(request)
+        cvar = self.context_var.setup(request)
         engine = None
         if field:
             # maybe a field has its own session schema as engine
             engine = self.get_engine(field)
         if cvar.contains():
             session: BaseSessionSchema = cvar.get()
             engine = engine or self.engine
@@ -409,15 +409,15 @@
             return session
         session = self.get_session(request, engine)
         cvar.set(session)
         return session
 
     @awaitable(getter)
     async def getter(self, request: Request, field=None):
-        cvar = self.context_var.init(request)
+        cvar = self.context_var.setup(request)
         engine = None
         if field:
             # maybe a field has its own session schema as engine
             engine = self.get_engine(field)
         if cvar.contains():
             session: BaseSessionSchema = await cvar.get()
             engine = engine or self.engine
@@ -431,15 +431,15 @@
                 cvar.set(session)
             return session
         session = await self.get_session(request, engine)
         cvar.set(session)
         return session
 
     def login(self, request, key: str, expiry_age: int = None, user_id_var=var.user_id):
-        new_user_id = user_id_var.get(request)
+        new_user_id = user_id_var.getter(request)
         if new_user_id is None:
             return
         session: BaseSessionSchema = self.getter(request)
         if session is None:
             # NOT [not session]
             # because an empty dict is False in bool too
             return
@@ -448,19 +448,22 @@
             if self.cycle_key_at_login:
                 session.cycle_key()
         else:
             if str(user_id) != str(new_user_id):
                 session.flush()
         session[key] = new_user_id
         if expiry_age is not None:
-            session.expiry = time_now() + timedelta(seconds=expiry_age)
+            if not expiry_age:
+                session.expiry = EPOCH
+            else:
+                session.expiry = time_now() + timedelta(seconds=expiry_age)
 
     @awaitable(login)
     async def login(self, request, key: str, expiry_age: int = None, user_id_var=var.user_id):
-        new_user_id = await user_id_var.get(request)
+        new_user_id = await user_id_var.getter(request)
         if new_user_id is None:
             return
         session: BaseSessionSchema = await self.getter(request)
         if session is None:
             # NOT [not session]
             # because an empty dict is False in bool too
             return
@@ -469,15 +472,18 @@
             if self.cycle_key_at_login:
                 await session.acycle_key()
         else:
             if str(user_id) != str(new_user_id):
                 await session.aflush()
         session[key] = new_user_id
         if expiry_age is not None:
-            session.expiry = time_now() + timedelta(seconds=expiry_age)
+            if not expiry_age:
+                session.expiry = EPOCH
+            else:
+                session.expiry = time_now() + timedelta(seconds=expiry_age)
 
     def is_empty(self, session: BaseSessionSchema):
         return session.is_empty
 
     def save_session(self, response: Response, session: BaseSessionSchema):
         response.patch_vary_headers("Cookie")
         if (session.modified or self.save_every_request) and not session.is_empty:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/base.py` & `utilmeta-2.5.2/utilmeta/core/cache/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/config.py` & `utilmeta-2.5.2/utilmeta/core/cache/config.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/lock.py` & `utilmeta-2.5.2/utilmeta/core/cache/lock.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/django.py` & `utilmeta-2.5.2/utilmeta/core/cache/backends/django.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/redis/aioredis.py` & `utilmeta-2.5.2/utilmeta/core/cache/backends/redis/aioredis.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/redis/config.py` & `utilmeta-2.5.2/utilmeta/core/cache/backends/redis/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 from .aioredis import AioredisAdaptor
 from ..django import DjangoCacheAdaptor
 
 
 class RedisCache(Cache):
     async_adaptor_cls = AioredisAdaptor
+    sync_adaptor_cls = DjangoCacheAdaptor
 
     username: Optional[str] = None
     password: Optional[str] = None
     db: int = 0
     scheme: str = 'redis'
 
     def __init__(
```

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/redis/entity.py` & `utilmeta-2.5.2/utilmeta/core/cache/backends/redis/entity.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/redis/lock.py` & `utilmeta-2.5.2/utilmeta/core/cache/backends/redis/lock.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/backends/redis/scripts/alter_amount.lua` & `utilmeta-2.5.2/utilmeta/core/cache/backends/redis/scripts/alter_amount.lua`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/plugins/api.py` & `utilmeta-2.5.2/utilmeta/core/cache/plugins/api.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/plugins/base.py` & `utilmeta-2.5.2/utilmeta/core/cache/plugins/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/plugins/entity.py` & `utilmeta-2.5.2/utilmeta/core/cache/plugins/entity.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cache/plugins/sdk.py` & `utilmeta-2.5.2/utilmeta/core/cache/plugins/sdk.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cli/backends/aiohttp.py` & `utilmeta-2.5.2/utilmeta/core/cli/backends/aiohttp.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,8 +13,10 @@
             resp = await session.request(
                 method=self.request.method,
                 url=self.request.url,
                 data=self.request.body,
                 headers=self.request.headers,
                 allow_redirects=allow_redirects,
             )
+            await resp.read()
+            # read here, not outside the session
             return AiohttpClientResponseAdaptor(resp)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/cli/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/cli/backends/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/cli/backends/httpx.py` & `utilmeta-2.5.2/utilmeta/core/cli/backends/httpx.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 from .base import ClientRequestAdaptor
 from utilmeta.utils import awaitable
 
 
 class HttpxClientRequestAdaptor(ClientRequestAdaptor):
     backend = httpx
 
+    @property
+    def request_kwargs(self):
+        kwargs = dict(
+            method=self.request.method,
+            url=self.request.url,
+            headers=self.request.headers,
+        )
+        if self.request.body:
+            if isinstance(self.request.body, bytes):
+                kwargs.update(content=self.request.body)
+            elif isinstance(self.request.body, (dict, list)):
+                kwargs.update(json=self.request.body)
+            else:
+                kwargs.update(data=self.request.body)
+        return kwargs
+
     def __call__(self, timeout: int = None, **kwargs):
         from utilmeta.core.response.backends.httpx import HttpxClientResponseAdaptor
         with httpx.Client(timeout=timeout) as client:
-            resp = client.request(
-                method=self.request.method,
-                url=self.request.url,
-                content=self.request.body,
-                headers=self.request.headers,
-            )
+            resp = client.request(**self.request_kwargs)
             return HttpxClientResponseAdaptor(resp)
 
     @awaitable(__call__)
     async def __call__(self, timeout: int = None, **kwargs):
         from utilmeta.core.response.backends.httpx import HttpxClientResponseAdaptor
         async with httpx.AsyncClient(timeout=timeout) as client:
-            resp = await client.request(
-                method=self.request.method,
-                url=self.request.url,
-                content=self.request.body,
-                headers=self.request.headers,
-            )
+            resp = await client.request(**self.request_kwargs)
             return HttpxClientResponseAdaptor(resp)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/cli/backends/urllib.py` & `utilmeta-2.5.2/utilmeta/core/cli/backends/urllib.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,14 @@
     backend = urllib
 
     def __call__(self, timeout: int = None, **kwargs):
         from utilmeta.core.response.backends.urllib import UrllibResponseAdaptor
         try:
             resp = urlopen(Request(
                 url=self.request.url,
-                method=self.request.method,
+                method=str(self.request.method).upper(),
                 data=self.request.body,
                 headers=self.request.headers,
             ), timeout=timeout)
         except HTTPError as e:
             resp = e
         return UrllibResponseAdaptor(resp)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/file/base.py` & `utilmeta-2.5.2/utilmeta/core/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class InvalidFileType(UnprocessableEntity):
     pass
 
 
 class File:
     file: BytesIO
+    format = 'binary'
+    # FOR JSON SCHEMA
 
     encoding = property(lambda self: self.file.encoding)
     fileno = property(lambda self: self.file.fileno)
     flush = property(lambda self: self.file.flush)
     isatty = property(lambda self: self.file.isatty)
     newlines = property(lambda self: self.file.newlines)
     read = property(lambda self: self.file.read)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/file/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/file/backends/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/file/backends/bytesio.py` & `utilmeta-2.5.2/utilmeta/core/file/backends/bytesio.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/file/backends/django.py` & `utilmeta-2.5.2/utilmeta/core/file/backends/django.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/__init__.py` & `utilmeta-2.5.2/utilmeta/core/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/compiler.py` & `utilmeta-2.5.2/utilmeta/core/orm/compiler.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/context.py` & `utilmeta-2.5.2/utilmeta/core/orm/context.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/exceptions.py` & `utilmeta-2.5.2/utilmeta/core/orm/exceptions.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/generator.py` & `utilmeta-2.5.2/utilmeta/core/orm/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .parser import QueryClassParser
 from .fields.filter import ParserFilter
 from .fields.order import Order, ParserOrderBy
 from .fields.pagination import Page, Limit, Offset
 from .fields.scope import Scope
 from typing import TYPE_CHECKING
 from .context import QueryContext
-# from utilmeta.utils import awaitable
+from utilmeta.utils import multi
 
 
 if TYPE_CHECKING:
     from .backends.base import ModelFieldAdaptor
 
 
 class BaseQuerysetGenerator:
@@ -71,14 +71,16 @@
     def process_order(self, order: Order, field: 'ModelFieldAdaptor', name: str, flag: int = 1):
         raise NotImplementedError
 
     def process_value(self, field, value):
         if isinstance(field, ParserFilter) and field.filterable:
             self.process_filter(field, value=value)
         elif isinstance(field, ParserOrderBy):
+            if not multi(value):
+                value = [value]
             for o in value:
                 if o in field.orders:
                     order, f, flag = field.orders[o]
                     self.process_order(
                         order,
                         field=f,
                         flag=flag,
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/param.py` & `utilmeta-2.5.2/utilmeta/core/orm/param.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/parser.py` & `utilmeta-2.5.2/utilmeta/core/orm/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,21 @@
     @property
     def kwargs(self):
         return dict(model=self.model)
 
     def get_generator(self, values: dict) -> 'BaseQuerysetGenerator':
         return self.model.generator_cls(self, values)
 
+    @property
+    def schema_annotations(self):
+        data = super().schema_annotations or {}
+        if self.model:
+            data.update(model=self.model.ident)
+        return data
+
 
 class SchemaClassParser(ClassParser):
     parser_field_cls = ParserQueryField
 
     def __init__(self, obj, *args, **kwargs):
         model = getattr(obj, '__model__', None)
         from .backends.base import ModelAdaptor
@@ -72,7 +79,14 @@
         return self.model.init_instance(**inst)
 
     def get_pk(self, data: dict):
         for name in self.pk_names:
             pk = data.get(name)
             if pk is not None:
                 return pk
+
+    @property
+    def schema_annotations(self):
+        data = super().schema_annotations or {}
+        if self.model:
+            data.update(model=self.model.ident)
+        return data
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/schema.py` & `utilmeta-2.5.2/utilmeta/core/orm/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import utype
 from typing import TypeVar, Type, List
 from utilmeta.core import request as req
 from .parser import SchemaClassParser, QueryClassParser
 # from .generator import BaseQuerysetGenerator
 # from .backends.base import ModelAdaptor
-from . import exceptions
+from utilmeta.core.orm import exceptions
 
 T = TypeVar('T')
 
 # class ModLogicalMeta(utype.LogicalMeta):
 #     def __mod__(cls: T, other) -> T:
 #         if isinstance(other, str):
 #             other = utype.Options(mode=other)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,22 @@
     def __init__(self, field, addon: str = None, model: 'ModelAdaptor' = None, lookup_name: str = None):
         self.field = field
         self.addon = addon
         self.lookup_name = lookup_name
         self._model = model
 
     @property
+    def title(self) -> Optional[str]:
+        return None
+
+    @property
+    def description(self) -> Optional[str]:
+        return None
+
+    @property
     def related_model(self) -> Optional['ModelAdaptor']:
         raise NotImplementedError
 
     @property
     def remote_field(self) -> Optional['ModelFieldAdaptor']:
         raise NotImplementedError
 
@@ -64,14 +72,22 @@
     def check_query(self):
         raise NotImplementedError
 
     @property
     def column_name(self) -> str:
         raise NotImplementedError
 
+    @property
+    def to_field(self) -> str:
+        raise NotImplementedError
+
+    @property
+    def relate_name(self) -> str:
+        raise NotImplementedError
+
     def get_supported_operators(self):
         pass
 
     @property
     def is_nullable(self):
         raise NotImplementedError
 
@@ -84,14 +100,22 @@
         raise NotImplementedError
 
     @property
     def is_writable(self):
         raise NotImplementedError
 
     @property
+    def is_unique(self):
+        raise NotImplementedError
+
+    @property
+    def is_db_index(self):
+        raise NotImplementedError
+
+    @property
     def is_exp(self):
         raise NotImplementedError
 
     @property
     def is_pk(self):
         raise NotImplementedError
 
@@ -127,14 +151,18 @@
     def is_many(self):
         return self.is_2m or self.is_m2
 
     @property
     def is_combined(self):
         raise NotImplementedError
 
+    @property
+    def multi_relations(self):
+        raise NotImplementedError
+
     @classmethod
     def get_exp_field(cls, exp) -> Optional[str]:
         raise NotImplementedError
 
     @classmethod
     def iter_combined_expression(cls, exp):
         raise NotImplementedError
@@ -155,14 +183,18 @@
 
     def __init__(self, model):
         if not self.qualify(model):
             raise TypeError(f'{self.__class__}: Invalid model: {model}')
         self.model = model
 
     @property
+    def ident(self):
+        return f'{self.model.__module__}.{self.model.__name__}'
+
+    @property
     def pk_field(self) -> field_adaptor_cls:
         raise NotImplementedError
 
     def update(self, data: dict, q=None, **filters):
         raise NotImplementedError
 
     @awaitable(update)
@@ -175,16 +207,15 @@
     @awaitable(create)
     async def create(self, d=None, **data):
         raise NotImplementedError
 
     def delete(self, q=None, **filters):
         raise NotImplementedError
 
-    @awaitable(delete)
-    async def delete(self, q=None, **filters):
+    async def adelete(self, q=None, **filters):
         raise NotImplementedError
 
     # def update_queryset(self, queryset, data: dict):
     #     raise NotImplementedError
     #
     # def serialize_queryset(self, queryset):
     #     raise NotImplementedError
@@ -195,16 +226,16 @@
 
     def get_instance(self, q=None, **filters):
         raise NotImplementedError
 
     def init_instance(self, pk=None, **data):
         raise NotImplementedError
 
-    @awaitable(get_instance)
-    async def get_instance(self, q=None, **filters):
+    # @awaitable(get_instance)
+    async def aget_instance(self, q=None, **filters):
         raise NotImplementedError
 
     def check_related_queryset(self, qs):
         raise NotImplementedError
 
     def get_model(self, qs) -> 'ModelAdaptor':
         raise NotImplementedError
@@ -239,16 +270,16 @@
 
     def get_reverse_lookup(self, lookup: str) -> Tuple[str, Optional[str]]:
         raise NotImplementedError
 
     def get_last_many_relates(self, lookup: str):
         raise NotImplementedError
 
-    def get_fields(self) -> List[ModelFieldAdaptor]:
-        pass
+    def get_fields(self, many=False, no_inherit=False) -> List[ModelFieldAdaptor]:
+        raise NotImplementedError
 
     def get_related_adaptor(self, field):
         return self.__class__(field.related_model) if field.related_model else None
 
     def gen_lookup_keys(self, field: str, keys, strict: bool = True, excludes: List[str] = None) -> list:
         raise NotImplementedError
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/compiler.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,16 +265,31 @@
                             )
 
                     # normalize user input
                 else:
                     # many related field / common values
                     # like author__followers / author__followers__join_date
                     # we need to serialize its value first
-                    if field.model_field.remote_field and field.model_field.remote_field.is_pk:
+
+                    if field.is_sub_relation:
                         pk_map = {str(pk): pk for pk in pk_list}
+
+                    elif field.model_field.is_2o:
+                        f, c = field.model_field.reverse_lookup
+                        m = field.model_field.related_model
+                        # use reverse query due to the unfixed issue on the async backend
+                        # also prevent redundant "None" over the non-exist fk
+
+                        if m and f:
+                            for val in m.get_queryset(
+                                    **{f + '__in': pk_list}).values(c or PK, __target=exp.F(f)):
+                                rel = val['__target']
+                                if rel is not None:
+                                    pk_map.setdefault(rel, []).append(val[c or PK])
+
                     else:
                         _args = []
                         _kw = {}
                         qn = self.get_query_name(field)
                         if qn == key:
                             _args = (key,)
                         else:
@@ -479,29 +494,31 @@
                         for pk in self.pk_list:
                             rel_qs = field.func(pk, __class__=self.parser.obj)
                             if inspect.isawaitable(rel_qs):
                                 rel_qs = await rel_qs
                             pk_map[str(pk)] = await self.normalize_pk_list(rel_qs)
 
                 else:
-                    if field.model_field.is_2o:
-                        # fixme: also no many-relates included in the reverse relations
-                        # many to one
-                        if field.model_field.remote_field and field.model_field.remote_field.is_pk:
-                            pk_map = {str(pk): pk for pk in pk_list}
-                        else:
-                            f, c = field.model_field.reverse_lookup
-                            m = field.model_field.related_model
-                            # use reverse query due to the unfixed issue on the async backend
-                            if m and f:
-                                async for val in m.get_queryset(
-                                        **{f + '__in': pk_list}).values(c or PK, __target=exp.F(f)):
-                                    rel = val['__target']
-                                    if rel is not None:
-                                        pk_map.setdefault(rel, []).append(val[c or PK])
+                    if field.is_sub_relation:
+                        # fixme: async backend may not fetch pk along with one-to-rel
+
+                        pk_map = {str(pk): pk for pk in pk_list}
+
+                    elif field.model_field.is_2o:
+                        f, c = field.model_field.reverse_lookup
+                        m = field.model_field.related_model
+                        # use reverse query due to the unfixed issue on the async backend
+                        # also prevent redundant "None" over the non-exist fk
+                        if m and f:
+                            async for val in m.get_queryset(
+                                    **{f + '__in': pk_list}).values(c or PK, __target=exp.F(f)):
+                                rel = val['__target']
+                                if rel is not None:
+                                    pk_map.setdefault(rel, []).append(val[c or PK])
+
                     else:
                         _args = []
                         _kw = {}
                         qn = self.get_query_name(field)
                         if qn == key:
                             _args = (key,)
                         else:
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/constant.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/constant.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/database.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/database.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/deletion.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/deletion.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/expressions.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/expressions.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/field.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,14 @@
 
 
 def to_many(field):
     return isinstance(field, (models.ManyToManyField, models.ManyToManyRel, models.ForeignKey))
 
 
 def to_one(field):
-    """
-    This kind of field is mutable in Module side, because the modify can only be done from the certain One
-    (OneRel | Fk)
-    """
     return isinstance(field, (models.OneToOneField, models.OneToOneRel, models.ManyToOneRel))
 
 
 class DjangoModelFieldAdaptor(ModelFieldAdaptor):
     field: Union[models.Field, ForeignObjectRel, exp.BaseExpression, exp.Combinable]
     model: 'DjangoModelAdaptor'
 
@@ -51,28 +47,43 @@
 
         if not self.qualify(field):
             raise TypeError(f'Invalid field: {field}')
 
         super().__init__(field, addon, model, lookup_name)
         self.validate_addon()
 
+    @property
+    def multi_relations(self):
+        return self.lookup_name and '__' in self.lookup_name
+
     def validate_addon(self):
         if not self.addon:
             return
         if not isinstance(self.addon, str):
             raise TypeError(f'Invalid addon: {repr(self.addon)}, must be str')
         if self.is_concrete:
             _t = self.field.get_internal_type()
             addons = constant.ADDON_FIELD_LOOKUPS.get(_t, [])
             if self.addon not in addons:
                 warnings.warn(f'Invalid addon: {repr(self.addon)} for field: {self.field},'
                               f' only {addons} are supported')
         else:
             raise TypeError(f'Not concrete field: {self.field} cannot have addon: {repr(self.addon)}')
 
+    @property
+    def title(self) -> Optional[str]:
+        name = self.field.verbose_name
+        if name != self.field.name:
+            return name
+        return None
+
+    @property
+    def description(self) -> Optional[str]:
+        return self.field.help_text or None
+
     @classmethod
     def qualify(cls, obj):
         return isinstance(obj, (models.Field, ForeignObjectRel, exp.BaseExpression, exp.Combinable))
 
     @property
     def field_model(self):
         if self.is_exp:
@@ -95,14 +106,16 @@
 
     @property
     def related_model(self):
         if self.is_exp:
             return None
         rel = getattr(self.field, 'related_model')
         if rel:
+            if rel == 'self':
+                return self
             from .model import DjangoModelAdaptor
             return DjangoModelAdaptor(rel)
         return None
 
     @property
     def is_nullable(self):
         if not self.is_concrete:
@@ -125,14 +138,26 @@
         auto_now_add = param.get('auto_now_add')
         auto_created = param.get('auto_created')
         if auto_now_add or auto_created:
             return False
         return True
 
     @property
+    def is_unique(self):
+        if not self.is_concrete:
+            return False
+        return self.field.unique
+
+    @property
+    def is_db_index(self):
+        if not self.is_concrete:
+            return False
+        return self.field.db_index
+
+    @property
     def is_auto(self):
         if not self.is_concrete:
             return False
         param = self.params
         auto_now_add = param.get('auto_now_add')
         auto_now = param.get('auto_now')
         auto_created = param.get('auto_created')
@@ -279,14 +304,29 @@
 
     @property
     def column_name(self) -> Optional[str]:
         if isinstance(self.field, models.Field):
             return self.field.column
         return None
 
+    @property
+    def to_field(self) -> Optional[str]:
+        if self.is_fk:
+            try:
+                return self.field.to_fields[0]
+            except IndexError:
+                pass
+        return None
+
+    @property
+    def relate_name(self) -> Optional[str]:
+        if self.is_fk:
+            return self.field.remote_field.get_cache_name()
+        return None
+
     def get_supported_operators(self):
         pass
 
     @property
     def is_exp(self):
         return isinstance(self.field, (exp.BaseExpression, exp.Combinable))
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/generator.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/generator.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/model.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,23 @@
     field_adaptor_cls = DjangoModelFieldAdaptor
     generator_cls = DjangoQuerysetGenerator
     compiler_cls = DjangoQueryCompiler
     queryset_cls = models.QuerySet
     model_cls = models.Model
     model: Type[models.Model]
 
+    @property
+    def ident(self):
+        meta = self.meta
+        if not meta:
+            return ''
+        app_label = meta.app_label
+        tag = '.'.join((app_label, self.model.__name__))
+        return tag.lower()
+
     @classmethod
     def qualify(cls, obj):
         return isinstance(obj, ModelBase)
 
     @property
     def pk_field(self) -> field_adaptor_cls:
         return self.field_adaptor_cls(self.meta.pk)
@@ -56,16 +65,15 @@
 
     def delete(self, q=None, **filters):
         if not q and not filters:
             # no filters
             return
         return self.get_queryset(q, **filters).delete()
 
-    @awaitable(delete)
-    async def delete(self, q=None, **filters):
+    async def adelete(self, q=None, **filters):
         if not q and not filters:
             # no filters
             return
         return await self.get_queryset(q, **filters).adelete()
 
     def get_queryset(self, q=None, **filters) -> queryset_cls:
         # for django it's like model.objects.all()
@@ -74,16 +82,15 @@
         if args or filters:
             return base.filter(*args, **filters)
         return base
 
     def get_instance(self, q=None, **filters) -> model_cls:
         return self.get_queryset(q, **filters).first()
 
-    @awaitable(get_instance)
-    async def get_instance(self, q=None, **filters) -> model_cls:
+    async def aget_instance(self, q=None, **filters) -> model_cls:
         return await self.get_queryset(q, **filters).afirst()
 
     def init_instance(self, pk=None, **data):
         if pk:
             data.setdefault('pk', pk)
         obj = self.model(**data)
         if getattr(obj, 'id', None) is None:
@@ -191,15 +198,15 @@
         meta = self.meta
         if not meta:
             return []
         fields = []
         pk = meta.pk
         if pk:
             # abstract model meta.pk is None
-            fields.append(pk)
+            fields.append(DjangoModelFieldAdaptor(pk, model=self))
         for f in meta.get_fields() if many else meta.fields:
             if self.field_adaptor_cls(f).is_pk:
                 continue
             if f.remote_field:
                 if self.field_adaptor_cls(f.remote_field).is_pk:
                     continue
             if no_inherit:
@@ -207,15 +214,15 @@
                     # parent model
                     continue
             if many:
                 try:
                     self.get_field(f.name)
                 except exc.FieldDoesNotExist:
                     continue
-            fields.append(f)
+            fields.append(DjangoModelFieldAdaptor(f, model=self))
         return fields
 
     def get_related_adaptor(self, field):
         return self.__class__(field.related_model) if field.related_model else None
 
     def gen_lookup_keys(self, field: str, keys, strict: bool = True, excludes: List[str] = None) -> list:
         raise NotImplementedError
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/models.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/models.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/query.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/query.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/django/queryset.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/django/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -632,15 +632,17 @@
         # return await self.aupdate_or_create(defaults, **kwargs)
         defaults = defaults or {}
         self._for_write = True
         db = self.connections_cls.get(self.db)
         async with db.async_transaction():
             # Lock the row so that a concurrent update is blocked until
             # update_or_create() has performed its save.
-            obj, created = await self.select_for_update().aget_or_create(defaults, **kwargs)
+            # obj, created = await self.select_for_update().aget_or_create(defaults, **kwargs)
+            obj, created = await self.aget_or_create(defaults, **kwargs)
+            # fixme: SELECT FOR UPDATE IN ASYNC CONTEXT
             if created:
                 return obj, created
             if obj.pk:
                 params = dict(resolve_callables(defaults))
                 await self.__class__(self.model).filter(pk=obj.pk).aupdate(**params)
         return obj, False
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/peewee/example.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/peewee/example.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/backends/peewee/peewee.py` & `utilmeta-2.5.2/utilmeta/core/orm/backends/peewee/peewee.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/databases/base.py` & `utilmeta-2.5.2/utilmeta/core/orm/databases/base.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/databases/config.py` & `utilmeta-2.5.2/utilmeta/core/orm/databases/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     DEFAULT_PORTS = {
         'postgres': 5432,
         'mysql': 3306
     }
 
     sync_adaptor_cls = None
     async_adaptor_cls = EncodeDatabasesAsyncAdaptor
+    # fixme:
+    # for backend that does not support async startup function
+    # the async connection cannot be established
+
     # ---
     name: str
     engine: str = 'sqlite'
     user: str = ''
     password: str = ''
     host: str = ''
     port: Optional[int] = None
@@ -100,14 +104,19 @@
     def apply(self, alias: str, asynchronous: bool = None):
         if asynchronous:
             if self.async_adaptor_cls:
                 self.adaptor = self.async_adaptor_cls(self, alias)
         else:
             if self.sync_adaptor_cls:
                 self.adaptor = self.sync_adaptor_cls(self, alias)
+            else:
+                # default
+                from ..backends.django.database import DjangoDatabaseAdaptor
+                self.adaptor = DjangoDatabaseAdaptor(self, alias)
+
         if not self.adaptor:
             raise exceptions.NotConfigured('Database adaptor not implemented')
         self.asynchronous = asynchronous
         self.adaptor.check()
 
     def get_adaptor(self, asynchronous: bool = False) -> BaseDatabaseAdaptor:
         if self.asynchronous == asynchronous and self.adaptor:
@@ -163,21 +172,26 @@
 
     def __init__(self, dbs: Dict[str, Database] = None, **databases: Database):
         self.databases = dbs or databases
         super().__init__(**self.databases)
 
     def hook(self, service: UtilMeta):
         for name, db in self.databases.items():
-            if not db.sync_adaptor_cls:
-                if service.adaptor and service.adaptor.sync_db_adaptor_cls:
-                    db.sync_adaptor_cls = service.adaptor.sync_db_adaptor_cls
-            if not db.async_adaptor_cls:
-                if service.adaptor and service.adaptor.async_db_adaptor_cls:
-                    db.async_adaptor_cls = service.adaptor.async_db_adaptor_cls
-            db.apply(name, asynchronous=service.asynchronous)
+            self.add_database(service, alias=name, database=db)
+
+    def add_database(self, service: UtilMeta, alias: str, database: Database):
+        if not database.sync_adaptor_cls:
+            if service.adaptor and service.adaptor.sync_db_adaptor_cls:
+                database.sync_adaptor_cls = service.adaptor.sync_db_adaptor_cls
+        if not database.async_adaptor_cls:
+            if service.adaptor and service.adaptor.async_db_adaptor_cls:
+                database.async_adaptor_cls = service.adaptor.async_db_adaptor_cls
+        database.apply(alias, asynchronous=service.asynchronous)
+        if alias not in self.databases:
+            self.databases.setdefault(alias, database)
 
     @classmethod
     def get(cls, alias: str = 'default') -> Database:
         config = cls.config()
         if not config:
             raise exceptions.NotConfigured(cls)
         return config.databases[alias]
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/databases/encode.py` & `utilmeta-2.5.2/utilmeta/core/orm/databases/encode.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/fields/field.py` & `utilmeta-2.5.2/utilmeta/core/orm/fields/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,35 +68,41 @@
                         self.related_single = False
         else:
             # try to find Optional[schema]
             for origin in self.input_origins:
                 cls_parser = ClassParser.resolve_parser(origin)
                 if cls_parser:
                     parser = cls_parser
+                    schema = origin
                     self.related_single = True
                     break
 
         if parser:
             if isinstance(parser, SchemaClassParser):
                 if parser.model:
                     if self.model_field and self.related_model:
                         # if parser.model and self.model_field:
                         # check model if not queryset
                         if self.related_model.is_sub_model(parser.model) \
                                 or parser.model.is_sub_model(self.related_model):
                             schema = schema or parser.obj
                         else:
                             raise TypeError(f'orm.Field({repr(self.name)}): '
-                                            f'Invalid related model: {self.related_model.model},'
-                                            f' sub model of {parser.model.model} expected')
+                                            f'Invalid related model: {parser.model.model},'
+                                            f' sub model of {self.related_model.model} expected')
                     else:
                         schema = schema or parser.obj
                         # 1. func field
                         # 2. common field (or array field) with not constraint relation
 
+                # schema should set AS IS and prevent from going to [parser.obj]
+                # because when using __future__.annotations
+                # parser.obj will be orm.Schema until the Schema class is initialized
+                # so if the schema contains self-reference, it will not provide the correct related schema
+
             if not schema:
                 if not self.related_model:
                     # treat as a common field (like JSONField)
                     # with inner schema
                     return
                     # raise TypeError(f'orm.Field({repr(self.name)})) no model '
                     #                 f'specified for related schema: {parser.obj}')
@@ -131,16 +137,14 @@
     def setup(self, options: utype.Options):
         super().setup(options)
 
         from ..backends.base import ModelAdaptor
         if not isinstance(self.model, ModelAdaptor):
             return
 
-        self.get_query_schema()
-
         if class_func(self.field_name):
             from utype.parser.func import FunctionParser
             func = FunctionParser.apply_for(self.field_name)
             # fixme: ugly approach, getting the awaitable async function
             async_func = getattr(func.obj, '_asyncfunc', None)
             sync_func = getattr(func.obj, '_syncfunc', None)
             if async_func and sync_func:
@@ -165,35 +169,45 @@
                     parse_params=True,
                     parse_result=True
                 )
             self.func_multi = bool(func.pos_var)
 
             if not self.mode:
                 self.mode = 'r'
+
+            self.get_query_schema()
             return
 
         if self.model.check_related_queryset(self.field_name):
             self.queryset = self.field_name
             if not self.mode:
                 self.mode = 'r'
             self.related_model = self.model.get_model(self.queryset)
             if not self.related_model:
                 raise ValueError(f'No model detected in queryset: {self.queryset}')
+
+            self.get_query_schema()
+
             if self.related_single is False:
                 warnings.warn(f'{self.model} schema field: {repr(self.name)} is a multi-relation with a subquery, '
                               f'you need to make sure that only 1 row of the query is returned, '
                               f'otherwise use query function instead')
             self.isolated = True
             # force isolated for queryset query (even without schema)
             return
 
         self.model_field = self.model.get_field(self.field_name, allow_addon=True, silently=True)
+        self.related_model = self.model_field.related_model if self.model_field else None
+
+        # fix: get related model before get query schema
+        self.get_query_schema()
+
         if self.model_field:
-            self.primary_key = self.model_field and self.model_field.is_pk \
-                               and self.model.is_sub_model(self.model_field.field_model)
+            self.primary_key = self.model_field and self.model_field.is_pk and \
+                               self.model.is_sub_model(self.model_field.field_model)
             # use is sub model, because pk might be its base model
 
             if self.primary_key and self.model_field.is_auto:
                 self.required = False
 
             if not self.model_field.is_writable or self.model.cross_models(self.field_name):
                 # read only
@@ -212,16 +226,14 @@
             # this is too far...
             # maybe user wants to assign after initialization
             # if not self.model_field.is_optional:
             #     if not self.required:
             #         # required when creating
             #         self.required = 'a'
 
-            self.related_model = self.model_field.related_model
-
             self.many_included = self.model.include_many_relates(self.field_name)
             if self.many_included:
                 # 1. many included fields will be force isolated
                 # if not self.model_field.is_exp:
                 # expression need to be isolated, otherwise multiple many included query will blow the query
                 self.isolated = True
 
@@ -294,14 +306,40 @@
             # do not use [or] / [bool] to validate such field
             # because that might be a queryset
             if self.field.field is None:
                 return self.attname
             return self.field.field
         return self.attname
 
+    @property
+    def is_sub_relation(self):
+        # relate to a sub model, which is identical to the primary key of the queried pks
+        # eg.
+        # class Content(Model):
+        #    pass
+        # class Article(Content):
+        #    pass
+        # content.article is a sub relation
+        if self.related_model:
+            if issubclass(self.related_model.model, self.model.model):
+                if not self.model_field.multi_relations and \
+                        self.model_field.remote_field and \
+                        self.model_field.remote_field.is_pk:
+                    return True
+        return False
+
+    @property
+    def schema_annotations(self):
+        data = dict(self.field.schema_annotations or {})
+        if self.model_field:
+            data.update(field=self.model_field.query_name)
+        if self.related_model:
+            data.update(related_model=self.related_model.ident)
+        return data
+
 
 class QueryField(Field):
     parser_field_cls = ParserQueryField
 
     def __init__(self, field=None, *,
                  fail_silently: bool = None,
                  auth: dict = None,
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/fields/filter.py` & `utilmeta-2.5.2/utilmeta/core/orm/fields/filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,20 @@
                  ):
         self.field = field
         self.query = query
         self.order = order
         self.fail_silently = fail_silently
         super().__init__(**kwargs, required=required)
 
+    @property
+    def schema_annotations(self):
+        return {
+            'class': 'filter',
+        }
+
 
 class ParserFilter(ParserField):
     field: 'Filter'
     field_cls = Filter
 
     def __init__(
             self,
@@ -91,8 +97,15 @@
     @property
     def field_name(self):
         if isinstance(self.field, Filter):
             if self.field.field:
                 return self.field.field
             if self.field.query:
                 return None
-        return self.attname
+        return self.attname
+
+    @property
+    def schema_annotations(self):
+        data = dict(self.field.schema_annotations or {})
+        if self.model_field:
+            data.update(field=self.model_field.query_name)
+        return data
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/fields/order.py` & `utilmeta-2.5.2/utilmeta/core/orm/fields/order.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,27 +75,54 @@
 
                 if order.asc:
                     orders.setdefault(name, (order, field, 1))
                 if order.desc:
                     orders.setdefault(self.desc_prefix + name, (order, field, -1))
 
             self.orders = orders
-            self.type = enum_array(list(orders))
+            self.type = enum_array(
+                list(orders),
+                item_type=str,
+                # name=f'{self.model.ident}.{self.name}.enum',
+                unique=True
+            )
 
     # def parse_value(self, value, context):
     #     value = super().parse_value(value, context=context)
     #     if isinstance(context, QueryContext):
     #         orders = []
     #         for o in value:
     #             if o in self.orders:
     #                 order, flag = self.orders[o]
     #                 context.orders.append((o, order, flag))
     #         return orders
     #     return value
 
+    @property
+    def schema_annotations(self):
+        data = dict(self.field.schema_annotations or {})
+        orders = {}
+        for key, order in self.field.orders.items():
+            order: Order
+            field_name = order.field or key
+            name = key
+            if not isinstance(name, str):
+                field = self.model.get_field(field_name, allow_addon=True)
+                name = field_name = field.query_name
+            orders[name] = dict(
+                document=order.document,
+                field=str(field_name),
+                asc=order.asc,
+                desc=order.desc,
+                nulls_first=order.nulls_first,
+                nulls_last=order.nulls_last
+            )
+        data.update(orders=orders)
+        return data
+
 
 class OrderBy(Field):
     parser_field_cls = ParserOrderBy
 
     def __init__(self, orders: Union[list, Dict[Any, Order]],
                  *,
                  # orders can be a list of model fields, or a dict of order configuration
@@ -129,7 +156,13 @@
         )
 
         self.orders = orders
         self.desc_prefix = desc_prefix
         self.ignore_invalids = ignore_invalids
         self.ignore_conflicts = ignore_conflicts
         self.single = single
+
+    @property
+    def schema_annotations(self):
+        return {
+            'class': 'order_by',
+        }
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/fields/pagination.py` & `utilmeta-2.5.2/utilmeta/core/orm/fields/pagination.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,34 @@
 class Page(Field):
     type = types.PositiveInt
     # parser_field_cls = ParserPagination
 
     def __init__(self, ge: int = 1, required: bool = False, **kwargs):
         super().__init__(**kwargs, required=required, ge=ge)
 
+    @property
+    def schema_annotations(self):
+        return {'class': 'page'}
+
 
 class Offset(Field):
     type = types.PositiveInt
     # parser_field_cls = ParserPagination
 
     def __init__(self, ge: int = 0, required: bool = False, **kwargs):
         super().__init__(**kwargs, required=required, ge=ge)
 
+    @property
+    def schema_annotations(self):
+        return {'class': 'offset'}
+
 
 class Limit(Field):
     type = types.PositiveInt
     # parser_field_cls = ParserPagination
 
     def __init__(self, ge: int = 0, required: bool = False, **kwargs):
         super().__init__(**kwargs, required=required, ge=ge)
+
+    @property
+    def schema_annotations(self):
+        return {'class': 'limit'}
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/fields/scope.py` & `utilmeta-2.5.2/utilmeta/core/orm/fields/scope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from utype import Field
 from utilmeta.utils import multi
+from typing import Union, List, Dict
 
 
 class Scope(Field):
     # cascade
     # if like, the comments or article is cascaded
     # we can use @template: {"comments": {"id": "", "body": "", "comments": "@cascade"}}
 
@@ -29,7 +30,18 @@
         if isinstance(value, str):
             return {value: None}
         elif isinstance(value, dict):
             return value
         elif multi(value):
             return {v: None for v in value}
         return None
+
+    @property
+    def schema_annotations(self):
+        return {
+            'class': 'scope',
+            'excluded':  self.excluded
+        }
+
+    @property
+    def default_type(self):
+        return Union[List[str], Dict[str, str]]
```

### Comparing `utilmeta-2.4.1/utilmeta/core/orm/plugins/atomic.py` & `utilmeta-2.5.2/utilmeta/core/orm/plugins/atomic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from utilmeta.utils.plugin import Plugin
+from utilmeta.utils import awaitable
 from ..databases.config import DatabaseConnections
 import inspect
 import functools
 
 
 class AtomicPlugin(Plugin):
     def __init__(self, alias: str = 'default', savepoint: bool = True, durable: bool = False,
@@ -37,10 +38,21 @@
             )
 
             @functools.wraps(f)
             def wrapper(*args, **kwargs):
                 with transaction:
                     return f(*args, **kwargs)
 
+            try:
+                from utilmeta import service
+            except ImportError:
+                pass
+            else:
+                if service.asynchronous:
+                    @functools.wraps(f)
+                    def threaded_wrapper(*args, **kwargs):
+                        return service.pool.get_result(wrapper, *args, **kwargs)
+                    return threaded_wrapper
+
             return wrapper
 
         return super().__call__(f, *_, **__)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/base.py` & `utilmeta-2.5.2/utilmeta/utils/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,240 +1,200 @@
-from utype.types import *
-from typing import Optional, Union, Callable, List, Any, Dict, Tuple
-from datetime import datetime, date, timedelta
-from .backends.base import RequestAdaptor
-from utilmeta.utils import MetaMethod, time_now, get_interval
-from http.cookies import SimpleCookie
-from collections.abc import Mapping
-from . import var
-from urllib.parse import urlsplit, parse_qs
-from utilmeta.utils import Headers
-
-
-__all__ = [
-    'Request',
-]
-
-
-class DummyRequest:
-    def __init__(self,
-                 method: str,
-                 url: str,
-                 query: dict = None,
-                 data=None,
-                 headers: Dict[str, str] = None):
-        self.method = method
-        self.url = url or ''
-        self.query = query or {}
-        self.data = data
-        self.headers = Headers(headers or {})
-        cookie = SimpleCookie(self.headers.get('cookie', {}))
-        self.cookies = {k: v.value for k, v in cookie.items()}
+from . import multi, represent, Attr, SEG, ImmutableDict, distinct_add
+from typing import Dict, Any, TypeVar, List
+import inspect
+
+T = TypeVar('T')
+
+__all__ = ['Util', 'Meta']
+
+
+# class UtilKey:
+#     CLS = '@'
+#     PATH = '@path'
+#     ARGS = '@args'
+#     OPERATOR = '@operator'
+#     CONDITIONS = '@conditions'
+
+
+class Meta(type):
+    def __init__(cls, name, bases: tuple, attrs: dict, **kwargs):
+        super().__init__(name, bases, attrs)
+
+        __init = attrs.get(Attr.INIT)   # only track current init
+
+        cls._kwargs = kwargs
+        cls._pos_var = None
+        cls._key_var = None
+        cls._pos_keys = []
+        cls._kw_keys = []
+        cls._defaults = {}
+        cls._requires = set()
+
+        if not bases:
+            return
+
+        defaults = {}
+        requires = set()
+        for base in bases:
+            if isinstance(base, Meta):
+                defaults.update(base._defaults)
+                requires.update(base._requires)
+                distinct_add(cls._pos_keys, base._pos_keys)
+                distinct_add(cls._kw_keys, base._kw_keys)
+                if base._key_var:
+                    cls._key_var = base._key_var
+                if base._pos_var:
+                    cls._pos_var = base._pos_var
+
+        if __init:
+            _self, *parameters = inspect.signature(__init).parameters.items()
+            for k, v in parameters:
+                v: inspect.Parameter
+                if k.startswith(SEG) and k.endswith(SEG):
+                    continue
+                if v.default is not v.empty:
+                    defaults[k] = v.default
+                    if k in requires:
+                        # if base is required but subclass not
+                        requires.remove(k)
+                elif v.kind not in (v.VAR_KEYWORD, v.VAR_POSITIONAL):
+                    requires.add(k)
+
+                if v.kind == v.VAR_POSITIONAL:
+                    cls._pos_var = k
+                elif v.kind == v.POSITIONAL_ONLY:
+                    if k not in cls._pos_keys:
+                        cls._pos_keys.append(k)
+                elif v.kind == v.VAR_KEYWORD:
+                    cls._key_var = k
+                else:
+                    if k not in cls._kw_keys:
+                        cls._kw_keys.append(k)
+
+        cls._defaults = ImmutableDict(defaults)
+        cls._requires = requires
+        cls._attr_names = [a for a in attrs if not a.startswith('_')]
+
+    @property
+    def cls_path(cls):
+        return f'{cls.__module__}.{cls.__name__}'
+
+    @property
+    def kw_keys(cls):
+        return cls._kw_keys
+
+    @property
+    def pos_slice(cls) -> slice:
+        if cls._pos_var:
+            return slice(0, None)
+        return slice(0, len(cls._pos_keys))
+
+
+class Util(metaclass=Meta):
+    def __init__(self, __params__: Dict[str, Any]):
+        args = []
+        kwargs = {}
+        spec = {}
+
+        for key, val in __params__.items():
+            if key.startswith(SEG) and key.endswith(SEG):
+                continue
+            if val is self:
+                continue
+            if key == self._pos_var:
+                args += list(val)
+                continue
+            elif key == self._key_var:
+                if isinstance(val, dict):
+                    _kwargs = {k: v for k, v in val.items() if not k.startswith(SEG)}
+                    kwargs.update(_kwargs)
+                    spec.update(_kwargs)    # also update spec
+                continue
+            elif key in self._pos_keys:
+                args.append(key)
+            elif key in self._kw_keys:
+                kwargs[key] = val
+            else:
+                continue
+            if val != self._defaults.get(key):   # for key_var or pos_var the default is None
+                spec[key] = val
+
+        self.__args__ = tuple(args)
+        self.__kwargs__ = kwargs
+        self.__spec_kwargs__ = ImmutableDict(spec)
+
+    def __hash__(self):
+        return hash(repr(self))
+
+    def __eq__(self, other: 'Util'):
+        if inspect.isclass(self):
+            return super().__eq__(other)
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__spec_kwargs__ == other.__spec_kwargs__ and self.__args__ == other.__args__
+
+    def __bool__(self):
+        # !! return not self.vacuum
+        # prevent use <not self.vacuum> as bool (causing lots of recessive errors)
+        # let sub utils define there own way of bool
+        return True
 
-    @property
-    def route(self):
-        return urlsplit(self.url).path.strip('/')
-
-
-class DummyRequestAdaptor(RequestAdaptor):
-    request: DummyRequest
-
-    def __init__(self, request: DummyRequest, route: str = None, *args, **kwargs):
-        super().__init__(request, route=route or request.route, *args, **kwargs)
-
-    @classmethod
-    def qualify(cls, obj):
-        return isinstance(obj, DummyRequest)
-
-    @property
-    def address(self):
-        from ipaddress import ip_address
-        return ip_address('127.0.0.1')
-
-    @property
-    def content_type(self) -> Optional[str]:
-        ct = super().content_type
-        if ct:
-            return ct
-        if isinstance(self.request.data, (dict, list)):
-            return 'application/json'
-        return None
-
-    @property
-    def request_method(self) -> str:
-        return self.request.method
-
-    @property
-    def url(self) -> str:
-        return str(self.request.url)        # request.url is a URL structure, str will get the inner _url
-
-    @property
-    def cookies(self):
-        return self.request.cookies
-
-    @property
-    def query_params(self):
-        params = super().query_params
-        if self.request.query:
-            params.update(self.request.query)
-        return params
+    def __str__(self):
+        return self._repr()
 
-    @property
-    def query_string(self):
-        return urlsplit(self.request.url).query
-
-    @property
-    def path(self):
-        return urlsplit(self.request.url).path
-
-    @property
-    def scheme(self):
-        return urlsplit(self.request.url).scheme or 'http'
-
-    @property
-    def headers(self):
-        return self.request.headers
-
-    def get_form(self):
-        if isinstance(self.request.data, dict):
-            return self.request.data
-        return None
-
-    @property
-    def body(self) -> bytes:
-        return self.request.data
-
-    async def async_read(self):
-        return self.request.data
-
-    async def async_load(self):
-        return self.get_content()
-
-
-class Request:
-    adaptor_cls: Type[RequestAdaptor]
-
-    method: str
-    url: str
-    query: dict
-    data: Any
-    headers: Union[Mapping, dict]
-    cookies: Union[SimpleCookie, dict]
+    def __repr__(self):
+        return self._repr()
 
     @classmethod
-    def apply_for(cls, req):
-        if isinstance(req, Request):
-            return req
-        return cls(req)
-
-    def __init__(self,
-                 request=None, *,
-                 method: str = None,
-                 url: str = None,
-                 query: dict = None,
-                 data=None,
-                 headers: Union[Mapping, Dict[str, str]] = None,
-                 backend=None,
-                 ):
-        request = request or DummyRequest(
-            method=method,
-            url=url,
-            query=query,
-            data=data,
-            headers=headers
-        )
-        self.adaptor = RequestAdaptor.dispatch(request)
-        self.backend = self.adaptor.backend or backend
-        # self.timeout = None
-
-    # def set_timeout(self, timeout: Union[int, float, timedelta, datetime, None]):
-    #     if isinstance(timeout, datetime):
-    #         timeout = time_now() - timeout
-    #     self.timeout = get_interval(timeout, null=True)
-
-    @property
-    def url(self):
-        return self.adaptor.url
-
-    @property
-    def method(self):
-        return self.adaptor.method
-
-    @property
-    def is_options(self):
-        return self.adaptor.request_method.lower() == MetaMethod.OPTIONS
-
-    @property
-    def path(self) -> str:
-        return self.adaptor.path
-
-    @property
-    def encoded_path(self) -> str:
-        return self.adaptor.encoded_path
-
-    @property
-    def scheme(self):
-        return self.adaptor.scheme
-
-    @property
-    def query_string(self) -> str:
-        return self.adaptor.query_string
-
-    @property
-    def query(self) -> dict:
-        return self.adaptor.query_params
-
-    @property
-    def cookies(self):
-        return self.adaptor.cookies
-
-    @property
-    def origin(self):
-        return self.adaptor.origin
-
-    @property
-    def headers(self) -> dict:
-        return self.adaptor.headers
-
-    @property
-    def authorization(self) -> Tuple[Optional[str], Optional[str]]:
-        auth: str = self.headers.get('authorization')
-        if not auth:
-            return None, None
-        if ' ' in auth:
-            lst = auth.split()
-            return lst[0], ' '.join(lst[1:])
-        return None, auth
-
-    @property
-    def content_type(self) -> Optional[str]:
-        return self.adaptor.content_type
-
-    @property
-    def content_length(self) -> int:
-        return self.adaptor.content_length
-
-    @property
-    def host(self):
-        return self.adaptor.hostname
-
-    @property
-    def body(self) -> bytes:
-        return self.adaptor.body
-
-    async def aread(self) -> bytes:
-        return await self.adaptor.async_read()
-
-    @property
-    def data(self):
-        data = var.data.init(self)
-        if data.contains():
-            return data.get()
-        return None
-
-    @property
-    def time(self) -> datetime:
-        return self.adaptor.time
-
-    @property
-    def ip_address(self):
-        return self.adaptor.address
+    def _copy(cls, data, copy_class: bool = False):
+        if multi(data):
+            return type(data)([cls._copy(d) for d in data])
+        if isinstance(data, dict):
+            return {key: cls._copy(val) for key, val in data.items()}
+        if inspect.isclass(data) and not copy_class:
+            # prevent class util that carry other utils cause RecursiveError
+            return data
+        if isinstance(data, Util):
+            return data.__copy__()
+        return data
+
+    def __deepcopy__(self, memo):
+        return self.__copy__()
+
+    def __copy__(self):
+        # use copied version of sub utils
+        # return self.__class__(*self._args, **self._kwargs)
+        if inspect.isclass(self):
+            bases = getattr(self, Attr.BASES, ())
+            attrs = dict(self.__dict__)
+            # pop(attrs, Attr.LOCK)       # pop __lock__
+            cls: type = self.__class__
+            return cls(self.__name__, bases, self._copy(attrs))
+        return self.__class__(*self._copy(self.__args__), **self._copy(self.__spec_kwargs__))
+
+    @property
+    def _cls_name(self):
+        if inspect.isclass(self):
+            cls = self
+        else:
+            cls = self.__class__
+        try:
+            return cls.__qualname__
+        except AttributeError:
+            return cls.__name__
+
+    def _repr(self, params: List[str] = None, excludes: List[str] = None):
+        if inspect.isclass(self):
+            return f'<{self._cls_name} class "{self.__module__}.{self._cls_name}">'
+        attrs = []
+        for k, v in self.__spec_kwargs__.items():
+            # if not isinstance(v, bool) and any([s in str(k).lower() for s in self._secret_names]) and v:
+            #     v = SECRET
+            if k.startswith('_'):
+                continue
+            if params is not None and k not in params:
+                continue
+            if excludes is not None and k in excludes:
+                continue
+            attrs.append(k + '=' + represent(v))     # str(self.display(v)))
+        s = ', '.join([represent(v) for v in self.__args__] + attrs)
+        return f'{self._cls_name}({s})'
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/properties.py` & `utilmeta-2.5.2/utilmeta/core/request/properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,31 +81,38 @@
     __ident__ = 'body'
     __no_default__ = True
 
     content_type = None
 
     def getter(self, request: Request, field: ParserField = None):
         self.validate_content_type(request)
-        body = request.body
-        self.validate_max_length(body)
-        return body
+        data = request.data
+        var_data = var.data.setup(request)
+        if not var_data.contains():
+            var_data.set(data)
+        self.validate_max_length(request)
+        return data
 
     @awaitable(getter)
     async def getter(self, request: Request, field: ParserField = None):
         self.validate_content_type(request)
-        body = await request.adaptor.async_read()
-        self.validate_max_length(body)
-        return body
+        var_data = var.data.setup(request)
+        if var_data.contains():
+            return await var_data.get()
+        data = await request.adaptor.async_load()
+        var_data.set(data)
+        self.validate_max_length(request)
+        return data
 
     def validate_content_type(self, request: Request):
         if self.content_type and request.content_type != self.content_type:
             raise exc.UnprocessableEntity('invalid content type')
 
-    def validate_max_length(self, body: bytes):
-        if self.max_length and len(body) > self.max_length:
+    def validate_max_length(self, request: Request):
+        if self.max_length and request.content_length and request.content_length > self.max_length:
             raise exc.RequestEntityTooLarge
 
     def __init__(self, content_type: str = None, *,
                  description: str = None,
                  example: Any = None,
                  # options=None,
                  # default=unprovided,
@@ -348,15 +355,15 @@
 
 # single param
 
 
 class PathParam(RequestParam):
     @classmethod
     def get_mapping(cls, request: Request) -> Optional[Mapping]:
-        return var.path_params.get(request)
+        return var.path_params.getter(request)
 
     __in__ = Path
     __no_default__ = True
 
     regex = '[^/]+'  # default regex, can be override
 
     def __init__(self, regex: str = None, *, min_length: str = None, max_length: str = None, required: bool = True):
@@ -399,30 +406,30 @@
 
 
 class BodyParam(RequestParam):
     __in__ = Body
 
     @classmethod
     def get_mapping(cls, request: Request):
-        data = var.data.init(request)
+        data = var.data.setup(request)
         if data.contains():
             return data.get()
         if request.adaptor.json_type:
             mp = request.adaptor.get_json()
         elif request.adaptor.form_type:
             mp = request.adaptor.get_form()
         else:
             raise exc.UnprocessableEntity(f'invalid content type, must be json or form')
         data.set(mp)
         return mp
 
     @classmethod
     @awaitable(get_mapping)
     async def get_mapping(cls, request: Request):
-        data = var.data.init(request)
+        data = var.data.setup(request)
         if data.contains():
             return await data.get()
         if request.adaptor.json_type or request.adaptor.form_type:
             mp = await request.adaptor.async_load()
         else:
             raise exc.UnprocessableEntity(f'invalid content type, must be json or form')
         data.set(mp)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/var.py` & `utilmeta-2.5.2/utilmeta/core/request/var.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,109 @@
 import warnings
 
 
 from typing import Callable
 from utilmeta.utils import awaitable
+from utilmeta.utils.context import Property
 from utype.utils.datastructures import unprovided
 import inspect
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .base import Request
 
 
-class RequestContextVar:
-    def __init__(self, key: str, cached: bool = False, static: bool = False, default=None, factory: Callable = None):
+class RequestContextVar(Property):
+    def __init__(self, key: str, cached: bool = False, static: bool = False,
+                 default=None, factory: Callable = None):
+        super().__init__(
+            default_factory=default if callable(default) else None,
+            default=default if not callable(default) else unprovided
+        )
         self.key = key
         self.default = default
         self.factory = factory
         self.cached = cached
         self.static = static
 
-    def init(self, request: 'Request'):
+    def setup(self, request: 'Request'):
         class c:
             @staticmethod
             def contains():
                 return self.contains(request)
 
             @staticmethod
             def get():
-                return self.get(request)
+                return self.getter(request)
 
             @staticmethod
             @awaitable(get)
             async def get():
-                return await self.get(request)
+                return await self.getter(request)
 
             @staticmethod
             def set(v):
-                return self.set(request, value=v)
+                return self.setter(request, value=v)
+
+            @staticmethod
+            def delete():
+                return self.deleter(request)
+
         return c
 
     def contains(self, request: 'Request'):
         return request.adaptor.in_context(self.key)
 
-    def get(self, request: 'Request'):
-        r = unprovided
+    def getter(self, request: 'Request', field=None, default=unprovided):
+        r = default
         if self.contains(request):
             r = request.adaptor.get_context(self.key)
-        else:
+        elif unprovided(r):
             if callable(self.factory):
                 r = self.factory(request)
             if unprovided(r):
                 if callable(self.default):
                     r = self.default()
                 else:
                     r = self.default
-        if self.cached:
-            self.set(request, r)
+        if self.cached and not unprovided(r):
+            self.setter(request, r)
         return r
 
-    @awaitable(get)
-    async def get(self, request: 'Request'):
-        r = unprovided
+    @awaitable(getter)
+    async def getter(self, request: 'Request', field=None, default=unprovided):
+        r = default
         if self.contains(request):
             r = request.adaptor.get_context(self.key)
-        else:
+        elif unprovided(r):
             if callable(self.factory):
                 r = self.factory(request)
                 if inspect.isawaitable(r):
                     r = await r
             if unprovided(r):
                 if callable(self.default):
                     r = self.default()
+                    if inspect.isawaitable(r):
+                        r = await r
                 else:
                     r = self.default
             # else:
             #     raise KeyError(f'context: {repr(self.key)} missing')
-        if self.cached:
-            self.set(request, r)
+        if self.cached and not unprovided(r):
+            self.setter(request, r)
         return r
 
-    def set(self, request: 'Request', value):
+    def setter(self, request: 'Request', value, field=None):
+        if self.static and self.contains(request):
+            return
         request.adaptor.update_context(**{self.key: value})
 
-    def clear(self, request: 'Request'):
+    def deleter(self, request: 'Request', field=None):
+        if self.static and self.contains(request):
+            return
         request.adaptor.delete_context(self.key)
 
     def register_factory(self, func, force: bool = False):
         if self.factory:
             if self.factory != func:
                 if force:
                     raise ValueError(f'factory conflicted: {func}, {self.factory}')
@@ -103,7 +120,10 @@
 data = RequestContextVar('_data', cached=True)      # parsed str/dict data
 # variable context var
 time = RequestContextVar('_time', factory=lambda request: request.adaptor.time, static=True)
 path_params = RequestContextVar('_path_params', default=dict)
 allow_methods = RequestContextVar('_allow_methods', default=list)
 allow_headers = RequestContextVar('_allow_headers', default=list)
 unmatched_route = RequestContextVar('_unmatched_route', factory=lambda request: request.adaptor.route)
+operation_names = RequestContextVar('_operation_names', default=list)
+# all the passing-by route's name, to combine the endpoint operationId
+endpoint_ref = RequestContextVar('_endpoint_ref', default=None)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/aiohttp.py` & `utilmeta-2.5.2/utilmeta/core/request/backends/aiohttp.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,19 +28,25 @@
     def encoded_path(self):
         return self.request.path_qs
 
     @property
     def headers(self):
         return self.request.headers
 
+    @property
+    def cookies(self):
+        return self.request.cookies
+
     def get_form(self):
         return async_to_sync(self.request.post)()
 
     @property
     def body(self):
+        if 'body' in self.__dict__:
+            return self.__dict__.get('body')
         return async_to_sync(self.async_read)()
 
     async def async_load(self):
         try:
             if self.form_type:
                 return await self.request.post()
             elif self.json_type:
@@ -48,15 +54,15 @@
             elif self.text_type:
                 return await self.request.text()
             self.__dict__['body'] = await self.request.read()
             return self.get_content()
         except NotImplementedError:
             raise
         except Exception as e:
-            raise exc.UnprocessableEntity(f'process request body failed with error: {e}')
+            raise exc.UnprocessableEntity(f'process request body failed with error: {e}') from e
 
     async def async_read(self):
         return await self.request.read()
 
     def __init__(self, request: Request):
         super().__init__(request)
         self.request = request
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/request/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from urllib.parse import urlsplit, urlunsplit
 from typing import Optional
 from utilmeta.utils import MetaMethod, CommonMethod, Header, \
-    RequestType, cached_property, time_now, gen_key
+    RequestType, cached_property, time_now, gen_key, parse_query_string
 from utilmeta.utils import exceptions as exc
 from utilmeta.utils import LOCAL_IP
+from utilmeta.core.file import File
 from ipaddress import ip_address
 from utilmeta.utils.adaptor import BaseAdaptor
 import json
 from collections.abc import Mapping
+import io
 
 
 def get_request_ip(headers: Mapping):
     ips = [*headers.get('x-forwarded-for', '').replace(' ', '').split(','),
            headers.get('remote-addr')]
     if '' in ips:
         ips.remove('')
@@ -144,16 +146,15 @@
 
     @property
     def query_string(self):
         return urlsplit(self.url).query
 
     @property
     def query_params(self):
-        from urllib.parse import parse_qs
-        return parse_qs(self.query_string)
+        return parse_query_string(self.query_string)
 
     @property
     def cookies(self):
         raise NotImplementedError
 
     @property
     def headers(self):
@@ -215,21 +216,15 @@
     def get_xml(self):
         from xml.etree.ElementTree import XMLParser
         parser = XMLParser()
         parser.feed(self.body)
         return parser.close()
 
     def get_file(self):
-        raise NotImplementedError
-        # from utilmeta.utils.media import File
-        # from io import BytesIO
-        # return File(
-        #     file=BytesIO(self.body),
-        #     name=self.gen_file_name(self.content_type)
-        # )
+        return File(io.BytesIO(self.body))
 
     def get_form(self):
         raise NotImplementedError
 
     def get_text(self):
         return self.body.decode()
 
@@ -244,15 +239,15 @@
             name = f'{maj}_{date_str}_{key}.{sec}'
         else:
             name = f'file_{date_str}_{key}'
         return name
 
     def get_content(self):
         if not self.content_type:
-            return None
+            return self.body
         if self.json_type:
             return self.get_json()
         elif self.form_type:
             return self.get_form()
         elif self.file_type:
             return self.get_file()
         elif self.xml_type:
@@ -278,22 +273,26 @@
         except Exception as e:
             raise exc.UnprocessableEntity(f'process request body failed with error: {e}')
 
     @property
     def body(self) -> bytes:
         raise NotImplementedError
 
+    @body.setter
+    def body(self, data):
+        raise NotImplementedError
+
     async def async_load(self):
         self.__dict__['body'] = await self.async_read()
         try:
             return self.get_content()
         except NotImplementedError:
             raise
         except Exception as e:
-            raise exc.UnprocessableEntity(f'process request body failed with error: {e}')
+            raise exc.UnprocessableEntity(f'process request body failed with error: {e}') from e
 
     async def async_read(self):
         raise NotImplementedError
 
     def close(self):
         pass
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/django.py` & `utilmeta-2.5.2/utilmeta/core/request/backends/django.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import io
+
 from .base import RequestAdaptor
 from django.http.request import HttpRequest
 from django.middleware.csrf import CsrfViewMiddleware, get_token
-from utilmeta.utils import parse_query_dict, cached_property, Header, LOCAL_IP
+from utilmeta.utils import parse_query_dict, cached_property, Header, LOCAL_IP, multi, exceptions
 from ipaddress import ip_address
 from utilmeta.core.file.backends.django import DjangoFileAdaptor
 from utilmeta.core.file.base import File
 import django
 
 
 def get_request_ip(meta: dict):
@@ -38,15 +40,19 @@
     def request_method(self):
         return self.request.method
 
     @cached_property
     def url(self):
         if hasattr(self.request, 'get_raw_uri'):
             return self.request.get_raw_uri()
-        self.request.build_absolute_uri()
+        return self.request.build_absolute_uri()
+
+    @property
+    def path(self):
+        return self.request.path
 
     @cached_property
     def address(self):
         return get_request_ip(self.request.META)
 
     @classmethod
     def load_form_data(cls, request):
@@ -65,21 +71,30 @@
                 load_call()
                 request.META['REQUEST_METHOD'] = m
 
     def get_form(self):
         self.load_form_data(self.request)
         data = parse_query_dict(self.request.POST)
         parsed_files = {}
-        for key, files in self.request.FILES.items():
-            parsed_files[key] = [File(self.file_adaptor_cls(file)) for file in files]
+        for key in self.request.FILES:
+            files = self.request.FILES.getlist(key)
+            if multi(files):
+                parsed_files[key] = [File(self.file_adaptor_cls(file)) for file in files]
+            else:
+                parsed_files[key] = File(self.file_adaptor_cls(files))
         data.update(parsed_files)
         return data
 
     async def async_load(self):
-        raise NotImplementedError
+        try:
+            return self.get_content()
+        except NotImplementedError:
+            raise
+        except Exception as e:
+            raise exceptions.UnprocessableEntity(f'process request body failed with error: {e}') from e
 
     async def async_read(self):
         # from django.core.handlers.asgi import ASGIRequest
         # if isinstance(self.request, ASGIRequest):
         #     return self.request.read()
         return self.body
         # not actually "async", but could be used from async server
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/sanic.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/aiohttp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,76 @@
-from sanic.request import Request
-from .base import RequestAdaptor
-import sanic
+from aiohttp.client_reqrep import ClientResponse
+from aiohttp.web_response import Response as ServerResponse
+# from utilmeta.utils import async_to_sync
+from .base import ResponseAdaptor
 
 
-class SanicRequestAdaptor(RequestAdaptor):
-    backend = sanic
+class AiohttpClientResponseAdaptor(ResponseAdaptor):
+    response: ClientResponse
 
-    def gen_csrf_token(self):
-        pass
+    @classmethod
+    def qualify(cls, obj):
+        return isinstance(obj, ClientResponse)
 
-    def check_csrf_token(self) -> bool:
-        pass
+    @property
+    def status(self):
+        return self.response.status
 
     @property
-    def address(self):
-        return self.request.remote_addr
+    def reason(self):
+        return self.response.reason
 
     @property
-    def cookies(self):
-        return self.request.cookies
+    def headers(self):
+        return self.response.headers
 
-    def get_form(self):
-        form = dict(self.request.form)
-        form.update(self.request.files)
-        return form
+    @property
+    def body(self) -> bytes:
+        return getattr(self.response, '_body', None)
 
-    async def async_read(self):
-        await self.request.receive_body()
-        return self.body
+    async def async_read(self) -> bytes:
+        return await self.response.read()
 
-    request: Request
+    async def async_load(self):
+        if self.text_type:
+            return await self.response.text()
+        elif self.json_type:
+            return await self.response.json()
+        self.__dict__['body'] = await self.async_read()
+        return self.get_content()
 
     @property
-    def request_method(self):
-        return self.request.method
+    def cookies(self):
+        return self.response.cookies
+
+    def close(self):
+        if isinstance(self.response, ClientResponse):
+            pass
+        self.response.close()
+
+
+class AiohttpServerResponseAdaptor(ResponseAdaptor):
+    response: ServerResponse
+
+    @classmethod
+    def qualify(cls, obj):
+        return isinstance(obj, ServerResponse)
 
     @property
-    def url(self):
-        return self.request.url
+    def status(self):
+        return self.response.status
 
     @property
-    def body(self):
-        return self.request.body
+    def reason(self):
+        return self.response.reason
 
     @property
     def headers(self):
-        return self.request.headers
+        return self.response.headers
 
     @property
-    def query_string(self):
-        return self.request.query_string
+    def body(self) -> bytes:
+        return self.response.body
+
+    @property
+    def cookies(self):
+        return self.response.cookies
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/starlette.py` & `utilmeta-2.5.2/utilmeta/core/request/backends/starlette.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,38 +73,46 @@
             return path + '?' + query
         return path
 
     @property
     def headers(self):
         return self.request.headers
 
+    @property
+    def body(self) -> bytes:
+        if 'body' in self.__dict__:
+            return self.__dict__['body']
+        return async_to_sync(self.async_read)()
+
+    async def async_read(self):
+        return await self.request.body()
+
     def get_form(self):
         return self.process_form(async_to_sync(self.request.form)())
 
     def process_form(self, data: FormData):
         form = {}
+        result = {}
         for key, value in data.multi_items():
             if isinstance(value, UploadFile):
                 value = File(self.file_adaptor_cls(value))
             form.setdefault(key, []).append(value)
-        return form
-
-    @property
-    def body(self) -> bytes:
-        return async_to_sync(self.async_read)()
-
-    async def async_read(self):
-        return await self.request.body()
+        for key, val in form.items():
+            if len(val) == 1:
+                result[key] = val[0]
+            else:
+                result[key] = val
+        return result
 
     async def async_load(self):
         try:
             if self.form_type:
                 data = await self.request.form()
                 return self.process_form(data)
             if self.json_type:
                 return await self.request.json()
             self.__dict__['body'] = await self.request.body()
             return self.get_content()
         except NotImplementedError:
             raise
         except Exception as e:
-            raise exc.UnprocessableEntity(f'process request body failed with error: {e}')
+            raise exc.UnprocessableEntity(f'process request body failed with error: {e}') from e
```

### Comparing `utilmeta-2.4.1/utilmeta/core/request/backends/tornado.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/werkzeug.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-from tornado.httpserver import HTTPRequest as ServerRequest
-# from tornado.httpclient import HTTPRequest as ClientRequest
-from ..base import RequestAdaptor
-from utilmeta.core.file.backends.tornado import TornadoFileAdaptor
-from utilmeta.core.file.base import File
-import tornado
+from .base import ResponseAdaptor
+from werkzeug.wrappers import Response as WerkzeugResponse
+from typing import Union
 
 
-class TornadoServerRequestAdaptor(RequestAdaptor):
-    request: ServerRequest
-    file_adaptor_cls = TornadoFileAdaptor
-    backend = tornado
+class WerkzeugResponseAdaptor(ResponseAdaptor):
+    response: WerkzeugResponse
 
     @classmethod
-    def reconstruct(cls, adaptor: 'RequestAdaptor') -> ServerRequest:
-        if isinstance(adaptor, cls):
-            return adaptor.request
-        raise ServerRequest(
-            method=adaptor.method,
-            uri=adaptor.url,
-            headers=adaptor.headers,
-            body=adaptor.body,
+    def reconstruct(cls, resp: Union['ResponseAdaptor', 'WerkzeugResponse']):
+        from utilmeta.core.response import Response
+
+        if isinstance(resp, ResponseAdaptor):
+            resp = Response(response=resp)
+        elif not isinstance(resp, Response):
+            resp = Response(resp)
+
+        response = WerkzeugResponse(
+            resp.body,
+            status=resp.status,
+            headers=resp.prepare_headers(),
+            content_type=resp.content_type,
         )
+        return response
 
-    @property
-    def request_method(self):
-        return self.request.method
+    @classmethod
+    def qualify(cls, obj):
+        return isinstance(obj, WerkzeugResponse)
 
     @property
-    def url(self):
-        return self.request.full_url()
+    def status(self):
+        return self.response.status_code
 
     @property
-    def body(self):
-        return self.request.body
+    def reason(self):
+        return ''
 
     @property
     def headers(self):
-        return self.request.headers
+        return self.response.headers
 
     @property
-    def query_params(self):
-        return self.request.query_arguments
+    def body(self) -> bytes:
+        return self.response.data
 
-    def get_form(self):
-        form = dict(self.request.body_arguments)
-        parsed_files = {}
-        for key, files in self.request.files.items():
-            parsed_files[key] = [File(self.file_adaptor_cls(file)) for file in files]
-        form.update(parsed_files)
-        return form
+    def close(self):
+        self.response.close()
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/base.py` & `utilmeta-2.5.2/utilmeta/core/response/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import io
 import json
 from http.cookies import SimpleCookie
 from utilmeta.core.request import Request
 from utype.types import *
 from utilmeta.utils import Header,\
     get_generator_result, get_doc, is_hop_by_hop, http_time, file_like, \
     STATUS_WITHOUT_BODY, time_now
@@ -11,14 +12,15 @@
 from .backends.base import ResponseAdaptor
 from utilmeta.utils.error import Error
 from utype.parser.cls import ClassParser
 from utype.utils.functional import get_obj_name
 import utype
 import re
 from ..file.base import File
+# from utype.parser.rule import LogicalType
 
 
 class ResponseClassParser(ClassParser):
     NAMES = ('result', 'headers')
 
     @classmethod
     def validate_field_name(cls, name: str):
@@ -52,15 +54,15 @@
     # when response is json type and __params__ specified result is the inner result key
     # otherwise result is an alias of data, but often be inherited and annotated
     strict: bool = None
 
     status: int = None
     reason: str = None
     charset: str = None
-    content_type: str = None
+    content_type: Optional[str] = None
     headers: Headers        # can be any inherited map, or assign to a HeadersSchema
     cookies: SimpleCookie
     name: str = None
     description: str = None
 
     wrapped: bool = False
 
@@ -130,18 +132,29 @@
                  file=None,
                  # metadata
                  mocked: bool = False,
                  cached: bool = False,
                  timeout: bool = False,
                  aborted: bool = False,
                  # when timeout set to True, raw_response is None
-                 stack: list = None
+                 stack: list = None,
+                 strict: bool = None
                  ):
 
-        self.adaptor = ResponseAdaptor.dispatch(response) if response else None
+        self.adaptor = None
+
+        if response:
+            if isinstance(response, ResponseAdaptor):
+                self.adaptor = response
+            elif isinstance(response, Response):
+                self.adaptor = response.adaptor
+                request = request or response.request
+            else:
+                self.adaptor = ResponseAdaptor.dispatch(response)
+
         self._request = request
         self._content = content
         self._extra = extra
 
         if self.adaptor:
             status = status or self.adaptor.status
             reason = reason or self.adaptor.reason
@@ -154,14 +167,17 @@
         self.status = status or self.status
         self.charset = charset or self.charset
         self.content_type = content_type or self.content_type
         self.state = state or self.state
         self.message = message
         self.count = count
 
+        if strict is not None:
+            self.strict = strict
+
         self.init_headers(headers)
         self.cookies = SimpleCookie(cookies or {})
 
         self._cached = cached
         self._mocked = mocked
         # this is just a lazy shortcut that does not deal with TimeoutError
         self._timeout = timeout
@@ -172,59 +188,65 @@
         # 2. response: 301 (redirect2)
         # 3. response: retry 1
         # 4. response: retry 2
         self._stack = stack
 
         self._file = None
         self._error = None
+        self._traffic = None
         self._setup_time = time_now()
 
-        self.init_error(error)
-        self.init_result(result)
-        self.init_file(file)
+        if not self.adaptor:
+            self.init_error(error)
+            self.init_result(result)
+            self.init_file(file)
 
         self.parse_headers()
+
         self.status = self.status or 200
         # default status is 200
         if self.state is None:
             self.state = 1 if self.success else 0
         # set default state after status
 
-        # build content at last
-        self.build_content()
-
         # represent the loaded data
         self._data = None
 
+        # build content at last
+        self.build_content()
+
     def __contains__(self, item):
         return item in self.headers
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def close(self):
-        return self.adaptor.close()
+        if self.adaptor:
+            self.adaptor.close()
 
     def parse_content(self):
         if self.result is not None:
             return
         if isinstance(self._content, dict) and self.wrapped:
             if self.result_key:
-                self.result = self._content.get(self.result_key, self._content)
+                self.init_result(
+                    self._content.get(self.result_key, self._content)
+                )
             if self.message_key:
                 self.message = self._content.get(self.message_key)
             if self.state_key:
                 self.state = self._content.get(self.state_key)
             if self.count_key:
                 self.count = self._content.get(self.count_key)
         else:
-            self.result = self._content
+            self.init_result(self._content)
 
     def match(self):
         if not self.adaptor:
             return True
         if self.__class__.status and self.__class__.status != self.status:
             return False
         if self.__class__.state and self.__class__.state != self.state:
@@ -263,17 +285,21 @@
 
         if self.strict:
             field = self.__parser__.fields.get('result')
             if field:
                 result = field.parse_value(result, context=self.__parser__.options.make_context())
 
         if not self.adaptor and self._response_like(result):
-            self.adaptor = ResponseAdaptor.dispatch(result)
-            self.result = None
-            return
+            try:
+                self.adaptor = ResponseAdaptor.dispatch(result)
+                self.result = None
+                return
+            except NotImplementedError:
+                # continue: this is not a response
+                pass
 
         if file_like(result):
             self.init_file(result)
             return
 
         self.result = result
 
@@ -318,31 +344,38 @@
             if self.count_key:
                 data[self.count_key] = self.count or 0
             return data
         else:
             data = self.result
         return data
 
+    # async def async_load(self):
+    #     if self.adaptor:
+    #         self._content = await self.adaptor.async_load()
+    #         self.parse_content()
+
     def build_content(self):
         if self._content is not None:
             return
         if self.adaptor:
             self._content = self.adaptor.get_content()
             self.parse_content()
             return
         if self.status in STATUS_WITHOUT_BODY:
+            self.content_type = None
             return
         if self._file:
             self._content = self._file
             return
         data = self.build_data()
         if hasattr(data, '__iter__') and not isinstance(data, (bytes, memoryview, str, list, dict)):
             # must convert to list iterable
             # this data is guarantee that not file_like
             data = list(data)
+        # self._data = data
         if data is None or data == '':
             data = b''
         self._content = data
         self.build_content_type()
 
     def build_content_type(self):
         if self.content_type is not None:
@@ -359,26 +392,28 @@
         elif isinstance(self._content, str):
             self.content_type = PLAIN
         elif isinstance(self._content, bytes) or file_like(self._content):
             self.content_type = OCTET_STREAM
 
     @property
     def data(self):
-        if self._data:
-            return self._data
-        data = self.body
-        if not data:
+        if not self._content:
             return None
         if self.content_type:
             if self.content_type.startswith(JSON):
-                data = json.loads(data)
-            elif self.content_type.startswith('text/'):
-                data = data.decode(errors='ignore')
-        self._data = data
-        return data
+                if self._data:
+                    return self._data
+                self._data = json.loads(self.dump_json())
+                return self._data
+        if isinstance(self._content, io.BytesIO):
+            self._content.seek(0)
+            data = self._content.read()
+            self._content.seek(0)
+            return data
+        return self._content
 
     # @classmethod
     # def get_data(cls, resp: 'Response'):
     #     body = resp.body
     #     if not body:
     #         return None
     #     if resp.content_type:
@@ -387,15 +422,16 @@
     #         elif resp.content_type.startswith('text/'):
     #             return body.decode(errors='ignore')
     #     return body
 
     def __str__(self):
         reason = f' {self.reason}' if self.reason else ''
         return f'{self.__class__.__name__} [{self.status}{reason}] ' \
-               f'"{self.request.method.upper()} /%s"' % self.request.encoded_path.strip('/') if self.request else ''
+               f'"{self.request.method.upper()} /%s"' % self.request.encoded_path.strip('/') \
+            if self.request else f'{self.__class__.__name__} [{self.status}{reason}]'
 
     def __repr__(self):
         return self.__str__()
 
     def print(self):
         print(str(self))
         content_type = self.content_type or self.headers.get('content-type')
@@ -501,15 +537,18 @@
 
     @property
     def language(self):
         return self.headers.get(Header.CONTENT_LANGUAGE)
 
     @property
     def content_length(self):
-        return self.headers.get(Header.LENGTH)
+        if self.adaptor:
+            if Header.LENGTH in self.adaptor.headers:
+                return int(self.adaptor.headers.get(Header.LENGTH) or 0)
+        return int(self.headers.get(Header.LENGTH) or 0)
 
     @property
     def count(self):
         return self._count
 
     @count.setter
     def count(self, val: int):
@@ -521,16 +560,16 @@
 
     @message.setter
     def message(self, val):
         self._message = val
 
     @property
     def file(self):
-        if self.adaptor:
-            return self.adaptor.get_file()
+        # if self.adaptor:
+        #     return self.adaptor.get_file()
         return self._file
 
     @file.setter
     def file(self, file):
         self.init_file(file)
 
     @property
@@ -604,36 +643,35 @@
         header_values = []
         for key, val in self.headers.items():
             if self.adaptor and is_hop_by_hop(key):
                 continue
             if str(key).lower() == 'content-type':
                 with_content_type = False
             header_values.append((str(key), str(val)))
-        if with_content_type and self.content_type:
+        if with_content_type and self.content_type and self._content:       # non empty
             content_type = self.content_type
             if content_type and self.charset:
                 content_type = f'{content_type}; charset={self.charset}'
             header_values.append(('Content-Type', content_type))
         for cookie in self.cookies.values():
             header_values.append(('Set-Cookie', cookie.OutputString()))
         return header_values
 
     def prepare_body(self):
         if self.adaptor:
             return self.adaptor.body
         if self._file:
             return self._file
+        if not self._content:
+            return b''
         if self.content_type and self.content_type.startswith(JSON):
             return self.dump_json()
         # this content might not be bytes, leave the encoding to the adaptor
         return self._content
 
-    async def load(self):
-        await self.adaptor.async_load()
-
     @property
     def body(self) -> bytes:
         if self.adaptor:
             return self.adaptor.body
         body = self.prepare_body()
         if hasattr(body, 'read'):
             return body.read()      # noqa
@@ -641,36 +679,56 @@
             return body
         if not isinstance(body, str):
             body = str(body)
         return body.encode(self.charset or 'utf-8', errors='replace')
 
     @property
     def error(self) -> Optional[Error]:
-        if self.success:
-            return None
+        return self._error
+
+    @error.setter
+    def error(self, e):
+        self.init_error(e)
+
+    def get_error(self):
         if self._error:
             return self._error
+        if self.success:
+            return None
         e = exc.HttpError.STATUS_EXCEPTIONS.get(self.status, exc.ServerError)(self.message)
         return Error(e)
 
-    @error.setter
-    def error(self, e):
-        self.init_error(e)
+    @property
+    def traffic(self):
+        if self._traffic:
+            return self._traffic
+        value = 12      # HTTP/1.1 200 OK
+        value += len(str(self.status)) + len(str(self.reason or 'ok'))
+        value += self.content_length or 0
+        for key, val in self.headers.items():
+            value += len(str(key)) + len(str(val)) + 4
+        self._traffic = value
+        return value
 
     def throw(self):
-        err = self.error
+        err = self.get_error()
         if err:
             raise err.throw()
 
-    def valid(self, *_, **__):
-        return self.success
+    # def valid(self, *_, **__):
+    #     return self.success
 
     @classmethod
     def mock(cls):
-        pass
+        from utype.utils.example import get_example_from_parser
+        parser = getattr(cls, '__parser__', None)
+        kwargs = {}
+        if parser:
+            kwargs = get_example_from_parser(parser)
+        return cls(**kwargs)
 
     @property
     def success(self):
         if not self.status:
             return False
         if self.status >= 400:
             return False
@@ -744,10 +802,12 @@
             self.headers["Vary"] = ", ".join(vary_headers)
 
 
 @utype.register_transformer(Response)
 def transform_response(transformer, resp, cls):
     if isinstance(resp, ResponseAdaptor):
         resp = cls(response=resp)
-    elif not isinstance(resp, Response):
-        resp = cls(resp)
-    return resp
+    elif isinstance(resp, Response):
+        if isinstance(resp, cls):
+            return resp
+        return cls(response=resp, request=resp.request, strict=True)
+    return cls(resp)
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/aiohttp.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/requests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,36 @@
-from aiohttp.client_reqrep import ClientResponse
-from aiohttp.web_response import Response as ServerResponse
-from utilmeta.utils import async_to_sync
+from requests import Response
+from typing import Union
 from .base import ResponseAdaptor
 
 
-class AiohttpClientResponseAdaptor(ResponseAdaptor):
-    response: ClientResponse
+class RequestsResponseAdaptor(ResponseAdaptor):
+    response: Response
 
     @classmethod
     def qualify(cls, obj):
-        return isinstance(obj, ClientResponse)
+        return isinstance(obj, Response)
 
     @property
     def status(self):
-        return self.response.status
+        return self.response.status_code
 
     @property
     def reason(self):
         return self.response.reason
 
     @property
     def headers(self):
         return self.response.headers
 
     @property
     def body(self) -> bytes:
-        return async_to_sync(self.response.read)()
+        return self.response.content
 
-    async def async_read(self) -> bytes:
-        return await self.response.read()
+    def get_text(self) -> str:
+        return self.response.text
 
-    async def async_load(self):
-        if self.text_type:
-            return await self.response.text()
-        elif self.json_type:
-            return await self.response.json()
-        self.__dict__['body'] = await self.async_read()
-        return self.get_content()
-
-    @property
-    def cookies(self):
-        return self.response.cookies
+    def get_json(self, **kwargs) -> Union[dict, list]:
+        return self.response.json(**kwargs)
 
     def close(self):
-        if isinstance(self.response, ClientResponse):
-            pass
         self.response.close()
-
-
-class AiohttpServerResponseAdaptor(ResponseAdaptor):
-    response: ServerResponse
-
-    @classmethod
-    def qualify(cls, obj):
-        return isinstance(obj, ServerResponse)
-
-    @property
-    def status(self):
-        return self.response.status
-
-    @property
-    def reason(self):
-        return self.response.reason
-
-    @property
-    def headers(self):
-        return self.response.headers
-
-    @property
-    def body(self) -> bytes:
-        return self.response.body
-
-    @property
-    def cookies(self):
-        return self.response.cookies
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,28 +87,35 @@
         return content_type.startswith('text')
 
     @property
     def file_type(self):
         content_type = self.content_type
         if not content_type:
             return False
-        maj, sec = content_type.split('/')
+        if '/' not in content_type:
+            return False
+        try:
+            maj, sec = content_type.split('/')
+        except ValueError:
+            return False
         if maj in ('video', 'audio', 'image'):
             return True
         if sec == 'octet-stream':
             return True
         return False
 
     def get_content(self):
         """
         Parsed content:
         text/*           : str
         application/json : dict/list
         image/*          : Image
         """
+        if not self.content_type:
+            return None
         if self.json_type:
             return self.get_json()
         elif self.xml_type:
             return self.get_xml()
         elif self.file_type:
             return self.get_file()
         elif self.text_type:
@@ -120,18 +127,21 @@
         return BytesIO(self.body)
         # from utilmeta.utils.media import File
         # return File(file=BytesIO(self.body))
 
     def get_text(self) -> str:
         return self.body.decode(encoding=self.charset or 'utf-8', errors='replace')
 
-    def get_json(self) -> Union[dict, list]:
+    def get_json(self) -> Union[dict, list, None]:
         text = self.get_text()
         import json
-        return json.loads(text, cls=self.json_decoder_cls)
+        try:
+            return json.loads(text, cls=self.json_decoder_cls)
+        except json.decoder.JSONDecodeError:
+            return None
 
     def get_xml(self):
         from xml.etree.ElementTree import XMLParser
         parser = XMLParser()
         parser.feed(self.body)
         return parser.close()
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/django.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/django.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,18 @@
             status=resp.status,
             reason=resp.reason,
             content_type=resp.content_type,
             charset=resp.charset,
             headers=resp.prepare_headers()
         )
         if resp.file:
-            return FileResponse(resp.file, **kwargs)
-        return HttpResponse(resp.body, **kwargs)
+            response = FileResponse(resp.file, **kwargs)
+        else:
+            response = HttpResponse(resp.body, **kwargs)
+        return response
 
     @property
     def status(self):
         return self.response.status_code
 
     @property
     def reason(self):
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/httpx.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/httpx.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/sanic.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/sanic.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     def headers(self):
         return self.response.headers
 
     @property
     def body(self):
         return self.response.body
 
-    @property
-    def cookies(self):
-        return self.response.cookies
+    # @property
+    # def cookies(self):
+    #     return self.response.cookies
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/starlette.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/starlette.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,21 +47,20 @@
 
     @property
     def headers(self):
         return self.response.headers
 
     @property
     def body(self):
-        return self.response.body
+        # StreamResponse does not have body attribute
+        return getattr(self.response, 'body', b'')
 
     @property
     def cookies(self):
         from http.cookies import SimpleCookie
         cookies = SimpleCookie()
-        for key, value in self.response.raw_headers:
-            if key.lower() == b'set-cookie':
-                # use get_all, cause Set-Cookie can be multiple
-                cookies.load(value)
+        for cookie in self.response.headers.getlist('set-cookie'):
+            cookies.load(cookie)
         return cookies
 
     def close(self):
         pass
```

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/tornado.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/tornado.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/core/response/backends/urllib.py` & `utilmeta-2.5.2/utilmeta/core/response/backends/urllib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from http.client import HTTPResponse
 from urllib.error import HTTPError
 from typing import Union
 from .base import ResponseAdaptor
+from utilmeta.utils import Headers
 
 
 class UrllibResponseAdaptor(ResponseAdaptor):
     response: Union[HTTPResponse, HTTPError]
 
     @classmethod
     def qualify(cls, obj):
@@ -17,15 +18,15 @@
 
     @property
     def reason(self):
         return self.response.reason
 
     @property
     def headers(self):
-        return dict(self.response.headers)
+        return Headers(dict(self.response.headers))
 
     @property
     def body(self):
         if self._body is not None:
             return self._body
         self._body = self.response.read()
         return self._body
```

### Comparing `utilmeta-2.4.1/utilmeta/core/server/service.py` & `utilmeta-2.5.2/utilmeta/core/server/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import warnings
 from typing import Union, Callable, Type, TypeVar, Optional
 import sys
 import os
-from utilmeta.utils import import_obj, awaitable, search_file
+from utilmeta.utils import import_obj, awaitable, search_file, cached_property
 from utilmeta.conf.base import Config
 import inspect
 from utilmeta.core.api import API
 
 # if TYPE_CHECKING:
 #     from utilmeta.core.api.specs.base import BaseAPISpec
 
@@ -22,14 +23,15 @@
         name: str,
         title: str = None,
         description: str = None,
         production: bool = None,
         host: str = None,
         port: int = None,
         scheme: str = 'http',
+        origin: str = None,
         version: Union[str, tuple] = None,
         # application=None,
         info: dict = None,
         # for document generation
         background: bool = False,
         asynchronous: bool = None,
         auto_reload: bool = None,
@@ -77,14 +79,15 @@
         self.info = info
         self.configs = {}
         self.commands = {}
         self.events = {}
         self.document = None
         # generated API document will be here
 
+        self._origin = origin
         self._application = None
         self._ready = False
 
         import utilmeta
         try:
             srv: 'UtilMeta' = utilmeta.service
         except AttributeError:
@@ -102,14 +105,34 @@
         self.adaptor: Optional[ServerAdaptor] = None
         self.set_backend(backend)
 
         self.routes = {}
 
         self._pool = None
 
+    def set_asynchronous(self, asynchronous: bool):
+        if asynchronous is None:
+            return
+        if asynchronous == self.asynchronous:
+            return
+        self.asynchronous = asynchronous
+        if self.adaptor:
+            self.adaptor.asynchronous = asynchronous
+        from utilmeta.core.orm.databases.config import DatabaseConnections
+        from utilmeta.core.cache.config import CacheConnections
+        dbs = self.get_config(DatabaseConnections)
+        if dbs:
+            for alias, database in dbs.databases.items():
+                database.apply(alias, asynchronous)
+        caches = self.get_config(CacheConnections)
+        if caches:
+            for alias, cache in caches.caches.items():
+                cache.apply(alias, asynchronous)
+        # fixme: other config that dependent on asynchronous
+
     def set_backend(self, backend):
         if not backend:
             return
 
         from utilmeta.core.server.backends.base import ServerAdaptor
 
         backend_version = None
@@ -146,20 +169,27 @@
         self.backend = backend
         self.backend_name = backend_name
         self.backend_version = backend_version
 
         if application:
             self._application = application
 
-        if not self.adaptor:
-            self.adaptor = ServerAdaptor.dispatch(self)
-            self.port = self.port or self.adaptor.DEFAULT_PORT
+        if self.adaptor:
+            if self._application and self.adaptor.application_cls:
+                if not isinstance(self._application, self.adaptor.application_cls):
+                    self._application = None
+
+            warnings.warn(f'Replacing server backend from [{self.adaptor.backend}] to [{self.backend_name}]')
+
+        # if not self.adaptor:
+        self.adaptor = ServerAdaptor.dispatch(self)
+        # self.port = self.port or self.adaptor.DEFAULT_PORT
 
-        if self._application and self.adaptor.application_cls:
-            if not isinstance(self._application, self.adaptor.application_cls):
+        if application and self.adaptor.application_cls:
+            if not isinstance(application, self.adaptor.application_cls):
                 raise ValueError(f'Invalid application for {repr(self.backend_name)}: {application}')
 
     def __repr__(self):
         return f'UtilMeta({repr(self.module_name)}, ' \
                f'name={repr(self.name)}, ' \
                f'backend={self.backend}, ' \
                f'version={self.version}, background={self.background})'
@@ -211,30 +241,41 @@
         if obj:
             return obj
         for cls, config in self.configs.items():
             if issubclass(cls, config_class):
                 return config
         return None
 
-    def get_client(self, live: bool = False, backend=None):
+    def get_client(self, live: bool = False, backend=None, **kwargs):
         from utilmeta.core.cli.base import Client
-        return Client(service=self, internal=not live, backend=backend)
+        return Client(service=self, internal=not live, backend=backend, **kwargs)
 
     def setup(self):
         if self._ready:
             return
+
+        # ------- EAGER ---
         for cls, config in self.configs.items():
-            if isinstance(config, Config):
+            if isinstance(config, Config) and config.__eager__:
                 config.setup(self)
+
+        # ------- COMMON ---
+        for cls, config in self.configs.items():
+            if isinstance(config, Config) and not config.__eager__:
+                config.setup(self)
+
         self._ready = True
 
     def startup(self):
         for cls, config in self.configs.items():
             if isinstance(config, Config):
-                config.on_startup(self)
+                r = config.on_startup(self)
+                if inspect.isawaitable(r):
+                    raise ValueError(f'detect awaitable config setup: {config}, you should use async '
+                                     f'backend such as starlette / sanic / tornado')
         for func in self.events.get('startup', []):
             func()
 
     @awaitable(startup)
     async def startup(self):
         for cls, config in self.configs.items():
             if isinstance(config, Config):
@@ -288,15 +329,15 @@
                 raise ValueError('Mounting applications required not-empty route')
             if not self.adaptor:
                 raise ValueError('UtilMeta: backend is required to mount applications')
             self.adaptor.mount(api, route=route)
             return
 
         if self.root_api:
-            if self.root_api != api:
+            if getattr(self.root_api, '__ref__', str(self.root_api)) != getattr(api, '__ref__', str(api)):
                 raise ValueError(f'UtilMeta: root api conflicted: {api}, {self.root_api}, '
                                  f'you can only mount a service once')
             return
         self.root_api = api
         self.root_url = str(route).strip('/')
 
     # def mount_ws(self, ws: Union[str, Callable], route: str = ''):
@@ -323,33 +364,55 @@
         print(BLUE % '|', '    version:', self.version_str)
         print(BLUE % '|', '      stage:', (BLUE % f'{DOT} production') if self.production else (GREEN % f'{DOT} debug'))
         print(BLUE % '|', '    backend:', f'{self.backend_name} ({self.backend_version})',
               (BLUE % f'| asynchronous') if self.asynchronous else '')
         print(BLUE % '|', '   base url:', f'{self.base_url}')
         print('')
 
+    def resolve_port(self):
+        print('PID:', os.getpid())
+        if self.port:
+            return
+
+        import socket
+        if self.adaptor and self.adaptor.DEFAULT_PORT:
+            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+                if s.connect_ex((self.host, self.adaptor.DEFAULT_PORT)) != 0:
+                    self.port = self.adaptor.DEFAULT_PORT
+                    return
+
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            s.bind(("127.0.0.1", 0))
+            addr = s.getsockname()
+            port = addr[1]
+            self.port = port
+            return
+
     def run(self, **kwargs):
         if not self.adaptor:
             raise NotImplementedError('UtilMeta: service backend not specified')
+        self.resolve_port()
         self.print_info()
         self.setup()
         return self.adaptor.run(**kwargs)
 
     def application(self):
         if not self.adaptor:
             raise NotImplementedError('UtilMeta: service backend not specified')
         self.setup()
         app = self.adaptor.application()
         self._application = app
         return app
 
     @property
     def origin(self):
+        if self._origin:
+            return self._origin
         host = self.host or '127.0.0.1'
-        port = self.port
+        port = self.port or (self.adaptor.DEFAULT_PORT if self.adaptor else None)
         if port == 80 and self.scheme == 'http':
             port = None
         elif port == 443 and self.scheme == 'https':
             port = None
         if port:
             host += f':{port}'
         return f'{self.scheme or "http"}://{host}'
@@ -365,10 +428,11 @@
         from utilmeta.conf.pool import ThreadPool
         pool = self.get_config(ThreadPool)
         if not pool:
             pool = ThreadPool()
         self._pool = pool
         return pool
 
-    # def generate(self, spec: Union[str, Type['BaseAPISpec']] = DEFAULT_API_SPEC):
-    #     if self.document:
-    #         return self.document
+    @cached_property
+    def ip(self):
+        from utilmeta.utils import get_server_ip
+        return get_server_ip()
```

### Comparing `utilmeta-2.4.1/utilmeta/core/server/backends/base.py` & `utilmeta-2.5.2/utilmeta/core/server/backends/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,31 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 if TYPE_CHECKING:
     from utilmeta import UtilMeta
     from utilmeta.core.api import API
-from utilmeta.utils import BaseAdaptor, exceptions
+from utilmeta.utils import BaseAdaptor, exceptions, import_obj
 import re
 import inspect
+from utilmeta.core.request import Request
+from utilmeta.core.response import Response
+import socket
+
+
+class ServiceMiddleware:
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
+        from utilmeta import service
+        self.service = service
+
+    def process_request(self, request: Request):
+        pass
+
+    def process_response(self, response: Response):
+        pass
 
 
 class ServerAdaptor(BaseAdaptor):
     # __backends_route__ = 'backends'
 
     @classmethod
     def reconstruct(cls, adaptor: 'BaseAdaptor'):
@@ -43,14 +60,15 @@
         self.root = None
         self.config = config
         self.background = config.background
         self.asynchronous = config.asynchronous
         if self.asynchronous is None:
             config.asynchronous = self.asynchronous = self.default_asynchronous
         self.proxy = None
+        self.middlewares: List[ServiceMiddleware] = []
 
     @property
     def root_pattern(self):
         if not self.config.root_url:
             return None
         return re.compile('%s/(.*)' % self.config.root_url.strip('/'))
 
@@ -86,7 +104,20 @@
     @classmethod
     def is_asgi(cls, app):
         if not inspect.isfunction(app):
             app = getattr(app, '__call__', None)
         if not app:
             return False
         return inspect.iscoroutinefunction(app)
+
+    def setup_middlewares(self):
+        raise NotImplementedError
+
+    def add_middleware(self, middleware):
+        if isinstance(middleware, str):
+            middleware = import_obj(middleware)
+        if inspect.isclass(middleware):
+            middleware = middleware()
+        if isinstance(middleware, ServiceMiddleware):
+            self.middlewares.append(middleware)
+        else:
+            raise NotImplementedError(f'middleware of {middleware} no implemented')
```

### Comparing `utilmeta-2.4.1/utilmeta/core/server/backends/starlette.py` & `utilmeta-2.5.2/utilmeta/core/server/backends/werkzeug.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,121 @@
-import starlette
-from starlette.requests import Request
-from starlette.applications import Starlette
-# from starlette.routing import Route
-from .base import ServerAdaptor
+from utilmeta.core.request.backends.werkzeug import WerkzeugRequestAdaptor
+from utilmeta.core.response.backends.werkzeug import WerkzeugResponseAdaptor
+import werkzeug
 from utilmeta.core.response import Response
-from utilmeta.core.request.backends.starlette import StarletteRequestAdaptor
-from utilmeta.core.response.backends.starlette import StarletteResponseAdaptor
-from utilmeta.core.api import API
-
+from .base import ServerAdaptor
+from werkzeug.wrappers import Request, Response
 
-class StarletteServerAdaptor(ServerAdaptor):
-    backend = starlette
-    application_cls = Starlette  # can be inherit and replace with FastAPI
-    request_adaptor_cls = StarletteRequestAdaptor
-    response_adaptor_cls = StarletteResponseAdaptor
-    default_asynchronous = True
-    DEFAULT_PORT = 8000
-    DEFAULT_HOST = '127.0.0.1'
-    HANDLED_METHODS = ["DELETE", "HEAD", "GET", "OPTIONS", "PATCH", "POST", "PUT"]
 
+class Application(object):
     def __init__(self, config):
-        super().__init__(config=config)
-        self.app = self.config._application or self.application_cls(debug=not self.config.production)
-        self._ready = False
+        pass
 
-    def adapt(self, api: 'API', route: str, asynchronous: bool = None):
-        if asynchronous is None:
-            asynchronous = self.default_asynchronous
-        self.add_api(self.app, api, asynchronous=asynchronous, route=route)
-
-    def mount(self, app, route: str):
-        if not self.is_asgi(app):
-            from starlette.middleware.wsgi import WSGIMiddleware
-            # todo: fix deprecated
-            app = WSGIMiddleware(app)
-        self.app.mount(route, app)
-
-    def setup(self):
-        # TODO: execute setup plugins
-        # self._monkey_patch()
-        if self._ready:
-            return
-        self.add_api(
-            self.app,
-            self.resolve(),
-            asynchronous=self.asynchronous,
-        )
-
-        if self.asynchronous:
-            @self.app.on_event('startup')
-            async def on_startup():
-                await self.config.startup()
-
-            @self.app.on_event('shutdown')
-            async def on_shutdown():
-                await self.config.shutdown()
-        else:
-            @self.app.on_event('startup')
-            def on_startup():
-                self.config.startup()
-
-            @self.app.on_event('shutdown')
-            def on_shutdown():
-                self.config.shutdown()
+    def dispatch_request(self, request):
+        raise ModuleNotFoundError
 
-        self._ready = True
+    def wsgi_app(self, environ, start_response):
+        request = Request(environ)
+        response = self.dispatch_request(request)
+        return response(environ, start_response)
+
+    def __call__(self, environ, start_response):
+        return self.wsgi_app(environ, start_response)
+
+
+class WerkzeugServerAdaptor(ServerAdaptor):
+    backend = werkzeug
+    request_adaptor_cls = WerkzeugRequestAdaptor
+    response_adaptor_cls = WerkzeugResponseAdaptor
+    default_asynchronous = True
+    HANDLED_METHODS = ("DELETE", "HEAD", "GET", "OPTIONS", "PATCH", "POST", "PUT")
 
-    def add_wsgi(self):
-        pass
+    def __init__(self, config):
+        super().__init__(config)
+        self.app = self.application_cls(self.config.name)
+        self._ready = False
 
-    def add_api(self, app: Starlette, utilmeta_api_class, route: str = '', asynchronous: bool = False):
-        """
-        Mount a API class
-        make sure it is called after all your fastapi route is set
-        """
-        from utilmeta.core.api.base import API
-        if not isinstance(utilmeta_api_class, type) or not issubclass(utilmeta_api_class, API):
-            raise TypeError(f'Invalid api class: {utilmeta_api_class}')
-        if route and route.strip('/'):
-            route = '/' + route.strip('/') + '/'
-        else:
-            route = '/'
-
-        # utilmeta_api_class: Type[API]
-        if asynchronous:
-            # @app.route('%s/{path:path}' % route, methods=cls.HANDLED_METHODS)
-            async def f(request: Request):
-                try:
-                    path = self.load_route(request.path_params['path'])
-                    resp = await utilmeta_api_class(
-                        self.request_adaptor_cls(request, path)
-                    )()
-                except Exception as e:
-                    resp = getattr(utilmeta_api_class, 'response', Response)(error=e)
-                return self.response_adaptor_cls.reconstruct(resp)
-        else:
-            # @app.route('%s/{path:path}' % route, methods=cls.HANDLED_METHODS)
-            def f(request: Request):
-                try:
-                    path = self.load_route(request.path_params['path'])
-                    resp = utilmeta_api_class(
-                        self.request_adaptor_cls(request, path)
-                    )()
-                except Exception as e:
-                    resp = getattr(utilmeta_api_class, 'response', Response)(error=e)
-                return self.response_adaptor_cls.reconstruct(resp)
-
-        app.add_route(
-            path='%s{path:path}' % route,
-            route=f,
-            methods=self.HANDLED_METHODS
-        )
+    @property
+    def application_cls(self):
+        class _Application(Application):
+            def dispatch_request(self, request):
+                return Response('Hello World!')
+
+            def wsgi_app(self, environ, start_response):
+                request = Request(environ)
+                response = self.dispatch_request(request)
+                return response(environ, start_response)
+
+            def __call__(self, environ, start_response):
+                return self.wsgi_app(environ, start_response)
+        return _Application
 
     def application(self):
         self.setup()
         return self.app
 
-    def run(self, **kwargs):
-        self.setup()
-        if self.background:
-            pass
-        else:
-            import uvicorn
-            uvicorn.run(
-                self.app,
-                host=self.config.host or self.DEFAULT_HOST,
-                port=self.config.port or self.DEFAULT_PORT,
-                **kwargs
-            )
+    @property
+    def root_route(self):
+        if not self.config.root_url:
+            return ''
+        return '/' + self.config.root_url.strip('/')
+    #
+    # def setup(self):
+    #     if self._ready:
+    #         return
+    #     self.add_api(
+    #         self.app,
+    #         self.resolve(),
+    #         route=self.root_route,
+    #         asynchronous=self.asynchronous
+    #     )
+    #
+    #     @self.app.after_server_start
+    #     async def startup(*_):
+    #         await self.config.startup()
+    #
+    #     @self.app.before_server_stop
+    #     async def shutdown(*_):
+    #         await self.config.shutdown()
+    #
+    #     self._ready = True
+    #
+    # def run(self, **kwargs):
+    #     self.setup()
+    #     self.app.run(
+    #         # port=self.config.port,
+    #         debug=not self.config.production,
+    #         **kwargs
+    #     )
+    #
+    # @classmethod
+    # def add_api(cls, app: Sanic, utilmeta_api_class, route: str = '', asynchronous: bool = False):
+    #     """
+    #     Mount a API class
+    #     make sure it is called after all your fastapi route is set
+    #     """
+    #     from utilmeta.core.api.base import API
+    #     if not issubclass(utilmeta_api_class, API):
+    #         raise TypeError(f'Invalid api class: {utilmeta_api_class}')
+    #
+    #     if asynchronous:
+    #         @app.route('%s/<path:path>' % route, methods=cls.HANDLED_METHODS)
+    #         async def f(request, path: str):
+    #             try:
+    #                 resp = await utilmeta_api_class(
+    #                     cls.request_adaptor_cls(request, path)
+    #                 )()
+    #             except Exception as e:
+    #                 resp = getattr(utilmeta_api_class, 'response', Response)(error=e)
+    #             return cls.response_adaptor_cls.reconstruct(resp)
+    #     else:
+    #         @app.route('%s/<path:path>' % route, methods=cls.HANDLED_METHODS)
+    #         def f(request, path: str):
+    #             try:
+    #                 resp = utilmeta_api_class(
+    #                     cls.request_adaptor_cls(request, path)
+    #                 )()
+    #             except Exception as e:
+    #                 resp = getattr(utilmeta_api_class, 'response', Response)(error=e)
+    #             return cls.response_adaptor_cls.reconstruct(resp)
+
+
```

### Comparing `utilmeta-2.4.1/utilmeta/core/server/backends/django/cmd.py` & `utilmeta-2.5.2/utilmeta/core/server/backends/django/cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 initial_file = '0001_initial'
 
 
 class DjangoCommand(BaseServiceCommand):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.settings = self.service.get_config(DjangoSettings)
-        self.settings.setup(self.service)
+        # self.settings.setup(self.service)
+        self.service.setup()        # setup here
 
     @command
     def add(self, name: str):
         """
         <name>: add an application to this service, if your service specify an <apps_dir> in config,
                 new application packages will create at there, elsewhere will create at current directory
         """
```

### Comparing `utilmeta-2.4.1/utilmeta/core/server/backends/django/settings.py` & `utilmeta-2.5.2/utilmeta/core/server/backends/django/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             # current settings module for django project
             root_urlconf: str = None,
             # current url conf (if there is an exists django project)
             secret_key: str = None,
             apps_package: str = None,
             # package ref (such as 'domain' / 'service.applications')
             apps: Union[tuple, List[str]] = (),
+            database_routers: tuple = (),
             allowed_hosts: list = (),
             middleware: Union[tuple, List[str]] = (),
             default_autofield: str = None,
             wsgi_application: str = None,
             # time_zone: str = None,
             # use_tz: bool = None,
             user_i18n: bool = None,
@@ -85,32 +86,35 @@
             extra: dict = None,
             # urlpatterns: list = None,
     ):
         super().__init__(**locals())
         self.module_name = module_name
         self.secret_key = secret_key
         self.apps_package = apps_package
-        self.apps = apps
+        self.apps = list(apps)
         self.allowed_hosts = allowed_hosts
         self.middleware = middleware
         self.root_urlconf = root_urlconf
         self.default_autofield = default_autofield
         self.wsgi_application = wsgi_application
         # self.time_zone = DEFAULT_TIME_ZONE if time_zone is None else time_zone
         # self.use_tz = DEFAULT_USE_TZ if use_tz is None else use_tz
         self.language = DEFAULT_LANGUAGE_CODE if language is None else language
         self.use_i18n = DEFAULT_USE_I18N if user_i18n is None else user_i18n
         self.append_slash = append_slash
         self.module = None
         self.url_conf = None
+        self.database_routers = list(database_routers)
         # self.urlpatterns = urlpatterns
         self._settings = {}
         self._extra_settings = extra
         self._plugin_settings = {}
 
+        self.load_apps()
+
     def register(self, plugin):
         getter = getattr(plugin, 'as_django', None)
         if callable(getter):
             plugin_settings = getter()
             if not isinstance(plugin_settings, dict):
                 raise TypeError(f'Invalid settings: {plugin_settings}')
             self._plugin_settings.update(plugin_settings)
@@ -157,22 +161,25 @@
         tag = f'{service.name}:{service.description}:{service.version}' \
               f'{service.backend_name}:{service.module_name}' \
               f'{django.__version__}{utilmeta.__version__}{sys.version}{platform.platform()}'.encode()
         return hashlib.sha256(tag).hexdigest()
 
     def load_apps(self):
         installed_apps = list(DEFAULT_APPS)
+        installed_apps.extend(self.apps)
+
         if self.apps_package:
-            # if self.apps_package == '.':
-            #     installed_apps.append(self.module.__package__)
-            # else:
             apps_path = self.apps_path
             hosted_labels = [p for p in next(os.walk(apps_path))[1] if '__' not in p]
-            installed_apps.extend([f'{self.apps_package}.{app}' for app in hosted_labels])
-        installed_apps.extend(self.apps)
+            for app in hosted_labels:
+                label = f'{self.apps_package}.{app}'
+                if label not in installed_apps:
+                    installed_apps.append(label)
+
+        self.apps = installed_apps
         return installed_apps
 
     @classmethod
     def get_cache(cls, cache: Cache):
         return {
             'BACKEND': CACHE_BACKENDS.get(cache.engine) or cache.engine,
             'LOCATION': cache.get_location(),
@@ -226,18 +233,27 @@
             service.adaptor.settings = self
             # replace settings
 
     def setup(self, service: UtilMeta):
         if self._settings:
             # already configured
             return
+
+        # print('SETUP:', service.module, self.apps)
+        # from utilmeta.ops.config import Operations
+        # ops_config = service.get_config(Operations)
+        # if ops_config:
+        #     ops_config.setup(service)
+        #     return
+
         if self.module_name:
             module = sys.modules[self.module_name]
         else:
             module = service.module
+            self.module_name = service.module_name
 
         self.module = module
         db_config = service.get_config(DatabaseConnections)
         cache_config = service.get_config(CacheConnections)
         databases = {}
         caches = {}
 
@@ -251,22 +267,31 @@
         if cache_config:
             from utilmeta.core.cache.backends.django import DjangoCacheAdaptor
             for name, cache in cache_config.caches.items():
                 if not cache.sync_adaptor_cls:
                     cache.sync_adaptor_cls = DjangoCacheAdaptor
                 caches[name] = self.get_cache(cache)
 
+        middleware = list(self.middleware or DEFAULT_MIDDLEWARE)
+        adaptor = service.adaptor
+        from .adaptor import DjangoServerAdaptor
+        if isinstance(adaptor, DjangoServerAdaptor):
+            middleware_func = adaptor.middleware_func
+            if middleware_func:
+                setattr(self.module, middleware_func.__name__, middleware_func)
+                middleware.append(f'{self.module_name}.{middleware_func.__name__}')
+
         settings = {
             'DEBUG': not service.production,
             'SECRET_KEY': self.get_secret(service),
             'BASE_DIR': service.project_dir,
-            'MIDDLEWARE': self.middleware or DEFAULT_MIDDLEWARE,
-            'INSTALLED_APPS': self.load_apps(),
+            'MIDDLEWARE': middleware,
+            'INSTALLED_APPS': self.apps,
             'ALLOWED_HOSTS': self.allowed_hosts,
-            # 'DATABASE_ROUTERS': self.routers,
+            'DATABASE_ROUTERS': self.database_routers,
             'APPEND_SLASH': self.append_slash,
             'LANGUAGE_CODE': self.language,
             'USE_I18N': self.use_i18n,
             'DEFAULT_AUTO_FIELD': self.default_autofield or DEFAULT_AUTO_FIELD,
             # 'DATABASES': databases,
             # 'CACHES': caches,
             ROOT_URLCONF: self.root_urlconf or service.module_name,
```

### Comparing `utilmeta-2.4.1/utilmeta/core/websocket/properties.py` & `utilmeta-2.5.2/utilmeta/core/websocket/properties.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/ops/models.py` & `utilmeta-2.5.2/utilmeta/ops/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,223 @@
 from django.db import models
-from utilmeta.core.orm.backends.django.models import AwaitableModel, ACASCADE
-from utilmeta.core.orm.backends.django import expressions as exp
-from django.contrib.postgres import fields
 from utype.types import *
-from utilmeta.utils import time_now
+from utilmeta.utils import time_now, convert_time
 
 
-class Supervisor(AwaitableModel):
+class Supervisor(models.Model):
+    objects = models.Manager()
+
     service = models.CharField(max_length=100)
     node_id = models.CharField(max_length=40, default=None, null=True)
 
-    name = models.CharField(max_length=64, default=None, null=True)
+    ident = models.CharField(max_length=20, default=None, null=True)
     # offline_enabled = BooleanField(default=True)
     # enable offline (ak/signature-only, no remote-auth/token-retrieve) to open resources to utilmeta ecosystem
-    backup_urls = fields.ArrayField(models.URLField(), default=list)
+    backup_urls = models.JSONField(default=list)
     # direct callback to master url, like https://utilmeta.com/api/action/backup?id=<ID> for backup node servers
     base_url = models.URLField()
     # remote_ops_api = URLField(default=None, null=True)
     # when local ops_api changed on proxy (including base_url/host altered)
     # action_token = models.CharField(max_length=64, unique=True)
     # platform can carry this token to identify itself
+    local = models.BooleanField(default=False)
+    # REMOTE FOR LOCAL NODE
 
     # <not> public actually
     public_key = models.TextField(default=None, null=True)  # used to decode token
     # None when generated as placeholder
 
-    init_token = models.CharField(max_length=200, default=None, null=True)
+    init_key = models.TextField(default=None, null=True)
     # used to identify the init add supervisor request
 
     created_time = models.DateTimeField(auto_now_add=True)
 
     ops_api = models.URLField()  # correlate with node.ops_api in platform
     # if ops_api is different from the new version ops api
     # will require an update
+    url = models.URLField(default=None, null=True)
 
     operation_timeout = models.DecimalField(max_digits=8, decimal_places=3, default=None, null=True)
-    open_scopes = fields.ArrayField(models.CharField(max_length=40), default=list)
-    disabled_scopes = fields.ArrayField(models.CharField(max_length=40), default=list)
+    # open_scopes = models.JSONField(default=list)
+    # disabled_scopes = models.JSONField(default=list)
 
     heartbeat_interval = models.PositiveIntegerField(default=None, null=True)
     # open for every request user
     latency = models.PositiveIntegerField(default=None, null=True)  # ms
 
     settings: dict = models.JSONField(default=dict)
     # heartbeat_enabled: False
     # report_enabled: true
     # notify_enabled: false
-    # instance_sync_enabled: false
-    # document_sync_enabled: false
+    # users_analytics: false
+    # endpoints_analytics: false
 
     # info = models.JSONField(default=dict)  # store backward compat information
     connected = models.BooleanField(default=False)
     disabled = models.BooleanField(default=False)
 
     # -- advanced
     alert_settings: dict = models.JSONField(default=dict)
     task_settings: dict = models.JSONField(default=dict)
     # heartbeat_settings: dict = models.JSONField(default=dict)
     aggregate_settings: dict = models.JSONField(default=dict)
 
     data = models.JSONField(default=dict)
 
+    resources_etag = models.TextField(default=None, null=True)
+    # if resources etag doesn't change
+    # there is not need to re-update
+    # etag is generated from supervisor
+
     class Meta:
-        db_table = 'supervisor'
+        db_table = 'utilmeta_supervisor'
+
+    @classmethod
+    def filter(cls, *args, **kwargs) -> models.QuerySet:
+        kwargs.update(
+            node_id__isnull=False,
+            public_key__isnull=False,
+            disabled=False
+        )
+        return cls.objects.filter(*args, **kwargs)
+
+
+class AccessToken(models.Model):
+    objects = models.Manager()
+
+    issuer = models.ForeignKey(Supervisor, related_name='access_tokens', on_delete=models.CASCADE)
+    token_id = models.CharField(max_length=200, unique=True)
+    issued_at = models.DateTimeField(default=None, null=True)
+    subject = models.CharField(max_length=500, default=None, null=True)
+    expiry_time = models.DateTimeField(default=None, null=True)
+    # clear tokens beyond the expiry time
+
+    # ACTIVITY -----------------
+    last_activity = models.DateTimeField(default=None, null=True)
+    used_times = models.PositiveIntegerField(default=0)
+    ip = models.GenericIPAddressField(default=None, null=True)
+
+    # PERMISSION ---------------
+    scope = models.JSONField(default=list)
+    # excludes = models.JSONField(default=list)
+    # readonly = models.BooleanField(default=False)
+    # -------
 
+    revoked = models.BooleanField(default=False)
+    # revoke tokens of a subject if it's permission is changed or revoked
+
+    class Meta:
+        db_table = 'utilmeta_access_token'
+
+
+class Resource(models.Model):
+    objects = models.Manager()
 
-class Resource(AwaitableModel):
     # id = models.CharField(max_length=40, primary_key=True)
     service = models.CharField(max_length=100, null=True)
     node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
     # common utils like server, service is None
     type = models.CharField(max_length=40)
-    route = models.CharField(max_length=200)
-    # <node>/type/ident
+    # server
+    # instance
+    # task
+    # endpoint
+    # table (data model)
+    # database
+    # cache
+    ident = models.CharField(max_length=200)
+    route = models.CharField(max_length=500)
+    # :type/:node/:ident
 
-    id_map = models.JSONField(default=dict)
+    remote_id = models.CharField(max_length=100, default=None, null=True)
+    # id_map = models.JSONField(default=dict)
     # supervisor: id
     # remote_id = models.CharField(max_length=40, default=None, null=True)
-    # supervisor = models.ForeignKey(Supervisor, related_name='resources', on_delete=ACASCADE)
+    # supervisor = models.ForeignKey(Supervisor, related_name='resources', on_delete=models.CASCADE)
 
     created_time = models.DateTimeField(auto_now_add=True)
-    data = models.JSONField(default=dict)
+
+    server = models.ForeignKey(
+        'self', related_name='resources',
+        on_delete=models.SET_NULL,
+        default=None, null=True
+    )
+    server_id: Optional[int]
+    data: dict = models.JSONField(default=dict)
 
     deleted = models.BooleanField(default=False)
     deprecated = models.BooleanField(default=False)
 
     class Meta:
         db_table = 'utilmeta_resource'
 
     @classmethod
     def get_current_server(cls) -> Optional['Resource']:
         from utilmeta.utils import get_server_ip
         return cls.objects.filter(
             type='server',
-            route=get_server_ip()
+            ident=get_server_ip(),
+            deleted=False
+        ).first()
+
+    @classmethod
+    def get_current_instance(cls) -> Optional['Resource']:
+        from utilmeta import service
+        return cls.objects.filter(
+            type='instance',
+            service=service.name,
+            server=cls.get_current_server(),
+            deleted=False
         ).first()
 
 
-class SystemMetrics(AwaitableModel):
+class SystemMetrics(models.Model):
+    objects = models.Manager()
+
     cpu_percent = models.DecimalField(max_digits=6, decimal_places=2, default=0.00)
     memory_percent = models.DecimalField(max_digits=6, decimal_places=2, default=0.00)
     used_memory = models.PositiveBigIntegerField(default=0)
     disk_percent = models.DecimalField(max_digits=6, decimal_places=2, default=0.00)
     file_descriptors = models.PositiveIntegerField(default=None, null=True)
     open_files = models.PositiveBigIntegerField(default=None, null=True)
     active_net_connections = models.PositiveIntegerField(default=0)
     total_net_connections = models.PositiveIntegerField(default=0)
     net_connections_info = models.JSONField(default=dict)
 
     class Meta:
         abstract = True
 
 
-class DatabaseConnection(AwaitableModel):
-    database: Resource = models.ForeignKey(Resource, related_name='database_connections', on_delete=ACASCADE)
+class DatabaseConnection(models.Model):
+    database: Resource = models.ForeignKey(Resource, related_name='database_connections', on_delete=models.CASCADE)
     # remote_id = CharField(max_length=100)
     status = models.CharField(max_length=40)
     active = models.BooleanField(default=False)
     client_addr = models.GenericIPAddressField()   # mysql use ADDR:PORT as HOST
     client_port = models.PositiveIntegerField()
     pid = models.PositiveIntegerField(default=None, null=True)
 
     query = models.TextField(default='')
     operation = models.CharField(max_length=32, default=None, null=True)
-    tables = fields.ArrayField(models.CharField(max_length=200), default=list)
+    tables = models.JSONField(default=list)
 
     backend_start = models.DateTimeField(default=None, null=True)
     transaction_start = models.DateTimeField(default=None, null=True)
     wait_event = models.TextField(default=None, null=True)
     query_start = models.DateTimeField(default=None, null=True)
     state_change = models.DateTimeField(default=None, null=True)
 
     data = models.JSONField(default=dict)
 
     class Meta:
         db_table = 'utilmeta_database_connection'
         # unique_together = ('database', 'remote_id')
 
 
-class ServiceMetrics(AwaitableModel):
+class ServiceMetrics(models.Model):
     """
     request metrics that can simply be calculated in form of incr and divide
     """
     in_traffic = models.PositiveBigIntegerField(default=0, null=True)    # in bytes
     out_traffic = models.PositiveBigIntegerField(default=0, null=True)    # in bytes
     # avg process time of requests made from this service
     outbound_requests = models.PositiveIntegerField(default=0)      # total request log count
@@ -165,23 +240,23 @@
     # avg process time of requests made from this service
 
     class Meta:
         abstract = True
 
 
 class Worker(SystemMetrics, ServiceMetrics):
-    server = models.ForeignKey(Resource, related_name='server_workers', on_delete=ACASCADE)
-    instance = models.ForeignKey(Resource, related_name='instance_workers', on_delete=ACASCADE)
+    server = models.ForeignKey(Resource, related_name='server_workers', on_delete=models.CASCADE)
+    instance = models.ForeignKey(Resource, related_name='instance_workers', on_delete=models.CASCADE)
 
     pid: int = models.PositiveIntegerField()
     memory_info = models.JSONField(default=dict)
     threads = models.PositiveIntegerField(default=0)
     start_time: datetime = models.DateTimeField(default=time_now)
     # utility = ForeignKey(ServiceUtility, related_name='workers', on_delete=SET_NULL, null=True, default=None)
-    master = models.ForeignKey('self', related_name='workers', on_delete=ACASCADE, null=True, default=None)
+    master = models.ForeignKey('self', related_name='workers', on_delete=models.CASCADE, null=True, default=None)
     connected = models.BooleanField(default=True)
     # type = ChoiceField(WorkerType.gen(), retrieve_key=False, store_key=False, default=WorkerType.common)
     time: datetime = models.DateTimeField(default=time_now)  # latest metrics update time
 
     status = models.CharField(max_length=100, default=None, null=True)
     user = models.CharField(max_length=100, default=None, null=True)
 
@@ -198,21 +273,108 @@
 
     @classmethod
     def get(cls, pid: int):
         if not pid:
             return None
         return cls.objects.filter(pid=pid, server=Resource.get_current_server()).first()
 
+    def get_sys_metrics(self):
+        import psutil
+        try:
+            process = psutil.Process(self.pid)
+        except psutil.Error:
+            return None
+        mem_info = process.memory_full_info()
+
+        try:
+            open_files = len(process.open_files())
+        except psutil.Error:
+            open_files = 0
+
+        return dict(
+            used_memory=getattr(mem_info, 'uss', getattr(mem_info, 'rss')),
+            memory_info={f: getattr(mem_info, f) for f in getattr(mem_info, '_fields')},
+            total_net_connections=len(process.connections()),
+            active_net_connections=len([c for c in process.connections() if c.status != 'CLOSE_WAIT']),
+            file_descriptors=process.num_fds() if psutil.POSIX else None,
+            cpu_percent=process.cpu_percent(interval=1),
+            memory_percent=round(process.memory_percent('uss'), 2),
+            open_files=open_files,
+            threads=process.num_threads(),
+        )
+
+    @classmethod
+    def load(cls, pid: int = None, **kwargs) -> Optional['Worker']:
+        import psutil
+        import os
+        pid = pid or os.getpid()
+        try:
+            proc = psutil.Process(pid)
+        except psutil.Error:
+            return None
+        server = Resource.get_current_server()
+        if not server:
+            return None
+        instance = Resource.get_current_instance()
+        if not instance:
+            return None
+
+        parent_pid = None
+        if proc.parent():
+            parent_pid = proc.parent().pid
+
+        data = dict(
+            start_time=convert_time(datetime.fromtimestamp(proc.create_time())),
+            user=proc.username(),
+            status=proc.status(),
+        )
+
+        data.update(kwargs)
+        master = cls.objects.filter(
+            pid=parent_pid,
+            server=server,
+            instance=instance
+        ).first()
+
+        if master:
+            data.update(master_id=master.pk)    # do not user master=
+
+        # prevent transaction
+        worker_qs = cls.objects.filter(
+            server_id=server.pk,
+            pid=pid,
+        )
+        if worker_qs.exists():
+            # IMPORTANT: update time as soon as Worker.load is triggered
+            # to provide realtime metrics for representative
+            data.update(
+                time=time_now(),
+                connected=True
+            )
+            worker_qs.update(**data)
+            return worker_qs.first()
+
+        from django.db.utils import IntegrityError
+        try:
+            return cls.objects.create(
+                server=server,
+                instance=instance,
+                pid=pid,
+                **data
+            )
+        except IntegrityError:
+            return worker_qs.first()
+
 
 class ServerMonitor(SystemMetrics):
     time = models.DateTimeField(default=time_now)
     # task_settings = ForeignKey(TaskSettings, on_delete=SET_NULL, default=None, null=True)
     layer = models.PositiveSmallIntegerField(default=0)
     interval = models.PositiveIntegerField(default=None, null=True)  # in seconds
-    server = models.ForeignKey(Resource, related_name='metrics', on_delete=ACASCADE)
+    server = models.ForeignKey(Resource, related_name='server_metrics', on_delete=models.CASCADE)
     # version = ForeignKey(VersionLog, on_delete=SET_NULL, null=True, default=None)
     load_avg_1 = models.DecimalField(max_digits=8, decimal_places=2, default=None, null=True)
     load_avg_5 = models.DecimalField(max_digits=8, decimal_places=2, default=None, null=True)
     load_avg_15 = models.DecimalField(max_digits=8, decimal_places=2, default=None, null=True)
     # alert = ForeignKey(AlertLog, related_name='source_metrics', on_delete=SET_NULL, null=True, default=None)
     metrics = models.JSONField(default=dict)
 
@@ -224,15 +386,15 @@
     def current(cls) -> Optional['ServerMonitor']:
         return cls.objects.last()   # already order by time
 
 
 class WorkerMonitor(SystemMetrics, ServiceMetrics):
     time = models.DateTimeField(default=time_now)
     interval = models.PositiveIntegerField(default=None, null=True)  # in seconds
-    worker = models.ForeignKey(Worker, related_name='metrics', on_delete=ACASCADE)
+    worker = models.ForeignKey(Worker, related_name='worker_metrics', on_delete=models.CASCADE)
     memory_info = models.JSONField(default=dict)
     threads = models.PositiveIntegerField(default=0)
     metrics = models.JSONField(default=dict)  # extra metrics
 
     class Meta:
         db_table = 'utilmeta_worker_monitor'
         ordering = ('time',)
@@ -243,15 +405,15 @@
 
 
 class InstanceMonitor(SystemMetrics, ServiceMetrics):
     time = models.DateTimeField(default=time_now)
     layer = models.PositiveSmallIntegerField(default=0)
     interval = models.PositiveIntegerField(default=None, null=True)  # in seconds
 
-    instance = models.ForeignKey(Resource, related_name='metrics', on_delete=ACASCADE)
+    instance = models.ForeignKey(Resource, related_name='instance_metrics', on_delete=models.CASCADE)
     threads = models.PositiveIntegerField(default=0)
 
     current_workers = models.PositiveIntegerField(default=0)
 
     avg_worker_lifetime = models.PositiveBigIntegerField(default=None, null=True)
     new_spawned_workers = models.PositiveBigIntegerField(default=0)
     avg_workers = models.DecimalField(default=None, null=True, max_digits=10, decimal_places=2)
@@ -259,20 +421,22 @@
     metrics = models.JSONField(default=dict)   # extra metrics
 
     class Meta:
         db_table = 'utilmeta_instance_monitor'
         ordering = ('time',)
 
 
-class DatabaseMonitor(AwaitableModel):
+class DatabaseMonitor(models.Model):
+    objects = models.Manager()
+
     time = models.DateTimeField(default=time_now)
     layer = models.PositiveSmallIntegerField(default=0)
     interval = models.PositiveIntegerField(default=None, null=True)  # in seconds
 
-    database = models.ForeignKey(Resource, on_delete=ACASCADE, related_name='database_metrics')
+    database = models.ForeignKey(Resource, on_delete=models.CASCADE, related_name='database_metrics')
 
     used_space = models.PositiveBigIntegerField(default=0)  # used disk space
     server_used_space = models.PositiveBigIntegerField(default=0)  # used disk space
     active_connections = models.PositiveBigIntegerField(default=0)
     current_connections = models.PositiveBigIntegerField(default=0)
     server_connections = models.PositiveBigIntegerField(default=0)
 
@@ -286,20 +450,22 @@
     operations = models.JSONField(default=dict)  # {'SELECT': 100, 'UPDATE': 21, ...}
 
     class Meta:
         db_table = 'utilmeta_database_monitor'
         ordering = ('time',)
 
 
-class CacheMonitor(AwaitableModel):
+class CacheMonitor(models.Model):
+    objects = models.Manager()
+
     time = models.DateTimeField(default=time_now)
     layer = models.PositiveSmallIntegerField(default=0)
     interval = models.PositiveIntegerField(default=None, null=True)  # in seconds
 
-    cache = models.ForeignKey(Resource, on_delete=ACASCADE, related_name='cache_metrics')
+    cache = models.ForeignKey(Resource, on_delete=models.CASCADE, related_name='cache_metrics')
 
     cpu_percent = models.DecimalField(max_digits=6, decimal_places=2, default=None, null=True)
     memory_percent = models.DecimalField(max_digits=6, decimal_places=2, default=None, null=True)
     used_memory = models.PositiveBigIntegerField(default=0)
     file_descriptors = models.PositiveIntegerField(default=None, null=True)
     open_files = models.PositiveBigIntegerField(default=None, null=True)
     # used_memory = PositiveBigIntegerField(default=0)
@@ -310,15 +476,15 @@
     metrics = models.JSONField(default=dict)
 
     class Meta:
         db_table = 'utilmeta_cache_monitor'
         ordering = ('time',)
 
 
-class WebMixin(AwaitableModel):
+class WebMixin(models.Model):
     """
         Log data using http/https schemes
     """
     scheme = models.CharField(default=None, null=True, max_length=20)
     method = models.CharField(default=None, null=True, max_length=20)
     # replace the unit property
     request_type = models.CharField(max_length=200, default=None, null=True)
@@ -341,18 +507,20 @@
     public = models.BooleanField(default=True)
     # public request or invoke
 
     class Meta:
         abstract = True
 
 
-class VersionLog(AwaitableModel):
+class VersionLog(models.Model):
+    objects = models.Manager()
+
     service = models.CharField(max_length=100)
     node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
-    instance: Resource = models.ForeignKey(Resource, on_delete=ACASCADE, related_name='restart_records')
+    instance: Resource = models.ForeignKey(Resource, on_delete=models.CASCADE, related_name='restart_records')
     time: datetime = models.DateTimeField(auto_now_add=True)
     # finish_time: datetime = models.DateTimeField(default=None, null=True)
     down_time = models.PositiveBigIntegerField(default=None, null=True)     # ms
     # down time, None means no down time
 
     success = models.BooleanField(default=None, null=True)
     restart_data = models.JSONField(default=dict)
@@ -383,39 +551,39 @@
     #     due = f' due to [{self.trigger_index} > {self.threshold}]' \
     #           f' (={self.trigger_value})' if self.trigger_value else ''
     #     ident = f'[{self.instance.service}]({self.instance.server.ip})'
     #     return f'{man_str} triggered {type} instance {ident} {restart}' \
     #            f'{due} at {self.time.strftime(DateFormat.DATETIME)}'
 
 
-class AlertType(AwaitableModel):
+class AlertType(models.Model):
     service = models.CharField(max_length=100)
     node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
     category = models.CharField(max_length=40)
     level = models.CharField(max_length=40)
 
     settings_id = models.CharField(max_length=40, default=None, null=True)
     # settings: AlertSettings = OneToOneField(
     #     AlertSettings, on_delete=SET_NULL, default=None, null=True, related_name='alert_type')
     threshold = models.FloatField(default=None, null=True)
     # for downgrade types, configurable
 
     subcategory = models.CharField(max_length=200)
     name = models.CharField(max_length=100)   # settings name or custom name
-    target = models.CharField(max_length=100)
+    target = models.TextField()
     # eg
     # type.category: resource_saturated
     # type.subcategory: cpu_percent_exceed
     # type.name: cpu_percent > 80
 
     # type.category: service_downgrade
     # type.subcategory: slow_response
     # type.name: Slow response at POST /api/user
 
-    ident = models.CharField(max_length=200)
+    ident = models.CharField(max_length=500)
 
     compress_window: int = models.PositiveBigIntegerField(null=True, default=None)   # seconds
     min_times: int = models.PositiveIntegerField(default=1)
 
     resource = models.ForeignKey(
         Resource, on_delete=models.SET_NULL,
         null=True, default=None, related_name='alert_types',
@@ -429,39 +597,44 @@
 
     # @classmethod
     # def get(cls, ident: str) -> Optional['AlertSettings']:
     #     from utilmeta.conf import config
     #     return cls.objects.filter(service_id=config.name, ident=ident).first()
 
 
-class AlertLog(AwaitableModel):
-    type: AlertType = models.ForeignKey(AlertType, on_delete=ACASCADE, related_name='alert_logs')
+class AlertLog(models.Model):
+    objects = models.Manager()
+
+    type: AlertType = models.ForeignKey(AlertType, on_delete=models.CASCADE, related_name='alert_logs')
     server: Resource = models.ForeignKey(
-        Resource, on_delete=ACASCADE,
-        related_name='server_alert_logs', default=None, null=True
+        Resource, on_delete=models.CASCADE,
+        related_name='server_alert_logs', default=None, null=True,
     )
     instance: Resource = models.ForeignKey(
-        Resource, on_delete=ACASCADE,
-        related_name='instance_alert_logs', default=None, null=True
+        Resource, on_delete=models.CASCADE,
+        related_name='instance_alert_logs', default=None, null=True,
     )
     version = models.ForeignKey(
         VersionLog, related_name='alert_logs',
-        on_delete=models.SET_NULL, null=True, default=None
+        on_delete=models.SET_NULL, null=True, default=None,
     )
 
     # impact_requests = models.PositiveBigIntegerField(default=None, null=True)
     # impact_users = models.PositiveIntegerField(default=None, null=True)
     # impact_ips = models.PositiveIntegerField(default=None, null=True)
     # impact services / tasks can be interfere from [server] field
 
     relieved_time = models.DateTimeField(default=None, null=True)
     # relieved_time=None (opening alert) are open for new count
 
-    trigger_times: list = fields.ArrayField(models.DateTimeField(), default=list)
-    trigger_values: list = fields.ArrayField(models.FloatField(), default=list)
+    # trigger_times: list = fields.ArrayField(models.DateTimeField(), default=list)
+    # trigger_values: list = fields.ArrayField(models.FloatField(), default=list)
+
+    trigger_times = models.JSONField(default=list)
+    trigger_values = models.JSONField(default=list)
 
     # [dict(value=<SOME_VALUE>, time=<SOME_TIME>), ...]
     time = models.DateTimeField(default=time_now)
     # start time (first alert trigger time)
     latest_time: datetime = models.DateTimeField(default=time_now)
     # latest time (latest alert trigger time)
 
@@ -498,34 +671,40 @@
             return True
         self.relieved_time = time_now()
         self.save(update_fields=['relieved_time'])
         return self.compressible        # only report legit relieve
 
 
 class ServiceLog(WebMixin):
+    objects = models.Manager()
+
     id = models.BigAutoField(primary_key=True)
 
     service = models.CharField(max_length=100)
     node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
     # supervisor.remote_id
     # node.id (in the supervisor)
     # global identifier
 
     version = models.ForeignKey(
         VersionLog, related_name='service_logs',
-        on_delete=models.SET_NULL, null=True, default=None
+        on_delete=models.SET_NULL, null=True, default=None,
     )
     instance = models.ForeignKey(
         Resource, related_name='instance_logs',
-        on_delete=models.SET_NULL, null=True, default=None
+        on_delete=models.SET_NULL, null=True, default=None,
     )
     endpoint = models.ForeignKey(
         Resource, on_delete=models.SET_NULL,
         null=True, default=None, related_name='endpoint_logs',
     )
+    # incase the endpoint not loaded yet
+    endpoint_ident = models.CharField(max_length=200, default=None, null=True)
+    endpoint_ref = models.CharField(max_length=200, default=None, null=True)
+
     # add redundant field endpoint_ident to make a quick query index and remain even after endpoint is deleted
     # endpoint_ident = models.CharField(max_length=200, null=True, default=None, db_index=True)
     # endpoint_path = URLField(default=None, null=True)
     # units = ArrayField(CharField(max_length=10), default=list)
     # the orders that the process unit is called
     worker = models.ForeignKey(
         Worker, related_name='logs',
@@ -543,32 +722,45 @@
     # thread id that handle this request / invoke
 
     user_id = models.CharField(max_length=100, null=True, default=None, db_index=True)
     # referrer = URLField(default=None, null=True)
     ip = models.GenericIPAddressField()
 
     trace = models.JSONField(default=list)
-    messages = fields.ArrayField(models.TextField(), default=list)
+    messages = models.JSONField(default=list)
 
     alert = models.ForeignKey(
         'AlertLog', related_name='service_logs',
         on_delete=models.SET_NULL, null=True, default=None,
     )
 
     volatile = models.BooleanField(default=True)
+    # deleted_time = models.DateTimeField(default=None, null=True)
+    # ----------
+    supervisor = models.ForeignKey(
+        Supervisor, related_name='logs', on_delete=models.SET_NULL,
+        default=None, null=True,
+    )
+    access_token = models.ForeignKey(
+        AccessToken, related_name='logs', on_delete=models.SET_NULL,
+        default=None, null=True,
+    )
 
     class Meta:
-        db_table = 'utilmeta_request_log'
+        db_table = 'utilmeta_service_log'
 
 
 class RequestLog(WebMixin):
+    objects = models.Manager()
+
     id = models.BigAutoField(primary_key=True)
     service = models.CharField(max_length=100)
     node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
 
+    # volatile = models.BooleanField(default=True)
     # requests made in other service request context
     time = models.DateTimeField()  # not auto_now_add, cache stored log may add after request for some time
     # version = models.ForeignKey(
     #     VersionLog, related_name='service_logs',
     #     on_delete=models.SET_NULL, null=True, default=None
     # )
 
@@ -582,17 +774,17 @@
     # request
     context_id = models.CharField(max_length=200, default=None, null=True)
     # log id / execution id
 
     host = models.URLField(default=None, null=True)      # host of the requested host (ip or domain name)
 
     remote_log = models.TextField(default=None, null=True)     # able to supply other type ident (eg. uuid)
-
     # remote utilmeta log id (in target service) to support recursive tracing
-    block = models.BooleanField(default=None, null=True)
+
+    asynchronous = models.BooleanField(default=None, null=True)
     timeout = models.DecimalField(max_digits=10, decimal_places=2, default=None, null=True)
     # SINGLE REQUEST, RETIRES NOT INCLUDED
 
     timeout_error = models.BooleanField(default=False)     # request is timeout
     server_error = models.BooleanField(default=False)     # ssl cert error when query the target host
     client_error = models.BooleanField(default=False)     # ssl cert error when query the target host
     ssl_error = models.BooleanField(default=False)     # ssl cert error when query the target host
@@ -603,39 +795,75 @@
         on_delete=models.SET_NULL, null=True, default=None,
     )
 
     class Meta:
         db_table = 'utilmeta_request_log'
 
 
-class QueryLog(AwaitableModel):
+class QueryLog(models.Model):
+    objects = models.Manager()
+
     # SLOW or error db query log
     id = models.BigAutoField(primary_key=True)
     time = models.DateTimeField()
     # version = models.ForeignKey(
     #     VersionLog, related_name='service_logs',
     #     on_delete=models.SET_NULL, null=True, default=None
     # )
-    database = models.ForeignKey(Resource, on_delete=ACASCADE, related_name='query_logs')
+    database = models.ForeignKey(
+        Resource, on_delete=models.CASCADE,
+        related_name='query_logs',
+    )
     query = models.TextField()
     duration = models.PositiveBigIntegerField(default=None, null=True)  # ms
     message = models.TextField(default='')
     worker = models.ForeignKey(
         Worker, related_name='query_logs', on_delete=models.SET_NULL,
         null=True, default=None,
     )
 
     operation = models.CharField(max_length=32, default=None, null=True)
-    tables = fields.ArrayField(models.CharField(max_length=200), default=list)
+    tables = models.JSONField(default=list)
 
     context_type = models.CharField(max_length=40, default=None, null=True)
     # request
     context_id = models.CharField(max_length=200, default=None, null=True)
     # log id / execution id
 
     alert = models.ForeignKey(
         AlertLog, related_name='query_logs',
         on_delete=models.SET_NULL, null=True, default=None,
     )
 
     class Meta:
         db_table = 'utilmeta_query_log'
+
+
+class AggregationLog(models.Model):
+    objects = models.Manager()
+
+    service = models.CharField(max_length=100)
+    node_id = models.CharField(max_length=100, default=None, null=True, db_index=True)
+    supervisor = models.ForeignKey(
+        Supervisor, related_name='aggregation_logs', on_delete=models.SET_NULL,
+        default=None, null=True,
+    )
+    data = models.JSONField(default=dict)
+
+    # report the aggregated analytics from log from time span
+    layer = models.PositiveSmallIntegerField(default=0)
+    # 0: hourly
+    # 1: daily
+    # 2: monthly
+
+    from_time = models.DateTimeField()
+    to_time = models.DateTimeField()
+    date = models.DateField(default=None, null=True)
+
+    created_time = models.DateTimeField(auto_now_add=True)
+    reported_time = models.DateTimeField(default=None, null=True)
+    error = models.TextField(default=None, null=True)
+    remote_id = models.CharField(max_length=40, default=None, null=True)
+    # remote id is not None means the report is successful
+
+    class Meta:
+        db_table = 'utilmeta_aggregation_log'
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/adaptor.py` & `utilmeta-2.5.2/utilmeta/utils/adaptor.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/datastructure.py` & `utilmeta-2.5.2/utilmeta/utils/datastructure.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/decorator.py` & `utilmeta-2.5.2/utilmeta/utils/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .constant import COMMON_ERRORS
 from .exceptions import BadRequest, CombinedError
 from datetime import timedelta
 from utilmeta.utils.error import Error
 import warnings
 
 __all__ = ['omit', 'error_convert', 'handle_retries', 'cached_property',
-           'awaitable', 'async_to_sync',
+           'awaitable', 'async_to_sync', 'adapt_async',
            'handle_parse', 'handle_timeout', 'ignore_errors', 'static_require']
 
 
 def ignore_errors(_f=None, *, default=None, log: bool = True,
                   log_detail: bool = True, errors=(Exception,), on_finally=None):
     if on_finally:
         assert callable(on_finally), f'@ignore_errors on_finally must be a callable, got {on_finally}'
@@ -231,14 +231,31 @@
         if f_code.co_flags & _CO_NESTED and f_code.co_name[0] == '<':
             return from_coroutine(level + 2)
         else:
             _cache[f_code] = False
             return False
 
 
+def adapt_async(func):
+    if inspect.iscoroutinefunction(func) or inspect.isasyncgenfunction(func):
+        return func
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            from utilmeta import service
+        except ImportError:
+            pass
+        else:
+            if service.asynchronous:
+                return service.pool.get_result(func, *args, **kwargs)
+        return func(*args, **kwargs)
+    return wrapper
+
+
 def awaitable(syncfunc, bind_service: bool = False):
     '''
     Decorator that allows an asynchronous function to be paired with a
     synchronous function in a single function call.  The selection of
     which function executes depends on the calling context.  For example:
         def spam(sock, maxbytes):                       (A)
             return sock.recv(maxbytes)
@@ -296,15 +313,28 @@
 try:
     from asgiref.sync import async_to_sync
 except ImportError:
     def async_to_sync(to_await):
         import asyncio
         async_response = []
 
-        async def run_and_capture_result():
-            r = await to_await
-            async_response.append(r)
-
-        loop = asyncio.get_event_loop()
-        coroutine = run_and_capture_result()
-        loop.run_until_complete(coroutine)
-        return async_response[0]
+        def wrapper(*args, **kwargs):
+            try:
+                event_loop = asyncio.get_running_loop()
+            except RuntimeError:
+                pass
+            else:
+                if event_loop.is_running():
+                    raise RuntimeError(
+                        "You cannot use AsyncToSync in the same thread as an async event loop - "
+                        "just await the async function directly."
+                    )
+
+            async def run_and_capture_result():
+                r = await to_await(*args, **kwargs)
+                async_response.append(r)
+
+            loop = asyncio.get_event_loop()
+            coroutine = run_and_capture_result()
+            loop.run_until_complete(coroutine)
+            return async_response[0]
+        return wrapper
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/error.py` & `utilmeta-2.5.2/utilmeta/utils/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import traceback
 from typing import Type, Dict, Callable, Optional, List
 from . import Attr, SEG, readable
 import sys
 import inspect
+import time
+
+
+CAUSE_DIVIDER = '\n# The above exception was the direct cause of the following exception:\n'
 
 
 class Error:
     def __init__(self, e: Exception = None):
         if isinstance(e, Exception):
             self.exc = e
             self.type = e.__class__
@@ -22,41 +26,40 @@
             self.exc_traceback = exc_traceback
 
         self.locals = {}
         self.current_traceback = ''
         self.traceback = ''
         self.variable_info = ''
         self.full_info = ''
+        self.ts = time.time()
 
-    def setup(self):
+    def setup(self, from_errors: list = ()):
         if self.current_traceback:
             return
         # FIXME: lots of performance cost in this function
         self.current_traceback = ''.join(traceback.format_tb(self.exc_traceback))
-        causes = self.get_causes()
-        if len(causes) > 1:
-            traces = []
-            local_vars = {}
-            for cause in causes:
-                if cause is self:
-                    traces.append(self.current_traceback)
-                else:
-                    cause.setup()
-                    traces.append(cause.current_traceback)
-                local_vars.update(cause.locals)
-            self.traceback = '# this error is caused by:\n'.join(traces)
-            self.locals = local_vars
-        else:
-            self.traceback = self.current_traceback
+        self.traceback = self.current_traceback
+        if not from_errors:
             try:
                 self.locals = inspect.trace()[-1][0].f_locals
                 # self.locals: Dict[str, Any] = Util.clean_kwargs(inspect.trace()[-1][0].f_locals, display=True)
             except IndexError:
                 self.locals = {}
 
+        cause = self.exc.__cause__
+        from_errors = [self.exc] + list(from_errors)
+
+        if cause and cause not in from_errors:
+            cause_error = self.__class__(cause)
+            cause_error.setup(from_errors=from_errors)
+            self.traceback = cause_error.full_info + CAUSE_DIVIDER + self.traceback
+            # self.locals.update({
+            #     f'{cause.__class__.__name__}.{key}': val for key, val in cause_error.locals.items()
+            # })
+
         variables = []
         if self.locals:
             variables.append('Exception Local Variables:')
         for key, val in self.locals.items():
             if key.startswith(SEG) and key.endswith(SEG):
                 continue
             try:
@@ -78,24 +81,35 @@
     def message(self) -> str:
         return '{0}{1}: {2}'.format(
             self.traceback,
             self.type.__name__,
             self.exc
         )
 
-    @property
-    def root_cause(self) -> 'Error':
-        return self.get_causes()[0]
+    # @property
+    # def root_cause(self) -> Exception:
+    #     return self.get_causes()[0]
 
-    def get_causes(self) -> List['Error']:
-        # causes = getattr(self.exc, Attr.CAUSES, [])
-        # cause_reasons = [str(c.current_traceback) for c in causes]
-        # if self.current_traceback in cause_reasons:
-        #     return causes
-        return [self, *getattr(self.exc, Attr.CAUSES, [])]
+    # def get_causes(self) -> List[Exception]:
+    #     # causes = getattr(self.exc, Attr.CAUSES, [])
+    #     # cause_reasons = [str(c.current_traceback) for c in causes]
+    #     # if self.current_traceback in cause_reasons:
+    #     #     return causes
+    #     causes = []
+    #     cause = self.exc
+    #     while cause:
+    #         causes.append(cause)
+    #         cause = cause.__cause__
+    #         if cause in causes:
+    #             break
+    #
+    #     causes.reverse()
+    #     print('CAUSES:', causes)
+    #     # return [self, *getattr(self.exc, Attr.CAUSES, [])]
+    #     return causes
 
     # @property
     # def target(self) -> 'Error':
     #     errors = []
     #     target = None
     #     for e in [*self.causes, self]:
     #         if str(e) in errors:
@@ -140,15 +154,16 @@
 
     def throw(self, type=None, prepend: str = '', **kwargs):
         if not (inspect.isclass(type) and issubclass(type, Exception)):
             type = None
         type = type or self.type
         if prepend or not isinstance(self.exc, type):
             e = type(f'{prepend}{self.exc}', **kwargs)  # noqa
-            setattr(e, Attr.CAUSES, self.get_causes())
+            e.__cause__ = self.exc
+            # setattr(e, Attr.CAUSES, self.get_causes())
         else:
             e = self.exc
         # it need the throw caller to raise the error like: raise Error().throw()
         # cause in that way can track the original variables
         return e
 
     def get_hook(self, hooks: Dict[Type[Exception], Callable], exact: bool = False) -> Optional[Callable]:
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/logical.py` & `utilmeta-2.5.2/utilmeta/utils/logical.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/plugin.py` & `utilmeta-2.5.2/utilmeta/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/constant/data.py` & `utilmeta-2.5.2/utilmeta/utils/constant/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     PROXY = '__proxy__'
     RELATED = '__related__'
     STATUS = '__status__'
     ORIGIN = '__origin__'
     TARGET = '__target__'
     CATEGORY = '__category__'
     CAUSES = '__causes__'
+    CAUSE = '__cause__'
     CLS = '__class__'
     PARSER = '__parser__'
     BUILTINS = '__builtins__'
     ANNOTATES = '__annotations__'
     ISOLATE = '__isolate__'
     CONFIG = '__config__'
     OPTIONS = '__options__'
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/constant/i18n.py` & `utilmeta-2.5.2/utilmeta/utils/constant/i18n.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/constant/vendor.py` & `utilmeta-2.5.2/utilmeta/utils/constant/vendor.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/constant/web.py` & `utilmeta-2.5.2/utilmeta/utils/constant/web.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ..datastructure import Static
+import re
 
 SCHEME = '://'
 LOCAL = 'localhost'
 LOCAL_IP = '127.0.0.1'
 ALL_IP = '0.0.0.0'
+PATH_REGEX = re.compile("{([a-zA-Z][a-zA-Z0-9_]*)}")
 
 
 class HTTPMethod(Static):
     GET = 'GET'
     PUT = 'PUT'
     POST = 'POST'
     PATCH = 'PATCH'
@@ -163,14 +165,38 @@
     OPTIONS_HEADERS = 'Access-Control-Request-Headers'
 
     @classmethod
     def attr_name(cls, key: str):
         return key.replace('-', '_').lower()
 
 
+class TCPStatus(Static):
+    ESTABLISHED = "ESTABLISHED"
+    SYN_SENT = "SYN_SENT"
+    SYN_RECV = "SYN_RECV"
+    FIN_WAIT1 = "FIN_WAIT1"
+    FIN_WAIT2 = "FIN_WAIT2"
+    TIME_WAIT = "TIME_WAIT"
+    CLOSE = "CLOSE"
+    CLOSE_WAIT = "CLOSE_WAIT"
+    LAST_ACK = "LAST_ACK"
+    LISTEN = "LISTEN"
+    CLOSING = "CLOSING"
+    NONE = "NONE"
+
+
+IDLE_TCP_STATUSES = [
+    TCPStatus.CLOSE,
+    TCPStatus.CLOSING,
+    TCPStatus.CLOSE_WAIT,
+    TCPStatus.TIME_WAIT,
+    TCPStatus.FIN_WAIT1,
+    TCPStatus.FIN_WAIT2,
+    TCPStatus.LAST_ACK
+]
 HTTP = Scheme.HTTP + SCHEME
 HTTPS = Scheme.HTTPS + SCHEME
 REQUEST_TYPES = RequestType.gen()
 CONTENT_TYPE = Header.attr_name(Header.TYPE)
 DICT_TYPES = (RequestType.JSON, RequestType.XML, RequestType.FORM_URLENCODED, RequestType.FORM_DATA)
 GENERAL_TYPES = GeneralType.gen()
 STREAM_TYPES = (GeneralType.IMAGE, GeneralType.AUDIO, GeneralType.VIDEO, GeneralType.OCTET_STREAM)
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/exceptions/config.py` & `utilmeta-2.5.2/utilmeta/utils/exceptions/config.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/exceptions/http.py` & `utilmeta-2.5.2/utilmeta/utils/exceptions/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
             value += ' ' + ','.join([f'{k}={v}' for k, v in auth_params.items()])
         self.append_headers = {Header.WWW_AUTH: value}
 
 
 class PermissionDenied(RequestError):
     status = 403
 
-    def __init__(self, msg: str = None, *, scopes=None, required_scopes=None, name: str = None, **kwargs):
+    def __init__(self, msg: str = None, *, scope=None, required_scope=None, name: str = None, **kwargs):
         super().__init__(msg, **kwargs)
-        self.scopes = scopes
-        self.required_scopes = required_scopes
+        self.scope = scope
+        self.required_scope = required_scope
         self.name = name
 
 
 class NotFound(RequestError):
     status = 404
 
     def __init__(self, message: str = None, *, path: str = None, query: dict = None, **kwargs):
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/exceptions/runtime.py` & `utilmeta-2.5.2/utilmeta/utils/exceptions/runtime.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/functional/data.py` & `utilmeta-2.5.2/utilmeta/utils/functional/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import typing
 import string
 import json
 import re
 import hashlib
 import decimal
 from collections import OrderedDict
+from collections.abc import Mapping
 from typing import List, Dict, Callable, Union, Any
 
 
 __all__ = [
     'repeat', 'multi', 'duplicate',
     'pop',
     'distinct',
@@ -150,16 +151,16 @@
 
 
 def multi(f):
     return isinstance(f, (list, set, frozenset, tuple, type({}.values()), type({}.keys())))
 
 
 def pop(data, key, default=None):
-    if isinstance(data, dict):
-        return data.pop(key) if key in data else default
+    if isinstance(data, (dict, Mapping)):
+        return data.pop(key) if key in data and hasattr(data, 'pop') else default
     elif isinstance(data, list):
         return data.pop(key) if key < len(data) else default
     return default
 
 
 def make_dict_by(values: List[dict], key: str, formatter: Callable = lambda x: x) -> Dict[Any, List[dict]]:
     """
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/functional/py.py` & `utilmeta-2.5.2/utilmeta/utils/functional/py.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/functional/sys.py` & `utilmeta-2.5.2/utilmeta/utils/functional/sys.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,24 @@
     'get_max_socket_conn',
     'get_max_open_files',
     'ip_belong_networks',
     'get_system_open_files',
     'create_only_write',
     'get_recursive_dirs',
     'get_sys_net_connections_info',
+    'get_mac_address',
 ]
 
+import uuid
+
+
+def get_mac_address():
+    h = iter(hex(uuid.getnode())[2:].zfill(12))
+    return ":".join(i + next(h) for i in h)
+
 
 def remove_file(file: str, ignore_not_found: bool = True):
     try:
         os.remove(file)
         return True
     except FileNotFoundError as e:
         if ignore_not_found:
@@ -110,22 +118,30 @@
                 fds += proc.num_fds()
             except psutil.Error:
                 continue
     return fds
 
 
 def get_system_open_files():
-    import psutil
-    files = 0
-    for proc in psutil.process_iter():
-        try:
-            files += len(proc.open_files())
-        except psutil.Error:
-            continue
-    return files
+    try:
+        with open('/proc/sys/fs/file-nr') as file_nr:
+            stats = file_nr.read().split()
+            total_fds = int(stats[0]) - int(stats[1])
+            return total_fds
+    except Exception:
+        return None
+        # import psutil
+        # files = 0
+        # for proc in psutil.process_iter(['open_files']):
+        #     try:
+        #         proc.open_files()
+        #         files += len(proc.info['open_files'])
+        #     except psutil.Error:
+        #         continue
+        # return files
 
 
 def get_network_ip(ifname: str):
     import struct
     try:
         import fcntl
     except ModuleNotFoundError:
@@ -627,21 +643,23 @@
     if match:
         return match.group()
     from urllib.parse import urlparse, ParseResult
     res: ParseResult = urlparse(host)
     match = ip_reg.match(res.netloc)
     if match:
         return match.group()
+    if res.hostname == constant.LOCAL:
+        return constant.LOCAL_IP
     if ip_only:
         return None
     from .web import get_hostname
     try:
         return socket.gethostbyname(get_hostname(host))
     except (socket.error, OSError):
-        return constant.LOCAL_IP
+        return None
 
 
 def get_real_ip(ip: str):
     from .web import localhost
     if localhost(ip):
         return get_server_ip()
     return get_ip(ip)
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/functional/time.py` & `utilmeta-2.5.2/utilmeta/utils/functional/time.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/functional/web.py` & `utilmeta-2.5.2/utilmeta/utils/functional/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,28 +79,30 @@
             return "Infinity"
         if data == float('-inf'):
             return '-Infinity'
     return data
 
 
 def fast_digest(value, compress: Union[bool, int] = False, case_insensitive: bool = False,
-                consistent: bool = True, mod: int = 2 ** 32):
+                consistent: bool = True, mod: int = 2 ** 64):
     if consistent:
         encoded = value if isinstance(value, bytes) else str(value).encode()
         dig_mod = int(hashlib.md5(encoded).hexdigest(), 16) % mod
         # if consistent required, we cannot use hash()
         # because every python restart will bring inconsistency to the same value hash
     else:
         dig_mod = hash(str(value)) % mod
 
     if compress:
-        if isinstance(compress, int):
+        if isinstance(compress, bool):
+            base = 36 if case_insensitive else 62
+        elif isinstance(compress, int):
             base = compress
         else:
-            base = 36 if case_insensitive else 62
+            raise TypeError(f'Invalid compress: {compress}')
         return based_number(dig_mod, base)
     return str(dig_mod)
 
 
 def etag(data, weak: bool = False) -> str:
     if isinstance(data, str):
         if re.fullmatch(r'\A((?:W/)?"[^"]*")\Z', data):
@@ -182,15 +184,16 @@
     boundary = boundary or binascii.hexlify(os.urandom(16))
     if isinstance(boundary, str):
         boundary = boundary.encode('ascii')
     items = []
     for field, value in form.items():
         key = str(field).encode()
         beg = b"--%s\r\nContent-Disposition: form-data; name=\"%s\"" % (boundary, key)
-        for val in (value if multi(value) else [value]):
+        files = value if multi(value) else [value]
+        for val in files:
             if file_like(val):
                 content = val.read()
                 filename = str(getattr(val, 'name', 'file')).encode()
                 content_type = str(getattr(val, 'content_type', RequestType.OCTET_STREAM)).encode()
                 prep = b'; filename=\"%s\"\r\nContent-Type: %s' % (filename, content_type)
             else:
                 if isinstance(val, bytes):
@@ -329,15 +332,15 @@
         # force convert to str
         base = ''
     route_list = []
     if not any(routes):
         if append_slash:
             if not base.endswith('/'):
                 base = base + '/'
-        else:
+        elif append_slash is False:
             base = base.rstrip('/')
         return base
     if not isinstance(base, str):
         base = str(base) if base else ''
     final_route = base
     for route in routes:
         if not route:
@@ -389,14 +392,17 @@
     from django.http.request import QueryDict
     return res.path, parse_query_dict(QueryDict(res.query))
 
 
 def parse_query_dict(qd: Dict[str, List[str]]) -> dict:
     data = {}
     for key, val in dict(qd).items():
+        if not multi(val):
+            data[key] = str(val or '')
+            continue
         if key.endswith('[]'):
             data[key.rstrip('[]')] = val
             continue
         if len(val) > 1:
             data[key] = val
             continue
         v = val[0]
```

### Comparing `utilmeta-2.4.1/utilmeta/utils/schema/backends/attrs.py` & `utilmeta-2.5.2/utilmeta/utils/schema/backends/attrs.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/utilmeta/utils/schema/backends/dataclass.py` & `utilmeta-2.5.2/utilmeta/utils/schema/backends/dataclass.py`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/LICENSE` & `utilmeta-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utilmeta-2.4.1/README.md` & `utilmeta-2.5.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,209 +1,269 @@
-# UtilMeta API Framework - Python
-<img src="https://utilmeta.com/img/py-intro.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
-
-
-**UtilMeta** is a progressive meta-framework for backend applications, which efficiently builds declarative APIs based on the Python type annotation standard, and supports the integration of mainstream Python frameworks as runtime backend
-
-* Homepage: [https://utilmeta.com/py](https://utilmeta.com/py)
-* Documentation: [https://docs.utilmeta.com/py/en/](https://docs.utilmeta.com/py/en/)
-* Author: <a href="https://github.com/voidZXL" target="_blank">@voidZXL</a>
-
-
-<a href="https://pypi.org/project/utilmeta/" target="_blank">
-	<img src="https://img.shields.io/pypi/v/utilmeta" alt="">
-</a>
-<a href="https://pypi.org/project/utilmeta/" target="_blank">
-	<img src="https://img.shields.io/pypi/pyversions/utilmeta" alt="">
-</a>
-<a href="https://github.com/utilmeta/utilmeta-py/blob/main/LICENSE" target="_blank">
-	<img src="https://img.shields.io/badge/license-Apache%202.0-blue" alt="">
-</a>
-<a href="https://github.com/utilmeta/utilmeta-py/actions?query=branch%3Amain+" target="_blank">
-	<img src="https://img.shields.io/github/actions/workflow/status/utilmeta/utilmeta-py/test.yaml?branch=main&label=CI" alt="">
-</a>
-
-## Installation
-```
-pip install utilmeta
-```
-
-## Core Features
-
-### Declarative Development
-Using the declarative power from UtilMeta, you can easily write APIs with auto request validation, efficient ORM queries, and auto OpenAPI document generation
-<img src="https://utilmeta.com/img/py.section1.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
-### Progressive Meta Framework
-UtilMeta developed a standard that support all major Python web framework like **django**, **flask**, **fastapi** (starlette), **sanic**, **tornado** as runtime backend, and support current projects using these frameworks to develop new API using UtilMeta progressively
-<img src="https://utilmeta.com/img/py.section2.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
-### Highly Flexible & Extensible
-UtilMeta is highly flexible with a series of plugins includes authentication (Session/JWT), CORS, rate limit, retry, and can be extended to support more features.
-
-### Full-lifecycle DevOps Solution
-The [UtilMeta Platform](https://utilmeta.com/) provided the full-lifecycle DevOps solution for this framework, the API Docs, Debug, Logs, Monitoring, Alerts, Analytics will all been taken care of in the platform
-<img src="https://utilmeta.com/img/py.section3.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
-## Hello World
- Create a Python file named `server.py` and write the following code 
-```python
-from utilmeta import UtilMeta
-from utilmeta.core import api
-import django
-
-class RootAPI(api.API):
-    @api.get
-    def hello(self):
-        return 'world'
-
-service = UtilMeta(
-    __name__,
-    name='demo',
-    backend=django,    # or flask / starlette / tornado / sanic
-    api=RootAPI,
-    route='/api'
-)
-
-app = service.application()  # wsgi app
-
-if __name__ == '__main__':
-    service.run()
-```
-
-> You can use `flask`, `starlette`, `sanic`, `tornado` instead of `django` as runtime backend, just install them first and replace them in the demo code
-
-### Run
-You can execute this file by python to run the server
-```shell
-python server.py
-```
-The following info Implies that the service has live
-```
-Running on http://127.0.0.1:8000
-Press CTRL+C to quit
-```
-Then we can use our browser to open [http://127.0.0.1:8000/api/hello](http://127.0.0.1:8000/api/hello) to call this API directly, we will see
-```
-world
-```
-It means this API works
-## Examples
-
-### Declarative RESTful API
-
-Declarative ORM in UtilMeta can handle relational queries concisely without N+1 problem, both sync and async queries are supported
-```python
-from utilmeta.core import api, orm
-from django.db import models
-
-class User(models.Model):
-    username = models.CharField(max_length=20, unique=True)
-
-class Article(models.Model):
-    author = models.ForeignKey(User, related_name="articles", on_delete=models.CASCADE)
-    content = models.TextField()
-
-class UserSchema(orm.Schema[User]):
-    username: str
-    articles_num: int = models.Count('articles')
-
-class ArticleSchema(orm.Schema[Article]):
-    id: int
-    author: UserSchema
-    content: str
-
-class ArticleAPI(api.API):
-    async def get(self, id: int) -> ArticleSchema:
-        return await ArticleSchema.ainit(id)
-```
-
-if you request the ArticleAPI like `GET /article?id=1`, you will get the result like
-
-```python
-{
-  "id": 1,
-  "author": {
-    "username": "alice",
-    "articles_num": 3
-  },
-  "content": "hello world"
-}
-```
-This is conform to what you declared, and the OpenAPI docs will be generated automatically
-### Migrate
-
-Integrate current django/flask/fastapi/... project with UtilMeta API is as easy as follows 
-```python
-import django
-from django.urls import re_path
-from django.http.response import HttpResponse
-from utilmeta.core import api, response
-
-class CalcAPI(api.API):
-    @api.get
-    def add(self, a: int, b: int) -> int:
-        return a + b
-
-def django_test(request, route: str):
-    return HttpResponse(route)
-
-urlpatterns = [
-    re_path('test/(.*)', django_test),
-    CalcAPI.__as__(django, route='/calc'),
-]
-```
-
-Integrate with Flask example
-```python
-from flask import Flask
-from utilmeta.core import api, response
-
-app = Flask(__name__)
-
-@app.route("/")
-def hello_world():
-    return "<p>Hello, World!</p>"
-
-class CalcAPI(api.API):
-    @api.get
-    def add(self, a: int, b: int) -> int:
-        return a + b
-
-CalcAPI.__as__(app, route='/calc')
-```
-
-## Quick Guide
-We have several introductory case tutorials from easy to complex, covering most usage of the framework. You can read and learn in the following order.
-
-1. [BMI Calculation API](https://docs.utilmeta.com/py/en/tutorials/bmi-calc)
-2. [User Login & RESTful API](https://docs.utilmeta.com/py/en/tutorials/user-auth)
-3. [Realworld Blog Project](https://docs.utilmeta.com/py/en/tutorials/realworld-blog)
-4. Websocket Chatroom (coming soon)
-
-If you prefer to learn from a specific feature, you can refer to
-
-* [Handle Request](https://docs.utilmeta.com/py/en/guide/handle-request): How to handle path, query parameters, request body, file upload, request headers and cookies.
-* [API Class and Routing](https://docs.utilmeta.com/py/en/guide/api-route) How to use API class mounts to define tree-like API routing, and use  hooks to easily reuse code between APIs, handle errors, and template responses.
-* [Schema query and ORM](https://docs.utilmeta.com/py/en/guide/schema-query) How to use Schema to declaratively write the CRUD query, and ORM operations required by a RESTful interface.
-* [API Authentication](https://docs.utilmeta.com/py/en/guide/auth): How to use Session, JWT, OAuth and other methods to authenticate the request of the interface, get the current request's user and simplify the login operation
-* [Config, Run & Deploy](https://docs.utilmeta.com/py/en/guide/config-run): How to configure the run settings, startup, and deployment of a service using features such as declarative environment variables
-* [Migrate from current project](https://docs.utilmeta.com/py/en/guide/migration) How to progressively integrate UtilMeta API to an existing backend project or migrate to UtilMeta
-
-## Community
-Join our community to build great things together
-
-* [Discord](https://discord.gg/JdmEkFS6dS)
-* [X(Twitter)](https://twitter.com/@utilmeta)
-* [Reddit](https://www.reddit.com/r/utilmeta)
-* [中文讨论区](https://lnzhou.com/channels/utilmeta/community)
-
-## Enterprise Solutions & Support
-The UtilMeta team is providing custom solutions and enterprise-level support at
-
-* [https://utilmeta.com/solutions](https://utilmeta.com/solutions)
-
-You can also contact us in [this page](https://utilmeta.com/about#contact)
-
-### Wechat
-
-Contact the creator's wechat for support or join the developers wechat group
-
-
+Metadata-Version: 2.1
+Name: UtilMeta
+Version: 2.5.2
+Summary: UtilMeta - progressive meta framework for API development in Python
+Project-URL: Homepage, https://utilmeta.com/py
+Project-URL: Documentation, https://docs.utilmeta.com/py/en
+Project-URL: Repository, https://github.com/utilmeta/utilmeta-py
+Author-email: "Xulin Zhou (voidZXL)" <zxl@utilmeta.com>
+License: Copyright (c) 2019-present Xulin Zhou (周煦林)
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+License-File: LICENSE
+Keywords: API,RESTful,backend,declarative,meta,orm,progressive,utype,web
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: databases>=0.7.0
+Requires-Dist: django>=4.1.0
+Requires-Dist: jwcrypto>=1.5.4
+Requires-Dist: psutil>=5.8.0
+Requires-Dist: utype>=0.4.0
+Provides-Extra: all
+Requires-Dist: flask>=2.3.0; extra == 'all'
+Requires-Dist: sanic>=22.0.0; extra == 'all'
+Requires-Dist: starlette>=0.27.0; extra == 'all'
+Requires-Dist: tornado>=6.2; extra == 'all'
+Description-Content-Type: text/markdown
+
+# UtilMeta API Framework - Python
+<img src="https://utilmeta.com/img/py-intro.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
+
+
+**UtilMeta** is a progressive meta-framework for backend applications, which efficiently builds declarative APIs based on the Python type annotation standard, and supports the integration of mainstream Python frameworks as runtime backend
+
+* Homepage: [https://utilmeta.com/py](https://utilmeta.com/py)
+* Documentation: [https://docs.utilmeta.com/py/en/](https://docs.utilmeta.com/py/en/)
+* Author: <a href="https://github.com/voidZXL" target="_blank">@voidZXL</a>
+
+
+<a href="https://pypi.org/project/utilmeta/" target="_blank">
+	<img src="https://img.shields.io/pypi/v/utilmeta" alt="">
+</a>
+<a href="https://pypi.org/project/utilmeta/" target="_blank">
+	<img src="https://img.shields.io/pypi/pyversions/utilmeta" alt="">
+</a>
+<a href="https://github.com/utilmeta/utilmeta-py/blob/main/LICENSE" target="_blank">
+	<img src="https://img.shields.io/badge/license-Apache%202.0-blue" alt="">
+</a>
+<a href="https://github.com/utilmeta/utilmeta-py/actions?query=branch%3Amain+" target="_blank">
+	<img src="https://img.shields.io/github/actions/workflow/status/utilmeta/utilmeta-py/test.yaml?branch=main&label=CI" alt="">
+</a>
+
+## Installation
+```
+pip install utilmeta
+```
+
+## Core Features
+
+### Declarative Development
+Using the declarative power from UtilMeta, you can easily write APIs with auto request validation, efficient ORM queries, and auto OpenAPI document generation
+<img src="https://utilmeta.com/img/py.section1.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
+### Progressive Meta Framework
+UtilMeta developed a standard that support all major Python web framework like **django**, **flask**, **fastapi** (starlette), **sanic**, **tornado** as runtime backend, and support current projects using these frameworks to develop new API using UtilMeta progressively
+<img src="https://utilmeta.com/img/py.section2.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
+### Highly Flexible & Extensible
+UtilMeta is highly flexible with a series of plugins including authentication (Session/JWT), CORS, rate limit, retry, and can be extended to support more features.
+
+### Full-lifecycle DevOps Solution
+The [UtilMeta Platform](https://utilmeta.com/) provided the full-lifecycle DevOps solution for this framework, the API Docs, Debug, Logs, Monitoring, Alerts, Analytics will all been taken care of in the platform
+<img src="https://utilmeta.com/img/py.section3.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="720"/>
+## Hello World
+ Create a Python file named `server.py` and write the following code 
+```python
+from utilmeta import UtilMeta
+from utilmeta.core import api
+import django
+
+class RootAPI(api.API):
+    @api.get
+    def hello(self):
+        return 'world'
+
+service = UtilMeta(
+    __name__,
+    name='demo',
+    backend=django,    # or flask / starlette / tornado / sanic
+    api=RootAPI,
+    route='/api'
+)
+
+app = service.application()  # wsgi app
+
+if __name__ == '__main__':
+    service.run()
+```
+
+> You can use `flask`, `starlette`, `sanic`, `tornado` instead of `django` as runtime backend, just install them first and replace them in the demo code
+
+### Run
+You can execute this file by python to run the server
+```shell
+python server.py
+```
+The following info Implies that the service has live
+```
+Running on http://127.0.0.1:8000
+Press CTRL+C to quit
+```
+Then we can use our browser to open [http://127.0.0.1:8000/api/hello](http://127.0.0.1:8000/api/hello) to call this API directly, we will see
+```
+world
+```
+It means this API works
+## Examples
+
+### Declarative RESTful API
+
+Declarative ORM in UtilMeta can handle relational queries concisely without N+1 problem, both sync and async queries are supported
+```python
+from utilmeta.core import api, orm
+from django.db import models
+
+class User(models.Model):
+    username = models.CharField(max_length=20, unique=True)
+
+class Article(models.Model):
+    author = models.ForeignKey(User, related_name="articles", on_delete=models.CASCADE)
+    content = models.TextField()
+
+class UserSchema(orm.Schema[User]):
+    username: str
+    articles_num: int = models.Count('articles')
+
+class ArticleSchema(orm.Schema[Article]):
+    id: int
+    author: UserSchema
+    content: str
+
+class ArticleAPI(api.API):
+    async def get(self, id: int) -> ArticleSchema:
+        return await ArticleSchema.ainit(id)
+```
+
+if you request the ArticleAPI like `GET /article?id=1`, you will get the result like
+
+```python
+{
+  "id": 1,
+  "author": {
+    "username": "alice",
+    "articles_num": 3
+  },
+  "content": "hello world"
+}
+```
+This conforms to what you declared, and the OpenAPI docs will be generated automatically
+### Migrate
+
+Integrate current django/flask/fastapi/... project with UtilMeta API is as easy as follows 
+```python
+import django
+from django.urls import re_path
+from django.http.response import HttpResponse
+from utilmeta.core import api, response
+
+class CalcAPI(api.API):
+    @api.get
+    def add(self, a: int, b: int) -> int:
+        return a + b
+
+def django_test(request, route: str):
+    return HttpResponse(route)
+
+urlpatterns = [
+    re_path('test/(.*)', django_test),
+    CalcAPI.__as__(django, route='/calc'),
+]
+```
+
+Integrate with Flask example
+```python
+from flask import Flask
+from utilmeta.core import api, response
+
+app = Flask(__name__)
+
+@app.route("/")
+def hello_world():
+    return "<p>Hello, World!</p>"
+
+class CalcAPI(api.API):
+    @api.get
+    def add(self, a: int, b: int) -> int:
+        return a + b
+
+CalcAPI.__as__(app, route='/calc')
+```
+
+## Quick Guide
+We have several introductory case tutorials from easy to complex, covering most usage of the framework. You can read and learn in the following order.
+
+1. [BMI Calculation API](https://docs.utilmeta.com/py/en/tutorials/bmi-calc)
+2. [User Login & RESTful API](https://docs.utilmeta.com/py/en/tutorials/user-auth)
+3. [Realworld Blog Project](https://docs.utilmeta.com/py/en/tutorials/realworld-blog)
+4. Websocket Chatroom (coming soon)
+
+If you prefer to learn from a specific feature, you can refer to
+
+* [Handle Request](https://docs.utilmeta.com/py/en/guide/handle-request): How to handle path, query parameters, request body, file upload, request headers and cookies.
+* [API Class and Routing](https://docs.utilmeta.com/py/en/guide/api-route) How to use API class mounts to define tree-like API routing, and use  hooks to easily reuse code between APIs, handle errors, and template responses.
+* [Schema query and ORM](https://docs.utilmeta.com/py/en/guide/schema-query) How to use Schema to declaratively write the CRUD query, and ORM operations required by a RESTful interface.
+* [API Authentication](https://docs.utilmeta.com/py/en/guide/auth): How to use Session, JWT, OAuth and other methods to authenticate the request of the interface, get the current request's user and simplify the login operation
+* [Config, Run & Deploy](https://docs.utilmeta.com/py/en/guide/config-run): How to configure the run settings, startup, and deployment of a service using features such as declarative environment variables
+* [Migrate from current project](https://docs.utilmeta.com/py/en/guide/migration) How to progressively integrate UtilMeta API to an existing backend project or migrate to UtilMeta
+
+## Community
+Join our community to build great things together
+
+* [Discord](https://discord.gg/JdmEkFS6dS)
+* [X(Twitter)](https://twitter.com/@utilmeta)
+* [Reddit](https://www.reddit.com/r/utilmeta)
+* [中文讨论区](https://lnzhou.com/channels/utilmeta/community)
+
+## Enterprise Solutions & Support
+The UtilMeta team is providing custom solutions and enterprise-level support at
+
+* [https://utilmeta.com/solutions](https://utilmeta.com/solutions)
+
+You can also contact us in [this page](https://utilmeta.com/about#contact)
+
+### Wechat
+
+Contact the creator's wechat for support or join the developers wechat group
+
+
 <img src="https://utilmeta.com/img/wx_zxl.png" href="https://utilmeta.com/py" target="_blank"  alt="drawing" width="240"/>
```

### Comparing `utilmeta-2.4.1/pyproject.toml` & `utilmeta-2.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,20 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "utype>=0.4.0",
+    "django>=4.1.0",
     "databases>=0.7.0",
-    "django>=4.1.0"
+    "jwcrypto>=1.5.4",
+    "psutil>=5.8.0"
 ]
+
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://utilmeta.com/py"
 Documentation = "https://docs.utilmeta.com/py/en"
 Repository = "https://github.com/utilmeta/utilmeta-py"
```

